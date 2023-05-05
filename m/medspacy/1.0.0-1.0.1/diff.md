# Comparing `tmp/medspacy-1.0.0.tar.gz` & `tmp/medspacy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medspacy-1.0.0.tar", last modified: Mon Oct 17 23:23:36 2022, max compression
+gzip compressed data, was "medspacy-1.0.1.tar", last modified: Mon Nov 28 20:19:52 2022, max compression
```

## Comparing `medspacy-1.0.0.tar` & `medspacy-1.0.1.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxrwxrwx   0        0        0        0 2022-10-17 23:23:36.940515 medspacy-1.0.0/
--rw-rw-rw-   0        0        0     1086 2022-10-17 23:12:39.000000 medspacy-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     7102 2022-10-17 23:23:36.940016 medspacy-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     6916 2022-10-17 23:12:39.000000 medspacy-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2022-10-17 23:23:36.612789 medspacy-1.0.0/medspacy/
--rw-rw-rw-   0        0        0      225 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/__init__.py
--rw-rw-rw-   0        0        0     9786 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/_extensions.py
--rw-rw-rw-   0        0        0       23 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/_version.py
-drwxrwxrwx   0        0        0        0 2022-10-17 23:23:36.884521 medspacy-1.0.0/medspacy/common/
--rw-rw-rw-   0        0        0       33 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/common/__init__.py
--rw-rw-rw-   0        0        0     2130 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/common/base_rule.py
--rw-rw-rw-   0        0        0     6003 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/common/medspacy_matcher.py
--rw-rw-rw-   0        0        0     6845 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/common/regex_matcher.py
--rw-rw-rw-   0        0        0     6335 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/common/util.py
--rw-rw-rw-   0        0        0      518 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/components.py
-drwxrwxrwx   0        0        0        0 2022-10-17 23:23:36.893516 medspacy-1.0.0/medspacy/context/
--rw-rw-rw-   0        0        0      354 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/context/__init__.py
--rw-rw-rw-   0        0        0    13692 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/context/context.py
--rw-rw-rw-   0        0        0     4572 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/context/context_graph.py
--rw-rw-rw-   0        0        0    15439 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/context/context_modifier.py
--rw-rw-rw-   0        0        0    11079 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/context/context_rule.py
--rw-rw-rw-   0        0        0      687 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/context/util.py
--rw-rw-rw-   0        0        0     1934 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/custom_tokenizer.py
-drwxrwxrwx   0        0        0        0 2022-10-17 23:23:36.907016 medspacy-1.0.0/medspacy/io/
--rw-rw-rw-   0        0        0      250 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/io/__init__.py
--rw-rw-rw-   0        0        0     5027 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/io/config_example.py
--rw-rw-rw-   0        0        0      133 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/io/db.py
--rw-rw-rw-   0        0        0     3415 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/io/db_connect.py
--rw-rw-rw-   0        0        0      910 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/io/db_reader.py
--rw-rw-rw-   0        0        0     5737 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/io/db_writer.py
--rw-rw-rw-   0        0        0    11707 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/io/doc_consumer.py
--rw-rw-rw-   0        0        0     2847 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/io/pipeline.py
--rw-rw-rw-   0        0        0       98 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/ner.py
-drwxrwxrwx   0        0        0        0 2022-10-17 23:23:36.914517 medspacy-1.0.0/medspacy/postprocess/
--rw-rw-rw-   0        0        0      298 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/postprocess/__init__.py
--rw-rw-rw-   0        0        0     8954 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/postprocess/postprocessing_functions.py
--rw-rw-rw-   0        0        0     1529 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/postprocess/postprocessing_pattern.py
--rw-rw-rw-   0        0        0     3450 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/postprocess/postprocessing_rule.py
--rw-rw-rw-   0        0        0     4313 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/postprocess/postprocessor.py
-drwxrwxrwx   0        0        0        0 2022-10-17 23:23:36.919017 medspacy-1.0.0/medspacy/preprocess/
--rw-rw-rw-   0        0        0      142 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/preprocess/__init__.py
--rw-rw-rw-   0        0        0     4507 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/preprocess/preprocessing_rule.py
--rw-rw-rw-   0        0        0     1840 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/preprocess/preprocessor.py
-drwxrwxrwx   0        0        0        0 2022-10-17 23:23:36.926016 medspacy-1.0.0/medspacy/section_detection/
--rw-rw-rw-   0        0        0      192 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/section_detection/__init__.py
--rw-rw-rw-   0        0        0     5399 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/section_detection/section.py
--rw-rw-rw-   0        0        0     6085 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/section_detection/section_rule.py
--rw-rw-rw-   0        0        0    22288 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/section_detection/sectionizer.py
--rw-rw-rw-   0        0        0     1627 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/section_detection/util.py
--rw-rw-rw-   0        0        0      765 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/sentence_splitting.py
-drwxrwxrwx   0        0        0        0 2022-10-17 23:23:36.933016 medspacy-1.0.0/medspacy/target_matcher/
--rw-rw-rw-   0        0        0      123 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/target_matcher/__init__.py
--rw-rw-rw-   0        0        0     2873 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/target_matcher/concept_tagger.py
--rw-rw-rw-   0        0        0     7355 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/target_matcher/target_matcher.py
--rw-rw-rw-   0        0        0     5196 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/target_matcher/target_rule.py
--rw-rw-rw-   0        0        0     8771 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/util.py
--rw-rw-rw-   0        0        0    11337 2022-10-17 23:12:39.000000 medspacy-1.0.0/medspacy/visualization.py
-drwxrwxrwx   0        0        0        0 2022-10-17 23:23:36.627789 medspacy-1.0.0/medspacy.egg-info/
--rw-rw-rw-   0        0        0     7102 2022-10-17 23:23:36.000000 medspacy-1.0.0/medspacy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     9130 2022-10-17 23:23:36.000000 medspacy-1.0.0/medspacy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-17 23:23:36.000000 medspacy-1.0.0/medspacy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2022-10-17 23:23:36.000000 medspacy-1.0.0/medspacy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2022-10-17 23:23:36.000000 medspacy-1.0.0/medspacy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-10-17 23:23:36.633289 medspacy-1.0.0/resources/
--rw-rw-rw-   0        0        0    29201 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/context_rules.json
-drwxrwxrwx   0        0        0        0 2022-10-17 23:23:36.589789 medspacy-1.0.0/resources/quickumls/
-drwxrwxrwx   0        0        0        0 2022-10-17 23:23:36.658288 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/
--rw-rw-rw-   0        0        0      183 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/README.md
-drwxrwxrwx   0        0        0        0 2022-10-17 23:23:36.661290 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/
--rw-rw-rw-   0        0        0    12288 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/cui.unqlite
--rw-rw-rw-   0        0        0    12288 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/semtypes.unqlite
--rw-rw-rw-   0        0        0        7 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/database_backend.flag
--rw-rw-rw-   0        0        0        3 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/language.flag
--rw-rw-rw-   0        0        0        0 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/lowercase.flag
--rw-rw-rw-   0        0        0        0 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/normalize-unicode.flag
-drwxrwxrwx   0        0        0        0 2022-10-17 23:23:36.795253 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/
--rw-rw-rw-   0        0        0     6116 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring
--rw-rw-rw-   0        0        0     6892 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb
--rw-rw-rw-   0        0        0     2788 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb
--rw-rw-rw-   0        0        0     2664 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb
--rw-rw-rw-   0        0        0     2744 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb
--rw-rw-rw-   0        0        0     3016 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb
--rw-rw-rw-   0        0        0     2904 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb
--rw-rw-rw-   0        0        0     3140 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb
--rw-rw-rw-   0        0        0     3228 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb
--rw-rw-rw-   0        0        0     3460 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb
--rw-rw-rw-   0        0        0     3148 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb
--rw-rw-rw-   0        0        0     7344 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb
--rw-rw-rw-   0        0        0     3224 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb
--rw-rw-rw-   0        0        0     4984 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb
--rw-rw-rw-   0        0        0     5152 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb
--rw-rw-rw-   0        0        0     5024 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb
--rw-rw-rw-   0        0        0     3384 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb
--rw-rw-rw-   0        0        0     3824 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb
--rw-rw-rw-   0        0        0     3544 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb
--rw-rw-rw-   0        0        0     4064 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb
--rw-rw-rw-   0        0        0     3624 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb
--rw-rw-rw-   0        0        0     5160 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb
--rw-rw-rw-   0        0        0     3788 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb
--rw-rw-rw-   0        0        0     5368 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb
--rw-rw-rw-   0        0        0     2384 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb
-drwxrwxrwx   0        0        0        0 2022-10-17 23:23:36.829163 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/
--rw-rw-rw-   0        0        0      183 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/README.md
-drwxrwxrwx   0        0        0        0 2022-10-17 23:23:36.832163 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/
--rw-rw-rw-   0        0        0    20480 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/cui.unqlite
--rw-rw-rw-   0        0        0    12288 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/semtypes.unqlite
--rw-rw-rw-   0        0        0        7 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/database_backend.flag
--rw-rw-rw-   0        0        0        3 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/language.flag
--rw-rw-rw-   0        0        0        0 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/lowercase.flag
--rw-rw-rw-   0        0        0        0 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/normalize-unicode.flag
-drwxrwxrwx   0        0        0        0 2022-10-17 23:23:36.877016 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/
--rw-rw-rw-   0        0        0     2912 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring
--rw-rw-rw-   0        0        0     6162 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb
--rw-rw-rw-   0        0        0     2540 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb
--rw-rw-rw-   0        0        0     2574 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb
--rw-rw-rw-   0        0        0     2642 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb
--rw-rw-rw-   0        0        0     2884 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb
--rw-rw-rw-   0        0        0     2778 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb
--rw-rw-rw-   0        0        0     2990 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb
--rw-rw-rw-   0        0        0     3066 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb
--rw-rw-rw-   0        0        0     3262 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb
--rw-rw-rw-   0        0        0     2984 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb
--rw-rw-rw-   0        0        0     5574 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb
--rw-rw-rw-   0        0        0     3050 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb
--rw-rw-rw-   0        0        0     4526 2022-10-17 23:12:39.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb
--rw-rw-rw-   0        0        0     3546 2022-10-17 23:12:40.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb
--rw-rw-rw-   0        0        0     4616 2022-10-17 23:12:40.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb
--rw-rw-rw-   0        0        0     3186 2022-10-17 23:12:40.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb
--rw-rw-rw-   0        0        0     3576 2022-10-17 23:12:40.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb
--rw-rw-rw-   0        0        0     3322 2022-10-17 23:12:40.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb
--rw-rw-rw-   0        0        0     3780 2022-10-17 23:12:40.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb
--rw-rw-rw-   0        0        0     3390 2022-10-17 23:12:40.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb
--rw-rw-rw-   0        0        0     4696 2022-10-17 23:12:40.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb
--rw-rw-rw-   0        0        0     3528 2022-10-17 23:12:40.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb
--rw-rw-rw-   0        0        0     4828 2022-10-17 23:12:40.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb
--rw-rw-rw-   0        0        0     2336 2022-10-17 23:12:40.000000 medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb
--rw-rw-rw-   0        0        0    24403 2022-10-17 23:12:40.000000 medspacy-1.0.0/resources/rush_rules.tsv
--rw-rw-rw-   0        0        0    12637 2022-10-17 23:12:40.000000 medspacy-1.0.0/resources/section_patterns.json
--rw-rw-rw-   0        0        0       42 2022-10-17 23:23:36.941017 medspacy-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     2497 2022-10-17 23:22:41.000000 medspacy-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-10-17 23:23:36.938516 medspacy-1.0.0/tests/
--rw-rw-rw-   0        0        0        0 2022-10-17 23:12:40.000000 medspacy-1.0.0/tests/__init__.py
--rw-rw-rw-   0        0        0     3078 2022-10-17 23:12:40.000000 medspacy-1.0.0/tests/test_extensions.py
--rw-rw-rw-   0        0        0     7542 2022-10-17 23:12:40.000000 medspacy-1.0.0/tests/test_medspacy.py
--rw-rw-rw-   0        0        0     3678 2022-10-17 23:12:40.000000 medspacy-1.0.0/tests/test_notebooks.py
+drwxrwxrwx   0        0        0        0 2022-11-28 20:19:52.609281 medspacy-1.0.1/
+-rw-rw-rw-   0        0        0     1086 2022-10-17 23:12:39.000000 medspacy-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     7128 2022-11-28 20:19:52.608280 medspacy-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6916 2022-10-17 23:12:39.000000 medspacy-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2022-11-28 20:19:51.460780 medspacy-1.0.1/medspacy/
+-rw-rw-rw-   0        0        0      225 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/__init__.py
+-rw-rw-rw-   0        0        0     9786 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/_extensions.py
+-rw-rw-rw-   0        0        0       23 2022-11-28 20:17:59.000000 medspacy-1.0.1/medspacy/_version.py
+drwxrwxrwx   0        0        0        0 2022-11-28 20:19:52.219281 medspacy-1.0.1/medspacy/common/
+-rw-rw-rw-   0        0        0       33 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/common/__init__.py
+-rw-rw-rw-   0        0        0     2130 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/common/base_rule.py
+-rw-rw-rw-   0        0        0     6003 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/common/medspacy_matcher.py
+-rw-rw-rw-   0        0        0     6845 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/common/regex_matcher.py
+-rw-rw-rw-   0        0        0     6335 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/common/util.py
+-rw-rw-rw-   0        0        0      518 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/components.py
+drwxrwxrwx   0        0        0        0 2022-11-28 20:19:52.288280 medspacy-1.0.1/medspacy/context/
+-rw-rw-rw-   0        0        0      354 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/context/__init__.py
+-rw-rw-rw-   0        0        0    13692 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/context/context.py
+-rw-rw-rw-   0        0        0     4572 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/context/context_graph.py
+-rw-rw-rw-   0        0        0    15439 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/context/context_modifier.py
+-rw-rw-rw-   0        0        0    11079 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/context/context_rule.py
+-rw-rw-rw-   0        0        0      687 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/context/util.py
+-rw-rw-rw-   0        0        0     1934 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/custom_tokenizer.py
+drwxrwxrwx   0        0        0        0 2022-11-28 20:19:52.386281 medspacy-1.0.1/medspacy/io/
+-rw-rw-rw-   0        0        0      250 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/io/__init__.py
+-rw-rw-rw-   0        0        0     5027 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/io/config_example.py
+-rw-rw-rw-   0        0        0      133 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/io/db.py
+-rw-rw-rw-   0        0        0     3415 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/io/db_connect.py
+-rw-rw-rw-   0        0        0      910 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/io/db_reader.py
+-rw-rw-rw-   0        0        0     5737 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/io/db_writer.py
+-rw-rw-rw-   0        0        0    11707 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/io/doc_consumer.py
+-rw-rw-rw-   0        0        0     2847 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/io/pipeline.py
+-rw-rw-rw-   0        0        0       98 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/ner.py
+drwxrwxrwx   0        0        0        0 2022-11-28 20:19:52.447780 medspacy-1.0.1/medspacy/postprocess/
+-rw-rw-rw-   0        0        0      298 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/postprocess/__init__.py
+-rw-rw-rw-   0        0        0     8954 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/postprocess/postprocessing_functions.py
+-rw-rw-rw-   0        0        0     1529 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/postprocess/postprocessing_pattern.py
+-rw-rw-rw-   0        0        0     3450 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/postprocess/postprocessing_rule.py
+-rw-rw-rw-   0        0        0     4313 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/postprocess/postprocessor.py
+drwxrwxrwx   0        0        0        0 2022-11-28 20:19:52.478281 medspacy-1.0.1/medspacy/preprocess/
+-rw-rw-rw-   0        0        0      142 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/preprocess/__init__.py
+-rw-rw-rw-   0        0        0     4507 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/preprocess/preprocessing_rule.py
+-rw-rw-rw-   0        0        0     1840 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/preprocess/preprocessor.py
+drwxrwxrwx   0        0        0        0 2022-11-28 20:19:52.530780 medspacy-1.0.1/medspacy/section_detection/
+-rw-rw-rw-   0        0        0      192 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/section_detection/__init__.py
+-rw-rw-rw-   0        0        0     5399 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/section_detection/section.py
+-rw-rw-rw-   0        0        0     6085 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/section_detection/section_rule.py
+-rw-rw-rw-   0        0        0    22288 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/section_detection/sectionizer.py
+-rw-rw-rw-   0        0        0     1627 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/section_detection/util.py
+-rw-rw-rw-   0        0        0      765 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/sentence_splitting.py
+drwxrwxrwx   0        0        0        0 2022-11-28 20:19:52.569781 medspacy-1.0.1/medspacy/target_matcher/
+-rw-rw-rw-   0        0        0      123 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/target_matcher/__init__.py
+-rw-rw-rw-   0        0        0     2873 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/target_matcher/concept_tagger.py
+-rw-rw-rw-   0        0        0     7355 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/target_matcher/target_matcher.py
+-rw-rw-rw-   0        0        0     5196 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/target_matcher/target_rule.py
+-rw-rw-rw-   0        0        0     8771 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/util.py
+-rw-rw-rw-   0        0        0    11337 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/visualization.py
+drwxrwxrwx   0        0        0        0 2022-11-28 20:19:51.531280 medspacy-1.0.1/medspacy.egg-info/
+-rw-rw-rw-   0        0        0     7128 2022-11-28 20:19:51.000000 medspacy-1.0.1/medspacy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     9130 2022-11-28 20:19:51.000000 medspacy-1.0.1/medspacy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-11-28 20:19:51.000000 medspacy-1.0.1/medspacy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2022-11-28 20:19:51.000000 medspacy-1.0.1/medspacy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2022-11-28 20:19:51.000000 medspacy-1.0.1/medspacy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-11-28 20:19:51.564783 medspacy-1.0.1/resources/
+-rw-rw-rw-   0        0        0    29201 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/context_rules.json
+drwxrwxrwx   0        0        0        0 2022-11-28 20:19:51.351781 medspacy-1.0.1/resources/quickumls/
+drwxrwxrwx   0        0        0        0 2022-11-28 20:19:51.601782 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/
+-rw-rw-rw-   0        0        0      183 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/README.md
+drwxrwxrwx   0        0        0        0 2022-11-28 20:19:51.619279 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/
+-rw-rw-rw-   0        0        0    12288 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/cui.unqlite
+-rw-rw-rw-   0        0        0    12288 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/semtypes.unqlite
+-rw-rw-rw-   0        0        0        7 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/database_backend.flag
+-rw-rw-rw-   0        0        0        3 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/language.flag
+-rw-rw-rw-   0        0        0        0 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/lowercase.flag
+-rw-rw-rw-   0        0        0        0 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/normalize-unicode.flag
+drwxrwxrwx   0        0        0        0 2022-11-28 20:19:51.835780 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/
+-rw-rw-rw-   0        0        0     6116 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring
+-rw-rw-rw-   0        0        0     6892 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb
+-rw-rw-rw-   0        0        0     2788 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb
+-rw-rw-rw-   0        0        0     2664 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb
+-rw-rw-rw-   0        0        0     2744 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb
+-rw-rw-rw-   0        0        0     3016 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb
+-rw-rw-rw-   0        0        0     2904 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb
+-rw-rw-rw-   0        0        0     3140 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb
+-rw-rw-rw-   0        0        0     3228 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb
+-rw-rw-rw-   0        0        0     3460 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb
+-rw-rw-rw-   0        0        0     3148 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb
+-rw-rw-rw-   0        0        0     7344 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb
+-rw-rw-rw-   0        0        0     3224 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb
+-rw-rw-rw-   0        0        0     4984 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb
+-rw-rw-rw-   0        0        0     5152 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb
+-rw-rw-rw-   0        0        0     5024 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb
+-rw-rw-rw-   0        0        0     3384 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb
+-rw-rw-rw-   0        0        0     3824 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb
+-rw-rw-rw-   0        0        0     3544 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb
+-rw-rw-rw-   0        0        0     4064 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb
+-rw-rw-rw-   0        0        0     3624 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb
+-rw-rw-rw-   0        0        0     5160 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb
+-rw-rw-rw-   0        0        0     3788 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb
+-rw-rw-rw-   0        0        0     5368 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb
+-rw-rw-rw-   0        0        0     2384 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb
+drwxrwxrwx   0        0        0        0 2022-11-28 20:19:51.863781 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/
+-rw-rw-rw-   0        0        0      183 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/README.md
+drwxrwxrwx   0        0        0        0 2022-11-28 20:19:51.881781 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/
+-rw-rw-rw-   0        0        0    20480 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/cui.unqlite
+-rw-rw-rw-   0        0        0    12288 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/semtypes.unqlite
+-rw-rw-rw-   0        0        0        7 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/database_backend.flag
+-rw-rw-rw-   0        0        0        3 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/language.flag
+-rw-rw-rw-   0        0        0        0 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/lowercase.flag
+-rw-rw-rw-   0        0        0        0 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/normalize-unicode.flag
+drwxrwxrwx   0        0        0        0 2022-11-28 20:19:52.164781 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/
+-rw-rw-rw-   0        0        0     2912 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring
+-rw-rw-rw-   0        0        0     6162 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb
+-rw-rw-rw-   0        0        0     2540 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb
+-rw-rw-rw-   0        0        0     2574 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb
+-rw-rw-rw-   0        0        0     2642 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb
+-rw-rw-rw-   0        0        0     2884 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb
+-rw-rw-rw-   0        0        0     2778 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb
+-rw-rw-rw-   0        0        0     2990 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb
+-rw-rw-rw-   0        0        0     3066 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb
+-rw-rw-rw-   0        0        0     3262 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb
+-rw-rw-rw-   0        0        0     2984 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb
+-rw-rw-rw-   0        0        0     5574 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb
+-rw-rw-rw-   0        0        0     3050 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb
+-rw-rw-rw-   0        0        0     4526 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb
+-rw-rw-rw-   0        0        0     3546 2022-10-17 23:12:40.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb
+-rw-rw-rw-   0        0        0     4616 2022-10-17 23:12:40.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb
+-rw-rw-rw-   0        0        0     3186 2022-10-17 23:12:40.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb
+-rw-rw-rw-   0        0        0     3576 2022-10-17 23:12:40.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb
+-rw-rw-rw-   0        0        0     3322 2022-10-17 23:12:40.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb
+-rw-rw-rw-   0        0        0     3780 2022-10-17 23:12:40.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb
+-rw-rw-rw-   0        0        0     3390 2022-10-17 23:12:40.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb
+-rw-rw-rw-   0        0        0     4696 2022-10-17 23:12:40.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb
+-rw-rw-rw-   0        0        0     3528 2022-10-17 23:12:40.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb
+-rw-rw-rw-   0        0        0     4828 2022-10-17 23:12:40.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb
+-rw-rw-rw-   0        0        0     2336 2022-10-17 23:12:40.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb
+-rw-rw-rw-   0        0        0    24473 2022-11-28 20:06:06.000000 medspacy-1.0.1/resources/rush_rules.tsv
+-rw-rw-rw-   0        0        0    12637 2022-10-17 23:12:40.000000 medspacy-1.0.1/resources/section_patterns.json
+-rw-rw-rw-   0        0        0       42 2022-11-28 20:19:52.609781 medspacy-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     2529 2022-11-28 20:17:36.000000 medspacy-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2022-11-28 20:19:52.605780 medspacy-1.0.1/tests/
+-rw-rw-rw-   0        0        0        0 2022-10-17 23:12:40.000000 medspacy-1.0.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     3078 2022-10-17 23:12:40.000000 medspacy-1.0.1/tests/test_extensions.py
+-rw-rw-rw-   0        0        0     7542 2022-10-17 23:12:40.000000 medspacy-1.0.1/tests/test_medspacy.py
+-rw-rw-rw-   0        0        0     3678 2022-10-17 23:12:40.000000 medspacy-1.0.1/tests/test_notebooks.py
```

### Comparing `medspacy-1.0.0/LICENSE` & `medspacy-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/PKG-INFO` & `medspacy-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: medspacy
-Version: 1.0.0
+Version: 1.0.1
 Summary: Library for clinical NLP with spaCy.
 Author: medSpaCy
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 ![Build Status](https://github.com/medspacy/medspacy/workflows/medspacy/badge.svg)
 
 # medspacy
```

### Comparing `medspacy-1.0.0/README.md` & `medspacy-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/medspacy/_extensions.py` & `medspacy-1.0.1/medspacy/_extensions.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/medspacy/common/base_rule.py` & `medspacy-1.0.1/medspacy/common/base_rule.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/medspacy/common/medspacy_matcher.py` & `medspacy-1.0.1/medspacy/common/medspacy_matcher.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/medspacy/common/regex_matcher.py` & `medspacy-1.0.1/medspacy/common/regex_matcher.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/medspacy/common/util.py` & `medspacy-1.0.1/medspacy/common/util.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/medspacy/components.py` & `medspacy-1.0.1/medspacy/components.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/medspacy/context/context.py` & `medspacy-1.0.1/medspacy/context/context.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/medspacy/context/context_graph.py` & `medspacy-1.0.1/medspacy/context/context_graph.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/medspacy/context/context_modifier.py` & `medspacy-1.0.1/medspacy/context/context_modifier.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/medspacy/context/context_rule.py` & `medspacy-1.0.1/medspacy/context/context_rule.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/medspacy/context/util.py` & `medspacy-1.0.1/medspacy/context/util.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/medspacy/custom_tokenizer.py` & `medspacy-1.0.1/medspacy/custom_tokenizer.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/medspacy/io/config_example.py` & `medspacy-1.0.1/medspacy/io/config_example.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/medspacy/io/db_connect.py` & `medspacy-1.0.1/medspacy/io/db_connect.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/medspacy/io/db_reader.py` & `medspacy-1.0.1/medspacy/io/db_reader.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/medspacy/io/db_writer.py` & `medspacy-1.0.1/medspacy/io/db_writer.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/medspacy/io/doc_consumer.py` & `medspacy-1.0.1/medspacy/io/doc_consumer.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/medspacy/io/pipeline.py` & `medspacy-1.0.1/medspacy/io/pipeline.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/medspacy/postprocess/postprocessing_functions.py` & `medspacy-1.0.1/medspacy/postprocess/postprocessing_functions.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/medspacy/postprocess/postprocessing_pattern.py` & `medspacy-1.0.1/medspacy/postprocess/postprocessing_pattern.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/medspacy/postprocess/postprocessing_rule.py` & `medspacy-1.0.1/medspacy/postprocess/postprocessing_rule.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/medspacy/postprocess/postprocessor.py` & `medspacy-1.0.1/medspacy/postprocess/postprocessor.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/medspacy/preprocess/preprocessing_rule.py` & `medspacy-1.0.1/medspacy/preprocess/preprocessing_rule.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/medspacy/preprocess/preprocessor.py` & `medspacy-1.0.1/medspacy/preprocess/preprocessor.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/medspacy/section_detection/section.py` & `medspacy-1.0.1/medspacy/section_detection/section.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/medspacy/section_detection/section_rule.py` & `medspacy-1.0.1/medspacy/section_detection/section_rule.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/medspacy/section_detection/sectionizer.py` & `medspacy-1.0.1/medspacy/section_detection/sectionizer.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/medspacy/section_detection/util.py` & `medspacy-1.0.1/medspacy/section_detection/util.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/medspacy/sentence_splitting.py` & `medspacy-1.0.1/medspacy/sentence_splitting.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/medspacy/target_matcher/concept_tagger.py` & `medspacy-1.0.1/medspacy/target_matcher/concept_tagger.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/medspacy/target_matcher/target_matcher.py` & `medspacy-1.0.1/medspacy/target_matcher/target_matcher.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/medspacy/target_matcher/target_rule.py` & `medspacy-1.0.1/medspacy/target_matcher/target_rule.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/medspacy/util.py` & `medspacy-1.0.1/medspacy/util.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/medspacy/visualization.py` & `medspacy-1.0.1/medspacy/visualization.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/medspacy.egg-info/PKG-INFO` & `medspacy-1.0.1/medspacy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: medspacy
-Version: 1.0.0
+Version: 1.0.1
 Summary: Library for clinical NLP with spaCy.
 Author: medSpaCy
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 ![Build Status](https://github.com/medspacy/medspacy/workflows/medspacy/badge.svg)
 
 # medspacy
```

### Comparing `medspacy-1.0.0/medspacy.egg-info/SOURCES.txt` & `medspacy-1.0.1/medspacy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/context_rules.json` & `medspacy-1.0.1/resources/context_rules.json`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/cui.unqlite` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/cui.unqlite`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/semtypes.unqlite` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/semtypes.unqlite`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/cui.unqlite` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/cui.unqlite`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/semtypes.unqlite` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/semtypes.unqlite`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb` & `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/resources/rush_rules.tsv` & `medspacy-1.0.1/resources/rush_rules.tsv`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 #this list is optimized for shorter rule length rules for semeval were added
 @MaxRepeatLength	100
 @Version	1.0.3.4
 
 #stbegin is the marker for sentence begin, the span of sentence will start at the begin of the captured group
 #stbegin has two scores 0, 1: 0 for true sentence begin clues, 1 for false sentence begin clues which will overwrite 0-scored rules when they are overlapping.
-#stend is the marker for sentence begin, the span of sentence will end at the end of the captured group
+#stend is the marker for sentence end, the span of sentence will end at the end of the captured group
 #stend also has two scores 2, 3: 2 for true sentence end clues, 3 for false sentence end clues which will overwrite 2-scored rules when they are overlapping
 
 # \b the begin of an input
 # \e the end of an input
 # \d A digit
 # \C A capital letter
 # \c A lowercase letter
@@ -38,15 +38,18 @@
 # \p A punctuation
 #
 # \+ An addition symbol (to distinguish the "+" after a wildcard)
 # \( A left parentheses symbol
 # \) A right parentheses symbol
 #
 #  A wildcard followed by a "+": 1 or more characters that match the wildcard
-
+\b(\C	0	stbegin
+\b(\d	0	stbegin
+\b\s+(\C	0	stbegin
+\b\s+(\d	0	stbegin
 \c.\s+(\C)	0	stbegin
  mL.\s+(\C)	0	stbegin
 *)	1	stbegin
 \c\c.\s+(\C)	0	stbegin
 \c\).\s+(\C)	0	stbegin
 \d\).\s+(\C)	0	stbegin
 \C\C\C.\s+(\C)\c	0	stbegin
```

### Comparing `medspacy-1.0.0/resources/section_patterns.json` & `medspacy-1.0.1/resources/section_patterns.json`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/setup.py` & `medspacy-1.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     print(
         "Not installing QuickUMLS for Windows since it currently requires conda (as opposed to just pip)"
     )
 else:
     # Using a trick from StackOverflow to set an impossibly high version number
     # to force getting latest from GitHub as opposed to PyPi
     # since QuickUMLS has not made a release with some recent MedSpacy contributions...
-    quickumls_package = "medspacy_quickumls==2.6"
+    quickumls_package = "medspacy_quickumls==2.7"
     additional_installs.append(quickumls_package)
     print("Attempting to install quickumls package: {}".format(quickumls_package))
 
 # function to recursively get files for resourcee
 def package_files(directory):
     paths = []
     for (p, directories, filenames) in os.walk(directory):
@@ -59,16 +59,17 @@
     name="medspacy",
     version=get_version(),
     description="Library for clinical NLP with spaCy.",
     author="medSpaCy",
     packages=find_packages(),
     install_requires=[
         "spacy>=3.4.1",
-        "PyRuSH>=1.0.6",
+        "PyRuSH>=1.0.8",
         "pysbd==0.3.4",
         "jsonschema",
     ]
     + additional_installs,
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_data={"medspacy": resource_files},
+    python_requires=">=3.8.0",
 )
```

### Comparing `medspacy-1.0.0/tests/test_extensions.py` & `medspacy-1.0.1/tests/test_extensions.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/tests/test_medspacy.py` & `medspacy-1.0.1/tests/test_medspacy.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.0/tests/test_notebooks.py` & `medspacy-1.0.1/tests/test_notebooks.py`

 * *Files identical despite different names*

