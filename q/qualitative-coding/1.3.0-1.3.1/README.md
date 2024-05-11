# Comparing `tmp/qualitative_coding-1.3.0.tar.gz` & `tmp/qualitative_coding-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qualitative_coding-1.3.0.tar", max compression
+gzip compressed data, was "qualitative_coding-1.3.1.tar", max compression
```

## Comparing `qualitative_coding-1.3.0.tar` & `qualitative_coding-1.3.1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0      781 2021-07-13 19:40:03.158793 qualitative_coding-1.3.0/LICENSE
--rw-r--r--   0        0        0    13681 2024-04-22 23:05:52.179536 qualitative_coding-1.3.0/README.md
--rw-r--r--   0        0        0      717 2024-04-27 14:34:39.045306 qualitative_coding-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     1010 2024-04-22 23:05:52.183290 qualitative_coding-1.3.0/qualitative_coding/cli/__init__.py
--rw-r--r--   0        0        0      498 2024-04-22 23:05:52.185526 qualitative_coding-1.3.0/qualitative_coding/cli/check.py
--rw-r--r--   0        0        0     3278 2024-02-11 22:24:40.918879 qualitative_coding-1.3.0/qualitative_coding/cli/click_aliases.py
--rw-r--r--   0        0        0     2182 2024-04-22 23:05:52.186779 qualitative_coding-1.3.0/qualitative_coding/cli/code.py
--rw-r--r--   0        0        0      481 2024-04-22 23:05:52.187514 qualitative_coding-1.3.0/qualitative_coding/cli/codebook.py
--rw-r--r--   0        0        0      664 2024-04-22 23:05:52.188160 qualitative_coding-1.3.0/qualitative_coding/cli/coders.py
--rw-r--r--   0        0        0      649 2024-04-22 23:05:52.188529 qualitative_coding-1.3.0/qualitative_coding/cli/codes/__init__.py
--rw-r--r--   0        0        0     3733 2024-04-22 23:05:52.189249 qualitative_coding-1.3.0/qualitative_coding/cli/codes/crosstab.py
--rw-r--r--   0        0        0     2533 2024-04-22 23:05:52.190015 qualitative_coding-1.3.0/qualitative_coding/cli/codes/find.py
--rw-r--r--   0        0        0      668 2024-04-22 23:05:52.191009 qualitative_coding-1.3.0/qualitative_coding/cli/codes/list.py
--rw-r--r--   0        0        0     1010 2024-04-22 23:05:52.191500 qualitative_coding-1.3.0/qualitative_coding/cli/codes/rename.py
--rw-r--r--   0        0        0     3551 2024-04-22 23:05:52.192331 qualitative_coding-1.3.0/qualitative_coding/cli/codes/stats.py
--rw-r--r--   0        0        0      611 2024-04-22 23:05:52.193027 qualitative_coding-1.3.0/qualitative_coding/cli/corpus/__init__.py
--rw-r--r--   0        0        0     1108 2024-04-22 23:05:52.193719 qualitative_coding-1.3.0/qualitative_coding/cli/corpus/import_media.py
--rw-r--r--   0        0        0      620 2024-04-22 23:05:52.194269 qualitative_coding-1.3.0/qualitative_coding/cli/corpus/list.py
--rw-r--r--   0        0        0      629 2024-04-22 23:05:52.194961 qualitative_coding-1.3.0/qualitative_coding/cli/corpus/move.py
--rw-r--r--   0        0        0      581 2024-04-22 23:05:52.196220 qualitative_coding-1.3.0/qualitative_coding/cli/corpus/remove.py
--rw-r--r--   0        0        0      611 2024-04-22 23:05:52.196563 qualitative_coding-1.3.0/qualitative_coding/cli/decorators.py
--rw-r--r--   0        0        0      748 2024-04-26 23:45:57.835343 qualitative_coding-1.3.0/qualitative_coding/cli/export.py
--rw-r--r--   0        0        0      895 2024-04-22 23:05:52.197716 qualitative_coding-1.3.0/qualitative_coding/cli/init.py
--rw-r--r--   0        0        0      836 2024-04-22 23:05:52.198230 qualitative_coding-1.3.0/qualitative_coding/cli/memo.py
--rw-r--r--   0        0        0     1575 2024-02-11 22:24:40.931614 qualitative_coding-1.3.0/qualitative_coding/cli/options.py
--rw-r--r--   0        0        0      743 2024-04-22 23:05:52.198892 qualitative_coding-1.3.0/qualitative_coding/cli/upgrade.py
--rw-r--r--   0        0        0      216 2024-02-11 22:24:40.936290 qualitative_coding-1.3.0/qualitative_coding/cli/version.py
--rw-r--r--   0        0        0       96 2021-07-13 19:40:03.159583 qualitative_coding-1.3.0/qualitative_coding/codebook.py
--rw-r--r--   0        0        0    36531 2024-04-26 22:37:51.291135 qualitative_coding-1.3.0/qualitative_coding/corpus.py
--rw-r--r--   0        0        0       50 2024-02-11 22:24:40.939611 qualitative_coding-1.3.0/qualitative_coding/database/errors.py
--rw-r--r--   0        0        0     3293 2024-04-22 23:05:52.201577 qualitative_coding-1.3.0/qualitative_coding/database/models.py
--rw-r--r--   0        0        0      865 2024-04-22 23:05:52.202334 qualitative_coding-1.3.0/qualitative_coding/editors.py
--rw-r--r--   0        0        0      210 2024-04-22 23:05:52.203924 qualitative_coding-1.3.0/qualitative_coding/exceptions.py
--rw-r--r--   0        0        0     4220 2024-04-22 23:05:52.205339 qualitative_coding-1.3.0/qualitative_coding/helpers.py
--rw-r--r--   0        0        0      895 2021-07-13 19:40:03.160344 qualitative_coding-1.3.0/qualitative_coding/logs.py
--rw-r--r--   0        0        0      288 2024-02-11 22:24:40.943568 qualitative_coding-1.3.0/qualitative_coding/media_importers/__init__.py
--rw-r--r--   0        0        0      560 2024-04-22 23:05:52.205760 qualitative_coding-1.3.0/qualitative_coding/media_importers/base.py
--rw-r--r--   0        0        0      335 2024-04-22 23:05:52.206697 qualitative_coding-1.3.0/qualitative_coding/media_importers/pandoc.py
--rw-r--r--   0        0        0      353 2024-04-22 23:05:52.207100 qualitative_coding-1.3.0/qualitative_coding/media_importers/verbatim.py
--rw-r--r--   0        0        0     1758 2024-04-22 23:05:52.207406 qualitative_coding-1.3.0/qualitative_coding/migrations/__init__.py
--rw-r--r--   0        0        0     1297 2024-04-22 23:05:52.207666 qualitative_coding-1.3.0/qualitative_coding/migrations/migration.py
--rw-r--r--   0        0        0      235 2024-04-22 23:05:52.207966 qualitative_coding-1.3.0/qualitative_coding/migrations/migration_0_2_3.py
--rw-r--r--   0        0        0     4779 2024-04-22 23:05:52.208250 qualitative_coding-1.3.0/qualitative_coding/migrations/migration_1_0_0.py
--rw-r--r--   0        0        0     7262 2024-04-27 14:32:51.866123 qualitative_coding-1.3.0/qualitative_coding/refi_qda/reader.py
--rw-r--r--   0        0        0    26395 2024-04-22 23:05:52.210734 qualitative_coding-1.3.0/qualitative_coding/refi_qda/schema.xsd
--rw-r--r--   0        0        0     6718 2024-04-27 12:29:30.699216 qualitative_coding-1.3.0/qualitative_coding/refi_qda/writer.py
--rw-r--r--   0        0        0        0 2024-04-22 23:05:52.211669 qualitative_coding-1.3.0/qualitative_coding/tests/__init__.py
--rw-r--r--   0        0        0     5376 2024-04-22 23:05:52.212557 qualitative_coding-1.3.0/qualitative_coding/tests/fixtures.py
--rwxr-xr-x   0        0        0     1764 2024-04-22 23:05:52.213687 qualitative_coding-1.3.0/qualitative_coding/tests/mock_editor.py
--rw-r--r--   0        0        0     1272 2024-04-22 23:05:52.214516 qualitative_coding-1.3.0/qualitative_coding/tests/test_check.py
--rw-r--r--   0        0        0     1435 2024-04-22 23:05:52.214800 qualitative_coding-1.3.0/qualitative_coding/tests/test_code.py
--rw-r--r--   0        0        0     1622 2024-04-22 23:05:52.215589 qualitative_coding-1.3.0/qualitative_coding/tests/test_code_parsing.py
--rw-r--r--   0        0        0      608 2024-04-22 23:05:52.215870 qualitative_coding-1.3.0/qualitative_coding/tests/test_codebook.py
--rw-r--r--   0        0        0      489 2024-04-22 23:05:52.216106 qualitative_coding-1.3.0/qualitative_coding/tests/test_coders.py
--rw-r--r--   0        0        0      889 2024-04-22 23:05:52.216404 qualitative_coding-1.3.0/qualitative_coding/tests/test_codes_crosstab.py
--rw-r--r--   0        0        0      606 2024-04-22 23:05:52.217275 qualitative_coding-1.3.0/qualitative_coding/tests/test_codes_find.py
--rw-r--r--   0        0        0     1015 2024-04-22 23:05:52.217555 qualitative_coding-1.3.0/qualitative_coding/tests/test_codes_list.py
--rw-r--r--   0        0        0      805 2024-04-22 23:05:52.217853 qualitative_coding-1.3.0/qualitative_coding/tests/test_codes_rename.py
--rw-r--r--   0        0        0     1646 2024-04-22 23:05:52.218694 qualitative_coding-1.3.0/qualitative_coding/tests/test_codes_stats.py
--rw-r--r--   0        0        0     2663 2024-04-22 23:05:52.219419 qualitative_coding-1.3.0/qualitative_coding/tests/test_corpus_import.py
--rw-r--r--   0        0        0     1501 2024-04-22 23:05:52.219879 qualitative_coding-1.3.0/qualitative_coding/tests/test_corpus_move.py
--rw-r--r--   0        0        0      655 2024-04-22 23:05:52.220668 qualitative_coding-1.3.0/qualitative_coding/tests/test_corpus_remove.py
--rw-r--r--   0        0        0      440 2024-04-22 23:05:52.221513 qualitative_coding-1.3.0/qualitative_coding/tests/test_export.py
--rw-r--r--   0        0        0     1561 2024-04-22 23:05:52.222311 qualitative_coding-1.3.0/qualitative_coding/tests/test_init.py
--rw-r--r--   0        0        0     1270 2024-04-22 23:05:52.223117 qualitative_coding-1.3.0/qualitative_coding/tests/test_init_import.py
--rw-r--r--   0        0        0      300 2024-04-22 23:05:52.223384 qualitative_coding-1.3.0/qualitative_coding/tests/test_memo.py
--rw-r--r--   0        0        0     1646 2024-04-26 23:41:13.289436 qualitative_coding-1.3.0/qualitative_coding/tests/test_refi_qda_writer.py
--rw-r--r--   0        0        0      849 2024-04-22 23:05:52.224866 qualitative_coding-1.3.0/qualitative_coding/tests/test_tree_node.py
--rw-r--r--   0        0        0      685 2024-04-22 23:05:52.225137 qualitative_coding-1.3.0/qualitative_coding/tests/test_upgrade.py
--rw-r--r--   0        0        0      313 2024-04-22 23:05:52.225832 qualitative_coding-1.3.0/qualitative_coding/tests/test_version.py
--rw-r--r--   0        0        0     6300 2024-04-22 23:05:52.226807 qualitative_coding-1.3.0/qualitative_coding/tree_node.py
--rw-r--r--   0        0        0      556 2023-12-07 20:04:17.916204 qualitative_coding-1.3.0/qualitative_coding/user_input.py
--rw-r--r--   0        0        0    12042 2024-02-11 22:24:40.952711 qualitative_coding-1.3.0/qualitative_coding/views/coding_ui.py
--rw-r--r--   0        0        0      910 2024-02-11 22:24:40.954722 qualitative_coding-1.3.0/qualitative_coding/views/styles.py
--rw-r--r--   0        0        0    31613 2024-04-26 22:41:04.840295 qualitative_coding-1.3.0/qualitative_coding/views/viewer.py
--rw-r--r--   0        0        0    14582 1970-01-01 00:00:00.000000 qualitative_coding-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      781 2021-07-13 19:40:03.158793 qualitative_coding-1.3.1/LICENSE
+-rw-r--r--   0        0        0    13681 2024-04-22 23:05:52.179536 qualitative_coding-1.3.1/README.md
+-rw-r--r--   0        0        0      717 2024-05-11 01:04:17.146573 qualitative_coding-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1010 2024-04-22 23:05:52.183290 qualitative_coding-1.3.1/qualitative_coding/cli/__init__.py
+-rw-r--r--   0        0        0      498 2024-04-22 23:05:52.185526 qualitative_coding-1.3.1/qualitative_coding/cli/check.py
+-rw-r--r--   0        0        0     3278 2024-02-11 22:24:40.918879 qualitative_coding-1.3.1/qualitative_coding/cli/click_aliases.py
+-rw-r--r--   0        0        0     2182 2024-04-22 23:05:52.186779 qualitative_coding-1.3.1/qualitative_coding/cli/code.py
+-rw-r--r--   0        0        0      481 2024-04-22 23:05:52.187514 qualitative_coding-1.3.1/qualitative_coding/cli/codebook.py
+-rw-r--r--   0        0        0      664 2024-04-22 23:05:52.188160 qualitative_coding-1.3.1/qualitative_coding/cli/coders.py
+-rw-r--r--   0        0        0      649 2024-04-22 23:05:52.188529 qualitative_coding-1.3.1/qualitative_coding/cli/codes/__init__.py
+-rw-r--r--   0        0        0     3795 2024-05-11 01:04:09.192093 qualitative_coding-1.3.1/qualitative_coding/cli/codes/crosstab.py
+-rw-r--r--   0        0        0     2533 2024-04-22 23:05:52.190015 qualitative_coding-1.3.1/qualitative_coding/cli/codes/find.py
+-rw-r--r--   0        0        0      668 2024-04-22 23:05:52.191009 qualitative_coding-1.3.1/qualitative_coding/cli/codes/list.py
+-rw-r--r--   0        0        0     1010 2024-04-22 23:05:52.191500 qualitative_coding-1.3.1/qualitative_coding/cli/codes/rename.py
+-rw-r--r--   0        0        0     3551 2024-04-22 23:05:52.192331 qualitative_coding-1.3.1/qualitative_coding/cli/codes/stats.py
+-rw-r--r--   0        0        0      611 2024-04-22 23:05:52.193027 qualitative_coding-1.3.1/qualitative_coding/cli/corpus/__init__.py
+-rw-r--r--   0        0        0     1108 2024-04-22 23:05:52.193719 qualitative_coding-1.3.1/qualitative_coding/cli/corpus/import_media.py
+-rw-r--r--   0        0        0      620 2024-04-22 23:05:52.194269 qualitative_coding-1.3.1/qualitative_coding/cli/corpus/list.py
+-rw-r--r--   0        0        0      629 2024-04-22 23:05:52.194961 qualitative_coding-1.3.1/qualitative_coding/cli/corpus/move.py
+-rw-r--r--   0        0        0      581 2024-04-22 23:05:52.196220 qualitative_coding-1.3.1/qualitative_coding/cli/corpus/remove.py
+-rw-r--r--   0        0        0      611 2024-04-22 23:05:52.196563 qualitative_coding-1.3.1/qualitative_coding/cli/decorators.py
+-rw-r--r--   0        0        0      748 2024-04-26 23:45:57.835343 qualitative_coding-1.3.1/qualitative_coding/cli/export.py
+-rw-r--r--   0        0        0      895 2024-04-22 23:05:52.197716 qualitative_coding-1.3.1/qualitative_coding/cli/init.py
+-rw-r--r--   0        0        0      836 2024-04-22 23:05:52.198230 qualitative_coding-1.3.1/qualitative_coding/cli/memo.py
+-rw-r--r--   0        0        0     1575 2024-02-11 22:24:40.931614 qualitative_coding-1.3.1/qualitative_coding/cli/options.py
+-rw-r--r--   0        0        0      743 2024-04-22 23:05:52.198892 qualitative_coding-1.3.1/qualitative_coding/cli/upgrade.py
+-rw-r--r--   0        0        0      216 2024-02-11 22:24:40.936290 qualitative_coding-1.3.1/qualitative_coding/cli/version.py
+-rw-r--r--   0        0        0       96 2021-07-13 19:40:03.159583 qualitative_coding-1.3.1/qualitative_coding/codebook.py
+-rw-r--r--   0        0        0    36531 2024-04-26 22:37:51.291135 qualitative_coding-1.3.1/qualitative_coding/corpus.py
+-rw-r--r--   0        0        0       50 2024-02-11 22:24:40.939611 qualitative_coding-1.3.1/qualitative_coding/database/errors.py
+-rw-r--r--   0        0        0     3293 2024-04-22 23:05:52.201577 qualitative_coding-1.3.1/qualitative_coding/database/models.py
+-rw-r--r--   0        0        0      865 2024-04-22 23:05:52.202334 qualitative_coding-1.3.1/qualitative_coding/editors.py
+-rw-r--r--   0        0        0      210 2024-04-22 23:05:52.203924 qualitative_coding-1.3.1/qualitative_coding/exceptions.py
+-rw-r--r--   0        0        0     4220 2024-04-22 23:05:52.205339 qualitative_coding-1.3.1/qualitative_coding/helpers.py
+-rw-r--r--   0        0        0      895 2021-07-13 19:40:03.160344 qualitative_coding-1.3.1/qualitative_coding/logs.py
+-rw-r--r--   0        0        0      288 2024-02-11 22:24:40.943568 qualitative_coding-1.3.1/qualitative_coding/media_importers/__init__.py
+-rw-r--r--   0        0        0      560 2024-04-22 23:05:52.205760 qualitative_coding-1.3.1/qualitative_coding/media_importers/base.py
+-rw-r--r--   0        0        0      335 2024-04-22 23:05:52.206697 qualitative_coding-1.3.1/qualitative_coding/media_importers/pandoc.py
+-rw-r--r--   0        0        0      353 2024-04-22 23:05:52.207100 qualitative_coding-1.3.1/qualitative_coding/media_importers/verbatim.py
+-rw-r--r--   0        0        0     1758 2024-04-22 23:05:52.207406 qualitative_coding-1.3.1/qualitative_coding/migrations/__init__.py
+-rw-r--r--   0        0        0     1297 2024-04-22 23:05:52.207666 qualitative_coding-1.3.1/qualitative_coding/migrations/migration.py
+-rw-r--r--   0        0        0      235 2024-04-22 23:05:52.207966 qualitative_coding-1.3.1/qualitative_coding/migrations/migration_0_2_3.py
+-rw-r--r--   0        0        0     4779 2024-04-22 23:05:52.208250 qualitative_coding-1.3.1/qualitative_coding/migrations/migration_1_0_0.py
+-rw-r--r--   0        0        0     7262 2024-04-27 14:32:51.866123 qualitative_coding-1.3.1/qualitative_coding/refi_qda/reader.py
+-rw-r--r--   0        0        0    26395 2024-04-22 23:05:52.210734 qualitative_coding-1.3.1/qualitative_coding/refi_qda/schema.xsd
+-rw-r--r--   0        0        0     6718 2024-04-27 12:29:30.699216 qualitative_coding-1.3.1/qualitative_coding/refi_qda/writer.py
+-rw-r--r--   0        0        0        0 2024-04-22 23:05:52.211669 qualitative_coding-1.3.1/qualitative_coding/tests/__init__.py
+-rw-r--r--   0        0        0     5376 2024-04-22 23:05:52.212557 qualitative_coding-1.3.1/qualitative_coding/tests/fixtures.py
+-rwxr-xr-x   0        0        0     1764 2024-04-22 23:05:52.213687 qualitative_coding-1.3.1/qualitative_coding/tests/mock_editor.py
+-rw-r--r--   0        0        0     1272 2024-04-22 23:05:52.214516 qualitative_coding-1.3.1/qualitative_coding/tests/test_check.py
+-rw-r--r--   0        0        0     1435 2024-04-22 23:05:52.214800 qualitative_coding-1.3.1/qualitative_coding/tests/test_code.py
+-rw-r--r--   0        0        0     1622 2024-04-22 23:05:52.215589 qualitative_coding-1.3.1/qualitative_coding/tests/test_code_parsing.py
+-rw-r--r--   0        0        0      608 2024-04-22 23:05:52.215870 qualitative_coding-1.3.1/qualitative_coding/tests/test_codebook.py
+-rw-r--r--   0        0        0      489 2024-04-22 23:05:52.216106 qualitative_coding-1.3.1/qualitative_coding/tests/test_coders.py
+-rw-r--r--   0        0        0      889 2024-04-22 23:05:52.216404 qualitative_coding-1.3.1/qualitative_coding/tests/test_codes_crosstab.py
+-rw-r--r--   0        0        0      606 2024-04-22 23:05:52.217275 qualitative_coding-1.3.1/qualitative_coding/tests/test_codes_find.py
+-rw-r--r--   0        0        0     1015 2024-04-22 23:05:52.217555 qualitative_coding-1.3.1/qualitative_coding/tests/test_codes_list.py
+-rw-r--r--   0        0        0      805 2024-04-22 23:05:52.217853 qualitative_coding-1.3.1/qualitative_coding/tests/test_codes_rename.py
+-rw-r--r--   0        0        0     1646 2024-04-22 23:05:52.218694 qualitative_coding-1.3.1/qualitative_coding/tests/test_codes_stats.py
+-rw-r--r--   0        0        0     2663 2024-04-22 23:05:52.219419 qualitative_coding-1.3.1/qualitative_coding/tests/test_corpus_import.py
+-rw-r--r--   0        0        0     1501 2024-04-22 23:05:52.219879 qualitative_coding-1.3.1/qualitative_coding/tests/test_corpus_move.py
+-rw-r--r--   0        0        0      655 2024-04-22 23:05:52.220668 qualitative_coding-1.3.1/qualitative_coding/tests/test_corpus_remove.py
+-rw-r--r--   0        0        0      440 2024-04-22 23:05:52.221513 qualitative_coding-1.3.1/qualitative_coding/tests/test_export.py
+-rw-r--r--   0        0        0     1561 2024-04-22 23:05:52.222311 qualitative_coding-1.3.1/qualitative_coding/tests/test_init.py
+-rw-r--r--   0        0        0     1270 2024-04-22 23:05:52.223117 qualitative_coding-1.3.1/qualitative_coding/tests/test_init_import.py
+-rw-r--r--   0        0        0      300 2024-04-22 23:05:52.223384 qualitative_coding-1.3.1/qualitative_coding/tests/test_memo.py
+-rw-r--r--   0        0        0     1646 2024-04-26 23:41:13.289436 qualitative_coding-1.3.1/qualitative_coding/tests/test_refi_qda_writer.py
+-rw-r--r--   0        0        0      849 2024-04-22 23:05:52.224866 qualitative_coding-1.3.1/qualitative_coding/tests/test_tree_node.py
+-rw-r--r--   0        0        0      685 2024-04-22 23:05:52.225137 qualitative_coding-1.3.1/qualitative_coding/tests/test_upgrade.py
+-rw-r--r--   0        0        0      313 2024-04-22 23:05:52.225832 qualitative_coding-1.3.1/qualitative_coding/tests/test_version.py
+-rw-r--r--   0        0        0     6300 2024-04-22 23:05:52.226807 qualitative_coding-1.3.1/qualitative_coding/tree_node.py
+-rw-r--r--   0        0        0      556 2023-12-07 20:04:17.916204 qualitative_coding-1.3.1/qualitative_coding/user_input.py
+-rw-r--r--   0        0        0    12042 2024-02-11 22:24:40.952711 qualitative_coding-1.3.1/qualitative_coding/views/coding_ui.py
+-rw-r--r--   0        0        0      910 2024-02-11 22:24:40.954722 qualitative_coding-1.3.1/qualitative_coding/views/styles.py
+-rw-r--r--   0        0        0    31613 2024-04-26 22:41:04.840295 qualitative_coding-1.3.1/qualitative_coding/views/viewer.py
+-rw-r--r--   0        0        0    14582 1970-01-01 00:00:00.000000 qualitative_coding-1.3.1/PKG-INFO
```

### Comparing `qualitative_coding-1.3.0/LICENSE` & `qualitative_coding-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/README.md` & `qualitative_coding-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/pyproject.toml` & `qualitative_coding-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qualitative-coding"
-version = "1.3.0"
+version = "1.3.1"
 description = "Qualitative coding tools for computer scientists"
 authors = ["Chris Proctor <chris@chrisproctor.net>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "qualitative_coding"}]
 include = ["refi_qda/schema.xml"]
```

### Comparing `qualitative_coding-1.3.0/qualitative_coding/cli/__init__.py` & `qualitative_coding-1.3.1/qualitative_coding/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/cli/click_aliases.py` & `qualitative_coding-1.3.1/qualitative_coding/cli/click_aliases.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/cli/code.py` & `qualitative_coding-1.3.1/qualitative_coding/cli/code.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/cli/coders.py` & `qualitative_coding-1.3.1/qualitative_coding/cli/coders.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/cli/codes/__init__.py` & `qualitative_coding-1.3.1/qualitative_coding/cli/codes/__init__.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/cli/codes/crosstab.py` & `qualitative_coding-1.3.1/qualitative_coding/cli/codes/crosstab.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import yaml
 from pathlib import Path
 from tabulate import tabulate_formats
 from qualitative_coding.corpus import QCCorpus
 from qualitative_coding.views.viewer import QCCorpusViewer
 from qualitative_coding.cli.decorators import handle_qc_errors
+from qualitative_coding.exceptions import IncompatibleOptions
 from qualitative_coding.helpers import read_file_list
 
 @click.command()
 @click.argument("codes", nargs=-1)
 @click.option("-s", "--settings", type=click.Path(exists=True), help="Settings file")
 @click.option("-p", "--pattern", 
         help="Pattern to filter corpus filenames (glob-style)")
```

### Comparing `qualitative_coding-1.3.0/qualitative_coding/cli/codes/find.py` & `qualitative_coding-1.3.1/qualitative_coding/cli/codes/find.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/cli/codes/list.py` & `qualitative_coding-1.3.1/qualitative_coding/cli/codes/list.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/cli/codes/rename.py` & `qualitative_coding-1.3.1/qualitative_coding/cli/codes/rename.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/cli/codes/stats.py` & `qualitative_coding-1.3.1/qualitative_coding/cli/codes/stats.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/cli/corpus/__init__.py` & `qualitative_coding-1.3.1/qualitative_coding/cli/corpus/__init__.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/cli/corpus/import_media.py` & `qualitative_coding-1.3.1/qualitative_coding/cli/corpus/import_media.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/cli/corpus/list.py` & `qualitative_coding-1.3.1/qualitative_coding/cli/corpus/list.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/cli/corpus/move.py` & `qualitative_coding-1.3.1/qualitative_coding/cli/corpus/move.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/cli/corpus/remove.py` & `qualitative_coding-1.3.1/qualitative_coding/cli/corpus/remove.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/cli/decorators.py` & `qualitative_coding-1.3.1/qualitative_coding/cli/decorators.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/cli/export.py` & `qualitative_coding-1.3.1/qualitative_coding/cli/export.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/cli/init.py` & `qualitative_coding-1.3.1/qualitative_coding/cli/init.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/cli/memo.py` & `qualitative_coding-1.3.1/qualitative_coding/cli/memo.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/cli/options.py` & `qualitative_coding-1.3.1/qualitative_coding/cli/options.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/cli/upgrade.py` & `qualitative_coding-1.3.1/qualitative_coding/cli/upgrade.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/corpus.py` & `qualitative_coding-1.3.1/qualitative_coding/corpus.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/database/models.py` & `qualitative_coding-1.3.1/qualitative_coding/database/models.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/editors.py` & `qualitative_coding-1.3.1/qualitative_coding/editors.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/helpers.py` & `qualitative_coding-1.3.1/qualitative_coding/helpers.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/logs.py` & `qualitative_coding-1.3.1/qualitative_coding/logs.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/media_importers/base.py` & `qualitative_coding-1.3.1/qualitative_coding/media_importers/base.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/migrations/__init__.py` & `qualitative_coding-1.3.1/qualitative_coding/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/migrations/migration.py` & `qualitative_coding-1.3.1/qualitative_coding/migrations/migration.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/migrations/migration_1_0_0.py` & `qualitative_coding-1.3.1/qualitative_coding/migrations/migration_1_0_0.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/refi_qda/reader.py` & `qualitative_coding-1.3.1/qualitative_coding/refi_qda/reader.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/refi_qda/schema.xsd` & `qualitative_coding-1.3.1/qualitative_coding/refi_qda/schema.xsd`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/refi_qda/writer.py` & `qualitative_coding-1.3.1/qualitative_coding/refi_qda/writer.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/tests/fixtures.py` & `qualitative_coding-1.3.1/qualitative_coding/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/tests/mock_editor.py` & `qualitative_coding-1.3.1/qualitative_coding/tests/mock_editor.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/tests/test_check.py` & `qualitative_coding-1.3.1/qualitative_coding/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/tests/test_code.py` & `qualitative_coding-1.3.1/qualitative_coding/tests/test_code.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/tests/test_code_parsing.py` & `qualitative_coding-1.3.1/qualitative_coding/tests/test_code_parsing.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/tests/test_codebook.py` & `qualitative_coding-1.3.1/qualitative_coding/tests/test_codebook.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/tests/test_codes_crosstab.py` & `qualitative_coding-1.3.1/qualitative_coding/tests/test_codes_crosstab.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/tests/test_codes_find.py` & `qualitative_coding-1.3.1/qualitative_coding/tests/test_codes_find.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/tests/test_codes_list.py` & `qualitative_coding-1.3.1/qualitative_coding/tests/test_codes_list.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/tests/test_codes_rename.py` & `qualitative_coding-1.3.1/qualitative_coding/tests/test_codes_rename.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/tests/test_codes_stats.py` & `qualitative_coding-1.3.1/qualitative_coding/tests/test_codes_stats.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/tests/test_corpus_import.py` & `qualitative_coding-1.3.1/qualitative_coding/tests/test_corpus_import.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/tests/test_corpus_move.py` & `qualitative_coding-1.3.1/qualitative_coding/tests/test_corpus_move.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/tests/test_corpus_remove.py` & `qualitative_coding-1.3.1/qualitative_coding/tests/test_corpus_remove.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/tests/test_init.py` & `qualitative_coding-1.3.1/qualitative_coding/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/tests/test_init_import.py` & `qualitative_coding-1.3.1/qualitative_coding/tests/test_init_import.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/tests/test_refi_qda_writer.py` & `qualitative_coding-1.3.1/qualitative_coding/tests/test_refi_qda_writer.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/tests/test_tree_node.py` & `qualitative_coding-1.3.1/qualitative_coding/tests/test_tree_node.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/tests/test_upgrade.py` & `qualitative_coding-1.3.1/qualitative_coding/tests/test_upgrade.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/tree_node.py` & `qualitative_coding-1.3.1/qualitative_coding/tree_node.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/user_input.py` & `qualitative_coding-1.3.1/qualitative_coding/user_input.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/views/coding_ui.py` & `qualitative_coding-1.3.1/qualitative_coding/views/coding_ui.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/views/styles.py` & `qualitative_coding-1.3.1/qualitative_coding/views/styles.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/qualitative_coding/views/viewer.py` & `qualitative_coding-1.3.1/qualitative_coding/views/viewer.py`

 * *Files identical despite different names*

### Comparing `qualitative_coding-1.3.0/PKG-INFO` & `qualitative_coding-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qualitative-coding
-Version: 1.3.0
+Version: 1.3.1
 Summary: Qualitative coding tools for computer scientists
 License: MIT
 Author: Chris Proctor
 Author-email: chris@chrisproctor.net
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

