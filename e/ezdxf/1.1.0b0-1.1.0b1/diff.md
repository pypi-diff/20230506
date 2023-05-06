# Comparing `tmp/ezdxf-1.1.0b0.zip` & `tmp/ezdxf-1.1.0b1.zip`

## zipinfo {}

```diff
@@ -1,821 +1,831 @@
-Zip file size: 2055057 bytes, number of entries: 819
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/
--rw-rw-rw-  2.0 fat     1092 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/LICENSE
--rw-rw-rw-  2.0 fat      302 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/MANIFEST.in
--rw-rw-rw-  2.0 fat   101099 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/NEWS.md
--rw-rw-rw-  2.0 fat    68966 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/PKG-INFO
--rw-rw-rw-  2.0 fat     6142 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/README.md
--rw-rw-rw-  2.0 fat       55 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/requirements.txt
--rw-rw-rw-  2.0 fat       74 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/setup.cfg
--rw-rw-rw-  2.0 fat     5402 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/setup.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/
--rw-rw-rw-  2.0 fat      567 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/check_disable_c_ext_by_config_file.py
--rw-rw-rw-  2.0 fat      541 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/check_disable_c_ext_by_env_var.py
--rw-rw-rw-  2.0 fat      402 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/conftest.py
--rw-rw-rw-  2.0 fat     1054 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_acad_table.py
--rw-rw-rw-  2.0 fat     4686 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_all_dimline_styles.py
--rw-rw-rw-  2.0 fat     4133 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_all_ellipse_transformations.py
--rw-rw-rw-  2.0 fat     1064 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_anonymous_blocks.py
--rw-rw-rw-  2.0 fat      871 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_audit_critical_dxf_files.py
--rw-rw-rw-  2.0 fat     1603 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_audit_layouts.py
--rw-rw-rw-  2.0 fat     1726 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_complex_line_type_2.py
--rw-rw-rw-  2.0 fat     1003 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_create_basic_graphics.py
--rw-rw-rw-  2.0 fat     1921 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_document_guid.py
--rw-rw-rw-  2.0 fat     1832 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_document_page_setup.py
--rw-rw-rw-  2.0 fat      998 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_dxf_info_scanning.py
--rw-rw-rw-  2.0 fat     1558 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_entities_iterator.py
--rw-rw-rw-  2.0 fat      934 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_fix_dulicate_handles.py
--rw-rw-rw-  2.0 fat     1901 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_geo.py
--rw-rw-rw-  2.0 fat     1250 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_groups.py
--rw-rw-rw-  2.0 fat      630 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_ignore_junk_beyond_EOF.py
--rw-rw-rw-  2.0 fat     1155 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_launcher.py
--rw-rw-rw-  2.0 fat      631 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_leica_disto_r12.py
--rw-rw-rw-  2.0 fat      737 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_load_dxf_unicode_notation.py
--rw-rw-rw-  2.0 fat     2931 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_mapbox_earcut.py
--rw-rw-rw-  2.0 fat     2230 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_mtext_columns.py
--rw-rw-rw-  2.0 fat     2392 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_mtext_explode_addon.py
--rw-rw-rw-  2.0 fat     1846 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_mtext_text_frame.py
--rw-rw-rw-  2.0 fat     1053 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_new_table_entries.py
--rw-rw-rw-  2.0 fat      887 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_none_ascii_read_write.py
--rw-rw-rw-  2.0 fat     3435 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_odafc.py
--rw-rw-rw-  2.0 fat     1737 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_open_binary_DXF_files.py
--rw-rw-rw-  2.0 fat      751 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_open_coord_order_issue.py
--rw-rw-rw-  2.0 fat     3842 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_open_exotic_dxf_files.py
--rw-rw-rw-  2.0 fat      879 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_open_R13_R14.py
--rw-rw-rw-  2.0 fat     3152 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_polyline_entity.py
--rw-rw-rw-  2.0 fat     1749 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_preserve_binary_data_in_xrecords.py
--rw-rw-rw-  2.0 fat     6944 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_r12export.py
--rw-rw-rw-  2.0 fat     6256 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_r12strict.py
--rw-rw-rw-  2.0 fat     3410 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_r12writer.py
--rw-rw-rw-  2.0 fat      567 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_read_file_without_handles.py
--rw-rw-rw-  2.0 fat     1121 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_read_write_modern_entites.py
--rw-rw-rw-  2.0 fat     5375 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_recover.py
--rw-rw-rw-  2.0 fat     1959 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_redraw_order.py
--rw-rw-rw-  2.0 fat     1819 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_rotated_block_attributes.py
--rw-rw-rw-  2.0 fat      774 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_surface_entities.py
--rw-rw-rw-  2.0 fat      928 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_write_fixed_meta_data.py
--rw-rw-rw-  2.0 fat     1806 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_write_without_handles.py
--rw-rw-rw-  2.0 fat     3638 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_xref_detach.py
--rw-rw-rw-  2.0 fat     3060 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/AC1003_LINE_Example.dxf
--rw-rw-rw-  2.0 fat   179505 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/acad_table_with_blk_ref.dxf
--rw-rw-rw-  2.0 fat     7956 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/ASCII_R12.dxf
--rw-rw-rw-  2.0 fat     3761 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/bin_dxf_r12.dxf
--rw-rw-rw-  2.0 fat    20914 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/bin_dxf_r13.dxf
--rw-rw-rw-  2.0 fat    21137 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/bin_dxf_r14.dxf
--rw-rw-rw-  2.0 fat    11564 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/bin_dxf_r2000.dxf
--rw-rw-rw-  2.0 fat     6424 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/cc_dxflib.dxf
--rw-rw-rw-  2.0 fat   173753 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/custom_blocks.dxf
--rw-rw-rw-  2.0 fat    32203 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/duplicate_handles.dxf
--rw-rw-rw-  2.0 fat    18554 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/dxf_unicode.dxf
--rw-rw-rw-  2.0 fat     1592 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/empty_handles.dxf
--rw-rw-rw-  2.0 fat    97103 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/groups.dxf
--rw-rw-rw-  2.0 fat     9146 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/Leica_Disto_S910.dxf
--rw-rw-rw-  2.0 fat    17986 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/MODEL.dxf
--rw-rw-rw-  2.0 fat    25799 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/mtext_columns_R2007.dxf
--rw-rw-rw-  2.0 fat    23927 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/mtext_columns_R2018.dxf
--rw-rw-rw-  2.0 fat    98230 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/mtext_framed_columns.dxf
--rw-rw-rw-  2.0 fat   106574 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/mtext_text_frame.dxf
--rw-rw-rw-  2.0 fat    12001 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/no_layouts.dxf
--rw-rw-rw-  2.0 fat    28788 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/POLI-ALL210_12.DXF
--rw-rw-rw-  2.0 fat      144 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/R12_with_trash_beyond_EOF.dxf
--rw-rw-rw-  2.0 fat   212407 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/recover01.dxf
--rw-rw-rw-  2.0 fat   115423 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/recover02.dxf
--rw-rw-rw-  2.0 fat    21178 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/small_r13.dxf
--rw-rw-rw-  2.0 fat    10326 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/small_r14.dxf
--rw-rw-rw-  2.0 fat    11286 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/XRECORD_0.bin
--rw-rw-rw-  2.0 fat    11662 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/XRECORD_1.bin
--rw-rw-rw-  2.0 fat    15337 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/XRECORD_2.bin
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf.egg-info/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acis/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/layouts/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/lldxf/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/path/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/pp/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/resources/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/sections/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/
--rw-rw-rw-  2.0 fat     4710 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/appsettings.py
--rw-rw-rw-  2.0 fat    19818 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/audit.py
--rw-rw-rw-  2.0 fat     5324 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/bbox.py
--rw-rw-rw-  2.0 fat     7888 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/blkrefs.py
--rw-rw-rw-  2.0 fat    13157 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/colors.py
--rw-rw-rw-  2.0 fat    31737 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/commands.py
--rw-rw-rw-  2.0 fat     1549 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/comments.py
--rw-rw-rw-  2.0 fat    22100 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/disassemble.py
--rw-rw-rw-  2.0 fat    52708 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/document.py
--rw-rw-rw-  2.0 fat      832 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/dwginfo.py
--rw-rw-rw-  2.0 fat    16248 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entitydb.py
--rw-rw-rw-  2.0 fat     7495 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/enums.py
--rw-rw-rw-  2.0 fat    13948 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/explode.py
--rw-rw-rw-  2.0 fat     1653 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/eztypes.py
--rw-rw-rw-  2.0 fat    10289 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/filemanagement.py
--rw-rw-rw-  2.0 fat    12157 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/gfxattribs.py
--rw-rw-rw-  2.0 fat   107500 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/graphicsfactory.py
--rw-rw-rw-  2.0 fat     3416 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/groupby.py
--rw-rw-rw-  2.0 fat     2942 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/npshapes.py
--rw-rw-rw-  2.0 fat     2567 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/protocols.py
--rw-rw-rw-  2.0 fat    32672 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/proxygraphic.py
--rw-rw-rw-  2.0 fat       95 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/py.typed
--rw-rw-rw-  2.0 fat    22499 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/query.py
--rw-rw-rw-  2.0 fat     2780 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/queryparser.py
--rw-rw-rw-  2.0 fat     9580 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/r12strict.py
--rw-rw-rw-  2.0 fat    30769 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/recover.py
--rw-rw-rw-  2.0 fat     3515 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/reorder.py
--rw-rw-rw-  2.0 fat    30244 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/shapefile.py
--rw-rw-rw-  2.0 fat    10364 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/transform.py
--rw-rw-rw-  2.0 fat     5648 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/units.py
--rw-rw-rw-  2.0 fat     8280 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/upright.py
--rw-rw-rw-  2.0 fat     9875 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/urecord.py
--rw-rw-rw-  2.0 fat     1024 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/version.py
--rw-rw-rw-  2.0 fat    63359 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/xref.py
--rw-rw-rw-  2.0 fat     2853 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/zoom.py
--rw-rw-rw-  2.0 fat    11516 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/_options.py
--rw-rw-rw-  2.0 fat     2583 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/__init__.py
--rw-rw-rw-  2.0 fat     2781 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/__main__.py
--rw-rw-rw-  2.0 fat     6072 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/bezier3p.pyx
--rw-rw-rw-  2.0 fat     9983 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/bezier4p.pyx
--rw-rw-rw-  2.0 fat    12964 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/bspline.pyx
--rw-rw-rw-  2.0 fat       90 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/construct.pxd
--rw-rw-rw-  2.0 fat     6584 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/construct.pyx
--rw-rw-rw-  2.0 fat     3113 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/linetypes.pyx
--rw-rw-rw-  2.0 fat    23989 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/mapbox_earcut.pyx
--rw-rw-rw-  2.0 fat      381 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/matrix44.pxd
--rw-rw-rw-  2.0 fat    21938 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/matrix44.pyx
--rw-rw-rw-  2.0 fat     2014 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/vector.pxd
--rw-rw-rw-  2.0 fat    23705 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/vector.pyx
--rw-rw-rw-  2.0 fat     1784 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_cubic_bezier.cpp
--rw-rw-rw-  2.0 fat      599 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_cubic_bezier.hpp
--rw-rw-rw-  2.0 fat      424 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_cubic_bezier.pxd
--rw-rw-rw-  2.0 fat      960 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_quad_bezier.cpp
--rw-rw-rw-  2.0 fat      464 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_quad_bezier.hpp
--rw-rw-rw-  2.0 fat      407 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_quad_bezier.pxd
--rw-rw-rw-  2.0 fat     2135 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_vec3.hpp
--rw-rw-rw-  2.0 fat      572 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_vec3.pxd
--rw-rw-rw-  2.0 fat     1265 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/__init__.py
--rw-rw-rw-  2.0 fat     6393 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acis/abstract.py
--rw-rw-rw-  2.0 fat      884 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acis/api.py
--rw-rw-rw-  2.0 fat     5484 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acis/const.py
--rw-rw-rw-  2.0 fat     6726 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acis/dbg.py
--rw-rw-rw-  2.0 fat     2980 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acis/dxf.py
--rw-rw-rw-  2.0 fat    28991 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acis/entities.py
--rw-rw-rw-  2.0 fat     4088 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acis/hdr.py
--rw-rw-rw-  2.0 fat    12823 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acis/mesh.py
--rw-rw-rw-  2.0 fat    18690 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acis/sab.py
--rw-rw-rw-  2.0 fat    13184 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acis/sat.py
--rw-rw-rw-  2.0 fat      115 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acis/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/acisbrowser/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/browser/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/drawing/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/dwg/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/
--rw-rw-rw-  2.0 fat    26415 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/acadctb.py
--rw-rw-rw-  2.0 fat    22229 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/binpacking.py
--rw-rw-rw-  2.0 fat    27692 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/dimlines.py
--rw-rw-rw-  2.0 fat    31371 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/dxf2code.py
--rw-rw-rw-  2.0 fat    22037 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/genetic_algorithm.py
--rw-rw-rw-  2.0 fat    36445 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/geo.py
--rw-rw-rw-  2.0 fat     2674 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/gerber_D6673.py
--rw-rw-rw-  2.0 fat    25472 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/importer.py
--rw-rw-rw-  2.0 fat    17355 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/iterdxf.py
--rw-rw-rw-  2.0 fat     8940 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/menger_sponge.py
--rw-rw-rw-  2.0 fat    24787 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/meshex.py
--rw-rw-rw-  2.0 fat      492 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/mixins.py
--rw-rw-rw-  2.0 fat     6203 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/mtextsurrogate.py
--rw-rw-rw-  2.0 fat    13499 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/mtxpl.py
--rw-rw-rw-  2.0 fat    16400 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/odafc.py
--rw-rw-rw-  2.0 fat     9456 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/openscad.py
--rw-rw-rw-  2.0 fat    15878 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/pycsg.py
--rw-rw-rw-  2.0 fat    22496 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/r12export.py
--rw-rw-rw-  2.0 fat    27198 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/r12writer.py
--rw-rw-rw-  2.0 fat     7615 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/sierpinski_pyramid.py
--rw-rw-rw-  2.0 fat    33167 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/tablepainter.py
--rw-rw-rw-  2.0 fat    12766 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/text2path.py
--rw-rw-rw-  2.0 fat     2312 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/xqt.py
--rw-rw-rw-  2.0 fat      453 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/__init__.py
--rw-rw-rw-  2.0 fat    10023 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/acisbrowser/browser.py
--rw-rw-rw-  2.0 fat     1907 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/acisbrowser/data.py
--rw-rw-rw-  2.0 fat       64 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/acisbrowser/__init__.py
--rw-rw-rw-  2.0 fat      820 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/browser/bookmarks.py
--rw-rw-rw-  2.0 fat    29367 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/browser/browser.py
--rw-rw-rw-  2.0 fat    14891 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/browser/data.py
--rw-rw-rw-  2.0 fat    10993 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/browser/find_dialog.py
--rw-rw-rw-  2.0 fat     1281 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/browser/loader.py
--rw-rw-rw-  2.0 fat    20974 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/browser/model.py
--rw-rw-rw-  2.0 fat     2214 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/browser/tags.py
--rw-rw-rw-  2.0 fat     1382 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/browser/views.py
--rw-rw-rw-  2.0 fat      133 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/browser/__init__.py
--rw-rw-rw-  2.0 fat     7094 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/drawing/backend.py
--rw-rw-rw-  2.0 fat     3611 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/drawing/clipper.py
--rw-rw-rw-  2.0 fat     6737 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/drawing/config.py
--rw-rw-rw-  2.0 fat     1392 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/drawing/debug_backend.py
--rw-rw-rw-  2.0 fat      503 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/drawing/debug_utils.py
--rw-rw-rw-  2.0 fat    41820 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/drawing/frontend.py
--rw-rw-rw-  2.0 fat     1823 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/drawing/gfxproxy.py
--rw-rw-rw-  2.0 fat    12613 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/drawing/matplotlib.py
--rw-rw-rw-  2.0 fat     9854 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/drawing/mtext_complex.py
--rw-rw-rw-  2.0 fat    37741 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/drawing/properties.py
--rw-rw-rw-  2.0 fat    10774 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/drawing/pyqt.py
--rw-rw-rw-  2.0 fat    16738 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/drawing/qtviewer.py
--rw-rw-rw-  2.0 fat    13011 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/drawing/text.py
--rw-rw-rw-  2.0 fat      860 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/drawing/text_renderer.py
--rw-rw-rw-  2.0 fat      344 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/drawing/type_hints.py
--rw-rw-rw-  2.0 fat     2461 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/drawing/unified_text_renderer.py
--rw-rw-rw-  2.0 fat      171 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/drawing/__init__.py
--rw-rw-rw-  2.0 fat     3112 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/dwg/classes_section.py
--rw-rw-rw-  2.0 fat      763 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/dwg/const.py
--rw-rw-rw-  2.0 fat     6091 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/dwg/crc.py
--rw-rw-rw-  2.0 fat     3160 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/dwg/fileheader.py
--rw-rw-rw-  2.0 fat    14851 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/dwg/header_section.py
--rw-rw-rw-  2.0 fat     2976 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/dwg/loader.py
--rw-rw-rw-  2.0 fat      141 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/dwg/__init__.py
--rw-rw-rw-  2.0 fat     9531 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/api.py
--rw-rw-rw-  2.0 fat     6651 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/backend.py
--rw-rw-rw-  2.0 fat      513 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/compiler.py
--rw-rw-rw-  2.0 fat      571 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/deps.py
--rw-rw-rw-  2.0 fat     4720 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/dxf_backend.py
--rw-rw-rw-  2.0 fat    16087 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/interpreter.py
--rw-rw-rw-  2.0 fat     4836 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/page.py
--rw-rw-rw-  2.0 fat     3527 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/pdf_backend.py
--rw-rw-rw-  2.0 fat    11957 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/plotter.py
--rw-rw-rw-  2.0 fat     1411 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/polygon_buffer.py
--rw-rw-rw-  2.0 fat     5953 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/properties.py
--rw-rw-rw-  2.0 fat     3731 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/svg_backend.py
--rw-rw-rw-  2.0 fat     6258 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/tokenizer.py
--rw-rw-rw-  2.0 fat      164 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/__init__.py
--rw-rw-rw-  2.0 fat     4757 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/acad_proxy_entity.py
--rw-rw-rw-  2.0 fat    18315 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/acad_table.py
--rw-rw-rw-  2.0 fat    25923 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/acis.py
--rw-rw-rw-  2.0 fat     4890 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/appdata.py
--rw-rw-rw-  2.0 fat     1954 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/appid.py
--rw-rw-rw-  2.0 fat     4942 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/arc.py
--rw-rw-rw-  2.0 fat    26138 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/attrib.py
--rw-rw-rw-  2.0 fat     7867 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/block.py
--rw-rw-rw-  2.0 fat    10536 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/blockrecord.py
--rw-rw-rw-  2.0 fat    50143 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/boundary_paths.py
--rw-rw-rw-  2.0 fat     7961 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/circle.py
--rw-rw-rw-  2.0 fat    23664 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/dictionary.py
--rw-rw-rw-  2.0 fat    48743 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/dimension.py
--rw-rw-rw-  2.0 fat    35012 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/dimstyle.py
--rw-rw-rw-  2.0 fat    23829 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/dimstyleoverride.py
--rw-rw-rw-  2.0 fat     4399 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/dxfclass.py
--rw-rw-rw-  2.0 fat    42404 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/dxfentity.py
--rw-rw-rw-  2.0 fat    26923 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/dxfgfx.py
--rw-rw-rw-  2.0 fat    15279 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/dxfgroups.py
--rw-rw-rw-  2.0 fat    23699 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/dxfns.py
--rw-rw-rw-  2.0 fat    13746 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/dxfobj.py
--rw-rw-rw-  2.0 fat    11186 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/ellipse.py
--rw-rw-rw-  2.0 fat     4170 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/factory.py
--rw-rw-rw-  2.0 fat    23785 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/geodata.py
--rw-rw-rw-  2.0 fat     4020 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/gradient.py
--rw-rw-rw-  2.0 fat    12263 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/hatch.py
--rw-rw-rw-  2.0 fat     3944 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/helix.py
--rw-rw-rw-  2.0 fat     4747 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/idbuffer.py
--rw-rw-rw-  2.0 fat    26057 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/image.py
--rw-rw-rw-  2.0 fat    27932 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/insert.py
--rw-rw-rw-  2.0 fat    27834 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/layer.py
--rw-rw-rw-  2.0 fat    14252 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/layout.py
--rw-rw-rw-  2.0 fat    12978 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/leader.py
--rw-rw-rw-  2.0 fat     4718 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/light.py
--rw-rw-rw-  2.0 fat     3718 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/line.py
--rw-rw-rw-  2.0 fat     9677 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/ltype.py
--rw-rw-rw-  2.0 fat    18878 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/lwpolyline.py
--rw-rw-rw-  2.0 fat    19653 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/material.py
--rw-rw-rw-  2.0 fat    18435 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/mesh.py
--rw-rw-rw-  2.0 fat    57367 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/mleader.py
--rw-rw-rw-  2.0 fat    37144 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/mline.py
--rw-rw-rw-  2.0 fat     8385 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/mpolygon.py
--rw-rw-rw-  2.0 fat    48153 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/mtext.py
--rw-rw-rw-  2.0 fat     4351 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/mtext_columns.py
--rw-rw-rw-  2.0 fat     6284 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/objectcollection.py
--rw-rw-rw-  2.0 fat     2111 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/oleframe.py
--rw-rw-rw-  2.0 fat     4332 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/pattern.py
--rw-rw-rw-  2.0 fat     5238 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/point.py
--rw-rw-rw-  2.0 fat    16416 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/polygon.py
--rw-rw-rw-  2.0 fat    40087 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/polyline.py
--rw-rw-rw-  2.0 fat     4822 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/shape.py
--rw-rw-rw-  2.0 fat    10443 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/solid.py
--rw-rw-rw-  2.0 fat    24085 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/spline.py
--rw-rw-rw-  2.0 fat     8246 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/subentity.py
--rw-rw-rw-  2.0 fat     5196 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/sun.py
--rw-rw-rw-  2.0 fat     2449 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/table.py
--rw-rw-rw-  2.0 fat    17602 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/text.py
--rw-rw-rw-  2.0 fat     9042 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/textstyle.py
--rw-rw-rw-  2.0 fat     3597 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/tolerance.py
--rw-rw-rw-  2.0 fat     2703 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/ucs.py
--rw-rw-rw-  2.0 fat    14366 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/underlay.py
--rw-rw-rw-  2.0 fat     6040 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/view.py
--rw-rw-rw-  2.0 fat    27893 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/viewport.py
--rw-rw-rw-  2.0 fat     7867 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/visualstyle.py
--rw-rw-rw-  2.0 fat     9970 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/vport.py
--rw-rw-rw-  2.0 fat    17024 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/xdata.py
--rw-rw-rw-  2.0 fat     8495 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/xdict.py
--rw-rw-rw-  2.0 fat     3062 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/xline.py
--rw-rw-rw-  2.0 fat     3127 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/__init__.py
--rw-rw-rw-  2.0 fat    16696 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/layouts/base.py
--rw-rw-rw-  2.0 fat     4343 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/layouts/blocklayout.py
--rw-rw-rw-  2.0 fat    29014 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/layouts/layout.py
--rw-rw-rw-  2.0 fat    15314 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/layouts/layouts.py
--rw-rw-rw-  2.0 fat      232 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/layouts/__init__.py
--rw-rw-rw-  2.0 fat     8327 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/lldxf/attributes.py
--rw-rw-rw-  2.0 fat    16500 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/lldxf/const.py
--rw-rw-rw-  2.0 fat     1614 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/lldxf/encoding.py
--rw-rw-rw-  2.0 fat    17013 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/lldxf/extendedtags.py
--rw-rw-rw-  2.0 fat     5363 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/lldxf/fileindex.py
--rw-rw-rw-  2.0 fat      727 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/lldxf/hdrvars.py
--rw-rw-rw-  2.0 fat     5469 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/lldxf/loader.py
--rw-rw-rw-  2.0 fat     7447 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/lldxf/packedtags.py
--rw-rw-rw-  2.0 fat     6355 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/lldxf/repair.py
--rw-rw-rw-  2.0 fat    13058 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/lldxf/tagger.py
--rw-rw-rw-  2.0 fat    14336 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/lldxf/tags.py
--rw-rw-rw-  2.0 fat     8952 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/lldxf/tagwriter.py
--rw-rw-rw-  2.0 fat    12064 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/lldxf/types.py
--rw-rw-rw-  2.0 fat    17069 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/lldxf/validator.py
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/lldxf/__init__.py
--rw-rw-rw-  2.0 fat    19193 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/arc.py
--rw-rw-rw-  2.0 fat    16270 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/bbox.py
--rw-rw-rw-  2.0 fat     9318 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/bezier.py
--rw-rw-rw-  2.0 fat     2452 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/bezier_interpolation.py
--rw-rw-rw-  2.0 fat     8730 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/box.py
--rw-rw-rw-  2.0 fat    52916 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/bspline.py
--rw-rw-rw-  2.0 fat     5608 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/bulge.py
--rw-rw-rw-  2.0 fat     9002 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/circle.py
--rw-rw-rw-  2.0 fat    24003 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/clipping.py
--rw-rw-rw-  2.0 fat     4319 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/clustering.py
--rw-rw-rw-  2.0 fat    12236 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/construct2d.py
--rw-rw-rw-  2.0 fat    26265 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/construct3d.py
--rw-rw-rw-  2.0 fat     1283 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/cspline.py
--rw-rw-rw-  2.0 fat     9114 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/curvetools.py
--rw-rw-rw-  2.0 fat    22048 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/ellipse.py
--rw-rw-rw-  2.0 fat     4406 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/eulerspiral.py
--rw-rw-rw-  2.0 fat    38883 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/linalg.py
--rw-rw-rw-  2.0 fat    10231 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/line.py
--rw-rw-rw-  2.0 fat     3053 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/offset2d.py
--rw-rw-rw-  2.0 fat     8256 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/parametrize.py
--rw-rw-rw-  2.0 fat    15602 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/perlin.py
--rw-rw-rw-  2.0 fat    15921 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/polyline.py
--rw-rw-rw-  2.0 fat    11867 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/rtree.py
--rw-rw-rw-  2.0 fat     3910 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/shape.py
--rw-rw-rw-  2.0 fat     2568 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/surfaces.py
--rw-rw-rw-  2.0 fat    12155 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/transformtools.py
--rw-rw-rw-  2.0 fat     3631 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/triangulation.py
--rw-rw-rw-  2.0 fat    16971 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/ucs.py
--rw-rw-rw-  2.0 fat     7213 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/_bezier3p.py
--rw-rw-rw-  2.0 fat    12967 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/_bezier4p.py
--rw-rw-rw-  2.0 fat     9440 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/_bspline.py
--rw-rw-rw-  2.0 fat     7272 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/_construct.py
--rw-rw-rw-  2.0 fat     2261 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/_ctypes.py
--rw-rw-rw-  2.0 fat    24954 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/_mapbox_earcut.py
--rw-rw-rw-  2.0 fat    26418 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/_matrix44.py
--rw-rw-rw-  2.0 fat    25912 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/_vector.py
--rw-rw-rw-  2.0 fat     2003 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/__init__.py
--rw-rw-rw-  2.0 fat     1306 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/path/commands.py
--rw-rw-rw-  2.0 fat    39194 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/path/converter.py
--rw-rw-rw-  2.0 fat     6748 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/path/nesting.py
--rw-rw-rw-  2.0 fat    20453 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/path/path.py
--rw-rw-rw-  2.0 fat    10140 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/path/shapes.py
--rw-rw-rw-  2.0 fat    34692 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/path/tools.py
--rw-rw-rw-  2.0 fat      385 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/path/__init__.py
--rw-rw-rw-  2.0 fat     2987 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/pp/dxfpp.css
--rw-rw-rw-  2.0 fat     1148 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/pp/dxfpp.html
--rw-rw-rw-  2.0 fat    11304 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/pp/dxfpp.js
--rw-rw-rw-  2.0 fat    17144 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/pp/dxfpp.py
--rw-rw-rw-  2.0 fat     3770 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/pp/pprint.py
--rw-rw-rw-  2.0 fat      812 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/pp/rawpp.css
--rw-rw-rw-  2.0 fat      316 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/pp/rawpp.html
--rw-rw-rw-  2.0 fat     2545 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/pp/rawpp.py
--rw-rw-rw-  2.0 fat     6896 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/pp/reflinks.py
--rw-rw-rw-  2.0 fat      123 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/pp/__init__.py
--rw-rw-rw-  2.0 fat    10076 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/abstract_mtext_renderer.py
--rw-rw-rw-  2.0 fat    20495 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/arrows.py
--rw-rw-rw-  2.0 fat    17749 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/curves.py
--rw-rw-rw-  2.0 fat     4041 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/dimension.py
--rw-rw-rw-  2.0 fat    52028 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/dim_base.py
--rw-rw-rw-  2.0 fat    35702 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/dim_curved.py
--rw-rw-rw-  2.0 fat     6894 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/dim_diameter.py
--rw-rw-rw-  2.0 fat    24751 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/dim_linear.py
--rw-rw-rw-  2.0 fat     8084 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/dim_ordinate.py
--rw-rw-rw-  2.0 fat    20295 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/dim_radius.py
--rw-rw-rw-  2.0 fat    47170 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/forms.py
--rw-rw-rw-  2.0 fat    24213 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/hatching.py
--rw-rw-rw-  2.0 fat     4728 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/leader.py
--rw-rw-rw-  2.0 fat      664 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/linetypes.py
--rw-rw-rw-  2.0 fat    64121 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/mesh.py
--rw-rw-rw-  2.0 fat    60923 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/mleader.py
--rw-rw-rw-  2.0 fat     8437 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/mline.py
--rw-rw-rw-  2.0 fat     2964 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/point.py
--rw-rw-rw-  2.0 fat     8736 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/polyline.py
--rw-rw-rw-  2.0 fat     7886 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/r12spline.py
--rw-rw-rw-  2.0 fat    22541 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/trace.py
--rw-rw-rw-  2.0 fat     2881 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/_linetypes.py
--rw-rw-rw-  2.0 fat      778 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/__init__.py
--rw-rw-rw-  2.0 fat     1050 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/resources/16x16.png
--rw-rw-rw-  2.0 fat     1420 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/resources/24x24.png
--rw-rw-rw-  2.0 fat    10638 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/resources/256x256.png
--rw-rw-rw-  2.0 fat     1758 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/resources/32x32.png
--rw-rw-rw-  2.0 fat     2335 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/resources/48x48.png
--rw-rw-rw-  2.0 fat     3050 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/resources/64x64.png
--rw-rw-rw-  2.0 fat     2090 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/resources/icon-copy-64px.png
--rw-rw-rw-  2.0 fat     3109 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/resources/icon-find-64px.png
--rw-rw-rw-  2.0 fat     2388 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/resources/icon-goto-bookmark-64px.png
--rw-rw-rw-  2.0 fat     2519 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/resources/icon-goto-handle-64px.png
--rw-rw-rw-  2.0 fat     2409 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/resources/icon-goto-line-64px.png
--rw-rw-rw-  2.0 fat     2231 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/resources/icon-left-arrow-64px.png
--rw-rw-rw-  2.0 fat     2322 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/resources/icon-next-entity-64px.png
--rw-rw-rw-  2.0 fat     2320 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/resources/icon-prev-entity-64px.png
--rw-rw-rw-  2.0 fat     2244 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/resources/icon-right-arrow-64px.png
--rw-rw-rw-  2.0 fat     2553 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/resources/icon-show-in-tree-64px.png
--rw-rw-rw-  2.0 fat     2373 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/resources/icon-store-bookmark-64px.png
--rw-rw-rw-  2.0 fat    10650 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/sections/acdsdata.py
--rw-rw-rw-  2.0 fat    16508 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/sections/blocks.py
--rw-rw-rw-  2.0 fat    11639 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/sections/classes.py
--rw-rw-rw-  2.0 fat     4137 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/sections/entities.py
--rw-rw-rw-  2.0 fat    11953 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/sections/header.py
--rw-rw-rw-  2.0 fat    60696 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/sections/headervars.py
--rw-rw-rw-  2.0 fat    27009 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/sections/objects.py
--rw-rw-rw-  2.0 fat    26581 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/sections/table.py
--rw-rw-rw-  2.0 fat     5270 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/sections/tables.py
--rw-rw-rw-  2.0 fat       67 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/sections/__init__.py
--rw-rw-rw-  2.0 fat    19711 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/analyze.py
--rw-rw-rw-  2.0 fat    20434 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/binarydata.py
--rw-rw-rw-  2.0 fat     2931 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/codepage.py
--rw-rw-rw-  2.0 fat     7645 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/complex_ltype.py
--rw-rw-rw-  2.0 fat     1782 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/crypt.py
--rw-rw-rw-  2.0 fat     1511 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/debug.py
--rw-rw-rw-  2.0 fat     2341 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/difftags.py
--rw-rw-rw-  2.0 fat    15940 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/fonts.py
--rw-rw-rw-  2.0 fat     2233 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/font_face.py
--rw-rw-rw-  2.0 fat    10887 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/font_manager.py
--rw-rw-rw-  2.0 fat     1235 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/handle.py
--rw-rw-rw-  2.0 fat      780 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/indexing.py
--rw-rw-rw-  2.0 fat     2145 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/juliandate.py
--rw-rw-rw-  2.0 fat     6166 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/pattern.py
--rw-rw-rw-  2.0 fat     1256 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/rawloader.py
--rw-rw-rw-  2.0 fat   129174 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/standards.py
--rw-rw-rw-  2.0 fat     6049 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/strip.py
--rw-rw-rw-  2.0 fat     1466 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/test.py
--rw-rw-rw-  2.0 fat    65388 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/text.py
--rw-rw-rw-  2.0 fat    54234 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/text_layout.py
--rw-rw-rw-  2.0 fat     6883 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/text_size.py
--rw-rw-rw-  2.0 fat     6678 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/ttfonts.py
--rw-rw-rw-  2.0 fat     3077 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/zipmanager.py
--rw-rw-rw-  2.0 fat   142734 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/_iso_pattern.py
--rw-rw-rw-  2.0 fat     3564 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/__init__.py
--rw-rw-rw-  2.0 fat        1 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf.egg-info/dependency_links.txt
--rw-rw-rw-  2.0 fat       47 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf.egg-info/entry_points.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf.egg-info/not-zip-safe
--rw-rw-rw-  2.0 fat    68966 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf.egg-info/PKG-INFO
--rw-rw-rw-  2.0 fat      302 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf.egg-info/requires.txt
--rw-rw-rw-  2.0 fat    31075 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf.egg-info/SOURCES.txt
--rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf.egg-info/top_level.txt
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_03_dxf_layouts/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_09_cython_acceleration/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_10_issues/
--rw-rw-rw-  2.0 fat      402 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/conftest.py
--rw-rw-rw-  2.0 fat     2336 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
--rw-rw-rw-  2.0 fat      780 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
--rw-rw-rw-  2.0 fat     2599 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
--rw-rw-rw-  2.0 fat     1124 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
--rw-rw-rw-  2.0 fat     5456 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
--rw-rw-rw-  2.0 fat      582 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_010_binary_data.py
--rw-rw-rw-  2.0 fat      473 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_011_codepage.py
--rw-rw-rw-  2.0 fat    11593 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_012_crypt.py
--rw-rw-rw-  2.0 fat     1191 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_013_juliandate.py
--rw-rw-rw-  2.0 fat     1033 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py
--rw-rw-rw-  2.0 fat     4792 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py
--rw-rw-rw-  2.0 fat      989 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_016_encoding.py
--rw-rw-rw-  2.0 fat     1383 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_018_handle.py
--rw-rw-rw-  2.0 fat     5518 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py
--rw-rw-rw-  2.0 fat     8168 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py
--rw-rw-rw-  2.0 fat     3787 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py
--rw-rw-rw-  2.0 fat      401 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_022_set_flag_state.py
--rw-rw-rw-  2.0 fat      539 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py
--rw-rw-rw-  2.0 fat     2092 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_024_render_tag.py
--rw-rw-rw-  2.0 fat    10917 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_040_tags.py
--rw-rw-rw-  2.0 fat     3073 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_041_group_tags.py
--rw-rw-rw-  2.0 fat     6419 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py
--rw-rw-rw-  2.0 fat     1632 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py
--rw-rw-rw-  2.0 fat    11265 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py
--rw-rw-rw-  2.0 fat     3363 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py
--rw-rw-rw-  2.0 fat     1974 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py
--rw-rw-rw-  2.0 fat     2321 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py
--rw-rw-rw-  2.0 fat      568 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py
--rw-rw-rw-  2.0 fat     8682 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py
--rw-rw-rw-  2.0 fat     1051 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py
--rw-rw-rw-  2.0 fat     1500 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py
--rw-rw-rw-  2.0 fat    11689 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_101_dxfnamespace.py
--rw-rw-rw-  2.0 fat     2893 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_102_appdata.py
--rw-rw-rw-  2.0 fat     2312 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_103_reactors.py
--rw-rw-rw-  2.0 fat     4001 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_104_extension_dict.py
--rw-rw-rw-  2.0 fat    20860 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_105_xdata.py
--rw-rw-rw-  2.0 fat    14169 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_110_dxfentity.py
--rw-rw-rw-  2.0 fat     2433 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py
--rw-rw-rw-  2.0 fat     6781 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_112a_dxfgfx.py
--rw-rw-rw-  2.0 fat      695 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_112b_dxfobj.py
--rw-rw-rw-  2.0 fat     2431 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_113_dxfclass.py
--rw-rw-rw-  2.0 fat     4044 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_114_factory.py
--rw-rw-rw-  2.0 fat     2256 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_115_new_empty_drawing.py
--rw-rw-rw-  2.0 fat    15794 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_116_dictionary.py
--rw-rw-rw-  2.0 fat     4999 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_117_layer_table_entry.py
--rw-rw-rw-  2.0 fat      385 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_118_appid_table_entry.py
--rw-rw-rw-  2.0 fat     1058 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_119_ucs_table_entry.py
--rw-rw-rw-  2.0 fat     3003 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_120_style_table_entry.py
--rw-rw-rw-  2.0 fat     2943 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_121_ltype_table_entry.py
--rw-rw-rw-  2.0 fat      379 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_122_vport_table_entry.py
--rw-rw-rw-  2.0 fat     1113 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_123_view_table_entry.py
--rw-rw-rw-  2.0 fat     8757 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py
--rw-rw-rw-  2.0 fat     1698 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_125_image_def.py
--rw-rw-rw-  2.0 fat     1312 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_126_image_def_reactor.py
--rw-rw-rw-  2.0 fat     1430 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_127_raster_variables.py
--rw-rw-rw-  2.0 fat     1540 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_128_pdf_definition.py
--rw-rw-rw-  2.0 fat     2778 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_129_xrecord.py
--rw-rw-rw-  2.0 fat     2423 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_130_id_buffer.py
--rw-rw-rw-  2.0 fat     2470 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_131_field_list.py
--rw-rw-rw-  2.0 fat     2435 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_132_layer_filter.py
--rw-rw-rw-  2.0 fat     2153 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_133_sun.py
--rw-rw-rw-  2.0 fat      852 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_134_material.py
--rw-rw-rw-  2.0 fat    11497 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_135_geo_data.py
--rw-rw-rw-  2.0 fat     1087 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_136_vba_project.py
--rw-rw-rw-  2.0 fat     3099 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_137_sortentstable.py
--rw-rw-rw-  2.0 fat      704 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_138_setup_visual_styles.py
--rw-rw-rw-  2.0 fat     7570 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_139_user_record.py
--rw-rw-rw-  2.0 fat      714 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_140_block_record.py
--rw-rw-rw-  2.0 fat     9153 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_141_layer_vp_override.py
--rw-rw-rw-  2.0 fat     2231 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/conftest.py
--rw-rw-rw-  2.0 fat     6532 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_200_line.py
--rw-rw-rw-  2.0 fat     4273 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_201_point.py
--rw-rw-rw-  2.0 fat     6827 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_202_circle.py
--rw-rw-rw-  2.0 fat     8949 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_203_arc.py
--rw-rw-rw-  2.0 fat     2852 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_204_shape.py
--rw-rw-rw-  2.0 fat     8242 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_205_solid.py
--rw-rw-rw-  2.0 fat     8476 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_206_text.py
--rw-rw-rw-  2.0 fat     4947 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_207_attdef.py
--rw-rw-rw-  2.0 fat     6312 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_208_attrib.py
--rw-rw-rw-  2.0 fat     2671 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_209_vertex.py
--rw-rw-rw-  2.0 fat     5930 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_210_polyline_1.py
--rw-rw-rw-  2.0 fat    13489 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_210_polyline_2.py
--rw-rw-rw-  2.0 fat     6650 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_210_polyline_explode.py
--rw-rw-rw-  2.0 fat     1780 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py
--rw-rw-rw-  2.0 fat     7847 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_211_viewport.py
--rw-rw-rw-  2.0 fat    12629 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_212_insert.py
--rw-rw-rw-  2.0 fat     6024 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_213_minsert.py
--rw-rw-rw-  2.0 fat     3284 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_214_block.py
--rw-rw-rw-  2.0 fat     6882 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_215_dimension.py
--rw-rw-rw-  2.0 fat     4907 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_216_dimlines_R12.py
--rw-rw-rw-  2.0 fat    13186 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py
--rw-rw-rw-  2.0 fat     6471 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py
--rw-rw-rw-  2.0 fat     5535 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py
--rw-rw-rw-  2.0 fat     3056 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py
--rw-rw-rw-  2.0 fat     7181 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py
--rw-rw-rw-  2.0 fat     2066 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py
--rw-rw-rw-  2.0 fat     3615 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py
--rw-rw-rw-  2.0 fat     6919 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_221_ellipse.py
--rw-rw-rw-  2.0 fat     2223 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_222_xline.py
--rw-rw-rw-  2.0 fat     1493 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_223_ray.py
--rw-rw-rw-  2.0 fat     2176 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_224_group.py
--rw-rw-rw-  2.0 fat    10917 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_225_mtext.py
--rw-rw-rw-  2.0 fat    12020 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_226_spline.py
--rw-rw-rw-  2.0 fat     5529 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py
--rw-rw-rw-  2.0 fat    10893 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py
--rw-rw-rw-  2.0 fat    15116 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_228_mesh.py
--rw-rw-rw-  2.0 fat     2695 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py
--rw-rw-rw-  2.0 fat    21421 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_229b_hatch_extended.py
--rw-rw-rw-  2.0 fat     6587 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py
--rw-rw-rw-  2.0 fat     3140 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py
--rw-rw-rw-  2.0 fat    12486 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py
--rw-rw-rw-  2.0 fat     2274 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_231_underlay.py
--rw-rw-rw-  2.0 fat     5243 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_231_underlay_2.py
--rw-rw-rw-  2.0 fat     2294 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_232_acis.py
--rw-rw-rw-  2.0 fat     6799 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_232_acis_2.py
--rw-rw-rw-  2.0 fat     1854 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_232_surface.py
--rw-rw-rw-  2.0 fat     2695 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_233_helix.py
--rw-rw-rw-  2.0 fat     2040 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_234_light.py
--rw-rw-rw-  2.0 fat     3806 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_235_leader.py
--rw-rw-rw-  2.0 fat    20392 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_236_multileader.py
--rw-rw-rw-  2.0 fat    10992 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_237_mline.py
--rw-rw-rw-  2.0 fat     2356 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_238_tolerance.py
--rw-rw-rw-  2.0 fat    27392 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_239_proxy_graphic.py
--rw-rw-rw-  2.0 fat     4347 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_240_arc_dimension.py
--rw-rw-rw-  2.0 fat     1069 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_241_hyperlink.py
--rw-rw-rw-  2.0 fat    11313 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_242_random_transform.py
--rw-rw-rw-  2.0 fat     3725 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_243_replace_entity.py
--rw-rw-rw-  2.0 fat     1445 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py
--rw-rw-rw-  2.0 fat     4456 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_245_wipeout.py
--rw-rw-rw-  2.0 fat     6175 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_246_spline_audit.py
--rw-rw-rw-  2.0 fat     8165 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py
--rw-rw-rw-  2.0 fat     6003 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_248_mpolygon.py
--rw-rw-rw-  2.0 fat    13682 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py
--rw-rw-rw-  2.0 fat     5713 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_249_boundary_paths.py
--rw-rw-rw-  2.0 fat     8331 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py
--rw-rw-rw-  2.0 fat     7331 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_251_upright.py
--rw-rw-rw-  2.0 fat     4795 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py
--rw-rw-rw-  2.0 fat     2082 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_253_ole2frame.py
--rw-rw-rw-  2.0 fat      821 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_254_get_font_name.py
--rw-rw-rw-  2.0 fat     5149 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_300_layout.py
--rw-rw-rw-  2.0 fat     4274 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py
--rw-rw-rw-  2.0 fat     5582 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_302_block_references.py
--rw-rw-rw-  2.0 fat     2695 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_303_auto_block_references.py
--rw-rw-rw-  2.0 fat      913 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_304_new_entity_space.py
--rw-rw-rw-  2.0 fat     3279 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py
--rw-rw-rw-  2.0 fat     2609 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py
--rw-rw-rw-  2.0 fat     2343 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_307_groupby.py
--rw-rw-rw-  2.0 fat    17748 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_308_query.py
--rw-rw-rw-  2.0 fat     6382 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_309_query_parser.py
--rw-rw-rw-  2.0 fat     5031 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py
--rw-rw-rw-  2.0 fat     5782 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_312_virtual_layout.py
--rw-rw-rw-  2.0 fat      647 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_313_redraw_order.py
--rw-rw-rw-  2.0 fat     6128 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_401_headersection.py
--rw-rw-rw-  2.0 fat     2750 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_402_classessection.py
--rw-rw-rw-  2.0 fat     5208 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_403_entity_database.py
--rw-rw-rw-  2.0 fat     6795 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_404a_tables.py
--rw-rw-rw-  2.0 fat     4981 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py
--rw-rw-rw-  2.0 fat     2450 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_405_classes.py
--rw-rw-rw-  2.0 fat     9094 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py
--rw-rw-rw-  2.0 fat      848 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_407_entity_section.py
--rw-rw-rw-  2.0 fat     3375 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_408_objects_section.py
--rw-rw-rw-  2.0 fat     1433 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_409_create_objects.py
--rw-rw-rw-  2.0 fat     5736 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_410_table.py
--rw-rw-rw-  2.0 fat     6607 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_411_acds_data.py
--rw-rw-rw-  2.0 fat     1058 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py
--rw-rw-rw-  2.0 fat     2246 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py
--rw-rw-rw-  2.0 fat    18072 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py
--rw-rw-rw-  2.0 fat     4638 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_415_layout_management.py
--rw-rw-rw-  2.0 fat    12354 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py
--rw-rw-rw-  2.0 fat     6509 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py
--rw-rw-rw-  2.0 fat     5656 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_417_bbox.py
--rw-rw-rw-  2.0 fat     5434 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py
--rw-rw-rw-  2.0 fat      733 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py
--rw-rw-rw-  2.0 fat     1240 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py
--rw-rw-rw-  2.0 fat     5007 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py
--rw-rw-rw-  2.0 fat      769 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py
--rw-rw-rw-  2.0 fat     7289 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_424_audit.py
--rw-rw-rw-  2.0 fat     3737 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py
--rw-rw-rw-  2.0 fat     2981 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py
--rw-rw-rw-  2.0 fat     2416 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_427_appsettings.py
--rw-rw-rw-  2.0 fat     2533 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py
--rw-rw-rw-  2.0 fat   112800 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/conftest.py
--rw-rw-rw-  2.0 fat     5510 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_500_units.py
--rw-rw-rw-  2.0 fat     1052 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_501_truecolor.py
--rw-rw-rw-  2.0 fat     1021 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_502_raw_color.py
--rw-rw-rw-  2.0 fat     1695 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_503_indexing.py
--rw-rw-rw-  2.0 fat     1442 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_504_suppress_zeros.py
--rw-rw-rw-  2.0 fat      216 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_506_version.py
--rw-rw-rw-  2.0 fat      579 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_507_dxf_pretty_printer.py
--rw-rw-rw-  2.0 fat      657 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_508_read_zip.py
--rw-rw-rw-  2.0 fat     1445 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_509_comments.py
--rw-rw-rw-  2.0 fat     1185 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_510_byte_stream.py
--rw-rw-rw-  2.0 fat     4239 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_511_bit_stream.py
--rw-rw-rw-  2.0 fat     5595 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_512_pattern.py
--rw-rw-rw-  2.0 fat     2372 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_513_reorder_entities.py
--rw-rw-rw-  2.0 fat    17710 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_514_text.py
--rw-rw-rw-  2.0 fat     6261 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_515_fonts.py
--rw-rw-rw-  2.0 fat     4002 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_516_zoom.py
--rw-rw-rw-  2.0 fat    34209 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_517_text_layout.py
--rw-rw-rw-  2.0 fat      474 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_518_header_guid.py
--rw-rw-rw-  2.0 fat     3716 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_519_mtext_editor.py
--rw-rw-rw-  2.0 fat     3205 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_520_mtext_context.py
--rw-rw-rw-  2.0 fat    24496 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_521_mtext_parser.py
--rw-rw-rw-  2.0 fat     3863 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_522_text_scanner.py
--rw-rw-rw-  2.0 fat     5207 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_523_text_size.py
--rw-rw-rw-  2.0 fat     5063 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_524_block_reference_manager.py
--rw-rw-rw-  2.0 fat      773 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_525_transparency.py
--rw-rw-rw-  2.0 fat     2133 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_526_explode.py
--rw-rw-rw-  2.0 fat    13521 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_527_gfxattribs.py
--rw-rw-rw-  2.0 fat     2748 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_528_difftags.py
--rw-rw-rw-  2.0 fat     6700 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_529_acis_sat.py
--rw-rw-rw-  2.0 fat     2062 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_530_acis_sab.py
--rw-rw-rw-  2.0 fat    12366 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_531_acis_entities.py
--rw-rw-rw-  2.0 fat     7533 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_532_acis_mesh.py
--rw-rw-rw-  2.0 fat    42518 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_533_shapefiles.py
--rw-rw-rw-  2.0 fat     1034 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_534_dwg_info.py
--rw-rw-rw-  2.0 fat    47915 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_535_xref_basic.py
--rw-rw-rw-  2.0 fat    27614 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_536_xref_conflict.py
--rw-rw-rw-  2.0 fat     6887 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_537_transform.py
--rw-rw-rw-  2.0 fat     2246 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_538_scale_mtext_inline_commands.py
--rw-rw-rw-  2.0 fat     2763 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_539_npshapes.py
--rw-rw-rw-  2.0 fat     4026 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/conftest.py
--rw-rw-rw-  2.0 fat     7460 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_600_base.py
--rw-rw-rw-  2.0 fat     2098 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_601_bulge.py
--rw-rw-rw-  2.0 fat    14651 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_602_vec3.py
--rw-rw-rw-  2.0 fat     8956 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_603_vec2.py
--rw-rw-rw-  2.0 fat     2801 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_604_banded_matrix.py
--rw-rw-rw-  2.0 fat     9738 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_604_linalg.py
--rw-rw-rw-  2.0 fat    13007 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_605_matrix44.py
--rw-rw-rw-  2.0 fat     5888 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_606_convexhull.py
--rw-rw-rw-  2.0 fat     1010 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_607_perlin_noise.py
--rw-rw-rw-  2.0 fat     3833 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_608_intersection_line_line_2d.py
--rw-rw-rw-  2.0 fat     1676 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_609_point_on_line.py
--rw-rw-rw-  2.0 fat     3171 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_610_ocs.py
--rw-rw-rw-  2.0 fat     7529 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_611_ucs.py
--rw-rw-rw-  2.0 fat     1831 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_612_ucs_pass_trough.py
--rw-rw-rw-  2.0 fat     2586 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_613_point_in_poygon.py
--rw-rw-rw-  2.0 fat    10913 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_614_construct_3d.py
--rw-rw-rw-  2.0 fat      602 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_615_rytz_axis.py
--rw-rw-rw-  2.0 fat     5215 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_616_plane.py
--rw-rw-rw-  2.0 fat      772 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_617_clockwise_orientation.py
--rw-rw-rw-  2.0 fat     6384 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_618_clipping.py
--rw-rw-rw-  2.0 fat    10108 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_619_greiner_hormann.py
--rw-rw-rw-  2.0 fat     2669 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_620_knot.py
--rw-rw-rw-  2.0 fat    18821 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_621_bspline.py
--rw-rw-rw-  2.0 fat     7652 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_622_bsplineu.py
--rw-rw-rw-  2.0 fat    11327 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_623_rbspline.py
--rw-rw-rw-  2.0 fat    10809 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_624_global_bspline_interpolation.py
--rw-rw-rw-  2.0 fat     1247 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_626_local_bspline_interpolation.py
--rw-rw-rw-  2.0 fat     1967 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_627_bspline_basis.py
--rw-rw-rw-  2.0 fat    10545 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_629_bezier.py
--rw-rw-rw-  2.0 fat    10714 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_630a_bezier4p_base.py
--rw-rw-rw-  2.0 fat    10204 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_630b_bezier4p_functions.py
--rw-rw-rw-  2.0 fat     1683 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_631_euler_spiral.py
--rw-rw-rw-  2.0 fat     4021 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_632_bezier3p.py
--rw-rw-rw-  2.0 fat    19463 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_640_bbox.py
--rw-rw-rw-  2.0 fat     5393 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_641_construction_ray.py
--rw-rw-rw-  2.0 fat     3673 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_642_construction_line.py
--rw-rw-rw-  2.0 fat     9459 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_643_construction_box.py
--rw-rw-rw-  2.0 fat    10941 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_644_construction_circle.py
--rw-rw-rw-  2.0 fat    10988 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_645_construction_arc.py
--rw-rw-rw-  2.0 fat     3422 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_646_offset_vertices_2d.py
--rw-rw-rw-  2.0 fat     7672 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_647_transform_tools.py
--rw-rw-rw-  2.0 fat     8993 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_648_construction_ellipse.py
--rw-rw-rw-  2.0 fat     4243 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_650_elliptic_arc_span.py
--rw-rw-rw-  2.0 fat     9011 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_651_construction_polyline.py
--rw-rw-rw-  2.0 fat     3168 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_652_approx_param_t.py
--rw-rw-rw-  2.0 fat     5806 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_653_polyline_intersection.py
--rw-rw-rw-  2.0 fat     5193 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_654_rtree.py
--rw-rw-rw-  2.0 fat      788 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_655_dbscan.py
--rw-rw-rw-  2.0 fat      834 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_656_k_means.py
--rw-rw-rw-  2.0 fat     4654 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_657_mapbox_earcut.py
--rw-rw-rw-  2.0 fat    11628 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_658_bevel_tools.py
--rw-rw-rw-  2.0 fat     1875 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_659_intersection_line_polygon_3d.py
--rw-rw-rw-  2.0 fat     1428 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_660_intersection_ray_polygon_3d.py
--rw-rw-rw-  2.0 fat     1741 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py
--rw-rw-rw-  2.0 fat     3307 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_662_is_convex_polygon_2d.py
--rw-rw-rw-  2.0 fat     1466 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/test_701_arrows.py
--rw-rw-rw-  2.0 fat    17245 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/test_702_render_forms.py
--rw-rw-rw-  2.0 fat    34220 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/test_703_mesh_builder.py
--rw-rw-rw-  2.0 fat     3852 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/test_704_render_linear_dimension.py
--rw-rw-rw-  2.0 fat     1345 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/test_705_shape.py
--rw-rw-rw-  2.0 fat      483 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/test_706_random_path.py
--rw-rw-rw-  2.0 fat     5603 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/test_707_trace.py
--rw-rw-rw-  2.0 fat    33834 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/test_708a_path.py
--rw-rw-rw-  2.0 fat    27351 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/test_708b_path_tools.py
--rw-rw-rw-  2.0 fat     3633 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/test_708c_matplotlib_path_tools.py
--rw-rw-rw-  2.0 fat     3099 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/test_708d_qpainter_path_tools.py
--rw-rw-rw-  2.0 fat     4589 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/test_708e_path_shapes.py
--rw-rw-rw-  2.0 fat     4118 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/test_708f_path_nesting.py
--rw-rw-rw-  2.0 fat     1308 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/test_709_linetype_renderer.py
--rw-rw-rw-  2.0 fat     2815 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/test_711_points.py
--rw-rw-rw-  2.0 fat     6594 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/test_712_render_curved_dimension.py
--rw-rw-rw-  2.0 fat     1472 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/test_713_mleader_builder.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/test_714_mleader_render_engine.py
--rw-rw-rw-  2.0 fat    11778 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/test_715_hatching.py
--rw-rw-rw-  2.0 fat     2626 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/test_715_issue_747_explode_3d_dim.py
--rw-rw-rw-  2.0 fat     4771 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_800_mtext_surrogate.py
--rw-rw-rw-  2.0 fat     1352 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_801_r12spline.py
--rw-rw-rw-  2.0 fat     7881 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_802_table_painter.py
--rw-rw-rw-  2.0 fat    12386 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_803_entities_to_code.py
--rw-rw-rw-  2.0 fat     6844 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_804_importer.py
--rw-rw-rw-  2.0 fat     2362 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_805_pycsg.py
--rw-rw-rw-  2.0 fat    15467 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_806_acadctb.py
--rw-rw-rw-  2.0 fat     4860 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_807_dwg_loader_basics.py
--rw-rw-rw-  2.0 fat    10862 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_810_drawing_properties.py
--rw-rw-rw-  2.0 fat    11175 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_811_drawing_frontend.py
--rw-rw-rw-  2.0 fat     4157 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_812_drawing_graphic_proxy.py
--rw-rw-rw-  2.0 fat    12547 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_813_geo_interface.py
--rw-rw-rw-  2.0 fat    15590 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_814_text2path.py
--rw-rw-rw-  2.0 fat    16239 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_815_dxf_browser.py
--rw-rw-rw-  2.0 fat    11275 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_816_bin_packing.py
--rw-rw-rw-  2.0 fat    12554 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_817_genetic_algorithm.py
--rw-rw-rw-  2.0 fat     9008 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_818_meshex.py
--rw-rw-rw-  2.0 fat     1003 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_819_menger_sponge.py
--rw-rw-rw-  2.0 fat     4433 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_820_openscad.py
--rw-rw-rw-  2.0 fat    15527 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_821_hpgl2.py
--rw-rw-rw-  2.0 fat     1322 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
--rw-rw-rw-  2.0 fat      976 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_822_clipper.py
--rw-rw-rw-  2.0 fat     2527 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_09_cython_acceleration/test_901_acc_vec2.py
--rw-rw-rw-  2.0 fat     2199 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_09_cython_acceleration/test_902_acc_vec3.py
--rw-rw-rw-  2.0 fat     1732 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_09_cython_acceleration/test_903_acc_matrix44.py
--rw-rw-rw-  2.0 fat     3158 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
--rw-rw-rw-  2.0 fat     1452 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
--rw-rw-rw-  2.0 fat     4755 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_09_cython_acceleration/test_906_acc_bspline.py
--rw-rw-rw-  2.0 fat     2656 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_10_issues/test_issue_414_bbox_calculation.py
--rw-rw-rw-  2.0 fat     1213 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
--rw-rw-rw-  2.0 fat     2268 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_10_issues/test_issue_574_flattening_error.py
--rw-rw-rw-  2.0 fat     1754 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
--rw-rw-rw-  2.0 fat      682 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_10_issues/test_issue_749_text_layout.py
-819 files, 8482167 bytes uncompressed, 1907843 bytes compressed:  77.5%
+Zip file size: 2070630 bytes, number of entries: 829
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/integration_tests/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/tests/
+-rw-rw-rw-  2.0 fat     1092 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/LICENSE
+-rw-rw-rw-  2.0 fat      302 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/MANIFEST.in
+-rw-rw-rw-  2.0 fat   101339 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/NEWS.md
+-rw-rw-rw-  2.0 fat    69206 b- defN 23-May-06 04:16 ezdxf-1.1.0b1/PKG-INFO
+-rw-rw-rw-  2.0 fat     6142 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/README.md
+-rw-rw-rw-  2.0 fat       55 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/requirements.txt
+-rw-rw-rw-  2.0 fat       74 b- defN 23-May-06 04:16 ezdxf-1.1.0b1/setup.cfg
+-rw-rw-rw-  2.0 fat     5402 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/setup.py
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/integration_tests/data/
+-rw-rw-rw-  2.0 fat      567 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/check_disable_c_ext_by_config_file.py
+-rw-rw-rw-  2.0 fat      541 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/check_disable_c_ext_by_env_var.py
+-rw-rw-rw-  2.0 fat      410 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/conftest.py
+-rw-rw-rw-  2.0 fat     1054 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_acad_table.py
+-rw-rw-rw-  2.0 fat     4686 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_all_dimline_styles.py
+-rw-rw-rw-  2.0 fat     4133 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_all_ellipse_transformations.py
+-rw-rw-rw-  2.0 fat     1064 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_anonymous_blocks.py
+-rw-rw-rw-  2.0 fat      871 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_audit_critical_dxf_files.py
+-rw-rw-rw-  2.0 fat     1603 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_audit_layouts.py
+-rw-rw-rw-  2.0 fat     1726 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_complex_line_type_2.py
+-rw-rw-rw-  2.0 fat     1003 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_create_basic_graphics.py
+-rw-rw-rw-  2.0 fat     1921 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_document_guid.py
+-rw-rw-rw-  2.0 fat     1832 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_document_page_setup.py
+-rw-rw-rw-  2.0 fat      998 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_dxf_info_scanning.py
+-rw-rw-rw-  2.0 fat     1558 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_entities_iterator.py
+-rw-rw-rw-  2.0 fat      934 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_fix_dulicate_handles.py
+-rw-rw-rw-  2.0 fat     1901 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_geo.py
+-rw-rw-rw-  2.0 fat     1250 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_groups.py
+-rw-rw-rw-  2.0 fat      630 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_ignore_junk_beyond_EOF.py
+-rw-rw-rw-  2.0 fat     1155 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_launcher.py
+-rw-rw-rw-  2.0 fat      631 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_leica_disto_r12.py
+-rw-rw-rw-  2.0 fat      737 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_load_dxf_unicode_notation.py
+-rw-rw-rw-  2.0 fat     2931 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_mapbox_earcut.py
+-rw-rw-rw-  2.0 fat     2230 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_mtext_columns.py
+-rw-rw-rw-  2.0 fat     2392 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_mtext_explode_addon.py
+-rw-rw-rw-  2.0 fat     1846 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_mtext_text_frame.py
+-rw-rw-rw-  2.0 fat     1053 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_new_table_entries.py
+-rw-rw-rw-  2.0 fat      887 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_none_ascii_read_write.py
+-rw-rw-rw-  2.0 fat     3435 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_odafc.py
+-rw-rw-rw-  2.0 fat     1737 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_open_binary_DXF_files.py
+-rw-rw-rw-  2.0 fat      751 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_open_coord_order_issue.py
+-rw-rw-rw-  2.0 fat     3842 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_open_exotic_dxf_files.py
+-rw-rw-rw-  2.0 fat      879 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_open_R13_R14.py
+-rw-rw-rw-  2.0 fat     3152 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_polyline_entity.py
+-rw-rw-rw-  2.0 fat     1749 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_preserve_binary_data_in_xrecords.py
+-rw-rw-rw-  2.0 fat     6944 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_r12export.py
+-rw-rw-rw-  2.0 fat     6256 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_r12strict.py
+-rw-rw-rw-  2.0 fat     3410 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_r12writer.py
+-rw-rw-rw-  2.0 fat      567 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_read_file_without_handles.py
+-rw-rw-rw-  2.0 fat     1121 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_read_write_modern_entites.py
+-rw-rw-rw-  2.0 fat     5375 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_recover.py
+-rw-rw-rw-  2.0 fat     1959 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_redraw_order.py
+-rw-rw-rw-  2.0 fat     1819 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_rotated_block_attributes.py
+-rw-rw-rw-  2.0 fat      774 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_surface_entities.py
+-rw-rw-rw-  2.0 fat      928 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_write_fixed_meta_data.py
+-rw-rw-rw-  2.0 fat     1806 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_write_without_handles.py
+-rw-rw-rw-  2.0 fat     3638 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/test_xref_detach.py
+-rw-rw-rw-  2.0 fat     3060 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/AC1003_LINE_Example.dxf
+-rw-rw-rw-  2.0 fat   179505 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/acad_table_with_blk_ref.dxf
+-rw-rw-rw-  2.0 fat     7956 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/ASCII_R12.dxf
+-rw-rw-rw-  2.0 fat     3761 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/bin_dxf_r12.dxf
+-rw-rw-rw-  2.0 fat    20914 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/bin_dxf_r13.dxf
+-rw-rw-rw-  2.0 fat    21137 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/bin_dxf_r14.dxf
+-rw-rw-rw-  2.0 fat    11564 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/bin_dxf_r2000.dxf
+-rw-rw-rw-  2.0 fat     6424 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/cc_dxflib.dxf
+-rw-rw-rw-  2.0 fat   173753 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/custom_blocks.dxf
+-rw-rw-rw-  2.0 fat    32203 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/duplicate_handles.dxf
+-rw-rw-rw-  2.0 fat    18554 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/dxf_unicode.dxf
+-rw-rw-rw-  2.0 fat     1592 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/empty_handles.dxf
+-rw-rw-rw-  2.0 fat    97103 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/groups.dxf
+-rw-rw-rw-  2.0 fat     9146 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/Leica_Disto_S910.dxf
+-rw-rw-rw-  2.0 fat    17986 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/MODEL.dxf
+-rw-rw-rw-  2.0 fat    25799 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/mtext_columns_R2007.dxf
+-rw-rw-rw-  2.0 fat    23927 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/mtext_columns_R2018.dxf
+-rw-rw-rw-  2.0 fat    98230 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/mtext_framed_columns.dxf
+-rw-rw-rw-  2.0 fat   106574 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/mtext_text_frame.dxf
+-rw-rw-rw-  2.0 fat    12001 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/no_layouts.dxf
+-rw-rw-rw-  2.0 fat    28788 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/POLI-ALL210_12.DXF
+-rw-rw-rw-  2.0 fat      144 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/R12_with_trash_beyond_EOF.dxf
+-rw-rw-rw-  2.0 fat   212407 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/recover01.dxf
+-rw-rw-rw-  2.0 fat   115423 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/recover02.dxf
+-rw-rw-rw-  2.0 fat    21178 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/small_r13.dxf
+-rw-rw-rw-  2.0 fat    10326 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/small_r14.dxf
+-rw-rw-rw-  2.0 fat    11286 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/XRECORD_0.bin
+-rw-rw-rw-  2.0 fat    11662 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/XRECORD_1.bin
+-rw-rw-rw-  2.0 fat    15337 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/integration_tests/data/XRECORD_2.bin
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf.egg-info/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf/acc/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf/acis/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf/addons/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf/entities/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf/fonts/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf/layouts/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf/lldxf/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf/math/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf/path/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf/pp/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf/render/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf/resources/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf/sections/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf/tools/
+-rw-rw-rw-  2.0 fat     4710 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/appsettings.py
+-rw-rw-rw-  2.0 fat    19818 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/audit.py
+-rw-rw-rw-  2.0 fat     5324 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/bbox.py
+-rw-rw-rw-  2.0 fat     7888 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/blkrefs.py
+-rw-rw-rw-  2.0 fat    13157 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/colors.py
+-rw-rw-rw-  2.0 fat    31861 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/commands.py
+-rw-rw-rw-  2.0 fat     1549 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/comments.py
+-rw-rw-rw-  2.0 fat    22100 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/disassemble.py
+-rw-rw-rw-  2.0 fat    52708 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/document.py
+-rw-rw-rw-  2.0 fat      832 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/dwginfo.py
+-rw-rw-rw-  2.0 fat    16248 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entitydb.py
+-rw-rw-rw-  2.0 fat     7495 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/enums.py
+-rw-rw-rw-  2.0 fat    13948 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/explode.py
+-rw-rw-rw-  2.0 fat     1653 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/eztypes.py
+-rw-rw-rw-  2.0 fat    10333 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/filemanagement.py
+-rw-rw-rw-  2.0 fat    12157 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/gfxattribs.py
+-rw-rw-rw-  2.0 fat   107500 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/graphicsfactory.py
+-rw-rw-rw-  2.0 fat     3416 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/groupby.py
+-rw-rw-rw-  2.0 fat     3244 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/npshapes.py
+-rw-rw-rw-  2.0 fat     2567 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/protocols.py
+-rw-rw-rw-  2.0 fat    32672 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/proxygraphic.py
+-rw-rw-rw-  2.0 fat       95 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/py.typed
+-rw-rw-rw-  2.0 fat    22499 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/query.py
+-rw-rw-rw-  2.0 fat     2780 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/queryparser.py
+-rw-rw-rw-  2.0 fat     9580 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/r12strict.py
+-rw-rw-rw-  2.0 fat    30769 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/recover.py
+-rw-rw-rw-  2.0 fat     3515 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/reorder.py
+-rw-rw-rw-  2.0 fat    10364 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/transform.py
+-rw-rw-rw-  2.0 fat     5648 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/units.py
+-rw-rw-rw-  2.0 fat     8280 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/upright.py
+-rw-rw-rw-  2.0 fat     9875 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/urecord.py
+-rw-rw-rw-  2.0 fat     1024 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/version.py
+-rw-rw-rw-  2.0 fat    63359 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/xref.py
+-rw-rw-rw-  2.0 fat     2853 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/zoom.py
+-rw-rw-rw-  2.0 fat    10979 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/_options.py
+-rw-rw-rw-  2.0 fat     2566 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/__init__.py
+-rw-rw-rw-  2.0 fat     2786 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/__main__.py
+-rw-rw-rw-  2.0 fat     6072 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acc/bezier3p.pyx
+-rw-rw-rw-  2.0 fat     9983 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acc/bezier4p.pyx
+-rw-rw-rw-  2.0 fat    12964 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acc/bspline.pyx
+-rw-rw-rw-  2.0 fat       90 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acc/construct.pxd
+-rw-rw-rw-  2.0 fat     6584 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acc/construct.pyx
+-rw-rw-rw-  2.0 fat     3113 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acc/linetypes.pyx
+-rw-rw-rw-  2.0 fat    23989 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acc/mapbox_earcut.pyx
+-rw-rw-rw-  2.0 fat      386 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acc/matrix44.pxd
+-rw-rw-rw-  2.0 fat    23742 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acc/matrix44.pyx
+-rw-rw-rw-  2.0 fat     2014 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acc/vector.pxd
+-rw-rw-rw-  2.0 fat    23705 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acc/vector.pyx
+-rw-rw-rw-  2.0 fat     1784 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_cubic_bezier.cpp
+-rw-rw-rw-  2.0 fat      599 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_cubic_bezier.hpp
+-rw-rw-rw-  2.0 fat      424 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_cubic_bezier.pxd
+-rw-rw-rw-  2.0 fat      960 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_quad_bezier.cpp
+-rw-rw-rw-  2.0 fat      464 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_quad_bezier.hpp
+-rw-rw-rw-  2.0 fat      407 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_quad_bezier.pxd
+-rw-rw-rw-  2.0 fat     2135 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_vec3.hpp
+-rw-rw-rw-  2.0 fat      572 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_vec3.pxd
+-rw-rw-rw-  2.0 fat     1265 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acc/__init__.py
+-rw-rw-rw-  2.0 fat     6393 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acis/abstract.py
+-rw-rw-rw-  2.0 fat      884 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acis/api.py
+-rw-rw-rw-  2.0 fat     5484 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acis/const.py
+-rw-rw-rw-  2.0 fat     6726 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acis/dbg.py
+-rw-rw-rw-  2.0 fat     2980 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acis/dxf.py
+-rw-rw-rw-  2.0 fat    28991 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acis/entities.py
+-rw-rw-rw-  2.0 fat     4088 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acis/hdr.py
+-rw-rw-rw-  2.0 fat    12823 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acis/mesh.py
+-rw-rw-rw-  2.0 fat    18690 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acis/sab.py
+-rw-rw-rw-  2.0 fat    13184 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acis/sat.py
+-rw-rw-rw-  2.0 fat      115 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/acis/__init__.py
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf/addons/acisbrowser/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf/addons/browser/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf/addons/drawing/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf/addons/dwg/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/
+-rw-rw-rw-  2.0 fat    26415 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/acadctb.py
+-rw-rw-rw-  2.0 fat    22229 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/binpacking.py
+-rw-rw-rw-  2.0 fat    27692 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/dimlines.py
+-rw-rw-rw-  2.0 fat    31371 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/dxf2code.py
+-rw-rw-rw-  2.0 fat    22037 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/genetic_algorithm.py
+-rw-rw-rw-  2.0 fat    36445 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/geo.py
+-rw-rw-rw-  2.0 fat     2674 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/gerber_D6673.py
+-rw-rw-rw-  2.0 fat    25472 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/importer.py
+-rw-rw-rw-  2.0 fat    17355 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/iterdxf.py
+-rw-rw-rw-  2.0 fat     8940 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/menger_sponge.py
+-rw-rw-rw-  2.0 fat    24787 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/meshex.py
+-rw-rw-rw-  2.0 fat      492 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/mixins.py
+-rw-rw-rw-  2.0 fat     6203 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/mtextsurrogate.py
+-rw-rw-rw-  2.0 fat    13528 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/mtxpl.py
+-rw-rw-rw-  2.0 fat    16400 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/odafc.py
+-rw-rw-rw-  2.0 fat     9456 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/openscad.py
+-rw-rw-rw-  2.0 fat    15878 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/pycsg.py
+-rw-rw-rw-  2.0 fat    22496 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/r12export.py
+-rw-rw-rw-  2.0 fat    27198 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/r12writer.py
+-rw-rw-rw-  2.0 fat     7615 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/sierpinski_pyramid.py
+-rw-rw-rw-  2.0 fat    33167 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/tablepainter.py
+-rw-rw-rw-  2.0 fat    12789 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/text2path.py
+-rw-rw-rw-  2.0 fat     2312 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/xqt.py
+-rw-rw-rw-  2.0 fat      453 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/__init__.py
+-rw-rw-rw-  2.0 fat    10023 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/acisbrowser/browser.py
+-rw-rw-rw-  2.0 fat     1907 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/acisbrowser/data.py
+-rw-rw-rw-  2.0 fat       64 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/acisbrowser/__init__.py
+-rw-rw-rw-  2.0 fat      820 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/browser/bookmarks.py
+-rw-rw-rw-  2.0 fat    29367 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/browser/browser.py
+-rw-rw-rw-  2.0 fat    14891 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/browser/data.py
+-rw-rw-rw-  2.0 fat    10993 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/browser/find_dialog.py
+-rw-rw-rw-  2.0 fat     1281 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/browser/loader.py
+-rw-rw-rw-  2.0 fat    20974 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/browser/model.py
+-rw-rw-rw-  2.0 fat     2214 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/browser/tags.py
+-rw-rw-rw-  2.0 fat     1382 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/browser/views.py
+-rw-rw-rw-  2.0 fat      133 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/browser/__init__.py
+-rw-rw-rw-  2.0 fat     7301 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/drawing/backend.py
+-rw-rw-rw-  2.0 fat     3611 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/drawing/clipper.py
+-rw-rw-rw-  2.0 fat     6737 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/drawing/config.py
+-rw-rw-rw-  2.0 fat     1716 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/drawing/debug_backend.py
+-rw-rw-rw-  2.0 fat      514 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/drawing/debug_utils.py
+-rw-rw-rw-  2.0 fat    42098 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/drawing/frontend.py
+-rw-rw-rw-  2.0 fat     1823 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/drawing/gfxproxy.py
+-rw-rw-rw-  2.0 fat    12669 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/drawing/matplotlib.py
+-rw-rw-rw-  2.0 fat     9878 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/drawing/mtext_complex.py
+-rw-rw-rw-  2.0 fat    39188 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/drawing/properties.py
+-rw-rw-rw-  2.0 fat    10656 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/drawing/pyqt.py
+-rw-rw-rw-  2.0 fat    16738 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/drawing/qtviewer.py
+-rw-rw-rw-  2.0 fat     5914 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/drawing/recorder.py
+-rw-rw-rw-  2.0 fat    13023 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/drawing/text.py
+-rw-rw-rw-  2.0 fat      963 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/drawing/text_renderer.py
+-rw-rw-rw-  2.0 fat      344 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/drawing/type_hints.py
+-rw-rw-rw-  2.0 fat     1899 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/drawing/unified_text_renderer.py
+-rw-rw-rw-  2.0 fat      171 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/drawing/__init__.py
+-rw-rw-rw-  2.0 fat     3112 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/dwg/classes_section.py
+-rw-rw-rw-  2.0 fat      763 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/dwg/const.py
+-rw-rw-rw-  2.0 fat     6091 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/dwg/crc.py
+-rw-rw-rw-  2.0 fat     3160 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/dwg/fileheader.py
+-rw-rw-rw-  2.0 fat    14851 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/dwg/header_section.py
+-rw-rw-rw-  2.0 fat     2976 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/dwg/loader.py
+-rw-rw-rw-  2.0 fat      141 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/dwg/__init__.py
+-rw-rw-rw-  2.0 fat     9531 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/api.py
+-rw-rw-rw-  2.0 fat     6655 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/backend.py
+-rw-rw-rw-  2.0 fat      513 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/compiler.py
+-rw-rw-rw-  2.0 fat      571 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/deps.py
+-rw-rw-rw-  2.0 fat     4720 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/dxf_backend.py
+-rw-rw-rw-  2.0 fat    16087 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/interpreter.py
+-rw-rw-rw-  2.0 fat     4836 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/page.py
+-rw-rw-rw-  2.0 fat     3527 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/pdf_backend.py
+-rw-rw-rw-  2.0 fat    11957 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/plotter.py
+-rw-rw-rw-  2.0 fat     1411 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/polygon_buffer.py
+-rw-rw-rw-  2.0 fat     5953 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/properties.py
+-rw-rw-rw-  2.0 fat     3731 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/svg_backend.py
+-rw-rw-rw-  2.0 fat     6258 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/tokenizer.py
+-rw-rw-rw-  2.0 fat      164 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/__init__.py
+-rw-rw-rw-  2.0 fat     4757 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/acad_proxy_entity.py
+-rw-rw-rw-  2.0 fat    18315 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/acad_table.py
+-rw-rw-rw-  2.0 fat    25923 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/acis.py
+-rw-rw-rw-  2.0 fat     4890 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/appdata.py
+-rw-rw-rw-  2.0 fat     1954 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/appid.py
+-rw-rw-rw-  2.0 fat     4942 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/arc.py
+-rw-rw-rw-  2.0 fat    26138 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/attrib.py
+-rw-rw-rw-  2.0 fat     7867 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/block.py
+-rw-rw-rw-  2.0 fat    10536 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/blockrecord.py
+-rw-rw-rw-  2.0 fat    50143 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/boundary_paths.py
+-rw-rw-rw-  2.0 fat     7961 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/circle.py
+-rw-rw-rw-  2.0 fat    23664 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/dictionary.py
+-rw-rw-rw-  2.0 fat    48743 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/dimension.py
+-rw-rw-rw-  2.0 fat    35012 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/dimstyle.py
+-rw-rw-rw-  2.0 fat    23829 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/dimstyleoverride.py
+-rw-rw-rw-  2.0 fat     4399 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/dxfclass.py
+-rw-rw-rw-  2.0 fat    42404 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/dxfentity.py
+-rw-rw-rw-  2.0 fat    26923 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/dxfgfx.py
+-rw-rw-rw-  2.0 fat    15279 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/dxfgroups.py
+-rw-rw-rw-  2.0 fat    23699 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/dxfns.py
+-rw-rw-rw-  2.0 fat    13746 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/dxfobj.py
+-rw-rw-rw-  2.0 fat    11186 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/ellipse.py
+-rw-rw-rw-  2.0 fat     4170 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/factory.py
+-rw-rw-rw-  2.0 fat    23785 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/geodata.py
+-rw-rw-rw-  2.0 fat     4020 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/gradient.py
+-rw-rw-rw-  2.0 fat    12263 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/hatch.py
+-rw-rw-rw-  2.0 fat     3944 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/helix.py
+-rw-rw-rw-  2.0 fat     4747 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/idbuffer.py
+-rw-rw-rw-  2.0 fat    26057 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/image.py
+-rw-rw-rw-  2.0 fat    27932 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/insert.py
+-rw-rw-rw-  2.0 fat    27834 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/layer.py
+-rw-rw-rw-  2.0 fat    14252 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/layout.py
+-rw-rw-rw-  2.0 fat    12978 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/leader.py
+-rw-rw-rw-  2.0 fat     4718 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/light.py
+-rw-rw-rw-  2.0 fat     3718 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/line.py
+-rw-rw-rw-  2.0 fat     9677 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/ltype.py
+-rw-rw-rw-  2.0 fat    18878 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/lwpolyline.py
+-rw-rw-rw-  2.0 fat    19653 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/material.py
+-rw-rw-rw-  2.0 fat    18435 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/mesh.py
+-rw-rw-rw-  2.0 fat    57367 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/mleader.py
+-rw-rw-rw-  2.0 fat    37144 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/mline.py
+-rw-rw-rw-  2.0 fat     8385 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/mpolygon.py
+-rw-rw-rw-  2.0 fat    48153 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/mtext.py
+-rw-rw-rw-  2.0 fat     4351 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/mtext_columns.py
+-rw-rw-rw-  2.0 fat     6284 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/objectcollection.py
+-rw-rw-rw-  2.0 fat     2111 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/oleframe.py
+-rw-rw-rw-  2.0 fat     4332 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/pattern.py
+-rw-rw-rw-  2.0 fat     5238 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/point.py
+-rw-rw-rw-  2.0 fat    16416 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/polygon.py
+-rw-rw-rw-  2.0 fat    40087 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/polyline.py
+-rw-rw-rw-  2.0 fat     4822 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/shape.py
+-rw-rw-rw-  2.0 fat    10443 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/solid.py
+-rw-rw-rw-  2.0 fat    24085 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/spline.py
+-rw-rw-rw-  2.0 fat     8246 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/subentity.py
+-rw-rw-rw-  2.0 fat     5196 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/sun.py
+-rw-rw-rw-  2.0 fat     2449 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/table.py
+-rw-rw-rw-  2.0 fat    17602 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/text.py
+-rw-rw-rw-  2.0 fat     9035 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/textstyle.py
+-rw-rw-rw-  2.0 fat     3597 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/tolerance.py
+-rw-rw-rw-  2.0 fat     2703 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/ucs.py
+-rw-rw-rw-  2.0 fat    14366 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/underlay.py
+-rw-rw-rw-  2.0 fat     6040 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/view.py
+-rw-rw-rw-  2.0 fat    27893 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/viewport.py
+-rw-rw-rw-  2.0 fat     7867 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/visualstyle.py
+-rw-rw-rw-  2.0 fat     9970 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/vport.py
+-rw-rw-rw-  2.0 fat    17024 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/xdata.py
+-rw-rw-rw-  2.0 fat     8495 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/xdict.py
+-rw-rw-rw-  2.0 fat     3062 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/xline.py
+-rw-rw-rw-  2.0 fat     3127 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/entities/__init__.py
+-rw-rw-rw-  2.0 fat    22867 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/fonts/fonts.py
+-rw-rw-rw-  2.0 fat     2242 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/fonts/font_face.py
+-rw-rw-rw-  2.0 fat    15227 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/fonts/font_manager.py
+-rw-rw-rw-  2.0 fat     1702 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/fonts/font_measurements.py
+-rw-rw-rw-  2.0 fat      825 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/fonts/glyphs.py
+-rw-rw-rw-  2.0 fat    10794 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/fonts/lff.py
+-rw-rw-rw-  2.0 fat    35217 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/fonts/shapefile.py
+-rw-rw-rw-  2.0 fat     7086 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/fonts/ttfonts.py
+-rw-rw-rw-  2.0 fat       64 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/fonts/__init__.py
+-rw-rw-rw-  2.0 fat    16696 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/layouts/base.py
+-rw-rw-rw-  2.0 fat     4343 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/layouts/blocklayout.py
+-rw-rw-rw-  2.0 fat    29014 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/layouts/layout.py
+-rw-rw-rw-  2.0 fat    15314 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/layouts/layouts.py
+-rw-rw-rw-  2.0 fat      232 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/layouts/__init__.py
+-rw-rw-rw-  2.0 fat     8327 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/lldxf/attributes.py
+-rw-rw-rw-  2.0 fat    16500 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/lldxf/const.py
+-rw-rw-rw-  2.0 fat     1614 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/lldxf/encoding.py
+-rw-rw-rw-  2.0 fat    17013 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/lldxf/extendedtags.py
+-rw-rw-rw-  2.0 fat     5363 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/lldxf/fileindex.py
+-rw-rw-rw-  2.0 fat      727 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/lldxf/hdrvars.py
+-rw-rw-rw-  2.0 fat     5469 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/lldxf/loader.py
+-rw-rw-rw-  2.0 fat     7447 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/lldxf/packedtags.py
+-rw-rw-rw-  2.0 fat     6355 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/lldxf/repair.py
+-rw-rw-rw-  2.0 fat    13058 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/lldxf/tagger.py
+-rw-rw-rw-  2.0 fat    14336 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/lldxf/tags.py
+-rw-rw-rw-  2.0 fat     8952 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/lldxf/tagwriter.py
+-rw-rw-rw-  2.0 fat    12064 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/lldxf/types.py
+-rw-rw-rw-  2.0 fat    17069 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/lldxf/validator.py
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/lldxf/__init__.py
+-rw-rw-rw-  2.0 fat    19193 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/arc.py
+-rw-rw-rw-  2.0 fat    16270 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/bbox.py
+-rw-rw-rw-  2.0 fat     9318 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/bezier.py
+-rw-rw-rw-  2.0 fat     2452 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/bezier_interpolation.py
+-rw-rw-rw-  2.0 fat     8730 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/box.py
+-rw-rw-rw-  2.0 fat    52916 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/bspline.py
+-rw-rw-rw-  2.0 fat     5608 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/bulge.py
+-rw-rw-rw-  2.0 fat     9002 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/circle.py
+-rw-rw-rw-  2.0 fat    24003 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/clipping.py
+-rw-rw-rw-  2.0 fat     4319 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/clustering.py
+-rw-rw-rw-  2.0 fat    12236 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/construct2d.py
+-rw-rw-rw-  2.0 fat    26265 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/construct3d.py
+-rw-rw-rw-  2.0 fat     1283 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/cspline.py
+-rw-rw-rw-  2.0 fat     9114 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/curvetools.py
+-rw-rw-rw-  2.0 fat    22048 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/ellipse.py
+-rw-rw-rw-  2.0 fat     4406 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/eulerspiral.py
+-rw-rw-rw-  2.0 fat    38883 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/linalg.py
+-rw-rw-rw-  2.0 fat    10231 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/line.py
+-rw-rw-rw-  2.0 fat     3053 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/offset2d.py
+-rw-rw-rw-  2.0 fat     8256 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/parametrize.py
+-rw-rw-rw-  2.0 fat    15602 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/perlin.py
+-rw-rw-rw-  2.0 fat    15921 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/polyline.py
+-rw-rw-rw-  2.0 fat    11867 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/rtree.py
+-rw-rw-rw-  2.0 fat     3910 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/shape.py
+-rw-rw-rw-  2.0 fat     2568 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/surfaces.py
+-rw-rw-rw-  2.0 fat    12155 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/transformtools.py
+-rw-rw-rw-  2.0 fat     3631 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/triangulation.py
+-rw-rw-rw-  2.0 fat    16971 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/ucs.py
+-rw-rw-rw-  2.0 fat     7213 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/_bezier3p.py
+-rw-rw-rw-  2.0 fat    12967 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/_bezier4p.py
+-rw-rw-rw-  2.0 fat     9440 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/_bspline.py
+-rw-rw-rw-  2.0 fat     7272 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/_construct.py
+-rw-rw-rw-  2.0 fat     2261 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/_ctypes.py
+-rw-rw-rw-  2.0 fat    24954 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/_mapbox_earcut.py
+-rw-rw-rw-  2.0 fat    27606 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/_matrix44.py
+-rw-rw-rw-  2.0 fat    25912 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/_vector.py
+-rw-rw-rw-  2.0 fat     2003 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/math/__init__.py
+-rw-rw-rw-  2.0 fat     1306 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/path/commands.py
+-rw-rw-rw-  2.0 fat    39194 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/path/converter.py
+-rw-rw-rw-  2.0 fat     6748 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/path/nesting.py
+-rw-rw-rw-  2.0 fat    20453 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/path/path.py
+-rw-rw-rw-  2.0 fat    10140 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/path/shapes.py
+-rw-rw-rw-  2.0 fat    34692 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/path/tools.py
+-rw-rw-rw-  2.0 fat      385 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/path/__init__.py
+-rw-rw-rw-  2.0 fat     2987 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/pp/dxfpp.css
+-rw-rw-rw-  2.0 fat     1148 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/pp/dxfpp.html
+-rw-rw-rw-  2.0 fat    11304 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/pp/dxfpp.js
+-rw-rw-rw-  2.0 fat    17144 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/pp/dxfpp.py
+-rw-rw-rw-  2.0 fat     3770 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/pp/pprint.py
+-rw-rw-rw-  2.0 fat      812 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/pp/rawpp.css
+-rw-rw-rw-  2.0 fat      316 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/pp/rawpp.html
+-rw-rw-rw-  2.0 fat     2545 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/pp/rawpp.py
+-rw-rw-rw-  2.0 fat     6896 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/pp/reflinks.py
+-rw-rw-rw-  2.0 fat      123 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/pp/__init__.py
+-rw-rw-rw-  2.0 fat    10039 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/abstract_mtext_renderer.py
+-rw-rw-rw-  2.0 fat    20495 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/arrows.py
+-rw-rw-rw-  2.0 fat    17749 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/curves.py
+-rw-rw-rw-  2.0 fat     4041 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/dimension.py
+-rw-rw-rw-  2.0 fat    52028 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/dim_base.py
+-rw-rw-rw-  2.0 fat    35702 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/dim_curved.py
+-rw-rw-rw-  2.0 fat     6894 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/dim_diameter.py
+-rw-rw-rw-  2.0 fat    24751 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/dim_linear.py
+-rw-rw-rw-  2.0 fat     8084 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/dim_ordinate.py
+-rw-rw-rw-  2.0 fat    20295 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/dim_radius.py
+-rw-rw-rw-  2.0 fat    47170 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/forms.py
+-rw-rw-rw-  2.0 fat    24213 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/hatching.py
+-rw-rw-rw-  2.0 fat     4728 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/leader.py
+-rw-rw-rw-  2.0 fat      664 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/linetypes.py
+-rw-rw-rw-  2.0 fat    64121 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/mesh.py
+-rw-rw-rw-  2.0 fat    60923 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/mleader.py
+-rw-rw-rw-  2.0 fat     8437 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/mline.py
+-rw-rw-rw-  2.0 fat     2964 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/point.py
+-rw-rw-rw-  2.0 fat     8736 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/polyline.py
+-rw-rw-rw-  2.0 fat     7886 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/r12spline.py
+-rw-rw-rw-  2.0 fat    22541 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/trace.py
+-rw-rw-rw-  2.0 fat     2881 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/_linetypes.py
+-rw-rw-rw-  2.0 fat      778 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/render/__init__.py
+-rw-rw-rw-  2.0 fat     1050 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/resources/16x16.png
+-rw-rw-rw-  2.0 fat     1420 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/resources/24x24.png
+-rw-rw-rw-  2.0 fat    10638 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/resources/256x256.png
+-rw-rw-rw-  2.0 fat     1758 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/resources/32x32.png
+-rw-rw-rw-  2.0 fat     2335 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/resources/48x48.png
+-rw-rw-rw-  2.0 fat     3050 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/resources/64x64.png
+-rw-rw-rw-  2.0 fat     2090 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/resources/icon-copy-64px.png
+-rw-rw-rw-  2.0 fat     3109 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/resources/icon-find-64px.png
+-rw-rw-rw-  2.0 fat     2388 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/resources/icon-goto-bookmark-64px.png
+-rw-rw-rw-  2.0 fat     2519 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/resources/icon-goto-handle-64px.png
+-rw-rw-rw-  2.0 fat     2409 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/resources/icon-goto-line-64px.png
+-rw-rw-rw-  2.0 fat     2231 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/resources/icon-left-arrow-64px.png
+-rw-rw-rw-  2.0 fat     2322 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/resources/icon-next-entity-64px.png
+-rw-rw-rw-  2.0 fat     2320 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/resources/icon-prev-entity-64px.png
+-rw-rw-rw-  2.0 fat     2244 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/resources/icon-right-arrow-64px.png
+-rw-rw-rw-  2.0 fat     2553 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/resources/icon-show-in-tree-64px.png
+-rw-rw-rw-  2.0 fat     2373 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/resources/icon-store-bookmark-64px.png
+-rw-rw-rw-  2.0 fat    10650 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/sections/acdsdata.py
+-rw-rw-rw-  2.0 fat    16508 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/sections/blocks.py
+-rw-rw-rw-  2.0 fat    11639 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/sections/classes.py
+-rw-rw-rw-  2.0 fat     4137 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/sections/entities.py
+-rw-rw-rw-  2.0 fat    11953 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/sections/header.py
+-rw-rw-rw-  2.0 fat    60696 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/sections/headervars.py
+-rw-rw-rw-  2.0 fat    27009 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/sections/objects.py
+-rw-rw-rw-  2.0 fat    26581 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/sections/table.py
+-rw-rw-rw-  2.0 fat     5270 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/sections/tables.py
+-rw-rw-rw-  2.0 fat       67 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/sections/__init__.py
+-rw-rw-rw-  2.0 fat    19711 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/analyze.py
+-rw-rw-rw-  2.0 fat    20434 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/binarydata.py
+-rw-rw-rw-  2.0 fat     2931 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/codepage.py
+-rw-rw-rw-  2.0 fat     7645 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/complex_ltype.py
+-rw-rw-rw-  2.0 fat     1782 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/crypt.py
+-rw-rw-rw-  2.0 fat     1511 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/debug.py
+-rw-rw-rw-  2.0 fat     2341 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/difftags.py
+-rw-rw-rw-  2.0 fat     1235 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/handle.py
+-rw-rw-rw-  2.0 fat      780 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/indexing.py
+-rw-rw-rw-  2.0 fat     2145 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/juliandate.py
+-rw-rw-rw-  2.0 fat     6166 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/pattern.py
+-rw-rw-rw-  2.0 fat     1256 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/rawloader.py
+-rw-rw-rw-  2.0 fat   129174 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/standards.py
+-rw-rw-rw-  2.0 fat     6049 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/strip.py
+-rw-rw-rw-  2.0 fat     1466 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/test.py
+-rw-rw-rw-  2.0 fat    65518 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/text.py
+-rw-rw-rw-  2.0 fat    54234 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/text_layout.py
+-rw-rw-rw-  2.0 fat     6893 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/text_size.py
+-rw-rw-rw-  2.0 fat     3077 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/zipmanager.py
+-rw-rw-rw-  2.0 fat   142734 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/_iso_pattern.py
+-rw-rw-rw-  2.0 fat     3564 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/src/ezdxf/tools/__init__.py
+-rw-rw-rw-  2.0 fat        1 b- defN 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf.egg-info/dependency_links.txt
+-rw-rw-rw-  2.0 fat       47 b- defN 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf.egg-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf.egg-info/not-zip-safe
+-rw-rw-rw-  2.0 fat    69206 b- defN 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf.egg-info/PKG-INFO
+-rw-rw-rw-  2.0 fat      302 b- defN 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf.egg-info/requires.txt
+-rw-rw-rw-  2.0 fat    31430 b- defN 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf.egg-info/SOURCES.txt
+-rw-rw-rw-  2.0 fat        6 b- defN 23-May-06 04:16 ezdxf-1.1.0b1/src/ezdxf.egg-info/top_level.txt
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/tests/test_01_dxf_entities/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/tests/test_03_dxf_layouts/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/tests/test_05_tools/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/tests/test_06_math/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/tests/test_07_render/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/tests/test_08_addons/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/tests/test_09_cython_acceleration/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-06 04:16 ezdxf-1.1.0b1/tests/test_10_issues/
+-rw-rw-rw-  2.0 fat      410 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/conftest.py
+-rw-rw-rw-  2.0 fat     2336 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
+-rw-rw-rw-  2.0 fat      780 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
+-rw-rw-rw-  2.0 fat     2599 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
+-rw-rw-rw-  2.0 fat     1124 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
+-rw-rw-rw-  2.0 fat     5456 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
+-rw-rw-rw-  2.0 fat      582 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_010_binary_data.py
+-rw-rw-rw-  2.0 fat      473 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_011_codepage.py
+-rw-rw-rw-  2.0 fat    11593 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_012_crypt.py
+-rw-rw-rw-  2.0 fat     1191 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_013_juliandate.py
+-rw-rw-rw-  2.0 fat     1033 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py
+-rw-rw-rw-  2.0 fat     4792 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py
+-rw-rw-rw-  2.0 fat      989 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_016_encoding.py
+-rw-rw-rw-  2.0 fat     1383 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_018_handle.py
+-rw-rw-rw-  2.0 fat     5518 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py
+-rw-rw-rw-  2.0 fat     8168 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py
+-rw-rw-rw-  2.0 fat     3787 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py
+-rw-rw-rw-  2.0 fat      401 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_022_set_flag_state.py
+-rw-rw-rw-  2.0 fat      539 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py
+-rw-rw-rw-  2.0 fat     2092 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_024_render_tag.py
+-rw-rw-rw-  2.0 fat    10917 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_040_tags.py
+-rw-rw-rw-  2.0 fat     3073 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_041_group_tags.py
+-rw-rw-rw-  2.0 fat     6419 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py
+-rw-rw-rw-  2.0 fat     1632 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py
+-rw-rw-rw-  2.0 fat    11265 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py
+-rw-rw-rw-  2.0 fat     3363 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py
+-rw-rw-rw-  2.0 fat     1974 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py
+-rw-rw-rw-  2.0 fat     2321 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py
+-rw-rw-rw-  2.0 fat      568 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py
+-rw-rw-rw-  2.0 fat     8682 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py
+-rw-rw-rw-  2.0 fat     1051 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py
+-rw-rw-rw-  2.0 fat     1500 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py
+-rw-rw-rw-  2.0 fat    11689 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_101_dxfnamespace.py
+-rw-rw-rw-  2.0 fat     2893 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_102_appdata.py
+-rw-rw-rw-  2.0 fat     2312 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_103_reactors.py
+-rw-rw-rw-  2.0 fat     4001 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_104_extension_dict.py
+-rw-rw-rw-  2.0 fat    20860 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_105_xdata.py
+-rw-rw-rw-  2.0 fat    14169 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_110_dxfentity.py
+-rw-rw-rw-  2.0 fat     2433 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py
+-rw-rw-rw-  2.0 fat     6781 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_112a_dxfgfx.py
+-rw-rw-rw-  2.0 fat      695 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_112b_dxfobj.py
+-rw-rw-rw-  2.0 fat     2431 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_113_dxfclass.py
+-rw-rw-rw-  2.0 fat     4044 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_114_factory.py
+-rw-rw-rw-  2.0 fat     2256 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_115_new_empty_drawing.py
+-rw-rw-rw-  2.0 fat    15794 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_116_dictionary.py
+-rw-rw-rw-  2.0 fat     4999 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_117_layer_table_entry.py
+-rw-rw-rw-  2.0 fat      385 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_118_appid_table_entry.py
+-rw-rw-rw-  2.0 fat     1058 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_119_ucs_table_entry.py
+-rw-rw-rw-  2.0 fat     3003 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_120_style_table_entry.py
+-rw-rw-rw-  2.0 fat     2943 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_121_ltype_table_entry.py
+-rw-rw-rw-  2.0 fat      379 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_122_vport_table_entry.py
+-rw-rw-rw-  2.0 fat     1113 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_123_view_table_entry.py
+-rw-rw-rw-  2.0 fat     8757 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py
+-rw-rw-rw-  2.0 fat     1698 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_125_image_def.py
+-rw-rw-rw-  2.0 fat     1312 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_126_image_def_reactor.py
+-rw-rw-rw-  2.0 fat     1430 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_127_raster_variables.py
+-rw-rw-rw-  2.0 fat     1540 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_128_pdf_definition.py
+-rw-rw-rw-  2.0 fat     2778 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_129_xrecord.py
+-rw-rw-rw-  2.0 fat     2423 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_130_id_buffer.py
+-rw-rw-rw-  2.0 fat     2470 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_131_field_list.py
+-rw-rw-rw-  2.0 fat     2435 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_132_layer_filter.py
+-rw-rw-rw-  2.0 fat     2153 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_133_sun.py
+-rw-rw-rw-  2.0 fat      852 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_134_material.py
+-rw-rw-rw-  2.0 fat    11497 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_135_geo_data.py
+-rw-rw-rw-  2.0 fat     1087 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_136_vba_project.py
+-rw-rw-rw-  2.0 fat     3099 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_137_sortentstable.py
+-rw-rw-rw-  2.0 fat      704 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_138_setup_visual_styles.py
+-rw-rw-rw-  2.0 fat     7570 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_139_user_record.py
+-rw-rw-rw-  2.0 fat      714 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_140_block_record.py
+-rw-rw-rw-  2.0 fat     9153 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_141_layer_vp_override.py
+-rw-rw-rw-  2.0 fat     2231 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/conftest.py
+-rw-rw-rw-  2.0 fat     6532 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_200_line.py
+-rw-rw-rw-  2.0 fat     4273 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_201_point.py
+-rw-rw-rw-  2.0 fat     6827 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_202_circle.py
+-rw-rw-rw-  2.0 fat     8949 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_203_arc.py
+-rw-rw-rw-  2.0 fat     2852 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_204_shape.py
+-rw-rw-rw-  2.0 fat     8242 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_205_solid.py
+-rw-rw-rw-  2.0 fat     8476 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_206_text.py
+-rw-rw-rw-  2.0 fat     4947 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_207_attdef.py
+-rw-rw-rw-  2.0 fat     6312 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_208_attrib.py
+-rw-rw-rw-  2.0 fat     2671 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_209_vertex.py
+-rw-rw-rw-  2.0 fat     5930 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_210_polyline_1.py
+-rw-rw-rw-  2.0 fat    13489 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_210_polyline_2.py
+-rw-rw-rw-  2.0 fat     6650 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_210_polyline_explode.py
+-rw-rw-rw-  2.0 fat     1780 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py
+-rw-rw-rw-  2.0 fat     7847 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_211_viewport.py
+-rw-rw-rw-  2.0 fat    12629 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_212_insert.py
+-rw-rw-rw-  2.0 fat     6024 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_213_minsert.py
+-rw-rw-rw-  2.0 fat     3284 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_214_block.py
+-rw-rw-rw-  2.0 fat     6882 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_215_dimension.py
+-rw-rw-rw-  2.0 fat     4907 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_216_dimlines_R12.py
+-rw-rw-rw-  2.0 fat    13186 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py
+-rw-rw-rw-  2.0 fat     6471 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py
+-rw-rw-rw-  2.0 fat     5535 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py
+-rw-rw-rw-  2.0 fat     3056 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py
+-rw-rw-rw-  2.0 fat     7181 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py
+-rw-rw-rw-  2.0 fat     2066 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py
+-rw-rw-rw-  2.0 fat     3615 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py
+-rw-rw-rw-  2.0 fat     6919 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_221_ellipse.py
+-rw-rw-rw-  2.0 fat     2223 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_222_xline.py
+-rw-rw-rw-  2.0 fat     1493 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_223_ray.py
+-rw-rw-rw-  2.0 fat     2176 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_224_group.py
+-rw-rw-rw-  2.0 fat    10917 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_225_mtext.py
+-rw-rw-rw-  2.0 fat    12020 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_226_spline.py
+-rw-rw-rw-  2.0 fat     5529 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py
+-rw-rw-rw-  2.0 fat    10893 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py
+-rw-rw-rw-  2.0 fat    15116 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_228_mesh.py
+-rw-rw-rw-  2.0 fat     2695 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py
+-rw-rw-rw-  2.0 fat    21421 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_229b_hatch_extended.py
+-rw-rw-rw-  2.0 fat     6587 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py
+-rw-rw-rw-  2.0 fat     3140 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py
+-rw-rw-rw-  2.0 fat    12486 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py
+-rw-rw-rw-  2.0 fat     2274 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_231_underlay.py
+-rw-rw-rw-  2.0 fat     5243 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_231_underlay_2.py
+-rw-rw-rw-  2.0 fat     2294 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_232_acis.py
+-rw-rw-rw-  2.0 fat     6799 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_232_acis_2.py
+-rw-rw-rw-  2.0 fat     1854 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_232_surface.py
+-rw-rw-rw-  2.0 fat     2695 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_233_helix.py
+-rw-rw-rw-  2.0 fat     2040 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_234_light.py
+-rw-rw-rw-  2.0 fat     3806 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_235_leader.py
+-rw-rw-rw-  2.0 fat    20392 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_236_multileader.py
+-rw-rw-rw-  2.0 fat    10992 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_237_mline.py
+-rw-rw-rw-  2.0 fat     2356 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_238_tolerance.py
+-rw-rw-rw-  2.0 fat    27392 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_239_proxy_graphic.py
+-rw-rw-rw-  2.0 fat     4347 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_240_arc_dimension.py
+-rw-rw-rw-  2.0 fat     1069 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_241_hyperlink.py
+-rw-rw-rw-  2.0 fat    11313 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_242_random_transform.py
+-rw-rw-rw-  2.0 fat     3725 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_243_replace_entity.py
+-rw-rw-rw-  2.0 fat     1445 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py
+-rw-rw-rw-  2.0 fat     4456 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_245_wipeout.py
+-rw-rw-rw-  2.0 fat     6175 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_246_spline_audit.py
+-rw-rw-rw-  2.0 fat     8165 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py
+-rw-rw-rw-  2.0 fat     6003 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_248_mpolygon.py
+-rw-rw-rw-  2.0 fat    13682 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py
+-rw-rw-rw-  2.0 fat     5713 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_249_boundary_paths.py
+-rw-rw-rw-  2.0 fat     8331 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py
+-rw-rw-rw-  2.0 fat     7331 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_251_upright.py
+-rw-rw-rw-  2.0 fat     4795 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py
+-rw-rw-rw-  2.0 fat     2082 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_253_ole2frame.py
+-rw-rw-rw-  2.0 fat      821 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_254_get_font_name.py
+-rw-rw-rw-  2.0 fat     5149 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_300_layout.py
+-rw-rw-rw-  2.0 fat     4274 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py
+-rw-rw-rw-  2.0 fat     5582 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_302_block_references.py
+-rw-rw-rw-  2.0 fat     2695 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_303_auto_block_references.py
+-rw-rw-rw-  2.0 fat      913 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_304_new_entity_space.py
+-rw-rw-rw-  2.0 fat     3279 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py
+-rw-rw-rw-  2.0 fat     2609 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py
+-rw-rw-rw-  2.0 fat     2343 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_307_groupby.py
+-rw-rw-rw-  2.0 fat    17748 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_308_query.py
+-rw-rw-rw-  2.0 fat     6382 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_309_query_parser.py
+-rw-rw-rw-  2.0 fat     5031 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py
+-rw-rw-rw-  2.0 fat     5782 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_312_virtual_layout.py
+-rw-rw-rw-  2.0 fat      647 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_313_redraw_order.py
+-rw-rw-rw-  2.0 fat     6128 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_401_headersection.py
+-rw-rw-rw-  2.0 fat     2750 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_402_classessection.py
+-rw-rw-rw-  2.0 fat     5208 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_403_entity_database.py
+-rw-rw-rw-  2.0 fat     6795 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_404a_tables.py
+-rw-rw-rw-  2.0 fat     4981 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py
+-rw-rw-rw-  2.0 fat     2450 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_405_classes.py
+-rw-rw-rw-  2.0 fat     9094 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py
+-rw-rw-rw-  2.0 fat      848 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_407_entity_section.py
+-rw-rw-rw-  2.0 fat     3375 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_408_objects_section.py
+-rw-rw-rw-  2.0 fat     1433 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_409_create_objects.py
+-rw-rw-rw-  2.0 fat     5736 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_410_table.py
+-rw-rw-rw-  2.0 fat     6607 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_411_acds_data.py
+-rw-rw-rw-  2.0 fat     1058 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py
+-rw-rw-rw-  2.0 fat     2246 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py
+-rw-rw-rw-  2.0 fat    18072 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py
+-rw-rw-rw-  2.0 fat     4638 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_415_layout_management.py
+-rw-rw-rw-  2.0 fat    12327 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py
+-rw-rw-rw-  2.0 fat     6509 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py
+-rw-rw-rw-  2.0 fat     5656 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_417_bbox.py
+-rw-rw-rw-  2.0 fat     5434 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py
+-rw-rw-rw-  2.0 fat      733 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py
+-rw-rw-rw-  2.0 fat     1240 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py
+-rw-rw-rw-  2.0 fat     5007 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py
+-rw-rw-rw-  2.0 fat      769 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py
+-rw-rw-rw-  2.0 fat     7289 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_424_audit.py
+-rw-rw-rw-  2.0 fat     3737 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py
+-rw-rw-rw-  2.0 fat     2981 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py
+-rw-rw-rw-  2.0 fat     2416 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_427_appsettings.py
+-rw-rw-rw-  2.0 fat     2533 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py
+-rw-rw-rw-  2.0 fat   112800 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/conftest.py
+-rw-rw-rw-  2.0 fat     5510 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_500_units.py
+-rw-rw-rw-  2.0 fat     1052 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_501_truecolor.py
+-rw-rw-rw-  2.0 fat     1021 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_502_raw_color.py
+-rw-rw-rw-  2.0 fat     1695 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_503_indexing.py
+-rw-rw-rw-  2.0 fat     1442 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_504_suppress_zeros.py
+-rw-rw-rw-  2.0 fat      216 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_506_version.py
+-rw-rw-rw-  2.0 fat      579 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_507_dxf_pretty_printer.py
+-rw-rw-rw-  2.0 fat      657 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_508_read_zip.py
+-rw-rw-rw-  2.0 fat     1445 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_509_comments.py
+-rw-rw-rw-  2.0 fat     1185 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_510_byte_stream.py
+-rw-rw-rw-  2.0 fat     4239 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_511_bit_stream.py
+-rw-rw-rw-  2.0 fat     5595 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_512_pattern.py
+-rw-rw-rw-  2.0 fat     2372 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_513_reorder_entities.py
+-rw-rw-rw-  2.0 fat    17710 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_514_text.py
+-rw-rw-rw-  2.0 fat     9269 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_515a_fonts_truetype.py
+-rw-rw-rw-  2.0 fat     4729 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_515b_fonts_shapefiles.py
+-rw-rw-rw-  2.0 fat     2225 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_515c_fonts_lff.py
+-rw-rw-rw-  2.0 fat     4002 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_516_zoom.py
+-rw-rw-rw-  2.0 fat    34209 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_517_text_layout.py
+-rw-rw-rw-  2.0 fat      474 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_518_header_guid.py
+-rw-rw-rw-  2.0 fat     3716 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_519_mtext_editor.py
+-rw-rw-rw-  2.0 fat     3205 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_520_mtext_context.py
+-rw-rw-rw-  2.0 fat    24496 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_521_mtext_parser.py
+-rw-rw-rw-  2.0 fat     3863 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_522_text_scanner.py
+-rw-rw-rw-  2.0 fat     5207 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_523_text_size.py
+-rw-rw-rw-  2.0 fat     5063 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_524_block_reference_manager.py
+-rw-rw-rw-  2.0 fat      773 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_525_transparency.py
+-rw-rw-rw-  2.0 fat     2133 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_526_explode.py
+-rw-rw-rw-  2.0 fat    13521 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_527_gfxattribs.py
+-rw-rw-rw-  2.0 fat     2748 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_528_difftags.py
+-rw-rw-rw-  2.0 fat     6700 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_529_acis_sat.py
+-rw-rw-rw-  2.0 fat     2062 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_530_acis_sab.py
+-rw-rw-rw-  2.0 fat    12366 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_531_acis_entities.py
+-rw-rw-rw-  2.0 fat     7533 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_532_acis_mesh.py
+-rw-rw-rw-  2.0 fat    43206 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_533_shapefiles.py
+-rw-rw-rw-  2.0 fat     1034 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_534_dwg_info.py
+-rw-rw-rw-  2.0 fat    47915 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_535_xref_basic.py
+-rw-rw-rw-  2.0 fat    27614 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_536_xref_conflict.py
+-rw-rw-rw-  2.0 fat     6887 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_537_transform.py
+-rw-rw-rw-  2.0 fat     2246 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_538_scale_mtext_inline_commands.py
+-rw-rw-rw-  2.0 fat     3159 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_539_npshapes.py
+-rw-rw-rw-  2.0 fat     2605 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_05_tools/test_540_lff_parser.py
+-rw-rw-rw-  2.0 fat     4026 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/conftest.py
+-rw-rw-rw-  2.0 fat     7460 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_600_base.py
+-rw-rw-rw-  2.0 fat     2098 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_601_bulge.py
+-rw-rw-rw-  2.0 fat    14651 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_602_vec3.py
+-rw-rw-rw-  2.0 fat     8956 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_603_vec2.py
+-rw-rw-rw-  2.0 fat     2801 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_604_banded_matrix.py
+-rw-rw-rw-  2.0 fat     9738 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_604_linalg.py
+-rw-rw-rw-  2.0 fat    13943 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_605_matrix44.py
+-rw-rw-rw-  2.0 fat     5888 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_606_convexhull.py
+-rw-rw-rw-  2.0 fat     1010 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_607_perlin_noise.py
+-rw-rw-rw-  2.0 fat     3833 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_608_intersection_line_line_2d.py
+-rw-rw-rw-  2.0 fat     1676 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_609_point_on_line.py
+-rw-rw-rw-  2.0 fat     3171 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_610_ocs.py
+-rw-rw-rw-  2.0 fat     7529 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_611_ucs.py
+-rw-rw-rw-  2.0 fat     1831 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_612_ucs_pass_trough.py
+-rw-rw-rw-  2.0 fat     2586 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_613_point_in_poygon.py
+-rw-rw-rw-  2.0 fat    10913 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_614_construct_3d.py
+-rw-rw-rw-  2.0 fat      602 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_615_rytz_axis.py
+-rw-rw-rw-  2.0 fat     5215 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_616_plane.py
+-rw-rw-rw-  2.0 fat      772 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_617_clockwise_orientation.py
+-rw-rw-rw-  2.0 fat     6384 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_618_clipping.py
+-rw-rw-rw-  2.0 fat    10108 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_619_greiner_hormann.py
+-rw-rw-rw-  2.0 fat     2669 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_620_knot.py
+-rw-rw-rw-  2.0 fat    18821 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_621_bspline.py
+-rw-rw-rw-  2.0 fat     7652 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_622_bsplineu.py
+-rw-rw-rw-  2.0 fat    11327 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_623_rbspline.py
+-rw-rw-rw-  2.0 fat    10809 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_624_global_bspline_interpolation.py
+-rw-rw-rw-  2.0 fat     1247 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_626_local_bspline_interpolation.py
+-rw-rw-rw-  2.0 fat     1967 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_627_bspline_basis.py
+-rw-rw-rw-  2.0 fat    10545 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_629_bezier.py
+-rw-rw-rw-  2.0 fat    10714 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_630a_bezier4p_base.py
+-rw-rw-rw-  2.0 fat    10204 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_630b_bezier4p_functions.py
+-rw-rw-rw-  2.0 fat     1683 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_631_euler_spiral.py
+-rw-rw-rw-  2.0 fat     4021 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_632_bezier3p.py
+-rw-rw-rw-  2.0 fat    19463 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_640_bbox.py
+-rw-rw-rw-  2.0 fat     5393 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_641_construction_ray.py
+-rw-rw-rw-  2.0 fat     3673 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_642_construction_line.py
+-rw-rw-rw-  2.0 fat     9459 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_643_construction_box.py
+-rw-rw-rw-  2.0 fat    10941 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_644_construction_circle.py
+-rw-rw-rw-  2.0 fat    10988 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_645_construction_arc.py
+-rw-rw-rw-  2.0 fat     3422 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_646_offset_vertices_2d.py
+-rw-rw-rw-  2.0 fat     7672 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_647_transform_tools.py
+-rw-rw-rw-  2.0 fat     8993 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_648_construction_ellipse.py
+-rw-rw-rw-  2.0 fat     4243 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_650_elliptic_arc_span.py
+-rw-rw-rw-  2.0 fat     9011 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_651_construction_polyline.py
+-rw-rw-rw-  2.0 fat     3168 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_652_approx_param_t.py
+-rw-rw-rw-  2.0 fat     5806 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_653_polyline_intersection.py
+-rw-rw-rw-  2.0 fat     5193 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_654_rtree.py
+-rw-rw-rw-  2.0 fat      788 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_655_dbscan.py
+-rw-rw-rw-  2.0 fat      834 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_656_k_means.py
+-rw-rw-rw-  2.0 fat     4654 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_657_mapbox_earcut.py
+-rw-rw-rw-  2.0 fat    11628 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_658_bevel_tools.py
+-rw-rw-rw-  2.0 fat     1875 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_659_intersection_line_polygon_3d.py
+-rw-rw-rw-  2.0 fat     1428 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_660_intersection_ray_polygon_3d.py
+-rw-rw-rw-  2.0 fat     1741 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py
+-rw-rw-rw-  2.0 fat     3307 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_06_math/test_662_is_convex_polygon_2d.py
+-rw-rw-rw-  2.0 fat     1466 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_07_render/test_701_arrows.py
+-rw-rw-rw-  2.0 fat    17245 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_07_render/test_702_render_forms.py
+-rw-rw-rw-  2.0 fat    34220 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_07_render/test_703_mesh_builder.py
+-rw-rw-rw-  2.0 fat     3852 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_07_render/test_704_render_linear_dimension.py
+-rw-rw-rw-  2.0 fat     1345 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_07_render/test_705_shape.py
+-rw-rw-rw-  2.0 fat      483 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_07_render/test_706_random_path.py
+-rw-rw-rw-  2.0 fat     5603 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_07_render/test_707_trace.py
+-rw-rw-rw-  2.0 fat    33834 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_07_render/test_708a_path.py
+-rw-rw-rw-  2.0 fat    27351 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_07_render/test_708b_path_tools.py
+-rw-rw-rw-  2.0 fat     3633 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_07_render/test_708c_matplotlib_path_tools.py
+-rw-rw-rw-  2.0 fat     3099 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_07_render/test_708d_qpainter_path_tools.py
+-rw-rw-rw-  2.0 fat     4589 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_07_render/test_708e_path_shapes.py
+-rw-rw-rw-  2.0 fat     4118 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_07_render/test_708f_path_nesting.py
+-rw-rw-rw-  2.0 fat     1308 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_07_render/test_709_linetype_renderer.py
+-rw-rw-rw-  2.0 fat     2815 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_07_render/test_711_points.py
+-rw-rw-rw-  2.0 fat     6594 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_07_render/test_712_render_curved_dimension.py
+-rw-rw-rw-  2.0 fat     1472 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_07_render/test_713_mleader_builder.py
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_07_render/test_714_mleader_render_engine.py
+-rw-rw-rw-  2.0 fat    11778 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_07_render/test_715_hatching.py
+-rw-rw-rw-  2.0 fat     2626 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_07_render/test_715_issue_747_explode_3d_dim.py
+-rw-rw-rw-  2.0 fat     4771 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_800_mtext_surrogate.py
+-rw-rw-rw-  2.0 fat     1352 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_801_r12spline.py
+-rw-rw-rw-  2.0 fat     7881 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_802_table_painter.py
+-rw-rw-rw-  2.0 fat    12386 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_803_entities_to_code.py
+-rw-rw-rw-  2.0 fat     6844 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_804_importer.py
+-rw-rw-rw-  2.0 fat     2362 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_805_pycsg.py
+-rw-rw-rw-  2.0 fat    15467 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_806_acadctb.py
+-rw-rw-rw-  2.0 fat     4860 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_807_dwg_loader_basics.py
+-rw-rw-rw-  2.0 fat    10862 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_810_drawing_properties.py
+-rw-rw-rw-  2.0 fat    11353 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_811a_drawing_frontend.py
+-rw-rw-rw-  2.0 fat     2619 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_811b_drawing_recorder.py
+-rw-rw-rw-  2.0 fat     4157 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_812_drawing_graphic_proxy.py
+-rw-rw-rw-  2.0 fat    12547 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_813_geo_interface.py
+-rw-rw-rw-  2.0 fat    14853 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_814_text2path.py
+-rw-rw-rw-  2.0 fat    16239 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_815_dxf_browser.py
+-rw-rw-rw-  2.0 fat    11275 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_816_bin_packing.py
+-rw-rw-rw-  2.0 fat    12554 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_817_genetic_algorithm.py
+-rw-rw-rw-  2.0 fat     9008 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_818_meshex.py
+-rw-rw-rw-  2.0 fat     1003 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_819_menger_sponge.py
+-rw-rw-rw-  2.0 fat     4433 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_820_openscad.py
+-rw-rw-rw-  2.0 fat    15527 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_821_hpgl2.py
+-rw-rw-rw-  2.0 fat     1322 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
+-rw-rw-rw-  2.0 fat      976 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_08_addons/test_822_clipper.py
+-rw-rw-rw-  2.0 fat     2527 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_09_cython_acceleration/test_901_acc_vec2.py
+-rw-rw-rw-  2.0 fat     2199 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_09_cython_acceleration/test_902_acc_vec3.py
+-rw-rw-rw-  2.0 fat     2142 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_09_cython_acceleration/test_903_acc_matrix44.py
+-rw-rw-rw-  2.0 fat     3158 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
+-rw-rw-rw-  2.0 fat     1452 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
+-rw-rw-rw-  2.0 fat     4755 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_09_cython_acceleration/test_906_acc_bspline.py
+-rw-rw-rw-  2.0 fat     2656 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_10_issues/test_issue_414_bbox_calculation.py
+-rw-rw-rw-  2.0 fat     1213 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
+-rw-rw-rw-  2.0 fat     2268 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_10_issues/test_issue_574_flattening_error.py
+-rw-rw-rw-  2.0 fat     1754 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
+-rw-rw-rw-  2.0 fat      682 b- defN 23-May-06 04:15 ezdxf-1.1.0b1/tests/test_10_issues/test_issue_749_text_layout.py
+829 files, 8541096 bytes uncompressed, 1921652 bytes compressed:  77.5%
```

## zipnote {}

```diff
@@ -1,2458 +1,2488 @@
-Filename: ezdxf-1.1.0b0/
+Filename: ezdxf-1.1.0b1/
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/
+Filename: ezdxf-1.1.0b1/integration_tests/
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/
+Filename: ezdxf-1.1.0b1/src/
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/
+Filename: ezdxf-1.1.0b1/tests/
 Comment: 
 
-Filename: ezdxf-1.1.0b0/LICENSE
+Filename: ezdxf-1.1.0b1/LICENSE
 Comment: 
 
-Filename: ezdxf-1.1.0b0/MANIFEST.in
+Filename: ezdxf-1.1.0b1/MANIFEST.in
 Comment: 
 
-Filename: ezdxf-1.1.0b0/NEWS.md
+Filename: ezdxf-1.1.0b1/NEWS.md
 Comment: 
 
-Filename: ezdxf-1.1.0b0/PKG-INFO
+Filename: ezdxf-1.1.0b1/PKG-INFO
 Comment: 
 
-Filename: ezdxf-1.1.0b0/README.md
+Filename: ezdxf-1.1.0b1/README.md
 Comment: 
 
-Filename: ezdxf-1.1.0b0/requirements.txt
+Filename: ezdxf-1.1.0b1/requirements.txt
 Comment: 
 
-Filename: ezdxf-1.1.0b0/setup.cfg
+Filename: ezdxf-1.1.0b1/setup.cfg
 Comment: 
 
-Filename: ezdxf-1.1.0b0/setup.py
+Filename: ezdxf-1.1.0b1/setup.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/data/
+Filename: ezdxf-1.1.0b1/integration_tests/data/
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/check_disable_c_ext_by_config_file.py
+Filename: ezdxf-1.1.0b1/integration_tests/check_disable_c_ext_by_config_file.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/check_disable_c_ext_by_env_var.py
+Filename: ezdxf-1.1.0b1/integration_tests/check_disable_c_ext_by_env_var.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/conftest.py
+Filename: ezdxf-1.1.0b1/integration_tests/conftest.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_acad_table.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_acad_table.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_all_dimline_styles.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_all_dimline_styles.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_all_ellipse_transformations.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_all_ellipse_transformations.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_anonymous_blocks.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_anonymous_blocks.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_audit_critical_dxf_files.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_audit_critical_dxf_files.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_audit_layouts.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_audit_layouts.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_complex_line_type_2.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_complex_line_type_2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_create_basic_graphics.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_create_basic_graphics.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_document_guid.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_document_guid.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_document_page_setup.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_document_page_setup.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_dxf_info_scanning.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_dxf_info_scanning.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_entities_iterator.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_entities_iterator.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_fix_dulicate_handles.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_fix_dulicate_handles.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_geo.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_geo.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_groups.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_groups.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_ignore_junk_beyond_EOF.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_ignore_junk_beyond_EOF.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_launcher.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_launcher.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_leica_disto_r12.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_leica_disto_r12.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_load_dxf_unicode_notation.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_load_dxf_unicode_notation.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_mapbox_earcut.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_mapbox_earcut.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_mtext_columns.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_mtext_columns.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_mtext_explode_addon.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_mtext_explode_addon.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_mtext_text_frame.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_mtext_text_frame.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_new_table_entries.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_new_table_entries.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_none_ascii_read_write.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_none_ascii_read_write.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_odafc.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_odafc.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_open_binary_DXF_files.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_open_binary_DXF_files.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_open_coord_order_issue.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_open_coord_order_issue.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_open_exotic_dxf_files.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_open_exotic_dxf_files.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_open_R13_R14.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_open_R13_R14.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_polyline_entity.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_polyline_entity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_preserve_binary_data_in_xrecords.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_preserve_binary_data_in_xrecords.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_r12export.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_r12export.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_r12strict.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_r12strict.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_r12writer.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_r12writer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_read_file_without_handles.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_read_file_without_handles.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_read_write_modern_entites.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_read_write_modern_entites.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_recover.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_recover.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_redraw_order.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_redraw_order.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_rotated_block_attributes.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_rotated_block_attributes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_surface_entities.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_surface_entities.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_write_fixed_meta_data.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_write_fixed_meta_data.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_write_without_handles.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_write_without_handles.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/test_xref_detach.py
+Filename: ezdxf-1.1.0b1/integration_tests/test_xref_detach.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/data/AC1003_LINE_Example.dxf
+Filename: ezdxf-1.1.0b1/integration_tests/data/AC1003_LINE_Example.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/data/acad_table_with_blk_ref.dxf
+Filename: ezdxf-1.1.0b1/integration_tests/data/acad_table_with_blk_ref.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/data/ASCII_R12.dxf
+Filename: ezdxf-1.1.0b1/integration_tests/data/ASCII_R12.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/data/bin_dxf_r12.dxf
+Filename: ezdxf-1.1.0b1/integration_tests/data/bin_dxf_r12.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/data/bin_dxf_r13.dxf
+Filename: ezdxf-1.1.0b1/integration_tests/data/bin_dxf_r13.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/data/bin_dxf_r14.dxf
+Filename: ezdxf-1.1.0b1/integration_tests/data/bin_dxf_r14.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/data/bin_dxf_r2000.dxf
+Filename: ezdxf-1.1.0b1/integration_tests/data/bin_dxf_r2000.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/data/cc_dxflib.dxf
+Filename: ezdxf-1.1.0b1/integration_tests/data/cc_dxflib.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/data/custom_blocks.dxf
+Filename: ezdxf-1.1.0b1/integration_tests/data/custom_blocks.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/data/duplicate_handles.dxf
+Filename: ezdxf-1.1.0b1/integration_tests/data/duplicate_handles.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/data/dxf_unicode.dxf
+Filename: ezdxf-1.1.0b1/integration_tests/data/dxf_unicode.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/data/empty_handles.dxf
+Filename: ezdxf-1.1.0b1/integration_tests/data/empty_handles.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/data/groups.dxf
+Filename: ezdxf-1.1.0b1/integration_tests/data/groups.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/data/Leica_Disto_S910.dxf
+Filename: ezdxf-1.1.0b1/integration_tests/data/Leica_Disto_S910.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/data/MODEL.dxf
+Filename: ezdxf-1.1.0b1/integration_tests/data/MODEL.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/data/mtext_columns_R2007.dxf
+Filename: ezdxf-1.1.0b1/integration_tests/data/mtext_columns_R2007.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/data/mtext_columns_R2018.dxf
+Filename: ezdxf-1.1.0b1/integration_tests/data/mtext_columns_R2018.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/data/mtext_framed_columns.dxf
+Filename: ezdxf-1.1.0b1/integration_tests/data/mtext_framed_columns.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/data/mtext_text_frame.dxf
+Filename: ezdxf-1.1.0b1/integration_tests/data/mtext_text_frame.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/data/no_layouts.dxf
+Filename: ezdxf-1.1.0b1/integration_tests/data/no_layouts.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/data/POLI-ALL210_12.DXF
+Filename: ezdxf-1.1.0b1/integration_tests/data/POLI-ALL210_12.DXF
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/data/R12_with_trash_beyond_EOF.dxf
+Filename: ezdxf-1.1.0b1/integration_tests/data/R12_with_trash_beyond_EOF.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/data/recover01.dxf
+Filename: ezdxf-1.1.0b1/integration_tests/data/recover01.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/data/recover02.dxf
+Filename: ezdxf-1.1.0b1/integration_tests/data/recover02.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/data/small_r13.dxf
+Filename: ezdxf-1.1.0b1/integration_tests/data/small_r13.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/data/small_r14.dxf
+Filename: ezdxf-1.1.0b1/integration_tests/data/small_r14.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/data/XRECORD_0.bin
+Filename: ezdxf-1.1.0b1/integration_tests/data/XRECORD_0.bin
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/data/XRECORD_1.bin
+Filename: ezdxf-1.1.0b1/integration_tests/data/XRECORD_1.bin
 Comment: 
 
-Filename: ezdxf-1.1.0b0/integration_tests/data/XRECORD_2.bin
+Filename: ezdxf-1.1.0b1/integration_tests/data/XRECORD_2.bin
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/
+Filename: ezdxf-1.1.0b1/src/ezdxf/
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf.egg-info/
+Filename: ezdxf-1.1.0b1/src/ezdxf.egg-info/
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/acc/
+Filename: ezdxf-1.1.0b1/src/ezdxf/acc/
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/acis/
+Filename: ezdxf-1.1.0b1/src/ezdxf/acis/
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/layouts/
+Filename: ezdxf-1.1.0b1/src/ezdxf/fonts/
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/lldxf/
+Filename: ezdxf-1.1.0b1/src/ezdxf/layouts/
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/math/
+Filename: ezdxf-1.1.0b1/src/ezdxf/lldxf/
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/path/
+Filename: ezdxf-1.1.0b1/src/ezdxf/math/
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/pp/
+Filename: ezdxf-1.1.0b1/src/ezdxf/path/
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/render/
+Filename: ezdxf-1.1.0b1/src/ezdxf/pp/
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/resources/
+Filename: ezdxf-1.1.0b1/src/ezdxf/render/
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/sections/
+Filename: ezdxf-1.1.0b1/src/ezdxf/resources/
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/tools/
+Filename: ezdxf-1.1.0b1/src/ezdxf/sections/
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/appsettings.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/tools/
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/audit.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/appsettings.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/bbox.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/audit.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/blkrefs.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/bbox.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/colors.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/blkrefs.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/commands.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/colors.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/comments.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/commands.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/disassemble.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/comments.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/document.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/disassemble.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/dwginfo.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/document.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entitydb.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/dwginfo.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/enums.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entitydb.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/explode.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/enums.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/eztypes.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/explode.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/filemanagement.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/eztypes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/gfxattribs.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/filemanagement.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/graphicsfactory.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/gfxattribs.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/groupby.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/graphicsfactory.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/npshapes.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/groupby.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/protocols.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/npshapes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/proxygraphic.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/protocols.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/py.typed
+Filename: ezdxf-1.1.0b1/src/ezdxf/proxygraphic.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/query.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/py.typed
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/queryparser.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/query.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/r12strict.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/queryparser.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/recover.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/r12strict.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/reorder.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/recover.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/shapefile.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/reorder.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/transform.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/transform.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/units.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/units.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/upright.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/upright.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/urecord.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/urecord.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/version.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/version.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/xref.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/xref.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/zoom.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/zoom.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/_options.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/_options.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/__init__.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/__main__.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/__main__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/acc/bezier3p.pyx
+Filename: ezdxf-1.1.0b1/src/ezdxf/acc/bezier3p.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/acc/bezier4p.pyx
+Filename: ezdxf-1.1.0b1/src/ezdxf/acc/bezier4p.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/acc/bspline.pyx
+Filename: ezdxf-1.1.0b1/src/ezdxf/acc/bspline.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/acc/construct.pxd
+Filename: ezdxf-1.1.0b1/src/ezdxf/acc/construct.pxd
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/acc/construct.pyx
+Filename: ezdxf-1.1.0b1/src/ezdxf/acc/construct.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/acc/linetypes.pyx
+Filename: ezdxf-1.1.0b1/src/ezdxf/acc/linetypes.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/acc/mapbox_earcut.pyx
+Filename: ezdxf-1.1.0b1/src/ezdxf/acc/mapbox_earcut.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/acc/matrix44.pxd
+Filename: ezdxf-1.1.0b1/src/ezdxf/acc/matrix44.pxd
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/acc/matrix44.pyx
+Filename: ezdxf-1.1.0b1/src/ezdxf/acc/matrix44.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/acc/vector.pxd
+Filename: ezdxf-1.1.0b1/src/ezdxf/acc/vector.pxd
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/acc/vector.pyx
+Filename: ezdxf-1.1.0b1/src/ezdxf/acc/vector.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_cubic_bezier.cpp
+Filename: ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_cubic_bezier.cpp
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_cubic_bezier.hpp
+Filename: ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_cubic_bezier.hpp
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_cubic_bezier.pxd
+Filename: ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_cubic_bezier.pxd
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_quad_bezier.cpp
+Filename: ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_quad_bezier.cpp
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_quad_bezier.hpp
+Filename: ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_quad_bezier.hpp
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_quad_bezier.pxd
+Filename: ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_quad_bezier.pxd
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_vec3.hpp
+Filename: ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_vec3.hpp
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_vec3.pxd
+Filename: ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_vec3.pxd
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/acc/__init__.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/acc/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/acis/abstract.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/acis/abstract.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/acis/api.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/acis/api.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/acis/const.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/acis/const.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/acis/dbg.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/acis/dbg.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/acis/dxf.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/acis/dxf.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/acis/entities.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/acis/entities.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/acis/hdr.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/acis/hdr.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/acis/mesh.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/acis/mesh.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/acis/sab.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/acis/sab.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/acis/sat.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/acis/sat.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/acis/__init__.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/acis/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/acisbrowser/
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/acisbrowser/
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/browser/
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/browser/
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/drawing/
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/drawing/
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/dwg/
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/dwg/
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/acadctb.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/acadctb.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/binpacking.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/binpacking.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/dimlines.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/dimlines.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/dxf2code.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/dxf2code.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/genetic_algorithm.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/genetic_algorithm.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/geo.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/geo.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/gerber_D6673.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/gerber_D6673.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/importer.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/importer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/iterdxf.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/iterdxf.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/menger_sponge.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/menger_sponge.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/meshex.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/meshex.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/mixins.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/mixins.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/mtextsurrogate.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/mtextsurrogate.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/mtxpl.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/mtxpl.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/odafc.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/odafc.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/openscad.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/openscad.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/pycsg.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/pycsg.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/r12export.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/r12export.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/r12writer.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/r12writer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/sierpinski_pyramid.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/sierpinski_pyramid.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/tablepainter.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/tablepainter.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/text2path.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/text2path.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/xqt.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/xqt.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/__init__.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/acisbrowser/browser.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/acisbrowser/browser.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/acisbrowser/data.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/acisbrowser/data.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/acisbrowser/__init__.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/acisbrowser/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/browser/bookmarks.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/browser/bookmarks.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/browser/browser.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/browser/browser.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/browser/data.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/browser/data.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/browser/find_dialog.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/browser/find_dialog.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/browser/loader.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/browser/loader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/browser/model.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/browser/model.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/browser/tags.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/browser/tags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/browser/views.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/browser/views.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/browser/__init__.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/browser/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/drawing/backend.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/drawing/backend.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/drawing/clipper.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/drawing/clipper.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/drawing/config.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/drawing/config.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/drawing/debug_backend.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/drawing/debug_backend.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/drawing/debug_utils.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/drawing/debug_utils.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/drawing/frontend.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/drawing/frontend.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/drawing/gfxproxy.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/drawing/gfxproxy.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/drawing/matplotlib.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/drawing/matplotlib.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/drawing/mtext_complex.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/drawing/mtext_complex.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/drawing/properties.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/drawing/properties.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/drawing/pyqt.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/drawing/pyqt.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/drawing/qtviewer.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/drawing/qtviewer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/drawing/text.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/drawing/recorder.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/drawing/text_renderer.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/drawing/text.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/drawing/type_hints.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/drawing/text_renderer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/drawing/unified_text_renderer.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/drawing/type_hints.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/drawing/__init__.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/drawing/unified_text_renderer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/dwg/classes_section.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/drawing/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/dwg/const.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/dwg/classes_section.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/dwg/crc.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/dwg/const.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/dwg/fileheader.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/dwg/crc.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/dwg/header_section.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/dwg/fileheader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/dwg/loader.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/dwg/header_section.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/dwg/__init__.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/dwg/loader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/api.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/dwg/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/backend.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/api.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/compiler.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/backend.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/deps.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/compiler.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/dxf_backend.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/deps.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/interpreter.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/dxf_backend.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/page.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/interpreter.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/pdf_backend.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/page.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/plotter.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/pdf_backend.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/polygon_buffer.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/plotter.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/properties.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/polygon_buffer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/svg_backend.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/properties.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/tokenizer.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/svg_backend.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/__init__.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/tokenizer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/acad_proxy_entity.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/acad_table.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/acad_proxy_entity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/acis.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/acad_table.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/appdata.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/acis.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/appid.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/appdata.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/arc.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/appid.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/attrib.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/arc.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/block.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/attrib.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/blockrecord.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/block.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/boundary_paths.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/blockrecord.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/circle.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/boundary_paths.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/dictionary.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/circle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/dimension.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/dictionary.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/dimstyle.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/dimension.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/dimstyleoverride.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/dimstyle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/dxfclass.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/dimstyleoverride.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/dxfentity.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/dxfclass.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/dxfgfx.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/dxfentity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/dxfgroups.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/dxfgfx.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/dxfns.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/dxfgroups.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/dxfobj.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/dxfns.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/ellipse.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/dxfobj.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/factory.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/ellipse.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/geodata.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/factory.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/gradient.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/geodata.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/hatch.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/gradient.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/helix.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/hatch.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/idbuffer.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/helix.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/image.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/idbuffer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/insert.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/image.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/layer.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/insert.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/layout.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/layer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/leader.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/light.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/leader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/line.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/light.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/ltype.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/line.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/lwpolyline.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/ltype.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/material.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/lwpolyline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/mesh.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/material.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/mleader.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/mesh.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/mline.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/mleader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/mpolygon.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/mline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/mtext.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/mpolygon.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/mtext_columns.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/mtext.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/objectcollection.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/mtext_columns.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/oleframe.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/objectcollection.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/pattern.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/oleframe.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/point.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/pattern.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/polygon.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/point.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/polyline.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/polygon.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/shape.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/polyline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/solid.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/shape.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/spline.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/solid.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/subentity.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/spline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/sun.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/subentity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/table.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/sun.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/text.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/table.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/textstyle.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/text.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/tolerance.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/textstyle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/ucs.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/tolerance.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/underlay.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/ucs.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/view.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/underlay.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/viewport.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/view.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/visualstyle.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/viewport.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/vport.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/visualstyle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/xdata.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/vport.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/xdict.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/xdata.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/xline.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/xdict.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/entities/__init__.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/xline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/layouts/base.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/entities/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/layouts/blocklayout.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/fonts/fonts.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/layouts/layout.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/fonts/font_face.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/layouts/layouts.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/fonts/font_manager.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/layouts/__init__.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/fonts/font_measurements.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/lldxf/attributes.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/fonts/glyphs.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/lldxf/const.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/fonts/lff.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/lldxf/encoding.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/fonts/shapefile.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/lldxf/extendedtags.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/fonts/ttfonts.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/lldxf/fileindex.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/fonts/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/lldxf/hdrvars.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/layouts/base.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/lldxf/loader.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/layouts/blocklayout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/lldxf/packedtags.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/layouts/layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/lldxf/repair.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/layouts/layouts.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/lldxf/tagger.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/layouts/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/lldxf/tags.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/lldxf/attributes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/lldxf/tagwriter.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/lldxf/const.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/lldxf/types.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/lldxf/encoding.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/lldxf/validator.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/lldxf/extendedtags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/lldxf/__init__.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/lldxf/fileindex.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/math/arc.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/lldxf/hdrvars.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/math/bbox.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/lldxf/loader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/math/bezier.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/lldxf/packedtags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/math/bezier_interpolation.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/lldxf/repair.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/math/box.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/lldxf/tagger.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/math/bspline.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/lldxf/tags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/math/bulge.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/lldxf/tagwriter.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/math/circle.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/lldxf/types.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/math/clipping.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/lldxf/validator.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/math/clustering.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/lldxf/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/math/construct2d.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/math/arc.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/math/construct3d.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/math/bbox.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/math/cspline.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/math/bezier.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/math/curvetools.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/math/bezier_interpolation.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/math/ellipse.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/math/box.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/math/eulerspiral.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/math/bspline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/math/linalg.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/math/bulge.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/math/line.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/math/circle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/math/offset2d.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/math/clipping.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/math/parametrize.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/math/clustering.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/math/perlin.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/math/construct2d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/math/polyline.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/math/construct3d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/math/rtree.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/math/cspline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/math/shape.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/math/curvetools.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/math/surfaces.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/math/ellipse.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/math/transformtools.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/math/eulerspiral.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/math/triangulation.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/math/linalg.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/math/ucs.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/math/line.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/math/_bezier3p.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/math/offset2d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/math/_bezier4p.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/math/parametrize.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/math/_bspline.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/math/perlin.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/math/_construct.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/math/polyline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/math/_ctypes.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/math/rtree.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/math/_mapbox_earcut.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/math/shape.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/math/_matrix44.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/math/surfaces.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/math/_vector.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/math/transformtools.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/math/__init__.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/math/triangulation.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/path/commands.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/math/ucs.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/path/converter.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/math/_bezier3p.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/path/nesting.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/math/_bezier4p.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/path/path.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/math/_bspline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/path/shapes.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/math/_construct.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/path/tools.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/math/_ctypes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/path/__init__.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/math/_mapbox_earcut.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/pp/dxfpp.css
+Filename: ezdxf-1.1.0b1/src/ezdxf/math/_matrix44.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/pp/dxfpp.html
+Filename: ezdxf-1.1.0b1/src/ezdxf/math/_vector.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/pp/dxfpp.js
+Filename: ezdxf-1.1.0b1/src/ezdxf/math/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/pp/dxfpp.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/path/commands.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/pp/pprint.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/path/converter.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/pp/rawpp.css
+Filename: ezdxf-1.1.0b1/src/ezdxf/path/nesting.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/pp/rawpp.html
+Filename: ezdxf-1.1.0b1/src/ezdxf/path/path.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/pp/rawpp.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/path/shapes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/pp/reflinks.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/path/tools.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/pp/__init__.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/path/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/render/abstract_mtext_renderer.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/pp/dxfpp.css
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/render/arrows.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/pp/dxfpp.html
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/render/curves.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/pp/dxfpp.js
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/render/dimension.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/pp/dxfpp.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/render/dim_base.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/pp/pprint.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/render/dim_curved.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/pp/rawpp.css
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/render/dim_diameter.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/pp/rawpp.html
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/render/dim_linear.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/pp/rawpp.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/render/dim_ordinate.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/pp/reflinks.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/render/dim_radius.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/pp/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/render/forms.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/render/abstract_mtext_renderer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/render/hatching.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/render/arrows.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/render/leader.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/render/curves.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/render/linetypes.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/render/dimension.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/render/mesh.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/render/dim_base.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/render/mleader.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/render/dim_curved.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/render/mline.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/render/dim_diameter.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/render/point.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/render/dim_linear.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/render/polyline.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/render/dim_ordinate.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/render/r12spline.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/render/dim_radius.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/render/trace.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/render/forms.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/render/_linetypes.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/render/hatching.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/render/__init__.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/render/leader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/resources/16x16.png
+Filename: ezdxf-1.1.0b1/src/ezdxf/render/linetypes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/resources/24x24.png
+Filename: ezdxf-1.1.0b1/src/ezdxf/render/mesh.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/resources/256x256.png
+Filename: ezdxf-1.1.0b1/src/ezdxf/render/mleader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/resources/32x32.png
+Filename: ezdxf-1.1.0b1/src/ezdxf/render/mline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/resources/48x48.png
+Filename: ezdxf-1.1.0b1/src/ezdxf/render/point.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/resources/64x64.png
+Filename: ezdxf-1.1.0b1/src/ezdxf/render/polyline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/resources/icon-copy-64px.png
+Filename: ezdxf-1.1.0b1/src/ezdxf/render/r12spline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/resources/icon-find-64px.png
+Filename: ezdxf-1.1.0b1/src/ezdxf/render/trace.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/resources/icon-goto-bookmark-64px.png
+Filename: ezdxf-1.1.0b1/src/ezdxf/render/_linetypes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/resources/icon-goto-handle-64px.png
+Filename: ezdxf-1.1.0b1/src/ezdxf/render/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/resources/icon-goto-line-64px.png
+Filename: ezdxf-1.1.0b1/src/ezdxf/resources/16x16.png
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/resources/icon-left-arrow-64px.png
+Filename: ezdxf-1.1.0b1/src/ezdxf/resources/24x24.png
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/resources/icon-next-entity-64px.png
+Filename: ezdxf-1.1.0b1/src/ezdxf/resources/256x256.png
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/resources/icon-prev-entity-64px.png
+Filename: ezdxf-1.1.0b1/src/ezdxf/resources/32x32.png
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/resources/icon-right-arrow-64px.png
+Filename: ezdxf-1.1.0b1/src/ezdxf/resources/48x48.png
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/resources/icon-show-in-tree-64px.png
+Filename: ezdxf-1.1.0b1/src/ezdxf/resources/64x64.png
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/resources/icon-store-bookmark-64px.png
+Filename: ezdxf-1.1.0b1/src/ezdxf/resources/icon-copy-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/sections/acdsdata.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/resources/icon-find-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/sections/blocks.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/resources/icon-goto-bookmark-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/sections/classes.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/resources/icon-goto-handle-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/sections/entities.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/resources/icon-goto-line-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/sections/header.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/resources/icon-left-arrow-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/sections/headervars.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/resources/icon-next-entity-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/sections/objects.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/resources/icon-prev-entity-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/sections/table.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/resources/icon-right-arrow-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/sections/tables.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/resources/icon-show-in-tree-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/sections/__init__.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/resources/icon-store-bookmark-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/tools/analyze.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/sections/acdsdata.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/tools/binarydata.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/sections/blocks.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/tools/codepage.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/sections/classes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/tools/complex_ltype.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/sections/entities.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/tools/crypt.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/sections/header.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/tools/debug.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/sections/headervars.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/tools/difftags.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/sections/objects.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/tools/fonts.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/sections/table.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/tools/font_face.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/sections/tables.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/tools/font_manager.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/sections/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/tools/handle.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/tools/analyze.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/tools/indexing.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/tools/binarydata.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/tools/juliandate.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/tools/codepage.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/tools/pattern.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/tools/complex_ltype.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/tools/rawloader.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/tools/crypt.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/tools/standards.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/tools/debug.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/tools/strip.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/tools/difftags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/tools/test.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/tools/handle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/tools/text.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/tools/indexing.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/tools/text_layout.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/tools/juliandate.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/tools/text_size.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/tools/pattern.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/tools/ttfonts.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/tools/rawloader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/tools/zipmanager.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/tools/standards.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/tools/_iso_pattern.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/tools/strip.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf/tools/__init__.py
+Filename: ezdxf-1.1.0b1/src/ezdxf/tools/test.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf.egg-info/dependency_links.txt
+Filename: ezdxf-1.1.0b1/src/ezdxf/tools/text.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf.egg-info/entry_points.txt
+Filename: ezdxf-1.1.0b1/src/ezdxf/tools/text_layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf.egg-info/not-zip-safe
+Filename: ezdxf-1.1.0b1/src/ezdxf/tools/text_size.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf.egg-info/PKG-INFO
+Filename: ezdxf-1.1.0b1/src/ezdxf/tools/zipmanager.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf.egg-info/requires.txt
+Filename: ezdxf-1.1.0b1/src/ezdxf/tools/_iso_pattern.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf.egg-info/SOURCES.txt
+Filename: ezdxf-1.1.0b1/src/ezdxf/tools/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/src/ezdxf.egg-info/top_level.txt
+Filename: ezdxf-1.1.0b1/src/ezdxf.egg-info/dependency_links.txt
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/
+Filename: ezdxf-1.1.0b1/src/ezdxf.egg-info/entry_points.txt
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/
+Filename: ezdxf-1.1.0b1/src/ezdxf.egg-info/not-zip-safe
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/
+Filename: ezdxf-1.1.0b1/src/ezdxf.egg-info/PKG-INFO
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_03_dxf_layouts/
+Filename: ezdxf-1.1.0b1/src/ezdxf.egg-info/requires.txt
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/
+Filename: ezdxf-1.1.0b1/src/ezdxf.egg-info/SOURCES.txt
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_05_tools/
+Filename: ezdxf-1.1.0b1/src/ezdxf.egg-info/top_level.txt
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/
+Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_07_render/
+Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_08_addons/
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_09_cython_acceleration/
+Filename: ezdxf-1.1.0b1/tests/test_03_dxf_layouts/
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_10_issues/
+Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/conftest.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
+Filename: ezdxf-1.1.0b1/tests/test_07_render/
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
+Filename: ezdxf-1.1.0b1/tests/test_08_addons/
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
+Filename: ezdxf-1.1.0b1/tests/test_09_cython_acceleration/
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
+Filename: ezdxf-1.1.0b1/tests/test_10_issues/
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_010_binary_data.py
+Filename: ezdxf-1.1.0b1/tests/conftest.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_011_codepage.py
+Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_012_crypt.py
+Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_013_juliandate.py
+Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py
+Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py
+Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_016_encoding.py
+Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_010_binary_data.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_018_handle.py
+Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_011_codepage.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py
+Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_012_crypt.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py
+Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_013_juliandate.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py
+Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_022_set_flag_state.py
+Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py
+Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_016_encoding.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_024_render_tag.py
+Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_018_handle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_040_tags.py
+Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_041_group_tags.py
+Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py
+Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py
+Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_022_set_flag_state.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py
+Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py
+Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_024_render_tag.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py
+Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_040_tags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py
+Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_041_group_tags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py
+Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py
+Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py
+Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py
+Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_101_dxfnamespace.py
+Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_102_appdata.py
+Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_103_reactors.py
+Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_104_extension_dict.py
+Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_105_xdata.py
+Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_110_dxfentity.py
+Filename: ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py
+Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_101_dxfnamespace.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_112a_dxfgfx.py
+Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_102_appdata.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_112b_dxfobj.py
+Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_103_reactors.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_113_dxfclass.py
+Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_104_extension_dict.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_114_factory.py
+Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_105_xdata.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_115_new_empty_drawing.py
+Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_110_dxfentity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_116_dictionary.py
+Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_117_layer_table_entry.py
+Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_112a_dxfgfx.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_118_appid_table_entry.py
+Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_112b_dxfobj.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_119_ucs_table_entry.py
+Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_113_dxfclass.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_120_style_table_entry.py
+Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_114_factory.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_121_ltype_table_entry.py
+Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_115_new_empty_drawing.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_122_vport_table_entry.py
+Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_116_dictionary.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_123_view_table_entry.py
+Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_117_layer_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py
+Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_118_appid_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_125_image_def.py
+Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_119_ucs_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_126_image_def_reactor.py
+Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_120_style_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_127_raster_variables.py
+Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_121_ltype_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_128_pdf_definition.py
+Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_122_vport_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_129_xrecord.py
+Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_123_view_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_130_id_buffer.py
+Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_131_field_list.py
+Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_125_image_def.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_132_layer_filter.py
+Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_126_image_def_reactor.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_133_sun.py
+Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_127_raster_variables.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_134_material.py
+Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_128_pdf_definition.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_135_geo_data.py
+Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_129_xrecord.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_136_vba_project.py
+Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_130_id_buffer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_137_sortentstable.py
+Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_131_field_list.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_138_setup_visual_styles.py
+Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_132_layer_filter.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_139_user_record.py
+Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_133_sun.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_140_block_record.py
+Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_134_material.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_141_layer_vp_override.py
+Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_135_geo_data.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/conftest.py
+Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_136_vba_project.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_200_line.py
+Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_137_sortentstable.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_201_point.py
+Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_138_setup_visual_styles.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_202_circle.py
+Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_139_user_record.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_203_arc.py
+Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_140_block_record.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_204_shape.py
+Filename: ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_141_layer_vp_override.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_205_solid.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/conftest.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_206_text.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_200_line.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_207_attdef.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_201_point.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_208_attrib.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_202_circle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_209_vertex.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_203_arc.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_210_polyline_1.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_204_shape.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_210_polyline_2.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_205_solid.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_210_polyline_explode.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_206_text.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_207_attdef.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_211_viewport.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_208_attrib.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_212_insert.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_209_vertex.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_213_minsert.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_210_polyline_1.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_214_block.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_210_polyline_2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_215_dimension.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_210_polyline_explode.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_216_dimlines_R12.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_211_viewport.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_212_insert.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_213_minsert.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_214_block.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_215_dimension.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_216_dimlines_R12.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_221_ellipse.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_222_xline.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_223_ray.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_224_group.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_225_mtext.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_226_spline.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_221_ellipse.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_222_xline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_228_mesh.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_223_ray.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_224_group.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_229b_hatch_extended.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_225_mtext.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_226_spline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_231_underlay.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_228_mesh.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_231_underlay_2.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_232_acis.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_229b_hatch_extended.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_232_acis_2.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_232_surface.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_233_helix.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_234_light.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_231_underlay.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_235_leader.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_231_underlay_2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_236_multileader.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_232_acis.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_237_mline.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_232_acis_2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_238_tolerance.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_232_surface.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_239_proxy_graphic.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_233_helix.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_240_arc_dimension.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_234_light.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_241_hyperlink.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_235_leader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_242_random_transform.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_236_multileader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_243_replace_entity.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_237_mline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_238_tolerance.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_245_wipeout.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_239_proxy_graphic.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_246_spline_audit.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_240_arc_dimension.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_241_hyperlink.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_248_mpolygon.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_242_random_transform.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_243_replace_entity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_249_boundary_paths.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_245_wipeout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_251_upright.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_246_spline_audit.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_253_ole2frame.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_248_mpolygon.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_254_get_font_name.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_300_layout.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_249_boundary_paths.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_302_block_references.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_251_upright.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_303_auto_block_references.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_304_new_entity_space.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_253_ole2frame.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py
+Filename: ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_254_get_font_name.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py
+Filename: ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_300_layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_307_groupby.py
+Filename: ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_308_query.py
+Filename: ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_302_block_references.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_309_query_parser.py
+Filename: ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_303_auto_block_references.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py
+Filename: ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_304_new_entity_space.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_312_virtual_layout.py
+Filename: ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_313_redraw_order.py
+Filename: ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_401_headersection.py
+Filename: ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_307_groupby.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_402_classessection.py
+Filename: ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_308_query.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_403_entity_database.py
+Filename: ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_309_query_parser.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_404a_tables.py
+Filename: ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py
+Filename: ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_312_virtual_layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_405_classes.py
+Filename: ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_313_redraw_order.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py
+Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_401_headersection.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_407_entity_section.py
+Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_402_classessection.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_408_objects_section.py
+Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_403_entity_database.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_409_create_objects.py
+Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_404a_tables.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_410_table.py
+Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_411_acds_data.py
+Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_405_classes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py
+Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py
+Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_407_entity_section.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py
+Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_408_objects_section.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_415_layout_management.py
+Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_409_create_objects.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py
+Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_410_table.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py
+Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_411_acds_data.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_417_bbox.py
+Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py
+Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py
+Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py
+Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_415_layout_management.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py
+Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py
+Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_424_audit.py
+Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_417_bbox.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py
+Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py
+Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_427_appsettings.py
+Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py
+Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_05_tools/conftest.py
+Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_500_units.py
+Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_424_audit.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_501_truecolor.py
+Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_502_raw_color.py
+Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_503_indexing.py
+Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_427_appsettings.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_504_suppress_zeros.py
+Filename: ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_506_version.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/conftest.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_507_dxf_pretty_printer.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_500_units.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_508_read_zip.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_501_truecolor.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_509_comments.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_502_raw_color.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_510_byte_stream.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_503_indexing.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_511_bit_stream.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_504_suppress_zeros.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_512_pattern.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_506_version.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_513_reorder_entities.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_507_dxf_pretty_printer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_514_text.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_508_read_zip.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_515_fonts.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_509_comments.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_516_zoom.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_510_byte_stream.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_517_text_layout.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_511_bit_stream.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_518_header_guid.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_512_pattern.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_519_mtext_editor.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_513_reorder_entities.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_520_mtext_context.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_514_text.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_521_mtext_parser.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_515a_fonts_truetype.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_522_text_scanner.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_515b_fonts_shapefiles.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_523_text_size.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_515c_fonts_lff.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_524_block_reference_manager.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_516_zoom.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_525_transparency.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_517_text_layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_526_explode.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_518_header_guid.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_527_gfxattribs.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_519_mtext_editor.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_528_difftags.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_520_mtext_context.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_529_acis_sat.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_521_mtext_parser.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_530_acis_sab.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_522_text_scanner.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_531_acis_entities.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_523_text_size.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_532_acis_mesh.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_524_block_reference_manager.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_533_shapefiles.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_525_transparency.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_534_dwg_info.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_526_explode.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_535_xref_basic.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_527_gfxattribs.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_536_xref_conflict.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_528_difftags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_537_transform.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_529_acis_sat.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_538_scale_mtext_inline_commands.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_530_acis_sab.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_539_npshapes.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_531_acis_entities.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/conftest.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_532_acis_mesh.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_600_base.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_533_shapefiles.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_601_bulge.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_534_dwg_info.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_602_vec3.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_535_xref_basic.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_603_vec2.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_536_xref_conflict.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_604_banded_matrix.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_537_transform.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_604_linalg.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_538_scale_mtext_inline_commands.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_605_matrix44.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_539_npshapes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_606_convexhull.py
+Filename: ezdxf-1.1.0b1/tests/test_05_tools/test_540_lff_parser.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_607_perlin_noise.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/conftest.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_608_intersection_line_line_2d.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_600_base.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_609_point_on_line.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_601_bulge.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_610_ocs.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_602_vec3.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_611_ucs.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_603_vec2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_612_ucs_pass_trough.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_604_banded_matrix.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_613_point_in_poygon.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_604_linalg.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_614_construct_3d.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_605_matrix44.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_615_rytz_axis.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_606_convexhull.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_616_plane.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_607_perlin_noise.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_617_clockwise_orientation.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_608_intersection_line_line_2d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_618_clipping.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_609_point_on_line.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_619_greiner_hormann.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_610_ocs.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_620_knot.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_611_ucs.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_621_bspline.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_612_ucs_pass_trough.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_622_bsplineu.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_613_point_in_poygon.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_623_rbspline.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_614_construct_3d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_624_global_bspline_interpolation.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_615_rytz_axis.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_626_local_bspline_interpolation.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_616_plane.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_627_bspline_basis.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_617_clockwise_orientation.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_629_bezier.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_618_clipping.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_630a_bezier4p_base.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_619_greiner_hormann.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_630b_bezier4p_functions.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_620_knot.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_631_euler_spiral.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_621_bspline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_632_bezier3p.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_622_bsplineu.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_640_bbox.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_623_rbspline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_641_construction_ray.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_624_global_bspline_interpolation.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_642_construction_line.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_626_local_bspline_interpolation.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_643_construction_box.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_627_bspline_basis.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_644_construction_circle.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_629_bezier.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_645_construction_arc.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_630a_bezier4p_base.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_646_offset_vertices_2d.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_630b_bezier4p_functions.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_647_transform_tools.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_631_euler_spiral.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_648_construction_ellipse.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_632_bezier3p.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_650_elliptic_arc_span.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_640_bbox.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_651_construction_polyline.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_641_construction_ray.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_652_approx_param_t.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_642_construction_line.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_653_polyline_intersection.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_643_construction_box.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_654_rtree.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_644_construction_circle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_655_dbscan.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_645_construction_arc.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_656_k_means.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_646_offset_vertices_2d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_657_mapbox_earcut.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_647_transform_tools.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_658_bevel_tools.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_648_construction_ellipse.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_659_intersection_line_polygon_3d.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_650_elliptic_arc_span.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_660_intersection_ray_polygon_3d.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_651_construction_polyline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_652_approx_param_t.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_06_math/test_662_is_convex_polygon_2d.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_653_polyline_intersection.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_07_render/test_701_arrows.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_654_rtree.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_07_render/test_702_render_forms.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_655_dbscan.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_07_render/test_703_mesh_builder.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_656_k_means.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_07_render/test_704_render_linear_dimension.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_657_mapbox_earcut.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_07_render/test_705_shape.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_658_bevel_tools.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_07_render/test_706_random_path.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_659_intersection_line_polygon_3d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_07_render/test_707_trace.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_660_intersection_ray_polygon_3d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_07_render/test_708a_path.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_07_render/test_708b_path_tools.py
+Filename: ezdxf-1.1.0b1/tests/test_06_math/test_662_is_convex_polygon_2d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_07_render/test_708c_matplotlib_path_tools.py
+Filename: ezdxf-1.1.0b1/tests/test_07_render/test_701_arrows.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_07_render/test_708d_qpainter_path_tools.py
+Filename: ezdxf-1.1.0b1/tests/test_07_render/test_702_render_forms.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_07_render/test_708e_path_shapes.py
+Filename: ezdxf-1.1.0b1/tests/test_07_render/test_703_mesh_builder.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_07_render/test_708f_path_nesting.py
+Filename: ezdxf-1.1.0b1/tests/test_07_render/test_704_render_linear_dimension.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_07_render/test_709_linetype_renderer.py
+Filename: ezdxf-1.1.0b1/tests/test_07_render/test_705_shape.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_07_render/test_711_points.py
+Filename: ezdxf-1.1.0b1/tests/test_07_render/test_706_random_path.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_07_render/test_712_render_curved_dimension.py
+Filename: ezdxf-1.1.0b1/tests/test_07_render/test_707_trace.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_07_render/test_713_mleader_builder.py
+Filename: ezdxf-1.1.0b1/tests/test_07_render/test_708a_path.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_07_render/test_714_mleader_render_engine.py
+Filename: ezdxf-1.1.0b1/tests/test_07_render/test_708b_path_tools.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_07_render/test_715_hatching.py
+Filename: ezdxf-1.1.0b1/tests/test_07_render/test_708c_matplotlib_path_tools.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_07_render/test_715_issue_747_explode_3d_dim.py
+Filename: ezdxf-1.1.0b1/tests/test_07_render/test_708d_qpainter_path_tools.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_800_mtext_surrogate.py
+Filename: ezdxf-1.1.0b1/tests/test_07_render/test_708e_path_shapes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_801_r12spline.py
+Filename: ezdxf-1.1.0b1/tests/test_07_render/test_708f_path_nesting.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_802_table_painter.py
+Filename: ezdxf-1.1.0b1/tests/test_07_render/test_709_linetype_renderer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_803_entities_to_code.py
+Filename: ezdxf-1.1.0b1/tests/test_07_render/test_711_points.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_804_importer.py
+Filename: ezdxf-1.1.0b1/tests/test_07_render/test_712_render_curved_dimension.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_805_pycsg.py
+Filename: ezdxf-1.1.0b1/tests/test_07_render/test_713_mleader_builder.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_806_acadctb.py
+Filename: ezdxf-1.1.0b1/tests/test_07_render/test_714_mleader_render_engine.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_807_dwg_loader_basics.py
+Filename: ezdxf-1.1.0b1/tests/test_07_render/test_715_hatching.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_810_drawing_properties.py
+Filename: ezdxf-1.1.0b1/tests/test_07_render/test_715_issue_747_explode_3d_dim.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_811_drawing_frontend.py
+Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_800_mtext_surrogate.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_812_drawing_graphic_proxy.py
+Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_801_r12spline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_813_geo_interface.py
+Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_802_table_painter.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_814_text2path.py
+Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_803_entities_to_code.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_815_dxf_browser.py
+Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_804_importer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_816_bin_packing.py
+Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_805_pycsg.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_817_genetic_algorithm.py
+Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_806_acadctb.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_818_meshex.py
+Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_807_dwg_loader_basics.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_819_menger_sponge.py
+Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_810_drawing_properties.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_820_openscad.py
+Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_811a_drawing_frontend.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_821_hpgl2.py
+Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_811b_drawing_recorder.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
+Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_812_drawing_graphic_proxy.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_822_clipper.py
+Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_813_geo_interface.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_09_cython_acceleration/test_901_acc_vec2.py
+Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_814_text2path.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_09_cython_acceleration/test_902_acc_vec3.py
+Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_815_dxf_browser.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_09_cython_acceleration/test_903_acc_matrix44.py
+Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_816_bin_packing.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
+Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_817_genetic_algorithm.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
+Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_818_meshex.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_09_cython_acceleration/test_906_acc_bspline.py
+Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_819_menger_sponge.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_10_issues/test_issue_414_bbox_calculation.py
+Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_820_openscad.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
+Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_821_hpgl2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_10_issues/test_issue_574_flattening_error.py
+Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
+Filename: ezdxf-1.1.0b1/tests/test_08_addons/test_822_clipper.py
 Comment: 
 
-Filename: ezdxf-1.1.0b0/tests/test_10_issues/test_issue_749_text_layout.py
+Filename: ezdxf-1.1.0b1/tests/test_09_cython_acceleration/test_901_acc_vec2.py
+Comment: 
+
+Filename: ezdxf-1.1.0b1/tests/test_09_cython_acceleration/test_902_acc_vec3.py
+Comment: 
+
+Filename: ezdxf-1.1.0b1/tests/test_09_cython_acceleration/test_903_acc_matrix44.py
+Comment: 
+
+Filename: ezdxf-1.1.0b1/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
+Comment: 
+
+Filename: ezdxf-1.1.0b1/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
+Comment: 
+
+Filename: ezdxf-1.1.0b1/tests/test_09_cython_acceleration/test_906_acc_bspline.py
+Comment: 
+
+Filename: ezdxf-1.1.0b1/tests/test_10_issues/test_issue_414_bbox_calculation.py
+Comment: 
+
+Filename: ezdxf-1.1.0b1/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
+Comment: 
+
+Filename: ezdxf-1.1.0b1/tests/test_10_issues/test_issue_574_flattening_error.py
+Comment: 
+
+Filename: ezdxf-1.1.0b1/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
+Comment: 
+
+Filename: ezdxf-1.1.0b1/tests/test_10_issues/test_issue_749_text_layout.py
 Comment: 
 
 Zip file comment:
```

## Comparing `ezdxf-1.1.0b0/LICENSE` & `ezdxf-1.1.0b1/LICENSE`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/NEWS.md` & `ezdxf-1.1.0b1/NEWS.md`

 * *Files 0% similar despite different names*

```diff
@@ -7,27 +7,30 @@
 
 - Release notes: https://ezdxf.mozman.at/release-v1-1.html
 - WARNING: The font support changed drastically in this version, if you use the 
   `ezdxf.tools.fonts` module your code will break, sorry! Pin the `ezdxf` version to 
   v1.0.3 in your `requirements.txt` file to use the previous version!
 - NEW: `numpy` is a hard dependency, requires Python version >= 3.8
 - NEW: `fontTools` is a hard dependency
-- NEW: `Matrix44.Path2d()` class, `Path` class with `Vec2` vertices
-- NEW: optimized `Matrix44.fast_2d_transform()` method
-- NEW: added setter to `BlockLayout.base_point` property
+- NEW: `ezdxf.path.Path2d()` class, `Path` class with `Vec2` vertices
 - NEW: `ezdxf.xref` new core module to manage XREFs and load resources from DXF files
 - NEW: `ezdxf.addons.hpgl2` add-on to convert HPGL/2 plot files to DXF or SVG
 - NEW: `ezdxf plt2dxf` command to convert HPGL/2 plot files to DXF
 - NEW: `ezdxf plt2svg` command to convert HPGL/2 plot files to SVG
 - NEW: `ezdxf plt2pdf` command to convert HPGL/2 plot files to PDF
-- CHANGED: refactoring of `ezdxf.tools.fonts`
+- NEW: support for measuring and rendering of .shx, .shp and .lff fonts, the basic 
+  stroke fonts included in CAD applications
+- NEW: added setter to `BlockLayout.base_point` property
+- CHANGED: moved font related modules into a new subpackage `ezdxf.fonts` 
+  including a big refactoring
 - CHANGED: `FontFace` class - `weight` attribute is an int value (0-1000), `stretch` is 
   renamed to `width` and is also an int value (1-9) now
 - REMOVED: replaced `matplotlib` font support module by `fontTools`
-- REMOVED: configuration option `use_matplotlib`
+- REMOVED: configuration option `use_matplotlib` - is not needed anymore
+- REMOVED: configuration option `font_cache_directory` - is not needed anymore
 - CHANGED: text rendering for the `drawing` add-on and text measurement is done by the
   `fontTools` package
 - CHANGED: moved text rendering from backend classes to the `Frontend` class
 - CHANGED: moved clipping support from backend classes to the `Frontend` class
 - REMOVED: `PillowBackend` and the `pillow` command
 - REMOVED: `geomdl` test dependency
 - BUGFIX: invalid bulge to Bezier curve conversion for bulge values >= 1
```

## Comparing `ezdxf-1.1.0b0/PKG-INFO` & `ezdxf-1.1.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezdxf
-Version: 1.1.0b0
+Version: 1.1.0b1
 Summary: A Python package to create/manipulate DXF drawings.
 Home-page: https://ezdxf.mozman.at
 Author: Manfred Moitzi
 Author-email: me@mozman.at
 License: MIT License
 Download-URL: https://pypi.org/project/ezdxf/
 Keywords: DXF,CAD
@@ -220,27 +220,30 @@
 
 - Release notes: https://ezdxf.mozman.at/release-v1-1.html
 - WARNING: The font support changed drastically in this version, if you use the 
   `ezdxf.tools.fonts` module your code will break, sorry! Pin the `ezdxf` version to 
   v1.0.3 in your `requirements.txt` file to use the previous version!
 - NEW: `numpy` is a hard dependency, requires Python version >= 3.8
 - NEW: `fontTools` is a hard dependency
-- NEW: `Matrix44.Path2d()` class, `Path` class with `Vec2` vertices
-- NEW: optimized `Matrix44.fast_2d_transform()` method
-- NEW: added setter to `BlockLayout.base_point` property
+- NEW: `ezdxf.path.Path2d()` class, `Path` class with `Vec2` vertices
 - NEW: `ezdxf.xref` new core module to manage XREFs and load resources from DXF files
 - NEW: `ezdxf.addons.hpgl2` add-on to convert HPGL/2 plot files to DXF or SVG
 - NEW: `ezdxf plt2dxf` command to convert HPGL/2 plot files to DXF
 - NEW: `ezdxf plt2svg` command to convert HPGL/2 plot files to SVG
 - NEW: `ezdxf plt2pdf` command to convert HPGL/2 plot files to PDF
-- CHANGED: refactoring of `ezdxf.tools.fonts`
+- NEW: support for measuring and rendering of .shx, .shp and .lff fonts, the basic 
+  stroke fonts included in CAD applications
+- NEW: added setter to `BlockLayout.base_point` property
+- CHANGED: moved font related modules into a new subpackage `ezdxf.fonts` 
+  including a big refactoring
 - CHANGED: `FontFace` class - `weight` attribute is an int value (0-1000), `stretch` is 
   renamed to `width` and is also an int value (1-9) now
 - REMOVED: replaced `matplotlib` font support module by `fontTools`
-- REMOVED: configuration option `use_matplotlib`
+- REMOVED: configuration option `use_matplotlib` - is not needed anymore
+- REMOVED: configuration option `font_cache_directory` - is not needed anymore
 - CHANGED: text rendering for the `drawing` add-on and text measurement is done by the
   `fontTools` package
 - CHANGED: moved text rendering from backend classes to the `Frontend` class
 - CHANGED: moved clipping support from backend classes to the `Frontend` class
 - REMOVED: `PillowBackend` and the `pillow` command
 - REMOVED: `geomdl` test dependency
 - BUGFIX: invalid bulge to Bezier curve conversion for bulge values >= 1
```

## Comparing `ezdxf-1.1.0b0/README.md` & `ezdxf-1.1.0b1/README.md`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/setup.py` & `ezdxf-1.1.0b1/setup.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/check_disable_c_ext_by_config_file.py` & `ezdxf-1.1.0b1/integration_tests/check_disable_c_ext_by_config_file.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/check_disable_c_ext_by_env_var.py` & `ezdxf-1.1.0b1/integration_tests/check_disable_c_ext_by_env_var.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_acad_table.py` & `ezdxf-1.1.0b1/integration_tests/test_acad_table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_all_dimline_styles.py` & `ezdxf-1.1.0b1/integration_tests/test_all_dimline_styles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_all_ellipse_transformations.py` & `ezdxf-1.1.0b1/integration_tests/test_all_ellipse_transformations.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_anonymous_blocks.py` & `ezdxf-1.1.0b1/integration_tests/test_anonymous_blocks.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_audit_critical_dxf_files.py` & `ezdxf-1.1.0b1/integration_tests/test_audit_critical_dxf_files.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_audit_layouts.py` & `ezdxf-1.1.0b1/integration_tests/test_audit_layouts.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_complex_line_type_2.py` & `ezdxf-1.1.0b1/integration_tests/test_complex_line_type_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_create_basic_graphics.py` & `ezdxf-1.1.0b1/integration_tests/test_create_basic_graphics.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_document_guid.py` & `ezdxf-1.1.0b1/integration_tests/test_document_guid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_document_page_setup.py` & `ezdxf-1.1.0b1/integration_tests/test_document_page_setup.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_dxf_info_scanning.py` & `ezdxf-1.1.0b1/integration_tests/test_dxf_info_scanning.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_entities_iterator.py` & `ezdxf-1.1.0b1/integration_tests/test_entities_iterator.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_fix_dulicate_handles.py` & `ezdxf-1.1.0b1/integration_tests/test_fix_dulicate_handles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_geo.py` & `ezdxf-1.1.0b1/integration_tests/test_geo.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_groups.py` & `ezdxf-1.1.0b1/integration_tests/test_groups.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_ignore_junk_beyond_EOF.py` & `ezdxf-1.1.0b1/integration_tests/test_ignore_junk_beyond_EOF.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_launcher.py` & `ezdxf-1.1.0b1/integration_tests/test_launcher.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_leica_disto_r12.py` & `ezdxf-1.1.0b1/integration_tests/test_leica_disto_r12.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_load_dxf_unicode_notation.py` & `ezdxf-1.1.0b1/integration_tests/test_load_dxf_unicode_notation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_mapbox_earcut.py` & `ezdxf-1.1.0b1/integration_tests/test_mapbox_earcut.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_mtext_columns.py` & `ezdxf-1.1.0b1/integration_tests/test_mtext_columns.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_mtext_explode_addon.py` & `ezdxf-1.1.0b1/integration_tests/test_mtext_explode_addon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_mtext_text_frame.py` & `ezdxf-1.1.0b1/integration_tests/test_mtext_text_frame.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_new_table_entries.py` & `ezdxf-1.1.0b1/integration_tests/test_new_table_entries.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_none_ascii_read_write.py` & `ezdxf-1.1.0b1/integration_tests/test_none_ascii_read_write.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_odafc.py` & `ezdxf-1.1.0b1/integration_tests/test_odafc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_open_binary_DXF_files.py` & `ezdxf-1.1.0b1/integration_tests/test_open_binary_DXF_files.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_open_coord_order_issue.py` & `ezdxf-1.1.0b1/integration_tests/test_open_coord_order_issue.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_open_exotic_dxf_files.py` & `ezdxf-1.1.0b1/integration_tests/test_open_exotic_dxf_files.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_open_R13_R14.py` & `ezdxf-1.1.0b1/integration_tests/test_open_R13_R14.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_polyline_entity.py` & `ezdxf-1.1.0b1/integration_tests/test_polyline_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_preserve_binary_data_in_xrecords.py` & `ezdxf-1.1.0b1/integration_tests/test_preserve_binary_data_in_xrecords.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_r12export.py` & `ezdxf-1.1.0b1/integration_tests/test_r12export.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_r12strict.py` & `ezdxf-1.1.0b1/integration_tests/test_r12strict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_r12writer.py` & `ezdxf-1.1.0b1/integration_tests/test_r12writer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_read_file_without_handles.py` & `ezdxf-1.1.0b1/integration_tests/test_read_file_without_handles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_read_write_modern_entites.py` & `ezdxf-1.1.0b1/integration_tests/test_read_write_modern_entites.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_recover.py` & `ezdxf-1.1.0b1/integration_tests/test_recover.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_redraw_order.py` & `ezdxf-1.1.0b1/integration_tests/test_redraw_order.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_rotated_block_attributes.py` & `ezdxf-1.1.0b1/integration_tests/test_rotated_block_attributes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_surface_entities.py` & `ezdxf-1.1.0b1/integration_tests/test_surface_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_write_fixed_meta_data.py` & `ezdxf-1.1.0b1/integration_tests/test_write_fixed_meta_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_write_without_handles.py` & `ezdxf-1.1.0b1/integration_tests/test_write_without_handles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/test_xref_detach.py` & `ezdxf-1.1.0b1/integration_tests/test_xref_detach.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/data/AC1003_LINE_Example.dxf` & `ezdxf-1.1.0b1/integration_tests/data/AC1003_LINE_Example.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/data/acad_table_with_blk_ref.dxf` & `ezdxf-1.1.0b1/integration_tests/data/acad_table_with_blk_ref.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/data/ASCII_R12.dxf` & `ezdxf-1.1.0b1/integration_tests/data/ASCII_R12.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/data/bin_dxf_r12.dxf` & `ezdxf-1.1.0b1/integration_tests/data/bin_dxf_r12.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/data/bin_dxf_r13.dxf` & `ezdxf-1.1.0b1/integration_tests/data/bin_dxf_r13.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/data/bin_dxf_r14.dxf` & `ezdxf-1.1.0b1/integration_tests/data/bin_dxf_r14.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/data/bin_dxf_r2000.dxf` & `ezdxf-1.1.0b1/integration_tests/data/bin_dxf_r2000.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/data/cc_dxflib.dxf` & `ezdxf-1.1.0b1/integration_tests/data/cc_dxflib.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/data/custom_blocks.dxf` & `ezdxf-1.1.0b1/integration_tests/data/custom_blocks.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/data/duplicate_handles.dxf` & `ezdxf-1.1.0b1/integration_tests/data/duplicate_handles.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/data/dxf_unicode.dxf` & `ezdxf-1.1.0b1/integration_tests/data/dxf_unicode.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/data/empty_handles.dxf` & `ezdxf-1.1.0b1/integration_tests/data/empty_handles.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/data/groups.dxf` & `ezdxf-1.1.0b1/integration_tests/data/groups.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/data/Leica_Disto_S910.dxf` & `ezdxf-1.1.0b1/integration_tests/data/Leica_Disto_S910.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/data/MODEL.dxf` & `ezdxf-1.1.0b1/integration_tests/data/MODEL.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/data/mtext_columns_R2007.dxf` & `ezdxf-1.1.0b1/integration_tests/data/mtext_columns_R2007.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/data/mtext_columns_R2018.dxf` & `ezdxf-1.1.0b1/integration_tests/data/mtext_columns_R2018.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/data/mtext_framed_columns.dxf` & `ezdxf-1.1.0b1/integration_tests/data/mtext_framed_columns.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/data/mtext_text_frame.dxf` & `ezdxf-1.1.0b1/integration_tests/data/mtext_text_frame.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/data/no_layouts.dxf` & `ezdxf-1.1.0b1/integration_tests/data/no_layouts.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/data/POLI-ALL210_12.DXF` & `ezdxf-1.1.0b1/integration_tests/data/POLI-ALL210_12.DXF`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/data/recover01.dxf` & `ezdxf-1.1.0b1/integration_tests/data/recover01.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/data/recover02.dxf` & `ezdxf-1.1.0b1/integration_tests/data/recover02.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/data/small_r13.dxf` & `ezdxf-1.1.0b1/integration_tests/data/small_r13.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/data/small_r14.dxf` & `ezdxf-1.1.0b1/integration_tests/data/small_r14.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/data/XRECORD_0.bin` & `ezdxf-1.1.0b1/integration_tests/data/XRECORD_0.bin`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/data/XRECORD_1.bin` & `ezdxf-1.1.0b1/integration_tests/data/XRECORD_1.bin`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/integration_tests/data/XRECORD_2.bin` & `ezdxf-1.1.0b1/integration_tests/data/XRECORD_2.bin`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/appsettings.py` & `ezdxf-1.1.0b1/src/ezdxf/appsettings.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/audit.py` & `ezdxf-1.1.0b1/src/ezdxf/audit.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/bbox.py` & `ezdxf-1.1.0b1/src/ezdxf/bbox.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/blkrefs.py` & `ezdxf-1.1.0b1/src/ezdxf/blkrefs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/colors.py` & `ezdxf-1.1.0b1/src/ezdxf/colors.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/commands.py` & `ezdxf-1.1.0b1/src/ezdxf/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -645,28 +645,32 @@
             help="factory reset, delete default config files 'ezdxf.ini'",
         )
 
     @staticmethod
     def run(args):
         from ezdxf import options
 
+        action = False
         if args.reset:
             options.reset()
             options.delete_default_config_files()
+            action = True
         if args.home:
             options.write_home_config()
-        if args.print:
-            options.print()
+            action = True
         if args.write:
+            action = True
             filepath = Path(args.write).expanduser()
             try:
                 options.write_file(str(filepath))
                 print(f"configuration written to: {filepath}")
             except IOError as e:
                 print(str(e))
+        if args.print or action is False:
+            options.print()
 
 
 def load_every_document(filename: str):
     def io_error() -> str:
         msg = f'Not a DXF file or a generic I/O error: "{filename}"'
         print(msg, file=sys.stderr)
         return msg
```

## Comparing `ezdxf-1.1.0b0/src/ezdxf/comments.py` & `ezdxf-1.1.0b1/src/ezdxf/comments.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/disassemble.py` & `ezdxf-1.1.0b1/src/ezdxf/disassemble.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright (c) 2021-2022, Manfred Moitzi
+#  Copyright (c) 2021-2023, Manfred Moitzi
 #  License: MIT License
 from __future__ import annotations
 from typing import Iterable, Optional, cast, TYPE_CHECKING
 import abc
 import math
 from ezdxf.entities import DXFEntity, Insert, get_font_name
 
@@ -16,15 +16,15 @@
 from ezdxf.tools.text import (
     TextLine,
     unified_alignment,
     plain_text,
     text_wrap,
     estimate_mtext_content_extents,
 )
-from ezdxf.tools import fonts
+from ezdxf.fonts import fonts
 
 if TYPE_CHECKING:
     from ezdxf.entities import LWPolyline, Polyline, MText, Text
 
 __all__ = [
     "make_primitive",
     "recursive_decompose",
```

## Comparing `ezdxf-1.1.0b0/src/ezdxf/document.py` & `ezdxf-1.1.0b1/src/ezdxf/document.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/dwginfo.py` & `ezdxf-1.1.0b1/src/ezdxf/dwginfo.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entitydb.py` & `ezdxf-1.1.0b1/src/ezdxf/entitydb.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/enums.py` & `ezdxf-1.1.0b1/src/ezdxf/enums.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/explode.py` & `ezdxf-1.1.0b1/src/ezdxf/explode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/eztypes.py` & `ezdxf-1.1.0b1/src/ezdxf/eztypes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/filemanagement.py` & `ezdxf-1.1.0b1/src/ezdxf/filemanagement.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,11 +265,12 @@
 ) -> str:
     """Find file `filename` in the support directories`."""
     if pathlib.Path(filename).exists():
         return filename
     if support_dirs is None:
         support_dirs = []
     for directory in support_dirs:
+        directory = directory.strip("\"'")
         filepath = pathlib.Path(directory).expanduser() / filename
         if filepath.exists():
             return str(filepath)
     return filename
```

## Comparing `ezdxf-1.1.0b0/src/ezdxf/gfxattribs.py` & `ezdxf-1.1.0b1/src/ezdxf/gfxattribs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/graphicsfactory.py` & `ezdxf-1.1.0b1/src/ezdxf/graphicsfactory.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/groupby.py` & `ezdxf-1.1.0b1/src/ezdxf/groupby.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/npshapes.py` & `ezdxf-1.1.0b1/src/ezdxf/npshapes.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,65 +1,79 @@
 #  Copyright (c) 2023, Manfred Moitzi
 #  License: MIT License
 from __future__ import annotations
 from typing import Iterable
+import abc
+
 import numpy as np
-from ezdxf.math import BoundingBox2d, Matrix44, Vec2, Vec3
+from ezdxf.math import Matrix44, Vec2, UVec
 from ezdxf.path import AbstractPath, Path2d, Command
 
-__all__ = ["NumpyPath", "NumpyPolyline"]
+__all__ = ["NumpyPath2d", "NumpyPoints2d", "NumpyShapesException", "EmptyShapeError"]
+
+
+class NumpyShapesException(Exception):
+    pass
+
+
+class EmptyShapeError(NumpyShapesException):
+    pass
 
 
-class _NumpyShape:
+class _NumpyShape2d(abc.ABC):
     """This is an optimization to store many 2D paths and polylines in a compact way
     without sacrificing basic functions like transformation and bounding box calculation.
     """
 
     _vertices: np.ndarray
 
-    def bbox(self) -> BoundingBox2d:
-        """Returns the 2d bounding box of the shape vertices."""
-        return BoundingBox2d((self._vertices.min(0), self._vertices.max(0)))
+    def extents(self) -> tuple[Vec2, Vec2]:
+        """Returns the extents of the bounding box as tuple (extmin, extmax)."""
+        v = self._vertices
+        if len(v) > 0:
+            return Vec2(v.min(0)), Vec2(v.max(0))
+        else:
+            raise EmptyShapeError("empty shape has no extends")
 
-    def transform_inplace(self, m: Matrix44 | np.ndarray) -> None:
+    def transform_inplace(self, m: Matrix44) -> None:
         """Transforms the vertices of the shape inplace."""
-        if isinstance(m, Matrix44):
-            m = np.array(m.get_2d_transformation(), dtype=np.double)
-            m.shape = (3, 3)
         v = self._vertices
-        v = np.matmul(np.concatenate((v, np.ones((v.shape[0], 1))), axis=1), m)
-        self._vertices = v[:, :-1]
+        if len(v) == 0:
+            return
+        m.transform_array_inplace(v, 2)
 
     def vertices(self) -> list[Vec2]:
         """Returns the shape vertices as list of :class:`Vec2`."""
         return Vec2.list(self._vertices)
 
 
-class NumpyPolyline(_NumpyShape):
-    """Represents a 2D Polyline, the polyline vertices are stored as a numpy array.
-    Optimized for compactness not for speed.
-    """
+class NumpyPoints2d(_NumpyShape2d):
+    """Represents an array of 2D points stored as a ndarray."""
 
-    def __init__(self, polyline: Iterable[Vec2 | Vec3]):
-        self._vertices = np.array(Vec2.list(polyline), dtype=np.double)
+    def __init__(self, points: Iterable[UVec]) -> None:
+        self._vertices = np.array(Vec2.list(points), dtype=np.float64)
 
-    def __len__(self):
+    def __len__(self) -> int:
         return len(self._vertices)
 
 
-class NumpyPath(_NumpyShape):
-    """Represents a 2D path, the path control vertices  and commands are stored as
-    numpy arrays. Optimized for compactness not for speed.
-    """
+class NumpyPath2d(_NumpyShape2d):
+    """Represents a 2D path, the path control vertices and commands are stored as ndarray."""
 
-    def __init__(self, path: AbstractPath):
-        self._vertices = np.array(Vec2.list(path.control_vertices()), dtype=np.double)
+    def __init__(self, path: AbstractPath) -> None:
+        vertices = Vec2.list(path.control_vertices())
+        if len(vertices) == 0:
+            try:  # control_vertices() does not return start point of empty paths
+                vertices = [path.start]
+            except IndexError:
+                vertices = [Vec2()]  # default start point of empty paths
+        self._vertices = np.array(vertices, dtype=np.float64)
         self._commands = np.array(path.command_codes(), dtype=np.int8)
 
-    def __len__(self):
+    def __len__(self) -> int:
         return len(self._commands)
 
     def to_path2d(self) -> Path2d:
         v = self._vertices
         if len(v) == 0:
             return Path2d()
         path = Path2d(v[0])
```

## Comparing `ezdxf-1.1.0b0/src/ezdxf/protocols.py` & `ezdxf-1.1.0b1/src/ezdxf/protocols.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/proxygraphic.py` & `ezdxf-1.1.0b1/src/ezdxf/proxygraphic.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/query.py` & `ezdxf-1.1.0b1/src/ezdxf/query.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/queryparser.py` & `ezdxf-1.1.0b1/src/ezdxf/queryparser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/r12strict.py` & `ezdxf-1.1.0b1/src/ezdxf/r12strict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/recover.py` & `ezdxf-1.1.0b1/src/ezdxf/recover.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/reorder.py` & `ezdxf-1.1.0b1/src/ezdxf/reorder.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/shapefile.py` & `ezdxf-1.1.0b1/src/ezdxf/fonts/shapefile.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,47 +1,61 @@
-#  Copyright (c) 2022, Manfred Moitzi
+#  Copyright (c) 2022-2023, Manfred Moitzi
 #  License: MIT License
 
 """
 This module provides support for fonts stored as SHX and SHP files.
 (SHP is not the GIS file format!)
 
 The documentation about the SHP file format can be found at Autodesk:
 https://help.autodesk.com/view/OARX/2018/ENU/?guid=GUID-DE941DB5-7044-433C-AA68-2A9AE98A5713
 
-Using bytes for strings because no encoding is defined in of shape-files.
+Using bytes for strings because no encoding is defined in shape-files.
 
 """
 from __future__ import annotations
 from typing import (
     Sequence,
     Iterable,
     Iterator,
     Callable,
     Optional,
     Any,
     Set,
+    no_type_check,
 )
 import dataclasses
 import enum
 import math
 import pathlib
 
+from ezdxf.math import (
+    UVec,
+    Vec2,
+    ConstructionEllipse,
+    bulge_to_arc,
+    BoundingBox2d,
+    Matrix44,
+)
 from ezdxf import path
-from ezdxf.math import UVec, Vec2, Vec3, ConstructionEllipse, bulge_to_arc
+from .font_measurements import FontMeasurements
+from .glyphs import GlyphPath, Glyphs
 
 
 class ShapeFileException(Exception):
     pass
 
 
 class UnsupportedShapeFile(ShapeFileException):
     pass
 
 
+class UnsupportedShapeNumber(ShapeFileException):
+    pass
+
+
 class InvalidFontDefinition(ShapeFileException):
     pass
 
 
 class InvalidFontParameters(ShapeFileException):
     pass
 
@@ -110,14 +124,15 @@
             s = f",{num},".encode()
     if s:
         export.append(s[:-1])
     return export
 
 
 class ShapeFile:
+    """Low level representation of a SHX/SHP file."""
     def __init__(
         self,
         name: bytes,
         above: int,
         below: int,
         mode=FontMode.HORIZONTAL,
         encoding=FontEncoding.UNICODE,
@@ -216,31 +231,29 @@
             symbol = Symbol(int_num, int(byte_count), name)
             data = b"".join(record[1:])
             symbol.data = tuple(parse_codes(split_record(data)))
             if symbol.data[-1] == 0:
                 self.shapes[int_num] = symbol
             else:
                 s = record[0].decode(errors="ignore")
-                raise FileStructureError(
-                    f"file structure error at symbol <{s}>"
-                )
+                raise FileStructureError(f"file structure error at symbol <{s}>")
 
     def get_codes(self, number: int) -> Sequence[int]:
         symbol = self.shapes.get(number)
         if symbol is None:
-            return tuple()  # return codes for non-printable chars
+            raise UnsupportedShapeNumber(number)
         return symbol.data
 
-    def render_shape(self, number: int, stacked=False) -> path.Path:
+    def render_shape(self, number: int, stacked=False) -> GlyphPath:
         return render_shapes([number], self.get_codes, stacked=stacked)
 
-    def render_shapes(self, numbers: Sequence[int], stacked=False) -> path.Path:
+    def render_shapes(self, numbers: Sequence[int], stacked=False) -> GlyphPath:
         return render_shapes(numbers, self.get_codes, stacked=stacked)
 
-    def render_text(self, text: str, stacked=False) -> path.Path:
+    def render_text(self, text: str, stacked=False) -> GlyphPath:
         numbers = [ord(char) for char in text]
         return render_shapes(
             numbers, self.get_codes, stacked=stacked, reset_to_baseline=True
         )
 
     def shape_string(self, shape_number: int, as_num: int = 0) -> list[bytes]:
         return self.shapes[shape_number].export_str(as_num)
@@ -387,14 +400,15 @@
 
 
 # the old 'AutoCAD-86 shapes 1.0' format
 SHX_SHAPES_START_INDEX = 0x17
 
 
 def parse_shx_shapes(data: bytes) -> dict[int, Symbol]:
+    """SHX/SHP shape parser."""
     shapes: dict[int, Symbol] = dict()
     reader = DataReader(data, SHX_SHAPES_START_INDEX)
     if reader.u8() != 0x1A:
         raise FileStructureError("signature byte 0x1A not found")
     first_number = reader.u16()
     last_number = reader.u16()
     shape_count = reader.u16()
@@ -412,38 +426,35 @@
         try:
             name, shape_data = parse_shx_data_record(record)
         except IndexError:
             raise FileStructureError(
                 f"SHX parsing error shape *{shape_number:05X}: {str(record)}"
             )
         byte_count = length - len(name) - 1
-        shapes[shape_number] = Symbol(
-            shape_number, byte_count, name, shape_data
-        )
+        shapes[shape_number] = Symbol(shape_number, byte_count, name, shape_data)
     if reader.read_bytes(3) != b"EOF":
         raise FileStructureError("EOF marker not found")
     return shapes
 
 
 def parse_shx_data_record(data: bytes) -> tuple[bytes, Sequence[int]]:
+    """Low level SHX/SHP shape record parser."""
     reader = DataReader(data)
     name = reader.read_str()
     codes = parse_shape_codes(reader)
     return name, codes
 
 
 # the new 'AutoCAD-86 unifont 1.0' format
 SHX_UNIFONT_START_INDEX = 0x18
 
 
 def load_shx_unifont_file_1_0(data: bytes) -> ShapeFile:
     reader = DataReader(data, SHX_UNIFONT_START_INDEX)
-    name, above, below, mode, encoding, embed = parse_shx_unifont_definition(
-        reader
-    )
+    name, above, below, mode, encoding, embed = parse_shx_unifont_definition(reader)
     shape_file = ShapeFile(
         name,
         above=above,
         below=below,
         mode=mode,
         encoding=encoding,
         embed=embed,
@@ -452,15 +463,14 @@
         shape_file.shapes = parse_shx_unifont_shapes(reader)
     except IndexError:
         raise FileStructureError("pre-mature end of file")
     return shape_file
 
 
 def parse_shx_unifont_definition(reader: DataReader) -> Sequence[Any]:
-
     if reader.u8() != 0x1A:
         raise FileStructureError("signature byte 0x1A not found")
     reader.skip(6)
     # u16 record count: in isocp.shx = 238 (0xEE 0x00)
     #     = 1 definition record + 237 character records
     # u16 isocp.shx: 0 (0x00 0x00), always 0???
     # u16 font definition record size; isocp.shx: 52 (0x34 0x00)
@@ -578,17 +588,15 @@
     lines: Iterable[bytes],
 ) -> dict[bytes, Sequence[bytes]]:
     records: dict[bytes, Sequence[bytes]] = dict()
     name = None
     record = []
     for line in lines:
         if line.startswith(b"*BIGFONT"):
-            raise UnsupportedShapeFile(
-                "BIGFONT shape files are not supported yet"
-            )
+            raise UnsupportedShapeFile("BIGFONT shape files are not supported yet")
         if line.startswith(b"*"):
             if name is not None:
                 records[name] = tuple(record)
             name = line.split(b",")[0].strip()
             record = [line]
         else:
             record.append(line)
@@ -600,24 +608,27 @@
 
 def render_shapes(
     shape_numbers: Sequence[int],
     get_codes: Callable[[int], Sequence[int]],
     stacked: bool,
     start: UVec = (0, 0),
     reset_to_baseline=False,
-) -> path.Path:
+) -> GlyphPath:
+    """Renders multiple shapes into a single glyph path."""
     ctx = ShapeRenderer(
-        path.Path(start),
+        GlyphPath(start),
         pen_down=True,
         stacked=stacked,
         get_codes=get_codes,
     )
     for shape_number in shape_numbers:
         try:
             ctx.render(shape_number, reset_to_baseline=reset_to_baseline)
+        except UnsupportedShapeNumber:
+            pass
         except StackUnderflow:
             raise StackUnderflow(
                 f"stack underflow while rendering shape number {shape_number}"
             )
         # move cursor to the start of the next char???
     return ctx.p
 
@@ -625,33 +636,34 @@
 #        0, 1, 2,   3, 4,    5,  6,  7,  8,  9,  A,    B, C,   D, E, F
 VEC_X = [1, 1, 1, 0.5, 0, -0.5, -1, -1, -1, -1, -1, -0.5, 0, 0.5, 1, 1]
 #        0,   1, 2, 3, 4, 5, 6,   7, 8,    9,  A,  B,  C,  D,  E,    F
 VEC_Y = [0, 0.5, 1, 1, 1, 1, 1, 0.5, 0, -0.5, -1, -1, -1, -1, -1, -0.5]
 
 
 class ShapeRenderer:
+    """Low level glyph renderer for SHX/SHP fonts."""
     def __init__(
         self,
-        p: path.Path,
+        p: GlyphPath,
         get_codes: Callable[[int], Sequence[int]],
         *,
         vector_length: float = 1.0,
         pen_down: bool = True,
         stacked: bool = False,
     ):
         self.p = p
         self.vector_length = float(vector_length)  # initial vector length
         self.pen_down = pen_down
         self.stacked = stacked  # vertical stacked text
-        self._location_stack: list[Vec3] = []
+        self._location_stack: list[Vec2] = []
         self._get_codes = get_codes
         self._baseline_y = self.p.start.y
 
     @property
-    def current_location(self) -> Vec3:
+    def current_location(self) -> Vec2:
         return self.p.end
 
     def push(self) -> None:
         self._location_stack.append(self.current_location)
 
     def pop(self) -> None:
         self.p.move_to(self._location_stack.pop())
@@ -714,17 +726,15 @@
                     index += 2
                     if x == 0 and y == 0:
                         break
                     if not skip_next:
                         self.draw_displacement(x, y)
             elif code == 10:  # 10 octant arc
                 radius = codes[index]
-                start_octant, octant_span, ccw = decode_octant_specs(
-                    codes[index + 1]
-                )
+                start_octant, octant_span, ccw = decode_octant_specs(codes[index + 1])
                 if octant_span == 0:  # full circle
                     octant_span = 8
                 index += 2
                 if not skip_next:
                     self.draw_arc_span(
                         radius * self.vector_length,
                         math.radians(start_octant * 45),
@@ -737,17 +747,15 @@
                 #  This is solved by placing the end point on the baseline after
                 #  each character rendering, but only for text rendering.
                 #  The remaining problems can possibly be due to a loss of
                 #  precision when converting floats to ints.
                 start_offset = codes[index]
                 end_offset = codes[index + 1]
                 radius = (codes[index + 2] << 8) + codes[index + 3]
-                start_octant, octant_span, ccw = decode_octant_specs(
-                    codes[index + 4]
-                )
+                start_octant, octant_span, ccw = decode_octant_specs(codes[index + 4])
                 index += 5
                 if end_offset == 0:
                     end_offset = 256
                 binary_deg = 45.0 / 256.0
                 start_offset_angle = start_offset * binary_deg
                 end_offset_angle = end_offset * binary_deg
                 if ccw:
@@ -798,15 +806,15 @@
     def draw_vector(self, code: int) -> None:
         angle: int = code & 0xF
         length: int = (code >> 4) & 0xF
         self.draw_displacement(VEC_X[angle] * length, VEC_Y[angle] * length)
 
     def draw_displacement(self, x: float, y: float):
         scale = self.vector_length
-        target = self.current_location + (x * scale, y * scale)
+        target = self.current_location + Vec2(x * scale, y * scale)
         if self.pen_down:
             self.p.line_to(target)
         else:
             self.p.move_to(target)
 
     def draw_arc_span(
         self, radius: float, start_angle: float, span_angle: float, ccw: bool
@@ -824,19 +832,19 @@
             major_axis=(radius, 0),
             start_param=start_angle,
             end_param=end_angle,
             ccw=ccw,
         )
         # arc goes start -> end if ccw otherwise end -> start
         # move arc start-point to the end-point of current path
-        arc.center += self.current_location - (
+        arc.center += self.current_location - Vec2(
             arc.start_point if ccw else arc.end_point
         )
         if self.pen_down:
-            path.add_ellipse(self.p, arc, reset=False)
+            path.add_ellipse(self.p, arc, reset=False)  # type: ignore
         else:
             self.p.move_to(arc.end_point if ccw else arc.start_point)
 
     def draw_arc(
         self,
         center: Vec2,
         radius: float,
@@ -849,24 +857,24 @@
             center=center,
             major_axis=(radius, 0),
             start_param=start_param,
             end_param=end_param,
             ccw=ccw,
         )
         if self.pen_down:
-            path.add_ellipse(self.p, arc, reset=False)
+            path.add_ellipse(self.p, arc, reset=False)  # type: ignore
         else:
             self.p.move_to(arc.end_point if ccw else arc.start_point)
 
     def draw_bulge(self, x: float, y: float, bulge: float):
         if self.pen_down and bulge:
             start_point = self.current_location
             scale = self.vector_length
             ccw = bulge > 0
-            end_point = start_point + (x * scale, y * scale)
+            end_point = start_point + Vec2(x * scale, y * scale)
             bulge = abs(bulge) / 127.0
             if ccw:  # counter-clockwise
                 center, start_angle, end_angle, radius = bulge_to_arc(
                     start_point, end_point, bulge
                 )
             else:  # clockwise
                 center, start_angle, end_angle, radius = bulge_to_arc(
@@ -904,7 +912,130 @@
         shapes = readfile(shape_file_name)
     except (IOError, ShapeFileException):
         return index
     shx_symbol = shapes.find(name)
     if shx_symbol is not None:
         return shx_symbol.number
     return index
+
+
+class GlyphCache(Glyphs):
+    def __init__(self, font: ShapeFile) -> None:
+        """Text render engine for SHX/SHP fonts with integrated glyph caching."""
+        self.font: ShapeFile = font
+        self._glyph_cache: dict[int, GlyphPath] = dict()
+        self._advance_width_cache: dict[int, float] = dict()
+        self.space_width: float = self.detect_space_width()
+        self.empty_box: GlyphPath = self.get_empty_box()
+        self.font_measurements: FontMeasurements = self._get_font_measurements()
+
+    def get_scaling_factor(self, cap_height: float) -> float:
+        try:
+            return cap_height / self.font_measurements.cap_height
+        except ZeroDivisionError:
+            return 1.0
+
+    def detect_space_width(self) -> float:
+        if 32 not in self.font.shapes:
+            return self.get_shape(65).end.x  # width of "A"
+        space = self.get_shape(32)
+        return space.end.x
+
+    def get_empty_box(self) -> GlyphPath:
+        glyph_A = self.get_shape(65)
+        box = BoundingBox2d(glyph_A.control_vertices())
+        height = box.size.y
+        width = box.size.x
+        start = glyph_A.start
+        p = GlyphPath(start)
+        p.line_to(start + Vec2(width, 0))
+        p.line_to(start + Vec2(width, height))
+        p.line_to(start + Vec2(0, height))
+        p.close()
+        p.move_to(glyph_A.end)
+        return p
+
+    def _render_shape(self, shape_number) -> GlyphPath:
+        ctx = ShapeRenderer(
+            GlyphPath(),
+            pen_down=True,
+            stacked=False,
+            get_codes=self.font.get_codes,
+        )
+        try:
+            ctx.render(shape_number, reset_to_baseline=False)
+        except StackUnderflow:
+            pass
+        return ctx.p
+
+    def get_shape(self, shape_number: int) -> GlyphPath:
+        try:
+            return self._glyph_cache[shape_number]
+        except KeyError:
+            pass
+        try:
+            glyph = self._render_shape(shape_number)
+        except UnsupportedShapeNumber:
+            if shape_number < 32:
+                glyph = GlyphPath()
+            else:
+                glyph = self.empty_box
+        self._glyph_cache[shape_number] = glyph
+        self._advance_width_cache[shape_number] = glyph.end.x
+        return glyph
+
+    def get_advance_width(self, shape_number: int) -> float:
+        if shape_number == 32:
+            return self.space_width
+        try:
+            return self._advance_width_cache[shape_number]
+        except KeyError:
+            pass
+        return self.get_shape(shape_number).end.x
+
+    @no_type_check
+    def _get_font_measurements(self) -> FontMeasurements:
+        # ignore last move_to command, which places the pen at the start of the
+        # following glyph
+        bbox = BoundingBox2d(self.get_shape(ord("x")).control_vertices()[:-1])
+        baseline = bbox.extmin.y
+        x_height = bbox.extmax.y - baseline
+
+        cap_height = self.font.above
+        if cap_height == 0:
+            bbox = BoundingBox2d(self.get_shape(ord("A")).control_vertices()[:-1])
+            cap_height = bbox.extmax.y - baseline
+        descender_height = self.font.below
+        if descender_height == 0:
+            bbox = BoundingBox2d(self.get_shape(ord("p")).control_vertices()[:-1])
+            descender_height = baseline - bbox.extmin.y
+        return FontMeasurements(
+            baseline=baseline,
+            cap_height=cap_height,
+            x_height=x_height,
+            descender_height=descender_height,
+        )
+
+    def get_text_length(
+        self, text: str, cap_height: float, width_factor: float = 1.0
+    ) -> float:
+        scaling_factor = self.get_scaling_factor(cap_height) * width_factor
+        return sum(self.get_advance_width(ord(c)) for c in text) * scaling_factor
+
+    def get_text_path(
+        self, text: str, cap_height: float, width_factor: float = 1.0
+    ) -> GlyphPath:
+        p = GlyphPath()
+        sy = self.get_scaling_factor(cap_height)
+        sx = sy * width_factor
+        m = Matrix44.scale(sx, sy, 1)
+        current_location = 0.0
+        for c in text:
+            shape_number = ord(c)
+            if shape_number > 32:
+                glyph = self.get_shape(shape_number)
+                m[3, 0] = current_location
+                p.extend_multi_path(glyph.transform(m))
+            current_location += self.get_advance_width(shape_number) * sx
+        if not p.end.isclose((current_location, 0)):
+            p.move_to((current_location, 0))
+        return p
```

## Comparing `ezdxf-1.1.0b0/src/ezdxf/transform.py` & `ezdxf-1.1.0b1/src/ezdxf/transform.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/units.py` & `ezdxf-1.1.0b1/src/ezdxf/units.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/upright.py` & `ezdxf-1.1.0b1/src/ezdxf/upright.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/urecord.py` & `ezdxf-1.1.0b1/src/ezdxf/urecord.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/version.py` & `ezdxf-1.1.0b1/src/ezdxf/version.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,9 +20,9 @@
 # examples:
 #   major pre-release alpha 2: VERSION = "0.9.0a2"; version = (0, 9, 0, 'a2')
 #   major release candidate 0: VERSION = "0.9.0rc0"; version = (0, 9, 0, 'rc0')
 #   major release: VERSION = "0.9.0"; version = (0, 9, 0, 'release')
 #   1. bug fix release beta0: VERSION = "0.9.1b0"; version = (0, 9, 1, 'b0')
 #   2. bug fix release: VERSION = "0.9.2"; version = (0, 9, 2, 'release')
 
-version = (1, 0, 4, "b0")
-__version__ = "1.1.0b0"
+version = (1, 1, 0, "b1")
+__version__ = "1.1.0b1"
```

## Comparing `ezdxf-1.1.0b0/src/ezdxf/xref.py` & `ezdxf-1.1.0b1/src/ezdxf/xref.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/zoom.py` & `ezdxf-1.1.0b1/src/ezdxf/zoom.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/_options.py` & `ezdxf-1.1.0b1/src/ezdxf/_options.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,15 +54,14 @@
 
 
 def default_config() -> ConfigParser:
     config = ConfigParser()
     config[CORE] = {
         "DEFAULT_DIMENSION_TEXT_STYLE": "OpenSansCondensed-Light",
         "TEST_FILES": "",
-        "FONT_CACHE_DIRECTORY": "",
         "SUPPORT_DIRS": "",
         "LOAD_PROXY_GRAPHICS": "true",
         "STORE_PROXY_GRAPHICS": "true",
         "LOG_UNPROCESSED_TAGS": "false",
         "FILTER_INVALID_XDATA_GROUP_CODES": "true",
         "WRITE_FIXED_META_DATA_FOR_TESTING": "false",
         "DISABLE_C_EXT": "false",
@@ -79,14 +78,16 @@
     config[OPENSCAD_ADDON] = {
         "WIN_EXEC_PATH": r'"C:\Program Files\OpenSCAD\openscad.exe"'
     }
     config[DRAWING_ADDON] = {
         # These options are just for testing scenarios!
         "TRY_PYSIDE6": "true",
         "TRY_PYQT5": "true",
+        # Order for resolving SHX fonts: 1. "t"=TrueType; 2. "s"=SHX; 3. "l"=LFF
+        "SHX_RESOLVE_ORDER": "tsl",
     }
     return config
 
 
 def config_files() -> list[Path]:
     # Loading order for config files:
     # 1. user home directory:
@@ -225,30 +226,14 @@
         self.set(
             CORE,
             "DEFAULT_DIMENSION_TEXT_STYLE",
             style,
         )
 
     @property
-    def font_cache_directory(self) -> str:
-        return os.path.expanduser(self.get(CORE, "FONT_CACHE_DIRECTORY"))
-
-    @font_cache_directory.setter
-    def font_cache_directory(self, dirname: Union[str, Path]) -> None:
-        p = Path(dirname).expanduser()
-        if p.exists():
-            absolute = p.absolute()
-            if p.is_dir():
-                self.set(CORE, "FONT_CACHE_DIRECTORY", str(absolute))
-            else:
-                raise ValueError(f'"{absolute}" is not a directory')
-        else:
-            raise ValueError(f'directory "{dirname}" does not exist')
-
-    @property
     def support_dirs(self) -> Sequence[str]:
         return self.get(CORE, "SUPPORT_DIRS", "").split(DIR_SEPARATOR)
 
     @support_dirs.setter
     def support_dirs(self, support_dirs: Sequence[str]) -> None:
         self.set(CORE, "SUPPORT_DIRS", DIR_SEPARATOR.join(support_dirs))
```

## Comparing `ezdxf-1.1.0b0/src/ezdxf/__init__.py` & `ezdxf-1.1.0b1/src/ezdxf/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from ezdxf.filemanagement import readzip, new, read, readfile, decode_base64
 from ezdxf.tools.standards import (
     setup_linetypes,
     setup_styles,
     setup_dimstyles,
     setup_dimstyle,
 )
-from ezdxf.tools import pattern, fonts
+from ezdxf.tools import pattern
 from ezdxf.render.arrows import ARROWS
 from ezdxf.lldxf.const import (
     DXFError,
     DXFStructureError,
     DXFVersionError,
     DXFTableEntryError,
     DXFAppDataError,
@@ -64,21 +64,18 @@
     decode_dxf_unicode,
 )
 
 # setup DXF unicode encoder -> '\U+nnnn'
 codecs.register_error("dxfreplace", dxf_backslash_replace)
 
 EZDXF_TEST_FILES = options.test_files
-
 YES_NO = {True: "yes", False: "no"}
 
 
-def print_config(
-    verbose: bool = False, stream: Optional[TextIO] = None
-) -> None:
+def print_config(verbose: bool = False, stream: Optional[TextIO] = None) -> None:
     from pathlib import Path
 
     if stream is None:
         stream = sys.stdout
     stream.writelines(
         [
             f"ezdxf {__version__} from {Path(__file__).parent}\n",
```

## Comparing `ezdxf-1.1.0b0/src/ezdxf/__main__.py` & `ezdxf-1.1.0b1/src/ezdxf/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-#  Copyright (c) 2021, Manfred Moitzi
+#  Copyright (c) 2021-2023, Manfred Moitzi
 #  License: MIT License
 import sys
 import argparse
 from pathlib import Path
 from ezdxf import options, print_config
 from ezdxf import commands
-from ezdxf.tools import fonts
+from ezdxf.fonts import fonts
 
 YES_NO = {True: "yes", False: "no"}
 options.set(options.CORE, "LOAD_PROXY_GRAPHICS", "true")
 
 
 def add_common_arguments(parser):
     parser.add_argument(
```

## Comparing `ezdxf-1.1.0b0/src/ezdxf/acc/bezier3p.pyx` & `ezdxf-1.1.0b1/src/ezdxf/acc/bezier3p.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/acc/bezier4p.pyx` & `ezdxf-1.1.0b1/src/ezdxf/acc/bezier4p.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/acc/bspline.pyx` & `ezdxf-1.1.0b1/src/ezdxf/acc/bspline.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/acc/construct.pyx` & `ezdxf-1.1.0b1/src/ezdxf/acc/construct.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/acc/linetypes.pyx` & `ezdxf-1.1.0b1/src/ezdxf/acc/linetypes.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/acc/mapbox_earcut.pyx` & `ezdxf-1.1.0b1/src/ezdxf/acc/mapbox_earcut.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/acc/matrix44.pyx` & `ezdxf-1.1.0b1/src/ezdxf/acc/matrix44.pyx`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # cython: language_level=3
 # distutils: language = c++
-# Copyright (c) 2020-2021, Manfred Moitzi
+# Copyright (c) 2020-2023, Manfred Moitzi
 # License: MIT License
 from typing import Sequence, Iterable, Tuple, TYPE_CHECKING, Iterator
 from itertools import chain
 import math
+import numpy as np
+import cython
+
 from .vector cimport (
 Vec2, Vec3, v3_normalize, v3_isclose, v3_cross, v3_dot,
 )
 from .vector import X_AXIS, Y_AXIS, Z_AXIS, NULLVEC
 
 from libc.math cimport fabs, sin, cos, tan
 
@@ -580,14 +583,32 @@
             res = Vec2(pnt)
             x = res.x
             y = res.y
             res.x = x * m0 + y * m4 + m12
             res.y = x * m1 + y * m5 + m13
             yield res
 
+    def transform_array_inplace(self, array: np.ndarray, ndim: int) -> None:
+        """Transforms a numpy array inplace, the argument `ndim` defines the dimensions
+        to transform, this allows 2D/3D transformation on arrays with more columns
+        e.g. a polyline array which stores points as (x, y, start_width, end_width,
+        bulge) values.
+
+        """
+        cdef int _ndim = ndim
+        if _ndim == 2:
+            assert array.shape[1] > 1
+            transform_2d_array_inplace(self.m, array, array.shape[0])
+        elif _ndim == 3:
+            assert array.shape[1] > 2
+            transform_3d_array_inplace(self.m, array, array.shape[0])
+        else:
+            raise ValueError("ndim has to be 2 or 3")
+
+
     def transform_directions(
         self, vectors: Iterable[UVec], normalize=False
     ) -> Iterator[Vec3]:
         cdef double *m = self.m
         cdef Vec3 res
         cdef double x, y, z
         cdef bint _normalize = normalize
@@ -615,7 +636,41 @@
 
         res.x = x * m[0] + y * m[1] + z * m[2]
         res.y = x * m[4] + y * m[5] + z * m[6]
         res.z = x * m[8] + y * m[9] + z * m[10]
         return res
 
     ocs_from_wcs = ucs_direction_from_wcs
+
+
+@cython.boundscheck(False)
+@cython.wraparound(False)
+cdef void transform_2d_array_inplace(double *m, double [:, ::1] array, Py_ssize_t size):
+    cdef double m0 = m[0]
+    cdef double m1 = m[1]
+    cdef double m4 = m[4]
+    cdef double m5 = m[5]
+    cdef double m12 = m[12]
+    cdef double m13 = m[13]
+    cdef double x, y
+    cdef Py_ssize_t i
+
+    for i in range(size):
+        x = array[i, 0]
+        y = array[i, 1]
+        array[i, 0] = x * m0 + y * m4 + m12
+        array[i, 1] = x * m1 + y * m5 + m13
+
+@cython.boundscheck(False)
+@cython.wraparound(False)
+cdef void transform_3d_array_inplace(double *m, double [:, ::1] array, Py_ssize_t size):
+    cdef double x, y, z
+    cdef Py_ssize_t i
+
+    for i in range(size):
+        x = array[i, 0]
+        y = array[i, 1]
+        z = array[i, 2]
+
+        array[i, 0] = x * m[0] + y * m[4] + z * m[8] + m[12]
+        array[i, 1] = x * m[1] + y * m[5] + z * m[9] + m[13]
+        array[i, 2] = x * m[2] + y * m[6] + z * m[10] + m[14]
```

## Comparing `ezdxf-1.1.0b0/src/ezdxf/acc/vector.pxd` & `ezdxf-1.1.0b1/src/ezdxf/acc/vector.pxd`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/acc/vector.pyx` & `ezdxf-1.1.0b1/src/ezdxf/acc/vector.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_cubic_bezier.cpp` & `ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_cubic_bezier.cpp`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_cubic_bezier.hpp` & `ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_cubic_bezier.hpp`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_quad_bezier.cpp` & `ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_quad_bezier.cpp`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_vec3.hpp` & `ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_vec3.hpp`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_vec3.pxd` & `ezdxf-1.1.0b1/src/ezdxf/acc/_cpp_vec3.pxd`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/acc/__init__.py` & `ezdxf-1.1.0b1/src/ezdxf/acc/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/acis/abstract.py` & `ezdxf-1.1.0b1/src/ezdxf/acis/abstract.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/acis/api.py` & `ezdxf-1.1.0b1/src/ezdxf/acis/api.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/acis/const.py` & `ezdxf-1.1.0b1/src/ezdxf/acis/const.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/acis/dbg.py` & `ezdxf-1.1.0b1/src/ezdxf/acis/dbg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/acis/dxf.py` & `ezdxf-1.1.0b1/src/ezdxf/acis/dxf.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/acis/entities.py` & `ezdxf-1.1.0b1/src/ezdxf/acis/entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/acis/hdr.py` & `ezdxf-1.1.0b1/src/ezdxf/acis/hdr.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/acis/mesh.py` & `ezdxf-1.1.0b1/src/ezdxf/acis/mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/acis/sab.py` & `ezdxf-1.1.0b1/src/ezdxf/acis/sab.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/acis/sat.py` & `ezdxf-1.1.0b1/src/ezdxf/acis/sat.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/acadctb.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/acadctb.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/binpacking.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/binpacking.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/dimlines.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/dimlines.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/dxf2code.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/dxf2code.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/genetic_algorithm.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/genetic_algorithm.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/geo.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/geo.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/gerber_D6673.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/gerber_D6673.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/importer.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/importer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/iterdxf.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/iterdxf.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/menger_sponge.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/menger_sponge.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/meshex.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/meshex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/mtextsurrogate.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/mtextsurrogate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/mtxpl.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/mtxpl.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import ezdxf
 from ezdxf.entities import MText, DXFGraphic, Textstyle
 from ezdxf.enums import TextEntityAlignment
 
 # from ezdxf.layouts import BaseLayout
 from ezdxf.document import Drawing
 from ezdxf.math import Matrix44
-from ezdxf.tools import text_layout as tl, fonts
+from ezdxf.fonts import fonts
+from ezdxf.tools import text_layout as tl
 from ezdxf.tools.text import MTextContext
 from ezdxf.render.abstract_mtext_renderer import AbstractMTextRenderer
 
 if TYPE_CHECKING:
     from ezdxf.eztypes import GenericLayoutType
 
 __all__ = ["MTextExplode"]
@@ -355,15 +356,15 @@
             try:
                 text_styles.add_entry(style)
             except ezdxf.DXFTableEntryError:
                 pass
 
     def make_required_style_table_entries(self) -> list[Textstyle]:
         def ttf_path(font_face: fonts.FontFace) -> str:
-            ttf = font_face.ttf
+            ttf = font_face.filename
             if not ttf:
                 ttf = fonts.find_font_file_name(font_face)
             else:
                 # remapping SHX replacement fonts to SHX fonts,
                 # like "txt_____.ttf" to "TXT.SHX":
                 shx = fonts.map_ttf_to_shx(ttf)
                 if shx:
```

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/odafc.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/odafc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/openscad.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/openscad.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/pycsg.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/pycsg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/r12export.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/r12export.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/r12writer.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/r12writer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/sierpinski_pyramid.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/sierpinski_pyramid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/tablepainter.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/tablepainter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/text2path.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/text2path.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-#  Copyright (c) 2021-2022, Manfred Moitzi
+#  Copyright (c) 2021-2023, Manfred Moitzi
 #  License: MIT License
 from __future__ import annotations
 from typing import Union
 import enum
 
 from ezdxf.entities import Text, Attrib, Hatch, DXFGraphic
 from ezdxf.lldxf import const
 from ezdxf.enums import TextEntityAlignment, MAP_TEXT_ENUM_TO_ALIGN_FLAGS
 from ezdxf.math import Matrix44, BoundingBox
 from ezdxf import path
 from ezdxf.path import Path
-from ezdxf.tools import fonts
-from ezdxf.tools.ttfonts import TTFontRenderer
+from ezdxf.fonts import fonts
 from ezdxf.query import EntityQuery
 
 __all__ = [
     "make_path_from_str",
     "make_paths_from_str",
     "make_hatches_from_str",
     "make_path_from_entity",
@@ -51,22 +50,22 @@
             default is :attr:`LEFT`
          length: target length for the :attr:`ALIGNED` and :attr:`FIT` alignments
          m: transformation :class:`~ezdxf.math.Matrix44`
 
     """
     if len(s) == 0:
         return Path()
-    render_engine = get_render_engine(font)
+    abstract_font = get_font(font)
     # scale font rendering units to drawing units:
-    p = _str_to_path(s, render_engine, size)
+    p = _str_to_path(s, abstract_font, size)
     bbox = path.bbox([p], fast=True)
 
     # Text is rendered in drawing units,
     # therefore do alignment in drawing units:
-    draw_units_fm = render_engine.font_measurements.scale_from_baseline(size)
+    draw_units_fm = abstract_font.measurements.scale_from_baseline(size)
     matrix = alignment_transformation(draw_units_fm, bbox, align, length)
     if m is not None:
         matrix *= m
     return p.transform(matrix)
 
 
 def make_paths_from_str(
@@ -96,24 +95,21 @@
     """
     if len(s) == 0:
         return []
     p = make_path_from_str(s, font, size, align, length, m)
     return list(p.sub_paths())
 
 
-def get_render_engine(
-    font: fonts.FontFace,
-) -> TTFontRenderer:
-    font_name = fonts.font_manager.find_font_file_name(font)
-    ttfont = fonts.font_manager.get_ttf_font(font_name)
-    return TTFontRenderer(ttfont)
+def get_font(font: fonts.FontFace) -> fonts.AbstractFont:
+    font_name = fonts.font_manager.find_font_name(font)
+    return fonts.make_font(font_name, cap_height=1.0)
 
 
-def _str_to_path(s: str, render_engine: TTFontRenderer, size: float = 1.0) -> Path:
-    return render_engine.get_text_path(s, cap_height=size).to_3d_path()
+def _str_to_path(s: str, render_engine: fonts.AbstractFont, size: float = 1.0) -> Path:
+    return render_engine.text_path_ex(s, cap_height=size).to_3d_path()
 
 
 def alignment_transformation(
     fm: fonts.FontMeasurements,
     bbox: BoundingBox,
     align: TextEntityAlignment,
     length: float,
@@ -183,25 +179,33 @@
     """Convert a single line string `s` into a list of virtual
     :class:`~ezdxf.entities.Hatch` entities.
     The text `size` is the height of the uppercase letter "X" (cap height).
     The paths are aligned about the insertion point at (0, 0).
     The HATCH entities are aligned to this insertion point. BASELINE means the
     bottom of the letter "X".
 
+    .. important::
+
+        Returns an empty list for .shx, .shp and .lff fonts a.k.a. stroke fonts.
+
     Args:
          s: text to convert
          font: font face definition as :class:`~ezdxf.tools.fonts.FontFace` object
          size: text size (cap height) in drawing units
          align: alignment as :class:`ezdxf.enums.TextEntityAlignment`,
             default is :attr:`LEFT`
          length: target length for the :attr:`ALIGNED` and :attr:`FIT` alignments
          dxfattribs: additional DXF attributes
          m: transformation :class:`~ezdxf.math.Matrix44`
 
     """
+    font_ = get_font(font)
+    if font_.font_render_type is fonts.FontRenderType.STROKE:
+        return []
+
     # HATCH is an OCS entity, transforming just the polyline paths
     # is not correct! The Hatch has to be created in the xy-plane!
     paths = make_paths_from_str(s, font, size, align, length)
     dxfattribs = dict(dxfattribs or {})
     dxfattribs.setdefault("solid_fill", 1)
     dxfattribs.setdefault("pattern_name", "SOLID")
     dxfattribs.setdefault("color", const.BYLAYER)
@@ -312,30 +316,24 @@
     entities: list[DXFGraphic] = []
 
     if kind & Kind.HATCHES:
         entities.extend(make_hatches_from_entity(entity))
     if kind & (Kind.SPLINES + Kind.LWPOLYLINES):
         paths = make_paths_from_entity(entity)
         if kind & Kind.SPLINES:
-            entities.extend(
-                path.to_splines_and_polylines(paths, dxfattribs=attribs)
-            )
+            entities.extend(path.to_splines_and_polylines(paths, dxfattribs=attribs))
         if kind & Kind.LWPOLYLINES:
             entities.extend(
-                path.to_lwpolylines(
-                    paths, extrusion=extrusion, dxfattribs=attribs
-                )
+                path.to_lwpolylines(paths, extrusion=extrusion, dxfattribs=attribs)
             )
 
     return EntityQuery(entities)
 
 
-def explode(
-    entity: AnyText, kind: int = Kind.HATCHES, target=None
-) -> EntityQuery:
+def explode(entity: AnyText, kind: int = Kind.HATCHES, target=None) -> EntityQuery:
     """Explode the text `entity` into virtual entities,
     see :func:`virtual_entities`. The source entity will be destroyed.
 
     The target layout is given by the `target` argument, if `target` is ``None``,
     the target layout is the source layout of the text entity.
 
     Returns the created DXF entities as an :class:`~ezdxf.query.EntityQuery`
```

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/xqt.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/xqt.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/acisbrowser/browser.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/acisbrowser/browser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/acisbrowser/data.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/acisbrowser/data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/browser/bookmarks.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/browser/bookmarks.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/browser/browser.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/browser/browser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/browser/data.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/browser/data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/browser/find_dialog.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/browser/find_dialog.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/browser/loader.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/browser/loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/browser/model.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/browser/model.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/browser/tags.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/browser/tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/browser/views.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/browser/views.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/drawing/backend.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/drawing/backend.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) 2020-2023, Matthew Broadway
 # License: MIT License
 from __future__ import annotations
 from abc import ABC, abstractmethod, ABCMeta
 from typing import Optional, Iterable
 
 from ezdxf.addons.drawing.config import Configuration
-from ezdxf.addons.drawing.properties import Properties
+from ezdxf.addons.drawing.properties import Properties, BackendProperties
 from ezdxf.addons.drawing.type_hints import Color
 from ezdxf.entities import DXFGraphic
 from ezdxf.math import AnyVec
 from ezdxf.path import Path, Path2d
 
 
 class BackendInterface(ABC):
@@ -17,54 +17,55 @@
 
     @abstractmethod
     def configure(self, config: Configuration) -> None:
         raise NotImplementedError
 
     @abstractmethod
     def enter_entity(self, entity: DXFGraphic, properties: Properties) -> None:
+        # gets the full DXF properties information
         raise NotImplementedError
 
     @abstractmethod
     def exit_entity(self, entity: DXFGraphic) -> None:
         raise NotImplementedError
 
     @abstractmethod
     def set_background(self, color: Color) -> None:
         raise NotImplementedError
 
     @abstractmethod
-    def draw_point(self, pos: AnyVec, properties: Properties) -> None:
+    def draw_point(self, pos: AnyVec, properties: BackendProperties) -> None:
         raise NotImplementedError
 
     @abstractmethod
-    def draw_line(self, start: AnyVec, end: AnyVec, properties: Properties) -> None:
+    def draw_line(self, start: AnyVec, end: AnyVec, properties: BackendProperties) -> None:
         raise NotImplementedError
 
     @abstractmethod
     def draw_solid_lines(
-        self, lines: Iterable[tuple[AnyVec, AnyVec]], properties: Properties
+        self, lines: Iterable[tuple[AnyVec, AnyVec]], properties: BackendProperties
     ) -> None:
         raise NotImplementedError
 
     @abstractmethod
-    def draw_path(self, path: Path | Path2d, properties: Properties) -> None:
+    def draw_path(self, path: Path | Path2d, properties: BackendProperties) -> None:
         raise NotImplementedError
 
     @abstractmethod
     def draw_filled_paths(
         self,
         paths: Iterable[Path | Path2d],
         holes: Iterable[Path | Path2d],
-        properties: Properties,
+        properties: BackendProperties,
     ) -> None:
         raise NotImplementedError
 
     @abstractmethod
     def draw_filled_polygon(
-        self, points: Iterable[AnyVec], properties: Properties
+        self, points: Iterable[AnyVec], properties: BackendProperties
     ) -> None:
         raise NotImplementedError
 
     @abstractmethod
     def clear(self) -> None:
         raise NotImplementedError
 
@@ -78,14 +79,15 @@
         self.entity_stack: list[tuple[DXFGraphic, Properties]] = []
         self.config: Configuration
 
     def configure(self, config: Configuration) -> None:
         self.config = config
 
     def enter_entity(self, entity: DXFGraphic, properties: Properties) -> None:
+        # gets the full DXF properties information
         self.entity_stack.append((entity, properties))
 
     def exit_entity(self, entity: DXFGraphic) -> None:
         e, p = self.entity_stack.pop()
         assert e is entity, "entity stack mismatch"
 
     @property
@@ -94,38 +96,38 @@
         return self.entity_stack[-1][0] if self.entity_stack else None
 
     @abstractmethod
     def set_background(self, color: Color) -> None:
         raise NotImplementedError
 
     @abstractmethod
-    def draw_point(self, pos: AnyVec, properties: Properties) -> None:
+    def draw_point(self, pos: AnyVec, properties: BackendProperties) -> None:
         """Draw a real dimensionless point, because not all backends support
         zero-length lines!
         """
         raise NotImplementedError
 
     @abstractmethod
-    def draw_line(self, start: AnyVec, end: AnyVec, properties: Properties) -> None:
+    def draw_line(self, start: AnyVec, end: AnyVec, properties: BackendProperties) -> None:
         raise NotImplementedError
 
     def draw_solid_lines(
-        self, lines: Iterable[tuple[AnyVec, AnyVec]], properties: Properties
+        self, lines: Iterable[tuple[AnyVec, AnyVec]], properties: BackendProperties
     ) -> None:
         """Fast method to draw a bunch of solid lines with the same properties."""
         # Must be overridden by the backend to gain a performance benefit.
         # This is the default implementation to ensure compatibility with
         # existing backends.
         for s, e in lines:
             if e.isclose(s):
                 self.draw_point(s, properties)
             else:
                 self.draw_line(s, e, properties)
 
-    def draw_path(self, path: Path | Path2d, properties: Properties) -> None:
+    def draw_path(self, path: Path | Path2d, properties: BackendProperties) -> None:
         """Draw an outline path (connected string of line segments and Bezier
         curves).
 
         The :meth:`draw_path` implementation is a fall-back implementation
         which approximates Bezier curves by flattening as line segments.
         Backends can override this method if better path drawing functionality
         is available for that backend.
@@ -140,15 +142,15 @@
                 self.draw_line(prev, vertex, properties)
                 prev = vertex
 
     def draw_filled_paths(
         self,
         paths: Iterable[Path | Path2d],
         holes: Iterable[Path | Path2d],
-        properties: Properties,
+        properties: BackendProperties,
     ) -> None:
         """Draw multiple filled paths (connected string of line segments and
         Bezier curves) with holes.
 
         The strategy to draw multiple paths at once was chosen, because a HATCH
         entity can contain multiple unconnected areas and the holes are not easy
         to assign to an external path.
@@ -176,15 +178,15 @@
             self.draw_filled_polygon(
                 path.flattening(distance=self.config.max_flattening_distance),
                 properties,
             )
 
     @abstractmethod
     def draw_filled_polygon(
-        self, points: Iterable[AnyVec], properties: Properties
+        self, points: Iterable[AnyVec], properties: BackendProperties
     ) -> None:
         """Fill a polygon whose outline is defined by the given points.
         Used to draw entities with simple outlines where :meth:`draw_path` may
         be an inefficient way to draw such a polygon.
         """
         raise NotImplementedError
```

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/drawing/clipper.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/drawing/clipper.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/drawing/config.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/drawing/config.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/drawing/debug_backend.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/drawing/debug_backend.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,52 @@
 #  Copyright (c) 2021-2022, Manfred Moitzi
 #  License: MIT License
 from __future__ import annotations
 from typing import Iterable
 from ezdxf.math import AnyVec
 from ezdxf.path import Path, Path2d
-from .properties import Properties
+from .properties import BackendProperties
 from .backend import Backend
 from .config import Configuration
 
 
 class BasicBackend(Backend):
     """The basic backend has no draw_path() support and approximates all curves
     by lines.
     """
 
     def __init__(self):
         super().__init__()
         self.collector = []
         self.configure(Configuration.defaults())
 
-    def draw_point(self, pos: AnyVec, properties: Properties) -> None:
+    def draw_point(self, pos: AnyVec, properties: BackendProperties) -> None:
         self.collector.append(("point", pos, properties))
 
-    def draw_line(self, start: AnyVec, end: AnyVec, properties: Properties) -> None:
+    def draw_line(
+        self, start: AnyVec, end: AnyVec, properties: BackendProperties
+    ) -> None:
         self.collector.append(("line", start, end, properties))
 
     def draw_filled_polygon(
-        self, points: Iterable[AnyVec], properties: Properties
+        self, points: Iterable[AnyVec], properties: BackendProperties
     ) -> None:
         self.collector.append(("filled_polygon", list(points), properties))
 
     def set_background(self, color: str) -> None:
         self.collector.append(("bgcolor", color))
 
     def clear(self) -> None:
         self.collector = []
 
 
 class PathBackend(BasicBackend):
-    def draw_path(self, path: Path | Path2d, properties: Properties) -> None:
+    def draw_path(self, path: Path | Path2d, properties: BackendProperties) -> None:
         self.collector.append(("path", path, properties))
+
+    def draw_filled_paths(
+        self,
+        paths: Iterable[Path | Path2d],
+        holes: Iterable[Path | Path2d],
+        properties: BackendProperties,
+    ) -> None:
+        self.collector.append(("filled_path", (tuple(paths), tuple(holes)), properties))
```

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/drawing/frontend.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/drawing/frontend.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 from ezdxf.protocols import SupportsVirtualEntities, virtual_entities
 from ezdxf.tools.text import (
     has_inline_formatting_codes,
     replace_non_printable_characters,
 )
 from ezdxf.lldxf import const
 from ezdxf.render import hatching
-from ezdxf.tools import fonts
+from ezdxf.fonts import fonts
 
 
 __all__ = ["Frontend"]
 
 
 TDispatchTable: TypeAlias = Dict[str, Callable[[DXFGraphic, Properties], None]]
 PatternKey: TypeAlias = Tuple[str, float]
@@ -757,15 +757,15 @@
 
     def __init__(self, frontend: Frontend, backend: BackendInterface):
         self.frontend = frontend
         self.backend = backend
         self.config = frontend.config
         self.pattern_cache: dict[PatternKey, Sequence[float]] = dict()
         self.text_engine = UnifiedTextRenderer()
-        self.default_font_face = self.text_engine.default_font_face
+        self.default_font_face = fonts.FontFace()
         self.clipper = ClippingRect()
         self.current_vp_scale = 1.0
 
     @property
     def vp_ltype_scale(self) -> float:
         """The linetype pattern should look the same in all viewports
         independent of the viewport scaling.
@@ -815,27 +815,27 @@
 
     def draw_point(self, pos: AnyVec, properties: Properties) -> None:
         if self.clipper.is_active:
             point = self.clipper.clip_point(pos)
             if point is None:
                 return
             pos = point
-        self.backend.draw_point(pos, properties)
+        self.backend.draw_point(pos, properties.backend_properties)
 
     def draw_line(self, start: AnyVec, end: AnyVec, properties: Properties):
         if (
             self.config.line_policy == LinePolicy.SOLID
             or len(properties.linetype_pattern) < 2  # CONTINUOUS
         ):
             if self.clipper.is_active:
                 points = self.clipper.clip_line(start, end)
                 if points:
-                    self.backend.draw_line(start, end, properties)
+                    self.backend.draw_line(start, end, properties.backend_properties)
             else:
-                self.backend.draw_line(start, end, properties)
+                self.backend.draw_line(start, end, properties.backend_properties)
         else:
             renderer = linetypes.LineTypeRenderer(self.pattern(properties))
             self.draw_solid_lines(  # including transformation
                 ((s, e) for s, e in renderer.line_segment(start, end)),
                 properties,
             )
 
@@ -845,28 +845,28 @@
         if self.clipper.is_active:
             clipped_lines: list[Sequence[AnyVec]] = []
             for start, end in lines:
                 points = self.clipper.clip_line(start, end)
                 if points:
                     clipped_lines.append(points)
             lines = clipped_lines  # type: ignore
-        self.backend.draw_solid_lines(lines, properties)
+        self.backend.draw_solid_lines(lines, properties.backend_properties)
 
     def draw_path(self, path: Path | Path2d, properties: Properties):
         if (
             self.config.line_policy == LinePolicy.SOLID
             or len(properties.linetype_pattern) < 2  # CONTINUOUS
         ):
             if self.clipper.is_active:
                 for clipped_path in self.clipper.clip_paths(
                     [path], self.config.max_flattening_distance
                 ):
-                    self.backend.draw_path(clipped_path, properties)
+                    self.backend.draw_path(clipped_path, properties.backend_properties)
                 return
-            self.backend.draw_path(path, properties)
+            self.backend.draw_path(path, properties.backend_properties)
         else:
             renderer = linetypes.LineTypeRenderer(self.pattern(properties))
             vertices = path.flattening(self.config.max_flattening_distance, segments=16)
             self.draw_solid_lines(
                 ((s, e) for s, e in renderer.line_segments(vertices)),
                 properties,
             )
@@ -882,22 +882,22 @@
             max_sagitta = self.config.max_flattening_distance
             paths = self.clipper.clip_filled_paths(
                 (p.transform(m) for p in paths), max_sagitta
             )
             holes = self.clipper.clip_filled_paths(
                 (h.transform(m) for h in holes), max_sagitta
             )
-        self.backend.draw_filled_paths(paths, holes, properties)
+        self.backend.draw_filled_paths(paths, holes, properties.backend_properties)
 
     def draw_filled_polygon(
         self, points: Iterable[AnyVec], properties: Properties
     ) -> None:
         if self.clipper.is_active:
             points = self.clipper.clip_polygon(points)
-        self.backend.draw_filled_polygon(points, properties)
+        self.backend.draw_filled_polygon(points, properties.backend_properties)
 
     def pattern(self, properties: Properties) -> Sequence[float]:
         """Get pattern - implements pattern caching."""
         if self.config.line_policy == LinePolicy.SOLID:
             scale = 0.0
         else:
             scale = properties.linetype_scale * self.vp_ltype_scale
@@ -937,15 +937,19 @@
         font_face = properties.font
         if font_face is None:
             font_face = self.default_font_face
         try:
             text_path = self.text_engine.get_text_path(text, font_face, cap_height)
         except (RuntimeError, ValueError):
             return
+        
         transformed_path = text_path.transform(transform)
+        if self.text_engine.is_stroke_font(font_face):
+            self.draw_path(transformed_path, properties)
+            return
         polygons = fast_bbox_detection(single_paths([transformed_path]))  # type: ignore
         external_paths, holes = winding_deconstruction(polygons)  # type: ignore
         if properties.filling is None:
             properties.filling = Filling()
         self.draw_filled_paths(external_paths, holes, properties)  # type: ignore
```

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/drawing/gfxproxy.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/drawing/gfxproxy.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/drawing/matplotlib.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/drawing/matplotlib.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from matplotlib.collections import LineCollection
 from matplotlib.lines import Line2D
 from matplotlib.patches import PathPatch
 from matplotlib.path import Path
 
 import ezdxf.path
 from ezdxf.addons.drawing.backend import Backend
-from ezdxf.addons.drawing.properties import Properties, LayoutProperties
+from ezdxf.addons.drawing.properties import BackendProperties, LayoutProperties
 from ezdxf.addons.drawing.type_hints import FilterFunc
 from ezdxf.addons.drawing.type_hints import Color
 from ezdxf.math import Vec3, Matrix44, AnyVec
 from ezdxf.layouts import Layout
 from .config import Configuration, HatchPolicy
 
 logger = logging.getLogger("ezdxf")
@@ -79,34 +79,34 @@
         z = self._current_z
         self._current_z += 1
         return z
 
     def set_background(self, color: Color):
         self.ax.set_facecolor(color)
 
-    def draw_point(self, pos: AnyVec, properties: Properties):
+    def draw_point(self, pos: AnyVec, properties: BackendProperties):
         """Draw a real dimensionless point."""
         color = properties.color
         self.ax.scatter(
             [pos.x],
             [pos.y],
             s=SCATTER_POINT_SIZE,
             c=color,
             zorder=self._get_z(),
         )
 
-    def get_lineweight(self, properties: Properties) -> float:
+    def get_lineweight(self, properties: BackendProperties) -> float:
         """Set lineweight_scaling=0 to use a constant minimal lineweight."""
         assert self.config.min_lineweight is not None
         return max(
             properties.lineweight * self.config.lineweight_scaling,
             self.config.min_lineweight,
         )
 
-    def draw_line(self, start: AnyVec, end: AnyVec, properties: Properties):
+    def draw_line(self, start: AnyVec, end: AnyVec, properties: BackendProperties):
         """Draws a single solid line, line type rendering is done by the
         frontend since v0.18.1
         """
         if start.isclose(end):
             # matplotlib draws nothing for a zero-length line:
             self.draw_point(start, properties)
         else:
@@ -119,15 +119,15 @@
                     zorder=self._get_z(),
                 )
             )
 
     def draw_solid_lines(
         self,
         lines: Iterable[tuple[AnyVec, AnyVec]],
-        properties: Properties,
+        properties: BackendProperties,
     ):
         """Fast method to draw a bunch of solid lines with the same properties."""
         color = properties.color
         lineweight = self.get_lineweight(properties)
         _lines = []
         point_x = []
         point_y = []
@@ -147,15 +147,15 @@
                 color=color,
                 zorder=z,
                 capstyle="butt",
             )
         )
 
     def draw_path(
-        self, path: ezdxf.path.Path | ezdxf.path.Path2d, properties: Properties
+        self, path: ezdxf.path.Path | ezdxf.path.Path2d, properties: BackendProperties
     ):
         """Draw a solid line path, line type rendering is done by the
         frontend since v0.18.1
         """
         mpl_path = ezdxf.path.to_matplotlib_path([path])
         try:
             patch = PathPatch(
@@ -170,15 +170,15 @@
         else:
             self.ax.add_patch(patch)
 
     def draw_filled_paths(
         self,
         paths: Iterable[ezdxf.path.Path | ezdxf.path.Path2d],
         holes: Iterable[ezdxf.path.Path | ezdxf.path.Path2d],
-        properties: Properties,
+        properties: BackendProperties,
     ):
         # Hatch patterns are handled by the frontend since v0.18.1
         if self.config.hatch_policy == HatchPolicy.SHOW_OUTLINE:
             return
         linewidth = 0
         oriented_paths: list[ezdxf.path.Path | ezdxf.path.Path2d] = []
         for path in paths:
@@ -204,15 +204,15 @@
                 zorder=self._get_z(),
             )
         except ValueError as e:
             logger.info(f"ignored matplotlib error in draw_filled_paths(): {str(e)}")
         else:
             self.ax.add_patch(patch)
 
-    def draw_filled_polygon(self, points: Iterable[AnyVec], properties: Properties):
+    def draw_filled_polygon(self, points: Iterable[AnyVec], properties: BackendProperties):
         self.ax.fill(
             *zip(*((p.x, p.y) for p in points)),
             color=properties.color,
             linewidth=0,
             zorder=self._get_z(),
         )
```

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/drawing/mtext_complex.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/drawing/mtext_complex.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 import math
 
 from ezdxf import colors
 from ezdxf.entities import MText
 from ezdxf.lldxf import const
 from ezdxf.math import Matrix44, Vec3, AnyVec
 from ezdxf.render.abstract_mtext_renderer import AbstractMTextRenderer
-from ezdxf.tools import text_layout as tl, fonts
+from ezdxf.fonts import fonts
+from ezdxf.tools import text_layout as tl
 from ezdxf.tools.text import MTextContext
 from .properties import Properties, RenderContext, rgb_to_hex
 from .type_hints import Color
 
 __all__ = ["complex_mtext_renderer"]
```

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/drawing/properties.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/drawing/properties.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # Copyright (c) 2020-2021, Matthew Broadway
-# Copyright (c) 2020-2022, Manfred Moitzi
+# Copyright (c) 2020-2023, Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
 from typing import (
     TYPE_CHECKING,
     Optional,
     Union,
     cast,
     Sequence,
     Callable,
     Iterable,
+    NamedTuple,
 )
 import re
 import copy
 
 from ezdxf import options
 from ezdxf.addons import acadctb
 from ezdxf.addons.drawing.config import Configuration
@@ -32,24 +33,25 @@
 )
 from ezdxf.entities.ltype import CONTINUOUS_PATTERN
 from ezdxf.entities.polygon import DXFPolygon
 from ezdxf.enums import InsertUnits, Measurement
 from ezdxf.filemanagement import find_support_file
 from ezdxf.lldxf import const
 from ezdxf.lldxf.validator import make_table_key as layer_key
-from ezdxf.tools import fonts
+from ezdxf.fonts import fonts
 from ezdxf.tools.pattern import scale_pattern, HatchPatternType
 
 if TYPE_CHECKING:
     from ezdxf.document import Drawing
     from ezdxf.sections.table import Table
     from ezdxf.layouts import Layout
 
 __all__ = [
     "Properties",
+    "BackendProperties",
     "LayerProperties",
     "LayoutProperties",
     "RenderContext",
     "layer_key",
     "is_valid_color",
     "rgb_to_hex",
     "hex_to_rgb",
@@ -84,78 +86,67 @@
         # Gradient- or pattern name
         self.name: str = "SOLID"
         # Gradient- or pattern angle
         self.angle: float = 0.0  # in degrees
         self.gradient_color1: Optional[Color] = None
         self.gradient_color2: Optional[Color] = None
         self.gradient_centered: float = 0.0  # todo: what's the meaning?
-        # TODO: remove HATCH pattern definition, backends do not
-        #   render hatch patterns since v0.18.1:
         self.pattern_scale: float = 1.0
         self.pattern: HatchPatternType = []
 
 
 class Properties:
     """An implementation agnostic representation of DXF entity properties like
     color and linetype. These properties represent the actual values after
     resolving all DXF specific rules like "by layer", "by block" and so on.
     """
 
     def __init__(self) -> None:
         self.color: str = "#ffffff"  # format #RRGGBB or #RRGGBBAA
-        # Color names should be resolved into a actual color value
+        self.pen = 7  # equals the ACI (1-255), for pen based backends like plotters
 
-        # Store linetype name for backends which don't have the ability to use
-        # user-defined linetypes, but have some predefined linetypes, maybe
-        # matching most common AutoCAD linetypes is possible.
-        # Store linetype names in UPPERCASE.
+        # Linetype rendering is done by the frontend, the backend receives only solid
+        # lines.
         self.linetype_name: str = "CONTINUOUS"
 
-        # Linetypes: Complex DXF linetypes are not supported:
-        # 1. Don't know if there are any backends which can use linetypes
-        #    including text or shapes
-        # 2. No decoder for SHX files available, which are the source for
-        #    shapes in linetypes
-        # 3. SHX files are copyrighted - including in ezdxf not possible
-        #
         # Simplified DXF linetype definition:
         # all line elements >= 0.0, 0.0 = point
         # all gap elements > 0.0
         # Usage as alternating line - gap sequence: line-gap-line-gap ....
         # (line could be a point 0.0), line-line or gap-gap - makes no sense
         # Examples:
         # DXF: ("DASHED", "Dashed __ __ __ __ __ __ __ __ __ __ __ __ __ _",
         #      [0.6, 0.5, -0.1])
         # first entry 0.6 is the total pattern length = sum(linetype_pattern)
         # linetype_pattern: [0.5, 0.1] = line-gap
         # DXF: ("DASHDOTX2", "Dash dot (2x) ____  .  ____  .  ____  .  ____",
         #      [2.4, 2.0, -0.2, 0.0, -0.2])
         # linetype_pattern: [2.0, 0.2, 0.0, 0.2] = line-gap-point-gap
-        # Stored as tuple, so pattern could be used as key for caching.
-        # SVG dash-pattern does not support points, so a minimal line length
-        # (maybe inferred from linewidth?) has to be used, which may alter the
-        # overall line appearance - but linetype mapping will never be perfect.
         # The continuous pattern is an empty tuple ()
         self.linetype_pattern: Sequence[float] = CONTINUOUS_PATTERN
         self.linetype_scale: float = 1.0
         # line weight in mm, todo: default lineweight is 0.25?
         self.lineweight: float = 0.25
         self.is_visible = True
 
         # The 'layer' attribute stores the resolved layer of an entity:
         # Entities inside a block references get properties from the layer
         # of the INSERT entity, if they reside on the layer '0'.
         # To get the "real" layer of an entity, you have to use `entity.dxf.layer`
         self.layer: str = "0"
 
         # Font definition object for text entities:
-        # `None` is for the default font
-        self.font: Optional[fonts.FontFace] = None
+        # Font rendering is done by the frontend, backends receive paths for
+        # stroke-fonts (.shx) and filled paths for outline fonts (.ttf).
+        self.font: Optional[fonts.FontFace] = None  # use default font
 
         # Filling properties: Solid, Pattern, Gradient
+        # Pattern rendering is done by the frontend, backends receive only solid lines,
+        # and the fill color for filled polygons and filled paths is passed as the
+        # color attribute in the BackendProperties, gradients are not supported.
         self.filling: Optional[Filling] = None
 
         self.units = InsertUnits.Unitless
 
     def __str__(self):
         return (
             f"({self.color}, {self.linetype_name}, {self.lineweight}, "
@@ -168,14 +159,36 @@
         return hex_to_rgb(self.color[:7])  # ignore alpha if present
 
     @property
     def luminance(self) -> float:
         """Returns perceived color luminance in range [0, 1] from dark to light."""
         return luminance(self.rgb)
 
+    @property
+    def backend_properties(self) -> BackendProperties:
+        return BackendProperties(self.color, self.lineweight, self.layer, self.pen)
+
+
+class BackendProperties(NamedTuple):
+    """The backend receives a condensed version of the entity properties."""
+    color: Color = "#000000"
+    lineweight: float = 0.25  # in mm
+    layer: str = "0"  # maybe useful to group entities (SVG, PDF)
+    pen: int = 1  # equals the ACI (1-255), for pen based backends like plotters
+
+    @property
+    def rgb(self) -> RGB:
+        """Returns color as RGB tuple."""
+        return hex_to_rgb(self.color[:7])  # ignore alpha if present
+
+    @property
+    def luminance(self) -> float:
+        """Returns perceived color luminance in range [0, 1] from dark to light."""
+        return luminance(self.rgb)
+
 
 class LayerProperties(Properties):
     """Modified attribute meaning:
 
     is_visible: Whether entities belonging to this layer should be drawn
     layer: Stores real layer name (mixed case)
 
@@ -319,15 +332,18 @@
         self.linetype_scale: float = 1.0  # overall modelspace linetype scaling
         self.measurement = Measurement.Imperial
         self.pdsize: float = 0
         self.pdmode: int = 0
         self._hatch_pattern_cache: dict[str, HatchPatternType] = dict()
         self.current_layout_properties = LayoutProperties.modelspace()
         self.plot_styles = self._load_plot_style_table(self.override_ctb)
-
+        # Order for resolving SHX fonts: 1. "t"=TrueType; 2. "s"=SHX; 3. "l"=LFF
+        self.shx_resolve_order = options.get(
+            "drawing-addon", "shx_resolve_order", "tsl"
+        )
         # callable to override layer properties:
         self._layer_properties_override: Optional[LayerPropsOverride] = None
 
         if doc:
             self.set_current_layout(doc.modelspace())
             self.line_pattern = _load_line_pattern(doc.linetypes)
             self.linetype_scale = doc.header.get("$LTSCALE", 1.0)
@@ -452,14 +468,15 @@
         return vp_ctx
 
     def resolve_layer_properties(self, layer: Layer) -> LayerProperties:
         """Resolve layer properties."""
         properties = LayerProperties()
         # Store real layer name (mixed case):
         properties.layer = layer.dxf.name
+        properties.pen = layer.dxf.color
         properties.color = self._true_layer_color(layer)
 
         # set layer transparency
         alpha = transparency_to_alpha(layer.transparency)
         if alpha < 255:
             properties.color = set_color_alpha(properties.color, alpha)
 
@@ -488,15 +505,15 @@
         if font_file == "":  # Font family stored in XDATA?
             family, italic, bold = text_style.get_extended_font_data()
             if family:
                 font_face = fonts.find_best_match(
                     family=family, weight=700 if bold else 400, italic=italic
                 )
         else:
-            font_face = fonts.get_font_face(font_file, map_shx=True)
+            font_face = fonts.resolve_font_face(font_file, order=self.shx_resolve_order)
 
         if font_face is None:  # fall back to default font
             font_face = fonts.FontFace()
         self.fonts[name] = font_face
 
     def _true_layer_color(self, layer: Layer) -> Color:
         if layer.dxf.hasattr("true_color"):
@@ -553,14 +570,15 @@
     def resolve_all(self, entity: DXFGraphic) -> Properties:
         """Resolve all properties of `entity`."""
         p = Properties()
         p.layer = self.resolve_layer(entity)
         resolved_layer = layer_key(p.layer)
         p.units = self.resolve_units()
         p.color = self.resolve_color(entity, resolved_layer=resolved_layer)
+        p.pen = self.resolve_pen(entity, resolved_layer=resolved_layer)
         p.linetype_name, p.linetype_pattern = self.resolve_linetype(
             entity, resolved_layer=resolved_layer
         )
         p.lineweight = self.resolve_lineweight(entity, resolved_layer=resolved_layer)
         p.linetype_scale = self.resolve_linetype_scale(entity)
         p.is_visible = self.resolve_visible(entity, resolved_layer=resolved_layer)
         if entity.is_supported_dxf_attrib("style"):
@@ -638,14 +656,34 @@
         else:  # BYOBJECT
             color = self._true_entity_color(entity.rgb, aci)
         alpha = self._entity_alpha_str(
             entity.dxf.get("transparency"), layer_properties.color
         )
         return color[:7] + alpha
 
+    def resolve_pen(
+        self, entity: DXFGraphic, *, resolved_layer: Optional[str] = None
+    ) -> int:
+        """Resolve the aci-color of `entity` as pen number in the range of [1..255].
+        """
+        pen = entity.dxf.color  # defaults to BYLAYER
+        entity_layer = resolved_layer or layer_key(self.resolve_layer(entity))
+        layer_properties = self.layers.get(entity_layer, DEFAULT_LAYER_PROPERTIES)
+
+        if pen == const.BYLAYER:
+            pen = layer_properties.pen
+        elif pen == const.BYBLOCK:
+            if not self.inside_block_reference:
+                pen = 7
+            else:
+                pen = self.current_block_reference_properties.pen  # type: ignore
+        elif pen == const.BYOBJECT:
+            pen = 7  # ???
+        return pen
+
     def _entity_alpha_str(
         self, raw_transparency: Optional[int], layer_color: Color
     ) -> str:
         """Returns the alpha value as hex string "xx" or empty string if opaque."""
         # alpha 0 = fully transparent
         # alpha 255 = opaque
         # DXF Transparency 0 = fully transparent
```

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/drawing/pyqt.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/drawing/pyqt.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing_extensions import TypeAlias
 import math
 
 from ezdxf.addons.xqt import QtCore as qc, QtGui as qg, QtWidgets as qw
 from ezdxf.addons.drawing.backend import Backend
 from ezdxf.addons.drawing.config import Configuration
 from ezdxf.addons.drawing.type_hints import Color
-from ezdxf.addons.drawing.properties import Properties
+from ezdxf.addons.drawing.properties import BackendProperties
 from ezdxf.math import Vec3, Matrix44
 from ezdxf.path import Path, to_qpainter_path
 
 PatternKey: TypeAlias = Tuple[str, float]
 
 
 class _Point(qw.QAbstractGraphicsShapeItem):
@@ -115,15 +115,15 @@
                 qt_color = qg.QColor(f"#{alpha}{rgb}")  # '#AARRGGBB'
             else:
                 raise TypeError(color)
 
             self._color_cache[color] = qt_color
         return qt_color
 
-    def _get_pen(self, properties: Properties) -> qg.QPen:
+    def _get_pen(self, properties: BackendProperties) -> qg.QPen:
         """Returns a cosmetic pen with applied lineweight but without line type
         support.
         """
         px = (
             properties.lineweight
             / 0.3527
             * self.config.lineweight_scaling
@@ -131,20 +131,16 @@
         )
         pen = qg.QPen(self._get_color(properties.color), px)
         # Use constant width in pixel:
         pen.setCosmetic(True)
         pen.setJoinStyle(qc.Qt.RoundJoin)
         return pen
 
-    def _get_brush(self, properties: Properties) -> qg.QBrush:
-        # Hatch patterns are handled by the frontend since v0.18.1
-        filling = properties.filling
-        if filling:
-            return qg.QBrush(self._get_color(properties.color), qc.Qt.SolidPattern)  # type: ignore
-        return self._no_fill
+    def _get_fill_brush(self, color: Color) -> qg.QBrush:
+        return qg.QBrush(self._get_color(color), qc.Qt.SolidPattern)  # type: ignore
 
     def _set_item_data(self, item: qw.QGraphicsItem) -> None:
         parent_stack = tuple(e for e, props in self.entity_stack[:-1])
         current_entity = self.current_entity
         if isinstance(item, list):
             for item_ in item:
                 item_.setData(CorrespondingDXFEntity, current_entity)
@@ -152,57 +148,57 @@
         else:
             item.setData(CorrespondingDXFEntity, current_entity)
             item.setData(CorrespondingDXFParentStack, parent_stack)
 
     def set_background(self, color: Color):
         self._scene.setBackgroundBrush(qg.QBrush(self._get_color(color)))
 
-    def draw_point(self, pos: Vec3, properties: Properties) -> None:
+    def draw_point(self, pos: Vec3, properties: BackendProperties) -> None:
         """Draw a real dimensionless point."""
-        brush = qg.QBrush(self._get_color(properties.color), qc.Qt.SolidPattern)
+        brush = self._get_fill_brush(properties.color)
         item = _Point(pos.x, pos.y, brush)
         self._set_item_data(item)
         self._add_item(item)
 
-    def draw_line(self, start: Vec3, end: Vec3, properties: Properties) -> None:
+    def draw_line(self, start: Vec3, end: Vec3, properties: BackendProperties) -> None:
         # PyQt draws a long line for a zero-length line:
         if start.isclose(end):
             self.draw_point(start, properties)
         else:
             item = qw.QGraphicsLineItem(start.x, start.y, end.x, end.y)
             item.setPen(self._get_pen(properties))
             self._add_item(item)
 
     def draw_solid_lines(
         self,
         lines: Iterable[tuple[Vec3, Vec3]],
-        properties: Properties,
+        properties: BackendProperties,
     ):
         """Fast method to draw a bunch of solid lines with the same properties."""
         pen = self._get_pen(properties)
         add_line = self._add_item
         for s, e in lines:
             if s.isclose(e):
                 self.draw_point(s, properties)
             else:
                 item = qw.QGraphicsLineItem(s.x, s.y, e.x, e.y)
                 item.setPen(pen)
                 add_line(item)
 
-    def draw_path(self, path: Path, properties: Properties) -> None:
+    def draw_path(self, path: Path, properties: BackendProperties) -> None:
         item = qw.QGraphicsPathItem(to_qpainter_path([path]))
         item.setPen(self._get_pen(properties))
         item.setBrush(self._no_fill)
         self._add_item(item)
 
     def draw_filled_paths(
         self,
         paths: Iterable[Path],
         holes: Iterable[Path],
-        properties: Properties,
+        properties: BackendProperties,
     ) -> None:
         oriented_paths: list[Path] = []
         for path in paths:
             try:
                 path = path.counter_clockwise()
             except ValueError:  # cannot detect path orientation
                 continue
@@ -213,21 +209,21 @@
             except ValueError:  # cannot detect path orientation
                 continue
             oriented_paths.append(path)
         if len(oriented_paths) == 0:
             return
         item = _CosmeticPath(to_qpainter_path(oriented_paths))
         item.setPen(self._get_pen(properties))
-        item.setBrush(self._get_brush(properties))
+        item.setBrush(self._get_fill_brush(properties.color))
         self._add_item(item)
 
     def draw_filled_polygon(
-        self, points: Iterable[Vec3], properties: Properties
+        self, points: Iterable[Vec3], properties: BackendProperties
     ) -> None:
-        brush = self._get_brush(properties)
+        brush = self._get_fill_brush(properties.color)
         polygon = qg.QPolygonF()
         for p in points:
             polygon.append(qc.QPointF(p.x, p.y))
         item = _CosmeticPolygon(polygon)
         item.setPen(self._no_line)
         item.setBrush(brush)
         self._add_item(item)
@@ -235,15 +231,15 @@
     def clear(self) -> None:
         self._scene.clear()
 
     def finalize(self) -> None:
         super().finalize()
         self._scene.setSceneRect(self._scene.itemsBoundingRect())
         if self._debug_draw_rect:
-            properties = Properties()
+            properties = BackendProperties()
             properties.color = "#000000"
             self._scene.addRect(
                 self._scene.sceneRect(),
                 self._get_pen(properties),
                 self._no_fill,
             )
```

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/drawing/qtviewer.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/drawing/qtviewer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/drawing/text.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/drawing/text.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2022, Matthew Broadway
+# Copyright (c) 2020-2023, Matthew Broadway
 # License: MIT License
 from __future__ import annotations
 from typing import Union, Tuple, Iterable, Optional, Callable
 from typing_extensions import TypeAlias
 import enum
 from math import radians
 
@@ -10,16 +10,16 @@
 from ezdxf.enums import (
     TextEntityAlignment,
     MAP_TEXT_ENUM_TO_ALIGN_FLAGS,
     MTextEntityAlignment,
 )
 from ezdxf.entities import MText, Text, Attrib, AttDef
 from ezdxf.math import Matrix44, Vec3, sign
-from ezdxf.tools import fonts
-from ezdxf.tools.fonts import FontMeasurements
+from ezdxf.fonts import fonts
+from ezdxf.fonts.font_measurements import FontMeasurements
 from ezdxf.tools.text import plain_text, text_wrap
 from .text_renderer import TextRenderer
 
 """
 Search google for 'typography' or 'font anatomy' for explanations of terms like 
 'baseline' and 'x-height'
```

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/drawing/text_renderer.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/drawing/text_renderer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 #  Copyright (c) 2022-2023, Manfred Moitzi
 #  License: MIT License
 from __future__ import annotations
 from typing import TypeVar
 import abc
-from ezdxf.tools.fonts import FontFace, FontMeasurements
+from ezdxf.fonts import fonts
 from ezdxf.path import Path2d
 
 T = TypeVar("T")
 
 
 class TextRenderer(abc.ABC):
     """Minimal requirement to be usable as a universal text renderer"""
 
     @abc.abstractmethod
     def get_font_measurements(
-        self, font_face: FontFace, cap_height: float = 1.0
-    ) -> FontMeasurements:
+        self, font_face: fonts.FontFace, cap_height: float = 1.0
+    ) -> fonts.FontMeasurements:
         ...
 
     @abc.abstractmethod
     def get_text_line_width(
         self,
         text: str,
-        font_face: FontFace,
+        font_face: fonts.FontFace,
         cap_height: float = 1.0,
     ) -> float:
         ...
 
     @abc.abstractmethod
     def get_text_path(
-        self, text: str, font_face: FontFace, cap_height: float = 1.0
+        self, text: str, font_face: fonts.FontFace, cap_height: float = 1.0
     ) -> Path2d:
         ...
+
+    @abc.abstractmethod
+    def is_stroke_font(self, font_face: fonts.FontFace) -> bool:
+        ...
```

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/dwg/classes_section.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/dwg/classes_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/dwg/const.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/dwg/const.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/dwg/crc.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/dwg/crc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/dwg/fileheader.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/dwg/fileheader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/dwg/header_section.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/dwg/header_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/dwg/loader.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/dwg/loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/api.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/api.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/backend.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 #  Copyright (c) 2023, Manfred Moitzi
 #  License: MIT License
 from __future__ import annotations
 from typing import Sequence, NamedTuple, Any
 import abc
 import enum
 import math
-import numpy as np
 from .deps import (
     Vec2,
     Path,
     luminance,
     Matrix44,
     BoundingBox2d,
 )
 from .properties import Properties, Pen
-from ezdxf.npshapes import NumpyPath, NumpyPolyline
+from ezdxf.npshapes import NumpyPath2d, NumpyPoints2d
 
 # Page coordinates are always plot units:
 # 1 plot unit (plu) = 0.025mm
 # 40 plu = 1mm
 # 1016 plu = 1 inch
 # 3.39 plu = 1 dot @300 dpi
 # positive x-axis is horizontal from left to right
@@ -92,29 +91,31 @@
         """Returns the bounding box of all recorded polylines and polygons as
         :class:`~ezdxf.math.BoundingBox2d`.
         """
         if not self._bbox.has_data:
             self.update_bbox()
         return self._bbox
 
-    def update_bbox(self):
+    def update_bbox(self) -> None:
+        points: list[Vec2] = []
         for record in self.records:
             if record.type == RecordType.POLYLINE:
-                self._bbox.extend(record.data.bbox())
+                points.extend(record.data.extents())
             else:
                 for path in record.data:
-                    self._bbox.extend(path.bbox())
+                    points.extend(path.extents())
+        self._bbox = BoundingBox2d(points)
 
     def draw_polyline(self, properties: Properties, points: Sequence[Vec2]) -> None:
-        self.store(RecordType.POLYLINE, properties, NumpyPolyline(points))
+        self.store(RecordType.POLYLINE, properties, NumpyPoints2d(points))
 
     def draw_filled_polygon(
         self, properties: Properties, paths: Sequence[Path]
     ) -> None:
-        data = tuple(NumpyPath(p) for p in paths)
+        data = tuple(NumpyPath2d(p) for p in paths)
         self.store(RecordType.FILLED_POLYGON, properties, data)
 
     def store(self, record_type: RecordType, properties: Properties, args) -> None:
         prop_hash = properties.hash()
         if prop_hash not in self.properties:
             self.properties[prop_hash] = properties.copy()
         self.records.append(DataRecord(record_type, prop_hash, args))
@@ -133,24 +134,23 @@
                 paths = [p.to_path2d() for p in record.data]
                 backend.draw_filled_polygon(current_props, paths)
 
     def transform(self, m: Matrix44) -> None:
         """Transforms the recordings by a transformation matrix `m` of type
         :class:`~ezdxf.math.Matrix44`.
         """
-        np_mat = np.array(m.get_2d_transformation(), dtype=np.double)
-        np_mat.shape = (3, 3)
         for record in self.records:
             if record.type == RecordType.POLYLINE:
-                record.data.transform_inplace(np_mat)
+                record.data.transform_inplace(m)
             else:
                 for path in record.data:
-                    path.transform_inplace(np_mat)
+                    path.transform_inplace(m)
 
         if self._bbox.has_data:
+            # fast, but maybe inaccurate update
             self._bbox = BoundingBox2d(m.fast_2d_transform(self._bbox.rect_vertices()))
 
     def sort_filled_polygons(self) -> None:
         """Sort filled polygons by descending luminance (from light to dark).
 
         This also changes the plot order in the way that all filled polygons are plotted
         before the polylines.
```

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/compiler.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/compiler.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/deps.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/deps.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/dxf_backend.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/dxf_backend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/interpreter.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/interpreter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/page.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/page.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/pdf_backend.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/pdf_backend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/plotter.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/plotter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/polygon_buffer.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/polygon_buffer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/properties.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/properties.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/svg_backend.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/svg_backend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/tokenizer.py` & `ezdxf-1.1.0b1/src/ezdxf/addons/hpgl2/tokenizer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/acad_proxy_entity.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/acad_proxy_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/acad_table.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/acad_table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/acis.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/acis.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/appdata.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/appdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/appid.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/appid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/arc.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/arc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/attrib.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/attrib.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/block.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/block.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/blockrecord.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/blockrecord.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/boundary_paths.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/boundary_paths.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/circle.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/circle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/dictionary.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/dictionary.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/dimension.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/dimstyle.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/dimstyle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/dimstyleoverride.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/dimstyleoverride.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/dxfclass.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/dxfclass.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/dxfentity.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/dxfentity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/dxfgfx.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/dxfgfx.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/dxfgroups.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/dxfgroups.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/dxfns.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/dxfns.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/dxfobj.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/dxfobj.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/ellipse.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/ellipse.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/factory.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/factory.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/geodata.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/geodata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/gradient.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/gradient.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/hatch.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/hatch.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/helix.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/helix.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/idbuffer.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/idbuffer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/image.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/image.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/insert.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/insert.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/layer.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/layer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/layout.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/leader.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/leader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/light.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/light.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/line.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/ltype.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/ltype.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/lwpolyline.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/lwpolyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/material.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/material.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/mesh.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/mleader.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/mleader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/mline.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/mline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/mpolygon.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/mpolygon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/mtext.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/mtext.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/mtext_columns.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/mtext_columns.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/objectcollection.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/objectcollection.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/oleframe.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/oleframe.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/pattern.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/pattern.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/point.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/point.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/polygon.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/polygon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/polyline.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/polyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/shape.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/shape.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/solid.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/solid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/spline.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/spline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/subentity.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/subentity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/sun.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/sun.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/table.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/text.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/textstyle.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/textstyle.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from ezdxf.entities.dxfentity import base_class, SubclassProcessor, DXFEntity
 from ezdxf.entities.layer import acdb_symbol_table_record
 from .factory import register_entity
 
 if TYPE_CHECKING:
     from ezdxf.entities import DXFNamespace
     from ezdxf.lldxf.tagwriter import AbstractTagWriter
-    from ezdxf.tools.fonts import AbstractFont
+    from ezdxf.fonts import fonts
 
 __all__ = ["Textstyle"]
 logger = logging.getLogger("ezdxf")
 
 acdb_style = DefSubclass(
     "AcDbTextStyleTableRecord",
     {
@@ -210,24 +210,24 @@
         """``True`` if entry describes a shape."""
         return self.dxf.name == "" and bool(self.dxf.flags & 1)
 
     def make_font(
         self,
         cap_height: Optional[float] = None,
         width_factor: Optional[float] = None,
-    ) -> AbstractFont:
+    ) -> fonts.AbstractFont:
         """Returns a font abstraction :class:`~ezdxf.tools.fonts.AbstractFont`
         for this text style. Returns a font for a cap height of 1, if the
         text style has auto height (:attr:`Textstyle.dxf.height` is 0) and
         the given `cap_height` is ``None`` or 0.
         Uses the :attr:`Textstyle.dxf.width` attribute if the given `width_factor`
         is ``None`` or 0, the default value is 1.
         The attribute :attr:`Textstyle.dxf.big_font` is ignored.
         """
-        from ezdxf.tools import fonts
+        from ezdxf.fonts import fonts
 
         ttf = ""
         if self.has_extended_font_data:
             family, italic, bold = self.get_extended_font_data()
             if family:
                 text_style = "Italic" if italic else "Regular"
                 text_weight = 700 if bold else 400
```

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/tolerance.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/tolerance.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/ucs.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/ucs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/underlay.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/underlay.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/view.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/view.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/viewport.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/viewport.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/visualstyle.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/visualstyle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/vport.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/vport.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/xdata.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/xdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/xdict.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/xdict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/xline.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/xline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/entities/__init__.py` & `ezdxf-1.1.0b1/src/ezdxf/entities/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/layouts/base.py` & `ezdxf-1.1.0b1/src/ezdxf/layouts/base.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/layouts/blocklayout.py` & `ezdxf-1.1.0b1/src/ezdxf/layouts/blocklayout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/layouts/layout.py` & `ezdxf-1.1.0b1/src/ezdxf/layouts/layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/layouts/layouts.py` & `ezdxf-1.1.0b1/src/ezdxf/layouts/layouts.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/lldxf/attributes.py` & `ezdxf-1.1.0b1/src/ezdxf/lldxf/attributes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/lldxf/const.py` & `ezdxf-1.1.0b1/src/ezdxf/lldxf/const.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/lldxf/encoding.py` & `ezdxf-1.1.0b1/src/ezdxf/lldxf/encoding.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/lldxf/extendedtags.py` & `ezdxf-1.1.0b1/src/ezdxf/lldxf/extendedtags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/lldxf/fileindex.py` & `ezdxf-1.1.0b1/src/ezdxf/lldxf/fileindex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/lldxf/hdrvars.py` & `ezdxf-1.1.0b1/src/ezdxf/lldxf/hdrvars.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/lldxf/loader.py` & `ezdxf-1.1.0b1/src/ezdxf/lldxf/loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/lldxf/packedtags.py` & `ezdxf-1.1.0b1/src/ezdxf/lldxf/packedtags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/lldxf/repair.py` & `ezdxf-1.1.0b1/src/ezdxf/lldxf/repair.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/lldxf/tagger.py` & `ezdxf-1.1.0b1/src/ezdxf/lldxf/tagger.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/lldxf/tags.py` & `ezdxf-1.1.0b1/src/ezdxf/lldxf/tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/lldxf/tagwriter.py` & `ezdxf-1.1.0b1/src/ezdxf/lldxf/tagwriter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/lldxf/types.py` & `ezdxf-1.1.0b1/src/ezdxf/lldxf/types.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/lldxf/validator.py` & `ezdxf-1.1.0b1/src/ezdxf/lldxf/validator.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/math/arc.py` & `ezdxf-1.1.0b1/src/ezdxf/math/arc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/math/bbox.py` & `ezdxf-1.1.0b1/src/ezdxf/math/bbox.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/math/bezier.py` & `ezdxf-1.1.0b1/src/ezdxf/math/bezier.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/math/bezier_interpolation.py` & `ezdxf-1.1.0b1/src/ezdxf/math/bezier_interpolation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/math/box.py` & `ezdxf-1.1.0b1/src/ezdxf/math/box.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/math/bspline.py` & `ezdxf-1.1.0b1/src/ezdxf/math/bspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/math/bulge.py` & `ezdxf-1.1.0b1/src/ezdxf/math/bulge.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/math/circle.py` & `ezdxf-1.1.0b1/src/ezdxf/math/circle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/math/clipping.py` & `ezdxf-1.1.0b1/src/ezdxf/math/clipping.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/math/clustering.py` & `ezdxf-1.1.0b1/src/ezdxf/math/clustering.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/math/construct2d.py` & `ezdxf-1.1.0b1/src/ezdxf/math/construct2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/math/construct3d.py` & `ezdxf-1.1.0b1/src/ezdxf/math/construct3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/math/cspline.py` & `ezdxf-1.1.0b1/src/ezdxf/math/cspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/math/curvetools.py` & `ezdxf-1.1.0b1/src/ezdxf/math/curvetools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/math/ellipse.py` & `ezdxf-1.1.0b1/src/ezdxf/math/ellipse.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/math/eulerspiral.py` & `ezdxf-1.1.0b1/src/ezdxf/math/eulerspiral.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/math/linalg.py` & `ezdxf-1.1.0b1/src/ezdxf/math/linalg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/math/line.py` & `ezdxf-1.1.0b1/src/ezdxf/math/line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/math/offset2d.py` & `ezdxf-1.1.0b1/src/ezdxf/math/offset2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/math/parametrize.py` & `ezdxf-1.1.0b1/src/ezdxf/math/parametrize.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/math/perlin.py` & `ezdxf-1.1.0b1/src/ezdxf/math/perlin.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/math/polyline.py` & `ezdxf-1.1.0b1/src/ezdxf/math/polyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/math/rtree.py` & `ezdxf-1.1.0b1/src/ezdxf/math/rtree.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/math/shape.py` & `ezdxf-1.1.0b1/src/ezdxf/math/shape.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/math/surfaces.py` & `ezdxf-1.1.0b1/src/ezdxf/math/surfaces.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/math/transformtools.py` & `ezdxf-1.1.0b1/src/ezdxf/math/transformtools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/math/triangulation.py` & `ezdxf-1.1.0b1/src/ezdxf/math/triangulation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/math/ucs.py` & `ezdxf-1.1.0b1/src/ezdxf/math/ucs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/math/_bezier3p.py` & `ezdxf-1.1.0b1/src/ezdxf/math/_bezier3p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/math/_bezier4p.py` & `ezdxf-1.1.0b1/src/ezdxf/math/_bezier4p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/math/_bspline.py` & `ezdxf-1.1.0b1/src/ezdxf/math/_bspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/math/_construct.py` & `ezdxf-1.1.0b1/src/ezdxf/math/_construct.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/math/_ctypes.py` & `ezdxf-1.1.0b1/src/ezdxf/math/_ctypes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/math/_mapbox_earcut.py` & `ezdxf-1.1.0b1/src/ezdxf/math/_mapbox_earcut.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/math/_matrix44.py` & `ezdxf-1.1.0b1/src/ezdxf/math/_matrix44.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 # Author: Will McGugan
 # Download-URL: http://code.google.com/p/gameobjects/downloads/list
 # Copyright (c) 2011-2023 Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
 from typing import Sequence, Iterable, Iterator, TYPE_CHECKING, Optional
 import math
+import numpy as np
+
 from math import sin, cos, tan
 from itertools import chain
 
 # The pure Python implementation can't import from ._ctypes or ezdxf.math!
 from ._vector import Vec3, X_AXIS, Y_AXIS, Z_AXIS, NULLVEC, Vec2
 
 if TYPE_CHECKING:
@@ -613,15 +615,15 @@
             - pure Python code: ~1.6x
             - Python with C-extensions: less than 1.1x
             - PyPy 3.8: ~4.3x
 
         But speed isn't everything, returning the processed input points as :class:`Vec2`
         instances is another advantage.
 
-        .. versionadded:: 1.0.4
+        .. versionadded:: 1.1
 
         """
         m = self._matrix
         m0 = m[0]
         m1 = m[1]
         m4 = m[4]
         m5 = m[5]
@@ -629,14 +631,40 @@
         m13 = m[13]
         for pnt in points:
             v = Vec2(pnt)
             x = v.x
             y = v.y
             yield Vec2(x * m0 + y * m4 + m12, x * m1 + y * m5 + m13)
 
+    def transform_array_inplace(self, array: np.ndarray, ndim: int) -> None:
+        """Transforms a numpy array inplace, the argument `ndim` defines the dimensions
+        to transform, this allows 2D/3D transformation on arrays with more columns
+        e.g. a polyline array which stores points as (x, y, start_width, end_width,
+        bulge) values.
+
+        .. versionadded:: 1.1
+
+        """
+        # This implementation exist only for compatibility to the Cython implementation!
+        # This version is 3.4x faster than the Cython version of Matrix44.fast_2d_transform()
+        # for larger point arrays but 10.5x slower than the Cython version of this method.
+        if ndim == 2:
+            m = np.array(self.get_2d_transformation(), dtype=np.float64)
+            m.shape = (3, 3)
+        elif ndim == 3:
+            m = np.array(self._matrix, dtype=np.float64)
+            m.shape = (4, 4)
+        else:
+            raise ValueError("ndim has to be 2 or 3")
+
+        v = np.matmul(
+            np.concatenate((array[:, :ndim], np.ones((array.shape[0], 1))), axis=1), m
+        )
+        array[:, :ndim] = v[:, :ndim].copy()
+
     def transform_directions(
         self, vectors: Iterable[UVec], normalize=False
     ) -> Iterator[Vec3]:
         """Returns an iterable of transformed direction vectors without
         translation.
 
         """
```

## Comparing `ezdxf-1.1.0b0/src/ezdxf/math/_vector.py` & `ezdxf-1.1.0b1/src/ezdxf/math/_vector.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/math/__init__.py` & `ezdxf-1.1.0b1/src/ezdxf/math/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/path/commands.py` & `ezdxf-1.1.0b1/src/ezdxf/path/commands.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/path/converter.py` & `ezdxf-1.1.0b1/src/ezdxf/path/converter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/path/nesting.py` & `ezdxf-1.1.0b1/src/ezdxf/path/nesting.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/path/path.py` & `ezdxf-1.1.0b1/src/ezdxf/path/path.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/path/shapes.py` & `ezdxf-1.1.0b1/src/ezdxf/path/shapes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/path/tools.py` & `ezdxf-1.1.0b1/src/ezdxf/path/tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/pp/dxfpp.css` & `ezdxf-1.1.0b1/src/ezdxf/pp/dxfpp.css`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/pp/dxfpp.html` & `ezdxf-1.1.0b1/src/ezdxf/pp/dxfpp.html`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/pp/dxfpp.js` & `ezdxf-1.1.0b1/src/ezdxf/pp/dxfpp.js`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/pp/dxfpp.py` & `ezdxf-1.1.0b1/src/ezdxf/pp/dxfpp.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/pp/pprint.py` & `ezdxf-1.1.0b1/src/ezdxf/pp/pprint.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/pp/rawpp.css` & `ezdxf-1.1.0b1/src/ezdxf/pp/rawpp.css`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/pp/rawpp.py` & `ezdxf-1.1.0b1/src/ezdxf/pp/rawpp.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/pp/reflinks.py` & `ezdxf-1.1.0b1/src/ezdxf/pp/reflinks.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/render/abstract_mtext_renderer.py` & `ezdxf-1.1.0b1/src/ezdxf/render/abstract_mtext_renderer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-# Copyright (c) 2021-2022, Manfred Moitzi
+# Copyright (c) 2021-2023, Manfred Moitzi
 # License: MIT License
 
 # This is the abstract link between the text layout engine implemented in
 # ezdxf.tools.text_layout and a concrete MTEXT renderer implementation like
 # MTextExplode or ComplexMTextRenderer.
 from __future__ import annotations
 from typing import Sequence, Optional
 import abc
 from ezdxf.lldxf import const
 from ezdxf.entities.mtext import MText, MTextColumns
 from ezdxf.enums import (
     MTextParagraphAlignment,
 )
-from ezdxf.tools import text_layout as tl, fonts
+from ezdxf.fonts import fonts
+from ezdxf.tools import text_layout as tl
 from ezdxf.tools.text import (
     MTextParser,
     MTextContext,
     TokenType,
     ParagraphProperties,
-    AbstractFont,
     estimate_mtext_extents,
 )
 
 __all__ = ["AbstractMTextRenderer"]
 
 ALIGN = {
     MTextParagraphAlignment.LEFT: tl.ParagraphAlignment.LEFT,
@@ -122,17 +122,15 @@
         align = ALIGN.get(p.align, tl.ParagraphAlignment.LEFT)
         left = p.left * cap_height
         right = p.right * cap_height
         first = left + p.indent * cap_height  # relative to left
         _default_stops: Sequence[tl.TabStop] = default_stops or []
         tab_stops = _default_stops
         if p.tab_stops:
-            tab_stops = make_tab_stops(
-                cap_height, width, p.tab_stops, _default_stops
-            )
+            tab_stops = make_tab_stops(cap_height, width, p.tab_stops, _default_stops)
         paragraph = tl.Paragraph(
             align=align,
             indent=(first, left, right),
             line_spacing=line_spacing,
             tab_stops=tab_stops,
         )
         paragraph.append_content(cells)
@@ -163,24 +161,22 @@
     else:  # static, dynamic auto
         heights = [columns.defined_height] * columns.count
     return heights
 
 
 class AbstractMTextRenderer(abc.ABC):
     def __init__(self) -> None:
-        self._font_cache: dict[tuple[str, float, float], AbstractFont] = {}
+        self._font_cache: dict[tuple[str, float, float], fonts.AbstractFont] = {}
 
     @abc.abstractmethod
     def word(self, test: str, ctx: MTextContext) -> tl.ContentCell:
         ...
 
     @abc.abstractmethod
-    def fraction(
-        self, data: tuple[str, str, str], ctx: MTextContext
-    ) -> tl.ContentCell:
+    def fraction(self, data: tuple[str, str, str], ctx: MTextContext) -> tl.ContentCell:
         ...
 
     @abc.abstractmethod
     def get_font_face(self, mtext: MText) -> fonts.FontFace:
         ...
 
     @abc.abstractmethod
```

## Comparing `ezdxf-1.1.0b0/src/ezdxf/render/arrows.py` & `ezdxf-1.1.0b1/src/ezdxf/render/arrows.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/render/curves.py` & `ezdxf-1.1.0b1/src/ezdxf/render/curves.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/render/dimension.py` & `ezdxf-1.1.0b1/src/ezdxf/render/dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/render/dim_base.py` & `ezdxf-1.1.0b1/src/ezdxf/render/dim_base.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/render/dim_curved.py` & `ezdxf-1.1.0b1/src/ezdxf/render/dim_curved.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/render/dim_diameter.py` & `ezdxf-1.1.0b1/src/ezdxf/render/dim_diameter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/render/dim_linear.py` & `ezdxf-1.1.0b1/src/ezdxf/render/dim_linear.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/render/dim_ordinate.py` & `ezdxf-1.1.0b1/src/ezdxf/render/dim_ordinate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/render/dim_radius.py` & `ezdxf-1.1.0b1/src/ezdxf/render/dim_radius.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/render/forms.py` & `ezdxf-1.1.0b1/src/ezdxf/render/forms.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/render/hatching.py` & `ezdxf-1.1.0b1/src/ezdxf/render/hatching.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/render/leader.py` & `ezdxf-1.1.0b1/src/ezdxf/render/leader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/render/linetypes.py` & `ezdxf-1.1.0b1/src/ezdxf/render/linetypes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/render/mesh.py` & `ezdxf-1.1.0b1/src/ezdxf/render/mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/render/mleader.py` & `ezdxf-1.1.0b1/src/ezdxf/render/mleader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/render/mline.py` & `ezdxf-1.1.0b1/src/ezdxf/render/mline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/render/point.py` & `ezdxf-1.1.0b1/src/ezdxf/render/point.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/render/polyline.py` & `ezdxf-1.1.0b1/src/ezdxf/render/polyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/render/r12spline.py` & `ezdxf-1.1.0b1/src/ezdxf/render/r12spline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/render/trace.py` & `ezdxf-1.1.0b1/src/ezdxf/render/trace.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/render/_linetypes.py` & `ezdxf-1.1.0b1/src/ezdxf/render/_linetypes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/render/__init__.py` & `ezdxf-1.1.0b1/src/ezdxf/render/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/resources/16x16.png` & `ezdxf-1.1.0b1/src/ezdxf/resources/16x16.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/resources/24x24.png` & `ezdxf-1.1.0b1/src/ezdxf/resources/24x24.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/resources/256x256.png` & `ezdxf-1.1.0b1/src/ezdxf/resources/256x256.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/resources/32x32.png` & `ezdxf-1.1.0b1/src/ezdxf/resources/32x32.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/resources/48x48.png` & `ezdxf-1.1.0b1/src/ezdxf/resources/48x48.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/resources/64x64.png` & `ezdxf-1.1.0b1/src/ezdxf/resources/64x64.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/resources/icon-copy-64px.png` & `ezdxf-1.1.0b1/src/ezdxf/resources/icon-copy-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/resources/icon-find-64px.png` & `ezdxf-1.1.0b1/src/ezdxf/resources/icon-find-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/resources/icon-goto-bookmark-64px.png` & `ezdxf-1.1.0b1/src/ezdxf/resources/icon-goto-bookmark-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/resources/icon-goto-handle-64px.png` & `ezdxf-1.1.0b1/src/ezdxf/resources/icon-goto-handle-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/resources/icon-goto-line-64px.png` & `ezdxf-1.1.0b1/src/ezdxf/resources/icon-goto-line-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/resources/icon-left-arrow-64px.png` & `ezdxf-1.1.0b1/src/ezdxf/resources/icon-left-arrow-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/resources/icon-next-entity-64px.png` & `ezdxf-1.1.0b1/src/ezdxf/resources/icon-next-entity-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/resources/icon-prev-entity-64px.png` & `ezdxf-1.1.0b1/src/ezdxf/resources/icon-prev-entity-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/resources/icon-right-arrow-64px.png` & `ezdxf-1.1.0b1/src/ezdxf/resources/icon-right-arrow-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/resources/icon-show-in-tree-64px.png` & `ezdxf-1.1.0b1/src/ezdxf/resources/icon-show-in-tree-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/resources/icon-store-bookmark-64px.png` & `ezdxf-1.1.0b1/src/ezdxf/resources/icon-store-bookmark-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/sections/acdsdata.py` & `ezdxf-1.1.0b1/src/ezdxf/sections/acdsdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/sections/blocks.py` & `ezdxf-1.1.0b1/src/ezdxf/sections/blocks.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/sections/classes.py` & `ezdxf-1.1.0b1/src/ezdxf/sections/classes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/sections/entities.py` & `ezdxf-1.1.0b1/src/ezdxf/sections/entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/sections/header.py` & `ezdxf-1.1.0b1/src/ezdxf/sections/header.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/sections/headervars.py` & `ezdxf-1.1.0b1/src/ezdxf/sections/headervars.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/sections/objects.py` & `ezdxf-1.1.0b1/src/ezdxf/sections/objects.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/sections/table.py` & `ezdxf-1.1.0b1/src/ezdxf/sections/table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/sections/tables.py` & `ezdxf-1.1.0b1/src/ezdxf/sections/tables.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/tools/analyze.py` & `ezdxf-1.1.0b1/src/ezdxf/tools/analyze.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/tools/binarydata.py` & `ezdxf-1.1.0b1/src/ezdxf/tools/binarydata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/tools/codepage.py` & `ezdxf-1.1.0b1/src/ezdxf/tools/codepage.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/tools/complex_ltype.py` & `ezdxf-1.1.0b1/src/ezdxf/tools/complex_ltype.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/tools/crypt.py` & `ezdxf-1.1.0b1/src/ezdxf/tools/crypt.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/tools/debug.py` & `ezdxf-1.1.0b1/src/ezdxf/tools/debug.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/tools/difftags.py` & `ezdxf-1.1.0b1/src/ezdxf/tools/difftags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/tools/fonts.py` & `ezdxf-1.1.0b1/src/ezdxf/fonts/fonts.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,68 +1,27 @@
 #  Copyright (c) 2021-2023, Manfred Moitzi
 #  License: MIT License
-"""
-This module manages a backend agnostic font database.
-
-Weight Values: https://developer.mozilla.org/de/docs/Web/CSS/font-weight
-
-Supported by matplotlib, pyqt, SVG
-
-=========== =====
-Thin        100
-Hairline    100
-ExtraLight  200
-UltraLight  200
-Light       300
-Normal      400
-Medium      500
-DemiBold    600
-SemiBold    600
-Bold        700
-ExtraBold   800
-UltraBold   800
-Black       900
-Heavy       900
-ExtraBlack  950
-UltraBlack  950
-=========== =====
-
-Stretch Values: https://developer.mozilla.org/en-US/docs/Web/CSS/font-stretch
-
-Supported by matplotlib, SVG
-
-=============== ======
-ultra-condensed 50%
-extra-condensed 62.5%
-condensed       75%
-semi-condensed  87.5%
-normal          100%
-semi-expanded   112.5%
-expanded        125%
-extra-expanded  150%
-ultra-expanded  200%
-=============== ======
-
-"""
 from __future__ import annotations
-from typing import Optional, NamedTuple, TYPE_CHECKING, cast
+from typing import Optional, TYPE_CHECKING, cast
 import abc
+import enum
 import logging
-from pathlib import Path
-import json
-import os
+import sys
+import pathlib
 
 from ezdxf import options
 from .font_face import FontFace
-from .font_manager import FontManager
+from .font_manager import FontManager, SUPPORTED_TTF_TYPES, FontNotFoundError
+from .font_measurements import FontMeasurements
+from .glyphs import GlyphPath, Glyphs
 
 if TYPE_CHECKING:
     from ezdxf.document import Drawing
     from ezdxf.entities import DXFEntity, Textstyle
-    from .ttfonts import TTFontRenderer
+    from ezdxf.path import Path2d
 
 logger = logging.getLogger("ezdxf")
 FONT_MANAGER_CACHE_FILE = "font_manager_cache.json"
 CACHE_DIRECTORY = ".cache"
 font_manager = FontManager()
 
 SHX_FONTS = {
@@ -101,81 +60,158 @@
     "SYMAP": "symap___.ttf",
     "SYMAP.SHX": "symap___.ttf",
     "SYMETEO": "symeteo_.ttf",
     "SYMETEO.SHX": "symeteo_.ttf",
     "TXT": "txt_____.ttf",  # Default AutoCAD font
     "TXT.SHX": "txt_____.ttf",
 }
+LFF_FONTS = {
+    "TXT": "standard.lff",
+    "TXT.SHX": "standard.lff",
+}
 TTF_TO_SHX = {v: k for k, v in SHX_FONTS.items() if k.endswith("SHX")}
 DESCENDER_FACTOR = 0.333  # from TXT SHX font - just guessing
 X_HEIGHT_FACTOR = 0.666  # from TXT SHX font - just guessing
+MONOSPACE = "*monospace"  # last resort fallback font only for measurement
 
 
 def map_shx_to_ttf(font_name: str) -> str:
-    """Map SHX font names to TTF file names. e.g. "TXT" -> "txt_____.ttf" """
+    """Map .shx font names to .ttf file names. e.g. "TXT" -> "txt_____.ttf" """
     # Map SHX fonts to True Type Fonts:
     font_upper = font_name.upper()
     if font_upper in SHX_FONTS:
         font_name = SHX_FONTS[font_upper]
     return font_name
 
 
+def map_shx_to_lff(font_name: str) -> str:
+    """Map .shx font names to .lff file names. e.g. "TXT" -> "standard.lff" """
+    font_upper = font_name.upper()
+    name = LFF_FONTS.get(font_upper, "")
+    if font_manager.has_font(name):
+        return name
+    if not font_upper.endswith(".SHX"):
+        lff_name = font_name + ".lff"
+    else:
+        lff_name = font_name[:-4] + ".lff"
+    if font_manager.has_font(lff_name):
+        return lff_name
+    return font_name
+
+
 def is_shx_font_name(font_name: str) -> bool:
-    name = font_name.upper()
-    if name.endswith(".SHX"):
+    name = font_name.lower()
+    if name.endswith(".shx"):
         return True
     if "." not in name:
         return True
     return False
 
 
 def map_ttf_to_shx(ttf: str) -> Optional[str]:
-    """Map TTF file names to SHX font names. e.g. "txt_____.ttf" -> "TXT" """
+    """Maps .ttf filenames to .shx font names. e.g. "txt_____.ttf" -> "TXT" """
     return TTF_TO_SHX.get(ttf.lower())
 
 
-def build_system_font_cache(**kwargs) -> None:
+def build_system_font_cache() -> None:
     """Builds or rebuilds the font manager cache. The font manager cache has a fixed
     location in the cache directory of the users home directory "~/.cache/ezdxf" or the
     directory specified by the environment variable "XDG_CACHE_HOME".
     """
     build_font_manager_cache(_get_font_manger_path())
 
 
 def find_font_face(font_name: str) -> FontFace:
-    """Get the font face definition by the font file name e.g. "Arial.ttf",
-    returns the default font if `font_name` was not found.
+    """Returns the :class:`FontFace` definition for the given font filename
+    e.g. "LiberationSans-Regular.ttf".
 
     """
     return font_manager.get_font_face(font_name)
 
 
 def get_font_face(font_name: str, map_shx=True) -> FontFace:
-    """Get the font face definition by the font file name e.g. "Arial.ttf".
+    """Returns  the :class:`FontFace` definition for the given font filename
+    e.g. "LiberationSans-Regular.ttf".
 
     This function translates a DXF font definition by the TTF font file name into a
-    :class:`FontFace` object. Fonts which are not available on the current system gets
-    a default font face.
+    :class:`FontFace` object. Returns the :class:`FontFace` of the default font when a
+    font is not available on the current system.
 
     Args:
         font_name: raw font file name as stored in the
             :class:`~ezdxf.entities.Textstyle` entity
         map_shx: maps SHX font names to TTF replacement fonts,
             e.g. "TXT" -> "txt_____.ttf"
 
     """
     if not isinstance(font_name, str):
-        raise TypeError("ttf_path has invalid type")
+        raise TypeError("font_name has invalid type")
     if map_shx:
-        ttf_path = map_shx_to_ttf(font_name)
+        font_name = map_shx_to_ttf(font_name)
+    return find_font_face(font_name)
+
+
+def resolve_shx_font_name(font_name: str, order: str) -> str:
+    """Resolves a .shx font name, the argument `order` defines the resolve order:
+
+    - "t" = map .shx fonts to TrueType fonts (.ttf, .ttc, .otf)
+    - "s" = use shapefile fonts (.shx, .shp)
+    - "l" = map .shx fonts to LibreCAD fonts (.lff)
+
+    """
+    if len(order) == 0:
+        return font_name
+    order = order.lower()
+    for type_str in order:
+        if type_str == "t":
+            name = map_shx_to_ttf(font_name)
+            if font_manager.has_font(name):
+                return name
+        elif type_str == "s":
+            if not font_name.lower().endswith(".shx"):
+                font_name += ".shx"
+            if font_manager.has_font(font_name):
+                return font_name
+        elif type_str == "l":
+            name = map_shx_to_lff(font_name)
+            if font_manager.has_font(name):
+                return name
+    return font_name
+
+
+def resolve_font_face(font_name: str, order="tsl") -> FontFace:
+    """Returns the :class:`FontFace` definition for the given font filename
+    e.g. "LiberationSans-Regular.ttf".
+
+    This function translates a DXF font definition by the TTF font file name into a
+    :class:`FontFace` object. Returns the :class:`FontFace` of the default font when a
+    font is not available on the current system.
+
+    The order argument defines the resolve order for .shx fonts:
+
+    - "t" = map .shx fonts to TrueType fonts (.ttf, .ttc, .otf)
+    - "s" = use shapefile fonts (.shx, .shp)
+    - "l" = map .shx fonts to LibreCAD fonts (.lff)
+
+    Args:
+        font_name: raw font file name as stored in the
+            :class:`~ezdxf.entities.Textstyle` entity
+        order: resolving order
+
+    """
+    if not isinstance(font_name, str):
+        raise TypeError("font_name has invalid type")
+    if is_shx_font_name(font_name):
+        font_name = resolve_shx_font_name(font_name, order)
     return find_font_face(font_name)
 
 
 def get_font_measurements(font_name: str, map_shx=True) -> FontMeasurements:
-    """Get cached font measurements by TTF file name e.g. "Arial.ttf".
+    """Get :class:`FontMeasurements` for the given font filename
+    e.g. "LiberationSans-Regular.ttf".
 
     Args:
         font_name: raw font file name as stored in the
             :class:`~ezdxf.entities.Textstyle` entity
         map_shx: maps SHX font names to TTF replacement fonts,
             e.g. "TXT" -> "txt_____.ttf"
 
@@ -197,212 +233,158 @@
     *,
     family: str = "sans-serif",
     style: str = "Regular",
     weight: int = 400,
     width: int = 5,
     italic: Optional[bool] = False,
 ) -> Optional[FontFace]:
-    """Returns the :class:`FontFace` that matches the given properties best.
+    """Returns a :class:`FontFace` that matches the given properties best. The search
+    is based the descriptive properties and not on comparing glyph shapes.
 
     Args:
         family: font family name e.g. "sans-serif", "Liberation Sans"
         style: font style e.g. "Regular", "Italic", "Bold"
         weight: weight in the range from 1-1000 (usWeightClass)
         width: width in the range from 1-9 (usWidthClass)
         italic: ``True``, ``False`` or ``None`` to ignore this flag
 
     """
     return font_manager.find_best_match(family, style, weight, width, italic)
 
 
 def find_font_file_name(font_face: FontFace) -> str:
     """Returns the true type font file name without parent directories e.g. "Arial.ttf"."""
-    return font_manager.find_font_file_name(font_face)
+    return font_manager.find_font_name(font_face)
 
 
 def load():
-    """Load all cache files."""
+    """Reload all cache files. The cache files are loaded automatically at the import
+    of `ezdxf`.
+    """
     _load_font_manager()
 
 
 def _get_font_manger_path():
     cache_path = options.xdg_path("XDG_CACHE_HOME", CACHE_DIRECTORY)
     return cache_path / FONT_MANAGER_CACHE_FILE
 
 
 def _load_font_manager() -> None:
-    repo_fonts_path = os.environ.get("EZDXF_REPO_FONTS")
-    if repo_fonts_path:
-        _build_sut_font_manager(Path(repo_fonts_path))
-        return
+    if "pytest" in sys.modules:
+        return  # do nothing: system under test (sut)
 
     fm_path = _get_font_manger_path()
     if fm_path.exists():
         try:
             font_manager.loads(fm_path.read_text())
             return
         except IOError as e:
             logger.info(f"Error loading cache file: {str(e)}")
     build_font_manager_cache(fm_path)
 
 
-def _build_sut_font_manager(repo_fonts_path: Path) -> None:
-    """Load font manger for system under test (sut).
+def build_sut_font_manager_cache(repo_font_path: pathlib.Path) -> None:
+    """Load font manger cache for system under test (sut).
 
     Load the fonts included in the repository folder "./fonts" to guarantee the tests
-    have the same fonts available on all systems. The environment variable
-    "EZDXF_REPO_FONTS" is set in "conftest.py" at session start.
+    have the same fonts available on all systems.
     """
+    if font_manager.has_font("DejaVuSans.ttf"):
+        return
     font_manager.clear()
-    cache_file = repo_fonts_path / "font_manager_cache.json"
+    cache_file = repo_font_path / "font_manager_cache.json"
     if cache_file.exists():
         try:
             font_manager.loads(cache_file.read_text())
             return
         except IOError as e:
             print(f"Error loading cache file: {str(e)}")
-    font_manager.build([str(repo_fonts_path)])
+    font_manager.build([str(repo_font_path)])
     s = font_manager.dumps()
     try:
         cache_file.write_text(s)
     except IOError as e:
         print(f"Error writing cache file: {str(e)}")
 
 
-def build_font_manager_cache(path: Path) -> None:
+def build_font_manager_cache(path: pathlib.Path) -> None:
     font_manager.build()
     s = font_manager.dumps()
     if not path.parent.exists():
         path.parent.mkdir(parents=True)
     try:
         path.write_text(s)
     except IOError as e:
         logger.info(f"Error writing cache file: {str(e)}")
 
 
-# A Visual Guide to the Anatomy of Typography: https://visme.co/blog/type-anatomy/
-# Anatomy of a Character: https://www.fonts.com/content/learning/fontology/level-1/type-anatomy/anatomy
+class FontRenderType(enum.Enum):
+    # render glyphs as filled paths: TTF, OTF
+    OUTLINE = enum.auto()
 
-
-class FontMeasurements(NamedTuple):
-    baseline: float
-    cap_height: float
-    x_height: float
-    descender_height: float
-
-    def scale(self, factor: float = 1.0) -> FontMeasurements:
-        return FontMeasurements(
-            self.baseline * factor,
-            self.cap_height * factor,
-            self.x_height * factor,
-            self.descender_height * factor,
-        )
-
-    def shift(self, distance: float = 0.0) -> FontMeasurements:
-        return FontMeasurements(
-            self.baseline + distance,
-            self.cap_height,
-            self.x_height,
-            self.descender_height,
-        )
-
-    def scale_from_baseline(self, desired_cap_height: float) -> FontMeasurements:
-        factor = desired_cap_height / self.cap_height
-        return FontMeasurements(
-            self.baseline,
-            desired_cap_height,
-            self.x_height * factor,
-            self.descender_height * factor,
-        )
-
-    @property
-    def cap_top(self) -> float:
-        return self.baseline + self.cap_height
-
-    @property
-    def x_top(self) -> float:
-        return self.baseline + self.x_height
-
-    @property
-    def bottom(self) -> float:
-        return self.baseline - self.descender_height
-
-    @property
-    def total_height(self) -> float:
-        return self.cap_height + self.descender_height
+    # render glyphs as line strokes: SHX, SHP
+    STROKE = enum.auto
 
 
 class AbstractFont:
-    """The `ezdxf` font abstraction."""
+    """The `ezdxf` font abstraction for text measurement and text path rendering."""
+
+    font_render_type = FontRenderType.STROKE
+    name: str = "undefined"
 
     def __init__(self, measurements: FontMeasurements):
         self.measurements = measurements
 
     @abc.abstractmethod
     def text_width(self, text: str) -> float:
+        """Returns the text width in drawing units for the given `text` string."""
         pass
 
     @abc.abstractmethod
-    def space_width(self) -> float:
-        pass
-
-
-class TrueTypeFont(AbstractFont):
-    _ttf_render_engines: dict[str, TTFontRenderer] = dict()
-
-    def __init__(self, ttf: str, cap_height: float, width_factor: float = 1.0):
-        self.engine = self._create_engine(ttf)
-        self.cap_height = float(cap_height)
-        self.width_factor = float(width_factor)
-        measurements = self.engine.font_measurements
-        scale_factor = self.engine.get_scaling_factor(self.cap_height)
-        super().__init__(measurements.scale(scale_factor))
-        self._space_width = (
-            self.engine.get_text_length(" ", self.cap_height) * self.width_factor
-        )
-
-    def _create_engine(self, ttf: str) -> TTFontRenderer:
-        from .ttfonts import TTFontRenderer
-
-        key = Path(ttf).name.lower()
-        try:
-            return self._ttf_render_engines[key]
-        except KeyError:
-            pass
-        engine = TTFontRenderer(font_manager.get_ttf_font(ttf))
-        self._ttf_render_engines[key] = engine
-        return engine
-
-    def text_width(self, text: str) -> float:
-        """Returns the text width in drawing units for the given `text` string.
-        Text rendering and width calculation is based on fontTools.
+    def text_width_ex(
+        self, text: str, cap_height: float, width_factor: float = 1.0
+    ) -> float:
+        """Returns the text width in drawing units, bypasses the stored `cap_height` and
+        `width_factor`.
         """
-        if not text.strip():
-            return 0
-        return self.engine.get_text_length(text, self.cap_height) * self.width_factor
+        pass
 
+    @abc.abstractmethod
     def space_width(self) -> float:
-        """Returns the width of a "space" char."""
-        return self._space_width
+        """Returns the width of a "space" character a.k.a. word spacing."""
+        pass
 
+    @abc.abstractmethod
+    def text_path(self, text: str) -> GlyphPath:
+        """Returns the 2D text path for the given text."""
+        ...
 
-# Matplotlib provided the TrueType font renderer til v1.0.4,
-# was replaced by fontTools
-MatplotlibFont = TrueTypeFont
+    @abc.abstractmethod
+    def text_path_ex(
+        self, text: str, cap_height: float, width_factor: float = 1.0
+    ) -> GlyphPath:
+        """Returns the 2D text path for the given text, bypasses the stored `cap_height`
+        and `width_factor`."""
+        ...
 
 
 class MonospaceFont(AbstractFont):
-    """Defines a monospaced font without knowing the real font properties.
-    Each letter has the same cap- and descender height and the same width.
-    This font abstraction is used if no Matplotlib font support is available.
+    """Represents a monospaced font where each letter has the same cap- and descender
+    height and the same width. The given cap height and width factor are the default
+    values for measurements and rendering. The extended methods can override these
+    default values.
 
-    Use the :func:`make_font` factory function to create a font abstraction.
+    This font exists only for generic text measurement in tests and does not render any
+    glyphs!
 
     """
 
+    font_render_type = FontRenderType.STROKE
+    name = MONOSPACE
+
     def __init__(
         self,
         cap_height: float,
         width_factor: float = 1.0,
         baseline: float = 0,
         descender_factor: float = DESCENDER_FACTOR,
         x_height_factor: float = X_HEIGHT_FACTOR,
@@ -415,41 +397,221 @@
                 descender_height=cap_height * descender_factor,
             )
         )
         self._width_factor: float = abs(width_factor)
         self._space_width = self.measurements.cap_height * self._width_factor
 
     def text_width(self, text: str) -> float:
-        """Returns the text width in drawing units for the given `text` based
-        on a simple monospaced font calculation.
+        """Returns the text width in drawing units for the given `text`."""
+        return self.text_width_ex(
+            text, self.measurements.cap_height, self._width_factor
+        )
+
+    def text_width_ex(
+        self, text: str, cap_height: float, width_factor: float = 1.0
+    ) -> float:
+        """Returns the text width in drawing units, bypasses the stored `cap_height` and
+        `width_factor`.
+        """
+        return len(text) * cap_height * width_factor
+
+    def text_path(self, text: str) -> GlyphPath:
+        """Returns the rectangle text width x cap height as :class:`~ezdxf.path.Path2d` instance."""
+        return self.text_path_ex(text, self.measurements.cap_height, self._width_factor)
+
+    def text_path_ex(
+        self, text: str, cap_height: float, width_factor: float = 1.0
+    ) -> GlyphPath:
+        """Returns the rectangle text width x cap height as  :class:`~ezdxf.path.Path2d`
+        instance, bypasses the stored `cap_height` and `width_factor`.
+        """
+        from ezdxf.path import Path2d
+
+        text_width = self.text_width_ex(text, cap_height, width_factor)
+        p = Path2d((0, 0))
+        p.line_to((text_width, 0))
+        p.line_to((text_width, cap_height))
+        p.line_to((0, cap_height))
+        p.close()
+        return p
+
+    def space_width(self) -> float:
+        """Returns the width of a "space" char."""
+        return self._space_width
+
+
+class _CachedFont(AbstractFont, abc.ABC):
+    """Abstract font with caching support."""
+
+    _glyph_caches: dict[str, Glyphs] = dict()
+
+    def __init__(self, font_name: str, cap_height: float, width_factor: float = 1.0):
+        self.name = font_name
+        cache = self.create_cache(font_name)
+        self.glyph_cache = cache
+        self.cap_height = float(cap_height)
+        self.width_factor = float(width_factor)
+        scale_factor: float = cache.get_scaling_factor(self.cap_height)
+        super().__init__(cache.font_measurements.scale(scale_factor))
+        self._space_width: float = (
+            self.glyph_cache.space_width * scale_factor * width_factor
+        )
+
+    @abc.abstractmethod
+    def create_cache(self, font_name: str) -> Glyphs:
+        ...
+
+    def text_width(self, text: str) -> float:
+        """Returns the text width in drawing units for the given `text` string."""
+        return self.text_width_ex(text, self.cap_height, self.width_factor)
 
+    def text_width_ex(
+        self, text: str, cap_height: float, width_factor: float = 1.0
+    ) -> float:
+        """Returns the text width in drawing units, bypasses the stored `cap_height` and
+        `width_factor`.
         """
-        return len(text) * self.measurements.cap_height * self._width_factor
+        if not text.strip():
+            return 0
+        return self.glyph_cache.get_text_length(text, cap_height, width_factor)
+
+    def text_path(self, text: str) -> GlyphPath:
+        """Returns the 2D text path for the given text."""
+
+        return self.text_path_ex(text, self.cap_height, self.width_factor)
+
+    def text_path_ex(
+        self, text: str, cap_height: float, width_factor: float = 1.0
+    ) -> GlyphPath:
+        """Returns the 2D text path for the given text, bypasses the stored `cap_height`
+        and `width_factor`."""
+        return self.glyph_cache.get_text_path(text, cap_height, width_factor)
 
     def space_width(self) -> float:
         """Returns the width of a "space" char."""
         return self._space_width
 
 
+class TrueTypeFont(_CachedFont):
+    """Represents a TrueType font. Font measurement and glyph rendering is done by the
+    `fontTools` package. The given cap height and width factor are the default values
+    for measurements and glyph rendering. The extended methods can override these
+    default values.
+    """
+
+    font_render_type = FontRenderType.OUTLINE
+
+    def create_cache(self, ttf: str) -> Glyphs:
+        from .ttfonts import TTFontRenderer
+
+        key = pathlib.Path(ttf).name.lower()
+        try:
+            return self._glyph_caches[key]
+        except KeyError:
+            pass
+        cache = TTFontRenderer(font_manager.get_ttf_font(ttf))
+        self._glyph_caches[key] = cache
+        return cache
+
+
+class ShapeFileFont(_CachedFont):
+    """Represents a shapefile font (.shx, .shp). Font measurement and glyph rendering is
+    done by the ezdxf.fonts.shapefile module. The given cap height and width factor are
+    the default values for measurements and glyph rendering. The extended methods can
+    override these default values.
+
+    """
+
+    font_render_type = FontRenderType.STROKE
+
+    def create_cache(self, font_name: str) -> Glyphs:
+        key = font_name.lower()
+        try:
+            return self._glyph_caches[key]
+        except KeyError:
+            pass
+        glyph_cache = font_manager.get_shapefile_glyph_cache(font_name)
+        self._glyph_caches[key] = glyph_cache
+        return glyph_cache
+
+
+class LibreCadFont(_CachedFont):
+    """Represents a LibreCAD font (.shx, .shp). Font measurement and glyph rendering is
+    done by the ezdxf.fonts.lff module. The given cap height and width factor are the
+    default values for measurements and glyph rendering. The extended methods can
+    override these default values.
+
+    """
+
+    font_render_type = FontRenderType.STROKE
+
+    def create_cache(self, font_name: str) -> Glyphs:
+        key = font_name.lower()
+        try:
+            return self._glyph_caches[key]
+        except KeyError:
+            pass
+        glyph_cache = font_manager.get_lff_glyph_cache(font_name)
+        self._glyph_caches[key] = glyph_cache
+        return glyph_cache
+
+
 def make_font(
-    ttf_path: str, cap_height: float, width_factor: float = 1.0
+    font_name: str, cap_height: float, width_factor: float = 1.0
 ) -> AbstractFont:
-    """Factory function to create a font abstraction.
+    r"""Returns a font abstraction based on class :class:`AbstractFont`.
+
+    Supported font types:
 
-    Creates a :class:`TrueTypeFont` if the Matplotlib font support is
-    available and enabled or else a :class:`MonospaceFont`.
+    - .ttf, .ttc and .otf - TrueType fonts
+    - .shx, .shp - Autodesk® shapefile fonts
+    - .lff - LibreCAD font format
+
+    The special name "\*monospace" returns the fallback font :class:`MonospaceFont` for
+    testing and basic measurements.
+
+    .. note:: The font definition files are not included in `ezdxf`.
 
     Args:
-        ttf_path: raw font file name as stored in the
-            :class:`~ezdxf.entities.Textstyle` entity
+        font_name: font file name as stored in the :class:`~ezdxf.entities.Textstyle`
+            entity e.g. "OpenSans-Regular.ttf"
         cap_height: desired cap height in drawing units.
         width_factor: horizontal text stretch factor
 
     """
-    return TrueTypeFont(ttf_path, cap_height, width_factor)
+    if font_name == MONOSPACE:
+        return MonospaceFont(cap_height, width_factor)
+    ext = pathlib.Path(font_name).suffix
+    last_resort = MonospaceFont(cap_height, width_factor)
+    if ext in SUPPORTED_TTF_TYPES:
+        try:
+            return TrueTypeFont(font_name, cap_height, width_factor)
+        except FontNotFoundError:
+            return last_resort
+    elif ext == ".shx" or ext == ".shp":
+        try:
+            return ShapeFileFont(font_name, cap_height, width_factor)
+        except FontNotFoundError:
+            pass  # no shape file fonts available
+    elif ext == ".lff":
+        try:
+            return LibreCadFont(font_name, cap_height, width_factor)
+        except FontNotFoundError:
+            pass  # no libreCAD fonts available
+    elif ext == "":  # e.g. "TXT"
+        font_face = font_manager.find_best_match(
+            family=font_name, style=".shx", italic=None
+        )
+        if font_face is not None:
+            return make_font(font_face.filename, cap_height, width_factor)
+    # return default TrueType font
+    try:
+        return TrueTypeFont(font_name, cap_height, width_factor)
+    except FontNotFoundError:
+        return last_resort
 
 
 def get_entity_font_face(entity: DXFEntity, doc: Optional[Drawing] = None) -> FontFace:
     """Returns the :class:`FontFace` defined by the associated text style.
     Returns the default font face if the `entity` does not have or support
     the DXF attribute "style". Supports the extended font information stored in
     :class:`~ezdxf.entities.Textstyle` table entries.
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `ezdxf-1.1.0b0/src/ezdxf/tools/font_face.py` & `ezdxf-1.1.0b1/src/ezdxf/fonts/font_face.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #  Copyright (c) 2023, Manfred Moitzi
 #  License: MIT License
 from __future__ import annotations
 from typing import NamedTuple
 
 
 class FontFace(NamedTuple):
-    # ttf is the font file name without parent directories e.g. "OpenSans-Regular.ttf"
-    ttf: str = ""
+    # filename without parent directories e.g. "OpenSans-Regular.ttf"
+    filename: str = ""
     family: str = "sans-serif"
     style: str = "Regular"
     weight: int = 400  # Normal - usWeightClass
     width: int = 5  # Medium(Normal) - usWidthClass
 
     @property
     def is_italic(self) -> bool:
@@ -31,15 +31,15 @@
     def weight_str(self) -> str:
         """Returns the :attr:`weight` as string e.g. "Thin", "Normal", "Bold", ..."""
         return get_weight_str(self.weight)
 
     @property
     def width_str(self) -> str:
         """Returns the :attr:`width` as string e.g. "Condensed", "Expanded", ..."""
-        return get_width_str(self.weight)
+        return get_width_str(self.width)
 
     def distance(self, font_face: FontFace) -> tuple[int, int]:
         return self.weight - font_face.weight, self.width - font_face.width
 
 
 WEIGHT_STR = {
     100: "Thin",
@@ -64,14 +64,15 @@
     8: "ExtraExpanded",
     9: "UltraExpanded",
 }
 
 
 def get_weight_str(weight: int) -> str:
     """Returns the :attr:`weight` as string e.g. "Thin", "Normal", "Bold", ..."""
-    index = max(min(round(weight + 1 / 100), 1), 9)
-    return WEIGHT_STR[index]
+    key = max(min(round((weight + 1) / 100) * 100, 900), 100)
+    return WEIGHT_STR[key]
 
 
 def get_width_str(width: int) -> str:
     """Returns the :attr:`width` as string e.g. "Condensed", "Expanded", ..."""
-    return WEIGHT_STR[max(min(width, 1), 9)]
+    key = max(min(width, 9), 1)
+    return WIDTH_STR[key]
```

## Comparing `ezdxf-1.1.0b0/src/ezdxf/tools/font_manager.py` & `ezdxf-1.1.0b1/src/ezdxf/fonts/font_manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 #  Copyright (c) 2023, Manfred Moitzi
 #  License: MIT License
 from __future__ import annotations
+
+import pathlib
 from typing import Iterable, NamedTuple, Optional, Sequence
 import os
 import platform
 import json
 
 from pathlib import Path
 from fontTools.ttLib import TTFont
 from .font_face import FontFace
+from . import shapefile, lff
 
 WINDOWS = "Windows"
 LINUX = "Linux"
 MACOS = "Darwin"
 
 
 WIN_SYSTEM_ROOT = os.environ.get("SystemRoot", "C:/Windows")
@@ -42,15 +45,15 @@
     "LiberationSans-Regular.ttf",
     "OpenSans-Regular.ttf",
 ]
 CURRENT_CACHE_VERSION = 1
 
 
 class CacheEntry(NamedTuple):
-    file_path: Path
+    file_path: Path  # full file path e.g. "C:\Windows\Fonts\DejaVuSans.ttf"
     font_face: FontFace
 
 
 GENERIC_FONT_FAMILY = {
     "serif": "DejaVu Serif",
     "sans-serif": "DejaVu Sans",
     "monospace": "DejaVu Sans Mono",
@@ -59,14 +62,17 @@
 
 class FontCache:
     def __init__(self) -> None:
         # cache key is the lowercase ttf font name without parent directories
         # e.g. "arial.ttf" for "C:\Windows\Fonts\Arial.ttf"
         self._cache: dict[str, CacheEntry] = dict()
 
+    def __contains__(self, font_name: str) -> bool:
+        return self.key(font_name) in self._cache
+
     def __getitem__(self, item: str) -> CacheEntry:
         return self._cache[self.key(item)]
 
     def __len__(self):
         return len(self._cache)
 
     def clear(self) -> None:
@@ -82,15 +88,15 @@
     def get(self, font_name: str, fallback: str) -> CacheEntry:
         try:
             return self._cache[self.key(font_name)]
         except KeyError:
             return self._cache[self.key(fallback)]
 
     def find_best_match(self, font_face: FontFace) -> Optional[FontFace]:
-        entry = self._cache.get(self.key(font_face.ttf), None)
+        entry = self._cache.get(self.key(font_face.filename), None)
         if entry:
             return entry.font_face
         return self.find_best_match_ex(
             family=font_face.family,
             style=font_face.style,
             weight=font_face.weight,
             width=font_face.width,
@@ -114,22 +120,25 @@
             return entries[0].font_face
         entries_ = filter_style(style, entries)
         if len(entries_) == 1:
             return entries_[0].font_face
         elif len(entries_):
             entries = entries_
         # best match by weight, italic, width
-        return sorted(
+        # Note: the width property is used to prioritize shapefile types:
+        # 1st .shx; 2nd: .shp; 3rd: .lff
+        result = sorted(
             entries,
             key=lambda e: (
                 abs(e.font_face.weight - weight),
                 e.font_face.is_italic is not italic,
                 abs(e.font_face.width - width),
             ),
-        )[0].font_face
+        )
+        return result[0].font_face
 
     def loads(self, s: str) -> None:
         cache: dict[str, CacheEntry] = dict()
         try:
             content = json.loads(s)
         except json.JSONDecodeError:
             raise IOError("invalid JSON file format")
@@ -142,15 +151,15 @@
             for entry in content:
                 try:
                     file_path, family, style, weight, width = entry
                 except ValueError:
                     raise IOError("invalid cache file format")
                 path = Path(file_path)  # full path, e.g. "C:\Windows\Fonts\Arial.ttf"
                 font_face = FontFace(
-                    ttf=path.name,  # file name without parent dirs, e.g. "Arial.ttf"
+                    filename=path.name,  # file name without parent dirs, e.g. "Arial.ttf"
                     family=family,  # Arial
                     style=style,  # Regular
                     weight=weight,  # 400 (Normal)
                     width=width,  # 5 (Normal)
                 )
                 cache[self.key(path.name)] = CacheEntry(path, font_face)
         else:
@@ -178,32 +187,45 @@
 
 
 def filter_style(style: str, entries: Iterable[CacheEntry]) -> list[CacheEntry]:
     key = str(style).lower()
     return [e for e in entries if key in e.font_face.style.lower()]
 
 
-SUPPORTED_FONT_TYPES = {".ttf", ".ttc", ".otf"}
+# TrueType and OpenType fonts:
+# Note: CAD applications like AutoCAD/BricsCAD do not support OpenType fonts!
+SUPPORTED_TTF_TYPES = {".ttf", ".ttc", ".otf"}
+# Basic stroke-fonts included in CAD applications:
+SUPPORTED_SHAPE_FILES = {".shx", ".shp", ".lff"}
 NO_FONT_FACE = FontFace()
+FALLBACK_SHAPE_FILES = ["txt.shx", "txt.shp", "iso.shx", "iso.shp"]
+FALLBACK_LFF = ["standard.lff", "iso.lff", "simplex.lff"]
 
 
 class FontNotFoundError(Exception):
     pass
 
 
 class FontManager:
     def __init__(self) -> None:
         self.platform = platform.system()
         self._font_cache: FontCache = FontCache()
-        self._loaded_fonts: dict[str, TTFont] = dict()
+        self._loaded_ttf_fonts: dict[str, TTFont] = dict()
+        self._loaded_shape_file_glyph_caches: dict[str, shapefile.GlyphCache] = dict()
+        self._loaded_lff_glyph_caches: dict[str, lff.GlyphCache] = dict()
         self._fallback_font_name = ""
+        self._fallback_shape_file = ""
+        self._fallback_lff = ""
+
+    def has_font(self, font_name: str) -> bool:
+        return font_name in self._font_cache
 
     def clear(self) -> None:
         self._font_cache = FontCache()
-        self._loaded_fonts.clear()
+        self._loaded_ttf_fonts.clear()
         self._fallback_font_name = ""
 
     def fallback_font_name(self) -> str:
         fallback_name = self._fallback_font_name
         if fallback_name:
             return fallback_name
         fallback_name = DEFAULT_FONTS[0]
@@ -213,32 +235,91 @@
                 fallback_name = cache_entry.file_path.name
                 break
             except KeyError:
                 pass
         self._fallback_font_name = fallback_name
         return fallback_name
 
+    def fallback_shapefile(self) -> str:
+        fallback_shape_file = self._fallback_shape_file
+        if fallback_shape_file:
+            return fallback_shape_file
+
+        for name in FALLBACK_SHAPE_FILES:
+            if name in self._font_cache:
+                self._fallback_shape_file = name
+                return name
+        return ""
+
+    def fallback_lff(self) -> str:
+        fallback_lff = self._fallback_lff
+        if fallback_lff:
+            return fallback_lff
+
+        for name in FALLBACK_SHAPE_FILES:
+            if name in self._font_cache:
+                self._fallback_shape_file = name
+                return name
+        return ""
+
     def get_ttf_font(self, font_name: str, font_number: int = 0) -> TTFont:
         try:
-            return self._loaded_fonts[font_name]
+            return self._loaded_ttf_fonts[font_name]
         except KeyError:
             pass
         fallback_name = self.fallback_font_name()
         try:
             font = TTFont(
                 self._font_cache.get(font_name, fallback_name).file_path,
                 fontNumber=font_number,
             )
         except IOError as e:
             raise FontNotFoundError(str(e))
-        self._loaded_fonts[font_name] = font
+        self._loaded_ttf_fonts[font_name] = font
         return font
 
     def ttf_font_from_font_face(self, font_face: FontFace) -> TTFont:
-        return self.get_ttf_font(Path(font_face.ttf).name)
+        return self.get_ttf_font(Path(font_face.filename).name)
+
+    def get_shapefile_glyph_cache(self, font_name: str) -> shapefile.GlyphCache:
+        try:
+            return self._loaded_shape_file_glyph_caches[font_name]
+        except KeyError:
+            pass
+        fallback_name = self.fallback_shapefile()
+        try:
+            file_path = self._font_cache.get(font_name, fallback_name).file_path
+        except KeyError:
+            raise FontNotFoundError(f"shape font '{font_name}' not found")
+        try:
+            file = shapefile.readfile(str(file_path))
+        except IOError:
+            raise FontNotFoundError(f"shape file '{file_path}' not found")
+        glyph_cache = shapefile.GlyphCache(file)
+        self._loaded_shape_file_glyph_caches[font_name] = glyph_cache
+        return glyph_cache
+
+    def get_lff_glyph_cache(self, font_name: str) -> lff.GlyphCache:
+        try:
+            return self._loaded_lff_glyph_caches[font_name]
+        except KeyError:
+            pass
+        fallback_name = self.fallback_lff()
+        try:
+            file_path = self._font_cache.get(font_name, fallback_name).file_path
+        except KeyError:
+            raise FontNotFoundError(f"LibreCAD font '{font_name}' not found")
+        try:
+            s = pathlib.Path(file_path).read_text(encoding="utf8")
+            font = lff.loads(s)
+        except IOError:
+            raise FontNotFoundError(f"LibreCAD font file '{file_path}' not found")
+        glyph_cache = lff.GlyphCache(font)
+        self._loaded_lff_glyph_caches[font_name] = glyph_cache
+        return glyph_cache
 
     def get_font_face(self, font_name: str) -> FontFace:
         cache_entry = self._font_cache.get(font_name, self.fallback_font_name())
         return cache_entry.font_face
 
     def find_best_match(
         self,
@@ -246,85 +327,116 @@
         style: str = "Regular",
         weight=400,
         width=5,
         italic: Optional[bool] = False,
     ) -> Optional[FontFace]:
         return self._font_cache.find_best_match_ex(family, style, weight, width, italic)
 
-    def find_font_file_name(self, font_face: FontFace) -> str:
-        """Returns the file name of the font without parent directories
+    def find_font_name(self, font_face: FontFace) -> str:
+        """Returns the font file name of the font without parent directories
         e.g. "LiberationSans-Regular.ttf".
         """
         font_face = self._font_cache.find_best_match(font_face)  # type: ignore
         if font_face is None:
             font_face = self.get_font_face(self.fallback_font_name())
-            return font_face.ttf
+            return font_face.filename
         else:
-            return font_face.ttf
+            return font_face.filename
 
     def build(self, folders: Optional[Sequence[str]] = None) -> None:
         """Adds all supported font types located in the given `folders` to the font
         manager. If no directories are specified, the known font folders for Windows,
         Linux and macOS are searched by default. Searches recursively all
         subdirectories.
+
+        The folders stored in the config SUPPORT_DIRS option are scanned recursively for
+        .shx, .shp and .lff fonts, the basic stroke fonts included in CAD applications.
+
         """
+        from ezdxf._options import options
+
         if folders:
             dirs = list(folders)
         else:
             dirs = FONT_DIRECTORIES.get(self.platform, LINUX_FONT_DIRS)
-        self.scan_all(dirs)
-        if len(self._font_cache) == 0:  # system under test - github action
-            path = Path(__file__)
-            fonts = path.parent.parent.parent.parent / "fonts"
-            self.scan_folder(fonts)
+        self.scan_all(dirs + list(options.support_dirs))
 
     def scan_all(self, folders: Iterable[str]) -> None:
         for folder in folders:
+            folder = folder.strip("'\"")  # strip quotes
             self.scan_folder(Path(folder).expanduser())
 
     def scan_folder(self, folder: Path):
         if not folder.exists():
             return
         for file in folder.iterdir():
             if file.is_dir():
                 self.scan_folder(file)
                 continue
             ext = file.suffix.lower()
-            if ext in SUPPORTED_FONT_TYPES:
+            if ext in SUPPORTED_TTF_TYPES:
                 font_face = get_ttf_font_face(file)
                 self._font_cache.add_entry(file, font_face)
+            elif ext in SUPPORTED_SHAPE_FILES:
+                font_face = get_shape_file_font_face(file)
+                self._font_cache.add_entry(file, font_face)
 
     def dumps(self) -> str:
         return self._font_cache.dumps()
 
     def loads(self, s: str) -> None:
         self._font_cache.loads(s)
 
 
+def normalize_style(style: str) -> str:
+    if style in {"Book"}:
+        style = "Regular"
+    return style
+
+
 def get_ttf_font_face(font_path: Path) -> FontFace:
     try:
         ttf = TTFont(font_path, fontNumber=0)
     except IOError:
-        return FontFace(ttf=font_path.name)
+        return FontFace(filename=font_path.name)
 
     names = ttf["name"].names
     family = ""
     style = ""
     for record in names:
         if record.nameID == 1:
             family = record.string.decode(record.getEncoding())
         elif record.nameID == 2:
             style = record.string.decode(record.getEncoding())
         if family and style:
             break
     os2_table = ttf["OS/2"]
     weight = os2_table.usWeightClass
     width = os2_table.usWidthClass
-    if style == "Book":
-        style = "Regular"
     return FontFace(
-        ttf=font_path.name,
+        filename=font_path.name,
         family=family,
-        style=style,
+        style=normalize_style(style),
         width=width,
         weight=weight,
     )
+
+
+def get_shape_file_font_face(font_path: Path) -> FontFace:
+    ext = font_path.suffix.lower()
+    # Note: the width property is not defined in shapefiles and is used to
+    # prioritize the shapefile types for find_best_match():
+    # 1st .shx; 2nd: .shp; 3rd: .lff
+
+    width = 5
+    if ext == ".shp":
+        width = 6
+    if ext == ".lff":
+        width = 7
+
+    return FontFace(
+        filename=font_path.name,  # "txt.shx", "simplex.shx", ...
+        family=font_path.stem.lower(),  # "txt", "simplex", ...
+        style=font_path.suffix.lower(),  # ".shx", ".shp" or ".lff"
+        width=width,
+        weight=400,
+    )
```

## Comparing `ezdxf-1.1.0b0/src/ezdxf/tools/handle.py` & `ezdxf-1.1.0b1/src/ezdxf/tools/handle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/tools/indexing.py` & `ezdxf-1.1.0b1/src/ezdxf/tools/indexing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/tools/juliandate.py` & `ezdxf-1.1.0b1/src/ezdxf/tools/juliandate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/tools/pattern.py` & `ezdxf-1.1.0b1/src/ezdxf/tools/pattern.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/tools/rawloader.py` & `ezdxf-1.1.0b1/src/ezdxf/tools/rawloader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/tools/standards.py` & `ezdxf-1.1.0b1/src/ezdxf/tools/standards.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/tools/strip.py` & `ezdxf-1.1.0b1/src/ezdxf/tools/strip.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/tools/test.py` & `ezdxf-1.1.0b1/src/ezdxf/tools/test.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/tools/text.py` & `ezdxf-1.1.0b1/src/ezdxf/tools/text.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2021-2022, Manfred Moitzi
+# Copyright (c) 2021-2023, Manfred Moitzi
 # License: MIT License
 """
 Tools in this module should be as independent of DXF entities as possible!
 """
 from __future__ import annotations
 from typing import (
     Iterable,
@@ -34,19 +34,20 @@
     BASELINE,
     MIDDLE,
     TOP,
     MAX_STR_LEN,
 )
 from ezdxf.math import Vec3, Vec2, UVec
 from ezdxf.colors import rgb2int, RGB, int2rgb
-from .fonts import FontMeasurements, AbstractFont, FontFace, make_font
+
 
 if TYPE_CHECKING:
     from ezdxf.entities import Text, MText, DXFEntity
     from ezdxf.lldxf.tags import Tags
+    from ezdxf.fonts import fonts
 
 X_MIDDLE = 4  # special case for overall alignment "MIDDLE"
 
 
 class TextLine:
     """Helper class which represents a single line text entity
     (e.g. :class:`~ezdxf.entities.Text`).
@@ -54,15 +55,15 @@
     Args:
         text: content string
         font: ezdxf font definition like :class:`~ezdxf.tools.fonts.MonospaceFont`
             or :class:`~ezdxf.tools.fonts.MatplotlibFont`
 
     """
 
-    def __init__(self, text: str, font: "AbstractFont"):
+    def __init__(self, text: str, font: fonts.AbstractFont):
         self._font = font
         self._text_width: float = font.text_width(text)
         self._stretch_x: float = 1.0
         self._stretch_y: float = 1.0
 
     def stretch(self, alignment: TextEntityAlignment, p1: Vec3, p2: Vec3) -> None:
         """Set stretch factors for FIT and ALIGNED alignments to fit the
@@ -88,15 +89,15 @@
         return self._text_width * self._stretch_x
 
     @property
     def height(self) -> float:
         """Returns the final (stretched) text height."""
         return self._font.measurements.total_height * self._stretch_y
 
-    def font_measurements(self) -> FontMeasurements:
+    def font_measurements(self) -> fonts.FontMeasurements:
         """Returns the scaled font measurements."""
         return self._font.measurements.scale(self._stretch_y)
 
     def baseline_vertices(
         self,
         insert: UVec,
         halign: int = 0,
@@ -152,15 +153,15 @@
             Vec2(self.width, fm.cap_top),
             Vec2(0, fm.cap_top),
         ]
         shift = self._shift_vector(halign, valign, fm)
         return TextLine.transform_2d(vertices, insert, shift, angle, scale, oblique)
 
     def _shift_vector(
-        self, halign: int, valign: int, fm: FontMeasurements
+        self, halign: int, valign: int, fm: fonts.FontMeasurements
     ) -> tuple[float, float]:
         return _shift_x(self.width, halign), _shift_y(fm, valign)
 
     @staticmethod
     def transform_2d(
         vertices: Iterable[UVec],
         insert: UVec = Vec3(0, 0, 0),
@@ -224,15 +225,15 @@
     if halign == CENTER:
         return -total_width / 2.0
     elif halign == RIGHT:
         return -total_width
     return 0.0  # LEFT
 
 
-def _shift_y(fm: FontMeasurements, valign: int) -> float:
+def _shift_y(fm: fonts.FontMeasurements, valign: int) -> float:
     if valign == BASELINE:
         return fm.baseline
     elif valign == MIDDLE:
         return -fm.cap_top + fm.cap_height / 2
     elif valign == X_MIDDLE:
         return -fm.cap_top + fm.total_height / 2
     elif valign == TOP:
@@ -1000,20 +1001,22 @@
     pass
 
 
 class MTextContext:
     """Internal class to store the MTEXT context state."""
 
     def __init__(self) -> None:
+        from ezdxf.fonts import fonts
+
         self._stroke: int = 0
         self.continue_stroke: bool = False
         self._aci = 7  # used if rgb is None
         self.rgb: Optional[RGB] = None  # overrules aci
         self.align = MTextLineAlignment.BOTTOM
-        self.font_face: FontFace = FontFace()  # is immutable
+        self.font_face = fonts.FontFace()  # is immutable
         self.cap_height: float = 1.0
         self.width_factor: float = 1.0
         self.char_tracking_factor: float = 1.0
         self.oblique: float = 0.0  # in degrees, where 0 is vertical (TEXT entity)
         self.paragraph = ParagraphProperties()
 
     def __copy__(self) -> MTextContext:
@@ -1626,28 +1629,30 @@
                             # and try again:
                             paragraph_scanner.consume()
         ctx.paragraph = ParagraphProperties(
             indent, left, right, align, tuple(tab_stops)
         )
 
     def parse_font_properties(self, ctx: MTextContext):
+        from ezdxf.fonts import fonts
+
         parts = self.extract_expression().split("|")
         # an empty font family name does not change the font properties
         if parts and parts[0]:
             name = parts[0]
             style = "Regular"
             weight = 400
             # ignore codepage and pitch - it seems not to be used in newer
             # CAD applications.
             for part in parts[1:]:
                 if part.startswith("b1"):
                     weight = 700
                 elif part.startswith("i1"):
                     style = "Italic"
-            ctx.font_face = FontFace(family=name, style=style, weight=weight)
+            ctx.font_face = fonts.FontFace(family=name, style=style, weight=weight)
 
     def consume_optional_terminator(self):
         if self.scanner.peek() == ";":
             self.scanner.consume(1)
 
 
 def load_mtext_content(tags: Tags) -> str:
@@ -1729,34 +1734,36 @@
     This function uses the optional `Matplotlib` package if available.
 
     Returns:
         Tuple[width, height]
 
     """
 
-    def _make_font() -> AbstractFont:
+    def _make_font() -> fonts.AbstractFont:
+        from ezdxf.fonts import fonts
+
         cap_height: float = mtext.dxf.get_default("char_height")
         doc = mtext.doc
         if doc:
             style = doc.styles.get(mtext.dxf.get_default("style"))
             if style is not None:
                 return style.make_font(cap_height)  # type: ignore
-        return make_font(const.DEFAULT_TTF, cap_height=cap_height)
+        return fonts.make_font(const.DEFAULT_TTF, cap_height=cap_height)
 
     return estimate_mtext_content_extents(
         content=mtext.text,
         font=_make_font(),
         column_width=mtext.dxf.get("width", 0.0),
         line_spacing_factor=mtext.dxf.get_default("line_spacing_factor"),
     )
 
 
 def estimate_mtext_content_extents(
     content: str,
-    font: AbstractFont,
+    font: fonts.AbstractFont,
     column_width: float = 0.0,
     line_spacing_factor: float = 1.0,
 ) -> tuple[float, float]:
     """Estimate the width and height of the :class:`~ezdxf.entities.MText`
     content string. The result is very inaccurate if inline codes are used or
     line wrapping at the column border is involved!
     Column breaks ``\\N`` will be ignored.
```

## Comparing `ezdxf-1.1.0b0/src/ezdxf/tools/text_layout.py` & `ezdxf-1.1.0b1/src/ezdxf/tools/text_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/tools/text_size.py` & `ezdxf-1.1.0b1/src/ezdxf/tools/text_size.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# Copyright (c) 2021-2022, Manfred Moitzi
+# Copyright (c) 2021-2023, Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
 from typing import Sequence, Optional
 from dataclasses import dataclass
 
-import ezdxf
 from ezdxf.math import Matrix44, Vec2
 from ezdxf.entities import Text, MText, get_font_name
-from ezdxf.tools import text_layout as tl, fonts
+from ezdxf.fonts import fonts
+from ezdxf.tools import text_layout as tl
 from ezdxf.tools.text import MTextContext
 from ezdxf.render.abstract_mtext_renderer import AbstractMTextRenderer
 from ezdxf.tools.text import estimate_mtext_extents
 
 __all__ = [
     "text_size",
     "mtext_size",
```

## Comparing `ezdxf-1.1.0b0/src/ezdxf/tools/ttfonts.py` & `ezdxf-1.1.0b1/src/ezdxf/fonts/ttfonts.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 #  Copyright (c) 2023, Manfred Moitzi
 #  License: MIT License
 from __future__ import annotations
 from typing import Any, no_type_check
 from fontTools.pens.basePen import BasePen
 from fontTools.ttLib import TTFont
 
-import ezdxf.path
 from ezdxf.math import Matrix44, UVec, BoundingBox2d
-from ezdxf.tools.font_manager import FontManager
-from ezdxf.tools.fonts import FontMeasurements
+from .font_manager import FontManager
+from .font_measurements import FontMeasurements
+from .glyphs import GlyphPath, Glyphs
 
 UNICODE_WHITE_SQUARE = 9633  # U+25A1
 UNICODE_REPLACEMENT_CHAR = 65533  # U+FFFD
 
 font_manager = FontManager()
 
 
 class PathPen(BasePen):
     def __init__(self, glyph_set) -> None:
         super().__init__(glyph_set)
-        self._path = ezdxf.path.Path2d()
+        self._path = GlyphPath()
 
     @property
-    def path(self) -> ezdxf.path.Path2d:
+    def path(self) -> GlyphPath:
         return self._path
 
     def _moveTo(self, pt: UVec) -> None:
         self._path.move_to(pt)
 
     def _lineTo(self, pt: UVec) -> None:
         self._path.line_to(pt)
@@ -64,30 +64,31 @@
     names = font["name"].names
     for record in names:
         if record.nameID == 1:
             return record.string.decode(record.getEncoding())
     return "unknown"
 
 
-class TTFontRenderer:
+class TTFontRenderer(Glyphs):
     def __init__(self, font: TTFont, kerning=False):
-        self._glyph_path_cache: dict[str, ezdxf.path.Path2d] = dict()
+        self._glyph_path_cache: dict[str, GlyphPath] = dict()
         self._generic_glyph_cache: dict[str, Any] = dict()
         self._glyph_width_cache: dict[str, float] = dict()
         self.font = font
         self.cmap = self.font.getBestCmap()
         self.glyph_set = self.font.getGlyphSet()
         self.kerning = NoKerning()
         if kerning:
             try:
                 self.kerning = KerningTable(self.font, self.cmap)
             except KeyError:  # kerning table does not exist
                 pass
         self.undefined_generic_glyph = self.glyph_set[".notdef"]
         self.font_measurements = self._get_font_measurements()
+        self.space_width = self.detect_space_width()
 
     @property
     def font_name(self) -> str:
         return get_fontname(self.font)
 
     @no_type_check
     def _get_font_measurements(self) -> FontMeasurements:
@@ -101,27 +102,30 @@
         return FontMeasurements(
             baseline=baseline,
             cap_height=cap_height,
             x_height=x_height,
             descender_height=descender_height,
         )
 
+    def get_scaling_factor(self, cap_height: float) -> float:
+        return 1.0 / self.font_measurements.cap_height * cap_height
+
     def get_generic_glyph(self, char: str):
         try:
             return self._generic_glyph_cache[char]
         except KeyError:
             pass
         try:
             generic_glyph = self.glyph_set[self.cmap[ord(char)]]
         except KeyError:
             generic_glyph = self.undefined_generic_glyph
         self._generic_glyph_cache[char] = generic_glyph
         return generic_glyph
 
-    def get_glyph_path(self, char: str) -> ezdxf.path.Path2d:
+    def get_glyph_path(self, char: str) -> GlyphPath:
         """Returns the raw glyph path, without any scaling applied."""
         try:
             return self._glyph_path_cache[char]
         except KeyError:
             pass
         pen = PathPen(self.glyph_set)
         self.get_generic_glyph(char).draw(pen)
@@ -139,50 +143,62 @@
         try:
             width = self.get_generic_glyph(char).width
         except KeyError:
             pass
         self._glyph_width_cache[char] = width
         return width
 
-    def get_text_path(self, s: str, cap_height: float = 1.0) -> ezdxf.path.Path2d:
+    def get_text_path(
+        self, s: str, cap_height: float = 1.0, width_factor: float = 1.0
+    ) -> GlyphPath:
         """Returns the concatenated glyph paths of string s, scaled to cap height."""
-        text_path = ezdxf.path.Path2d()
+        text_path = GlyphPath()
         x_offset: float = 0
         requires_kerning = isinstance(self.kerning, KerningTable)
         resize_factor = self.get_scaling_factor(cap_height)
+        y_factor = resize_factor
+        x_factor = resize_factor * width_factor
         # set scaling factor:
-        m = Matrix44.scale(resize_factor, resize_factor, 1.0)
+        m = Matrix44.scale(x_factor, y_factor, 1.0)
         # set vertical offset:
-        m[3, 1] = -self.font_measurements.baseline * resize_factor
+        m[3, 1] = -self.font_measurements.baseline * y_factor
         prev_char = ""
+
         for char in s:
             if requires_kerning:
-                x_offset += self.kerning.get(prev_char, char) * resize_factor
+                x_offset += self.kerning.get(prev_char, char) * x_factor
             # set horizontal offset:
             m[3, 0] = x_offset
             glyph_path = self.get_glyph_path(char).transform(m)
             if x_offset == 0:
                 text_path = glyph_path
             elif len(glyph_path):
                 text_path.extend_multi_path(glyph_path)
-            x_offset += self.get_glyph_width(char) * resize_factor
+            x_offset += self.get_glyph_width(char) * x_factor
             prev_char = char
         return text_path
 
-    def get_scaling_factor(self, cap_height: float) -> float:
-        return 1.0 / self.font_measurements.cap_height * cap_height
+    def detect_space_width(self) -> float:
+        """Returns the space width for the raw (unscaled) font."""
+        return self.get_glyph_width(" ")
 
     def _get_text_length_with_kerning(self, s: str, cap_height: float = 1.0) -> float:
         length = 0.0
         c0 = ""
         kern = self.kerning.get
         width = self.get_glyph_width
         for c1 in s:
             length += kern(c0, c1) + width(c1)
             c0 = c1
         return length * self.get_scaling_factor(cap_height)
 
-    def get_text_length(self, s: str, cap_height: float = 1.0) -> float:
+    def get_text_length(
+        self, s: str, cap_height: float = 1.0, width_factor: float = 1.0
+    ) -> float:
         if isinstance(self.kerning, KerningTable):
-            return self._get_text_length_with_kerning(s, cap_height)
+            return self._get_text_length_with_kerning(s, cap_height) * width_factor
         width = self.get_glyph_width
-        return sum(width(c) for c in s) * self.get_scaling_factor(cap_height)
+        return (
+            sum(width(c) for c in s)
+            * self.get_scaling_factor(cap_height)
+            * width_factor
+        )
```

## Comparing `ezdxf-1.1.0b0/src/ezdxf/tools/zipmanager.py` & `ezdxf-1.1.0b1/src/ezdxf/tools/zipmanager.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/tools/_iso_pattern.py` & `ezdxf-1.1.0b1/src/ezdxf/tools/_iso_pattern.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf/tools/__init__.py` & `ezdxf-1.1.0b1/src/ezdxf/tools/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/src/ezdxf.egg-info/PKG-INFO` & `ezdxf-1.1.0b1/src/ezdxf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezdxf
-Version: 1.1.0b0
+Version: 1.1.0b1
 Summary: A Python package to create/manipulate DXF drawings.
 Home-page: https://ezdxf.mozman.at
 Author: Manfred Moitzi
 Author-email: me@mozman.at
 License: MIT License
 Download-URL: https://pypi.org/project/ezdxf/
 Keywords: DXF,CAD
@@ -220,27 +220,30 @@
 
 - Release notes: https://ezdxf.mozman.at/release-v1-1.html
 - WARNING: The font support changed drastically in this version, if you use the 
   `ezdxf.tools.fonts` module your code will break, sorry! Pin the `ezdxf` version to 
   v1.0.3 in your `requirements.txt` file to use the previous version!
 - NEW: `numpy` is a hard dependency, requires Python version >= 3.8
 - NEW: `fontTools` is a hard dependency
-- NEW: `Matrix44.Path2d()` class, `Path` class with `Vec2` vertices
-- NEW: optimized `Matrix44.fast_2d_transform()` method
-- NEW: added setter to `BlockLayout.base_point` property
+- NEW: `ezdxf.path.Path2d()` class, `Path` class with `Vec2` vertices
 - NEW: `ezdxf.xref` new core module to manage XREFs and load resources from DXF files
 - NEW: `ezdxf.addons.hpgl2` add-on to convert HPGL/2 plot files to DXF or SVG
 - NEW: `ezdxf plt2dxf` command to convert HPGL/2 plot files to DXF
 - NEW: `ezdxf plt2svg` command to convert HPGL/2 plot files to SVG
 - NEW: `ezdxf plt2pdf` command to convert HPGL/2 plot files to PDF
-- CHANGED: refactoring of `ezdxf.tools.fonts`
+- NEW: support for measuring and rendering of .shx, .shp and .lff fonts, the basic 
+  stroke fonts included in CAD applications
+- NEW: added setter to `BlockLayout.base_point` property
+- CHANGED: moved font related modules into a new subpackage `ezdxf.fonts` 
+  including a big refactoring
 - CHANGED: `FontFace` class - `weight` attribute is an int value (0-1000), `stretch` is 
   renamed to `width` and is also an int value (1-9) now
 - REMOVED: replaced `matplotlib` font support module by `fontTools`
-- REMOVED: configuration option `use_matplotlib`
+- REMOVED: configuration option `use_matplotlib` - is not needed anymore
+- REMOVED: configuration option `font_cache_directory` - is not needed anymore
 - CHANGED: text rendering for the `drawing` add-on and text measurement is done by the
   `fontTools` package
 - CHANGED: moved text rendering from backend classes to the `Frontend` class
 - CHANGED: moved clipping support from backend classes to the `Frontend` class
 - REMOVED: `PillowBackend` and the `pillow` command
 - REMOVED: `geomdl` test dependency
 - BUGFIX: invalid bulge to Bezier curve conversion for bulge values >= 1
```

## Comparing `ezdxf-1.1.0b0/src/ezdxf.egg-info/SOURCES.txt` & `ezdxf-1.1.0b1/src/ezdxf.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,14 @@
 src/ezdxf/proxygraphic.py
 src/ezdxf/py.typed
 src/ezdxf/query.py
 src/ezdxf/queryparser.py
 src/ezdxf/r12strict.py
 src/ezdxf/recover.py
 src/ezdxf/reorder.py
-src/ezdxf/shapefile.py
 src/ezdxf/transform.py
 src/ezdxf/units.py
 src/ezdxf/upright.py
 src/ezdxf/urecord.py
 src/ezdxf/version.py
 src/ezdxf/xref.py
 src/ezdxf/zoom.py
@@ -202,14 +201,15 @@
 src/ezdxf/addons/drawing/frontend.py
 src/ezdxf/addons/drawing/gfxproxy.py
 src/ezdxf/addons/drawing/matplotlib.py
 src/ezdxf/addons/drawing/mtext_complex.py
 src/ezdxf/addons/drawing/properties.py
 src/ezdxf/addons/drawing/pyqt.py
 src/ezdxf/addons/drawing/qtviewer.py
+src/ezdxf/addons/drawing/recorder.py
 src/ezdxf/addons/drawing/text.py
 src/ezdxf/addons/drawing/text_renderer.py
 src/ezdxf/addons/drawing/type_hints.py
 src/ezdxf/addons/drawing/unified_text_renderer.py
 src/ezdxf/addons/dwg/__init__.py
 src/ezdxf/addons/dwg/classes_section.py
 src/ezdxf/addons/dwg/const.py
@@ -296,14 +296,23 @@
 src/ezdxf/entities/view.py
 src/ezdxf/entities/viewport.py
 src/ezdxf/entities/visualstyle.py
 src/ezdxf/entities/vport.py
 src/ezdxf/entities/xdata.py
 src/ezdxf/entities/xdict.py
 src/ezdxf/entities/xline.py
+src/ezdxf/fonts/__init__.py
+src/ezdxf/fonts/font_face.py
+src/ezdxf/fonts/font_manager.py
+src/ezdxf/fonts/font_measurements.py
+src/ezdxf/fonts/fonts.py
+src/ezdxf/fonts/glyphs.py
+src/ezdxf/fonts/lff.py
+src/ezdxf/fonts/shapefile.py
+src/ezdxf/fonts/ttfonts.py
 src/ezdxf/layouts/__init__.py
 src/ezdxf/layouts/base.py
 src/ezdxf/layouts/blocklayout.py
 src/ezdxf/layouts/layout.py
 src/ezdxf/layouts/layouts.py
 src/ezdxf/lldxf/__init__.py
 src/ezdxf/lldxf/attributes.py
@@ -429,29 +438,25 @@
 src/ezdxf/tools/analyze.py
 src/ezdxf/tools/binarydata.py
 src/ezdxf/tools/codepage.py
 src/ezdxf/tools/complex_ltype.py
 src/ezdxf/tools/crypt.py
 src/ezdxf/tools/debug.py
 src/ezdxf/tools/difftags.py
-src/ezdxf/tools/font_face.py
-src/ezdxf/tools/font_manager.py
-src/ezdxf/tools/fonts.py
 src/ezdxf/tools/handle.py
 src/ezdxf/tools/indexing.py
 src/ezdxf/tools/juliandate.py
 src/ezdxf/tools/pattern.py
 src/ezdxf/tools/rawloader.py
 src/ezdxf/tools/standards.py
 src/ezdxf/tools/strip.py
 src/ezdxf/tools/test.py
 src/ezdxf/tools/text.py
 src/ezdxf/tools/text_layout.py
 src/ezdxf/tools/text_size.py
-src/ezdxf/tools/ttfonts.py
 src/ezdxf/tools/zipmanager.py
 tests/conftest.py
 tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
 tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
 tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
 tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
 tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
@@ -642,15 +647,17 @@
 tests/test_05_tools/test_508_read_zip.py
 tests/test_05_tools/test_509_comments.py
 tests/test_05_tools/test_510_byte_stream.py
 tests/test_05_tools/test_511_bit_stream.py
 tests/test_05_tools/test_512_pattern.py
 tests/test_05_tools/test_513_reorder_entities.py
 tests/test_05_tools/test_514_text.py
-tests/test_05_tools/test_515_fonts.py
+tests/test_05_tools/test_515a_fonts_truetype.py
+tests/test_05_tools/test_515b_fonts_shapefiles.py
+tests/test_05_tools/test_515c_fonts_lff.py
 tests/test_05_tools/test_516_zoom.py
 tests/test_05_tools/test_517_text_layout.py
 tests/test_05_tools/test_518_header_guid.py
 tests/test_05_tools/test_519_mtext_editor.py
 tests/test_05_tools/test_520_mtext_context.py
 tests/test_05_tools/test_521_mtext_parser.py
 tests/test_05_tools/test_522_text_scanner.py
@@ -667,14 +674,15 @@
 tests/test_05_tools/test_533_shapefiles.py
 tests/test_05_tools/test_534_dwg_info.py
 tests/test_05_tools/test_535_xref_basic.py
 tests/test_05_tools/test_536_xref_conflict.py
 tests/test_05_tools/test_537_transform.py
 tests/test_05_tools/test_538_scale_mtext_inline_commands.py
 tests/test_05_tools/test_539_npshapes.py
+tests/test_05_tools/test_540_lff_parser.py
 tests/test_06_math/conftest.py
 tests/test_06_math/test_600_base.py
 tests/test_06_math/test_601_bulge.py
 tests/test_06_math/test_602_vec3.py
 tests/test_06_math/test_603_vec2.py
 tests/test_06_math/test_604_banded_matrix.py
 tests/test_06_math/test_604_linalg.py
@@ -752,15 +760,16 @@
 tests/test_08_addons/test_802_table_painter.py
 tests/test_08_addons/test_803_entities_to_code.py
 tests/test_08_addons/test_804_importer.py
 tests/test_08_addons/test_805_pycsg.py
 tests/test_08_addons/test_806_acadctb.py
 tests/test_08_addons/test_807_dwg_loader_basics.py
 tests/test_08_addons/test_810_drawing_properties.py
-tests/test_08_addons/test_811_drawing_frontend.py
+tests/test_08_addons/test_811a_drawing_frontend.py
+tests/test_08_addons/test_811b_drawing_recorder.py
 tests/test_08_addons/test_812_drawing_graphic_proxy.py
 tests/test_08_addons/test_813_geo_interface.py
 tests/test_08_addons/test_814_text2path.py
 tests/test_08_addons/test_815_dxf_browser.py
 tests/test_08_addons/test_816_bin_packing.py
 tests/test_08_addons/test_817_genetic_algorithm.py
 tests/test_08_addons/test_818_meshex.py
```

## Comparing `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py` & `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py` & `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py` & `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py` & `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py` & `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_010_binary_data.py` & `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_010_binary_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_012_crypt.py` & `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_012_crypt.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_013_juliandate.py` & `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_013_juliandate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py` & `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py` & `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_016_encoding.py` & `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_016_encoding.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_018_handle.py` & `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_018_handle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py` & `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py` & `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py` & `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py` & `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_024_render_tag.py` & `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_024_render_tag.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_040_tags.py` & `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_040_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_041_group_tags.py` & `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_041_group_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py` & `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py` & `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py` & `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py` & `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py` & `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py` & `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py` & `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py` & `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py` & `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py` & `ezdxf-1.1.0b1/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_101_dxfnamespace.py` & `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_101_dxfnamespace.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_102_appdata.py` & `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_102_appdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_103_reactors.py` & `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_103_reactors.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_104_extension_dict.py` & `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_104_extension_dict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_105_xdata.py` & `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_105_xdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_110_dxfentity.py` & `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_110_dxfentity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py` & `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_112a_dxfgfx.py` & `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_112a_dxfgfx.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_112b_dxfobj.py` & `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_112b_dxfobj.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_113_dxfclass.py` & `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_113_dxfclass.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_114_factory.py` & `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_114_factory.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_115_new_empty_drawing.py` & `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_115_new_empty_drawing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_116_dictionary.py` & `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_116_dictionary.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_117_layer_table_entry.py` & `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_117_layer_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_119_ucs_table_entry.py` & `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_119_ucs_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_120_style_table_entry.py` & `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_120_style_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_121_ltype_table_entry.py` & `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_121_ltype_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_123_view_table_entry.py` & `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_123_view_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py` & `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_125_image_def.py` & `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_125_image_def.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_126_image_def_reactor.py` & `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_126_image_def_reactor.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_127_raster_variables.py` & `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_127_raster_variables.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_128_pdf_definition.py` & `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_128_pdf_definition.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_129_xrecord.py` & `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_129_xrecord.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_130_id_buffer.py` & `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_130_id_buffer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_131_field_list.py` & `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_131_field_list.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_132_layer_filter.py` & `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_132_layer_filter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_133_sun.py` & `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_133_sun.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_134_material.py` & `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_134_material.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_135_geo_data.py` & `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_135_geo_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_136_vba_project.py` & `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_136_vba_project.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_137_sortentstable.py` & `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_137_sortentstable.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_138_setup_visual_styles.py` & `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_138_setup_visual_styles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_139_user_record.py` & `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_139_user_record.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_140_block_record.py` & `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_140_block_record.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_141_layer_vp_override.py` & `ezdxf-1.1.0b1/tests/test_01_dxf_entities/test_141_layer_vp_override.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/conftest.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/conftest.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_200_line.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_200_line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_201_point.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_201_point.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_202_circle.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_202_circle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_203_arc.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_203_arc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_204_shape.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_204_shape.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_205_solid.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_205_solid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_206_text.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_206_text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_207_attdef.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_207_attdef.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_208_attrib.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_208_attrib.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_209_vertex.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_209_vertex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_210_polyline_1.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_210_polyline_1.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_210_polyline_2.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_210_polyline_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_210_polyline_explode.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_210_polyline_explode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_211_viewport.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_211_viewport.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_212_insert.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_212_insert.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_213_minsert.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_213_minsert.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_214_block.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_214_block.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_215_dimension.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_215_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_216_dimlines_R12.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_216_dimlines_R12.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_221_ellipse.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_221_ellipse.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_222_xline.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_222_xline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_223_ray.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_223_ray.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_224_group.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_224_group.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_225_mtext.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_225_mtext.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_226_spline.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_226_spline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_228_mesh.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_228_mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_229b_hatch_extended.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_229b_hatch_extended.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_231_underlay.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_231_underlay.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_231_underlay_2.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_231_underlay_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_232_acis.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_232_acis.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_232_acis_2.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_232_acis_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_232_surface.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_232_surface.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_233_helix.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_233_helix.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_234_light.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_234_light.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_235_leader.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_235_leader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_236_multileader.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_236_multileader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_237_mline.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_237_mline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_238_tolerance.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_238_tolerance.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_239_proxy_graphic.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_239_proxy_graphic.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_240_arc_dimension.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_240_arc_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_241_hyperlink.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_241_hyperlink.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_242_random_transform.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_242_random_transform.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_243_replace_entity.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_243_replace_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_245_wipeout.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_245_wipeout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_246_spline_audit.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_246_spline_audit.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_248_mpolygon.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_248_mpolygon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_249_boundary_paths.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_249_boundary_paths.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_251_upright.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_251_upright.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_253_ole2frame.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_253_ole2frame.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_254_get_font_name.py` & `ezdxf-1.1.0b1/tests/test_02_dxf_graphics/test_254_get_font_name.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_300_layout.py` & `ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_300_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py` & `ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_302_block_references.py` & `ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_302_block_references.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_303_auto_block_references.py` & `ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_303_auto_block_references.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_304_new_entity_space.py` & `ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_304_new_entity_space.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py` & `ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py` & `ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_307_groupby.py` & `ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_307_groupby.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_308_query.py` & `ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_308_query.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_309_query_parser.py` & `ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_309_query_parser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py` & `ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_312_virtual_layout.py` & `ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_312_virtual_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_313_redraw_order.py` & `ezdxf-1.1.0b1/tests/test_03_dxf_layouts/test_313_redraw_order.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_401_headersection.py` & `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_401_headersection.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_402_classessection.py` & `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_402_classessection.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_403_entity_database.py` & `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_403_entity_database.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_404a_tables.py` & `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_404a_tables.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py` & `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_405_classes.py` & `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_405_classes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py` & `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_407_entity_section.py` & `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_407_entity_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_408_objects_section.py` & `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_408_objects_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_409_create_objects.py` & `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_409_create_objects.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_410_table.py` & `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_410_table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_411_acds_data.py` & `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_411_acds_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py` & `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py` & `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py` & `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_415_layout_management.py` & `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_415_layout_management.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py` & `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py`

 * *Files 2% similar despite different names*

```diff
@@ -287,16 +287,16 @@
     p = disassemble.make_primitive(text)
     assert p.is_empty is False
     assert p.path is not None
     assert p.mesh is None
     assert len(list(p.vertices())) == 5, "expected closed box"
 
     box = p.bbox()
-    # exact bounding box size depends on platform and matplotlib usage!
-    assert 18 < box.size.x < 22
+    # exact bounding box size depends on available fonts
+    assert 18 < box.size.x < 24
     assert box.size.y > 2.5
 
 
 def test_mtext_to_primitive():
     # Testing just the control flow, correct bounding boxes are visually tested.
     # see: ezdxf/examples/entities/mtext.py
     mtext = factory.new("MTEXT")
@@ -304,16 +304,16 @@
     p = disassemble.make_primitive(mtext)
     assert p.is_empty is False
     assert p.path is not None
     assert p.mesh is None
     assert len(list(p.vertices())) == 5, "expected closed box"
 
     box = p.bbox()
-    # exact bounding box size depends on platform and matplotlib usage!
-    assert 18 < box.size.x < 22  # pypy
+    # exact bounding box size depends on available fonts
+    assert 18 < box.size.x < 24  # txt.shx
     assert box.size.y > 2.5
 
 
 def test_mtext_columns_to_primitive():
     from ezdxf.entities.mtext import MTextColumns
 
     mtext = factory.new("MTEXT")
```

## Comparing `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py` & `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_417_bbox.py` & `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_417_bbox.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py` & `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py` & `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py` & `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py` & `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py` & `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_424_audit.py` & `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_424_audit.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py` & `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py` & `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_427_appsettings.py` & `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_427_appsettings.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py` & `ezdxf-1.1.0b1/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_05_tools/conftest.py` & `ezdxf-1.1.0b1/tests/test_05_tools/conftest.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_05_tools/test_500_units.py` & `ezdxf-1.1.0b1/tests/test_05_tools/test_500_units.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_05_tools/test_501_truecolor.py` & `ezdxf-1.1.0b1/tests/test_05_tools/test_501_truecolor.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_05_tools/test_502_raw_color.py` & `ezdxf-1.1.0b1/tests/test_05_tools/test_502_raw_color.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_05_tools/test_503_indexing.py` & `ezdxf-1.1.0b1/tests/test_05_tools/test_503_indexing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_05_tools/test_504_suppress_zeros.py` & `ezdxf-1.1.0b1/tests/test_05_tools/test_504_suppress_zeros.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_05_tools/test_507_dxf_pretty_printer.py` & `ezdxf-1.1.0b1/tests/test_05_tools/test_507_dxf_pretty_printer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_05_tools/test_508_read_zip.py` & `ezdxf-1.1.0b1/tests/test_05_tools/test_508_read_zip.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_05_tools/test_509_comments.py` & `ezdxf-1.1.0b1/tests/test_05_tools/test_509_comments.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_05_tools/test_510_byte_stream.py` & `ezdxf-1.1.0b1/tests/test_05_tools/test_510_byte_stream.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_05_tools/test_511_bit_stream.py` & `ezdxf-1.1.0b1/tests/test_05_tools/test_511_bit_stream.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_05_tools/test_512_pattern.py` & `ezdxf-1.1.0b1/tests/test_05_tools/test_512_pattern.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_05_tools/test_513_reorder_entities.py` & `ezdxf-1.1.0b1/tests/test_05_tools/test_513_reorder_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_05_tools/test_514_text.py` & `ezdxf-1.1.0b1/tests/test_05_tools/test_514_text.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     fast_plain_mtext,
     plain_mtext,
     has_inline_formatting_codes,
     is_upside_down_text_angle,
     upright_text_angle,
     estimate_mtext_content_extents,
 )
-from ezdxf.tools.fonts import MonospaceFont
+from ezdxf.fonts.fonts import MonospaceFont
 from ezdxf.enums import TextEntityAlignment
 from ezdxf.math import Vec3
 from ezdxf.lldxf import const
 
 
 @pytest.fixture
 def font():
```

## Comparing `ezdxf-1.1.0b0/tests/test_05_tools/test_516_zoom.py` & `ezdxf-1.1.0b1/tests/test_05_tools/test_516_zoom.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_05_tools/test_517_text_layout.py` & `ezdxf-1.1.0b1/tests/test_05_tools/test_517_text_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_05_tools/test_519_mtext_editor.py` & `ezdxf-1.1.0b1/tests/test_05_tools/test_519_mtext_editor.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_05_tools/test_520_mtext_context.py` & `ezdxf-1.1.0b1/tests/test_05_tools/test_520_mtext_context.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_05_tools/test_521_mtext_parser.py` & `ezdxf-1.1.0b1/tests/test_05_tools/test_521_mtext_parser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_05_tools/test_522_text_scanner.py` & `ezdxf-1.1.0b1/tests/test_05_tools/test_522_text_scanner.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_05_tools/test_523_text_size.py` & `ezdxf-1.1.0b1/tests/test_05_tools/test_523_text_size.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_05_tools/test_524_block_reference_manager.py` & `ezdxf-1.1.0b1/tests/test_05_tools/test_524_block_reference_manager.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_05_tools/test_525_transparency.py` & `ezdxf-1.1.0b1/tests/test_05_tools/test_525_transparency.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_05_tools/test_526_explode.py` & `ezdxf-1.1.0b1/tests/test_05_tools/test_526_explode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_05_tools/test_527_gfxattribs.py` & `ezdxf-1.1.0b1/tests/test_05_tools/test_527_gfxattribs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_05_tools/test_528_difftags.py` & `ezdxf-1.1.0b1/tests/test_05_tools/test_528_difftags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_05_tools/test_529_acis_sat.py` & `ezdxf-1.1.0b1/tests/test_05_tools/test_529_acis_sat.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_05_tools/test_530_acis_sab.py` & `ezdxf-1.1.0b1/tests/test_05_tools/test_530_acis_sab.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_05_tools/test_531_acis_entities.py` & `ezdxf-1.1.0b1/tests/test_05_tools/test_531_acis_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_05_tools/test_532_acis_mesh.py` & `ezdxf-1.1.0b1/tests/test_05_tools/test_532_acis_mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_05_tools/test_533_shapefiles.py` & `ezdxf-1.1.0b1/tests/test_05_tools/test_533_shapefiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 #  Copyright (c) 2022, Manfred Moitzi
 #  License: MIT License
 
 import pytest
-from ezdxf import shapefile, path
+from ezdxf.fonts import shapefile
+from ezdxf import path
+from ezdxf.math import BoundingBox2d
 
 
 def test_filter_noise():
     lines = list(
         shapefile.filter_noise(
             b"""
     ;; comment
@@ -287,14 +289,29 @@
         assert p.start.isclose((-2, 30))
         p2 = shp.render_shape(0x43)
         assert p2.end.isclose((64, 0))
         assert p2.end.isclose(
             p.end
         ), "should be perfect rendering - no placing-hack required"
 
+    def test_unsupported_non_printable_shape_number_returns_empty_path(self, shp):
+        cache = shapefile.GlyphCache(shp)
+        p = cache.get_shape(10)
+        assert len(p) == 0
+
+    def test_unsupported_printable_shape_number_returns_empty_box(self, shp):
+        cache = shapefile.GlyphCache(shp)
+        box = cache.get_shape(1234)
+        assert box is cache.empty_box
+        assert box.end.x == cache.space_width
+
+    def test_empty_box_has_advance_width_like_glyph_A(self, shp):
+        cache = shapefile.GlyphCache(shp)
+        assert cache.get_advance_width(1234) == cache.get_advance_width(65)
+
 
 FILE_1 = b"""
 ;; isocp.shp
 *00026,41,&
 2,8,(30,14),1,3,10,4,2,8,(-72,-54),3,2,12,(-89,76,-102),4,4,
 8,(31,45),3,4,4,10,11,(68,187,0,6,076),8,(17,-27),2,8,(10,-2),0
```

## Comparing `ezdxf-1.1.0b0/tests/test_05_tools/test_534_dwg_info.py` & `ezdxf-1.1.0b1/tests/test_05_tools/test_534_dwg_info.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_05_tools/test_535_xref_basic.py` & `ezdxf-1.1.0b1/tests/test_05_tools/test_535_xref_basic.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_05_tools/test_536_xref_conflict.py` & `ezdxf-1.1.0b1/tests/test_05_tools/test_536_xref_conflict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_05_tools/test_537_transform.py` & `ezdxf-1.1.0b1/tests/test_05_tools/test_537_transform.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_05_tools/test_538_scale_mtext_inline_commands.py` & `ezdxf-1.1.0b1/tests/test_05_tools/test_538_scale_mtext_inline_commands.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_05_tools/test_539_npshapes.py` & `ezdxf-1.1.0b1/tests/test_05_tools/test_539_npshapes.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 #  Copyright (c) 2023, Manfred Moitzi
 #  License: MIT License
 
 import pytest
 
-from ezdxf.npshapes import NumpyPolyline, NumpyPath
+from ezdxf.npshapes import NumpyPoints2d, NumpyPath2d
 from ezdxf.math import Matrix44, BoundingBox2d
 from ezdxf.path import Path2d, Command
 
 
-class TestNumpyPolyline:
+class TestNumpyPoints:
     @pytest.fixture
     def points(self):
         return [(1, 2), (7, 4), (4, 7), (0, 1)]
 
     def test_conversion(self, points):
-        pl = NumpyPolyline(points)
+        pl = NumpyPoints2d(points)
         assert len(pl) == len(points)
         assert all(v0.isclose(v1) for v0, v1 in zip(pl.vertices(), points))
 
-    def test_bounding_box(self, points):
-        pl = NumpyPolyline(points)
-        bbox = pl.bbox()
-        assert bbox.extmin.isclose((0, 1))
-        assert bbox.extmax.isclose((7, 7))
+    def test_extents(self, points):
+        pl = NumpyPoints2d(points)
+        extmin, extmax = pl.extents()
+        assert extmin.isclose((0, 1))
+        assert extmax.isclose((7, 7))
 
     def test_transform_inplace(self, points):
         m = Matrix44.translate(7, 8, 0)
         t_pts = m.fast_2d_transform(points)
-        pl = NumpyPolyline(points)
+        pl = NumpyPoints2d(points)
         pl.transform_inplace(m)
         assert all(v0.isclose(v1) for v0, v1 in zip(pl.vertices(), t_pts))
 
 
 class TestNumpyPath:
     @pytest.fixture
     def path(self):
@@ -39,15 +39,15 @@
         p.line_to((7, 4))
         p.curve3_to((4, 7), (0, 1))
         p.move_to((10, 0))
         p.curve4_to((15, 7), (13, 3), (14, 5))
         return p
 
     def test_to_path_2d(self, path):
-        np_path = NumpyPath(path)
+        np_path = NumpyPath2d(path)
         assert len(np_path) == len(path)
 
         path2d = np_path.to_path2d()
         assert len(path2d) == 4
         assert path2d.start.isclose((1, 2))
         assert path2d.end.isclose((15, 7))
 
@@ -63,27 +63,39 @@
         assert cmds[2].end.isclose((10, 0))
 
         assert cmds[3].type == Command.CURVE4_TO
         assert cmds[3].end.isclose((15, 7))
         assert cmds[3].ctrl1.isclose((13, 3))
         assert cmds[3].ctrl2.isclose((14, 5))
 
-    def test_bounding_box(self, path):
-        np_path = NumpyPath(path)
-        np_bbox = np_path.bbox()
+    def test_extents(self, path):
+        np_path = NumpyPath2d(path)
+        extmin, extmax = np_path.extents()
         box = BoundingBox2d(path.control_vertices())
 
-        assert np_bbox.extmin.isclose(box.extmin)
-        assert np_bbox.extmax.isclose(box.extmax)
+        assert extmin.isclose(box.extmin)
+        assert extmax.isclose(box.extmax)
 
     def test_transform(self, path):
         m = Matrix44.scale(2, 3, 1) @ Matrix44.translate(-2, 10, 0)
-        np_path = NumpyPath(path)
+        np_path = NumpyPath2d(path)
         np_path.transform_inplace(m)
         assert all(
             v0.isclose(v1)
             for v0, v1 in zip(np_path.vertices(), path.transform(m).control_vertices())
         )
 
+    def test_start_point_only_path(self):
+        p = NumpyPath2d(Path2d((10, 20)))
+        assert p.vertices()[0].isclose((10, 20))
+        # and back
+        assert p.to_path2d().start.isclose((10, 20))
+
+    def test_real_empty_path(self):
+        p = NumpyPath2d(Path2d())
+        assert len(p) == 0
+        # and back
+        assert p.to_path2d().start == (0, 0)  # default start point
+
 
 if __name__ == "__main__":
     pytest.main([__file__])
```

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/conftest.py` & `ezdxf-1.1.0b1/tests/test_06_math/conftest.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_600_base.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_600_base.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_601_bulge.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_601_bulge.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_602_vec3.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_602_vec3.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_603_vec2.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_603_vec2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_604_banded_matrix.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_604_banded_matrix.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_604_linalg.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_604_linalg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_605_matrix44.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_605_matrix44.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (c) 2010-2023, Manfred Moitzi
 # License: MIT License
 import pytest
 import pickle
 from math import radians, sin, cos, pi, isclose
+import numpy as np
 
 # Import from 'ezdxf.math._matrix44' to test Python implementation
 from ezdxf.math import (
     close_vectors,
     has_matrix_2d_stretching,
     has_matrix_3d_stretching,
 )
@@ -367,7 +368,33 @@
         m = m44.scale(2, 3, 4) @ m44.z_rotate(radians(90)) @ m44.translate(10, 20, 0)
         points = [(10, 10), (-20, -20, 1)]
         res_3d = list(m.transform_vertices(points))
         res_2d = list(m.fast_2d_transform(points))
 
         assert res_2d[0].isclose(res_3d[0])
         assert res_2d[1].isclose(res_3d[1])
+
+
+class TestTransformArrayInplace:
+    def test_ndim_2(self, m44):
+        points = (23.0, 97.0), (2.0, 7.0)
+        s = m44.scale(10, 20, 1)
+        t = m44.translate(10, 20, 0)
+        r = m44.z_rotate(angle=pi / 2)
+        m = m44.chain(s, r, t)
+        array = np.array(points, dtype=np.float64)
+
+        control = list(m.fast_2d_transform(points))
+        m.transform_array_inplace(array, ndim=2)
+        assert close_vectors(control, array) is True
+
+    def test_ndim_3(self, m44):
+        points = (23.0, 97.0, 0.5), (2.0, 7.0, 13.0)
+        s = m44.scale(10, 20, 30)
+        t = m44.translate(10, 20, 30)
+        r = m44.z_rotate(angle=pi / 2)
+        m = m44.chain(s, r, t)
+        array = np.array(points, dtype=np.float64)
+
+        control = list(m.transform_vertices(points))
+        m.transform_array_inplace(array, ndim=3)
+        assert close_vectors(control, array) is True
```

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_606_convexhull.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_606_convexhull.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_607_perlin_noise.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_607_perlin_noise.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_608_intersection_line_line_2d.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_608_intersection_line_line_2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_609_point_on_line.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_609_point_on_line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_610_ocs.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_610_ocs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_611_ucs.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_611_ucs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_612_ucs_pass_trough.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_612_ucs_pass_trough.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_613_point_in_poygon.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_613_point_in_poygon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_614_construct_3d.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_614_construct_3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_615_rytz_axis.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_615_rytz_axis.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_616_plane.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_616_plane.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_617_clockwise_orientation.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_617_clockwise_orientation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_618_clipping.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_618_clipping.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_619_greiner_hormann.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_619_greiner_hormann.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_620_knot.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_620_knot.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_621_bspline.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_621_bspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_622_bsplineu.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_622_bsplineu.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_623_rbspline.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_623_rbspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_624_global_bspline_interpolation.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_624_global_bspline_interpolation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_626_local_bspline_interpolation.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_626_local_bspline_interpolation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_627_bspline_basis.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_627_bspline_basis.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_629_bezier.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_629_bezier.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_630a_bezier4p_base.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_630a_bezier4p_base.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_630b_bezier4p_functions.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_630b_bezier4p_functions.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_631_euler_spiral.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_631_euler_spiral.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_632_bezier3p.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_632_bezier3p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_640_bbox.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_640_bbox.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_641_construction_ray.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_641_construction_ray.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_642_construction_line.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_642_construction_line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_643_construction_box.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_643_construction_box.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_644_construction_circle.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_644_construction_circle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_645_construction_arc.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_645_construction_arc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_646_offset_vertices_2d.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_646_offset_vertices_2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_647_transform_tools.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_647_transform_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_648_construction_ellipse.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_648_construction_ellipse.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_650_elliptic_arc_span.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_650_elliptic_arc_span.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_651_construction_polyline.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_651_construction_polyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_652_approx_param_t.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_652_approx_param_t.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_653_polyline_intersection.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_653_polyline_intersection.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_654_rtree.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_654_rtree.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_655_dbscan.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_655_dbscan.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_656_k_means.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_656_k_means.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_657_mapbox_earcut.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_657_mapbox_earcut.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_658_bevel_tools.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_658_bevel_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_659_intersection_line_polygon_3d.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_659_intersection_line_polygon_3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_660_intersection_ray_polygon_3d.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_660_intersection_ray_polygon_3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_06_math/test_662_is_convex_polygon_2d.py` & `ezdxf-1.1.0b1/tests/test_06_math/test_662_is_convex_polygon_2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_07_render/test_701_arrows.py` & `ezdxf-1.1.0b1/tests/test_07_render/test_701_arrows.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_07_render/test_702_render_forms.py` & `ezdxf-1.1.0b1/tests/test_07_render/test_702_render_forms.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_07_render/test_703_mesh_builder.py` & `ezdxf-1.1.0b1/tests/test_07_render/test_703_mesh_builder.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_07_render/test_704_render_linear_dimension.py` & `ezdxf-1.1.0b1/tests/test_07_render/test_704_render_linear_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_07_render/test_705_shape.py` & `ezdxf-1.1.0b1/tests/test_07_render/test_705_shape.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_07_render/test_707_trace.py` & `ezdxf-1.1.0b1/tests/test_07_render/test_707_trace.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_07_render/test_708a_path.py` & `ezdxf-1.1.0b1/tests/test_07_render/test_708a_path.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_07_render/test_708b_path_tools.py` & `ezdxf-1.1.0b1/tests/test_07_render/test_708b_path_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_07_render/test_708c_matplotlib_path_tools.py` & `ezdxf-1.1.0b1/tests/test_07_render/test_708c_matplotlib_path_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_07_render/test_708d_qpainter_path_tools.py` & `ezdxf-1.1.0b1/tests/test_07_render/test_708d_qpainter_path_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_07_render/test_708e_path_shapes.py` & `ezdxf-1.1.0b1/tests/test_07_render/test_708e_path_shapes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_07_render/test_708f_path_nesting.py` & `ezdxf-1.1.0b1/tests/test_07_render/test_708f_path_nesting.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_07_render/test_709_linetype_renderer.py` & `ezdxf-1.1.0b1/tests/test_07_render/test_709_linetype_renderer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_07_render/test_711_points.py` & `ezdxf-1.1.0b1/tests/test_07_render/test_711_points.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_07_render/test_712_render_curved_dimension.py` & `ezdxf-1.1.0b1/tests/test_07_render/test_712_render_curved_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_07_render/test_713_mleader_builder.py` & `ezdxf-1.1.0b1/tests/test_07_render/test_713_mleader_builder.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_07_render/test_714_mleader_render_engine.py` & `ezdxf-1.1.0b1/tests/test_07_render/test_714_mleader_render_engine.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_07_render/test_715_hatching.py` & `ezdxf-1.1.0b1/tests/test_07_render/test_715_hatching.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_07_render/test_715_issue_747_explode_3d_dim.py` & `ezdxf-1.1.0b1/tests/test_07_render/test_715_issue_747_explode_3d_dim.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_08_addons/test_800_mtext_surrogate.py` & `ezdxf-1.1.0b1/tests/test_08_addons/test_800_mtext_surrogate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_08_addons/test_801_r12spline.py` & `ezdxf-1.1.0b1/tests/test_08_addons/test_801_r12spline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_08_addons/test_802_table_painter.py` & `ezdxf-1.1.0b1/tests/test_08_addons/test_802_table_painter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_08_addons/test_803_entities_to_code.py` & `ezdxf-1.1.0b1/tests/test_08_addons/test_803_entities_to_code.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_08_addons/test_804_importer.py` & `ezdxf-1.1.0b1/tests/test_08_addons/test_804_importer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_08_addons/test_805_pycsg.py` & `ezdxf-1.1.0b1/tests/test_08_addons/test_805_pycsg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_08_addons/test_806_acadctb.py` & `ezdxf-1.1.0b1/tests/test_08_addons/test_806_acadctb.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_08_addons/test_807_dwg_loader_basics.py` & `ezdxf-1.1.0b1/tests/test_08_addons/test_807_dwg_loader_basics.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_08_addons/test_810_drawing_properties.py` & `ezdxf-1.1.0b1/tests/test_08_addons/test_810_drawing_properties.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_08_addons/test_811_drawing_frontend.py` & `ezdxf-1.1.0b1/tests/test_08_addons/test_811a_drawing_frontend.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # Copyright (c) 2020-2022, Manfred Moitzi
 # License: MIT License
 
 import pytest
 import ezdxf
 from ezdxf.addons.drawing import Frontend, RenderContext
-from ezdxf.addons.drawing.properties import Properties
+from ezdxf.addons.drawing.properties import BackendProperties
 
 from ezdxf.addons.drawing.backend import Backend
 from ezdxf.addons.drawing.debug_backend import BasicBackend, PathBackend
 from ezdxf.entities import DXFGraphic
 from ezdxf.render.forms import cube
 from ezdxf.path import from_vertices
 
 
 @pytest.fixture
 def doc():
     d = ezdxf.new()
     d.layers.new("Test1")
+    d.styles.add("DEJAVU", font="DejaVuSans.ttf")
     return d
 
 
 @pytest.fixture
 def msp(doc):
     return doc.modelspace()
 
@@ -40,140 +41,142 @@
     return Frontend(ctx, PathBackend())
 
 
 def unique_types(result):
     return {e[0] for e in result}
 
 
+def get_result(frontend):
+    return frontend.out.collector
+
+
 def test_basic_frontend_init(basic):
     assert isinstance(basic.out, BasicBackend)
 
 
 def test_backend_default_draw_path():
     backend = BasicBackend()
     path = from_vertices([(0, 0), (1, 0), (2, 0)])
-    backend.draw_path(path, Properties())
+    backend.draw_path(path, BackendProperties())
     result = backend.collector
     assert len(result) == 2
     assert result[0][0] == "line"
 
 
 def test_draw_layout(msp, basic):
     msp.add_point((0, 0))
     msp.add_point((0, 0))
     basic.draw_layout(msp)
-    result = basic.out.collector
+    result = get_result(basic)
     assert len(result) == 3
     assert result[0][0] == "bgcolor"
     assert result[1][0] == "point"
     assert result[2][0] == "point"
 
 
 def test_draw_entities(msp, basic):
     msp.add_point((0, 0))
     msp.add_point((0, 0))
 
     basic.draw_entities(msp)
-    result = basic.out.collector
+    result = get_result(basic)
     assert len(result) == 2
     assert result[0][0] == "point"
     assert result[1][0] == "point"
 
 
 def test_filter_draw_entities(msp, basic):
     def filter_layer_l1(e: DXFGraphic) -> bool:
         return e.dxf.layer == "L1"
 
     msp.add_point((0, 0), dxfattribs={"layer": "L1"})
     msp.add_point((0, 0), dxfattribs={"layer": "L2"})
 
     basic.draw_entities(msp, filter_func=filter_layer_l1)
-    result = basic.out.collector
+    result = get_result(basic)
     assert len(result) == 1
     assert result[0][2].layer == "L1"
 
 
 def test_point_and_layers(msp, basic):
     msp.add_point((0, 0), dxfattribs={"layer": "Test1"})
     # a non-existing layer shouldn't be a problem
     msp.add_point((0, 0), dxfattribs={"layer": "fail"})
     basic.draw_entities(msp)
-    result = basic.out.collector
+    result = get_result(basic)
     assert len(result) == 2
     assert result[0][0] == "point"
     assert result[0][-1].layer == "Test1"
     assert result[1][0] == "point"
     assert result[1][-1].layer == "fail"
 
 
 def test_line(msp, basic):
     msp.add_line((0, 0), (1, 0))
     basic.draw_entities(msp)
-    result = basic.out.collector
+    result = get_result(basic)
     assert len(result) == 1
     assert result[0][0] == "line"
 
 
 def test_lwpolyline_basic(msp, basic):
     msp.add_lwpolyline([(0, 0), (1, 0), (2, 0)])
     basic.draw_entities(msp)
-    result = basic.out.collector
+    result = get_result(basic)
     assert len(result) == 2
     assert unique_types(result) == {"line"}
 
 
 def test_lwpolyline_path(msp, path_backend):
     msp.add_lwpolyline([(0, 0), (1, 0), (2, 0)])
     path_backend.draw_entities(msp)
-    result = path_backend.out.collector
+    result = get_result(path_backend)
     assert len(result) == 1
     assert unique_types(result) == {"path"}
 
 
 def test_banded_lwpolyline(msp, basic):
-    msp.add_lwpolyline(
-        [(0, 0), (1, 0), (2, 0)], dxfattribs={"const_width": 0.1}
-    )
+    msp.add_lwpolyline([(0, 0), (1, 0), (2, 0)], dxfattribs={"const_width": 0.1})
     basic.draw_entities(msp)
-    result = basic.out.collector
+    result = get_result(basic)
     assert len(result) == 1
     assert unique_types(result) == {"filled_polygon"}
 
 
 def test_polyline_2d(msp, basic):
     msp.add_polyline2d([(0, 0), (1, 0), (2, 0)])
     basic.draw_entities(msp)
-    result = basic.out.collector
+    result = get_result(basic)
     assert len(result) == 2
     assert result[0][0] == "line"
     assert result[1][0] == "line"
 
 
 def test_banded_polyline_2d(msp, basic):
     msp.add_polyline2d(
         [(0, 0, 0.1, 0.2), (1, 0, 0.2, 0.1), (2, 0, 0.1, 0.5)], format="xyse"
     )
     basic.draw_entities(msp)
-    result = basic.out.collector
+    result = get_result(basic)
     assert len(result) == 1
     assert result[0][0] == "filled_polygon"
 
 
 def test_polyline_3d_basic(msp, basic):
     msp.add_polyline3d([(0, 0, 0), (1, 0, 1), (2, 0, 5)])
     basic.draw_entities(msp)
-    result = basic.out.collector
+    result = get_result(basic)
     assert len(result) == 2
     assert unique_types(result) == {"line"}
 
 
 def test_polyline_3d_path(msp, path_backend):
     msp.add_polyline3d([(0, 0, 0), (1, 0, 1), (2, 0, 5)])
     path_backend.draw_entities(msp)
-    result = path_backend.out.collector
+    result = get_result(path_backend)
     assert len(result) == 1
     assert unique_types(result) == {"path"}
 
 
 def test_2d_arc_basic(msp, basic):
     msp.add_circle((0, 0), radius=2)
     msp.add_arc(
@@ -188,183 +191,185 @@
         major_axis=(1, 0, 0),
         ratio=0.5,
         start_param=1,
         end_param=2,
         dxfattribs={"layer": "Test1"},
     )
     basic.draw_entities(msp)
-    result = basic.out.collector
+    result = get_result(basic)
     assert len(result) > 3
     assert unique_types(result) == {"line"}
 
 
 def test_3d_circle_basic(msp, basic):
     msp.add_circle((0, 0), radius=2, dxfattribs={"extrusion": (0, 1, 1)})
     basic.draw_entities(msp)
-    result = basic.out.collector
+    result = get_result(basic)
     assert len(result) > 30
     assert unique_types(result) == {"line"}
 
 
 def test_3d_circle_path(msp, path_backend):
     msp.add_circle((0, 0), radius=2, dxfattribs={"extrusion": (0, 1, 1)})
     path_backend.draw_entities(msp)
-    result = path_backend.out.collector
+    result = get_result(path_backend)
     assert len(result) == 1
     assert unique_types(result) == {"path"}
 
 
 def test_3d_arc_basic(msp, basic):
     msp.add_arc(
         (0, 0),
         radius=2,
         start_angle=30,
         end_angle=60,
         dxfattribs={"extrusion": (0, 1, 1)},
     )
     basic.draw_entities(msp)
-    result = basic.out.collector
+    result = get_result(basic)
     assert len(result) > 10
     assert unique_types(result) == {"line"}
 
 
 def test_3d_arc_path(msp, path_backend):
     msp.add_arc(
         (0, 0),
         radius=2,
         start_angle=30,
         end_angle=60,
         dxfattribs={"extrusion": (0, 1, 1)},
     )
     path_backend.draw_entities(msp)
-    result = path_backend.out.collector
+    result = get_result(path_backend)
     assert len(result) == 1
     assert unique_types(result) == {"path"}
 
 
 def test_3d_ellipse_basic(msp, basic):
     msp.add_ellipse(
         (0, 0),
         major_axis=(1, 0, 0),
         ratio=0.5,
         start_param=1,
         end_param=2,
         dxfattribs={"extrusion": (0, 1, 1)},
     )
     basic.draw_entities(msp)
-    result = basic.out.collector
+    result = get_result(basic)
     assert len(result) > 10
     assert unique_types(result) == {"line"}
 
 
 def test_3d_ellipse_path(msp, path_backend):
     msp.add_ellipse(
         (0, 0),
         major_axis=(1, 0, 0),
         ratio=0.5,
         start_param=1,
         end_param=2,
         dxfattribs={"extrusion": (0, 1, 1)},
     )
     path_backend.draw_entities(msp)
-    result = path_backend.out.collector
+    result = get_result(path_backend)
     assert len(result) == 1
     assert unique_types(result) == {"path"}
 
 
 def test_2d_text(msp, basic):
     # since v1.0.4 the frontend does the text rendering and passes only filled
     # polygons to the backend
-    msp.add_text("test\ntest")  # \n shouldn't be  problem. Will be ignored
+    msp.add_text(
+        "test\ntest", dxfattribs={"style": "DEJAVU"}
+    )  # \n shouldn't be  problem. Will be ignored
     basic.draw_entities(msp)
-    result = basic.out.collector
+    result = get_result(basic)
     assert len(result) == 8
     assert result[0][0] == "filled_polygon"
 
 
 def test_ignore_3d_text(msp, basic):
     msp.add_text("test", dxfattribs={"extrusion": (0, 1, 1)})
     basic.draw_entities(msp)
-    result = basic.out.collector
+    result = get_result(basic)
     assert len(result) == 0
 
 
 def test_mtext(msp, basic):
     # since v1.0.4 the frontend does the text rendering and passes only filled
     # polygons to the backend
-    msp.add_mtext("line1\nline2")
+    msp.add_mtext("line1\nline2", dxfattribs={"style": "DEJAVU"})
     basic.draw_entities(msp)
-    result = basic.out.collector
+    result = get_result(basic)
     assert len(result) == 12
     assert result[0][0] == "filled_polygon"
 
 
 def test_hatch(msp, path_backend):
     hatch = msp.add_hatch()
     hatch.paths.add_polyline_path([(0, 0), (1, 0), (1, 1), (0, 1)])
     path_backend.draw_entities(msp)
-    result = path_backend.out.collector
+    result = get_result(path_backend)
     assert len(result) == 1
-    assert result[0][0] == "filled_polygon"  # default implementation
+    assert result[0][0] == "filled_path"
 
 
 def test_basic_spline(msp, basic):
     msp.add_spline(fit_points=[(0, 0), (3, 2), (4, 5), (6, 4), (12, 0)])
     basic.draw_entities(msp)
-    result = basic.out.collector
+    result = get_result(basic)
     assert len(result) > 1
     entities = {e[0] for e in result}
     assert entities == {"line"}
 
 
 def test_mesh(msp, basic):
     # draw mesh as wire frame
     c = cube()
     c.render_mesh(msp)
     basic.draw_entities(msp)
-    result = basic.out.collector
+    result = get_result(basic)
     assert len(result) == 24
     assert unique_types(result) == {"line"}
 
 
 def test_polyface(msp, basic):
     # draw mesh as wire frame
     c = cube()
     c.render_polyface(msp)
     basic.draw_entities(msp)
-    result = basic.out.collector
+    result = get_result(basic)
     assert len(result) == 24
     entities = {e[0] for e in result}
     assert entities == {"line"}
 
 
 def test_override_filter(msp, ctx):
     class FrontendWithOverride(Frontend):
         def __init__(self, ctx: RenderContext, out: Backend):
             super().__init__(ctx, out)
             self.override_enabled = True
 
         def override_properties(
-            self, entity: DXFGraphic, properties: Properties
+            self, entity: DXFGraphic, properties: BackendProperties
         ) -> None:
             if not self.override_enabled:
                 return
             if properties.layer == "T1":
                 properties.layer = "Tx"
             properties.color = "#000000"
             if entity.dxf.text == "T2":
                 properties.is_visible = False
 
     backend = BasicBackend()
     frontend = FrontendWithOverride(ctx, backend)
 
     msp.delete_all_entities()
-    msp.add_text("T0", dxfattribs={"layer": "T0", "color": 7})
-    msp.add_text("T1", dxfattribs={"layer": "T1", "color": 6})
-    msp.add_text("T2", dxfattribs={"layer": "T2", "color": 5})
+    msp.add_text("T0", dxfattribs={"layer": "T0", "color": 7, "style": "DEJAVU"})
+    msp.add_text("T1", dxfattribs={"layer": "T1", "color": 6, "style": "DEJAVU"})
+    msp.add_text("T2", dxfattribs={"layer": "T2", "color": 5, "style": "DEJAVU"})
     frontend.draw_entities(msp)
     frontend.override_enabled = False
     frontend.draw_entities(msp)
 
     # since v1.0.4 the frontend does the text rendering and passes only filled
     # polygons to the backend
     assert len(backend.collector) == 10
```

## Comparing `ezdxf-1.1.0b0/tests/test_08_addons/test_812_drawing_graphic_proxy.py` & `ezdxf-1.1.0b1/tests/test_08_addons/test_812_drawing_graphic_proxy.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_08_addons/test_813_geo_interface.py` & `ezdxf-1.1.0b1/tests/test_08_addons/test_813_geo_interface.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_08_addons/test_814_text2path.py` & `ezdxf-1.1.0b1/tests/test_08_addons/test_814_text2path.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,26 @@
 #  Copyright (c) 2021-2023, Manfred Moitzi
 #  License: MIT License
 
 import pytest
-import platform
-
-if platform.system() != "Windows":
-    pytest.skip(
-        reason="works for some reasons only on Windows", allow_module_level=True
-    )
-# These test do not work on my Linux Mint system.
-# The test file fails when started as a whole session, but passes if I start
-# failing test classes individually by the PyCharm debugger.
-# The problem is the font_manager:
-# When started as single test class or in debugger mode the repo fonts are loaded as it
-# should be. Started as normal session the system fonts are loaded, which shouldn't be
-# possible - I guess there is some pytest magic happening in the background which messes
-# things up.
-# On Windows everything works fine, so the module works as expected.
-
-from ezdxf.tools.font_face import FontFace
+from ezdxf.fonts.font_face import FontFace
 from ezdxf.addons import text2path
 from ezdxf.path import Path
 from ezdxf import path, bbox
 from ezdxf.entities import Text, Hatch
 from ezdxf.layouts import VirtualLayout
 from ezdxf.enums import TextEntityAlignment
 
 # always available in common test scenarios:
 DEFAULT = "LiberationSans-Regular.ttf"
 NOTO_SANS_SC = "NotoSansSC-Regular.otf"
 
 
 def _to_paths(s, f=DEFAULT):
-    return text2path.make_paths_from_str(s, font=FontFace(ttf=f))
+    return text2path.make_paths_from_str(s, font=FontFace(filename=f))
 
 
 # Font 'Arial' required, a replacement fonts may return a different
 # path/hole configuration! issue #515
 CHAR_TO_PATH = [
     ["1", 1],
     ["2", 1],
```

## Comparing `ezdxf-1.1.0b0/tests/test_08_addons/test_815_dxf_browser.py` & `ezdxf-1.1.0b1/tests/test_08_addons/test_815_dxf_browser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_08_addons/test_816_bin_packing.py` & `ezdxf-1.1.0b1/tests/test_08_addons/test_816_bin_packing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_08_addons/test_817_genetic_algorithm.py` & `ezdxf-1.1.0b1/tests/test_08_addons/test_817_genetic_algorithm.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_08_addons/test_818_meshex.py` & `ezdxf-1.1.0b1/tests/test_08_addons/test_818_meshex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_08_addons/test_819_menger_sponge.py` & `ezdxf-1.1.0b1/tests/test_08_addons/test_819_menger_sponge.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_08_addons/test_820_openscad.py` & `ezdxf-1.1.0b1/tests/test_08_addons/test_820_openscad.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_08_addons/test_821_hpgl2.py` & `ezdxf-1.1.0b1/tests/test_08_addons/test_821_hpgl2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py` & `ezdxf-1.1.0b1/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_08_addons/test_822_clipper.py` & `ezdxf-1.1.0b1/tests/test_08_addons/test_822_clipper.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_09_cython_acceleration/test_901_acc_vec2.py` & `ezdxf-1.1.0b1/tests/test_09_cython_acceleration/test_901_acc_vec2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_09_cython_acceleration/test_902_acc_vec3.py` & `ezdxf-1.1.0b1/tests/test_09_cython_acceleration/test_902_acc_vec3.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_09_cython_acceleration/test_903_acc_matrix44.py` & `ezdxf-1.1.0b1/tests/test_09_cython_acceleration/test_903_acc_matrix44.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-#  Copyright (c) 2020, Manfred Moitzi
+#  Copyright (c) 2020-2023, Manfred Moitzi
 #  License: MIT License
 # Test only basic features of Cython implementation,
 # Full testing and compatibility check with Python implementation
 # is located in test suite 605.
-
 import pytest
+import numpy as np
 
 matrix44 = pytest.importorskip("ezdxf.acc.matrix44")
-Matrix44 = matrix44.Matrix44
+Matrix44: matrix44.Matrix44 = matrix44.Matrix44
 
 
 def test_default_constructor():
     m = Matrix44()
     assert m[0, 0] == 1.0
     assert m[1, 1] == 1.0
     assert m[2, 2] == 1.0
@@ -70,9 +70,21 @@
 
 def test_get_origin():
     m = Matrix44()
     m.set_row(3, (7, 8, 9))
     assert m.origin == (7, 8, 9)
 
 
+def test_array_inplace_transformation():
+    from ezdxf.math import Vec2
+
+    m = matrix44.Matrix44.translate(1, 2, 0)
+    points = [(0, 0), (1, 1), (2, 2)]
+    control = m.fast_2d_transform(points)
+
+    array = np.array(points, dtype=np.float64)
+    m.transform_array_inplace(array, 2)
+    assert all(Vec2(c).isclose(r) for c, r in zip(control, array))
+
+
 if __name__ == "__main__":
     pytest.main([__file__])
```

## Comparing `ezdxf-1.1.0b0/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py` & `ezdxf-1.1.0b1/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py` & `ezdxf-1.1.0b1/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_09_cython_acceleration/test_906_acc_bspline.py` & `ezdxf-1.1.0b1/tests/test_09_cython_acceleration/test_906_acc_bspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_10_issues/test_issue_414_bbox_calculation.py` & `ezdxf-1.1.0b1/tests/test_10_issues/test_issue_414_bbox_calculation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py` & `ezdxf-1.1.0b1/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_10_issues/test_issue_574_flattening_error.py` & `ezdxf-1.1.0b1/tests/test_10_issues/test_issue_574_flattening_error.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py` & `ezdxf-1.1.0b1/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b0/tests/test_10_issues/test_issue_749_text_layout.py` & `ezdxf-1.1.0b1/tests/test_10_issues/test_issue_749_text_layout.py`

 * *Files identical despite different names*

