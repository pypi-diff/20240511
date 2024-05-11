# Comparing `tmp/iog-randomizer-4.7.2.2.tar.gz` & `tmp/iog_randomizer-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iog-randomizer-4.7.2.2.tar", last modified: Sat Apr  6 18:59:47 2024, max compression
+gzip compressed data, was "iog_randomizer-5.0.0.tar", last modified: Fri May 10 13:43:32 2024, max compression
```

## Comparing `iog-randomizer-4.7.2.2.tar` & `iog_randomizer-5.0.0.tar`

### file list

```diff
@@ -1,54 +1,134 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 18:59:47.115169 iog-randomizer-4.7.2.2/
--rw-rw-rw-   0        0        0     1233 2020-01-25 15:57:27.000000 iog-randomizer-4.7.2.2/LICENSE
--rw-rw-rw-   0        0        0      235 2024-04-06 18:59:47.114168 iog-randomizer-4.7.2.2/PKG-INFO
--rw-rw-rw-   0        0        0    16459 2020-01-25 15:57:27.000000 iog-randomizer-4.7.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-06 18:59:47.113168 iog-randomizer-4.7.2.2/iog_randomizer.egg-info/
--rw-rw-rw-   0        0        0      235 2024-04-06 18:59:47.000000 iog-randomizer-4.7.2.2/iog_randomizer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1385 2024-04-06 18:59:47.000000 iog-randomizer-4.7.2.2/iog_randomizer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 18:59:47.000000 iog-randomizer-4.7.2.2/iog_randomizer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-06 18:59:47.000000 iog-randomizer-4.7.2.2/iog_randomizer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-06 18:59:47.000000 iog-randomizer-4.7.2.2/iog_randomizer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-06 18:59:47.109170 iog-randomizer-4.7.2.2/randomizer/
--rw-rw-rw-   0        0        0      834 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/ATlMpMuSEWaterHighSub_Tilemap1_comp.bin
--rw-rw-rw-   0        0        0      511 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/ATlMpMuSWWaterHighSub_Tilemap1_comp.bin
--rw-rw-rw-   0        0        0     2341 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/ATlMpSpecInvBg_comp.bin
--rw-rw-rw-   0        0        0     4437 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/ConfigValueArray.asr
--rw-rw-rw-   0        0        0     1257 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/Tilemap6D.bin
--rw-rw-rw-   0        0        0      486 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/TilemapMuPassage.bin
--rw-rw-rw-   0        0        0       25 2020-01-25 15:57:27.000000 iog-randomizer-4.7.2.2/randomizer/__init__.py
--rw-rw-rw-   0        0        0    72688 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/apocalypse_gaia_1.asr
--rw-rw-rw-   0        0        0    20962 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/apocalypse_gaia_2.asr
--rw-rw-rw-   0        0        0   489472 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/asar-x64.dll
--rw-rw-rw-   0        0        0   330280 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/asar-x64.so
--rw-rw-rw-   0        0        0   344576 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/asar-x86.dll
--rw-rw-rw-   0        0        0    14569 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/asar.py
-drwxrwxrwx   0        0        0        0 2024-04-06 18:59:47.109170 iog-randomizer-4.7.2.2/randomizer/bin/
--rw-rw-rw-   0        0        0        0 2020-01-25 15:57:27.000000 iog-randomizer-4.7.2.2/randomizer/bin/__init__.py
--rw-rw-rw-   0        0        0   422504 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/classes.py
--rw-rw-rw-   0        0        0      191 2020-01-25 15:57:27.000000 iog-randomizer-4.7.2.2/randomizer/errors.py
--rw-rw-rw-   0        0        0   247876 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/iogr.asr
--rw-rw-rw-   0        0        0    38030 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/iogr_81_exit_table.asr
--rw-rw-rw-   0        0        0   218181 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/iogr_8C_actor_table.asr
--rw-rw-rw-   0        0        0    71930 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/iogr_8D_asset_table.asr
--rw-rw-rw-   0        0        0    12872 2024-04-06 18:55:39.000000 iog-randomizer-4.7.2.2/randomizer/iogr_asset_ledger.asr
--rw-rw-rw-   0        0        0    75385 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/iogr_code_overflow.asr
--rw-rw-rw-   0        0        0    29315 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/iogr_dialogue_overflow.asr
--rw-rw-rw-   0        0        0    52543 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/iogr_exit_ledger.asr
--rw-rw-rw-   0        0        0      112 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/iogr_fluteless_melody_anim.bin
--rw-rw-rw-   0        0        0    12140 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/iogr_misc_defines.asr
--rw-rw-rw-   0        0        0   436119 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/iogr_monster_defaults.asr
--rw-rw-rw-   0        0        0    57365 2024-04-06 18:58:48.000000 iog-randomizer-4.7.2.2/randomizer/iogr_rom.py
-drwxrwxrwx   0        0        0        0 2024-04-06 18:59:47.111168 iog-randomizer-4.7.2.2/randomizer/models/
--rw-rw-rw-   0        0        0        0 2020-01-25 15:57:27.000000 iog-randomizer-4.7.2.2/randomizer/models/__init__.py
--rw-rw-rw-   0        0        0     1452 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/models/enums.py
--rw-rw-rw-   0        0        0     3164 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/models/randomizer_data.py
--rw-rw-rw-   0        0        0      818 2023-02-24 03:45:40.000000 iog-randomizer-4.7.2.2/randomizer/patch.py
--rw-rw-rw-   0        0        0     4190 2020-01-25 15:57:27.000000 iog-randomizer-4.7.2.2/randomizer/quintet_comp.py
--rw-rw-rw-   0        0        0    18409 2020-01-25 15:57:27.000000 iog-randomizer-4.7.2.2/randomizer/quintet_text.py
--rw-rw-rw-   0        0        0      544 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/table_dialogue.txt
--rw-rw-rw-   0        0        0      520 2024-04-06 18:53:32.000000 iog-randomizer-4.7.2.2/randomizer/table_invtext.txt
-drwxrwxrwx   0        0        0        0 2024-04-06 18:59:47.112168 iog-randomizer-4.7.2.2/randomizer/tests/
--rw-rw-rw-   0        0        0        0 2020-01-25 15:57:27.000000 iog-randomizer-4.7.2.2/randomizer/tests/__init__.py
--rw-rw-rw-   0        0        0      407 2020-01-25 15:57:27.000000 iog-randomizer-4.7.2.2/randomizer/tests/test_generate_filename.py
--rw-rw-rw-   0        0        0       42 2024-04-06 18:59:47.115169 iog-randomizer-4.7.2.2/setup.cfg
--rw-rw-rw-   0        0        0      553 2024-04-06 18:59:06.000000 iog-randomizer-4.7.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:43:32.526042 iog_randomizer-5.0.0/
+drwxrwxrwx   0        0        0        0 2024-05-10 13:43:32.381009 iog_randomizer-5.0.0/.venv/
+drwxrwxrwx   0        0        0        0 2024-05-10 13:43:32.381009 iog_randomizer-5.0.0/.venv/Lib/
+drwxrwxrwx   0        0        0        0 2024-05-10 13:43:32.388010 iog_randomizer-5.0.0/.venv/Lib/site-packages/
+drwxrwxrwx   0        0        0        0 2024-05-10 13:43:32.402014 iog_randomizer-5.0.0/.venv/Lib/site-packages/bitarray-2.9.2.dist-info/
+-rw-rw-rw-   0        0        0        9 2024-05-10 12:38:15.000000 iog_randomizer-5.0.0/.venv/Lib/site-packages/bitarray-2.9.2.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 13:43:32.404014 iog_randomizer-5.0.0/.venv/Lib/site-packages/bitstring-4.2.1.dist-info/
+-rw-rw-rw-   0        0        0       10 2024-05-10 12:38:16.000000 iog_randomizer-5.0.0/.venv/Lib/site-packages/bitstring-4.2.1.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 13:43:32.406014 iog_randomizer-5.0.0/.venv/Lib/site-packages/bsdiff4-1.2.4.dist-info/
+-rw-rw-rw-   0        0        0       90 2024-05-10 12:38:14.000000 iog_randomizer-5.0.0/.venv/Lib/site-packages/bsdiff4-1.2.4.dist-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2024-05-10 12:38:14.000000 iog_randomizer-5.0.0/.venv/Lib/site-packages/bsdiff4-1.2.4.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 13:43:32.407015 iog_randomizer-5.0.0/.venv/Lib/site-packages/build-1.2.1.dist-info/
+-rw-rw-rw-   0        0        0      105 2024-05-10 13:37:24.000000 iog_randomizer-5.0.0/.venv/Lib/site-packages/build-1.2.1.dist-info/entry_points.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 13:43:32.384010 iog_randomizer-5.0.0/.venv/Lib/site-packages/colorama-0.4.6.dist-info/
+drwxrwxrwx   0        0        0        0 2024-05-10 13:43:32.408015 iog_randomizer-5.0.0/.venv/Lib/site-packages/colorama-0.4.6.dist-info/licenses/
+-rw-rw-rw-   0        0        0     1491 2024-05-10 13:37:24.000000 iog_randomizer-5.0.0/.venv/Lib/site-packages/colorama-0.4.6.dist-info/licenses/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 13:43:32.410015 iog_randomizer-5.0.0/.venv/Lib/site-packages/importlib_metadata-7.1.0.dist-info/
+-rw-rw-rw-   0        0        0       19 2024-05-10 13:37:24.000000 iog_randomizer-5.0.0/.venv/Lib/site-packages/importlib_metadata-7.1.0.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 13:43:32.412016 iog_randomizer-5.0.0/.venv/Lib/site-packages/iog_randomizer-5.0.0.dist-info/
+-rw-rw-rw-   0        0        0      115 2024-05-10 12:38:42.000000 iog_randomizer-5.0.0/.venv/Lib/site-packages/iog_randomizer-5.0.0.dist-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2024-05-10 12:38:42.000000 iog_randomizer-5.0.0/.venv/Lib/site-packages/iog_randomizer-5.0.0.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 13:43:32.413016 iog_randomizer-5.0.0/.venv/Lib/site-packages/ips.py-0.1.2.dist-info/
+-rw-rw-rw-   0        0        0        4 2024-05-10 12:38:12.000000 iog_randomizer-5.0.0/.venv/Lib/site-packages/ips.py-0.1.2.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 13:43:32.386010 iog_randomizer-5.0.0/.venv/Lib/site-packages/pip/
+drwxrwxrwx   0        0        0        0 2024-05-10 13:43:32.419017 iog_randomizer-5.0.0/.venv/Lib/site-packages/pip/_vendor/
+-rw-rw-rw-   0        0        0      475 2024-05-10 12:37:53.000000 iog_randomizer-5.0.0/.venv/Lib/site-packages/pip/_vendor/vendor.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 13:43:32.418017 iog_randomizer-5.0.0/.venv/Lib/site-packages/pip-23.2.1.dist-info/
+-rw-rw-rw-   0        0        0    10082 2024-05-10 12:37:56.000000 iog_randomizer-5.0.0/.venv/Lib/site-packages/pip-23.2.1.dist-info/AUTHORS.txt
+-rw-rw-rw-   0        0        0     1093 2024-05-10 12:37:56.000000 iog_randomizer-5.0.0/.venv/Lib/site-packages/pip-23.2.1.dist-info/LICENSE.txt
+-rw-rw-rw-   0        0        0      125 2024-05-10 12:37:56.000000 iog_randomizer-5.0.0/.venv/Lib/site-packages/pip-23.2.1.dist-info/entry_points.txt
+-rw-rw-rw-   0        0        0        4 2024-05-10 12:37:56.000000 iog_randomizer-5.0.0/.venv/Lib/site-packages/pip-23.2.1.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 13:43:32.421018 iog_randomizer-5.0.0/.venv/Lib/site-packages/setuptools-68.2.0.dist-info/
+-rw-rw-rw-   0        0        0     2676 2024-05-10 12:37:54.000000 iog_randomizer-5.0.0/.venv/Lib/site-packages/setuptools-68.2.0.dist-info/entry_points.txt
+-rw-rw-rw-   0        0        0       41 2024-05-10 12:37:54.000000 iog_randomizer-5.0.0/.venv/Lib/site-packages/setuptools-68.2.0.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 13:43:32.387010 iog_randomizer-5.0.0/.venv/Lib/site-packages/wheel/
+drwxrwxrwx   0        0        0        0 2024-05-10 13:43:32.425018 iog_randomizer-5.0.0/.venv/Lib/site-packages/wheel/vendored/
+-rw-rw-rw-   0        0        0       16 2024-05-10 12:37:52.000000 iog_randomizer-5.0.0/.venv/Lib/site-packages/wheel/vendored/vendor.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 13:43:32.423018 iog_randomizer-5.0.0/.venv/Lib/site-packages/wheel-0.41.2.dist-info/
+-rw-rw-rw-   0        0        0     1107 2024-05-10 12:37:52.000000 iog_randomizer-5.0.0/.venv/Lib/site-packages/wheel-0.41.2.dist-info/LICENSE.txt
+-rw-rw-rw-   0        0        0      104 2024-05-10 12:37:52.000000 iog_randomizer-5.0.0/.venv/Lib/site-packages/wheel-0.41.2.dist-info/entry_points.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 13:43:32.426019 iog_randomizer-5.0.0/.venv/Lib/site-packages/zipp-3.18.1.dist-info/
+-rw-rw-rw-   0        0        0        5 2024-05-10 13:37:24.000000 iog_randomizer-5.0.0/.venv/Lib/site-packages/zipp-3.18.1.dist-info/top_level.txt
+-rw-rw-rw-   0        0        0     1233 2021-11-14 05:08:52.000000 iog_randomizer-5.0.0/LICENSE
+-rw-rw-rw-   0        0        0      162 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    37560 2024-05-10 13:43:32.525041 iog_randomizer-5.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    37181 2024-05-10 12:19:06.000000 iog_randomizer-5.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 13:43:32.441022 iog_randomizer-5.0.0/data/
+-rw-rw-rw-   0        0        0    12000 2021-11-14 05:08:52.000000 iog_randomizer-5.0.0/data/ChangeLog.txt
+-rw-rw-rw-   0        0        0     6805 2021-11-14 05:08:52.000000 iog_randomizer-5.0.0/data/IoG RAM Map.txt
+-rw-rw-rw-   0        0        0    48063 2021-11-14 05:08:52.000000 iog_randomizer-5.0.0/data/IoG ROM Map.txt
+-rw-rw-rw-   0        0        0     7397 2021-11-14 05:08:52.000000 iog_randomizer-5.0.0/data/IoG Text Table.txt
+-rw-rw-rw-   0        0        0     7972 2021-11-14 05:08:52.000000 iog_randomizer-5.0.0/data/IoGR Tutorial.txt
+-rw-rw-rw-   0        0        0   108526 2021-11-14 05:08:52.000000 iog_randomizer-5.0.0/data/IoGR_Notes.txt
+-rw-rw-rw-   0        0        0    28118 2021-11-14 05:08:52.000000 iog_randomizer-5.0.0/data/ItemEvents.txt
+-rw-rw-rw-   0        0        0     5183 2021-11-14 05:08:52.000000 iog_randomizer-5.0.0/data/RAM_Data_for_Autotracker.txt
+-rw-rw-rw-   0        0        0    52242 2021-11-14 05:08:52.000000 iog_randomizer-5.0.0/data/WorldMapEvents.txt
+-rw-rw-rw-   0        0        0    28765 2021-11-14 05:08:52.000000 iog_randomizer-5.0.0/data/mapdataset.txt
+-rw-rw-rw-   0        0        0    30064 2021-11-14 05:08:52.000000 iog_randomizer-5.0.0/data/mapdataset_van.txt
+-rw-rw-rw-   0        0        0   150620 2021-11-14 05:08:52.000000 iog_randomizer-5.0.0/data/text_boxes.txt
+-rw-rw-rw-   0        0        0      826 2024-05-10 13:42:59.000000 iog_randomizer-5.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       26 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/requirements.txt
+-rw-rw-rw-   0        0        0       44 2024-05-10 12:40:08.000000 iog_randomizer-5.0.0/rompath.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 13:43:32.526042 iog_randomizer-5.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-10 13:43:32.389011 iog_randomizer-5.0.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-10 13:43:32.390011 iog_randomizer-5.0.0/src/iog_randomizer/
+drwxrwxrwx   0        0        0        0 2024-05-10 13:43:32.462027 iog_randomizer-5.0.0/src/iog_randomizer/cli/
+-rw-rw-rw-   0        0        0        0 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/cli/__init__.py
+-rw-rw-rw-   0        0        0     4549 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/cli/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:43:32.464028 iog_randomizer-5.0.0/src/iog_randomizer/gui/
+-rw-rw-rw-   0        0        0        0 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/gui/__init__.py
+-rw-rw-rw-   0        0        0    36201 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/gui/gui.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:43:32.506037 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/
+-rw-rw-rw-   0        0        0      834 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/ATlMpMuSEWaterHighSub_Tilemap1_comp.bin
+-rw-rw-rw-   0        0        0      511 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/ATlMpMuSWWaterHighSub_Tilemap1_comp.bin
+-rw-rw-rw-   0        0        0     2341 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/ATlMpSpecInvBg_comp.bin
+-rw-rw-rw-   0        0        0     4505 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/ConfigValueArray.asr
+-rw-rw-rw-   0        0        0     1257 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/Tilemap6D.bin
+-rw-rw-rw-   0        0        0      486 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/TilemapMuPassage.bin
+-rw-rw-rw-   0        0        0       25 2024-05-10 13:42:59.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:43:32.507037 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/__pycache__/
+-rw-rw-rw-   0        0        0    13314 2024-05-10 12:38:55.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/__pycache__/asar.cpython-39.pyc
+-rw-rw-rw-   0        0        0    72688 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/apocalypse_gaia_1.asr
+-rw-rw-rw-   0        0        0    20949 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/apocalypse_gaia_2.asr
+-rw-rw-rw-   0        0        0   489472 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/asar-x64.dll
+-rw-rw-rw-   0        0        0   330280 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/asar-x64.so
+-rw-rw-rw-   0        0        0   344576 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/asar-x86.dll
+-rw-rw-rw-   0        0        0    14617 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/asar.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:43:32.508038 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/bin/
+-rw-rw-rw-   0        0        0        0 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/bin/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:43:32.392012 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/bin/plugins/
+drwxrwxrwx   0        0        0        0 2024-05-10 13:43:32.394012 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/bin/plugins/sprites/
+drwxrwxrwx   0        0        0        0 2024-05-10 13:43:32.511038 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/bin/plugins/sprites/bagu/
+-rw-rw-rw-   0        0        0    16384 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/bin/plugins/sprites/bagu/1a8000.bin
+-rw-rw-rw-   0        0        0     5120 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/bin/plugins/sprites/bagu/1b8000.bin
+drwxrwxrwx   0        0        0        0 2024-05-10 13:43:32.512038 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/bin/plugins/sprites/freet/
+-rw-rw-rw-   0        0        0     2356 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/bin/plugins/sprites/freet/1a820a.bin
+drwxrwxrwx   0        0        0        0 2024-05-10 13:43:32.516039 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/bin/plugins/sprites/invisible/
+-rw-rw-rw-   0        0        0    32768 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/bin/plugins/sprites/invisible/1a8000.bin
+-rw-rw-rw-   0        0        0    32768 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/bin/plugins/sprites/invisible/1b8000.bin
+-rw-rw-rw-   0        0        0    16384 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/bin/plugins/sprites/invisible/1c8000.bin
+drwxrwxrwx   0        0        0        0 2024-05-10 13:43:32.517040 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/bin/plugins/sprites/solar/
+-rw-rw-rw-   0        0        0    69280 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/bin/plugins/sprites/solar/1a8000.bin
+drwxrwxrwx   0        0        0        0 2024-05-10 13:43:32.518040 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/bin/plugins/sprites/sye/
+-rw-rw-rw-   0        0        0    69280 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/bin/plugins/sprites/sye/1a8000.bin
+-rw-rw-rw-   0        0        0   429283 2024-05-10 12:37:27.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/classes.py
+-rw-rw-rw-   0        0        0      190 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/errors.py
+-rw-rw-rw-   0        0        0   256360 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/iogr.asr
+-rw-rw-rw-   0        0        0    38030 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/iogr_81_exit_table.asr
+-rw-rw-rw-   0        0        0   218229 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/iogr_8C_actor_table.asr
+-rw-rw-rw-   0        0        0    71930 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/iogr_8D_asset_table.asr
+-rw-rw-rw-   0        0        0    12872 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/iogr_asset_ledger.asr
+-rw-rw-rw-   0        0        0    77851 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/iogr_code_overflow.asr
+-rw-rw-rw-   0        0        0    29624 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/iogr_dialogue_overflow.asr
+-rw-rw-rw-   0        0        0    52543 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/iogr_exit_ledger.asr
+-rw-rw-rw-   0        0        0      112 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/iogr_fluteless_melody_anim.bin
+-rw-rw-rw-   0        0        0    12516 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/iogr_misc_defines.asr
+-rw-rw-rw-   0        0        0   436119 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/iogr_monster_defaults.asr
+-rw-rw-rw-   0        0        0    56196 2024-05-10 13:43:22.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/iogr_rom.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:43:32.522040 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/models/
+-rw-rw-rw-   0        0        0        0 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/models/__init__.py
+-rw-rw-rw-   0        0        0     1468 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/models/enums.py
+-rw-rw-rw-   0        0        0     2401 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/models/randomizer_data.py
+-rw-rw-rw-   0        0        0      818 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/patch.py
+-rw-rw-rw-   0        0        0     4118 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/quintet_comp.py
+-rw-rw-rw-   0        0        0    17365 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/quintet_text.py
+-rw-rw-rw-   0        0        0      544 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/table_dialogue.txt
+-rw-rw-rw-   0        0        0      520 2024-05-10 12:20:09.000000 iog_randomizer-5.0.0/src/iog_randomizer/randomizer/table_invtext.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 13:43:32.524041 iog_randomizer-5.0.0/src/iog_randomizer.egg-info/
+-rw-rw-rw-   0        0        0    37560 2024-05-10 13:43:32.000000 iog_randomizer-5.0.0/src/iog_randomizer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4432 2024-05-10 13:43:32.000000 iog_randomizer-5.0.0/src/iog_randomizer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 13:43:32.000000 iog_randomizer-5.0.0/src/iog_randomizer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2024-05-10 13:43:32.000000 iog_randomizer-5.0.0/src/iog_randomizer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       25 2024-05-10 13:43:32.000000 iog_randomizer-5.0.0/src/iog_randomizer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-10 13:43:32.000000 iog_randomizer-5.0.0/src/iog_randomizer.egg-info/top_level.txt
```

### Comparing `iog-randomizer-4.7.2.2/LICENSE` & `iog_randomizer-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.2/README.md` & `iog_randomizer-5.0.0/data/ChangeLog.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,1029 +1,750 @@
-00000000: 2323 2054 6865 2049 6c6c 7573 696f 6e20  ## The Illusion 
-00000010: 6f66 2047 6169 6120 5261 6e64 6f6d 697a  of Gaia Randomiz
-00000020: 6572 2028 7631 2e35 2e31 2920 2d20 3c61  er (v1.5.1) - <a
-00000030: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
-00000040: 6974 6875 622e 636f 6d2f 446f 6e74 4261  ithub.com/DontBa
-00000050: 6775 4d65 2f49 6f47 522f 7265 6c65 6173  guMe/IoGR/releas
-00000060: 6573 2f74 6167 2f76 312e 352e 3122 3e44  es/tag/v1.5.1">D
-00000070: 6f77 6e6c 6f61 643c 2f61 3e0d 0a54 6869  ownload</a>..Thi
-00000080: 7320 7261 6e64 6f6d 697a 6572 2069 7320  s randomizer is 
-00000090: 636f 6d70 6174 6962 6c65 2077 6974 6820  compatible with 
-000000a0: 7468 6520 5553 2076 6572 7369 6f6e 206f  the US version o
-000000b0: 6620 7468 6520 496c 6c75 7369 6f6e 206f  f the Illusion o
-000000c0: 6620 4761 6961 2052 4f4d 2e0d 0a0d 0a3c  f Gaia ROM.....<
-000000d0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-000000e0: 6469 7363 6f72 642e 6767 2f4b 665a 3456  discord.gg/KfZ4V
-000000f0: 6544 223e 4a6f 696e 2074 6865 2043 6f6d  eD">Join the Com
-00000100: 6d75 6e69 7479 206f 6e20 4469 7363 6f72  munity on Discor
-00000110: 643c 2f61 3e0d 0a0d 0a3c 6120 6872 6566  d</a>....<a href
-00000120: 3d22 6874 7470 733a 2f2f 7777 772e 796f  ="https://www.yo
-00000130: 7574 7562 652e 636f 6d2f 7761 7463 683f  utube.com/watch?
-00000140: 763d 5935 3562 746f 4466 7544 7726 6c69  v=Y55btoDfuDw&li
-00000150: 7374 3d50 4c65 3252 7a37 424f 576b 3032  st=PLe2Rz7BOWk02
-00000160: 6773 4734 4d6e 5854 3544 5f37 366f 6d56  gsG4MnXT5D_76omV
-00000170: 5438 5137 6b22 3e57 6174 6368 2061 2056  T8Q7k">Watch a V
-00000180: 6964 656f 2054 7574 6f72 6961 6c3c 2f61  ideo Tutorial</a
-00000190: 3e0d 0a0d 0a54 6865 203c 6120 6872 6566  >....The <a href
-000001a0: 3d22 6874 7470 733a 2f2f 656d 6f74 7261  ="https://emotra
-000001b0: 636b 6572 2e6e 6574 2f64 6f77 6e6c 6f61  cker.net/downloa
-000001c0: 642f 223e 496f 4752 2045 6d6f 5472 6163  d/">IoGR EmoTrac
-000001d0: 6b65 723c 2f61 3e20 6973 206e 6f77 206c  ker</a> is now l
-000001e0: 6976 6521 0d0a 0d0a 2323 2323 2054 6865  ive!....#### The
-000001f0: 202e 6578 6520 7061 636b 6167 650d 0a54   .exe package..T
-00000200: 6865 2065 7865 6375 7461 626c 6520 6861  he executable ha
-00000210: 7320 6265 656e 2076 6572 6966 6965 6420  s been verified 
-00000220: 746f 2077 6f72 6b20 6f6e 2057 696e 646f  to work on Windo
-00000230: 7773 2c20 4c69 6e75 7820 616e 6420 5769  ws, Linux and Wi
-00000240: 6e65 2e0d 0a0d 0a4e 4f54 453a 2049 7420  ne.....NOTE: It 
-00000250: 6973 2063 6f6d 6d6f 6e20 666f 7220 7468  is common for th
-00000260: 6520 7261 6e64 6f6d 697a 6572 2070 726f  e randomizer pro
-00000270: 6772 616d 2074 6f20 6265 2066 6c61 6767  gram to be flagg
-00000280: 6564 2061 7320 6120 7669 7275 7320 696e  ed as a virus in
-00000290: 2057 696e 646f 7773 2044 6566 656e 6465   Windows Defende
-000002a0: 722e 2020 5468 6973 2069 7320 6120 6b6e  r.  This is a kn
-000002b0: 6f77 6e20 6973 7375 6520 666f 7220 6d61  own issue for ma
-000002c0: 6e79 2070 726f 6772 616d 7320 7468 6174  ny programs that
-000002d0: 2068 6176 6520 6265 656e 2063 6f6d 7069   have been compi
-000002e0: 6c65 6420 696e 2050 7969 6e73 7461 6c6c  led in Pyinstall
-000002f0: 6572 2c20 616e 6420 6120 7469 636b 6574  er, and a ticket
-00000300: 2068 6173 2062 6565 6e20 7375 626d 6974   has been submit
-00000310: 7465 6420 666f 7220 7468 6973 2070 726f  ted for this pro
-00000320: 6772 616d 2069 6e20 7061 7274 6963 756c  gram in particul
-00000330: 6172 2e20 2049 6e20 7468 6520 6d65 616e  ar.  In the mean
-00000340: 7469 6d65 2c20 796f 7520 6361 6e20 3c61  time, you can <a
-00000350: 2068 7265 663d 2268 7474 7073 3a2f 2f73   href="https://s
-00000360: 7570 706f 7274 2e6d 6963 726f 736f 6674  upport.microsoft
-00000370: 2e63 6f6d 2f65 6e2d 7573 2f68 656c 702f  .com/en-us/help/
-00000380: 3430 3238 3438 352f 7769 6e64 6f77 732d  4028485/windows-
-00000390: 3130 2d61 6464 2d61 6e2d 6578 636c 7573  10-add-an-exclus
-000003a0: 696f 6e2d 746f 2d77 696e 646f 7773 2d73  ion-to-windows-s
-000003b0: 6563 7572 6974 7922 3e63 7265 6174 6520  ecurity">create 
-000003c0: 616e 2065 7863 6c75 7369 6f6e 3c2f 613e  an exclusion</a>
-000003d0: 2066 6f72 2074 6865 2066 6f6c 6465 7220   for the folder 
-000003e0: 746f 2077 6869 6368 2079 6f75 2065 7874  to which you ext
-000003f0: 7261 6374 2074 6865 2049 6f47 5220 7072  ract the IoGR pr
-00000400: 6f67 7261 6d20 6669 6c65 732e 0d0a 0d0a  ogram files.....
-00000410: 2323 2323 2074 6865 202e 7079 2070 6163  #### the .py pac
-00000420: 6b61 6765 0d0a 466f 7220 6e6f 6e2d 5769  kage..For non-Wi
-00000430: 6e64 6f77 7320 7573 6572 2077 6974 6820  ndows user with 
-00000440: 5079 7468 6f6e 2032 2e37 2069 6e73 7461  Python 2.7 insta
-00000450: 6c6c 6564 2c20 7573 6520 7468 6520 2270  lled, use the "p
-00000460: 7922 2070 6163 6b61 6765 2061 6e64 2072  y" package and r
-00000470: 756e 2074 6865 2022 696f 6772 2e70 7922  un the "iogr.py"
-00000480: 2073 6372 6970 7420 746f 2065 7865 6375   script to execu
-00000490: 7465 2074 6865 2072 616e 646f 6d69 7a65  te the randomize
-000004a0: 7220 696e 7465 7266 6163 652e 0d0a 0d0a  r interface.....
-000004b0: 2323 2320 4372 6561 7469 6e67 2061 2052  ### Creating a R
-000004c0: 616e 646f 6d69 7a65 6420 524f 4d0d 0a46  andomized ROM..F
-000004d0: 6f72 2074 6865 2072 616e 646f 6d69 7a65  or the randomize
-000004e0: 7220 746f 2066 756e 6374 696f 6e2c 2079  r to function, y
-000004f0: 6f75 206d 7573 7420 656e 7375 7265 2074  ou must ensure t
-00000500: 6861 7420 2269 6f67 722e 6578 6522 206f  hat "iogr.exe" o
-00000510: 7220 2269 6f67 722e 7079 2220 6973 2072  r "iogr.py" is r
-00000520: 756e 2066 726f 6d20 7468 6520 7361 6d65  un from the same
-00000530: 2064 6972 6563 746f 7279 2074 6861 7420   directory that 
-00000540: 616c 736f 2063 6f6e 7461 696e 7320 7468  also contains th
-00000550: 6520 2262 696e 2220 6469 7265 6374 6f72  e "bin" director
-00000560: 7920 2861 7320 7765 6c6c 2061 7320 2269  y (as well as "i
-00000570: 6f67 722e 6963 6f22 206f 7220 2269 6f67  ogr.ico" or "iog
-00000580: 722e 706e 6722 2066 6f72 2074 6865 202e  r.png" for the .
-00000590: 6578 6529 2e20 2049 7420 6973 2072 6563  exe).  It is rec
-000005a0: 6f6d 6d65 6e64 6564 2074 6861 7420 6120  ommended that a 
-000005b0: 636f 7079 206f 6620 7468 6520 5553 2076  copy of the US v
-000005c0: 6572 7369 6f6e 206f 6620 7468 6520 496c  ersion of the Il
-000005d0: 6c75 7369 6f6e 206f 6620 4761 6961 2052  lusion of Gaia R
-000005e0: 4f4d 2061 6c73 6f20 6578 6973 7420 7769  OM also exist wi
-000005f0: 7468 696e 2074 6869 7320 6469 7265 6374  thin this direct
-00000600: 6f72 792c 2074 6f20 6d61 6b65 2062 726f  ory, to make bro
-00000610: 7773 696e 6720 7769 7468 696e 2074 6865  wsing within the
-00000620: 2075 7365 7220 696e 7465 7266 6163 6520   user interface 
-00000630: 6d6f 7265 2063 6f6e 7665 6e69 656e 742e  more convenient.
-00000640: 2020 5468 6520 6e61 6d65 206f 6620 7468    The name of th
-00000650: 6520 524f 4d20 6669 6c65 2064 6f65 7320  e ROM file does 
-00000660: 6e6f 7420 6e65 6564 2074 6f20 6164 6865  not need to adhe
-00000670: 7265 2074 6f20 6120 7374 616e 6461 7264  re to a standard
-00000680: 2066 6f72 6d61 742e 0d0a 0d0a 5275 6e6e   format.....Runn
-00000690: 696e 6720 2269 6f67 722e 6578 6522 206f  ing "iogr.exe" o
-000006a0: 7220 2269 6f67 722e 7079 222c 2069 6e70  r "iogr.py", inp
-000006b0: 7574 7469 6e67 2074 6865 2064 6573 6972  utting the desir
-000006c0: 6564 2073 6574 7469 6e67 732c 2061 6e64  ed settings, and
-000006d0: 2068 6974 7469 6e67 2022 4765 6e65 7261   hitting "Genera
-000006e0: 7465 2052 4f4d 2220 7769 6c6c 2063 7265  te ROM" will cre
-000006f0: 6174 6520 6120 7261 6e64 6f6d 697a 6564  ate a randomized
-00000700: 2052 4f4d 2028 6173 2077 656c 6c20 6173   ROM (as well as
-00000710: 2061 2073 706f 696c 6572 206c 6f67 2920   a spoiler log) 
-00000720: 696e 2074 6865 2073 616d 6520 6469 7265  in the same dire
-00000730: 6374 6f72 7920 6173 2079 6f75 7220 6f72  ctory as your or
-00000740: 6967 696e 616c 2052 4f4d 2066 696c 652e  iginal ROM file.
-00000750: 2020 5468 6520 6f72 6967 696e 616c 2066    The original f
-00000760: 696c 6520 7769 6c6c 2072 656d 6169 6e20  ile will remain 
-00000770: 696e 7461 6374 2e0d 0a0d 0a23 2323 2052  intact.....### R
-00000780: 616e 646f 6d69 7a65 7220 5365 7474 696e  andomizer Settin
-00000790: 6773 0d0a 4265 6c6f 7720 6172 6520 6578  gs..Below are ex
-000007a0: 706c 616e 6174 696f 6e73 206f 6620 7468  planations of th
-000007b0: 6520 7661 7269 6f75 7320 7365 7474 696e  e various settin
-000007c0: 6773 206f 6620 7468 6520 7261 6e64 6f6d  gs of the random
-000007d0: 697a 6572 2e0d 0a23 2323 2320 4469 6666  izer...#### Diff
-000007e0: 6963 756c 7479 0d0a 5468 6572 6520 6172  iculty..There ar
-000007f0: 6520 666f 7572 2064 6966 6669 6375 6c74  e four difficult
-00000800: 7920 7365 7474 696e 6773 3a20 4561 7379  y settings: Easy
-00000810: 2c20 4e6f 726d 616c 2c20 4861 7264 2c20  , Normal, Hard, 
-00000820: 616e 6420 4578 7472 656d 652e 2054 6865  and Extreme. The
-00000830: 2064 6966 6669 6375 6c74 7920 6368 6f73   difficulty chos
-00000840: 656e 2061 6666 6563 7473 2074 6865 2066  en affects the f
-00000850: 6f6c 6c6f 7769 6e67 2067 616d 6520 6d65  ollowing game me
-00000860: 6368 616e 6963 733a 0d0a 2d20 456e 656d  chanics:..- Enem
-00000870: 6965 733a 2045 6e65 6d69 6573 2073 6361  ies: Enemies sca
-00000880: 6c65 2069 6e20 7374 7265 6e67 7468 2077  le in strength w
-00000890: 6974 6820 6561 6368 2064 6966 6669 6375  ith each difficu
-000008a0: 6c74 7920 6d6f 6465 2e0d 0a2d 2052 6f6f  lty mode...- Roo
-000008b0: 6d20 5265 7761 7264 733a 2054 6865 206e  m Rewards: The n
-000008c0: 756d 6265 7220 6f66 2072 6f6f 6d2d 636c  umber of room-cl
-000008d0: 6561 7269 6e67 2072 6577 6172 6473 2061  earing rewards a
-000008e0: 7661 696c 6162 6c65 2074 6f20 7468 6520  vailable to the 
-000008f0: 706c 6179 6572 2069 7320 6166 6665 6374  player is affect
-00000900: 6564 2062 7920 6469 6666 6963 756c 7479  ed by difficulty
-00000910: 2028 7365 6520 6265 6c6f 7729 2e0d 0a2d   (see below)...-
-00000920: 2049 7465 6d20 616e 6420 4162 696c 6974   Item and Abilit
-00000930: 7920 506c 6163 656d 656e 743a 2045 6173  y Placement: Eas
-00000940: 7920 616e 6420 4e6f 726d 616c 206d 6f64  y and Normal mod
-00000950: 6573 2062 6f74 6820 696e 636c 7564 6520  es both include 
-00000960: 6120 736c 6967 6874 2062 6961 7320 746f  a slight bias to
-00000970: 7761 7264 206d 616b 696e 6720 7265 7175  ward making requ
-00000980: 6972 6564 2069 7465 6d73 2061 6e64 2061  ired items and a
-00000990: 6269 6c69 7469 6573 2061 7661 696c 6162  bilities availab
-000009a0: 6c65 2074 6f20 7468 6520 706c 6179 6572  le to the player
-000009b0: 2065 6172 6c69 6572 206f 6e2e 0d0a 2d20   earlier on...- 
-000009c0: 496e 2d47 616d 6520 5370 6f69 6c65 7273  In-Game Spoilers
-000009d0: 3a20 4869 6e74 7320 6861 7665 2062 6565  : Hints have bee
-000009e0: 6e20 7265 6d6f 7665 6420 696e 2045 7874  n removed in Ext
-000009f0: 7265 6d65 206d 6f64 652e 0d0a 0d0a 2323  reme mode.....##
-00000a00: 2323 2047 6f61 6c0d 0a54 6869 7320 616c  ## Goal..This al
-00000a10: 6c6f 7773 2079 6f75 2074 6f20 6368 6f6f  lows you to choo
-00000a20: 7365 2061 2067 616d 6520 6d6f 6465 2c20  se a game mode, 
-00000a30: 7768 6574 6865 7220 4461 726b 2047 6169  whether Dark Gai
-00000a40: 6120 6f72 2052 6564 204a 6577 656c 2048  a or Red Jewel H
-00000a50: 756e 7420 2873 6565 2062 656c 6f77 292e  unt (see below).
-00000a60: 0d0a 0d0a 2323 2323 204c 6f67 6963 0d0a  ....#### Logic..
-00000a70: 5468 6572 6520 6172 6520 7468 7265 6520  There are three 
-00000a80: 6c6f 6769 6320 6d6f 6465 7320 6176 6169  logic modes avai
-00000a90: 6c61 626c 6520 746f 2074 6865 2070 6c61  lable to the pla
-00000aa0: 7965 722e 0d0a 2d20 436f 6d70 6c65 7461  yer...- Completa
-00000ab0: 626c 653a 2054 6869 7320 6c6f 6769 6320  ble: This logic 
-00000ac0: 656e 7375 7265 7320 7468 6174 2065 7665  ensures that eve
-00000ad0: 7279 2069 7465 6d20 616e 6420 6162 696c  ry item and abil
-00000ae0: 6974 7920 6c6f 6361 7469 6f6e 2069 7320  ity location is 
-00000af0: 7265 6163 6861 626c 652c 2061 6c6c 6f77  reachable, allow
-00000b00: 696e 6720 6576 6572 7920 7365 6564 2074  ing every seed t
-00000b10: 6f20 6265 2063 6f6d 706c 6574 6564 2031  o be completed 1
-00000b20: 3030 252e 2054 6869 7320 7465 6e64 7320  00%. This tends 
-00000b30: 746f 2079 6965 6c64 2073 6c69 6768 746c  to yield slightl
-00000b40: 7920 6c6f 6e67 6572 2067 616d 6570 6c61  y longer gamepla
-00000b50: 7920 6578 7065 7269 656e 6365 732e 0d0a  y experiences...
-00000b60: 2d20 4265 6174 6162 6c65 3a20 496e 2042  - Beatable: In B
-00000b70: 6561 7461 626c 6520 7365 6564 732c 2079  eatable seeds, y
-00000b80: 6f75 2061 7265 2067 7561 7261 6e74 6565  ou are guarantee
-00000b90: 6420 746f 2068 6176 6520 6163 6365 7373  d to have access
-00000ba0: 2074 6f20 6576 6572 7920 6974 656d 2061   to every item a
-00000bb0: 6e64 2061 6269 6c69 7479 2079 6f75 206e  nd ability you n
-00000bc0: 6565 6420 746f 2063 6f6d 706c 6574 6520  eed to complete 
-00000bd0: 796f 7572 2067 6f61 6c2c 2074 686f 7567  your goal, thoug
-00000be0: 6820 796f 7520 6d61 7920 6e6f 7420 6861  h you may not ha
-00000bf0: 7665 2061 6363 6573 7320 746f 2065 7665  ve access to eve
-00000c00: 7279 2069 7465 6d20 6c6f 6361 7469 6f6e  ry item location
-00000c10: 2069 6e20 7468 6520 6761 6d65 2e20 5468   in the game. Th
-00000c20: 6973 2074 656e 6473 2074 6f20 7969 656c  is tends to yiel
-00000c30: 6420 736c 6967 6874 6c79 206d 6f72 6520  d slightly more 
-00000c40: 7374 7265 616d 6c69 6e65 6420 7365 6564  streamlined seed
-00000c50: 7320 2d2d 2068 6f77 6576 6572 2c20 6974  s -- however, it
-00000c60: 2063 6f75 6c64 2061 6c73 6f20 6d61 6b65   could also make
-00000c70: 2068 656c 7066 756c 2069 7465 6d73 206c   helpful items l
-00000c80: 696b 6520 7374 6174 7573 2075 7067 7261  ike status upgra
-00000c90: 6465 7320 756e 6174 7461 696e 6162 6c65  des unattainable
-00000ca0: 2c20 6d61 6b69 6e67 2074 6869 7320 6d6f  , making this mo
-00000cb0: 6465 2073 6c69 6768 746c 7920 6d6f 7265  de slightly more
-00000cc0: 2064 616e 6765 726f 7573 2e0d 0a2d 2043   dangerous...- C
-00000cd0: 6861 6f73 3a20 4162 696c 6974 7920 706c  haos: Ability pl
-00000ce0: 6163 656d 656e 7420 7265 7374 7269 6374  acement restrict
-00000cf0: 696f 6e73 2068 6176 6520 6265 656e 2064  ions have been d
-00000d00: 7261 7374 6963 616c 6c79 206c 6f6f 7365  rastically loose
-00000d10: 6e65 6420 696e 2074 6869 7320 6d6f 6465  ned in this mode
-00000d20: 202d 2d20 666f 7220 696e 7374 616e 6365   -- for instance
-00000d30: 2c20 4672 6565 6461 6e20 6162 696c 6974  , Freedan abilit
-00000d40: 6965 7320 6361 6e20 7368 6f77 2075 7020  ies can show up 
-00000d50: 696e 2074 6f77 6e73 2c20 616e 6420 4461  in towns, and Da
-00000d60: 726b 2053 7061 6365 7320 7468 6174 2061  rk Spaces that a
-00000d70: 7265 2074 7970 6963 616c 6c79 2072 6573  re typically res
-00000d80: 6572 7665 6420 666f 7220 666f 726d 2063  erved for form c
-00000d90: 6861 6e67 6573 206d 6967 6874 2063 6f6e  hanges might con
-00000da0: 7461 696e 2061 6269 6c69 7469 6573 2c20  tain abilities, 
-00000db0: 7072 6576 656e 7469 6e67 2074 6865 2070  preventing the p
-00000dc0: 6c61 7965 7220 6672 6f6d 2063 6f6d 706c  layer from compl
-00000dd0: 6574 696e 6720 6475 6e67 656f 6e73 2061  eting dungeons a
-00000de0: 6e64 2061 6363 6573 7369 6e67 2063 6572  nd accessing cer
-00000df0: 7461 696e 2069 7465 6d20 6c6f 6361 7469  tain item locati
-00000e00: 6f6e 732e 2020 4173 2069 6e20 4265 6174  ons.  As in Beat
-00000e10: 6162 6c65 2c20 4368 616f 7320 6d6f 6465  able, Chaos mode
-00000e20: 2073 7469 6c6c 2065 6e73 7572 6573 2074   still ensures t
-00000e30: 6861 7420 7468 6520 706c 6179 6572 2068  hat the player h
-00000e40: 6173 2061 6363 6573 7320 746f 2061 6c6c  as access to all
-00000e50: 2074 6865 2069 7465 6d73 2061 6e64 206c   the items and l
-00000e60: 6f63 6174 696f 6e73 206e 6563 6573 7361  ocations necessa
-00000e70: 7279 2074 6f20 6265 6174 2074 6865 2067  ry to beat the g
-00000e80: 616d 652e 0d0a 0d0a 2323 2323 2053 7461  ame.....#### Sta
-00000e90: 7475 6573 0d0a 596f 7520 6361 6e20 6368  tues..You can ch
-00000ea0: 6f6f 7365 2074 6865 206e 756d 6265 7220  oose the number 
-00000eb0: 6f66 204d 7973 7469 6320 5374 6174 7565  of Mystic Statue
-00000ec0: 7320 7265 7175 6972 6564 2074 6f20 636f  s required to co
-00000ed0: 6d70 6c65 7465 2044 6172 6b20 4761 6961  mplete Dark Gaia
-00000ee0: 2073 6565 6473 2c20 6f72 206d 616b 6520   seeds, or make 
-00000ef0: 7468 6520 6e75 6d62 6572 2072 616e 646f  the number rando
-00000f00: 6d2e 2054 6869 7320 7061 7261 6d65 7465  m. This paramete
-00000f10: 7220 6973 2069 676e 6f72 6564 2066 6f72  r is ignored for
-00000f20: 2052 6564 204a 6577 656c 2048 756e 7473   Red Jewel Hunts
-00000f30: 2e0d 0a0d 0a23 2323 2042 6561 7469 6e67  .....### Beating
-00000f40: 2074 6865 2047 616d 650d 0a54 6865 7265   the Game..There
-00000f50: 2061 7265 2063 7572 7265 6e74 6c79 2074   are currently t
-00000f60: 776f 206d 6f64 6573 2028 676f 616c 7329  wo modes (goals)
-00000f70: 2066 6f72 2063 6f6d 706c 6574 696e 6720   for completing 
-00000f80: 7468 6520 6761 6d65 3a0d 0a23 2323 2320  the game:..#### 
-00000f90: 4461 726b 2047 6169 610d 0a49 6e20 7468  Dark Gaia..In th
-00000fa0: 6973 206d 6f64 652c 2079 6f75 206d 7573  is mode, you mus
-00000fb0: 7420 6669 6e64 2074 6865 204d 6167 6963  t find the Magic
-00000fc0: 2044 7573 7420 616e 6420 7573 6520 6974   Dust and use it
-00000fd0: 2074 6f20 6672 6565 204b 6172 6120 6672   to free Kara fr
-00000fe0: 6f6d 2068 6572 2070 6f72 7472 6169 742e  om her portrait.
-00000ff0: 2020 596f 7520 6d75 7374 2074 6865 6e20    You must then 
-00001000: 756e 6974 6520 7769 7468 2068 6572 2074  unite with her t
-00001010: 6f20 6465 6665 6174 2044 6172 6b20 4761  o defeat Dark Ga
-00001020: 6961 2c20 6120 7072 6f63 6573 7320 7768  ia, a process wh
-00001030: 6963 6820 7265 7175 6972 6573 2079 6f75  ich requires you
-00001040: 2074 6f20 6861 7665 2053 6861 646f 7727   to have Shadow'
-00001050: 7320 666f 726d 2075 6e6c 6f63 6b65 6420  s form unlocked 
-00001060: 2862 7920 6f62 7461 696e 696e 6720 616e  (by obtaining an
-00001070: 6420 7573 696e 6720 7468 6520 4175 7261  d using the Aura
-00001080: 2920 6173 2077 656c 6c20 6173 2061 2063  ) as well as a c
-00001090: 6572 7461 696e 206e 756d 6265 7220 6f66  ertain number of
-000010a0: 2074 6865 2067 616d 6527 7320 7369 7820   the game's six 
-000010b0: 4d79 7374 6963 2053 7461 7475 6573 2e0d  Mystic Statues..
-000010c0: 0a0d 0a4b 6172 6127 7320 706f 7274 7261  ...Kara's portra
-000010d0: 6974 2063 616e 2062 6520 666f 756e 6420  it can be found 
-000010e0: 696e 206f 6e65 206f 6620 7468 6520 6669  in one of the fi
-000010f0: 7665 206d 696e 6f72 2064 756e 6765 6f6e  ve minor dungeon
-00001100: 732c 2073 7065 6369 6669 6564 2062 656c  s, specified bel
-00001110: 6f77 2e20 2054 6865 206c 6f63 6174 696f  ow.  The locatio
-00001120: 6e20 6f66 204b 6172 6127 7320 706f 7274  n of Kara's port
-00001130: 7261 6974 2077 696c 6c20 6265 2063 6f6e  rait will be con
-00001140: 7461 696e 6564 2069 6e20 4c61 6e63 6527  tained in Lance'
-00001150: 7320 4c65 7474 6572 2e0d 0a2d 2045 6477  s Letter...- Edw
-00001160: 6172 6427 7320 556e 6465 7267 726f 756e  ard's Undergroun
-00001170: 6420 5475 6e6e 656c 0d0a 2d20 5468 6520  d Tunnel..- The 
-00001180: 4469 616d 6f6e 6420 4d69 6e65 0d0a 2d20  Diamond Mine..- 
-00001190: 5468 6520 416e 6765 6c20 5669 6c6c 6167  The Angel Villag
-000011a0: 650d 0a2d 204d 742e 204b 7265 7373 0d0a  e..- Mt. Kress..
-000011b0: 2d20 416e 6b6f 7220 5761 742e 0d0a 0d0a  - Ankor Wat.....
-000011c0: 4561 6368 2073 6565 6420 6d61 7920 7265  Each seed may re
-000011d0: 7175 6972 6520 6120 6365 7274 6169 6e20  quire a certain 
-000011e0: 6e75 6d62 6572 206f 6620 7468 6520 7369  number of the si
-000011f0: 7820 4d79 7374 6963 2053 7461 7475 6573  x Mystic Statues
-00001200: 2e20 5461 6c6b 696e 6720 746f 2074 6865  . Talking to the
-00001210: 2073 6368 6f6f 6c74 6561 6368 6572 2069   schoolteacher i
-00001220: 6e20 536f 7574 6820 4361 7065 2061 7420  n South Cape at 
-00001230: 7468 6520 7374 6172 7420 6f66 2074 6865  the start of the
-00001240: 2067 616d 6520 7769 6c6c 2069 6e64 6963   game will indic
-00001250: 6174 6520 7768 6963 6820 7374 6174 7565  ate which statue
-00001260: 7320 6172 6520 7265 7175 6972 6564 2e20  s are required. 
-00001270: 5468 6520 7374 6174 7565 7320 6172 6520  The statues are 
-00001280: 6163 7175 6972 6564 2062 7920 636f 6d70  acquired by comp
-00001290: 6c65 7469 6e67 2074 6865 2066 6f6c 6c6f  leting the follo
-000012a0: 7769 6e67 2062 6f73 7365 732f 6c6f 6361  wing bosses/loca
-000012b0: 7469 6f6e 733a 0d0a 0d0a 2d20 5374 6174  tions:....- Stat
-000012c0: 7565 2031 3a20 4361 7374 6f74 6820 2849  ue 1: Castoth (I
-000012d0: 6e63 6120 5275 696e 7329 0d0a 2d20 5374  nca Ruins)..- St
-000012e0: 6174 7565 2032 3a20 5669 7065 7220 2853  atue 2: Viper (S
-000012f0: 6b79 2047 6172 6465 6e29 0d0a 2d20 5374  ky Garden)..- St
-00001300: 6174 7565 2033 3a20 5661 6d70 6972 6573  atue 3: Vampires
-00001310: 2028 4d75 290d 0a2d 2053 7461 7475 6520   (Mu)..- Statue 
-00001320: 343a 2053 616e 6720 4661 6e67 6572 2028  4: Sang Fanger (
-00001330: 4772 6561 7420 5761 6c6c 290d 0a2d 2053  Great Wall)..- S
-00001340: 7461 7475 6520 353a 204d 756d 6d79 2051  tatue 5: Mummy Q
-00001350: 7565 656e 2028 5079 7261 6d69 6429 0d0a  ueen (Pyramid)..
-00001360: 2d20 5374 6174 7565 2036 3a20 426f 7373  - Statue 6: Boss
-00001370: 2052 7573 6820 2842 6162 656c 2054 6f77   Rush (Babel Tow
-00001380: 6572 2920 4f52 2053 6f6c 6964 2041 726d  er) OR Solid Arm
-00001390: 2028 4a65 7765 6c65 7227 7320 4d61 6e73   (Jeweler's Mans
-000013a0: 696f 6e29 0d0a 0d0a 4f6e 6365 2079 6f75  ion)....Once you
-000013b0: 2072 6573 6375 6520 4b61 7261 2c20 756e   rescue Kara, un
-000013c0: 6c6f 636b 2053 6861 646f 7727 7320 666f  lock Shadow's fo
-000013d0: 726d 2c20 616e 6420 6561 726e 2074 6865  rm, and earn the
-000013e0: 2061 7070 6c69 6361 626c 6520 5374 6174   applicable Stat
-000013f0: 7565 7320 2869 6620 616e 7929 2c20 796f  ues (if any), yo
-00001400: 7520 6d61 7920 7461 6c6b 2074 6f20 4761  u may talk to Ga
-00001410: 6961 2061 7420 616e 7920 4461 726b 2053  ia at any Dark S
-00001420: 7061 6365 2c20 7768 6f20 7769 6c6c 2067  pace, who will g
-00001430: 7261 6e74 2079 6f75 2074 6865 206f 7074  rant you the opt
-00001440: 696f 6e20 746f 2066 6163 6520 4461 726b  ion to face Dark
-00001450: 2047 6169 6120 616e 6420 7769 6e20 7468   Gaia and win th
-00001460: 6520 6761 6d65 2e0d 0a0d 0a23 2323 2320  e game.....#### 
-00001470: 5265 6420 4a65 7765 6c20 4875 6e74 0d0a  Red Jewel Hunt..
-00001480: 466f 7220 7468 6973 206d 6f64 652c 2074  For this mode, t
-00001490: 6865 2073 6f6c 6520 6f62 6a65 6374 6976  he sole objectiv
-000014a0: 6520 6973 2074 6f20 636f 6c6c 6563 7420  e is to collect 
-000014b0: 7468 6520 7265 7175 6972 6564 206e 756d  the required num
-000014c0: 6265 7220 6f66 2052 6564 204a 6577 656c  ber of Red Jewel
-000014d0: 7320 6173 2071 7569 636b 6c79 2061 7320  s as quickly as 
-000014e0: 706f 7373 6962 6c65 2061 6e64 2074 7572  possible and tur
-000014f0: 6e20 7468 656d 2069 6e74 6f20 7468 6520  n them into the 
-00001500: 4a65 7765 6c65 722e 2020 5468 6520 6e75  Jeweler.  The nu
-00001510: 6d62 6572 206f 6620 5265 6420 4a65 7765  mber of Red Jewe
-00001520: 6c73 2072 6571 7569 7265 6420 6973 2033  ls required is 3
-00001530: 3520 666f 7220 4561 7379 2c20 3430 2066  5 for Easy, 40 f
-00001540: 6f72 204e 6f72 6d61 6c2c 2061 6e64 2035  or Normal, and 5
-00001550: 3020 666f 7220 4861 7264 2f45 7874 7265  0 for Hard/Extre
-00001560: 6d65 2e20 2054 7572 6e69 6e67 2074 6865  me.  Turning the
-00001570: 7365 2069 6e74 6f20 7468 6520 4a65 7765  se into the Jewe
-00001580: 6c65 7220 616e 6420 7370 6561 6b69 6e67  ler and speaking
-00001590: 2077 6974 6820 6869 6d20 616c 6c6f 7773   with him allows
-000015a0: 2079 6f75 2074 6f20 6265 6174 2074 6865   you to beat the
-000015b0: 2067 616d 652e 0d0a 0d0a 2323 2320 4665   game.....### Fe
-000015c0: 6174 7572 6573 0d0a 2323 2323 2049 7465  atures..#### Ite
-000015d0: 6d20 5368 7566 666c 650d 0a54 6865 2069  m Shuffle..The i
-000015e0: 7465 6d73 2069 6e20 7468 6520 6761 6d65  tems in the game
-000015f0: 2077 696c 6c20 6265 2073 6875 6666 6c65   will be shuffle
-00001600: 6420 6163 726f 7373 2074 6865 2067 616d  d across the gam
-00001610: 652e 2020 4966 2074 6865 2072 616e 646f  e.  If the rando
-00001620: 6d69 7a65 7220 6973 2063 7265 6174 6564  mizer is created
-00001630: 2077 6974 6820 2243 6f6d 706c 6574 6162   with "Completab
-00001640: 6c65 2220 6c6f 6769 632c 2065 7665 7279  le" logic, every
-00001650: 2069 7465 6d20 6c6f 6361 7469 6f6e 2077   item location w
-00001660: 696c 6c20 6265 2061 6363 6573 7369 626c  ill be accessibl
-00001670: 653b 2069 6620 6974 2069 7320 2242 6561  e; if it is "Bea
-00001680: 7461 626c 6522 2c20 6365 7274 6169 6e20  table", certain 
-00001690: 6974 656d 7320 6e6f 7420 7265 7175 6972  items not requir
-000016a0: 6564 2074 6f20 6675 6c66 696c 6c20 7468  ed to fulfill th
-000016b0: 6520 6761 6d65 2773 206f 626a 6563 7469  e game's objecti
-000016c0: 7665 7320 6d61 7920 6265 2069 6e61 6363  ves may be inacc
-000016d0: 6573 7369 626c 652e 0d0a 2323 2323 2041  essible...#### A
-000016e0: 6269 6c69 7479 2053 6875 6666 6c65 0d0a  bility Shuffle..
-000016f0: 5468 6520 7370 6563 6961 6c20 6174 7461  The special atta
-00001700: 636b 7320 6172 6520 7368 7566 666c 6564  cks are shuffled
-00001710: 2074 6872 6f75 6768 6f75 7420 7468 6520   throughout the 
-00001720: 4461 726b 2053 7061 6365 7320 696e 2074  Dark Spaces in t
-00001730: 6865 2067 616d 652e 2020 4461 726b 2053  he game.  Dark S
-00001740: 7061 6365 7320 696e 2070 6561 6365 6675  paces in peacefu
-00001750: 6c20 6c6f 6361 7469 6f6e 7320 6361 6e20  l locations can 
-00001760: 6f6e 6c79 2063 6f6e 7461 696e 2057 696c  only contain Wil
-00001770: 6c20 6162 696c 6974 6965 732c 2077 6865  l abilities, whe
-00001780: 7265 6173 2044 6172 6b20 5370 6163 6573  reas Dark Spaces
-00001790: 2069 6e20 6261 7474 6c65 2061 7265 6173   in battle areas
-000017a0: 2063 616e 2063 6f6e 7461 696e 2065 6974   can contain eit
-000017b0: 6865 7220 5769 6c6c 206f 7220 4672 6565  her Will or Free
-000017c0: 6461 6e20 6162 696c 6974 6965 732e 2020  dan abilities.  
-000017d0: 496e 2022 436f 6d70 6c65 7461 626c 6522  In "Completable"
-000017e0: 206d 6f64 652c 2073 6f6d 6520 4461 726b   mode, some Dark
-000017f0: 2053 7061 6365 7320 6172 6520 7265 7365   Spaces are rese
-00001800: 7276 6564 2066 6f72 2066 6f72 6d20 6368  rved for form ch
-00001810: 616e 6765 7320 616e 6420 7769 6c6c 206e  anges and will n
-00001820: 6576 6572 2063 6f6e 7461 696e 2061 6269  ever contain abi
-00001830: 6c69 7469 6573 202d 2d20 7375 6368 2061  lities -- such a
-00001840: 7320 7468 6520 4461 726b 2053 7061 6365  s the Dark Space
-00001850: 2069 6e20 7468 6520 556e 6465 7267 726f   in the Undergro
-00001860: 756e 6420 5475 6e6e 656c 2c20 666f 7220  und Tunnel, for 
-00001870: 6578 616d 706c 652e 0d0a 2323 2323 204f  example...#### O
-00001880: 7665 7277 6f72 6c64 204d 6f76 656d 656e  verworld Movemen
-00001890: 740d 0a54 6865 2077 6f72 6c64 2069 7320  t..The world is 
-000018a0: 6272 6f6b 656e 2075 7020 696e 746f 2063  broken up into c
-000018b0: 6f6e 7469 6e65 6e74 732e 2054 6865 206c  ontinents. The l
-000018c0: 6f63 6174 696f 6e73 2069 6e20 6120 636f  ocations in a co
-000018d0: 6e74 696e 656e 7420 6172 6520 616c 6c20  ntinent are all 
-000018e0: 6163 6365 7373 6962 6c65 2074 6f20 6f6e  accessible to on
-000018f0: 6520 616e 6f74 6865 7220 7468 726f 7567  e another throug
-00001900: 6820 7468 6520 776f 726c 6420 6d61 7020  h the world map 
-00001910: 7363 7265 656e 2e20 5468 6520 666f 6c6c  screen. The foll
-00001920: 6f77 696e 6720 6c6f 6361 7469 6f6e 7320  owing locations 
-00001930: 6172 6520 6163 6365 7373 6962 6c65 2074  are accessible t
-00001940: 6f20 6f6e 6520 616e 6f74 6865 7220 7669  o one another vi
-00001950: 6120 7468 6520 6f76 6572 776f 726c 643a  a the overworld:
-00001960: 0d0a 2d20 536f 7574 682d 5765 7374 2043  ..- South-West C
-00001970: 6f6e 7469 6e65 6e74 2028 536f 7574 6820  ontinent (South 
-00001980: 4361 7065 2c20 4564 7761 7264 2773 2043  Cape, Edward's C
-00001990: 6173 746c 652c 2049 746f 7279 2056 696c  astle, Itory Vil
-000019a0: 6c61 6765 2c20 4d6f 6f6e 2054 7269 6265  lage, Moon Tribe
-000019b0: 2043 616d 702c 2049 6e63 6120 5275 696e   Camp, Inca Ruin
-000019c0: 7329 0d0a 2d20 536f 7574 682d 4561 7374  s)..- South-East
-000019d0: 2043 6f6e 7469 6e65 6e74 2028 4469 616d   Continent (Diam
-000019e0: 6f6e 6420 436f 6173 742c 2046 7265 656a  ond Coast, Freej
-000019f0: 6961 2c20 4469 616d 6f6e 6420 4d69 6e65  ia, Diamond Mine
-00001a00: 2c20 4e65 696c 2773 2043 6f74 7461 6765  , Neil's Cottage
-00001a10: 2c20 4e61 7a63 6120 506c 6169 6e29 0d0a  , Nazca Plain)..
-00001a20: 2d20 4e6f 7274 682d 4561 7374 2043 6f6e  - North-East Con
-00001a30: 7469 6e65 6e74 2028 416e 6765 6c20 5669  tinent (Angel Vi
-00001a40: 6c6c 6167 652c 2057 6174 6572 6d69 612c  llage, Watermia,
-00001a50: 2047 7265 6174 2057 616c 6c29 0d0a 2d20   Great Wall)..- 
-00001a60: 4e6f 7274 6820 436f 6e74 696e 656e 7420  North Continent 
-00001a70: 2845 7572 6f2c 204d 742e 204b 7265 7373  (Euro, Mt. Kress
-00001a80: 2c20 4e61 7469 7665 7327 2056 696c 6c61  , Natives' Villa
-00001a90: 6765 2c20 416e 6b6f 7220 5761 7429 0d0a  ge, Ankor Wat)..
-00001aa0: 2d20 4e6f 7274 682d 5765 7374 2043 6f6e  - North-West Con
-00001ab0: 7469 6e65 6e74 2028 4461 6f2c 2050 7972  tinent (Dao, Pyr
-00001ac0: 616d 6964 290d 0a0d 0a4d 6f76 656d 656e  amid)....Movemen
-00001ad0: 7420 6265 7477 6565 6e20 636f 6e74 696e  t between contin
-00001ae0: 656e 7473 2028 616e 6420 746f 206c 6f63  ents (and to loc
-00001af0: 6174 696f 6e73 206e 6f74 2073 7065 6369  ations not speci
-00001b00: 6669 6564 2061 626f 7665 2920 6265 636f  fied above) beco
-00001b10: 6d65 7320 706f 7373 6962 6c65 2061 7320  mes possible as 
-00001b20: 6974 656d 7320 6172 6520 6163 7175 6972  items are acquir
-00001b30: 6564 2c20 6f72 2061 7320 7175 6573 7420  ed, or as quest 
-00001b40: 6576 656e 7473 2061 7265 2063 6f6d 706c  events are compl
-00001b50: 6574 6564 3a0d 0a2d 2044 6566 6561 7469  eted:..- Defeati
-00001b60: 6e67 2043 6173 746f 7468 2069 6e20 496e  ng Castoth in In
-00001b70: 6361 2052 7569 6e73 2067 7261 6e74 7320  ca Ruins grants 
-00001b80: 796f 7520 6163 6365 7373 2074 6f20 7468  you access to th
-00001b90: 6520 476f 6c64 2053 6869 702c 2077 6869  e Gold Ship, whi
-00001ba0: 6368 2074 616b 6573 2079 6f75 2074 6f20  ch takes you to 
-00001bb0: 7468 6520 4469 616d 6f6e 6420 436f 6173  the Diamond Coas
-00001bc0: 742e 0d0a 2d20 4465 6665 6174 696e 6720  t...- Defeating 
-00001bd0: 5669 7065 7220 696e 2053 6b79 2047 6172  Viper in Sky Gar
-00001be0: 6465 6e20 7461 6b65 7320 796f 7520 746f  den takes you to
-00001bf0: 2074 6865 2053 6561 7369 6465 2050 616c   the Seaside Pal
-00001c00: 6163 652e 0d0a 2d20 4163 7175 6972 696e  ace...- Acquirin
-00001c10: 6720 7468 6520 5465 6170 6f74 2061 6c6c  g the Teapot all
-00001c20: 6f77 7320 796f 7520 746f 2075 7365 2069  ows you to use i
-00001c30: 7420 6f6e 2074 6865 2070 6c61 7465 6175  t on the plateau
-00001c40: 2069 6e20 7468 6520 4d6f 6f6e 2054 7269   in the Moon Tri
-00001c50: 6265 2063 616d 702e 2054 6869 7320 6772  be camp. This gr
-00001c60: 616e 7473 2079 6f75 2061 6363 6573 7320  ants you access 
-00001c70: 746f 2074 6865 2053 6b79 2047 6172 6465  to the Sky Garde
-00001c80: 6e2e 2028 4166 7465 7220 7573 696e 6720  n. (After using 
-00001c90: 7468 6520 5465 6170 6f74 2c20 796f 7520  the Teapot, you 
-00001ca0: 6361 6e20 7573 6520 7468 6520 536b 7920  can use the Sky 
-00001cb0: 4761 7264 656e 2074 6f20 7472 6176 656c  Garden to travel
-00001cc0: 2074 6f20 7468 6520 4d6f 6f6e 2054 7269   to the Moon Tri
-00001cd0: 6265 2043 616d 702c 2074 6865 204e 6163  be Camp, the Nac
-00001ce0: 7a61 2050 6c61 696e 2c20 6f72 2074 6865  za Plain, or the
-00001cf0: 2053 6561 7369 6465 2050 616c 6163 652e   Seaside Palace.
-00001d00: 290d 0a2d 2041 6371 7569 7269 6e67 204c  )..- Acquiring L
-00001d10: 6f6c 6127 7320 4c65 7474 6572 2061 6c6c  ola's Letter all
-00001d20: 6f77 7320 796f 7520 746f 206c 6561 726e  ows you to learn
-00001d30: 204d 6f72 7365 2043 6f64 652e 2041 6674   Morse Code. Aft
-00001d40: 6572 2072 6561 6469 6e67 2074 6865 206c  er reading the l
-00001d50: 6574 7465 722c 2074 616c 6b20 746f 2045  etter, talk to E
-00001d60: 7269 6b20 696e 2074 6865 2053 6561 7369  rik in the Seasi
-00001d70: 6465 2043 6176 6520 696e 2053 6f75 7468  de Cave in South
-00001d80: 2043 6170 652e 2054 6f67 6574 6865 7220   Cape. Together 
-00001d90: 796f 7520 6361 6e20 636f 6d6d 756e 6963  you can communic
-00001da0: 6174 6520 7769 7468 2053 6574 6820 2877  ate with Seth (w
-00001db0: 686f 2069 7320 696e 2052 6976 6572 736f  ho is in Riverso
-00001dc0: 6e20 666f 726d 292c 2077 686f 2063 616e  n form), who can
-00001dd0: 2074 7261 6e73 706f 7274 2079 6f75 2074   transport you t
-00001de0: 6f20 7468 6520 4469 616d 6f6e 6420 436f  o the Diamond Co
-00001df0: 6173 7420 6f72 2057 6174 6572 6d69 612e  ast or Watermia.
-00001e00: 2054 7572 626f 2074 6865 2064 6f67 2028   Turbo the dog (
-00001e10: 4469 616d 6f6e 6420 436f 6173 7429 2061  Diamond Coast) a
-00001e20: 6e64 2074 6865 206d 616e 2073 7461 6e64  nd the man stand
-00001e30: 696e 6720 6174 2074 6865 2065 6e74 7261  ing at the entra
-00001e40: 6e63 6520 696e 2057 6174 6572 6d69 6120  nce in Watermia 
-00001e50: 6361 6e20 616c 736f 2063 6f6d 6d75 6e69  can also communi
-00001e60: 6361 7465 2077 6974 6820 5365 7468 2066  cate with Seth f
-00001e70: 6f72 2079 6f75 2e0d 0a2d 2055 706f 6e20  or you...- Upon 
-00001e80: 6163 7175 6972 696e 6720 7468 6520 4d65  acquiring the Me
-00001e90: 6d6f 7279 204d 656c 6f64 792c 2079 6f75  mory Melody, you
-00001ea0: 2063 616e 2076 6973 6974 204e 6569 6c20   can visit Neil 
-00001eb0: 696e 2068 6973 2063 6f74 7461 6765 2c20  in his cottage, 
-00001ec0: 7768 6f20 6861 7320 666f 7267 6f74 7465  who has forgotte
-00001ed0: 6e20 686f 7720 746f 2070 696c 6f74 2068  n how to pilot h
-00001ee0: 6973 2061 6972 706c 616e 652e 2050 6c61  is airplane. Pla
-00001ef0: 7969 6e67 2074 6869 7320 6d65 6c6f 6479  ying this melody
-00001f00: 2066 6f72 2068 696d 2072 6573 746f 7265   for him restore
-00001f10: 7320 6869 7320 6d65 6d6f 7279 2e20 4672  s his memory. Fr
-00001f20: 6f6d 2074 6865 6e20 6f6e 2c20 6865 2069  om then on, he i
-00001f30: 7320 6861 7070 7920 746f 2074 616b 6520  s happy to take 
-00001f40: 796f 7520 746f 2045 7572 6f2c 2044 616f  you to Euro, Dao
-00001f50: 2c20 6f72 2042 6162 656c 2054 6f77 6572  , or Babel Tower
-00001f60: 2e20 4865 2063 616e 2062 6520 666f 756e  . He can be foun
-00001f70: 6420 6569 7468 6572 2069 6e20 6869 7320  d either in his 
-00001f80: 686f 6d65 2c20 696e 2068 6973 206d 616e  home, in his man
-00001f90: 7369 6f6e 2069 6e20 4575 726f 2c20 6f72  sion in Euro, or
-00001fa0: 2069 6e20 6869 7320 726f 6f6d 2069 6e20   in his room in 
-00001fb0: 4461 6f2e 0d0a 2d20 4163 7175 6972 696e  Dao...- Acquirin
-00001fc0: 6720 7468 6520 5769 6c6c 2061 6c6c 6f77  g the Will allow
-00001fd0: 7320 796f 7520 746f 2075 7365 204b 7275  s you to use Kru
-00001fe0: 6b73 2074 6f20 7472 6176 656c 2062 6574  ks to travel bet
-00001ff0: 7765 656e 2057 6174 6572 6d69 6120 616e  ween Watermia an
-00002000: 6420 4575 726f 2e20 5768 656e 2074 6865  d Euro. When the
-00002010: 2057 696c 6c20 6973 2069 6e20 796f 7572   Will is in your
-00002020: 2069 6e76 656e 746f 7279 2c20 7370 6561   inventory, spea
-00002030: 6b20 746f 2074 6865 206d 616e 2074 656e  k to the man ten
-00002040: 6469 6e67 2068 6973 204b 7275 6b73 2069  ding his Kruks i
-00002050: 6e20 5761 7465 726d 6961 206a 7573 7420  n Watermia just 
-00002060: 6561 7374 206f 6620 7468 6520 746f 776e  east of the town
-00002070: 2065 6e74 7261 6e63 652c 206f 7220 746f   entrance, or to
-00002080: 2074 6865 206d 616e 2073 7461 6e64 696e   the man standin
-00002090: 6720 6279 2074 6865 2065 6173 7420 656e  g by the east en
-000020a0: 7472 616e 6365 2074 6f20 7468 6520 6369  trance to the ci
-000020b0: 7479 206f 6620 4575 726f 2e20 0d0a 2d20  ty of Euro. ..- 
-000020c0: 5570 6f6e 2061 6371 7569 7269 6e67 2074  Upon acquiring t
-000020d0: 6865 204c 6172 6765 2052 6f61 7374 2c20  he Large Roast, 
-000020e0: 676f 2074 6f20 7468 6520 4e61 7469 7665  go to the Native
-000020f0: 7327 2056 696c 6c61 6765 2061 6e64 2074  s' Village and t
-00002100: 616c 6b20 746f 2074 6865 2079 6f75 6e67  alk to the young
-00002110: 2062 6f79 2e20 4966 2079 6f75 2067 6976   boy. If you giv
-00002120: 6520 6869 6d20 7468 6520 726f 6173 742c  e him the roast,
-00002130: 2068 6520 7769 6c6c 2067 7261 7465 6675   he will gratefu
-00002140: 6c6c 7920 6775 6964 6520 796f 7520 6163  lly guide you ac
-00002150: 726f 7373 2074 6865 2074 7265 6163 6865  ross the treache
-00002160: 726f 7573 2065 7870 616e 7365 2066 726f  rous expanse fro
-00002170: 6d20 7468 6520 7669 6c6c 6167 6520 746f  m the village to
-00002180: 2044 616f 2e20 5468 6520 6d61 6e20 696e   Dao. The man in
-00002190: 2044 616f 2077 686f 2067 7261 6e74 7320   Dao who grants 
-000021a0: 796f 7520 7477 6f20 6974 656d 7320 6361  you two items ca
-000021b0: 6e20 616c 736f 2068 6972 6520 6120 6775  n also hire a gu
-000021c0: 6964 6520 746f 2074 616b 6520 796f 7520  ide to take you 
-000021d0: 6261 636b 2074 6f20 4e61 7469 7665 7327  back to Natives'
-000021e0: 2066 6f72 2066 7265 652e 0d0a 2d20 496e   for free...- In
-000021f0: 2074 6865 204e 617a 6361 2050 6c61 696e   the Nazca Plain
-00002200: 2c20 6966 2079 6f75 2067 6f20 746f 2074  , if you go to t
-00002210: 6865 206c 6f63 6174 696f 6e20 6f66 2074  he location of t
-00002220: 6865 2074 696c 6520 6275 7269 6564 2069  he tile buried i
-00002230: 6e20 7468 6520 7361 6e64 2c20 796f 7520  n the sand, you 
-00002240: 6361 6e20 7761 7270 2074 6f20 7468 6520  can warp to the 
-00002250: 536b 7920 4761 7264 656e 2e20 486f 7765  Sky Garden. Howe
-00002260: 7665 722c 2074 6865 204d 6f6f 6e20 5472  ver, the Moon Tr
-00002270: 6962 6520 7769 6c6c 206f 6e6c 7920 6170  ibe will only ap
-00002280: 7065 6172 2074 6865 7265 2069 6620 796f  pear there if yo
-00002290: 7520 6861 7665 2068 6561 6c65 6420 7468  u have healed th
-000022a0: 656d 2077 6974 6820 7468 6520 5465 6170  em with the Teap
-000022b0: 6f74 2e20 596f 7520 6361 6e20 6578 6974  ot. You can exit
-000022c0: 2074 6f20 7468 6520 6f76 6572 776f 726c   to the overworl
-000022d0: 6420 6672 6f6d 2074 6865 2053 6b79 2047  d from the Sky G
-000022e0: 6172 6465 6e20 6279 2067 6f69 6e67 2075  arden by going u
-000022f0: 7020 696e 746f 2074 6865 2061 7265 6120  p into the area 
-00002300: 7768 6572 6520 796f 7520 6e6f 726d 616c  where you normal
-00002310: 6c79 2065 6e74 6572 2066 726f 6d20 4e61  ly enter from Na
-00002320: 7a63 612e 0d0a 2d20 4d75 2061 6e64 2074  zca...- Mu and t
-00002330: 6865 2053 6561 7369 6465 2050 616c 6163  he Seaside Palac
-00002340: 6520 6172 6520 6163 6365 7373 6962 6c65  e are accessible
-00002350: 2064 6972 6563 746c 7920 6672 6f6d 2041   directly from A
-00002360: 6e67 656c 2056 696c 6c61 6765 2e20 5768  ngel Village. Wh
-00002370: 6174 2069 7320 6f72 6967 696e 616c 6c79  at is originally
-00002380: 2074 6865 2067 7565 7374 2072 6f6f 6d20   the guest room 
-00002390: 696e 2074 6865 2076 616e 696c 6c61 2067  in the vanilla g
-000023a0: 616d 6520 7461 6b65 7320 796f 7520 746f  ame takes you to
-000023b0: 2074 6865 2050 6173 7361 6765 2074 6f20   the Passage to 
-000023c0: 4d75 2069 6e73 6964 6520 7468 6520 5365  Mu inside the Se
-000023d0: 6173 6964 6520 5061 6c61 6365 2e20 4d75  aside Palace. Mu
-000023e0: 2069 7320 6672 6565 6c79 2061 6363 6573   is freely acces
-000023f0: 7369 626c 6520 7468 6973 2077 6179 2c20  sible this way, 
-00002400: 6275 7420 7468 6520 4d75 2050 616c 6163  but the Mu Palac
-00002410: 6520 4b65 7920 6973 2072 6571 7569 7265  e Key is require
-00002420: 6420 746f 2065 6e74 6572 2074 6865 2053  d to enter the S
-00002430: 6561 7369 6465 2050 616c 6163 6520 7669  easide Palace vi
-00002440: 6120 7468 6973 2072 6f75 7465 2e0d 0a23  a this route...#
-00002450: 2323 2320 526f 6f6d 2052 6577 6172 6473  ### Room Rewards
-00002460: 2061 6e64 2053 7461 7420 5570 6772 6164   and Stat Upgrad
-00002470: 6573 0d0a 5468 6520 6e75 6d62 6572 206f  es..The number o
-00002480: 6620 4850 2c20 5354 5220 616e 6420 4445  f HP, STR and DE
-00002490: 4620 7570 6772 6164 6573 2061 7661 696c  F upgrades avail
-000024a0: 6162 6c65 2069 6e20 7468 6520 6761 6d65  able in the game
-000024b0: 2068 6173 2062 6565 6e20 7265 6475 6365   has been reduce
-000024c0: 6420 746f 2072 6566 6c65 6374 2074 6865  d to reflect the
-000024d0: 2065 7874 7265 6d65 2062 616c 616e 6369   extreme balanci
-000024e0: 6e67 206f 6620 656e 656d 7920 7374 6174  ng of enemy stat
-000024f0: 6973 7469 6373 2074 6872 6f75 6768 6f75  istics throughou
-00002500: 7420 7468 6520 6761 6d65 202d 2d20 736f  t the game -- so
-00002510: 2074 686f 7567 6820 7468 6520 6e75 6d62   though the numb
-00002520: 6572 206f 6620 7570 6772 6164 6573 2068  er of upgrades h
-00002530: 6173 2064 6563 7265 6173 6564 2c20 6561  as decreased, ea
-00002540: 6368 2075 7067 7261 6465 2069 7320 6d75  ch upgrade is mu
-00002550: 6368 206d 6f72 6520 7369 676e 6966 6963  ch more signific
-00002560: 616e 7420 7468 616e 2069 6e20 7468 6520  ant than in the 
-00002570: 7661 6e69 6c6c 6120 6761 6d65 2e20 2048  vanilla game.  H
-00002580: 5020 7570 6772 6164 6573 2067 7261 6e74  P upgrades grant
-00002590: 2079 6f75 202b 3320 4850 2065 6163 682e   you +3 HP each.
-000025a0: 0d0a 0d0a 5468 6520 7265 7761 7264 7320  ....The rewards 
-000025b0: 6172 6520 7368 7566 666c 6564 2061 7420  are shuffled at 
-000025c0: 7261 6e64 6f6d 2074 6872 6f75 6768 6f75  random throughou
-000025d0: 7420 7468 6520 656e 7469 7265 2067 616d  t the entire gam
-000025e0: 652c 206d 6170 2062 7920 6d61 702e 2020  e, map by map.  
-000025f0: 5468 6520 746f 7461 6c20 7265 7761 7264  The total reward
-00002600: 7320 6176 6169 6c61 626c 6520 6279 2064  s available by d
-00002610: 6966 6669 6375 6c74 7920 2848 502f 5354  ifficulty (HP/ST
-00002620: 522f 4445 4629 2061 7265 3a0d 0a2d 2045  R/DEF) are:..- E
-00002630: 6173 793a 2031 302f 372f 370d 0a2d 204e  asy: 10/7/7..- N
-00002640: 6f72 6d61 6c3a 2031 302f 342f 340d 0a2d  ormal: 10/4/4..-
-00002650: 2048 6172 643a 2038 2f32 2f32 2028 6d61   Hard: 8/2/2 (ma
-00002660: 7820 4850 2033 3529 0d0a 2d20 4578 7472  x HP 35)..- Extr
-00002670: 656d 653a 2036 2f30 2f30 2028 6d61 7820  eme: 6/0/0 (max 
-00002680: 4850 2032 3929 0d0a 0d0a 5570 6772 6164  HP 29)....Upgrad
-00002690: 6573 2063 616e 2062 6520 6163 6365 7373  es can be access
-000026a0: 6564 2062 7920 636c 6561 7269 6e67 2072  ed by clearing r
-000026b0: 6f6f 6d73 2074 6861 7420 6861 7665 2061  ooms that have a
-000026c0: 2022 466f 7263 6522 2069 6e20 7468 656d   "Force" in them
-000026d0: 206f 6e20 7468 6520 7374 6172 7420 6d65   on the start me
-000026e0: 6e75 2e20 2028 4966 2079 6f75 2068 6176  nu.  (If you hav
-000026f0: 6520 7468 6520 426c 6163 6b20 476c 6173  e the Black Glas
-00002700: 7365 7320 6f72 2074 6865 2043 7279 7374  ses or the Cryst
-00002710: 616c 2052 696e 6720 6571 7569 7070 6564  al Ring equipped
-00002720: 2c20 7468 6520 7374 6172 7420 6d65 6e75  , the start menu
-00002730: 2077 696c 6c20 666f 7265 6361 7374 2077   will forecast w
-00002740: 6869 6368 2073 7461 7420 7570 6772 6164  hich stat upgrad
-00002750: 6520 796f 7527 6c6c 2072 6563 6569 7665  e you'll receive
-00002760: 2066 6f72 2063 6c65 6172 696e 6720 6120   for clearing a 
-00002770: 726f 6f6d 2e29 0d0a 0d0a 416c 7465 726e  room.)....Altern
-00002780: 6174 6976 656c 792c 2064 6566 6561 7469  atively, defeati
-00002790: 6e67 2061 2062 6f73 7320 7769 6c6c 2067  ng a boss will g
-000027a0: 7261 6e74 2079 6f75 2061 6e79 2075 6e6f  rant you any uno
-000027b0: 6274 6169 6e65 6420 7570 6772 6164 6573  btained upgrades
-000027c0: 2069 6e20 7468 6520 666f 6c6c 6f77 696e   in the followin
-000027d0: 6720 6475 6e67 656f 6e73 2c20 6279 2062  g dungeons, by b
-000027e0: 6f73 733a 0d0a 2d20 4361 7374 6f74 683a  oss:..- Castoth:
-000027f0: 2055 6e64 6572 6772 6f75 6e64 2054 756e   Underground Tun
-00002800: 6e65 6c20 616e 6420 496e 6361 2052 7569  nel and Inca Rui
-00002810: 6e73 0d0a 2d20 5669 7065 723a 2044 6961  ns..- Viper: Dia
-00002820: 6d6f 6e64 204d 696e 6520 616e 6420 536b  mond Mine and Sk
-00002830: 7920 4761 7264 656e 0d0a 2d20 5661 6d70  y Garden..- Vamp
-00002840: 6972 6573 3a20 4d75 2061 6e64 2041 6e67  ires: Mu and Ang
-00002850: 656c 2044 756e 6765 6f6e 0d0a 2d20 5361  el Dungeon..- Sa
-00002860: 6e64 2046 616e 6765 723a 2047 7265 6174  nd Fanger: Great
-00002870: 2057 616c 6c20 616e 6420 4d74 2e20 4b72   Wall and Mt. Kr
-00002880: 6573 730d 0a2d 204d 756d 6d79 2051 7565  ess..- Mummy Que
-00002890: 656e 3a20 5079 7261 6d69 640d 0a2d 2042  en: Pyramid..- B
-000028a0: 6162 656c 2054 6f77 6572 3a20 416e 6b6f  abel Tower: Anko
-000028b0: 7220 5761 740d 0a0d 0a45 6163 6820 626f  r Wat....Each bo
-000028c0: 7373 2028 616e 642c 2062 7920 6578 7465  ss (and, by exte
-000028d0: 6e73 696f 6e2c 2074 6865 2064 756e 6765  nsion, the dunge
-000028e0: 6f6e 7320 756e 6465 7220 6561 6368 2062  ons under each b
-000028f0: 6f73 7329 2069 7320 6775 6172 616e 7465  oss) is guarante
-00002900: 6564 2074 6f20 6772 616e 7420 6120 746f  ed to grant a to
-00002910: 7461 6c20 6e75 6d62 6572 206f 6620 7570  tal number of up
-00002920: 6772 6164 6573 2062 6173 6564 206f 6e20  grades based on 
-00002930: 6469 6666 6963 756c 7479 3a20 3420 666f  difficulty: 4 fo
-00002940: 7220 4561 7379 2c20 3320 666f 7220 4e6f  r Easy, 3 for No
-00002950: 726d 616c 2c20 3220 666f 7220 4861 7264  rmal, 2 for Hard
-00002960: 2c20 616e 6420 3120 666f 7220 4578 7472  , and 1 for Extr
-00002970: 656d 652e 0d0a 2323 2323 2049 6e2d 4761  eme...#### In-Ga
-00002980: 6d65 2054 7574 6f72 6961 6c0d 0a59 6f75  me Tutorial..You
-00002990: 2063 616e 2073 7065 616b 2074 6f20 7468   can speak to th
-000029a0: 6520 4e50 4320 7374 616e 6469 6e67 2069  e NPC standing i
-000029b0: 6e20 6672 6f6e 7420 6f66 2074 6865 2073  n front of the s
-000029c0: 6368 6f6f 6c20 696e 2053 6f75 7468 2043  chool in South C
-000029d0: 6170 6520 666f 7220 616e 2069 6e2d 6761  ape for an in-ga
-000029e0: 6d65 2074 7574 6f72 6961 6c2e 2020 5468  me tutorial.  Th
-000029f0: 6973 2067 7569 6465 2077 696c 6c20 6265  is guide will be
-00002a00: 2074 6169 6c6f 7265 6420 746f 2074 6865   tailored to the
-00002a10: 2073 6565 6420 7365 7474 696e 6773 2e0d   seed settings..
-00002a20: 0a0d 0a41 6464 6974 696f 6e61 6c6c 792c  ...Additionally,
-00002a30: 2066 6f72 2045 6173 7920 4d6f 6465 2c20   for Easy Mode, 
-00002a40: 656e 7465 7220 7269 6768 742d 6d6f 7374  enter right-most
-00002a50: 2068 6f75 7365 2069 6e20 536f 7574 6820   house in South 
-00002a60: 4361 7065 2066 6f72 2061 6e20 696e 7465  Cape for an inte
-00002a70: 7261 6374 6976 6520 6f76 6572 776f 726c  ractive overworl
-00002a80: 6420 6d61 7020 7468 6174 2061 6c6c 6f77  d map that allow
-00002a90: 7320 796f 7520 746f 2065 7870 6c6f 7265  s you to explore
-00002aa0: 2068 6f77 206d 616e 7920 6974 656d 7320   how many items 
-00002ab0: 616e 6420 4461 726b 2053 7061 6365 7320  and Dark Spaces 
-00002ac0: 6172 6520 6176 6169 6c61 626c 6520 696e  are available in
-00002ad0: 2065 6163 6820 6c6f 6361 7469 6f6e 2c20   each location, 
-00002ae0: 6173 2077 656c 6c20 6173 2074 6865 206e  as well as the n
-00002af0: 756d 6265 7220 6f66 2069 7465 6d73 2079  umber of items y
-00002b00: 6f75 2776 6520 6761 7468 6572 6564 2066  ou've gathered f
-00002b10: 6f72 2065 6163 6820 6c6f 6361 7469 6f6e  or each location
-00002b20: 2e0d 0a23 2323 2320 496e 2d47 616d 6520  ...#### In-Game 
-00002b30: 4869 6e74 730d 0a0d 0a59 6f75 206d 6179  Hints....You may
-00002b40: 2073 7065 616b 2074 6f20 6120 6e75 6d62   speak to a numb
-00002b50: 6572 206f 6620 4e50 4373 2074 6872 6f75  er of NPCs throu
-00002b60: 6768 6f75 7420 7468 6520 6761 6d65 2074  ghout the game t
-00002b70: 6f20 7265 6365 6976 6520 6869 6e74 7320  o receive hints 
-00002b80: 6173 2074 6f20 7468 6520 6c6f 6361 7469  as to the locati
-00002b90: 6f6e 206f 6620 6365 7274 6169 6e20 6b65  on of certain ke
-00002ba0: 7920 6974 656d 7320 696e 2074 6865 2067  y items in the g
-00002bb0: 616d 652c 2061 7320 7765 6c6c 2061 7320  ame, as well as 
-00002bc0: 7468 6520 636f 6e74 656e 7473 206f 6620  the contents of 
-00002bd0: 6365 7274 6169 6e20 6861 7264 2d74 6f2d  certain hard-to-
-00002be0: 7265 6163 6820 6c6f 6361 7469 6f6e 732e  reach locations.
-00002bf0: 2020 5468 6520 666f 6c6c 6f77 696e 6720    The following 
-00002c00: 4e50 4373 2077 696c 6c20 6769 7665 2079  NPCs will give y
-00002c10: 6f75 2061 2068 696e 7420 2868 696e 7473  ou a hint (hints
-00002c20: 2068 6176 6520 6265 656e 2072 656d 6f76   have been remov
-00002c30: 6564 2069 6e20 4578 7472 656d 6520 6469  ed in Extreme di
-00002c40: 6666 6963 756c 7479 293a 0d0a 2d20 4b61  fficulty):..- Ka
-00002c50: 7261 2773 2047 7561 7264 2069 6e20 4564  ra's Guard in Ed
-00002c60: 7761 7264 2773 2043 6173 746c 650d 0a2d  ward's Castle..-
-00002c70: 2054 6865 2045 6c64 6572 2061 7420 4974   The Elder at It
-00002c80: 6f72 7920 5669 6c6c 6167 650d 0a2d 2054  ory Village..- T
-00002c90: 6865 2051 7565 656e 206f 6e20 7468 6520  he Queen on the 
-00002ca0: 476f 6c64 2053 6869 700d 0a2d 2054 6865  Gold Ship..- The
-00002cb0: 206d 616e 2061 7420 4469 616d 6f6e 6420   man at Diamond 
-00002cc0: 436f 6173 740d 0a2d 2054 6865 2065 6d70  Coast..- The emp
-00002cd0: 7479 2063 6f66 6669 6e20 6174 2074 6865  ty coffin at the
-00002ce0: 2053 6561 7369 6465 2050 616c 6163 650d   Seaside Palace.
-00002cf0: 0a2d 2049 7368 7461 7227 7320 4170 7072  .- Ishtar's Appr
-00002d00: 656e 7469 6365 2069 6e20 416e 6765 6c20  entice in Angel 
-00002d10: 5669 6c6c 6167 650d 0a2d 204b 6172 6127  Village..- Kara'
-00002d20: 7320 4a6f 7572 6e61 6c20 696e 2057 6174  s Journal in Wat
-00002d30: 6572 6d69 610d 0a2d 2045 7261 7371 7565  ermia..- Erasque
-00002d40: 7a20 7468 6520 4578 706c 6f72 6572 2069  z the Explorer i
-00002d50: 6e20 4575 726f 0d0a 2d20 5468 6520 7370  n Euro..- The sp
-00002d60: 6972 6974 2061 7420 7468 6520 656e 6420  irit at the end 
-00002d70: 6f66 2041 6e6b 6f72 2057 6174 0d0a 2d20  of Ankor Wat..- 
-00002d80: 5468 6520 6769 726c 2077 6974 6820 4a61  The girl with Ja
-00002d90: 636b 616c 2773 206e 6f74 6520 696e 2044  ckal's note in D
-00002da0: 616f 0d0a 2d20 5468 6520 6669 7273 7420  ao..- The first 
-00002db0: 7370 6972 6974 2069 6e20 4261 6265 6c20  spirit in Babel 
-00002dc0: 546f 7765 720d 0a23 2323 2320 4f74 6865  Tower..#### Othe
-00002dd0: 7220 4665 6174 7572 6573 0d0a 2d20 5468  r Features..- Th
-00002de0: 6520 6c6f 6361 7469 6f6e 206f 6620 7468  e location of th
-00002df0: 6520 676c 6f77 696e 6720 476f 6c64 2054  e glowing Gold T
-00002e00: 696c 6520 696e 2049 6e63 6120 5275 696e  ile in Inca Ruin
-00002e10: 7320 6861 7320 6265 656e 2072 616e 646f  s has been rando
-00002e20: 6d69 7a65 642c 206d 616b 696e 6720 7468  mized, making th
-00002e30: 6520 5769 6e64 204d 656c 6f64 7920 6120  e Wind Melody a 
-00002e40: 7265 7175 6972 656d 656e 7420 746f 2070  requirement to p
-00002e50: 726f 6772 6573 7320 746f 2074 6865 2065  rogress to the e
-00002e60: 6e64 206f 6620 7468 6174 2064 756e 6765  nd of that dunge
-00002e70: 6f6e 2e0d 0a2d 2054 6865 2064 6966 6665  on...- The diffe
-00002e80: 7265 6e63 6573 2062 6574 7765 656e 2074  rences between t
-00002e90: 6865 2070 757a 7a6c 6520 726f 6f6d 7320  he puzzle rooms 
-00002ea0: 696e 2049 7368 7461 7227 7320 5374 7564  in Ishtar's Stud
-00002eb0: 696f 2069 6e20 416e 6765 6c20 5669 6c6c  io in Angel Vill
-00002ec0: 6167 6520 6172 6520 616c 736f 2072 616e  age are also ran
-00002ed0: 646f 6d20 616e 6420 636f 756c 6420 6469  dom and could di
-00002ee0: 6666 6572 2066 726f 6d20 7468 6520 7661  ffer from the va
-00002ef0: 6e69 6c6c 6120 6761 6d65 2e0d 0a2d 2054  nilla game...- T
-00002f00: 6865 206f 7264 6572 206f 6620 7468 6520  he order of the 
-00002f10: 6869 6572 6f67 6c79 7068 7320 696e 2074  hieroglyphs in t
-00002f20: 6865 2050 7972 616d 6964 2068 6173 2062  he Pyramid has b
-00002f30: 6565 6e20 7368 7566 666c 6564 2c20 6d61  een shuffled, ma
-00002f40: 6b69 6e67 2074 6865 2046 6174 6865 7227  king the Father'
-00002f50: 7320 4a6f 7572 6e61 6c20 6120 7265 7175  s Journal a requ
-00002f60: 6972 6564 2069 7465 6d20 746f 2066 6163  ired item to fac
-00002f70: 6520 7468 6520 4d75 6d6d 7920 5175 6565  e the Mummy Quee
-00002f80: 6e2e 2028 596f 7520 6361 6e20 6769 7665  n. (You can give
-00002f90: 2074 6865 2046 6174 6865 7227 7320 4a6f   the Father's Jo
-00002fa0: 7572 6e61 6c20 746f 2074 6865 2067 7569  urnal to the gui
-00002fb0: 6465 2069 6e20 7468 6520 6869 6572 6f67  de in the hierog
-00002fc0: 6c79 7068 2072 6f6f 6d20 6f66 2074 6865  lyph room of the
-00002fd0: 2050 7972 616d 6964 2066 6f72 2073 6166   Pyramid for saf
-00002fe0: 6520 6b65 6570 696e 672e 290d 0a2d 2048  e keeping.)..- H
-00002ff0: 6572 6273 2072 6573 746f 7265 2048 5020  erbs restore HP 
-00003000: 6174 2072 6174 6573 2074 6861 7420 6465  at rates that de
-00003010: 7065 6e64 206f 6e20 7468 6520 6469 6666  pend on the diff
-00003020: 6963 756c 7479 2073 6574 7469 6e67 2c20  iculty setting, 
-00003030: 6569 7468 6572 2066 756c 6c20 7265 7374  either full rest
-00003040: 6f72 6520 2845 6173 7929 2c20 3820 4850  ore (Easy), 8 HP
-00003050: 2028 4e6f 726d 616c 292c 2034 2048 5020   (Normal), 4 HP 
-00003060: 2848 6172 6429 2c20 6f72 2032 2048 5020  (Hard), or 2 HP 
-00003070: 2845 7874 7265 6d65 292e 2020 416e 2048  (Extreme).  An H
-00003080: 5020 4a65 7765 6c20 7769 6c6c 2072 6573  P Jewel will res
-00003090: 746f 7265 2079 6f75 7220 4850 2074 6f20  tore your HP to 
-000030a0: 6675 6c6c 2077 6865 6e20 7573 6564 2069  full when used i
-000030b0: 6e20 4561 7379 206d 6f64 6520 6f6e 6c79  n Easy mode only
-000030c0: 2e0d 0a2d 2055 706f 6e20 6163 7175 6972  ...- Upon acquir
-000030d0: 696e 6720 7468 6520 4175 7261 2c20 6571  ing the Aura, eq
-000030e0: 7569 7020 6974 2061 6e64 2075 7365 2069  uip it and use i
-000030f0: 7420 746f 2075 6e6c 6f63 6b20 5368 6164  t to unlock Shad
-00003100: 6f77 2773 2066 6f72 6d2e 2046 726f 6d20  ow's form. From 
-00003110: 7468 656e 206f 6e2c 2079 6f75 2063 616e  then on, you can
-00003120: 2066 6967 6874 2061 7320 5368 6164 6f77   fight as Shadow
-00003130: 2069 6e20 616e 7920 6475 6e67 656f 6e2e   in any dungeon.
-00003140: 0d0a 2d20 5368 6164 6f77 2773 2066 6f72  ..- Shadow's for
-00003150: 6d20 6d75 7374 2062 6520 756e 6c6f 636b  m must be unlock
-00003160: 6564 2074 6f20 656e 7465 7220 4261 6265  ed to enter Babe
-00003170: 6c20 546f 7765 722c 2061 7320 7765 6c6c  l Tower, as well
-00003180: 2061 7320 6661 6365 2044 6172 6b20 4761   as face Dark Ga
-00003190: 6961 2e0d 0a2d 2049 6620 796f 7520 6272  ia...- If you br
-000031a0: 696e 6720 7468 6520 4e65 636b 6c61 6365  ing the Necklace
-000031b0: 2062 6163 6b20 746f 204c 696c 6c79 2069   back to Lilly i
-000031c0: 6e20 4974 6f72 7920 5669 6c6c 6167 652c  n Itory Village,
-000031d0: 2073 6865 2077 696c 6c20 6163 636f 6d70   she will accomp
-000031e0: 616e 7920 796f 752e 2020 5468 6973 2077  any you.  This w
-000031f0: 696c 6c20 616c 6c6f 7720 796f 7520 746f  ill allow you to
-00003200: 2070 726f 6772 6573 7320 746f 2074 6865   progress to the
-00003210: 2065 6e64 206f 6620 4564 7761 7264 2773   end of Edward's
-00003220: 2055 6e64 6572 6772 6f75 6e64 2054 756e   Underground Tun
-00003230: 6e65 6c2c 2061 7320 7765 6c6c 2061 7320  nel, as well as 
-00003240: 6163 6365 7373 2074 6865 2069 7465 6d20  access the item 
-00003250: 6c6f 636b 6564 2069 6e20 7468 6520 636f  locked in the co
-00003260: 6666 696e 2069 6e20 7468 6520 5365 6173  ffin in the Seas
-00003270: 6964 6520 5061 6c61 6365 2e0d 0a2d 2041  ide Palace...- A
-00003280: 206e 756d 6265 7220 6f66 206e 6577 2069   number of new i
-00003290: 7465 6d73 2068 6176 6520 6265 656e 2061  tems have been a
-000032a0: 6464 6564 2074 6f20 7468 6520 6761 6d65  dded to the game
-000032b0: 2074 6f20 7369 6d75 6c61 7465 2061 6269   to simulate abi
-000032c0: 6c69 7479 2075 7067 7261 6465 732e 2054  lity upgrades. T
-000032d0: 6865 7365 206a 6577 656c 7320 6170 7065  hese jewels appe
-000032e0: 6172 2061 7320 6369 7263 6c65 7320 6f66  ar as circles of
-000032f0: 2066 6c61 6d65 2069 6e20 796f 7572 2069   flame in your i
-00003300: 6e76 656e 746f 7279 2061 6e64 2c20 7768  nventory and, wh
-00003310: 656e 2075 7365 642c 2075 7067 7261 6465  en used, upgrade
-00003320: 2074 6865 2061 7070 726f 7072 6961 7465   the appropriate
-00003330: 2061 6269 6c69 7479 202d 2d20 6569 7468   ability -- eith
-00003340: 6572 2079 6f75 7220 4850 2c20 5354 522c  er your HP, STR,
-00003350: 2044 4546 2c20 5073 7963 686f 2044 6173   DEF, Psycho Das
-00003360: 682c 206f 7220 4461 726b 2046 7269 6172  h, or Dark Friar
-00003370: 2061 6269 6c69 7469 6573 2e20 4974 656d   abilities. Item
-00003380: 7320 7265 7072 6573 656e 7469 6e67 206d  s representing m
-00003390: 756c 7469 706c 6520 5265 6420 4a65 7765  ultiple Red Jewe
-000033a0: 6c73 2061 7265 2068 616e 646c 6564 2073  ls are handled s
-000033b0: 696d 696c 6172 6c79 2061 6e64 206d 7573  imilarly and mus
-000033c0: 7420 6265 2075 7365 6420 2d2d 2074 616c  t be used -- tal
-000033d0: 6b69 6e67 2074 6f20 7468 6520 4a65 7765  king to the Jewe
-000033e0: 6c65 7220 7769 6c6c 206e 6f74 2072 656d  ler will not rem
-000033f0: 6f76 6520 7468 6573 6520 6974 656d 7320  ove these items 
-00003400: 6672 6f6d 2079 6f75 7220 696e 7665 6e74  from your invent
-00003410: 6f72 792e 0d0a 2d20 416e 7920 6261 7272  ory...- Any barr
-00003420: 6965 7220 7468 6174 2063 616e 2062 6520  ier that can be 
-00003430: 7265 6d6f 7665 6420 7769 7468 2074 6865  removed with the
-00003440: 2050 7379 6368 6f20 4461 7368 2063 616e   Psycho Dash can
-00003450: 2061 6c73 6f20 6265 2064 6573 7472 6f79   also be destroy
-00003460: 6564 2077 6974 6820 6569 7468 6572 2074  ed with either t
-00003470: 6865 2050 7379 6368 6f20 536c 6964 6572  he Psycho Slider
-00003480: 206f 7220 7468 6520 5370 696e 2044 6173   or the Spin Das
-00003490: 682e 0d0a 2d20 5468 6520 4461 726b 2053  h...- The Dark S
-000034a0: 7061 6365 7320 696e 2062 6f74 6820 4564  paces in both Ed
-000034b0: 7761 7264 2773 2050 7269 736f 6e20 616e  ward's Prison an
-000034c0: 6420 4261 6265 6c20 546f 7765 7220 6861  d Babel Tower ha
-000034d0: 7665 2062 6565 6e20 7265 6c6f 6361 7465  ve been relocate
-000034e0: 6420 746f 2070 7265 7665 6e74 2073 6f66  d to prevent sof
-000034f0: 746c 6f63 6b73 2e0d 0a2d 2054 6865 2073  tlocks...- The s
-00003500: 7069 7269 7473 2069 6e20 4261 6265 6c20  pirits in Babel 
-00003510: 546f 7765 7220 6361 6e20 7761 7270 2079  Tower can warp y
-00003520: 6f75 2062 6163 6b20 746f 2074 6865 2062  ou back to the b
-00003530: 6f74 746f 6d20 6f66 2074 6865 2074 6f77  ottom of the tow
-00003540: 6572 2c20 616c 6c6f 7769 6e67 2079 6f75  er, allowing you
-00003550: 2074 6f20 6573 6361 7065 2069 6620 796f   to escape if yo
-00003560: 7520 6361 6e6e 6f74 2064 6566 6561 7420  u cannot defeat 
-00003570: 6f6e 6520 6f66 2074 6865 2062 6f73 7365  one of the bosse
-00003580: 732e 0d0a 2d20 596f 7520 6361 6e20 7461  s...- You can ta
-00003590: 6c6b 2074 6f20 7468 6520 4e50 4320 696e  lk to the NPC in
-000035a0: 2066 726f 6e74 206f 6620 7468 6520 7363   front of the sc
-000035b0: 686f 6f6c 2069 6e20 536f 7574 6820 4361  hool in South Ca
-000035c0: 7065 2066 6f72 2061 6e20 696e 2d67 616d  pe for an in-gam
-000035d0: 6520 7475 746f 7269 616c 2e0d 0a0d 0a23  e tutorial.....#
-000035e0: 2323 2320 4d69 7363 2e20 4e6f 7465 7320  ### Misc. Notes 
-000035f0: 616e 6420 5374 7261 7465 6769 6573 0d0a  and Strategies..
-00003600: 2d20 536b 7920 4761 7264 656e 3a20 5468  - Sky Garden: Th
-00003610: 6520 4461 726b 2053 7061 6365 2069 6e20  e Dark Space in 
-00003620: 7468 6520 5357 2072 6f6f 6d20 646f 6573  the SW room does
-00003630: 206e 6f74 2069 6e20 6661 6374 2072 6571   not in fact req
-00003640: 7569 7265 2044 6172 6b20 4672 6961 7220  uire Dark Friar 
-00003650: 746f 2061 6363 6573 732e 2059 6f75 2063  to access. You c
-00003660: 616e 2073 7461 6e64 2062 656c 6f77 2074  an stand below t
-00003670: 6865 2073 7769 7463 6820 6173 2046 7265  he switch as Fre
-00003680: 6564 616e 2061 6e64 2072 6561 6368 2069  edan and reach i
-00003690: 7420 6561 7369 6c79 2077 6974 6820 6869  t easily with hi
-000036a0: 7320 7377 6f72 642e 2041 6c73 6f2c 2079  s sword. Also, y
-000036b0: 6f75 2063 616e 2075 7365 2041 7572 6120  ou can use Aura 
-000036c0: 4261 7272 6965 7220 746f 2063 6f6d 706c  Barrier to compl
-000036d0: 6574 6520 7468 6520 4e57 2072 6f6f 6d20  ete the NW room 
-000036e0: 696e 7374 6561 6420 6f66 2044 6172 6b20  instead of Dark 
-000036f0: 4672 6961 722e 0d0a 0d0a 2d20 4772 6561  Friar.....- Grea
-00003700: 7420 5761 6c6c 3a20 5468 6520 4461 726b  t Wall: The Dark
-00003710: 2053 7061 6365 2077 6865 7265 2053 7069   Space where Spi
-00003720: 6e20 4461 7368 2069 7320 6e6f 726d 616c  n Dash is normal
-00003730: 6c79 2066 6f75 6e64 2c20 6173 2069 7427  ly found, as it'
-00003740: 7320 7468 6520 6f6e 6c79 2044 6172 6b20  s the only Dark 
-00003750: 5370 6163 6520 696e 2074 6861 7420 6172  Space in that ar
-00003760: 6561 2074 6861 7420 6361 6e20 6265 2061  ea that can be a
-00003770: 6363 6573 7365 6420 7769 7468 6f75 7420  ccessed without 
-00003780: 616e 7920 6162 696c 6974 6965 732c 2077  any abilities, w
-00003790: 696c 6c20 6163 7475 616c 6c79 206e 6576  ill actually nev
-000037a0: 6572 2068 6176 6520 616e 2061 6269 6c69  er have an abili
-000037b0: 7479 2061 6e64 2077 696c 6c20 616c 7761  ty and will alwa
-000037c0: 7973 2062 6520 6f70 656e 2066 6f72 2063  ys be open for c
-000037d0: 6861 6e67 696e 6720 666f 726d 732e 2020  hanging forms.  
-000037e0: 5468 6520 4461 726b 2053 7061 6365 2069  The Dark Space i
-000037f0: 6e20 7468 6520 7072 6576 696f 7573 2072  n the previous r
-00003800: 6f6f 6d20 6d69 6768 7420 6861 7665 2061  oom might have a
-00003810: 6e20 6162 696c 6974 792c 2061 6e64 2079  n ability, and y
-00003820: 6f75 2063 616e 2072 6561 6368 2069 7420  ou can reach it 
-00003830: 7769 7468 6f75 7420 5370 696e 2044 6173  without Spin Das
-00003840: 6820 6279 2074 7572 6e69 6e67 2069 6e74  h by turning int
-00003850: 6f20 4672 6565 6461 6e20 6f72 2053 6861  o Freedan or Sha
-00003860: 646f 772c 2077 616c 6b69 6e67 2062 6163  dow, walking bac
-00003870: 6b2c 2061 6e64 2075 7369 6e67 2074 6865  k, and using the
-00003880: 206c 6f6e 6765 7220 7265 6163 6820 6f66   longer reach of
-00003890: 206f 6e65 206f 6620 7468 6573 6520 6368   one of these ch
-000038a0: 6172 6163 7465 7273 2074 6f20 6869 7420  aracters to hit 
-000038b0: 7468 6520 7377 6974 6368 2074 6861 7420  the switch that 
-000038c0: 616c 6c6f 7773 2065 6e74 7261 6e63 6520  allows entrance 
-000038d0: 696e 746f 2074 6861 7420 6d61 702e 0d0a  into that map...
-000038e0: 0d0a 2d20 416e 6b6f 7220 5761 743a 2054  ..- Ankor Wat: T
-000038f0: 6865 2047 6f72 676f 6e20 7468 6174 2062  he Gorgon that b
-00003900: 6c6f 636b 7320 7468 6520 7761 7920 2866  locks the way (f
-00003910: 6f72 2077 6869 6368 2079 6f75 2061 7265  or which you are
-00003920: 2069 6e74 656e 6465 6420 746f 2075 7365   intended to use
-00003930: 2074 6865 2045 6172 7468 7175 616b 6572   the Earthquaker
-00003940: 2920 6361 6e20 6265 2065 6173 696c 7920  ) can be easily 
-00003950: 6465 6665 6174 6564 2069 6620 796f 7520  defeated if you 
-00003960: 6861 7665 2044 6172 6b20 4672 6961 722c  have Dark Friar,
-00003970: 2032 6e64 2075 7067 7261 6465 2c20 6279   2nd upgrade, by
-00003980: 2073 7461 6e64 696e 6720 6f6e 2074 6865   standing on the
-00003990: 2070 6c61 7466 6f72 6d20 616e 6420 7370   platform and sp
-000039a0: 616d 6d69 6e67 2068 696d 2077 6974 6820  amming him with 
-000039b0: 6669 7265 6261 6c6c 7320 6265 666f 7265  fireballs before
-000039c0: 2068 6520 626c 6f63 6b73 2074 6865 2070   he blocks the p
-000039d0: 6173 7361 6765 2e0d 0a0d 0a2d 2041 6e6b  assage.....- Ank
-000039e0: 6f72 2057 6174 3a20 546f 2067 6574 2074  or Wat: To get t
-000039f0: 6f20 7468 6520 4461 726b 2053 7061 6365  o the Dark Space
-00003a00: 2077 6974 6820 7661 6e69 6c6c 6120 4561   with vanilla Ea
-00003a10: 7274 6871 7561 6b65 722c 2079 6f75 2061  rthquaker, you a
-00003a20: 7265 2069 6e74 656e 6465 6420 746f 2068  re intended to h
-00003a30: 6176 6520 4461 726b 2046 7269 6172 2074  ave Dark Friar t
-00003a40: 6f20 6465 6665 6174 2074 6865 2046 7265  o defeat the Fre
-00003a50: 6e7a 7920 7468 6174 206d 6f76 6573 2061  nzy that moves a
-00003a60: 6c6f 6e67 2074 6865 2077 616c 6c20 6163  long the wall ac
-00003a70: 726f 7373 2074 6865 2067 6170 2e20 2048  ross the gap.  H
-00003a80: 6f77 6576 6572 2c20 6966 2079 6f75 2068  owever, if you h
-00003a90: 6176 6520 5368 6164 6f77 2075 6e6c 6f63  ave Shadow unloc
-00003aa0: 6b65 642c 2068 6973 2061 7474 6163 6b20  ked, his attack 
-00003ab0: 6861 7320 656e 6f75 6768 2072 6561 6368  has enough reach
-00003ac0: 2074 6f20 6465 6665 6174 2074 6869 7320   to defeat this 
-00003ad0: 656e 656d 792c 2073 6f20 7468 6973 206d  enemy, so this m
-00003ae0: 6179 2062 6520 7468 6520 696e 7465 6e64  ay be the intend
-00003af0: 6564 2077 6179 2074 6f20 6163 6365 7373  ed way to access
-00003b00: 2074 6861 7420 4461 726b 2053 7061 6365   that Dark Space
-00003b10: 2069 6e20 6120 7261 6e64 6f6d 697a 6564   in a randomized
-00003b20: 2073 6565 642e 0d0a 0d0a 2d20 5079 7261   seed.....- Pyra
-00003b30: 6d69 643a 2052 6f6f 6d20 3320 2874 6865  mid: Room 3 (the
-00003b40: 2022 6b69 6c6c 6572 2036 2220 726f 6f6d   "killer 6" room
-00003b50: 2920 6361 6e20 6265 2064 6f6e 6520 7769  ) can be done wi
-00003b60: 7468 2046 7265 6461 6e20 6966 2079 6f75  th Fredan if you
-00003b70: 2068 6176 6520 4461 726b 2046 7269 6172   have Dark Friar
-00003b80: 2e20 2053 6f6d 6520 6d69 6768 7420 6669  .  Some might fi
-00003b90: 6e64 2074 6869 7320 666f 726d 2074 6f20  nd this form to 
-00003ba0: 6265 2068 656c 7066 756c 2074 6f20 7375  be helpful to su
-00003bb0: 7276 6976 6520 696e 2074 6869 7320 6172  rvive in this ar
-00003bc0: 6561 2c20 6573 7065 6369 616c 6c79 2069  ea, especially i
-00003bd0: 6620 796f 7520 6861 7665 2075 7067 7261  f you have upgra
-00003be0: 6465 6420 4461 726b 2046 7269 6172 2061  ded Dark Friar a
-00003bf0: 6e64 2f6f 7220 4175 7261 2042 6172 7269  nd/or Aura Barri
-00003c00: 6572 2e20 2053 696d 696c 6172 6c79 2c20  er.  Similarly, 
-00003c10: 526f 6f6d 2035 2063 616e 2062 6520 636f  Room 5 can be co
-00003c20: 6d70 6c65 7465 6420 7769 7468 2046 7265  mpleted with Fre
-00003c30: 6564 616e 2069 6620 796f 7520 6861 7665  edan if you have
-00003c40: 2074 6865 2045 6172 7468 7175 616b 6572   the Earthquaker
-00003c50: 2061 6269 6c69 7479 2062 7920 7573 696e   ability by usin
-00003c60: 6720 7468 6174 2061 6269 6c69 7479 2066  g that ability f
-00003c70: 726f 6d20 7468 6520 7661 7269 6f75 7320  rom the various 
-00003c80: 706c 6174 666f 726d 7320 696e 2074 6869  platforms in thi
-00003c90: 7320 6172 6561 2e20 2028 5469 6c65 7320  s area.  (Tiles 
-00003ca0: 7769 6c6c 2066 616c 6c20 6672 6f6d 2074  will fall from t
-00003cb0: 6865 2063 6569 6c69 6e67 2c20 616c 6c6f  he ceiling, allo
-00003cc0: 7769 6e67 2079 6f75 2074 6f20 7072 6f67  wing you to prog
-00003cd0: 7265 7373 2e29 0d0a 0d0a 2323 2320 4974  ress.)....### It
-00003ce0: 656d 2054 7261 636b 6572 0d0a 5468 6572  em Tracker..Ther
-00003cf0: 6520 6973 2061 2073 696d 706c 6520 6974  e is a simple it
-00003d00: 656d 2074 7261 636b 6572 2069 6e63 6c75  em tracker inclu
-00003d10: 6465 6420 7769 7468 2074 6869 7320 7265  ded with this re
-00003d20: 6c65 6173 652e 2020 4f66 6669 6369 616c  lease.  Official
-00003d30: 2074 7261 636b 6572 7320 666f 7220 7468   trackers for th
-00003d40: 6520 6761 6d65 2061 7265 2069 6e20 6465  e game are in de
-00003d50: 7665 6c6f 706d 656e 742e 0d0a 0d0a 2323  velopment.....##
-00003d60: 2320 4675 7475 7265 2052 656c 6561 7365  # Future Release
-00003d70: 730d 0a2d 2045 6e65 6d69 7a65 720d 0a2d  s..- Enemizer..-
-00003d80: 2045 6e74 7261 6e63 6520 7261 6e64 6f6d   Entrance random
-00003d90: 697a 6572 0d0a 2d20 426f 7373 2073 6875  izer..- Boss shu
-00003da0: 6666 6c65 0d0a 2d20 4d6f 7265 2074 6578  ffle..- More tex
-00003db0: 7420 6564 6974 730d 0a0d 0a23 2323 204b  t edits....### K
-00003dc0: 6e6f 776e 2042 7567 7320 616e 6420 5175  nown Bugs and Qu
-00003dd0: 6972 6b73 0d0a 4966 2079 6f75 2068 6176  irks..If you hav
-00003de0: 6520 616e 2069 7373 7565 2077 6974 6820  e an issue with 
-00003df0: 7468 6520 7261 6e64 6f6d 697a 6572 2c20  the randomizer, 
-00003e00: 706c 6561 7365 206a 6f69 6e20 6f75 7220  please join our 
-00003e10: 0d0a 3c61 2068 7265 663d 2268 7474 7073  ..<a href="https
-00003e20: 3a2f 2f64 6973 636f 7264 2e67 672f 4b66  ://discord.gg/Kf
-00003e30: 5a34 5665 4422 3e44 6973 636f 7264 3c2f  Z4VeD">Discord</
-00003e40: 613e 2061 6e64 2072 6570 6f72 7420 796f  a> and report yo
-00003e50: 7572 2069 7373 7565 2069 6e20 7468 6520  ur issue in the 
-00003e60: 2362 7567 7320 6368 616e 6e65 6c2e 0d0a  #bugs channel...
-00003e70: 0d0a 2323 2320 5375 7070 6f72 7420 7468  ..### Support th
-00003e80: 6520 4465 760d 0a4e 6f20 6f6e 6520 646f  e Dev..No one do
-00003e90: 6573 2061 2070 726f 6a65 6374 206c 696b  es a project lik
-00003ea0: 6520 7468 6973 2066 6f72 2074 6865 206d  e this for the m
-00003eb0: 6f6e 6579 202d 2d20 4920 6c6f 7665 2074  oney -- I love t
-00003ec0: 6869 7320 6761 6d65 2c20 7761 6e74 6564  his game, wanted
-00003ed0: 2061 2072 616e 646f 6d69 7a65 7220 746f   a randomizer to
-00003ee0: 2065 7869 7374 2066 6f72 2069 742c 2061   exist for it, a
-00003ef0: 6e64 2068 6164 2061 2062 6c61 7374 206d  nd had a blast m
-00003f00: 616b 696e 6720 6f6e 652e 2020 4920 6e65  aking one.  I ne
-00003f10: 6974 6865 7220 6e65 6564 206e 6f72 2065  ither need nor e
-00003f20: 7870 6563 7420 616e 7920 636f 6d70 656e  xpect any compen
-00003f30: 7361 7469 6f6e 2066 6f72 206d 7920 776f  sation for my wo
-00003f40: 726b 202d 2d20 4920 686f 7065 2079 6f75  rk -- I hope you
-00003f50: 2065 6e6a 6f79 2069 742c 206e 6f20 7374   enjoy it, no st
-00003f60: 7269 6e67 7320 6174 7461 6368 6564 2e20  rings attached. 
-00003f70: 2048 6f77 6576 6572 2c20 6966 2079 6f75   However, if you
-00003f80: 2066 6565 6c20 636f 6d70 656c 6c65 6420   feel compelled 
-00003f90: 746f 2073 7570 706f 7274 206d 6520 666f  to support me fo
-00003fa0: 7220 7468 6973 2070 726f 6a65 6374 2028  r this project (
-00003fb0: 6f72 2069 6620 796f 7527 6420 6c69 6b65  or if you'd like
-00003fc0: 2074 6f20 7365 6520 6d6f 7265 2067 616d   to see more gam
-00003fd0: 652d 6d6f 6464 696e 6720 6672 6f6d 206d  e-modding from m
-00003fe0: 6529 2c20 4920 6875 6d62 6c79 2069 6e76  e), I humbly inv
-00003ff0: 6974 6520 796f 7520 746f 2063 6f6e 7369  ite you to consi
-00004000: 6465 7220 6265 636f 6d69 6e67 2061 200d  der becoming a .
-00004010: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
-00004020: 2f2f 7777 772e 7061 7472 656f 6e2e 636f  //www.patreon.co
-00004030: 6d2f 646f 6e74 6261 6775 6d65 223e 7061  m/dontbagume">pa
-00004040: 7472 6f6e 2e3c 2f61 3e0d 0a              tron.</a>..
+00000000: 7630 2e38 0d0a 4348 414e 4745 533a 0d0a  v0.8..CHANGES:..
+00000010: 3129 2054 6865 2069 6e2d 6761 6d65 2074  1) The in-game t
+00000020: 7574 6f72 6961 6c20 6e6f 7720 6368 616e  utorial now chan
+00000030: 6765 7320 6465 7065 6e64 696e 6720 6f6e  ges depending on
+00000040: 2074 6865 2067 616d 6520 676f 616c 2e0d   the game goal..
+00000050: 0a0d 0a76 302e 370d 0a43 4841 4e47 4553  ...v0.7..CHANGES
+00000060: 3a0d 0a31 2920 4e65 7720 6d6f 6465 7320  :..1) New modes 
+00000070: 6176 6169 6c61 626c 6520 7570 6f6e 2073  available upon s
+00000080: 6565 6420 6765 6e65 7261 7469 6f6e 3a0d  eed generation:.
+00000090: 0a2d 2047 6f61 6c3a 2043 616e 206e 6f77  .- Goal: Can now
+000000a0: 2062 6520 2244 6172 6b20 4761 6961 2220   be "Dark Gaia" 
+000000b0: 6f72 2022 5265 6420 4a65 7765 6c20 4875  or "Red Jewel Hu
+000000c0: 6e74 222e 2049 6e20 7468 6520 6c61 7474  nt". In the latt
+000000d0: 6572 2c20 796f 7520 6265 6174 2074 6865  er, you beat the
+000000e0: 2067 616d 6520 6279 2063 6f6c 6c65 6374   game by collect
+000000f0: 696e 6720 6120 6e75 6d62 6572 206f 6620  ing a number of 
+00000100: 5265 6420 4a65 7765 6c73 2028 3335 2066  Red Jewels (35 f
+00000110: 6f72 2045 6173 792c 2034 3020 666f 7220  or Easy, 40 for 
+00000120: 4e6f 726d 616c 2c20 616e 6420 3530 2066  Normal, and 50 f
+00000130: 6f72 2048 6172 642f 4578 7472 656d 6529  or Hard/Extreme)
+00000140: 2061 6e64 2074 616c 6b69 6e67 2074 6f20   and talking to 
+00000150: 7468 6520 4a65 7765 6c65 722e 0d0a 2d20  the Jeweler...- 
+00000160: 4c6f 6769 633a 2022 436f 6d70 6c65 7461  Logic: "Completa
+00000170: 626c 6522 206d 6561 6e73 2069 7420 6973  ble" means it is
+00000180: 2070 6f73 7369 626c 6520 746f 2061 6363   possible to acc
+00000190: 6573 7320 6576 6572 7920 6974 656d 2069  ess every item i
+000001a0: 6e20 7468 6520 6761 6d65 2e20 2242 6561  n the game. "Bea
+000001b0: 7461 626c 6522 206d 6561 6e73 2073 6f6d  table" means som
+000001c0: 6520 6974 656d 7320 6d61 7920 6265 2069  e items may be i
+000001d0: 6e61 6365 7373 6962 6c65 2c20 6275 7420  nacessible, but 
+000001e0: 796f 7520 6172 6520 6775 6172 616e 7465  you are guarante
+000001f0: 6564 2074 6f20 6265 2061 626c 6520 746f  ed to be able to
+00000200: 2066 756c 6669 6c6c 2074 6865 206f 626a   fulfill the obj
+00000210: 6563 7469 7665 7320 6f66 2074 6865 2073  ectives of the s
+00000220: 6565 642e 0d0a 3229 2041 6c6c 2072 6577  eed...2) All rew
+00000230: 6172 6473 2028 4850 2c20 4445 4620 616e  ards (HP, DEF an
+00000240: 6420 5354 5229 2061 7265 2061 7661 696c  d STR) are avail
+00000250: 6162 6c65 2074 6872 6f75 6768 2063 6c65  able through cle
+00000260: 6172 696e 6720 726f 6f6d 732e 0d0a 3329  aring rooms...3)
+00000270: 2048 5020 7265 7761 7264 7320 6772 616e   HP rewards gran
+00000280: 7420 796f 7520 2b33 2048 5020 6561 6368  t you +3 HP each
+00000290: 0d0a 3429 2054 6865 2072 6577 6172 6473  ..4) The rewards
+000002a0: 2061 7265 2073 6875 6666 6c65 6420 6174   are shuffled at
+000002b0: 2072 616e 646f 6d20 7468 726f 7567 686f   random througho
+000002c0: 7574 2074 6865 2065 6e74 6972 6520 6761  ut the entire ga
+000002d0: 6d65 2c20 6d61 7020 6279 206d 6170 2e20  me, map by map. 
+000002e0: 2054 6865 2074 6f74 616c 2072 6577 6172   The total rewar
+000002f0: 6473 2061 7661 696c 6162 6c65 2062 7920  ds available by 
+00000300: 6469 6666 6963 756c 7479 2028 4850 2f53  difficulty (HP/S
+00000310: 5452 2f44 4546 2920 6172 653a 0d0a 2d20  TR/DEF) are:..- 
+00000320: 4561 7379 3a20 3130 2f37 2f37 0d0a 2d20  Easy: 10/7/7..- 
+00000330: 4e6f 726d 616c 3a20 3130 2f34 2f34 0d0a  Normal: 10/4/4..
+00000340: 2d20 4861 7264 3a20 382f 322f 3220 286d  - Hard: 8/2/2 (m
+00000350: 6178 2048 5020 3335 290d 0a2d 2045 7874  ax HP 35)..- Ext
+00000360: 7265 6d65 3a20 362f 302f 3020 286d 6178  reme: 6/0/0 (max
+00000370: 2048 5020 3239 290d 0a35 2920 596f 7520   HP 29)..5) You 
+00000380: 7769 6c6c 206e 6f77 2067 6169 6e20 6120  will now gain a 
+00000390: 7265 7761 7264 2066 6f72 2064 6566 6561  reward for defea
+000003a0: 7469 6e67 204d 756d 6d79 2051 7565 656e  ting Mummy Queen
+000003b0: 2061 7420 7468 6520 746f 7020 6f66 2042   at the top of B
+000003c0: 6162 656c 2054 6f77 6572 2e20 2054 6865  abel Tower.  The
+000003d0: 2072 6577 6172 6473 2067 6174 6865 7265   rewards gathere
+000003e0: 6420 6279 2065 6163 6820 626f 7373 2061  d by each boss a
+000003f0: 7265 206e 6f77 2061 7320 666f 6c6c 6f77  re now as follow
+00000400: 733a 0d0a 2d20 4361 7374 6f74 683a 2055  s:..- Castoth: U
+00000410: 6e64 6572 6772 6f75 6e64 2054 756e 6e65  nderground Tunne
+00000420: 6c20 616e 6420 496e 6361 2028 6e6f 2063  l and Inca (no c
+00000430: 6861 6e67 6529 0d0a 2d20 5669 7065 723a  hange)..- Viper:
+00000440: 2044 6961 6d6f 6e64 204d 696e 6520 616e   Diamond Mine an
+00000450: 6420 536b 7920 4761 7264 656e 2028 6e6f  d Sky Garden (no
+00000460: 2063 6861 6e67 6529 0d0a 2d20 5661 6d70   change)..- Vamp
+00000470: 6972 6573 3a20 4d75 2061 6e64 2041 6e67  ires: Mu and Ang
+00000480: 656c 2044 756e 6765 6f6e 0d0a 2d20 5361  el Dungeon..- Sa
+00000490: 6e64 2046 616e 6765 723a 2047 7265 6174  nd Fanger: Great
+000004a0: 2057 616c 6c20 616e 6420 4d74 2e20 4b72   Wall and Mt. Kr
+000004b0: 6573 730d 0a2d 204d 756d 6d79 2051 7565  ess..- Mummy Que
+000004c0: 656e 3a20 5079 7261 6d69 640d 0a2d 2042  en: Pyramid..- B
+000004d0: 6162 656c 2054 6f77 6572 3a20 416e 6b6f  abel Tower: Anko
+000004e0: 7220 5761 740d 0a36 2920 5468 6520 6361  r Wat..6) The ca
+000004f0: 7074 6169 6e20 6f66 2074 6865 2047 6f6c  ptain of the Gol
+00000500: 6420 5368 6970 2063 616e 2062 6520 666f  d Ship can be fo
+00000510: 756e 6420 6174 2074 6865 2065 6e74 7261  und at the entra
+00000520: 6e63 6520 746f 2049 6e63 6120 5275 696e  nce to Inca Ruin
+00000530: 732e 2020 4966 2079 6f75 2068 6176 6520  s.  If you have 
+00000540: 6465 6665 6174 6564 2043 6173 746f 7468  defeated Castoth
+00000550: 2c20 796f 7520 6361 6e20 7461 6c6b 2074  , you can talk t
+00000560: 6f20 6869 6d20 666f 7220 696e 7374 616e  o him for instan
+00000570: 7420 7061 7373 6167 6520 746f 2074 6865  t passage to the
+00000580: 2044 6961 6d6f 6e64 2043 6f61 7374 2e0d   Diamond Coast..
+00000590: 0a37 2920 5468 6572 6520 6973 206e 6f77  .7) There is now
+000005a0: 2061 6e20 696e 2d67 616d 6520 7475 746f   an in-game tuto
+000005b0: 7269 616c 2074 6861 7420 796f 7520 6361  rial that you ca
+000005c0: 6e20 6765 7420 6672 6f6d 2074 6865 204e  n get from the N
+000005d0: 5043 2069 6e20 6672 6f6e 7420 6f66 2074  PC in front of t
+000005e0: 6865 2073 6368 6f6f 6c20 696e 2053 6f75  he school in Sou
+000005f0: 7468 2043 6170 652e 0d0a 0d0a 4255 4720  th Cape.....BUG 
+00000600: 4649 5845 533a 0d0a 2d20 5765 6972 6420  FIXES:..- Weird 
+00000610: 6368 6172 6163 7465 7273 2074 6861 7420  characters that 
+00000620: 7368 6f77 2075 7020 7768 656e 2079 6f75  show up when you
+00000630: 2072 6561 6420 4c6f 6c61 2773 204c 6574   read Lola's Let
+00000640: 7465 7220 6861 7665 2062 6565 6e20 7265  ter have been re
+00000650: 6d6f 7665 642e 0d0a 2d20 5468 6520 7370  moved...- The sp
+00000660: 6563 6961 6c20 6162 696c 6974 6965 7320  ecial abilities 
+00000670: 666f 7220 5769 6c6c 2061 6e64 2046 7265  for Will and Fre
+00000680: 6564 616e 206e 6f77 2077 6f72 6b20 636f  edan now work co
+00000690: 7272 6563 746c 7920 616e 6420 696e 6465  rrectly and inde
+000006a0: 7065 6e64 656e 746c 792e 0d0a 2d20 596f  pendently...- Yo
+000006b0: 7520 6d69 6768 7420 7374 696c 6c20 6765  u might still ge
+000006c0: 7420 736f 6674 6c6f 636b 6564 2069 6e20  t softlocked in 
+000006d0: 4469 616d 6f6e 6420 4d69 6e65 2062 7920  Diamond Mine by 
+000006e0: 6174 7465 6d70 7469 6e67 2074 6f20 7265  attempting to re
+000006f0: 7363 7565 2074 6865 2074 7261 7070 6564  scue the trapped
+00000700: 206c 6162 6f72 6572 2077 6974 6820 536c   laborer with Sl
+00000710: 6964 6572 206f 7220 5370 696e 202d 2d20  ider or Spin -- 
+00000720: 686f 7765 7665 722c 206c 6f67 6963 2068  however, logic h
+00000730: 6173 2062 6565 6e20 7570 6461 7465 6420  as been updated 
+00000740: 7375 6368 2074 6861 7420 5073 7963 686f  such that Psycho
+00000750: 2044 6173 6820 6973 2072 6571 7569 7265   Dash is require
+00000760: 6420 746f 2061 6371 7569 7265 2074 6869  d to acquire thi
+00000770: 7320 6974 656d 2e20 5365 7175 656e 6365  s item. Sequence
+00000780: 2062 7265 616b 2061 7420 796f 7572 206f   break at your o
+00000790: 776e 2072 6973 6b2e 0d0a 2d20 5468 6520  wn risk...- The 
+000007a0: 6275 6720 7468 6174 2061 6c6c 6f77 6564  bug that allowed
+000007b0: 2079 6f75 2074 6f20 7265 6d61 696e 2061   you to remain a
+000007c0: 7320 4672 6565 6461 6e2f 5368 6164 6f77  s Freedan/Shadow
+000007d0: 206f 7574 206f 6620 556e 6465 7267 726f   out of Undergro
+000007e0: 756e 6420 5475 6e6e 656c 2068 6173 2062  und Tunnel has b
+000007f0: 6565 6e20 6669 7865 642e 0d0a 2d20 5468  een fixed...- Th
+00000800: 6520 7465 7874 2062 6f78 2061 7373 6f63  e text box assoc
+00000810: 6961 7465 6420 7769 7468 2074 6865 2074  iated with the t
+00000820: 776f 2069 7465 6d73 2079 6f75 2067 6574  wo items you get
+00000830: 2066 726f 6d20 7468 6520 6d61 6e20 696e   from the man in
+00000840: 2044 616f 206e 6f77 2064 6973 706c 6179   Dao now display
+00000850: 2074 6865 2063 6f72 7265 6374 2069 7465   the correct ite
+00000860: 6d73 2e0d 0a2d 2054 6865 2062 7567 2077  ms...- The bug w
+00000870: 6865 7265 2056 616d 7069 7265 7320 776f  here Vampires wo
+00000880: 756c 6420 6e6f 7420 6761 7468 6572 2061  uld not gather a
+00000890: 6c6c 2074 6865 6972 2075 7067 7261 6465  ll their upgrade
+000008a0: 7320 6861 7320 6265 656e 2066 6978 6564  s has been fixed
+000008b0: 2e0d 0a2d 2053 7069 7269 7473 2069 6e20  ...- Spirits in 
+000008c0: 4261 6265 6c20 6861 7665 2062 6565 6e20  Babel have been 
+000008d0: 6469 7374 7269 6275 7465 6420 746f 2064  distributed to d
+000008e0: 6966 6665 7265 6e74 2066 6c6f 6f72 732c  ifferent floors,
+000008f0: 2074 6f20 616c 6c6f 7720 7761 7270 7320   to allow warps 
+00000900: 6966 2079 6f75 2063 616e 6e6f 7420 6465  if you cannot de
+00000910: 6665 6174 2062 6f73 7365 732e 0d0a 2d20  feat bosses...- 
+00000920: 4b61 7261 2773 2070 6f72 7472 6169 7420  Kara's portrait 
+00000930: 7769 6c6c 206e 6f77 2064 6973 6170 7065  will now disappe
+00000940: 6172 2077 6865 6e20 796f 7520 7573 6520  ar when you use 
+00000950: 7468 6520 4d61 6769 6320 4475 7374 206f  the Magic Dust o
+00000960: 6e20 6974 2e0d 0a2d 2054 6865 2045 7572  n it...- The Eur
+00000970: 6f20 6d61 7020 676c 6974 6368 2068 6173  o map glitch has
+00000980: 2062 6565 6e20 6669 7865 642e 0d0a 2d20   been fixed...- 
+00000990: 4974 6f72 7920 656c 6465 7220 6861 7320  Itory elder has 
+000009a0: 6265 656e 2066 6978 6564 2074 6f20 616c  been fixed to al
+000009b0: 7761 7973 2070 726f 7669 6465 2061 2073  ways provide a s
+000009c0: 706f 696c 6572 2e0d 0a2d 2044 7969 6e67  poiler...- Dying
+000009d0: 2074 6f20 7468 6520 5661 6d70 6972 6573   to the Vampires
+000009e0: 2069 6e20 4d75 2073 656e 6473 2079 6f75   in Mu sends you
+000009f0: 2062 6163 6b20 6f6e 6520 7363 7265 656e   back one screen
+00000a00: 2c20 696e 7374 6561 6420 6f66 2062 6163  , instead of bac
+00000a10: 6b20 746f 2074 6865 2062 6567 696e 6e69  k to the beginni
+00000a20: 6e67 206f 6620 7468 6520 6475 6e67 656f  ng of the dungeo
+00000a30: 6e2e 0d0a 2d20 5768 656e 2061 7070 726f  n...- When appro
+00000a40: 6163 6869 6e67 2074 6865 2067 7561 7264  aching the guard
+00000a50: 2062 6c6f 636b 696e 6720 7468 6520 7761   blocking the wa
+00000a60: 7920 6672 6f6d 2074 6865 2055 6e64 6572  y from the Under
+00000a70: 6772 6f75 6e64 2054 756e 6e65 6c2c 2079  ground Tunnel, y
+00000a80: 6f75 206e 6f20 6c6f 6e67 6572 2068 6176  ou no longer hav
+00000a90: 6520 746f 2062 6520 6167 6169 6e73 7420  e to be against 
+00000aa0: 7468 6520 746f 7020 7761 6c6c 2e0d 0a2d  the top wall...-
+00000ab0: 2056 6172 696f 7573 204e 5043 2064 6961   Various NPC dia
+00000ac0: 6c6f 6775 6520 6861 7320 6265 656e 2066  logue has been f
+00000ad0: 6978 6564 2e0d 0a0d 0a76 302e 360d 0a43  ixed.....v0.6..C
+00000ae0: 4841 4e47 4553 3a0d 0a2d 2054 6865 2072  HANGES:..- The r
+00000af0: 616e 646f 6d69 7a65 7220 6973 206e 6f77  andomizer is now
+00000b00: 2072 756e 2061 7320 6120 7374 616e 642d   run as a stand-
+00000b10: 616c 6f6e 6520 6578 6563 7574 6162 6c65  alone executable
+00000b20: 2077 6974 6820 6120 4755 4920 736f 2075   with a GUI so u
+00000b30: 7365 7273 2063 616e 2067 656e 6572 6174  sers can generat
+00000b40: 6520 7468 6569 7220 6f77 6e20 7365 6564  e their own seed
+00000b50: 732e 0d0a 2d20 5468 6520 6761 6d65 206e  s...- The game n
+00000b60: 6f77 2068 6176 6520 666f 7572 2064 6966  ow have four dif
+00000b70: 6669 6375 6c74 7920 6d6f 6465 733a 2045  ficulty modes: E
+00000b80: 6173 792c 204e 6f72 6d61 6c2c 2048 6172  asy, Normal, Har
+00000b90: 642c 2061 6e64 2045 7874 7265 6d65 2e20  d, and Extreme. 
+00000ba0: 5468 6520 6469 6666 6963 756c 7479 2061  The difficulty a
+00000bb0: 6666 6563 7473 2065 6e65 6d79 2073 7461  ffects enemy sta
+00000bc0: 7473 2c20 7570 6772 6164 6573 2061 7661  ts, upgrades ava
+00000bd0: 696c 6162 6c65 2c20 616e 6420 686f 7720  ilable, and how 
+00000be0: 6d61 6e79 2048 5020 6172 6520 7265 636f  many HP are reco
+00000bf0: 7665 7265 6420 6672 6f6d 2065 6174 696e  vered from eatin
+00000c00: 6720 6865 7262 732e 0d0a 2d20 526f 6f6d  g herbs...- Room
+00000c10: 2072 6577 6172 6473 2061 7265 2067 7561   rewards are gua
+00000c20: 7261 6e74 6565 6420 746f 2064 726f 7020  ranteed to drop 
+00000c30: 6569 7468 6572 2061 2053 5452 206f 7220  either a STR or 
+00000c40: 4445 4620 7570 6772 6164 652e 2020 4850  DEF upgrade.  HP
+00000c50: 2075 7067 7261 6465 7320 6172 6520 6176   upgrades are av
+00000c60: 6169 6c61 626c 6520 6672 6f6d 2062 6561  ailable from bea
+00000c70: 7469 6e67 2062 6f73 7365 732e 2020 5365  ting bosses.  Se
+00000c80: 6520 7468 6520 7475 746f 7269 616c 2066  e the tutorial f
+00000c90: 6f72 206d 6f72 6520 6465 7461 696c 6564  or more detailed
+00000ca0: 2069 6e66 6f72 6d61 7469 6f6e 2e0d 0a2d   information...-
+00000cb0: 2054 6865 2044 6172 6b20 5370 6163 6520   The Dark Space 
+00000cc0: 696e 2053 5720 536b 7920 4761 7264 656e  in SW Sky Garden
+00000cd0: 2063 616e 206e 6f77 2063 6f6e 7461 696e   can now contain
+00000ce0: 2044 6172 6b20 4672 6961 722e 2028 596f   Dark Friar. (Yo
+00000cf0: 7520 6361 6e20 7374 616e 6420 6265 6c6f  u can stand belo
+00000d00: 7720 7468 6520 7377 6974 6368 2061 6e64  w the switch and
+00000d10: 2072 6561 6368 2069 7420 7769 7468 2046   reach it with F
+00000d20: 7265 6461 6e27 7320 7377 6f72 642c 2073  redan's sword, s
+00000d30: 6f20 4461 726b 2046 7269 6172 2069 7320  o Dark Friar is 
+00000d40: 6e6f 7420 7265 7175 6972 6564 2074 6f20  not required to 
+00000d50: 7265 6163 6820 7468 6973 2044 6172 6b20  reach this Dark 
+00000d60: 5370 6163 6520 6173 2077 6173 206f 7269  Space as was ori
+00000d70: 6769 6e61 6c6c 7920 6173 7375 6d65 642e  ginally assumed.
+00000d80: 290d 0a2d 2043 7279 7374 616c 2052 696e  )..- Crystal Rin
+00000d90: 6720 616e 6420 4175 7261 2061 7265 206e  g and Aura are n
+00000da0: 6f77 2062 6f74 6820 7265 7175 6972 6564  ow both required
+00000db0: 2074 6f20 656e 7465 7220 4261 6265 6c20   to enter Babel 
+00000dc0: 546f 7765 722e 0d0a 2d20 4461 726b 2046  Tower...- Dark F
+00000dd0: 7269 6172 2069 7320 6e6f 7720 636f 6e73  riar is now cons
+00000de0: 6964 6572 6564 2061 7320 7265 7175 6972  idered as requir
+00000df0: 6564 2066 6f72 2070 726f 6772 6573 7369  ed for progressi
+00000e00: 6f6e 2074 6872 6f75 6768 204d 752e 2020  on through Mu.  
+00000e10: 5468 6973 206d 6561 6e73 2074 6865 2066  This means the f
+00000e20: 6972 7374 2044 6172 6b20 5370 6163 6520  irst Dark Space 
+00000e30: 7769 6c6c 2061 6c77 6179 7320 6265 206f  will always be o
+00000e40: 7065 6e20 666f 7220 7472 616e 7366 6f72  pen for transfor
+00000e50: 6d61 7469 6f6e 2c20 616e 6420 7468 6520  mation, and the 
+00000e60: 6f74 6865 7220 4461 726b 2053 7061 6365  other Dark Space
+00000e70: 2077 696c 6c20 6e65 7665 7220 636f 6e74   will never cont
+00000e80: 6169 6e20 4461 726b 2046 7269 6172 2e0d  ain Dark Friar..
+00000e90: 0a0d 0a4b 4e4f 574e 2042 5547 5320 4e4f  ...KNOWN BUGS NO
+00000ea0: 5420 5945 5420 4144 4452 4553 5345 443a  T YET ADDRESSED:
+00000eb0: 0d0a 2d20 4b61 7261 2773 2070 6f72 7472  ..- Kara's portr
+00000ec0: 6169 7420 7175 6573 7420 6973 2063 6f6d  ait quest is com
+00000ed0: 706c 6574 6520 7768 656e 2074 6865 204d  plete when the M
+00000ee0: 6167 6963 2044 7573 7420 6973 2073 7563  agic Dust is suc
+00000ef0: 6365 7373 6675 6c6c 7920 7573 6564 2e20  cessfully used. 
+00000f00: 204b 6172 6127 7320 706f 7274 7261 6974   Kara's portrait
+00000f10: 2077 696c 6c20 7265 6d61 696e 206f 6e20   will remain on 
+00000f20: 7468 6520 7363 7265 656e 2065 7665 6e20  the screen even 
+00000f30: 6166 7465 7220 7368 6520 6973 2066 7265  after she is fre
+00000f40: 6564 2077 6974 6820 7468 6520 4d61 6769  ed with the Magi
+00000f50: 6320 4475 7374 2e20 204c 6561 7669 6e67  c Dust.  Leaving
+00000f60: 2061 6e64 2072 6565 6e74 6572 696e 6720   and reentering 
+00000f70: 7468 6520 726f 6f6d 2077 696c 6c20 7072  the room will pr
+00000f80: 6f76 6964 6520 7669 7375 616c 2063 6f6e  ovide visual con
+00000f90: 6669 726d 6174 696f 6e20 7468 6174 2073  firmation that s
+00000fa0: 6865 2068 6173 2062 6565 6e20 6672 6565  he has been free
+00000fb0: 6420 2d2d 2068 6f77 6576 6572 2c20 7468  d -- however, th
+00000fc0: 6973 2069 7320 756e 6e65 6365 7373 6172  is is unnecessar
+00000fd0: 7920 746f 2063 6f6d 706c 6574 6520 7468  y to complete th
+00000fe0: 6520 7175 6573 742e 0d0a 2d20 5768 656e  e quest...- When
+00000ff0: 204b 6172 6127 7320 2270 6f72 7472 6169   Kara's "portrai
+00001000: 7422 2061 7070 6561 7273 2069 6e20 7468  t" appears in th
+00001010: 6520 4469 616d 6f6e 6420 4d69 6e65 2c20  e Diamond Mine, 
+00001020: 7368 6520 7769 6c6c 206c 6f6f 6b20 6c69  she will look li
+00001030: 6b65 2068 6572 206e 6f72 6d61 6c20 7370  ke her normal sp
+00001040: 7269 7465 2069 6e73 7465 6164 206f 6620  rite instead of 
+00001050: 6c69 6b65 2074 6865 2070 6f72 7472 6169  like the portrai
+00001060: 7420 6974 7365 6c66 2e20 4920 686f 7065  t itself. I hope
+00001070: 2074 6f20 6669 6e64 2061 2073 6f6c 7574   to find a solut
+00001080: 696f 6e20 666f 7220 7468 6973 2069 7373  ion for this iss
+00001090: 7565 2069 6e20 6675 7475 7265 2076 6572  ue in future ver
+000010a0: 7369 6f6e 732e 0d0a 2d20 4c65 6176 696e  sions...- Leavin
+000010b0: 6720 7468 6520 4a65 7765 6c65 7227 7320  g the Jeweler's 
+000010c0: 4d61 6e73 696f 6e20 616e 6420 696d 6d65  Mansion and imme
+000010d0: 6469 6174 656c 7920 7265 656e 7465 7269  diately reenteri
+000010e0: 6e67 2076 6961 2044 616f 2063 6175 7365  ng via Dao cause
+000010f0: 7320 7468 6520 746f 7020 6c61 7965 7220  s the top layer 
+00001100: 746f 206c 6f6f 6b20 7374 7261 6e67 652e  to look strange.
+00001110: 0d0a 2d20 4163 7175 6972 696e 6720 4561  ..- Acquiring Ea
+00001120: 7274 6871 7561 6b65 7220 7374 696c 6c20  rthquaker still 
+00001130: 6772 616e 7473 2079 6f75 2044 6172 6b20  grants you Dark 
+00001140: 4672 6961 720d 0a2d 2041 7572 6120 4261  Friar..- Aura Ba
+00001150: 7272 6965 7220 7769 6c6c 206e 6f74 2077  rrier will not w
+00001160: 6f72 6b20 756e 6c65 7373 2079 6f75 2068  ork unless you h
+00001170: 6176 6520 4461 726b 2046 7269 6172 0d0a  ave Dark Friar..
+00001180: 0d0a 0d0a 7630 2e35 0d0a 4348 414e 4745  ....v0.5..CHANGE
+00001190: 533a 0d0a 2d20 5769 6c6c 206e 6f77 2073  S:..- Will now s
+000011a0: 7461 7274 7320 7769 7468 2073 7461 6e64  tarts with stand
+000011b0: 6172 6420 6865 616c 7468 2c20 6465 6665  ard health, defe
+000011c0: 6e73 652c 2061 6e64 2073 7472 656e 6774  nse, and strengt
+000011d0: 682e 0d0a 2d20 5468 6520 6e75 6d62 6572  h...- The number
+000011e0: 206f 6620 746f 7461 6c20 726f 6f6d 2d63   of total room-c
+000011f0: 6c65 6172 696e 6720 7374 6174 7573 2075  learing status u
+00001200: 7067 7261 6465 7320 6861 7665 2062 6565  pgrades have bee
+00001210: 6e20 6164 6a75 7374 6564 2061 6e64 2073  n adjusted and s
+00001220: 6875 6666 6c65 6420 7468 726f 7567 686f  huffled througho
+00001230: 7574 2074 6865 206d 6170 7320 696e 2074  ut the maps in t
+00001240: 6865 2067 616d 652e 2020 5468 6520 6e75  he game.  The nu
+00001250: 6d62 6572 206f 6620 6865 616c 7468 2075  mber of health u
+00001260: 7067 7261 6465 7320 6861 7320 7265 6d61  pgrades has rema
+00001270: 696e 6564 2074 6865 2073 616d 6520 6672  ined the same fr
+00001280: 6f6d 2076 616e 696c 6c61 3b20 7468 6520  om vanilla; the 
+00001290: 6e75 6d62 6572 206f 6620 5354 5220 616e  number of STR an
+000012a0: 6420 4445 4620 7570 6772 6164 6573 2068  d DEF upgrades h
+000012b0: 6176 6520 6265 656e 2072 6f75 6768 6c79  ave been roughly
+000012c0: 2068 616c 7665 642e 2020 5468 6973 206d   halved.  This m
+000012d0: 6561 6e73 2074 6861 7420 736f 6d65 2072  eans that some r
+000012e0: 6f6f 6d73 2074 6861 7420 6e6f 726d 616c  ooms that normal
+000012f0: 6c79 2067 6976 6520 7265 7761 7264 7320  ly give rewards 
+00001300: 7769 6c6c 206e 6f74 2067 6976 6520 7265  will not give re
+00001310: 7761 7264 733b 2079 6f75 2063 616e 2063  wards; you can c
+00001320: 6865 636b 2074 6865 2073 7461 7274 2073  heck the start s
+00001330: 6372 6565 6e20 746f 2073 6565 2069 6620  creen to see if 
+00001340: 6120 726f 6f6d 2068 6173 2061 2022 666f  a room has a "fo
+00001350: 7263 6522 206f 7220 6e6f 742e 0d0a 2d20  rce" or not...- 
+00001360: 5468 6520 656e 656d 6965 7320 696e 2074  The enemies in t
+00001370: 6865 2067 616d 6520 6861 7665 2062 6565  he game have bee
+00001380: 6e20 7265 6261 6c61 6e63 6564 2074 6f20  n rebalanced to 
+00001390: 7265 666c 6563 7420 7468 6520 6c6f 7373  reflect the loss
+000013a0: 2069 6e20 6176 6169 6c61 626c 6520 7570   in available up
+000013b0: 6772 6164 6573 2061 6e64 206d 616b 6520  grades and make 
+000013c0: 7468 6520 6761 6d65 206d 6f72 6520 6261  the game more ba
+000013d0: 6c61 6e63 6564 2e20 284e 4f54 453a 2049  lanced. (NOTE: I
+000013e0: 2064 6f20 6e6f 7420 6775 6172 616e 7465   do not guarante
+000013f0: 6520 7468 6174 2049 2066 6f75 6e64 2065  e that I found e
+00001400: 7665 7279 2065 6e65 6d79 2069 6e20 7468  very enemy in th
+00001410: 6520 6761 6d65 2c20 736f 2069 6620 796f  e game, so if yo
+00001420: 7520 6669 6e64 2061 6e20 656e 656d 7920  u find an enemy 
+00001430: 7468 6174 2073 6565 6d73 2077 696c 646c  that seems wildl
+00001440: 7920 6f76 6572 2d70 6f77 6572 6564 2066  y over-powered f
+00001450: 6f72 2069 7473 2061 7265 612c 2070 6c65  or its area, ple
+00001460: 6173 6520 6d61 6b65 206e 6f74 6520 6f66  ase make note of
+00001470: 2069 7420 6966 2079 6f75 2063 616e 2e29   it if you can.)
+00001480: 0d0a 0d0a 4b4e 4f57 4e20 4255 4753 204e  ....KNOWN BUGS N
+00001490: 4f54 2059 4554 2041 4444 5245 5353 4544  OT YET ADDRESSED
+000014a0: 3a0d 0a2d 204b 6172 6127 7320 706f 7274  :..- Kara's port
+000014b0: 7261 6974 2071 7565 7374 2069 7320 636f  rait quest is co
+000014c0: 6d70 6c65 7465 2077 6865 6e20 7468 6520  mplete when the 
+000014d0: 4d61 6769 6320 4475 7374 2069 7320 7375  Magic Dust is su
+000014e0: 6363 6573 7366 756c 6c79 2075 7365 642e  ccessfully used.
+000014f0: 2020 4b61 7261 2773 2070 6f72 7472 6169    Kara's portrai
+00001500: 7420 7769 6c6c 2072 656d 6169 6e20 6f6e  t will remain on
+00001510: 2074 6865 2073 6372 6565 6e20 6576 656e   the screen even
+00001520: 2061 6674 6572 2073 6865 2069 7320 6672   after she is fr
+00001530: 6565 6420 7769 7468 2074 6865 204d 6167  eed with the Mag
+00001540: 6963 2044 7573 742e 2020 4c65 6176 696e  ic Dust.  Leavin
+00001550: 6720 616e 6420 7265 656e 7465 7269 6e67  g and reentering
+00001560: 2074 6865 2072 6f6f 6d20 7769 6c6c 2070   the room will p
+00001570: 726f 7669 6465 2076 6973 7561 6c20 636f  rovide visual co
+00001580: 6e66 6972 6d61 7469 6f6e 2074 6861 7420  nfirmation that 
+00001590: 7368 6520 6861 7320 6265 656e 2066 7265  she has been fre
+000015a0: 6564 202d 2d20 686f 7765 7665 722c 2074  ed -- however, t
+000015b0: 6869 7320 6973 2075 6e6e 6563 6573 7361  his is unnecessa
+000015c0: 7279 2074 6f20 636f 6d70 6c65 7465 2074  ry to complete t
+000015d0: 6865 2071 7565 7374 2e0d 0a2d 2057 6865  he quest...- Whe
+000015e0: 6e20 4b61 7261 2773 2022 706f 7274 7261  n Kara's "portra
+000015f0: 6974 2220 6170 7065 6172 7320 696e 2074  it" appears in t
+00001600: 6865 2044 6961 6d6f 6e64 204d 696e 652c  he Diamond Mine,
+00001610: 2073 6865 2077 696c 6c20 6c6f 6f6b 206c   she will look l
+00001620: 696b 6520 6865 7220 6e6f 726d 616c 2073  ike her normal s
+00001630: 7072 6974 6520 696e 7374 6561 6420 6f66  prite instead of
+00001640: 206c 696b 6520 7468 6520 706f 7274 7261   like the portra
+00001650: 6974 2069 7473 656c 662e 2049 2068 6f70  it itself. I hop
+00001660: 6520 746f 2066 696e 6420 6120 736f 6c75  e to find a solu
+00001670: 7469 6f6e 2066 6f72 2074 6869 7320 6973  tion for this is
+00001680: 7375 6520 696e 2066 7574 7572 6520 7665  sue in future ve
+00001690: 7273 696f 6e73 2e0d 0a2d 204c 6561 7669  rsions...- Leavi
+000016a0: 6e67 2074 6865 204a 6577 656c 6572 2773  ng the Jeweler's
+000016b0: 204d 616e 7369 6f6e 2061 6e64 2069 6d6d   Mansion and imm
+000016c0: 6564 6961 7465 6c79 2072 6565 6e74 6572  ediately reenter
+000016d0: 696e 6720 7669 6120 4461 6f20 6361 7573  ing via Dao caus
+000016e0: 6573 2074 6865 2074 6f70 206c 6179 6572  es the top layer
+000016f0: 2074 6f20 6c6f 6f6b 2073 7472 616e 6765   to look strange
+00001700: 2e0d 0a2d 2048 6967 6820 5354 5220 6d69  ...- High STR mi
+00001710: 6768 7420 7374 696c 6c20 6465 7374 726f  ght still destro
+00001720: 7920 736e 616b 6573 2069 6e20 736e 616b  y snakes in snak
+00001730: 6520 6761 6d65 2028 7461 6c6b 2074 6f20  e game (talk to 
+00001740: 4e50 4320 696e 2066 726f 6e74 206f 6620  NPC in front of 
+00001750: 7468 6520 7363 686f 6f6c 2074 6f20 7265  the school to re
+00001760: 7365 7420 796f 7572 2053 5452 2f44 4546  set your STR/DEF
+00001770: 290d 0a2d 2041 6371 7569 7269 6e67 2045  )..- Acquiring E
+00001780: 6172 7468 7175 616b 6572 2073 7469 6c6c  arthquaker still
+00001790: 2067 7261 6e74 7320 796f 7520 4461 726b   grants you Dark
+000017a0: 2046 7269 6172 0d0a 2d20 4175 7261 2042   Friar..- Aura B
+000017b0: 6172 7269 6572 2077 696c 6c20 6e6f 7420  arrier will not 
+000017c0: 776f 726b 2075 6e6c 6573 7320 796f 7520  work unless you 
+000017d0: 6861 7665 2044 6172 6b20 4672 6961 720d  have Dark Friar.
+000017e0: 0a0d 0a0d 0a0d 0a76 302e 340d 0a43 4841  .......v0.4..CHA
+000017f0: 4e47 4553 3a0d 0a2d 2054 6865 204b 6172  NGES:..- The Kar
+00001800: 6120 506f 7274 7261 6974 2071 7565 7374  a Portrait quest
+00001810: 2069 7320 6e6f 7720 6675 6e63 7469 6f6e   is now function
+00001820: 616c 2028 7365 6520 6265 6c6f 7729 2e0d  al (see below)..
+00001830: 0a2d 2054 6865 2062 6163 6b20 6f66 2074  .- The back of t
+00001840: 6865 2055 6e64 6572 6772 6f75 6e64 2054  he Underground T
+00001850: 756e 6e65 6c20 6973 206e 6f20 6c6f 6e67  unnel is no long
+00001860: 6572 2061 6363 6573 7369 626c 6520 6672  er accessible fr
+00001870: 6f6d 2045 6477 6172 6427 7320 4361 7374  om Edward's Cast
+00001880: 6c65 2e20 2054 6869 7320 6d65 616e 7320  le.  This means 
+00001890: 7468 6174 2074 6865 206c 6173 7420 7477  that the last tw
+000018a0: 6f20 6974 656d 7320 696e 2074 6869 7320  o items in this 
+000018b0: 6172 6561 2028 7468 6520 7468 6972 6420  area (the third 
+000018c0: 6368 6573 7420 616e 6420 7468 6520 5265  chest and the Re
+000018d0: 6420 4a65 7765 6c20 706f 7420 6265 6869  d Jewel pot behi
+000018e0: 6e64 2074 6865 2062 6172 7265 6c73 2920  nd the barrels) 
+000018f0: 6172 6520 6f6e 6c79 2061 6363 6573 7369  are only accessi
+00001900: 626c 6520 6279 2065 7363 6170 696e 6720  ble by escaping 
+00001910: 4564 7761 7264 2773 2050 7269 736f 6e20  Edward's Prison 
+00001920: 616e 6420 7072 6f67 7265 7373 696e 6720  and progressing 
+00001930: 7468 726f 7567 6820 7468 6520 6475 6e67  through the dung
+00001940: 656f 6e20 6e6f 726d 616c 6c79 2e0d 0a2d  eon normally...-
+00001950: 2048 6176 696e 6720 4c69 6c6c 7920 7769   Having Lilly wi
+00001960: 7468 2079 6f75 2061 6674 6572 2067 6976  th you after giv
+00001970: 696e 6720 6865 7220 7468 6520 6e65 636b  ing her the neck
+00001980: 6c61 6365 2069 7320 7265 7175 6972 6564  lace is required
+00001990: 2074 6f20 7072 6f67 7265 7373 2074 6872   to progress thr
+000019a0: 6f75 6768 2074 6865 2055 6e64 6572 6772  ough the Undergr
+000019b0: 6f75 6e64 2054 756e 6e65 6c2e 0d0a 2d20  ound Tunnel...- 
+000019c0: 4f66 2074 6865 2074 776f 2044 6172 6b20  Of the two Dark 
+000019d0: 5370 6163 6573 2061 6363 6573 7369 626c  Spaces accessibl
+000019e0: 6520 696e 2074 6865 2053 6b79 2047 6172  e in the Sky Gar
+000019f0: 6465 6e20 2869 2e65 2e20 7468 6520 7361  den (i.e. the sa
+00001a00: 7665 2072 6f6f 6d20 696e 2041 7265 6120  ve room in Area 
+00001a10: 322c 206f 7220 7468 6520 626f 7474 6f6d  2, or the bottom
+00001a20: 2d73 6964 6520 4461 726b 2053 7061 6365  -side Dark Space
+00001a30: 2069 6e20 4172 6561 2034 292c 206f 6e65   in Area 4), one
+00001a40: 2077 696c 6c20 616c 7761 7973 2062 6520   will always be 
+00001a50: 6176 6169 6c61 626c 6520 666f 7220 7377  available for sw
+00001a60: 6974 6368 696e 672e 2020 2849 6e20 6f74  itching.  (In ot
+00001a70: 6865 7220 776f 7264 732c 2074 6865 2044  her words, the D
+00001a80: 6172 6b20 5370 6163 6520 696e 2074 6865  ark Space in the
+00001a90: 2073 6d61 6c6c 2073 6176 6520 726f 6f6d   small save room
+00001aa0: 206d 6967 6874 2068 6176 6520 616e 2061   might have an a
+00001ab0: 6269 6c69 7479 2e29 0d0a 2d20 5468 6520  bility.)..- The 
+00001ac0: 6d61 6e20 6174 2074 6865 2065 6e74 7261  man at the entra
+00001ad0: 6e63 6520 6f66 2044 616f 206e 6f77 2074  nce of Dao now t
+00001ae0: 656c 6c73 2079 6f75 2077 6869 6368 2074  ells you which t
+00001af0: 776f 2069 7465 6d73 2068 6520 6769 7665  wo items he give
+00001b00: 7320 796f 752e 0d0a 2d20 5468 6520 6c61  s you...- The la
+00001b10: 626f 7265 7220 696e 2046 7265 656a 6961  borer in Freejia
+00001b20: 206e 6f20 6c6f 6e67 6572 2067 6976 6573   no longer gives
+00001b30: 2061 2073 706f 696c 6572 2e0d 0a2d 2054   a spoiler...- T
+00001b40: 6865 206d 616e 2061 7420 4469 616d 6f6e  he man at Diamon
+00001b50: 6420 436f 6173 7420 6e6f 7720 6769 7665  d Coast now give
+00001b60: 7320 6120 7370 6f69 6c65 722e 0d0a 0d0a  s a spoiler.....
+00001b70: 4b41 5241 2050 4f52 5452 4149 5420 5155  KARA PORTRAIT QU
+00001b80: 4553 543a 0d0a 4669 6e64 696e 6720 4b61  EST:..Finding Ka
+00001b90: 7261 2773 2070 6f72 7472 6169 7420 616e  ra's portrait an
+00001ba0: 6420 7265 7363 7569 6e67 2068 6572 2077  d rescuing her w
+00001bb0: 6974 6820 7468 6520 4d61 6769 6320 4475  ith the Magic Du
+00001bc0: 7374 2069 7320 6e6f 7720 6e65 6365 7373  st is now necess
+00001bd0: 6172 7920 746f 2063 6f6d 706c 6574 6520  ary to complete 
+00001be0: 7468 6520 6761 6d65 2e20 2054 6865 2070  the game.  The p
+00001bf0: 6f72 7472 6169 7420 7769 6c6c 2062 6520  ortrait will be 
+00001c00: 7261 6e64 6f6d 697a 6564 2074 6f20 6170  randomized to ap
+00001c10: 7065 6172 2061 7420 7468 6520 656e 6420  pear at the end 
+00001c20: 6f66 206f 6e65 206f 6620 7468 6520 6669  of one of the fi
+00001c30: 7665 206d 696e 6f72 2064 756e 6765 6f6e  ve minor dungeon
+00001c40: 732e 2020 4669 6e64 696e 6720 616e 6420  s.  Finding and 
+00001c50: 7265 6164 696e 6720 4c61 6e63 6527 7320  reading Lance's 
+00001c60: 4c65 7474 6572 2077 696c 6c20 7370 6f69  Letter will spoi
+00001c70: 6c20 7468 6520 6c6f 6361 7469 6f6e 206f  l the location o
+00001c80: 6620 4b61 7261 2773 2070 6f72 7472 6169  f Kara's portrai
+00001c90: 742e 2020 5468 6520 706f 7274 7261 6974  t.  The portrait
+00001ca0: 2077 696c 6c20 6170 7065 6172 2069 6e20   will appear in 
+00001cb0: 6f6e 6520 6f66 2074 6865 7365 206c 6f63  one of these loc
+00001cc0: 6174 696f 6e73 3a0d 0a2d 2055 6e64 6572  ations:..- Under
+00001cd0: 6772 6f75 6e64 2054 756e 6e65 6c20 286e  ground Tunnel (n
+00001ce0: 6f72 7468 206f 6620 7768 6572 6520 7468  orth of where th
+00001cf0: 6520 5265 6420 4a65 7765 6c20 6973 2066  e Red Jewel is f
+00001d00: 6f75 6e64 2062 6568 696e 6420 7468 6520  ound behind the 
+00001d10: 6261 7272 656c 7329 0d0a 2d20 4469 616d  barrels)..- Diam
+00001d20: 6f6e 6420 4d69 6e65 2028 696e 2074 6865  ond Mine (in the
+00001d30: 2073 616d 6520 726f 6f6d 2077 6865 7265   same room where
+00001d40: 2053 616d 2067 6976 6573 2079 6f75 2061   Sam gives you a
+00001d50: 6e20 6974 656d 290d 0a2d 2041 6e67 656c  n item)..- Angel
+00001d60: 2056 696c 6c61 6765 2028 7661 6e69 6c6c   Village (vanill
+00001d70: 6120 6c6f 6361 7469 6f6e 290d 0a2d 204d  a location)..- M
+00001d80: 742e 204b 7265 7373 2028 696e 2074 6865  t. Kress (in the
+00001d90: 206c 6173 7420 726f 6f6d 206e 6561 7220   last room near 
+00001da0: 7468 6520 6669 6e61 6c20 6368 6573 7429  the final chest)
+00001db0: 0d0a 2d20 416e 6b6f 7220 5761 7420 2869  ..- Ankor Wat (i
+00001dc0: 6e20 7468 6520 6c61 7374 2072 6f6f 6d2c  n the last room,
+00001dd0: 206f 6e20 7468 6520 7761 6c6c 2074 6f20   on the wall to 
+00001de0: 7468 6520 7269 6768 7429 0d0a 0d0a 4b4e  the right)....KN
+00001df0: 4f57 4e20 4255 4753 204e 4f54 2059 4554  OWN BUGS NOT YET
+00001e00: 2041 4444 5245 5353 4544 3a0d 0a2d 204b   ADDRESSED:..- K
+00001e10: 6172 6127 7320 706f 7274 7261 6974 2071  ara's portrait q
+00001e20: 7565 7374 2069 7320 636f 6d70 6c65 7465  uest is complete
+00001e30: 2077 6865 6e20 7468 6520 4d61 6769 6320   when the Magic 
+00001e40: 4475 7374 2069 7320 7375 6363 6573 7366  Dust is successf
+00001e50: 756c 6c79 2075 7365 642e 2020 4b61 7261  ully used.  Kara
+00001e60: 2773 2070 6f72 7472 6169 7420 7769 6c6c  's portrait will
+00001e70: 2072 656d 6169 6e20 6f6e 2074 6865 2073   remain on the s
+00001e80: 6372 6565 6e20 6576 656e 2061 6674 6572  creen even after
+00001e90: 2073 6865 2069 7320 6672 6565 6420 7769   she is freed wi
+00001ea0: 7468 2074 6865 204d 6167 6963 2044 7573  th the Magic Dus
+00001eb0: 742e 2020 4c65 6176 696e 6720 616e 6420  t.  Leaving and 
+00001ec0: 7265 656e 7465 7269 6e67 2074 6865 2072  reentering the r
+00001ed0: 6f6f 6d20 7769 6c6c 2070 726f 7669 6465  oom will provide
+00001ee0: 2076 6973 7561 6c20 636f 6e66 6972 6d61   visual confirma
+00001ef0: 7469 6f6e 2074 6861 7420 7368 6520 6861  tion that she ha
+00001f00: 7320 6265 656e 2066 7265 6564 202d 2d20  s been freed -- 
+00001f10: 686f 7765 7665 722c 2074 6869 7320 6973  however, this is
+00001f20: 2075 6e6e 6563 6573 7361 7279 2074 6f20   unnecessary to 
+00001f30: 636f 6d70 6c65 7465 2074 6865 2071 7565  complete the que
+00001f40: 7374 2e0d 0a2d 2057 6865 6e20 4b61 7261  st...- When Kara
+00001f50: 2773 2022 706f 7274 7261 6974 2220 6170  's "portrait" ap
+00001f60: 7065 6172 7320 696e 2074 6865 2044 6961  pears in the Dia
+00001f70: 6d6f 6e64 204d 696e 652c 2073 6865 2077  mond Mine, she w
+00001f80: 696c 6c20 6c6f 6f6b 206c 696b 6520 6865  ill look like he
+00001f90: 7220 6e6f 726d 616c 2073 7072 6974 6520  r normal sprite 
+00001fa0: 696e 7374 6561 6420 6f66 206c 696b 6520  instead of like 
+00001fb0: 7468 6520 706f 7274 7261 6974 2069 7473  the portrait its
+00001fc0: 656c 662e 2049 2068 6f70 6520 746f 2066  elf. I hope to f
+00001fd0: 696e 6420 6120 736f 6c75 7469 6f6e 2066  ind a solution f
+00001fe0: 6f72 2074 6869 7320 6973 7375 6520 696e  or this issue in
+00001ff0: 2066 7574 7572 6520 7665 7273 696f 6e73   future versions
+00002000: 2e0d 0a2d 204c 6561 7669 6e67 2074 6865  ...- Leaving the
+00002010: 204a 6577 656c 6572 2773 204d 616e 7369   Jeweler's Mansi
+00002020: 6f6e 2061 6e64 2069 6d6d 6564 6961 7465  on and immediate
+00002030: 6c79 2072 6565 6e74 6572 696e 6720 7669  ly reentering vi
+00002040: 6120 4461 6f20 6361 7573 6573 2074 6865  a Dao causes the
+00002050: 2074 6f70 206c 6179 6572 2074 6f20 6c6f   top layer to lo
+00002060: 6f6b 2073 7472 616e 6765 2e0d 0a2d 2048  ok strange...- H
+00002070: 6967 6820 5354 5220 6d69 6768 7420 7374  igh STR might st
+00002080: 696c 6c20 6465 7374 726f 7920 736e 616b  ill destroy snak
+00002090: 6573 2069 6e20 736e 616b 6520 6761 6d65  es in snake game
+000020a0: 2028 7461 6c6b 2074 6f20 4e50 4320 696e   (talk to NPC in
+000020b0: 2066 726f 6e74 206f 6620 7468 6520 7363   front of the sc
+000020c0: 686f 6f6c 2074 6f20 7265 7365 7420 796f  hool to reset yo
+000020d0: 7572 2053 5452 2f44 4546 290d 0a2d 2041  ur STR/DEF)..- A
+000020e0: 6371 7569 7269 6e67 2045 6172 7468 7175  cquiring Earthqu
+000020f0: 616b 6572 2073 7469 6c6c 2067 7261 6e74  aker still grant
+00002100: 7320 796f 7520 4461 726b 2046 7269 6172  s you Dark Friar
+00002110: 0d0a 2d20 4175 7261 2042 6172 7269 6572  ..- Aura Barrier
+00002120: 2077 696c 6c20 6e6f 7420 776f 726b 2075   will not work u
+00002130: 6e6c 6573 7320 796f 7520 6861 7665 2044  nless you have D
+00002140: 6172 6b20 4672 6961 720d 0a0d 0a0d 0a0d  ark Friar.......
+00002150: 0a76 302e 330d 0a43 4841 4e47 4553 3a0d  .v0.3..CHANGES:.
+00002160: 0a2d 2049 6e76 656e 746f 7279 2073 697a  .- Inventory siz
+00002170: 6520 636f 6e73 7472 6169 6e74 7320 6861  e constraints ha
+00002180: 7665 2062 6565 6e20 696d 706c 656d 656e  ve been implemen
+00002190: 7465 6420 696e 206c 6f67 6963 0d0a 2d20  ted in logic..- 
+000021a0: 4c6f 6769 6320 6275 6720 7468 6174 206f  Logic bug that o
+000021b0: 7665 722d 636f 756e 7465 6420 7468 6520  ver-counted the 
+000021c0: 6e75 6d62 6572 206f 6620 5265 6420 4a65  number of Red Je
+000021d0: 7765 6c73 2061 6371 7569 7265 6420 6861  wels acquired ha
+000021e0: 7320 6265 656e 2066 6978 6564 0d0a 2d20  s been fixed..- 
+000021f0: 4465 6665 6174 696e 6720 7468 6520 5661  Defeating the Va
+00002200: 6d70 6972 6573 2069 7320 6e6f 7720 7265  mpires is now re
+00002210: 7175 6972 6564 2074 6f20 6f62 7461 696e  quired to obtain
+00002220: 2053 7461 7475 6520 330d 0a2d 2059 6f75   Statue 3..- You
+00002230: 2063 616e 206e 6f77 2061 6363 6573 7320   can now access 
+00002240: 4361 7374 6f74 6820 616e 6420 5669 7065  Castoth and Vipe
+00002250: 7220 626f 7373 2072 6f6f 6d73 2061 6674  r boss rooms aft
+00002260: 6572 2064 6566 6561 7469 6e67 2074 6865  er defeating the
+00002270: 6d3b 2074 6869 7320 616c 6c6f 7773 2070  m; this allows p
+00002280: 6572 7065 7475 616c 2061 6363 6573 7320  erpetual access 
+00002290: 746f 2047 6f6c 6420 5368 6970 2061 6e64  to Gold Ship and
+000022a0: 2053 6561 7369 6465 2050 616c 6163 652c   Seaside Palace,
+000022b0: 2072 6573 7065 6374 6976 656c 790d 0a2d   respectively..-
+000022c0: 2057 6865 6e20 656e 7465 7269 6e67 2049   When entering I
+000022d0: 746f 7279 2056 696c 6c61 6765 2066 6f72  tory Village for
+000022e0: 2074 6865 2066 6972 7374 2074 696d 652c   the first time,
+000022f0: 2079 6f75 2063 616e 206d 6f76 6520 6172   you can move ar
+00002300: 6f75 6e64 2061 206c 6974 746c 6520 6265  ound a little be
+00002310: 666f 7265 2062 6569 6e67 2073 656e 7420  fore being sent 
+00002320: 6261 636b 2074 6f20 7468 6520 6f76 6572  back to the over
+00002330: 776f 726c 640d 0a2d 204a 6577 656c 6572  world..- Jeweler
+00002340: 2773 204d 616e 7369 6f6e 206c 6f67 6963  's Mansion logic
+00002350: 2068 6173 2063 6861 6e67 6564 3a20 0d0a   has changed: ..
+00002360: 2020 6129 2045 7869 7469 6e67 2074 6865    a) Exiting the
+00002370: 206d 616e 7369 6f6e 2069 6d6d 6564 6961   mansion immedia
+00002380: 7465 6c79 2073 656e 6473 2079 6f75 2074  tely sends you t
+00002390: 6f20 4461 6f3b 200d 0a20 2062 2920 4465  o Dao; ..  b) De
+000023a0: 6665 6174 696e 6720 536f 6c69 6420 4172  feating Solid Ar
+000023b0: 6d20 7365 6e64 7320 796f 7520 746f 2074  m sends you to t
+000023c0: 6865 2074 6f70 206f 6620 4261 6265 6c20  he top of Babel 
+000023d0: 546f 7765 7220 616e 6420 6361 7573 6573  Tower and causes
+000023e0: 2074 6865 2073 7069 7269 7420 696e 2044   the spirit in D
+000023f0: 616f 2074 6f20 6170 7065 6172 2061 7320  ao to appear as 
+00002400: 7765 6c6c 0d0a 2d20 476f 696e 6720 746f  well..- Going to
+00002410: 2073 6c65 6570 206f 6e20 7468 6520 476f   sleep on the Go
+00002420: 6c64 2053 6869 7020 2869 6620 796f 7520  ld Ship (if you 
+00002430: 6361 6e20 6d61 6e61 6765 2074 6f20 646f  can manage to do
+00002440: 2069 7429 2073 656e 6473 2079 6f75 2074   it) sends you t
+00002450: 6f20 7468 6520 4469 616d 6f6e 6420 436f  o the Diamond Co
+00002460: 6173 740d 0a2d 2054 616c 6b69 6e67 2074  ast..- Talking t
+00002470: 6f20 4973 6874 6172 2072 6573 6574 7320  o Ishtar resets 
+00002480: 7468 6520 7075 7a7a 6c65 2069 6e20 416e  the puzzle in An
+00002490: 6765 6c20 5669 6c6c 6167 650d 0a2d 204a  gel Village..- J
+000024a0: 6163 6b61 6c20 7368 6f75 6c64 206e 6f20  ackal should no 
+000024b0: 6c6f 6e67 6572 2073 6f66 7420 6c6f 636b  longer soft lock
+000024c0: 2079 6f75 2069 6e20 5079 7261 6d69 640d   you in Pyramid.
+000024d0: 0a2d 2045 7572 6f20 6775 6573 7420 726f  .- Euro guest ro
+000024e0: 6f6d 2061 6e64 2044 616f 2053 4520 686f  om and Dao SE ho
+000024f0: 7573 6520 6172 6520 6e6f 7720 6162 6c65  use are now able
+00002500: 2074 6f20 6265 2065 6e74 6572 6564 2077   to be entered w
+00002510: 6974 686f 7574 2068 6172 642d 6c6f 636b  ithout hard-lock
+00002520: 696e 670d 0a2d 2054 6865 2062 7567 2074  ing..- The bug t
+00002530: 6861 7420 6d61 6465 2074 6865 2069 6e74  hat made the int
+00002540: 6572 696f 7220 6f66 2045 7572 6f20 686f  erior of Euro ho
+00002550: 7573 6573 206c 6f6f 6b20 7374 7261 6e67  uses look strang
+00002560: 6520 6861 7320 6265 656e 2066 6978 6564  e has been fixed
+00002570: 0d0a 2d20 5468 6520 6973 7375 6520 7468  ..- The issue th
+00002580: 6174 2063 6175 7365 6420 7661 7269 6f75  at caused variou
+00002590: 7320 4e50 4373 2074 6f20 6d69 7362 6568  s NPCs to misbeh
+000025a0: 6176 6520 6f72 2064 6973 6170 7065 6172  ave or disappear
+000025b0: 2069 6e20 6c61 7465 2067 616d 6520 2865   in late game (e
+000025c0: 2e67 2e20 4572 696b 2c20 4c69 6c6c 792c  .g. Erik, Lilly,
+000025d0: 2065 7463 2e29 2068 6173 2062 6565 6e20   etc.) has been 
+000025e0: 6669 7865 640d 0a2d 2057 696e 6420 4d65  fixed..- Wind Me
+000025f0: 6c6f 6479 2069 7320 6e6f 7720 7265 6d6f  lody is now remo
+00002600: 7665 6420 7768 656e 2049 6e63 6120 646f  ved when Inca do
+00002610: 6f72 2069 7320 6f70 656e 6564 0d0a 2d20  or is opened..- 
+00002620: 4f70 656e 696e 6720 7365 7175 656e 6365  Opening sequence
+00002630: 2063 616e 2062 6520 706c 6179 6564 2066   can be played f
+00002640: 756c 6c79 2077 6974 686f 7574 2068 6172  ully without har
+00002650: 642d 6c6f 636b 696e 670d 0a2d 2049 6e2d  d-locking..- In-
+00002660: 6761 6d65 2073 706f 696c 6572 7320 6861  game spoilers ha
+00002670: 7665 2062 6565 6e20 696d 706c 656d 656e  ve been implemen
+00002680: 7465 6420 2873 6565 2062 656c 6f77 290d  ted (see below).
+00002690: 0a0d 0a49 4e2d 4741 4d45 2053 504f 494c  ...IN-GAME SPOIL
+000026a0: 4552 533a 0d0a 5468 6520 666f 6c6c 6f77  ERS:..The follow
+000026b0: 696e 6720 4e50 4373 2077 696c 6c20 6561  ing NPCs will ea
+000026c0: 6368 2067 6976 6520 7468 6520 6765 6e65  ch give the gene
+000026d0: 7261 6c20 6c6f 6361 7469 6f6e 206f 6620  ral location of 
+000026e0: 6f6e 6520 6974 656d 2069 6e20 7468 6520  one item in the 
+000026f0: 6761 6d65 3a0d 0a2d 204b 6172 6127 7320  game:..- Kara's 
+00002700: 4775 6172 6420 696e 2045 6477 6172 6427  Guard in Edward'
+00002710: 7320 4361 7374 6c65 0d0a 2d20 5468 6520  s Castle..- The 
+00002720: 656c 6465 7220 696e 2049 746f 7279 0d0a  elder in Itory..
+00002730: 2d20 5468 6520 7175 6565 6e20 6f6e 2074  - The queen on t
+00002740: 6865 2047 6f6c 6420 5368 6970 0d0a 2d20  he Gold Ship..- 
+00002750: 5468 6520 6c61 626f 7265 7220 666f 7220  The laborer for 
+00002760: 6175 6374 696f 6e20 696e 2046 7265 656a  auction in Freej
+00002770: 6961 0d0a 2d20 5468 6520 656d 7074 7920  ia..- The empty 
+00002780: 636f 6666 696e 2069 6e20 5365 6173 6964  coffin in Seasid
+00002790: 6520 5061 6c61 6365 0d0a 2d20 4973 6874  e Palace..- Isht
+000027a0: 6172 2773 2061 7070 7265 6e74 6963 6520  ar's apprentice 
+000027b0: 696e 2041 6e67 656c 2056 696c 6c61 6765  in Angel Village
+000027c0: 0d0a 2d20 4b61 7261 2773 206a 6f75 726e  ..- Kara's journ
+000027d0: 616c 2069 6e20 5761 7465 726d 6961 0d0a  al in Watermia..
+000027e0: 2d20 4572 6173 7175 657a 2069 6e20 4575  - Erasquez in Eu
+000027f0: 726f 0d0a 2d20 5468 6520 7370 6972 6974  ro..- The spirit
+00002800: 2069 6e20 416e 6b6f 7220 5761 740d 0a2d   in Ankor Wat..-
+00002810: 2047 6972 6c20 7769 7468 204a 6163 6b61   Girl with Jacka
+00002820: 6c27 7320 6e6f 7465 2069 6e20 4461 6f0d  l's note in Dao.
+00002830: 0a2d 2054 6865 2066 6972 7374 2073 7069  .- The first spi
+00002840: 7269 7420 696e 2042 6162 656c 2054 6f77  rit in Babel Tow
+00002850: 6572 0d0a 0d0a 4b4e 4f57 4e20 4255 4753  er....KNOWN BUGS
+00002860: 204e 4f54 2059 4554 2041 4444 5245 5353   NOT YET ADDRESS
+00002870: 4544 3a0d 0a2d 204b 6172 6120 7175 6573  ED:..- Kara ques
+00002880: 7420 6861 7320 6e6f 7420 7965 7420 6265  t has not yet be
+00002890: 656e 2069 6d70 6c65 6d65 6e74 6564 2028  en implemented (
+000028a0: 692e 652e 204d 6167 6963 2044 7573 7420  i.e. Magic Dust 
+000028b0: 616e 6420 4c61 6e63 6527 7320 4c65 7474  and Lance's Lett
+000028c0: 6572 2061 7265 2075 7365 6c65 7373 290d  er are useless).
+000028d0: 0a2d 2048 6967 6820 5354 5220 6d69 6768  .- High STR migh
+000028e0: 7420 7374 696c 6c20 6465 7374 726f 7920  t still destroy 
+000028f0: 736e 616b 6573 2069 6e20 736e 616b 6520  snakes in snake 
+00002900: 6761 6d65 2028 7461 6c6b 2074 6f20 4e50  game (talk to NP
+00002910: 4320 696e 2066 726f 6e74 206f 6620 7468  C in front of th
+00002920: 6520 7363 686f 6f6c 2074 6f20 7265 7365  e school to rese
+00002930: 7420 796f 7572 2053 5452 2f44 4546 290d  t your STR/DEF).
+00002940: 0a2d 2044 7969 6e67 2069 6e20 7468 6520  .- Dying in the 
+00002950: 556e 6465 7267 726f 756e 6420 5475 6e6e  Underground Tunn
+00002960: 656c 2062 6566 6f72 6520 7669 7369 7469  el before visiti
+00002970: 6e67 2045 6477 6172 6427 7320 5072 6973  ng Edward's Pris
+00002980: 6f6e 206d 6967 6874 2073 7469 6c6c 2068  on might still h
+00002990: 6172 6420 6c6f 636b 2079 6f75 0d0a 2d20  ard lock you..- 
+000029a0: 4163 7175 6972 696e 6720 4561 7274 6871  Acquiring Earthq
+000029b0: 7561 6b65 7220 7374 696c 6c20 6772 616e  uaker still gran
+000029c0: 7473 2079 6f75 2044 6172 6b20 4672 6961  ts you Dark Fria
+000029d0: 720d 0a2d 2041 7572 6120 4261 7272 6965  r..- Aura Barrie
+000029e0: 7220 7769 6c6c 206e 6f74 2077 6f72 6b20  r will not work 
+000029f0: 756e 6c65 7373 2079 6f75 2068 6176 6520  unless you have 
+00002a00: 4461 726b 2046 7269 6172 0d0a 0d0a 0d0a  Dark Friar......
+00002a10: 0d0a 0d0a 762e 302e 320d 0a43 6861 6e67  ....v.0.2..Chang
+00002a20: 6573 3a0d 0a2d 2043 616e 206e 6f20 6c6f  es:..- Can no lo
+00002a30: 6e67 6572 2062 6520 736f 6674 2d6c 6f63  nger be soft-loc
+00002a40: 6b65 6420 6279 2065 6e74 6572 696e 6720  ked by entering 
+00002a50: 686f 7573 6520 696e 2044 616f 0d0a 2d20  house in Dao..- 
+00002a60: 5472 6176 656c 206f 7074 696f 6e73 2075  Travel options u
+00002a70: 6e6c 6f63 6b65 6420 6279 204c 6f6c 6127  nlocked by Lola'
+00002a80: 7320 4c65 7474 6572 2061 6e64 2074 6865  s Letter and the
+00002a90: 2054 6561 706f 7420 6861 7665 2062 6565   Teapot have bee
+00002aa0: 6e20 6368 616e 6765 640d 0a2d 204c 6f6c  n changed..- Lol
+00002ab0: 6127 7320 4d65 6c6f 6479 206e 6f77 2072  a's Melody now r
+00002ac0: 6571 7569 7265 6420 746f 2061 6363 6573  equired to acces
+00002ad0: 7320 4974 6f72 7920 5669 6c6c 6167 650d  s Itory Village.
+00002ae0: 0a2d 204f 7665 7277 6f72 6c64 2065 7869  .- Overworld exi
+00002af0: 7473 2068 6176 6520 6265 656e 2061 6464  ts have been add
+00002b00: 6564 2074 6f20 4e65 696c 2773 2043 6f74  ed to Neil's Cot
+00002b10: 7461 6765 2061 6e64 2044 6961 6d6f 6e64  tage and Diamond
+00002b20: 2043 6f61 7374 0d0a 2d20 4974 656d 7320   Coast..- Items 
+00002b30: 6172 6520 7265 6d6f 7665 6420 6672 6f6d  are removed from
+00002b40: 2069 6e76 656e 746f 7279 206f 6e63 6520   inventory once 
+00002b50: 7573 6564 2c20 7768 6572 6520 6170 7072  used, where appr
+00002b60: 6f70 7269 6174 650d 0a2d 2042 6c61 636b  opriate..- Black
+00002b70: 2047 6c61 7373 6573 2061 6e64 2043 7279   Glasses and Cry
+00002b80: 7374 616c 2052 696e 6720 6361 6e20 6265  stal Ring can be
+00002b90: 2075 7365 6420 6f6e 6365 2061 6e64 2061   used once and a
+00002ba0: 7265 2063 6f6e 7369 6465 7265 6420 776f  re considered wo
+00002bb0: 726e 2066 726f 6d20 7468 656e 206f 6e0d  rn from then on.
+00002bc0: 0a2d 204e 6f6e 2d65 7373 656e 7469 616c  .- Non-essential
+00002bd0: 2069 7465 6d73 2063 616e 2062 6520 7265   items can be re
+00002be0: 6d6f 7665 6420 6672 6f6d 2069 6e76 656e  moved from inven
+00002bf0: 746f 7279 2061 7420 7769 6c6c 0d0a 2d20  tory at will..- 
+00002c00: 5468 6520 676c 6974 6368 2074 6861 7420  The glitch that 
+00002c10: 6d61 6465 2068 6965 726f 676c 7970 6873  made hieroglyphs
+00002c20: 2061 7070 6561 7220 6e6f 7420 746f 206d   appear not to m
+00002c30: 6174 6368 206f 6e63 6520 706c 6163 6564  atch once placed
+00002c40: 2068 6173 2062 6565 6e20 6669 7865 640d   has been fixed.
+00002c50: 0a2d 2042 7567 7320 6672 6f6d 2042 6162  .- Bugs from Bab
+00002c60: 656c 2066 6f72 6365 2066 6965 6c64 2065  el force field e
+00002c70: 7665 6e74 2068 6176 6520 6265 656e 2066  vent have been f
+00002c80: 6978 6564 0d0a 2d20 4275 6773 2074 6861  ixed..- Bugs tha
+00002c90: 7420 7265 7374 7269 6374 6564 2061 6269  t restricted abi
+00002ca0: 6c69 7479 2061 6371 7569 7369 7469 6f6e  lity acquisition
+00002cb0: 2066 726f 6d20 6365 7274 6169 6e20 4461   from certain Da
+00002cc0: 726b 2053 7061 6365 7320 6861 7320 6265  rk Spaces has be
+00002cd0: 656e 2066 6978 6564 0d0a 2d20 5468 6520  en fixed..- The 
+00002ce0: 6669 7273 7420 4461 726b 2053 7061 6365  first Dark Space
+00002cf0: 2069 6e20 496e 6361 2052 7569 6e73 2077   in Inca Ruins w
+00002d00: 696c 6c20 616c 7761 7973 2061 6c6c 6f77  ill always allow
+00002d10: 2066 6f72 6d20 6368 616e 6765 2e0d 0a0d   form change....
+00002d20: 0a0d 0a4b 6e6f 776e 2062 7567 7320 6e6f  ...Known bugs no
+00002d30: 7420 7965 7420 6164 6472 6573 7365 643a  t yet addressed:
+00002d40: 0d0a 2d20 4c6f 6769 6320 616c 676f 7269  ..- Logic algori
+00002d50: 7468 6d20 6d61 7920 7374 696c 6c20 6265  thm may still be
+00002d60: 2066 6175 6c74 790d 0a2d 2049 6e76 656e   faulty..- Inven
+00002d70: 746f 7279 2073 7061 6365 2068 6173 206e  tory space has n
+00002d80: 6f74 2079 6574 2062 6565 6e20 696e 636f  ot yet been inco
+00002d90: 7270 7261 7465 6420 696e 746f 206c 6f67  rprated into log
+00002da0: 6963 0d0a 2d20 4661 696c 696e 6720 746f  ic..- Failing to
+00002db0: 2063 6f6c 6c65 6374 2074 6865 2069 7465   collect the ite
+00002dc0: 6d73 2069 6e20 4973 6874 6172 2773 2070  ms in Ishtar's p
+00002dd0: 757a 7a6c 6520 6d69 6768 7420 7374 696c  uzzle might stil
+00002de0: 6c20 736f 6674 206c 6f63 6b20 796f 750d  l soft lock you.
+00002df0: 0a2d 2048 6967 6820 5354 5220 6d69 6768  .- High STR migh
+00002e00: 7420 7374 696c 6c20 6465 7374 726f 7920  t still destroy 
+00002e10: 736e 616b 6573 2069 6e20 736e 616b 6520  snakes in snake 
+00002e20: 6761 6d65 2028 7461 6c6b 2074 6f20 4e50  game (talk to NP
+00002e30: 4320 696e 2066 726f 6e74 206f 6620 7468  C in front of th
+00002e40: 6520 7363 686f 6f6c 2074 6f20 7265 7365  e school to rese
+00002e50: 7420 796f 7572 2053 5452 2f44 4546 290d  t your STR/DEF).
+00002e60: 0a2d 204d 7520 7374 696c 6c20 616c 6c6f  .- Mu still allo
+00002e70: 7773 2079 6f75 2074 6f20 6765 7420 7468  ws you to get th
+00002e80: 6520 4d79 7374 6963 2053 7461 7475 6520  e Mystic Statue 
+00002e90: 6265 666f 7265 2064 6566 6561 7469 6e67  before defeating
+00002ea0: 2056 616d 7069 7265 730d 0a2d 2041 6371   Vampires..- Acq
+00002eb0: 7569 7269 6e67 2045 6172 7468 7175 616b  uiring Earthquak
+00002ec0: 6572 2073 7469 6c6c 2067 7261 6e74 7320  er still grants 
+00002ed0: 796f 7520 4461 726b 2046 7269 6172 0d0a  you Dark Friar..
```

### Comparing `iog-randomizer-4.7.2.2/randomizer/ATlMpMuSEWaterHighSub_Tilemap1_comp.bin` & `iog_randomizer-5.0.0/src/iog_randomizer/randomizer/ATlMpMuSEWaterHighSub_Tilemap1_comp.bin`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.2/randomizer/ATlMpSpecInvBg_comp.bin` & `iog_randomizer-5.0.0/src/iog_randomizer/randomizer/ATlMpSpecInvBg_comp.bin`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.2/randomizer/ConfigValueArray.asr` & `iog_randomizer-5.0.0/src/iog_randomizer/randomizer/ConfigValueArray.asr`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ; and pass the assembler a define called ParamName.
 ; The value at BankAnchor can be used as a version check;
 ; increment it if you add or change parameter.
 
 namespace Config
 
 BankAnchor:
-dw $0001
+dw $0002
 
 macro MAddConfigAddr(ConfigName,DefaultValue)
 <ConfigName>:
 if defined("<ConfigName>")
 dw !{<ConfigName>}
 else
 !<ConfigName> = <DefaultValue>
@@ -72,45 +72,45 @@
 %MAddConfigAddr("SettingEarlyFirebird",0)    ; 0=No, 1=Yes
 
 %MAddConfigAddr("SettingFluteOpt",0)    ; 0=Start, 1=Shuffle, 2=Fluteless
 
 %MAddConfigAddr("IncaTileX",2)   ; 12 wide, range [0,11]
 %MAddConfigAddr("IncaTileY",4)   ; 6 high, range [0,5]
 
-; The code assumes 8 bytes per room.
+; The code assumes 8 bytes per room. The order of elements is strange; callers shouldn't worry about it.
 ; DifferenceIndex1 is applied to the right room; 2 and 3 are applied to both.
 ; Room 3 automatically ignores Index1 if the chest contents are different.
 IshtarRoomDifferencesAnchor:
-IshtarRoom1DifferenceIndex1:
-dw !IshtarRoom1DifferenceIndex1
-IshtarRoom1DifferenceIndex2:
-dw !IshtarRoom1DifferenceIndex2
 IshtarRoom1DifferenceIndex3:
 dw !IshtarRoom1DifferenceIndex3
+IshtarRoom1DifferenceIndex2:
+dw !IshtarRoom1DifferenceIndex2
+IshtarRoom1DifferenceIndex1:
+dw !IshtarRoom1DifferenceIndex1
 dw $ffff
-IshtarRoom2DifferenceIndex1:
-dw !IshtarRoom2DifferenceIndex1
-IshtarRoom2DifferenceIndex2:
-dw !IshtarRoom2DifferenceIndex2
 IshtarRoom2DifferenceIndex3:
 dw !IshtarRoom2DifferenceIndex3
+IshtarRoom2DifferenceIndex2:
+dw !IshtarRoom2DifferenceIndex2
+IshtarRoom2DifferenceIndex1:
+dw !IshtarRoom2DifferenceIndex1
 dw $ffff
-IshtarRoom3DifferenceIndex1:
-dw !IshtarRoom3DifferenceIndex1
-IshtarRoom3DifferenceIndex2:
-dw !IshtarRoom3DifferenceIndex2
 IshtarRoom3DifferenceIndex3:
 dw !IshtarRoom3DifferenceIndex3
+IshtarRoom3DifferenceIndex2:
+dw !IshtarRoom3DifferenceIndex2
+IshtarRoom3DifferenceIndex1:
+dw !IshtarRoom3DifferenceIndex1
 dw $ffff
-IshtarRoom4DifferenceIndex1:
-dw !IshtarRoom4DifferenceIndex1
-IshtarRoom4DifferenceIndex2:
-dw !IshtarRoom4DifferenceIndex2
 IshtarRoom4DifferenceIndex3:
 dw !IshtarRoom4DifferenceIndex3
+IshtarRoom4DifferenceIndex2:
+dw !IshtarRoom4DifferenceIndex2
+IshtarRoom4DifferenceIndex1:
+dw !IshtarRoom4DifferenceIndex1
 dw $ffff
 
 HieroOrderAnchor:
 %MAddConfigAddr("HieroOrder1",1)
 %MAddConfigAddr("HieroOrder2",2)
 %MAddConfigAddr("HieroOrder3",3)
 %MAddConfigAddr("HieroOrder4",4)
```

### Comparing `iog-randomizer-4.7.2.2/randomizer/Tilemap6D.bin` & `iog_randomizer-5.0.0/src/iog_randomizer/randomizer/Tilemap6D.bin`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.2/randomizer/apocalypse_gaia_1.asr` & `iog_randomizer-5.0.0/src/iog_randomizer/randomizer/apocalypse_gaia_1.asr`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.2/randomizer/apocalypse_gaia_2.asr` & `iog_randomizer-5.0.0/src/iog_randomizer/randomizer/apocalypse_gaia_2.asr`

 * *Files 0% similar despite different names*

```diff
@@ -373,15 +373,14 @@
 
 ; BG1&2 share a VRAM tilemap, but have separate (identical) RAM staging tilemaps.
 ;   So we can handle them separately if we want.
 ; BG1 unused tiles: $23,$31,$5B,$7C,$8E,$B3-$B7,$BB-$C0,$C3+
 ; BG2 unused tiles: $00-$B1,$B3-$B4,$B8-$BC,$C1-$C2,$C6,$E0-$E6
 ;   Unused in both: $23,$31,$5B,$7C,$8E,$B3,$B4,$BB,$BC,$C6,$E0-$E6
 ;
-org $87e9fc
 DataAGP1BG1: ; AG body P1 RAM tilemap
 db $00 
 DataAGP3BG2: ; BG2/comet tilemap for P3, makes the comet bigger
 db $c3,$c4,$be,$be,$c3,$c5,$be,$be,$bd,$be,$be,$be,$b5,$b6,$be,$be
 db $b5,$b6,$be,$be,$b5,$b6,$be,$be,$be,$c3,$c4,$c3,$bd,$be,$be,$be
 db $bd,$be,$be,$be,$bd,$be,$be,$c3,$c4,$be,$be,$be,$c5,$be,$b5,$b6
 db $e8,$e9,$ea,$eb,$ec,$ed,$ee,$ef,$c8,$c9,$ca,$cb,$cc,$cd,$ce,$cf ; \
```

### Comparing `iog-randomizer-4.7.2.2/randomizer/asar-x64.dll` & `iog_randomizer-5.0.0/src/iog_randomizer/randomizer/asar-x64.dll`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.2/randomizer/asar-x64.so` & `iog_randomizer-5.0.0/src/iog_randomizer/randomizer/asar-x64.so`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.2/randomizer/asar-x86.dll` & `iog_randomizer-5.0.0/src/iog_randomizer/randomizer/asar-x86.dll`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.2/randomizer/asar.py` & `iog_randomizer-5.0.0/src/iog_randomizer/randomizer/asar.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,18 @@
 Usage: import asar, call asar.init, call asar.patch, then use the various
 functions to get info about the patch
 """
 
 import ctypes
 import enum
 import sys
-from ctypes import c_int, c_char_p, POINTER
+from ctypes import POINTER
+from ctypes import c_char_p
+from ctypes import c_int
+
 c_int_ptr = POINTER(c_int)
 
 __all__ = ["errordata", "writtenblockdata", "mappertype", "version",
            "apiversion", "init", "reset", "patch", "maxromsize", "close",
            "geterrors", "getwarnings", "getprints", "getalllabels",
            "getlabelval", "getdefine", "getalldefines", "resolvedefines",
            "math", "getwrittenblocks", "getmapper", "getsymbolsfile"]
@@ -155,15 +158,15 @@
             self.setup_func("getsymbolsfile", (c_char_p,), c_char_p)
 
         except AttributeError:
             raise OSError("Asar DLL is missing some functions")
         api_ver = dll.asar_apiversion()
         if api_ver < _target_api_ver or \
                 (api_ver // 100) > (_target_api_ver // 100):
-            raise OSError("Asar DLL version "+str(api_ver)+" unsupported")
+            raise OSError("Asar DLL version " + str(api_ver) + " unsupported")
 
     def setup_func(self, name, argtypes, restype):
         """Setup argument and return types for a function.
 
         name: name of the function in the DLL. "asar_" is added automatically
         argtypes and restype: see ctypes documentation
         """
@@ -246,17 +249,19 @@
     """Clear out errors, warnings, printed statements and the file cache.
 
     Not really useful, since asar.patch() already does this.
     """
     return _asar.dll.asar_reset()
 
 
-def patch(patch_name, rom_data, includepaths=[], should_reset=True,
-          additional_defines={}, std_include_file=None, std_define_file=None,
-          warning_overrides={}, memory_files={}, override_checksum=None):
+def patch(
+    patch_name, rom_data, includepaths=[], should_reset=True,
+    additional_defines={}, std_include_file=None, std_define_file=None,
+    warning_overrides={}, memory_files={}, override_checksum=None
+    ):
     """Applies a patch.
 
     Returns (success, new_rom_data). If success is False you should call
     geterrors() to see what went wrong. rom_data is assumed to be headerless.
 
     If includepaths is specified, it lists additional include paths for asar
     to search.
@@ -288,15 +293,15 @@
     pp.patchloc = patch_name.encode()
     pp.romdata = ctypes.cast(rom_ptr, c_char_p)
     pp.buflen = maxromsize()
     pp.romlen = ctypes.pointer(romlen)
 
     # construct an array type of len(includepaths) elements and initialize
     # it with elements from includepaths
-    pp.includepaths = (c_char_p*len(includepaths))(*includepaths)
+    pp.includepaths = (c_char_p * len(includepaths))(*includepaths)
     pp.numincludepaths = len(includepaths)
 
     defines = (_definedata * len(additional_defines))()
     for i, (k, v) in enumerate(additional_defines.items()):
         defines[i].name = k.encode()
         defines[i].contents = v.encode()
     pp.additional_defines = defines
@@ -407,14 +412,15 @@
     return _getall(_asar.dll.asar_getwrittenblocks)
 
 
 def getmapper():
     """Get the ROM mapper currently used by Asar."""
     return mappertype(_asar.dll.asar_getmapper())
 
+
 def getsymbolsfile(fmt="wla"):
     """Generates the contents of a symbols file for in a specific format.
 
     Returns the textual contents of the symbols file.
     format specified the format of the symbols file that gets generated.
     """
     return _asar.dll.asar_getsymbolsfile(fmt.encode()).decode()
```

### Comparing `iog-randomizer-4.7.2.2/randomizer/classes.py` & `iog_randomizer-5.0.0/src/iog_randomizer/randomizer/classes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,47 @@
-import copy
+import itertools
+import random
 import time
 from datetime import datetime
-import binascii
-import random
-import itertools
 
-#from .models.enums.start_location import StartLocation
-#from .models.enums.goal import Goal
-#from .models.enums.statue_req import StatueReq
-#from .models.enums.entrance_shuffle import EntranceShuffle
-#from .models.enums.dungeon_shuffle import DungeonShuffle
-#from .models.enums.orb_rando import OrbRando
-#from .models.enums.darkrooms import DarkRooms
-#from .models.enums.enemizer import Enemizer
-#from .models.enums.flute import FluteOpt
-#from .models.enums.logic import Logic
 from .models.enums import *
 from .models.randomizer_data import RandomizerData
 
 MAX_INVENTORY = 15
 PROGRESS_ADJ = [1.5, 1.25, 1.0, 0.75]  # Required items are more likely to be placed in easier modes
 MAX_CYCLES = 200
 
 
 class World:
     # Severity: 0 = error/breakpoint, 1 = warning, 2 = info, 3 = verbose.
     def log(self, message, severity=0):
         prefixes = ["Error: ", "Warning: ", "", ""]
         prefix = prefixes[severity]
         if severity <= 1:
-            self.errorlog.append(prefix+message)
+            self.errorlog.append(prefix + message)
         if severity <= self.printlevel:
-            print(prefix+message)
+            print(prefix + message)
         return
+
     # Aliases, if using them is clearer to you
     def verbose(self, message):
         return self.log(message, 3)
+
     def info(self, message):
         return self.log(message, 2)
+
     def warn(self, message):
         return self.log(message, 1)
+
     def error(self, message):
         self.log(message, 0)
         if self.break_on_error:
             breakpoint()
         return
-    
+
     # Some basic validations for profiling
     def validate(self):
         val_messages = []
         val_success = True
         placed_item_counts = {}
         for loc in self.item_locations:
             item = self.item_locations[loc][3]
@@ -59,74 +51,77 @@
             if self.item_pool[item][6] == 0 and loc_pool == 0:
                 continue
             if item not in placed_item_counts:
                 placed_item_counts[item] = 0
             placed_item_counts[item] += 1
             if item not in self.item_pool:
                 val_success = False
-                val_messages.append("Item val error: Loc "+str(loc)+" contains deleted item "+str(item))
+                val_messages.append("Item val error: Loc " + str(loc) + " contains deleted item " + str(item))
             elif self.item_pool[item][6] != loc_pool:
                 val_success = False
-                val_messages.append("Item val error: Pool of loc "+str(loc)+" doesn't match pool of item "+str(item))
+                val_messages.append(
+                    "Item val error: Pool of loc " + str(loc) + " doesn't match pool of item " + str(item))
         for item in placed_item_counts:
             if placed_item_counts[item] != self.base_item_counts[item]:
                 val_success = False
-                val_messages.append("Item val error: Item "+str(item)+" placed "+str(placed_item_counts[item])+" times but expected "+str(self.base_item_counts[item]))
+                val_messages.append("Item val error: Item " + str(item) + " placed " + str(
+                    placed_item_counts[item]) + " times but expected " + str(self.base_item_counts[item]))
         if val_success:
             val_messages.append("Item val passed")
         val_success = True
         if self.orb_rando != "None" and not self.dungeon_shuffle:
             # Check whether certain problem orbs are locked behind themselves
-            for eddg_end_loc in [17,18,19,705,706]:
+            for eddg_end_loc in [17, 18, 19, 705, 706]:
                 if eddg_end_loc in self.item_locations and self.item_locations[eddg_end_loc][3] == 704:
                     val_success = False
                     val_messages.append("Orb val error: EdDg DS orb is inaccessible")
                     break
         if val_success:
             val_messages.append("Orb val passed")
         return val_messages
-    
+
     # Assigns item to location
-    def fill_item(self, item, location=-1,test=False,override_restrictions=False):
+    def fill_item(self, item, location=-1, test=False, override_restrictions=False):
         if location == -1:
             return False
         elif self.item_locations[location][2]:
-            self.verbose("Tried to place an item in a full location: "+str(self.item_pool[item][3])+" "+str(self.item_locations[location][6]))
+            self.verbose("Tried to place an item in a full location: " + str(self.item_pool[item][3]) + " " + str(
+                self.item_locations[location][6]))
             return False
         elif item in self.item_locations[location][4] and not override_restrictions:
-            self.verbose("Tried to place item in a restricted location: "+str(self.item_pool[item][3])+" "+str(self.item_locations[location][6]))
+            self.verbose("Tried to place item in a restricted location: " + str(self.item_pool[item][3]) + " " + str(
+                self.item_locations[location][6]))
             return False
         elif test:
             return True
 
         self.item_pool[item][0] -= 1
         self.item_locations[location][2] = True
         self.item_locations[location][3] = item
 
-        self.verbose("  "+str(self.item_pool[item][3])+" -> "+str(self.item_locations[location][6]))
+        self.verbose("  " + str(self.item_pool[item][3]) + " -> " + str(self.item_locations[location][6]))
 
         if self.is_accessible(self.item_locations[location][0]):
             self.items_collected.append(item)
             self.open_locations[self.item_locations[location][7]].remove(location)
 
         self.placement_log.append([item, location])
         return True
 
-
     # Removes an assigned item and returns it to item pool
     def unfill_item(self, location=-1):
         if location not in self.item_locations or not self.item_locations[location][2]:
             return -1
 
         item = self.item_locations[location][3]
         self.item_locations[location][2] = False
         self.item_locations[location][3] = 0
         self.item_pool[item][0] += 1
 
-        self.verbose("  "+str(self.item_pool[item][3])+"<-"+str(self.item_locations[location][6])+" removed")
+        self.verbose("  " + str(self.item_pool[item][3]) + "<-" + str(self.item_locations[location][6]) + " removed")
 
         if self.is_accessible(self.item_locations[location][0]):
             if item in self.items_collected:
                 self.items_collected.remove(item)
             pool = self.get_pool_id(item=item)
             if location not in self.open_locations[pool]:
                 self.open_locations[pool].append(location)
@@ -147,27 +142,28 @@
                 type = self.item_locations[loc][1]
             else:
                 return 0
         if type == 1:
             return 1
         elif type == 2:
             return 2
-        #elif type == 3:
+        # elif type == 3:
         #    pass   # Statues aren't shuffled
-        #elif type == 4:
+        # elif type == 4:
         #    pass   # Artificial event flags aren't shuffled
         elif type == 5:
             if self.orb_rando == "Basic":
                 return 5
             elif self.orb_rando == "Orbsanity":
                 return 1
         elif type > self.get_max_pool_id():
-            self.error("Type "+str(type)+" exceeds max pool ID")
+            self.error("Type " + str(type) + " exceeds max pool ID")
             return 0
         return 0
+
     # Many lists are instantiated with one element per pool, so we need to know how
     # large to make those lists. This constant is validated via get_pool_id.
     def get_max_pool_id(self):
         return 6
 
     # Returns whether the item and location are in the same shuffle pool
     def are_item_loc_pooled(self, item, loc):
@@ -182,14 +178,15 @@
                     if not shuffled_only or self.item_pool[x][6] > 0:
                         for _ in range(self.item_pool[x][0]):
                             item_list.append(x)
                         if incl_placed:
                             for _ in [loc for loc in self.item_locations if self.item_locations[loc][3] == x]:
                                 item_list.append(x)
         return item_list
+
     # Get list of items shuffled with given or all types, of any or all progression types.
     # If shuffled_only, items that aren't randomized (based on seed settings) are omitted.
     def list_pooled_items(self, types, progress_type=0, shuffled_only=False, incl_placed=False):
         if not types:
             return self.list_typed_items([], progress_type, shuffled_only, incl_placed)
         pools = set(self.get_pool_id(type=x) for x in types)
         item_list = []
@@ -229,158 +226,154 @@
         for x in sublist:
             if x in l:
                 l.remove(x)
             else:
                 return False
         return True
 
-
     # Returns graph node of an item location
     def location_node(self, location_id=-1):
         if location_id not in self.item_locations:
-            self.error("Invalid item location "+str(location_id))
+            self.error("Invalid item location " + str(location_id))
             return False
         else:
             return self.item_locations[location_id][0]
 
-
     # Returns whether an item location is already filled with an item
     def is_filled(self, location_id=-1):
         if location_id not in self.item_locations:
-            self.error("Invalid item location "+str(location_id))
+            self.error("Invalid item location " + str(location_id))
             return False
         else:
             return self.item_locations[location_id][2]
 
-
     # Returns whether the node is within the currently-accessible subgraph
     def is_accessible(self, node_id=-1):
         if node_id not in self.graph:
             return False
         elif self.graph[node_id][0]:
             return True
         else:
             return False
 
-
     # Zeroes out accessible flags for all world regions
-    def unsolve(self,reset_graph=False):
+    def unsolve(self, reset_graph=False):
         for x in self.graph:
             self.graph[x][0] = False
             if reset_graph:
                 self.graph[x][4] = 0
                 self.graph[x][8].clear()
                 self.graph[x][9].clear()
                 self.graph[x][10] = self.graph[x][1][:]
         for x in self.logic:
             if self.logic[x][0] == 1:
                 self.logic[x][0] = 0
         return True
 
-
     # Resets collected items and other traversal data
-    def reset_progress(self,reset_graph=False):
+    def reset_progress(self, reset_graph=False):
         self.visited.clear()
         self.items_collected.clear()
         self.item_destinations.clear()
-        self.open_locations = [ [] for _ in range(self.item_pool_count)]
+        self.open_locations = [[] for _ in range(self.item_pool_count)]
         self.open_edges = []
         self.unsolve(reset_graph)
         return True
 
-
     # Returns every accessible node from to_visit. Marks edges as traversed. 
     # If not test: marks nodes as traversed, collects self.items_collected/self.open_edges,
     # adds graph connections, and updates DS access.
     # Bug: if W can't reach a ForceWillForm node but F/S can, this traverses the node without propagating any
     # form access. I think currently this just causes a small number of boss shuffle + ER seeds to be
     # incorrectly rejected as unwinnable.
-    def traverse(self,to_visit=[],test=False):
+    def traverse(self, to_visit=[], test=False):
         self.verbose(" Beginning traversal...")
         visited = []
         new_items = []
         if not to_visit:
             to_visit.append(0)
         while to_visit:
             node = to_visit.pop(0)
             visited.append(node)
-            self.verbose("  Visiting node "+str(node)+" "+str(self.graph[node][5]))
+            self.verbose("  Visiting node " + str(node) + " " + str(self.graph[node][5]))
             # If we haven't been here yet...
             if not self.graph[node][0]:
                 # Get the newly-accessible items and record open item/ability locations
-                new_items += self.visit_node(node,test)
+                new_items += self.visit_node(node, test)
                 # Queue up newly-accessible nodes to visit
                 for x in self.graph[node][1]:
-                    if x != node and x not in to_visit+visited:
-                        to_visit.insert(0,x)
-                        self.verbose("  -Found node "+str(x)+" "+str(self.graph[x][5]))
+                    if x != node and x not in to_visit + visited:
+                        to_visit.insert(0, x)
+                        self.verbose("  -Found node " + str(x) + " " + str(self.graph[x][5]))
             # Propagate form access
             if not test:
                 self.update_ds_access([node], self.graph[node][4], self.graph[node][9])
             # If we've run out of nodes to visit, check if logic has opened up any new nodes
             if not to_visit:
-                open_edges = self.get_open_edges(visited,True)
+                open_edges = self.get_open_edges(visited, True)
                 bad_edges = []
-                #self.verbose(" All known nodes checked. Traversing edges...")
+                # self.verbose(" All known nodes checked. Traversing edges...")
                 for edge in open_edges:
                     origin = self.logic[edge][1]
                     dest = self.logic[edge][2]
                     if self.check_edge(edge, [], not test, self.graph[origin][4]):
                         self.logic[edge][0] = 1
                         if dest not in to_visit:
                             to_visit.append(dest)
-                            self.verbose("  -Found node "+str(dest)+" "+str(self.graph[dest][5]))
+                            self.verbose("  -Found node " + str(dest) + " " + str(self.graph[dest][5]))
                     else:
                         bad_edges.append(edge)
                 if not test:
                     self.open_edges = bad_edges
-        return [visited,new_items]
-
+        return [visited, new_items]
 
     # Return list of logic edges that originate in an accessible node in nodes, and
     # either are locked or terminate outside of nodes.
     # include_redundant to include edges whose destination is already traversed.
-    def get_open_edges(self,nodes=[],include_redundant=False):
+    def get_open_edges(self, nodes=[], include_redundant=False):
         test_edges = self.open_edges[:]
         open_edges = []
         for x in nodes:
             if not self.is_accessible(x):
                 test_edges += self.graph[x][12]
         for edge in test_edges:
             origin = self.logic[edge][1]
             dest = self.logic[edge][2]
-            if (self.logic[edge][0] >= 0) and (edge not in open_edges) and (not self.is_accessible(dest) or self.graph[origin][4] != self.graph[dest][4] or include_redundant) and (dest not in nodes or self.logic[edge][0] == 0):
+            if (self.logic[edge][0] >= 0) and (edge not in open_edges) and (
+                    not self.is_accessible(dest) or self.graph[origin][4] != self.graph[dest][
+                4] or include_redundant) and (dest not in nodes or self.logic[edge][0] == 0):
                 open_edges.append(edge)
         return open_edges
 
-
     # Visit a node, update graph info, return new items collected
-    def visit_node(self,node,test=False):
+    def visit_node(self, node, test=False):
         if not test and not self.graph[node][0]:
             self.graph[node][0] = True
             self.visited.append(node)
             self.item_destinations += self.graph[node][6]
             self.open_edges += self.graph[node][12]
-        return self.collect_items(node,test)
-
+        return self.collect_items(node, test)
 
     # Collect all items in given node
-    def collect_items(self,node=-1,test=False):
+    def collect_items(self, node=-1, test=False):
         if node not in self.graph:
             return False
         items_found = []
         for location in self.graph[node][11]:
             if self.item_locations[location][2]:
                 items_found.append(self.item_locations[location][3])
                 if not test:
                     self.items_collected.append(self.item_locations[location][3])
-                self.verbose("  -Got item "+str(self.item_locations[location][3])+" "+str(self.item_pool[self.item_locations[location][3]][3])+" from loc "+str(location)+" "+str(self.item_locations[location][6]).strip()+" in node "+str(node)+" "+str(self.graph[node][5]).strip())
+                self.verbose("  -Got item " + str(self.item_locations[location][3]) + " " + str(
+                    self.item_pool[self.item_locations[location][3]][3]) + " from loc " + str(location) + " " + str(
+                    self.item_locations[location][6]).strip() + " in node " + str(node) + " " + str(
+                    self.graph[node][5]).strip())
             elif not test:
                 self.open_locations[self.item_locations[location][7]].append(location)
-                #self.verbose("  -Found empty loc "+str(location)+" "+str(self.item_locations[location][6]))
+                # self.verbose("  -Found empty loc "+str(location)+" "+str(self.item_locations[location][6]))
         return items_found
 
     # Returns full list of accessible locations
     def accessible_locations(self, item_locations):
         accessible = []
         for x in item_locations:
             region = self.item_locations[x][0]
@@ -409,77 +402,78 @@
 
         while to_place:
             item = to_place.pop(0)
             for dest in to_fill:
                 region = self.item_locations[dest][0]
                 filled = self.item_locations[dest][2]
                 restrictions = self.item_locations[dest][4]
-                if not filled and self.are_item_loc_pooled(item,dest) and item not in restrictions:
+                if not filled and self.are_item_loc_pooled(item, dest) and item not in restrictions:
                     if not accessible or region >= 0:
                         if self.fill_item(item, dest, False, False):
                             to_fill.remove(dest)
                             break
 
         return True
 
     # Place list of items into random accessible locations
     def forward_fill(self, items=[], item_locations=[], test=False, override_restrictions=False, impose_penalty=False):
         if not items:
             return True
         elif not item_locations:
-            #self.verbose("forward_fill given items but no locations")
+            # self.verbose("forward_fill given items but no locations")
             return False
 
         to_place = items[:]
         if impose_penalty and not any(self.item_pool[item][7] > 0 for item in to_place):
-            impose_penalty = False   # Don't go through penalty code if there are no penalized items
-        if impose_penalty:   # More restrictive items are placed first
-            to_place.sort(key=lambda item : -1*self.item_pool[item][7])
-        to_fill = [ [] for _ in range(self.item_pool_count)]
-        loc_quarantine = [ [] for _ in range(self.item_pool_count)]
+            impose_penalty = False  # Don't go through penalty code if there are no penalized items
+        if impose_penalty:  # More restrictive items are placed first
+            to_place.sort(key=lambda item: -1 * self.item_pool[item][7])
+        to_fill = [[] for _ in range(self.item_pool_count)]
+        loc_quarantine = [[] for _ in range(self.item_pool_count)]
         for pool in range(self.item_pool_count):
-            to_fill[pool] = [loc for loc in item_locations if self.item_locations[loc][7] == pool and not self.item_locations[loc][2] and self.is_accessible(self.item_locations[loc][0])]
-            if impose_penalty:   # Later locations are preferred by more restrictive items
-                to_fill[pool].sort(key=lambda loc : -1*self.item_locations[loc][8])
+            to_fill[pool] = [loc for loc in item_locations if
+                             self.item_locations[loc][7] == pool and not self.item_locations[loc][
+                                 2] and self.is_accessible(self.item_locations[loc][0])]
+            if impose_penalty:  # Later locations are preferred by more restrictive items
+                to_fill[pool].sort(key=lambda loc: -1 * self.item_locations[loc][8])
             else:
                 random.shuffle(to_fill[pool])
         filled_locations = []
         while to_place:
             item = to_place.pop(0)
             pool = self.item_pool[item][6]
             preferred_locs = []
             if impose_penalty and self.item_pool[item][7] > 0 and len(to_fill[pool]) > 3:
                 # Item penalty N ignores the earliest N deciles, if there are enough locs to do so
                 preferred_locs = [to_fill[pool][0]]
-                priority_cutoff = len(to_fill[pool]) * (1.0 - (float(self.item_pool[item][7]) / 10.0) )
+                priority_cutoff = len(to_fill[pool]) * (1.0 - (float(self.item_pool[item][7]) / 10.0))
                 while len(preferred_locs) < priority_cutoff:
                     preferred_locs.append(to_fill[pool][len(preferred_locs)])
             filled = False
             while not filled and (preferred_locs or to_fill[pool]):
                 if preferred_locs:
                     location = preferred_locs.pop()
                     to_fill[pool].remove(location)
                 else:
                     location = to_fill[pool].pop(0)
-                if self.fill_item(item,location,test,override_restrictions):
+                if self.fill_item(item, location, test, override_restrictions):
                     filled = True
                     filled_locations.append(location)
                     to_fill[pool] += loc_quarantine[pool]
                 else:
                     loc_quarantine[pool].append(location)
             if not filled:
-                self.verbose("Not enough room to place item "+str(item))
+                self.verbose("Not enough room to place item " + str(item))
                 if not test:
                     for loc in filled_locations:
                         self.unfill_item(loc)
                 return False
 
         return True
 
-
     # Convert a prerequisite to a list of items needed to fulfill it
     def items_needed(self, edge=0):
         if not edge:
             return []
 
         prereq = []
         for req in self.logic[edge][4]:
@@ -503,74 +497,75 @@
             else:
                 prereq_new.append(x)
 
         return prereq_new
 
     # Returns list of item combinations that grant progression
     # Returns progression list in the following categories: [[available],[not enough room],[too many inventory items]]
-    def progression_list(self,open_edges=[],ignore_inv=False,penalty_threshold=MAX_CYCLES):
+    def progression_list(self, open_edges=[], ignore_inv=False, penalty_threshold=MAX_CYCLES):
         if not open_edges:
             open_edges = self.get_open_edges()
-        all_items = [item for item in self.list_pooled_items(types=[], shuffled_only=True) if self.item_pool[item][7] <= penalty_threshold]
-        prereq_list = [[],[],[]]    # [[available],[not enough room],[too many inventory items]]
+        all_items = [item for item in self.list_pooled_items(types=[], shuffled_only=True) if
+                     self.item_pool[item][7] <= penalty_threshold]
+        prereq_list = [[], [], []]  # [[available],[not enough room],[too many inventory items]]
         ds_list = []
 
         for edge in open_edges:
             prereq = self.items_needed(edge)
             if prereq and prereq not in prereq_list[0] and self.is_sublist(all_items, prereq):
                 all_open_locs = []
                 for locpool in self.open_locations:
                     all_open_locs.extend(locpool)
-                if prereq not in prereq_list[1] and not self.forward_fill(prereq,all_open_locs,True,self.logic_mode == "Chaos"):
+                if prereq not in prereq_list[1] and not self.forward_fill(prereq, all_open_locs, True,
+                                                                          self.logic_mode == "Chaos"):
                     prereq_list[1].append(prereq)
                 elif prereq not in prereq_list[2]:
                     dest = self.logic[edge][2]
-                    traverse_result = self.traverse([dest],True)
+                    traverse_result = self.traverse([dest], True)
                     new_nodes = traverse_result[0]
                     start_items_temp = self.items_collected[:] + prereq + traverse_result[1]
                     item_destinations_temp = self.item_destinations[:]
                     for x in new_nodes:
                         item_destinations_temp += self.graph[x][6]
-                    inv_temp = self.get_inventory(start_items_temp,item_destinations_temp)
+                    inv_temp = self.get_inventory(start_items_temp, item_destinations_temp)
                     if ignore_inv or len(inv_temp) <= MAX_INVENTORY:
-                        if True:# not self.entrance_shuffle or self.check_ds_access(dest,0x10,True,[]):
+                        if True:  # not self.entrance_shuffle or self.check_ds_access(dest,0x10,True,[]):
                             prereq_list[0].append(prereq)
                         else:
                             ds_list.append(prereq)
                     else:
                         prereq_list[2].append(prereq)
 
-        if prereq_list == [[],[],[]]:
+        if prereq_list == [[], [], []]:
             prereq_list[0] += ds_list
 
         return prereq_list
 
-
-
     # Remove a non-progression item to make room for a progression item.
     # Only works on type-1 items and type-1 locations.
     def make_room(self, progression_result):
         # For inventory bottlenecks, remove one inventory item and try again
         if not progression_result[1] and progression_result[2]:
-            return self.remove_nonprog(1,True)
+            return self.remove_nonprog(1, True)
         for node in self.visited:
             for x in self.graph[node][11]:
-                if self.is_filled(x) and self.item_locations[x][7]==1 and self.item_pool[self.item_locations[x][3]][5]>1 and self.item_pool[self.item_locations[x][3]][6]==1:
+                if self.is_filled(x) and self.item_locations[x][7] == 1 and self.item_pool[self.item_locations[x][3]][
+                    5] > 1 and self.item_pool[self.item_locations[x][3]][6] == 1:
                     if self.unfill_item(x):
                         return True
         return False
 
-
     # Remove accessible non-progression items to make room for a progression item.
-    def remove_nonprog(self,item_ct=0,inv=False):
+    def remove_nonprog(self, item_ct=0, inv=False):
         junk_locations = []
         quest_locations = []
 
         for location in self.item_locations:
-            if self.item_locations[location][2] and self.item_locations[location][7]==1 and self.is_accessible(self.item_locations[location][0]):
+            if self.item_locations[location][2] and self.item_locations[location][7] == 1 and self.is_accessible(
+                    self.item_locations[location][0]):
                 item = self.item_locations[location][3]
                 prog_type = self.item_pool[item][5]
                 inv_type = self.item_pool[item][4]
                 if prog_type == 2:
                     quest_locations.append(location)
                 elif prog_type == 3:
                     if not inv or inv_type:
@@ -592,18 +587,17 @@
                     locations = quest_locations
                 if not locations:
                     self.error("No room for prog items and no nonprog items to remove")
                     return False
                 location = locations.pop(0)
                 items_removed.append(self.unfill_item(location))
                 count -= 1
-        self.verbose("   Removed nonprog items: "+str(items_removed))
+        self.verbose("   Removed nonprog items: " + str(items_removed))
         return items_removed
 
-
     # Converts a progression list into a normalized Monte Carlo distribution
     def monte_carlo(self, progression_ls=[], start_items=[]):
         if not progression_ls:
             return []
 
         progression = progression_ls[:]
 
@@ -655,43 +649,42 @@
         for x in probabilities:
             x[0] = x[0] * prob_adj + rolling_sum
             rolling_sum = x[0]
 
         # print probabilities
         return probabilities
 
-
     # Returns a list of map lists, by boss
     def get_maps(self):
         maps = [[], [], [], [], [], [], []]
         for map in self.maps:
-            if self.maps[map][0] >= 0 and (not self.dungeon_shuffle or not self.maps[map][8]):    # Jumbo maps don't get rewards in dungeon shuffles
+            if self.maps[map][0] >= 0 and (not self.dungeon_shuffle or not self.maps[map][
+                8]):  # Jumbo maps don't get rewards in dungeon shuffles
                 boss = self.maps[map][1]
                 maps[boss].append(map)
-        maps.pop(0)    # Non-dungeon maps aren't included
+        maps.pop(0)  # Non-dungeon maps aren't included
         return maps
 
-
     # Randomize map-clearing rewards
     def map_rewards(self):
         maps = self.get_maps()
         for area in maps:
             random.shuffle(area)
 
         # Total rewards by type, by level (HP/STR/DEF)
         if "Z3 Mode" in self.variant:
-            rewards_tier1 = [1] * 6    # Expert: 6 HP
-            rewards_tier2 = [1] * 6    # Advanced: 12 HP
-            rewards_tier3 = [1] * 6    # Intermediate: 18 HP
-            rewards_tier4 = []         # Beginner: 18 HP
+            rewards_tier1 = [1] * 6  # Expert: 6 HP
+            rewards_tier2 = [1] * 6  # Advanced: 12 HP
+            rewards_tier3 = [1] * 6  # Intermediate: 18 HP
+            rewards_tier4 = []  # Beginner: 18 HP
         else:  # Remove all HP upgrades
-            rewards_tier1 = [1,1,1,1,1,1]    # Expert: 6/0/0
-            rewards_tier2 = [1,1,2,2,3,3]    # Advanced: 8/2/2
-            rewards_tier3 = [1,1,2,2,3,3]    # Intermediate: 10/4/4
-            rewards_tier4 = [2,2,2,3,3,3]    # Beginner: 10/7/7
+            rewards_tier1 = [1, 1, 1, 1, 1, 1]  # Expert: 6/0/0
+            rewards_tier2 = [1, 1, 2, 2, 3, 3]  # Advanced: 8/2/2
+            rewards_tier3 = [1, 1, 2, 2, 3, 3]  # Intermediate: 10/4/4
+            rewards_tier4 = [2, 2, 2, 3, 3, 3]  # Beginner: 10/7/7
 
         # Remove HP upgrades in OHKO
         if "OHKO" in self.variant:
             for n, i in enumerate(rewards_tier1):
                 if i == 1:
                     rewards_tier1[n] = 0
             for n, i in enumerate(rewards_tier2):
@@ -708,49 +701,46 @@
         random.shuffle(rewards_tier2)
         random.shuffle(rewards_tier3)
         random.shuffle(rewards_tier4)
 
         # Allocate rewards to maps
         for area in maps:
             random.shuffle(area)
-            self.maps[area[0]][2] = [rewards_tier1.pop(0),1]
-            self.maps[area[1]][2] = [rewards_tier2.pop(0),2]
-            self.maps[area[2]][2] = [rewards_tier3.pop(0),3]
+            self.maps[area[0]][2] = [rewards_tier1.pop(0), 1]
+            self.maps[area[1]][2] = [rewards_tier2.pop(0), 2]
+            self.maps[area[2]][2] = [rewards_tier3.pop(0), 3]
             if rewards_tier4:
-                self.maps[area[3]][2] = [rewards_tier4.pop(0),4]
+                self.maps[area[3]][2] = [rewards_tier4.pop(0), 4]
             else:
-                self.maps[area[3]][2] = [0,4]
-
+                self.maps[area[3]][2] = [0, 4]
 
     # Place Mystic Statues in World
     def fill_statues(self, locations=[148, 149, 150, 151, 152, 153]):
         if self.statue_req == StatueReq.PLAYER_CHOICE.value:
-            return self.random_fill([106]*6, locations)
+            return self.random_fill([106] * 6, locations)
         return self.random_fill([100, 101, 102, 103, 104, 105], locations)
 
-
     # If the vanilla exit is two-way (i.e. has a paired exit), returns the paired exit.
     # Otherwise, returns 0 to indicate the exit is one-way or doesn't exist.
-    def is_exit_coupled(self,exit):
+    def is_exit_coupled(self, exit):
         if exit not in self.exits:
             return 0
         if self.exits[exit][0]:
             sister_exit = self.exits[exit][0]
             if self.exits[sister_exit][0] == exit:
                 return sister_exit
             else:
-                self.warn("Exits linked incorrectly "+str(exit)+" "+str(sister_exit))
+                self.warn("Exits linked incorrectly " + str(exit) + " " + str(sister_exit))
                 return sister_exit
         return 0
 
-
     # Determine an exit's direction (e.g. outside to inside).
     # An exit from a "roof" (type-3 node) always counts as going outside,
     # to discourage attaching dead-end interior rooms to roof exits.
-    def exit_direction(self,exit):
+    def exit_direction(self, exit):
         if exit not in self.exits:
             return False
         origin = self.exits[exit][3]
         dest = self.exits[exit][4]
         if self.graph[origin][2] == 2:
             o_type = 2
         else:
@@ -759,153 +749,160 @@
             d_type = 1
         else:
             if self.graph[dest][2] == 2:
                 d_type = 2
             else:
                 d_type = 1
         if o_type == 2 and d_type == 2:
-            return (1,1)
+            return (1, 1)
         else:
             return d_type
 
-
     # Link one exit to another, making origin_exit act like dest_exit; that is,
     # replace the transition data of origin_exit with the vanilla transition data of dest_exit.
     def link_exits(self, origin_exit, dest_exit, check_connections=True, update_graph=True):
         if origin_exit not in self.exits:
-            self.error("Invalid origin (link) "+str(origin_exit))
+            self.error("Invalid origin (link) " + str(origin_exit))
             return False
         if dest_exit not in self.exits:
-            self.error("Invalid destination (link) "+str(dest_exit))
+            self.error("Invalid destination (link) " + str(dest_exit))
             return False
         if self.exits[origin_exit][1] > 0 and origin_exit > 21:
-            self.error("Origin already linked: "+str(origin_exit)+" "+str(self.exits[origin_exit]))
+            self.error("Origin already linked: " + str(origin_exit) + " " + str(self.exits[origin_exit]))
             return False
         if self.exits[dest_exit][2] > 0 and dest_exit > 21:
-            self.error("Destination already linked: "+str(dest_exit)+" "+str(self.exits[dest_exit]))
+            self.error("Destination already linked: " + str(dest_exit) + " " + str(self.exits[dest_exit]))
             return False
         self.exits[origin_exit][1] = dest_exit
         self.exits[dest_exit][2] = origin_exit
-        self.exit_log.append([origin_exit,dest_exit])
-        self.verbose("   Linked "+str(origin_exit)+" "+str(self.exits[origin_exit][10])+" - "+str(dest_exit)+" "+str(self.exits[dest_exit][10]))
+        self.exit_log.append([origin_exit, dest_exit])
+        self.verbose("   Linked " + str(origin_exit) + " " + str(self.exits[origin_exit][10]) + " - " + str(
+            dest_exit) + " " + str(self.exits[dest_exit][10]))
         if update_graph and self.exits[origin_exit][5]:
             origin = self.exits[origin_exit][3]
             dest = self.exits[dest_exit][4]
             if dest not in self.graph[origin][1]:
                 self.graph[origin][1].append(dest)
-            self.new_connection(origin,dest,0)
+            self.new_connection(origin, dest, 0)
             if self.is_accessible(origin) and not self.is_accessible(dest):
-                self.traverse([dest],test=False)
-        if (origin_exit <= 21 or self.coupled_exits) and check_connections and self.is_exit_coupled(origin_exit) and self.is_exit_coupled(dest_exit):
+                self.traverse([dest], test=False)
+        if (origin_exit <= 21 or self.coupled_exits) and check_connections and self.is_exit_coupled(
+                origin_exit) and self.is_exit_coupled(dest_exit):
             new_origin = self.exits[dest_exit][0]
             new_dest = self.exits[origin_exit][0]
             if new_origin <= 21:  # Boss exits
                 if self.exits[new_origin][5]:
                     self.link_exits(new_origin, new_dest, False, update_graph)
             else:
                 if self.exits[new_origin][1] != -1 or self.exits[new_dest][2] != -1:
-                    self.error("Return exit already linked: "+str(new_origin)+" "+str(new_dest))
+                    self.error("Return exit already linked: " + str(new_origin) + " " + str(new_dest))
                     return False
                 else:
                     self.link_exits(new_origin, new_dest, False, update_graph)
         return True
 
-
     # Unlinks two previously linked exits
     def unlink_exits(self, origin_exit, dest_exit, check_connections=True, update_graph=True):
         if origin_exit not in self.exits:
-            self.error("Invalid origin (unlink) "+str(origin_exit))
+            self.error("Invalid origin (unlink) " + str(origin_exit))
             return False
         if dest_exit and dest_exit not in self.exits:
-            self.error("Invalid destination (unlink) "+str(dest_exit))
+            self.error("Invalid destination (unlink) " + str(dest_exit))
             return False
         if dest_exit and (self.exits[origin_exit][1] != dest_exit or self.exits[dest_exit][2] != origin_exit):
-            self.warn("Attempted to unlink exits that are not correctly linked: "+str(origin_exit)+" "+str(dest_exit))
+            self.warn(
+                "Attempted to unlink exits that are not correctly linked: " + str(origin_exit) + " " + str(dest_exit))
         if not dest_exit:
             dest_exit = origin_exit
         self.exits[origin_exit][1] = -1
         self.exits[dest_exit][2] = -1
         for x in self.exit_log:
             if x[0] == origin_exit:
                 self.exit_log.remove(x)
-        self.verbose("   Unlinked "+str(origin_exit)+" "+str(self.exits[origin_exit][10])+" - "+str(dest_exit)+" "+str(self.exits[dest_exit][10]))
+        self.verbose("   Unlinked " + str(origin_exit) + " " + str(self.exits[origin_exit][10]) + " - " + str(
+            dest_exit) + " " + str(self.exits[dest_exit][10]))
         if update_graph and self.exits[origin_exit][5]:
             origin = self.exits[origin_exit][3]
             dest = self.exits[dest_exit][4]
             if dest in self.graph[origin][1]:
                 self.graph[origin][1].remove(dest)
             if dest in self.graph[origin][10]:
                 self.graph[origin][10].remove(dest)
-        if self.coupled_exits and check_connections and self.is_exit_coupled(origin_exit) and self.is_exit_coupled(dest_exit):
+        if self.coupled_exits and check_connections and self.is_exit_coupled(origin_exit) and self.is_exit_coupled(
+                dest_exit):
             new_origin = self.exits[dest_exit][0]
             new_dest = self.exits[origin_exit][0]
             self.unlink_exits(new_origin, new_dest, False, update_graph)
         if check_connections and update_graph:
-            self.update_graph(True,True,True)
+            self.update_graph(True, True, True)
         return True
 
-
     # Bidirectional exit link. Make exit1 send the player to where exit2 is, and vice versa.
     def join_exits(self, exit1, exit2):
-        return (self.link_exits(exit1, self.exits[exit2][0], False, False) and self.link_exits(exit2, self.exits[exit1][0], False, False))
+        return (self.link_exits(exit1, self.exits[exit2][0], False, False) and self.link_exits(exit2,
+                                                                                               self.exits[exit1][0],
+                                                                                               False, False))
 
     # Unlink both sides of a bidirectional exit.
     def unjoin_exit(self, exit):
         linked_exit = self.exits[exit][1]
         joined_exit = self.exits[self.exits[exit][0]][2]
         joined_linked_exit = self.exits[joined_exit][1]
-        return (self.unlink_exits(exit, linked_exit, False, False) and self.unlink_exits(joined_exit, joined_linked_exit, False, False))
+        return (self.unlink_exits(exit, linked_exit, False, False) and self.unlink_exits(joined_exit,
+                                                                                         joined_linked_exit, False,
+                                                                                         False))
 
     # Append/insert bidirectional exits. Joins base_exit to new_exit1.
     # If base_exit was already joined, its former partner is joined to new_exit2.
-    def insert_exit(self, base_exit, new_exit1, new_exit2 = 0):
+    def insert_exit(self, base_exit, new_exit1, new_exit2=0):
         if any(x not in self.exits for x in [base_exit, new_exit1]) or (new_exit2 > 0 and new_exit2 not in self.exits):
-            self.error("Can't insert nonexistent exit, one of: "+str(base_exit)+" "+str(new_exit1)+" "+str(new_exit2))
+            self.error("Can't insert nonexistent exit, one of: " + str(base_exit) + " " + str(new_exit1) + " " + str(
+                new_exit2))
             return False
         if self.exits[new_exit1][1] > 0:
-            self.error("Can't insert exit that's already joined: "+str(new_exit1))
+            self.error("Can't insert exit that's already joined: " + str(new_exit1))
             return False
-        if self.exits[base_exit][1] < 0:   # Append.
+        if self.exits[base_exit][1] < 0:  # Append.
             return self.join_exits(base_exit, new_exit1)
-        else:   # Insert.
+        else:  # Insert.
             if (new_exit2 == 0) or (self.exits[new_exit2][1] > 0):
-                self.error("Can't insert nonexistent or joined exit: "+str(new_exit2))
+                self.error("Can't insert nonexistent or joined exit: " + str(new_exit2))
                 return False
             joined_exit = self.exits[self.exits[base_exit][0]][2]
             self.unjoin_exit(base_exit)
             return (self.join_exits(base_exit, new_exit1) and self.join_exits(joined_exit, new_exit2))
 
-
-    def print_exit_log(self,exit_log=[]):
-        for origin,dest in exit_log:
-            self.verbose(str(self.exits[origin][10])+" - "+str(self.exits[dest][10]))
-
+    def print_exit_log(self, exit_log=[]):
+        for origin, dest in exit_log:
+            self.verbose(str(self.exits[origin][10]) + " - " + str(self.exits[dest][10]))
 
     # Returns lists of origin exits and destination exits that open up new nodes
-    def get_open_exits(self,check_progression=False):
-        open_exits = [[],[]]
+    def get_open_exits(self, check_progression=False):
+        open_exits = [[], []]
         for node in self.graph:
             if not check_progression or self.is_accessible(node):
                 for exit in self.graph[node][14]:
                     if self.exits[exit][1] == -1:
                         open_exits[0].append(exit)
             if not check_progression or not self.is_accessible(node):
                 for exit in self.graph[node][15]:
                     if self.exits[exit][2] == -1:
                         open_exits[1].append(exit)
         return open_exits
 
-
     # Takes a list of origin and destination exits, returns a suitable match
-    def find_exit(self,origin_exits_ls=[],dest_exits_ls=[],check_direction=False,check_progression=False,check_ds_access=False,test=False):
+    def find_exit(
+        self, origin_exits_ls=[], dest_exits_ls=[], check_direction=False, check_progression=False,
+        check_ds_access=False, test=False
+    ):
         if not origin_exits_ls:
             self.verbose("  No more accessible exits available")
             return False
         elif not dest_exits_ls:
-            self.verbose("  No destination exits available from "+str(origin_exits_ls))
+            self.verbose("  No destination exits available from " + str(origin_exits_ls))
             return False
 
         origin_exits = origin_exits_ls[:]
         dest_exits = dest_exits_ls[:]
 
         done = False
         quarantine_o = []
@@ -926,57 +923,56 @@
             dest_exit = 0
             quarantine_d = []
             while not done and dest_exits:
                 try_link = False
                 while not dest_exit and dest_exits:
                     dest_exit = dest_exits.pop(0)
                     dest = self.exits[dest_exit][4]
-                    if self.exits[dest_exit][2] != -1 or not self.cmp_exit_pool(origin_exit, dest_exit) or (check_progression and self.is_accessible(dest)):
+                    if self.exits[dest_exit][2] != -1 or not self.cmp_exit_pool(origin_exit, dest_exit) or (
+                            check_progression and self.is_accessible(dest)):
                         dest_exit = 0
 
                 if not dest_exit:
-                    self.verbose("  No destination exits available from "+str(origin_exit))
+                    self.verbose("  No destination exits available from " + str(origin_exit))
                     return False
 
                 direction_new = self.exit_direction(dest_exit)
                 if dest_exit != sister_exit and (not check_direction or direction_new == direction):
                     try_link = True
                     if self.link_exits(origin_exit, dest_exit, self.coupled_exits, True):
-                        if True: # or not check_ds_access or self.check_ds_access(dest):
+                        if True:  # or not check_ds_access or self.check_ds_access(dest):
                             done = True
                             origin_final = origin_exit
                             dest_final = dest_exit
 
                 if not done:
                     quarantine_d.append(dest_exit)
                     if try_link:
-                        self.unlink_exits(origin_exit,dest_exit,True,True)
+                        self.unlink_exits(origin_exit, dest_exit, True, True)
                     dest_exit = 0
 
-
             if not done:
                 quarantine_o.append(origin_exit)
                 dest_exits += quarantine_d
                 quarantine_d.clear()
 
         if not done:
-            self.verbose("No suitable links could be found - in quarantine: "+str(quarantine_o))
+            self.verbose("No suitable links could be found - in quarantine: " + str(quarantine_o))
             return False
 
         # Clean up O/D lists
         origin_exits += quarantine_o
         for exit in origin_exits:
             if self.exits[exit][1] != -1:
                 origin_exits.remove(exit)
         for exit in dest_exits:
             if self.exits[exit][2] != -1:
                 dest_exits.remove(exit)
 
-        return [origin_final,dest_final,origin_exits,dest_exits]
-
+        return [origin_final, dest_final, origin_exits, dest_exits]
 
     # Check if player at origin could reach dest via open edges.
     def check_access(self, origin=-1, dest=-1, check_mutual=False, formless=False):
         if origin not in self.graph or dest not in self.graph:
             return False
         if self.graph[origin][7] or self.graph[dest][7]:
             return False
@@ -985,40 +981,40 @@
             success = True
         elif formless:
             to_visit = [origin]
             visited = []
             while not success and to_visit:
                 node = to_visit.pop()
                 visited.append(node)
-                if self.graph[node][7]:   # Will-Only nodes don't propagate formless access
+                if self.graph[node][7]:  # Will-Only nodes don't propagate formless access
                     continue
                 elif node == dest:
                     success = True
                     break
                 else:
-                    to_visit.extend([n for n in self.graph[node][1] if n not in visited+to_visit])
+                    to_visit.extend([n for n in self.graph[node][1] if n not in visited + to_visit])
                     for edge in self.graph[node][12]:
-                        if (self.logic[edge][0] > 0) and self.edge_formless(edge) and (self.logic[edge][2] not in visited+to_visit):
+                        if (self.logic[edge][0] > 0) and self.edge_formless(edge) and (
+                                self.logic[edge][2] not in visited + to_visit):
                             to_visit.append(self.logic[edge][2])
         else:
             to_visit = self.graph[origin][10][:]
             visited = [origin]
             while not success and to_visit:
                 node = to_visit.pop(0)
                 visited.append(node)
                 if not self.graph[node][7] and dest in self.graph[node][10]:
                     success = True
                 else:
                     for x in self.graph[node][10]:
-                        if x not in to_visit+visited:
+                        if x not in to_visit + visited:
                             to_visit.append(x)
         if not check_mutual or not success:
             return success
-        return self.check_access(dest,origin,False,formless)
-
+        return self.check_access(dest, origin, False, formless)
 
     # Build islands, i.e. groups of nodes accessible from each other, generally assuming all progression.
     # With require_mutual, island nodes are mutually accessible, with no one-way drops or similar.
     # Examples: Freejia-Exterior; north half of Sky Garden SW Top.
     def build_islands(self, require_mutual=True):
         islands = [[] for _ in range(13)]
         visited = []
@@ -1038,56 +1034,55 @@
                     visited.append(x)
                     new_nodes.append(x)
                     if 0 in self.graph[x][8]:
                         is_start = True
                     for exit in self.graph[x][14]:
                         if self.exits[exit][1] == -1:
                             origin_exits.append(exit)
-                            dungeon = min(dungeon,self.exit_dungeon(exit))
+                            dungeon = min(dungeon, self.exit_dungeon(exit))
                     for exit in self.graph[x][15]:
                         if self.exits[exit][2] == -1:
                             dest_exits.append(exit)
                     for edge in self.graph[x][12]:
                         if self.logic[edge][0] == 0:
                             origin_logic.append(edge)
                     for edge in self.graph[x][13]:
                         if self.logic[edge][0] == 0:
                             dest_logic.append(edge)
                     for y in self.graph[x][10]:
-                        if y not in visited+to_visit and self.check_access(x,y,require_mutual):
+                        if y not in visited + to_visit and self.check_access(x, y, require_mutual):
                             to_visit.append(y)
                     if not require_mutual:
                         for y in self.graph[x][8]:
-                            if y not in visited+to_visit and self.check_access(y,x,False):
+                            if y not in visited + to_visit and self.check_access(y, x, False):
                                 to_visit.append(y)
-                island = [new_nodes,origin_exits,dest_exits,origin_logic,dest_logic]
+                island = [new_nodes, origin_exits, dest_exits, origin_logic, dest_logic]
                 if is_start:
                     start_island = island
                 if dungeon == 9999 or not self.dungeon_shuffle:
                     dungeon = 0
                 islands[dungeon].append(island)
 
-        return [start_island,islands]
+        return [start_island, islands]
 
-
-    def exit_dungeon(self,exit=-1):
+    def exit_dungeon(self, exit=-1):
         if exit not in self.exits:
             self.error("Exit not in database")
             return -1
-        if self.dungeon_shuffle:# == "Chaos":
+        if self.dungeon_shuffle:  # == "Chaos":
             return 1
         return self.exits[exit][8]
 
-    def check_dungeon(self,exit1=-1,exit2=-1):
+    def check_dungeon(self, exit1=-1, exit2=-1):
         if exit1 not in self.exits or exit2 not in self.exits:
             self.error("Exit not in database")
             return -1
         if self.exit_dungeon(exit1) != self.exit_dungeon(exit2):
             return False
-        #if self.dungeon_shuffle != "Chaos":   # Only link Mu rooms of the same water level
+        # if self.dungeon_shuffle != "Chaos":   # Only link Mu rooms of the same water level
         #    origin1 = self.exits[exit1][3]
         #    origin2 = self.exits[exit2][3]
         #    dest1 = self.exits[exit1][4]
         #    dest2 = self.exits[exit2][4]
         #    if self.graph[origin1][3][2] != self.graph[origin2][3][2] or self.graph[dest1][3][2] != self.graph[dest2][3][2]:
         #        return False
         return True
@@ -1096,46 +1091,47 @@
     # Otherwise returns the (arbitrary) ID of the pool it should be shuffled with, based on self.exits:
     # ER, no DS:  PoolType=1; one pool
     # ER and DSB: PoolType>0; pool all having PoolType=1, then pool PoolType>1 by DungeonID
     # ER and DSC: PoolType>0; pool by PoolType
     # DSB, no ER: PoolType>1, DungeonID>0; pool by DungeonID
     # DSC, no ER: PoolType>1, DungeonID>0; one pool
     def get_exit_pool(self, exit):
-        if (exit not in self.exits) or not self.entrance_shuffle: # (self.entrance_shuffle == "None" and self.dungeon_shuffle == "None"):
+        if (
+                exit not in self.exits) or not self.entrance_shuffle:  # (self.entrance_shuffle == "None" and self.dungeon_shuffle == "None"):
             return -1
         dungeon = self.exits[exit][8]
         pooltype = self.exits[exit][9]
-        ER = self.town_shuffle #(self.entrance_shuffle != "None")
-        DSB = False #(self.dungeon_shuffle == "Basic")
-        DSC = self.dungeon_shuffle #(self.dungeon_shuffle == "Chaos")
+        ER = self.town_shuffle  # (self.entrance_shuffle != "None")
+        DSB = False  # (self.dungeon_shuffle == "Basic")
+        DSC = self.dungeon_shuffle  # (self.dungeon_shuffle == "Chaos")
         if ER and (pooltype == 1):
             return 1
         if DSB and (pooltype > 1) and (dungeon > 0):
-            return 100+dungeon
+            return 100 + dungeon
         if DSC and (pooltype > 1) and (dungeon > 0):
-            return 2#pooltype
+            return 2  # pooltype
         return -1
-    
+
     # Returns whether two exits are pooled for shuffling.
     def cmp_exit_pool(self, exit1, exit2):
         return (self.get_exit_pool(exit1) == self.get_exit_pool(exit2))
-    
-    
+
     def shuffle_chaos_dungeon(self):
         # Build dungeon node islands for the skeleton, assuming free and all-form movement
         self.reset_progress(True)
-        self.items_collected = [800]+self.list_typed_items(types=[1, 2, 4, 5], shuffled_only=False, incl_placed=True)
-        for removed_orb in [707,708,709,735]:   # Due to awkward orb placement, treat Inca exterior and Wat Outer South as corridors
+        self.items_collected = [800] + self.list_typed_items(types=[1, 2, 4, 5], shuffled_only=False, incl_placed=True)
+        for removed_orb in [707, 708, 709,
+                            735]:  # Due to awkward orb placement, treat Inca exterior and Wat Outer South as corridors
             if removed_orb in self.items_collected:
                 self.items_collected.remove(removed_orb)
         for node in self.graph:
             self.graph[node][4] = 0x37
-        self.update_graph(True,False,True)
+        self.update_graph(True, False, True)
         island_result = self.build_islands()
-        islands = island_result[1].pop(1) # pop(1) = list of all islands assigned to the chaos dungeon
+        islands = island_result[1].pop(1)  # pop(1) = list of all islands assigned to the chaos dungeon
         # An island is: [ [nodes], [origin_exits], [dest_exits], [origin_logic], [dest_logic] ].
         # For dungeon construction, we want islands grouped by count of dungeon-internal exits.
         dungeon_exit_keys = [exit for exit in self.exits if self.exits[exit][9] == 3]
         deadend_islands = []
         corridor_islands = []
         free_ds_corridor_islands = []
         branch_islands = []
@@ -1144,53 +1140,56 @@
         for island in islands:
             internal_exits = [exit for exit in island[1] if self.exits[exit][9] == 2 and self.is_exit_coupled(exit)]
             if not internal_exits:
                 continue
             random.shuffle(internal_exits)
             for exit in internal_exits:
                 dungeon_exit_keys.append(exit)
-            subisland = [ island[0][:], internal_exits, [] ]   # [nodes, unmapped-exits, mapped-exits]
-            if any(region in subisland[0] for region in [170,212,413]):   # SkGn, Mu, and Pymd have branching foyers
-                foyer_islands.append( subisland )
+            subisland = [island[0][:], internal_exits, []]  # [nodes, unmapped-exits, mapped-exits]
+            if any(region in subisland[0] for region in [170, 212, 413]):  # SkGn, Mu, and Pymd have branching foyers
+                foyer_islands.append(subisland)
             elif len(subisland[1]) == 1:
-                deadend_islands.append( subisland )
+                deadend_islands.append(subisland)
             elif len(subisland[1]) == 2:
                 is_free_ds_corridor = False
                 ds_node = next((n for n in subisland[0] if n in self.ds_nodes), 0)
-                if ds_node > 0:    # Island contains a DS node
+                if ds_node > 0:  # Island contains a DS node
                     ds_loc = next(loc for loc in self.graph[ds_node][11] if self.item_locations[loc][1] == 2)
-                    if self.spawn_locations[ds_loc][3]:    # Island DS allows transform
-                        if all(self.edge_formless(e) for n in subisland[0] for e in self.graph[n][12]):   # Island is internally-formless
+                    if self.spawn_locations[ds_loc][3]:  # Island DS allows transform
+                        if all(self.edge_formless(e) for n in subisland[0] for e in
+                               self.graph[n][12]):  # Island is internally-formless
                             is_free_ds_corridor = True
                 if is_free_ds_corridor:
-                    free_ds_corridor_islands.append( subisland )
+                    free_ds_corridor_islands.append(subisland)
                 else:
-                    corridor_islands.append( subisland )
+                    corridor_islands.append(subisland)
             else:
-                branch_islands.append( subisland )
+                branch_islands.append(subisland)
         # At this point a "deadend" may be the bottom or top of a ledge, or behind or in front of a button.
         # Such one-way exits are functionally part of a corridor or branch, except that the low/back exit
         # can't be appended to an opening to grow the dungeon.
         # So, we coalesce the islands by one-way accessibility, keeping track of the "blocked" exits.
         blocked_exits = []
         merged_islands_for_deletion = []
-        all_islands = deadend_islands+corridor_islands+branch_islands
+        all_islands = deadend_islands + corridor_islands + branch_islands
         for lower_i in deadend_islands:
             lower_n = lower_i[0][0]
-            lower_map = self.graph[lower_n][3][3]   # One-way access must be within the same map
-            upper_i = next((i for i in all_islands if i != lower_i and any((lower_map == self.graph[upper_n][3][3]) and self.check_access(upper_n,lower_n,False) for upper_n in i[0])), [])
-            if upper_i:   # Merge the lower island into the upper one, and record the lower exit
+            lower_map = self.graph[lower_n][3][3]  # One-way access must be within the same map
+            upper_i = next((i for i in all_islands if i != lower_i and any(
+                (lower_map == self.graph[upper_n][3][3]) and self.check_access(upper_n, lower_n, False) for upper_n in
+                i[0])), [])
+            if upper_i:  # Merge the lower island into the upper one, and record the lower exit
                 upper_i[0].extend(lower_i[0][:])
                 upper_i[1].extend(lower_i[1][:])
                 blocked_exits.extend(lower_i[1][:])
                 merged_islands_for_deletion.append(lower_i)
-        for island in merged_islands_for_deletion:   # Removed merged deadends
+        for island in merged_islands_for_deletion:  # Removed merged deadends
             deadend_islands.remove(island)
-        for exit in blocked_exits:   # If any islands grew, move them to the correct list
-            grown_island = next(i for i in deadend_islands+corridor_islands+branch_islands if exit in i[1])
+        for exit in blocked_exits:  # If any islands grew, move them to the correct list
+            grown_island = next(i for i in deadend_islands + corridor_islands + branch_islands if exit in i[1])
             if grown_island in deadend_islands and len(grown_island[1]) > 1:
                 deadend_islands.remove(grown_island)
                 if len(grown_island[1]) == 2:
                     corridor_islands.append(grown_island)
                 else:
                     branch_islands.append(grown_island)
             elif grown_island in corridor_islands and len(grown_island[1]) > 2:
@@ -1198,39 +1197,43 @@
                 branch_islands.append(grown_island)
         # Various special exits that aren't detected programmatically: 72 back of EdDg, 126 behind D.Block, 234 Mine behind fences,
         # 293/295/305 SkGn SE behind robot / SW behind N pegs / NW behind statue, 534/538 Kress behind drops 1/2.
         blocked_exits.extend([72, 126, 234, 293, 295, 305, 534, 538])
         # Append non-oneway (=non-blocked), non-IncaExt, non-WatOuterS corridors to SkGn, Pymd, and Mu foyers, so they're not boring
         oneway_corridor_islands = [i for i in corridor_islands if any(x in blocked_exits for x in i[1])]
         random.shuffle(corridor_islands)
-        elig_foyer_corridors = [i for i in corridor_islands if i not in oneway_corridor_islands and not any(self.graph[n][3][3] in [0x1d,0xb1] for n in i[0])]
+        elig_foyer_corridors = [i for i in corridor_islands if i not in oneway_corridor_islands and not any(
+            self.graph[n][3][3] in [0x1d, 0xb1] for n in i[0])]
         # Pyramid is done first and given non-DS corridors; thus Mu and SkGn have increased DS corridor odds
         for base_island in sorted(foyer_islands, key=lambda i: max(self.graph[n][3][3] for n in i[0]), reverse=True):
             is_pymd_island = any(self.graph[n][3][3] == 204 for n in base_island[0])
             foyer_exits = base_island[1][:]
             for base_exit in foyer_exits:
                 if is_pymd_island:
-                    new_corridor = next(i for i in elig_foyer_corridors if not any(self.item_locations[loc][1] == 2 for n in i[0] for loc in self.graph[n][11]))
+                    new_corridor = next(i for i in elig_foyer_corridors if not any(
+                        self.item_locations[loc][1] == 2 for n in i[0] for loc in self.graph[n][11]))
                 else:
                     new_corridor = next(i for i in elig_foyer_corridors)
                 elig_foyer_corridors.remove(new_corridor)
                 corridor_islands.remove(new_corridor)
                 corridor_exit = new_corridor[1].pop()
                 base_island[1].remove(base_exit)
                 self.join_exits(corridor_exit, base_exit)
                 # The corridor is absorbed into the foyer, and the exits between them are forgotten
                 base_island[0].extend(new_corridor[0])
                 base_island[1].extend(new_corridor[1])
         # Promote a random Will-traversable branch to a foyer for dungeons that don't have a branching foyer
         random.shuffle(branch_islands)
         for exit in [x for x in self.exits if self.exits[x][9] == 3]:
-            new_foyer_island = next((i for i in branch_islands if all((edef[3] & 0x21) for edef in self.logic.values() if edef[1] in i[0])),[])
+            new_foyer_island = next(
+                (i for i in branch_islands if all((edef[3] & 0x21) for edef in self.logic.values() if edef[1] in i[0])),
+                [])
             if new_foyer_island:
                 branch_islands.remove(new_foyer_island)
-            else:   # Accept any island if there are no fully-Will-traversable ones
+            else:  # Accept any island if there are no fully-Will-traversable ones
                 new_foyer_island = branch_islands.pop()
             new_entr = next(x for x in new_foyer_island[1] if x not in blocked_exits)
             new_foyer_island[1].remove(new_entr)
             new_foyer_island[2].append(new_entr)
             self.join_exits(exit, new_entr)
             foyer_islands.append(new_foyer_island)
         # The foyers are our nascent (as-yet-unconnected) skeleton;
@@ -1245,23 +1248,24 @@
         for island in corridor_islands:
             corridor_nodesets.append(island[0][:])
         for island in branch_islands:
             branch_nodesets.append(island[0][:])
         for island in foyer_islands:
             foyer_nodesets.append(island[0][:])
         # Append all branches and one-way corridors, then append deadends to all openings.
-        while branch_islands+oneway_corridor_islands+deadend_islands and any(len(island[1]) > 0 for island in skeleton):
+        while branch_islands + oneway_corridor_islands + deadend_islands and any(
+                len(island[1]) > 0 for island in skeleton):
             random.shuffle(skeleton)
-            if branch_islands+oneway_corridor_islands:
-                if (not oneway_corridor_islands) or (branch_islands and (random.randint(0,1) == 1)):
+            if branch_islands + oneway_corridor_islands:
+                if (not oneway_corridor_islands) or (branch_islands and (random.randint(0, 1) == 1)):
                     new_island = branch_islands.pop()
                 else:
                     new_island = oneway_corridor_islands.pop()
                     corridor_islands.remove(new_island)
-            else:   # Deadends are the last type appended
+            else:  # Deadends are the last type appended
                 new_island = deadend_islands.pop()
             new_exit = next(exit for exit in new_island[1] if exit not in blocked_exits)
             new_island[1].remove(new_exit)
             new_island[2].append(new_exit)
             base_island = next(island for island in skeleton if len(island[1]) > 0)
             skeleton.remove(base_island)
             base_exit = base_island[1].pop()
@@ -1293,25 +1297,25 @@
             self.item_pool[0][0] -= 1
             self.item_locations[132][2] = True
             self.item_locations[132][3] = 0
             self.item_locations[132][7] = 0
             self.optional_nodes.append(442)
             self.link_exits(641, self.exits[641][0], False, False)
         if num_deadends > num_openings:
-            self.error("Not enough dungeon exits: need "+str(num_deadends-num_openings)+" more")
+            self.error("Not enough dungeon exits: need " + str(num_deadends - num_openings) + " more")
             return False
         elif num_deadends < num_openings:
             # Create loops by connecting openings with corridors
             remaining_inserts = (num_openings - num_deadends) / 2
             random.shuffle(skeleton)
             random.shuffle(corridor_islands)
             while remaining_inserts:
                 loop_island1 = next(x for x in skeleton if len(x[1]) > 0)
                 skeleton.remove(loop_island1)
-                loop_island2 = next((x for x in skeleton if len(x[1]) > 0),loop_island1)
+                loop_island2 = next((x for x in skeleton if len(x[1]) > 0), loop_island1)
                 # Allow for the case where one island remains and has 2 open exits
                 if loop_island2 != loop_island1:
                     skeleton.remove(loop_island2)
                 corridor_island = corridor_islands.pop()
                 loop_exit1 = loop_island1[1].pop()
                 loop_exit2 = loop_island2[1].pop()
                 corridor_exit1 = corridor_island[1].pop()
@@ -1332,73 +1336,82 @@
             random.shuffle(skeleton)
             random.shuffle(dungeon_exit_keys)
             new_island = corridor_islands.pop()
             new_exit1 = new_island[1].pop()
             new_exit2 = new_island[1].pop()
             new_island[2].append(new_exit1)
             new_island[2].append(new_exit2)
-            base_exit = next(x for x in dungeon_exit_keys if self.exits[x][1] > 0 and any(x in island[2] for island in skeleton))
+            base_exit = next(
+                x for x in dungeon_exit_keys if self.exits[x][1] > 0 and any(x in island[2] for island in skeleton))
             base_island = next(island for island in skeleton if base_exit in island[2])
             self.insert_exit(base_exit, new_exit1, new_exit2)
             skeleton.append(new_island)
         # Assuming all DSes are for transform, find and fix missing formful access if possible.
         # Need to reset and re-traverse in every iteration, because we're moving exits around.
-        graph_free_access = { n: self.graph[n][1][:] for n in self.graph }
+        graph_free_access = {n: self.graph[n][1][:] for n in self.graph}
         node_to_fix = 0
         nodes_fixed = [node_to_fix]
         f_missing_nodes = {-1}
         while free_ds_corridor_islands:
             random.shuffle(dungeon_exit_keys)
             self.reset_progress(True)
             for n in self.graph:
                 self.graph[n][1] = graph_free_access[n][:]
             self.items_collected = self.list_typed_items(types=[1, 2], shuffled_only=False, incl_placed=True)
             if self.orb_rando != "None":
                 self.items_collected.extend(self.list_typed_items(types=[5], shuffled_only=False, incl_placed=True))
             for loc in self.spawn_locations:
                 if self.spawn_locations[loc][3] and loc in self.item_locations and self.item_locations[loc][1] == 2:
                     self.item_locations[loc][2] = True
-            self.update_graph(True,True,True)
+            self.update_graph(True, True, True)
             for s in foyer_nodesets:
                 for n in s:
-                    self.graph[n][4] = 0x11   # Will can access all foyers
+                    self.graph[n][4] = 0x11  # Will can access all foyers
             trav_nodes = self.traverse(to_visit=[n for s in foyer_nodesets for n in s])
-            f_missing_nodes = {self.logic[e][1] for e in self.open_edges if not self.edge_formless(e) and any(self.logic[e][1] in i[0] for i in skeleton) and not (self.logic[e][3] & self.graph[self.logic[e][1]][4]) and not self.is_accessible(self.logic[e][2])}
+            f_missing_nodes = {self.logic[e][1] for e in self.open_edges if
+                               not self.edge_formless(e) and any(self.logic[e][1] in i[0] for i in skeleton) and not (
+                                       self.logic[e][3] & self.graph[self.logic[e][1]][
+                                   4]) and not self.is_accessible(self.logic[e][2])}
             if not f_missing_nodes:
-                break   # Success
+                break  # Success
             elif any(node in f_missing_nodes for node in nodes_fixed):
-                break   # Failed to get consistent DS access for a node; return the dungeon as-is and let the caller figure it out or fail
+                break  # Failed to get consistent DS access for a node; return the dungeon as-is and let the caller figure it out or fail
             node_to_fix = f_missing_nodes.pop()
             nodes_fixed.append(node_to_fix)
             island_to_fix = next(i for i in skeleton if node_to_fix in i[0])
             new_island = free_ds_corridor_islands.pop()
-            base_exit = next((x for x in dungeon_exit_keys if self.graph[self.exits[x][3]][0] and not self.graph[self.exits[x][3]][9] and x not in island_to_fix[2] and self.check_access(self.exits[x][3], node_to_fix, False, True)), island_to_fix[2][0])
+            base_exit = next((x for x in dungeon_exit_keys if
+                              self.graph[self.exits[x][3]][0] and not self.graph[self.exits[x][3]][9] and x not in
+                              island_to_fix[2] and self.check_access(self.exits[x][3], node_to_fix, False, True)),
+                             island_to_fix[2][0])
             new_exit1 = new_island[1].pop()
             new_exit2 = new_island[1].pop()
             new_island[2].extend([new_exit1, new_exit2])
             self.insert_exit(base_exit, new_exit1, new_exit2)
         # Insert any remaining free DS corridors
         while free_ds_corridor_islands:
             random.shuffle(skeleton)
             random.shuffle(dungeon_exit_keys)
             new_island = free_ds_corridor_islands.pop()
             new_exit1 = new_island[1].pop()
             new_exit2 = new_island[1].pop()
             new_island[2].append(new_exit1)
             new_island[2].append(new_exit2)
-            base_exit = next(x for x in dungeon_exit_keys if self.exits[x][1] > 0 and any(x in island[2] for island in skeleton))
+            base_exit = next(
+                x for x in dungeon_exit_keys if self.exits[x][1] > 0 and any(x in island[2] for island in skeleton))
             base_island = next(island for island in skeleton if base_exit in island[2])
             self.insert_exit(base_exit, new_exit1, new_exit2)
             skeleton.append(new_island)
         # Clean up the graph
         self.reset_progress(True)
         for n in self.graph:
             self.graph[n][1] = graph_free_access[n][:]
         for loc in self.spawn_locations:
-            if self.spawn_locations[loc][3] and loc in self.item_locations and self.item_locations[loc][1] == 2 and self.item_locations[loc][3] == 0:
+            if self.spawn_locations[loc][3] and loc in self.item_locations and self.item_locations[loc][1] == 2 and \
+                    self.item_locations[loc][3] == 0:
                 self.item_locations[loc][2] = False
 
     # Entrance randomizer
     def shuffle_exits(self):
         # Map passages and all fixed exits to graph.
         one_way_exits = []
         for x in self.exits:
@@ -1410,91 +1423,91 @@
 
         # Don't randomize Jeweler's final exit in RJH seeds
         if self.goal == "Red Jewel Hunt":
             self.link_exits(720, 720, False)
             self.link_exits(721, 721, False)
 
         # Special case for Slider exits in Angel Dungeon
-        if self.dungeon_shuffle: # != "None":
-            if random.randint(0,1):
-                self.link_exits(408,414,False)
-                self.link_exits(409,415,False)
-                self.link_exits(414,408,False)
-                self.link_exits(415,409,False)
+        if self.dungeon_shuffle:  # != "None":
+            if random.randint(0, 1):
+                self.link_exits(408, 414, False)
+                self.link_exits(409, 415, False)
+                self.link_exits(414, 408, False)
+                self.link_exits(415, 409, False)
             else:
-                self.link_exits(408,408,False)
-                self.link_exits(409,409,False)
-                self.link_exits(414,414,False)
-                self.link_exits(415,415,False)
-            
+                self.link_exits(408, 408, False)
+                self.link_exits(409, 409, False)
+                self.link_exits(414, 414, False)
+                self.link_exits(415, 415, False)
+
         # If using a coupled shuffle, map one-way exits to one-way dests
         exit_log = []
         if self.coupled_exits:
             one_way_dest = one_way_exits[:]
             random.shuffle(one_way_dest)
             while one_way_exits:
                 o_exit = one_way_exits.pop()
                 found_oneway = False
                 while not found_oneway:
                     d_exit = one_way_dest.pop()
                     if self.cmp_exit_pool(o_exit, d_exit):
                         self.link_exits(o_exit, d_exit, False)
-                        exit_log.append([o_exit,d_exit])
+                        exit_log.append([o_exit, d_exit])
                         found_oneway = True
                     else:
                         one_way_dest.append(d_exit)
                         random.shuffle(one_way_dest)
             self.info("One-way exits mapped")
 
         # Coupled dungeon shuffles need special handling
         if self.dungeon_shuffle and self.coupled_exits:
-            if self.dungeon_shuffle: # == "Chaos":
+            if self.dungeon_shuffle:  # == "Chaos":
                 # Link Pyramid room-pairs as in vanilla, reducing Pymd corridor count from 13 to 6.
                 dc_exits_within_pyramid_rooms = [638, 644, 650, 656, 658, 664, 670]
                 for exitnum in dc_exits_within_pyramid_rooms:
                     self.join_exits(exitnum, self.exits[exitnum][0])
                 self.shuffle_chaos_dungeon()
             self.info("Dungeon shuffle complete")
-            #elif self.dungeon_shuffle == "Basic":
+            # elif self.dungeon_shuffle == "Basic":
             #    # Ensure DS access for the top of rooms 3A and 5A
             #    db_exits_from_freedan_rooms = [649, 663]
             #    db_exits_from_pymd_branch = [636, 642, 648, 654, 662, 668]
             #    random.shuffle(db_exits_from_pymd_branch)
             #    self.join_exits(db_exits_from_freedan_rooms[0], db_exits_from_pymd_branch[0])
             #    self.join_exits(db_exits_from_freedan_rooms[1], db_exits_from_pymd_branch[1])
         # Clean up dungeon shuffle artificial edges
-        self.delete_objects(items=[800],with_close=True)
-        self.delete_objects(items=[801],with_close=False)
-        
+        self.delete_objects(items=[800], with_close=True)
+        self.delete_objects(items=[801], with_close=False)
+
         if self.dungeon_shuffle and self.coupled_exits and not self.town_shuffle:
             return True
 
         # Assume all items and abilities
         self.info("Beginning exit shuffle...")
         self.reset_progress(True)
         self.items_collected = self.list_typed_items(types=[1, 2, 4, 5], shuffled_only=True, incl_placed=True)
-        self.update_graph(True,True,True)
+        self.update_graph(True, True, True)
 
         # Build world skeleton with islands
         self.unsolve()
         island_result = self.build_islands()
-        islands = island_result[1].pop(0) # pop(0) = all non-dungeon islands
+        islands = island_result[1].pop(0)  # pop(0) = all non-dungeon islands
 
         traverse_result = self.traverse()
         visited = traverse_result[0]
         origin_exits = []
         for node in visited:
             origin_exits += self.graph[node][14]
 
         i = 0
         for x in islands:
             i += 1
-            self.verbose("Initial island "+str(i)+" ("+str(x[1])+","+str(x[2])+"):")
+            self.verbose("Initial island " + str(i) + " (" + str(x[1]) + "," + str(x[2]) + "):")
             for y in x[0]:
-                self.verbose(" - "+self.graph[y][5])
+                self.verbose(" - " + self.graph[y][5])
         self.info(" Joining initial islands...")
 
         check_direction = True
         check_progression = True
         quarantine = []
         while islands:
             random.shuffle(islands)
@@ -1502,27 +1515,28 @@
             nodes_new = island[0]
             origin_exits_new = island[1]
             dest_exits_new = island[2]
 
             if not dest_exits_new or not origin_exits_new or self.is_accessible(nodes_new[0]):
                 pass
             else:
-                if (check_progression and not origin_exits_new) or (self.coupled_exits and (len(origin_exits_new) < 2 or len(dest_exits_new) < 2)):
+                if (check_progression and not origin_exits_new) or (
+                        self.coupled_exits and (len(origin_exits_new) < 2 or len(dest_exits_new) < 2)):
                     quarantine.append(island)
                 else:
                     random.shuffle(origin_exits)
                     random.shuffle(dest_exits_new)
 
-                    result = self.find_exit(origin_exits,dest_exits_new,check_direction,True)
+                    result = self.find_exit(origin_exits, dest_exits_new, check_direction, True)
                     if not result:
                         quarantine.append(island)
                     else:
                         self.verbose("New island:")
                         for y in nodes_new:
-                            self.verbose(" - "+str(self.graph[y][5]))
+                            self.verbose(" - " + str(self.graph[y][5]))
                         traverse_result = self.traverse(island[0])
                         visited += traverse_result[0]
                         progression_result = self.get_open_exits()
                         origin_exits = progression_result[0]
                         check_direction = True
 
             if not islands:
@@ -1542,92 +1556,94 @@
                 quarantine = []
 
         self.info(" Island construction complete")
 
         # Check Dark Space access, map exits accordingly
         self.reset_progress()
         self.items_collected = self.list_typed_items(types=[1, 2, 4, 5], shuffled_only=True, incl_placed=True)
-        self.update_graph(True,True,True)
+        self.update_graph(True, True, True)
 
         island_result = self.build_islands()
         islands = island_result[1].pop(0)
 
         islands_no_ds = []
         ds_check_visited = []
         for island in islands:
-            if self.is_accessible(island[0][0]) and not self.check_ds_access(island[0][0], False, True, ds_check_visited):
+            if self.is_accessible(island[0][0]) and not self.check_ds_access(island[0][0], False, True,
+                                                                             ds_check_visited):
                 islands_no_ds.append(island)
 
         if islands_no_ds:
             self.verbose("Islands with no DS access:")
             i = 0
             for x in islands_no_ds:
                 i += 1
-                self.verbose("Island "+str(x))
+                self.verbose("Island " + str(x))
                 for y in x[0]:
-                    self.verbose("- "+str(self.graph[y][5]))
+                    self.verbose("- " + str(self.graph[y][5]))
 
             dest_exits_ds = []
             for node in self.graph:
                 if node not in visited and self.check_ds_access(node, False, True, ds_check_visited):
                     for exit in self.graph[node][15]:
                         if self.exits[exit][2] == -1:
                             dest_exits_ds.append(exit)
 
             while islands_no_ds:
                 island = islands_no_ds.pop(0)
-                result = self.find_exit(island[1],dest_exits_ds,check_direction)
+                result = self.find_exit(island[1], dest_exits_ds, check_direction)
                 if not result:
                     self.error("Could not find Dark Space access")
                     return False
                 else:
                     dest_exits_ds = result[3]
 
         self.info(" Dark Space access check successful")
 
         # Link exits forward
         self.reset_progress()
         self.items_collected = self.list_typed_items(types=[1, 2, 4, 5], shuffled_only=True, incl_placed=True)
-        self.update_graph(True,True,True)
+        self.update_graph(True, True, True)
         self.traverse()
 
         check_progression = True
         check_direction = True
         while origin_exits:
             progression_result = self.get_open_exits(check_progression)
             origin_exits = progression_result[0]
             dest_exits = progression_result[1]
             random.shuffle(origin_exits)
             random.shuffle(dest_exits)
             if origin_exits:
-                result = self.find_exit(origin_exits,dest_exits,check_direction,check_progression,True,False)
+                result = self.find_exit(origin_exits, dest_exits, check_direction, check_progression, True, False)
                 if result:
                     origin_exit = result[0]
                     dest_exit = result[1]
                     dest = self.exits[dest_exit][4]
                     self.traverse([dest])
                 elif check_direction:
                     check_direction = False
                 elif check_progression:
                     check_progression = False
                     check_direction = True
                     self.info("  Finished mapping progression exits")
                 else:
-                    self.info("Can't link any origin exit of "+str(origin_exits)+" to any dest exit of "+str(dest_exits))
+                    self.info("Can't link any origin exit of " + str(origin_exits) + " to any dest exit of " + str(
+                        dest_exits))
                     return False
 
         # Randomly link any leftover exits
         origin_exits = []
         dest_exits = []
         for exit in self.exits:
             if self.exits[exit][1] == -1:
-                self.verbose(" Unmapped exit: "+str(exit)+" "+str(self.exits[exit]))
+                self.verbose(" Unmapped exit: " + str(exit) + " " + str(self.exits[exit]))
                 origin_exits.append(exit)
             if self.exits[exit][2] == -1:
-                self.verbose(" No exit mapped to: "+str(exit)+" "+str(self.exits[exit]))
+                self.verbose(" No exit mapped to: " + str(exit) + " " + str(self.exits[exit]))
                 dest_exits.append(exit)
             if origin_exits:
                 random.shuffle(origin_exits)
             if dest_exits:
                 random.shuffle(dest_exits)
 
         while origin_exits:
@@ -1639,75 +1655,74 @@
             fallback_dest_exit_idx = -1
             while candidate_dest_exit_idx < len(dest_exits) - 1:
                 candidate_dest_exit = dest_exits[candidate_dest_exit_idx]
                 # Prefer mapping to an exit other than itself in the same pool.
                 if self.cmp_exit_pool(origin_exit, candidate_dest_exit):
                     if candidate_dest_exit == self.exits[origin_exit][0]:
                         fallback_dest_exit_idx = candidate_dest_exit_idx
-                    else:    # If we get here, candidate_dest_exit_idx meets both criteria, so use it.
+                    else:  # If we get here, candidate_dest_exit_idx meets both criteria, so use it.
                         fallback_dest_exit_idx = -1
                         break
                 candidate_dest_exit_idx += 1
             if fallback_dest_exit_idx > -1:
                 dest_exit = dest_exits.pop(fallback_dest_exit_idx)
             else:
                 dest_exit = dest_exits.pop(candidate_dest_exit_idx)
-            self.link_exits(origin_exit,dest_exit,False)
+            self.link_exits(origin_exit, dest_exit, False)
             if self.coupled_exits and origin_exit != self.exits[dest_exit][0]:  # Map reverse direction.
                 self.link_exits(self.exits[dest_exit][0], self.exits[origin_exit][0], False)
                 origin_exits.remove(self.exits[dest_exit][0])
                 dest_exits.remove(self.exits[origin_exit][0])
 
-        #self.reset_progress()
-        #self.update_graph(True,True,True)
+        # self.reset_progress()
+        # self.update_graph(True,True,True)
         self.info("Entrance rando successful")
-        #self.print_exit_graph()
+        # self.print_exit_graph()
 
         return True
 
-
     def print_exit_graph_from_node(self, node, visited=[], known_exits=[]):
         for exit in self.exits:
             if self.exits[exit][1] > 0 and self.exits[exit][3] == node and exit not in known_exits:
                 known_exits.append(exit)
                 if self.coupled_exits:
                     known_exits.append(self.exits[self.exits[exit][1]][0])
                 dest_node = self.exits[self.exits[exit][1]][4]
-                self.verbose(str(node)+" "+str(self.graph[node][5])+" -> "+str(exit)+" "+str(self.exits[exit][10])+" -> "+str(dest_node)+" "+str(self.graph[dest_node][5]))
+                self.verbose(str(node) + " " + str(self.graph[node][5]) + " -> " + str(exit) + " " + str(
+                    self.exits[exit][10]) + " -> " + str(dest_node) + " " + str(self.graph[dest_node][5]))
                 if dest_node in visited:
-                    self.verbose("   Looped to "+str(dest_node)+" "+str(self.graph[dest_node][5]))
+                    self.verbose("   Looped to " + str(dest_node) + " " + str(self.graph[dest_node][5]))
                 else:
                     visited.append(dest_node)
-                    self.print_exit_graph_from_node(dest_node,visited,known_exits)
+                    self.print_exit_graph_from_node(dest_node, visited, known_exits)
         return True
 
-
     def print_exit_graph(self):
         for node in self.graph:
-            self.print_exit_graph_from_node(node,[node],[])
+            self.print_exit_graph_from_node(node, [node], [])
         return True
 
-
     def initialize_ds(self):
         # Clear DS access data from graph
         for x in self.graph:
             self.graph[x][4] = 0
             self.graph[x][9].clear()
         # Find nodes that contain Dark Spaces, and of those, which allow transform and don't contain an ability
         self.ds_locations = [loc for loc in self.spawn_locations if loc in self.item_locations]
         self.ds_nodes = [self.item_locations[loc][0] for loc in self.ds_locations]
         # Transform DSes are marked "filled" but with item 0
-        self.txform_locations = [loc for loc in self.ds_locations if self.spawn_locations[loc][3] and self.item_locations[loc][2] and not self.item_locations[loc][3]]
-        self.txform_locations.append(130)   # --but upper Pyramid is special because it's a type-1 loc
+        self.txform_locations = [loc for loc in self.ds_locations if
+                                 self.spawn_locations[loc][3] and self.item_locations[loc][2] and not
+                                 self.item_locations[loc][3]]
+        self.txform_locations.append(130)  # --but upper Pyramid is special because it's a type-1 loc
         self.txform_nodes = [self.item_locations[loc][0] for loc in self.txform_locations]
         return True
 
-
     # Translates logic and exits to world graph
-    def update_graph(self,update_logic=True,update_ds=True,update_exits=False):
+    def update_graph(self, update_logic=True, update_ds=True, update_exits=False):
         self.info("Updating graph...")
         if update_exits:
             for exit in self.exits:
                 if exit > 21 or self.exits[exit][5]:
                     # Check if exit has been shuffled
                     if self.exits[exit][1] > 0:
                         new_exit = self.exits[exit][1]
@@ -1753,165 +1768,169 @@
                     self.graph[z][10].append(node)
         self.verbose(" Graph node-node connections updated")
 
         if update_ds:
             # Clear and recalculate DS access for all nodes (recursively from DS nodes)
             self.initialize_ds()
             for node in self.ds_nodes:
-                self.update_ds_access([node],0x10,[])
+                self.update_ds_access([node], 0x10, [])
                 for loc in self.graph[node][11]:
                     if loc in self.spawn_locations and self.spawn_locations[loc][3]:
-                        self.update_ds_access([node],0x20,[node])
+                        self.update_ds_access([node], 0x20, [node])
             for node in self.txform_nodes:
-                self.update_ds_access([node],(0x01|0x02|0x04),[])
-            for node in [0,10,11,12,13,14]:   # Will has access to overworld-connected nodes and the start node
-                self.update_ds_access([node],0x01,[])
+                self.update_ds_access([node], (0x01 | 0x02 | 0x04), [])
+            for node in [0, 10, 11, 12, 13, 14]:  # Will has access to overworld-connected nodes and the start node
+                self.update_ds_access([node], 0x01, [])
             self.verbose(" Graph DS access updated")
 
         # Update form-specific logic, repeatedly until access stops growing
         if update_logic:
             all_f_edges = [e for e in self.logic if not self.edge_formless(e)]
             checked_f_edges = []
             checked_new_edge = True
             while checked_new_edge:
                 checked_new_edge = False
                 for edge in all_f_edges:
-                    if edge not in checked_f_edges and self.check_edge(edge, [], True, self.graph[self.logic[edge][1]][4]):
+                    if edge not in checked_f_edges and self.check_edge(edge, [], True,
+                                                                       self.graph[self.logic[edge][1]][4]):
                         checked_f_edges.append(edge)
                         checked_new_edge = True
             self.verbose(" Graph formful logic updated")
 
         return True
 
-
     # Return (bool) whether an edge is form-specific
-    def edge_formless(self,edge):
+    def edge_formless(self, edge):
         return (False or (self.logic[edge][3] & (0x20)) or (self.logic[edge][3] == 0))
 
-
     # Check whether a node's DS access data needs to be updated
-    def consider_ds_node(self,node,access_mode,ds_nodes):
-        if access_mode not in [0x01,0x02,0x04,0x10,0x20]:   # --then it's a combined access mode
+    def consider_ds_node(self, node, access_mode, ds_nodes):
+        if access_mode not in [0x01, 0x02, 0x04, 0x10, 0x20]:  # --then it's a combined access mode
             result = False
-            for flag in [0x01,0x02,0x04,0x10,0x20]:
+            for flag in [0x01, 0x02, 0x04, 0x10, 0x20]:
                 if access_mode & flag:
-                    result |= self.consider_ds_node(node,flag,ds_nodes)
+                    result |= self.consider_ds_node(node, flag, ds_nodes)
             return result
-        if access_mode in [0x02,0x04,0x20] and self.graph[node][7]:
-            return False   # Always-Will nodes never allow not-Will or formless traversal
+        if access_mode in [0x02, 0x04, 0x20] and self.graph[node][7]:
+            return False  # Always-Will nodes never allow not-Will or formless traversal
         if access_mode == 0x20 and any(ds_node not in self.graph[node][9] for ds_node in ds_nodes):
             return True
         if not (self.graph[node][4] & access_mode):
             return True
         return False
 
-
     # Check if start_node can reach a DS or be reached by a form
     def check_ds_access(self, start_node, access_mode, do_recurse, visited):
-        if access_mode not in [0x01,0x02,0x04,0x10,0x20]:   # If combined access is checked, "or" logic is used
-            for flag in [0x01,0x02,0x04,0x10,0x20]:
+        if access_mode not in [0x01, 0x02, 0x04, 0x10, 0x20]:  # If combined access is checked, "or" logic is used
+            for flag in [0x01, 0x02, 0x04, 0x10, 0x20]:
                 sub_visited = visited[:]
                 if (access_mode & flag) and self.check_ds_access(start_node, flag, do_recurse, sub_visited):
                     return True
             return False
         if start_node not in self.graph or start_node < 0:
-            return False   # Not a real node, dude
-        if self.graph[start_node][7] and access_mode in [0x02,0x04,0x20]:
-            return False   # ForceWillForm denies non-Will and formless access
+            return False  # Not a real node, dude
+        if self.graph[start_node][7] and access_mode in [0x02, 0x04, 0x20]:
+            return False  # ForceWillForm denies non-Will and formless access
         if self.graph[start_node][4] & access_mode:
-            return True    # Node has already been evaluated to have the right DS access
+            return True  # Node has already been evaluated to have the right DS access
         if not do_recurse:
-            return False   # Caller only wants to check this node's evaluated access
+            return False  # Caller only wants to check this node's evaluated access
         if start_node in visited:
-            return False   # We've already recursed through this node
+            return False  # We've already recursed through this node
         to_visit = [start_node]
         while to_visit:
             node = to_visit.pop(0)
-            if node not in visited+[start_node] and self.check_ds_access(node,access_mode,do_recurse,visited):
-                self.verbose("Node "+str(start_node)+" has form "+str(access_mode)+" access via node "+str(node))
+            if node not in visited + [start_node] and self.check_ds_access(node, access_mode, do_recurse, visited):
+                self.verbose(
+                    "Node " + str(start_node) + " has form " + str(access_mode) + " access via node " + str(node))
                 return True
             else:
                 if node not in visited:
                     visited.append(node)
-                if access_mode in [0x01,0x02,0x04,0x20]:   # if checking "can be reached [by form]", find nodes that can reach here
-                    to_visit.extend([n for n in self.graph if node in self.graph[n][1] and n not in visited+to_visit])
+                if access_mode in [0x01, 0x02, 0x04,
+                                   0x20]:  # if checking "can be reached [by form]", find nodes that can reach here
+                    to_visit.extend([n for n in self.graph if node in self.graph[n][1] and n not in visited + to_visit])
                     for edge in self.graph[node][13]:
-                        if (self.logic[edge][0] > 0) and (self.logic[edge][3] & access_mode) and (self.logic[edge][1] not in visited+to_visit):
+                        if (self.logic[edge][0] > 0) and (self.logic[edge][3] & access_mode) and (
+                                self.logic[edge][1] not in visited + to_visit):
                             to_visit.append(self.logic[edge][1])
-                else:   # if checking "can reach any DS", follow edges forward
-                    to_visit.extend([n for n in self.graph[node][1] if n not in visited+to_visit])
+                else:  # if checking "can reach any DS", follow edges forward
+                    to_visit.extend([n for n in self.graph[node][1] if n not in visited + to_visit])
                     for edge in self.graph[node][12]:
-                        if (self.logic[edge][0] > 0) and ((self.logic[edge][3] & 0x07) == 0x07) and (self.logic[edge][2] not in visited+to_visit):
+                        if (self.logic[edge][0] > 0) and ((self.logic[edge][3] & 0x07) == 0x07) and (
+                                self.logic[edge][2] not in visited + to_visit):
                             to_visit.append(self.logic[edge][2])
         return False
 
     # Update DS access data for nodes, recursively to all connected nodes
     def update_ds_access(self, nodes, access_mode, ds_nodes):
         if not nodes:
             return True
-        visit_forward = [ [],[],[],[] ]   # visit for w, f, s, formless
+        visit_forward = [[], [], [], []]  # visit for w, f, s, formless
         visit_reverse = []
         for node in nodes:
             self.graph[node][4] |= access_mode
-            if access_mode & 0x10:    # Can reach a DS here, so propagate "can reach DS" backward
-                visit_reverse = [x for x in self.graph[node][8] if self.consider_ds_node(x,0x10,[])]
-            if access_mode & (0x01|0x02|0x04|0x20):    # Can be transformed here, so propagate the form forward
+            if access_mode & 0x10:  # Can reach a DS here, so propagate "can reach DS" backward
+                visit_reverse = [x for x in self.graph[node][8] if self.consider_ds_node(x, 0x10, [])]
+            if access_mode & (0x01 | 0x02 | 0x04 | 0x20):  # Can be transformed here, so propagate the form forward
                 if access_mode & 0x20:
                     self.graph[node][9].extend([ds_node for ds_node in ds_nodes if ds_node not in self.graph[node][9]])
-                for idx,flag in [ (0,0x01), (1,0x02), (2,0x04), (3,0x20) ]:
+                for idx, flag in [(0, 0x01), (1, 0x02), (2, 0x04), (3, 0x20)]:
                     if (access_mode & flag):
-                        visit_forward[idx].extend([n for n in self.graph[node][1] if self.consider_ds_node(n,flag,ds_nodes)])
+                        visit_forward[idx].extend(
+                            [n for n in self.graph[node][1] if self.consider_ds_node(n, flag, ds_nodes)])
                         for forward_edge in self.graph[node][12]:
-                            if self.check_edge(forward_edge,[],False,flag) and self.consider_ds_node(self.logic[forward_edge][2],flag,ds_nodes) and self.logic[forward_edge][2] not in visit_forward[idx]:
+                            if self.check_edge(forward_edge, [], False, flag) and self.consider_ds_node(
+                                    self.logic[forward_edge][2], flag, ds_nodes) and self.logic[forward_edge][2] not in \
+                                    visit_forward[idx]:
                                 visit_forward[idx].append(self.logic[forward_edge][2])
-        result = self.update_ds_access(visit_reverse,0x10,[])
-        for idx,flag in [(0,0x01),(1,0x02),(2,0x04)]:
+        result = self.update_ds_access(visit_reverse, 0x10, [])
+        for idx, flag in [(0, 0x01), (1, 0x02), (2, 0x04)]:
             if visit_forward[idx]:
-                result |= self.update_ds_access(set(visit_forward[idx]),flag,[])
+                result |= self.update_ds_access(set(visit_forward[idx]), flag, [])
         if visit_forward[3]:
-            result |= self.update_ds_access(set(visit_forward[3]),0x20,ds_nodes)
+            result |= self.update_ds_access(set(visit_forward[3]), 0x20, ds_nodes)
         return result
 
-
     # Check a logic edge to see if prerequisites have been met based on self.items_collected + items.
     def check_edge(self, edge, items=[], update_graph=True, form=0xff):
         success = False
         if not (self.logic[edge][3] & form):
             return False
         elif self.logic[edge][0] > 0:
             success = True
         req_items = []
         for req in self.logic[edge][4]:
             i = 0
             while i < req[1]:
                 req_items.append(req[0])
                 i += 1
-        if self.is_sublist(self.items_collected+items, req_items) and (self.edge_formless(edge) or self.check_ds_access(self.logic[edge][1], self.logic[edge][3] & form, False, [])):
+        if self.is_sublist(self.items_collected + items, req_items) and (
+                self.edge_formless(edge) or self.check_ds_access(self.logic[edge][1], self.logic[edge][3] & form, False,
+                                                                 [])):
             success = True
         if success and update_graph and not self.logic[edge][0]:
             self.logic[edge][0] = 1
-            self.new_connection(self.logic[edge][1],self.logic[edge][2],self.logic[edge][3] & form)
+            self.new_connection(self.logic[edge][1], self.logic[edge][2], self.logic[edge][3] & form)
         return success
 
-
     # Save a new connection (i.e. exit or edge) for forms to graph, and update DS access
     def new_connection(self, origin, dest, form):
         if dest not in self.graph[origin][10]:
             self.graph[origin][10].append(dest)
         if origin not in self.graph[dest][8]:
             self.graph[dest][8].append(origin)
-        if (self.graph[dest][4] & 0x10) and self.consider_ds_node(origin,0x10,[]):
-            self.update_ds_access([origin],0x10,[])   # If dest can reach a DS, origin now can too
-        for flag in [0x01,0x02,0x04,0x20]:
+        if (self.graph[dest][4] & 0x10) and self.consider_ds_node(origin, 0x10, []):
+            self.update_ds_access([origin], 0x10, [])  # If dest can reach a DS, origin now can too
+        for flag in [0x01, 0x02, 0x04, 0x20]:
             ds_nodes = self.graph[origin][9] if flag == 0x20 else []
-            if (self.graph[origin][4] & flag & form) and self.consider_ds_node(dest,flag,ds_nodes):
-                self.update_ds_access([dest], flag, ds_nodes)   # dest now reachable from origin's DS nodes
+            if (self.graph[origin][4] & flag & form) and self.consider_ds_node(dest, flag, ds_nodes):
+                self.update_ds_access([dest], flag, ds_nodes)  # dest now reachable from origin's DS nodes
         return True
 
-
     def restrict_edge(self, edge=-1):
         try:
             self.logic[edge][0] = -1
             return True
         except:
             return False
 
@@ -1923,162 +1942,166 @@
             return False
 
     # Set up the databases as required by this seed.
     # Future writer: be sure the databases are in the state you expect at the line where you're adding code;
     # for example, exit_logic and artificial grouping items are unused after they're decomposed.
     def initialize(self):
         # Will delete several database objects that aren't needed by this seed
-        free_items = []    # Items given for free, whose edges should be kept
+        free_items = []  # Items given for free, whose edges should be kept
         unused_items = []  # Inaccessible items, whose edges should be deleted
         unused_locs = []
         unused_nodes = []
         unused_edges = []
         unused_exits = []
-        
+
         # Save item shuffle pools in the database
         for item in self.item_pool:
             self.item_pool[item][6] = self.get_pool_id(item=item)
         for loc in self.item_locations:
             self.item_locations[loc][7] = self.get_pool_id(loc=loc)
-        
+
         # Save other "disallowed" items per location (ignored in Chaos logic):
         # No non-W abilities in towns
-        non_w_abilities = [item for item in self.form_items[1]+self.form_items[2] if self.item_pool[item][6] == 2]
+        non_w_abilities = [item for item in self.form_items[1] + self.form_items[2] if self.item_pool[item][6] == 2]
         for loc in self.spawn_locations:
             if loc in self.item_locations and not self.spawn_locations[loc][3]:
                 self.item_locations[loc][4].extend(non_w_abilities)
         # Jeweler inventory isn't fun if full of trash or front-loaded with goodies
-        for jeweler_loc in [0,2,4]:
-            self.item_locations[jeweler_loc + random.randint(0,1)][4].extend([0,1,6,41,42])
-        for jeweler_loc in [0,1,2,3]:
+        for jeweler_loc in [0, 2, 4]:
+            self.item_locations[jeweler_loc + random.randint(0, 1)][4].extend([0, 1, 6, 41, 42])
+        for jeweler_loc in [0, 1, 2, 3]:
             for item in self.item_pool:
-                if self.item_pool[item][7] > 1+(2*jeweler_loc) and item not in self.item_locations[jeweler_loc][4]:
+                if self.item_pool[item][7] > 1 + (2 * jeweler_loc) and item not in self.item_locations[jeweler_loc][4]:
                     self.item_locations[jeweler_loc][4].append(item)
-        
+
         # Clamp item progression penalty
         for item in self.item_pool:
             if self.item_pool[item][7] < -10:
                 self.item_pool[item][7] = -10.0
             elif self.item_pool[item][7] > 10:
                 self.item_pool[item][7] = 10.0
-        
+
         # Save implicit FromRegion/ToRegion for coupled exits, and mark exits for randomization.
         for x in self.exits:
             if self.is_exit_coupled(x) and (not self.exits[x][3] or not self.exits[x][4]):
                 xprime = self.exits[x][0]
                 self.exits[x][3] = self.exits[xprime][4]
                 self.exits[x][4] = self.exits[xprime][3]
             if (not self.exits[x][1] and self.get_exit_pool(x) > -1):
                 self.exits[x][1] = -1
                 self.exits[x][2] = -1
 
         # Random start location
         if self.start_mode != "South Cape":
             self.start_loc = self.random_start()
-            self.info("Start location: "+str(self.item_locations[self.start_loc][6]))
+            self.info("Start location: " + str(self.item_locations[self.start_loc][6]))
             if self.start_loc == 47:  # Diamond Mine behind fences: fences are free
                 self.graph[131][1].append(130)
         if self.start_mode == "South Cape" and not self.entrance_shuffle:
-            self.graph[0][1].append(22)    # Starts in school
+            self.graph[0][1].append(22)  # Starts in school
         else:
             # Connect node 0 to the start; for locs behind orbs, connect to the outer node
             if self.start_loc == 19:
-                start_node = 47   # Edward's
+                start_node = 47  # Edward's
             elif self.start_loc == 46:
                 start_node = 136  # Mine
             else:
                 start_node = self.item_locations[self.start_loc][0]
             self.graph[0][1].append(start_node)
         start_map = self.spawn_locations[self.start_loc][1]
         if start_map in self.maps:
-            self.maps[start_map][4] = 1   # Can only start in a dark map if cursed
+            self.maps[start_map][4] = 1  # Can only start in a dark map if cursed
 
         # Randomize darkness and add edges to exit_logic if applicable
-        if self.darkroom_level not in ["None","All"]:
+        if self.darkroom_level not in ["None", "All"]:
             if self.darkroom_level == "Few":
                 self.max_darkrooms = 7
             elif self.darkroom_level == "Some":
                 self.max_darkrooms = 14
             elif self.darkroom_level == "Many":
                 self.max_darkrooms = 21
             if self.darkroom_cursed:
                 self.max_darkrooms *= 2
             self.dr_randomize()
-        
+
         # Convert exits that have logic requirements into graph nodes with logic edges
         coupled_exit_logics = [edge for edge in self.exit_logic if self.exit_logic[edge][3]]
         for edge in coupled_exit_logics:
             this_exit = self.exit_logic[edge][0]
             sister_exit = self.exits[this_exit][0]
             if sister_exit > 0:
-                new_edge_id = 1+max(self.exit_logic)
+                new_edge_id = 1 + max(self.exit_logic)
                 new_edge = [sister_exit, self.exit_logic[edge][1][:], self.exit_logic[edge][2], False]
                 self.exit_logic[new_edge_id] = new_edge
                 self.exit_logic[edge][3] = False
         exits_with_logic = set(self.exit_logic[edge][0] for edge in self.exit_logic)
         for exit in exits_with_logic:
             src_node_id = self.exits[exit][3]
             src_node_type = self.graph[src_node_id][2]
             src_node_info = self.graph[src_node_id][3]
-            new_node_id = 1+max(self.graph)
-            new_node = [False, [], src_node_type, src_node_info[:], 0, self.exits[exit][10], [], False, [], [], [], [], [], [], [], []]
+            new_node_id = 1 + max(self.graph)
+            new_node = [False, [], src_node_type, src_node_info[:], 0, self.exits[exit][10], [], False, [], [], [], [],
+                        [], [], [], []]
             self.graph[new_node_id] = new_node
             sister_exit = self.exits[exit][0]
             exit_edges = [e for e in self.exit_logic if self.exit_logic[e][0] == exit]
             for edge in exit_edges:
-                new_edge_id = 1+max(self.logic)
-                if self.exit_logic[edge][2] == 0:   # Logic is for room->exit
+                new_edge_id = 1 + max(self.logic)
+                if self.exit_logic[edge][2] == 0:  # Logic is for room->exit
                     new_edge = [0, src_node_id, new_node_id, 0, self.exit_logic[edge][1][:], False]
-                    self.exits[exit][3] = new_node_id   # Exit is from its own node, sister_exit goes to the room
-                    self.graph[new_node_id][1].append(src_node_id)   # Exit->room is free
-                elif self.exit_logic[edge][2] == 1:   # Logic is for exit->room
+                    self.exits[exit][3] = new_node_id  # Exit is from its own node, sister_exit goes to the room
+                    self.graph[new_node_id][1].append(src_node_id)  # Exit->room is free
+                elif self.exit_logic[edge][2] == 1:  # Logic is for exit->room
                     new_edge = [0, new_node_id, src_node_id, 0, self.exit_logic[edge][1][:], False]
-                    self.graph[src_node_id][1].append(new_node_id)   # Room->exit is free
-                    if sister_exit and self.exits[sister_exit][4] == src_node_id:    # Exit is from the room, sister_exit goes to the new exitnode
+                    self.graph[src_node_id][1].append(new_node_id)  # Room->exit is free
+                    if sister_exit and self.exits[sister_exit][
+                        4] == src_node_id:  # Exit is from the room, sister_exit goes to the new exitnode
                         self.exits[sister_exit][4] = new_node_id
-                elif self.exit_logic[edge][2] == 2:   # Logic blocks both room->exitnode and exitnode->room
+                elif self.exit_logic[edge][2] == 2:  # Logic blocks both room->exitnode and exitnode->room
                     new_edge = [0, new_node_id, src_node_id, 0, self.exit_logic[edge][1][:], True]
-                    self.exits[exit][3] = new_node_id   # Exit is from its own node
-                    if sister_exit and self.exits[sister_exit][4] == src_node_id:    # Sister exit goes to the new exitnode
+                    self.exits[exit][3] = new_node_id  # Exit is from its own node
+                    if sister_exit and self.exits[sister_exit][
+                        4] == src_node_id:  # Sister exit goes to the new exitnode
                         self.exits[sister_exit][4] = new_node_id
-                else:    # Something's wrong
+                else:  # Something's wrong
                     self.error("exit_logic contains invalid directionality")
                     return False
                 self.logic[new_edge_id] = new_edge
-        
+
         # Convert locations that have logic requirements into graph nodes with logic edges
         for loc in self.item_locations:
             if self.item_locations[loc][9]:
                 outer_node_id = self.item_locations[loc][0]
                 outer_node_type = self.graph[outer_node_id][2]
                 outer_node_info = self.graph[outer_node_id][3]
                 loc_name = self.item_locations[loc][6]
-                new_node_id = 1+max(self.graph)
-                new_node = [False, [outer_node_id], outer_node_type, outer_node_info[:], 0, loc_name, [], False, [], [], [], [], [], [], [], []]
-                new_edge_id = 1+max(self.logic)
+                new_node_id = 1 + max(self.graph)
+                new_node = [False, [outer_node_id], outer_node_type, outer_node_info[:], 0, loc_name, [], False, [], [],
+                            [], [], [], [], [], []]
+                new_edge_id = 1 + max(self.logic)
                 new_edge = [0, outer_node_id, new_node_id, 0, self.item_locations[loc][9][:], False]
                 self.graph[new_node_id] = new_node
                 self.logic[new_edge_id] = new_edge
                 self.item_locations[loc][0] = new_node_id
-        
+
         # If no orb rando, assign default locs for all orbs (item ID == loc ID).
         # If additionally starting with flute, give the free orbs as free items.
         # most orbs are free, but programmatically identifying them is complex, so they're hardcoded.
         if self.orb_rando == "None":
             all_orbs = [item for item in self.item_pool if self.item_pool[item][1] == 5]
-            free_orbs = [701,702,703,704,710,713,718,721,725,727,728,736,739]   # progression orbs
-            free_orbs.extend([item for item in all_orbs if self.item_pool[item][5] == 3])   # nonprog
+            free_orbs = [701, 702, 703, 704, 710, 713, 718, 721, 725, 727, 728, 736, 739]  # progression orbs
+            free_orbs.extend([item for item in all_orbs if self.item_pool[item][5] == 3])  # nonprog
             for orb in all_orbs:
                 loc = orb
                 self.unfill_item(loc)
                 self.fill_item(orb, loc, False, True)
                 if self.flute == "Start" and orb in free_orbs:
                     free_items.append(orb)
                     unused_locs.append(loc)
-        
+
         # Manage required items
         if 1 in self.dungeons_req:
             self.required_items += [3, 4, 7, 8]
         if 2 in self.dungeons_req:
             self.required_items += [14]
         if 3 in self.dungeons_req:
             self.required_items += [18, 19]
@@ -2097,213 +2120,229 @@
 
         # Various gameplay variants
         if self.firebird:
             free_items.append(602)
         else:
             unused_items.append(602)
         if "Z3 Mode" not in self.variant:
-            unused_items.append(55)   # Heart pieces don't exist
+            unused_items.append(55)  # Heart pieces don't exist
         if "Open Mode" in self.variant:
             # Set all travel item edges open (Letter, M.Melody, Teapot, Will, Roast)
-            for travel_edge in [30,31,32,33,36,38,39,40]:
+            for travel_edge in [30, 31, 32, 33, 36, 38, 39, 40]:
                 self.logic[travel_edge][0] = 2
             # Remove travel items from pool and add some replacements
-            free_items.extend([10,13,24,25,37])
+            free_items.extend([10, 13, 24, 25, 37])
             self.item_pool[6][0] += 4  # Herbs
             self.item_pool[0][0] += 1  # Nothing
         # Some flute shuffle handling.
         if self.flute == "Start":
             # Starting with Flute, so give Flute and Can-Play-Song items
             free_items.append(604)
             free_items.append(611)
         else:
             # Starting without Flute; remove something so there's room for it
-            if self.item_pool[0][0] > 0:   # Try removing a Nothing
+            if self.item_pool[0][0] > 0:  # Try removing a Nothing
                 self.item_pool[0][0] -= 1
             else:
                 self.item_pool[6][0] -= 1  # Or settle for removing an herb
             if self.flute == "Shuffle":
                 # Must find the Flute to play songs
                 unused_items.append(611)
-                song_edges = [e for e in self.logic if e not in unused_edges and any(req[0] == 611 for req in self.logic[e][4])]
+                song_edges = [e for e in self.logic if
+                              e not in unused_edges and any(req[0] == 611 for req in self.logic[e][4])]
                 for edge in song_edges:
                     for req in self.logic[edge][4]:
                         if req[0] == 611:
                             req[0] = 604
             if self.flute == "Fluteless":
                 # The Flute isn't collectible, but Will can whistle
                 unused_items.append(604)
                 free_items.append(611)
-        
+
         # Decompose bidirectional and artificial-item edges to unidirectional with real items;
         # the former are easier to maintain, the latter allow simpler code
         bidirectional_edges = [edge for edge in self.logic if self.logic[edge][5] and edge not in unused_edges]
         for edge in bidirectional_edges:
             self.logic[edge][5] = False
-            new_edge_id = 1+max(self.logic)
-            self.logic[new_edge_id] = [ self.logic[edge][0], self.logic[edge][2], self.logic[edge][1], self.logic[edge][3], self.logic[edge][4][:], False ]
-        any_will_ability_edges = [edge for edge in self.logic if any(req[0] == 608 for req in self.logic[edge][4]) and edge not in unused_edges]
+            new_edge_id = 1 + max(self.logic)
+            self.logic[new_edge_id] = [self.logic[edge][0], self.logic[edge][2], self.logic[edge][1],
+                                       self.logic[edge][3], self.logic[edge][4][:], False]
+        any_will_ability_edges = [edge for edge in self.logic if
+                                  any(req[0] == 608 for req in self.logic[edge][4]) and edge not in unused_edges]
         unused_items.append(608)
         unused_edges.extend(any_will_ability_edges)
         for edge in any_will_ability_edges:
-            self.logic[edge][4].remove([608,1])
-            for will_ability in [61,62,63]:
-                new_edge_id = 1+max(self.logic)
-                self.logic[new_edge_id] = [ self.logic[edge][0], self.logic[edge][1], self.logic[edge][2], self.logic[edge][3], self.logic[edge][4][:]+[[will_ability,1]], self.logic[edge][5] ]
-        any_ranged_ability_edges = [edge for edge in self.logic if any(req[0] == 610 for req in self.logic[edge][4]) and edge not in unused_edges]
+            self.logic[edge][4].remove([608, 1])
+            for will_ability in [61, 62, 63]:
+                new_edge_id = 1 + max(self.logic)
+                self.logic[new_edge_id] = [self.logic[edge][0], self.logic[edge][1], self.logic[edge][2],
+                                           self.logic[edge][3], self.logic[edge][4][:] + [[will_ability, 1]],
+                                           self.logic[edge][5]]
+        any_ranged_ability_edges = [edge for edge in self.logic if
+                                    any(req[0] == 610 for req in self.logic[edge][4]) and edge not in unused_edges]
         unused_items.append(610)
         unused_edges.extend(any_ranged_ability_edges)
         for edge in any_ranged_ability_edges:
-            self.logic[edge][4].remove([610,1])
-            for ranged_ability in [64,67]:   # Friar-0, Firebird
-                new_edge_id = 1+max(self.logic)
-                self.logic[new_edge_id] = [ self.logic[edge][0], self.logic[edge][1], self.logic[edge][2], self.logic[edge][3], self.logic[edge][4][:]+[[ranged_ability,1]], self.logic[edge][5] ]
+            self.logic[edge][4].remove([610, 1])
+            for ranged_ability in [64, 67]:  # Friar-0, Firebird
+                new_edge_id = 1 + max(self.logic)
+                self.logic[new_edge_id] = [self.logic[edge][0], self.logic[edge][1], self.logic[edge][2],
+                                           self.logic[edge][3], self.logic[edge][4][:] + [[ranged_ability, 1]],
+                                           self.logic[edge][5]]
                 if ranged_ability == 67:
-                    self.logic[new_edge_id][4].append([602,1])
+                    self.logic[new_edge_id][4].append([602, 1])
         if self.flute == "Start":
             # If we start with flute, we have Any-Attack and Telekinesis
             free_items.append(609)
             free_items.append(612)
         else:
-            any_attack_edges = [edge for edge in self.logic if any(req[0] == 609 for req in self.logic[edge][4]) and edge not in unused_edges]
+            any_attack_edges = [edge for edge in self.logic if
+                                any(req[0] == 609 for req in self.logic[edge][4]) and edge not in unused_edges]
             unused_items.append(609)
             unused_edges.extend(any_attack_edges)
             for edge in any_attack_edges:
-                self.logic[edge][4].remove([609,1])
-                new_edge_id = 1+max(self.logic)
-                self.logic[new_edge_id] = [ self.logic[edge][0], self.logic[edge][1], self.logic[edge][2], 0x06, self.logic[edge][4][:], self.logic[edge][5] ]   # F/S always have an attack
-                for attack_item in [61,62,63,64,65,67,604]:
-                    new_edge_id = 1+max(self.logic)
-                    self.logic[new_edge_id] = [ self.logic[edge][0], self.logic[edge][1], self.logic[edge][2], 0, self.logic[edge][4][:]+[[attack_item,1]], self.logic[edge][5] ]
+                self.logic[edge][4].remove([609, 1])
+                new_edge_id = 1 + max(self.logic)
+                self.logic[new_edge_id] = [self.logic[edge][0], self.logic[edge][1], self.logic[edge][2], 0x06,
+                                           self.logic[edge][4][:], self.logic[edge][5]]  # F/S always have an attack
+                for attack_item in [61, 62, 63, 64, 65, 67, 604]:
+                    new_edge_id = 1 + max(self.logic)
+                    self.logic[new_edge_id] = [self.logic[edge][0], self.logic[edge][1], self.logic[edge][2], 0,
+                                               self.logic[edge][4][:] + [[attack_item, 1]], self.logic[edge][5]]
                     if attack_item == 67:
-                        self.logic[new_edge_id][4].append([602,1])   # Firebird is an attack only if Firebird is enabled
+                        self.logic[new_edge_id][4].append([602, 1])  # Firebird is an attack only if Firebird is enabled
             if self.flute == "Fluteless":
                 # Telekinesis is free in Fluteless
                 free_items.append(612)
             else:
                 # Replace telekinesis edges with F/S and Flute edges
-                telekinesis_edges = [edge for edge in self.logic if any(req[0] == 612 for req in self.logic[edge][4]) and edge not in unused_edges]
+                telekinesis_edges = [edge for edge in self.logic if
+                                     any(req[0] == 612 for req in self.logic[edge][4]) and edge not in unused_edges]
                 unused_items.append(612)
                 unused_edges.extend(telekinesis_edges)
                 for edge in telekinesis_edges:
-                    self.logic[edge][4].remove([612,1])
-                    new_edge_id = 1+max(self.logic)
-                    self.logic[new_edge_id] = [ self.logic[edge][0], self.logic[edge][1], self.logic[edge][2], 0x06, self.logic[edge][4][:], self.logic[edge][5] ]
-                    new_edge_id = 1+max(self.logic)
-                    self.logic[new_edge_id] = [ self.logic[edge][0], self.logic[edge][1], self.logic[edge][2], 0, self.logic[edge][4][:]+[[604, 1]], self.logic[edge][5] ]
-        
+                    self.logic[edge][4].remove([612, 1])
+                    new_edge_id = 1 + max(self.logic)
+                    self.logic[new_edge_id] = [self.logic[edge][0], self.logic[edge][1], self.logic[edge][2], 0x06,
+                                               self.logic[edge][4][:], self.logic[edge][5]]
+                    new_edge_id = 1 + max(self.logic)
+                    self.logic[new_edge_id] = [self.logic[edge][0], self.logic[edge][1], self.logic[edge][2], 0,
+                                               self.logic[edge][4][:] + [[604, 1]], self.logic[edge][5]]
+
         # Statue/Endgame logic
         if self.goal == "Red Jewel Hunt":
-            for jeweler_final_edge in [24,25,26,27]:
+            for jeweler_final_edge in [24, 25, 26, 27]:
                 self.logic[jeweler_final_edge][2] = 492
-            unused_edges.extend([406,407])
+            unused_edges.extend([406, 407])
         else:
             for x in self.statues:
                 self.logic[406][4][x][1] = 1
             if self.statue_req == StatueReq.PLAYER_CHOICE.value:
                 self.item_pool[106][0] = 6
-                unused_items.extend([100,101,102,103,104,105])
+                unused_items.extend([100, 101, 102, 103, 104, 105])
             else:
                 unused_items.append(106)
-        
+
         # Remove Jeweler edges that require more RJ items than exist, to help the traverser
         if self.gem[6] > self.item_pool[1][0]:
             unused_edges.append(24)
             if self.gem[6] > 2 + self.item_pool[1][0]:
                 unused_edges.append(25)
                 if self.gem[6] > 3 + self.item_pool[1][0]:
                     unused_edges.append(26)
 
         # Dungeon Shuffle.
         # Clean up unused nodes and artificial items
-        if not self.dungeon_shuffle: # if self.dungeon_shuffle == "None" or self.dungeon_shuffle == "Basic":
-            free_items.append(525)   # Pyramid portals open
+        if not self.dungeon_shuffle:  # if self.dungeon_shuffle == "None" or self.dungeon_shuffle == "Basic":
+            free_items.append(525)  # Pyramid portals open
             unused_locs.append(525)  # Loc is unused as item is free
-            unused_nodes.append(525) # Node is unused as item is free
-            if True: # self.dungeon_shuffle == "None":
+            unused_nodes.append(525)  # Node is unused as item is free
+            if True:  # self.dungeon_shuffle == "None":
                 unused_items.append(800)
-                free_items.append(801)     
-        if self.dungeon_shuffle and self.coupled_exits: # == "Chaos":
+                free_items.append(801)
+        if self.dungeon_shuffle and self.coupled_exits:  # == "Chaos":
             # Reduce walking times by removing some empty corridors; stabilize dungeon generation by removing lower Mu corridors.
             # Inca U-turn + statue "puzzle"; Mine elevator; Angl empty water room;
             # Wat hall before + road to main hall, + corridor before spirit.
-            useless_exits = [118,119,137,138,225,236,237,238,239,240,398,407,583,584,585,586,597,598, 359,360,365,366]
+            useless_exits = [118, 119, 137, 138, 225, 236, 237, 238, 239, 240, 398, 407, 583, 584, 585, 586, 597, 598,
+                             359, 360, 365, 366]
             useless_nodes = list(set([self.exits[x][3] for x in useless_exits]))
             useless_edges = []
             useless_node_count = 0
             while useless_node_count < len(useless_nodes):
                 useless_node_count = len(useless_nodes)
                 for i in range(len(useless_nodes)):
                     n = useless_nodes[i]
                     useless_nodes.extend(self.graph[n][1])
                     for o in self.graph[n][1]:
                         useless_nodes.extend([p for p in self.graph if o in self.graph[p][1]])
                     here_edges = [e for e in self.logic if self.logic[e][1] == n or self.logic[e][2] == n]
-                    useless_nodes.extend([self.logic[e][1] for e in here_edges]+[self.logic[e][2] for e in here_edges])
+                    useless_nodes.extend(
+                        [self.logic[e][1] for e in here_edges] + [self.logic[e][2] for e in here_edges])
                     unused_edges.extend(here_edges)
                 useless_nodes = list(set(useless_nodes))
             unused_nodes.extend(useless_nodes)
             unused_exits.extend(useless_exits)
-        
+
         # Save explicit form requirements in the logic database
         for edge in self.logic:
-            if self.logic[edge][3] == 0 and self.logic[edge][4]:   # Edges with no reqs will be cleaned up later
+            if self.logic[edge][3] == 0 and self.logic[edge][4]:  # Edges with no reqs will be cleaned up later
                 reqs = self.logic[edge][4]
-                if not any(req[0] in self.form_items[f] for f in [0,1,2] for req in reqs):
+                if not any(req[0] in self.form_items[f] for f in [0, 1, 2] for req in reqs):
                     self.logic[edge][3] = 0x27
                 else:
                     self.logic[edge][3] |= (0x01 * any(req[0] in self.form_items[0] for req in reqs))
                     self.logic[edge][3] |= (0x02 * any(req[0] in self.form_items[1] for req in reqs))
                     self.logic[edge][3] |= (0x04 * any(req[0] in self.form_items[2] for req in reqs))
-        
+
         # Clean up the objects so designated based on seed settings
-        self.delete_objects(items=unused_items,locs=unused_locs,nodes=unused_nodes,edges=unused_edges,exits=unused_exits,with_close=True)
-        self.delete_objects(items=free_items,with_close=False)
-        
+        self.delete_objects(items=unused_items, locs=unused_locs, nodes=unused_nodes, edges=unused_edges,
+                            exits=unused_exits, with_close=True)
+        self.delete_objects(items=free_items, with_close=False)
+
         # Clean up edges that now require neither items nor a specific form, or that go nowhere
         free_edges = [edge for edge in self.logic if self.edge_formless(edge) and not self.logic[edge][4]]
         free_edges.extend([edge for edge in self.logic if self.logic[edge][1] == self.logic[edge][2]])
         for edge in free_edges:
             here_node = self.logic[edge][1]
             other_node = self.logic[edge][2]
             self.graph[here_node][1].append(other_node)
-        self.delete_objects(edges=free_edges,with_close=True)
+        self.delete_objects(edges=free_edges, with_close=True)
 
         # Incorporate item locations and logic edges into world graph
         for x in self.item_locations:
             self.graph[self.item_locations[x][0]][11].append(x)
         for y in self.logic:
             if self.logic[y][0] != -1:
                 self.graph[self.logic[y][1]][12].append(y)
                 self.graph[self.logic[y][2]][13].append(y)
-        
+
         # Boss Shuffle -- boss_order[n] is the boss of dungeon n, 0<=n<=6, 1<=boss<=7
         if "Boss Shuffle" in self.variant:
-            boss_door_exits = [1,4,7,10,13,16,19]
-            boss_defeat_exits = [3,6,9,12,15,18,21]
-            self.verbose("Boss order: "+str(self.boss_order))
+            boss_door_exits = [1, 4, 7, 10, 13, 16, 19]
+            boss_defeat_exits = [3, 6, 9, 12, 15, 18, 21]
+            self.verbose("Boss order: " + str(self.boss_order))
             for dungeon in range(7):
                 this_dungeon_boss = self.boss_order[dungeon]
                 normal_boss_exit = boss_door_exits[dungeon]
-                new_boss_exit = boss_door_exits[this_dungeon_boss-1]
+                new_boss_exit = boss_door_exits[this_dungeon_boss - 1]
                 self.link_exits(normal_boss_exit, new_boss_exit)
                 normal_defeat_exit = boss_defeat_exits[dungeon]
-                new_defeat_exit = boss_defeat_exits[this_dungeon_boss-1]
+                new_defeat_exit = boss_defeat_exits[this_dungeon_boss - 1]
                 self.link_exits(new_defeat_exit, normal_defeat_exit)
-        
+
         # Cache the number of item pools, and create empty loc lists for them
         self.item_pool_count = 1 + self.get_max_pool_id()
-        self.open_locations = [ [] for _ in range(self.item_pool_count) ]
+        self.open_locations = [[] for _ in range(self.item_pool_count)]
 
-        self.reset_progress(True)          # Initialize graph with no items or logic
-        self.update_graph(True,True,True)  # Build basic graph connections from any unrandomized elements
+        self.reset_progress(True)  # Initialize graph with no items or logic
+        self.update_graph(True, True, True)  # Build basic graph connections from any unrandomized elements
 
         return True
 
-
     # Delete or hide sets of objects and linked objects. If with_close, an edge is deleted if any
     # required item is deleted; otherwise the item is just removed as a requirement.
     # Deleted objects are retained in deleted_* dicts to maintain their assembly labels and referential integrity.
     # For that reason, deleted items and locs aren't unfilled.
     # Exits remain in self.exits because, when shuffling, other exits still need to act-like the deleted exit.
     def delete_objects(self, items=[], locs=[], nodes=[], edges=[], exits=[], with_close=True):
         del_items = [x for x in items if x in self.item_pool]
@@ -2322,53 +2361,54 @@
                 else:
                     req = next(r for r in self.logic[edge][4] if r[0] == item)
                     self.logic[edge][4].remove(req)
             del self.item_pool[item]
         for node in set(del_nodes):
             self.deleted_graph[node] = self.graph[node]
             affected_locs = [loc for loc in self.item_locations if self.item_locations[loc][0] == node]
-            affected_nodes = [n for n in self.graph if node in self.graph[n][1] + self.graph[n][8] + self.graph[n][9] + self.graph[n][10]]
+            affected_nodes = [n for n in self.graph if
+                              node in self.graph[n][1] + self.graph[n][8] + self.graph[n][9] + self.graph[n][10]]
             affected_edges = [e for e in self.logic if node == self.logic[e][1] or node == self.logic[e][2]]
             affected_exits = [x for x in self.exits if self.exits[x][3] == node or self.exits[x][4] == node]
             del_locs.extend(affected_locs)
             del_edges.extend(affected_edges)
-            for other_node,subidx in itertools.product(affected_nodes,[1, 8, 9, 10]):
+            for other_node, subidx in itertools.product(affected_nodes, [1, 8, 9, 10]):
                 if node in self.graph[other_node][subidx]:
                     self.graph[other_node][subidx].remove(node)
             for exit in affected_exits:
                 if self.exits[exit][3] == node:
-                    self.exits[exit][3] = -1   # Exit source becomes "inaccessible"
+                    self.exits[exit][3] = -1  # Exit source becomes "inaccessible"
                 if self.exits[exit][4] == node:
-                    self.exits[exit][4] = -2   # Exit dest becomes "deleted"
+                    self.exits[exit][4] = -2  # Exit dest becomes "deleted"
             del self.graph[node]
         for loc in set(del_locs):
             self.deleted_item_locations[loc] = self.item_locations[loc]
             affected_nodes = [n for n in self.graph if loc in self.graph[n][11]]
             for node in affected_nodes:
                 self.graph[node][11].remove(loc)
             del self.item_locations[loc]
         for edge in set(del_edges):
             self.deleted_logic[edge] = self.logic[edge]
             affected_nodes = [n for n in self.graph if edge in self.graph[n][12] + self.graph[n][13]]
             for node in affected_nodes:
-                for subidx in [12,13]:
+                for subidx in [12, 13]:
                     if edge in self.graph[node][subidx]:
                         self.graph[node][subidx].remove(edge)
             del self.logic[edge]
         for exit in set(del_exits):
             if self.exits[exit][1] < 0 and self.exits[exit][0] > 0:
                 self.link_exits(exit, self.exits[exit][0], False, False)
             self.deleted_exits[exit] = self.exits[exit]
             affected_nodes = [n for n in self.graph if exit in self.graph[n][14] + self.graph[n][15]]
-            for node,subidx in itertools.product(affected_nodes,[14,15]):
+            for node, subidx in itertools.product(affected_nodes, [14, 15]):
                 if exit in self.graph[node][subidx]:
                     self.graph[node][subidx].remove(exit)
 
     # Simulate inventory
-    def get_inventory(self,start_items=[],item_destinations=[],new_nodes=[]):
+    def get_inventory(self, start_items=[], item_destinations=[], new_nodes=[]):
         if not start_items:
             start_items = self.items_collected[:]
         if not item_destinations:
             item_destinations = self.item_destinations[:]
         inventory_temp = []
         for item in start_items:
             if self.item_pool[item][4]:
@@ -2378,21 +2418,20 @@
             item = inventory_temp.pop(0)
             if item in item_destinations:
                 item_destinations.remove(item)
             else:
                 inventory.append(item)
         return inventory
 
-
     # Takes a random seed and builds out a randomized world
     def randomize(self, seed_adj=0, printlevel=-1, break_on_error=False, break_on_init=False):
         self.printlevel = printlevel
         self.break_on_error = break_on_error
-        
-        random.seed(self.seed + seed_adj)   # 3229535
+
+        random.seed(self.seed + seed_adj)  # 3229535
         if self.race_mode:
             for i in range(random.randint(100, 1000)):
                 _ = random.randint(0, 10000)
 
         if break_on_init:
             breakpoint()
         if not self.initialize():
@@ -2410,113 +2449,120 @@
 
         # Shuffle exits
         if self.entrance_shuffle:
             if not self.shuffle_exits():
                 self.error("Entrance rando failed")
                 return False
 
-        self.reset_progress(True)           # Forget items and logic used for ER/DS skeleton construction
-        self.update_graph(True,True,True)   # Rebuild graph connections with exits
+        self.reset_progress(True)  # Forget items and logic used for ER/DS skeleton construction
+        self.update_graph(True, True, True)  # Rebuild graph connections with exits
 
         # Initialize and shuffle location list
         item_locations = self.list_item_locations(shuffled_only=True)
         random.shuffle(item_locations)
 
         # Populate various pseudo-item pools
         self.fill_statues()
         self.map_rewards()
-        
+
         # Populate Dark Spaces; all non-DS items are granted so traversal can go to all DS-requiring edges
         self.reset_progress(True)
         self.items_collected = self.list_typed_items(types=[1], shuffled_only=False, incl_placed=True)
         if self.orb_rando != "None":
             self.items_collected.extend(self.list_typed_items(types=[5], shuffled_only=False, incl_placed=True))
-        self.update_graph(True,True,True)
+        self.update_graph(True, True, True)
         ds_items = self.list_typed_items(types=[2], shuffled_only=True, incl_placed=False)
         random.shuffle(ds_items)
         self.info("Populating Dark Spaces...")
         cycle = 0
         while True:
             cycle += 1
             if cycle >= MAX_CYCLES:
                 self.error("Couldn't populate DS items for an unknown reason")
                 return False
             if not ds_items:
                 # All remaining unoccupied dungeon DSes are for transform
                 for loc in self.spawn_locations:
-                    if self.spawn_locations[loc][3] and loc in self.item_locations and self.item_locations[loc][1] == 2 and not self.item_locations[loc][3]:
+                    if self.spawn_locations[loc][3] and loc in self.item_locations and self.item_locations[loc][
+                        1] == 2 and not self.item_locations[loc][3]:
                         self.item_locations[loc][2] = True
-                self.update_graph(True,True,False)
+                self.update_graph(True, True, False)
                 if self.logic_mode != "Completable":
-                    break    # Good enough: all DSes are populated and formful access isn't mandatory
+                    break  # Good enough: all DSes are populated and formful access isn't mandatory
             traverse_result = self.traverse()
             new_nodes = traverse_result[0]
             # A node needs a txform DS if it has an open formful edge, isn't accessible by that form, and the edge goes to an unreached area
-            f_missing_nodes = {self.logic[e][1] for e in self.open_edges if not self.edge_formless(e) and not (self.logic[e][3] & self.graph[self.logic[e][1]][4]) and not self.is_accessible(self.logic[e][2])}
+            f_missing_nodes = {self.logic[e][1] for e in self.open_edges if not self.edge_formless(e) and not (
+                    self.logic[e][3] & self.graph[self.logic[e][1]][4]) and not self.is_accessible(
+                self.logic[e][2])}
             if not f_missing_nodes and not ds_items:
-                break    # Success: no DS items left to place and no open formful edges to new areas
+                break  # Success: no DS items left to place and no open formful edges to new areas
             made_progress = False
             if f_missing_nodes:
                 # Lock txform DSes to cover nodes that need a form and aren't known to be accessible by that form
                 f_nodes_under_ds_node = {}
                 for node in f_missing_nodes:
                     for ds_node in self.graph[node][9]:
                         ds_loc = next(loc for loc in self.graph[ds_node][11] if self.item_locations[loc][1] == 2)
                         if self.graph[ds_node][0] and not self.item_locations[ds_loc][2]:
                             if ds_node not in f_nodes_under_ds_node:
                                 f_nodes_under_ds_node[ds_node] = set()
                             f_nodes_under_ds_node[ds_node].add(node)
                 while f_missing_nodes and f_nodes_under_ds_node:
                     # Lock the DS that covers the most remaining f nodes, breaking ties randomly
-                    lock_node = max(f_nodes_under_ds_node, key=lambda ds_node : len(f_missing_nodes.intersection(f_nodes_under_ds_node[ds_node]))+random.random() )
-                    lock_loc = next(loc for loc in self.item_locations if self.item_locations[loc][0] == lock_node and self.item_locations[loc][1] == 2)
-                    self.item_locations[lock_loc][2] = True   # Mark the DS as occupied, remove it from the pool, and clear its contents if any
+                    lock_node = max(f_nodes_under_ds_node, key=lambda ds_node: len(
+                        f_missing_nodes.intersection(f_nodes_under_ds_node[ds_node])) + random.random())
+                    lock_loc = next(loc for loc in self.item_locations if
+                                    self.item_locations[loc][0] == lock_node and self.item_locations[loc][1] == 2)
+                    self.item_locations[lock_loc][
+                        2] = True  # Mark the DS as occupied, remove it from the pool, and clear its contents if any
                     if self.item_locations[lock_loc][3]:
                         self.unfill_item(lock_loc)
                     self.item_locations[lock_loc][7] = 0
-                    self.info(" Locked for transform: "+str(self.item_locations[lock_loc][6]))
+                    self.info(" Locked for transform: " + str(self.item_locations[lock_loc][6]))
                     made_progress = True
                     f_missing_nodes = f_missing_nodes.difference(f_nodes_under_ds_node[lock_node])
                     for covered_node in f_nodes_under_ds_node[lock_node]:
                         for ds_node in f_nodes_under_ds_node:
                             if ds_node != lock_node and covered_node in f_nodes_under_ds_node[ds_node]:
                                 f_nodes_under_ds_node[ds_node].remove(covered_node)
                     del f_nodes_under_ds_node[lock_node]
                     while any(len(f_nodes_under_ds_node[ds_node]) == 0 for ds_node in f_nodes_under_ds_node):
-                        del f_nodes_under_ds_node[next(ds_node for ds_node in f_nodes_under_ds_node if len(f_nodes_under_ds_node[ds_node]) == 0)]
+                        del f_nodes_under_ds_node[next(
+                            ds_node for ds_node in f_nodes_under_ds_node if len(f_nodes_under_ds_node[ds_node]) == 0)]
                 if len(f_missing_nodes) > 0 and not made_progress and not ds_items:
                     # Can't expand formful access, and there are no more items to grant progress, so we're stuck
                     for n in f_missing_nodes:
-                        self.warn("No formless access from or formful access to "+str(n)+" "+self.graph[n][5])
+                        self.warn("No formless access from or formful access to " + str(n) + " " + self.graph[n][5])
                     if self.logic_mode == "Completable":
                         self.error("World is unsolvable: missing form access")
                         return False
                 # Reinitialize Dark Space access since more may now be for transform
-                self.update_graph(True,True,False)
+                self.update_graph(True, True, False)
             if ds_items:
                 # Now no accessible nodes are missing a form due to DS access, so we can safely place a DS item
-                progression_result = self.progression_list(ignore_inv=True,penalty_threshold=(6-len(ds_items)))
-                if not progression_result[0]:   # try again without the penalty
+                progression_result = self.progression_list(ignore_inv=True, penalty_threshold=(6 - len(ds_items)))
+                if not progression_result[0]:  # try again without the penalty
                     progression_result = self.progression_list(ignore_inv=True)
                 progression_list = [itemset for itemset in progression_result[0] if itemset[0] in ds_items]
                 if progression_list:
                     # Monte Carlo style
-                    key = random.uniform(0,100)
+                    key = random.uniform(0, 100)
                     progression_mc = self.monte_carlo(progression_list)
                     idx = 0
                     for x in progression_mc:
                         if key <= x[0] and not idx:
                             idx = x[1]
                     items = progression_list.pop(idx)
                     if self.forward_fill(items, item_locations, False, self.logic_mode == "Chaos"):
-                        self.info(" Placed "+self.item_pool[items[0]][3]+" for progression")
+                        self.info(" Placed " + self.item_pool[items[0]][3] + " for progression")
                         made_progress = True
                         for item in items:
                             ds_items.remove(item)
-                elif len(new_nodes) == 1:   # (the start node always counts as new)
+                elif len(new_nodes) == 1:  # (the start node always counts as new)
                     # The graph is maxed out and the other DS items aren't progression, so place them randomly
                     if self.forward_fill(ds_items, item_locations, False, self.logic_mode == "Chaos"):
                         self.info(" Placed remaining DS items")
                         made_progress = True
                         ds_items = []
             if not made_progress:
                 if len(f_missing_nodes) > 0 and len(ds_items) > 0:
@@ -2534,128 +2580,128 @@
         for item in non_prog_items:
             if item in self.items_collected:
                 self.items_collected.remove(item)
         self.forward_fill(non_prog_items, item_locations, False, self.logic_mode == "Chaos")
         # Forget collected items and edges; rebuild the graph with DSes set, ready to place items
         self.info("Beginning item placement...")
         self.reset_progress(True)
-        self.update_graph(True,True,False)   # no need to recalculate exits again
+        self.update_graph(True, True, False)  # no need to recalculate exits again
         high_penalty_items = {item for item in self.item_pool if self.item_pool[item][7] > 1}
         for loc in self.item_locations:
-            self.item_locations[loc][8] = MAX_CYCLES   # Initialize discovered-on-cycle value
+            self.item_locations[loc][8] = MAX_CYCLES  # Initialize discovered-on-cycle value
         done = False
         goal = False
         cycle = 0
         while not done:
             cycle += 1
-            self.info(" Cycle "+str(cycle))
+            self.info(" Cycle " + str(cycle))
             if cycle > MAX_CYCLES:
                 self.error("Max cycles exceeded in item placement")
                 return False
             self.traverse()
             # Good items resist being placed early; very good items can't be placed early at all
-            discovered_locs = [loc for loc in self.item_locations if self.graph[self.item_locations[loc][0]][0] and self.item_locations[loc][8] > cycle]
+            discovered_locs = [loc for loc in self.item_locations if
+                               self.graph[self.item_locations[loc][0]][0] and self.item_locations[loc][8] > cycle]
             for loc in discovered_locs:
                 self.item_locations[loc][8] = cycle
                 for item in high_penalty_items:
-                    if item not in self.item_locations[loc][4] and cycle < (self.item_pool[item][7] * 1.5 / PROGRESS_ADJ[self.difficulty]):
+                    if item not in self.item_locations[loc][4] and cycle < (
+                            self.item_pool[item][7] * 1.5 / PROGRESS_ADJ[self.difficulty]):
                         self.item_locations[loc][4].append(item)
             if len(self.get_inventory()) > MAX_INVENTORY:
                 goal = False
                 self.warn("Inventory capacity exceeded")
             else:
                 goal = self.is_accessible(492)
-            
-            progression_result = [ [], [], [] ]
-            trial_penalty = cycle/4
-            while not progression_result[0] and trial_penalty <= 8*cycle:
+
+            progression_result = [[], [], []]
+            trial_penalty = cycle / 4
+            while not progression_result[0] and trial_penalty <= 8 * cycle:
                 # The penalty threshold is lightened until progression is found
                 progression_result = self.progression_list(penalty_threshold=trial_penalty)
                 trial_penalty *= 2
             self.verbose("Progression options: {")
-            self.verbose(" "+str(progression_result[0]))   # Available
-            self.verbose(" "+str(progression_result[1]))   # Not enough locs
-            self.verbose(" "+str(progression_result[2]))   # Not enough inv space
+            self.verbose(" " + str(progression_result[0]))  # Available
+            self.verbose(" " + str(progression_result[1]))  # Not enough locs
+            self.verbose(" " + str(progression_result[2]))  # Not enough inv space
             self.verbose("}")
             progression_list = progression_result[0]
-            is_progression = (progression_result != [[],[],[]])
+            is_progression = (progression_result != [[], [], []])
             done = goal and (self.logic_mode != "Completable" or not is_progression)
 
             if not done:
                 if not is_progression:
                     self.error("World is unsolvable: can't progress further")
                     return False
 
                 progress = False
-                key = random.uniform(0,100)
+                key = random.uniform(0, 100)
                 while not progress and progression_list:
                     progression_mc = self.monte_carlo(progression_list)
                     idx = 0
                     for x in progression_mc:
                         if key <= x[0] and not idx:
                             idx = x[1]
                     items = progression_list.pop(idx)
                     if self.forward_fill(items, item_locations, False, self.logic_mode == "Chaos", True):
                         progress = True
-                        self.info("  Placed "+str(len(items))+" items successfully")
+                        self.info("  Placed " + str(len(items)) + " items successfully")
                 if not progress:
                     self.info("Removing some junk to make room...")
                     if not self.make_room(progression_result):
                         self.error("World is unsolvable: can't place progression items")
                         return False
 
         self.info("Placing leftover items...")
         junk_items = self.list_typed_items(types=[], shuffled_only=True)
         self.random_fill(junk_items, item_locations, False)
 
         self.info("Verifying completion...")
 
         self.reset_progress(True)
         self.update_graph()
-        self.traverse([])    # Fresh traverse with no nodes queued to visit
+        self.traverse([])  # Fresh traverse with no nodes queued to visit
 
         if self.logic_mode == "Completable" and self.goal != "Red Jewel Hunt":
             completed = all(self.graph[node][0] for node in self.graph if node not in self.optional_nodes)
         else:
             completed = self.graph[492][0]
         if not completed:
-            #self.print_graph()
+            # self.print_graph()
             unreachable = [node for node in self.graph if not self.graph[node][0] and node not in self.optional_nodes]
             for node in unreachable:
-                self.warn("Can't reach node "+str(node)+" "+str(self.graph[node]))
+                self.warn("Can't reach node " + str(node) + " " + str(self.graph[node]))
             self.error("Seed failed, trying again...")
             return False
 
         self.info("Writing hints...")
         placement_log = self.placement_log[:]
         random.shuffle(placement_log)
         self.in_game_spoilers(placement_log)
 
         self.info("Randomization complete")
 
         return True
-    
 
     def print_graph(self):
-        self.info("Open edges: "+str(self.open_edges))
-        self.info("Open locations: "+str(self.open_locations))
+        self.info("Open edges: " + str(self.open_edges))
+        self.info("Open locations: " + str(self.open_locations))
         for node in self.graph:
-            self.info(str(node)+" "+str(self.graph[node]))
-
+            self.info(str(node) + " " + str(self.graph[node]))
 
     # Prepares dataset to give in-game spoilers
     def in_game_spoilers(self, placement_log=[]):
         for x in placement_log:
             item = x[0]
             location = x[1]
             if location not in self.free_locations and location in self.area_short_name:
                 if item in self.required_items or item in self.good_items or location in self.trolly_locations:
-                    spoiler_str = self.area_short_name[location] + " has ]"   # ']' is a newline
+                    spoiler_str = self.area_short_name[location] + " has ]"  # ']' is a newline
                     if len(self.item_pool[item][3]) >= 26:
-                        spoiler_str += self.item_pool[item][3].replace(' ','_',2).replace(' ',']',1)
+                        spoiler_str += self.item_pool[item][3].replace(' ', '_', 2).replace(' ', ']', 1)
                     else:
                         spoiler_str += self.item_pool[item][3]
                     # No in-game spoilers in Expert mode
                     if self.difficulty >= 3:
                         spoiler_str = "nice try dodongo!"
                     self.spoilers.append(spoiler_str)
                     # print item, location
@@ -2701,46 +2747,45 @@
         spoiler["jeweler_amounts"] = self.gem
         spoiler["inca_tiles"] = self.incatile
         spoiler["hieroglyph_order"] = self.hieroglyphs
 
         items = []
         for x in self.item_locations:
             loc_type = self.item_locations[x][1]
-            if loc_type in [1,2,3] or (self.orb_rando != "None" and loc_type == 5):
+            if loc_type in [1, 2, 3] or (self.orb_rando != "None" and loc_type == 5):
                 item = self.item_locations[x][3]
                 location_name = self.item_locations[x][6].strip()
                 item_name = self.item_pool[item][3]
                 items.append({"location": location_name, "name": item_name})
         spoiler["items"] = items
 
         if "Overworld Shuffle" in self.variant:
             overworld_links = []
             for continent_id, continent_data in self.overworld_menus.items():
                 continent_name = continent_data[5]
                 region_name = self.overworld_menus[continent_data[0]][6]
-                region_name = region_name.replace('_','')
+                region_name = region_name.replace('_', '')
                 overworld_links.append({"region": region_name, "continent": continent_name})
             spoiler["overworld_entrances"] = overworld_links
 
         if self.entrance_shuffle:
             exit_links = []
             for exit in self.exits:
                 exit_name = self.exits[exit][10]
                 linked_exit = self.exits[exit][1]
-                if linked_exit:    # i.e. this acts like linked_exit, going to the area normally on the other side of linked_exit
+                if linked_exit:  # i.e. this acts like linked_exit, going to the area normally on the other side of linked_exit
                     coupled_linked_exit = self.exits[linked_exit][0]
-                    if coupled_linked_exit:    # in this case the exit leads to where the acted-like exit's coupled exit is
-                        target_name = "Near "+self.exits[coupled_linked_exit][10]
-                    else:    # the acted-like exit is one-way, so derive a destination name from the exit name
-                        target_name = "Target of "+self.exits[linked_exit][10]
+                    if coupled_linked_exit:  # in this case the exit leads to where the acted-like exit's coupled exit is
+                        target_name = "Near " + self.exits[coupled_linked_exit][10]
+                    else:  # the acted-like exit is one-way, so derive a destination name from the exit name
+                        target_name = "Target of " + self.exits[linked_exit][10]
                     exit_links.append({"transition": exit_name, "destination": target_name})
             spoiler["exit_links"] = exit_links
 
         self.spoiler = spoiler
-        
 
     # Prints item and ability locations
     def print_spoiler(self):
         if self.kara == 1:
             kara_txt = "Edward's Castle"
         elif self.kara == 2:
             kara_txt = "Diamond Mine"
@@ -2748,63 +2793,63 @@
             kara_txt = "Angel Dungeon"
         elif self.kara == 4:
             kara_txt = "Mt. Kress"
         elif self.kara == 5:
             kara_txt = "Ankor Wat"
 
         self.info("")
-        self.info("Seed                                   >  "+str(self.seed))
-        self.info("Statues Required                       >  "+str(self.statues))
-        self.info("Kara Location                          >  "+str(kara_txt))
-        self.info("Jeweler Reward Amounts                 >  "+str(self.gem))
-        self.info("Inca Tile (column, row)                >  "+str(self.incatile))
-        self.info("Hieroglyph Order                       >  "+str(self.hieroglyphs))
+        self.info("Seed                                   >  " + str(self.seed))
+        self.info("Statues Required                       >  " + str(self.statues))
+        self.info("Kara Location                          >  " + str(kara_txt))
+        self.info("Jeweler Reward Amounts                 >  " + str(self.gem))
+        self.info("Inca Tile (column, row)                >  " + str(self.incatile))
+        self.info("Hieroglyph Order                       >  " + str(self.hieroglyphs))
         self.info("")
 
         for x in self.item_locations:
             item = self.item_locations[x][3]
             location_name = self.item_locations[x][6]
             item_name = self.item_pool[item][3]
-            self.info(str(location_name)+"  >  "+str(item_name))
+            self.info(str(location_name) + "  >  " + str(item_name))
 
     # Generate assembly define dict based on World state
     def populate_asar_defines(self):
         # Room-clearing rewards
         for i in range(0x100):
-            self.asar_defines["RoomClearReward"+format(i,"02X")] = 0
+            self.asar_defines["RoomClearReward" + format(i, "02X")] = 0
         idx_tier2 = 1
         idx_tier3 = 1
         idx_tier4 = 1
-        for i in range(1,7):
-            self.asar_defines["RemovedRoomRewardExpertFlag"+str(i)] = 0
-            self.asar_defines["RemovedRoomRewardAdvancedFlag"+str(i)] = 0
-            self.asar_defines["RemovedRoomRewardIntermediateFlag"+str(i)] = 0
+        for i in range(1, 7):
+            self.asar_defines["RemovedRoomRewardExpertFlag" + str(i)] = 0
+            self.asar_defines["RemovedRoomRewardAdvancedFlag" + str(i)] = 0
+            self.asar_defines["RemovedRoomRewardIntermediateFlag" + str(i)] = 0
         for map in self.maps:
             reward_tier = self.maps[map][2][1]
             if reward_tier > 0:
                 reward = self.maps[map][2][0]
-                self.asar_defines["RoomClearReward"+format(map,"02X")] = reward
+                self.asar_defines["RoomClearReward" + format(map, "02X")] = reward
                 # Populate player level logic
                 if reward_tier == 4:
-                    self.asar_defines["RemovedRoomRewardIntermediateFlag"+str(idx_tier2)] = 0x300 + map
+                    self.asar_defines["RemovedRoomRewardIntermediateFlag" + str(idx_tier2)] = 0x300 + map
                     idx_tier2 += 1
                 elif reward_tier == 3:
-                    self.asar_defines["RemovedRoomRewardAdvancedFlag"+str(idx_tier3)] = 0x300 + map
+                    self.asar_defines["RemovedRoomRewardAdvancedFlag" + str(idx_tier3)] = 0x300 + map
                     idx_tier3 += 1
                 elif reward_tier == 2:
-                    self.asar_defines["RemovedRoomRewardExpertFlag"+str(idx_tier4)] = 0x300 + map
+                    self.asar_defines["RemovedRoomRewardExpertFlag" + str(idx_tier4)] = 0x300 + map
                     idx_tier4 += 1
 
         # Item placement
         ds_loc_idx = 1
         item_db = {}
         loc_db = {}
         for loc in self.item_locations:
             loc_db[loc] = self.item_locations[loc]
-        for loc in self.deleted_item_locations:   # Currently used for deleted (free) orb locs
+        for loc in self.deleted_item_locations:  # Currently used for deleted (free) orb locs
             loc_db[loc] = self.deleted_item_locations[loc]
         for item in self.item_pool:
             item_db[item] = self.item_pool[item]
         for item in self.deleted_item_pool:
             item_db[item] = self.deleted_item_pool[item]
         for x in loc_db:
             loc_type = loc_db[x][1]
@@ -2816,18 +2861,18 @@
                 self.asar_defines[loc_label] = item_id
             # Only six DS locs have items
             elif loc_type == 2:
                 item = loc_db[x][3]
                 item_id = item_db[item][2]
                 map = self.spawn_locations[x][1]
                 if item_id:
-                    self.asar_defines["DarkSpaceItem"+str(ds_loc_idx)+"Item"] = item_id
-                    self.asar_defines["DarkSpaceItem"+str(ds_loc_idx)+"Map"] = map
+                    self.asar_defines["DarkSpaceItem" + str(ds_loc_idx) + "Item"] = item_id
+                    self.asar_defines["DarkSpaceItem" + str(ds_loc_idx) + "Map"] = map
                     ds_loc_idx += 1
-                    
+
         # Write in-game spoilers
         i = 0
         for label in self.spoiler_labels:
             if i < len(self.spoilers):
                 self.asar_defines[self.spoiler_labels[label]] = self.spoilers[i]
                 i += 1
 
@@ -2841,148 +2886,150 @@
         self.asar_defines["StartLocationName"] = "South Cape"
         self.asar_defines["StartLocationId"] = 10
         if self.start_mode != "South Cape" or self.town_shuffle:
             self.asar_defines["StartAtWarpLocation"] = 1
             self.asar_defines["StartDsIndex"] = self.spawn_locations[self.start_loc][2]
             self.asar_defines["StartLocationName"] = self.area_short_name[self.start_loc]
             self.asar_defines["StartLocationId"] = self.start_loc
-        
+
         # Overworld
         for entry in self.overworld_menus:
             new_entry = entry
             if self.overworld_menus[entry][0] > 0:
                 new_entry = self.overworld_menus[entry][0]
             old_label = self.overworld_menus[entry][4]
             new_label = self.overworld_menus[new_entry][4]
-            self.asar_defines["OverworldShuffle"+old_label+"Label"] = new_label
-            self.asar_defines["OverworldShuffle"+old_label+"Text"] = self.overworld_menus[new_entry][6]
-            self.asar_defines["OverworldShuffle"+new_label+"MenuId"] = self.overworld_menus[entry][1]
-        
+            self.asar_defines["OverworldShuffle" + old_label + "Label"] = new_label
+            self.asar_defines["OverworldShuffle" + old_label + "Text"] = self.overworld_menus[new_entry][6]
+            self.asar_defines["OverworldShuffle" + new_label + "MenuId"] = self.overworld_menus[entry][1]
+
         # Entrances
         for exit in self.exits:
             new_exit = self.exits[exit][1]
             if new_exit > 0:
                 old_exit_label = self.exits[exit][5]
                 new_exit_string_label = self.exits[new_exit][5]
-                self.asar_defines[old_exit_label] = "!Default"+new_exit_string_label
-        
+                self.asar_defines[old_exit_label] = "!Default" + new_exit_string_label
+
         # Dark rooms
         if self.darkroom_level != "None":
-            self.asar_defines["SettingDarkRoomsLevel"] = { "None": 0, "Few": 1, "Some": 2, "Many": 3, "All": 4 }[self.darkroom_level]
+            self.asar_defines["SettingDarkRoomsLevel"] = {"None": 0, "Few": 1, "Some": 2, "Many": 3, "All": 4}[
+                self.darkroom_level]
             if len(self.all_darkrooms) > 0:
                 darkroom_str = ""
                 for room in self.all_darkrooms:
                     darkroom_str += str(room) + ","
-                    self.asar_defines["IsMap"+format(room,"02X")+"Dark"] = 1
+                    self.asar_defines["IsMap" + format(room, "02X") + "Dark"] = 1
                 darkroom_str += "$ff"
                 self.asar_defines["DarkMapList"] = darkroom_str
 
-        #print "ROM successfully created"
-
+        # print "ROM successfully created"
 
     # Pick random start location
     def random_start(self):
         if self.start_mode == "Safe":
             locations = [loc for loc in self.spawn_locations if self.spawn_locations[loc][0] == "Safe"]
         elif self.start_mode == "Unsafe":
-            locations = [loc for loc in self.spawn_locations if self.spawn_locations[loc][0] == "Safe" or self.spawn_locations[loc][0] == "Unsafe"]
-        else:   # "Forced Unsafe"
-            locations = [loc for loc in self.spawn_locations if self.spawn_locations[loc][0] == "Unsafe" or self.spawn_locations[loc][0] == "Forced Unsafe"]
+            locations = [loc for loc in self.spawn_locations if
+                         self.spawn_locations[loc][0] == "Safe" or self.spawn_locations[loc][0] == "Unsafe"]
+        else:  # "Forced Unsafe"
+            locations = [loc for loc in self.spawn_locations if
+                         self.spawn_locations[loc][0] == "Unsafe" or self.spawn_locations[loc][0] == "Forced Unsafe"]
         return locations[random.randint(0, len(locations) - 1)]
-    
-    
+
     # Dark rooms.
     def dr_randomize(self):
         if self.darkroom_cursed:
             max_cluster_size = 5
         else:
             max_cluster_size = 3
         darkness_clusters = []
         curr_cluster_idx = -1
         while len(self.all_darkrooms) < self.max_darkrooms:
             # If exactly 1 more room is needed, try growing an existing cluster
             if len(self.all_darkrooms) == self.max_darkrooms - 1:
                 this_cluster_idx = 0
-                while this_cluster_idx < len(darkness_clusters)-1:
+                while this_cluster_idx < len(darkness_clusters) - 1:
                     candidate_cluster = darkness_clusters[this_cluster_idx]
                     if len(candidate_cluster) < max_cluster_size:
                         if self.dr_spread_once(candidate_cluster):
-                            break   # It grew
+                            break  # It grew
                     this_cluster_idx += 1
             # If that didn't work or doesn't apply, add a new cluster
             if len(self.all_darkrooms) < self.max_darkrooms:
                 darkness_sources = [m for m in self.maps if self.maps[m][4] == 3 and m not in self.all_darkrooms]
                 random.shuffle(darkness_sources)
                 new_cluster = []
                 new_source = darkness_sources.pop(0)
                 if any(abs(m - new_source) < 4 for m in self.all_darkrooms):
                     # Try not to put clusters too close together
                     darkness_sources.append(new_source)
                     new_source = darkness_sources.pop(0)
                 new_cluster.append(new_source)
                 self.all_darkrooms.append(new_source)
                 # Spread to a random size between max/2 and max (or to the room cap or its boundary)
-                new_cluster_size = random.randint(1+int(max_cluster_size/2),max_cluster_size)
+                new_cluster_size = random.randint(1 + int(max_cluster_size / 2), max_cluster_size)
                 while (len(new_cluster) <= new_cluster_size) and (len(self.all_darkrooms) < self.max_darkrooms):
                     if not self.dr_spread_once(new_cluster):
-                        break    # The cluster hit a wall (e.g. a type-1 room if uncursed) and can't grow
+                        break  # The cluster hit a wall (e.g. a type-1 room if uncursed) and can't grow
                 # We're done with this cluster
                 darkness_clusters.append(new_cluster)
         # If uncursed, add logic edges for darkness
         if not self.darkroom_cursed:
-            dark_nodes = [n for n in self.graph if any(darkroom == self.graph[n][3][3] for darkroom in self.all_darkrooms)]
+            dark_nodes = [n for n in self.graph if
+                          any(darkroom == self.graph[n][3][3] for darkroom in self.all_darkrooms)]
             dark_exits = [x for x in self.exits if self.exits[x][3] in dark_nodes]
             for exit in dark_exits:
-                new_logic_id = 1+max(self.exit_logic)
-                new_logic = [exit, [[28, 1], [39, 1]], 2, False]   # Dark Glasses, Crystal Ring
+                new_logic_id = 1 + max(self.exit_logic)
+                new_logic = [exit, [[28, 1], [39, 1]], 2, False]  # Dark Glasses, Crystal Ring
                 self.exit_logic[new_logic_id] = new_logic
-        
+
     # Returns a list of non-dark rooms that darkness can spread to from cluster, of requested or default types.
     def dr_get_nondark_sinks(self, cluster, types):
         if not types:
             if not self.darkroom_cursed:
-                types = [2,3,4]
+                types = [2, 3, 4]
             else:
-                types = [1,2,3,4]
-        return [sink for src in cluster for sink in self.maps[src][9] if self.maps[sink][4] in types and sink not in self.all_darkrooms]
-    
+                types = [1, 2, 3, 4]
+        return [sink for src in cluster for sink in self.maps[src][9] if
+                self.maps[sink][4] in types and sink not in self.all_darkrooms]
+
     # Expands the darkness cluster into all adjacent rooms that inherit darkness.
     def dr_spread_to_free_sinks(self, cluster):
         new_free_sinks = [0]
         while new_free_sinks:
             new_free_sinks = self.dr_get_nondark_sinks(cluster, [4])
             cluster.extend(new_free_sinks)
             self.all_darkrooms.extend(new_free_sinks)
-    
+
     # Expands the darkness cluster by one room (plus any adjacent free sinks).
     def dr_spread_once(self, cluster):
         self.dr_spread_to_free_sinks(cluster)
         all_sinks = self.dr_get_nondark_sinks(cluster, [])
         if not all_sinks:
             return False
         random.shuffle(all_sinks)
         new_room = all_sinks.pop()
         self.all_darkrooms.append(new_room)
         cluster.append(new_room)
         self.dr_spread_to_free_sinks(cluster)
         return True
 
-
     # Shuffle travel destinations
     def shuffle_overworld(self):
-        new_continents = [[],[],[],[],[]]
+        new_continents = [[], [], [], [], []]
 
         # Ensure each continent has at least one travel location
-        destination_list = [1,6,12,14,16,18]
+        destination_list = [1, 6, 12, 14, 16, 18]
         random.shuffle(destination_list)
         for continent in new_continents:
             continent.append(destination_list.pop(0))
 
         # Randomly assign the rest of the locations
-        destination_list += [2,3,4,5,7,8,9,10,11,13,15,17,19]
+        destination_list += [2, 3, 4, 5, 7, 8, 9, 10, 11, 13, 15, 17, 19]
         random.shuffle(destination_list)
         new_continents[0] += destination_list[:4]
         new_continents[1] += destination_list[4:8]
         new_continents[2] += destination_list[8:10]
         new_continents[3] += destination_list[10:13]
         new_continents[4] += destination_list[-1:]
         for continent in new_continents:
@@ -3025,15 +3072,14 @@
             new_entry = self.overworld_menus[entry][0]
             self.graph[self.overworld_menus[entry][2]][1].append(self.overworld_menus[new_entry][3])
             self.graph[self.overworld_menus[new_entry][3]][1].remove(self.overworld_menus[new_entry][2])
             self.graph[self.overworld_menus[new_entry][3]][1].append(self.overworld_menus[entry][2])
 
         return True
 
-
     # Check whether this monster ID is compatible with this enemy type.
     def can_monster_be_type(self, monster_id, enemy_type):
         if monster_id in self.enemizer_restricted_enemies:
             if enemy_type in self.enemizer_restricted_enemies[monster_id]:
                 return False
         return True
 
@@ -3085,86 +3131,99 @@
             for enemy in self.enemies:
                 if self.enemies[enemy][0] == oldset:
                     old_enemies.append(enemy)
                 if self.enemies[enemy][0] == newset and self.enemies[enemy][5]:
                     new_enemies.append(enemy)
 
             # Update map header to reflect new enemyset
-            self.asar_defines["Map"+format(map,"02X")+"CardMonsters"] = "!"+self.enemysets[newset][0]
+            self.asar_defines["Map" + format(map, "02X") + "CardMonsters"] = "!" + self.enemysets[newset][0]
 
             # Randomize each enemy in map
             first_monster_id = self.maps[map][5]
             last_monster_id = self.maps[map][6]
             this_monster_id = first_monster_id
             while this_monster_id <= last_monster_id:
                 if this_monster_id not in self.default_enemies:
                     this_monster_id += 1
                     continue
                 old_enemy = self.default_enemies[this_monster_id]
                 enemytype = self.enemies[old_enemy][3]
                 walkable = self.enemies[old_enemy][4]
-                
+
                 random.shuffle(new_enemies)
                 i = 0
                 found_enemy = False
                 while not found_enemy:
                     new_enemy = new_enemies[i]
                     new_enemytype = self.enemies[new_enemy][3]
                     new_walkable = self.enemies[new_enemy][4]
-                    if (i == len(new_enemies) - 1) or (this_monster_id in self.enemizer_restricted_enemies and self.can_monster_be_type(this_monster_id,new_enemy)) or ((this_monster_id not in self.enemizer_restricted_enemies) and (complex_ct < max_complex or new_enemy not in complex_enemies) and (walkable or new_enemytype == 3 or walkable == new_walkable)):
+                    if (i == len(new_enemies) - 1) or (
+                            this_monster_id in self.enemizer_restricted_enemies and self.can_monster_be_type(
+                        this_monster_id, new_enemy)) or (
+                            (this_monster_id not in self.enemizer_restricted_enemies) and (
+                            complex_ct < max_complex or new_enemy not in complex_enemies) and (
+                                    walkable or new_enemytype == 3 or walkable == new_walkable)):
                         found_enemy = True
                         # Limit number of complex enemies per map
                         if new_enemy in complex_enemies:
                             complex_ct += 1
                     i += 1
-                self.asar_defines["Monster"+format(this_monster_id,"04X")+"Addr"] = "!"+self.enemies[new_enemy][1]
-                if map == 27:   # Moon Tribe doesn't shuffle stats
+                self.asar_defines["Monster" + format(this_monster_id, "04X") + "Addr"] = "!" + self.enemies[new_enemy][
+                    1]
+                if map == 27:  # Moon Tribe doesn't shuffle stats
                     new_enemy_stat_block = self.enemies[old_enemy][2]
-                elif self.enemizer == "Balanced":   # Balanced enemizer doesn't shuffle stats--
+                elif self.enemizer == "Balanced":  # Balanced enemizer doesn't shuffle stats--
                     new_enemy_stat_block = self.enemies[old_enemy][2]
-                    if old_enemy == 102:   # --except that we use the cyclops stat block for replaced zombies
+                    if old_enemy == 102:  # --except that we use the cyclops stat block for replaced zombies
                         new_enemy_stat_block = 0x47
-                elif self.enemizer == "Insane" and new_enemy != 102:   # Insane uses random stat blocks for non-zombies
+                elif self.enemizer == "Insane" and new_enemy != 102:  # Insane uses random stat blocks for non-zombies
                     new_enemy_stat_block = insane_dictionary[new_enemy]
-                else:   # Otherwise (Limited, Full, and zombies in Insane) the new monster uses its normal stat block
+                else:  # Otherwise (Limited, Full, and zombies in Insane) the new monster uses its normal stat block
                     new_enemy_stat_block = self.enemies[new_enemy][2]
-                self.asar_defines["Monster"+format(this_monster_id,"04X")+"Stats"] = new_enemy_stat_block
+                self.asar_defines["Monster" + format(this_monster_id, "04X") + "Stats"] = new_enemy_stat_block
 
                 # Nearly all monsters use Param to set layer priority (o = $00/$10/$20/$30),
                 # so should not override the Param (priority) of the monster they're replacing.
                 # Wat wall skulls use Param = 0/2/4/6 to set their movement direction.
                 # Inca statues with Param > 0 are frozen until a certain flag is set.
                 # So for wall skulls we want Param = a random direction, for Inca statues we want Param = 0,
                 # and for others we want to retain the priority bits but zero out the wall skull bits.
                 if new_enemy == 108:
-                    self.asar_defines["Monster"+format(this_monster_id,"04X")+"Param"] = random.randint(0,3) * 2
-                elif new_enemy in [16,17,18,19,20,21,22]:
-                    self.asar_defines["Monster"+format(this_monster_id,"04X")+"Param"] = 0
+                    self.asar_defines["Monster" + format(this_monster_id, "04X") + "Param"] = random.randint(0, 3) * 2
+                elif new_enemy in [16, 17, 18, 19, 20, 21, 22]:
+                    self.asar_defines["Monster" + format(this_monster_id, "04X") + "Param"] = 0
                 else:
-                    self.asar_defines["Monster"+format(this_monster_id,"04X")+"Param"] = "!DefaultMonster"+format(this_monster_id,"04X")+"Param&$F0"
-                
+                    self.asar_defines[
+                        "Monster" + format(this_monster_id, "04X") + "Param"] = "!DefaultMonster" + format(
+                        this_monster_id, "04X") + "Param&$F0"
+
                 this_monster_id += 1
 
     # Build world
-    def __init__(self, settings: RandomizerData, statues_required=6, statues=[1,2,3,4,5,6], statue_req=StatueReq.GAME_CHOICE.value, kara=3, gem=[3,5,8,12,20,30,50], incatile=[9,5], hieroglyphs=[1,2,3,4,5,6], boss_order=[1,2,3,4,5,6,7]):
+    def __init__(
+        self, settings: RandomizerData, statues_required=6, statues=[1, 2, 3, 4, 5, 6],
+        statue_req=StatueReq.GAME_CHOICE.value, kara=3, gem=[3, 5, 8, 12, 20, 30, 50], incatile=[9, 5],
+        hieroglyphs=[1, 2, 3, 4, 5, 6], boss_order=[1, 2, 3, 4, 5, 6, 7]
+    ):
         self.errorlog = []
         self.seed = settings.seed
         self.race_mode = settings.race_mode
         self.statues = statues
         self.statues_required = statues_required
         self.statue_req = statue_req
         self.boss_order = boss_order
         self.dungeons_req = []
         for x in self.statues:
-            self.dungeons_req.append(self.boss_order[x-1])
+            self.dungeons_req.append(self.boss_order[x - 1])
 
         gaia_coinflip = random.randint(0, 1)
         if settings.goal.value == Goal.RED_JEWEL_HUNT.value:
             self.goal = "Red Jewel Hunt"
-        elif settings.goal.value == Goal.APO_GAIA.value or (settings.goal.value == Goal.RANDOM_GAIA.value and gaia_coinflip):
+        elif settings.goal.value == Goal.APO_GAIA.value or (
+                settings.goal.value == Goal.RANDOM_GAIA.value and gaia_coinflip):
             self.goal = "Apocalypse Gaia"
         else:
             self.goal = "Dark Gaia"
 
         if settings.logic.value == Logic.COMPLETABLE.value:
             self.logic_mode = "Completable"
         elif settings.logic.value == Logic.BEATABLE.value:
@@ -3175,52 +3234,52 @@
         if settings.town_shuffle or settings.dungeon_shuffle:
             self.entrance_shuffle = True
         else:
             self.entrance_shuffle = False
         self.coupled_exits = settings.coupled_exits
         self.town_shuffle = settings.town_shuffle
         self.dungeon_shuffle = settings.dungeon_shuffle
-        
+
         if settings.flute.value == FluteOpt.START.value:
             self.flute = "Start"
         elif settings.flute.value == FluteOpt.SHUFFLE.value:
             self.flute = "Shuffle"
         else:
             self.flute = "Fluteless"
-        
-        #if settings.orb_rando.value == OrbRando.NONE.value:
+
+        # if settings.orb_rando.value == OrbRando.NONE.value:
         #    self.orb_rando = "None"
-        #elif settings.orb_rando.value == OrbRando.BASIC.value:
+        # elif settings.orb_rando.value == OrbRando.BASIC.value:
         #    self.orb_rando = "Basic"
-        #else:
+        # else:
         #    self.orb_rando = "Orbsanity"
         self.orb_rando = "Orbsanity" if settings.orb_rando else "None"
-        
+
         if abs(settings.darkrooms.value) == DarkRooms.NONE.value:
             self.darkroom_level = "None"
         elif abs(settings.darkrooms.value) == DarkRooms.FEW.value:
             self.darkroom_level = "Few"
         elif abs(settings.darkrooms.value) == DarkRooms.SOME.value:
             self.darkroom_level = "Some"
         elif abs(settings.darkrooms.value) == DarkRooms.MANY.value:
             self.darkroom_level = "Many"
         elif abs(settings.darkrooms.value) == DarkRooms.ALL.value:
             self.darkroom_level = "All"
         if settings.darkrooms.value >= 0:
             self.darkroom_cursed = False
         else:
             self.darkroom_cursed = True
- 
-        #if settings.dungeon_shuffle.value == DungeonShuffle.NONE.value:
+
+        # if settings.dungeon_shuffle.value == DungeonShuffle.NONE.value:
         #    self.dungeon_shuffle = "None"
-        #elif settings.dungeon_shuffle.value == DungeonShuffle.BASIC.value:
+        # elif settings.dungeon_shuffle.value == DungeonShuffle.BASIC.value:
         #    self.dungeon_shuffle = "Basic"
-        #elif settings.dungeon_shuffle.value == DungeonShuffle.CHAOS.value:
+        # elif settings.dungeon_shuffle.value == DungeonShuffle.CHAOS.value:
         #    self.dungeon_shuffle = "Chaos"
-        #elif settings.dungeon_shuffle.value == DungeonShuffle.CLUSTERED.value:
+        # elif settings.dungeon_shuffle.value == DungeonShuffle.CLUSTERED.value:
         #    self.dungeon_shuffle = "Clustered"
 
         if settings.start_location.value == StartLocation.SOUTH_CAPE.value:
             self.start_mode = "South Cape"
         elif settings.start_location.value == StartLocation.SAFE.value:
             self.start_mode = "Safe"
         elif settings.start_location.value == StartLocation.UNSAFE.value:
@@ -3259,99 +3318,101 @@
             self.variant.append("Open Mode")
 
         if settings.z3:
             self.variant.append("Z3 Mode")
 
         self.firebird = settings.firebird
         self.start_loc = 10
-#        self.level = settings.level.value
+        #        self.level = settings.level.value
         self.difficulty = settings.difficulty.value
         self.kara = kara
         self.gem = gem
         self.incatile = incatile
         self.hieroglyphs = hieroglyphs
         self.placement_log = []
         self.exit_log = []
         self.spoilers = []
         self.base_item_counts = {}
         self.required_items = [20, 36]
         self.good_items = [10, 13, 24, 25, 37, 62, 63, 64]
         self.trolly_locations = [32, 45, 64, 65, 102, 108, 121, 128, 136, 147]
         self.free_locations = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 24, 33, 34, 35, 36, 37, 38, 39]
-        self.optional_nodes = [-2, -1, 491, 600, 601, 602, 604, 605, 606, 607]  # Artificial nodes, not required by competable logic
+        self.optional_nodes = [-2, -1, 491, 600, 601, 602, 604, 605, 606,
+                               607]  # Artificial nodes, not required by competable logic
         self.map_patches = []
         self.visited = []
         self.items_collected = []
         self.item_destinations = []
-        self.open_locations = []   # Pool sublists are added to this in initialization
+        self.open_locations = []  # Pool sublists are added to this in initialization
         self.open_edges = []
         self.graph_viz = None
         self.all_darkrooms = []
         self.max_darkrooms = 0
-        self.asar_defines = { "DummyDefine": "DummyDefine" }
-        
+        self.asar_defines = {"DummyDefine": "DummyDefine"}
+
         dungeon_keys_nondroppable = []
-        for x in [3,5]:
+        for x in [3, 5]:
             # Generally can't drop Ramas/Hieros/Journal if Gold Ship or passage to a new room might be behind them
-            if x in self.dungeons_req or self.dungeon_shuffle or (self.boss_order != [1,2,3,4,5,6,7]):
+            if x in self.dungeons_req or self.dungeon_shuffle or (self.boss_order != [1, 2, 3, 4, 5, 6, 7]):
                 dungeon_keys_nondroppable.append(x)
-        
+
         # Items that transfer DS and form access.
         # Items not in any list are assumed to be form-independent.
         self.form_items = {
-            0:  [61,62,63], # Will
-            1:  [64,65,66], # Freedan
-            2:  [36,67]     # Shadow - Aura and Firebird
+            0: [61, 62, 63],  # Will
+            1: [64, 65, 66],  # Freedan
+            2: [36, 67]  # Shadow - Aura and Firebird
         }
 
         # Dark Space info required for random start.
         # ID is shared with the DS's entry in item_locations (or -1 for School).
         # Format: { ID: [0: Safety type,
         #                1: Map ID outside DS,
         #                2: DS index in-game,
         #                3: Allow txform/F abilities (bool)
         #               ] }
         self.spawn_locations = {
-            -1:  ["",       0x08, 0x00, 0],  # School
-            10:  ["Safe",   0x01, 0x00, 0],  # Cape exterior
-            14:  ["",       0x0b, 0x01, 0],  # Prison
-            19:  ["Unsafe", 0x12, 0x02, 1],  # EdDg final
-            22:  ["Safe",   0x15, 0x03, 0],  # Itory
-            29:  ["Unsafe", 0x28, 0x04, 1],  # Inca near melody
-            30:  ["Unsafe", 0x26, 0x05, 1],  # Inca slug DS
-            31:  ["",       0x1e, 0x06, 1],  # Inca Castoth
-            39:  ["Safe",   0x34, 0x07, 0],  # Freejia
-            46:  ["Unsafe", 0x40, 0x08, 1],  # Mine hidden
-            47:  ["Unsafe", 0x3d, 0x09, 1],  # Mine near false wall
-            48:  ["",       0x42, 0x0a, 1],  # Mine behind false wall
-            57:  ["Safe",   0x4c, 0x0b, 0],  # SkGn foyer
-            58:  ["Unsafe", 0x56, 0x0c, 1],  # SkGn blue room
-            59:  ["",       0x51, 0x0d, 1],  # SkGn inside fence
-            60:  ["Unsafe", 0x54, 0x0e, 1],  # SkGn NW dark side
-            66:  ["Safe",   0x5a, 0x0f, 0],  # SeaPal
-            74:  ["",       0x60, 0x10, 1],  # Mu NE
-            75:  ["",       0x62, 0x11, 1],  # Mu W
-            77:  ["Safe",   0x6c, 0x12, 0],  # Angl
-            88:  ["Safe",   0x7c, 0x13, 0],  # Wtrm
-            93:  ["Unsafe", 0x85, 0x14, 1],  # GtWl 1
-            94:  ["Unsafe", 0x86, 0x15, 1],  # GtWl Spin Dash
-            95:  ["",       0x88, 0x16, 1],  # GtWl final
-            103: ["Safe",   0x99, 0x17, 0],  # Euro
+            -1: ["", 0x08, 0x00, 0],  # School
+            10: ["Safe", 0x01, 0x00, 0],  # Cape exterior
+            14: ["", 0x0b, 0x01, 0],  # Prison
+            19: ["Unsafe", 0x12, 0x02, 1],  # EdDg final
+            22: ["Safe", 0x15, 0x03, 0],  # Itory
+            29: ["Unsafe", 0x28, 0x04, 1],  # Inca near melody
+            30: ["Unsafe", 0x26, 0x05, 1],  # Inca slug DS
+            31: ["", 0x1e, 0x06, 1],  # Inca Castoth
+            39: ["Safe", 0x34, 0x07, 0],  # Freejia
+            46: ["Unsafe", 0x40, 0x08, 1],  # Mine hidden
+            47: ["Unsafe", 0x3d, 0x09, 1],  # Mine near false wall
+            48: ["", 0x42, 0x0a, 1],  # Mine behind false wall
+            57: ["Safe", 0x4c, 0x0b, 0],  # SkGn foyer
+            58: ["Unsafe", 0x56, 0x0c, 1],  # SkGn blue room
+            59: ["", 0x51, 0x0d, 1],  # SkGn inside fence
+            60: ["Unsafe", 0x54, 0x0e, 1],  # SkGn NW dark side
+            66: ["Safe", 0x5a, 0x0f, 0],  # SeaPal
+            74: ["", 0x60, 0x10, 1],  # Mu NE
+            75: ["", 0x62, 0x11, 1],  # Mu W
+            77: ["Safe", 0x6c, 0x12, 0],  # Angl
+            88: ["Safe", 0x7c, 0x13, 0],  # Wtrm
+            93: ["Unsafe", 0x85, 0x14, 1],  # GtWl 1
+            94: ["Unsafe", 0x86, 0x15, 1],  # GtWl Spin Dash
+            95: ["", 0x88, 0x16, 1],  # GtWl final
+            103: ["Safe", 0x99, 0x17, 0],  # Euro
             109: ["Unsafe", 0xa1, 0x18, 1],  # Kress 1
             110: ["Unsafe", 0xa3, 0x19, 1],  # Kress 2
-            111: ["",       0xa7, 0x1a, 1],  # Kress 3
-            114: ["Safe",   0xac, 0x1b, 0],  # NtVl
+            111: ["", 0xa7, 0x1a, 1],  # Kress 3
+            114: ["Safe", 0xac, 0x1b, 0],  # NtVl
             122: ["Unsafe", 0xb6, 0x1c, 1],  # Ankr Garden
-            123: ["",       0xb8, 0x1d, 1],  # Ankr inner east
+            123: ["", 0xb8, 0x1d, 1],  # Ankr inner east
             124: ["Unsafe", 0xbb, 0x1e, 1],  # Ankr dropdown
-            129: ["Safe",   0xc3, 0x1f, 0],  # Dao
-            130: ["",       0xcc, 0x20, 1],  # Pymd upper
+            129: ["Safe", 0xc3, 0x1f, 0],  # Dao
+            130: ["", 0xcc, 0x20, 1],  # Pymd upper
             142: ["Unsafe", 0xcc, 0x21, 1],  # Pymd lower
-            145: ["Forced Unsafe" if self.difficulty == 3 and self.flute == "Start" else "", 0xdf, 0x22, 0],  # Babel lower
-            146: ["Safe",   0xe3, 0x23, 0]   # Babel upper
+            145: ["Forced Unsafe" if self.difficulty == 3 and self.flute == "Start" else "", 0xdf, 0x22, 0],
+            # Babel lower
+            146: ["Safe", 0xe3, 0x23, 0]  # Babel upper
         }
 
         # Initialize item pool
         # Format = { ID: [0: Quantity
         #                 1: Type (1=item, 2=ability, 3=statue, 4=game state, 5=monster orb, 6=artificial),
         #                 2: Engine item ID, 
         #                 3: Name, 
@@ -3359,54 +3420,64 @@
         #                 5: ProgressionType (1=unlocks new locations,2=quest item,3=no progression),
         #                 6: ShufflePool (populated during world initialization),
         #                 7: ProgressionPenalty (range [-10,10], higher numbers are placed deeper/later)
         #                ] }
         self.deleted_item_pool = {}
         self.item_pool = {
             # Normal items, high byte implicitly 0
-            0: [2, 1,  0x00, "Nothing", False, 3, 0, 0],
+            0: [2, 1, 0x00, "Nothing", False, 3, 0, 0],
             1: [45 if "Z3 Mode" not in self.variant else 29, 1, 0x01, "Red Jewel", False, 1, 0, 1],
-            2: [1, 1,  0x02, "Prison Key", True and not settings.infinite_inventory, 1, 0, 0],
-            3: [1, 1,  0x03, "Inca Statue A", True and not settings.infinite_inventory, 1, 0, 0],
-            4: [1, 1,  0x04, "Inca Statue B", True and not settings.infinite_inventory, 2, 0, 0],
-            #5: [0, 1,  0x05, "Inca Melody", True and not settings.infinite_inventory, 3, 0, 0],  # Not implemented
+            2: [1, 1, 0x02, "Prison Key", True and not settings.infinite_inventory, 1, 0, 0],
+            3: [1, 1, 0x03, "Inca Statue A", True and not settings.infinite_inventory, 1, 0, 0],
+            4: [1, 1, 0x04, "Inca Statue B", True and not settings.infinite_inventory, 2, 0, 0],
+            # 5: [0, 1,  0x05, "Inca Melody", True and not settings.infinite_inventory, 3, 0, 0],  # Not implemented
             6: [12, 1, 0x06, "Herb", False, 3, 0, 0],
-            7: [1, 1,  0x07, "Diamond Block", True and not settings.infinite_inventory, 1, 0, 6*settings.orb_rando],
-            8: [1, 1,  0x08, "Wind Melody", True and not settings.infinite_inventory, 1, 0, 0],
-            9: [1, 1,  0x09, "Lola's Melody", True and not settings.infinite_inventory, 1, 0, 0],
+            7: [1, 1, 0x07, "Diamond Block", True and not settings.infinite_inventory, 1, 0, 6 * settings.orb_rando],
+            8: [1, 1, 0x08, "Wind Melody", True and not settings.infinite_inventory, 1, 0, 0],
+            9: [1, 1, 0x09, "Lola's Melody", True and not settings.infinite_inventory, 1, 0, 0],
             10: [1, 1, 0x0a, "Large Roast", True and not settings.infinite_inventory, 1, 0, 0],
             11: [1, 1, 0x0b, "Mine Key A", True and not settings.infinite_inventory, 1, 0, 0],
             12: [1, 1, 0x0c, "Mine Key B", True and not settings.infinite_inventory, 2, 0, 0],
             13: [1, 1, 0x0d, "Memory Melody", True and not settings.infinite_inventory, 1, 0, 0],
             14: [4, 1, 0x0e, "Crystal Ball", True and not settings.infinite_inventory, 2, 0, 0],
             15: [1, 1, 0x0f, "Elevator Key", True and not settings.infinite_inventory, 1, 0, -1],
             16: [1, 1, 0x10, "Mu Palace Key", True and not settings.infinite_inventory, 1, 0, 0],
             17: [1, 1, 0x11, "Purity Stone", True and not settings.infinite_inventory, 1, 0, 0],
-            18: [2, 1, 0x12, "Hope Statue", True and not settings.infinite_inventory, 1, 0, -2*(1+self.dungeon_shuffle)],
-            19: [2, 1, 0x13, "Rama Statue", bool(3 in dungeon_keys_nondroppable) and not settings.infinite_inventory, 2, 0, 0],
+            18: [2, 1, 0x12, "Hope Statue", True and not settings.infinite_inventory, 1, 0,
+                 -2 * (1 + self.dungeon_shuffle)],
+            19: [2, 1, 0x13, "Rama Statue", bool(3 in dungeon_keys_nondroppable) and not settings.infinite_inventory, 2,
+                 0, 0],
             20: [1, 1, 0x14, "Magic Dust", True and not settings.infinite_inventory, 2, 0, 0],
             21: [0, 1, 0x15, "Blue Journal", False, 3, 0, 0],
             22: [1, 1, 0x16, "Lance Letter", False, 3, 0, 0],
             23: [1, 1, 0x17, "Necklace", True and not settings.infinite_inventory, 1, 0, 0],
             24: [1, 1, 0x18, "Will", True and not settings.infinite_inventory, 1, 0, 0],
             25: [1, 1, 0x19, "Teapot", True and not settings.infinite_inventory, 1, 0, 0],
             26: [3, 1, 0x1a, "Mushroom Drops", True and not settings.infinite_inventory, 1, 0, -1],
-            #27: [0, 1, 0x1b, "Bag of Gold", False, 3, 0, 0],  # Not implemented
-            28: [1, 1, 0x1c, "Black Glasses", False, 1, 0, 3*self.difficulty if settings.darkrooms.value != 0 else 0],
+            # 27: [0, 1, 0x1b, "Bag of Gold", False, 3, 0, 0],  # Not implemented
+            28: [1, 1, 0x1c, "Black Glasses", False, 1, 0, 3 * self.difficulty if settings.darkrooms.value != 0 else 0],
             29: [1, 1, 0x1d, "Gorgon Flower", True and not settings.infinite_inventory, 1, 0, 0],
-            30: [1, 1, 0x1e, "Hieroglyph", bool(5 in dungeon_keys_nondroppable) and not settings.infinite_inventory, 2, 0, 0],
-            31: [1, 1, 0x1f, "Hieroglyph", bool(5 in dungeon_keys_nondroppable) and not settings.infinite_inventory, 2, 0, 0],
-            32: [1, 1, 0x20, "Hieroglyph", bool(5 in dungeon_keys_nondroppable) and not settings.infinite_inventory, 2, 0, 0],
-            33: [1, 1, 0x21, "Hieroglyph", bool(5 in dungeon_keys_nondroppable) and not settings.infinite_inventory, 2, 0, 0],
-            34: [1, 1, 0x22, "Hieroglyph", bool(5 in dungeon_keys_nondroppable) and not settings.infinite_inventory, 2, 0, 0],
-            35: [1, 1, 0x23, "Hieroglyph", bool(5 in dungeon_keys_nondroppable) and not settings.infinite_inventory, 2, 0, 0],
-            36: [1, 1, 0x24, "Aura", True and not settings.infinite_inventory, 1, 0, 2*self.difficulty*self.dungeon_shuffle],
+            30: [1, 1, 0x1e, "Hieroglyph", bool(5 in dungeon_keys_nondroppable) and not settings.infinite_inventory, 2,
+                 0, 0],
+            31: [1, 1, 0x1f, "Hieroglyph", bool(5 in dungeon_keys_nondroppable) and not settings.infinite_inventory, 2,
+                 0, 0],
+            32: [1, 1, 0x20, "Hieroglyph", bool(5 in dungeon_keys_nondroppable) and not settings.infinite_inventory, 2,
+                 0, 0],
+            33: [1, 1, 0x21, "Hieroglyph", bool(5 in dungeon_keys_nondroppable) and not settings.infinite_inventory, 2,
+                 0, 0],
+            34: [1, 1, 0x22, "Hieroglyph", bool(5 in dungeon_keys_nondroppable) and not settings.infinite_inventory, 2,
+                 0, 0],
+            35: [1, 1, 0x23, "Hieroglyph", bool(5 in dungeon_keys_nondroppable) and not settings.infinite_inventory, 2,
+                 0, 0],
+            36: [1, 1, 0x24, "Aura", True and not settings.infinite_inventory, 1, 0,
+                 2 * self.difficulty * self.dungeon_shuffle],
             37: [1, 1, 0x25, "Lola's Letter", False, 1, 0, 0],
-            38: [1, 1, 0x26, "Journal", bool(5 in dungeon_keys_nondroppable) and not settings.infinite_inventory, 2, 0, 0],
-            39: [1, 1, 0x27, "Crystal Ring", False, 1, 0, 3*self.difficulty if settings.darkrooms.value != 0 else 0],
+            38: [1, 1, 0x26, "Journal", bool(5 in dungeon_keys_nondroppable) and not settings.infinite_inventory, 2, 0,
+                 0],
+            39: [1, 1, 0x27, "Crystal Ring", False, 1, 0, 3 * self.difficulty if settings.darkrooms.value != 0 else 0],
             40: [1, 1, 0x28, "Apple", True and not settings.infinite_inventory, 1, 0, 0],
             41: [1, 1, 0x2e, "2 Red Jewels", False, 1, 0, -2],
             42: [1, 1, 0x2f, "3 Red Jewels", False, 1, 0, -2],
 
             # Status Upgrades
             # Mapped to artificial items whose IDs are $5E lower (e.g. $87 -> $29),
             # so $8c/$8d are skipped since they'd map to $2e/$2f which are in use.
@@ -3468,33 +3539,34 @@
             528: [1, 4, "", "Mine: Blocked Tunnel Open", False, 1, 0, 0],
             529: [1, 4, "", "Underground Tunnel: Bridge Open", False, 1, 0, 0],
             530: [1, 4, "", "Inca: Slug Statue Broken", False, 1, 0, 0],
             531: [1, 4, "", "Mu: Beat Vampires", False, 1, 0, 0],
 
             # Misc. game states
             602: [1, 6, "", "Early Firebird enabled", False, 1, 0, 0],
-            #603: [0, 6, "", "Firebird", False, 1, 0, 0],   # Firebird item is 67 instead of this
-            604: [1, 1, 0x8f, "Flute", False, 1, 0, 2*(1+self.difficulty)],
-            608: [0, 6, "", "Has Any Will Ability", False, 1, 0, 0],   # Expanded to PDash|Slider|SDash during init
-            609: [0, 6, "", "Has Any Attack", False, 1, 0, 0],   # Expanded to many options during init, if not starting with flute
+            # 603: [0, 6, "", "Firebird", False, 1, 0, 0],   # Firebird item is 67 instead of this
+            604: [1, 1, 0x8f, "Flute", False, 1, 0, 2 * (1 + self.difficulty)],
+            608: [0, 6, "", "Has Any Will Ability", False, 1, 0, 0],  # Expanded to PDash|Slider|SDash during init
+            609: [0, 6, "", "Has Any Attack", False, 1, 0, 0],
+            # Expanded to many options during init, if not starting with flute
             610: [0, 6, "", "Has Any Ranged Attack", False, 1, 0, 0],  # Expanded to Friar|Firebird during init
-            611: [0, 6, "", "Can Play Songs", False, 1, 0, 0],   # Expanded during init to Flute|Fluteless
-            612: [0, 6, "", "Telekinesis", False, 1, 0, 0],   # Expanded during init to Flute|Fluteless|Freedan|Shadow
-            
+            611: [0, 6, "", "Can Play Songs", False, 1, 0, 0],  # Expanded during init to Flute|Fluteless
+            612: [0, 6, "", "Telekinesis", False, 1, 0, 0],  # Expanded during init to Flute|Fluteless|Freedan|Shadow
+
             # Orbs that open doors -- ASM ID is the map rearrangement flag + artificial 0x1000
             700: [1, 5, 0x1001, "Open Underground Tunnel Skeleton Cage", False, 3, 0, 0],
             701: [1, 5, 0x1002, "Open Underground Tunnel First Worm Door", False, 1, 0, -5],
             702: [1, 5, 0x1003, "Open Underground Tunnel Second Worm Door", False, 1, 0, -5],
             703: [1, 5, 0x1005, "Open Underground Tunnel West Room Bat Door", False, 1, 0, -5],
             704: [1, 5, 0x1016, "Open Underground Tunnel Hidden Dark Space", False, 1, 0, -5],
             705: [1, 5, 0x1017, "Open Underground Tunnel Red Skeleton Barrier 1", False, 1, 0, -5],
             706: [1, 5, 0x1018, "Open Underground Tunnel Red Skeleton Barrier 2", False, 1, 0, -5],
             707: [1, 5, 0x100d, "Open Incan Ruins West Ladder", False, 1, 0, 0],
             708: [1, 5, 0x100e, "Open Incan Ruins Final Ladder", False, 1, 0, 0],
-            709: [1, 5, 0x100f, "Open Incan Ruins Entrance Ladder", False, 1, 0, 6*settings.orb_rando],
+            709: [1, 5, 0x100f, "Open Incan Ruins Entrance Ladder", False, 1, 0, 6 * settings.orb_rando],
             710: [1, 5, 0x100c, "Open Incan Ruins Water Room Ramp", False, 1, 0, 0],
             711: [1, 5, 0x100b, "Open Incan Ruins East-West Freedan Ramp", False, 1, 0, 0],
             712: [1, 5, 0x100a, "Open Incan Ruins Diamond Block Stairs", False, 3, 0, 0],
             713: [1, 5, 0x1010, "Open Incan Ruins Singing Statue Stairs", False, 1, 0, 0],
             714: [1, 5, 0x1034, "Open Diamond Mine Tunnel Middle Fence", False, 1, 0, -3],
             715: [1, 5, 0x1035, "Open Diamond Mine Tunnel South Fence", False, 1, 0, -3],
             716: [1, 5, 0x1036, "Open Diamond Mine Tunnel North Fence", False, 1, 0, -3],
@@ -3510,27 +3582,27 @@
             726: [1, 5, 0x103d, "Open Mu Entrance Room Barrier", False, 1, 0, 0],
             727: [1, 5, 0x103e, "Open Mu Northeast Room Rock 1", False, 1, 0, 0],
             728: [1, 5, 0x103f, "Open Mu Northeast Room Rock 2", False, 1, 0, 0],
             729: [1, 5, 0x1042, "Open Mu West Room Slime Cages", False, 3, 0, 0],
             730: [1, 5, 0x1041, "Open Mu East-Facing Stone Head", False, 3, 0, 0],
             731: [1, 5, 0x1040, "Open Mu South-Facing Stone Head", False, 3, 0, 0],
             732: [1, 5, 0x1053, "Open Great Wall Archer Friar Barrier", False, 1, 0, 0],
-            #733: [1, 5, 0x106a, "Open Great Wall Fanger Arena Exit", False, 1, 0, 0], # Probably shouldn't randomize this...
+            # 733: [1, 5, 0x106a, "Open Great Wall Fanger Arena Exit", False, 1, 0, 0], # Probably shouldn't randomize this...
             734: [1, 5, 0x1068, "Open Mt. Temple West Chest Shortcut", False, 3, 0, 0],
             735: [1, 5, 0x106c, "Open Ankor Wat Entrance Stairs", False, 1, 0, 0],
             736: [1, 5, 0x106b, "Open Ankor Wat Outer East Slider Hole", False, 1, 0, 0],
-            #737: [1, 5, 0x106d, "Open Ankor Wat Pit Exit", False, 1, 0, 0], # Probably shouldn't randomize this...
+            # 737: [1, 5, 0x106d, "Open Ankor Wat Pit Exit", False, 1, 0, 0], # Probably shouldn't randomize this...
             738: [1, 5, 0x106f, "Open Ankor Wat Dark Space Corridor", False, 1, 0, 0],
             739: [1, 5, 0x1073, "Open Pyramid Foyer Upper Dark Space", False, 1, 0, 0],
             740: [1, 5, 0x109a, "Open Jeweler's Mansion First Barrier", False, 1, 0, 0],
             741: [1, 5, 0x109b, "Open Jeweler's Mansion Second Barrier", False, 1, 0, 0],
-            
+
             800: [1, 6, "", "Dungeon Shuffle artificial logic", False, 3, 0, 0],
             801: [0, 6, "", "Dungeon Shuffle artificial antilogic", False, 3, 0, 0],
-    
+
             900: [0, 1, 0x32, "Other World Item", False, 1, 0, 0]
         }
 
         # Define Item/Ability/Statue locations
         # Format: { ID: [0: Parent Node, 
         #                1: Type (1=item, 2=ability, 3=statue, 4=game state, 5=monster orb, 6=artificial),
         #                2: Filled Flag, 
@@ -3541,330 +3613,356 @@
         #                7: ShufflePool (populated during world initialization),
         #                8: DiscoveredCycle (populated during item placement),
         #                9: CollectionLogic (a form=0 reqset as in self.logic; for more complex logic, use a real node)
         #               ] }
         self.deleted_item_locations = {}
         self.item_locations = {
             # Jeweler
-            0:   [2, 1, False, 0, [], "Jeweler1Item", "Jeweler Reward 1", 0, 0, [] ],
-            1:   [3, 1, False, 0, [], "Jeweler2Item", "Jeweler Reward 2", 0, 0, [] ],
-            2:   [4, 1, False, 0, [], "Jeweler3Item", "Jeweler Reward 3", 0, 0, [] ],
-            3:   [5, 1, False, 0, [], "Jeweler4Item", "Jeweler Reward 4", 0, 0, [] ],
-            4:   [6, 1, False, 0, [], "Jeweler5Item", "Jeweler Reward 5", 0, 0, [] ],
-            5:   [7, 1, False, 0, [], "Jeweler6Item", "Jeweler Reward 6", 0, 0, [] ],
+            0: [2, 1, False, 0, [], "Jeweler1Item", "Jeweler Reward 1", 0, 0, []],
+            1: [3, 1, False, 0, [], "Jeweler2Item", "Jeweler Reward 2", 0, 0, []],
+            2: [4, 1, False, 0, [], "Jeweler3Item", "Jeweler Reward 3", 0, 0, []],
+            3: [5, 1, False, 0, [], "Jeweler4Item", "Jeweler Reward 4", 0, 0, []],
+            4: [6, 1, False, 0, [], "Jeweler5Item", "Jeweler Reward 5", 0, 0, []],
+            5: [7, 1, False, 0, [], "Jeweler6Item", "Jeweler Reward 6", 0, 0, []],
 
             # South Cape
-            6:   [21, 1, False, 0, [], "CapeTowerItem",       "South Cape: Bell Tower", 0, 0, [] ],
-            7:   [20, 1, False, 0, [], "CapeFisherItem",      "South Cape: Fisherman", 0, 0, [] ],
-            8:   [26, 1, False, 0, [], "CapeLancesHouseItem", "South Cape: Lance's House", 0, 0, [] ],
-            9:   [23, 1, False, 0, [], "CapeLolaItem",        "South Cape: Lola", 0, 0, [] ],
+            6: [21, 1, False, 0, [], "CapeTowerItem", "South Cape: Bell Tower", 0, 0, []],
+            7: [20, 1, False, 0, [], "CapeFisherItem", "South Cape: Fisherman", 0, 0, []],
+            8: [26, 1, False, 0, [], "CapeLancesHouseItem", "South Cape: Lance's House", 0, 0, []],
+            9: [23, 1, False, 0, [], "CapeLolaItem", "South Cape: Lola", 0, 0, []],
 
-            10:  [21, 2, False, 0, [], "", "South Cape: Dark Space", 0, 0, [] ],
+            10: [21, 2, False, 0, [], "", "South Cape: Dark Space", 0, 0, []],
 
             # Edward's
-            11:  [30, 1, False, 0, [], "ECHiddenGuardItem", "Edward's Castle: Hidden Guard", 0, 0, [] ],
-            12:  [30, 1, False, 0, [], "ECBasementItem",    "Edward's Castle: Basement", 0, 0, [] ],
-            13:  [32, 1, False, 0, [], "EDHamletItem",      "Edward's Prison: Hamlet", 0, 0, [] ],
+            11: [30, 1, False, 0, [], "ECHiddenGuardItem", "Edward's Castle: Hidden Guard", 0, 0, []],
+            12: [30, 1, False, 0, [], "ECBasementItem", "Edward's Castle: Basement", 0, 0, []],
+            13: [32, 1, False, 0, [], "EDHamletItem", "Edward's Prison: Hamlet", 0, 0, []],
 
-            14:  [32, 2, False, 0, [], "", "Edward's Prison: Dark Space", 0, 0, [] ],
+            14: [32, 2, False, 0, [], "", "Edward's Prison: Dark Space", 0, 0, []],
 
             # Underground Tunnel
-            15:  [39, 1, False, 0, [], "EDSpikeChestItem",     "Underground Tunnel: Spike's Chest", 0, 0, [] ],
-            16:  [44, 1, False, 0, [], "EDSmallRoomChestItem", "Underground Tunnel: Small Room Chest", 0, 0, [] ],
-            17:  [705,1, False, 0, [], "EDEndChestItem",       "Underground Tunnel: Ribber's Chest  ", 0, 0, [] ],
-            18:  [49, 1, False, 0, [], "EDEndBarrelsItem",     "Underground Tunnel: Barrels", 0, 0, [] ],
-
-            19:  [720,2, False, 0, [], "", "Underground Tunnel: Dark Space", 0, 0, [] ],
-            
-            700: [41, 5, False, 0, [],  "EDCageWormItem",      "Underground Tunnel: Worm for East Skeleton Cage", 0, 0, [[609, 1]] ],
-            701: [41, 5, False, 0, [],  "EDSoutheastWormItem", "Underground Tunnel: Worm for East Door", 0, 0, [[609, 1]] ],
-            702: [42, 5, False, 0, [],  "EDSouthwestWormItem", "Underground Tunnel: Worm for South Door", 0, 0, [[609, 1]] ],
-            703: [43, 5, False, 0, [],  "EDDoorBatItem",       "Underground Tunnel: Bat for West Door", 0, 0, [[609, 1]] ],
-            704: [47, 5, False, 0, [],  "EDDarkSpaceWormItem", "Underground Tunnel: Worm for Appearing Dark Space", 0, 0, [[609, 1]] ],
-            705: [704, 5, False, 0, [], "EDSkeleton1Item",     "Underground Tunnel: Red Skeleton 1", 0, 0, [[609, 1]] ],
-            706: [705, 5, False, 0, [], "EDSkeleton2Item",     "Underground Tunnel: Red Skeleton 2", 0, 0, [[609, 1]] ],
+            15: [39, 1, False, 0, [], "EDSpikeChestItem", "Underground Tunnel: Spike's Chest", 0, 0, []],
+            16: [44, 1, False, 0, [], "EDSmallRoomChestItem", "Underground Tunnel: Small Room Chest", 0, 0, []],
+            17: [705, 1, False, 0, [], "EDEndChestItem", "Underground Tunnel: Ribber's Chest  ", 0, 0, []],
+            18: [49, 1, False, 0, [], "EDEndBarrelsItem", "Underground Tunnel: Barrels", 0, 0, []],
+
+            19: [720, 2, False, 0, [], "", "Underground Tunnel: Dark Space", 0, 0, []],
+
+            700: [41, 5, False, 0, [], "EDCageWormItem", "Underground Tunnel: Worm for East Skeleton Cage", 0, 0,
+                  [[609, 1]]],
+            701: [41, 5, False, 0, [], "EDSoutheastWormItem", "Underground Tunnel: Worm for East Door", 0, 0,
+                  [[609, 1]]],
+            702: [42, 5, False, 0, [], "EDSouthwestWormItem", "Underground Tunnel: Worm for South Door", 0, 0,
+                  [[609, 1]]],
+            703: [43, 5, False, 0, [], "EDDoorBatItem", "Underground Tunnel: Bat for West Door", 0, 0, [[609, 1]]],
+            704: [47, 5, False, 0, [], "EDDarkSpaceWormItem", "Underground Tunnel: Worm for Appearing Dark Space", 0, 0,
+                  [[609, 1]]],
+            705: [704, 5, False, 0, [], "EDSkeleton1Item", "Underground Tunnel: Red Skeleton 1", 0, 0, [[609, 1]]],
+            706: [705, 5, False, 0, [], "EDSkeleton2Item", "Underground Tunnel: Red Skeleton 2", 0, 0, [[609, 1]]],
 
             # Itory
-            20:  [51, 1, False, 0, [], "ItoryLogsItem", "Itory Village: Logs", 0, 0, [] ],
-            21:  [58, 1, False, 0, [], "ItoryCaveItem", "Itory Village: Cave", 0, 0, [] ],
+            20: [51, 1, False, 0, [], "ItoryLogsItem", "Itory Village: Logs", 0, 0, []],
+            21: [58, 1, False, 0, [], "ItoryCaveItem", "Itory Village: Cave", 0, 0, []],
 
-            22:  [51, 2, False, 0, [], "", "Itory Village: Dark Space", 0, 0, [] ],
+            22: [51, 2, False, 0, [], "", "Itory Village: Dark Space", 0, 0, []],
 
             # Moon Tribe
-            23:  [62, 1, False, 0, [], "MoonTribeCaveItem", "Moon Tribe: Cave", 0, 0, [] ],
+            23: [62, 1, False, 0, [], "MoonTribeCaveItem", "Moon Tribe: Cave", 0, 0, []],
 
             # Inca
-            24:  [71, 1, False, 0, [], "IncaDiamondBlockChestItem", "Inca Ruins: Diamond-Block Chest", 0, 0, [] ],
-            25:  [92, 1, False, 0, [], "IncaMazeChestItem",         "Inca Ruins: Broken Statues Chest", 0, 0, [] ],
-            26:  [83, 1, False, 0, [], "IncaStatueChestItem",       "Inca Ruins: Stone Lord Chest", 0, 0, [] ],
-            27:  [93, 1, False, 0, [], "IncaWormChestItem",         "Inca Ruins: Slugger Chest", 0, 0, [] ],
-            28:  [76, 1, False, 0, [], "IncaCliffItem",             "Inca Ruins: Singing Statue", 0, 0, [] ],
-
-            29:  [96, 2, False, 0, [], "", "Inca Ruins: Dark Space 1", 0, 0, [] ],
-            30:  [93, 2, False, 0, [], "", "Inca Ruins: Dark Space 2", 0, 0, [] ],
-            31:  [77, 2, False, 0, [], "", "Inca Ruins: Final Dark Space", 0, 0, [] ],
-
-            707: [700, 5, False, 0, [], "IncaWestLadderItem",      "Inca Ruins: 4-Way for West Ladder", 0, 0, [[609, 1]] ],
-            708: [75, 5, False, 0, [],  "IncaSoutheastLadderItem", "Inca Ruins: 4-Way for SE Ladder", 0, 0, [[609, 1]] ],
-            709: [72, 5, False, 0, [],  "IncaNortheastLadderItem", "Inca Ruins: 4-Way for NE Ladder", 0, 0, [[609, 1]] ],
-            710: [82, 5, False, 0, [],  "IncaNSRampItem",          "Inca Ruins: Whirligig for N/S Ramp", 0, 0, [[609, 1]] ],
-            711: [707, 5, False, 0, [], "IncaEWRampItem",          "Inca Ruins: Whirligig for E/W Ramp", 0, 0, [[609, 1]] ],
-            712: [94, 5, False, 0, [],  "IncaDBlockMonsterItem",   "Inca Ruins: 4-Way West of Diamond Block Room", 0, 0, [[609, 1]] ],
-            713: [96, 5, False, 0, [],  "IncaWMelodyMonsterItem",  "Inca Ruins: 4-Way Before Singing Statue", 0, 0, [[609, 1]] ],
-            
+            24: [71, 1, False, 0, [], "IncaDiamondBlockChestItem", "Inca Ruins: Diamond-Block Chest", 0, 0, []],
+            25: [92, 1, False, 0, [], "IncaMazeChestItem", "Inca Ruins: Broken Statues Chest", 0, 0, []],
+            26: [83, 1, False, 0, [], "IncaStatueChestItem", "Inca Ruins: Stone Lord Chest", 0, 0, []],
+            27: [93, 1, False, 0, [], "IncaWormChestItem", "Inca Ruins: Slugger Chest", 0, 0, []],
+            28: [76, 1, False, 0, [], "IncaCliffItem", "Inca Ruins: Singing Statue", 0, 0, []],
+
+            29: [96, 2, False, 0, [], "", "Inca Ruins: Dark Space 1", 0, 0, []],
+            30: [93, 2, False, 0, [], "", "Inca Ruins: Dark Space 2", 0, 0, []],
+            31: [77, 2, False, 0, [], "", "Inca Ruins: Final Dark Space", 0, 0, []],
+
+            707: [700, 5, False, 0, [], "IncaWestLadderItem", "Inca Ruins: 4-Way for West Ladder", 0, 0, [[609, 1]]],
+            708: [75, 5, False, 0, [], "IncaSoutheastLadderItem", "Inca Ruins: 4-Way for SE Ladder", 0, 0, [[609, 1]]],
+            709: [72, 5, False, 0, [], "IncaNortheastLadderItem", "Inca Ruins: 4-Way for NE Ladder", 0, 0, [[609, 1]]],
+            710: [82, 5, False, 0, [], "IncaNSRampItem", "Inca Ruins: Whirligig for N/S Ramp", 0, 0, [[609, 1]]],
+            711: [707, 5, False, 0, [], "IncaEWRampItem", "Inca Ruins: Whirligig for E/W Ramp", 0, 0, [[609, 1]]],
+            712: [94, 5, False, 0, [], "IncaDBlockMonsterItem", "Inca Ruins: 4-Way West of Diamond Block Room", 0, 0,
+                  [[609, 1]]],
+            713: [96, 5, False, 0, [], "IncaWMelodyMonsterItem", "Inca Ruins: 4-Way Before Singing Statue", 0, 0,
+                  [[609, 1]]],
+
             # Gold Ship
-            32:  [100, 1, False, 0, [], "IncaGoldShipItem", "Gold Ship: Seth", 0, 0, [] ],
+            32: [100, 1, False, 0, [], "IncaGoldShipItem", "Gold Ship: Seth", 0, 0, []],
 
             # Diamond Coast
-            33:  [102, 1, False, 0, [], "DiamondCoastJarItem", "Diamond Coast: Jar", 0, 0, [] ],
+            33: [102, 1, False, 0, [], "DiamondCoastJarItem", "Diamond Coast: Jar", 0, 0, []],
 
             # Freejia
-            34:  [121, 1, False, 0, [], "FrejHotelItem",      "Freejia: Hotel", 0, 0, [] ],
-            35:  [110, 1, False, 0, [], "FrejEastSlaverItem", "Freejia: Creepy Guy", 0, 0, [] ],
-            36:  [110, 1, False, 0, [], "FrejBin1Item",       "Freejia: Trash Can 1", 0, 0, [] ],
-            37:  [110, 1, False, 0, [], "FrejBin2Item",       "Freejia: Trash Can 2", 0, 0, [] ],
-            38:  [110, 1, False, 0, [], "FrejSnitchItem",     "Freejia: Snitch", 0, 0, [[504, 1]] ],
+            34: [121, 1, False, 0, [], "FrejHotelItem", "Freejia: Hotel", 0, 0, []],
+            35: [110, 1, False, 0, [], "FrejEastSlaverItem", "Freejia: Creepy Guy", 0, 0, []],
+            36: [110, 1, False, 0, [], "FrejBin1Item", "Freejia: Trash Can 1", 0, 0, []],
+            37: [110, 1, False, 0, [], "FrejBin2Item", "Freejia: Trash Can 2", 0, 0, []],
+            38: [110, 1, False, 0, [], "FrejSnitchItem", "Freejia: Snitch", 0, 0, [[504, 1]]],
 
-            39:  [125, 2, False, 0, [], "", "Freejia: Dark Space", 0, 0, [] ],
+            39: [125, 2, False, 0, [], "", "Freejia: Dark Space", 0, 0, []],
 
             # Diamond Mine
-            40:  [134, 1, False, 0, [], "MineChestItem",       "Diamond Mine: Chest", 0, 0, [] ],
-            41:  [136, 1, False, 0, [], "MineWallSlaveItem",   "Diamond Mine: Trapped Laborer", 0, 0, [[608, 1]] ],
-            42:  [143, 1, False, 0, [], "MineRampSlaveItem",   "Diamond Mine: Laborer w/Elevator Key", 0, 0, [[609, 1]] ],
-            43:  [148, 1, False, 0, [], "MineMorgueItem",      "Diamond Mine: Morgue", 0, 0, [] ],
-            44:  [149, 1, False, 0, [], "MineCombatSlaveItem", "Diamond Mine: Laborer w/Mine Key", 0, 0, [[609, 1]] ],
-            45:  [150, 1, False, 0, [], "MineSamItem",         "Diamond Mine: Sam", 0, 0, [] ],
-
-            46:  [721, 2, False, 0, [], "", "Diamond Mine: Appearing Dark Space", 0, 0, [] ],
-            47:  [131, 2, False, 0, [], "", "Diamond Mine: Dark Space at Wall", 0, 0, [] ],
-            48:  [142, 2, False, 0, [], "", "Diamond Mine: Dark Space behind Wall", 0, 0, [] ],
-
-            714: [701, 5, False, 0, [], "MineMidFenceItem",      "Diamond Mine: Lizard for Tunnel Middle Fence", 0, 0, [[609, 1]] ],
-            715: [130, 5, False, 0, [], "MineSouthFenceItem",    "Diamond Mine: Eye for Tunnel South Fence", 0, 0, [[609, 1]] ],
-            716: [709, 5, False, 0, [], "MineNorthFenceItem",    "Diamond Mine: Eye for Tunnel North Fence", 0, 0, [[609, 1]] ],
-            717: [134, 5, False, 0, [], "MineWormCageItem",      "Diamond Mine: Worm for Big Room Cage", 0, 0, [[609, 1]] ],
-            718: [136, 5, False, 0, [], "MineWormDarkSpaceItem", "Diamond Mine: Worm for Appearing Dark Space", 0, 0, [[609, 1]] ],
-            719: [710, 5, False, 0, [], "MineFriarFenceItem",    "Diamond Mine: Worm for Friar Ramp Fence", 0, 0, [[609, 1]] ],
+            40: [134, 1, False, 0, [], "MineChestItem", "Diamond Mine: Chest", 0, 0, []],
+            41: [136, 1, False, 0, [], "MineWallSlaveItem", "Diamond Mine: Trapped Laborer", 0, 0, [[608, 1]]],
+            42: [143, 1, False, 0, [], "MineRampSlaveItem", "Diamond Mine: Laborer w/Elevator Key", 0, 0, [[609, 1]]],
+            43: [148, 1, False, 0, [], "MineMorgueItem", "Diamond Mine: Morgue", 0, 0, []],
+            44: [149, 1, False, 0, [], "MineCombatSlaveItem", "Diamond Mine: Laborer w/Mine Key", 0, 0, [[609, 1]]],
+            45: [150, 1, False, 0, [], "MineSamItem", "Diamond Mine: Sam", 0, 0, []],
+
+            46: [721, 2, False, 0, [], "", "Diamond Mine: Appearing Dark Space", 0, 0, []],
+            47: [131, 2, False, 0, [], "", "Diamond Mine: Dark Space at Wall", 0, 0, []],
+            48: [142, 2, False, 0, [], "", "Diamond Mine: Dark Space behind Wall", 0, 0, []],
+
+            714: [701, 5, False, 0, [], "MineMidFenceItem", "Diamond Mine: Lizard for Tunnel Middle Fence", 0, 0,
+                  [[609, 1]]],
+            715: [130, 5, False, 0, [], "MineSouthFenceItem", "Diamond Mine: Eye for Tunnel South Fence", 0, 0,
+                  [[609, 1]]],
+            716: [709, 5, False, 0, [], "MineNorthFenceItem", "Diamond Mine: Eye for Tunnel North Fence", 0, 0,
+                  [[609, 1]]],
+            717: [134, 5, False, 0, [], "MineWormCageItem", "Diamond Mine: Worm for Big Room Cage", 0, 0, [[609, 1]]],
+            718: [136, 5, False, 0, [], "MineWormDarkSpaceItem", "Diamond Mine: Worm for Appearing Dark Space", 0, 0,
+                  [[609, 1]]],
+            719: [710, 5, False, 0, [], "MineFriarFenceItem", "Diamond Mine: Worm for Friar Ramp Fence", 0, 0,
+                  [[609, 1]]],
 
             # Sky Garden
-            49:  [172, 1, False, 0, [], "SGNENorthChestItem",  "Sky Garden: (NE) Platform Chest", 0, 0, [] ],
-            50:  [173, 1, False, 0, [], "SGNEWestChestItem",   "Sky Garden: (NE) Blue Cyber Chest", 0, 0, [] ],
-            51:  [174, 1, False, 0, [], "SGNEStatueChestItem", "Sky Garden: (NE) Statue Chest", 0, 0, [] ],
-            52:  [716, 1, False, 0, [], "SGSEChestItem",       "Sky Garden: (SE) Dark Side Chest", 0, 0, [] ],
-            53:  [185, 1, False, 0, [], "SGSWTopChestItem",    "Sky Garden: (SW) Ramp Chest", 0, 0, [] ],
-            54:  [186, 1, False, 0, [], "SGSWBotChestItem",    "Sky Garden: (SW) Dark Side Chest", 0, 0, [] ],
-            55:  [194, 1, False, 0, [], "SGNWTopChestItem",    "Sky Garden: (NW) North Chest", 0, 0, [] ],
-            56:  [194, 1, False, 0, [], "SGNWBotChestItem",    "Sky Garden: (NW) South Chest", 0, 0, [[609, 1]] ],
-
-            57:  [170, 2, False, 0, [], "", "Sky Garden: Dark Space (Foyer)", 0, 0, [] ],
-            58:  [169, 2, False, 0, [], "", "Sky Garden: Dark Space (SE)", 0, 0, [] ],
-            59:  [183, 2, False, 0, [], "", "Sky Garden: Dark Space (SW)", 0, 0, [] ],
-            60:  [195, 2, False, 0, [], "", "Sky Garden: Dark Space (NW)", 0, 0, [] ],
-
-            720: [711, 5, False, 0, [], "SGSETopBarrierItem",   "Sky Garden: (SE) Top Robot for Center Barrier", 0, 0, [[609, 1]] ],
-            721: [180, 5, False, 0, [], "SGSEBotBarrierItem",   "Sky Garden: (SE) Bottom Robot for Chest", 0, 0, [[609, 1]] ],
-            722: [181, 5, False, 0, [], "SGSWTopPegGateItem",   "Sky Garden: (SW) Top Robot for Peg Gate", 0, 0, [[609, 1]] ],
-            723: [168, 5, False, 0, [], "SGSWTopRobotRampItem", "Sky Garden: (SW) Top Robot for Robot Ramp", 0, 0, [[609, 1]] ],
-            724: [182, 5, False, 0, [], "SGSWTopWormGateItem",  "Sky Garden: (SW) Top Worm for West Gate", 0, 0, [[609, 1]] ],
-            725: [187, 5, False, 0, [], "SGSWBotFireCageItem",  "Sky Garden: (SW) Bot Robot for Fire Cages", 0, 0, [[609, 1]] ],
+            49: [172, 1, False, 0, [], "SGNENorthChestItem", "Sky Garden: (NE) Platform Chest", 0, 0, []],
+            50: [173, 1, False, 0, [], "SGNEWestChestItem", "Sky Garden: (NE) Blue Cyber Chest", 0, 0, []],
+            51: [174, 1, False, 0, [], "SGNEStatueChestItem", "Sky Garden: (NE) Statue Chest", 0, 0, []],
+            52: [716, 1, False, 0, [], "SGSEChestItem", "Sky Garden: (SE) Dark Side Chest", 0, 0, []],
+            53: [185, 1, False, 0, [], "SGSWTopChestItem", "Sky Garden: (SW) Ramp Chest", 0, 0, []],
+            54: [186, 1, False, 0, [], "SGSWBotChestItem", "Sky Garden: (SW) Dark Side Chest", 0, 0, []],
+            55: [194, 1, False, 0, [], "SGNWTopChestItem", "Sky Garden: (NW) North Chest", 0, 0, []],
+            56: [194, 1, False, 0, [], "SGNWBotChestItem", "Sky Garden: (NW) South Chest", 0, 0, [[609, 1]]],
+
+            57: [170, 2, False, 0, [], "", "Sky Garden: Dark Space (Foyer)", 0, 0, []],
+            58: [169, 2, False, 0, [], "", "Sky Garden: Dark Space (SE)", 0, 0, []],
+            59: [183, 2, False, 0, [], "", "Sky Garden: Dark Space (SW)", 0, 0, []],
+            60: [195, 2, False, 0, [], "", "Sky Garden: Dark Space (NW)", 0, 0, []],
+
+            720: [711, 5, False, 0, [], "SGSETopBarrierItem", "Sky Garden: (SE) Top Robot for Center Barrier", 0, 0,
+                  [[609, 1]]],
+            721: [180, 5, False, 0, [], "SGSEBotBarrierItem", "Sky Garden: (SE) Bottom Robot for Chest", 0, 0,
+                  [[609, 1]]],
+            722: [181, 5, False, 0, [], "SGSWTopPegGateItem", "Sky Garden: (SW) Top Robot for Peg Gate", 0, 0,
+                  [[609, 1]]],
+            723: [168, 5, False, 0, [], "SGSWTopRobotRampItem", "Sky Garden: (SW) Top Robot for Robot Ramp", 0, 0,
+                  [[609, 1]]],
+            724: [182, 5, False, 0, [], "SGSWTopWormGateItem", "Sky Garden: (SW) Top Worm for West Gate", 0, 0,
+                  [[609, 1]]],
+            725: [187, 5, False, 0, [], "SGSWBotFireCageItem", "Sky Garden: (SW) Bot Robot for Fire Cages", 0, 0,
+                  [[609, 1]]],
 
             # Seaside Palace
-            61:  [202, 1, False, 0, [], "SeaPalSideChestItem", "Seaside Palace: Side Room Chest", 0, 0, [] ],
-            62:  [200, 1, False, 0, [], "SeaPalTopChestItem",  "Seaside Palace: First Area Chest", 0, 0, [] ],
-            63:  [205, 1, False, 0, [], "SeaPalBotChestItem",  "Seaside Palace: Second Area Chest", 0, 0, [] ],
-            64:  [200, 1, False, 0, [], "SeaPalBuffyItem",     "Seaside Palace: Buffy", 0, 0, [[510, 1]] ],
-            65:  [205, 1, False, 0, [], "SeaPalCoffinItem",    "Seaside Palace: Coffin", 0, 0, [[501, 1]] ],
+            61: [202, 1, False, 0, [], "SeaPalSideChestItem", "Seaside Palace: Side Room Chest", 0, 0, []],
+            62: [200, 1, False, 0, [], "SeaPalTopChestItem", "Seaside Palace: First Area Chest", 0, 0, []],
+            63: [205, 1, False, 0, [], "SeaPalBotChestItem", "Seaside Palace: Second Area Chest", 0, 0, []],
+            64: [200, 1, False, 0, [], "SeaPalBuffyItem", "Seaside Palace: Buffy", 0, 0, [[510, 1]]],
+            65: [205, 1, False, 0, [], "SeaPalCoffinItem", "Seaside Palace: Coffin", 0, 0, [[501, 1]]],
 
-            66:  [200, 2, False, 0, [], "", "Seaside Palace: Dark Space", 0, 0, [] ],
+            66: [200, 2, False, 0, [], "", "Seaside Palace: Dark Space", 0, 0, []],
 
             # Mu
-            67:  [217, 1, False, 0, [], "MuEmptyChest1Item", "Mu: Empty Chest 1", 0, 0, [] ],
-            68:  [220, 1, False, 0, [], "MuEmptyChest2Item", "Mu: Empty Chest 2", 0, 0, [] ],
-            69:  [225, 1, False, 0, [], "MuHopeStatue1Item", "Mu: Hope Statue 1", 0, 0, [] ],
-            70:  [236, 1, False, 0, [], "MuHopeStatue2Item", "Mu: Hope Statue 2", 0, 0, [] ],
-            71:  [215, 1, False, 0, [], "MuHopeRoomChestItem", "Mu: Chest s/o Hope Room 2", 0, 0, [] ],
-            72:  [214, 1, False, 0, [], "MuRamaChestNItem", "Mu: Rama Chest N", 0, 0, [] ],
-            73:  [219, 1, False, 0, [], "MuRamaChestEItem", "Mu: Rama Chest E", 0, 0, [] ],
-
-            74:  [218, 2, False, 0, [], "", "Mu: Northeast Dark Space", 0, 0, [] ],
-            75:  [228, 2, False, 0, [], "", "Mu: Slider Dark Space", 0, 0, [] ],
-
-            726: [212, 5, False, 0, [], "MuEntranceGolemItem", "Mu: Entrance Golem for Gate", 0, 0, [[609, 1]] ],
-            727: [726, 5, False, 0, [], "MuDroplet1Item", "Mu: NE Droplet for Rock 1", 0, 0, [[609, 1]] ],
-            728: [724, 5, False, 0, [], "MuDroplet2Item", "Mu: NE Droplet for Rock 2", 0, 0, [[609, 1]] ],
-            729: [227, 5, False, 0, [], "MuSlimeCageItem", "Mu: West Slime for Slime Cages", 0, 0, [[609, 1]] ],
-            730: [236, 5, False, 0, [], "MuEastFacingHeadGolemItem", "Mu: SE Golem for East-facing Head", 0, 0, [[609, 1]] ],
-            731: [236, 5, False, 0, [], "MuSouthFacingHeadGolemItem", "Mu: SE Golem for South-facing Head", 0, 0, [[609, 1]] ],
+            67: [217, 1, False, 0, [], "MuEmptyChest1Item", "Mu: Empty Chest 1", 0, 0, []],
+            68: [220, 1, False, 0, [], "MuEmptyChest2Item", "Mu: Empty Chest 2", 0, 0, []],
+            69: [225, 1, False, 0, [], "MuHopeStatue1Item", "Mu: Hope Statue 1", 0, 0, []],
+            70: [236, 1, False, 0, [], "MuHopeStatue2Item", "Mu: Hope Statue 2", 0, 0, []],
+            71: [215, 1, False, 0, [], "MuHopeRoomChestItem", "Mu: Chest s/o Hope Room 2", 0, 0, []],
+            72: [214, 1, False, 0, [], "MuRamaChestNItem", "Mu: Rama Chest N", 0, 0, []],
+            73: [219, 1, False, 0, [], "MuRamaChestEItem", "Mu: Rama Chest E", 0, 0, []],
+
+            74: [218, 2, False, 0, [], "", "Mu: Northeast Dark Space", 0, 0, []],
+            75: [228, 2, False, 0, [], "", "Mu: Slider Dark Space", 0, 0, []],
+
+            726: [212, 5, False, 0, [], "MuEntranceGolemItem", "Mu: Entrance Golem for Gate", 0, 0, [[609, 1]]],
+            727: [726, 5, False, 0, [], "MuDroplet1Item", "Mu: NE Droplet for Rock 1", 0, 0, [[609, 1]]],
+            728: [724, 5, False, 0, [], "MuDroplet2Item", "Mu: NE Droplet for Rock 2", 0, 0, [[609, 1]]],
+            729: [227, 5, False, 0, [], "MuSlimeCageItem", "Mu: West Slime for Slime Cages", 0, 0, [[609, 1]]],
+            730: [236, 5, False, 0, [], "MuEastFacingHeadGolemItem", "Mu: SE Golem for East-facing Head", 0, 0,
+                  [[609, 1]]],
+            731: [236, 5, False, 0, [], "MuSouthFacingHeadGolemItem", "Mu: SE Golem for South-facing Head", 0, 0,
+                  [[609, 1]]],
 
             # Angel Village
-            76:  [254, 1, False, 0, [], "AnglDanceHallItem", "Angel Village: Dance Hall", 0, 0, [] ],
-            77:  [255, 2, False, 0, [], "", "Angel Village: Dark Space", 0, 0, [] ],
+            76: [254, 1, False, 0, [], "AnglDanceHallItem", "Angel Village: Dance Hall", 0, 0, []],
+            77: [255, 2, False, 0, [], "", "Angel Village: Dark Space", 0, 0, []],
 
             # Angel Dungeon
-            78:  [265, 1, False, 0, [], "AnglSliderChestItem", "Angel Dungeon: Slider Chest", 0, 0, [] ],
-            79:  [271, 1, False, 0, [], "AnglIshtarSidePotItem", "Angel Dungeon: Ishtar's Room", 0, 0, [] ],
-            80:  [274, 1, False, 0, [], "AnglPuzzleChest1Item", "Angel Dungeon: Puzzle Chest 1", 0, 0, [] ],
-            81:  [274, 1, False, 0, [], "AnglPuzzleChest2Item", "Angel Dungeon: Puzzle Chest 2", 0, 0, [] ],
-            82:  [273, 1, False, 0, [], "AnglIshtarWinChestItem", "Angel Dungeon: Ishtar's Chest", 0, 0, [] ],
+            78: [265, 1, False, 0, [], "AnglSliderChestItem", "Angel Dungeon: Slider Chest", 0, 0, []],
+            79: [271, 1, False, 0, [], "AnglIshtarSidePotItem", "Angel Dungeon: Ishtar's Room", 0, 0, []],
+            80: [274, 1, False, 0, [], "AnglPuzzleChest1Item", "Angel Dungeon: Puzzle Chest 1", 0, 0, []],
+            81: [274, 1, False, 0, [], "AnglPuzzleChest2Item", "Angel Dungeon: Puzzle Chest 2", 0, 0, []],
+            82: [273, 1, False, 0, [], "AnglIshtarWinChestItem", "Angel Dungeon: Ishtar's Chest", 0, 0, []],
 
             # Watermia
-            83:  [280, 1, False, 0, [], "WtrmWestJarItem", "Watermia: West Jar", 0, 0, [] ],
-            85:  [286, 1, False, 0, [], "WtrmLanceItem", "Watermia: Lance", 0, 0, [] ],
-            86:  [283, 1, False, 0, [], "WtrmDesertJarItem", "Watermia: Gambling House", 0, 0, [] ],
-            87:  [280, 1, False, 0, [], "WtrmRussianGlassItem", "Watermia: Russian Glass", 0, 0, [] ],
+            83: [280, 1, False, 0, [], "WtrmWestJarItem", "Watermia: West Jar", 0, 0, []],
+            85: [286, 1, False, 0, [], "WtrmLanceItem", "Watermia: Lance", 0, 0, []],
+            86: [283, 1, False, 0, [], "WtrmDesertJarItem", "Watermia: Gambling House", 0, 0, []],
+            87: [280, 1, False, 0, [], "WtrmRussianGlassItem", "Watermia: Russian Glass", 0, 0, []],
 
-            88:  [282, 2, False, 0, [], "", "Watermia: Dark Space", 0, 0, [] ],
+            88: [282, 2, False, 0, [], "", "Watermia: Dark Space", 0, 0, []],
 
             # Great Wall
-            89:  [290, 1, False, 0, [], "GtWlNecklace1Item", "Great Wall: Necklace 1", 0, 0, [] ],
-            90:  [292, 1, False, 0, [], "GtWlNecklace2Item", "Great Wall: Necklace 2", 0, 0, [] ],
-            91:  [292, 1, False, 0, [], "GtWlChest1Item", "Great Wall: Chest 1", 0, 0, [] ],
-            92:  [294, 1, False, 0, [], "GtWlChest2Item", "Great Wall: Chest 2", 0, 0, [] ],
-
-            93:  [295, 2, False, 0, [], "", "Great Wall: Archer Dark Space", 0, 0, [] ],
-            94:  [297, 2, False, 0, [], "", "Great Wall: Platform Dark Space", 0, 0, [] ],
-            95:  [300, 2, False, 0, [], "", "Great Wall: Appearing Dark Space", 0, 0, [] ],
+            89: [290, 1, False, 0, [], "GtWlNecklace1Item", "Great Wall: Necklace 1", 0, 0, []],
+            90: [292, 1, False, 0, [], "GtWlNecklace2Item", "Great Wall: Necklace 2", 0, 0, []],
+            91: [292, 1, False, 0, [], "GtWlChest1Item", "Great Wall: Chest 1", 0, 0, []],
+            92: [294, 1, False, 0, [], "GtWlChest2Item", "Great Wall: Chest 2", 0, 0, []],
+
+            93: [295, 2, False, 0, [], "", "Great Wall: Archer Dark Space", 0, 0, []],
+            94: [297, 2, False, 0, [], "", "Great Wall: Platform Dark Space", 0, 0, []],
+            95: [300, 2, False, 0, [], "", "Great Wall: Appearing Dark Space", 0, 0, []],
 
-            732: [712, 5, False, 0, [], "GtWlArcherItem", "Great Wall: Archer for Friar Gate", 0, 0, [[609, 1]] ],
+            732: [712, 5, False, 0, [], "GtWlArcherItem", "Great Wall: Archer for Friar Gate", 0, 0, [[609, 1]]],
 
             # Euro
-            96:  [310, 1, False, 0, [], "EuroAlleyItem", "Euro: Alley", 0, 0, [] ],
-            97:  [310, 1, False, 0, [], "EuroAppleVendorItem", "Euro: Apple Vendor", 0, 0, [] ],
-            98:  [320, 1, False, 0, [], "EuroHiddenHouseItem", "Euro: Hidden House", 0, 0, [] ],
-            99:  [323, 1, False, 0, [], "EuroShop1Item", "Euro: Store Item 1", 0, 0, [] ],
-            100: [323, 1, False, 0, [], "EuroShop2Item", "Euro: Store Item 2", 0, 0, [] ],
-            101: [321, 1, False, 0, [], "EuroSlaveRoomBarrelItem", "Euro: Shrine", 0, 0, [] ],
-            102: [314, 1, False, 0, [], "EuroAnnItem", "Euro: Ann", 0, 0, [[40, 1]] ],
+            96: [310, 1, False, 0, [], "EuroAlleyItem", "Euro: Alley", 0, 0, []],
+            97: [310, 1, False, 0, [], "EuroAppleVendorItem", "Euro: Apple Vendor", 0, 0, []],
+            98: [320, 1, False, 0, [], "EuroHiddenHouseItem", "Euro: Hidden House", 0, 0, []],
+            99: [323, 1, False, 0, [], "EuroShop1Item", "Euro: Store Item 1", 0, 0, []],
+            100: [323, 1, False, 0, [], "EuroShop2Item", "Euro: Store Item 2", 0, 0, []],
+            101: [321, 1, False, 0, [], "EuroSlaveRoomBarrelItem", "Euro: Shrine", 0, 0, []],
+            102: [314, 1, False, 0, [], "EuroAnnItem", "Euro: Ann", 0, 0, [[40, 1]]],
 
-            103: [325, 2, False, 0, [], "", "Euro: Dark Space", 0, 0, [] ],
+            103: [325, 2, False, 0, [], "", "Euro: Dark Space", 0, 0, []],
 
             # Mt Temple
-            104: [336, 1, False, 0, [], "KressChest1Item", "Mt. Temple: Red Jewel Chest", 0, 0, [] ],
-            105: [338, 1, False, 0, [], "KressChest2Item", "Mt. Temple: Drops Chest 1", 0, 0, [] ],
-            106: [342, 1, False, 0, [], "KressChest3Item", "Mt. Temple: Drops Chest 2", 0, 0, [] ],
-            107: [343, 1, False, 0, [], "KressChest4Item", "Mt. Temple: Drops Chest 3", 0, 0, [] ],
-            108: [345, 1, False, 0, [], "KressChest5Item", "Mt. Temple: Final Chest", 0, 0, [] ],
-
-            109: [332, 2, False, 0, [], "", "Mt. Temple: Dark Space 1", 0, 0, [] ],
-            110: [337, 2, False, 0, [], "", "Mt. Temple: Dark Space 2", 0, 0, [] ],
-            111: [343, 2, False, 0, [], "", "Mt. Temple: Dark Space 3", 0, 0, [] ],
+            104: [336, 1, False, 0, [], "KressChest1Item", "Mt. Temple: Red Jewel Chest", 0, 0, []],
+            105: [338, 1, False, 0, [], "KressChest2Item", "Mt. Temple: Drops Chest 1", 0, 0, []],
+            106: [342, 1, False, 0, [], "KressChest3Item", "Mt. Temple: Drops Chest 2", 0, 0, []],
+            107: [343, 1, False, 0, [], "KressChest4Item", "Mt. Temple: Drops Chest 3", 0, 0, []],
+            108: [345, 1, False, 0, [], "KressChest5Item", "Mt. Temple: Final Chest", 0, 0, []],
+
+            109: [332, 2, False, 0, [], "", "Mt. Temple: Dark Space 1", 0, 0, []],
+            110: [337, 2, False, 0, [], "", "Mt. Temple: Dark Space 2", 0, 0, []],
+            111: [343, 2, False, 0, [], "", "Mt. Temple: Dark Space 3", 0, 0, []],
 
-            734: [338, 5, False, 0, [], "KressSkullShortcutItem", "Mt. Temple: Skull for Drops Chest 1 Shortcut", 0, 0, [[609, 1]] ],
+            734: [338, 5, False, 0, [], "KressSkullShortcutItem", "Mt. Temple: Skull for Drops Chest 1 Shortcut", 0, 0,
+                  [[609, 1]]],
 
             # Natives'
-            112: [353, 1, False, 0, [], "NativesPotItem", "Natives' Village: Statue Room", 0, 0, [] ],
-            113: [354, 1, False, 0, [], "NativesGirlItem", "Natives' Village: Statue", 0, 0, [] ],
+            112: [353, 1, False, 0, [], "NativesPotItem", "Natives' Village: Statue Room", 0, 0, []],
+            113: [354, 1, False, 0, [], "NativesGirlItem", "Natives' Village: Statue", 0, 0, []],
 
-            114: [350, 2, False, 0, [], "", "Natives' Village: Dark Space", 0, 0, [] ],
+            114: [350, 2, False, 0, [], "", "Natives' Village: Dark Space", 0, 0, []],
 
             # Ankor Wat
-            115: [361, 1, False, 0, [], "WatChest1Item", "Ankor Wat: Ramp Chest", 0, 0, [] ],
-            116: [370, 1, False, 0, [], "WatChest2Item", "Ankor Wat: Flyover Chest", 0, 0, [] ],
-            117: [378, 1, False, 0, [], "WatChest3Item", "Ankor Wat: U-Turn Chest", 0, 0, [] ],
-            118: [382, 1, False, 0, [], "WatChest4Item", "Ankor Wat: Drop Down Chest", 0, 0, [] ],
-            119: [389, 1, False, 0, [], "WatChest5Item", "Ankor Wat: Forgotten Chest", 0, 0, [] ],
-            120: [380, 1, False, 0, [], "WatGlassesItem", "Ankor Wat: Glasses Location", 0, 0, [] ],
-            121: [391, 1, False, 0, [], "WatSpiritItem", "Ankor Wat: Spirit", 0, 0, [] ],
-
-            122: [372, 2, False, 0, [], "", "Ankor Wat: Garden Dark Space", 0, 0, [] ],
-            123: [377, 2, False, 0, [], "", "Ankor Wat: Earthquaker Dark Space", 0, 0, [] ],
-            124: [383, 2, False, 0, [], "", "Ankor Wat: Drop Down Dark Space", 0, 0, [] ],
-
-            735: [739, 5, False, 0, [], "WatSouthScarabItem", "Ankor Wat: Scarab for Outer South Stair", 0, 0, [[609, 1]] ],
-            736: [364, 5, False, 0, [], "WatEastSliderHoleItem", "Ankor Wat: Scarab for Outer East Slider Hole", 0, 0, [[609, 1]] ],
-            738: [727, 5, False, 0, [], "WatDarkSpaceHallItem", "Ankor Wat: Skull for Inner East DS Hall", 0, 0, [[609, 1]] ],
+            115: [361, 1, False, 0, [], "WatChest1Item", "Ankor Wat: Ramp Chest", 0, 0, []],
+            116: [370, 1, False, 0, [], "WatChest2Item", "Ankor Wat: Flyover Chest", 0, 0, []],
+            117: [378, 1, False, 0, [], "WatChest3Item", "Ankor Wat: U-Turn Chest", 0, 0, []],
+            118: [382, 1, False, 0, [], "WatChest4Item", "Ankor Wat: Drop Down Chest", 0, 0, []],
+            119: [389, 1, False, 0, [], "WatChest5Item", "Ankor Wat: Forgotten Chest", 0, 0, []],
+            120: [380, 1, False, 0, [], "WatGlassesItem", "Ankor Wat: Glasses Location", 0, 0, []],
+            121: [391, 1, False, 0, [], "WatSpiritItem", "Ankor Wat: Spirit", 0, 0, []],
+
+            122: [372, 2, False, 0, [], "", "Ankor Wat: Garden Dark Space", 0, 0, []],
+            123: [377, 2, False, 0, [], "", "Ankor Wat: Earthquaker Dark Space", 0, 0, []],
+            124: [383, 2, False, 0, [], "", "Ankor Wat: Drop Down Dark Space", 0, 0, []],
+
+            735: [739, 5, False, 0, [], "WatSouthScarabItem", "Ankor Wat: Scarab for Outer South Stair", 0, 0,
+                  [[609, 1]]],
+            736: [364, 5, False, 0, [], "WatEastSliderHoleItem", "Ankor Wat: Scarab for Outer East Slider Hole", 0, 0,
+                  [[609, 1]]],
+            738: [727, 5, False, 0, [], "WatDarkSpaceHallItem", "Ankor Wat: Skull for Inner East DS Hall", 0, 0,
+                  [[609, 1]]],
 
             # Dao
-            125: [400, 1, False, 0, [], "DaoEntrance1Item", "Dao: Entrance Item 1", 0, 0, [] ],
-            126: [400, 1, False, 0, [], "DaoEntrance2Item", "Dao: Entrance Item 2", 0, 0, [] ],
-            127: [400, 1, False, 0, [], "DaoGrassItem", "Dao: East Grass", 0, 0, [] ],
-            128: [403, 1, False, 0, [], "DaoSnakeGameItem", "Dao: Snake Game", 0, 0, [[609, 1]] ],
+            125: [400, 1, False, 0, [], "DaoEntrance1Item", "Dao: Entrance Item 1", 0, 0, []],
+            126: [400, 1, False, 0, [], "DaoEntrance2Item", "Dao: Entrance Item 2", 0, 0, []],
+            127: [400, 1, False, 0, [], "DaoGrassItem", "Dao: East Grass", 0, 0, []],
+            128: [403, 1, False, 0, [], "DaoSnakeGameItem", "Dao: Snake Game", 0, 0, [[609, 1]]],
 
-            129: [400, 2, False, 0, [], "", "Dao: Dark Space", 0, 0, [] ],
+            129: [400, 2, False, 0, [], "", "Dao: Dark Space", 0, 0, []],
 
             # Pyramid
-            130: [713, 1, False, 0, [], "PyramidGaiaItem", "Pyramid: Dark Space Top", 0, 0, [] ],
-            131: [412, 1, False, 0, [], "PyramidFoyerItem", "Pyramid: Hidden Platform", 0, 0, [] ],
-            132: [442, 1, False, 0, [], "PyramidHiero1Item", "Pyramid: Hieroglyph 1", 0, 0, [] ],
-            133: [422, 1, False, 0, [], "PyramidRoom2ChestItem", "Pyramid: Room 2 Chest", 0, 0, [] ],
-            134: [443, 1, False, 0, [], "PyramidHiero2Item", "Pyramid: Hieroglyph 2", 0, 0, [] ],
-            135: [432, 1, False, 0, [], "PyramidRoom3ChestItem", "Pyramid: Room 3 Chest", 0, 0, [] ],
-            136: [444, 1, False, 0, [], "PyramidHiero3Item", "Pyramid: Hieroglyph 3", 0, 0, [] ],
-            137: [439, 1, False, 0, [], "PyramidRoom4ChestItem", "Pyramid: Room 4 Chest", 0, 0, [] ],
-            138: [445, 1, False, 0, [], "PyramidHiero4Item", "Pyramid: Hieroglyph 4", 0, 0, [] ],
-            139: [428, 1, False, 0, [], "PyramidRoom5ChestItem", "Pyramid: Room 5 Chest", 0, 0, [] ],
-            140: [446, 1, False, 0, [], "PyramidHiero5Item", "Pyramid: Hieroglyph 5", 0, 0, [] ],
-            141: [447, 1, False, 0, [], "PyramidHiero6Item", "Pyramid: Hieroglyph 6", 0, 0, [] ],
+            130: [713, 1, False, 0, [], "PyramidGaiaItem", "Pyramid: Dark Space Top", 0, 0, []],
+            131: [412, 1, False, 0, [], "PyramidFoyerItem", "Pyramid: Hidden Platform", 0, 0, []],
+            132: [442, 1, False, 0, [], "PyramidHiero1Item", "Pyramid: Hieroglyph 1", 0, 0, []],
+            133: [422, 1, False, 0, [], "PyramidRoom2ChestItem", "Pyramid: Room 2 Chest", 0, 0, []],
+            134: [443, 1, False, 0, [], "PyramidHiero2Item", "Pyramid: Hieroglyph 2", 0, 0, []],
+            135: [432, 1, False, 0, [], "PyramidRoom3ChestItem", "Pyramid: Room 3 Chest", 0, 0, []],
+            136: [444, 1, False, 0, [], "PyramidHiero3Item", "Pyramid: Hieroglyph 3", 0, 0, []],
+            137: [439, 1, False, 0, [], "PyramidRoom4ChestItem", "Pyramid: Room 4 Chest", 0, 0, []],
+            138: [445, 1, False, 0, [], "PyramidHiero4Item", "Pyramid: Hieroglyph 4", 0, 0, []],
+            139: [428, 1, False, 0, [], "PyramidRoom5ChestItem", "Pyramid: Room 5 Chest", 0, 0, []],
+            140: [446, 1, False, 0, [], "PyramidHiero5Item", "Pyramid: Hieroglyph 5", 0, 0, []],
+            141: [447, 1, False, 0, [], "PyramidHiero6Item", "Pyramid: Hieroglyph 6", 0, 0, []],
 
-            142: [413, 2, False, 0, [], "", "Pyramid: Dark Space Bottom", 0, 0, [] ],
+            142: [413, 2, False, 0, [], "", "Pyramid: Dark Space Bottom", 0, 0, []],
 
-            739: [411, 5, False, 0, [], "PyramidEntranceOrbsItem", "Pyramid: Entrance Orbs for DS Gate", 0, 0, [[609, 1]] ],
+            739: [411, 5, False, 0, [], "PyramidEntranceOrbsItem", "Pyramid: Entrance Orbs for DS Gate", 0, 0,
+                  [[609, 1]]],
 
             # Babel
-            143: [461, 1, False, 0, [], "BabelPillowItem", "Babel: Pillow", 0, 0, [] ],
-            144: [461, 1, False, 0, [], "BabelForceFieldItem", "Babel: Force Field", 0, 0, [] ],
+            143: [461, 1, False, 0, [], "BabelPillowItem", "Babel: Pillow", 0, 0, []],
+            144: [461, 1, False, 0, [], "BabelForceFieldItem", "Babel: Force Field", 0, 0, []],
 
-            145: [461, 2, False, 0, [], "", "Babel: Dark Space Bottom", 0, 0, [] ],
-            146: [472, 2, False, 0, [], "", "Babel: Dark Space Top", 0, 0, [] ],
+            145: [461, 2, False, 0, [], "", "Babel: Dark Space Bottom", 0, 0, []],
+            146: [472, 2, False, 0, [], "", "Babel: Dark Space Top", 0, 0, []],
 
             # Jeweler's Mansion
-            147: [715, 1, False, 0, [], "MansionChestItem", "Jeweler's Mansion: Chest", 0, 0, [] ],
+            147: [715, 1, False, 0, [], "MansionChestItem", "Jeweler's Mansion: Chest", 0, 0, []],
 
-            740: [480, 5, False, 0, [], "MansionEastGateItem", "Jeweler's Mansion: Enemy for East Gate", 0, 0, [[609, 1]] ],
-            741: [714, 5, False, 0, [], "MansionWestGateItem", "Jeweler's Mansion: Enemy for West Gate", 0, 0, [[609, 1]] ],
+            740: [480, 5, False, 0, [], "MansionEastGateItem", "Jeweler's Mansion: Enemy for East Gate", 0, 0,
+                  [[609, 1]]],
+            741: [714, 5, False, 0, [], "MansionWestGateItem", "Jeweler's Mansion: Enemy for West Gate", 0, 0,
+                  [[609, 1]]],
 
             # Mystic Statues
-            148: [101, 3, False, 0, [101, 102, 103, 104, 105], "", "Castoth Prize", 0, 0, [] ],
-            149: [198, 3, False, 0, [100, 102, 103, 104, 105], "", "Viper Prize", 0, 0, [] ],
-            150: [244, 3, False, 0, [100, 101, 103, 104, 105], "", "Vampires Prize", 0, 0, [] ],
-            151: [302, 3, False, 0, [100, 101, 102, 104, 105], "", "Sand Fanger Prize", 0, 0, [] ],
-            152: [448, 3, False, 0, [100, 101, 102, 103, 105], "", "Mummy Queen Prize", 0, 0, [] ],
-            153: [479, 3, False, 0, [100, 101, 102, 103, 104], "", "Babel Prize", 0, 0, [] ],
+            148: [101, 3, False, 0, [101, 102, 103, 104, 105], "", "Castoth Prize", 0, 0, []],
+            149: [198, 3, False, 0, [100, 102, 103, 104, 105], "", "Viper Prize", 0, 0, []],
+            150: [244, 3, False, 0, [100, 101, 103, 104, 105], "", "Vampires Prize", 0, 0, []],
+            151: [302, 3, False, 0, [100, 101, 102, 104, 105], "", "Sand Fanger Prize", 0, 0, []],
+            152: [448, 3, False, 0, [100, 101, 102, 103, 105], "", "Mummy Queen Prize", 0, 0, []],
+            153: [479, 3, False, 0, [100, 101, 102, 103, 104], "", "Babel Prize", 0, 0, []],
 
             # Event Switches
-            500: [500, 4, True, 500, [], "", "Kara", 0, 0, [] ],
-            501: [ 55, 4, True, 501, [], "", "Lilly", 0, 0, [[23, 1]] ],
-            502: [502, 4, True, 502, [], "", "Moon Tribe: Spirits Healed", 0, 0, [] ],
-            503: [503, 4, True, 503, [], "", "Inca: Castoth defeated", 0, 0, [] ],
-            504: [122, 4, True, 504, [], "", "Freejia: Found Laborer", 0, 0, [] ],
-            505: [505, 4, True, 505, [], "", "Neil's Memory Restored", 0, 0, [] ],
-            506: [186, 4, True, 506, [], "", "Sky Garden: Map 82 NW Switch pressed", 0, 0, [[609, 1]] ],
-            507: [189, 4, True, 507, [], "", "Sky Garden: Map 82 NE Switch pressed", 0, 0, [] ],
-            508: [508, 4, True, 508, [], "", "Sky Garden: Map 82 SE Switch pressed", 0, 0, [] ],
-            509: [509, 4, True, 509, [], "", "Sky Garden: Map 84 Statue Switch pressed", 0, 0, [] ],
-            510: [209, 4, True, 510, [], "", "Seaside: Fountain Purified", 0, 0, [[17, 1]] ],
-            511: [511, 4, True, 511, [], "", "Mu: Water Lowered 1", 0, 0, [] ],
-            512: [512, 4, True, 512, [], "", "Mu: Water Lowered 2", 0, 0, [] ],
-            513: [274, 4, True, 513, [], "", "Angel: Puzzle Complete", 0, 0, [] ],
-            514: [514, 4, True, 514, [], "", "Mt Kress: Drops used 1", 0, 0, [] ],
-            515: [515, 4, True, 515, [], "", "Mt Kress: Drops used 2", 0, 0, [] ],
-            516: [516, 4, True, 516, [], "", "Mt Kress: Drops used 3", 0, 0, [] ],
-            517: [517, 4, True, 517, [], "", "Pyramid: Hieroglyphs placed", 0, 0, [] ],
-            518: [518, 4, True, 518, [], "", "Babel: Castoth defeated", 0, 0, [] ],
-            519: [519, 4, True, 519, [], "", "Babel: Viper defeated", 0, 0, [] ],
-            520: [520, 4, True, 520, [], "", "Babel: Vampires defeated", 0, 0, [] ],
-            521: [521, 4, True, 521, [], "", "Babel: Sand Fanger defeated", 0, 0, [] ],
-            522: [522, 4, True, 522, [], "", "Babel: Mummy Queen defeated", 0, 0, [] ],
-            523: [523, 4, True, 523, [], "", "Mansion: Solid Arm defeated", 0, 0, [] ],
-            524: [ 89, 4, True, 524, [], "", "Inca: Diamond Block Placed", 0, 0, [[7, 1]] ],
-            525: [525, 4, True, 525, [], "", "Pyramid: Portals open", 0, 0, [] ],
-            526: [526, 4, True, 526, [], "", "Mu: Access to Hope Room 1", 0, 0, [] ],
-            527: [527, 4, True, 527, [], "", "Mu: Access to Hope Room 2", 0, 0, [] ],
-            528: [131, 4, True, 528, [], "", "Mine: Blocked Tunnel Open", 0, 0, [[608, 1]] ],
-            529: [529, 4, True, 529, [], "", "Underground Tunnel: Bridge Open", 0, 0, [] ],
-            530: [530, 4, True, 530, [], "", "Inca: Slug Statue Broken", 0, 0, [] ],
-            531: [531, 4, True, 531, [], "", "Mu: Beat Vampires", 0, 0, [] ],
+            500: [500, 4, True, 500, [], "", "Kara", 0, 0, []],
+            501: [55, 4, True, 501, [], "", "Lilly", 0, 0, [[23, 1]]],
+            502: [502, 4, True, 502, [], "", "Moon Tribe: Spirits Healed", 0, 0, []],
+            503: [503, 4, True, 503, [], "", "Inca: Castoth defeated", 0, 0, []],
+            504: [122, 4, True, 504, [], "", "Freejia: Found Laborer", 0, 0, []],
+            505: [505, 4, True, 505, [], "", "Neil's Memory Restored", 0, 0, []],
+            506: [186, 4, True, 506, [], "", "Sky Garden: Map 82 NW Switch pressed", 0, 0, [[609, 1]]],
+            507: [189, 4, True, 507, [], "", "Sky Garden: Map 82 NE Switch pressed", 0, 0, []],
+            508: [508, 4, True, 508, [], "", "Sky Garden: Map 82 SE Switch pressed", 0, 0, []],
+            509: [509, 4, True, 509, [], "", "Sky Garden: Map 84 Statue Switch pressed", 0, 0, []],
+            510: [209, 4, True, 510, [], "", "Seaside: Fountain Purified", 0, 0, [[17, 1]]],
+            511: [511, 4, True, 511, [], "", "Mu: Water Lowered 1", 0, 0, []],
+            512: [512, 4, True, 512, [], "", "Mu: Water Lowered 2", 0, 0, []],
+            513: [274, 4, True, 513, [], "", "Angel: Puzzle Complete", 0, 0, []],
+            514: [514, 4, True, 514, [], "", "Mt Kress: Drops used 1", 0, 0, []],
+            515: [515, 4, True, 515, [], "", "Mt Kress: Drops used 2", 0, 0, []],
+            516: [516, 4, True, 516, [], "", "Mt Kress: Drops used 3", 0, 0, []],
+            517: [517, 4, True, 517, [], "", "Pyramid: Hieroglyphs placed", 0, 0, []],
+            518: [518, 4, True, 518, [], "", "Babel: Castoth defeated", 0, 0, []],
+            519: [519, 4, True, 519, [], "", "Babel: Viper defeated", 0, 0, []],
+            520: [520, 4, True, 520, [], "", "Babel: Vampires defeated", 0, 0, []],
+            521: [521, 4, True, 521, [], "", "Babel: Sand Fanger defeated", 0, 0, []],
+            522: [522, 4, True, 522, [], "", "Babel: Mummy Queen defeated", 0, 0, []],
+            523: [523, 4, True, 523, [], "", "Mansion: Solid Arm defeated", 0, 0, []],
+            524: [89, 4, True, 524, [], "", "Inca: Diamond Block Placed", 0, 0, [[7, 1]]],
+            525: [525, 4, True, 525, [], "", "Pyramid: Portals open", 0, 0, []],
+            526: [526, 4, True, 526, [], "", "Mu: Access to Hope Room 1", 0, 0, []],
+            527: [527, 4, True, 527, [], "", "Mu: Access to Hope Room 2", 0, 0, []],
+            528: [131, 4, True, 528, [], "", "Mine: Blocked Tunnel Open", 0, 0, [[608, 1]]],
+            529: [529, 4, True, 529, [], "", "Underground Tunnel: Bridge Open", 0, 0, []],
+            530: [530, 4, True, 530, [], "", "Inca: Slug Statue Broken", 0, 0, []],
+            531: [531, 4, True, 531, [], "", "Mu: Beat Vampires", 0, 0, []],
 
             # Misc
-            #602: [0, 6, True, 602, [], "", "Early Firebird enabled", 0, 0, [] ],
-            603: [491, 6, True, 67,  [], "", "Firebird access", 0, 0, [] ],
-            #604: [604, 6, True, 604, [], "", "Flute", 0, 0, [] ],
-            #608: [608, 6, True, 608, [], "", "Has Any Will Ability", 0, 0, [] ],
-            #609: [609, 6, True, 609, [], "", "Has Any Attack", 0, 0, [] ],
-            #610: [610, 6, True, 610, [], "", "Has Any Ranged Attack", 0, 0]
+            # 602: [0, 6, True, 602, [], "", "Early Firebird enabled", 0, 0, [] ],
+            603: [491, 6, True, 67, [], "", "Firebird access", 0, 0, []],
+            # 604: [604, 6, True, 604, [], "", "Flute", 0, 0, [] ],
+            # 608: [608, 6, True, 608, [], "", "Has Any Will Ability", 0, 0, [] ],
+            # 609: [609, 6, True, 609, [], "", "Has Any Attack", 0, 0, [] ],
+            # 610: [610, 6, True, 610, [], "", "Has Any Ranged Attack", 0, 0]
         }
 
         # Shell world graph. Nodes for exits are added during initialization.
         # Format: { Region ID: [
         #                   0: Traversed_flag,
         #                   1: [AccessibleRegions],
         #                   2: type(0=other/misc,1=exterior,2=interior,3=roof),
@@ -3880,540 +3978,847 @@
         #                   12: [origin_logic],
         #                   13: [dest_logic],
         #                   14: [origin_exits],
         #                   15: [dest_exits]
         #                   ] }
         self.deleted_graph = {}
         self.graph = {
-            -2: [False, [], 0, [0,0,0,0], 0, "Deleted Node", [], False, [], [], [], [], [], [], [], []],
-            -1: [False, [], 0, [0,0,0,0], 0, "Inaccessible Node", [], False, [], [], [], [], [], [], [], []],
-            
+            -2: [False, [], 0, [0, 0, 0, 0], 0, "Deleted Node", [], False, [], [], [], [], [], [], [], []],
+            -1: [False, [], 0, [0, 0, 0, 0], 0, "Inaccessible Node", [], False, [], [], [], [], [], [], [], []],
+
             # Game Start
-            0: [False, [], 0, [0,0,0,0], 0, "Game Start", [], True, [], [], [], [], [], [], [], []],
+            0: [False, [], 0, [0, 0, 0, 0], 0, "Game Start", [], True, [], [], [], [], [], [], [], []],
 
             # Jeweler
-            1: [False, [], 0, [0,0,0,0], 0, "Jeweler Access", [], False, [], [], [], [], [], [], [], []],
-            2: [False, [], 0, [0,0,0,0], 0, "Jeweler Reward 1", [], False, [], [], [], [], [], [], [], []],
-            3: [False, [], 0, [0,0,0,0], 0, "Jeweler Reward 2", [], False, [], [], [], [], [], [], [], []],
-            4: [False, [], 0, [0,0,0,0], 0, "Jeweler Reward 3", [], False, [], [], [], [], [], [], [], []],
-            5: [False, [], 0, [0,0,0,0], 0, "Jeweler Reward 4", [], False, [], [], [], [], [], [], [], []],
-            6: [False, [], 0, [0,0,0,0], 0, "Jeweler Reward 5", [], False, [], [], [], [], [], [], [], []],
-            7: [False, [], 0, [0,0,0,0], 0, "Jeweler Reward 6", [], False, [], [], [], [], [], [], [], []],
-            8: [False, [], 0, [0,0,0,0], 0, "Jeweler Reward 7", [], False, [], [], [], [], [], [], [], []],
+            1: [False, [], 0, [0, 0, 0, 0], 0, "Jeweler Access", [], False, [], [], [], [], [], [], [], []],
+            2: [False, [], 0, [0, 0, 0, 0], 0, "Jeweler Reward 1", [], False, [], [], [], [], [], [], [], []],
+            3: [False, [], 0, [0, 0, 0, 0], 0, "Jeweler Reward 2", [], False, [], [], [], [], [], [], [], []],
+            4: [False, [], 0, [0, 0, 0, 0], 0, "Jeweler Reward 3", [], False, [], [], [], [], [], [], [], []],
+            5: [False, [], 0, [0, 0, 0, 0], 0, "Jeweler Reward 4", [], False, [], [], [], [], [], [], [], []],
+            6: [False, [], 0, [0, 0, 0, 0], 0, "Jeweler Reward 5", [], False, [], [], [], [], [], [], [], []],
+            7: [False, [], 0, [0, 0, 0, 0], 0, "Jeweler Reward 6", [], False, [], [], [], [], [], [], [], []],
+            8: [False, [], 0, [0, 0, 0, 0], 0, "Jeweler Reward 7", [], False, [], [], [], [], [], [], [], []],
 
             # Overworld Menus
-            10: [False, [20,30,50,60,63],      0, [1,0,0,0], 0, "Overworld: SW Continent", [], True, [], [], [], [], [], [], [], []],
-            11: [False, [102,110,133,160,162], 0, [2,0,0,0], 0, "Overworld: SE Continent", [], True, [], [], [], [], [], [], [], []],
-            12: [False, [250,280,290],         0, [3,0,0,0], 0, "Overworld: NE Continent", [], True, [], [], [], [], [], [], [], []],
-            13: [False, [310,330,350,360],     0, [4,0,0,0], 0, "Overworld: N Continent", [], True, [], [], [], [], [], [], [], []],
-            14: [False, [400,410],             0, [5,0,0,0], 0, "Overworld: NW Continent", [], True, [], [], [], [], [], [], [], []],
+            10: [False, [20, 30, 50, 60, 63], 0, [1, 0, 0, 0], 0, "Overworld: SW Continent", [], True, [], [], [], [],
+                 [], [], [], []],
+            11: [False, [102, 110, 133, 160, 162], 0, [2, 0, 0, 0], 0, "Overworld: SE Continent", [], True, [], [], [],
+                 [], [], [], [], []],
+            12: [False, [250, 280, 290], 0, [3, 0, 0, 0], 0, "Overworld: NE Continent", [], True, [], [], [], [], [],
+                 [], [], []],
+            13: [False, [310, 330, 350, 360], 0, [4, 0, 0, 0], 0, "Overworld: N Continent", [], True, [], [], [], [],
+                 [], [], [], []],
+            14: [False, [400, 410], 0, [5, 0, 0, 0], 0, "Overworld: NW Continent", [], True, [], [], [], [], [], [], [],
+                 []],
 
             # Passage Menus
-            15: [False, [], 0, [0,0,0,0], 0, "Passage: Seth", [], True, [], [], [], [], [], [], [], []],
-            16: [False, [], 0, [0,0,0,0], 0, "Passage: Moon Tribe", [], True, [], [], [], [], [], [], [], []],
-            17: [False, [], 0, [0,0,0,0], 0, "Passage: Neil", [], True, [], [], [], [], [], [], [], []],
+            15: [False, [], 0, [0, 0, 0, 0], 0, "Passage: Seth", [], True, [], [], [], [], [], [], [], []],
+            16: [False, [], 0, [0, 0, 0, 0], 0, "Passage: Moon Tribe", [], True, [], [], [], [], [], [], [], []],
+            17: [False, [], 0, [0, 0, 0, 0], 0, "Passage: Neil", [], True, [], [], [], [], [], [], [], []],
 
             # South Cape
-            20: [False, [1,10],  1, [1,1,0,1], 0, "South Cape: Main Area", [], False, [], [], [], [], [], [], [], []],
-            21: [False, [20],    3, [1,1,0,1], 0, "South Cape: School Roof", [], False, [], [], [], [], [], [], [], []],
-            22: [False, [],      2, [1,1,0,8], 0, "South Cape: School", [], False, [], [], [], [], [], [], [], []],
-            23: [False, [],      2, [1,1,0,6], 0, "South Cape: Will's House", [], False, [], [], [], [], [], [], [], []],
-            24: [False, [],      2, [1,1,0,7], 0, "South Cape: East House", [], False, [], [], [], [], [], [], [], []],
-            25: [False, [],      2, [1,1,0,5], 0, "South Cape: Seth's House", [], False, [], [], [], [], [], [], [], []],
-            26: [False, [],      2, [1,1,0,3], 0, "South Cape: Lance's House", [], False, [], [], [], [], [], [], [], []],
-            27: [False, [],      2, [1,1,0,4], 0, "South Cape: Erik's House", [], False, [], [], [], [], [], [], [], []],
-            28: [False, [],      2, [1,1,0,2], 0, "South Cape: Seaside Cave", [], False, [], [], [], [], [], [], [], []],
+            20: [False, [1, 10], 1, [1, 1, 0, 1], 0, "South Cape: Main Area", [], False, [], [], [], [], [], [], [],
+                 []],
+            21: [False, [20], 3, [1, 1, 0, 1], 0, "South Cape: School Roof", [], False, [], [], [], [], [], [], [], []],
+            22: [False, [], 2, [1, 1, 0, 8], 0, "South Cape: School", [], False, [], [], [], [], [], [], [], []],
+            23: [False, [], 2, [1, 1, 0, 6], 0, "South Cape: Will's House", [], False, [], [], [], [], [], [], [], []],
+            24: [False, [], 2, [1, 1, 0, 7], 0, "South Cape: East House", [], False, [], [], [], [], [], [], [], []],
+            25: [False, [], 2, [1, 1, 0, 5], 0, "South Cape: Seth's House", [], False, [], [], [], [], [], [], [], []],
+            26: [False, [], 2, [1, 1, 0, 3], 0, "South Cape: Lance's House", [], False, [], [], [], [], [], [], [], []],
+            27: [False, [], 2, [1, 1, 0, 4], 0, "South Cape: Erik's House", [], False, [], [], [], [], [], [], [], []],
+            28: [False, [], 2, [1, 1, 0, 2], 0, "South Cape: Seaside Cave", [], False, [], [], [], [], [], [], [], []],
 
             # Edward's / Prison
-            30: [False, [10], 1, [1,2,0,10], 0, "Edward's Castle: Main Area", [], False, [], [], [], [], [], [], [], []],
-            31: [False, [30], 3, [1,2,0,10], 0, "Edward's Castle: Behind Guard", [], False, [], [], [], [], [], [], [], []],
-            32: [False, [],   2, [1,2,0,11], 0, "Edward's Prison: Will's Cell", [2], False, [], [], [], [], [], [], [], []],
-            33: [False, [],   2, [1,2,0,11], 0, "Edward's Prison: Prison Main", [2], False, [], [], [], [], [], [], [], []],
+            30: [False, [10], 1, [1, 2, 0, 10], 0, "Edward's Castle: Main Area", [], False, [], [], [], [], [], [], [],
+                 []],
+            31: [False, [30], 3, [1, 2, 0, 10], 0, "Edward's Castle: Behind Guard", [], False, [], [], [], [], [], [],
+                 [], []],
+            32: [False, [], 2, [1, 2, 0, 11], 0, "Edward's Prison: Will's Cell", [2], False, [], [], [], [], [], [], [],
+                 []],
+            33: [False, [], 2, [1, 2, 0, 11], 0, "Edward's Prison: Prison Main", [2], False, [], [], [], [], [], [], [],
+                 []],
 
             # Underground Tunnel
-            40: [False, [],   2, [1,2,0,12], 0, "U.Tunnel: Entry (12/$0c)", [], False, [], [], [], [], [], [], [], []],
-            41: [False, [],   2, [1,2,0,13], 0, "U.Tunnel: East Room (13/$0d)", [], False, [], [], [], [], [], [], [], []],
-            38: [False, [],   2, [1,2,0,14], 0, "U.Tunnel: South Room (14/$0e) NE before statues", [], False, [], [], [], [], [], [], [], []],
-            39: [False, [],   2, [1,2,0,14], 0, "U.Tunnel: South Room (14/$0e) past spikes", [], False, [], [], [], [], [], [], [], []],
-            42: [False, [],   2, [1,2,0,14], 0, "U.Tunnel: South Room (14/$0e) past statues", [], False, [], [], [], [], [], [], [], []],
-            43: [False, [],   2, [1,2,0,15], 0, "U.Tunnel: West Room (15/$0f)", [], False, [], [], [], [], [], [], [], []],
-            44: [False, [],   2, [1,2,0,16], 0, "U.Tunnel: Chest Room (16/$10)", [], False, [], [], [], [], [], [], [], []],
-            45: [False, [],   2, [1,2,0,17], 0, "U.Tunnel: Flower Room (17/$11)", [], False, [], [], [], [], [], [], [], []],
-            47: [False, [],   2, [1,2,0,18], 0, "U.Tunnel: Big Room (18/$12) Entrance", [], False, [], [], [], [], [], [], [], []],
-            720: [False, [],  2, [1,2,0,18], 0, "U.Tunnel: Big Room (18/$12) Dark Space", [], False, [], [], [], [], [], [], [], []],
-            704: [False, [],  2, [1,2,0,18], 0, "U.Tunnel: Big Room (18/$12) Skeleton 1 area", [], False, [], [], [], [], [], [], [], []],
-            705: [False, [],  2, [1,2,0,18], 0, "U.Tunnel: Big Room (18/$12) Skeleton 2 area", [], False, [], [], [], [], [], [], [], []],
-            706: [False, [],  2, [1,2,0,18], 0, "U.Tunnel: Big Room (18/$12) Ending area", [], False, [], [], [], [], [], [], [], []],
-            49: [False, [],   2, [1,2,0,19], 0, "U.Tunnel: Exit (19/$13)", [], True, [], [], [], [], [], [], [], []],
+            40: [False, [], 2, [1, 2, 0, 12], 0, "U.Tunnel: Entry (12/$0c)", [], False, [], [], [], [], [], [], [], []],
+            41: [False, [], 2, [1, 2, 0, 13], 0, "U.Tunnel: East Room (13/$0d)", [], False, [], [], [], [], [], [], [],
+                 []],
+            38: [False, [], 2, [1, 2, 0, 14], 0, "U.Tunnel: South Room (14/$0e) NE before statues", [], False, [], [],
+                 [], [], [], [], [], []],
+            39: [False, [], 2, [1, 2, 0, 14], 0, "U.Tunnel: South Room (14/$0e) past spikes", [], False, [], [], [], [],
+                 [], [], [], []],
+            42: [False, [], 2, [1, 2, 0, 14], 0, "U.Tunnel: South Room (14/$0e) past statues", [], False, [], [], [],
+                 [], [], [], [], []],
+            43: [False, [], 2, [1, 2, 0, 15], 0, "U.Tunnel: West Room (15/$0f)", [], False, [], [], [], [], [], [], [],
+                 []],
+            44: [False, [], 2, [1, 2, 0, 16], 0, "U.Tunnel: Chest Room (16/$10)", [], False, [], [], [], [], [], [], [],
+                 []],
+            45: [False, [], 2, [1, 2, 0, 17], 0, "U.Tunnel: Flower Room (17/$11)", [], False, [], [], [], [], [], [],
+                 [], []],
+            47: [False, [], 2, [1, 2, 0, 18], 0, "U.Tunnel: Big Room (18/$12) Entrance", [], False, [], [], [], [], [],
+                 [], [], []],
+            720: [False, [], 2, [1, 2, 0, 18], 0, "U.Tunnel: Big Room (18/$12) Dark Space", [], False, [], [], [], [],
+                  [], [], [], []],
+            704: [False, [], 2, [1, 2, 0, 18], 0, "U.Tunnel: Big Room (18/$12) Skeleton 1 area", [], False, [], [], [],
+                  [], [], [], [], []],
+            705: [False, [], 2, [1, 2, 0, 18], 0, "U.Tunnel: Big Room (18/$12) Skeleton 2 area", [], False, [], [], [],
+                  [], [], [], [], []],
+            706: [False, [], 2, [1, 2, 0, 18], 0, "U.Tunnel: Big Room (18/$12) Ending area", [], False, [], [], [], [],
+                  [], [], [], []],
+            49: [False, [], 2, [1, 2, 0, 19], 0, "U.Tunnel: Exit (19/$13)", [], True, [], [], [], [], [], [], [], []],
 
             # Itory
-            50: [False, [10],     1, [1,3,0,21], 0, "Itory: Entrance", [9], False, [], [], [], [], [], [], [], []],
-            51: [False, [50],     1, [1,3,0,21], 0, "Itory: Main Area", [], False, [], [], [], [], [], [], [], []],
-            52: [False, [],       1, [1,3,0,21], 0, "Itory: Lilly's Back Porch", [], False, [], [], [], [], [], [], [], []],
-            53: [False, [],       2, [1,3,0,22], 0, "Itory: West House", [], False, [], [], [], [], [], [], [], []],
-            54: [False, [],       2, [1,3,0,24], 0, "Itory: North House", [], False, [], [], [], [], [], [], [], []],
-            55: [False, [],       2, [1,3,0,23], 0, "Itory: Lilly's House", [23], False, [], [], [], [], [], [], [], []],
-            56: [False, [],       2, [1,3,0,25], 0, "Itory: Cave (entrance)", [], False, [], [], [], [], [], [], [], []],
-            58: [False, [],       2, [1,3,0,25], 0, "Itory: Cave (secret room)", [], False, [], [], [], [], [], [], [], []],
+            50: [False, [10], 1, [1, 3, 0, 21], 0, "Itory: Entrance", [9], False, [], [], [], [], [], [], [], []],
+            51: [False, [50], 1, [1, 3, 0, 21], 0, "Itory: Main Area", [], False, [], [], [], [], [], [], [], []],
+            52: [False, [], 1, [1, 3, 0, 21], 0, "Itory: Lilly's Back Porch", [], False, [], [], [], [], [], [], [],
+                 []],
+            53: [False, [], 2, [1, 3, 0, 22], 0, "Itory: West House", [], False, [], [], [], [], [], [], [], []],
+            54: [False, [], 2, [1, 3, 0, 24], 0, "Itory: North House", [], False, [], [], [], [], [], [], [], []],
+            55: [False, [], 2, [1, 3, 0, 23], 0, "Itory: Lilly's House", [23], False, [], [], [], [], [], [], [], []],
+            56: [False, [], 2, [1, 3, 0, 25], 0, "Itory: Cave (entrance)", [], False, [], [], [], [], [], [], [], []],
+            58: [False, [], 2, [1, 3, 0, 25], 0, "Itory: Cave (secret room)", [], False, [], [], [], [], [], [], [],
+                 []],
 
             # Moon Tribe / Inca Entrance
-            60: [False, [10],     1, [1,4,0,26], 0, "Moon Tribe: Main Area", [25], True, [], [], [], [], [], [], [], []],
-            61: [False, [],       2, [1,4,0,27], 0, "Moon Tribe: Cave", [], False, [], [], [], [], [], [], [], []],
-            62: [False, [61],     2, [1,4,0,27], 0, "Moon Tribe: Cave (Pedestal)", [], False, [], [], [], [], [], [], [], []],
-            63: [False, [10],     1, [1,5,0,28], 0, "Inca: Entrance", [], False, [], [], [], [], [], [], [], []],
-            64: [False, [60,502], 0, [1,4,0,26], 0, "Moon Tribe: Spirits Awake", [], False, [], [], [], [], [], [], [], []],
+            60: [False, [10], 1, [1, 4, 0, 26], 0, "Moon Tribe: Main Area", [25], True, [], [], [], [], [], [], [], []],
+            61: [False, [], 2, [1, 4, 0, 27], 0, "Moon Tribe: Cave", [], False, [], [], [], [], [], [], [], []],
+            62: [False, [61], 2, [1, 4, 0, 27], 0, "Moon Tribe: Cave (Pedestal)", [], False, [], [], [], [], [], [], [],
+                 []],
+            63: [False, [10], 1, [1, 5, 0, 28], 0, "Inca: Entrance", [], False, [], [], [], [], [], [], [], []],
+            64: [False, [60, 502], 0, [1, 4, 0, 26], 0, "Moon Tribe: Spirits Awake", [], False, [], [], [], [], [], [],
+                 [], []],
 
             # Inca Ruins
-            70: [False, [],       2, [1,5,0,29], 0, "Inca: Exterior (29/$1d) NE", [], False, [], [], [], [], [], [], [], []],
-            71: [False, [],       2, [1,5,0,29], 0, "Inca: Exterior (29/$1d) NW", [], False, [], [], [], [], [], [], [], []],
-            72: [False, [73],     2, [1,5,0,29], 0, "Inca: Exterior (29/$1d) N", [], False, [], [], [], [], [], [], [], []],
-            73: [False, [],       2, [1,5,0,29], 0, "Inca: Exterior (29/$1d) Center", [], False, [], [], [], [], [], [], [], []],
-            74: [False, [700],    2, [1,5,0,29], 0, "Inca: Exterior (29/$1d) W", [], False, [], [], [], [], [], [], [], []],
-            700: [False, [],      2, [1,5,0,29], 0, "Inca: Exterior (29/$1d) W 4-Way with orb", [], False, [], [], [], [], [], [], [], []],
-            75: [False, [99],     2, [1,5,0,29], 0, "Inca: Exterior (29/$1d) S", [], False, [], [], [], [], [], [], [], []],
-            76: [False, [],       2, [1,5,0,29], 0, "Inca: Exterior (29/$1d) statue head", [], False, [], [], [], [], [], [], [], []],
-            77: [False, [],       2, [1,5,0,30], 0, "Inca: Outside Castoth (30/$1e) E", [3, 4], False, [], [], [], [], [], [], [], []],
-            78: [False, [77],     2, [1,5,0,30], 0, "Inca: Outside Castoth (30/$1e) W", [], False, [], [], [], [], [], [], [], []],
-            79: [False, [],       2, [1,5,0,31], 0, "Inca: Statue Puzzle (31/$1f) Main", [], False, [], [], [], [], [], [], [], []],
-            69: [False, [],       2, [1,5,0,31], 0, "Inca: Statue Puzzle (31/$1f) U-turn", [], False, [], [], [], [], [], [], [], []],
-            80: [False, [],       2, [1,5,0,32], 0, "Inca: Will Slugs (32/$20) S", [], False, [], [], [], [], [], [], [], []],
-            81: [False, [],       2, [1,5,0,32], 0, "Inca: Will Slugs (32/$20) N", [], False, [], [], [], [], [], [], [], []],
-            82: [False, [],       2, [1,5,0,33], 0, "Inca: Water Room (33/$21) N", [], False, [], [], [], [], [], [], [], []],
-            83: [False, [82],     2, [1,5,0,33], 0, "Inca: Water Room (33/$21) S", [], False, [], [], [], [], [], [], [], []],
-            84: [False, [],       2, [1,5,0,34], 0, "Inca: Big Room (34/$22)", [], False, [], [], [], [], [], [], [], []],
-            85: [False, [],       2, [1,5,0,35], 0, "Inca: E/W Freedan (35/$23) E", [], False, [], [], [], [], [], [], [], []],
-            707: [False, [],      2, [1,5,0,35], 0, "Inca: E/W Freedan (35/$23) Whirligig", [], False, [], [], [], [], [], [], [], []],
-            86: [False, [85],     2, [1,5,0,35], 0, "Inca: E/W Freedan (35/$23) W", [], False, [], [], [], [], [], [], [], []],
-            87: [False, [],       2, [1,5,0,36], 0, "Inca: Golden Tile room (36/$24)", [8], False, [], [], [], [], [], [], [], []],
-            89: [False, [],       2, [1,5,0,37], 0, "Inca: Diamond Block room (37/$25)", [7], False, [], [], [], [], [], [], [], []],
-            91: [False, [],       2, [1,5,0,38], 0, "Inca: Divided Room (38/$26) S", [], False, [], [], [], [], [], [], [], []],
-            92: [False, [91],     2, [1,5,0,38], 0, "Inca: Divided Room (38/$26) S Chest", [], False, [], [], [], [], [], [], [], []],
-            93: [False, [],       2, [1,5,0,38], 0, "Inca: Divided Room (38/$26) N", [], False, [], [], [], [], [], [], [], []],
-            94: [False, [],       2, [1,5,0,39], 0, "Inca: West of DBlock (39/$27)", [], False, [], [], [], [], [], [], [], []],
-            95: [False, [],       2, [1,5,0,40], 0, "Inca: DS Spike Hall (40/$28) E", [], False, [], [], [], [], [], [], [], []],
-            96: [False, [],       2, [1,5,0,40], 0, "Inca: DS Spike Hall (40/$28) SW", [], False, [], [], [], [], [], [], [], []],
-            97: [False, [],       2, [1,5,0,41], 0, "Inca: Boss Room", [], False, [], [], [], [], [], [], [], []],
-            98: [False, [97],     2, [1,5,0,41], 0, "Inca: Behind Boss Room", [], True, [], [], [], [], [], [], [], []],
-            99: [False, [],       2, [1,5,0,29], 0, "Inca: (29/$1d) SE door", [], False, [], [], [], [], [], [], [], []],
+            70: [False, [], 2, [1, 5, 0, 29], 0, "Inca: Exterior (29/$1d) NE", [], False, [], [], [], [], [], [], [],
+                 []],
+            71: [False, [], 2, [1, 5, 0, 29], 0, "Inca: Exterior (29/$1d) NW", [], False, [], [], [], [], [], [], [],
+                 []],
+            72: [False, [73], 2, [1, 5, 0, 29], 0, "Inca: Exterior (29/$1d) N", [], False, [], [], [], [], [], [], [],
+                 []],
+            73: [False, [], 2, [1, 5, 0, 29], 0, "Inca: Exterior (29/$1d) Center", [], False, [], [], [], [], [], [],
+                 [], []],
+            74: [False, [700], 2, [1, 5, 0, 29], 0, "Inca: Exterior (29/$1d) W", [], False, [], [], [], [], [], [], [],
+                 []],
+            700: [False, [], 2, [1, 5, 0, 29], 0, "Inca: Exterior (29/$1d) W 4-Way with orb", [], False, [], [], [], [],
+                  [], [], [], []],
+            75: [False, [99], 2, [1, 5, 0, 29], 0, "Inca: Exterior (29/$1d) S", [], False, [], [], [], [], [], [], [],
+                 []],
+            76: [False, [], 2, [1, 5, 0, 29], 0, "Inca: Exterior (29/$1d) statue head", [], False, [], [], [], [], [],
+                 [], [], []],
+            77: [False, [], 2, [1, 5, 0, 30], 0, "Inca: Outside Castoth (30/$1e) E", [3, 4], False, [], [], [], [], [],
+                 [], [], []],
+            78: [False, [77], 2, [1, 5, 0, 30], 0, "Inca: Outside Castoth (30/$1e) W", [], False, [], [], [], [], [],
+                 [], [], []],
+            79: [False, [], 2, [1, 5, 0, 31], 0, "Inca: Statue Puzzle (31/$1f) Main", [], False, [], [], [], [], [], [],
+                 [], []],
+            69: [False, [], 2, [1, 5, 0, 31], 0, "Inca: Statue Puzzle (31/$1f) U-turn", [], False, [], [], [], [], [],
+                 [], [], []],
+            80: [False, [], 2, [1, 5, 0, 32], 0, "Inca: Will Slugs (32/$20) S", [], False, [], [], [], [], [], [], [],
+                 []],
+            81: [False, [], 2, [1, 5, 0, 32], 0, "Inca: Will Slugs (32/$20) N", [], False, [], [], [], [], [], [], [],
+                 []],
+            82: [False, [], 2, [1, 5, 0, 33], 0, "Inca: Water Room (33/$21) N", [], False, [], [], [], [], [], [], [],
+                 []],
+            83: [False, [82], 2, [1, 5, 0, 33], 0, "Inca: Water Room (33/$21) S", [], False, [], [], [], [], [], [], [],
+                 []],
+            84: [False, [], 2, [1, 5, 0, 34], 0, "Inca: Big Room (34/$22)", [], False, [], [], [], [], [], [], [], []],
+            85: [False, [], 2, [1, 5, 0, 35], 0, "Inca: E/W Freedan (35/$23) E", [], False, [], [], [], [], [], [], [],
+                 []],
+            707: [False, [], 2, [1, 5, 0, 35], 0, "Inca: E/W Freedan (35/$23) Whirligig", [], False, [], [], [], [], [],
+                  [], [], []],
+            86: [False, [85], 2, [1, 5, 0, 35], 0, "Inca: E/W Freedan (35/$23) W", [], False, [], [], [], [], [], [],
+                 [], []],
+            87: [False, [], 2, [1, 5, 0, 36], 0, "Inca: Golden Tile room (36/$24)", [8], False, [], [], [], [], [], [],
+                 [], []],
+            89: [False, [], 2, [1, 5, 0, 37], 0, "Inca: Diamond Block room (37/$25)", [7], False, [], [], [], [], [],
+                 [], [], []],
+            91: [False, [], 2, [1, 5, 0, 38], 0, "Inca: Divided Room (38/$26) S", [], False, [], [], [], [], [], [], [],
+                 []],
+            92: [False, [91], 2, [1, 5, 0, 38], 0, "Inca: Divided Room (38/$26) S Chest", [], False, [], [], [], [], [],
+                 [], [], []],
+            93: [False, [], 2, [1, 5, 0, 38], 0, "Inca: Divided Room (38/$26) N", [], False, [], [], [], [], [], [], [],
+                 []],
+            94: [False, [], 2, [1, 5, 0, 39], 0, "Inca: West of DBlock (39/$27)", [], False, [], [], [], [], [], [], [],
+                 []],
+            95: [False, [], 2, [1, 5, 0, 40], 0, "Inca: DS Spike Hall (40/$28) E", [], False, [], [], [], [], [], [],
+                 [], []],
+            96: [False, [], 2, [1, 5, 0, 40], 0, "Inca: DS Spike Hall (40/$28) SW", [], False, [], [], [], [], [], [],
+                 [], []],
+            97: [False, [], 2, [1, 5, 0, 41], 0, "Inca: Boss Room", [], False, [], [], [], [], [], [], [], []],
+            98: [False, [97], 2, [1, 5, 0, 41], 0, "Inca: Behind Boss Room", [], True, [], [], [], [], [], [], [], []],
+            99: [False, [], 2, [1, 5, 0, 29], 0, "Inca: (29/$1d) SE door", [], False, [], [], [], [], [], [], [], []],
 
             # Gold Ship / Diamond Coast
-            100: [False, [104], 1, [1,5,0,44], 0, "Gold Ship: Deck", [], False, [], [], [], [], [], [], [], []],
-            101: [False, [],    2, [1,5,0,46], 0, "Gold Ship: Interior", [], False, [], [], [], [], [], [], [], []],
-            102: [False, [11],  1, [2,6,0,48], 0, "Diamond Coast: Main Area", [], False, [], [], [], [], [], [], [], []],
-            103: [False, [],    2, [2,6,0,49], 0, "Diamond Coast: House", [], False, [], [], [], [], [], [], [], []],
-            104: [False, [],    0, [1,5,0,44], 0, "Gold Ship: Crow's Nest Passage", [], False, [], [], [], [], [], [], [], []],
+            100: [False, [104], 1, [1, 5, 0, 44], 0, "Gold Ship: Deck", [], False, [], [], [], [], [], [], [], []],
+            101: [False, [], 2, [1, 5, 0, 46], 0, "Gold Ship: Interior", [], False, [], [], [], [], [], [], [], []],
+            102: [False, [11], 1, [2, 6, 0, 48], 0, "Diamond Coast: Main Area", [], False, [], [], [], [], [], [], [],
+                  []],
+            103: [False, [], 2, [2, 6, 0, 49], 0, "Diamond Coast: House", [], False, [], [], [], [], [], [], [], []],
+            104: [False, [], 0, [1, 5, 0, 44], 0, "Gold Ship: Crow's Nest Passage", [], False, [], [], [], [], [], [],
+                  [], []],
 
             # Freejia
-            110: [False, [11],       1, [2,7,0,50], 0, "Freejia: Main Area", [], False, [], [], [], [], [], [], [], []],
-            111: [False, [1, 110],   3, [2,7,0,50], 0, "Freejia: 2-story House Roof", [], False, [], [], [], [], [], [], [], []],
-            112: [False, [],         1, [2,7,0,50], 0, "Freejia: Laborer House Roof", [], False, [], [], [], [], [], [], [], []],
-            113: [False, [110, 114], 3, [2,7,0,50], 0, "Freejia: Labor Trade Roof", [], False, [], [], [], [], [], [], [], []],
-            114: [False, [110, 112], 1, [2,7,0,50], 0, "Freejia: Back Alley", [], False, [], [], [], [], [], [], [], []],
-            116: [False, [],         2, [2,7,0,54], 0, "Freejia: West House", [], False, [], [], [], [], [], [], [], []],
-            117: [False, [],         2, [2,7,0,55], 0, "Freejia: 2-story House", [], False, [], [], [], [], [], [], [], []],
-            118: [False, [],         2, [2,7,0,56], 0, "Freejia: Lovers' House", [], False, [], [], [], [], [], [], [], []],
-            119: [False, [],         2, [2,7,0,57], 0, "Freejia: Hotel (common area)", [], False, [], [], [], [], [], [], [], []],
-            120: [False, [],         2, [2,7,0,57], 0, "Freejia: Hotel (west room)", [], False, [], [], [], [], [], [], [], []],
-            121: [False, [],         2, [2,7,0,57], 0, "Freejia: Hotel (east room)", [], False, [], [], [], [], [], [], [], []],
-            122: [False, [],         2, [2,7,0,58], 0, "Freejia: Laborer House", [], False, [], [], [], [], [], [], [], []],
-            123: [False, [],         2, [2,7,0,59], 0, "Freejia: Messy House", [], False, [], [], [], [], [], [], [], []],
-            124: [False, [],         2, [2,7,0,51], 0, "Freejia: Erik House", [], False, [], [], [], [], [], [], [], []],
-            125: [False, [],         2, [2,7,0,52], 0, "Freejia: Dark Space House", [], False, [], [], [], [], [], [], [], []],
-            126: [False, [],         2, [2,7,0,53], 0, "Freejia: Labor Trade House", [], False, [], [], [], [], [], [], [], []],
-            127: [False, [],         2, [2,7,0,60], 0, "Freejia: Labor Market", [], False, [], [], [], [], [], [], [], []],
+            110: [False, [11], 1, [2, 7, 0, 50], 0, "Freejia: Main Area", [], False, [], [], [], [], [], [], [], []],
+            111: [False, [1, 110], 3, [2, 7, 0, 50], 0, "Freejia: 2-story House Roof", [], False, [], [], [], [], [],
+                  [], [], []],
+            112: [False, [], 1, [2, 7, 0, 50], 0, "Freejia: Laborer House Roof", [], False, [], [], [], [], [], [], [],
+                  []],
+            113: [False, [110, 114], 3, [2, 7, 0, 50], 0, "Freejia: Labor Trade Roof", [], False, [], [], [], [], [],
+                  [], [], []],
+            114: [False, [110, 112], 1, [2, 7, 0, 50], 0, "Freejia: Back Alley", [], False, [], [], [], [], [], [], [],
+                  []],
+            116: [False, [], 2, [2, 7, 0, 54], 0, "Freejia: West House", [], False, [], [], [], [], [], [], [], []],
+            117: [False, [], 2, [2, 7, 0, 55], 0, "Freejia: 2-story House", [], False, [], [], [], [], [], [], [], []],
+            118: [False, [], 2, [2, 7, 0, 56], 0, "Freejia: Lovers' House", [], False, [], [], [], [], [], [], [], []],
+            119: [False, [], 2, [2, 7, 0, 57], 0, "Freejia: Hotel (common area)", [], False, [], [], [], [], [], [], [],
+                  []],
+            120: [False, [], 2, [2, 7, 0, 57], 0, "Freejia: Hotel (west room)", [], False, [], [], [], [], [], [], [],
+                  []],
+            121: [False, [], 2, [2, 7, 0, 57], 0, "Freejia: Hotel (east room)", [], False, [], [], [], [], [], [], [],
+                  []],
+            122: [False, [], 2, [2, 7, 0, 58], 0, "Freejia: Laborer House", [], False, [], [], [], [], [], [], [], []],
+            123: [False, [], 2, [2, 7, 0, 59], 0, "Freejia: Messy House", [], False, [], [], [], [], [], [], [], []],
+            124: [False, [], 2, [2, 7, 0, 51], 0, "Freejia: Erik House", [], False, [], [], [], [], [], [], [], []],
+            125: [False, [], 2, [2, 7, 0, 52], 0, "Freejia: Dark Space House", [], False, [], [], [], [], [], [], [],
+                  []],
+            126: [False, [], 2, [2, 7, 0, 53], 0, "Freejia: Labor Trade House", [], False, [], [], [], [], [], [], [],
+                  []],
+            127: [False, [], 2, [2, 7, 0, 60], 0, "Freejia: Labor Market", [], False, [], [], [], [], [], [], [], []],
 
             # Diamond Mine
-            130: [False, [],    2,     [2,8,0,61], 0, "D.Mine: Tunnel (61/$3d) S", [], False, [], [], [], [], [], [], [], []],
-            708: [False, [701], 2,     [2,8,0,61], 0, "D.Mine: Tunnel (61/$3d) Between Fences 1/2", [], False, [], [], [], [], [], [], [], []],
-            701: [False, [],    2,     [2,8,0,61], 0, "D.Mine: Tunnel (61/$3d) Lizard with orb", [], False, [], [], [], [], [], [], [], []],
-            709: [False, [],    2,     [2,8,0,61], 0, "D.Mine: Tunnel (61/$3d) Between Fences 2/3", [], False, [], [], [], [], [], [], [], []],
-            131: [False, [],    2,     [2,8,0,61], 0, "D.Mine: Tunnel (61/$3d) N", [], False, [], [], [], [], [], [], [], []],
-            133: [False, [11],  2,     [2,8,0,62], 0, "D.Mine: Entrance (62/$3e)", [], False, [], [], [], [], [], [], [], []],
-            134: [False, [],    2,     [2,8,0,63], 0, "D.Mine: Big Room (63/$3f)", [], False, [], [], [], [], [], [], [], []],
-            136: [False, [],    2,     [2,8,0,64], 0, "D.Mine: Cave-In Room (64/$40) Main", [], False, [], [], [], [], [], [], [], []],
-            721: [False, [],    2,     [2,8,0,64], 0, "D.Mine: Cave-In Room (64/$40) Dark Space", [], False, [], [], [], [], [], [], [], []],
-            138: [False, [],    2,     [2,8,0,65], 0, "D.Mine: Friar Worm Room (65/$41) Main", [], False, [], [], [], [], [], [], [], []],
-            710: [False, [],    2,     [2,8,0,65], 0, "D.Mine: Friar Worm Room (65/$41) Worm", [], False, [], [], [], [], [], [], [], []],
-            139: [False, [138,710], 2, [2,8,0,65], 0, "D.Mine: Friar Worm Room (65/$41) Above Ramp", [], False, [], [], [], [], [], [], [], []],
-            140: [False, [],    2,     [2,8,0,66], 0, "D.Mine: Caverns (66/$42) Elevator 1", [], False, [], [], [], [], [], [], [], []],
-            141: [False, [],    2,     [2,8,0,66], 0, "D.Mine: Caverns (66/$42) Elevator 2", [], False, [], [], [], [], [], [], [], []],
-            142: [False, [],    2,     [2,8,0,66], 0, "D.Mine: Caverns (66/$42) Dark Space", [], False, [], [], [], [], [], [], [], []],
-            143: [False, [],    2,     [2,8,0,66], 0, "D.Mine: Caverns (66/$42) Slave", [], False, [], [], [], [], [], [], [], []],
-            144: [False, [145], 2,     [2,8,0,67], 0, "D.Mine: Chairlift (67/$43) E", [], False, [], [], [], [], [], [], [], []],
-            145: [False, [144], 2,     [2,8,0,67], 0, "D.Mine: Chairlift (67/$43) W", [], False, [], [], [], [], [], [], [], []],
-            146: [False, [],    2,     [2,8,0,68], 0, "D.Mine: End Branch (68/$44)", [], False, [], [], [], [], [], [], [], []],
-            148: [False, [],    2,     [2,8,0,69], 0, "D.Mine: End Morgue (69/$45)", [], False, [], [], [], [], [], [], [], []],
-            149: [False, [],    2,     [2,8,0,70], 0, "D.Mine: End East Room (70/$46)", [], False, [], [], [], [], [], [], [], []],
-            150: [False, [],    2,     [2,8,0,71], 0, "D.Mine: Sam (71/$47)", [], False, [], [], [], [], [], [], [], []],
+            130: [False, [], 2, [2, 8, 0, 61], 0, "D.Mine: Tunnel (61/$3d) S", [], False, [], [], [], [], [], [], [],
+                  []],
+            708: [False, [701], 2, [2, 8, 0, 61], 0, "D.Mine: Tunnel (61/$3d) Between Fences 1/2", [], False, [], [],
+                  [], [], [], [], [], []],
+            701: [False, [], 2, [2, 8, 0, 61], 0, "D.Mine: Tunnel (61/$3d) Lizard with orb", [], False, [], [], [], [],
+                  [], [], [], []],
+            709: [False, [], 2, [2, 8, 0, 61], 0, "D.Mine: Tunnel (61/$3d) Between Fences 2/3", [], False, [], [], [],
+                  [], [], [], [], []],
+            131: [False, [], 2, [2, 8, 0, 61], 0, "D.Mine: Tunnel (61/$3d) N", [], False, [], [], [], [], [], [], [],
+                  []],
+            133: [False, [11], 2, [2, 8, 0, 62], 0, "D.Mine: Entrance (62/$3e)", [], False, [], [], [], [], [], [], [],
+                  []],
+            134: [False, [], 2, [2, 8, 0, 63], 0, "D.Mine: Big Room (63/$3f)", [], False, [], [], [], [], [], [], [],
+                  []],
+            136: [False, [], 2, [2, 8, 0, 64], 0, "D.Mine: Cave-In Room (64/$40) Main", [], False, [], [], [], [], [],
+                  [], [], []],
+            721: [False, [], 2, [2, 8, 0, 64], 0, "D.Mine: Cave-In Room (64/$40) Dark Space", [], False, [], [], [], [],
+                  [], [], [], []],
+            138: [False, [], 2, [2, 8, 0, 65], 0, "D.Mine: Friar Worm Room (65/$41) Main", [], False, [], [], [], [],
+                  [], [], [], []],
+            710: [False, [], 2, [2, 8, 0, 65], 0, "D.Mine: Friar Worm Room (65/$41) Worm", [], False, [], [], [], [],
+                  [], [], [], []],
+            139: [False, [138, 710], 2, [2, 8, 0, 65], 0, "D.Mine: Friar Worm Room (65/$41) Above Ramp", [], False, [],
+                  [], [], [], [], [], [], []],
+            140: [False, [], 2, [2, 8, 0, 66], 0, "D.Mine: Caverns (66/$42) Elevator 1", [], False, [], [], [], [], [],
+                  [], [], []],
+            141: [False, [], 2, [2, 8, 0, 66], 0, "D.Mine: Caverns (66/$42) Elevator 2", [], False, [], [], [], [], [],
+                  [], [], []],
+            142: [False, [], 2, [2, 8, 0, 66], 0, "D.Mine: Caverns (66/$42) Dark Space", [], False, [], [], [], [], [],
+                  [], [], []],
+            143: [False, [], 2, [2, 8, 0, 66], 0, "D.Mine: Caverns (66/$42) Slave", [], False, [], [], [], [], [], [],
+                  [], []],
+            144: [False, [145], 2, [2, 8, 0, 67], 0, "D.Mine: Chairlift (67/$43) E", [], False, [], [], [], [], [], [],
+                  [], []],
+            145: [False, [144], 2, [2, 8, 0, 67], 0, "D.Mine: Chairlift (67/$43) W", [], False, [], [], [], [], [], [],
+                  [], []],
+            146: [False, [], 2, [2, 8, 0, 68], 0, "D.Mine: End Branch (68/$44)", [], False, [], [], [], [], [], [], [],
+                  []],
+            148: [False, [], 2, [2, 8, 0, 69], 0, "D.Mine: End Morgue (69/$45)", [], False, [], [], [], [], [], [], [],
+                  []],
+            149: [False, [], 2, [2, 8, 0, 70], 0, "D.Mine: End East Room (70/$46)", [], False, [], [], [], [], [], [],
+                  [], []],
+            150: [False, [], 2, [2, 8, 0, 71], 0, "D.Mine: Sam (71/$47)", [], False, [], [], [], [], [], [], [], []],
 
             # Neil's Cottage / Nazca
-            160: [False, [11],         2, [2,9,0,73],  0, "Neil's Cottage", [13], False, [], [], [], [], [], [], [], []],
-            161: [False, [17,160,505], 2, [2,9,0,73],  0, "Neil's Cottage: Neil", [], False, [], [], [], [], [], [], [], []],
-            162: [False, [11],         1, [2,10,0,75], 0, "Nazca Plain", [], False, [], [], [], [], [], [], [], []],
+            160: [False, [11], 2, [2, 9, 0, 73], 0, "Neil's Cottage", [13], False, [], [], [], [], [], [], [], []],
+            161: [False, [17, 160, 505], 2, [2, 9, 0, 73], 0, "Neil's Cottage: Neil", [], False, [], [], [], [], [], [],
+                  [], []],
+            162: [False, [11], 1, [2, 10, 0, 75], 0, "Nazca Plain", [], False, [], [], [], [], [], [], [], []],
 
             # Sky Garden
-            167: [False, [],         2, [2,10,0,83], 0, "Sky Garden: NW Top (83/$53) SE below chests", [], False, [], [], [], [], [], [], [], []],
-            168: [False, [],         2, [2,10,0,81], 0, "Sky Garden: SW Top (81/$51) N of pegs", [], False, [], [], [], [], [], [], [], []],
-            169: [False, [],         2, [2,10,0,86], 0, "Sky Garden: DS room (86/$56)", [], False, [], [], [], [], [], [], [], []],
-            170: [False, [],         1, [2,10,0,76], 0, "Sky Garden: Foyer (76/$4c) Main", [14, 14, 14, 14], False, [], [], [], [], [], [], [], []],
-            171: [False, [],         1, [2,10,0,76], 0, "Sky Garden: Foyer (76/$4c) Boss Door", [], False, [], [], [], [], [], [], [], []],
-            172: [False, [],         2, [2,10,0,77], 0, "Sky Garden: NE Top (77/$4d) Main", [], False, [], [], [], [], [], [], [], []],
-            173: [False, [],         2, [2,10,0,77], 0, "Sky Garden: NE Top (77/$4d) SW Chest", [], False, [], [], [], [], [], [], [], []],
-            174: [False, [],         2, [2,10,0,77], 0, "Sky Garden: NE Top (77/$4d) SE Chest", [], False, [], [], [], [], [], [], [], []],
-            175: [False, [],         2, [2,10,0,78], 0, "Sky Garden: NE Bot (78/$4e)", [], False, [], [], [], [], [], [], [], []],
-            176: [False, [],         2, [2,10,0,79], 0, "Sky Garden: SE Top (79/$4f) Main", [], False, [], [], [], [], [], [], [], []],
-            177: [False, [],         2, [2,10,0,79], 0, "Sky Garden: SE Top (79/$4f) N before robot", [], False, [], [], [], [], [], [], [], []],
-            711: [False, [],         2, [2,10,0,79], 0, "Sky Garden: SE Top (79/$4f) Robot for barrier", [], False, [], [], [], [], [], [], [], []],
-            178: [False, [],         2, [2,10,0,79], 0, "Sky Garden: SE Top (79/$4f) Behind barrier", [], False, [], [], [], [], [], [], [], []],
-            179: [False, [],         2, [2,10,0,80], 0, "Sky Garden: SE Bot (80/$50) N corridor", [], False, [], [], [], [], [], [], [], []],
-            180: [False, [],         2, [2,10,0,80], 0, "Sky Garden: SE Bot (80/$50) S main", [], False, [], [], [], [], [], [], [], []],
-            716: [False, [],         2, [2,10,0,80], 0, "Sky Garden: SE Bot (80/$50) S chest behind barrier", [], False, [], [], [], [], [], [], [], []],
-            181: [False, [],         2, [2,10,0,81], 0, "Sky Garden: SW Top (81/$51) Main", [], False, [], [], [], [], [], [], [], []],
-            182: [False, [181],      2, [2,10,0,81], 0, "Sky Garden: SW Top (81/$51) West", [], False, [], [], [], [], [], [], [], []],
-            183: [False, [],         2, [2,10,0,81], 0, "Sky Garden: SW Top (81/$51) Dark Space cage", [], False, [], [], [], [], [], [], [], []],
-            184: [False, [182],      2, [2,10,0,81], 0, "Sky Garden: SW Top (81/$51) SE platform", [], False, [], [], [], [], [], [], [], []],
-            185: [False, [182],      2, [2,10,0,81], 0, "Sky Garden: SW Top (81/$51) SW chest", [], False, [], [], [], [], [], [], [], []],
-            186: [False, [],         2, [2,10,0,82], 0, "Sky Garden: SW Bot (82/$52) N with chest", [], False, [], [], [], [], [], [], [], []],
-            187: [False, [],         2, [2,10,0,82], 0, "Sky Garden: SW Bot (82/$52) S before statue", [], False, [], [], [], [], [], [], [], []],
-            188: [False, [],         2, [2,10,0,82], 0, "Sky Garden: SW Bot (82/$52) NE before switch", [], False, [], [], [], [], [], [], [], []],
-            189: [False, [188],      2, [2,10,0,82], 0, "Sky Garden: SW Bot (82/$52) NE switch in cage", [], False, [], [], [], [], [], [], [], []],
-            190: [False, [191],      2, [2,10,0,83], 0, "Sky Garden: NW Top (83/$53) NE side", [], False, [], [], [], [], [], [], [], []],
-            191: [False, [190,192],  2, [2,10,0,83], 0, "Sky Garden: NW Top (83/$53) NW side", [], False, [], [], [], [], [], [], [], []],
-            192: [False, [],         2, [2,10,0,83], 0, "Sky Garden: NW Top (83/$53) C with ramp", [], False, [], [], [], [], [], [], [], []],
-            193: [False, [194],      2, [2,10,0,83], 0, "Sky Garden: NW Top (83/$53) SW before chests", [], False, [], [], [], [], [], [], [], []],
-            194: [False, [167],      2, [2,10,0,83], 0, "Sky Garden: NW Top (83/$53) Chests", [], False, [], [], [], [], [], [], [], []],
-            195: [False, [196],      2, [2,10,0,84], 0, "Sky Garden: NW Bot (84/$54) Main", [], False, [], [], [], [], [], [], [], []],
-            196: [False, [],         2, [2,10,0,84], 0, "Sky Garden: NW Bot (84/$54) NE below ledge", [], False, [], [], [], [], [], [], [], []],
-            197: [False, [],         2, [2,10,0,84], 0, "Sky Garden: NW Bot (84/$54) SE behind statue", [], False, [], [], [], [], [], [], [], []],
-            198: [False, [],         2, [2,10,0,85], 0, "Sky Garden: Viper (85/$55)", [], True, [], [], [], [], [], [], [], []],
+            167: [False, [], 2, [2, 10, 0, 83], 0, "Sky Garden: NW Top (83/$53) SE below chests", [], False, [], [], [],
+                  [], [], [], [], []],
+            168: [False, [], 2, [2, 10, 0, 81], 0, "Sky Garden: SW Top (81/$51) N of pegs", [], False, [], [], [], [],
+                  [], [], [], []],
+            169: [False, [], 2, [2, 10, 0, 86], 0, "Sky Garden: DS room (86/$56)", [], False, [], [], [], [], [], [],
+                  [], []],
+            170: [False, [], 1, [2, 10, 0, 76], 0, "Sky Garden: Foyer (76/$4c) Main", [14, 14, 14, 14], False, [], [],
+                  [], [], [], [], [], []],
+            171: [False, [], 1, [2, 10, 0, 76], 0, "Sky Garden: Foyer (76/$4c) Boss Door", [], False, [], [], [], [],
+                  [], [], [], []],
+            172: [False, [], 2, [2, 10, 0, 77], 0, "Sky Garden: NE Top (77/$4d) Main", [], False, [], [], [], [], [],
+                  [], [], []],
+            173: [False, [], 2, [2, 10, 0, 77], 0, "Sky Garden: NE Top (77/$4d) SW Chest", [], False, [], [], [], [],
+                  [], [], [], []],
+            174: [False, [], 2, [2, 10, 0, 77], 0, "Sky Garden: NE Top (77/$4d) SE Chest", [], False, [], [], [], [],
+                  [], [], [], []],
+            175: [False, [], 2, [2, 10, 0, 78], 0, "Sky Garden: NE Bot (78/$4e)", [], False, [], [], [], [], [], [], [],
+                  []],
+            176: [False, [], 2, [2, 10, 0, 79], 0, "Sky Garden: SE Top (79/$4f) Main", [], False, [], [], [], [], [],
+                  [], [], []],
+            177: [False, [], 2, [2, 10, 0, 79], 0, "Sky Garden: SE Top (79/$4f) N before robot", [], False, [], [], [],
+                  [], [], [], [], []],
+            711: [False, [], 2, [2, 10, 0, 79], 0, "Sky Garden: SE Top (79/$4f) Robot for barrier", [], False, [], [],
+                  [], [], [], [], [], []],
+            178: [False, [], 2, [2, 10, 0, 79], 0, "Sky Garden: SE Top (79/$4f) Behind barrier", [], False, [], [], [],
+                  [], [], [], [], []],
+            179: [False, [], 2, [2, 10, 0, 80], 0, "Sky Garden: SE Bot (80/$50) N corridor", [], False, [], [], [], [],
+                  [], [], [], []],
+            180: [False, [], 2, [2, 10, 0, 80], 0, "Sky Garden: SE Bot (80/$50) S main", [], False, [], [], [], [], [],
+                  [], [], []],
+            716: [False, [], 2, [2, 10, 0, 80], 0, "Sky Garden: SE Bot (80/$50) S chest behind barrier", [], False, [],
+                  [], [], [], [], [], [], []],
+            181: [False, [], 2, [2, 10, 0, 81], 0, "Sky Garden: SW Top (81/$51) Main", [], False, [], [], [], [], [],
+                  [], [], []],
+            182: [False, [181], 2, [2, 10, 0, 81], 0, "Sky Garden: SW Top (81/$51) West", [], False, [], [], [], [], [],
+                  [], [], []],
+            183: [False, [], 2, [2, 10, 0, 81], 0, "Sky Garden: SW Top (81/$51) Dark Space cage", [], False, [], [], [],
+                  [], [], [], [], []],
+            184: [False, [182], 2, [2, 10, 0, 81], 0, "Sky Garden: SW Top (81/$51) SE platform", [], False, [], [], [],
+                  [], [], [], [], []],
+            185: [False, [182], 2, [2, 10, 0, 81], 0, "Sky Garden: SW Top (81/$51) SW chest", [], False, [], [], [], [],
+                  [], [], [], []],
+            186: [False, [], 2, [2, 10, 0, 82], 0, "Sky Garden: SW Bot (82/$52) N with chest", [], False, [], [], [],
+                  [], [], [], [], []],
+            187: [False, [], 2, [2, 10, 0, 82], 0, "Sky Garden: SW Bot (82/$52) S before statue", [], False, [], [], [],
+                  [], [], [], [], []],
+            188: [False, [], 2, [2, 10, 0, 82], 0, "Sky Garden: SW Bot (82/$52) NE before switch", [], False, [], [],
+                  [], [], [], [], [], []],
+            189: [False, [188], 2, [2, 10, 0, 82], 0, "Sky Garden: SW Bot (82/$52) NE switch in cage", [], False, [],
+                  [], [], [], [], [], [], []],
+            190: [False, [191], 2, [2, 10, 0, 83], 0, "Sky Garden: NW Top (83/$53) NE side", [], False, [], [], [], [],
+                  [], [], [], []],
+            191: [False, [190, 192], 2, [2, 10, 0, 83], 0, "Sky Garden: NW Top (83/$53) NW side", [], False, [], [], [],
+                  [], [], [], [], []],
+            192: [False, [], 2, [2, 10, 0, 83], 0, "Sky Garden: NW Top (83/$53) C with ramp", [], False, [], [], [], [],
+                  [], [], [], []],
+            193: [False, [194], 2, [2, 10, 0, 83], 0, "Sky Garden: NW Top (83/$53) SW before chests", [], False, [], [],
+                  [], [], [], [], [], []],
+            194: [False, [167], 2, [2, 10, 0, 83], 0, "Sky Garden: NW Top (83/$53) Chests", [], False, [], [], [], [],
+                  [], [], [], []],
+            195: [False, [196], 2, [2, 10, 0, 84], 0, "Sky Garden: NW Bot (84/$54) Main", [], False, [], [], [], [], [],
+                  [], [], []],
+            196: [False, [], 2, [2, 10, 0, 84], 0, "Sky Garden: NW Bot (84/$54) NE below ledge", [], False, [], [], [],
+                  [], [], [], [], []],
+            197: [False, [], 2, [2, 10, 0, 84], 0, "Sky Garden: NW Bot (84/$54) SE behind statue", [], False, [], [],
+                  [], [], [], [], [], []],
+            198: [False, [], 2, [2, 10, 0, 85], 0, "Sky Garden: Viper (85/$55)", [], True, [], [], [], [], [], [], [],
+                  []],
 
             # Seaside Palace
-            200: [False,    [], 1, [3,11,0,90], 0, "Seaside Palace: Area 1", [16], False, [], [], [], [], [], [], [], []],
-            202: [False,    [], 2, [3,11,0,91], 0, "Seaside Palace: Area 1 NE Room", [], False, [], [], [], [], [], [], [], []],
-            203: [False,    [], 2, [3,11,0,91], 0, "Seaside Palace: Area 1 NW Room", [], False, [], [], [], [], [], [], [], []],
-            204: [False,    [], 2, [3,11,0,91], 0, "Seaside Palace: Area 1 SE Room", [], False, [], [], [], [], [], [], [], []],
-            205: [False,    [], 1, [3,11,0,92], 0, "Seaside Palace: Area 2", [], False, [], [], [], [], [], [], [], []],
-            207: [False,    [], 2, [3,11,0,92], 0, "Seaside Palace: Area 2 SW Room", [], False, [], [], [], [], [], [], [], []],
-            209: [False,    [], 2, [3,11,0,93], 0, "Seaside Palace: Fountain", [17], False, [], [], [], [], [], [], [], []],
-            210: [False,    [], 2, [3,11,0,94], 0, "Seaside Palace: Mu Passage", [16], False, [], [], [], [], [], [], [], []],
-            
+            200: [False, [], 1, [3, 11, 0, 90], 0, "Seaside Palace: Area 1", [16], False, [], [], [], [], [], [], [],
+                  []],
+            202: [False, [], 2, [3, 11, 0, 91], 0, "Seaside Palace: Area 1 NE Room", [], False, [], [], [], [], [], [],
+                  [], []],
+            203: [False, [], 2, [3, 11, 0, 91], 0, "Seaside Palace: Area 1 NW Room", [], False, [], [], [], [], [], [],
+                  [], []],
+            204: [False, [], 2, [3, 11, 0, 91], 0, "Seaside Palace: Area 1 SE Room", [], False, [], [], [], [], [], [],
+                  [], []],
+            205: [False, [], 1, [3, 11, 0, 92], 0, "Seaside Palace: Area 2", [], False, [], [], [], [], [], [], [], []],
+            207: [False, [], 2, [3, 11, 0, 92], 0, "Seaside Palace: Area 2 SW Room", [], False, [], [], [], [], [], [],
+                  [], []],
+            209: [False, [], 2, [3, 11, 0, 93], 0, "Seaside Palace: Fountain", [17], False, [], [], [], [], [], [], [],
+                  []],
+            210: [False, [], 2, [3, 11, 0, 94], 0, "Seaside Palace: Mu Passage", [16], False, [], [], [], [], [], [],
+                  [], []],
+
             # Mu
-            212: [False, [],         2, [3,12,0,95],  0, "Mu: NW (95/$5f) Entrance", [], False, [], [], [], [], [], [], [], []],
-            722: [False, [],         2, [3,12,0,95],  0, "Mu: NW (95/$5f) E of barrier", [], False, [], [], [], [], [], [], [], []],
-            213: [False, [],         2, [3,12,1,95],  0, "Mu: NW (95/$5f) MidE", [], False, [], [], [], [], [], [], [], []],
-            214: [False, [],         2, [3,12,1,95],  0, "Mu: NW (95/$5f) MidW", [], False, [], [], [], [], [], [], [], []],
-            215: [False, [],         2, [3,12,2,95],  0, "Mu: NW (95/$5f) BotE", [], False, [], [], [], [], [], [], [], []],
-            216: [False, [],         2, [3,12,2,95],  0, "Mu: NW (95/$5f) BotW", [], False, [], [], [], [], [], [], [], []],
-            217: [False, [726],      2, [3,12,0,96],  0, "Mu: NE (96/$60) TopN", [], False, [], [], [], [], [], [], [], []],
-            726: [False, [],         2, [3,12,0,96],  0, "Mu: NE (96/$60) Top monster orb N", [], False, [], [], [], [], [], [], [], []],
-            725: [False, [724,726],  2, [3,12,0,96],  0, "Mu: NE (96/$60) Top between rocks", [], False, [], [], [], [], [], [], [], []],
-            724: [False, [],         2, [3,12,0,96],  0, "Mu: NE (96/$60) Top monster orb S", [], False, [], [], [], [], [], [], [], []],
-            723: [False, [724],      2, [3,12,0,96],  0, "Mu: NE (96/$60) TopS", [], False, [], [], [], [], [], [], [], []],
-            218: [False, [],         2, [3,12,1,96],  0, "Mu: NE (96/$60) Mid", [], False, [], [], [], [], [], [], [], []],
-            219: [False, [],         2, [3,12,2,96],  0, "Mu: NE (96/$60) Bot", [], False, [], [], [], [], [], [], [], []],
-            220: [False, [],         2, [3,12,0,97],  0, "Mu: E (97/$61) Top Main", [], False, [], [], [], [], [], [], [], []],
-            221: [False, [222,223],  2, [3,12,0,97],  0, "Mu: E (97/$61) Top Island", [], False, [], [], [], [], [], [], [], []],
-            222: [False, [],         2, [3,12,1,97],  0, "Mu: E (97/$61) MidN", [], False, [], [], [], [], [], [], [], []],
-            223: [False, [221],      2, [3,12,1,97],  0, "Mu: E (97/$61) MidW", [], False, [], [], [], [], [], [], [], []],
-            224: [False, [],         2, [3,12,2,97],  0, "Mu: E (97/$61) Bot", [], False, [], [], [], [], [], [], [], []],
-            225: [False, [],         2, [3,12,0,98],  0, "Mu: W (98/$62) TopS", [], False, [], [], [], [], [], [], [], []],
-            226: [False, [],         2, [3,12,0,98],  0, "Mu: W (98/$62) TopN", [], False, [], [], [], [], [], [], [], []],
-            227: [False, [],         2, [3,12,1,98],  0, "Mu: W (98/$62) MidE", [], False, [], [], [], [], [], [], [], []],
-            229: [False, [],         2, [3,12,2,98],  0, "Mu: W (98/$62) BotE", [], False, [], [], [], [], [], [], [], []],
-            230: [False, [],         2, [3,12,2,98],  0, "Mu: W (98/$62) BotW", [], False, [], [], [], [], [], [], [], []],
-            228: [False, [],         2, [3,12,1,98],  0, "Mu: W (98/$62) MidW", [], False, [], [], [], [], [], [], [], []],
-            231: [False, [526],      2, [3,12,0,99],  0, "Mu: Hope Room 1 (99/$63)", [18], False, [], [], [], [], [], [], [], []],
-            232: [False, [527],      2, [3,12,0,99],  0, "Mu: Hope Room 2 (99/$63)", [18], False, [], [], [], [], [], [], [], []],
-            233: [False, [],         2, [3,12,1,100], 0, "Mu: SW (100/$64) MidE-N", [], False, [], [], [], [], [], [], [], []],
-            245: [False, [],         2, [3,12,1,100], 0, "Mu: SW (100/$64) MidE-S", [], False, [], [], [], [], [], [], [], []],
-            234: [False, [],         2, [3,12,1,100], 0, "Mu: SW (100/$64) MidW", [], False, [], [], [], [], [], [], [], []],
-            235: [False, [],         2, [3,12,2,100], 0, "Mu: SW (100/$64) Bot", [], False, [], [], [], [], [], [], [], []],
-            236: [False, [238],      2, [3,12,0,101], 0, "Mu: SE (101/$65) Top", [], False, [], [], [], [], [], [], [], []],
-            237: [False, [],         2, [3,12,1,101], 0, "Mu: SE (101/$65) MidW", [], False, [], [], [], [], [], [], [], []],
-            238: [False, [236],      2, [3,12,1,101], 0, "Mu: SE (101/$65) MidE", [], False, [], [], [], [], [], [], [], []],
-            239: [False, [],         2, [3,12,2,101], 0, "Mu: SE (101/$65) Bot", [], False, [], [], [], [], [], [], [], []],
-            240: [False, [],         2, [3,12,0,102], 0, "Mu: Rama rooms (102/$66) Pedestal area", [19, 19], False, [], [], [], [], [], [], [], []],
-            241: [False, [],         2, [3,12,0,102], 0, "Mu: Rama rooms (102/$66) Statues Placed", [], False, [], [], [], [], [], [], [], []],
-            242: [False, [],         2, [3,12,0,102], 0, "Mu: Rama rooms (102/$66) Statue-Get", [], True, [], [], [], [], [], [], [], []],
-            243: [False, [244],      2, [3,12,0,103], 0, "Mu: Boss Room (103/$67) Entrance", [], False, [], [], [], [], [], [], [], []],
-            244: [False, [243],      2, [3,12,0,103], 0, "Mu: Boss Room (103/$67) Main", [], False, [], [], [], [], [], [], [], []],
+            212: [False, [], 2, [3, 12, 0, 95], 0, "Mu: NW (95/$5f) Entrance", [], False, [], [], [], [], [], [], [],
+                  []],
+            722: [False, [], 2, [3, 12, 0, 95], 0, "Mu: NW (95/$5f) E of barrier", [], False, [], [], [], [], [], [],
+                  [], []],
+            213: [False, [], 2, [3, 12, 1, 95], 0, "Mu: NW (95/$5f) MidE", [], False, [], [], [], [], [], [], [], []],
+            214: [False, [], 2, [3, 12, 1, 95], 0, "Mu: NW (95/$5f) MidW", [], False, [], [], [], [], [], [], [], []],
+            215: [False, [], 2, [3, 12, 2, 95], 0, "Mu: NW (95/$5f) BotE", [], False, [], [], [], [], [], [], [], []],
+            216: [False, [], 2, [3, 12, 2, 95], 0, "Mu: NW (95/$5f) BotW", [], False, [], [], [], [], [], [], [], []],
+            217: [False, [726], 2, [3, 12, 0, 96], 0, "Mu: NE (96/$60) TopN", [], False, [], [], [], [], [], [], [],
+                  []],
+            726: [False, [], 2, [3, 12, 0, 96], 0, "Mu: NE (96/$60) Top monster orb N", [], False, [], [], [], [], [],
+                  [], [], []],
+            725: [False, [724, 726], 2, [3, 12, 0, 96], 0, "Mu: NE (96/$60) Top between rocks", [], False, [], [], [],
+                  [], [], [], [], []],
+            724: [False, [], 2, [3, 12, 0, 96], 0, "Mu: NE (96/$60) Top monster orb S", [], False, [], [], [], [], [],
+                  [], [], []],
+            723: [False, [724], 2, [3, 12, 0, 96], 0, "Mu: NE (96/$60) TopS", [], False, [], [], [], [], [], [], [],
+                  []],
+            218: [False, [], 2, [3, 12, 1, 96], 0, "Mu: NE (96/$60) Mid", [], False, [], [], [], [], [], [], [], []],
+            219: [False, [], 2, [3, 12, 2, 96], 0, "Mu: NE (96/$60) Bot", [], False, [], [], [], [], [], [], [], []],
+            220: [False, [], 2, [3, 12, 0, 97], 0, "Mu: E (97/$61) Top Main", [], False, [], [], [], [], [], [], [],
+                  []],
+            221: [False, [222, 223], 2, [3, 12, 0, 97], 0, "Mu: E (97/$61) Top Island", [], False, [], [], [], [], [],
+                  [], [], []],
+            222: [False, [], 2, [3, 12, 1, 97], 0, "Mu: E (97/$61) MidN", [], False, [], [], [], [], [], [], [], []],
+            223: [False, [221], 2, [3, 12, 1, 97], 0, "Mu: E (97/$61) MidW", [], False, [], [], [], [], [], [], [], []],
+            224: [False, [], 2, [3, 12, 2, 97], 0, "Mu: E (97/$61) Bot", [], False, [], [], [], [], [], [], [], []],
+            225: [False, [], 2, [3, 12, 0, 98], 0, "Mu: W (98/$62) TopS", [], False, [], [], [], [], [], [], [], []],
+            226: [False, [], 2, [3, 12, 0, 98], 0, "Mu: W (98/$62) TopN", [], False, [], [], [], [], [], [], [], []],
+            227: [False, [], 2, [3, 12, 1, 98], 0, "Mu: W (98/$62) MidE", [], False, [], [], [], [], [], [], [], []],
+            229: [False, [], 2, [3, 12, 2, 98], 0, "Mu: W (98/$62) BotE", [], False, [], [], [], [], [], [], [], []],
+            230: [False, [], 2, [3, 12, 2, 98], 0, "Mu: W (98/$62) BotW", [], False, [], [], [], [], [], [], [], []],
+            228: [False, [], 2, [3, 12, 1, 98], 0, "Mu: W (98/$62) MidW", [], False, [], [], [], [], [], [], [], []],
+            231: [False, [526], 2, [3, 12, 0, 99], 0, "Mu: Hope Room 1 (99/$63)", [18], False, [], [], [], [], [], [],
+                  [], []],
+            232: [False, [527], 2, [3, 12, 0, 99], 0, "Mu: Hope Room 2 (99/$63)", [18], False, [], [], [], [], [], [],
+                  [], []],
+            233: [False, [], 2, [3, 12, 1, 100], 0, "Mu: SW (100/$64) MidE-N", [], False, [], [], [], [], [], [], [],
+                  []],
+            245: [False, [], 2, [3, 12, 1, 100], 0, "Mu: SW (100/$64) MidE-S", [], False, [], [], [], [], [], [], [],
+                  []],
+            234: [False, [], 2, [3, 12, 1, 100], 0, "Mu: SW (100/$64) MidW", [], False, [], [], [], [], [], [], [], []],
+            235: [False, [], 2, [3, 12, 2, 100], 0, "Mu: SW (100/$64) Bot", [], False, [], [], [], [], [], [], [], []],
+            236: [False, [238], 2, [3, 12, 0, 101], 0, "Mu: SE (101/$65) Top", [], False, [], [], [], [], [], [], [],
+                  []],
+            237: [False, [], 2, [3, 12, 1, 101], 0, "Mu: SE (101/$65) MidW", [], False, [], [], [], [], [], [], [], []],
+            238: [False, [236], 2, [3, 12, 1, 101], 0, "Mu: SE (101/$65) MidE", [], False, [], [], [], [], [], [], [],
+                  []],
+            239: [False, [], 2, [3, 12, 2, 101], 0, "Mu: SE (101/$65) Bot", [], False, [], [], [], [], [], [], [], []],
+            240: [False, [], 2, [3, 12, 0, 102], 0, "Mu: Rama rooms (102/$66) Pedestal area", [19, 19], False, [], [],
+                  [], [], [], [], [], []],
+            241: [False, [], 2, [3, 12, 0, 102], 0, "Mu: Rama rooms (102/$66) Statues Placed", [], False, [], [], [],
+                  [], [], [], [], []],
+            242: [False, [], 2, [3, 12, 0, 102], 0, "Mu: Rama rooms (102/$66) Statue-Get", [], True, [], [], [], [], [],
+                  [], [], []],
+            243: [False, [244], 2, [3, 12, 0, 103], 0, "Mu: Boss Room (103/$67) Entrance", [], False, [], [], [], [],
+                  [], [], [], []],
+            244: [False, [243], 2, [3, 12, 0, 103], 0, "Mu: Boss Room (103/$67) Main", [], False, [], [], [], [], [],
+                  [], [], []],
 
             # Angel Village
-            250: [False, [12], 1, [3,13,0,105], 0, "Angel Village: Outside", [], True, [], [], [], [], [], [], [], []],
-            251: [False, [1],  1, [3,13,0,107], 0, "Angel Village: Underground", [], False, [], [], [], [], [], [], [], []],
-            252: [False, [],   2, [3,13,0,108], 0, "Angel Village: Room 1", [], False, [], [], [], [], [], [], [], []],
-            253: [False, [],   2, [3,13,0,108], 0, "Angel Village: Room 2", [], False, [], [], [], [], [], [], [], []],
-            254: [False, [],   2, [3,13,0,108], 0, "Angel Village: Dance Hall", [], False, [], [], [], [], [], [], [], []],
-            255: [False, [],   2, [3,13,0,108], 0, "Angel Village: DS Room", [], False, [], [], [], [], [], [], [], []],
+            250: [False, [12], 1, [3, 13, 0, 105], 0, "Angel Village: Outside", [], True, [], [], [], [], [], [], [],
+                  []],
+            251: [False, [1], 1, [3, 13, 0, 107], 0, "Angel Village: Underground", [], False, [], [], [], [], [], [],
+                  [], []],
+            252: [False, [], 2, [3, 13, 0, 108], 0, "Angel Village: Room 1", [], False, [], [], [], [], [], [], [], []],
+            253: [False, [], 2, [3, 13, 0, 108], 0, "Angel Village: Room 2", [], False, [], [], [], [], [], [], [], []],
+            254: [False, [], 2, [3, 13, 0, 108], 0, "Angel Village: Dance Hall", [], False, [], [], [], [], [], [], [],
+                  []],
+            255: [False, [], 2, [3, 13, 0, 108], 0, "Angel Village: DS Room", [], False, [], [], [], [], [], [], [],
+                  []],
 
             # Angel Dungeon
-            260: [False,    [], 2, [3,13,0,109], 0, "Angel Dungeon: Entrance (109/$6d)", [], False, [], [], [], [], [], [], [], []],
-            261: [False,    [], 2, [3,13,0,110], 0, "Angel Dungeon: Maze (110/$6e) Main", [], False, [], [], [], [], [], [], [], []],
-            278: [False,    [], 2, [3,13,0,110], 0, "Angel Dungeon: Maze (110/$6e) Behind Draco", [], False, [], [], [], [], [], [], [], []],
-            262: [False,    [], 2, [3,13,0,111], 0, "Angel Dungeon: Dark room (111/$6f)", [], False, [], [], [], [], [], [], [], []],
-            259: [False,    [], 2, [3,13,0,112], 0, "Angel Dungeon: Water room (112/$70) Entrance before false wall", [], False, [], [], [], [], [], [], [], []],
-            263: [False,    [], 2, [3,13,0,112], 0, "Angel Dungeon: Water room (112/$70) Main", [], False, [], [], [], [], [], [], [], []],
-            279: [False,    [], 2, [3,13,0,112], 0, "Angel Dungeon: Water room (112/$70) Behind Draco", [], False, [], [], [], [], [], [], [], []],
-            265: [False,    [], 2, [3,13,0,112], 0, "Angel Dungeon: Water room (112/$70) Alcove", [], False, [], [], [], [], [], [], [], []],
-            266: [False,    [], 2, [3,13,0,113], 0, "Angel Dungeon: Wind Tunnel (113/$71)", [], False, [], [], [], [], [], [], [], []],
-            267: [False,    [], 2, [3,13,0,114], 0, "Angel Dungeon: Long Room (114/$72)", [], False, [], [], [], [], [], [], [], []],
-            277: [False,    [], 2, [3,13,0,115], 0, "Angel Dungeon: Ishtar's hall (115/$73) Foyer with slider", [], False, [], [], [], [], [], [], [], []],
-            269: [False,    [], 2, [3,13,0,115], 0, "Angel Dungeon: Ishtar's hall (115/$73) Main with waterfalls", [], False, [], [], [], [], [], [], [], []],
-            270: [False,    [], 2, [3,13,0,116], 0, "Angel Dungeon: Portrait Rooms (116/$74) Kara", [], False, [], [], [], [], [], [], [], []],
-            271: [False,    [], 2, [3,13,0,116], 0, "Angel Dungeon: Portrait Rooms (116/$74) Middle room", [], False, [], [], [], [], [], [], [], []],
-            272: [False,    [], 2, [3,13,0,116], 0, "Angel Dungeon: Portrait Rooms (116/$74) Ishtar's room", [], False, [], [], [], [], [], [], [], []],
-            273: [False,    [], 2, [3,13,0,116], 0, "Angel Dungeon: Portrait Rooms (116/$74) Ishtar chest", [], False, [], [], [], [], [], [], [], []],
-            274: [False,    [], 2, [3,13,0,117], 0, "Angel Dungeon: Puzzle Rooms", [], False, [], [], [], [], [], [], [], []],
+            260: [False, [], 2, [3, 13, 0, 109], 0, "Angel Dungeon: Entrance (109/$6d)", [], False, [], [], [], [], [],
+                  [], [], []],
+            261: [False, [], 2, [3, 13, 0, 110], 0, "Angel Dungeon: Maze (110/$6e) Main", [], False, [], [], [], [], [],
+                  [], [], []],
+            278: [False, [], 2, [3, 13, 0, 110], 0, "Angel Dungeon: Maze (110/$6e) Behind Draco", [], False, [], [], [],
+                  [], [], [], [], []],
+            262: [False, [], 2, [3, 13, 0, 111], 0, "Angel Dungeon: Dark room (111/$6f)", [], False, [], [], [], [], [],
+                  [], [], []],
+            259: [False, [], 2, [3, 13, 0, 112], 0, "Angel Dungeon: Water room (112/$70) Entrance before false wall",
+                  [], False, [], [], [], [], [], [], [], []],
+            263: [False, [], 2, [3, 13, 0, 112], 0, "Angel Dungeon: Water room (112/$70) Main", [], False, [], [], [],
+                  [], [], [], [], []],
+            279: [False, [], 2, [3, 13, 0, 112], 0, "Angel Dungeon: Water room (112/$70) Behind Draco", [], False, [],
+                  [], [], [], [], [], [], []],
+            265: [False, [], 2, [3, 13, 0, 112], 0, "Angel Dungeon: Water room (112/$70) Alcove", [], False, [], [], [],
+                  [], [], [], [], []],
+            266: [False, [], 2, [3, 13, 0, 113], 0, "Angel Dungeon: Wind Tunnel (113/$71)", [], False, [], [], [], [],
+                  [], [], [], []],
+            267: [False, [], 2, [3, 13, 0, 114], 0, "Angel Dungeon: Long Room (114/$72)", [], False, [], [], [], [], [],
+                  [], [], []],
+            277: [False, [], 2, [3, 13, 0, 115], 0, "Angel Dungeon: Ishtar's hall (115/$73) Foyer with slider", [],
+                  False, [], [], [], [], [], [], [], []],
+            269: [False, [], 2, [3, 13, 0, 115], 0, "Angel Dungeon: Ishtar's hall (115/$73) Main with waterfalls", [],
+                  False, [], [], [], [], [], [], [], []],
+            270: [False, [], 2, [3, 13, 0, 116], 0, "Angel Dungeon: Portrait Rooms (116/$74) Kara", [], False, [], [],
+                  [], [], [], [], [], []],
+            271: [False, [], 2, [3, 13, 0, 116], 0, "Angel Dungeon: Portrait Rooms (116/$74) Middle room", [], False,
+                  [], [], [], [], [], [], [], []],
+            272: [False, [], 2, [3, 13, 0, 116], 0, "Angel Dungeon: Portrait Rooms (116/$74) Ishtar's room", [], False,
+                  [], [], [], [], [], [], [], []],
+            273: [False, [], 2, [3, 13, 0, 116], 0, "Angel Dungeon: Portrait Rooms (116/$74) Ishtar chest", [], False,
+                  [], [], [], [], [], [], [], []],
+            274: [False, [], 2, [3, 13, 0, 117], 0, "Angel Dungeon: Puzzle Rooms", [], False, [], [], [], [], [], [],
+                  [], []],
 
             # Watermia
-            280: [False,     [12], 1, [3,14,0,120], 0, "Watermia: Main Area", [24], False, [], [], [], [], [], [], [], []],
-            #281: [False, [15,280], 0, [3,14,0,0], 0, "Watermia: Bridge Man", [], False, [], [], [], [], [], [], [], []],
-            282: [False,       [], 2, [3,14,0,124], 0, "Watermia: DS House", [], False, [], [], [], [], [], [], [], []],
-            283: [False,      [1], 2, [3,14,0,123], 0, "Watermia: Gambling House", [], False, [], [], [], [], [], [], [], []],
-            284: [False,       [], 2, [3,14,0,126], 0, "Watermia: West House", [], False, [], [], [], [], [], [], [], []],
-            285: [False,       [], 2, [3,14,0,125], 0, "Watermia: East House", [], False, [], [], [], [], [], [], [], []],
-            286: [False,       [], 2, [3,14,0,121], 0, "Watermia: Lance's House", [], False, [], [], [], [], [], [], [], []],
-            287: [False,       [], 2, [3,14,0,122], 0, "Watermia: NW House", [], False, [], [], [], [], [], [], [], []],
-            288: [False,    [280], 0, [3,14,0,120], 0, "Watermia: Stablemaster", [], True, [], [], [], [], [], [], [], []],
+            280: [False, [12], 1, [3, 14, 0, 120], 0, "Watermia: Main Area", [24], False, [], [], [], [], [], [], [],
+                  []],
+            # 281: [False, [15,280], 0, [3,14,0,0], 0, "Watermia: Bridge Man", [], False, [], [], [], [], [], [], [], []],
+            282: [False, [], 2, [3, 14, 0, 124], 0, "Watermia: DS House", [], False, [], [], [], [], [], [], [], []],
+            283: [False, [1], 2, [3, 14, 0, 123], 0, "Watermia: Gambling House", [], False, [], [], [], [], [], [], [],
+                  []],
+            284: [False, [], 2, [3, 14, 0, 126], 0, "Watermia: West House", [], False, [], [], [], [], [], [], [], []],
+            285: [False, [], 2, [3, 14, 0, 125], 0, "Watermia: East House", [], False, [], [], [], [], [], [], [], []],
+            286: [False, [], 2, [3, 14, 0, 121], 0, "Watermia: Lance's House", [], False, [], [], [], [], [], [], [],
+                  []],
+            287: [False, [], 2, [3, 14, 0, 122], 0, "Watermia: NW House", [], False, [], [], [], [], [], [], [], []],
+            288: [False, [280], 0, [3, 14, 0, 120], 0, "Watermia: Stablemaster", [], True, [], [], [], [], [], [], [],
+                  []],
 
             # Great Wall
-            290: [False, [12],  2, [3,15,0,130], 0, "Great Wall: Entrance (130/$82)", [], False, [], [], [], [], [], [], [], []],
-            291: [False, [292], 2, [3,15,0,131], 0, "Great Wall: Long Drop (131/$83) NW", [], False, [], [], [], [], [], [], [], []],
-            292: [False, [],    2, [3,15,0,131], 0, "Great Wall: Long Drop (131/$83) Lower", [], False, [], [], [], [], [], [], [], []],
-            293: [False, [],    2, [3,15,0,131], 0, "Great Wall: Long Drop (131/$83) NE", [], False, [], [], [], [], [], [], [], []],
-            294: [False, [296], 2, [3,15,0,133], 0, "Great Wall: Ramps (133/$85) W", [], False, [], [], [], [], [], [], [], []],
-            295: [False, [296], 2, [3,15,0,133], 0, "Great Wall: Ramps (133/$85) Center", [], False, [], [], [], [], [], [], [], []],
-            296: [False, [],    2, [3,15,0,133], 0, "Great Wall: Ramps (133/$85) E", [], False, [], [], [], [], [], [], [], []],
-            297: [False, [],    2, [3,15,0,134], 0, "Great Wall: Platforms (134/$86)", [], False, [], [], [], [], [], [], [], []],
-            298: [False, [],    2, [3,15,0,135], 0, "Great Wall: Friar Room (135/$87) W", [], False, [], [], [], [], [], [], [], []],
-            712: [False, [],    2, [3,15,0,135], 0, "Great Wall: Friar Room (135/$87) Archer", [], False, [], [], [], [], [], [], [], []],
-            299: [False, [],    2, [3,15,0,135], 0, "Great Wall: Friar Room (135/$87) E", [], False, [], [], [], [], [], [], [], []],
-            300: [False, [],    2, [3,15,0,136], 0, "Great Wall: Final Room (136/$88) W", [], False, [], [], [], [], [], [], [], []],
-            301: [False, [],    2, [3,15,0,136], 0, "Great Wall: Final Room (136/$88) E", [], False, [], [], [], [], [], [], [], []],
-            302: [False, [702], 2, [3,15,0,138], 0, "Great Wall: Fanger (138/$8a) Entrance", [], False, [], [], [], [], [], [], [], []],
-            702: [False, [303], 2, [3,15,0,138], 0, "Great Wall: Fanger (138/$8a) Fight", [], False, [], [], [], [], [], [], [], []],
-            303: [False, [],    2, [3,15,0,138], 0, "Great Wall: Fanger (138/$8a) Exit", [], False, [], [], [], [], [], [], [], []],
+            290: [False, [12], 2, [3, 15, 0, 130], 0, "Great Wall: Entrance (130/$82)", [], False, [], [], [], [], [],
+                  [], [], []],
+            291: [False, [292], 2, [3, 15, 0, 131], 0, "Great Wall: Long Drop (131/$83) NW", [], False, [], [], [], [],
+                  [], [], [], []],
+            292: [False, [], 2, [3, 15, 0, 131], 0, "Great Wall: Long Drop (131/$83) Lower", [], False, [], [], [], [],
+                  [], [], [], []],
+            293: [False, [], 2, [3, 15, 0, 131], 0, "Great Wall: Long Drop (131/$83) NE", [], False, [], [], [], [], [],
+                  [], [], []],
+            294: [False, [296], 2, [3, 15, 0, 133], 0, "Great Wall: Ramps (133/$85) W", [], False, [], [], [], [], [],
+                  [], [], []],
+            295: [False, [296], 2, [3, 15, 0, 133], 0, "Great Wall: Ramps (133/$85) Center", [], False, [], [], [], [],
+                  [], [], [], []],
+            296: [False, [], 2, [3, 15, 0, 133], 0, "Great Wall: Ramps (133/$85) E", [], False, [], [], [], [], [], [],
+                  [], []],
+            297: [False, [], 2, [3, 15, 0, 134], 0, "Great Wall: Platforms (134/$86)", [], False, [], [], [], [], [],
+                  [], [], []],
+            298: [False, [], 2, [3, 15, 0, 135], 0, "Great Wall: Friar Room (135/$87) W", [], False, [], [], [], [], [],
+                  [], [], []],
+            712: [False, [], 2, [3, 15, 0, 135], 0, "Great Wall: Friar Room (135/$87) Archer", [], False, [], [], [],
+                  [], [], [], [], []],
+            299: [False, [], 2, [3, 15, 0, 135], 0, "Great Wall: Friar Room (135/$87) E", [], False, [], [], [], [], [],
+                  [], [], []],
+            300: [False, [], 2, [3, 15, 0, 136], 0, "Great Wall: Final Room (136/$88) W", [], False, [], [], [], [], [],
+                  [], [], []],
+            301: [False, [], 2, [3, 15, 0, 136], 0, "Great Wall: Final Room (136/$88) E", [], False, [], [], [], [], [],
+                  [], [], []],
+            302: [False, [702], 2, [3, 15, 0, 138], 0, "Great Wall: Fanger (138/$8a) Entrance", [], False, [], [], [],
+                  [], [], [], [], []],
+            702: [False, [303], 2, [3, 15, 0, 138], 0, "Great Wall: Fanger (138/$8a) Fight", [], False, [], [], [], [],
+                  [], [], [], []],
+            303: [False, [], 2, [3, 15, 0, 138], 0, "Great Wall: Fanger (138/$8a) Exit", [], False, [], [], [], [], [],
+                  [], [], []],
 
             # Euro
-            310: [False, [13],  1, [4,16,0,145], 0, "Euro: Main Area", [24], False, [], [], [], [], [], [], [], []],
-            311: [False, [310], 0, [4,16,0,145], 0, "Euro: Stablemaster", [], True, [], [], [], [], [], [], [], []],
-            312: [False, [],    2, [4,16,0,148], 0, "Euro: Rolek Company", [], False, [], [], [], [], [], [], [], []],
-            313: [False, [],    2, [4,16,0,152], 0, "Euro: West House", [], False, [], [], [], [], [], [], [], []],
-            314: [False, [],    2, [4,16,0,149], 0, "Euro: Rolek Mansion", [40], False, [], [], [], [], [], [], [], []],
-            316: [False, [],    2, [4,16,0,150], 0, "Euro: Guest Room", [], False, [], [], [], [], [], [], [], []],
-            317: [False, [],    2, [4,16,0,146], 0, "Euro: Central House", [], False, [], [], [], [], [], [], [], []],
-            318: [False, [1],   2, [4,16,0,155], 0, "Euro: Jeweler House", [], False, [], [], [], [], [], [], [], []],
-            319: [False, [],    2, [4,16,0,156], 0, "Euro: Twins House", [], False, [], [], [], [], [], [], [], []],
-            320: [False, [],    2, [4,16,0,147], 0, "Euro: Hidden House", [], False, [], [], [], [], [], [], [], []],
-            321: [False, [],    2, [4,16,0,157], 0, "Euro: Shrine", [], False, [], [], [], [], [], [], [], []],
-            322: [False, [],    2, [4,16,0,154], 0, "Euro: Explorer's House", [], False, [], [], [], [], [], [], [], []],
-            323: [False, [324], 2, [4,16,0,151], 0, "Euro: Store Entrance", [], False, [], [], [], [], [], [], [], []],
-            324: [False, [],    2, [4,16,0,151], 0, "Euro: Store Exit", [], False, [], [], [], [], [], [], [], []],
-            325: [False, [],    2, [4,16,0,153], 0, "Euro: Dark Space House", [], False, [], [], [], [], [], [], [], []],
+            310: [False, [13], 1, [4, 16, 0, 145], 0, "Euro: Main Area", [24], False, [], [], [], [], [], [], [], []],
+            311: [False, [310], 0, [4, 16, 0, 145], 0, "Euro: Stablemaster", [], True, [], [], [], [], [], [], [], []],
+            312: [False, [], 2, [4, 16, 0, 148], 0, "Euro: Rolek Company", [], False, [], [], [], [], [], [], [], []],
+            313: [False, [], 2, [4, 16, 0, 152], 0, "Euro: West House", [], False, [], [], [], [], [], [], [], []],
+            314: [False, [], 2, [4, 16, 0, 149], 0, "Euro: Rolek Mansion", [40], False, [], [], [], [], [], [], [], []],
+            316: [False, [], 2, [4, 16, 0, 150], 0, "Euro: Guest Room", [], False, [], [], [], [], [], [], [], []],
+            317: [False, [], 2, [4, 16, 0, 146], 0, "Euro: Central House", [], False, [], [], [], [], [], [], [], []],
+            318: [False, [1], 2, [4, 16, 0, 155], 0, "Euro: Jeweler House", [], False, [], [], [], [], [], [], [], []],
+            319: [False, [], 2, [4, 16, 0, 156], 0, "Euro: Twins House", [], False, [], [], [], [], [], [], [], []],
+            320: [False, [], 2, [4, 16, 0, 147], 0, "Euro: Hidden House", [], False, [], [], [], [], [], [], [], []],
+            321: [False, [], 2, [4, 16, 0, 157], 0, "Euro: Shrine", [], False, [], [], [], [], [], [], [], []],
+            322: [False, [], 2, [4, 16, 0, 154], 0, "Euro: Explorer's House", [], False, [], [], [], [], [], [], [],
+                  []],
+            323: [False, [324], 2, [4, 16, 0, 151], 0, "Euro: Store Entrance", [], False, [], [], [], [], [], [], [],
+                  []],
+            324: [False, [], 2, [4, 16, 0, 151], 0, "Euro: Store Exit", [], False, [], [], [], [], [], [], [], []],
+            325: [False, [], 2, [4, 16, 0, 153], 0, "Euro: Dark Space House", [], False, [], [], [], [], [], [], [],
+                  []],
 
             # Mt. Kress
-            330: [False, [13],        2, [4,17,0,160], 0, "Kress: Entrance (160/$A0)", [], False, [], [], [], [], [], [], [], []],
-            331: [False, [],          2, [4,17,0,161], 0, "Kress: DS1 Room (161/$A1) E", [], False, [], [], [], [], [], [], [], []],
-            332: [False, [],          2, [4,17,0,161], 0, "Kress: DS1 Room (161/$A1) W", [], False, [], [], [], [], [], [], [], []],
-            333: [False, [],          2, [4,17,0,162], 0, "Kress: First Vine Room (162/$A2) Main", [26], False, [], [], [], [], [], [], [], []],
-            334: [False, [333],       2, [4,17,0,162], 0, "Kress: First Vine Room (162/$A2) S before jump", [], False, [], [], [], [], [], [], [], []],
-            335: [False, [],          2, [4,17,0,162], 0, "Kress: First Vine Room (162/$A2) NW past drops", [], False, [], [], [], [], [], [], [], []],
-            336: [False, [],          2, [4,17,0,162], 0, "Kress: First Vine Room (162/$A2) SE chest", [], False, [], [], [], [], [], [], [], []],
-            337: [False, [],          2, [4,17,0,163], 0, "Kress: DS2 Corridor (163/$A3)", [], False, [], [], [], [], [], [], [], []],
-            338: [False, [],          2, [4,17,0,164], 0, "Kress: West Chest Room (164/$A4)", [], False, [], [], [], [], [], [], [], []],
-            339: [False, [],          2, [4,17,0,165], 0, "Kress: Second Vine Room (165/$A5) S", [26], False, [], [], [], [], [], [], [], []],
-            340: [False, [],          2, [4,17,0,165], 0, "Kress: Second Vine Room (165/$A5) NE", [26], False, [], [], [], [], [], [], [], []],
-            341: [False, [339],       2, [4,17,0,165], 0, "Kress: Second Vine Room (165/$A5) NW", [], False, [], [], [], [], [], [], [], []],
-            342: [False, [],          2, [4,17,0,166], 0, "Kress: Mushroom Arena (166/$A6)", [], False, [], [], [], [], [], [], [], []],
-            343: [False, [],          2, [4,17,0,167], 0, "Kress: Final DS Room (167/$A7)", [], False, [], [], [], [], [], [], [], []],
-            344: [False, [],          2, [4,17,0,168], 0, "Kress: Final Combat Corridor (168/$A8)", [], False, [], [], [], [], [], [], [], []],
-            345: [False, [],          2, [4,17,0,169], 0, "Kress: End with Chest (169/$A9)", [], False, [], [], [], [], [], [], [], []],
+            330: [False, [13], 2, [4, 17, 0, 160], 0, "Kress: Entrance (160/$A0)", [], False, [], [], [], [], [], [],
+                  [], []],
+            331: [False, [], 2, [4, 17, 0, 161], 0, "Kress: DS1 Room (161/$A1) E", [], False, [], [], [], [], [], [],
+                  [], []],
+            332: [False, [], 2, [4, 17, 0, 161], 0, "Kress: DS1 Room (161/$A1) W", [], False, [], [], [], [], [], [],
+                  [], []],
+            333: [False, [], 2, [4, 17, 0, 162], 0, "Kress: First Vine Room (162/$A2) Main", [26], False, [], [], [],
+                  [], [], [], [], []],
+            334: [False, [333], 2, [4, 17, 0, 162], 0, "Kress: First Vine Room (162/$A2) S before jump", [], False, [],
+                  [], [], [], [], [], [], []],
+            335: [False, [], 2, [4, 17, 0, 162], 0, "Kress: First Vine Room (162/$A2) NW past drops", [], False, [], [],
+                  [], [], [], [], [], []],
+            336: [False, [], 2, [4, 17, 0, 162], 0, "Kress: First Vine Room (162/$A2) SE chest", [], False, [], [], [],
+                  [], [], [], [], []],
+            337: [False, [], 2, [4, 17, 0, 163], 0, "Kress: DS2 Corridor (163/$A3)", [], False, [], [], [], [], [], [],
+                  [], []],
+            338: [False, [], 2, [4, 17, 0, 164], 0, "Kress: West Chest Room (164/$A4)", [], False, [], [], [], [], [],
+                  [], [], []],
+            339: [False, [], 2, [4, 17, 0, 165], 0, "Kress: Second Vine Room (165/$A5) S", [26], False, [], [], [], [],
+                  [], [], [], []],
+            340: [False, [], 2, [4, 17, 0, 165], 0, "Kress: Second Vine Room (165/$A5) NE", [26], False, [], [], [], [],
+                  [], [], [], []],
+            341: [False, [339], 2, [4, 17, 0, 165], 0, "Kress: Second Vine Room (165/$A5) NW", [], False, [], [], [],
+                  [], [], [], [], []],
+            342: [False, [], 2, [4, 17, 0, 166], 0, "Kress: Mushroom Arena (166/$A6)", [], False, [], [], [], [], [],
+                  [], [], []],
+            343: [False, [], 2, [4, 17, 0, 167], 0, "Kress: Final DS Room (167/$A7)", [], False, [], [], [], [], [], [],
+                  [], []],
+            344: [False, [], 2, [4, 17, 0, 168], 0, "Kress: Final Combat Corridor (168/$A8)", [], False, [], [], [], [],
+                  [], [], [], []],
+            345: [False, [], 2, [4, 17, 0, 169], 0, "Kress: End with Chest (169/$A9)", [], False, [], [], [], [], [],
+                  [], [], []],
 
             # Natives' Village
-            350: [False, [13],  1, [4,18,0,172], 0, "Natives' Village: Main Area", [10], False, [], [], [], [], [], [], [], []],
-            351: [False, [350], 0, [4,18,0,172], 0, "Natives' Village: Child Guide", [], True, [], [], [], [], [], [], [], []],
-            352: [False, [],    2, [4,18,0,173], 0, "Natives' Village: West House", [], False, [], [], [], [], [], [], [], []],
-            353: [False, [],    2, [4,18,0,174], 0, "Natives' Village: House w/Statues", [29], False, [], [], [], [], [], [], [], []],
-            354: [False, [],    0, [4,18,0,174], 0, "Natives' Village: Statues Awake", [], False, [], [], [], [], [], [], [], []],
+            350: [False, [13], 1, [4, 18, 0, 172], 0, "Natives' Village: Main Area", [10], False, [], [], [], [], [],
+                  [], [], []],
+            351: [False, [350], 0, [4, 18, 0, 172], 0, "Natives' Village: Child Guide", [], True, [], [], [], [], [],
+                  [], [], []],
+            352: [False, [], 2, [4, 18, 0, 173], 0, "Natives' Village: West House", [], False, [], [], [], [], [], [],
+                  [], []],
+            353: [False, [], 2, [4, 18, 0, 174], 0, "Natives' Village: House w/Statues", [29], False, [], [], [], [],
+                  [], [], [], []],
+            354: [False, [], 0, [4, 18, 0, 174], 0, "Natives' Village: Statues Awake", [], False, [], [], [], [], [],
+                  [], [], []],
 
             # Ankor Wat
-            360: [False, [13],  2, [4,19,0,176], 0, "Ankor Wat: Exterior (176/$B0)", [], False, [], [], [], [], [], [], [], []],
-            361: [False, [],    2, [4,19,0,177], 0, "Ankor Wat: Outer-S (177/$B1) E", [], False, [], [], [], [], [], [], [], []],
-            362: [False, [739], 2, [4,19,0,177], 0, "Ankor Wat: Outer-S (177/$B1) W", [], False, [], [], [], [], [], [], [], []],
-            739: [False, [],    2, [4,19,0,177], 0, "Ankor Wat: Outer-S (177/$B1) scarab with orb", [], False, [], [], [], [], [], [], [], []],
-            363: [False, [],    2, [4,19,0,178], 0, "Ankor Wat: Outer-E (178/$B2) S", [], False, [], [], [], [], [], [], [], []],
-            364: [False, [363], 2, [4,19,0,178], 0, "Ankor Wat: Outer-E (178/$B2) center", [], False, [], [], [], [], [], [], [], []],
-            365: [False, [],    2, [4,19,0,178], 0, "Ankor Wat: Outer-E (178/$B2) N", [], False, [], [], [], [], [], [], [], []],
-            366: [False, [],    2, [4,19,0,179], 0, "Ankor Wat: Outer-N (179/$B3) E", [], False, [], [], [], [], [], [], [], []],
-            367: [False, [],    2, [4,19,0,179], 0, "Ankor Wat: Outer-N (179/$B3) W", [], False, [], [], [], [], [], [], [], []],
-            368: [False, [703], 2, [4,19,0,180], 0, "Ankor Wat: Outer Pit (180/$B4)", [], False, [], [], [], [], [], [], [], []],
-            703: [False, [368], 2, [4,19,0,180], 0, "Ankor Wat: Outer Pit (180/$B4) scarab with orb", [], False, [], [], [], [], [], [], [], []],
-            369: [False, [],    2, [4,19,0,181], 0, "Ankor Wat: Outer-W (181/$B5) N", [], False, [], [], [], [], [], [], [], []],
-            370: [False, [],    2, [4,19,0,181], 0, "Ankor Wat: Outer-W (181/$B5) center", [], False, [], [], [], [], [], [], [], []],
-            371: [False, [],    2, [4,19,0,181], 0, "Ankor Wat: Outer-W (181/$B5) S", [], False, [], [], [], [], [], [], [], []],
-            372: [False, [],    2, [4,19,0,182], 0, "Ankor Wat: Garden (182/$B6)", [], False, [], [], [], [], [], [], [], []],
-            373: [False, [],    2, [4,19,0,183], 0, "Ankor Wat: Inner-S (183/$B7) S", [], False, [], [], [], [], [], [], [], []],
-            374: [False, [373], 2, [4,19,0,183], 0, "Ankor Wat: Inner-S (183/$B7) NW", [], False, [], [], [], [], [], [], [], []],
-            375: [False, [],    2, [4,19,0,183], 0, "Ankor Wat: Inner-S (183/$B7) N", [], False, [], [], [], [], [], [], [], []],
-            376: [False, [],    2, [4,19,0,184], 0, "Ankor Wat: Inner-E (184/$B8) S", [], False, [], [], [], [], [], [], [], []],
-            727: [False, [],    2, [4,19,0,184], 0, "Ankor Wat: Inner-E (184/$B8) wall skull", [], False, [], [], [], [], [], [], [], []],
-            377: [False, [],    2, [4,19,0,184], 0, "Ankor Wat: Inner-E (184/$B8) N", [], False, [], [], [], [], [], [], [], []],
-            378: [False, [],    2, [4,19,0,185], 0, "Ankor Wat: Inner-W (185/$B9)", [], False, [], [], [], [], [], [], [], []],
-            379: [False, [],    2, [4,19,0,186], 0, "Ankor Wat: Road to MH (186/$BA) main", [], False, [], [], [], [], [], [], [], []],
-            380: [False, [],    2, [4,19,0,186], 0, "Ankor Wat: Road to MH (186/$BA) NE", [], False, [], [], [], [], [], [], [], []],
-            381: [False, [],    2, [4,19,0,187], 0, "Ankor Wat: Main-1 (187/$BB) main", [], False, [], [], [], [], [], [], [], []],
-            382: [False, [381], 2, [4,19,0,187], 0, "Ankor Wat: Main-1 (187/$BB) chest", [], False, [], [], [], [], [], [], [], []],
-            383: [False, [381], 2, [4,19,0,187], 0, "Ankor Wat: Main-1 (187/$BB) Dark Space", [], False, [], [], [], [], [], [], [], []],
-            384: [False, [],    2, [4,19,0,188], 0, "Ankor Wat: Main-2 (188/$BC) N", [], False, [], [], [], [], [], [], [], []],
-            385: [False, [],    2, [4,19,0,188], 0, "Ankor Wat: Main-2 (188/$BC) S", [], False, [], [], [], [], [], [], [], []],
-            386: [False, [],    2, [4,19,0,189], 0, "Ankor Wat: Main-3 (189/$BD) floor S", [], False, [], [], [], [], [], [], [], []],
-            387: [False, [],    2, [4,19,0,189], 0, "Ankor Wat: Main-3 (189/$BD) floor N", [], False, [], [], [], [], [], [], [], []],
-            388: [False, [386], 2, [4,19,0,189], 0, "Ankor Wat: Main-3 (189/$BD) platform", [], False, [], [], [], [], [], [], [], []],
-            389: [False, [],    2, [4,19,0,190], 0, "Ankor Wat: Main-4 (190/$BE) SE", [], False, [], [], [], [], [], [], [], []],
-            390: [False, [],    2, [4,19,0,190], 0, "Ankor Wat: Main-4 (190/$BE) N", [], False, [], [], [], [], [], [], [], []],
-            391: [False, [],    2, [4,19,0,191], 0, "Ankor Wat: End (191/$BF)", [], False, [], [], [], [], [], [], [], []],
+            360: [False, [13], 2, [4, 19, 0, 176], 0, "Ankor Wat: Exterior (176/$B0)", [], False, [], [], [], [], [],
+                  [], [], []],
+            361: [False, [], 2, [4, 19, 0, 177], 0, "Ankor Wat: Outer-S (177/$B1) E", [], False, [], [], [], [], [], [],
+                  [], []],
+            362: [False, [739], 2, [4, 19, 0, 177], 0, "Ankor Wat: Outer-S (177/$B1) W", [], False, [], [], [], [], [],
+                  [], [], []],
+            739: [False, [], 2, [4, 19, 0, 177], 0, "Ankor Wat: Outer-S (177/$B1) scarab with orb", [], False, [], [],
+                  [], [], [], [], [], []],
+            363: [False, [], 2, [4, 19, 0, 178], 0, "Ankor Wat: Outer-E (178/$B2) S", [], False, [], [], [], [], [], [],
+                  [], []],
+            364: [False, [363], 2, [4, 19, 0, 178], 0, "Ankor Wat: Outer-E (178/$B2) center", [], False, [], [], [], [],
+                  [], [], [], []],
+            365: [False, [], 2, [4, 19, 0, 178], 0, "Ankor Wat: Outer-E (178/$B2) N", [], False, [], [], [], [], [], [],
+                  [], []],
+            366: [False, [], 2, [4, 19, 0, 179], 0, "Ankor Wat: Outer-N (179/$B3) E", [], False, [], [], [], [], [], [],
+                  [], []],
+            367: [False, [], 2, [4, 19, 0, 179], 0, "Ankor Wat: Outer-N (179/$B3) W", [], False, [], [], [], [], [], [],
+                  [], []],
+            368: [False, [703], 2, [4, 19, 0, 180], 0, "Ankor Wat: Outer Pit (180/$B4)", [], False, [], [], [], [], [],
+                  [], [], []],
+            703: [False, [368], 2, [4, 19, 0, 180], 0, "Ankor Wat: Outer Pit (180/$B4) scarab with orb", [], False, [],
+                  [], [], [], [], [], [], []],
+            369: [False, [], 2, [4, 19, 0, 181], 0, "Ankor Wat: Outer-W (181/$B5) N", [], False, [], [], [], [], [], [],
+                  [], []],
+            370: [False, [], 2, [4, 19, 0, 181], 0, "Ankor Wat: Outer-W (181/$B5) center", [], False, [], [], [], [],
+                  [], [], [], []],
+            371: [False, [], 2, [4, 19, 0, 181], 0, "Ankor Wat: Outer-W (181/$B5) S", [], False, [], [], [], [], [], [],
+                  [], []],
+            372: [False, [], 2, [4, 19, 0, 182], 0, "Ankor Wat: Garden (182/$B6)", [], False, [], [], [], [], [], [],
+                  [], []],
+            373: [False, [], 2, [4, 19, 0, 183], 0, "Ankor Wat: Inner-S (183/$B7) S", [], False, [], [], [], [], [], [],
+                  [], []],
+            374: [False, [373], 2, [4, 19, 0, 183], 0, "Ankor Wat: Inner-S (183/$B7) NW", [], False, [], [], [], [], [],
+                  [], [], []],
+            375: [False, [], 2, [4, 19, 0, 183], 0, "Ankor Wat: Inner-S (183/$B7) N", [], False, [], [], [], [], [], [],
+                  [], []],
+            376: [False, [], 2, [4, 19, 0, 184], 0, "Ankor Wat: Inner-E (184/$B8) S", [], False, [], [], [], [], [], [],
+                  [], []],
+            727: [False, [], 2, [4, 19, 0, 184], 0, "Ankor Wat: Inner-E (184/$B8) wall skull", [], False, [], [], [],
+                  [], [], [], [], []],
+            377: [False, [], 2, [4, 19, 0, 184], 0, "Ankor Wat: Inner-E (184/$B8) N", [], False, [], [], [], [], [], [],
+                  [], []],
+            378: [False, [], 2, [4, 19, 0, 185], 0, "Ankor Wat: Inner-W (185/$B9)", [], False, [], [], [], [], [], [],
+                  [], []],
+            379: [False, [], 2, [4, 19, 0, 186], 0, "Ankor Wat: Road to MH (186/$BA) main", [], False, [], [], [], [],
+                  [], [], [], []],
+            380: [False, [], 2, [4, 19, 0, 186], 0, "Ankor Wat: Road to MH (186/$BA) NE", [], False, [], [], [], [], [],
+                  [], [], []],
+            381: [False, [], 2, [4, 19, 0, 187], 0, "Ankor Wat: Main-1 (187/$BB) main", [], False, [], [], [], [], [],
+                  [], [], []],
+            382: [False, [381], 2, [4, 19, 0, 187], 0, "Ankor Wat: Main-1 (187/$BB) chest", [], False, [], [], [], [],
+                  [], [], [], []],
+            383: [False, [381], 2, [4, 19, 0, 187], 0, "Ankor Wat: Main-1 (187/$BB) Dark Space", [], False, [], [], [],
+                  [], [], [], [], []],
+            384: [False, [], 2, [4, 19, 0, 188], 0, "Ankor Wat: Main-2 (188/$BC) N", [], False, [], [], [], [], [], [],
+                  [], []],
+            385: [False, [], 2, [4, 19, 0, 188], 0, "Ankor Wat: Main-2 (188/$BC) S", [], False, [], [], [], [], [], [],
+                  [], []],
+            386: [False, [], 2, [4, 19, 0, 189], 0, "Ankor Wat: Main-3 (189/$BD) floor S", [], False, [], [], [], [],
+                  [], [], [], []],
+            387: [False, [], 2, [4, 19, 0, 189], 0, "Ankor Wat: Main-3 (189/$BD) floor N", [], False, [], [], [], [],
+                  [], [], [], []],
+            388: [False, [386], 2, [4, 19, 0, 189], 0, "Ankor Wat: Main-3 (189/$BD) platform", [], False, [], [], [],
+                  [], [], [], [], []],
+            389: [False, [], 2, [4, 19, 0, 190], 0, "Ankor Wat: Main-4 (190/$BE) SE", [], False, [], [], [], [], [], [],
+                  [], []],
+            390: [False, [], 2, [4, 19, 0, 190], 0, "Ankor Wat: Main-4 (190/$BE) N", [], False, [], [], [], [], [], [],
+                  [], []],
+            391: [False, [], 2, [4, 19, 0, 191], 0, "Ankor Wat: End (191/$BF)", [], False, [], [], [], [], [], [], [],
+                  []],
 
             # Dao
-            400: [False, [1,14], 1, [5,20,0,195], 0, "Dao: Main Area", [], False, [], [], [], [], [], [], [], []],
-            401: [False, [],     2, [5,20,0,196], 0, "Dao: NW House", [], False, [], [], [], [], [], [], [], []],
-            402: [False, [],     2, [5,20,0,200], 0, "Dao: Neil's House", [], False, [], [], [], [], [], [], [], []],
-            403: [False, [],     2, [5,20,0,198], 0, "Dao: Snake Game", [], False, [], [], [], [], [], [], [], []],
-            404: [False, [],     2, [5,20,0,199], 0, "Dao: SW House", [], False, [], [], [], [], [], [], [], []],
-            405: [False, [],     2, [5,20,0,197], 0, "Dao: S House", [], False, [], [], [], [], [], [], [], []],
-            406: [False, [],     2, [5,20,0,201], 0, "Dao: SE House", [], False, [], [], [], [], [], [], [], []],
+            400: [False, [1, 14], 1, [5, 20, 0, 195], 0, "Dao: Main Area", [], False, [], [], [], [], [], [], [], []],
+            401: [False, [], 2, [5, 20, 0, 196], 0, "Dao: NW House", [], False, [], [], [], [], [], [], [], []],
+            402: [False, [], 2, [5, 20, 0, 200], 0, "Dao: Neil's House", [], False, [], [], [], [], [], [], [], []],
+            403: [False, [], 2, [5, 20, 0, 198], 0, "Dao: Snake Game", [], False, [], [], [], [], [], [], [], []],
+            404: [False, [], 2, [5, 20, 0, 199], 0, "Dao: SW House", [], False, [], [], [], [], [], [], [], []],
+            405: [False, [], 2, [5, 20, 0, 197], 0, "Dao: S House", [], False, [], [], [], [], [], [], [], []],
+            406: [False, [], 2, [5, 20, 0, 201], 0, "Dao: SE House", [], False, [], [], [], [], [], [], [], []],
 
             # Pyramid
-            410: [False, [14],      2, [5,21,0,204], 0, "Pyramid: Entrance (main)", [], False, [], [], [], [], [], [], [], []],
-            713: [False, [],        2, [5,21,0,204], 0, "Pyramid: Entrance (top Dark Space)", [], False, [], [], [], [], [], [], [], []],
-            411: [False, [],        2, [5,21,0,204], 0, "Pyramid: Entrance (behind orbs)", [], False, [], [], [], [], [], [], [], []],
-            412: [False, [413],     2, [5,21,0,204], 0, "Pyramid: Entrance (hidden platform)", [], False, [], [], [], [], [], [], [], []],
-            413: [False, [],        2, [5,21,0,204], 0, "Pyramid: Entrance (bottom)", [], False, [], [], [], [], [], [], [], []],
-            414: [False, [],        2, [5,21,0,204], 0, "Pyramid: Entrance (boss entrance)", [], False, [], [], [], [], [], [], [], []],
-            415: [False, [],        2, [5,21,0,205], 0, "Pyramid: Hieroglyph room", [30, 31, 32, 33, 34, 35, 38], False, [], [], [], [], [], [], [], []],
-            416: [False, [],        2, [5,21,0,206], 0, "Pyramid: 206 / 1-A / Will ramps (E)", [], False, [], [], [], [], [], [], [], []],
-            417: [False, [],        2, [5,21,0,206], 0, "Pyramid: 206 / 1-A / Will ramps (W)", [], False, [], [], [], [], [], [], [], []],
-            418: [False, [],        2, [5,21,0,207], 0, "Pyramid: 207 / 1-B / Will ramps (NE)", [], False, [], [], [], [], [], [], [], []],
-            419: [False, [],        2, [5,21,0,207], 0, "Pyramid: 207 / 1-B / Will ramps (SW)", [], False, [], [], [], [], [], [], [], []],
-            420: [False, [421],     2, [5,21,0,208], 0, "Pyramid: 208 / 2-A / Breakable floors (N)", [], False, [], [], [], [], [], [], [], []],
-            421: [False, [420],     2, [5,21,0,208], 0, "Pyramid: 208 / 2-A / Breakable floors (S)", [], False, [], [], [], [], [], [], [], []],
-            422: [False, [423],     2, [5,21,0,209], 0, "Pyramid: 209 / 2-B / Breakable floors (W)", [], False, [], [], [], [], [], [], [], []],
-            423: [False, [422],     2, [5,21,0,209], 0, "Pyramid: 209 / 2-B / Breakable floors (E)", [], False, [], [], [], [], [], [], [], []],
-            424: [False, [],        2, [5,21,0,210], 0, "Pyramid: 210 / 6-A / Mummies", [], False, [], [], [], [], [], [], [], []],
-            425: [False, [],        2, [5,21,0,211], 0, "Pyramid: 211 / 6-B / Mummies", [], False, [], [], [], [], [], [], [], []],
-            426: [False, [],        2, [5,21,0,212], 0, "Pyramid: 212 / 5-A / Quake-Aura (N)", [], False, [], [], [], [], [], [], [], []],
-            427: [False, [],        2, [5,21,0,212], 0, "Pyramid: 212 / 5-A / Quake-Aura (center)", [], False, [], [], [], [], [], [], [], []],
-            428: [False, [],        2, [5,21,0,212], 0, "Pyramid: 212 / 5-A / Quake-Aura (SE chest)", [], False, [], [], [], [], [], [], [], []],
-            429: [False, [],        2, [5,21,0,212], 0, "Pyramid: 212 / 5-A / Quake-Aura (SW exit)", [], False, [], [], [], [], [], [], [], []],
-            430: [False, [],        2, [5,21,0,213], 0, "Pyramid: 213 / 5-B / Quake-Aura", [], False, [], [], [], [], [], [], [], []],
-            431: [False, [],        2, [5,21,0,214], 0, "Pyramid: 214 / 3-A / Friar-K6 (Upper)", [], False, [], [], [], [], [], [], [], []],
-            432: [False, [],        2, [5,21,0,214], 0, "Pyramid: 214 / 3-A / Friar-K6 (NE chest)", [], False, [], [], [], [], [], [], [], []],
-            433: [False, [431,434], 2, [5,21,0,214], 0, "Pyramid: 214 / 3-A / Friar-K6 (E platform)", [], False, [], [], [], [], [], [], [], []],
-            434: [False, [433],     2, [5,21,0,214], 0, "Pyramid: 214 / 3-A / Friar-K6 (Lower)", [], False, [], [], [], [], [], [], [], []],
-            435: [False, [],        2, [5,21,0,215], 0, "Pyramid: 215 / 3-B / Friar-K6 (main)", [], False, [], [], [], [], [], [], [], []],
-            436: [False, [437],     2, [5,21,0,216], 0, "Pyramid: 216 / 4-A / Crushers (N)", [], False, [], [], [], [], [], [], [], []],
-            437: [False, [],        2, [5,21,0,216], 0, "Pyramid: 216 / 4-A / Crushers (S)", [], False, [], [], [], [], [], [], [], []],
-            438: [False, [],        2, [5,21,0,217], 0, "Pyramid: 217 / 4-B / Crushers (W)", [], False, [], [], [], [], [], [], [], []],
-            439: [False, [],        2, [5,21,0,217], 0, "Pyramid: 217 / 4-B / Crushers (E)", [], False, [], [], [], [], [], [], [], []],
-            440: [False, [],        2, [5,21,0,219], 0, "Pyramid: 219 / 4-C / Crushers (W)", [], False, [], [], [], [], [], [], [], []],
-            441: [False, [],        2, [5,21,0,219], 0, "Pyramid: 219 / 4-C / Crushers (E)", [], False, [], [], [], [], [], [], [], []],
-            442: [False, [],        2, [5,21,0,218], 0, "Pyramid: Hieroglyph 1", [], False, [], [], [], [], [], [], [], []],
-            443: [False, [],        2, [5,21,0,218], 0, "Pyramid: Hieroglyph 2", [], False, [], [], [], [], [], [], [], []],
-            444: [False, [],        2, [5,21,0,218], 0, "Pyramid: Hieroglyph 3", [], False, [], [], [], [], [], [], [], []],
-            445: [False, [],        2, [5,21,0,218], 0, "Pyramid: Hieroglyph 4", [], False, [], [], [], [], [], [], [], []],
-            446: [False, [],        2, [5,21,0,218], 0, "Pyramid: Hieroglyph 5", [], False, [], [], [], [], [], [], [], []],
-            447: [False, [],        2, [5,21,0,218], 0, "Pyramid: Hieroglyph 6", [], False, [], [], [], [], [], [], [], []],
-            448: [False, [],        2, [5,21,0,221], 0, "Pyramid: Boss Room", [], True, [], [], [], [], [], [], [], []],
-            449: [False, [415,517], 0, [5,21,0,205], 0, "Pyramid: Hieroglyphs Placed", [], False, [], [], [], [], [], [], [], []],
-            450: [False, [],        2, [5,21,0,215], 0, "Pyramid: 215 / 3-B / Friar-K6 (past K6)", [], False, [], [], [], [], [], [], [], []],
+            410: [False, [14], 2, [5, 21, 0, 204], 0, "Pyramid: Entrance (main)", [], False, [], [], [], [], [], [], [],
+                  []],
+            713: [False, [], 2, [5, 21, 0, 204], 0, "Pyramid: Entrance (top Dark Space)", [], False, [], [], [], [], [],
+                  [], [], []],
+            411: [False, [], 2, [5, 21, 0, 204], 0, "Pyramid: Entrance (behind orbs)", [], False, [], [], [], [], [],
+                  [], [], []],
+            412: [False, [413], 2, [5, 21, 0, 204], 0, "Pyramid: Entrance (hidden platform)", [], False, [], [], [], [],
+                  [], [], [], []],
+            413: [False, [], 2, [5, 21, 0, 204], 0, "Pyramid: Entrance (bottom)", [], False, [], [], [], [], [], [], [],
+                  []],
+            414: [False, [], 2, [5, 21, 0, 204], 0, "Pyramid: Entrance (boss entrance)", [], False, [], [], [], [], [],
+                  [], [], []],
+            415: [False, [], 2, [5, 21, 0, 205], 0, "Pyramid: Hieroglyph room", [30, 31, 32, 33, 34, 35, 38], False, [],
+                  [], [], [], [], [], [], []],
+            416: [False, [], 2, [5, 21, 0, 206], 0, "Pyramid: 206 / 1-A / Will ramps (E)", [], False, [], [], [], [],
+                  [], [], [], []],
+            417: [False, [], 2, [5, 21, 0, 206], 0, "Pyramid: 206 / 1-A / Will ramps (W)", [], False, [], [], [], [],
+                  [], [], [], []],
+            418: [False, [], 2, [5, 21, 0, 207], 0, "Pyramid: 207 / 1-B / Will ramps (NE)", [], False, [], [], [], [],
+                  [], [], [], []],
+            419: [False, [], 2, [5, 21, 0, 207], 0, "Pyramid: 207 / 1-B / Will ramps (SW)", [], False, [], [], [], [],
+                  [], [], [], []],
+            420: [False, [421], 2, [5, 21, 0, 208], 0, "Pyramid: 208 / 2-A / Breakable floors (N)", [], False, [], [],
+                  [], [], [], [], [], []],
+            421: [False, [420], 2, [5, 21, 0, 208], 0, "Pyramid: 208 / 2-A / Breakable floors (S)", [], False, [], [],
+                  [], [], [], [], [], []],
+            422: [False, [423], 2, [5, 21, 0, 209], 0, "Pyramid: 209 / 2-B / Breakable floors (W)", [], False, [], [],
+                  [], [], [], [], [], []],
+            423: [False, [422], 2, [5, 21, 0, 209], 0, "Pyramid: 209 / 2-B / Breakable floors (E)", [], False, [], [],
+                  [], [], [], [], [], []],
+            424: [False, [], 2, [5, 21, 0, 210], 0, "Pyramid: 210 / 6-A / Mummies", [], False, [], [], [], [], [], [],
+                  [], []],
+            425: [False, [], 2, [5, 21, 0, 211], 0, "Pyramid: 211 / 6-B / Mummies", [], False, [], [], [], [], [], [],
+                  [], []],
+            426: [False, [], 2, [5, 21, 0, 212], 0, "Pyramid: 212 / 5-A / Quake-Aura (N)", [], False, [], [], [], [],
+                  [], [], [], []],
+            427: [False, [], 2, [5, 21, 0, 212], 0, "Pyramid: 212 / 5-A / Quake-Aura (center)", [], False, [], [], [],
+                  [], [], [], [], []],
+            428: [False, [], 2, [5, 21, 0, 212], 0, "Pyramid: 212 / 5-A / Quake-Aura (SE chest)", [], False, [], [], [],
+                  [], [], [], [], []],
+            429: [False, [], 2, [5, 21, 0, 212], 0, "Pyramid: 212 / 5-A / Quake-Aura (SW exit)", [], False, [], [], [],
+                  [], [], [], [], []],
+            430: [False, [], 2, [5, 21, 0, 213], 0, "Pyramid: 213 / 5-B / Quake-Aura", [], False, [], [], [], [], [],
+                  [], [], []],
+            431: [False, [], 2, [5, 21, 0, 214], 0, "Pyramid: 214 / 3-A / Friar-K6 (Upper)", [], False, [], [], [], [],
+                  [], [], [], []],
+            432: [False, [], 2, [5, 21, 0, 214], 0, "Pyramid: 214 / 3-A / Friar-K6 (NE chest)", [], False, [], [], [],
+                  [], [], [], [], []],
+            433: [False, [431, 434], 2, [5, 21, 0, 214], 0, "Pyramid: 214 / 3-A / Friar-K6 (E platform)", [], False, [],
+                  [], [], [], [], [], [], []],
+            434: [False, [433], 2, [5, 21, 0, 214], 0, "Pyramid: 214 / 3-A / Friar-K6 (Lower)", [], False, [], [], [],
+                  [], [], [], [], []],
+            435: [False, [], 2, [5, 21, 0, 215], 0, "Pyramid: 215 / 3-B / Friar-K6 (main)", [], False, [], [], [], [],
+                  [], [], [], []],
+            436: [False, [437], 2, [5, 21, 0, 216], 0, "Pyramid: 216 / 4-A / Crushers (N)", [], False, [], [], [], [],
+                  [], [], [], []],
+            437: [False, [], 2, [5, 21, 0, 216], 0, "Pyramid: 216 / 4-A / Crushers (S)", [], False, [], [], [], [], [],
+                  [], [], []],
+            438: [False, [], 2, [5, 21, 0, 217], 0, "Pyramid: 217 / 4-B / Crushers (W)", [], False, [], [], [], [], [],
+                  [], [], []],
+            439: [False, [], 2, [5, 21, 0, 217], 0, "Pyramid: 217 / 4-B / Crushers (E)", [], False, [], [], [], [], [],
+                  [], [], []],
+            440: [False, [], 2, [5, 21, 0, 219], 0, "Pyramid: 219 / 4-C / Crushers (W)", [], False, [], [], [], [], [],
+                  [], [], []],
+            441: [False, [], 2, [5, 21, 0, 219], 0, "Pyramid: 219 / 4-C / Crushers (E)", [], False, [], [], [], [], [],
+                  [], [], []],
+            442: [False, [], 2, [5, 21, 0, 218], 0, "Pyramid: Hieroglyph 1", [], False, [], [], [], [], [], [], [], []],
+            443: [False, [], 2, [5, 21, 0, 218], 0, "Pyramid: Hieroglyph 2", [], False, [], [], [], [], [], [], [], []],
+            444: [False, [], 2, [5, 21, 0, 218], 0, "Pyramid: Hieroglyph 3", [], False, [], [], [], [], [], [], [], []],
+            445: [False, [], 2, [5, 21, 0, 218], 0, "Pyramid: Hieroglyph 4", [], False, [], [], [], [], [], [], [], []],
+            446: [False, [], 2, [5, 21, 0, 218], 0, "Pyramid: Hieroglyph 5", [], False, [], [], [], [], [], [], [], []],
+            447: [False, [], 2, [5, 21, 0, 218], 0, "Pyramid: Hieroglyph 6", [], False, [], [], [], [], [], [], [], []],
+            448: [False, [], 2, [5, 21, 0, 221], 0, "Pyramid: Boss Room", [], True, [], [], [], [], [], [], [], []],
+            449: [False, [415, 517], 0, [5, 21, 0, 205], 0, "Pyramid: Hieroglyphs Placed", [], False, [], [], [], [],
+                  [], [], [], []],
+            450: [False, [], 2, [5, 21, 0, 215], 0, "Pyramid: 215 / 3-B / Friar-K6 (past K6)", [], False, [], [], [],
+                  [], [], [], [], []],
 
             # Babel
-            460: [False, [],       2, [6,22,0,222], 0, "Babel: Foyer", [], False, [], [], [], [], [], [], [], []],
-            461: [False, [],       2, [6,22,0,223], 0, "Babel: Map 223 (bottom)", [], False, [], [], [], [], [], [], [], []],
-            462: [False, [461],    2, [6,22,0,223], 0, "Babel: Map 223 (top)", [], False, [], [], [], [], [], [], [], []],
-            463: [False, [518,519],2, [6,22,0,224], 0, "Babel: Map 224 (bottom)", [], False, [], [], [], [], [], [], [], []],
-            464: [False, [520,521],2, [6,22,0,224], 0, "Babel: Map 224 (top)", [], False, [], [], [], [], [], [], [], []],
-            465: [False, [466],    2, [6,22,0,225], 0, "Babel: Map 225 (SW)", [], False, [], [], [], [], [], [], [], []],
-            466: [False, [],       2, [6,22,0,225], 0, "Babel: Map 225 (NW)", [], False, [], [], [], [], [], [], [], []],
-            467: [False, [468],    2, [6,22,0,225], 0, "Babel: Map 225 (SE)", [], False, [], [], [], [], [], [], [], []],
-            468: [False, [],       2, [6,22,0,225], 0, "Babel: Map 225 (NE)", [], False, [], [], [], [], [], [], [], []],
-            469: [False, [470],    2, [6,22,0,226], 0, "Babel: Map 226 (bottom)", [], False, [], [], [], [], [], [], [], []],
-            470: [False, [],       2, [6,22,0,226], 0, "Babel: Map 226 (top)", [], False, [], [], [], [], [], [], [], []],
-            471: [False, [522],    2, [6,22,0,227], 0, "Babel: Map 227 (bottom)", [], False, [], [], [], [], [], [], [], []],
-            472: [False, [],       2, [6,22,0,227], 0, "Babel: Map 227 (top)", [], False, [], [], [], [], [], [], [], []],
-            473: [False, [],       2, [6,22,0,222], 0, "Babel: Olman's Room", [], False, [], [], [], [], [], [], [], []],
-            474: [False, [],       0, [6,22,0,242], 0, "Babel: Castoth", [], False, [], [], [], [], [], [], [], []],
-            475: [False, [],       0, [6,22,0,243], 0, "Babel: Viper", [], False, [], [], [], [], [], [], [], []],
-            476: [False, [],       0, [6,22,0,244], 0, "Babel: Vampires", [], False, [], [], [], [], [], [], [], []],
-            477: [False, [],       0, [6,22,0,245], 0, "Babel: Sand Fanger", [], False, [], [], [], [], [], [], [], []],
-            478: [False, [],       0, [6,22,0,246], 0, "Babel: Mummy Queen", [], False, [], [], [], [], [], [], [], []],
-            479: [False, [473],    0, [6,22,0,246], 0, "Babel: Statue Get", [], False, [], [], [], [], [], [], [], []],
+            460: [False, [], 2, [6, 22, 0, 222], 0, "Babel: Foyer", [], False, [], [], [], [], [], [], [], []],
+            461: [False, [], 2, [6, 22, 0, 223], 0, "Babel: Map 223 (bottom)", [], False, [], [], [], [], [], [], [],
+                  []],
+            462: [False, [461], 2, [6, 22, 0, 223], 0, "Babel: Map 223 (top)", [], False, [], [], [], [], [], [], [],
+                  []],
+            463: [False, [518, 519], 2, [6, 22, 0, 224], 0, "Babel: Map 224 (bottom)", [], False, [], [], [], [], [],
+                  [], [], []],
+            464: [False, [520, 521], 2, [6, 22, 0, 224], 0, "Babel: Map 224 (top)", [], False, [], [], [], [], [], [],
+                  [], []],
+            465: [False, [466], 2, [6, 22, 0, 225], 0, "Babel: Map 225 (SW)", [], False, [], [], [], [], [], [], [],
+                  []],
+            466: [False, [], 2, [6, 22, 0, 225], 0, "Babel: Map 225 (NW)", [], False, [], [], [], [], [], [], [], []],
+            467: [False, [468], 2, [6, 22, 0, 225], 0, "Babel: Map 225 (SE)", [], False, [], [], [], [], [], [], [],
+                  []],
+            468: [False, [], 2, [6, 22, 0, 225], 0, "Babel: Map 225 (NE)", [], False, [], [], [], [], [], [], [], []],
+            469: [False, [470], 2, [6, 22, 0, 226], 0, "Babel: Map 226 (bottom)", [], False, [], [], [], [], [], [], [],
+                  []],
+            470: [False, [], 2, [6, 22, 0, 226], 0, "Babel: Map 226 (top)", [], False, [], [], [], [], [], [], [], []],
+            471: [False, [522], 2, [6, 22, 0, 227], 0, "Babel: Map 227 (bottom)", [], False, [], [], [], [], [], [], [],
+                  []],
+            472: [False, [], 2, [6, 22, 0, 227], 0, "Babel: Map 227 (top)", [], False, [], [], [], [], [], [], [], []],
+            473: [False, [], 2, [6, 22, 0, 222], 0, "Babel: Olman's Room", [], False, [], [], [], [], [], [], [], []],
+            474: [False, [], 0, [6, 22, 0, 242], 0, "Babel: Castoth", [], False, [], [], [], [], [], [], [], []],
+            475: [False, [], 0, [6, 22, 0, 243], 0, "Babel: Viper", [], False, [], [], [], [], [], [], [], []],
+            476: [False, [], 0, [6, 22, 0, 244], 0, "Babel: Vampires", [], False, [], [], [], [], [], [], [], []],
+            477: [False, [], 0, [6, 22, 0, 245], 0, "Babel: Sand Fanger", [], False, [], [], [], [], [], [], [], []],
+            478: [False, [], 0, [6, 22, 0, 246], 0, "Babel: Mummy Queen", [], False, [], [], [], [], [], [], [], []],
+            479: [False, [473], 0, [6, 22, 0, 246], 0, "Babel: Statue Get", [], False, [], [], [], [], [], [], [], []],
 
             # Jeweler's Mansion
-            480: [False, [],    2, [6,23,0,233], 0, "Jeweler's Mansion: Entrance", [], False, [], [], [], [], [], [], [], []],
-            714: [False, [],    2, [6,23,0,233], 0, "Jeweler's Mansion: Between Gates", [], False, [], [], [], [], [], [], [], []],
-            715: [False, [],    2, [6,23,0,233], 0, "Jeweler's Mansion: Main", [], False, [], [], [], [], [], [], [], []],
-            481: [False, [],    2, [6,23,0,233], 0, "Jeweler's Mansion: Behind Psycho Slider", [], False, [], [], [], [], [], [], [], []],
-            482: [False, [523], 2, [6,23,0,234], 0, "Jeweler's Mansion: Solid Arm", [], False, [], [], [], [], [], [], [], []],
+            480: [False, [], 2, [6, 23, 0, 233], 0, "Jeweler's Mansion: Entrance", [], False, [], [], [], [], [], [],
+                  [], []],
+            714: [False, [], 2, [6, 23, 0, 233], 0, "Jeweler's Mansion: Between Gates", [], False, [], [], [], [], [],
+                  [], [], []],
+            715: [False, [], 2, [6, 23, 0, 233], 0, "Jeweler's Mansion: Main", [], False, [], [], [], [], [], [], [],
+                  []],
+            481: [False, [], 2, [6, 23, 0, 233], 0, "Jeweler's Mansion: Behind Psycho Slider", [], False, [], [], [],
+                  [], [], [], [], []],
+            482: [False, [523], 2, [6, 23, 0, 234], 0, "Jeweler's Mansion: Solid Arm", [], False, [], [], [], [], [],
+                  [], [], []],
 
             # Game End
-            490: [False, [500], 0, [0,0,0,0], 0, "Kara Released", [20], False, [], [], [], [], [], [], [], []],
-            491: [False,    [], 0, [0,0,0,0], 0, "Firebird access", [], False, [], [], [], [], [], [], [], []],
-            492: [False,    [], 0, [0,0,0,0], 0, "Dark Gaia/End Game", [], False, [], [], [], [], [], [], [], []],
+            490: [False, [500], 0, [0, 0, 0, 0], 0, "Kara Released", [20], False, [], [], [], [], [], [], [], []],
+            491: [False, [], 0, [0, 0, 0, 0], 0, "Firebird access", [], False, [], [], [], [], [], [], [], []],
+            492: [False, [], 0, [0, 0, 0, 0], 0, "Dark Gaia/End Game", [], False, [], [], [], [], [], [], [], []],
 
             # Event Switches
-            500: [False, [], 0, [0,0,0,0], 0, "Kara", [], False, [], [], [], [], [], [], [], []],
-            502: [False, [], 0, [0,0,0,26], 0, "Moon Tribe: Spirits Healed", [], False, [], [], [], [], [], [], [], []],
-            503: [False, [], 0, [0,0,0,0], 0, "Inca: Castoth Defeated", [], False, [], [], [], [], [], [], [], []],
-            505: [False, [], 0, [0,0,0,0], 0, "Neil's Memory Restored", [], False, [], [], [], [], [], [], [], []],
-            508: [False, [], 0, [0,0,0,82], 0, "Sky Garden: Map 82 SE Switch", [], False, [], [], [], [], [], [], [], []],
-            509: [False, [], 0, [0,0,0,84], 0, "Sky Garden: Map 84 Switch", [], False, [], [], [], [], [], [], [], []],
-            511: [False, [], 0, [0,0,0,0], 0, "Mu: Water Lowered 1", [], False, [], [], [], [], [], [], [], []],
-            512: [False, [], 0, [0,0,0,0], 0, "Mu: Water Lowered 2", [], False, [], [], [], [], [], [], [], []],
-            514: [False, [], 0, [0,0,0,162], 0, "Mt Kress: Drops used 1", [], False, [], [], [], [], [], [], [], []],
-            515: [False, [], 0, [0,0,0,165], 0, "Mt Kress: Drops used 2", [], False, [], [], [], [], [], [], [], []],
-            516: [False, [], 0, [0,0,0,165], 0, "Mt Kress: Drops used 3", [], False, [], [], [], [], [], [], [], []],
-            517: [False, [], 0, [0,0,0,205], 0, "Pyramid: Hieroglyphs placed", [], False, [], [], [], [], [], [], [], []],
-            518: [False, [], 0, [0,0,0,242], 0, "Babel: Castoth defeated", [], False, [], [], [], [], [], [], [], []],
-            519: [False, [], 0, [0,0,0,243], 0, "Babel: Viper defeated", [], False, [], [], [], [], [], [], [], []],
-            520: [False, [], 0, [0,0,0,244], 0, "Babel: Vampires defeated", [], False, [], [], [], [], [], [], [], []],
-            521: [False, [], 0, [0,0,0,245], 0, "Babel: Sand Fanger defeated", [], False, [], [], [], [], [], [], [], []],
-            522: [False, [], 0, [0,0,0,246], 0, "Babel: Mummy Queen defeated", [], False, [], [], [], [], [], [], [], []],
-            523: [False, [], 0, [0,0,0,234], 0, "Mansion: Solid Arm defeated", [], False, [], [], [], [], [], [], [], []],
-            525: [False, [], 0, [0,0,0,0], 0, "Pyramid: Portals Open", [], False, [], [], [], [], [], [], [], []],
-            526: [False, [], 0, [0,0,0,0], 0, "Mu: Access to Hope Room 1", [], False, [], [], [], [], [], [], [], []],
-            527: [False, [], 0, [0,0,0,0], 0, "Mu: Access to Hope Room 2", [], False, [], [], [], [], [], [], [], []],
-            529: [False, [], 0, [0,0,0,0], 0, "Underground Tunnel: Bridge Open", [], False, [], [], [], [], [], [], [], []],
-            530: [False, [80, 81], 0, [0,0,0,0], 0, "Inca: Slug Statue Open", [], False, [], [], [], [], [], [], [], []],
-            531: [False, [], 0, [0,0,0,0], 0, "Mu: Beat Vampires", [], False, [], [], [], [], [], [], [], []]
+            500: [False, [], 0, [0, 0, 0, 0], 0, "Kara", [], False, [], [], [], [], [], [], [], []],
+            502: [False, [], 0, [0, 0, 0, 26], 0, "Moon Tribe: Spirits Healed", [], False, [], [], [], [], [], [], [],
+                  []],
+            503: [False, [], 0, [0, 0, 0, 0], 0, "Inca: Castoth Defeated", [], False, [], [], [], [], [], [], [], []],
+            505: [False, [], 0, [0, 0, 0, 0], 0, "Neil's Memory Restored", [], False, [], [], [], [], [], [], [], []],
+            508: [False, [], 0, [0, 0, 0, 82], 0, "Sky Garden: Map 82 SE Switch", [], False, [], [], [], [], [], [], [],
+                  []],
+            509: [False, [], 0, [0, 0, 0, 84], 0, "Sky Garden: Map 84 Switch", [], False, [], [], [], [], [], [], [],
+                  []],
+            511: [False, [], 0, [0, 0, 0, 0], 0, "Mu: Water Lowered 1", [], False, [], [], [], [], [], [], [], []],
+            512: [False, [], 0, [0, 0, 0, 0], 0, "Mu: Water Lowered 2", [], False, [], [], [], [], [], [], [], []],
+            514: [False, [], 0, [0, 0, 0, 162], 0, "Mt Kress: Drops used 1", [], False, [], [], [], [], [], [], [], []],
+            515: [False, [], 0, [0, 0, 0, 165], 0, "Mt Kress: Drops used 2", [], False, [], [], [], [], [], [], [], []],
+            516: [False, [], 0, [0, 0, 0, 165], 0, "Mt Kress: Drops used 3", [], False, [], [], [], [], [], [], [], []],
+            517: [False, [], 0, [0, 0, 0, 205], 0, "Pyramid: Hieroglyphs placed", [], False, [], [], [], [], [], [], [],
+                  []],
+            518: [False, [], 0, [0, 0, 0, 242], 0, "Babel: Castoth defeated", [], False, [], [], [], [], [], [], [],
+                  []],
+            519: [False, [], 0, [0, 0, 0, 243], 0, "Babel: Viper defeated", [], False, [], [], [], [], [], [], [], []],
+            520: [False, [], 0, [0, 0, 0, 244], 0, "Babel: Vampires defeated", [], False, [], [], [], [], [], [], [],
+                  []],
+            521: [False, [], 0, [0, 0, 0, 245], 0, "Babel: Sand Fanger defeated", [], False, [], [], [], [], [], [], [],
+                  []],
+            522: [False, [], 0, [0, 0, 0, 246], 0, "Babel: Mummy Queen defeated", [], False, [], [], [], [], [], [], [],
+                  []],
+            523: [False, [], 0, [0, 0, 0, 234], 0, "Mansion: Solid Arm defeated", [], False, [], [], [], [], [], [], [],
+                  []],
+            525: [False, [], 0, [0, 0, 0, 0], 0, "Pyramid: Portals Open", [], False, [], [], [], [], [], [], [], []],
+            526: [False, [], 0, [0, 0, 0, 0], 0, "Mu: Access to Hope Room 1", [], False, [], [], [], [], [], [], [],
+                  []],
+            527: [False, [], 0, [0, 0, 0, 0], 0, "Mu: Access to Hope Room 2", [], False, [], [], [], [], [], [], [],
+                  []],
+            529: [False, [], 0, [0, 0, 0, 0], 0, "Underground Tunnel: Bridge Open", [], False, [], [], [], [], [], [],
+                  [], []],
+            530: [False, [80, 81], 0, [0, 0, 0, 0], 0, "Inca: Slug Statue Open", [], False, [], [], [], [], [], [], [],
+                  []],
+            531: [False, [], 0, [0, 0, 0, 0], 0, "Mu: Beat Vampires", [], False, [], [], [], [], [], [], [], []]
 
         }
 
-
         # Shell logical paths for the world graph. Edges for exits etc. are added during initialization.
         # IsBidirectional is only used during initialization, and is False afterward.
         # Format: { ID: [0: Status(-1=restricted,0=locked,1=unlocked,2=forced_open), 
         #                1: StartRegion, 
         #                2: DestRegion, 
         #                3: Form flags (same as self.graph; 0 to inherit from items), 
         #                4: [[item1, qty1],[item2,qty2],...],
         #                5: IsBidirectional
         #               ] }
         self.deleted_logic = {}
         self.logic = {
             # Jeweler Rewards
-            0:  [0, 1, 2, 0, [[1, gem[0]]], False],  # Jeweler Reward 1
-            1:  [0, 1, 2, 0, [[1, gem[0] - 2], [41, 1]], False],
-            2:  [0, 1, 2, 0, [[1, gem[0] - 3], [42, 1]], False],
-            3:  [0, 1, 2, 0, [[1, gem[0] - 5], [41, 1], [42, 1]], False],
-            4:  [0, 2, 3, 0, [[1, gem[1]]], False],  # Jeweler Reward 2
-            5:  [0, 2, 3, 0, [[1, gem[1] - 2], [41, 1]], False],
-            6:  [0, 2, 3, 0, [[1, gem[1] - 3], [42, 1]], False],
-            7:  [0, 2, 3, 0, [[1, gem[1] - 5], [41, 1], [42, 1]], False],
-            8:  [0, 3, 4, 0, [[1, gem[2]]], False],  # Jeweler Reward 3
-            9:  [0, 3, 4, 0, [[1, gem[2] - 2], [41, 1]], False],
+            0: [0, 1, 2, 0, [[1, gem[0]]], False],  # Jeweler Reward 1
+            1: [0, 1, 2, 0, [[1, gem[0] - 2], [41, 1]], False],
+            2: [0, 1, 2, 0, [[1, gem[0] - 3], [42, 1]], False],
+            3: [0, 1, 2, 0, [[1, gem[0] - 5], [41, 1], [42, 1]], False],
+            4: [0, 2, 3, 0, [[1, gem[1]]], False],  # Jeweler Reward 2
+            5: [0, 2, 3, 0, [[1, gem[1] - 2], [41, 1]], False],
+            6: [0, 2, 3, 0, [[1, gem[1] - 3], [42, 1]], False],
+            7: [0, 2, 3, 0, [[1, gem[1] - 5], [41, 1], [42, 1]], False],
+            8: [0, 3, 4, 0, [[1, gem[2]]], False],  # Jeweler Reward 3
+            9: [0, 3, 4, 0, [[1, gem[2] - 2], [41, 1]], False],
             10: [0, 3, 4, 0, [[1, gem[2] - 3], [42, 1]], False],
             11: [0, 3, 4, 0, [[1, gem[2] - 5], [41, 1], [42, 1]], False],
             12: [0, 4, 5, 0, [[1, gem[3]]], False],  # Jeweler Reward 4
             13: [0, 4, 5, 0, [[1, gem[3] - 2], [41, 1]], False],
             14: [0, 4, 5, 0, [[1, gem[3] - 3], [42, 1]], False],
             15: [0, 4, 5, 0, [[1, gem[3] - 5], [41, 1], [42, 1]], False],
             16: [0, 5, 6, 0, [[1, gem[4]]], False],  # Jeweler Reward 5
@@ -4426,228 +4831,250 @@
             23: [0, 6, 7, 0, [[1, gem[5] - 5], [41, 1], [42, 1]], False],
             24: [0, 7, 8, 0, [[1, gem[6]]], False],  # Jeweler Reward 7 (Mansion)
             25: [0, 7, 8, 0, [[1, gem[6] - 2], [41, 1]], False],
             26: [0, 7, 8, 0, [[1, gem[6] - 3], [42, 1]], False],
             27: [0, 7, 8, 0, [[1, gem[6] - 5], [41, 1], [42, 1]], False],
 
             # Inter-Continental Travel
-            30: [0, 28,   15, 0, [[37, 1]], False],   # South Cape: Erik w/ Lola's Letter
-            31: [0, 102,  15, 0, [[37, 1]], False],   # Coast: Turbo w/ Lola's Letter
-            32: [0, 280,  15, 0, [[37, 1]], False],   # Watermia: Bridgeman w/ Lola's Letter
-            33: [0, 160, 161, 0, [[13, 1], [611, 1]], False],   # Neil's: Neil w/ Memory Melody
-            34: [0, 314,  17, 0, [[505, 1]], False],  # Euro: Neil w/ Memory restored
-            35: [0, 402,  17, 0, [[505, 1]], False],  # Dao: Neil w/ Memory restored
-            36: [0,  60,  64, 0, [[25, 1]], False],   # Moon Tribe healed w/ Teapot
-            37: [0, 170,  16, 0, [[502, 1]], False],  # Sky Garden: Spirits w/ spirits healed
-            38: [0, 280, 288, 0, [[24, 1]], False],   # Watermia: Stablemaster w/ Will
-            39: [0, 310, 311, 0, [[24, 1]], False],   # Euro: Stablemaster w/ Will
-            40: [0, 350, 351, 0, [[10, 1]], False],   # Natives': Child Guide w/ Large Roast
+            30: [0, 28, 15, 0, [[37, 1]], False],  # South Cape: Erik w/ Lola's Letter
+            31: [0, 102, 15, 0, [[37, 1]], False],  # Coast: Turbo w/ Lola's Letter
+            32: [0, 280, 15, 0, [[37, 1]], False],  # Watermia: Bridgeman w/ Lola's Letter
+            33: [0, 160, 161, 0, [[13, 1], [611, 1]], False],  # Neil's: Neil w/ Memory Melody
+            34: [0, 314, 17, 0, [[505, 1]], False],  # Euro: Neil w/ Memory restored
+            35: [0, 402, 17, 0, [[505, 1]], False],  # Dao: Neil w/ Memory restored
+            36: [0, 60, 64, 0, [[25, 1]], False],  # Moon Tribe healed w/ Teapot
+            37: [0, 170, 16, 0, [[502, 1]], False],  # Sky Garden: Spirits w/ spirits healed
+            38: [0, 280, 288, 0, [[24, 1]], False],  # Watermia: Stablemaster w/ Will
+            39: [0, 310, 311, 0, [[24, 1]], False],  # Euro: Stablemaster w/ Will
+            40: [0, 350, 351, 0, [[10, 1]], False],  # Natives': Child Guide w/ Large Roast
 
             # Edward's / Tunnel
-            60: [0, 32, 33,     0, [[2, 1]], True],     # Escape/Enter cell w/Prison Key
-            59: [0, 38, 42,     0, [[608, 1]], True],   # Pass statues with a Will ability
-            61: [0, 38, 42,     0, [[612, 1]], True],   # Pass statues with telekinesis
-            62: [0, 42, 39,     0, [[609, 1]], False],  # Pass spike balls to chest with any attack
-            703: [0,47, 720,    0, [[704, 1]], True],   # Worm orb opens Dark Space
-            63: [0, 47 ,529, 0x06, [], False],          # Open bridge via F/S
-            64: [0, 47, 704,    0, [[529, 1]], True],   # Traverse bridge to 2nd area
-            704: [0,704,705,    0, [[705, 1]], True],   # Skeleton barrier between 2nd and 3rd areas
-            705: [0,705,706,    0, [[706, 1]], True],   # Skeleton barrier between 3rd and final areas
+            60: [0, 32, 33, 0, [[2, 1]], True],  # Escape/Enter cell w/Prison Key
+            59: [0, 38, 42, 0, [[608, 1]], True],  # Pass statues with a Will ability
+            61: [0, 38, 42, 0, [[612, 1]], True],  # Pass statues with telekinesis
+            62: [0, 42, 39, 0, [[609, 1]], False],  # Pass spike balls to chest with any attack
+            703: [0, 47, 720, 0, [[704, 1]], True],  # Worm orb opens Dark Space
+            63: [0, 47, 529, 0x06, [], False],  # Open bridge via F/S
+            64: [0, 47, 704, 0, [[529, 1]], True],  # Traverse bridge to 2nd area
+            704: [0, 704, 705, 0, [[705, 1]], True],  # Skeleton barrier between 2nd and 3rd areas
+            705: [0, 705, 706, 0, [[706, 1]], True],  # Skeleton barrier between 3rd and final areas
 
             # Itory
-            70: [0, 50, 51, 0, [[9, 1], [611, 1]], False],     # Town appears w/ Lola's Melody
+            70: [0, 50, 51, 0, [[9, 1], [611, 1]], False],  # Town appears w/ Lola's Melody
 
             # Moon Tribe
-            80: [0, 61, 62, 0, [[608, 1]], False],   # Cave challenge w/ Will ability
-            600:[0, 61, 62 if settings.allow_glitches else 61, 0, [[604, 1]], False],   # Cave challenge itemless w/ glitches and flute
+            80: [0, 61, 62, 0, [[608, 1]], False],  # Cave challenge w/ Will ability
+            600: [0, 61, 62 if settings.allow_glitches else 61, 0, [[604, 1]], False],
+            # Cave challenge itemless w/ glitches and flute
 
             # Inca / Gold Ship / Freejia
-            88:  [0,  99,  75 if self.coupled_exits else 99, 0, [], False],  # Materialize Z-ladder door coupling if applicable
-            89:  [0,  72,  99 if self.enemizer == "None" and settings.allow_glitches else 72, 0, [], False],  # Map 29 progression w/ Z-ladder glitch
-            706: [0,  72,  70,     0, [[709, 1], [801, 1]], True],  # Inca exterior (29) N<->NE via 4-Way orb, ignored during dungeon construction
-            707: [0,  74,  72,     0, [[707, 1], [801, 1]], True],  # Inca exterior (29) SW<->N via 4-Way orb, ignored during dungeon construction
-            708: [0,  75,  72,     0, [[708, 1], [801, 1]], True],  # Inca exterior (29) SE<->N via 4-Way orb, ignored during dungeon construction
-            700: [0,  73, 700,     0, [[64, 1], [54, 2]], False],   # Inca west 4-Way orb from C with upgraded Friar
-            90:  [0,  77,  78,     0, [[3, 1], [4, 1]], False],  # Map 30 to Castoth w/ Inca Statues
-            91:  [0,  80,  530,    0, [[608, 1]], False],        # Break blocking slug statue w/ Will ability
-            92:  [0,  81,  530,    0, [[608, 1]], False],        # Break blocking slug statue w/ Will ability
-            93:  [0,  80,  81,     0, [[530, 1]], True],         # Passage after blocking slug statue is broken
-            710: [0,  82,  83,     0, [[710, 1]], False],        # Inca N/S ramp (33) via whirligig orb
-            94:  [0,  85, 707,  0x06, [], False],                # Map 35 get orb w/ F/S
-            95:  [0,  85, 707,     0, [[610, 1]], False],        # Map 35 get orb w/ ranged
-            709: [0,  85,  86,     0, [[711, 1]], False],        # Inca E/W ramp (35) via whirligig orb
-            97:  [0,  91,  92,     0, [[608, 1]], False],        # Map 38 break statues w/ Will ability
-            711: [0,  96,  95,     0, [[713, 1]], False],        # Map 40 reverse via 4-Way orb
-            98:  [0,  95,  96,     0, [[609, 1]], False],        # DS spike hall requires an attack to pass the 4-Way
-            99:  [0,  97, 503,  0x06, [], False],                # Castoth as F/S
-            100: [0,  97, 503,     0, [[604, 1]], False],        # Castoth with Flute
-            101: [0,  97,  98,     0, [[503, 1]], False],        # Pass Castoth; if you add the exit behind Castoth to exits, move this to exit_logic
+            88: [0, 99, 75 if self.coupled_exits else 99, 0, [], False],
+            # Materialize Z-ladder door coupling if applicable
+            89: [0, 72, 99 if self.enemizer == "None" and settings.allow_glitches else 72, 0, [], False],
+            # Map 29 progression w/ Z-ladder glitch
+            706: [0, 72, 70, 0, [[709, 1], [801, 1]], True],
+            # Inca exterior (29) N<->NE via 4-Way orb, ignored during dungeon construction
+            707: [0, 74, 72, 0, [[707, 1], [801, 1]], True],
+            # Inca exterior (29) SW<->N via 4-Way orb, ignored during dungeon construction
+            708: [0, 75, 72, 0, [[708, 1], [801, 1]], True],
+            # Inca exterior (29) SE<->N via 4-Way orb, ignored during dungeon construction
+            700: [0, 73, 700, 0, [[64, 1], [54, 2]], False],  # Inca west 4-Way orb from C with upgraded Friar
+            90: [0, 77, 78, 0, [[3, 1], [4, 1]], False],  # Map 30 to Castoth w/ Inca Statues
+            91: [0, 80, 530, 0, [[608, 1]], False],  # Break blocking slug statue w/ Will ability
+            92: [0, 81, 530, 0, [[608, 1]], False],  # Break blocking slug statue w/ Will ability
+            93: [0, 80, 81, 0, [[530, 1]], True],  # Passage after blocking slug statue is broken
+            710: [0, 82, 83, 0, [[710, 1]], False],  # Inca N/S ramp (33) via whirligig orb
+            94: [0, 85, 707, 0x06, [], False],  # Map 35 get orb w/ F/S
+            95: [0, 85, 707, 0, [[610, 1]], False],  # Map 35 get orb w/ ranged
+            709: [0, 85, 86, 0, [[711, 1]], False],  # Inca E/W ramp (35) via whirligig orb
+            97: [0, 91, 92, 0, [[608, 1]], False],  # Map 38 break statues w/ Will ability
+            711: [0, 96, 95, 0, [[713, 1]], False],  # Map 40 reverse via 4-Way orb
+            98: [0, 95, 96, 0, [[609, 1]], False],  # DS spike hall requires an attack to pass the 4-Way
+            99: [0, 97, 503, 0x06, [], False],  # Castoth as F/S
+            100: [0, 97, 503, 0, [[604, 1]], False],  # Castoth with Flute
+            101: [0, 97, 98, 0, [[503, 1]], False],
+            # Pass Castoth; if you add the exit behind Castoth to exits, move this to exit_logic
 
             # Diamond Mine
-            712: [0, 130, 708,    0, [[715, 1]], True],            # Map 61 S fence progression via monster
-            713: [0, 708, 709,    0, [[714, 1]], True],            # Map 61 C fence progression via monster
-            714: [0, 709, 131,    0, [[716, 1]], True],            # Map 61 N fence progression via monster
-            702: [0, 709, 701,    0, [[610, 1]], False],           # Map 61 C lizard from N via ranged
-            715: [0, 136, 721,    0, [[718, 1]],  True],           # Map 64 appearing DS via worm orb
-            117: [0, 138, 139,    0, [[63, 1]],  False],           # Map 65 ramp access via Spin Dash
-            716: [0, 138, 139,    0, [[719, 1]], False],           # Map 65 ramp access via worm orb
-            118: [0, 138, 710,    0, [[610, 1]], False],           # Map 65 worm access via ranged
+            712: [0, 130, 708, 0, [[715, 1]], True],  # Map 61 S fence progression via monster
+            713: [0, 708, 709, 0, [[714, 1]], True],  # Map 61 C fence progression via monster
+            714: [0, 709, 131, 0, [[716, 1]], True],  # Map 61 N fence progression via monster
+            702: [0, 709, 701, 0, [[610, 1]], False],  # Map 61 C lizard from N via ranged
+            715: [0, 136, 721, 0, [[718, 1]], True],  # Map 64 appearing DS via worm orb
+            117: [0, 138, 139, 0, [[63, 1]], False],  # Map 65 ramp access via Spin Dash
+            716: [0, 138, 139, 0, [[719, 1]], False],  # Map 65 ramp access via worm orb
+            118: [0, 138, 710, 0, [[610, 1]], False],  # Map 65 worm access via ranged
 
             # Sky Garden
-            130: [0, 170, 171,     0, [[14, 4]], False],            # Boss access w/ Crystal Balls
-            131: [0, 177, 711,     0, [[610, 1]], False],           # SE Top (79) robot orb via ranged
-            718: [0, 177, 178,     0, [[720, 1]], True],            # SE Top (79) barrier via robot orb
-            720: [0, 180, 716,     0, [[721, 1]], True],            # SE Bot (80) chest via robot orb
-            721: [0, 181, 168,     0, [[722, 1]], True],            # SW Top (81) C<->N via robot orb
-            723: [0, 181, 182,     0, [[724, 1]], True],            # SW Top (81) C<->W via worm orb
-            133: [0, 168, 182,     0, [[506, 1]], True],            # SW Top progression w/ switch 1
-            134: [0, 182, 183,     0, [[507, 1]], True],            # SW Top progression w/ switch 2
-            135: [0, 182, 184,     0, [[608, 1]], True],            # SW Top break statues w/ Will ability
-            138: [0, 184, 185,     0, [[508, 1], [608, 1]], False], # SW Top ramp chest w/ switch 3 & Will ability
-            141: [0, 181, 182,     0, [[63, 1]], False],            # SW Top (81) ramps w/ Spin Dash
-            142: [0, 181, 184,     0, [[63, 1]], False],            # SW Top (81) ramps w/ Spin Dash
-            143: [0, 182, 185,     0, [[63, 1]], False],            # SW Top (81) ramps w/ Spin Dash
+            130: [0, 170, 171, 0, [[14, 4]], False],  # Boss access w/ Crystal Balls
+            131: [0, 177, 711, 0, [[610, 1]], False],  # SE Top (79) robot orb via ranged
+            718: [0, 177, 178, 0, [[720, 1]], True],  # SE Top (79) barrier via robot orb
+            720: [0, 180, 716, 0, [[721, 1]], True],  # SE Bot (80) chest via robot orb
+            721: [0, 181, 168, 0, [[722, 1]], True],  # SW Top (81) C<->N via robot orb
+            723: [0, 181, 182, 0, [[724, 1]], True],  # SW Top (81) C<->W via worm orb
+            133: [0, 168, 182, 0, [[506, 1]], True],  # SW Top progression w/ switch 1
+            134: [0, 182, 183, 0, [[507, 1]], True],  # SW Top progression w/ switch 2
+            135: [0, 182, 184, 0, [[608, 1]], True],  # SW Top break statues w/ Will ability
+            138: [0, 184, 185, 0, [[508, 1], [608, 1]], False],  # SW Top ramp chest w/ switch 3 & Will ability
+            141: [0, 181, 182, 0, [[63, 1]], False],  # SW Top (81) ramps w/ Spin Dash
+            142: [0, 181, 184, 0, [[63, 1]], False],  # SW Top (81) ramps w/ Spin Dash
+            143: [0, 182, 185, 0, [[63, 1]], False],  # SW Top (81) ramps w/ Spin Dash
             601: [0, 181, 182 if settings.allow_glitches else 181, 0, [], False],  # SW Top (81) ramps w/ glitches
             602: [0, 181, 184 if settings.allow_glitches else 181, 0, [], False],  # SW Top (81) ramps w/ glitches
             603: [0, 182, 185 if settings.allow_glitches else 182, 0, [], False],  # SW Top (81) ramps w/ glitches
-            739: [0, 187, 508,     0, [[725, 1], [609, 1], [612, 1]], False],   # SW Bot (82) switch via fire cage orb, attack, and telekinesis
-            144: [0, 188, 189,  0x06, [], False],                   # SW Bot (82) cage switch w/ reach
-            145: [0, 188, 189 if settings.allow_glitches else 188, 0, [[604, 1]], False], # SW Bot (82) cage switch w/ Glitches + Flute
-            146: [0, 192, 190,     0, [[63, 1]], False],            # NW Top (83) backward w/ Spin Dash
-            148: [0, 195, 509,     0, [[610, 1], [612, 1]], False], # NW Bot (84) statue w/ ranged and telekinesis
-            149: [0, 195, 509,     0, [[65, 1], [612, 1]], False],  # NW Bot (84) statue w/ Aura Barrier and telekinesis
-            150: [0, 195, 197,     0, [[509, 1]], True],            # NW Bot (84) traversal with statue switch
-            152: [0, 170,  16,     0, [[502, 1]], False],           # Moon Tribe passage w/ spirits healed
+            739: [0, 187, 508, 0, [[725, 1], [609, 1], [612, 1]], False],
+            # SW Bot (82) switch via fire cage orb, attack, and telekinesis
+            144: [0, 188, 189, 0x06, [], False],  # SW Bot (82) cage switch w/ reach
+            145: [0, 188, 189 if settings.allow_glitches else 188, 0, [[604, 1]], False],
+            # SW Bot (82) cage switch w/ Glitches + Flute
+            146: [0, 192, 190, 0, [[63, 1]], False],  # NW Top (83) backward w/ Spin Dash
+            148: [0, 195, 509, 0, [[610, 1], [612, 1]], False],  # NW Bot (84) statue w/ ranged and telekinesis
+            149: [0, 195, 509, 0, [[65, 1], [612, 1]], False],  # NW Bot (84) statue w/ Aura Barrier and telekinesis
+            150: [0, 195, 197, 0, [[509, 1]], True],  # NW Bot (84) traversal with statue switch
+            152: [0, 170, 16, 0, [[502, 1]], False],  # Moon Tribe passage w/ spirits healed
 
             # Mu
-            724: [0, 212, 722,  0, [[726, 1]], True],             # Mu entrance (95) gate via golem orb
-            171: [0, 212, 213,  0, [[511, 1]], True],             # Map 95 top-midE w/ water lowered 1
-            172: [0, 213, 215,  0, [[512, 1]], True],             # Map 95 midE-botE w/ water lowered 2
-            173: [0, 214, 216,  0, [[512, 1]], True],             # Map 95 midw-botW w/ water lowered 2
-            174: [0, 217, 218,  0, [[511, 1]], True],             # Map 96 top-mid w/ water lowered 1
-            726: [0, 217, 725,  0, [[727, 1]], True],             # Mu NE (96) N/S semiprogression via rocks
-            727: [0, 723, 725,  0, [[728, 1]], True],             # Mu NE (96) N/S semiprogression via rocks
-            753: [0, 723, 726,  0, [[610, 1]], False],            # Mu NE, N orb from S, via ranged
-            754: [0, 217, 724,  0, [[610, 1]], False],            # Mu NE, S orb from N, via ranged
-            175: [0, 222, 221,  0, [[511, 1], [610, 1]], False],  # Map 97 midN->island w/ water lowered 1 & ranged
-            176: [0, 222, 221 if settings.allow_glitches else 222,  0, [[511, 1]], False],  # Map 97 midN->island w/ water lowered 1 & glitches
-            178: [0, 226, 227,  0, [[511, 1]], True],             # Map 98 top-midE w/ water lowered 1
-            179: [0, 227, 229,  0, [[512, 1]], True],             # Map 98 midE-botE w/ water lowered 2
-            180: [0, 228, 230,  0, [[512, 1]], True],             # Map 98 midW-botW w/ water lowered 2
-            181: [0, 229, 230,  0, [[62, 1], [512, 1]], True],    # Map 98 W/E Slider hole
-            182: [0, 233, 245,  0, [[609, 1]], True],             # SW MidE spike buttons require an attack
-            184: [0, 237, 238,  0, [[62, 1], [511, 1]], True],    # Map 101 midW-midE w/ Psycho Slider
-            185: [0, 240, 241,  0, [[19, 2]], False],             # Map 102 progression w/ Rama Statues
-            186: [0, 526, 511,  0, [[18, 1]], False],             # Water lowered 1 w/ Hope Statue
-            187: [0, 527, 511,  0, [[18, 1]], False],             # Water lowered 1 w/ Hope Statue
-            188: [0, 526, 512,  0, [[18, 2], [527, 1], [511, 1]], False],  # Water lowered 2 w/ Hope Statues, both rooms, and water lowered 1
-            189: [0, 527, 512,  0, [[18, 2], [526, 1], [511, 1]], False],  # Water lowered 2 w/ Hope Statues, both rooms, and water lowered 1
-            190: [0, 244, 531,0x6, [], False],                    # Vampires as F/S
-            191: [0, 244, 531,  0, [[604 if self.difficulty < 3 else 609, 1]], False], # Vampires with Flute, or any attack if playing Extreme
-            192: [0, 244, 242,  0, [[531, 1]], False],            # Pass Vampires if defeated
+            724: [0, 212, 722, 0, [[726, 1]], True],  # Mu entrance (95) gate via golem orb
+            171: [0, 212, 213, 0, [[511, 1]], True],  # Map 95 top-midE w/ water lowered 1
+            172: [0, 213, 215, 0, [[512, 1]], True],  # Map 95 midE-botE w/ water lowered 2
+            173: [0, 214, 216, 0, [[512, 1]], True],  # Map 95 midw-botW w/ water lowered 2
+            174: [0, 217, 218, 0, [[511, 1]], True],  # Map 96 top-mid w/ water lowered 1
+            726: [0, 217, 725, 0, [[727, 1]], True],  # Mu NE (96) N/S semiprogression via rocks
+            727: [0, 723, 725, 0, [[728, 1]], True],  # Mu NE (96) N/S semiprogression via rocks
+            753: [0, 723, 726, 0, [[610, 1]], False],  # Mu NE, N orb from S, via ranged
+            754: [0, 217, 724, 0, [[610, 1]], False],  # Mu NE, S orb from N, via ranged
+            175: [0, 222, 221, 0, [[511, 1], [610, 1]], False],  # Map 97 midN->island w/ water lowered 1 & ranged
+            176: [0, 222, 221 if settings.allow_glitches else 222, 0, [[511, 1]], False],
+            # Map 97 midN->island w/ water lowered 1 & glitches
+            178: [0, 226, 227, 0, [[511, 1]], True],  # Map 98 top-midE w/ water lowered 1
+            179: [0, 227, 229, 0, [[512, 1]], True],  # Map 98 midE-botE w/ water lowered 2
+            180: [0, 228, 230, 0, [[512, 1]], True],  # Map 98 midW-botW w/ water lowered 2
+            181: [0, 229, 230, 0, [[62, 1], [512, 1]], True],  # Map 98 W/E Slider hole
+            182: [0, 233, 245, 0, [[609, 1]], True],  # SW MidE spike buttons require an attack
+            184: [0, 237, 238, 0, [[62, 1], [511, 1]], True],  # Map 101 midW-midE w/ Psycho Slider
+            185: [0, 240, 241, 0, [[19, 2]], False],  # Map 102 progression w/ Rama Statues
+            186: [0, 526, 511, 0, [[18, 1]], False],  # Water lowered 1 w/ Hope Statue
+            187: [0, 527, 511, 0, [[18, 1]], False],  # Water lowered 1 w/ Hope Statue
+            188: [0, 526, 512, 0, [[18, 2], [527, 1], [511, 1]], False],
+            # Water lowered 2 w/ Hope Statues, both rooms, and water lowered 1
+            189: [0, 527, 512, 0, [[18, 2], [526, 1], [511, 1]], False],
+            # Water lowered 2 w/ Hope Statues, both rooms, and water lowered 1
+            190: [0, 244, 531, 0x6, [], False],  # Vampires as F/S
+            191: [0, 244, 531, 0, [[604 if self.difficulty < 3 else 609, 1]], False],
+            # Vampires with Flute, or any attack if playing Extreme
+            192: [0, 244, 242, 0, [[531, 1]], False],  # Pass Vampires if defeated
 
             # Angel Dungeon
-            214: [0, 272, 273, 0, [[513, 1]], False],   # Ishtar's chest w/ puzzle complete
-            215: [0, 261, 278, 0, [[609, 1]], True],    # Passing a Draco requires an attack
-            216: [0, 263, 279, 0, [[609, 1]], True],    # Passing a Draco requires an attack
+            214: [0, 272, 273, 0, [[513, 1]], False],  # Ishtar's chest w/ puzzle complete
+            215: [0, 261, 278, 0, [[609, 1]], True],  # Passing a Draco requires an attack
+            216: [0, 263, 279, 0, [[609, 1]], True],  # Passing a Draco requires an attack
 
             # Great Wall
-            218: [0, 292, 293,     0, [[609, 1]], False],           # Drop room forward requires an attack for the button
-            219: [0, 293, 291,     0, [[63, 1]], True],             # Map 131 (drop room) backwards w/ Spin Dash
-            220: [0, 296, 295 if settings.allow_glitches else 296, 0, [[604, 1]], False], # Map 133 E->C w/ glitches and Flute
-            221: [0, 296, 295,     0, [[63, 1]], False],            # Map 133 E->C w/ Spin Dash
-            222: [0, 296, 295,  0x06, [], False],                   # Map 133 E->C w/ Freedan or Shadow
-            223: [0, 296, 294,     0, [[63, 1]], False],            # Map 133 C->W w/ Spin Dash
-            728: [0, 298, 299,     0, [[732, 1]], True],            # Map 135 progression w/ archer orb
-            227: [0, 298, 712,     0, [[610, 1]], False],           # Map 135 archer via ranged
-            228: [0, 299, 712,     0, [[610, 1]], False],           # Map 135 archer via ranged
-            229: [0, 300, 301,     0, [[63, 1]], True],             # Map 136 progression w/ Spin Dash
+            218: [0, 292, 293, 0, [[609, 1]], False],  # Drop room forward requires an attack for the button
+            219: [0, 293, 291, 0, [[63, 1]], True],  # Map 131 (drop room) backwards w/ Spin Dash
+            220: [0, 296, 295 if settings.allow_glitches else 296, 0, [[604, 1]], False],
+            # Map 133 E->C w/ glitches and Flute
+            221: [0, 296, 295, 0, [[63, 1]], False],  # Map 133 E->C w/ Spin Dash
+            222: [0, 296, 295, 0x06, [], False],  # Map 133 E->C w/ Freedan or Shadow
+            223: [0, 296, 294, 0, [[63, 1]], False],  # Map 133 C->W w/ Spin Dash
+            728: [0, 298, 299, 0, [[732, 1]], True],  # Map 135 progression w/ archer orb
+            227: [0, 298, 712, 0, [[610, 1]], False],  # Map 135 archer via ranged
+            228: [0, 299, 712, 0, [[610, 1]], False],  # Map 135 archer via ranged
+            229: [0, 300, 301, 0, [[63, 1]], True],  # Map 136 progression w/ Spin Dash
 
             # Mt. Temple
-            240: [0, 331, 332, 0, [[63, 1]], True],              # Map 161 progression w/ Spin Dash
-            242: [0, 333, 514, 0, [[26, 1 if not self.dungeon_shuffle else 3]], False],   # Use Mushroom drops 1
-            750: [0, 333, 335, 0, [[514, 1]], True],             # Drops vine 1
-            244: [0, 339, 515, 0, [[26, 2 if not self.dungeon_shuffle else 3]], False],   # Use Mushroom drops 2
-            751: [0, 339, 340, 0, [[515, 1]], True],             # Drops vine 2
-            246: [0, 340, 516, 0, [[26, 3]], False],             # Use Mushroom drops 3
-            752: [0, 340, 341, 0, [[516, 1]], True],             # Drops vine 3
+            240: [0, 331, 332, 0, [[63, 1]], True],  # Map 161 progression w/ Spin Dash
+            242: [0, 333, 514, 0, [[26, 1 if not self.dungeon_shuffle else 3]], False],  # Use Mushroom drops 1
+            750: [0, 333, 335, 0, [[514, 1]], True],  # Drops vine 1
+            244: [0, 339, 515, 0, [[26, 2 if not self.dungeon_shuffle else 3]], False],  # Use Mushroom drops 2
+            751: [0, 339, 340, 0, [[515, 1]], True],  # Drops vine 2
+            246: [0, 340, 516, 0, [[26, 3]], False],  # Use Mushroom drops 3
+            752: [0, 340, 341, 0, [[516, 1]], True],  # Drops vine 3
 
             # Natives'
-            250: [0, 353, 354, 0, [[29, 1]], False],    # Statues awake w/ Gorgon Flower
+            250: [0, 353, 354, 0, [[29, 1]], False],  # Statues awake w/ Gorgon Flower
 
             # Ankor Wat
-            260: [0, 361, 739,    0, [[64, 1], [54, 2]], False],    # Map 177 orb w/ upgraded Friar
-            729: [0, 361, 362,    0, [[735, 1], [801, 1]], True],   # Wat Outer South (177) via scarab orb, ignored during dungeon construction
-            261: [0, 363, 364,    0, [[63, 1]], False],             # Map 178 S->C w/ Spin Dash
-            262: [0, 364, 365,    0, [[62, 1], [736, 1]], False],   # Map 178 C->N w/ Psycho Slider and scarab key
-            263: [0, 365, 364,    0, [[62, 1]], False],             # Map 178 N->C w/ Psycho Slider
-            264: [0, 367, 366,    0, [[63, 1]], False],             # Map 179 W->E w/ Spin Dash
-            265: [0, 369, 370,    0, [[62, 1]], False],             # Map 181 N->C w/ Psycho Slider
-            266: [0, 370, 371,    0, [[63, 1]], False],             # Map 181 C->S w/ Spin Dash
-            267: [0, 373, 374,    0, [[66, 1]], False],             # Map 183 S->NW w/ Earthquaker
-            268: [0, 373, 374,    0, [[64, 1], [54, 2]], False],    # Map 183 S->NW w/ upgraded Friar
-            269: [0, 373, 374 if settings.allow_glitches else 373, 0, [[64, 1]], False],   # Map 183 S->NW w/ Friar and glitches
-            271: [0, 376, 727,    0, [[64, 1]], False],             # Map 184 orb access via Friar
-            272: [0, 376, 727,    0, [[36, 1]], False],             # Map 184 orb access via Shadow
-            731: [0, 376, 377,    0, [[738, 1]], True],             # Map 184 S<->N w/ skull orb
-            273: [0, 384, 385 if settings.allow_glitches else 384, 0, [[62, 1]], True],    # Map 188 S-N w/ Slider and glitches
-            274: [0, 384, 385,    0, [[62, 1], [28, 1]], True],     # Map 188 S-N w/ Slider and Glasses
-            275: [0, 386, 387,    0, [[62, 1]], True],              # Map 189 S-N w/ Slider
+            260: [0, 361, 739, 0, [[64, 1], [54, 2]], False],  # Map 177 orb w/ upgraded Friar
+            729: [0, 361, 362, 0, [[735, 1], [801, 1]], True],
+            # Wat Outer South (177) via scarab orb, ignored during dungeon construction
+            261: [0, 363, 364, 0, [[63, 1]], False],  # Map 178 S->C w/ Spin Dash
+            262: [0, 364, 365, 0, [[62, 1], [736, 1]], False],  # Map 178 C->N w/ Psycho Slider and scarab key
+            263: [0, 365, 364, 0, [[62, 1]], False],  # Map 178 N->C w/ Psycho Slider
+            264: [0, 367, 366, 0, [[63, 1]], False],  # Map 179 W->E w/ Spin Dash
+            265: [0, 369, 370, 0, [[62, 1]], False],  # Map 181 N->C w/ Psycho Slider
+            266: [0, 370, 371, 0, [[63, 1]], False],  # Map 181 C->S w/ Spin Dash
+            267: [0, 373, 374, 0, [[66, 1]], False],  # Map 183 S->NW w/ Earthquaker
+            268: [0, 373, 374, 0, [[64, 1], [54, 2]], False],  # Map 183 S->NW w/ upgraded Friar
+            269: [0, 373, 374 if settings.allow_glitches else 373, 0, [[64, 1]], False],
+            # Map 183 S->NW w/ Friar and glitches
+            271: [0, 376, 727, 0, [[64, 1]], False],  # Map 184 orb access via Friar
+            272: [0, 376, 727, 0, [[36, 1]], False],  # Map 184 orb access via Shadow
+            731: [0, 376, 377, 0, [[738, 1]], True],  # Map 184 S<->N w/ skull orb
+            273: [0, 384, 385 if settings.allow_glitches else 384, 0, [[62, 1]], True],
+            # Map 188 S-N w/ Slider and glitches
+            274: [0, 384, 385, 0, [[62, 1], [28, 1]], True],  # Map 188 S-N w/ Slider and Glasses
+            275: [0, 386, 387, 0, [[62, 1]], True],  # Map 189 S-N w/ Slider
 
             # Pyramid
-            290: [0, 410, 411,    0, [[62, 1]], True],              # Map 204 pass orbs w/ Slider
-            291: [0, 410, 411,    0, [[63, 1]], True],              # Map 204 pass orbs w/ Spin
-            292: [0, 410, 411 if settings.allow_glitches else 410, 0, [], True], # Map 204 pass orbs w/ "glitches"
-            736: [0, 411, 713,    0, [[739, 1]], False],            # Map 204 top DS w/ orb orb
-            293: [0, 713, 412,    0, [[36, 1], [739, 1]], False],   # Map 204 progression w/ Aura and DS orb
-            294: [0, 713, 413,    0, [[36, 1], [739, 1]], False],   # Map 204 progression w/ Aura and DS orb
-            295: [0, 415, 449,    0, [[30, 1], [31, 1], [32, 1], [33, 1], [34, 1], [35, 1], [38, 1]], False],   # Boss w/ Hieros+Journal
-            296: [0, 416, 417,    0, [[63, 1]], True],              # Map 206 progression w/ Spin Dash
-            298: [0, 418, 419,    0, [[63, 1]], True],              # Map 207 progression w/ Spin Dash
-            300: [0, 426, 427,    0, [[36, 1]], False],             # Map 212 progression w/ Aura
-            301: [0, 426, 427,    0, [[66, 1]], False],             # Map 212 progression w/ Earthquaker
-            302: [0, 427, 428,    0, [[36, 1]], False],             # Map 212 to SE chest w/ Aura
-            303: [0, 427, 429,    0, [[36, 1]], False],             # Map 212 progression w/ Aura
-            304: [0, 427, 429,    0, [[66, 1]], False],             # Map 212 progression w/ Earthquaker
-            305: [0, 431, 432,    0, [[63, 1]], True],              # Map 214 to NE chest w/ Spin Dash
-            306: [0, 431, 434,    0, [[36, 1]], False],             # Map 214 progression w/ Aura
-            307: [0, 431, 433,    0, [[64, 1]], False],             # Map 214 progression w/ Friar
-            308: [0, 438, 439,    0, [[63, 1]], True],              # Map 217 progression w/ Spin Dash
-            310: [0, 440, 441,    0, [[63, 1]], True],              # Map 219 progression w/ Spin Dash
-            309: [0, 435, 450,    0, [[63, 1]], True],              # Killer 6 w/ Spin Dash
-            312: [0, 435, 450,    0, [[6, 6], [50, 2], [51, 1], [52, 1]], True],  # Killer 6 w/ herbs and stats
-            313: [0, 435, 450,    0, [[64, 1], [54, 1]], True],     # Killer 6 w/ Friar II
-            314: [0, 411, 414,    0, [[517, 1]], False],            # Pyramid to boss w/hieroglyphs placed
-            516: [0, 413, 411,    0, [[525, 1]], False],            # Pyramid portal
-            517: [0, 419, 411,    0, [[525, 1]], False],            # Pyramid portal
-            518: [0, 423, 411,    0, [[525, 1]], False],            # Pyramid portal
-            519: [0, 425, 411,    0, [[525, 1]], False],            # Pyramid portal
-            520: [0, 428, 411,    0, [[525, 1]], False],            # Pyramid portal
-            521: [0, 430, 411,    0, [[525, 1]], False],            # Pyramid portal
-            522: [0, 437, 411,    0, [[525, 1]], False],            # Pyramid portal
-            523: [0, 441, 411,    0, [[525, 1]], False],            # Pyramid portal
-            524: [0, 450, 411,    0, [[525, 1]], False],            # Pyramid portal
-            525: [0,   0, 525, 0x0f, [] if not self.dungeon_shuffle else [[36, 1]], False], # Portals require Aura in dungeon shuffle
+            290: [0, 410, 411, 0, [[62, 1]], True],  # Map 204 pass orbs w/ Slider
+            291: [0, 410, 411, 0, [[63, 1]], True],  # Map 204 pass orbs w/ Spin
+            292: [0, 410, 411 if settings.allow_glitches else 410, 0, [], True],  # Map 204 pass orbs w/ "glitches"
+            736: [0, 411, 713, 0, [[739, 1]], False],  # Map 204 top DS w/ orb orb
+            293: [0, 713, 412, 0, [[36, 1], [739, 1]], False],  # Map 204 progression w/ Aura and DS orb
+            294: [0, 713, 413, 0, [[36, 1], [739, 1]], False],  # Map 204 progression w/ Aura and DS orb
+            295: [0, 415, 449, 0, [[30, 1], [31, 1], [32, 1], [33, 1], [34, 1], [35, 1], [38, 1]], False],
+            # Boss w/ Hieros+Journal
+            296: [0, 416, 417, 0, [[63, 1]], True],  # Map 206 progression w/ Spin Dash
+            298: [0, 418, 419, 0, [[63, 1]], True],  # Map 207 progression w/ Spin Dash
+            300: [0, 426, 427, 0, [[36, 1]], False],  # Map 212 progression w/ Aura
+            301: [0, 426, 427, 0, [[66, 1]], False],  # Map 212 progression w/ Earthquaker
+            302: [0, 427, 428, 0, [[36, 1]], False],  # Map 212 to SE chest w/ Aura
+            303: [0, 427, 429, 0, [[36, 1]], False],  # Map 212 progression w/ Aura
+            304: [0, 427, 429, 0, [[66, 1]], False],  # Map 212 progression w/ Earthquaker
+            305: [0, 431, 432, 0, [[63, 1]], True],  # Map 214 to NE chest w/ Spin Dash
+            306: [0, 431, 434, 0, [[36, 1]], False],  # Map 214 progression w/ Aura
+            307: [0, 431, 433, 0, [[64, 1]], False],  # Map 214 progression w/ Friar
+            308: [0, 438, 439, 0, [[63, 1]], True],  # Map 217 progression w/ Spin Dash
+            310: [0, 440, 441, 0, [[63, 1]], True],  # Map 219 progression w/ Spin Dash
+            309: [0, 435, 450, 0, [[63, 1]], True],  # Killer 6 w/ Spin Dash
+            312: [0, 435, 450, 0, [[6, 6], [50, 2], [51, 1], [52, 1]], True],  # Killer 6 w/ herbs and stats
+            313: [0, 435, 450, 0, [[64, 1], [54, 1]], True],  # Killer 6 w/ Friar II
+            314: [0, 411, 414, 0, [[517, 1]], False],  # Pyramid to boss w/hieroglyphs placed
+            516: [0, 413, 411, 0, [[525, 1]], False],  # Pyramid portal
+            517: [0, 419, 411, 0, [[525, 1]], False],  # Pyramid portal
+            518: [0, 423, 411, 0, [[525, 1]], False],  # Pyramid portal
+            519: [0, 425, 411, 0, [[525, 1]], False],  # Pyramid portal
+            520: [0, 428, 411, 0, [[525, 1]], False],  # Pyramid portal
+            521: [0, 430, 411, 0, [[525, 1]], False],  # Pyramid portal
+            522: [0, 437, 411, 0, [[525, 1]], False],  # Pyramid portal
+            523: [0, 441, 411, 0, [[525, 1]], False],  # Pyramid portal
+            524: [0, 450, 411, 0, [[525, 1]], False],  # Pyramid portal
+            525: [0, 0, 525, 0x0f, [] if not self.dungeon_shuffle else [[36, 1]], False],
+            # Portals require Aura in dungeon shuffle
 
             # Babel / Mansion items 740,741
-            320: [0, 461, 462, 0x0f, [[36, 1], [39, 1]], False],    # Map 223 w/ Aura and Ring, any form
-            321: [0, 473, 479,    0, [[522, 1]], False],            # Olman statue w/ Mummy Queen 2
-            322: [0, 473, 479,    0, [[523, 1]], False],            # Olman statue w/ Solid Arm
-            732: [0, 480, 714,    0, [[740, 1]], True],             # Mansion east gate with monster orb
-            734: [0, 714, 715,    0, [[741, 1]], True],             # Mansion west gate with monster orb
-            323: [0, 715, 481,    0, [[62, 1]], True],              # Mansion progression w/ Slider
+            320: [0, 461, 462, 0x0f, [[36, 1], [39, 1]], False],  # Map 223 w/ Aura and Ring, any form
+            321: [0, 473, 479, 0, [[522, 1]], False],  # Olman statue w/ Mummy Queen 2
+            322: [0, 473, 479, 0, [[523, 1]], False],  # Olman statue w/ Solid Arm
+            732: [0, 480, 714, 0, [[740, 1]], True],  # Mansion east gate with monster orb
+            734: [0, 714, 715, 0, [[741, 1]], True],  # Mansion west gate with monster orb
+            323: [0, 715, 481, 0, [[62, 1]], True],  # Mansion progression w/ Slider
             # Solid Arm always warps to top of Babel, but only Extreme difficulty has an edge to include the warp in logic;
             # this prevents rare scenarios where the traverser would path through Solid Arm to warp to another continent.
             324: [0, 482, 482 if self.difficulty < 3 else 472, 0, [], False],
 
             # Endgame / Misc
-            400: [0, [49,150,270,345,391][self.kara - 1], 490, 0, [[20, 1]], False],   # Rescue Kara w/ Magic Dust
-            405: [0, 490, 491, 0x0f, [[36, 1], [39, 1], [602, 1]], False],    # (Early) Firebird w/ Kara, Aura, Ring, and the setting
-            406: [0, 490, 492, 0x0f, [[36, 1], [100, 0], [101, 0], [102, 0], [103, 0], [104, 0], [105, 0]], False], # Beat Game w/Statues and Aura
-            407: [0, 490, 492, 0x0f, [[36, 1], [106, self.statues_required]], False]  # Beat Game w/Statues and Aura (player choice)
+            400: [0, [49, 150, 270, 345, 391][self.kara - 1], 490, 0, [[20, 1]], False],  # Rescue Kara w/ Magic Dust
+            405: [0, 490, 491, 0x0f, [[36, 1], [39, 1], [602, 1]], False],
+            # (Early) Firebird w/ Kara, Aura, Ring, and the setting
+            406: [0, 490, 492, 0x0f, [[36, 1], [100, 0], [101, 0], [102, 0], [103, 0], [104, 0], [105, 0]], False],
+            # Beat Game w/Statues and Aura
+            407: [0, 490, 492, 0x0f, [[36, 1], [106, self.statues_required]], False]
+            # Beat Game w/Statues and Aura (player choice)
         }
 
         # Define addresses for in-game spoiler text
         self.spoiler_labels = {
             0: "SpoilerTextCastleGuard",
             1: "SpoilerTextItoryElder",
             2: "SpoilerTextGoldShipQueen",
@@ -4657,28 +5084,28 @@
             6: "SpoilerTextIshtarsApprentice",
             7: "SpoilerTextKarasJournal",
             8: "SpoilerTextEuroOldMan",
             9: "SpoilerTextAngkorWatSpirit",
             10: "SpoilerTextDaoGirl",
             11: "SpoilerTextBabelSpirit"
         }
-        
+
         # Area names for in-game spoilers
         self.area_short_name = {
             0: "Jeweler",
             1: "Jeweler",
             2: "Jeweler",
             3: "Jeweler",
             4: "Jeweler",
             5: "Jeweler",
 
-            6:  "South Cape",
-            7:  "South Cape",
-            8:  "South Cape",
-            9:  "South Cape",
+            6: "South Cape",
+            7: "South Cape",
+            8: "South Cape",
+            9: "South Cape",
             10: "South Cape",
 
             11: "Edward's Castle",
             12: "Edward's Castle",
             13: "Edward's Prison",
             14: "Edward's Prison",
             15: "Edward's Tunnel",
@@ -4805,18 +5232,18 @@
             91: "Great Wall",
             92: "Great Wall",
             93: "Great Wall",
             94: "Great Wall",
             95: "Great Wall",
             732: "Great Wall",
 
-            96:  "Euro",
-            97:  "Euro",
-            98:  "Euro",
-            99:  "Euro",
+            96: "Euro",
+            97: "Euro",
+            98: "Euro",
+            99: "Euro",
             100: "Euro",
             101: "Euro",
             102: "Ann",
             103: "Euro",
 
             104: "Mt. Kress",
             105: "Mt. Kress",
@@ -4883,24 +5310,24 @@
             152: "Mummy Queen",
             153: "Olman"
         }
 
         # Database of enemy groups and spritesets
         # FORMAT: { ID: [Header card define name, Friendly name]}
         self.enemysets = {
-            0:  ["CardMonstersEdDg", "Underground Tunnel"],
-            1:  ["CardMonstersIncaSpinners", "Inca Ruins (Mud Monster and Larva)"],
-            2:  ["CardMonstersIncaStatues", "Inca Ruins (Statues)"],
-            3:  ["CardMonstersMine", "Diamond Mine"],
-            4:  ["CardMonstersSkGnTop", "Sky Garden (top)"],
-            5:  ["CardMonstersSkGnBot", "Sky Garden (bottom)"],
-            6:  ["CardMonstersMu", "Mu"],
-            7:  ["CardMonstersAngl", "Angel Dungeon"],
-            8:  ["CardMonstersGtWl", "Great Wall"],
-            9:  ["CardMonstersKres", "Mt. Kress"],
+            0: ["CardMonstersEdDg", "Underground Tunnel"],
+            1: ["CardMonstersIncaSpinners", "Inca Ruins (Mud Monster and Larva)"],
+            2: ["CardMonstersIncaStatues", "Inca Ruins (Statues)"],
+            3: ["CardMonstersMine", "Diamond Mine"],
+            4: ["CardMonstersSkGnTop", "Sky Garden (top)"],
+            5: ["CardMonstersSkGnBot", "Sky Garden (bottom)"],
+            6: ["CardMonstersMu", "Mu"],
+            7: ["CardMonstersAngl", "Angel Dungeon"],
+            8: ["CardMonstersGtWl", "Great Wall"],
+            9: ["CardMonstersKres", "Mt. Kress"],
             10: ["CardMonstersAnkrOuter", "Ankor Wat (outside)"],
             11: ["CardMonstersAnkrInner", "Ankor Wat (inside)"],
             12: ["CardMonstersPymd", "Pyramid"],
             13: ["CardMonstersJwlr", "Jeweler's Mansion"]
         }
 
         # Enemy map database
@@ -4913,144 +5340,155 @@
         #                6: LastMonsterId, 
         #                7: ForbiddenEnemysets, 
         #                8: Jumbo map (room clear is frustrating or requires multiple visits), 
         #                9: DarknessSinkMaps
         #               ] }
         self.maps = {
             # Underground Tunnel
-            12: [0, 1, [0,0], "EdDg Entrance", 2, 0x0001, 0x0003, [], False, [13]],
-            13: [0, 1, [0,0], "EdDg East",     2, 0x0004, 0x0012, [6, 10], False, [12,14]],
-            14: [0, 1, [0,0], "EdDg South",    2, 0x0013, 0x0021, [6, 10], False, [13,15]],
-            15: [0, 1, [0,0], "EdDg West",     2, 0x0022, 0x002e, [10], False, [14,17]],
-            17: [-1,0, [0,0], "EdDg Flower",   4, 0,      0,      [], False, [15,18]],
-            18: [0, 1, [0,0], "EdDg Big",      3, 0x002f, 0x0044, [6, 10], True, [17]],
+            12: [0, 1, [0, 0], "EdDg Entrance", 2, 0x0001, 0x0003, [], False, [13]],
+            13: [0, 1, [0, 0], "EdDg East", 2, 0x0004, 0x0012, [6, 10], False, [12, 14]],
+            14: [0, 1, [0, 0], "EdDg South", 2, 0x0013, 0x0021, [6, 10], False, [13, 15]],
+            15: [0, 1, [0, 0], "EdDg West", 2, 0x0022, 0x002e, [10], False, [14, 17]],
+            17: [-1, 0, [0, 0], "EdDg Flower", 4, 0, 0, [], False, [15, 18]],
+            18: [0, 1, [0, 0], "EdDg Big", 3, 0x002f, 0x0044, [6, 10], True, [17]],
 
             # Inca Ruins
-            27: [1, 0, [0,0], "Moon Tribe Cave",     3, 0x0045, 0x004a, [10], False, []],
-            29: [1, 1, [0,0], "Inca Exterior",       1, 0x004b, 0x0059, [10], True, [31,32,33,34,35,37,38]],
-            30: [-1,0, [0,0], "Inca Near Castoth",   4, 0,      0,      [], False, [34,41]],
-            31: [-1,0, [0,0], "Inca Statue Puzzle",  2, 0,      0,      [], False, [29,40]],
-            32: [1, 1, [0,0], "Inca Will Ability",   1, 0x005e, 0x0065, [], False, [29,35]],
-            33: [2, 1, [0,0], "Inca Water",          1, 0x0066, 0x007a, [6, 10], True, [29,35]],
-            34: [2, 1, [0,0], "Inca Big",            2, 0x007b, 0x008e, [], True, [29,30,38]],
-            35: [2, 1, [0,0], "Inca E/W Jump",       1, 0x008f, 0x009d, [6, 10], False, [29,32,33]],
-            #36: [-1,0, [0,0], "Inca Golden Tile",    2, 0,      0,      [], False, [34,30]],
-            37: [1, 1, [0,0], "Inca D.Block",        1, 0x009e, 0x00a9, [], False, [29,39]],
-            38: [1, 1, [0,0], "Inca Divided",        3, 0x00aa, 0x00b3, [], True, [29,34]],
-            39: [1, 1, [0,0], "Inca West of D.Block",2, 0x00b4, 0x00c4, [], False, [37]],
-            40: [1, 1, [0,0], "Inca Before Melody",  3, 0x00c5, 0x00cc, [], False, [31]],
-            41: [-1,0, [0,0], "Inca Castoth",        3, 0,      0,      [], False, [30]],
+            27: [1, 0, [0, 0], "Moon Tribe Cave", 3, 0x0045, 0x004a, [10], False, []],
+            29: [1, 1, [0, 0], "Inca Exterior", 1, 0x004b, 0x0059, [10], True, [31, 32, 33, 34, 35, 37, 38]],
+            30: [-1, 0, [0, 0], "Inca Near Castoth", 4, 0, 0, [], False, [34, 41]],
+            31: [-1, 0, [0, 0], "Inca Statue Puzzle", 2, 0, 0, [], False, [29, 40]],
+            32: [1, 1, [0, 0], "Inca Will Ability", 1, 0x005e, 0x0065, [], False, [29, 35]],
+            33: [2, 1, [0, 0], "Inca Water", 1, 0x0066, 0x007a, [6, 10], True, [29, 35]],
+            34: [2, 1, [0, 0], "Inca Big", 2, 0x007b, 0x008e, [], True, [29, 30, 38]],
+            35: [2, 1, [0, 0], "Inca E/W Jump", 1, 0x008f, 0x009d, [6, 10], False, [29, 32, 33]],
+            # 36: [-1,0, [0,0], "Inca Golden Tile",    2, 0,      0,      [], False, [34,30]],
+            37: [1, 1, [0, 0], "Inca D.Block", 1, 0x009e, 0x00a9, [], False, [29, 39]],
+            38: [1, 1, [0, 0], "Inca Divided", 3, 0x00aa, 0x00b3, [], True, [29, 34]],
+            39: [1, 1, [0, 0], "Inca West of D.Block", 2, 0x00b4, 0x00c4, [], False, [37]],
+            40: [1, 1, [0, 0], "Inca Before Melody", 3, 0x00c5, 0x00cc, [], False, [31]],
+            41: [-1, 0, [0, 0], "Inca Castoth", 3, 0, 0, [], False, [30]],
 
             # Diamond Mine 
-            61: [3, 2, [0,0], "Mine Fences",    3, 0x00ce, 0x00d8, [10], False, [65,66]],
-            62: [3, 2, [0,0], "Mine Entrance",  1, 0x00d9, 0x00df, [], False, [63]],
-            63: [3, 2, [0,0], "Mine Big",       1, 0x00e0, 0x00f7, [], True, [62,64,67]],
-            64: [3, 2, [0,0], "Mine Cave-in",   2, 0x00f8, 0x00fd, [10], False, [63,65]],
-            65: [3, 2, [0,0], "Mine Friar",     2, 0x00fe, 0x0108, [1, 6, 7, 8, 9, 10, 12, 13], False, [61,64,66]],  # Stationary Grundit
-            66: [-1,0, [0,0], "Mine Caverns",   4, 0,      0,      [], False, []],
-            67: [-1,0, [0,0], "Mine Elevator",  4, 0,      0,      [], False, [66,63,68]],
-            68: [-1,0, [0,0], "Mine End Branch",4, 0,      0,      [], False, [66,67,69,70]],
-            69: [3, 2, [0,0], "Mine Morgue",    3, 0x0109, 0x010e, [], False, [68]],
-            70: [3, 2, [0,0], "Mine Other Key", 3, 0x010f, 0x0117, [0, 1, 2, 4, 5, 6, 7, 8, 9, 10, 11, 12], False, [68]],
-            71: [-1,0, [0,0], "Mine Sam",       4, 0,      0,      [], False, [70]],
+            61: [3, 2, [0, 0], "Mine Fences", 3, 0x00ce, 0x00d8, [10], False, [65, 66]],
+            62: [3, 2, [0, 0], "Mine Entrance", 1, 0x00d9, 0x00df, [], False, [63]],
+            63: [3, 2, [0, 0], "Mine Big", 1, 0x00e0, 0x00f7, [], True, [62, 64, 67]],
+            64: [3, 2, [0, 0], "Mine Cave-in", 2, 0x00f8, 0x00fd, [10], False, [63, 65]],
+            65: [3, 2, [0, 0], "Mine Friar", 2, 0x00fe, 0x0108, [1, 6, 7, 8, 9, 10, 12, 13], False, [61, 64, 66]],
+            # Stationary Grundit
+            66: [-1, 0, [0, 0], "Mine Caverns", 4, 0, 0, [], False, []],
+            67: [-1, 0, [0, 0], "Mine Elevator", 4, 0, 0, [], False, [66, 63, 68]],
+            68: [-1, 0, [0, 0], "Mine End Branch", 4, 0, 0, [], False, [66, 67, 69, 70]],
+            69: [3, 2, [0, 0], "Mine Morgue", 3, 0x0109, 0x010e, [], False, [68]],
+            70: [3, 2, [0, 0], "Mine Other Key", 3, 0x010f, 0x0117, [0, 1, 2, 4, 5, 6, 7, 8, 9, 10, 11, 12], False,
+                 [68]],
+            71: [-1, 0, [0, 0], "Mine Sam", 4, 0, 0, [], False, [70]],
 
             # Sky Garden 
-            76: [-1,0, [0,0], "SkGn Entrance", 1, 0,      0,      [], False, [77,79,81,83,85]],
-            77: [4, 2, [0,0], "SkGn NE Top",   2, 0x0118, 0x0129, [], True, [76, 78]],
-            78: [5, 2, [0,0], "SkGn NE Bot",   3, 0x012a, 0x0136, [], True, [77]],
-            79: [4, 2, [0,0], "SkGn SE Top",   2, 0x0137, 0x0143, [], True, [76, 80, 86]],
-            80: [5, 2, [0,0], "SkGn SE Bot",   3, 0x0144, 0x014f, [10], True, [79]],
-            81: [4, 2, [0,0], "SkGn SW Top",   2, 0x0150, 0x015c, [10], False, [76, 82]],
-            82: [5, 2, [0,0], "SkGn SW Bot",   3, 0x015d, 0x0163, [0, 1, 2, 3, 6, 7, 8, 9, 10, 11, 12, 13], True, [81]],
-            83: [4, 2, [0,0], "SkGn NW Top",   2, 0x0164, 0x0172, [], True, [76, 84]],
-            84: [5, 2, [0,0], "SkGn NW Bot",   3, 0x0173, 0x0182, [0, 1, 2, 3, 6, 7, 8, 9, 10, 11, 12, 13], True, [83]],
-            85: [-1,0, [0,0], "SkGn Viper",    3, 0,      0,      [], False, [76]],
-            86: [-1,0, [0,0], "SkGn Blue Room",4, 0,      0,      [], False, [79]],
+            76: [-1, 0, [0, 0], "SkGn Entrance", 1, 0, 0, [], False, [77, 79, 81, 83, 85]],
+            77: [4, 2, [0, 0], "SkGn NE Top", 2, 0x0118, 0x0129, [], True, [76, 78]],
+            78: [5, 2, [0, 0], "SkGn NE Bot", 3, 0x012a, 0x0136, [], True, [77]],
+            79: [4, 2, [0, 0], "SkGn SE Top", 2, 0x0137, 0x0143, [], True, [76, 80, 86]],
+            80: [5, 2, [0, 0], "SkGn SE Bot", 3, 0x0144, 0x014f, [10], True, [79]],
+            81: [4, 2, [0, 0], "SkGn SW Top", 2, 0x0150, 0x015c, [10], False, [76, 82]],
+            82: [5, 2, [0, 0], "SkGn SW Bot", 3, 0x015d, 0x0163, [0, 1, 2, 3, 6, 7, 8, 9, 10, 11, 12, 13], True, [81]],
+            83: [4, 2, [0, 0], "SkGn NW Top", 2, 0x0164, 0x0172, [], True, [76, 84]],
+            84: [5, 2, [0, 0], "SkGn NW Bot", 3, 0x0173, 0x0182, [0, 1, 2, 3, 6, 7, 8, 9, 10, 11, 12, 13], True, [83]],
+            85: [-1, 0, [0, 0], "SkGn Viper", 3, 0, 0, [], False, [76]],
+            86: [-1, 0, [0, 0], "SkGn Blue Room", 4, 0, 0, [], False, [79]],
 
             # Mu
-            95:  [6, 3, [0,0], "Mu NW", 1, 0x0193, 0x01a5, [10], True, [96,98]],
-            96:  [6, 3, [0,0], "Mu NE", 1, 0x01a6, 0x01bf, [7, 8, 9, 12], True, [95,97]],
-            97:  [6, 3, [0,0], "Mu E",  2, 0x01c0, 0x01d9, [7, 8, 9, 12], True, [96,98]],
-            98:  [6, 3, [0,0], "Mu W",  2, 0x01da, 0x01e5, [], True, [95,97,100]],
-            100: [6, 3, [0,0], "Mu SW", 2, 0x01e6, 0x01ed, [], True, [98,101]],
-            101: [6, 3, [0,0], "Mu SE", 3, 0x01ee, 0x01fe, [7, 8, 9, 12], False, [100]],
+            95: [6, 3, [0, 0], "Mu NW", 1, 0x0193, 0x01a5, [10], True, [96, 98]],
+            96: [6, 3, [0, 0], "Mu NE", 1, 0x01a6, 0x01bf, [7, 8, 9, 12], True, [95, 97]],
+            97: [6, 3, [0, 0], "Mu E", 2, 0x01c0, 0x01d9, [7, 8, 9, 12], True, [96, 98]],
+            98: [6, 3, [0, 0], "Mu W", 2, 0x01da, 0x01e5, [], True, [95, 97, 100]],
+            100: [6, 3, [0, 0], "Mu SW", 2, 0x01e6, 0x01ed, [], True, [98, 101]],
+            101: [6, 3, [0, 0], "Mu SE", 3, 0x01ee, 0x01fe, [7, 8, 9, 12], False, [100]],
 
             # Angel Dungeon
-            109: [7, 3, [0,0], "Angel Entrance", 2, 0x0201, 0x020f, [0, 1, 2, 3, 4, 5, 6, 11, 12, 13], True, [110]],
-            110: [7, 3, [0,0], "Angel Second",   2, 0x0210, 0x0222, [0, 1, 2, 3, 4, 5, 6, 11, 12, 13], True, [109,111]],
-            111: [7, 3, [0,0], "Angel Dark",     2, 0x0223, 0x0228, [0, 1, 2, 3, 4, 5, 6, 11, 12, 13], False, [110,112]],
-            112: [7, 3, [0,0], "Angel Water",    2, 0x0229, 0x022f, [0, 1, 2, 3, 4, 5, 6, 11, 12, 13], False, [111,113]],
-            113: [7, 3, [0,0], "Angel Wind",     2, 0x0230, 0x0231, [0, 1, 2, 3, 4, 5, 6, 11, 12, 13], False, [112,114]],
-            114: [7, 3, [0,0], "Angel Final",    3, 0x0232, 0x0242, [0, 1, 2, 3, 4, 5, 6, 11, 12, 13], False, [113]],
+            109: [7, 3, [0, 0], "Angel Entrance", 2, 0x0201, 0x020f, [0, 1, 2, 3, 4, 5, 6, 11, 12, 13], True, [110]],
+            110: [7, 3, [0, 0], "Angel Second", 2, 0x0210, 0x0222, [0, 1, 2, 3, 4, 5, 6, 11, 12, 13], True, [109, 111]],
+            111: [7, 3, [0, 0], "Angel Dark", 2, 0x0223, 0x0228, [0, 1, 2, 3, 4, 5, 6, 11, 12, 13], False, [110, 112]],
+            112: [7, 3, [0, 0], "Angel Water", 2, 0x0229, 0x022f, [0, 1, 2, 3, 4, 5, 6, 11, 12, 13], False, [111, 113]],
+            113: [7, 3, [0, 0], "Angel Wind", 2, 0x0230, 0x0231, [0, 1, 2, 3, 4, 5, 6, 11, 12, 13], False, [112, 114]],
+            114: [7, 3, [0, 0], "Angel Final", 3, 0x0232, 0x0242, [0, 1, 2, 3, 4, 5, 6, 11, 12, 13], False, [113]],
 
             # Great Wall
-            130: [8, 4, [0,0], "GtWl Entrance",  1, 0x0243, 0x0262, [0, 1, 2, 3, 4, 5, 6, 7, 11, 12, 13], True, [131]],
-            131: [8, 4, [0,0], "GtWl Tall Drop", 1, 0x0263, 0x0277, [0, 1, 2, 3, 4, 5, 6, 11, 12, 13], True, [130,133]],
-            133: [8, 4, [0,0], "GtWl Ramps",     1, 0x0278, 0x0291, [0, 1, 2, 3, 4, 5, 6, 7, 11, 12, 13], True, [131,134]],
-            134: [8, 4, [0,0], "GtWl Spin Dash", 1, 0x0292, 0x029a, [0, 1, 2, 3, 4, 5, 6, 11, 12, 13], False, [133,135]],
-            135: [8, 4, [0,0], "GtWl Friar",     2, 0x029b, 0x02a6, [0, 1, 2, 3, 4, 5, 6, 7, 9, 10, 11, 12, 13], True, [134,136]],
-            136: [8, 4, [0,0], "GtWl Final",     2, 0x02a7, 0x02b5, [0, 1, 2, 3, 4, 5, 6, 10, 11, 12, 13], True, [135,138]],
-            138: [-1,0, [0,0], "GtWl Fanger",    3, 0,      0,      [], False, [136]],
+            130: [8, 4, [0, 0], "GtWl Entrance", 1, 0x0243, 0x0262, [0, 1, 2, 3, 4, 5, 6, 7, 11, 12, 13], True, [131]],
+            131: [8, 4, [0, 0], "GtWl Tall Drop", 1, 0x0263, 0x0277, [0, 1, 2, 3, 4, 5, 6, 11, 12, 13], True,
+                  [130, 133]],
+            133: [8, 4, [0, 0], "GtWl Ramps", 1, 0x0278, 0x0291, [0, 1, 2, 3, 4, 5, 6, 7, 11, 12, 13], True,
+                  [131, 134]],
+            134: [8, 4, [0, 0], "GtWl Spin Dash", 1, 0x0292, 0x029a, [0, 1, 2, 3, 4, 5, 6, 11, 12, 13], False,
+                  [133, 135]],
+            135: [8, 4, [0, 0], "GtWl Friar", 2, 0x029b, 0x02a6, [0, 1, 2, 3, 4, 5, 6, 7, 9, 10, 11, 12, 13], True,
+                  [134, 136]],
+            136: [8, 4, [0, 0], "GtWl Final", 2, 0x02a7, 0x02b5, [0, 1, 2, 3, 4, 5, 6, 10, 11, 12, 13], True,
+                  [135, 138]],
+            138: [-1, 0, [0, 0], "GtWl Fanger", 3, 0, 0, [], False, [136]],
 
             # Mt Temple 
-            160: [9, 4, [0,0], "Kress Entrance",    1, 0x02b7, 0x02c1, [], False, [161]],
-            161: [9, 4, [0,0], "Kress First DS",    1, 0x02c2, 0x02d9, [0, 1, 2, 3, 4, 5, 6, 11, 12, 13], True, [160,162]],
-            162: [9, 4, [0,0], "Kress First Vine",  1, 0x02da, 0x02e7, [7, 11], True, [161,163,164,165]],
-            163: [9, 4, [0,0], "Kress Second DS",   3, 0x02e8, 0x02fb, [], False, [162]],
-            164: [9, 4, [0,0], "Kress West Chest",  3, 0x02fc, 0x0315, [6, 7], True, [162]],
-            165: [9, 4, [0,0], "Kress Two Vines",   2, 0x0316, 0x032d, [7, 11], True, [162,166,167,168]],
-            166: [9, 4, [0,0], "Kress Mushrooms",   3, 0x032e, 0x033c, [], True, [165]],
-            167: [9, 4, [0,0], "Kress Final DS",    3, 0x033d, 0x0363, [7], True, [165]],
-            168: [9, 4, [0,0], "Kress Last Combat", 3, 0x0364, 0x036b, [0, 1, 2, 3, 4, 5, 6, 11, 12, 13], False, [165,169]],
-            169: [-1,0, [0,0], "Kress Final Chest", 4, 0,      0,      [], False, [168]],
+            160: [9, 4, [0, 0], "Kress Entrance", 1, 0x02b7, 0x02c1, [], False, [161]],
+            161: [9, 4, [0, 0], "Kress First DS", 1, 0x02c2, 0x02d9, [0, 1, 2, 3, 4, 5, 6, 11, 12, 13], True,
+                  [160, 162]],
+            162: [9, 4, [0, 0], "Kress First Vine", 1, 0x02da, 0x02e7, [7, 11], True, [161, 163, 164, 165]],
+            163: [9, 4, [0, 0], "Kress Second DS", 3, 0x02e8, 0x02fb, [], False, [162]],
+            164: [9, 4, [0, 0], "Kress West Chest", 3, 0x02fc, 0x0315, [6, 7], True, [162]],
+            165: [9, 4, [0, 0], "Kress Two Vines", 2, 0x0316, 0x032d, [7, 11], True, [162, 166, 167, 168]],
+            166: [9, 4, [0, 0], "Kress Mushrooms", 3, 0x032e, 0x033c, [], True, [165]],
+            167: [9, 4, [0, 0], "Kress Final DS", 3, 0x033d, 0x0363, [7], True, [165]],
+            168: [9, 4, [0, 0], "Kress Last Combat", 3, 0x0364, 0x036b, [0, 1, 2, 3, 4, 5, 6, 11, 12, 13], False,
+                  [165, 169]],
+            169: [-1, 0, [0, 0], "Kress Final Chest", 4, 0, 0, [], False, [168]],
 
             # Ankor Wat
-            176: [10, 6, [0,0], "Wat Exterior",     1, 0x036c, 0x037a, [], True, [177]],
-            177: [11, 6, [0,0], "Wat Outer South",  1, 0x037b, 0x038d, [6, 10], True, [176,178,181,182]],
-            178: [11, 6, [0,0], "Wat Outer East",   1, 0x038e, 0x0398, [6, 10, 12], True, [177,179]],
-            179: [11, 6, [0,0], "Wat Outer North",  1, 0x0399, 0x039f, [], True, [178,181]],
-            180: [11, 6, [0,0], "Wat Outer Pit",    0, 0x03a0, 0x03a5, [6, 10, 12], False, []],
-            181: [11, 6, [0,0], "Wat Outer West",   1, 0x03a6, 0x03b0, [], True, [177,179]],
-            182: [10, 6, [0,0], "Wat Garden",       1, 0x03b1, 0x03d7, [7], True, [177,183]],
-            183: [11, 6, [0,0], "Wat Inner South",  1, 0x03d8, 0x03e3, [], True, [182,184,185,186]],  # Earthquaker Golem
-            184: [11, 6, [0,0], "Wat Inner East",   3, 0x03e4, 0x03e9, [2, 6, 10, 12], True, [183]],
-            185: [11, 6, [0,0], "Wat Inner West",   1, 0x03ea, 0x03f1, [], False, [183]],
-            186: [10, 6, [0,0], "Wat Road to Main", 4, 0x03f2, 0x03f6, [], True, [183,187]],
-            187: [11, 6, [0,0], "Wat Main 1F",      2, 0x03f7, 0x03fc, [], False, [186,188]],
-            188: [11, 6, [0,0], "Wat Main 2F",      0, 0x03fd, 0x0403, [], False, [187,189]],
-            189: [11, 6, [0,0], "Wat Main 3F",      3, 0x0404, 0x040e, [], False, [188,190]],
-            190: [11, 6, [0,0], "Wat Main 4F",      4, 0x040f, 0x0415, [], False, [189,191]],
-            191: [-1, 0, [0,0], "Wat Spirit",       4, 0,      0,      [], False, [190]],
+            176: [10, 6, [0, 0], "Wat Exterior", 1, 0x036c, 0x037a, [], True, [177]],
+            177: [11, 6, [0, 0], "Wat Outer South", 1, 0x037b, 0x038d, [6, 10], True, [176, 178, 181, 182]],
+            178: [11, 6, [0, 0], "Wat Outer East", 1, 0x038e, 0x0398, [6, 10, 12], True, [177, 179]],
+            179: [11, 6, [0, 0], "Wat Outer North", 1, 0x0399, 0x039f, [], True, [178, 181]],
+            180: [11, 6, [0, 0], "Wat Outer Pit", 0, 0x03a0, 0x03a5, [6, 10, 12], False, []],
+            181: [11, 6, [0, 0], "Wat Outer West", 1, 0x03a6, 0x03b0, [], True, [177, 179]],
+            182: [10, 6, [0, 0], "Wat Garden", 1, 0x03b1, 0x03d7, [7], True, [177, 183]],
+            183: [11, 6, [0, 0], "Wat Inner South", 1, 0x03d8, 0x03e3, [], True, [182, 184, 185, 186]],
+            # Earthquaker Golem
+            184: [11, 6, [0, 0], "Wat Inner East", 3, 0x03e4, 0x03e9, [2, 6, 10, 12], True, [183]],
+            185: [11, 6, [0, 0], "Wat Inner West", 1, 0x03ea, 0x03f1, [], False, [183]],
+            186: [10, 6, [0, 0], "Wat Road to Main", 4, 0x03f2, 0x03f6, [], True, [183, 187]],
+            187: [11, 6, [0, 0], "Wat Main 1F", 2, 0x03f7, 0x03fc, [], False, [186, 188]],
+            188: [11, 6, [0, 0], "Wat Main 2F", 0, 0x03fd, 0x0403, [], False, [187, 189]],
+            189: [11, 6, [0, 0], "Wat Main 3F", 3, 0x0404, 0x040e, [], False, [188, 190]],
+            190: [11, 6, [0, 0], "Wat Main 4F", 4, 0x040f, 0x0415, [], False, [189, 191]],
+            191: [-1, 0, [0, 0], "Wat Spirit", 4, 0, 0, [], False, [190]],
 
             # Pyramid
-            204: [12, 5, [0,0], "Pyramid Foyer",   1, 0x0416, 0x0417, [], False, [206,208,210,212,214,216,221]],
-            206: [12, 5, [0,0], "Pyramid Room 1A", 2, 0x0418, 0x0423, [], True, [204,207]],
-            207: [12, 5, [0,0], "Pyramid Room 1B", 3, 0x0424, 0x0431, [], True, [206]],
-            208: [12, 5, [0,0], "Pyramid Room 2A", 2, 0x0432, 0x0439, [], False, [204,209]],
-            209: [12, 5, [0,0], "Pyramid Room 2B", 3, 0x043a, 0x044c, [], True, [208]],
-            210: [12, 5, [0,0], "Pyramid Room 6A", 2, 0x044d, 0x0462, [], True, [204,211]],
-            211: [12, 5, [0,0], "Pyramid Room 6B", 3, 0x0463, 0x0473, [], True, [210]],
-            212: [12, 5, [0,0], "Pyramid Room 5A", 2, 0x0474, 0x0483, [], True, [204,213]],
-            213: [12, 5, [0,0], "Pyramid Room 5B", 3, 0x0484, 0x0497, [], True, [212]],
-            214: [12, 5, [0,0], "Pyramid Room 3A", 2, 0x0498, 0x04a8, [], True, [204,215]],
-            215: [12, 5, [0,0], "Pyramid Room 3B", 3, 0x04a9, 0x04b8, [1, 7, 10], False, [214]],
-            216: [12, 5, [0,0], "Pyramid Room 4A", 2, 0x04b9, 0x04db, [7], True, [204,217]],
-            217: [12, 5, [0,0], "Pyramid Room 4B", 2, 0x04dc, 0x04f2, [], True, [216,219]],
-            219: [12, 5, [0,0], "Pyramid Room 4C", 3, 0x04f3, 0x04f6, [1, 2, 3, 6, 7, 10, 13], False, [217]],  #Spike elevators
-            221: [-1, 0, [0,0], "Pyramid MQ",      3, 0,      0,      [], False, [204]],
+            204: [12, 5, [0, 0], "Pyramid Foyer", 1, 0x0416, 0x0417, [], False, [206, 208, 210, 212, 214, 216, 221]],
+            206: [12, 5, [0, 0], "Pyramid Room 1A", 2, 0x0418, 0x0423, [], True, [204, 207]],
+            207: [12, 5, [0, 0], "Pyramid Room 1B", 3, 0x0424, 0x0431, [], True, [206]],
+            208: [12, 5, [0, 0], "Pyramid Room 2A", 2, 0x0432, 0x0439, [], False, [204, 209]],
+            209: [12, 5, [0, 0], "Pyramid Room 2B", 3, 0x043a, 0x044c, [], True, [208]],
+            210: [12, 5, [0, 0], "Pyramid Room 6A", 2, 0x044d, 0x0462, [], True, [204, 211]],
+            211: [12, 5, [0, 0], "Pyramid Room 6B", 3, 0x0463, 0x0473, [], True, [210]],
+            212: [12, 5, [0, 0], "Pyramid Room 5A", 2, 0x0474, 0x0483, [], True, [204, 213]],
+            213: [12, 5, [0, 0], "Pyramid Room 5B", 3, 0x0484, 0x0497, [], True, [212]],
+            214: [12, 5, [0, 0], "Pyramid Room 3A", 2, 0x0498, 0x04a8, [], True, [204, 215]],
+            215: [12, 5, [0, 0], "Pyramid Room 3B", 3, 0x04a9, 0x04b8, [1, 7, 10], False, [214]],
+            216: [12, 5, [0, 0], "Pyramid Room 4A", 2, 0x04b9, 0x04db, [7], True, [204, 217]],
+            217: [12, 5, [0, 0], "Pyramid Room 4B", 2, 0x04dc, 0x04f2, [], True, [216, 219]],
+            219: [12, 5, [0, 0], "Pyramid Room 4C", 3, 0x04f3, 0x04f6, [1, 2, 3, 6, 7, 10, 13], False, [217]],
+            # Spike elevators
+            221: [-1, 0, [0, 0], "Pyramid MQ", 3, 0, 0, [], False, [204]],
 
             # Jeweler's Mansion
-            233: [13, 0, [0,0], "Mansion",   3, 0x04f9, 0x051e, [7, 10], True, [234]],
-            234: [-1, 0, [0,0], "Solid Arm", 4, 0,      0,      [], False, [233]],
-            
+            233: [13, 0, [0, 0], "Mansion", 3, 0x04f9, 0x051e, [7, 10], True, [234]],
+            234: [-1, 0, [0, 0], "Solid Arm", 4, 0, 0, [], False, [233]],
+
             # Babel bosses
-            242: [-1, 0, [0,0], "Babel Castoth", 3, 0, 0, [], False, []],
-            243: [-1, 0, [0,0], "Babel Viper",   3, 0, 0, [], False, []],
-            245: [-1, 0, [0,0], "Babel Fanger",  3, 0, 0, [], False, []],
-            246: [-1, 0, [0,0], "Babel MQ",      3, 0, 0, [], False, []]
+            242: [-1, 0, [0, 0], "Babel Castoth", 3, 0, 0, [], False, []],
+            243: [-1, 0, [0, 0], "Babel Viper", 3, 0, 0, [], False, []],
+            245: [-1, 0, [0, 0], "Babel Fanger", 3, 0, 0, [], False, []],
+            246: [-1, 0, [0, 0], "Babel MQ", 3, 0, 0, [], False, []]
         }
 
         # Database of enemy types
         # FORMAT: { ID: [0: Enemyset ID, 
         #                1: ASM define for addr, 
         #                2: Default stat block,
         #                3: Type(1=stationary,2=walking,3=flying),
@@ -5145,33 +5583,33 @@
             93: [9, "EnemizerAcidSplasherStationaryNAddr", 0x3c, 2, True, False, "Acid Splasher (stationary N)"],
 
             # Ankor Wat
             100: [10, "EnemizerShrubberAddr", 0x49, 2, True, True, "Shrubber"],
             101: [10, "EnemizerShrubber2Addr", 0x49, 2, True, False, "Shrubber 2"],
             102: [10, "EnemizerZombieAddr", 0x46, 2, True, True, "Zombie"],
             103: [10, "EnemizerZipFlyAddr", 0x4a, 3, True, True, "Zip Fly"],  # False for now...
-            104: [11, "EnemizerGoldcapAddr", 0x42, 3, True, True, "Goldcap"],    # i.e. flying skull
+            104: [11, "EnemizerGoldcapAddr", 0x42, 3, True, True, "Goldcap"],  # i.e. flying skull
             105: [11, "EnemizerGorgonAddr", 0x45, 2, True, True, "Gorgon"],
             106: [11, "EnemizerGorgonDropperAddr", 0x45, 2, True, False, "Gorgon Dropper"],
-            107: [11, "EnemizerFrenzie1Addr", 0x43, 2, True, False, "Frenzie 1"],   # i.e. wall skull stationary
-            108: [11, "EnemizerFrenzie2Addr", 0x43, 2, True, True, "Frenzie 2"],    # i.e. wall skull moving
+            107: [11, "EnemizerFrenzie1Addr", 0x43, 2, True, False, "Frenzie 1"],  # i.e. wall skull stationary
+            108: [11, "EnemizerFrenzie2Addr", 0x43, 2, True, True, "Frenzie 2"],  # i.e. wall skull moving
             109: [11, "EnemizerWatScarab1Addr", 0x44, 1, False, True, "Wall Walker 1"],
             110: [11, "EnemizerWatScarab2Addr", 0x3a, 1, False, False, "Wall Walker 2"],
             111: [11, "EnemizerWatScarab3Addr", 0x44, 1, False, False, "Wall Walker 3"],
             112: [11, "EnemizerWatScarab4Addr", 0x3a, 1, False, False, "Wall Walker 4"],
             113: [11, "EnemizerGorgonBlockAddr", 0x45, 2, True, False, "Gorgon (block)"],
 
             # Pyramid
             120: [12, "EnemizerMysticBallStationaryAddr", 0x4f, 1, True, True, "Mystic Ball (stationary)"],
             121: [12, "EnemizerMysticBall1Addr", 0x4f, 2, True, True, "Mystic Ball 1"],
             122: [12, "EnemizerMysticBall2Addr", 0x4f, 2, True, True, "Mystic Ball 2"],
-            123: [12, "EnemizerTutsAddr", 0x4e, 2, True, True, "Tuts"],   # i.e. spearman
-            124: [12, "EnemizerBlasterAddr", 0x51, 1, True, True, "Blaster"],   # i.e. bird head
-            125: [12, "EnemizerHauntStationaryAddr", 0x4c, 2, True, False, "Haunt (stationary)"],   # i.e. wall mummy
-            126: [12, "EnemizerHauntAddr", 0x4c, 2, True, True, "Haunt"],   # i.e. loose mummy
+            123: [12, "EnemizerTutsAddr", 0x4e, 2, True, True, "Tuts"],  # i.e. spearman
+            124: [12, "EnemizerBlasterAddr", 0x51, 1, True, True, "Blaster"],  # i.e. bird head
+            125: [12, "EnemizerHauntStationaryAddr", 0x4c, 2, True, False, "Haunt (stationary)"],  # i.e. wall mummy
+            126: [12, "EnemizerHauntAddr", 0x4c, 2, True, True, "Haunt"],  # i.e. loose mummy
 
             # Babel Tower
             #            130: [14,"\xd7\x99\x8a",0x5a,"Castoth (boss)"],
             #            131: [14,"\xd5\xd0\x8a",0x5b,"Viper (boss)"],
             #            132: [14,"\x50\xf1\x8a",0x5c,"Vampire (boss)"],
             #            133: [14,"\x9c\xf1\x8a",0x5c,"Vampire (boss)"],
             #            134: [14,"\x00\x80\x8",0x5d,"Sand Fanger (boss)"],
@@ -5188,15 +5626,15 @@
             #            55: [15,"\xf7\xf1\x8a",0x2f,"Vampire (boss)"],
             #            56: [15,"\xc8\xf3\x8a",0x30,"Vampire (boss)"],
             #            79: [15,"\x5c\x81\x8",0x36,"Sand Fanger (boss)"],
             #            128: [15,"\xb6\xa6\x8",0x50,"Mummy Queen (boss)"],
             #            143: [15,"\x09\xf7\x88",0x5f,"Solid Arm (boss)"],
             #            140: [15,"\xaa\xee\x8c",0x54,"Dark Gaia"]
         }
-        
+
         # Default (vanilla) enemy type for each non-boss monster ID
         self.default_enemies = {
             0x0001: 0,
             0x0002: 0,
             0x0003: 0,
             0x0004: 2,
             0x0005: 2,
@@ -5447,15 +5885,15 @@
             0x00FB: 33,
             0x00FC: 35,
             0x00FD: 35,
             0x00FE: 35,
             0x00FF: 35,
             0x0100: 35,
             0x0101: 35,
-            #0x0102: xx,    # Friar worm fence worm; always a special stationary worm actor
+            # 0x0102: xx,    # Friar worm fence worm; always a special stationary worm actor
             0x0103: 33,
             0x0104: 33,
             0x0105: 33,
             0x0106: 30,
             0x0107: 30,
             0x0108: 30,
             0x0109: 35,
@@ -6495,97 +6933,101 @@
             0x0519: 141,
             0x051A: 141,
             0x051B: 141,
             0x051C: 141,
             0x051D: 141,
             0x051E: 141
         }
-        
+
         # List of disallowed enemy types at each monster ID, for ensuring that orbs are reachable
         # and solid monsters can't softlock you, etc.
         self.enemizer_restricted_enemies = {
-            0x0004: [53,60,73,80,81,102,103,104],  # U.Tunnel Skeleton Cage
-            0x0006: [53,60,73,80,81,102,103,104],  # U.Tunnel First Door
-            0x0016: [53,60,73,80,81,102,103,104],  # U.Tunnel Second Door
-            0x002A: [53,60,73,80,81,102,103,104],  # U.Tunnel Bat Door
-            0x0034: [53,60,73,80,81,102,103,104],  # U.Tunnel Dark Space
-            0x0043: [53,60,73,80,81,102,103,104],  # U.Tunnel Skeleton Door 1
-            0x0044: [53,60,73,80,81,102,103,104],  # U.Tunnel Skeleton Door 2
-            0x0051: [53,60,73,80,81,102,103,104],  # Inca West Ladder
-            0x0052: [53,60,73,80,81,102,103,104],  # Inca Entrance Ladder
-            0x0055: [53,60,73,80,81,102,103,104],  # Inca Final Ladder
-            0x007A: [53,60,73,80,81,102,103,104],  # Inca N/S Ramp Room Ramp
-            0x009D: [14,33,52,53,60,73,80,81,102,103,104,143],  # Inca E/W Ramp Room Ramp
-            0x00BF: [53,60,73,80,81,102,103,104],  # Inca Diamond Block Stair
-            0x00CA: [53,60,73,80,81,102,103,104],  # Inca Singing Statue Stair
-            0x00CF: [53,60,73,80,81,102,103,104],  # Mine Tunnel Middle Fence
-            0x00D2: [53,60,73,80,81,102,103,104],  # Mine Tunnel South Fence
-            0x00D3: [53,60,73,80,81,102,103,104],  # Mine Tunnel North Fence
-            0x00E0: [53,60,73,80,81,102,103,104],  # Mine Big Room Cage
-            0x00FD: [53,60,73,80,81,102,103,104],  # Mine Appearing Dark Space
-            #0x0102: [],   # Friar worm fence worm is never randomized
-            0x013B: [2,14,17,22,33,35,41,43,52,53,55,60,62,73,80,81,102,103,104,123,141,143],  # Garden SE Top Gate
-            0x0148: [53,60,73,80,81,102,103,104],  # Garden SE Darkside Chest
-            0x0150: [53,60,73,80,81,102,103,104],  # Garden SW Top Robot Gate
-            0x0153: [53,60,73,80,81,102,103,104],  # Garden SW Top Robot Ramp
-            0x015C: [53,60,73,80,81,102,103,104],  # Garden SW Top Worm Gate
-            0x0161: [53,60,73,80,81,102,103,104],  # Garden SW Darkside Cage
-            0x0194: [53,60,73,80,81,102,103,104],  # Mu Entrance Gate
-            0x01A7: [2,14,17,22,33,35,41,43,52,53,55,60,62,73,80,81,102,103,104,123,141,143],  # Mu NE First Rock
-            0x01A9: [2,14,17,22,33,35,41,43,52,53,55,60,62,73,80,81,102,103,104,123,141,143],  # Mu NE Second Rock
-            0x01DE: [53,60,73,80,81,102,103,104],  # Mu West Slime Cages
-            0x01EE: [53,60,73,80,81,102,103,104],  # Mu SE East-facing Head
-            0x01FC: [53,60,73,80,81,102,103,104],  # Mu SE South-facing Head
-            0x029B: [2,14,17,22,33,35,41,43,52,53,55,60,62,73,80,81,102,103,104,123,141,143],  # Great Wall Friar Gate
-            #0x02B6: [],   # Fanger is never randomized
-            0x030A: [53,60,73,80,81,102,103,104],  # Kress West Room Shortcut
-            0x0388: [53,60,73,80,81,102,103,104],  # Wat Entrance Stair
-            0x0395: [53,60,73,80,81,102,103,104],  # Wat East Slider Hole
-            0x03A0: [53,60,73,80,81,102,103,104],  # Ankor Wat Pit Exit
-            0x03E9: [2,14,17,22,33,35,41,43,52,53,55,60,62,73,80,81,102,103,104,123,141,143],  # Wat Dark Space Corridor
-            0x0417: [53,60,73,80,81,102,103,104],  # Pyramid Foyer Dark Space
-            0x04FA: [53,60,73,80,81,102,103,104],  # Mansion First Barrier
-            0x0505: [53,60,73,80,81,102,103,104]   # Mansion Second Barrier
+            0x0004: [53, 60, 73, 80, 81, 102, 103, 104],  # U.Tunnel Skeleton Cage
+            0x0006: [53, 60, 73, 80, 81, 102, 103, 104],  # U.Tunnel First Door
+            0x0016: [53, 60, 73, 80, 81, 102, 103, 104],  # U.Tunnel Second Door
+            0x002A: [53, 60, 73, 80, 81, 102, 103, 104],  # U.Tunnel Bat Door
+            0x0034: [53, 60, 73, 80, 81, 102, 103, 104],  # U.Tunnel Dark Space
+            0x0043: [53, 60, 73, 80, 81, 102, 103, 104],  # U.Tunnel Skeleton Door 1
+            0x0044: [53, 60, 73, 80, 81, 102, 103, 104],  # U.Tunnel Skeleton Door 2
+            0x0051: [53, 60, 73, 80, 81, 102, 103, 104],  # Inca West Ladder
+            0x0052: [53, 60, 73, 80, 81, 102, 103, 104],  # Inca Entrance Ladder
+            0x0055: [53, 60, 73, 80, 81, 102, 103, 104],  # Inca Final Ladder
+            0x007A: [53, 60, 73, 80, 81, 102, 103, 104],  # Inca N/S Ramp Room Ramp
+            0x009D: [14, 33, 52, 53, 60, 73, 80, 81, 102, 103, 104, 143],  # Inca E/W Ramp Room Ramp
+            0x00BF: [53, 60, 73, 80, 81, 102, 103, 104],  # Inca Diamond Block Stair
+            0x00CA: [53, 60, 73, 80, 81, 102, 103, 104],  # Inca Singing Statue Stair
+            0x00CF: [53, 60, 73, 80, 81, 102, 103, 104],  # Mine Tunnel Middle Fence
+            0x00D2: [53, 60, 73, 80, 81, 102, 103, 104],  # Mine Tunnel South Fence
+            0x00D3: [53, 60, 73, 80, 81, 102, 103, 104],  # Mine Tunnel North Fence
+            0x00E0: [53, 60, 73, 80, 81, 102, 103, 104],  # Mine Big Room Cage
+            0x00FD: [53, 60, 73, 80, 81, 102, 103, 104],  # Mine Appearing Dark Space
+            # 0x0102: [],   # Friar worm fence worm is never randomized
+            0x013B: [2, 14, 17, 22, 33, 35, 41, 43, 52, 53, 55, 60, 62, 73, 80, 81, 102, 103, 104, 123, 141, 143],
+            # Garden SE Top Gate
+            0x0148: [53, 60, 73, 80, 81, 102, 103, 104],  # Garden SE Darkside Chest
+            0x0150: [53, 60, 73, 80, 81, 102, 103, 104],  # Garden SW Top Robot Gate
+            0x0153: [53, 60, 73, 80, 81, 102, 103, 104],  # Garden SW Top Robot Ramp
+            0x015C: [53, 60, 73, 80, 81, 102, 103, 104],  # Garden SW Top Worm Gate
+            0x0161: [53, 60, 73, 80, 81, 102, 103, 104],  # Garden SW Darkside Cage
+            0x0194: [53, 60, 73, 80, 81, 102, 103, 104],  # Mu Entrance Gate
+            0x01A7: [2, 14, 17, 22, 33, 35, 41, 43, 52, 53, 55, 60, 62, 73, 80, 81, 102, 103, 104, 123, 141, 143],
+            # Mu NE First Rock
+            0x01A9: [2, 14, 17, 22, 33, 35, 41, 43, 52, 53, 55, 60, 62, 73, 80, 81, 102, 103, 104, 123, 141, 143],
+            # Mu NE Second Rock
+            0x01DE: [53, 60, 73, 80, 81, 102, 103, 104],  # Mu West Slime Cages
+            0x01EE: [53, 60, 73, 80, 81, 102, 103, 104],  # Mu SE East-facing Head
+            0x01FC: [53, 60, 73, 80, 81, 102, 103, 104],  # Mu SE South-facing Head
+            0x029B: [2, 14, 17, 22, 33, 35, 41, 43, 52, 53, 55, 60, 62, 73, 80, 81, 102, 103, 104, 123, 141, 143],
+            # Great Wall Friar Gate
+            # 0x02B6: [],   # Fanger is never randomized
+            0x030A: [53, 60, 73, 80, 81, 102, 103, 104],  # Kress West Room Shortcut
+            0x0388: [53, 60, 73, 80, 81, 102, 103, 104],  # Wat Entrance Stair
+            0x0395: [53, 60, 73, 80, 81, 102, 103, 104],  # Wat East Slider Hole
+            0x03A0: [53, 60, 73, 80, 81, 102, 103, 104],  # Ankor Wat Pit Exit
+            0x03E9: [2, 14, 17, 22, 33, 35, 41, 43, 52, 53, 55, 60, 62, 73, 80, 81, 102, 103, 104, 123, 141, 143],
+            # Wat Dark Space Corridor
+            0x0417: [53, 60, 73, 80, 81, 102, 103, 104],  # Pyramid Foyer Dark Space
+            0x04FA: [53, 60, 73, 80, 81, 102, 103, 104],  # Mansion First Barrier
+            0x0505: [53, 60, 73, 80, 81, 102, 103, 104]  # Mansion Second Barrier
         }
 
         # Database of overworld menus
         # FORMAT: { ID: [ShuffleID (0=no shuffle), Menu_ID, FromRegion, ToRegion, AssemblyLabel, ContinentName, AreaName]}
         # Names are 10 characters, padded with white space (underscores).
         self.overworld_menus = {
             # SW Continent "\x01"
-            1:  [0, 1, 10, 20, "Cape", "SW Continent", "South Cape"],
-            2:  [0, 1, 10, 30, "Ed",   "SW Continent", "Edward's__"],
-            3:  [0, 1, 10, 50, "Itry", "SW Continent", "Itory_____"],
-            4:  [0, 1, 10, 60, "Moon", "SW Continent", "Moon Tribe"],
-            5:  [0, 1, 10, 63, "Inca", "SW Continent", "Inca______"],
+            1: [0, 1, 10, 20, "Cape", "SW Continent", "South Cape"],
+            2: [0, 1, 10, 30, "Ed", "SW Continent", "Edward's__"],
+            3: [0, 1, 10, 50, "Itry", "SW Continent", "Itory_____"],
+            4: [0, 1, 10, 60, "Moon", "SW Continent", "Moon Tribe"],
+            5: [0, 1, 10, 63, "Inca", "SW Continent", "Inca______"],
 
             # SE Continent "\x02"
-            6:  [0, 2, 11, 102, "DCst", "SE Continent", "D. Coast__"],
-            7:  [0, 2, 11, 110, "Frej", "SE Continent", "Freejia___"],
-            8:  [0, 2, 11, 133, "Mine", "SE Continent", "D. Mine___"],
-            9:  [0, 2, 11, 160, "Neil", "SE Continent", "Neil's____"],
+            6: [0, 2, 11, 102, "DCst", "SE Continent", "D. Coast__"],
+            7: [0, 2, 11, 110, "Frej", "SE Continent", "Freejia___"],
+            8: [0, 2, 11, 133, "Mine", "SE Continent", "D. Mine___"],
+            9: [0, 2, 11, 160, "Neil", "SE Continent", "Neil's____"],
             10: [0, 2, 11, 162, "Nzca", "SE Continent", "Nazca_____"],
 
             # NE Continent "\x03"
             11: [0, 3, 12, 250, "Angl", "NE Continent", "Angel Vil."],
             12: [0, 3, 12, 280, "Wtma", "NE Continent", "Watermia__"],
             13: [0, 3, 12, 290, "GtWl", "NE Continent", "Great Wall"],
 
             # N Continent "\x04"
             14: [0, 4, 13, 310, "Euro", "N Continent", "Euro______"],
             15: [0, 4, 13, 330, "Kres", "N Continent", "Mt. Temple"],
             16: [0, 4, 13, 350, "NtVl", "N Continent", "Natives'__"],
             17: [0, 4, 13, 360, "Ankr", "N Continent", "Ankor Wat_"],
 
             # NW Continent Overworld "\x05"
-            18: [0, 5, 14, 400, "Dao",  "NW Continent", "Dao_______"],
+            18: [0, 5, 14, 400, "Dao", "NW Continent", "Dao_______"],
             19: [0, 5, 14, 410, "Pymd", "NW Continent", "Pyramid___"]
         }
 
-
         # Database of map exits
         # FORMAT: { ID: [0: Vanilla exit that reverses this one (0 if one-way), 
         #                1: ShuffleTo/ActLike (0 if no shuffle), 
         #                2: ShuffleFrom/BeActedLikeBy (0 if no shuffle), 
         #                3: FromRegion, 
         #                4: ToRegion,
         #                5: AssemblyLabel, 
@@ -6594,641 +7036,734 @@
         #                8: DungeonID (1 = EdDg, ..., 12 = Mansion), 
         #                9: PoolType (0 = never, 1 = ER pool, 2 = dungeon internal pool, 3 = dungeon entrance pool) 
         #                10: Name
         #               ] }
         self.deleted_exits = {}
         self.exits = {
             # Bosses; due to boss shuffle, all need a return exit and a post-defeat warp
-            1:  [ 2, 0, 0,  78,  97, "Map1EExit02", 0, True, 2, 0, "Castoth entrance (in)" ],
-            2:  [ 1, 0, 0,   0,   0, "Map29Exit01", 0, True, 2, 0, "Castoth entrance (out)" ],
-            3:  [ 0, 0, 0, 104, 102, "MapShipExitString", 0, True, 2, 0, "Post-Boss Warp to Diamond Coast" ],
-            
-            4:  [ 5, 0, 0, 171, 198, "Map4CExit01", 0, True, 4, 0, "Viper entrance (in)" ],
-            5:  [ 4, 0, 0,   0,   0, "Map55Exit01", 0, True, 4, 0, "Viper entrance (out)" ],
-            6:  [ 0, 0, 0, 198, 200, "MapViperExitString", 0, True, 4, 0, "Post-Boss Warp to Sea Palace" ],
-            
-            7:  [ 8, 0, 0, 241, 243, "MapVampEntranceString", 0, True, 5, 0, "Vampires entrance (in)" ],
-            8:  [ 7, 0, 0,   0,   0, "Map67Exit01", 0, True, 5, 0, "Vampires entrance (out)" ],
-            9:  [ 0, 0, 0, 242, 240, "Map66Exit03", 0, True, 5, 0, "Post-Boss Warp to Mu" ],  # Treated as warping to pedestals so the traverser doesn't path pedestals->boss->Mu
-            
-            10: [11, 0, 0, 301, 302, "Map88Exit02", 0, True, 7, 0, "Sand Fanger entrance (in)" ],
-            11: [10, 0, 0,   0,   0, "Map8AExit01", 0, True, 7, 0, "Sand Fanger entrance (out)" ],
-            12: [ 0, 0, 0, 303, 290, "Map8AExit02", 0, True, 7, 0, "Post-Boss Warp to Great Wall" ],
-            
-            13: [14, 0, 0, 414, 448, "MapMQEntranceString", 0, True, 10, 0, "Mummy Queen entrance (in)" ],
-            14: [13, 0, 0,   0,   0, "MapMQReturnString", 0, True, 10, 0, "Mummy Queen entrance (out)" ],
-            15: [ 0, 0, 0, 448, 415, "MapMQExitString", 0, True, 10, 0, "Post-Boss Warp to Pyramid" ],
-
-            16: [17, 0, 0, 470, 471, "MapE2Exit02", 0, True, 11, 0, "Babel statue boss corridor entrance (in)" ],
-            17: [16, 0, 0,   0,   0, "MapE3Exit01", 0, True, 11, 0, "Babel statue boss corridor entrance (out)" ],
-            18: [ 0, 0, 0, 472, 400, "MapBabelDaoWarpString", 0, True, 11, 0, "Post-Babel Warp to Dao" ],  # Warp effect of talking to the spirit at the top of Dao
-
-            19: [20, 0, 0, 481, 482, "MapE9Exit01", 0, True, 12, 0, "Solid Arm entrance (in)" ],
-            20: [19, 0, 0,   0,   0, "MapSolidArmReturnString", 0, True, 12, 0, "Solid Arm entrance (out)" ],
-            21: [ 0, 0, 0, 400, 400, "MapMansionBossDefeatedWarpString", 0, True, 12, 0, "Post-Mansion Warp to Dao"],  # Used if the Mansion boss isn't MQ2 or SA
+            1: [2, 0, 0, 78, 97, "Map1EExit02", 0, True, 2, 0, "Castoth entrance (in)"],
+            2: [1, 0, 0, 0, 0, "Map29Exit01", 0, True, 2, 0, "Castoth entrance (out)"],
+            3: [0, 0, 0, 104, 102, "MapShipExitString", 0, True, 2, 0, "Post-Boss Warp to Diamond Coast"],
+
+            4: [5, 0, 0, 171, 198, "Map4CExit01", 0, True, 4, 0, "Viper entrance (in)"],
+            5: [4, 0, 0, 0, 0, "Map55Exit01", 0, True, 4, 0, "Viper entrance (out)"],
+            6: [0, 0, 0, 198, 200, "MapViperExitString", 0, True, 4, 0, "Post-Boss Warp to Sea Palace"],
+
+            7: [8, 0, 0, 241, 243, "MapVampEntranceString", 0, True, 5, 0, "Vampires entrance (in)"],
+            8: [7, 0, 0, 0, 0, "Map67Exit01", 0, True, 5, 0, "Vampires entrance (out)"],
+            9: [0, 0, 0, 242, 240, "Map66Exit03", 0, True, 5, 0, "Post-Boss Warp to Mu"],
+            # Treated as warping to pedestals so the traverser doesn't path pedestals->boss->Mu
+
+            10: [11, 0, 0, 301, 302, "Map88Exit02", 0, True, 7, 0, "Sand Fanger entrance (in)"],
+            11: [10, 0, 0, 0, 0, "Map8AExit01", 0, True, 7, 0, "Sand Fanger entrance (out)"],
+            12: [0, 0, 0, 303, 290, "Map8AExit02", 0, True, 7, 0, "Post-Boss Warp to Great Wall"],
+
+            13: [14, 0, 0, 414, 448, "MapMQEntranceString", 0, True, 10, 0, "Mummy Queen entrance (in)"],
+            14: [13, 0, 0, 0, 0, "MapMQReturnString", 0, True, 10, 0, "Mummy Queen entrance (out)"],
+            15: [0, 0, 0, 448, 415, "MapMQExitString", 0, True, 10, 0, "Post-Boss Warp to Pyramid"],
+
+            16: [17, 0, 0, 470, 471, "MapE2Exit02", 0, True, 11, 0, "Babel statue boss corridor entrance (in)"],
+            17: [16, 0, 0, 0, 0, "MapE3Exit01", 0, True, 11, 0, "Babel statue boss corridor entrance (out)"],
+            18: [0, 0, 0, 472, 400, "MapBabelDaoWarpString", 0, True, 11, 0, "Post-Babel Warp to Dao"],
+            # Warp effect of talking to the spirit at the top of Dao
+
+            19: [20, 0, 0, 481, 482, "MapE9Exit01", 0, True, 12, 0, "Solid Arm entrance (in)"],
+            20: [19, 0, 0, 0, 0, "MapSolidArmReturnString", 0, True, 12, 0, "Solid Arm entrance (out)"],
+            21: [0, 0, 0, 400, 400, "MapMansionBossDefeatedWarpString", 0, True, 12, 0, "Post-Mansion Warp to Dao"],
+            # Used if the Mansion boss isn't MQ2 or SA
 
             # Passage Menus
-            22: [0, 0, 0, 15,  28, "", 0, False, 0, 0, "Seth: Passage 1 (South Cape)" ],
-            23: [0, 0, 0, 15, 102, "", 0, False, 0, 0, "Seth: Passage 2 (Diamond Coast)" ],
-            24: [0, 0, 0, 15, 280, "", 0, False, 0, 0, "Seth: Passage 3 (Watermia)" ],
-            25: [0, 0, 0, 16,  60, "", 0, False, 0, 0, "Moon Tribe: Passage 1 (Moon Tribe)" ],
-            26: [0, 0, 0, 16, 200, "", 0, False, 0, 0, "Moon Tribe: Passage 2 (Seaside Palace)" ],
-            27: [0, 0, 0, 17, 161, "", 0, False, 0, 0, "Neil: Passage 1 (Neil's)" ],
-            28: [0, 0, 0, 17, 314, "", 0, False, 0, 0, "Neil: Passage 2 (Euro)" ],
-            29: [0, 0, 0, 17, 402, "", 0, False, 0, 0, "Neil: Passage 3 (Dao)" ],
-            30: [0, 0, 0, 17, 460, "", 0, False, 0, 0, "Neil: Passage 4 (Babel)" ],
+            22: [0, 0, 0, 15, 28, "", 0, False, 0, 0, "Seth: Passage 1 (South Cape)"],
+            23: [0, 0, 0, 15, 102, "", 0, False, 0, 0, "Seth: Passage 2 (Diamond Coast)"],
+            24: [0, 0, 0, 15, 280, "", 0, False, 0, 0, "Seth: Passage 3 (Watermia)"],
+            25: [0, 0, 0, 16, 60, "", 0, False, 0, 0, "Moon Tribe: Passage 1 (Moon Tribe)"],
+            26: [0, 0, 0, 16, 200, "", 0, False, 0, 0, "Moon Tribe: Passage 2 (Seaside Palace)"],
+            27: [0, 0, 0, 17, 161, "", 0, False, 0, 0, "Neil: Passage 1 (Neil's)"],
+            28: [0, 0, 0, 17, 314, "", 0, False, 0, 0, "Neil: Passage 2 (Euro)"],
+            29: [0, 0, 0, 17, 402, "", 0, False, 0, 0, "Neil: Passage 3 (Dao)"],
+            30: [0, 0, 0, 17, 460, "", 0, False, 0, 0, "Neil: Passage 4 (Babel)"],
 
             # South Cape
-            31: [32, 0, 0, 20, 22, "Map01Exit02", 0, False, 0, 1, "South Cape: School main (in)" ],
-            32: [31, 0, 0,  0,  0, "Map08Exit02", 0, False, 0, 1, "South Cape: School main (out)" ],
-            33: [34, 0, 0, 21, 22, "Map01Exit09", 0, False, 0, 1, "South Cape: School roof (in)" ],
-            34: [33, 0, 0,  0,  0, "Map08Exit01", 0, False, 0, 1, "South Cape: School roof (out)" ],
-            35: [36, 0, 0, 20, 23, "Map01Exit06", 0, False, 0, 1, "South Cape: Will's House (in)" ],
-            36: [35, 0, 0,  0,  0, "Map06Exit01", 0, False, 0, 1, "South Cape: Will's House (out)" ],
-            37: [38, 0, 0, 20, 24, "Map01Exit07", 0, False, 0, 1, "South Cape: East House (in)" ],
-            38: [37, 0, 0,  0,  0, "Map07Exit01", 0, False, 0, 1, "South Cape: East House (out)" ],
-            39: [40, 0, 0, 20, 27, "Map01Exit04", 0, False, 0, 1, "South Cape: Erik's House main (in)" ],
-            40: [39, 0, 0,  0,  0, "Map04Exit01", 0, False, 0, 1, "South Cape: Erik's House main (out)" ],
-            41: [42, 0, 0, 20, 27, "Map01Exit0A", 0, False, 0, 1, "South Cape: Erik's House roof (in)" ],
-            42: [41, 0, 0,  0,  0, "Map04Exit02", 0, False, 0, 1, "South Cape: Erik's House roof (out)" ],
-            43: [44, 0, 0, 20, 26, "Map01Exit03", 0, False, 0, 1, "South Cape: Lance's House (in)" ],
-            44: [43, 0, 0,  0,  0, "Map03Exit01", 0, False, 0, 1, "South Cape: Lance's House (out)" ],
-            45: [46, 0, 0, 20, 25, "Map01Exit05", 0, False, 0, 1, "South Cape: Seth's House (in)" ],
-            46: [45, 0, 0,  0,  0, "Map05Exit01", 0, False, 0, 1, "South Cape: Seth's House (out)" ],
-            47: [48, 0, 0, 20, 28, "Map01Exit08", 0, False, 0, 1, "South Cape: Seaside Cave (in)" ],
-            48: [47, 0, 0,  0,  0, "Map02Exit01", 0, False, 0, 1, "South Cape: Seaside Cave (out)" ],
+            31: [32, 0, 0, 20, 22, "Map01Exit02", 0, False, 0, 1, "South Cape: School main (in)"],
+            32: [31, 0, 0, 0, 0, "Map08Exit02", 0, False, 0, 1, "South Cape: School main (out)"],
+            33: [34, 0, 0, 21, 22, "Map01Exit09", 0, False, 0, 1, "South Cape: School roof (in)"],
+            34: [33, 0, 0, 0, 0, "Map08Exit01", 0, False, 0, 1, "South Cape: School roof (out)"],
+            35: [36, 0, 0, 20, 23, "Map01Exit06", 0, False, 0, 1, "South Cape: Will's House (in)"],
+            36: [35, 0, 0, 0, 0, "Map06Exit01", 0, False, 0, 1, "South Cape: Will's House (out)"],
+            37: [38, 0, 0, 20, 24, "Map01Exit07", 0, False, 0, 1, "South Cape: East House (in)"],
+            38: [37, 0, 0, 0, 0, "Map07Exit01", 0, False, 0, 1, "South Cape: East House (out)"],
+            39: [40, 0, 0, 20, 27, "Map01Exit04", 0, False, 0, 1, "South Cape: Erik's House main (in)"],
+            40: [39, 0, 0, 0, 0, "Map04Exit01", 0, False, 0, 1, "South Cape: Erik's House main (out)"],
+            41: [42, 0, 0, 20, 27, "Map01Exit0A", 0, False, 0, 1, "South Cape: Erik's House roof (in)"],
+            42: [41, 0, 0, 0, 0, "Map04Exit02", 0, False, 0, 1, "South Cape: Erik's House roof (out)"],
+            43: [44, 0, 0, 20, 26, "Map01Exit03", 0, False, 0, 1, "South Cape: Lance's House (in)"],
+            44: [43, 0, 0, 0, 0, "Map03Exit01", 0, False, 0, 1, "South Cape: Lance's House (out)"],
+            45: [46, 0, 0, 20, 25, "Map01Exit05", 0, False, 0, 1, "South Cape: Seth's House (in)"],
+            46: [45, 0, 0, 0, 0, "Map05Exit01", 0, False, 0, 1, "South Cape: Seth's House (out)"],
+            47: [48, 0, 0, 20, 28, "Map01Exit08", 0, False, 0, 1, "South Cape: Seaside Cave (in)"],
+            48: [47, 0, 0, 0, 0, "Map02Exit01", 0, False, 0, 1, "South Cape: Seaside Cave (out)"],
 
             # Edward's / Prison
-            50: [51, 0, 0, 31, 49, "Map0AExit01", 0, False, 1, 1, "Tunnel back entrance (in)" ],
-            51: [50, 0, 0,  0,  0, "Map13Exit02", 0, False, 1, 1, "Tunnel back entrance (out)" ],
-            52: [53, 0, 0, 33, 40, "Map0BExit01", 0, False, 1, 1, "Tunnel entrance (in)" ],
-            53: [52, 0, 0,  0,  0, "Map0CExit01", 0, False, 1, 1, "Tunnel entrance (out)" ],
-            54: [ 0, 0, 0, 30, 32, "MapPrisonWarpString", 0, False, 0, 1, "Prison entrance (king)" ],
+            50: [51, 0, 0, 31, 49, "Map0AExit01", 0, False, 1, 1, "Tunnel back entrance (in)"],
+            51: [50, 0, 0, 0, 0, "Map13Exit02", 0, False, 1, 1, "Tunnel back entrance (out)"],
+            52: [53, 0, 0, 33, 40, "Map0BExit01", 0, False, 1, 1, "Tunnel entrance (in)"],
+            53: [52, 0, 0, 0, 0, "Map0CExit01", 0, False, 1, 1, "Tunnel entrance (out)"],
+            54: [0, 0, 0, 30, 32, "MapPrisonWarpString", 0, False, 0, 1, "Prison entrance (king)"],
 
             # Tunnel
-            60: [61, 0, 0, 40, 41, "Map0CExit02", 0, False, 1, 3, "U. Tunnel: Entry exit to East (12->13)" ],
-            61: [60, 0, 0,  0,  0, "Map0DExit01", 0, False, 1, 2, "U. Tunnel: East room N exit (13->12)" ],
-            62: [63, 0, 0, 41, 38, "Map0DExit02", 0, False, 1, 2, "U. Tunnel: East room S exit (13->14)" ],
-            63: [62, 0, 0,  0,  0, "Map0EExit01", 0, False, 1, 2, "U. Tunnel: South room NE exit (14->13)" ],
-            64: [65, 0, 0, 42, 43, "Map0EExit02", 0, False, 1, 2, "U. Tunnel: South room NW exit (14->15)" ],
-            65: [64, 0, 0,  0,  0, "Map0FExit02", 0, False, 1, 2, "U. Tunnel: West room S exit (15->14)" ],
-            66: [67, 0, 0, 43, 44, "Map0FExit03", 0, False, 1, 2, "U. Tunnel: West room C exit (15->16)" ],
-            67: [66, 0, 0,  0,  0, "Map10Exit01", 0, False, 1, 2, "U. Tunnel: Chest room exit (16->15)" ],
-            68: [69, 0, 0, 43, 45, "Map0FExit01", 0, False, 1, 2, "U. Tunnel: West room N exit (15->17)" ],
-            69: [68, 0, 0,  0,  0, "Map11Exit01", 0, False, 1, 2, "U. Tunnel: Flower room S door (17->15)" ],
-            70: [71, 0, 0, 45, 47, "Map11Exit02", 0, False, 1, 2, "U. Tunnel: Flower room N door (17->18)" ],
-            71: [70, 0, 0,  0,  0, "Map12Exit01", 0, False, 1, 2, "U. Tunnel: BigRoom S exit (18->17)" ],
-            72: [73, 0, 0,706, 49, "Map12Exit02", 0, False, 1, 2, "U. Tunnel: BigRoom N exit (18->19)" ],
-            73: [72, 0, 0,  0,  0, "Map13Exit01", 0, False, 1, 3 if self.town_shuffle else 2, "U. Tunnel: Barrel room S exit (19->18)" ],
-            
+            60: [61, 0, 0, 40, 41, "Map0CExit02", 0, False, 1, 3, "U. Tunnel: Entry exit to East (12->13)"],
+            61: [60, 0, 0, 0, 0, "Map0DExit01", 0, False, 1, 2, "U. Tunnel: East room N exit (13->12)"],
+            62: [63, 0, 0, 41, 38, "Map0DExit02", 0, False, 1, 2, "U. Tunnel: East room S exit (13->14)"],
+            63: [62, 0, 0, 0, 0, "Map0EExit01", 0, False, 1, 2, "U. Tunnel: South room NE exit (14->13)"],
+            64: [65, 0, 0, 42, 43, "Map0EExit02", 0, False, 1, 2, "U. Tunnel: South room NW exit (14->15)"],
+            65: [64, 0, 0, 0, 0, "Map0FExit02", 0, False, 1, 2, "U. Tunnel: West room S exit (15->14)"],
+            66: [67, 0, 0, 43, 44, "Map0FExit03", 0, False, 1, 2, "U. Tunnel: West room C exit (15->16)"],
+            67: [66, 0, 0, 0, 0, "Map10Exit01", 0, False, 1, 2, "U. Tunnel: Chest room exit (16->15)"],
+            68: [69, 0, 0, 43, 45, "Map0FExit01", 0, False, 1, 2, "U. Tunnel: West room N exit (15->17)"],
+            69: [68, 0, 0, 0, 0, "Map11Exit01", 0, False, 1, 2, "U. Tunnel: Flower room S door (17->15)"],
+            70: [71, 0, 0, 45, 47, "Map11Exit02", 0, False, 1, 2, "U. Tunnel: Flower room N door (17->18)"],
+            71: [70, 0, 0, 0, 0, "Map12Exit01", 0, False, 1, 2, "U. Tunnel: BigRoom S exit (18->17)"],
+            72: [73, 0, 0, 706, 49, "Map12Exit02", 0, False, 1, 2, "U. Tunnel: BigRoom N exit (18->19)"],
+            73: [72, 0, 0, 0, 0, "Map13Exit01", 0, False, 1, 3 if self.town_shuffle else 2,
+                 "U. Tunnel: Barrel room S exit (19->18)"],
+
             # Itory
-            80: [81, 0, 0, 51, 53, "Map15Exit01", 0, False, 0, 1, "Itory: West House (in)" ],
-            81: [80, 0, 0,  0,  0, "Map16Exit01", 0, False, 0, 1, "Itory: West House (out)" ],
-            82: [83, 0, 0, 51, 54, "Map15Exit04", 0, False, 0, 1, "Itory: North House (in)" ],
-            83: [82, 0, 0,  0,  0, "Map18Exit01", 0, False, 0, 1, "Itory: North House (out)" ],
-            84: [85, 0, 0, 51, 55, "Map15Exit02", 0, False, 0, 1, "Itory: Lilly Front Door (in)" ],
-            85: [84, 0, 0,  0,  0, "Map17Exit01", 0, False, 0, 1, "Itory: Lilly Front Door (out)" ],
-            86: [87, 0, 0, 52, 55, "Map15Exit03", 0, False, 0, 1, "Itory: Lilly Back Door (in)" ],
-            87: [86, 0, 0,  0,  0, "Map17Exit02", 0, False, 0, 1, "Itory: Lilly Back Door (out)" ],
-            88: [89, 0, 0, 51, 56, "Map15Exit05", 0, False, 0, 1, "Itory Cave (in)" ],
-            89: [88, 0, 0,  0,  0, "Map19Exit01", 0, False, 0, 1, "Itory Cave (out)" ],
-            90: [91, 0, 0, 56, 58, "Map19Exit02", 0, False, 0, 1, "Itory Cave Hidden Room (in)" ],  # always linked?
-            91: [90, 0, 0,  0,  0, "Map19Exit03", 0, False, 0, 1, "Itory Cave Hidden Room (out)" ],
-            
+            80: [81, 0, 0, 51, 53, "Map15Exit01", 0, False, 0, 1, "Itory: West House (in)"],
+            81: [80, 0, 0, 0, 0, "Map16Exit01", 0, False, 0, 1, "Itory: West House (out)"],
+            82: [83, 0, 0, 51, 54, "Map15Exit04", 0, False, 0, 1, "Itory: North House (in)"],
+            83: [82, 0, 0, 0, 0, "Map18Exit01", 0, False, 0, 1, "Itory: North House (out)"],
+            84: [85, 0, 0, 51, 55, "Map15Exit02", 0, False, 0, 1, "Itory: Lilly Front Door (in)"],
+            85: [84, 0, 0, 0, 0, "Map17Exit01", 0, False, 0, 1, "Itory: Lilly Front Door (out)"],
+            86: [87, 0, 0, 52, 55, "Map15Exit03", 0, False, 0, 1, "Itory: Lilly Back Door (in)"],
+            87: [86, 0, 0, 0, 0, "Map17Exit02", 0, False, 0, 1, "Itory: Lilly Back Door (out)"],
+            88: [89, 0, 0, 51, 56, "Map15Exit05", 0, False, 0, 1, "Itory Cave (in)"],
+            89: [88, 0, 0, 0, 0, "Map19Exit01", 0, False, 0, 1, "Itory Cave (out)"],
+            90: [91, 0, 0, 56, 58, "Map19Exit02", 0, False, 0, 1, "Itory Cave Hidden Room (in)"],  # always linked?
+            91: [90, 0, 0, 0, 0, "Map19Exit03", 0, False, 0, 1, "Itory Cave Hidden Room (out)"],
+
             # Moon Tribe
-            100: [101, 0, 0, 60,  61, "Map1AExit02", 0, False, 0, 1, "Moon Tribe Cave (in)" ],
-            101: [100, 0, 0,  0,   0, "Map1BExit01", 0, False, 0, 1, "Moon Tribe Cave (out)" ],
-            102: [  0, 0, 0, 64, 170, "MapMoonWarpString", 0, False, 4,  1, "Moon Tribe: Sky Garden passage" ],
-            
+            100: [101, 0, 0, 60, 61, "Map1AExit02", 0, False, 0, 1, "Moon Tribe Cave (in)"],
+            101: [100, 0, 0, 0, 0, "Map1BExit01", 0, False, 0, 1, "Moon Tribe Cave (out)"],
+            102: [0, 0, 0, 64, 170, "MapMoonWarpString", 0, False, 4, 1, "Moon Tribe: Sky Garden passage"],
+
             # Inca foyer
-            110: [111, 0, 0, 63,  70, "Map1CExit01", 0, False, 2, 1, "Inca Ruins entrance (in)" ],
-            111: [110, 0, 0,  0,   0, "Map1DExit01", 0, False, 2, 1, "Inca Ruins entrance (out)" ],
-            #114: [  0, 0, 0, 65, 102, "", 0, False, False,  True, "Inca: Diamond Coast passage" ],
-            
+            110: [111, 0, 0, 63, 70, "Map1CExit01", 0, False, 2, 1, "Inca Ruins entrance (in)"],
+            111: [110, 0, 0, 0, 0, "Map1DExit01", 0, False, 2, 1, "Inca Ruins entrance (out)"],
+            # 114: [  0, 0, 0, 65, 102, "", 0, False, False,  True, "Inca: Diamond Coast passage" ],
+
             # Inca Ruins
-            118: [119, 0, 0, 79,  69, "Map1FExit02", 0, False,  2, 2, "Inca: Statue Puzzle N door (31->31)" ],
-            119: [118, 0, 0,  0,   0, "Map1FExit03", 0, False,  2, 2, "Inca: U-Turn SE door (31->31)" ],
-            120: [121, 0, 0, 70,  89, "Map1DExit07", 0, False,  2, 2, "Inca: Exterior->DBlock (29->37) East door" ],
-            121: [120, 0, 0,  0,   0, "Map25Exit01", 0, False,  2, 2, "Inca: DBlock->Exterior (37->29) East door" ],
-            122: [123, 0, 0, 89,  94, "Map25Exit03", 0, False,  2, 2, "Inca: DBlock room W exit (37->39)" ],
-            123: [122, 0, 0,  0,   0, "Map27Exit01", 0, False,  2, 2, "Inca: Room West of DBlock, E exit (39->37)" ],
-            124: [125, 0, 0, 94,  71, "Map27Exit02", 0, False,  2, 2, "Inca: Room West of DBlock, S exit (39->29)" ],
-            125: [124, 0, 0,  0,   0, "Map1DExit0A", 0, False,  2, 2, "Inca: Exterior NW chest door (29->39)" ],
-            126: [127, 0, 0, 89,  72, "Map25Exit02", 0, False,  2, 2, "Inca: DBlock->Exterior (37->29) West door" ],
-            127: [126, 0, 0,  0,   0, "Map1DExit08", 0, False,  2, 2, "Inca: Exterior->DBlock (29->37) West door" ],
-            128: [129, 0, 0, 72,  91, "Map1DExit09", 0, False,  2, 2, "Inca: Exterior Center-East Exit (29->38)" ],
-            129: [128, 0, 0,  0,   0, "Map26Exit02", 0, False,  2, 2, "Inca: Divided Room South Exit (38->29)" ],
-            130: [131, 0, 0, 73,  80, "Map1DExit03", 0, False,  2, 2, "Inca: Exterior Center Drop-Down Exit (29->32)" ],
-            131: [130, 0, 0,  0,   0, "Map20Exit01", 0, False,  2, 2, "Inca: Slug room S exit (32->29)" ],
-            132: [133, 0, 0, 81,  85, "Map20Exit02", 0, False,  2, 2, "Inca: Slug room N exit (32->35)" ],
-            133: [132, 0, 0,  0,   0, "Map23Exit01", 0, False,  2, 2, "Inca: Freedan room N exit (35->32)" ],
-            134: [135, 0, 0, 85,  74, "Map23Exit03", 0, False,  2, 2, "Inca: Freedan room SE exit (35->29)" ],
-            135: [134, 0, 0,  0,   0, "Map1DExit06", 0, False,  2, 2, "Inca: Exterior Center-West Lower Exit (29->35)" ],
-            136: [137, 0, 0, 74,  79, "Map1DExit02", 0, False,  2, 2, "Inca: Exterior Center-West Upper Exit (29->31)" ],
-            137: [136, 0, 0,  0,   0, "Map1FExit04", 0, False,  2, 2, "Inca: Statue Puzzle S door (31->29)" ],
-            138: [139, 0, 0, 69,  95, "Map1FExit01", 0, False,  2, 2, "Inca: U-Turn SW door (31->40)" ],
-            139: [138, 0, 0,  0,   0, "Map28Exit01", 0, False,  2, 2, "Inca: DS Spike Hall NE exit (40->31)" ],
-            140: [141, 0, 0, 96,  76, "Map28Exit02", 0, False,  2, 2, "Inca: DS Spike Hall S exit (40->29)" ],
-            141: [140, 0, 0,  0,   0, "Map1DExit0B", 0, False,  2, 2, "Inca: Exterior Singing Statue door (29->40)" ],
-            142: [143, 0, 0, 86,  82, "Map23Exit02", 0, False,  2, 2, "Inca: Freedan room SW exit (35->33)" ],
-            143: [142, 0, 0,  0,   0, "Map21Exit02", 0, False,  2, 2, "Inca: Water room N exit (33->35)" ],
-            144: [145, 0, 0, 83,  75, "Map21Exit01", 0, False,  2, 2, "Inca: Water room S exit (33->29)" ],
-            145: [144, 0, 0,  0,   0, "Map1DExit04", 0, False,  2, 2, "Inca: Exterior far SW door (29->33)" ],
-            146: [147, 0, 0, 99,  84, "Map1DExit05", 0, False,  2, 2, "Inca: Exterior far SE door (29->34)" ], # Special quasi-coupled case to allow for Z-ladder glitch
-            147: [146, 0, 0, 84,  75, "Map22Exit01", 0, False,  2, 2, "Inca: BigRoom SW exit (34->29)" ],
-            148: [149, 0, 0, 84,  93, "Map22Exit03", 0, False,  2, 2, "Inca: BigRoom NE exit (34->38)" ],
-            149: [148, 0, 0,  0,   0, "Map26Exit01", 0, False,  2, 2, "Inca: Divided Room North Exit (38->34)" ],
-            150: [151, 0, 0, 84,  87, "Map22Exit02", 0, False,  2, 2, "Inca: BigRoom SE exit (34->36)" ],
-            151: [150, 0, 0,  0,   0, "Map24Exit01", 0, False,  2, 2, "Inca: Golden Tile Room N exit (36->34)" ],
-            152: [153, 0, 0, 87,  77, "Map24Exit02", 0, False,  2, 2, "Inca: Golden Tile Room S exit (36->30)" ],
-            153: [152, 0, 0,  0,   0, "Map1EExit01", 0, False,  2, 2, "Inca: Outside Castoth, E exit (30->36)" ],
-            154: [  0, 0, 0, 98, 100, "", 0, False,  0, 0, "Gold Ship entrance" ],
-            
+            118: [119, 0, 0, 79, 69, "Map1FExit02", 0, False, 2, 2, "Inca: Statue Puzzle N door (31->31)"],
+            119: [118, 0, 0, 0, 0, "Map1FExit03", 0, False, 2, 2, "Inca: U-Turn SE door (31->31)"],
+            120: [121, 0, 0, 70, 89, "Map1DExit07", 0, False, 2, 2, "Inca: Exterior->DBlock (29->37) East door"],
+            121: [120, 0, 0, 0, 0, "Map25Exit01", 0, False, 2, 2, "Inca: DBlock->Exterior (37->29) East door"],
+            122: [123, 0, 0, 89, 94, "Map25Exit03", 0, False, 2, 2, "Inca: DBlock room W exit (37->39)"],
+            123: [122, 0, 0, 0, 0, "Map27Exit01", 0, False, 2, 2, "Inca: Room West of DBlock, E exit (39->37)"],
+            124: [125, 0, 0, 94, 71, "Map27Exit02", 0, False, 2, 2, "Inca: Room West of DBlock, S exit (39->29)"],
+            125: [124, 0, 0, 0, 0, "Map1DExit0A", 0, False, 2, 2, "Inca: Exterior NW chest door (29->39)"],
+            126: [127, 0, 0, 89, 72, "Map25Exit02", 0, False, 2, 2, "Inca: DBlock->Exterior (37->29) West door"],
+            127: [126, 0, 0, 0, 0, "Map1DExit08", 0, False, 2, 2, "Inca: Exterior->DBlock (29->37) West door"],
+            128: [129, 0, 0, 72, 91, "Map1DExit09", 0, False, 2, 2, "Inca: Exterior Center-East Exit (29->38)"],
+            129: [128, 0, 0, 0, 0, "Map26Exit02", 0, False, 2, 2, "Inca: Divided Room South Exit (38->29)"],
+            130: [131, 0, 0, 73, 80, "Map1DExit03", 0, False, 2, 2, "Inca: Exterior Center Drop-Down Exit (29->32)"],
+            131: [130, 0, 0, 0, 0, "Map20Exit01", 0, False, 2, 2, "Inca: Slug room S exit (32->29)"],
+            132: [133, 0, 0, 81, 85, "Map20Exit02", 0, False, 2, 2, "Inca: Slug room N exit (32->35)"],
+            133: [132, 0, 0, 0, 0, "Map23Exit01", 0, False, 2, 2, "Inca: Freedan room N exit (35->32)"],
+            134: [135, 0, 0, 85, 74, "Map23Exit03", 0, False, 2, 2, "Inca: Freedan room SE exit (35->29)"],
+            135: [134, 0, 0, 0, 0, "Map1DExit06", 0, False, 2, 2, "Inca: Exterior Center-West Lower Exit (29->35)"],
+            136: [137, 0, 0, 74, 79, "Map1DExit02", 0, False, 2, 2, "Inca: Exterior Center-West Upper Exit (29->31)"],
+            137: [136, 0, 0, 0, 0, "Map1FExit04", 0, False, 2, 2, "Inca: Statue Puzzle S door (31->29)"],
+            138: [139, 0, 0, 69, 95, "Map1FExit01", 0, False, 2, 2, "Inca: U-Turn SW door (31->40)"],
+            139: [138, 0, 0, 0, 0, "Map28Exit01", 0, False, 2, 2, "Inca: DS Spike Hall NE exit (40->31)"],
+            140: [141, 0, 0, 96, 76, "Map28Exit02", 0, False, 2, 2, "Inca: DS Spike Hall S exit (40->29)"],
+            141: [140, 0, 0, 0, 0, "Map1DExit0B", 0, False, 2, 2, "Inca: Exterior Singing Statue door (29->40)"],
+            142: [143, 0, 0, 86, 82, "Map23Exit02", 0, False, 2, 2, "Inca: Freedan room SW exit (35->33)"],
+            143: [142, 0, 0, 0, 0, "Map21Exit02", 0, False, 2, 2, "Inca: Water room N exit (33->35)"],
+            144: [145, 0, 0, 83, 75, "Map21Exit01", 0, False, 2, 2, "Inca: Water room S exit (33->29)"],
+            145: [144, 0, 0, 0, 0, "Map1DExit04", 0, False, 2, 2, "Inca: Exterior far SW door (29->33)"],
+            146: [147, 0, 0, 99, 84, "Map1DExit05", 0, False, 2, 2, "Inca: Exterior far SE door (29->34)"],
+            # Special quasi-coupled case to allow for Z-ladder glitch
+            147: [146, 0, 0, 84, 75, "Map22Exit01", 0, False, 2, 2, "Inca: BigRoom SW exit (34->29)"],
+            148: [149, 0, 0, 84, 93, "Map22Exit03", 0, False, 2, 2, "Inca: BigRoom NE exit (34->38)"],
+            149: [148, 0, 0, 0, 0, "Map26Exit01", 0, False, 2, 2, "Inca: Divided Room North Exit (38->34)"],
+            150: [151, 0, 0, 84, 87, "Map22Exit02", 0, False, 2, 2, "Inca: BigRoom SE exit (34->36)"],
+            151: [150, 0, 0, 0, 0, "Map24Exit01", 0, False, 2, 2, "Inca: Golden Tile Room N exit (36->34)"],
+            152: [153, 0, 0, 87, 77, "Map24Exit02", 0, False, 2, 2, "Inca: Golden Tile Room S exit (36->30)"],
+            153: [152, 0, 0, 0, 0, "Map1EExit01", 0, False, 2, 2, "Inca: Outside Castoth, E exit (30->36)"],
+            154: [0, 0, 0, 98, 100, "", 0, False, 0, 0, "Gold Ship entrance"],
+
             # Gold Ship
-            160: [161, 0, 0, 100, 101, "", 0, False, 0, 0, "Gold Ship Interior (in)" ],
-            161: [160, 0, 0,   0,   0, "", 0, False, 0, 0, "Gold Ship Interior (out)" ],
-            
+            160: [161, 0, 0, 100, 101, "", 0, False, 0, 0, "Gold Ship Interior (in)"],
+            161: [160, 0, 0, 0, 0, "", 0, False, 0, 0, "Gold Ship Interior (out)"],
+
             # Diamond Coast
-            172: [173, 0, 0, 102, 103, "Map30Exit01", 0, False, 0, 1, "Coast House (in)" ],
-            173: [172, 0, 0,   0,   0, "Map31Exit01", 0, False, 0, 1, "Coast House (out)" ],
-            
+            172: [173, 0, 0, 102, 103, "Map30Exit01", 0, False, 0, 1, "Coast House (in)"],
+            173: [172, 0, 0, 0, 0, "Map31Exit01", 0, False, 0, 1, "Coast House (out)"],
+
             # Freejia
-            182: [183, 0, 0, 110, 116, "Map32Exit05", 0, False, 0, 1, "Freejia: West House (in)" ],
-            183: [182, 0, 0,   0,   0, "Map36Exit01", 0, False, 0, 1, "Freejia: West House (out)" ],
-            184: [185, 0, 0, 110, 117, "Map32Exit06", 0, False, 0, 1, "Freejia: 2-story House (in)" ],
-            185: [184, 0, 0,   0,   0, "Map37Exit01", 0, False, 0, 1, "Freejia: 2-story House (out)" ],
-            186: [187, 0, 0, 111, 117, "Map32Exit07", 0, False, 0, 1, "Freejia: 2-story Roof (in)" ],
-            187: [186, 0, 0,   0,   0, "Map37Exit02", 0, False, 0, 1, "Freejia: 2-story Roof (out)" ],
-            188: [189, 0, 0, 110, 118, "Map32Exit08", 0, False, 0, 1, "Freejia: Lovers' House (in)" ],
-            189: [188, 0, 0,   0,   0, "Map38Exit01", 0, False, 0, 1, "Freejia: Lovers' House (out)" ],
-            190: [191, 0, 0, 110, 119, "Map32Exit09", 0, False, 0, 1, "Freejia: Hotel (in)" ],
-            191: [190, 0, 0,   0,   0, "Map39Exit01", 0, False, 0, 1, "Freejia: Hotel (out)" ],
-            192: [193, 0, 0, 119, 120, "Map39Exit02", 0, False, 0, 1, "Freejia: Hotel West Room (in)" ],
-            193: [192, 0, 0,   0,   0, "Map39Exit04", 0, False, 0, 1, "Freejia: Hotel West Room (out)" ],
-            194: [195, 0, 0, 119, 121, "Map39Exit03", 0, False, 0, 1, "Freejia: Hotel East Room (in)" ],
-            195: [194, 0, 0,   0,   0, "Map39Exit05", 0, False, 0, 1, "Freejia: Hotel East Room (out)" ],
-            196: [197, 0, 0, 110, 122, "Map32Exit0A", 0, False, 0, 1, "Freejia: Laborer House (in)" ],
-            197: [196, 0, 0,   0,   0, "Map3AExit02", 0, False, 0, 1, "Freejia: Laborer House (out)" ],
-            198: [199, 0, 0, 112, 122, "Map32Exit0B", 0, False, 0, 1, "Freejia: Laborer Roof (in)" ],
-            199: [198, 0, 0,   0,   0, "Map3AExit01", 0, False, 0, 1, "Freejia: Laborer Roof (out)" ],
-            200: [201, 0, 0, 110, 123, "Map32Exit0C", 0, False, 0, 1, "Freejia: Messy House (in)" ],
-            201: [200, 0, 0,   0,   0, "Map3BExit01", 0, False, 0, 1, "Freejia: Messy House (out)" ],
-            202: [203, 0, 0, 110, 124, "Map32Exit01", 0, False, 0, 1, "Freejia: Erik House (in)" ],
-            203: [202, 0, 0,   0,   0, "Map33Exit01", 0, False, 0, 1, "Freejia: Erik House (out)" ],
-            204: [205, 0, 0, 110, 125, "Map32Exit02", 0, False, 0, 1, "Freejia: Dark Space House (in)" ],
-            205: [204, 0, 0,   0,   0, "Map34Exit01", 0, False, 0, 1, "Freejia: Dark Space House (out)" ],
-            206: [207, 0, 0, 110, 126, "Map32Exit03", 0, False, 0, 1, "Freejia: Labor Trade House (in)" ],
-            207: [206, 0, 0,   0,   0, "Map35Exit01", 0, False, 0, 1, "Freejia: Labor Trade House (out)" ],
-            208: [209, 0, 0, 113, 126, "Map32Exit04", 0, False, 0, 1, "Freejia: Labor Trade Roof (in)" ],
-            209: [208, 0, 0,   0,   0, "Map35Exit02", 0, False, 0, 1, "Freejia: Labor Trade Roof (out)" ],
-            210: [211, 0, 0, 114, 127, "Map32Exit0D", 0, False, 0, 1, "Freejia: Labor Market (in)" ],
-            211: [210, 0, 0,   0,   0, "Map3CExit01", 0, False, 0, 1, "Freejia: Labor Market (out)" ],
-            
+            182: [183, 0, 0, 110, 116, "Map32Exit05", 0, False, 0, 1, "Freejia: West House (in)"],
+            183: [182, 0, 0, 0, 0, "Map36Exit01", 0, False, 0, 1, "Freejia: West House (out)"],
+            184: [185, 0, 0, 110, 117, "Map32Exit06", 0, False, 0, 1, "Freejia: 2-story House (in)"],
+            185: [184, 0, 0, 0, 0, "Map37Exit01", 0, False, 0, 1, "Freejia: 2-story House (out)"],
+            186: [187, 0, 0, 111, 117, "Map32Exit07", 0, False, 0, 1, "Freejia: 2-story Roof (in)"],
+            187: [186, 0, 0, 0, 0, "Map37Exit02", 0, False, 0, 1, "Freejia: 2-story Roof (out)"],
+            188: [189, 0, 0, 110, 118, "Map32Exit08", 0, False, 0, 1, "Freejia: Lovers' House (in)"],
+            189: [188, 0, 0, 0, 0, "Map38Exit01", 0, False, 0, 1, "Freejia: Lovers' House (out)"],
+            190: [191, 0, 0, 110, 119, "Map32Exit09", 0, False, 0, 1, "Freejia: Hotel (in)"],
+            191: [190, 0, 0, 0, 0, "Map39Exit01", 0, False, 0, 1, "Freejia: Hotel (out)"],
+            192: [193, 0, 0, 119, 120, "Map39Exit02", 0, False, 0, 1, "Freejia: Hotel West Room (in)"],
+            193: [192, 0, 0, 0, 0, "Map39Exit04", 0, False, 0, 1, "Freejia: Hotel West Room (out)"],
+            194: [195, 0, 0, 119, 121, "Map39Exit03", 0, False, 0, 1, "Freejia: Hotel East Room (in)"],
+            195: [194, 0, 0, 0, 0, "Map39Exit05", 0, False, 0, 1, "Freejia: Hotel East Room (out)"],
+            196: [197, 0, 0, 110, 122, "Map32Exit0A", 0, False, 0, 1, "Freejia: Laborer House (in)"],
+            197: [196, 0, 0, 0, 0, "Map3AExit02", 0, False, 0, 1, "Freejia: Laborer House (out)"],
+            198: [199, 0, 0, 112, 122, "Map32Exit0B", 0, False, 0, 1, "Freejia: Laborer Roof (in)"],
+            199: [198, 0, 0, 0, 0, "Map3AExit01", 0, False, 0, 1, "Freejia: Laborer Roof (out)"],
+            200: [201, 0, 0, 110, 123, "Map32Exit0C", 0, False, 0, 1, "Freejia: Messy House (in)"],
+            201: [200, 0, 0, 0, 0, "Map3BExit01", 0, False, 0, 1, "Freejia: Messy House (out)"],
+            202: [203, 0, 0, 110, 124, "Map32Exit01", 0, False, 0, 1, "Freejia: Erik House (in)"],
+            203: [202, 0, 0, 0, 0, "Map33Exit01", 0, False, 0, 1, "Freejia: Erik House (out)"],
+            204: [205, 0, 0, 110, 125, "Map32Exit02", 0, False, 0, 1, "Freejia: Dark Space House (in)"],
+            205: [204, 0, 0, 0, 0, "Map34Exit01", 0, False, 0, 1, "Freejia: Dark Space House (out)"],
+            206: [207, 0, 0, 110, 126, "Map32Exit03", 0, False, 0, 1, "Freejia: Labor Trade House (in)"],
+            207: [206, 0, 0, 0, 0, "Map35Exit01", 0, False, 0, 1, "Freejia: Labor Trade House (out)"],
+            208: [209, 0, 0, 113, 126, "Map32Exit04", 0, False, 0, 1, "Freejia: Labor Trade Roof (in)"],
+            209: [208, 0, 0, 0, 0, "Map35Exit02", 0, False, 0, 1, "Freejia: Labor Trade Roof (out)"],
+            210: [211, 0, 0, 114, 127, "Map32Exit0D", 0, False, 0, 1, "Freejia: Labor Market (in)"],
+            211: [210, 0, 0, 0, 0, "Map3CExit01", 0, False, 0, 1, "Freejia: Labor Market (out)"],
+
             # Diamond Mine
-            222: [223, 0, 0, 133, 134, "Map3EExit01", 0, False,  3, 3, "Mine: Entrance N exit (62->63)" ],
-            223: [222, 0, 0,   0,   0, "Map3FExit01", 0, False,  3, 2, "Mine: BigRoom SW exit (63->62)" ],
-            224: [225, 0, 0, 134, 140, "Map3FExit03", 0, False,  3, 2, "Mine: BigRoom elevator exit (63->66)" ],
-            225: [224, 0, 0,   0,   0, "Map42Exit01", 0, False,  3, 2, "Mine: East Elevator, N exit toward BigRoom (66->63)" ],
-            226: [227, 0, 0, 134, 136, "Map3FExit02", 0, False,  3, 2, "Mine: BigRoom Center exit (63->64)" ],
-            227: [226, 0, 0,   0,   0, "Map40Exit01", 0, False,  3, 2, "Mine: Cave-In Room N exit (64->63)" ],
-            228: [229, 0, 0, 136, 138, "Map40Exit02", 0, False,  3, 2, "Mine: Cave-In Room S exit (64->65)" ],
-            229: [228, 0, 0,   0,   0, "Map41Exit01", 0, False,  3, 2, "Mine: Friar Room SE exit (65->64)" ],
-            230: [231, 0, 0, 139, 143, "Map41Exit02", 0, False,  3, 2, "Mine: Friar Room upper NE exit (65->66)" ],
-            231: [230, 0, 0,   0,   0, "Map42Exit06", 0, False,  3, 2, "Mine: Single dead-end slave exit (66->65)" ],
-            232: [233, 0, 0, 138, 130, "Map41Exit03", 0, False,  3, 2, "Mine: Friar Room lower NE exit (65->61)" ],
-            233: [232, 0, 0,   0,   0, "Map3DExit01", 0, False,  3, 2, "Mine: Fence Tunnel S exit (61->65)" ],
-            234: [235, 0, 0, 131, 142, "Map3DExit02", 0, False,  3, 2, "Mine: Fence Tunnel N blocked exit (61->66)" ],
-            235: [234, 0, 0,   0,   0, "Map42Exit05", 0, False,  3, 2, "Mine: Dead-end Dark Space exit (66->61)" ],
-            236: [237, 0, 0, 140, 144, "Map42Exit02", 0, False,  3, 2, "Mine: East Elevator, S exit toward chairlift (66->67) (1)" ],
-            237: [236, 0, 0,   0,   0, "Map43Exit01", 0, False,  3, 2, "Mine: Chairlift E exit (67->66) (1)" ],
-            238: [239, 0, 0, 145, 141, "Map43Exit02", 0, False,  3, 2, "Mine: Chairlift W exit (67->66) (2)" ],
-            239: [238, 0, 0,   0,   0, "Map42Exit03", 0, False,  3, 2, "Mine: West Elevator, E exit toward chairlift (66->67) (2)" ],
-            240: [241, 0, 0, 141, 146, "Map42Exit04", 0, False,  3, 2, "Mine: West Elevator, S exit (66->68)" ],
-            241: [240, 0, 0,   0,   0, "Map44Exit01", 0, False,  3, 2, "Mine: End branch N exit (68->66)" ],
-            242: [243, 0, 0, 146, 148, "Map44Exit02", 0, False,  3, 2, "Mine: End branch W exit (68->69)" ],
-            243: [242, 0, 0,   0,   0, "Map45Exit01", 0, False,  3, 2, "Mine: Morgue exit (69->68)" ],
-            244: [245, 0, 0, 146, 149, "Map44Exit04", 0, False,  3, 2, "Mine: End branch E exit (68->70)" ],
-            245: [244, 0, 0,   0,   0, "Map46Exit01", 0, False,  3, 2, "Mine: Final combat room exit (70->68)" ],
-            246: [247, 0, 0, 146, 150, "Map44Exit03", 0, False,  3, 2, "Mine: End branch C exit behind gate (68->71)" ],
-            247: [246, 0, 0,   0,   0, "Map47Exit01", 0, False,  3, 2, "Mine: Sam's room exit (71->68)" ],
-            
+            222: [223, 0, 0, 133, 134, "Map3EExit01", 0, False, 3, 3, "Mine: Entrance N exit (62->63)"],
+            223: [222, 0, 0, 0, 0, "Map3FExit01", 0, False, 3, 2, "Mine: BigRoom SW exit (63->62)"],
+            224: [225, 0, 0, 134, 140, "Map3FExit03", 0, False, 3, 2, "Mine: BigRoom elevator exit (63->66)"],
+            225: [224, 0, 0, 0, 0, "Map42Exit01", 0, False, 3, 2,
+                  "Mine: East Elevator, N exit toward BigRoom (66->63)"],
+            226: [227, 0, 0, 134, 136, "Map3FExit02", 0, False, 3, 2, "Mine: BigRoom Center exit (63->64)"],
+            227: [226, 0, 0, 0, 0, "Map40Exit01", 0, False, 3, 2, "Mine: Cave-In Room N exit (64->63)"],
+            228: [229, 0, 0, 136, 138, "Map40Exit02", 0, False, 3, 2, "Mine: Cave-In Room S exit (64->65)"],
+            229: [228, 0, 0, 0, 0, "Map41Exit01", 0, False, 3, 2, "Mine: Friar Room SE exit (65->64)"],
+            230: [231, 0, 0, 139, 143, "Map41Exit02", 0, False, 3, 2, "Mine: Friar Room upper NE exit (65->66)"],
+            231: [230, 0, 0, 0, 0, "Map42Exit06", 0, False, 3, 2, "Mine: Single dead-end slave exit (66->65)"],
+            232: [233, 0, 0, 138, 130, "Map41Exit03", 0, False, 3, 2, "Mine: Friar Room lower NE exit (65->61)"],
+            233: [232, 0, 0, 0, 0, "Map3DExit01", 0, False, 3, 2, "Mine: Fence Tunnel S exit (61->65)"],
+            234: [235, 0, 0, 131, 142, "Map3DExit02", 0, False, 3, 2, "Mine: Fence Tunnel N blocked exit (61->66)"],
+            235: [234, 0, 0, 0, 0, "Map42Exit05", 0, False, 3, 2, "Mine: Dead-end Dark Space exit (66->61)"],
+            236: [237, 0, 0, 140, 144, "Map42Exit02", 0, False, 3, 2,
+                  "Mine: East Elevator, S exit toward chairlift (66->67) (1)"],
+            237: [236, 0, 0, 0, 0, "Map43Exit01", 0, False, 3, 2, "Mine: Chairlift E exit (67->66) (1)"],
+            238: [239, 0, 0, 145, 141, "Map43Exit02", 0, False, 3, 2, "Mine: Chairlift W exit (67->66) (2)"],
+            239: [238, 0, 0, 0, 0, "Map42Exit03", 0, False, 3, 2,
+                  "Mine: West Elevator, E exit toward chairlift (66->67) (2)"],
+            240: [241, 0, 0, 141, 146, "Map42Exit04", 0, False, 3, 2, "Mine: West Elevator, S exit (66->68)"],
+            241: [240, 0, 0, 0, 0, "Map44Exit01", 0, False, 3, 2, "Mine: End branch N exit (68->66)"],
+            242: [243, 0, 0, 146, 148, "Map44Exit02", 0, False, 3, 2, "Mine: End branch W exit (68->69)"],
+            243: [242, 0, 0, 0, 0, "Map45Exit01", 0, False, 3, 2, "Mine: Morgue exit (69->68)"],
+            244: [245, 0, 0, 146, 149, "Map44Exit04", 0, False, 3, 2, "Mine: End branch E exit (68->70)"],
+            245: [244, 0, 0, 0, 0, "Map46Exit01", 0, False, 3, 2, "Mine: Final combat room exit (70->68)"],
+            246: [247, 0, 0, 146, 150, "Map44Exit03", 0, False, 3, 2, "Mine: End branch C exit behind gate (68->71)"],
+            247: [246, 0, 0, 0, 0, "Map47Exit01", 0, False, 3, 2, "Mine: Sam's room exit (71->68)"],
+
             # Nazca
-            260: [261, 0, 0, 162, 170, "MapGardenEntranceString", 0, False, 4, 1, "Nazca: Sky Garden entrance" ],
-            261: [260, 0, 0,   0,   0, "MapGardenExitString", 0, False, 4, 1, "Nazca: Sky Garden exit" ],
-            
+            260: [261, 0, 0, 162, 170, "MapGardenEntranceString", 0, False, 4, 1, "Nazca: Sky Garden entrance"],
+            261: [260, 0, 0, 0, 0, "MapGardenExitString", 0, False, 4, 1, "Nazca: Sky Garden exit"],
+
             # Sky Garden
-            #270: [  0, 0, 0, 171,  16, "", 0, False,  4,  True, "Moon Tribe: Sky Garden passage" ],
-            273: [274, 0, 0, 170, 172, "Map4CExit02", 0, False,  4, 2, "Sky Garden: Foyer NE exit (76->77)" ],
-            274: [273, 0, 0,   0,   0, "Map4DExit01", 0, False,  4, 2, "Sky Garden: NE Top room, NW exit (77->76)" ],
-            275: [276, 0, 0, 170, 176, "Map4CExit03", 0, False,  4, 2, "Sky Garden: Foyer SE exit (76->79)" ],
-            276: [275, 0, 0,   0,   0, "Map4FExit01", 0, False,  4, 2, "Sky Garden: SE Top room, NW exit (79->76)" ],
-            277: [278, 0, 0, 170, 181, "Map4CExit05", 0, False,  4, 2, "Sky Garden: Foyer SW exit (76->81)" ],
-            278: [277, 0, 0,   0,   0, "Map51Exit01", 0, False,  4, 2, "Sky Garden: SW Top room, NE exit (81->76)" ],
-            279: [280, 0, 0, 170, 190, "Map4CExit04", 0, False,  4, 2, "Sky Garden: Foyer NW exit (76->83)" ],
-            280: [279, 0, 0,   0,   0, "Map53Exit01", 0, False,  4, 2, "Sky Garden: NW Top room, NE exit (83->76)" ],
-            281: [282, 0, 0, 172, 175, "Map4DExit02", 0, False,  4, 2, "Sky Garden: NE Top room, E exit (77->78)" ],
-            282: [281, 0, 0,   0,   0, "Map4EExit01", 0, False,  4, 2, "Sky Garden: NE Bot room, W exit (78->77)" ],
-            283: [284, 0, 0, 175, 173, "Map4EExit03", 0, False,  4, 2, "Sky Garden: NE Bot room, SE exit (78->77)" ],
-            284: [283, 0, 0,   0,   0, "Map4DExit04", 0, False,  4, 2, "Sky Garden: NE Top room, SW exit (77->78)" ],
-            285: [286, 0, 0, 175, 174, "Map4EExit02", 0, False,  4, 2, "Sky Garden: NE Bot room, SW exit (78->77)" ],
-            286: [285, 0, 0,   0,   0, "Map4DExit03", 0, False,  4, 2, "Sky Garden: NE Top room, SE exit (77->78)" ],
-            287: [288, 0, 0, 176, 169, "Map4FExit05", 0, False,  4, 2, "Sky Garden: SE Top room, statue door (79->86)" ],
-            288: [287, 0, 0,   0,   0, "Map56Exit01", 0, False,  4, 2, "Sky Garden: Dead-end Dark Space room exit (86->79)" ],
-            289: [290, 0, 0, 176, 179, "Map4FExit02", 0, False,  4, 2, "Sky Garden: SE Top room, NE exit (79->80)" ],
-            290: [289, 0, 0,   0,   0, "Map50Exit01", 0, False,  4, 2, "Sky Garden: SE Bottom corridor, W exit (80->79)" ],
-            291: [292, 0, 0, 179, 177, "Map50Exit02", 0, False,  4, 2, "Sky Garden: SE Bottom corridor, E exit (80->79)" ],
-            292: [291, 0, 0,   0,   0, "Map4FExit03", 0, False,  4, 2, "Sky Garden: SE Top room, exit before Friar barrier (79->80)" ],
-            293: [294, 0, 0, 178, 180, "Map4FExit04", 0, False,  4, 2, "Sky Garden: SE Top room, exit after Friar barrier (79->80)" ],
-            294: [293, 0, 0,   0,   0, "Map50Exit03", 0, False,  4, 2, "Sky Garden: SE Bottom chest area exit (80->79)" ],
-            295: [296, 0, 0, 168, 186, "Map51Exit02", 0, False,  4, 2, "Sky Garden: SW Top, N exit behind pegs (81->82)" ],
-            296: [295, 0, 0,   0,   0, "Map52Exit01", 0, False,  4, 2, "Sky Garden: SW Bot, N exit near chest (82->81)" ],
-            297: [298, 0, 0, 182, 188, "Map51Exit03", 0, False,  4, 2, "Sky Garden: SW Top, NW exit near Dark Space cage (81->82)" ],
-            298: [297, 0, 0,   0,   0, "Map52Exit02", 0, False,  4, 2, "Sky Garden: SW Bot, NE exit near cage switch (82->81)" ],
-            299: [300, 0, 0, 184, 187, "Map51Exit04", 0, False,  4, 2, "Sky Garden: SW Top, SE exit with ramp (81->82)" ],
-            300: [299, 0, 0,   0,   0, "Map52Exit03", 0, False,  4, 2, "Sky Garden: SW Bot, SW exit near fire cages (82->81)" ],
-            301: [302, 0, 0, 191, 196, "Map53Exit05", 0, False,  4, 2, "Sky Garden: NW Top, useless NW exit (83->84)" ],
-            302: [301, 0, 0,   0,   0, "Map54Exit04", 0, False,  4, 2, "Sky Garden: NW Bot, NE exit after one-way ledge (84->83)" ],
-            303: [304, 0, 0, 192, 195, "Map53Exit02", 0, False,  4, 2, "Sky Garden: NW Top, Center exit (83->84)" ],
-            304: [303, 0, 0,   0,   0, "Map54Exit01", 0, False,  4, 2, "Sky Garden: NW Bot, Center exit (84->83)" ],
-            305: [306, 0, 0, 197, 193, "Map54Exit02", 0, False,  4, 2, "Sky Garden: NW Bot, SE exit behind statue (84->83)" ],
-            306: [305, 0, 0,   0,   0, "Map53Exit03", 0, False,  4, 2, "Sky Garden: NW Top, SW exit before chests (83->84)" ],
-            307: [308, 0, 0, 167, 195, "Map53Exit04", 0, False,  4, 2, "Sky Garden: NW Top, E exit after chests (83->84)" ],
-            308: [307, 0, 0,   0,   0, "Map54Exit03", 0, False,  4, 2, "Sky Garden: NW Bot, useless W exit (84->83)" ],
-            
+            # 270: [  0, 0, 0, 171,  16, "", 0, False,  4,  True, "Moon Tribe: Sky Garden passage" ],
+            273: [274, 0, 0, 170, 172, "Map4CExit02", 0, False, 4, 2, "Sky Garden: Foyer NE exit (76->77)"],
+            274: [273, 0, 0, 0, 0, "Map4DExit01", 0, False, 4, 2, "Sky Garden: NE Top room, NW exit (77->76)"],
+            275: [276, 0, 0, 170, 176, "Map4CExit03", 0, False, 4, 2, "Sky Garden: Foyer SE exit (76->79)"],
+            276: [275, 0, 0, 0, 0, "Map4FExit01", 0, False, 4, 2, "Sky Garden: SE Top room, NW exit (79->76)"],
+            277: [278, 0, 0, 170, 181, "Map4CExit05", 0, False, 4, 2, "Sky Garden: Foyer SW exit (76->81)"],
+            278: [277, 0, 0, 0, 0, "Map51Exit01", 0, False, 4, 2, "Sky Garden: SW Top room, NE exit (81->76)"],
+            279: [280, 0, 0, 170, 190, "Map4CExit04", 0, False, 4, 2, "Sky Garden: Foyer NW exit (76->83)"],
+            280: [279, 0, 0, 0, 0, "Map53Exit01", 0, False, 4, 2, "Sky Garden: NW Top room, NE exit (83->76)"],
+            281: [282, 0, 0, 172, 175, "Map4DExit02", 0, False, 4, 2, "Sky Garden: NE Top room, E exit (77->78)"],
+            282: [281, 0, 0, 0, 0, "Map4EExit01", 0, False, 4, 2, "Sky Garden: NE Bot room, W exit (78->77)"],
+            283: [284, 0, 0, 175, 173, "Map4EExit03", 0, False, 4, 2, "Sky Garden: NE Bot room, SE exit (78->77)"],
+            284: [283, 0, 0, 0, 0, "Map4DExit04", 0, False, 4, 2, "Sky Garden: NE Top room, SW exit (77->78)"],
+            285: [286, 0, 0, 175, 174, "Map4EExit02", 0, False, 4, 2, "Sky Garden: NE Bot room, SW exit (78->77)"],
+            286: [285, 0, 0, 0, 0, "Map4DExit03", 0, False, 4, 2, "Sky Garden: NE Top room, SE exit (77->78)"],
+            287: [288, 0, 0, 176, 169, "Map4FExit05", 0, False, 4, 2, "Sky Garden: SE Top room, statue door (79->86)"],
+            288: [287, 0, 0, 0, 0, "Map56Exit01", 0, False, 4, 2, "Sky Garden: Dead-end Dark Space room exit (86->79)"],
+            289: [290, 0, 0, 176, 179, "Map4FExit02", 0, False, 4, 2, "Sky Garden: SE Top room, NE exit (79->80)"],
+            290: [289, 0, 0, 0, 0, "Map50Exit01", 0, False, 4, 2, "Sky Garden: SE Bottom corridor, W exit (80->79)"],
+            291: [292, 0, 0, 179, 177, "Map50Exit02", 0, False, 4, 2,
+                  "Sky Garden: SE Bottom corridor, E exit (80->79)"],
+            292: [291, 0, 0, 0, 0, "Map4FExit03", 0, False, 4, 2,
+                  "Sky Garden: SE Top room, exit before Friar barrier (79->80)"],
+            293: [294, 0, 0, 178, 180, "Map4FExit04", 0, False, 4, 2,
+                  "Sky Garden: SE Top room, exit after Friar barrier (79->80)"],
+            294: [293, 0, 0, 0, 0, "Map50Exit03", 0, False, 4, 2, "Sky Garden: SE Bottom chest area exit (80->79)"],
+            295: [296, 0, 0, 168, 186, "Map51Exit02", 0, False, 4, 2,
+                  "Sky Garden: SW Top, N exit behind pegs (81->82)"],
+            296: [295, 0, 0, 0, 0, "Map52Exit01", 0, False, 4, 2, "Sky Garden: SW Bot, N exit near chest (82->81)"],
+            297: [298, 0, 0, 182, 188, "Map51Exit03", 0, False, 4, 2,
+                  "Sky Garden: SW Top, NW exit near Dark Space cage (81->82)"],
+            298: [297, 0, 0, 0, 0, "Map52Exit02", 0, False, 4, 2,
+                  "Sky Garden: SW Bot, NE exit near cage switch (82->81)"],
+            299: [300, 0, 0, 184, 187, "Map51Exit04", 0, False, 4, 2, "Sky Garden: SW Top, SE exit with ramp (81->82)"],
+            300: [299, 0, 0, 0, 0, "Map52Exit03", 0, False, 4, 2,
+                  "Sky Garden: SW Bot, SW exit near fire cages (82->81)"],
+            301: [302, 0, 0, 191, 196, "Map53Exit05", 0, False, 4, 2, "Sky Garden: NW Top, useless NW exit (83->84)"],
+            302: [301, 0, 0, 0, 0, "Map54Exit04", 0, False, 4, 2,
+                  "Sky Garden: NW Bot, NE exit after one-way ledge (84->83)"],
+            303: [304, 0, 0, 192, 195, "Map53Exit02", 0, False, 4, 2, "Sky Garden: NW Top, Center exit (83->84)"],
+            304: [303, 0, 0, 0, 0, "Map54Exit01", 0, False, 4, 2, "Sky Garden: NW Bot, Center exit (84->83)"],
+            305: [306, 0, 0, 197, 193, "Map54Exit02", 0, False, 4, 2,
+                  "Sky Garden: NW Bot, SE exit behind statue (84->83)"],
+            306: [305, 0, 0, 0, 0, "Map53Exit03", 0, False, 4, 2, "Sky Garden: NW Top, SW exit before chests (83->84)"],
+            307: [308, 0, 0, 167, 195, "Map53Exit04", 0, False, 4, 2,
+                  "Sky Garden: NW Top, E exit after chests (83->84)"],
+            308: [307, 0, 0, 0, 0, "Map54Exit03", 0, False, 4, 2, "Sky Garden: NW Bot, useless W exit (84->83)"],
+
             # Seaside Palace
-            310: [311, 0, 0, 210, 200, "Map5EExit03", 0, False, 0, 0, "Seaside entrance" ],  # always linked
-            311: [310, 0, 0,   0,   0, "Map5AExit05", 0, False, 0, 0, "Seaside exit" ],      # always linked
-            312: [313, 0, 0, 200, 202, "Map5AExit02", 0, False, 0, 1, "Seaside: Area 1 NE Room (in)" ],
-            313: [312, 0, 0,   0,   0, "Map5BExit01", 0, False, 0, 1, "Seaside: Area 1 NE Room (out)" ],
-            314: [315, 0, 0, 200, 203, "Map5AExit03", 0, False, 0, 1, "Seaside: Area 1 NW Room (in)" ],
-            315: [314, 0, 0,   0,   0, "Map5BExit02", 0, False, 0, 1, "Seaside: Area 1 NW Room (out)" ],
-            316: [317, 0, 0, 200, 204, "Map5AExit04", 0, False, 0, 1, "Seaside: Area 1 SE Room (in)" ],
-            317: [316, 0, 0,   0,   0, "Map5BExit03", 0, False, 0, 1, "Seaside: Area 1 SE Room (out)" ],
-            318: [319, 0, 0, 200, 205, "Map5AExit01", 0, False, 0, 1, "Seaside: Area 2 entrance" ],
-            319: [318, 0, 0,   0,   0, "Map5CExit01", 0, False, 0, 1, "Seaside: Area 2 exit" ],
-            320: [321, 0, 0, 205, 207, "Map5CExit03", 0, False, 0, 1, "Seaside: Area 2 SW Room (in)" ],
-            321: [320, 0, 0,   0,   0, "Map5BExit04", 0, False, 0, 1, "Seaside: Area 2 SW Room (out)" ],
-            322: [323, 0, 0, 205, 209, "Map5CExit02", 0, False, 0, 1, "Seaside: Fountain (in)" ],
-            323: [322, 0, 0,   0,   0, "Map5DExit01", 0, False, 0, 1, "Seaside: Fountain (out)" ],
-            
+            310: [311, 0, 0, 210, 200, "Map5EExit03", 0, False, 0, 0, "Seaside entrance"],  # always linked
+            311: [310, 0, 0, 0, 0, "Map5AExit05", 0, False, 0, 0, "Seaside exit"],  # always linked
+            312: [313, 0, 0, 200, 202, "Map5AExit02", 0, False, 0, 1, "Seaside: Area 1 NE Room (in)"],
+            313: [312, 0, 0, 0, 0, "Map5BExit01", 0, False, 0, 1, "Seaside: Area 1 NE Room (out)"],
+            314: [315, 0, 0, 200, 203, "Map5AExit03", 0, False, 0, 1, "Seaside: Area 1 NW Room (in)"],
+            315: [314, 0, 0, 0, 0, "Map5BExit02", 0, False, 0, 1, "Seaside: Area 1 NW Room (out)"],
+            316: [317, 0, 0, 200, 204, "Map5AExit04", 0, False, 0, 1, "Seaside: Area 1 SE Room (in)"],
+            317: [316, 0, 0, 0, 0, "Map5BExit03", 0, False, 0, 1, "Seaside: Area 1 SE Room (out)"],
+            318: [319, 0, 0, 200, 205, "Map5AExit01", 0, False, 0, 1, "Seaside: Area 2 entrance"],
+            319: [318, 0, 0, 0, 0, "Map5CExit01", 0, False, 0, 1, "Seaside: Area 2 exit"],
+            320: [321, 0, 0, 205, 207, "Map5CExit03", 0, False, 0, 1, "Seaside: Area 2 SW Room (in)"],
+            321: [320, 0, 0, 0, 0, "Map5BExit04", 0, False, 0, 1, "Seaside: Area 2 SW Room (out)"],
+            322: [323, 0, 0, 205, 209, "Map5CExit02", 0, False, 0, 1, "Seaside: Fountain (in)"],
+            323: [322, 0, 0, 0, 0, "Map5DExit01", 0, False, 0, 1, "Seaside: Fountain (out)"],
+
             # Mu
-            330: [331, 0, 0, 210, 212, "Map5EExit02", 0, False,  5, 1, "Mu entrance" ],
-            331: [330, 0, 0,   0,   0, "Map5FExit01", 0, False,  5, 1, "Mu exit toward Palace corridor" ], # NW to Palace corridor
-            332: [333, 0, 0, 722, 217, "Map5FExit02", 0, False,  5, 2, "Mu: NW room, NE exit (95->96)" ],
-            333: [332, 0, 0,   0,   0, "Map60Exit01", 0, False,  5, 2, "Mu: NE room, NW exit (96->95)" ],
-            334: [335, 0, 0, 723, 220, "Map60Exit02", 0, False,  5, 2, "Mu: NE room, upper SE exit (96->97)" ],
-            335: [334, 0, 0,   0,   0, "Map61Exit01", 0, False,  5, 2, "Mu: E room, upper N exit (97->96)" ],
-            336: [337, 0, 0, 220, 231, "Map61Exit07", 0, False,  5, 2, "Mu: E room door to Hope Room (97->99)" ], # E to Hope Room 1
-            337: [336, 0, 0,   0,   0, "Map63Exit01", 0, False,  5, 2, "Mu: Hope Room 1 exit out (99->97)" ],
-            338: [339, 0, 0, 220, 225, "Map61Exit04", 0, False,  5, 2, "Mu: E room, upper SW exit (97->98)" ],
-            339: [338, 0, 0,   0,   0, "Map62Exit02", 0, False,  5, 2, "Mu: W room, SE exit from Hope Statue dead-end (98->97)" ],
-            340: [341, 0, 0, 218, 222, "Map60Exit03", 0, False,  5, 2, "Mu: NE room, mid-water SE exit (96->97)" ],
-            341: [340, 0, 0,   0,   0, "Map61Exit02", 0, False,  5, 2, "Mu: E room, mid-water N exit (97->96)" ], # E-Mid to NE-Mid
-            342: [343, 0, 0, 223, 227, "Map61Exit05", 0, False,  5, 2, "Mu: E room, mid-water W exit (97->98)" ],
-            343: [342, 0, 0,   0,   0, "Map62Exit03", 0, False,  5, 2, "Mu: W room, mid-water E exit (98->97)" ],
-            346: [347, 0, 0, 227, 233, "Map62Exit06", 0, False,  5, 2, "Mu: W room, eastern mid-water S exit (98->100)" ],
-            347: [346, 0, 0,   0,   0, "Map64Exit01", 0, False,  5, 2, "Mu: SW room, east side, N exit (100->98)" ],
-            348: [349, 0, 0, 245, 237, "Map64Exit04", 0, False,  5, 2, "Mu: SW room, east side, SE exit (100->101)" ],
-            349: [348, 0, 0,   0,   0, "Map65Exit01", 0, False,  5, 2, "Mu: SE room, northern mid-water exit (101->100)" ],
-            350: [351, 0, 0, 237, 234, "Map65Exit03", 0, False,  5, 2, "Mu: SE room, southern mid-water exit (101->100)" ],
-            351: [350, 0, 0,   0,   0, "Map64Exit06", 0, False,  5, 2, "Mu: SW room, lower SE exit (100->101)" ],
-            352: [353, 0, 0, 234, 228, "Map64Exit03", 0, False,  5, 2, "Mu: SW room, south/west corridor, NW exit (100->98)" ],
-            353: [352, 0, 0,   0,   0, "Map62Exit08", 0, False,  5, 2, "Mu: W room, western mid-water S exit (98->100)" ],
-            354: [355, 0, 0, 213, 232, "Map5FExit05", 0, False,  5, 2, "Mu: NW room door to Hope Room (95->99)" ], # NW to Hope Room 2
-            355: [354, 0, 0,   0,   0, "Map63Exit02", 0, False,  5, 2, "Mu: Hope Room 2 exit out (99->95)" ],
-            356: [357, 0, 0, 722, 226, "",            0, False,  5, 0, "Mu: NW room Slider hole (95->98)" ], # Slider, always linked
-            357: [356, 0, 0,   0,   0, "",            0, False,  5, 0, "Mu: W room Slider hole (98->95)" ], # Slider, always linked
-            358: [359, 0, 0, 229, 224, "Map62Exit04", 0, False,  5, 2, "Mu: W room, lower E exit (98->97)" ],
-            359: [358, 0, 0,   0,   0, "Map61Exit06", 0, False,  5, 2, "Mu: E room, lower corridor W exit (97->98)" ],
-            360: [361, 0, 0, 224, 219, "Map61Exit03", 0, False,  5, 2, "Mu: E room, lower corridor N exit (97->96)" ],
-            361: [360, 0, 0,   0,   0, "Map60Exit04", 0, False,  5, 2, "Mu: NE room, lower S exit (96->97)" ],
-            362: [363, 0, 0, 230, 216, "Map62Exit01", 0, False,  5, 2, "Mu: W room, lower N exit (98->95)" ],
-            363: [362, 0, 0,   0,   0, "Map5FExit03", 0, False,  5, 2, "Mu: NW room, lower S exit (95->98)" ],
-            364: [365, 0, 0, 230, 235, "Map62Exit07", 0, False,  5, 2, "Mu: W room, lower S exit (98->100)" ],
-            365: [364, 0, 0,   0,   0, "Map64Exit02", 0, False,  5, 2, "Mu: SW room, lower corridor N exit (100->98)" ],
-            366: [367, 0, 0, 235, 239, "Map64Exit05", 0, False,  5, 2, "Mu: SW room, lower corridor SE exit (100->101)" ],
-            367: [366, 0, 0,   0,   0, "Map65Exit02", 0, False,  5, 2, "Mu: SE room, lower W exit (101->100)" ],
-            368: [369, 0, 0, 239, 240, "Map65Exit04", 0, False,  5, 0, "Mu: SE room, boss door (101->102)" ], # Not randomized; Mu boss always requires Hope+Rama Statues
-            369: [368, 0, 0,   0,   0, "Map66Exit02", 0, False,  5, 0, "Mu: Rama Statue room exit out (102->101)" ],
-            
+            330: [331, 0, 0, 210, 212, "Map5EExit02", 0, False, 5, 1, "Mu entrance"],
+            331: [330, 0, 0, 0, 0, "Map5FExit01", 0, False, 5, 1, "Mu exit toward Palace corridor"],
+            # NW to Palace corridor
+            332: [333, 0, 0, 722, 217, "Map5FExit02", 0, False, 5, 2, "Mu: NW room, NE exit (95->96)"],
+            333: [332, 0, 0, 0, 0, "Map60Exit01", 0, False, 5, 2, "Mu: NE room, NW exit (96->95)"],
+            334: [335, 0, 0, 723, 220, "Map60Exit02", 0, False, 5, 2, "Mu: NE room, upper SE exit (96->97)"],
+            335: [334, 0, 0, 0, 0, "Map61Exit01", 0, False, 5, 2, "Mu: E room, upper N exit (97->96)"],
+            336: [337, 0, 0, 220, 231, "Map61Exit07", 0, False, 5, 2, "Mu: E room door to Hope Room (97->99)"],
+            # E to Hope Room 1
+            337: [336, 0, 0, 0, 0, "Map63Exit01", 0, False, 5, 2, "Mu: Hope Room 1 exit out (99->97)"],
+            338: [339, 0, 0, 220, 225, "Map61Exit04", 0, False, 5, 2, "Mu: E room, upper SW exit (97->98)"],
+            339: [338, 0, 0, 0, 0, "Map62Exit02", 0, False, 5, 2,
+                  "Mu: W room, SE exit from Hope Statue dead-end (98->97)"],
+            340: [341, 0, 0, 218, 222, "Map60Exit03", 0, False, 5, 2, "Mu: NE room, mid-water SE exit (96->97)"],
+            341: [340, 0, 0, 0, 0, "Map61Exit02", 0, False, 5, 2, "Mu: E room, mid-water N exit (97->96)"],
+            # E-Mid to NE-Mid
+            342: [343, 0, 0, 223, 227, "Map61Exit05", 0, False, 5, 2, "Mu: E room, mid-water W exit (97->98)"],
+            343: [342, 0, 0, 0, 0, "Map62Exit03", 0, False, 5, 2, "Mu: W room, mid-water E exit (98->97)"],
+            346: [347, 0, 0, 227, 233, "Map62Exit06", 0, False, 5, 2, "Mu: W room, eastern mid-water S exit (98->100)"],
+            347: [346, 0, 0, 0, 0, "Map64Exit01", 0, False, 5, 2, "Mu: SW room, east side, N exit (100->98)"],
+            348: [349, 0, 0, 245, 237, "Map64Exit04", 0, False, 5, 2, "Mu: SW room, east side, SE exit (100->101)"],
+            349: [348, 0, 0, 0, 0, "Map65Exit01", 0, False, 5, 2, "Mu: SE room, northern mid-water exit (101->100)"],
+            350: [351, 0, 0, 237, 234, "Map65Exit03", 0, False, 5, 2,
+                  "Mu: SE room, southern mid-water exit (101->100)"],
+            351: [350, 0, 0, 0, 0, "Map64Exit06", 0, False, 5, 2, "Mu: SW room, lower SE exit (100->101)"],
+            352: [353, 0, 0, 234, 228, "Map64Exit03", 0, False, 5, 2,
+                  "Mu: SW room, south/west corridor, NW exit (100->98)"],
+            353: [352, 0, 0, 0, 0, "Map62Exit08", 0, False, 5, 2, "Mu: W room, western mid-water S exit (98->100)"],
+            354: [355, 0, 0, 213, 232, "Map5FExit05", 0, False, 5, 2, "Mu: NW room door to Hope Room (95->99)"],
+            # NW to Hope Room 2
+            355: [354, 0, 0, 0, 0, "Map63Exit02", 0, False, 5, 2, "Mu: Hope Room 2 exit out (99->95)"],
+            356: [357, 0, 0, 722, 226, "", 0, False, 5, 0, "Mu: NW room Slider hole (95->98)"],  # Slider, always linked
+            357: [356, 0, 0, 0, 0, "", 0, False, 5, 0, "Mu: W room Slider hole (98->95)"],  # Slider, always linked
+            358: [359, 0, 0, 229, 224, "Map62Exit04", 0, False, 5, 2, "Mu: W room, lower E exit (98->97)"],
+            359: [358, 0, 0, 0, 0, "Map61Exit06", 0, False, 5, 2, "Mu: E room, lower corridor W exit (97->98)"],
+            360: [361, 0, 0, 224, 219, "Map61Exit03", 0, False, 5, 2, "Mu: E room, lower corridor N exit (97->96)"],
+            361: [360, 0, 0, 0, 0, "Map60Exit04", 0, False, 5, 2, "Mu: NE room, lower S exit (96->97)"],
+            362: [363, 0, 0, 230, 216, "Map62Exit01", 0, False, 5, 2, "Mu: W room, lower N exit (98->95)"],
+            363: [362, 0, 0, 0, 0, "Map5FExit03", 0, False, 5, 2, "Mu: NW room, lower S exit (95->98)"],
+            364: [365, 0, 0, 230, 235, "Map62Exit07", 0, False, 5, 2, "Mu: W room, lower S exit (98->100)"],
+            365: [364, 0, 0, 0, 0, "Map64Exit02", 0, False, 5, 2, "Mu: SW room, lower corridor N exit (100->98)"],
+            366: [367, 0, 0, 235, 239, "Map64Exit05", 0, False, 5, 2, "Mu: SW room, lower corridor SE exit (100->101)"],
+            367: [366, 0, 0, 0, 0, "Map65Exit02", 0, False, 5, 2, "Mu: SE room, lower W exit (101->100)"],
+            368: [369, 0, 0, 239, 240, "Map65Exit04", 0, False, 5, 0, "Mu: SE room, boss door (101->102)"],
+            # Not randomized; Mu boss always requires Hope+Rama Statues
+            369: [368, 0, 0, 0, 0, "Map66Exit02", 0, False, 5, 0, "Mu: Rama Statue room exit out (102->101)"],
+
             # Angel Village
-            382: [383, 0, 0, 250, 210, "Map69Exit01", 0, False, 0, 1, "Angel: Mu Passage (in)" ],
-            383: [382, 0, 0,   0,   0, "Map5EExit01", 0, False, 0, 1, "Angel: Mu Passage (out)" ], #custom
-            384: [385, 0, 0, 250, 251, "Map69Exit02", 0, False, 0, 1, "Angel: Underground entrance (in)" ],
-            385: [384, 0, 0,   0,   0, "Map6BExit01", 0, False, 0, 1, "Angel: Underground entrance (out)" ],
-            386: [387, 0, 0, 251, 252, "Map6BExit02", 0, False, 0, 1, "Angel: Room 1 (in)" ],
-            387: [386, 0, 0,   0,   0, "Map6CExit01", 0, False, 0, 1, "Angel: Room 1 (out)" ],
-            388: [389, 0, 0, 251, 253, "Map6BExit05", 0, False, 0, 1, "Angel: Room 2 (in)" ],
-            389: [388, 0, 0,   0,   0, "Map6CExit04", 0, False, 0, 1, "Angel: Room 2 (out)" ],
-            390: [391, 0, 0, 251, 254, "Map6BExit03", 0, False, 0, 1, "Angel: Dance Hall (in)" ],
-            391: [390, 0, 0,   0,   0, "Map6CExit05", 0, False, 0, 1, "Angel: Dance Hall (out)" ],
-            392: [393, 0, 0, 251, 255, "Map6BExit04", 0, False, 0, 1, "Angel: DS Room (in)" ],
-            393: [392, 0, 0,   0,   0, "Map6CExit03", 0, False, 0, 1, "Angel: DS Room (out)" ],
-            
+            382: [383, 0, 0, 250, 210, "Map69Exit01", 0, False, 0, 1, "Angel: Mu Passage (in)"],
+            383: [382, 0, 0, 0, 0, "Map5EExit01", 0, False, 0, 1, "Angel: Mu Passage (out)"],  # custom
+            384: [385, 0, 0, 250, 251, "Map69Exit02", 0, False, 0, 1, "Angel: Underground entrance (in)"],
+            385: [384, 0, 0, 0, 0, "Map6BExit01", 0, False, 0, 1, "Angel: Underground entrance (out)"],
+            386: [387, 0, 0, 251, 252, "Map6BExit02", 0, False, 0, 1, "Angel: Room 1 (in)"],
+            387: [386, 0, 0, 0, 0, "Map6CExit01", 0, False, 0, 1, "Angel: Room 1 (out)"],
+            388: [389, 0, 0, 251, 253, "Map6BExit05", 0, False, 0, 1, "Angel: Room 2 (in)"],
+            389: [388, 0, 0, 0, 0, "Map6CExit04", 0, False, 0, 1, "Angel: Room 2 (out)"],
+            390: [391, 0, 0, 251, 254, "Map6BExit03", 0, False, 0, 1, "Angel: Dance Hall (in)"],
+            391: [390, 0, 0, 0, 0, "Map6CExit05", 0, False, 0, 1, "Angel: Dance Hall (out)"],
+            392: [393, 0, 0, 251, 255, "Map6BExit04", 0, False, 0, 1, "Angel: DS Room (in)"],
+            393: [392, 0, 0, 0, 0, "Map6CExit03", 0, False, 0, 1, "Angel: DS Room (out)"],
+
             # Angel Dungeon
-            398: [399, 0, 0, 259, 263, "Map70Exit04", 0, False, 6, 2, "Angel: Water room hidden door (112->112)" ],
-            399: [398, 0, 0,   0,   0, "Map70Exit05", 0, False, 6, 2, "Angel: Water room monster area SW door (112->112)" ],
-            400: [401, 0, 0, 251, 260, "Map6BExit06", 0, False, 6, 1, "Angel Dungeon entrance (in)" ],
-            401: [400, 0, 0,   0,   0, "Map6DExit02", 0, False, 6, 1, "Angel Dungeon exit (out)" ],
-            402: [403, 0, 0, 260, 261, "Map6DExit01", 0, False, 6, 3, "Angel: First room SE door (109->110)" ],
-            403: [402, 0, 0,   0,   0, "Map6EExit01", 0, False, 6, 2, "Angel: Maze room NW door (110->109)" ],
-            404: [405, 0, 0, 278, 262, "Map6EExit02", 0, False, 6, 2, "Angel: Maze room SE door (110->111)" ],
-            405: [404, 0, 0,   0,   0, "Map6FExit01", 0, False, 6, 2, "Angel: Dark room W door (111->110)" ],
-            406: [407, 0, 0, 262, 259, "Map6FExit02", 0, False, 6, 2, "Angel: Dark room E door (111->112)" ],
-            407: [406, 0, 0,   0,   0, "Map70Exit01", 0, False, 6, 2, "Angel: Water room area without monsters, W door (112->111)" ],
-            408: [409, 0, 0, 263, 265, "Map70Exit02", 0, False, 6, 2, "Angel: Water room Slider hole to chest (112->112)" ],  # Slider
-            409: [408, 0, 0,   0,   0, "Map70Exit03", 0, False, 6, 2, "Angel: Slider hole from chest toward water room (112->112)" ],  # Slider
-            410: [411, 0, 0, 279, 266, "Map70Exit06", 0, False, 6, 2, "Angel: Water room monster area E door (112->113)" ],
-            411: [410, 0, 0,   0,   0, "Map71Exit01", 0, False, 6, 2, "Angel: Wind Tunnel W door (113->112)" ],
-            412: [413, 0, 0, 266, 267, "Map71Exit02", 0, False, 6, 2, "Angel: Wind Tunnel E door (113->114)" ],
-            413: [412, 0, 0,   0,   0, "Map72Exit01", 0, False, 6, 2, "Angel: Long room W door (114->113)" ],
-            414: [415, 0, 0, 267, 277, "Map72Exit02", 0, False, 6, 2, "Angel: Long room Slider hole toward Ishtar (114->115)" ],  # Slider
-            415: [414, 0, 0,   0,   0, "Map73Exit01", 0, False, 6, 2, "Angel: Ishtar foyer Slider hole (115->114)" ],  # Slider
-            
+            398: [399, 0, 0, 259, 263, "Map70Exit04", 0, False, 6, 2, "Angel: Water room hidden door (112->112)"],
+            399: [398, 0, 0, 0, 0, "Map70Exit05", 0, False, 6, 2, "Angel: Water room monster area SW door (112->112)"],
+            400: [401, 0, 0, 251, 260, "Map6BExit06", 0, False, 6, 1, "Angel Dungeon entrance (in)"],
+            401: [400, 0, 0, 0, 0, "Map6DExit02", 0, False, 6, 1, "Angel Dungeon exit (out)"],
+            402: [403, 0, 0, 260, 261, "Map6DExit01", 0, False, 6, 3, "Angel: First room SE door (109->110)"],
+            403: [402, 0, 0, 0, 0, "Map6EExit01", 0, False, 6, 2, "Angel: Maze room NW door (110->109)"],
+            404: [405, 0, 0, 278, 262, "Map6EExit02", 0, False, 6, 2, "Angel: Maze room SE door (110->111)"],
+            405: [404, 0, 0, 0, 0, "Map6FExit01", 0, False, 6, 2, "Angel: Dark room W door (111->110)"],
+            406: [407, 0, 0, 262, 259, "Map6FExit02", 0, False, 6, 2, "Angel: Dark room E door (111->112)"],
+            407: [406, 0, 0, 0, 0, "Map70Exit01", 0, False, 6, 2,
+                  "Angel: Water room area without monsters, W door (112->111)"],
+            408: [409, 0, 0, 263, 265, "Map70Exit02", 0, False, 6, 2,
+                  "Angel: Water room Slider hole to chest (112->112)"],  # Slider
+            409: [408, 0, 0, 0, 0, "Map70Exit03", 0, False, 6, 2,
+                  "Angel: Slider hole from chest toward water room (112->112)"],  # Slider
+            410: [411, 0, 0, 279, 266, "Map70Exit06", 0, False, 6, 2,
+                  "Angel: Water room monster area E door (112->113)"],
+            411: [410, 0, 0, 0, 0, "Map71Exit01", 0, False, 6, 2, "Angel: Wind Tunnel W door (113->112)"],
+            412: [413, 0, 0, 266, 267, "Map71Exit02", 0, False, 6, 2, "Angel: Wind Tunnel E door (113->114)"],
+            413: [412, 0, 0, 0, 0, "Map72Exit01", 0, False, 6, 2, "Angel: Long room W door (114->113)"],
+            414: [415, 0, 0, 267, 277, "Map72Exit02", 0, False, 6, 2,
+                  "Angel: Long room Slider hole toward Ishtar (114->115)"],  # Slider
+            415: [414, 0, 0, 0, 0, "Map73Exit01", 0, False, 6, 2, "Angel: Ishtar foyer Slider hole (115->114)"],
+            # Slider
+
             # Ishtar's Studio
-            420: [421, 0, 0, 277, 269, "Map73Exit02", 0, False, 6, 1, "Ishtar entrance" ],
-            421: [420, 0, 0,   0,   0, "Map73Exit03", 0, False, 6, 1, "Ishtar exit" ],
-            422: [423, 0, 0, 269, 270, "Map73Exit04", 0, False, 0, 1, "Ishtar: Portrait room (in)" ],
-            423: [422, 0, 0,   0,   0, "Map74Exit01", 0, False, 0, 1, "Ishtar: Portrait room (out)" ],
-            424: [425, 0, 0, 269, 271, "Map73Exit05", 0, False, 0, 1, "Ishtar: Side room (in)" ],
-            425: [424, 0, 0,   0,   0, "Map74Exit02", 0, False, 0, 1, "Ishtar: Side room (out)" ],
-            426: [427, 0, 0, 269, 272, "Map73Exit06", 0, False, 0, 1, "Ishtar: Ishtar's room (in)" ],
-            427: [426, 0, 0,   0,   0, "Map74Exit03", 0, False, 0, 1, "Ishtar: Ishtar's room (out)" ],
-            428: [429, 0, 0, 272, 274, "Map74Exit04", 0, False, 0, 1, "Ishtar: Puzzle room (in)" ],
-            429: [428, 0, 0,   0,   0, "Map75Exit11", 0, False, 0, 1, "Ishtar: Puzzle room (out)" ],
-            
+            420: [421, 0, 0, 277, 269, "Map73Exit02", 0, False, 6, 1, "Ishtar entrance"],
+            421: [420, 0, 0, 0, 0, "Map73Exit03", 0, False, 6, 1, "Ishtar exit"],
+            422: [423, 0, 0, 269, 270, "Map73Exit04", 0, False, 0, 1, "Ishtar: Portrait room (in)"],
+            423: [422, 0, 0, 0, 0, "Map74Exit01", 0, False, 0, 1, "Ishtar: Portrait room (out)"],
+            424: [425, 0, 0, 269, 271, "Map73Exit05", 0, False, 0, 1, "Ishtar: Side room (in)"],
+            425: [424, 0, 0, 0, 0, "Map74Exit02", 0, False, 0, 1, "Ishtar: Side room (out)"],
+            426: [427, 0, 0, 269, 272, "Map73Exit06", 0, False, 0, 1, "Ishtar: Ishtar's room (in)"],
+            427: [426, 0, 0, 0, 0, "Map74Exit03", 0, False, 0, 1, "Ishtar: Ishtar's room (out)"],
+            428: [429, 0, 0, 272, 274, "Map74Exit04", 0, False, 0, 1, "Ishtar: Puzzle room (in)"],
+            429: [428, 0, 0, 0, 0, "Map75Exit11", 0, False, 0, 1, "Ishtar: Puzzle room (out)"],
+
             # Watermia
-            440: [441, 0, 0, 280, 286, "Map78Exit01", 0, False, 0, 1, "Watermia: Lance House (in)" ],
-            441: [440, 0, 0,   0,   0, "Map79Exit01", 0, False, 0, 1, "Watermia: Lance House (out)" ],
-            442: [443, 0, 0, 280, 282, "Map78Exit04", 0, False, 0, 1, "Watermia: DS House (in)" ],
-            443: [442, 0, 0,   0,   0, "Map7CExit01", 0, False, 0, 1, "Watermia: DS House (out)" ],
-            444: [445, 0, 0, 280, 283, "Map78Exit03", 0, False, 0, 1, "Watermia: Gambling House (in)" ],
-            445: [444, 0, 0,   0,   0, "Map7BExit01", 0, False, 0, 1, "Watermia: Gambling House (out)" ],
-            446: [447, 0, 0, 280, 284, "Map78Exit05", 0, False, 0, 1, "Watermia: West House (in)" ],
-            447: [446, 0, 0,   0,   0, "Map7DExit01", 0, False, 0, 1, "Watermia: West House (out)" ],
-            448: [449, 0, 0, 280, 285, "Map78Exit06", 0, False, 0, 1, "Watermia: East House (in)" ],
-            449: [448, 0, 0,   0,   0, "Map7EExit01", 0, False, 0, 1, "Watermia: East House (out)" ],
-            450: [451, 0, 0, 280, 287, "Map78Exit02", 0, False, 0, 1, "Watermia: NW House (in)" ],
-            451: [450, 0, 0,   0,   0, "Map7AExit01", 0, False, 0, 1, "Watermia: NW House (out)" ],
-            452: [453, 0, 0, 288, 311, "",            0, False, 0, 0, "Watermia: Euro passage" ],
-            453: [452, 0, 0,   0,   0, "",            0, False, 0, 0, "Euro: Watermia passage" ],
-            
+            440: [441, 0, 0, 280, 286, "Map78Exit01", 0, False, 0, 1, "Watermia: Lance House (in)"],
+            441: [440, 0, 0, 0, 0, "Map79Exit01", 0, False, 0, 1, "Watermia: Lance House (out)"],
+            442: [443, 0, 0, 280, 282, "Map78Exit04", 0, False, 0, 1, "Watermia: DS House (in)"],
+            443: [442, 0, 0, 0, 0, "Map7CExit01", 0, False, 0, 1, "Watermia: DS House (out)"],
+            444: [445, 0, 0, 280, 283, "Map78Exit03", 0, False, 0, 1, "Watermia: Gambling House (in)"],
+            445: [444, 0, 0, 0, 0, "Map7BExit01", 0, False, 0, 1, "Watermia: Gambling House (out)"],
+            446: [447, 0, 0, 280, 284, "Map78Exit05", 0, False, 0, 1, "Watermia: West House (in)"],
+            447: [446, 0, 0, 0, 0, "Map7DExit01", 0, False, 0, 1, "Watermia: West House (out)"],
+            448: [449, 0, 0, 280, 285, "Map78Exit06", 0, False, 0, 1, "Watermia: East House (in)"],
+            449: [448, 0, 0, 0, 0, "Map7EExit01", 0, False, 0, 1, "Watermia: East House (out)"],
+            450: [451, 0, 0, 280, 287, "Map78Exit02", 0, False, 0, 1, "Watermia: NW House (in)"],
+            451: [450, 0, 0, 0, 0, "Map7AExit01", 0, False, 0, 1, "Watermia: NW House (out)"],
+            452: [453, 0, 0, 288, 311, "", 0, False, 0, 0, "Watermia: Euro passage"],
+            453: [452, 0, 0, 0, 0, "", 0, False, 0, 0, "Euro: Watermia passage"],
+
             # Great Wall
-            462: [463, 0, 0, 290, 291, "Map82Exit01", 0, False, 7, 3, "Great Wall: Entrance room E exit (130->131)" ],
-            463: [462, 0, 0,   0,   0, "Map83Exit01", 0, False, 7, 2, "Great Wall: Long drop room W exit (131->130)" ],
-            464: [465, 0, 0, 293, 294, "Map83Exit02", 0, False, 7, 2, "Great Wall: Long drop room E exit (131->133)" ],
-            465: [464, 0, 0,   0,   0, "Map85Exit01", 0, False, 7, 2, "Great Wall: Forced ramp room W exit (133->131)" ],
-            466: [467, 0, 0, 296, 297, "Map85Exit02", 0, False, 7, 2, "Great Wall: Forced ramp room E exit (133->134)" ],
-            467: [466, 0, 0,   0,   0, "Map86Exit01", 0, False, 7, 2, "Great Wall: Dark Space platform room W exit (134->133)" ],
-            468: [469, 0, 0, 297, 298, "Map86Exit02", 0, False, 7, 2, "Great Wall: Dark Space platform room E exit (134->135)" ],
-            469: [468, 0, 0,   0,   0, "Map87Exit01", 0, False, 7, 2, "Great Wall: Friar room W exit (135->134)" ],
-            470: [471, 0, 0, 299, 300, "Map87Exit02", 0, False, 7, 2, "Great Wall: Friar room E exit (135->136)" ],
-            471: [470, 0, 0,   0,   0, "Map88Exit01", 0, False, 7, 2, "Great Wall: Final Dark Space room W exit (136->135)" ],
-            
+            462: [463, 0, 0, 290, 291, "Map82Exit01", 0, False, 7, 3, "Great Wall: Entrance room E exit (130->131)"],
+            463: [462, 0, 0, 0, 0, "Map83Exit01", 0, False, 7, 2, "Great Wall: Long drop room W exit (131->130)"],
+            464: [465, 0, 0, 293, 294, "Map83Exit02", 0, False, 7, 2, "Great Wall: Long drop room E exit (131->133)"],
+            465: [464, 0, 0, 0, 0, "Map85Exit01", 0, False, 7, 2, "Great Wall: Forced ramp room W exit (133->131)"],
+            466: [467, 0, 0, 296, 297, "Map85Exit02", 0, False, 7, 2, "Great Wall: Forced ramp room E exit (133->134)"],
+            467: [466, 0, 0, 0, 0, "Map86Exit01", 0, False, 7, 2,
+                  "Great Wall: Dark Space platform room W exit (134->133)"],
+            468: [469, 0, 0, 297, 298, "Map86Exit02", 0, False, 7, 2,
+                  "Great Wall: Dark Space platform room E exit (134->135)"],
+            469: [468, 0, 0, 0, 0, "Map87Exit01", 0, False, 7, 2, "Great Wall: Friar room W exit (135->134)"],
+            470: [471, 0, 0, 299, 300, "Map87Exit02", 0, False, 7, 2, "Great Wall: Friar room E exit (135->136)"],
+            471: [470, 0, 0, 0, 0, "Map88Exit01", 0, False, 7, 2,
+                  "Great Wall: Final Dark Space room W exit (136->135)"],
+
             # Euro
-            482: [483, 0, 0, 310, 312, "Map91Exit03", 0, False, 0, 1, "Euro: Rolek Company (in)" ],
-            483: [482, 0, 0,   0,   0, "Map94Exit01", 0, False, 0, 1, "Euro: Rolek Company (out)" ],
-            484: [485, 0, 0, 310, 313, "Map91Exit08", 0, False, 0, 1, "Euro: West House (in)" ],
-            485: [484, 0, 0,   0,   0, "Map98Exit01", 0, False, 0, 1, "Euro: West House (out)" ],
-            486: [487, 0, 0, 310, 314, "Map91Exit04", 0, False, 0, 1, "Euro: Rolek Mansion West (in)" ],
-            487: [486, 0, 0,   0,   0, "Map95Exit01", 0, False, 0, 1, "Euro: Rolek Mansion West (out)" ],
-            488: [489, 0, 0, 310, 314, "Map91Exit05", 0, False, 0, 1, "Euro: Rolek Mansion East (in)" ],
-            489: [488, 0, 0,   0,   0, "Map95Exit02", 0, False, 0, 1, "Euro: Rolek Mansion East (out)" ],
-            490: [491, 0, 0, 310, 317, "Map91Exit0A", 0, False, 0, 1, "Euro: Central House (in)" ],
-            491: [490, 0, 0,   0,   0, "Map9AExit01", 0, False, 0, 1, "Euro: Central House (out)" ],
-            492: [493, 0, 0, 310, 318, "Map91Exit0B", 0, False, 0, 1, "Euro: Jeweler House (in)" ],
-            493: [492, 0, 0,   0,   0, "Map9BExit01", 0, False, 0, 1, "Euro: Jeweler House (out)" ],
-            494: [495, 0, 0, 310, 319, "Map91Exit0C", 0, False, 0, 1, "Euro: Twins House (in)" ],
-            495: [494, 0, 0,   0,   0, "Map9CExit01", 0, False, 0, 1, "Euro: Twins House (out)" ],
-            496: [497, 0, 0, 310, 320, "Map91Exit02", 0, False, 0, 1, "Euro: Hidden House (in)" ],
-            497: [496, 0, 0,   0,   0, "Map93Exit01", 0, False, 0, 1, "Euro: Hidden House (out)" ],
-            498: [499, 0, 0, 310, 321, "Map91Exit0D", 0, False, 0, 1, "Euro: Shrine (in)" ],
-            499: [498, 0, 0,   0,   0, "Map9DExit01", 0, False, 0, 1, "Euro: Shrine (out)" ],
-            500: [501, 0, 0, 310, 322, "Map91Exit01", 0, False, 0, 1, "Euro: Explorer's House (in)" ],
-            501: [500, 0, 0,   0,   0, "Map92Exit01", 0, False, 0, 1, "Euro: Explorer's House (out)" ],
-            502: [  0, 0, 0, 310, 323, "Map91Exit06", 0, False, 0, 1, "Euro: Store Entrance (in)" ],
-            #503: [502, 0, 0,   0,   0, "",           0, False, 0, 0, "Euro: Store Entrance (out)" ], #this doesn't exist!
-            504: [505, 0, 0, 310, 324, "Map91Exit07", 0, False, 0, 1, "Euro: Store Exit (in)" ],
-            505: [504, 0, 0,   0,   0, "Map97Exit01", 0, False, 0, 1, "Euro: Store Exit (out)" ],
-            506: [507, 0, 0, 314, 316, "Map95Exit03", 0, False, 0, 1, "Euro: Guest Room (in)" ],
-            507: [506, 0, 0,   0,   0, "Map96Exit01", 0, False, 0, 1, "Euro: Guest Room (out)" ],
-            508: [509, 0, 0, 310, 325, "Map91Exit09", 0, False, 0, 1, "Euro: Dark Space House (in)" ],
-            509: [508, 0, 0,   0,   0, "Map99Exit01", 0, False, 0, 1, "Euro: Dark Space House (out)" ],
-            
+            482: [483, 0, 0, 310, 312, "Map91Exit03", 0, False, 0, 1, "Euro: Rolek Company (in)"],
+            483: [482, 0, 0, 0, 0, "Map94Exit01", 0, False, 0, 1, "Euro: Rolek Company (out)"],
+            484: [485, 0, 0, 310, 313, "Map91Exit08", 0, False, 0, 1, "Euro: West House (in)"],
+            485: [484, 0, 0, 0, 0, "Map98Exit01", 0, False, 0, 1, "Euro: West House (out)"],
+            486: [487, 0, 0, 310, 314, "Map91Exit04", 0, False, 0, 1, "Euro: Rolek Mansion West (in)"],
+            487: [486, 0, 0, 0, 0, "Map95Exit01", 0, False, 0, 1, "Euro: Rolek Mansion West (out)"],
+            488: [489, 0, 0, 310, 314, "Map91Exit05", 0, False, 0, 1, "Euro: Rolek Mansion East (in)"],
+            489: [488, 0, 0, 0, 0, "Map95Exit02", 0, False, 0, 1, "Euro: Rolek Mansion East (out)"],
+            490: [491, 0, 0, 310, 317, "Map91Exit0A", 0, False, 0, 1, "Euro: Central House (in)"],
+            491: [490, 0, 0, 0, 0, "Map9AExit01", 0, False, 0, 1, "Euro: Central House (out)"],
+            492: [493, 0, 0, 310, 318, "Map91Exit0B", 0, False, 0, 1, "Euro: Jeweler House (in)"],
+            493: [492, 0, 0, 0, 0, "Map9BExit01", 0, False, 0, 1, "Euro: Jeweler House (out)"],
+            494: [495, 0, 0, 310, 319, "Map91Exit0C", 0, False, 0, 1, "Euro: Twins House (in)"],
+            495: [494, 0, 0, 0, 0, "Map9CExit01", 0, False, 0, 1, "Euro: Twins House (out)"],
+            496: [497, 0, 0, 310, 320, "Map91Exit02", 0, False, 0, 1, "Euro: Hidden House (in)"],
+            497: [496, 0, 0, 0, 0, "Map93Exit01", 0, False, 0, 1, "Euro: Hidden House (out)"],
+            498: [499, 0, 0, 310, 321, "Map91Exit0D", 0, False, 0, 1, "Euro: Shrine (in)"],
+            499: [498, 0, 0, 0, 0, "Map9DExit01", 0, False, 0, 1, "Euro: Shrine (out)"],
+            500: [501, 0, 0, 310, 322, "Map91Exit01", 0, False, 0, 1, "Euro: Explorer's House (in)"],
+            501: [500, 0, 0, 0, 0, "Map92Exit01", 0, False, 0, 1, "Euro: Explorer's House (out)"],
+            502: [0, 0, 0, 310, 323, "Map91Exit06", 0, False, 0, 1, "Euro: Store Entrance (in)"],
+            # 503: [502, 0, 0,   0,   0, "",           0, False, 0, 0, "Euro: Store Entrance (out)" ], #this doesn't exist!
+            504: [505, 0, 0, 310, 324, "Map91Exit07", 0, False, 0, 1, "Euro: Store Exit (in)"],
+            505: [504, 0, 0, 0, 0, "Map97Exit01", 0, False, 0, 1, "Euro: Store Exit (out)"],
+            506: [507, 0, 0, 314, 316, "Map95Exit03", 0, False, 0, 1, "Euro: Guest Room (in)"],
+            507: [506, 0, 0, 0, 0, "Map96Exit01", 0, False, 0, 1, "Euro: Guest Room (out)"],
+            508: [509, 0, 0, 310, 325, "Map91Exit09", 0, False, 0, 1, "Euro: Dark Space House (in)"],
+            509: [508, 0, 0, 0, 0, "Map99Exit01", 0, False, 0, 1, "Euro: Dark Space House (out)"],
+
             # Mt. Kress
-            522: [523, 0, 0, 330, 331, "MapA0Exit01", 0, False, 8, 3, "Mt. Kress: Entrance room NW exit (160->161)" ],
-            523: [522, 0, 0,   0,   0, "MapA1Exit01", 0, False, 8, 2, "Mt. Kress: First DS room, E exit (161->160)" ],
-            524: [525, 0, 0, 332, 333, "MapA1Exit02", 0, False, 8, 2, "Mt. Kress: First DS room, western N exit (161->162)" ],
-            525: [524, 0, 0,   0,   0, "MapA2Exit01", 0, False, 8, 2, "Mt. Kress: First vine room, SW exit (162->161)" ],
-            526: [527, 0, 0, 332, 334, "MapA1Exit03", 0, False, 8, 2, "Mt. Kress: First DS room, eastern N exit (161->162)" ],
-            527: [526, 0, 0,   0,   0, "MapA2Exit02", 0, False, 8, 2, "Mt. Kress: First vine room, S exit before ramp (162->161)" ],
-            528: [529, 0, 0, 333, 337, "MapA2Exit04", 0, False, 8, 2, "Mt. Kress: First vine room, E exit (162->163)" ],
-            529: [528, 0, 0,   0,   0, "MapA3Exit02", 0, False, 8, 2, "Mt. Kress: Second DS room, NW exit (163->162)" ],
-            530: [531, 0, 0, 337, 336, "MapA3Exit01", 0, False, 8, 2, "Mt. Kress: Second DS room, SW exit (163->162)" ],
-            531: [530, 0, 0,   0,   0, "MapA2Exit03", 0, False, 8, 2, "Mt. Kress: First vine room, exit from chest area (162->163)" ],
-            532: [533, 0, 0, 333, 338, "MapA2Exit05", 0, False, 8, 2, "Mt. Kress: First vine room, W exit (162->164)" ],
-            533: [532, 0, 0,   0,   0, "MapA4Exit01", 0, False, 8, 2, "Mt. Kress: West Drops chest room exit (164->162)" ],
-            534: [535, 0, 0, 335, 339, "MapA2Exit06", 0, False, 8, 2, "Mt. Kress: First vine room NW exit (162->165)" ],
-            535: [534, 0, 0,   0,   0, "MapA5Exit01", 0, False, 8, 2, "Mt. Kress: Second vine room SW exit (165->162)" ],
-            536: [537, 0, 0, 339, 342, "MapA5Exit02", 0, False, 8, 2, "Mt. Kress: Second vine room SE exit (165->166)" ],
-            537: [536, 0, 0,   0,   0, "MapA6Exit01", 0, False, 8, 2, "Mt. Kress: Mushroom arena exit (166->165)" ],
-            538: [539, 0, 0, 340, 343, "MapA5Exit03", 0, False, 8, 2, "Mt. Kress: Second vine room NE exit (165->167)" ],
-            539: [538, 0, 0,   0,   0, "MapA7Exit01", 0, False, 8, 2, "Mt. Kress: Third Drops/DS room exit (167->165)" ],
-            540: [541, 0, 0, 341, 344, "MapA5Exit04", 0, False, 8, 2, "Mt. Kress: Second vine room NW exit (165->168)" ],
-            541: [540, 0, 0,   0,   0, "MapA8Exit01", 0, False, 8, 2, "Mt. Kress: Final combat corridor E exit (168->165)" ],
-            542: [543, 0, 0, 344, 345, "MapA8Exit02", 0, False, 8, 2, "Mt. Kress: Final combat corridor NW exit (168->169)" ],
-            543: [542, 0, 0,   0,   0, "MapA9Exit01", 0, False, 8, 2, "Mt. Kress: End Teapot chest room exit (169->168)" ],
-            
+            522: [523, 0, 0, 330, 331, "MapA0Exit01", 0, False, 8, 3, "Mt. Kress: Entrance room NW exit (160->161)"],
+            523: [522, 0, 0, 0, 0, "MapA1Exit01", 0, False, 8, 2, "Mt. Kress: First DS room, E exit (161->160)"],
+            524: [525, 0, 0, 332, 333, "MapA1Exit02", 0, False, 8, 2,
+                  "Mt. Kress: First DS room, western N exit (161->162)"],
+            525: [524, 0, 0, 0, 0, "MapA2Exit01", 0, False, 8, 2, "Mt. Kress: First vine room, SW exit (162->161)"],
+            526: [527, 0, 0, 332, 334, "MapA1Exit03", 0, False, 8, 2,
+                  "Mt. Kress: First DS room, eastern N exit (161->162)"],
+            527: [526, 0, 0, 0, 0, "MapA2Exit02", 0, False, 8, 2,
+                  "Mt. Kress: First vine room, S exit before ramp (162->161)"],
+            528: [529, 0, 0, 333, 337, "MapA2Exit04", 0, False, 8, 2, "Mt. Kress: First vine room, E exit (162->163)"],
+            529: [528, 0, 0, 0, 0, "MapA3Exit02", 0, False, 8, 2, "Mt. Kress: Second DS room, NW exit (163->162)"],
+            530: [531, 0, 0, 337, 336, "MapA3Exit01", 0, False, 8, 2, "Mt. Kress: Second DS room, SW exit (163->162)"],
+            531: [530, 0, 0, 0, 0, "MapA2Exit03", 0, False, 8, 2,
+                  "Mt. Kress: First vine room, exit from chest area (162->163)"],
+            532: [533, 0, 0, 333, 338, "MapA2Exit05", 0, False, 8, 2, "Mt. Kress: First vine room, W exit (162->164)"],
+            533: [532, 0, 0, 0, 0, "MapA4Exit01", 0, False, 8, 2, "Mt. Kress: West Drops chest room exit (164->162)"],
+            534: [535, 0, 0, 335, 339, "MapA2Exit06", 0, False, 8, 2, "Mt. Kress: First vine room NW exit (162->165)"],
+            535: [534, 0, 0, 0, 0, "MapA5Exit01", 0, False, 8, 2, "Mt. Kress: Second vine room SW exit (165->162)"],
+            536: [537, 0, 0, 339, 342, "MapA5Exit02", 0, False, 8, 2, "Mt. Kress: Second vine room SE exit (165->166)"],
+            537: [536, 0, 0, 0, 0, "MapA6Exit01", 0, False, 8, 2, "Mt. Kress: Mushroom arena exit (166->165)"],
+            538: [539, 0, 0, 340, 343, "MapA5Exit03", 0, False, 8, 2, "Mt. Kress: Second vine room NE exit (165->167)"],
+            539: [538, 0, 0, 0, 0, "MapA7Exit01", 0, False, 8, 2, "Mt. Kress: Third Drops/DS room exit (167->165)"],
+            540: [541, 0, 0, 341, 344, "MapA5Exit04", 0, False, 8, 2, "Mt. Kress: Second vine room NW exit (165->168)"],
+            541: [540, 0, 0, 0, 0, "MapA8Exit01", 0, False, 8, 2, "Mt. Kress: Final combat corridor E exit (168->165)"],
+            542: [543, 0, 0, 344, 345, "MapA8Exit02", 0, False, 8, 2,
+                  "Mt. Kress: Final combat corridor NW exit (168->169)"],
+            543: [542, 0, 0, 0, 0, "MapA9Exit01", 0, False, 8, 2, "Mt. Kress: End Teapot chest room exit (169->168)"],
+
             # Native's Village
-            552: [553, 0, 0, 350, 352, "MapACExit01", 0, False, 0, 1, "Native's Village: West House (in)" ],
-            553: [552, 0, 0,   0,   0, "MapADExit01", 0, False, 0, 1, "Native's Village: West House (out)" ],
-            554: [555, 0, 0, 350, 353, "MapACExit02", 0, False, 0, 1, "Native's Village: House w/Statues (in)" ],
-            555: [554, 0, 0,   0,   0, "MapAEExit01", 0, False, 0, 1, "Native's Village: House w/Statues (out)" ],
-            556: [557, 0, 0, 351, 400, "",            0, False, 0, 0, "Native's Village: Dao Passage" ],
-            557: [556, 0, 0,   0,   0, "",            0, False, 0, 0, "Dao: Natives' Passage" ],
-            
+            552: [553, 0, 0, 350, 352, "MapACExit01", 0, False, 0, 1, "Native's Village: West House (in)"],
+            553: [552, 0, 0, 0, 0, "MapADExit01", 0, False, 0, 1, "Native's Village: West House (out)"],
+            554: [555, 0, 0, 350, 353, "MapACExit02", 0, False, 0, 1, "Native's Village: House w/Statues (in)"],
+            555: [554, 0, 0, 0, 0, "MapAEExit01", 0, False, 0, 1, "Native's Village: House w/Statues (out)"],
+            556: [557, 0, 0, 351, 400, "", 0, False, 0, 0, "Native's Village: Dao Passage"],
+            557: [556, 0, 0, 0, 0, "", 0, False, 0, 0, "Dao: Natives' Passage"],
+
             # Ankor Wat
-            562: [563, 0, 0, 360, 361, "MapB0Exit01", 0, False, 9, 3, "Ankor Wat: Exterior entry door (176->177)" ],
-            563: [562, 0, 0,   0,   0, "MapB1Exit01", 0, False, 9, 2, "Ankor Wat: Outer-South room S door (177->176)" ],
-            564: [565, 0, 0, 361, 363, "MapB1Exit02", 0, False, 9, 2, "Ankor Wat: Outer-South room NE door (177->178)" ],
-            565: [564, 0, 0,   0,   0, "MapB2Exit01", 0, False, 9, 2, "Ankor Wat: Outer-East room S door (178->177)" ],
-            566: [567, 0, 0, 365, 366, "MapB2Exit02", 0, False, 9, 2, "Ankor Wat: Outer-East room N door (178->179)" ],
-            567: [566, 0, 0,   0,   0, "MapB3Exit01", 0, False, 9, 2, "Ankor Wat: Outer-North room SE door (179->178)" ],
-            568: [569, 0, 0, 368, 367, "MapB4Exit01", 0, False, 9, 2, "Ankor Wat: Pit exit (180->179)" ],
-            569: [568, 0, 0,   0,   0, "MapB3Exit03", 0, False, 9, 2, "Ankor Wat: Outer-North room NW door (179->180)" ],
-            570: [571, 0, 0, 367, 369, "MapB3Exit04", 0, False, 9, 2, "Ankor Wat: Outer-North room SW door (179->181)" ],
-            571: [570, 0, 0,   0,   0, "MapB5Exit01", 0, False, 9, 2, "Ankor Wat: Outer-West room N door (181->179)" ],
-            572: [573, 0, 0, 371, 362, "MapB5Exit02", 0, False, 9, 2, "Ankor Wat: Outer-West room S door (181->177)" ],
-            573: [572, 0, 0,   0,   0, "MapB1Exit04", 0, False, 9, 2, "Ankor Wat: Outer-South room NW door (177->181)" ],
-            574: [575, 0, 0, 362, 372, "MapB1Exit03", 0, False, 9, 2, "Ankor Wat: Outer-South room N door toward Garden (177->182)" ],
-            575: [574, 0, 0,   0,   0, "MapB6Exit01", 0, False, 9, 2, "Ankor Wat: Garden S exit (182->177)" ],
-            576: [577, 0, 0, 372, 373, "MapB6Exit02", 0, False, 9, 2, "Ankor Wat: Garden N exit (182->183)" ],
-            577: [576, 0, 0,   0,   0, "MapB7Exit01", 0, False, 9, 2, "Ankor Wat: Inner-South room, main area S door (183->182)" ],
-            578: [579, 0, 0, 373, 376, "MapB7Exit04", 0, False, 9, 2, "Ankor Wat: Inner-South room, main area NE door (183->184)" ],
-            579: [578, 0, 0,   0,   0, "MapB8Exit01", 0, False, 9, 2, "Ankor Wat: Inner-East room S door (184->183)" ],
-            580: [581, 0, 0, 374, 378, "MapB7Exit02", 0, False, 9, 2, "Ankor Wat: Inner-South room, NW door behind Quake (183->185)" ],
-            581: [580, 0, 0,   0,   0, "MapB9Exit01", 0, False, 9, 2, "Ankor Wat: Inner-West room, SW exit (185->183)" ],
-            582: [583, 0, 0, 378, 375, "MapB9Exit02", 0, False, 9, 2, "Ankor Wat: Inner-West room, SE exit (185->183)" ],
-            583: [582, 0, 0,   0,   0, "MapB7Exit03", 0, False, 9, 2, "Ankor Wat: Inner-South room, north corridor NW exit (183->185)" ],
-            584: [585, 0, 0, 375, 379, "MapB7Exit05", 0, False, 9, 2, "Ankor Wat: Inner-South room, north corridor N exit toward Main Hall (183->186)" ],
-            585: [584, 0, 0,   0,   0, "MapBAExit01", 0, False, 9, 2, "Ankor Wat: Road to Main Hall S door (186->183)" ],
-            586: [587, 0, 0, 379, 381, "MapBAExit02", 0, False, 9, 2, "Ankor Wat: Road to Main Hall N door (186->187)" ],
-            587: [586, 0, 0,   0,   0, "MapBBExit01", 0, False, 9, 2, "Ankor Wat: Main Hall 1F, SW exit (187->186)" ],
-            588: [589, 0, 0, 381, 380, "MapBBExit02", 0, False, 9, 2, "Ankor Wat: Main Hall 1F, SE exit (187->186)" ],
-            589: [588, 0, 0,   0,   0, "MapBAExit03", 0, False, 9, 2, "Ankor Wat: Road to Main Hall, dead-end Glasses area exit (186->187)" ],
-            590: [591, 0, 0, 381, 384, "MapBBExit03", 0, False, 9, 2, "Ankor Wat: Main Hall 1F, stairs up (187->188)" ],
-            591: [590, 0, 0,   0,   0, "MapBCExit01", 0, False, 9, 2, "Ankor Wat: Main Hall 2F, N stairs down (188->187)" ],
-            592: [593, 0, 0, 385, 386, "MapBCExit06", 0, False, 9, 2, "Ankor Wat: Main Hall 2F, S stairs up (188->189)" ],
-            593: [592, 0, 0,   0,   0, "MapBDExit01", 0, False, 9, 2, "Ankor Wat: Main Hall 3F, S stairs down (189->188)" ],
-            594: [595, 0, 0, 387, 389, "MapBDExit03", 0, False, 9, 2, "Ankor Wat: Main Hall 3F, NE stairs up (189->190)" ],
-            595: [594, 0, 0,   0,   0, "MapBEExit02", 0, False, 9, 2, "Ankor Wat: Main Hall 4F chest area, NE stairs down (190->189)" ],
-            596: [597, 0, 0, 388, 390, "MapBDExit02", 0, False, 9, 2, "Ankor Wat: Main Hall 3F above ledge, NW stairs up (189->190)" ],
-            597: [596, 0, 0,   0,   0, "MapBEExit01", 0, False, 9, 2, "Ankor Wat: Main Hall 4F final corridor, NW stairs down (190->189)" ],
-            598: [599, 0, 0, 390, 391, "MapBEExit04", 0, False, 9, 2, "Ankor Wat: Main Hall 4F final corridor, center stairs (190->191)" ],
-            599: [598, 0, 0,   0,   0, "MapBFExit01", 0, False, 9, 2, "Ankor Wat: Spirit room exit (191->190)" ],
-            600: [  0, 0, 0, 366, 368, "MapB3Exit02", 0, False, 9, 2, "Ankor Wat: Outer-North room drop (179->180)" ],
-            601: [  0, 0, 0, 384, 381, "MapBCExit02", 0, False, 9, 2, "Ankor Wat: Main Hall 2F, left useless drop (188->187)" ],
-            602: [  0, 0, 0, 384, 381, "MapBCExit03", 0, False, 9, 2, "Ankor Wat: Main Hall 2F, right useless drop (188->187)" ],
-            603: [  0, 0, 0, 384, 383, "MapBCExit04", 0, False, 9, 2, "Ankor Wat: Main Hall 2F, E drop toward DS (188->187)" ],
-            604: [  0, 0, 0, 385, 382, "MapBCExit05", 0, False, 9, 2, "Ankor Wat: Main Hall 2F, SW drop toward chest (188->187)" ],
-            605: [  0, 0, 0, 389, 388, "MapBEExit03", 0, False, 9, 2, "Ankor Wat: Main Hall 4F chest area drop (190->189)" ],
-            
+            562: [563, 0, 0, 360, 361, "MapB0Exit01", 0, False, 9, 3, "Ankor Wat: Exterior entry door (176->177)"],
+            563: [562, 0, 0, 0, 0, "MapB1Exit01", 0, False, 9, 2, "Ankor Wat: Outer-South room S door (177->176)"],
+            564: [565, 0, 0, 361, 363, "MapB1Exit02", 0, False, 9, 2, "Ankor Wat: Outer-South room NE door (177->178)"],
+            565: [564, 0, 0, 0, 0, "MapB2Exit01", 0, False, 9, 2, "Ankor Wat: Outer-East room S door (178->177)"],
+            566: [567, 0, 0, 365, 366, "MapB2Exit02", 0, False, 9, 2, "Ankor Wat: Outer-East room N door (178->179)"],
+            567: [566, 0, 0, 0, 0, "MapB3Exit01", 0, False, 9, 2, "Ankor Wat: Outer-North room SE door (179->178)"],
+            568: [569, 0, 0, 368, 367, "MapB4Exit01", 0, False, 9, 2, "Ankor Wat: Pit exit (180->179)"],
+            569: [568, 0, 0, 0, 0, "MapB3Exit03", 0, False, 9, 2, "Ankor Wat: Outer-North room NW door (179->180)"],
+            570: [571, 0, 0, 367, 369, "MapB3Exit04", 0, False, 9, 2, "Ankor Wat: Outer-North room SW door (179->181)"],
+            571: [570, 0, 0, 0, 0, "MapB5Exit01", 0, False, 9, 2, "Ankor Wat: Outer-West room N door (181->179)"],
+            572: [573, 0, 0, 371, 362, "MapB5Exit02", 0, False, 9, 2, "Ankor Wat: Outer-West room S door (181->177)"],
+            573: [572, 0, 0, 0, 0, "MapB1Exit04", 0, False, 9, 2, "Ankor Wat: Outer-South room NW door (177->181)"],
+            574: [575, 0, 0, 362, 372, "MapB1Exit03", 0, False, 9, 2,
+                  "Ankor Wat: Outer-South room N door toward Garden (177->182)"],
+            575: [574, 0, 0, 0, 0, "MapB6Exit01", 0, False, 9, 2, "Ankor Wat: Garden S exit (182->177)"],
+            576: [577, 0, 0, 372, 373, "MapB6Exit02", 0, False, 9, 2, "Ankor Wat: Garden N exit (182->183)"],
+            577: [576, 0, 0, 0, 0, "MapB7Exit01", 0, False, 9, 2,
+                  "Ankor Wat: Inner-South room, main area S door (183->182)"],
+            578: [579, 0, 0, 373, 376, "MapB7Exit04", 0, False, 9, 2,
+                  "Ankor Wat: Inner-South room, main area NE door (183->184)"],
+            579: [578, 0, 0, 0, 0, "MapB8Exit01", 0, False, 9, 2, "Ankor Wat: Inner-East room S door (184->183)"],
+            580: [581, 0, 0, 374, 378, "MapB7Exit02", 0, False, 9, 2,
+                  "Ankor Wat: Inner-South room, NW door behind Quake (183->185)"],
+            581: [580, 0, 0, 0, 0, "MapB9Exit01", 0, False, 9, 2, "Ankor Wat: Inner-West room, SW exit (185->183)"],
+            582: [583, 0, 0, 378, 375, "MapB9Exit02", 0, False, 9, 2, "Ankor Wat: Inner-West room, SE exit (185->183)"],
+            583: [582, 0, 0, 0, 0, "MapB7Exit03", 0, False, 9, 2,
+                  "Ankor Wat: Inner-South room, north corridor NW exit (183->185)"],
+            584: [585, 0, 0, 375, 379, "MapB7Exit05", 0, False, 9, 2,
+                  "Ankor Wat: Inner-South room, north corridor N exit toward Main Hall (183->186)"],
+            585: [584, 0, 0, 0, 0, "MapBAExit01", 0, False, 9, 2, "Ankor Wat: Road to Main Hall S door (186->183)"],
+            586: [587, 0, 0, 379, 381, "MapBAExit02", 0, False, 9, 2, "Ankor Wat: Road to Main Hall N door (186->187)"],
+            587: [586, 0, 0, 0, 0, "MapBBExit01", 0, False, 9, 2, "Ankor Wat: Main Hall 1F, SW exit (187->186)"],
+            588: [589, 0, 0, 381, 380, "MapBBExit02", 0, False, 9, 2, "Ankor Wat: Main Hall 1F, SE exit (187->186)"],
+            589: [588, 0, 0, 0, 0, "MapBAExit03", 0, False, 9, 2,
+                  "Ankor Wat: Road to Main Hall, dead-end Glasses area exit (186->187)"],
+            590: [591, 0, 0, 381, 384, "MapBBExit03", 0, False, 9, 2, "Ankor Wat: Main Hall 1F, stairs up (187->188)"],
+            591: [590, 0, 0, 0, 0, "MapBCExit01", 0, False, 9, 2, "Ankor Wat: Main Hall 2F, N stairs down (188->187)"],
+            592: [593, 0, 0, 385, 386, "MapBCExit06", 0, False, 9, 2,
+                  "Ankor Wat: Main Hall 2F, S stairs up (188->189)"],
+            593: [592, 0, 0, 0, 0, "MapBDExit01", 0, False, 9, 2, "Ankor Wat: Main Hall 3F, S stairs down (189->188)"],
+            594: [595, 0, 0, 387, 389, "MapBDExit03", 0, False, 9, 2,
+                  "Ankor Wat: Main Hall 3F, NE stairs up (189->190)"],
+            595: [594, 0, 0, 0, 0, "MapBEExit02", 0, False, 9, 2,
+                  "Ankor Wat: Main Hall 4F chest area, NE stairs down (190->189)"],
+            596: [597, 0, 0, 388, 390, "MapBDExit02", 0, False, 9, 2,
+                  "Ankor Wat: Main Hall 3F above ledge, NW stairs up (189->190)"],
+            597: [596, 0, 0, 0, 0, "MapBEExit01", 0, False, 9, 2,
+                  "Ankor Wat: Main Hall 4F final corridor, NW stairs down (190->189)"],
+            598: [599, 0, 0, 390, 391, "MapBEExit04", 0, False, 9, 2,
+                  "Ankor Wat: Main Hall 4F final corridor, center stairs (190->191)"],
+            599: [598, 0, 0, 0, 0, "MapBFExit01", 0, False, 9, 2, "Ankor Wat: Spirit room exit (191->190)"],
+            600: [0, 0, 0, 366, 368, "MapB3Exit02", 0, False, 9, 2, "Ankor Wat: Outer-North room drop (179->180)"],
+            601: [0, 0, 0, 384, 381, "MapBCExit02", 0, False, 9, 2,
+                  "Ankor Wat: Main Hall 2F, left useless drop (188->187)"],
+            602: [0, 0, 0, 384, 381, "MapBCExit03", 0, False, 9, 2,
+                  "Ankor Wat: Main Hall 2F, right useless drop (188->187)"],
+            603: [0, 0, 0, 384, 383, "MapBCExit04", 0, False, 9, 2,
+                  "Ankor Wat: Main Hall 2F, E drop toward DS (188->187)"],
+            604: [0, 0, 0, 385, 382, "MapBCExit05", 0, False, 9, 2,
+                  "Ankor Wat: Main Hall 2F, SW drop toward chest (188->187)"],
+            605: [0, 0, 0, 389, 388, "MapBEExit03", 0, False, 9, 2,
+                  "Ankor Wat: Main Hall 4F chest area drop (190->189)"],
+
             # Dao
-            612: [613, 0, 0, 400, 401, "MapC3Exit01", 0, False, 0, 1, "Dao: NW House (in)" ],
-            613: [612, 0, 0,   0,   0, "MapC4Exit01", 0, False, 0, 1, "Dao: NW House (out)" ],
-            614: [615, 0, 0, 400, 402, "MapC3Exit02", 0, False, 0, 1, "Dao: Neil's House (in)" ],
-            615: [614, 0, 0,   0,   0, "MapC8Exit01", 0, False, 0, 1, "Dao: Neil's House (out)" ],
-            616: [617, 0, 0, 400, 403, "MapC3Exit03", 0, False, 0, 1, "Dao: Snake Game House (in)" ],
-            617: [616, 0, 0,   0,   0, "MapC6Exit01", 0, False, 0, 1, "Dao: Snake Game House (out)" ],
-            618: [619, 0, 0, 400, 404, "MapC3Exit04", 0, False, 0, 1, "Dao: SW House (in)" ],
-            619: [618, 0, 0,   0,   0, "MapC7Exit01", 0, False, 0, 1, "Dao: SW House (out)" ],
-            620: [621, 0, 0, 400, 405, "MapC3Exit05", 0, False, 0, 1, "Dao: S House (in)" ],
-            621: [620, 0, 0,   0,   0, "MapC5Exit01", 0, False, 0, 1, "Dao: S House (out)" ],
-            622: [623, 0, 0, 400, 406, "MapC3Exit06", 0, False, 0, 1, "Dao: SE House (in)" ],
-            623: [622, 0, 0,   0,   0, "MapC9Exit01", 0, False, 0, 1, "Dao: SE House (out)" ],
-            
+            612: [613, 0, 0, 400, 401, "MapC3Exit01", 0, False, 0, 1, "Dao: NW House (in)"],
+            613: [612, 0, 0, 0, 0, "MapC4Exit01", 0, False, 0, 1, "Dao: NW House (out)"],
+            614: [615, 0, 0, 400, 402, "MapC3Exit02", 0, False, 0, 1, "Dao: Neil's House (in)"],
+            615: [614, 0, 0, 0, 0, "MapC8Exit01", 0, False, 0, 1, "Dao: Neil's House (out)"],
+            616: [617, 0, 0, 400, 403, "MapC3Exit03", 0, False, 0, 1, "Dao: Snake Game House (in)"],
+            617: [616, 0, 0, 0, 0, "MapC6Exit01", 0, False, 0, 1, "Dao: Snake Game House (out)"],
+            618: [619, 0, 0, 400, 404, "MapC3Exit04", 0, False, 0, 1, "Dao: SW House (in)"],
+            619: [618, 0, 0, 0, 0, "MapC7Exit01", 0, False, 0, 1, "Dao: SW House (out)"],
+            620: [621, 0, 0, 400, 405, "MapC3Exit05", 0, False, 0, 1, "Dao: S House (in)"],
+            621: [620, 0, 0, 0, 0, "MapC5Exit01", 0, False, 0, 1, "Dao: S House (out)"],
+            622: [623, 0, 0, 400, 406, "MapC3Exit06", 0, False, 0, 1, "Dao: SE House (in)"],
+            623: [622, 0, 0, 0, 0, "MapC9Exit01", 0, False, 0, 1, "Dao: SE House (out)"],
+
             # Pyramid
-            634: [635, 0, 0, 411, 415, "",            0, False, 10, 0, "Pyramid: Foyer N exit (204->205)" ], # Hieroglyph room, ALWAYS LINKED
-            635: [634, 0, 0,   0,   0, "",            0, False, 10, 0, "Pyramid: Hieroglyph room exit (205->204)" ], # Hieroglyph room, ALWAYS LINKED
-            636: [637, 0, 0, 413, 416, "MapCCExit02", 0, False, 10, 2, "Pyramid: Lower foyer door 1 (204->206)" ], # Foyer to Room 1 (Will ramps)
-            637: [636, 0, 0,   0,   0, "MapCEExit01", 0, False, 10, 2, "Pyramid: Room 1A (Will ramps) upper exit (206->204)" ],
-            638: [639, 0, 0, 417, 418, "MapCEExit02", 0, False, 10, 2, "Pyramid: Room 1A (Will ramps) lower exit (206->207)" ],
-            639: [638, 0, 0,   0,   0, "MapCFExit01", 0, False, 10, 2, "Pyramid: Room 1B (Will ramps) upper exit (207->206)" ],
-            640: [641, 0, 0, 419, 442, "MapCFExit02", 0, False, 10, 2, "Pyramid: Room 1B (Will ramps) lower exit (207->218)" ],
-            641: [640, 0, 0,   0,   0, "MapDAExit01", 0, False, 10, 2, "Pyramid: Hieroglyph 1 exit (218->207)" ],
-            642: [643, 0, 0, 413, 420, "MapCCExit03", 0, False, 10, 2, "Pyramid: Lower foyer door 2 (204->208)" ], # Foyer to Room 2 (breakable floors)
-            643: [642, 0, 0,   0,   0, "MapD0Exit01", 0, False, 10, 2, "Pyramid: Room 2A (breakable floors) upper exit (208->204)" ],
-            644: [645, 0, 0, 421, 422, "MapD0Exit02", 0, False, 10, 2, "Pyramid: Room 2A (breakable floors) lower exit (208->209)" ],
-            645: [644, 0, 0,   0,   0, "MapD1Exit01", 0, False, 10, 2, "Pyramid: Room 2B (breakable floors) upper exit (209->208)" ],
-            646: [647, 0, 0, 423, 443, "MapD1Exit02", 0, False, 10, 2, "Pyramid: Room 2B (breakable floors) lower exit (209->218)" ],
-            647: [646, 0, 0,   0,   0, "MapDAExit02", 0, False, 10, 2, "Pyramid: Hieroglyph 2 exit (218->209)" ],
-            648: [649, 0, 0, 413, 431, "MapCCExit04", 0, False, 10, 2, "Pyramid: Lower foyer door 3 (204->214)" ], # Foyer to Room 3 (Friar, Killer 6, Will chest)
-            649: [648, 0, 0,   0,   0, "MapD6Exit01", 0, False, 10, 2, "Pyramid: Room 3A (Friar+K6+Will chest) upper exit (214->204)" ],
-            650: [651, 0, 0, 434, 435, "MapD6Exit02", 0, False, 10, 2, "Pyramid: Room 3A (Friar+K6+Will chest) lower exit (214->215)" ],
-            651: [650, 0, 0,   0,   0, "MapD7Exit01", 0, False, 10, 2, "Pyramid: Room 3B (Friar+K6+Will chest) upper exit (215->214)" ],
-            652: [653, 0, 0, 450, 444, "MapD7Exit02", 0, False, 10, 2, "Pyramid: Room 3B (Friar+K6+Will chest) lower exit (215->218)" ],
-            653: [652, 0, 0,   0,   0, "MapDAExit05", 0, False, 10, 2, "Pyramid: Hieroglyph 3 exit (218->215)" ],
-            654: [655, 0, 0, 413, 436, "MapCCExit05", 0, False, 10, 2, "Pyramid: Lower foyer door 4 (204->216)" ], # Foyer to Room 4 (crushers, req. Spin Dash)
-            655: [654, 0, 0,   0,   0, "MapD8Exit01", 0, False, 10, 2, "Pyramid: Room 4A (crusher ceilings) upper exit (216->204)" ],
-            656: [657, 0, 0, 437, 438, "MapD8Exit02", 0, False, 10, 2, "Pyramid: Room 4A (crusher ceilings) lower exit (216->217)" ],
-            657: [656, 0, 0,   0,   0, "MapD9Exit01", 0, False, 10, 2, "Pyramid: Room 4B (crusher ceilings) W exit (217->216)" ],
-            658: [659, 0, 0, 439, 440, "MapD9Exit02", 0, False, 10, 2, "Pyramid: Room 4B (crusher ceilings) E exit (217->219)" ],
-            659: [658, 0, 0,   0,   0, "MapDBExit01", 0, False, 10, 2, "Pyramid: Room 4C (crusher ceilings) W exit (219->217)" ],
-            660: [661, 0, 0, 441, 445, "MapDBExit02", 0, False, 10, 2, "Pyramid: Room 4C (crusher ceilings) E door (219->218)" ],
-            661: [660, 0, 0,   0,   0, "MapDAExit06", 0, False, 10, 2, "Pyramid: Hieroglyph 4 exit (218->219)" ],
-            662: [663, 0, 0, 413, 426, "MapCCExit06", 0, False, 10, 2, "Pyramid: Lower foyer door 5 (204->212)" ], # Foyer to Room 5 (Quake/Aura one-way)
-            663: [662, 0, 0,   0,   0, "MapD4Exit01", 0, False, 10, 2, "Pyramid: Room 5A (Quake/Aura one-way) upper exit (212->204)" ],
-            664: [665, 0, 0, 429, 430, "MapD4Exit02", 0, False, 10, 2, "Pyramid: Room 5A (Quake/Aura one-way) lower exit (212->213)" ],
-            665: [664, 0, 0,   0,   0, "MapD5Exit01", 0, False, 10, 2, "Pyramid: Room 5B (Quake/Aura one-way) upper exit (213->212)" ],
-            666: [667, 0, 0, 430, 446, "MapD5Exit02", 0, False, 10, 2, "Pyramid: Room 5B (Quake/Aura one-way) lower exit (213->218)" ],
-            667: [666, 0, 0,   0,   0, "MapDAExit04", 0, False, 10, 2, "Pyramid: Hieroglyph 5 exit (218->213)" ],
-            668: [669, 0, 0, 413, 424, "MapCCExit07", 0, False, 10, 2, "Pyramid: Lower foyer door 6 (204->210)" ], # Foyer to Room 6 (mummies)
-            669: [668, 0, 0,   0,   0, "MapD2Exit01", 0, False, 10, 2, "Pyramid: Room 6A (mummy doors) upper exit (210->204)" ],
-            670: [671, 0, 0, 424, 425, "MapD2Exit02", 0, False, 10, 2, "Pyramid: Room 6A (mummy doors) lower exit (210->211)" ],
-            671: [670, 0, 0,   0,   0, "MapD3Exit01", 0, False, 10, 2, "Pyramid: Room 6B (mummy doors) upper exit (211->210)" ],
-            672: [673, 0, 0, 425, 447, "MapD3Exit02", 0, False, 10, 2, "Pyramid: Room 6B (mummy doors) lower exit (211->218)" ],
-            673: [672, 0, 0,   0,   0, "MapDAExit03", 0, False, 10, 2, "Pyramid: Hieroglyph 6 exit (218->211)" ],
-            
+            634: [635, 0, 0, 411, 415, "", 0, False, 10, 0, "Pyramid: Foyer N exit (204->205)"],
+            # Hieroglyph room, ALWAYS LINKED
+            635: [634, 0, 0, 0, 0, "", 0, False, 10, 0, "Pyramid: Hieroglyph room exit (205->204)"],
+            # Hieroglyph room, ALWAYS LINKED
+            636: [637, 0, 0, 413, 416, "MapCCExit02", 0, False, 10, 2, "Pyramid: Lower foyer door 1 (204->206)"],
+            # Foyer to Room 1 (Will ramps)
+            637: [636, 0, 0, 0, 0, "MapCEExit01", 0, False, 10, 2,
+                  "Pyramid: Room 1A (Will ramps) upper exit (206->204)"],
+            638: [639, 0, 0, 417, 418, "MapCEExit02", 0, False, 10, 2,
+                  "Pyramid: Room 1A (Will ramps) lower exit (206->207)"],
+            639: [638, 0, 0, 0, 0, "MapCFExit01", 0, False, 10, 2,
+                  "Pyramid: Room 1B (Will ramps) upper exit (207->206)"],
+            640: [641, 0, 0, 419, 442, "MapCFExit02", 0, False, 10, 2,
+                  "Pyramid: Room 1B (Will ramps) lower exit (207->218)"],
+            641: [640, 0, 0, 0, 0, "MapDAExit01", 0, False, 10, 2, "Pyramid: Hieroglyph 1 exit (218->207)"],
+            642: [643, 0, 0, 413, 420, "MapCCExit03", 0, False, 10, 2, "Pyramid: Lower foyer door 2 (204->208)"],
+            # Foyer to Room 2 (breakable floors)
+            643: [642, 0, 0, 0, 0, "MapD0Exit01", 0, False, 10, 2,
+                  "Pyramid: Room 2A (breakable floors) upper exit (208->204)"],
+            644: [645, 0, 0, 421, 422, "MapD0Exit02", 0, False, 10, 2,
+                  "Pyramid: Room 2A (breakable floors) lower exit (208->209)"],
+            645: [644, 0, 0, 0, 0, "MapD1Exit01", 0, False, 10, 2,
+                  "Pyramid: Room 2B (breakable floors) upper exit (209->208)"],
+            646: [647, 0, 0, 423, 443, "MapD1Exit02", 0, False, 10, 2,
+                  "Pyramid: Room 2B (breakable floors) lower exit (209->218)"],
+            647: [646, 0, 0, 0, 0, "MapDAExit02", 0, False, 10, 2, "Pyramid: Hieroglyph 2 exit (218->209)"],
+            648: [649, 0, 0, 413, 431, "MapCCExit04", 0, False, 10, 2, "Pyramid: Lower foyer door 3 (204->214)"],
+            # Foyer to Room 3 (Friar, Killer 6, Will chest)
+            649: [648, 0, 0, 0, 0, "MapD6Exit01", 0, False, 10, 2,
+                  "Pyramid: Room 3A (Friar+K6+Will chest) upper exit (214->204)"],
+            650: [651, 0, 0, 434, 435, "MapD6Exit02", 0, False, 10, 2,
+                  "Pyramid: Room 3A (Friar+K6+Will chest) lower exit (214->215)"],
+            651: [650, 0, 0, 0, 0, "MapD7Exit01", 0, False, 10, 2,
+                  "Pyramid: Room 3B (Friar+K6+Will chest) upper exit (215->214)"],
+            652: [653, 0, 0, 450, 444, "MapD7Exit02", 0, False, 10, 2,
+                  "Pyramid: Room 3B (Friar+K6+Will chest) lower exit (215->218)"],
+            653: [652, 0, 0, 0, 0, "MapDAExit05", 0, False, 10, 2, "Pyramid: Hieroglyph 3 exit (218->215)"],
+            654: [655, 0, 0, 413, 436, "MapCCExit05", 0, False, 10, 2, "Pyramid: Lower foyer door 4 (204->216)"],
+            # Foyer to Room 4 (crushers, req. Spin Dash)
+            655: [654, 0, 0, 0, 0, "MapD8Exit01", 0, False, 10, 2,
+                  "Pyramid: Room 4A (crusher ceilings) upper exit (216->204)"],
+            656: [657, 0, 0, 437, 438, "MapD8Exit02", 0, False, 10, 2,
+                  "Pyramid: Room 4A (crusher ceilings) lower exit (216->217)"],
+            657: [656, 0, 0, 0, 0, "MapD9Exit01", 0, False, 10, 2,
+                  "Pyramid: Room 4B (crusher ceilings) W exit (217->216)"],
+            658: [659, 0, 0, 439, 440, "MapD9Exit02", 0, False, 10, 2,
+                  "Pyramid: Room 4B (crusher ceilings) E exit (217->219)"],
+            659: [658, 0, 0, 0, 0, "MapDBExit01", 0, False, 10, 2,
+                  "Pyramid: Room 4C (crusher ceilings) W exit (219->217)"],
+            660: [661, 0, 0, 441, 445, "MapDBExit02", 0, False, 10, 2,
+                  "Pyramid: Room 4C (crusher ceilings) E door (219->218)"],
+            661: [660, 0, 0, 0, 0, "MapDAExit06", 0, False, 10, 2, "Pyramid: Hieroglyph 4 exit (218->219)"],
+            662: [663, 0, 0, 413, 426, "MapCCExit06", 0, False, 10, 2, "Pyramid: Lower foyer door 5 (204->212)"],
+            # Foyer to Room 5 (Quake/Aura one-way)
+            663: [662, 0, 0, 0, 0, "MapD4Exit01", 0, False, 10, 2,
+                  "Pyramid: Room 5A (Quake/Aura one-way) upper exit (212->204)"],
+            664: [665, 0, 0, 429, 430, "MapD4Exit02", 0, False, 10, 2,
+                  "Pyramid: Room 5A (Quake/Aura one-way) lower exit (212->213)"],
+            665: [664, 0, 0, 0, 0, "MapD5Exit01", 0, False, 10, 2,
+                  "Pyramid: Room 5B (Quake/Aura one-way) upper exit (213->212)"],
+            666: [667, 0, 0, 430, 446, "MapD5Exit02", 0, False, 10, 2,
+                  "Pyramid: Room 5B (Quake/Aura one-way) lower exit (213->218)"],
+            667: [666, 0, 0, 0, 0, "MapDAExit04", 0, False, 10, 2, "Pyramid: Hieroglyph 5 exit (218->213)"],
+            668: [669, 0, 0, 413, 424, "MapCCExit07", 0, False, 10, 2, "Pyramid: Lower foyer door 6 (204->210)"],
+            # Foyer to Room 6 (mummies)
+            669: [668, 0, 0, 0, 0, "MapD2Exit01", 0, False, 10, 2,
+                  "Pyramid: Room 6A (mummy doors) upper exit (210->204)"],
+            670: [671, 0, 0, 424, 425, "MapD2Exit02", 0, False, 10, 2,
+                  "Pyramid: Room 6A (mummy doors) lower exit (210->211)"],
+            671: [670, 0, 0, 0, 0, "MapD3Exit01", 0, False, 10, 2,
+                  "Pyramid: Room 6B (mummy doors) upper exit (211->210)"],
+            672: [673, 0, 0, 425, 447, "MapD3Exit02", 0, False, 10, 2,
+                  "Pyramid: Room 6B (mummy doors) lower exit (211->218)"],
+            673: [672, 0, 0, 0, 0, "MapDAExit03", 0, False, 10, 2, "Pyramid: Hieroglyph 6 exit (218->211)"],
+
             # Babel
-            682: [683, 0, 0, 460, 461, "MapDEExit01", 0, False, 11, 0, "Babel: Entry door in (222->223)" ],
-            683: [682, 0, 0,   0,   0, "MapDFExit01", 0, False, 11, 0, "Babel: Flute room SW exit (223->222)" ],
-            684: [685, 0, 0, 462, 463, "MapDFExit02", 0, False, 11, 0, "Babel: Flute room upper exit (223->224)" ],
-            685: [684, 0, 0,   0,   0, "MapE0Exit01", 0, False, 11, 0, "Babel: Castoth/Viper hall lower exit (224->223)" ],
-            686: [687, 0, 0, 463, 474, "",            0, False, 11, 0, "Babel: Castoth Door (224->242)" ],
-            687: [686, 0, 0,   0,   0, "",            0, False, 11, 0, "Babel: Return from Castoth (242->224)" ],
-            688: [689, 0, 0, 463, 475, "",            0, False, 11, 0, "Babel: Viper Door (224->243)" ],
-            689: [688, 0, 0,   0,   0, "",            0, False, 11, 0, "Babel: Return from Viper (243->224)" ],
-            690: [691, 0, 0, 463, 465, "MapE0Exit02", 0, False, 11, 0, "Babel: Castoth/Viper hall upper exit (224->225)" ],
-            691: [690, 0, 0,   0,   0, "MapE1Exit01", 0, False, 11, 0, "Babel: First elevator lower exit (225->224)" ],
-            692: [693, 0, 0, 466, 464, "MapE1Exit02", 0, False, 11, 0, "Babel: First elevator upper exit (225->224)" ],
-            693: [692, 0, 0,   0,   0, "MapE0Exit03", 0, False, 11, 0, "Babel: Vamps/Fanger hall lower exit (224->225)" ],
-            694: [695, 0, 0, 464, 476, "",            0, False, 11, 0, "Babel: Vampires Door (224->244)" ],
-            695: [694, 0, 0,   0,   0, "",            0, False, 11, 0, "Babel: Return from Vampires (244->224)" ],
-            696: [697, 0, 0, 464, 477, "",            0, False, 11, 0, "Babel: Fanger Door (224->245)" ],
-            697: [696, 0, 0,   0,   0, "",            0, False, 11, 0, "Babel: Return from Fanger (245->224)" ],
-            698: [699, 0, 0, 464, 469, "MapE0Exit04", 0, False, 11, 0, "Babel: Vamps/Fanger hall upper exit (224->226)" ],
-            699: [698, 0, 0,   0,   0, "MapE2Exit01", 0, False, 11, 0, "Babel: Exterior lower exit (226->224)" ],
-            #700: [701, 0, 0, 470, 471, "",           0, False, 11, 0, "Babel:  (226->227)" ], # Treated as a boss room exit, up there with the boss room exits
-            #701: [700, 0, 0,   0,   0, "",           0, False, 11, 0, "Babel:  (227->226)" ], # Treated as a boss room exit, up there with the boss room exits
-            702: [703, 0, 0, 471, 478, "",            0, False, 11, 0, "Babel: Mummy Queen door (227->246)" ],
-            703: [702, 0, 0,   0,   0, "",            0, False, 11, 0, "Babel: Return from Mummy Queen (246->227)" ],
-            704: [705, 0, 0, 471, 467, "",            0, False, 11, 0, "Babel: MQ hall upper exit (227->225)" ],
-            705: [704, 0, 0,   0,   0, "",            0, False, 11, 0, "Babel: Last elevator lower exit (225->227)" ],
-            706: [707, 0, 0, 468, 472, "",            0, False, 11, 0, "Babel: Last elevator upper exit (225->227)" ],
-            707: [706, 0, 0,   0,   0, "",            0, False, 11, 0, "Babel: End hall lower exit (227->225)" ],
-            708: [709, 0, 0, 472, 473, "",            0, False, 11, 0, "Babel: End hall upper exit (227->222)" ],
-            709: [708, 0, 0,   0,   0, "",            0, False, 11, 0, "Babel: Olman room exit (222->227)" ],
-            
+            682: [683, 0, 0, 460, 461, "MapDEExit01", 0, False, 11, 0, "Babel: Entry door in (222->223)"],
+            683: [682, 0, 0, 0, 0, "MapDFExit01", 0, False, 11, 0, "Babel: Flute room SW exit (223->222)"],
+            684: [685, 0, 0, 462, 463, "MapDFExit02", 0, False, 11, 0, "Babel: Flute room upper exit (223->224)"],
+            685: [684, 0, 0, 0, 0, "MapE0Exit01", 0, False, 11, 0, "Babel: Castoth/Viper hall lower exit (224->223)"],
+            686: [687, 0, 0, 463, 474, "", 0, False, 11, 0, "Babel: Castoth Door (224->242)"],
+            687: [686, 0, 0, 0, 0, "", 0, False, 11, 0, "Babel: Return from Castoth (242->224)"],
+            688: [689, 0, 0, 463, 475, "", 0, False, 11, 0, "Babel: Viper Door (224->243)"],
+            689: [688, 0, 0, 0, 0, "", 0, False, 11, 0, "Babel: Return from Viper (243->224)"],
+            690: [691, 0, 0, 463, 465, "MapE0Exit02", 0, False, 11, 0,
+                  "Babel: Castoth/Viper hall upper exit (224->225)"],
+            691: [690, 0, 0, 0, 0, "MapE1Exit01", 0, False, 11, 0, "Babel: First elevator lower exit (225->224)"],
+            692: [693, 0, 0, 466, 464, "MapE1Exit02", 0, False, 11, 0, "Babel: First elevator upper exit (225->224)"],
+            693: [692, 0, 0, 0, 0, "MapE0Exit03", 0, False, 11, 0, "Babel: Vamps/Fanger hall lower exit (224->225)"],
+            694: [695, 0, 0, 464, 476, "", 0, False, 11, 0, "Babel: Vampires Door (224->244)"],
+            695: [694, 0, 0, 0, 0, "", 0, False, 11, 0, "Babel: Return from Vampires (244->224)"],
+            696: [697, 0, 0, 464, 477, "", 0, False, 11, 0, "Babel: Fanger Door (224->245)"],
+            697: [696, 0, 0, 0, 0, "", 0, False, 11, 0, "Babel: Return from Fanger (245->224)"],
+            698: [699, 0, 0, 464, 469, "MapE0Exit04", 0, False, 11, 0,
+                  "Babel: Vamps/Fanger hall upper exit (224->226)"],
+            699: [698, 0, 0, 0, 0, "MapE2Exit01", 0, False, 11, 0, "Babel: Exterior lower exit (226->224)"],
+            # 700: [701, 0, 0, 470, 471, "",           0, False, 11, 0, "Babel:  (226->227)" ], # Treated as a boss room exit, up there with the boss room exits
+            # 701: [700, 0, 0,   0,   0, "",           0, False, 11, 0, "Babel:  (227->226)" ], # Treated as a boss room exit, up there with the boss room exits
+            702: [703, 0, 0, 471, 478, "", 0, False, 11, 0, "Babel: Mummy Queen door (227->246)"],
+            703: [702, 0, 0, 0, 0, "", 0, False, 11, 0, "Babel: Return from Mummy Queen (246->227)"],
+            704: [705, 0, 0, 471, 467, "", 0, False, 11, 0, "Babel: MQ hall upper exit (227->225)"],
+            705: [704, 0, 0, 0, 0, "", 0, False, 11, 0, "Babel: Last elevator lower exit (225->227)"],
+            706: [707, 0, 0, 468, 472, "", 0, False, 11, 0, "Babel: Last elevator upper exit (225->227)"],
+            707: [706, 0, 0, 0, 0, "", 0, False, 11, 0, "Babel: End hall lower exit (227->225)"],
+            708: [709, 0, 0, 472, 473, "", 0, False, 11, 0, "Babel: End hall upper exit (227->222)"],
+            709: [708, 0, 0, 0, 0, "", 0, False, 11, 0, "Babel: Olman room exit (222->227)"],
+
             # Jeweler's Mansion
-            720: [721, 0, 0,   8, 480, "MapMansionEntranceString", 0, False, 12, 1, "Mansion entrance" ],
-            721: [720, 0, 0, 480, 400, "MapMansionExitString",     0, False, 12, 1, "Mansion exit" ]
+            720: [721, 0, 0, 8, 480, "MapMansionEntranceString", 0, False, 12, 1, "Mansion entrance"],
+            721: [720, 0, 0, 480, 400, "MapMansionExitString", 0, False, 12, 1, "Mansion exit"]
         }
-        
+
         # Logic requirements for exits to be traversable. For more complex logic, manually create an artificial node.
         # During initialization, new nodes are created and entries are added to self.logic as needed.
         # If IsCoupled, the logic will be applied to the coupled exit too.
         # Format: { ID: [0: ExitId,
         #                1: [[item1, qty1],[item2,qty2],...],
         #                2: Direction (0 = to exit from node, 1 = from exit to node, 2 = both),
         #                3: IsCoupled
         #               ] }
         self.exit_logic = {
-            1:  [ 62,  [[701, 1]], 0, False ],   # Edward's first worm door
-            2:  [ 64,  [[702, 1]], 0, False ],   # Edward's second worm door
-            3:  [ 68,  [[703, 1]], 0, False ],   # Edward's bat door
-            4:  [ 70,  [[501, 1], [609, 1]], 0, False ],   # Edward's Lilly door requires Lilly and an attack
-            5:  [ 90,  [[608, 1]], 0, False ],   # Itory cave wall
-            6:  [ 152, [[8, 1], [611, 1]], 0, False ],     # Inca Golden Tile
-            7:  [ 126, [[524, 1]], 2, False ],   # Inca Diamond Block
-            52: [ 118, [[612, 1]], 0, False ],   # Inca statue puzzle requires pulling the statues
-            8:  [ 234, [[528, 1]], 0, False ],   # Mine tunnel wall
-            9:  [ 224, [[15, 1]], 0, False ],    # Mine elevator
-            50: [ 226, [[609, 1]], 0, False],    # Mine big room requires hitting buttons
-            10: [ 246, [[11, 1], [12, 1]], 0, False ],   # Mine end
-            51: [ 287, [[609, 1], [612, 1]], 0, False ], # Sky Garden to blue room requires moving the statue
-            11: [ 310, [[16, 1]], 0, True ],     # Sea Palace door
-            12: [ 354, [[511, 1]], 2, False ],    # Mu-NW door (Hope Room)
-            13: [ 362, [[512, 1]], 2, True ],    # Mu-NW/W exit (Bot)
-            14: [ 356, [[62, 1], [801, 1]], 0, True ],     # Mu-NW/W Slider hole, blocked for dungeon construction
-            15: [ 360, [[512, 1]], 2, True ],    # Mu-NE/E exit 1 (Bot)
-            16: [ 340, [[511, 1]], 2, True ],    # Mu-NE/E exit 2 (Mid)
-            17: [ 358, [[512, 1]], 2, True ],    # Mu-E/W exit 1 (Bot)
-            18: [ 342, [[511, 1]], 2, True ],    # Mu-E/W exit 2 (Mid)
-            19: [ 352, [[511, 1]], 2, True ],    # Mu-W/SW exit 1 (Mid)
-            20: [ 364, [[512, 1]], 2, True ],    # Mu-W/SW exit 2 (Bot)
-            21: [ 346, [[511, 1]], 2, True ],    # Mu-W/SW exit 3 (Mid)
-            22: [ 348, [[511, 1]], 2, True ],    # Mu-SW/SE exit 1 (Mid)
-            23: [ 366, [[512, 1]], 2, True ],    # Mu-SW/SE exit 2 (Bot)
-            24: [ 350, [[511, 1]], 2, True ],    # Mu-SW/SE exit 3 (Mid)
-            25: [ 368, [[512, 1]], 2, False ],   # Mu-SE exit door (Bot)
-            26: [ 408, [[62, 1]], 0, True ],     # Angl chest slider
-            27: [ 414, [[62, 1]], 0, True ],     # Angl Ishtar slider
-            28: [ 591, [] if settings.allow_glitches else [[28, 1]], 2, False],     # Wat bright room N
-            30: [ 592, [] if settings.allow_glitches else [[28, 1]], 2, False],     # Wat bright room S
+            1: [62, [[701, 1]], 0, False],  # Edward's first worm door
+            2: [64, [[702, 1]], 0, False],  # Edward's second worm door
+            3: [68, [[703, 1]], 0, False],  # Edward's bat door
+            4: [70, [[501, 1], [609, 1]], 0, False],  # Edward's Lilly door requires Lilly and an attack
+            5: [90, [[608, 1]], 0, False],  # Itory cave wall
+            6: [152, [[8, 1], [611, 1]], 0, False],  # Inca Golden Tile
+            7: [126, [[524, 1]], 2, False],  # Inca Diamond Block
+            52: [118, [[612, 1]], 0, False],  # Inca statue puzzle requires pulling the statues
+            8: [234, [[528, 1]], 0, False],  # Mine tunnel wall
+            9: [224, [[15, 1]], 0, False],  # Mine elevator
+            50: [226, [[609, 1]], 0, False],  # Mine big room requires hitting buttons
+            10: [246, [[11, 1], [12, 1]], 0, False],  # Mine end
+            51: [287, [[609, 1], [612, 1]], 0, False],  # Sky Garden to blue room requires moving the statue
+            11: [310, [[16, 1]], 0, True],  # Sea Palace door
+            12: [354, [[511, 1]], 2, False],  # Mu-NW door (Hope Room)
+            13: [362, [[512, 1]], 2, True],  # Mu-NW/W exit (Bot)
+            14: [356, [[62, 1], [801, 1]], 0, True],  # Mu-NW/W Slider hole, blocked for dungeon construction
+            15: [360, [[512, 1]], 2, True],  # Mu-NE/E exit 1 (Bot)
+            16: [340, [[511, 1]], 2, True],  # Mu-NE/E exit 2 (Mid)
+            17: [358, [[512, 1]], 2, True],  # Mu-E/W exit 1 (Bot)
+            18: [342, [[511, 1]], 2, True],  # Mu-E/W exit 2 (Mid)
+            19: [352, [[511, 1]], 2, True],  # Mu-W/SW exit 1 (Mid)
+            20: [364, [[512, 1]], 2, True],  # Mu-W/SW exit 2 (Bot)
+            21: [346, [[511, 1]], 2, True],  # Mu-W/SW exit 3 (Mid)
+            22: [348, [[511, 1]], 2, True],  # Mu-SW/SE exit 1 (Mid)
+            23: [366, [[512, 1]], 2, True],  # Mu-SW/SE exit 2 (Bot)
+            24: [350, [[511, 1]], 2, True],  # Mu-SW/SE exit 3 (Mid)
+            25: [368, [[512, 1]], 2, False],  # Mu-SE exit door (Bot)
+            26: [408, [[62, 1]], 0, True],  # Angl chest slider
+            27: [414, [[62, 1]], 0, True],  # Angl Ishtar slider
+            28: [591, [] if settings.allow_glitches else [[28, 1]], 2, False],  # Wat bright room N
+            30: [592, [] if settings.allow_glitches else [[28, 1]], 2, False],  # Wat bright room S
             # Require an attack for bosses; Castoth and Vamps are special
             # Rigorously we need a "defeated" flag item for each boss, but this suffices for now
-            101: [ 5, [[609, 1]], 2, False ],     # Viper
-            103: [ 11, [[609, 1]], 2, False ],    # Fanger
-            104: [ 14, [[36, 1]], 2, False ],     # MQ
-            106: [ 20, [[609, 1]], 2, False ]     # Solid Arm
+            101: [5, [[609, 1]], 2, False],  # Viper
+            103: [11, [[609, 1]], 2, False],  # Fanger
+            104: [14, [[36, 1]], 2, False],  # MQ
+            106: [20, [[609, 1]], 2, False]  # Solid Arm
         }
-
```

### Comparing `iog-randomizer-4.7.2.2/randomizer/iogr.asr` & `iog_randomizer-5.0.0/src/iog_randomizer/randomizer/iogr.asr`

 * *Files 2% similar despite different names*

```diff
@@ -690,16 +690,40 @@
 
 org $80f48f
 ; bank $80 free space begins here
 SR_RunIogrMapCode:
 lda #$09c4 : jsl LR_SecOnAnyFlagA : bcc .PostDsWarpCheck
   cop #$CF : dw $09c4
   cop #$9C : dl EDarkSpaceWarper : dw $2300
+  lda $0012,y : ora #$1000 : sta $0012,y   ; Make the warp ignore Earthquaker
   lda $0bf6 : sta $0026,y
 .PostDsWarpCheck:
+if !SettingInfiniteInventory == 1
+.StoreSmallInvTank:
+sep #$20
+phx
+ldx #$0000
+ldy #$0000
+..CheckSmallSlot:
+lda.w SramInvSmallHoldingTank,y : bne ..FindNextLargeSlot
+..NextSmallSlot:
+  iny : cpy #$0010 : bcc ..CheckSmallSlot
+    bra .DoneStoringSmallInvTank
+..FindNextLargeSlot:
+lda.l SramInvHoldingTank,x : beq ...GotSlot
+  inx : cpx #$0100 : bcs .DoneStoringSmallInvTank   ; if the big tank is full, I guess we have to give up
+  bra ..FindNextLargeSlot
+...GotSlot:
+lda.w SramInvSmallHoldingTank,y : sta.l SramInvHoldingTank,x
+lda #$00 : sta.w SramInvSmallHoldingTank,y
+bra ..NextSmallSlot
+.DoneStoringSmallInvTank:
+plx
+rep #$20
+endif
 if !SettingDebug == 1
 jsr SR_CameraUpdatesPositionHundreds
 endif
 rts
 
 
 SR_SecIfCameraFrozen:
@@ -2976,14 +3000,52 @@
 jsr SR_SetWillAbilitySpriteSetOnFlute
 org $82beea
 jsr SR_SetWillAbilitySpriteSetOnFlute
 org $82befa
 jsr SR_SetWillAbilitySpriteSetOnFlute
 org $82c0be
 jsr SR_SetWillAbilitySpriteSetOnFlute
+
+
+org $82c4dd
+EPlayer_ActPressDown:
+nop
+lda #$0000 : jsr SR_SecIfCanStartRunningInDirectionA : bcc $13
+;...
+org $82c514
+jsr SR_RunningConsiderReturnToActRepl
+
+
+org $82C524
+EPlayer_ActPressUp:
+nop : nop
+lda #$0001 : jsr SR_SecIfCanStartRunningInDirectionA : bcc $13
+;...
+org $82c55c
+jsr SR_RunningConsiderReturnToActRepl
+
+
+org $82C56C
+EPlayer_ActPressLeft:
+nop : nop : nop
+lda #$0002 : jsr SR_SecIfCanStartRunningInDirectionA : bcc $13
+;...
+org $82c5a5
+jsr SR_RunningConsiderReturnToActRepl
+
+
+org $82C5B5
+EPlayer_ActPressRight:
+nop : nop : nop : nop
+lda #$0003 : jsr SR_SecIfCanStartRunningInDirectionA : bcc $13
+;...
+org $82c5ef
+jsr SR_RunningConsiderReturnToActRepl
+
+
 org $82cc05
 jsr SR_SetWillAbilitySpriteSetOnFlute
 org $82cc58
 jsr SR_SetWillAbilitySpriteSetOnFlute
 
 
 org $82ca63
@@ -4265,14 +4327,142 @@
 +:
 rts
 
 SR_InvCleanupPointedItem:
 lda.l SramInvActivePageId : inc : sta $0bfa
 lda #$c040 : tsb $0658
 rts
+
+; In the base game, you run if you tap in the direction you're facing while $040c is non-negative.
+; $040c is non-negative only for ~12 frames after you tap any direction from a stationary position.
+; This routine extends the logic to allow running under some circumstances if the unused button is pressed.
+; Input is a proposed direction, 0/1/2/3 = S/N/W/E; player's facing direction should be in $24.
+SR_SecIfCanStartRunningInDirectionA:
+{
+sta $0000
+cmp $24 : beq .FacingInProposedDirection
+.NotFacingInProposedDirection:
+; If A-to-run is enabled, you can run in a non-blocked direction if you aren't pressing your facing direction.
+;lda $0bea : beq .ClcAndReturn
+lda $0656 : bit #$0080 : beq .ClcAndReturn
+lda $24 : beq ..FacingSouth
+  dec : beq ..FacingNorth
+  dec : beq ..FacingWest
+..FacingEast:
+lda #$0100
+bra ..CheckButtons
+..FacingSouth:
+lda #$0400
+bra ..CheckButtons
+..FacingNorth:
+lda #$0800
+bra ..CheckButtons
+..FacingWest:
+lda #$0200
+;bra ..CheckButtons
+..CheckButtons:
+bit $0656 : bne .ClcAndReturn
+lda $0000 : jsr .SR_SecIfDirectionAIsBlocked : bcs .ClcAndReturn
+bra .SecAndReturn
+.FacingInProposedDirection:
+lda $040c : bpl .SecAndReturn   ; Double-tapping a direction works.
+; If A-to-run is enabled, you can start running in the non-blocked direction you're facing.
+;lda $0bea : beq .ClcAndReturn
+lda $0656 : bit #$0080 : beq .ClcAndReturn
+lda $09ae : bit #$1000 : bne .ClcAndReturn   ; no running up ramps
+lda $24 : jsr .SR_SecIfDirectionAIsBlocked : bcs .ClcAndReturn
+;bra .SecAndReturn
+.SecAndReturn:
+sec
+rts
+.ClcAndReturn:
+clc
+rts
+.SR_SecIfDirectionAIsBlocked:
+pha
+lda $1014 : lsr : lsr : lsr : lsr : sta $0018
+lda $1016 : sec : sbc #$0008 : lsr : lsr : lsr : lsr : sta $001c
+pla : beq ..FacingSouth
+  dec : beq ..FacingNorth
+  dec : beq ..FacingWest
+..FacingEast:
+inc $0018
+bra ..CheckBlocked
+..FacingSouth:
+inc $001c
+bra ..CheckBlocked
+..FacingNorth:
+dec $001c
+bra ..CheckBlocked
+..FacingWest:
+dec $0018
+;bra ..CheckBlocked
+..CheckBlocked:
+phd
+lda #$0000 : tcd
+jsl $83d78a    ; = jsl LR_GetTileTableIndex83
+pld
+sep #$20
+phx
+  tyx
+  lda $7fc000,x
+plx
+  bit #$f0 : beq +
+    lsr : lsr : lsr : lsr   ; Use the current effective type, if any
++:
+  cmp #$02 : bcc ..NotBlocked  ; Nonsolid and semisolid never block.
+  cmp #$0e : bcs ..IsBlocked   ; Solids always block.
+  cmp #$0c : beq ...RampNorth
+  cmp #$0a : beq ...RampEast
+  cmp #$05 : beq ...RampWest
+  cmp #$03 : beq ...RampSouth
+  cmp #$02 : beq ..IsBlocked   ; Ladder
+  cmp #$07 : beq ..IsBlocked   ; Sideling wall
+  cmp #$08 : beq ..IsBlocked   ; Dropdown ledge
+bra ..NotBlocked
+...RampNorth:
+lda $24 : beq ..IsBlocked
+bra ..NotBlocked
+...RampEast:
+lda $24 : cmp #$02 : beq ..IsBlocked
+bra ..NotBlocked
+...RampWest:
+lda $24 : cmp #$03 : beq ..IsBlocked
+bra ..NotBlocked
+...RampSouth:
+lda $24 : dec : beq ..IsBlocked
+;bra ..NotBlocked
+..NotBlocked:
+rep #$20
+clc
+rts
+..IsBlocked:
+rep #$20
+sec
+rts
+}
+
+SR_RunningConsiderReturnToActRepl:
+cop #$40 : dw $8000, .DoReturn
+lda $09b2 : ora $09b4 : bne .DoReturn
+lda $0656 : bit #$0080 : beq .NoReturn
+lda $09ae : bit #$1000 : bne .NoReturn
+; With A-to-run and A pressed, should ParseAct occasionally to e.g. start running from a walk.
+lda $2a : cmp #$0004 : bcc .NoReturn
+lda $24 : cmp #$0002 : bcs .NoReturn
+bra .DoReturn
+.NoReturn:
+lda $09ae : bit #$1000
+rts
+.DoReturn:
+pla
+cop #$C5
+
+
+
 }
 
 
 
 ; Bank $83
 {
 
@@ -4383,15 +4573,23 @@
 jsr SR_SecIfCanPlayMusic : db $90   ; i.e. jsr ... : bcc ..., replacing lda $0ad4 : bne ...
 
 
 org $838BA4
 SR_UseItemLolasMelody:
 {
 jsr SR_SecIfCanPlayMusic : bcc .NoFlute
-lda $0644 : cmp #$0015 : bne .NothingHappened
+lda $0644 : cmp #$0015 : beq .InItory
+  cmp #$0011 : bne .NothingHappened
+.InEdwardsFlowerRoom:
+cop #$BF : dw ..Text
+rts
+..Text:
+db $d3
+db $cd : dl TextLongLolasMelodyInEdwards
+db $c0
 .InItory:
 cop #$D0 : db $40, $01 : dw .NothingHappened
 .DoPlaySong:
 lda #$0080 : tsb $09EC
 cop #$BF : dw TextLayDownDatFunkCat
 phx
 ldx #$0000
@@ -4664,21 +4862,20 @@
 ;skip 4
 ;db !HieroItemTile5
 ;skip 4
 ;db !HieroItemTile6
 
 
 org $839CDC    ; In SR_UseItemAura, this is the not-Shadow branch.
-cop #$BF : dw TextShadowsFormUnlocked
-cop #$CC : db $b4
+cop #$BF : dw TextYouCantUseAura
 rts
-TextShadowsFormUnlocked:
+TextYouCantUseAura:
 table "table_dialogue.txt",rtl
 db $d3
-db $cd : dl TextLongShadowsFormUnlocked
+db $cd : dl TextLongYouCantUseAura
 db $c0
 
 warnpc $839d09
 org $839d09
 ; End of Lola's Letter use code.
 {
 cop #$CC : db $11
@@ -5887,15 +6084,15 @@
 cop #$0F : db $0e,$11
 cop #$0F : db $0f,$11
 cop #$9C : dl ECDoorOpeningListener : dw $2000
 lda #$0800 : trb $10
 .DoorAlreadyOpen:
 cop #$D0 : db $23,$01 : dw .Die ; $d2d6
 .SpawnHamlet:
-cop #$C2
+cop #$DA : db $04
 lda #$1000 : tsb $10
 lda #$2000 : trb $10
 cop #$BF : dw $d4a5
 cop #$86 : db $27,$06,$02
 cop #$8A
 cop #$85 : db $29,$02,$01
 cop #$8A
@@ -5942,16 +6139,28 @@
 db $00 : dw $3000
 EItoryEntranceHandler:
 cop #$45 : db $20,$30,$40,$40 : dw .PlayerInArea
 cop #$E0
 .PlayerInArea:
 cop #$C1
 cop #$D0 : db $40,$01 : dw .DoEnterItory
-cop #$40 : dw $0f01 : dw .TryLeaveItory
+cop #$45 : db $2d,$37,$2e,$38 : dw .DoNothing
+.LeaveItory:
+cop #$BF : dw .TextYouNeedLolasMelody
+cop #$66 : dw $00c0,$02c0 : db !OverworldShuffleItryMenuId
+cop #$C1
+.DoNothing:
 rtl
+.TextYouNeedLolasMelody:
+db $d3
+db "(Looks like you'll",$cb
+db "need to find and use",$cb
+db "a certain item to",$cb
+db "enter the town...)"
+db $c0
 .DoEnterItory:
 lda #$1000 : tsb $10
 lda #$eff0 : tsb $065a
 lda #$0380 : sta $2130
 cop #$3C : dl $80b7ce
 cop #$DA : db $af
 cop #$CC : db $01
@@ -5996,22 +6205,16 @@
 cop #$BF : dw $e53c
 lda #$0800 : tsb $10
 cop #$86 : db $1f,$02,$12
 cop #$8A
 cop #$86 : db $1f,$04,$12
 cop #$8A
 cop #$E0
-.TryLeaveItory:
-cop #$45 : db $2c,$36,$2f,$39 : dw ..DoNothing
-cop #$66 : dw $00c0,$02c0 : db !OverworldShuffleItryMenuId
-cop #$C1
-..DoNothing:
-rtl
 }
-
+warnpc $84e5a1
 
 
 org $84e5a1
 db $1c : dw $1000
 ELillyInItory:
 cop #$D0 : db $6f,$01 : dw .Die
 cop #$0B
@@ -7172,42 +7375,46 @@
 db $d3
 db "!SpoilerTextIshtarsApprentice"
 db $c0
 
 org $86dcd8
 ; Bank $86 free space begins here.
 
-TextItemCounterDisplay:
 ; Item collection tracker in map room.
 {
+TextItemCounterDisplay:
 table "table_dialogue.txt",rtl
 db $D3
-db "_Items Collected:_"
+db "__Item Checks:_"
 db $C6 : dw $0002, $00f0
 db "/"
 db $C6 : dw $0002, $00f2
 db $CB
 if !SettingOrbRando > 0
-db "__Orbs Collected:_"
+db "_Monster Orbs:_"
 db $C6 : dw $0002, $00f4
 db "/"
 db $C6 : dw $0002, $00f6
 db $CB
 endif
-db "_____Dark Spaces:_"
+db "__Dark Spaces:_"
 db $C6 : dw $0002, $00f8
+db "/"
+db $C6 : dw $0002, $00fa
 db $C0
 
 ; Format is:
 ; db <flags with high byte $00: normal items>
 ; db $ff
 ; db <flags with high byte $02: chests are $01-$2E, RJs are $80-$8f>
 ; db $ff
 ; db <monster orb numbers, $01 - $2A>
 ; db $ff
+; db <DS indices; at time of writing these are offsets from flag $09a0>
+db $ff
 Lut_TrackerItemFlagsByArea:
 .Pointers:
 {
 dw .Cape
 dw .EdDg
 dw .Itry
 dw .Moon
@@ -7233,168 +7440,183 @@
 {
 .Cape:
 db $35,$d7
 db $ff
 db $80,$81
 db $ff
 db $ff
+db $00
+db $ff
 .EdDg:
 db $23,$46,$d8
 db $ff
 db $01,$02,$03,$82
 db $ff
 db $01,$02,$03,$04,$05,$06,$07
 db $ff
+db $01,$02
+db $ff
 .Itry:
 db $2d
 db $ff
 db $83
 db $ff
 db $ff
+db $03
+db $ff
 .Moon:
 db $48
 db $ff
 db $ff
 db $ff
+db $ff
 .Inca:
 db $32,$e0
 db $ff
 db $04,$05,$06,$07
 db $ff
 db $08,$09,$0a,$0b,$0c,$0d,$0e
 db $ff
+db $04,$05,$06
+db $ff
 .Coast:
 db $ff
 db $84
 db $ff
 db $ff
+db $ff
 .Frej:
 db $53,$54,$5a,$e1
 db $ff
 db $85
 db $ff
 db $ff
+db $07
+db $ff
 .Mine:
 db $5d,$5e,$a2,$a3,$d9
 db $ff
 db $09
 db $ff
 db $0f,$10,$11,$12,$13,$14
 db $ff
+db $08,$09,$0a
+db $ff
 .Neil:
 db $ff
 db $ff
 db $ff
+db $ff
 .SkGn:
 db $ff
 db $0a,$0b,$0c,$0d,$0e,$0f,$10,$11
 db $ff
 db $15,$16,$17,$18,$19,$1a
 db $ff
+db $0b,$0c,$0d,$0e
+db $ff
 .SeaP:
 db $13,$85
 db $ff
 db $12,$13,$14
 db $ff
 db $ff
+db $0f
+db $ff
 .Mu:
 db $79,$7f
 db $ff
 db $15,$16,$17,$18,$2e
 db $ff
 db $1b,$1c,$1d,$1e,$1f,$20
 db $ff
+db $10,$11
+db $ff
 .Angl:
 db $ff
 db $19,$1a,$1b,$1c,$86,$87
 db $ff
 db $ff
+db $12
+db $ff
 .Wtma:
 db $e2,$95
 db $ff
 db $88,$89
 db $ff
 db $ff
+db $13
+db $ff
 .GtWl:
 db $98,$99
 db $ff
 db $1d,$1e
 db $ff
 db $21
 db $ff
+db $14,$15,$16
+db $ff
 .Euro:
 db $9a,$a6,$e5,$f0,$f1
 db $ff
 db $8a,$8b
 db $ff
 db $ff
+db $17
+db $ff
 .Kres:
 db $ff
 db $1f,$20,$21,$22,$23
 db $ff
 db $23
 db $ff
+db $18,$19,$1a
+db $ff
 .NtVl:
 db $e6
 db $ff
 db $8c
 db $ff
 db $ff
+db $1b
+db $ff
 .Ankr:
 db $ba,$be
 db $ff
 db $24,$25,$26,$27,$28
 db $ff
 db $24,$25,$27
 db $ff
+db $1c,$1d,$1e
+db $ff
 .Dao:
 db $b8,$b8,$e7
 db $ff
 db $8d
 db $ff
 db $ff
+db $1f
+db $ff
 .Pymd:
 db $bd,$c2,$c3,$c4,$c5,$c6,$c7
 db $ff
 db $29,$2a,$2b,$2c,$8e
 db $ff
 db $28
 db $ff
+db $20,$21
+db $ff
 .Babl:
 db $dc
 db $ff
 db $8f
 db $ff
 db $ff
-}
-
-TblTrackerDarkSpaceCountsByArea:
-{
-db $01   ; South Cape
-db $02   ; Edward's
-db $01   ; Itory
-db $00   ; Moon Tribe
-db $03   ; Inca
-db $00   ; Coast
-db $01   ; Freejia
-db $03   ; Mine
-db $00   ; Neil's
-db $04   ; SkGn
-db $01   ; SeaP
-db $02   ; Mu
-db $01   ; Angl
-db $01   ; Wtma
-db $03   ; GtWl
-db $01   ; Euro
-db $03   ; Kres
-db $01   ; NtVl
-db $03   ; Ankr
-db $01   ; Dao
-db $02   ; Pymd
-db $02   ; Babl
+db $22,$23
+db $ff
 }
 
 db $00 : dw $3000
 EInGameCollectionTracker:
 stz $26
 cop #$45 : db $0C,$39,$0E,$3B : dw .InSomeArea
 inc $26
@@ -7442,37 +7664,36 @@
 .OutsideAreasClearFlags:
 cop #$CE : db $02
 .DoNothing:
 rtl
 .InSomeArea:
 cop #$D0 : db $02,$01 : dw .DoNothing
 cop #$CC : db $02
-stz $00f0
-stz $00f2
-stz $00f4
-stz $00f6
-stz $00f8
+stz $00f0   ; Collected items
+stz $00f2   ; Total items
+stz $00f4   ; Collected orbs
+stz $00f6   ; Total orbs
+stz $00f8   ; Visited Dark Spaces
+stz $00fa   ; Total Dark Spaces
 phx
-lda $26 : tax
-lda.l TblTrackerDarkSpaceCountsByArea,x : and #$00ff : sta $00f8
 lda $26 : asl : tax
 lda.l Lut_TrackerItemFlagsByArea,x : tax
 .CountNextLowFlag:
 lda.l Lut_TrackerItemFlagsByArea&$ff0000,x : and #$00ff : cmp #$00ff : beq ..DoneCountingLowFlags
 jsl LR_SecOnAnyFlagA : bcc ..PostCollectionCheck
   jsr SR_IncrementCollectedItems
 ..PostCollectionCheck:
 jsr SR_IncrementTotalItems
 inx
 bra .CountNextLowFlag
 ..DoneCountingLowFlags:
 inx
 .CountNextHighFlag:
 lda.l Lut_TrackerItemFlagsByArea&$ff0000,x : and #$00ff : cmp #$00ff : beq ..DoneCountingHighFlags
-lda.l Lut_TrackerItemFlagsByArea&$ff0000,x : jsl LR_SecOnFlag20A : bcc ..PostCollectionCheck
+jsl LR_SecOnFlag20A : bcc ..PostCollectionCheck
   jsr SR_IncrementCollectedItems
 ..PostCollectionCheck:
 jsr SR_IncrementTotalItems
 inx
 bra .CountNextHighFlag
 ..DoneCountingHighFlags:
 inx
@@ -7485,14 +7706,28 @@
 ..PostCollectionCheck:
 sed
   lda $00f6 : clc : adc #$0001 : sta $00f6
 cld
 inx
 bra .CountNextOrbFlag
 ..DoneCountingOrbFlags:
+inx
+.CountNextDarkSpace:
+lda.l Lut_TrackerItemFlagsByArea&$ff0000,x : and #$00ff : cmp #$00ff : beq ..DoneCountingDarkSpaces
+clc : adc #$09a0 : jsl LR_SecOnAnyFlagA : bcc ..PostCollectionCheck
+sed
+  lda $00f8 : clc : adc #$0001 : sta $00f8
+cld
+..PostCollectionCheck:
+sed
+  lda $00fa : clc : adc #$0001 : sta $00fa
+cld
+inx
+bra .CountNextDarkSpace
+..DoneCountingDarkSpaces:
 plx
 cop #$BF : dw TextItemCounterDisplay
 rtl
 
 SR_IncrementCollectedItems:
 sed
   lda $00f0 : clc : adc #$0001 : sta $00f0
@@ -7518,17 +7753,17 @@
 and #$ff00 : xba : lsr : clc : asl : asl : asl
 rts
 
 SR_SecIfThisIshtarRoomHasWind:
 phx
 lda $1016 : cmp #$0100 : bcs .NoWind
 lda $1014 : jsr SR_GetIshtarRoomAddrOffsetForXPos : tax
-lda.l 0+Config_IshtarRoomDifferencesAnchor,x : beq .MaybeHasWind
+lda.l 4+Config_IshtarRoomDifferencesAnchor,x : beq .MaybeHasWind
 lda.l 2+Config_IshtarRoomDifferencesAnchor,x : beq .HasWind
-lda.l 4+Config_IshtarRoomDifferencesAnchor,x : beq .HasWind
+lda.l 0+Config_IshtarRoomDifferencesAnchor,x : beq .HasWind
 .NoWind:
 plx
 clc
 rts
 .MaybeHasWind:
 ; Room difference is wind, so right room has wind, unless it's room 3 and the chests are different
 lda $1014 : and #$0100 : beq .NoWind
@@ -7631,76 +7866,76 @@
 rep #$20
 txa : clc : adc #$0100 : tax
 sep #$20
 cpx #$0600 : bcc -
 rep #$20
 ; Then draw indexed differences on the tilemaps
 lda #$0000 : tcd
-lda #$0000 : pha   ; $01,s = whether we've drawn Index1 for this room
-lda #$0000 : pha   ; $01,s = room index (0,1,2,3); $03,s = is this Index > 1
+lda #$0002 : pha   ; $01,s = difference index less 1 (=2,1,0; 0 = DifferenceIndex1 is drawn last to ensure its effect isn't overwritten)
+lda #$0000 : pha   ; $01,s = room index (0,1,2,3); $03,s = DifferenceIndex
 .DrawNextRoom:
 lda $01,s : asl : tax
-lda.l .TablePointers,x : pha   ; $01,s = #.TableRoomN; $03,s = room index; $05,s = is this difference index > 1
+lda.l .TablePointers,x : pha   ; $01,s = #.TableRoomN; $03,s = room index; $05,s = DifferenceIndex
 lda $03,s : asl : xba : clc : adc #$0080 : jsr SR_GetIshtarRoomAddrOffsetForXPos : tax
-phx   ; $01,s = base offset from DifferencesAnchor for this room; $03,s = #.TableRoomN; $05,s = room index; $07,s = is this difference index > 1
-.DrawNextDiff:   ; Here X = $01,s should be DifferenceIndexM - DifferencesAnchor; $03,s = #.TableRoomN; $05,s = room index; $07,s = is M>1.
-..CheckRoom3Special:
-lda $05,s : cmp #$0002 : bne ..CheckDifferenceIndex
-lda $07,s : bne ..CheckDifferenceIndex
-jsr SR_SecIfIshtarChestsAreDifferent : bcs ..SkipDifferenceIndex
-..CheckDifferenceIndex:
-lda.l Config_IshtarRoomDifferencesAnchor,x : bmi .PrepNextRoom
-  bne ..GotGoodDifferenceIndex
+phx   ; $01,s = base offset from DifferencesAnchor for this room; $03,s = #.TableRoomN; $05,s = room index; $07,s = DifferenceIndex
+.MaybeDrawNextDifferenceIndex:   ; Here X = $01,s should be DifferenceIndexM - DifferencesAnchor; $03,s = #.TableRoomN; $05,s = room index; $07,s = DifferenceIndex.
+lda $07,s : bpl +
+  jmp .PrepNextRoom              ; All DifferenceIndexes have been drawn or skipped
++:
+lda.l Config_IshtarRoomDifferencesAnchor,x
+  bmi ..SkipDifferenceIndex      ; $FFFF is skipped
+  beq ..SkipDifferenceIndex      ; Wind is skipped, being handled elsewhere because it's not a tile draw
+lda $05,s : cmp #$0002 : bne ..UseDifferenceIndex    ; Room 3 (only) skips index 1 (only), if the chests are different
+lda $07,s : bne ..UseDifferenceIndex
+jsr SR_SecIfIshtarChestsAreDifferent : bcc ..UseDifferenceIndex
 ..SkipDifferenceIndex:
-    inx : inx
-    lda #$0001 : sta $07,s
-    bra .DrawNextDiff   ; Skip the diff if it's 0 (wind, handled elsewhere), or if it's the first diff in room 3 and the difference is supposed to be chest contents
-..GotGoodDifferenceIndex:
-  asl : clc : adc $03,s : tax   ; X = #.TableRoomN + 2 * DifferenceIndex
+  jmp .PrepNextDiff
+..UseDifferenceIndex:
+lda.l Config_IshtarRoomDifferencesAnchor,x : asl : clc : adc $03,s : tax   ; X = #.TableRoomN + 2 * DifferenceIndex
 lda.l $ff0000&SR_DrawIshtarMapDifferences,x : tax   ; X = #.TableRoomN_IndexM
 ..DrawNextTile:
 lda.l $ff0000&SR_DrawIshtarMapDifferences,x : and #$00ff : cmp #$00ff : beq .PrepNextDiff
   sta $18
 inx
 lda.l $ff0000&SR_DrawIshtarMapDifferences,x : and #$00ff : sta $1c
 inx
-lda.l $ff0000&SR_DrawIshtarMapDifferences,x : and #$00ff : pha   ; note this pha temporarily shifts the stack
+lda.l $ff0000&SR_DrawIshtarMapDifferences,x : and #$00ff : pha   ; the stack shifts for a few lines here
 inx
 lda $07,s : asl : xba : lsr : lsr : lsr : lsr : clc : adc $18 : sta $18
 phx   ; X = addr of next line of #.TableRoomN_IndexM
 ldx #$0000
 jsl $82B0A3   ; = jsl LR_GetTileTableIndex82; returns index in X
 ply   ; Y = addr of next line of #.TableRoomN_IndexM
-pla   ; A = tile type to draw
+pla   ; A = tile type to draw; the stack is back to normal now
 sep #$20
   sta $7ea100,x   ; Update MapLayer
   phx
     tax
     lda $7f0000,x
   plx
   sta $7fc100,x   ; Update CollisionLayer
   lda $07,s : beq +
-    lda $7ea100,x : sta $7ea000,x   ; DifferenceIndexes after 1 are drawn in both sides of the room
+    lda $7ea100,x : sta $7ea000,x   ; DifferenceIndexes above 1 are drawn in both sides of the room
     lda $7fc100,x : sta $7fc000,x
 +:
 rep #$20
 tyx
 bra ..DrawNextTile
 .PrepNextRoom:
-lda #$0000 : sta $07,s   ; Next DifferenceIndex will be 1
+lda #$0002 : sta $07,s   ; Next DifferenceIndex will be 3 again
 pla   ; Discard the DifferenceIndexM offset for this room
 pla   ; Discard #.TableRoomN
 pla : inc : cmp #$0004 : bcs .Done
   pha   ; Update room index
 jmp .DrawNextRoom
 .PrepNextDiff:
-lda #$0001 : sta $07,s   ; Next DifferenceIndex will be >1
-lda $01,s : inc : inc : sta $01,s   ; Advance to next difference for this room
+lda $01,s : inc : inc : sta $01,s   ; Advance the difference pointer
   tax
-jmp .DrawNextDiff
+lda $07,s : dec : sta $07,s   ; "Advance" the DifferenceIndex identifier
+jmp .MaybeDrawNextDifferenceIndex
 .Done:
 pla   ; Discard whether M>1
 plx   ; Restore ActorID
 txa : tcd
 rts
 
 .TablePointers:
@@ -7961,14 +8196,20 @@
 }
 
 org $879c81
 db $d3
 db "!SpoilerTextKarasJournal"
 db $c0
 
+org $879fb9
+jsl LR_WatermiaLeafCheckPlayerPosition
+
+org $879fe9
+jsl LR_WatermiaLeafCheckPlayerPosition
+
 org $87a871
 db $e0,$6b    ; Disable Lilly in Watermia
 
 org $87ad1b
 nop : nop : nop : nop   ; "cop #$BF : dw $...." Skip Lance's speech.
 %MTryGiveItemAndFlag("WtrmLanceItem", $e2)
 rtl
@@ -8260,15 +8501,18 @@
 EuroSecretGotItemAlready:
 cop #$BF : dw Text_EuroSecretGotItemAlready
 rtl
 Text_EuroSecretGotItemAlready:
 db $d3,$d6,$63,$86,$8e,$2a,$c0
 }
 
+
 org $87e927
+; Bank $87 free space begins here.
+
 SethWatermiaOnInteract:
 cop #$D0 : db $11,$01 : dw .CanTravel
 .NoTravel:
 cop #$BF : dw .TextNoTravel
 rtl
 .CanTravel:
 cop #$D0 : db $12,$01 : dw .OfferTravel
@@ -8286,14 +8530,31 @@
 .TextFirstTravel:
 db $d3
 db "Oh, you know Bagu? Then",$cb
 db "I can help you cross.",$cb
 db "(And by Bagu I mean",$cb
 db "Morse Code.)",$c0
 
+
+; Replaces the routine at $87a018. Forces the leaf to always wait for the player.
+LR_WatermiaLeafCheckPlayerPosition:
+stz $0000
+lda $1016 : cmp #$0100 : rol $0000   ; Now $0000 is 1 if player is in the south part of the map.
+lda $16 : cmp #$0100 : rol : and #$0001 : cmp $0000 : bne .DoMoveNow
+.AwaitPlayer:
+lda $26 : cmp #$0002 : beq .DoMoveNow
+phb
+pla
+pla
+rtl
+.DoMoveNow:
+lda $26
+jmp $a020
+
+
 }
 
 
 
 ; Bank $88
 {
 
@@ -9534,18 +9795,32 @@
 ; Speed up Babel rooftop sequence
 cop #$CC : db $0e
 cop #$CC : db $0f
 cop #$CE : db $F4
 rtl
 
 ; Speed up Babel warp/elevator sequences
-org $8995a9
-db $01,$00
-org $8995b0
-db $01,$00
+org $8995a7
+cop #$DB : dw $0002
+cop #$CC : db $00
+cop #$DB : dw $0002
+cop #$CC : db $01
+if !SettingDungeonShuffle > 0
+cop #$9C : dl EPymdPortalToFoyer_EVanishingPlayerSprite : dw $1002
+else
+cop #$9C : dl $88B6F4 : dw $1002   ; This is the normal address for this object. Dungeon Shuffle moves it.
+endif
+
+org $8995f6
+if !SettingDungeonShuffle > 0
+cop #$9C : dl EPymdPortalToFoyer_EVanishingPlayerSprite : dw $1002
+else
+cop #$9C : dl $88B6F4 : dw $1002   ; This is the normal address for this object. Dungeon Shuffle moves it.
+endif
+
 org $8996ab
 db $03
 org $8996fd
 db $10
 org $89982a
 db $10
 org $899848
@@ -10159,18 +10434,29 @@
 db $03    ; 4 difficulty levels available
 
 ; Upon starting a new game, set IOGR flags.
 org $8be515
 jsl LR_WarpToStart
 jmp EIogrGameInitFlagSetter
 
-org $8be6a6
-nop : nop : nop : nop : nop : nop    ; Disable code that disables X button.
-org $8be6b3
-nop : nop : nop : nop : nop : nop    ; Disable other code that disables X button.
+; To support button mappings, IOG stores a dynamic bitmask for each SNES button, and the mask determines functionality;
+; so e.g. mask #$8000 represents the Attack button, and whichever SNES button sets that mask is thus the Attack button.
+; The "default" (actually Style 2) mappings are the same as the SNES hardware bitmasks, except that X is ignored.
+; Oddly, in Style 1 the "unused" button (A or Y) has the same bitmask as the hardware X button.
+; Here we remove the code that disables the X button, and fix the "unused" button mapping in Style 1.
+org $8be695
+#SR_SetControlStyle:
+lda $0B26 : bne .Style2
+.Style1:
+  lda #$8000 : sta $0DAC    ; Remap A ($0dac) to action of #$8000 = Attack
+  lda #$4000 : sta $0DAA    ; Remap B ($0daa) to action of #$4000 = Cancel
+  lda #$0080 : sta $0DAE    ; Remap Y ($0dae) to action of #$0080 = unused
+rts
+.Style2:
+rts
 
 ; 4 difficulty levels available on the other menu too
 org $8be7b5
 db $03
 org $8be855
 db $04
 
@@ -10343,18 +10629,60 @@
 ; No text for second save file (unnecessary?)
 db $ca
 org $8bf511
 ; No text for third save file (unnecessary?)
 db $ca
 endif
 
-org $8bf5d2
-db "Level"    ; Change "Sound" to "Level"
-org $8bf55a
-db "Level"    ; --- and on the other menu too
+org $8bf538
+Bg3_MenuChangeDiarySettings:
+db $C1 : db $06,$08
+db $C7 : db $0A,$08
+db $CC : db $02
+db "_____*Settings*",$cb
+db ">Done",$cb
+db "Level:",$cb
+db "Control Style:",$cb
+db $CC,$0d
+db "Attack/Talk",$cb
+db $CC,$0d
+db "Item/Cancel",$cb
+db $CC,$0d
+db "Item Screen",$cb
+db $CC,$0d
+db "Run"
+db $CA
+warnpc $8bf5ad
+org $8bf5ad
+Bg3_MenuNewDiarySettings:
+db $C1 : db $06,$08
+db $C7 : db $0A,$08
+db "____*Game Setup*",$cb
+db ">Start Game",$cb
+db "Level:",$cb
+db "Control Style:",$cb
+db $CC,$0d
+db "Attack/Talk",$cb
+db $CC,$0d
+db "Item/Cancel",$cb
+db $CC,$0d
+db "Item Screen",$cb
+db $CC,$0d
+db "Run"
+db $CA
+warnpc $8bf625
+
+org $8bf630
+Bg3_MenuBranchControlOptions:
+db $c1 : db $14,$0e
+db $d2 : db $00
+db $c5 : dw $f63b, $0d8e
+db $ca
+warnpc $8bf63b
+
 org $8bf667    ; Pointers to level name texts
 dw TextDifficultyLevel0
 dw TextDifficultyLevel1
 dw TextDifficultyLevel2
 dw TextDifficultyLevel3
 
 org $8bf8c4
@@ -10486,14 +10814,15 @@
 stz $0bfc   ; Default to fast item-get text speed.
 lda #$2800 : trb $09ae
 jsl LR_MarkRoomRewardsObtainedByDifficulty
 lda.l Config_SettingFluteOpt : bne +
   cop #$CC : db $13   ; Set "has Flute" flag if starting with flute
 +:
 if !SettingInfiniteInventory == 1
+cop #$CD : dw $09d0   ; tracker flag
 ldx #$0000
 lda #$0000
 -:
 sta $306400,x
 inx : inx : cpx #$0400 : bcc -
 tdc : tax
 endif
@@ -11380,14 +11709,27 @@
 db $06
 db $01 : db $02,$08, $02,$10 : dw $0006
 db $01 : db $00,$08, $0C,$1C : dw $0160 
 db $01 : db $08,$00, $0C,$18 : dw $0161 
 db $00 : db $04,$0E, $1B,$09 : dw $006E 
 db $00 : db $0A,$08, $1B,$09 : dw $006F 
 db $01 : db $03,$07, $1C,$00 : dw $000E 
+
+
+org $8fc000
+; AnimList for transformations.
+dw $c160   ; Replace W->S #1 (slow) with W->F #1 (fast)
+skip 2
+skip 2
+skip 2
+skip 2
+skip 2
+dw $c5e4   ; Replace F->W #1 (slow) with F->S #1 (fast)
+
+
 org $8fcf65   ; Overwriting an unused 8-tile metasprite
 MetaWillFlutelessFlute2:
 db $08,$10 : db $24,$08 
 db $F8,$F0 : db $01,$01 
 db $F8,$10 : db $F0,$10 
 db $06
 db $01 : db $02,$08, $03,$10 : dw $0046 ; Head
```

### Comparing `iog-randomizer-4.7.2.2/randomizer/iogr_81_exit_table.asr` & `iog_randomizer-5.0.0/src/iog_randomizer/randomizer/iogr_81_exit_table.asr`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.2/randomizer/iogr_8C_actor_table.asr` & `iog_randomizer-5.0.0/src/iog_randomizer/randomizer/iogr_8C_actor_table.asr`

 * *Files 0% similar despite different names*

```diff
@@ -1714,14 +1714,15 @@
 db $25,$3B,!Monster018DParam : dl !Monster018DAddr : db !Monster018DStats,$00,!Monster018DItemFlag
 db $27,$3A,!Monster018EParam : dl !Monster018EAddr : db !Monster018EStats,$00,!Monster018EItemFlag
 db $2A,$3C,!Monster018FParam : dl !Monster018FAddr : db !Monster018FStats,$00,!Monster018FItemFlag
 db $2B,$3A,!Monster0190Param : dl !Monster0190Addr : db !Monster0190Stats,$00,!Monster0190ItemFlag
 db $30,$3A,!Monster0191Param : dl !Monster0191Addr : db !Monster0191Stats,$00,!Monster0191ItemFlag
 db $32,$3C,!Monster0192Param : dl !Monster0192Addr : db !Monster0192Stats,$00,!Monster0192ItemFlag
 db $00,$00,$00 : dl EMonsterRespawner-3 : db $00
+db $00,$00,$00 : dl ESeaPalNpcFixer-3 : db $00
 db $FF,$CA 
 
 ActorList_Map5D:
 db $05,$0A,$02 : dl $82C38C : db $00
 db $00,$00,$00 : dl $80EAED : db $00
 db $11,$11,$00 : dl $80EA96 : db $00
 db $00,$01,$00 : dl $8693F8 : db $00
```

### Comparing `iog-randomizer-4.7.2.2/randomizer/iogr_8D_asset_table.asr` & `iog_randomizer-5.0.0/src/iog_randomizer/randomizer/iogr_8D_asset_table.asr`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.2/randomizer/iogr_asset_ledger.asr` & `iog_randomizer-5.0.0/src/iog_randomizer/randomizer/iogr_asset_ledger.asr`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.2/randomizer/iogr_code_overflow.asr` & `iog_randomizer-5.0.0/src/iog_randomizer/randomizer/iogr_code_overflow.asr`

 * *Files 1% similar despite different names*

```diff
@@ -8,22 +8,25 @@
 ; $0bf0 = number of stacked Mushroom Drops
 ; $0bf2 = number of stacked Crystal Balls
 ; $0bf4 = number of stacked Red Jewels
 ; $0bf6 = stores index of last DS visited
 ; $0bf8 = during DS warp, DS index of text lines and of selected DS
 ; $0bfa = used for text branches ("FORCE" text, inv page number, count spacing, Lance's letter, etc.)
 ; $0bfc = used during item pickup to write text slowly (for chests and Dark Spaces)
-; $0bfe = used during item pickup to flag a stat as maxed out
+; $0bfe = used by Z3 to flag a stat as maxed out
+; $0dc0-$0dff = used by infinite inventory
 ; $1ffc = Player X pos in debug mode
 ; $1ffe = Player Y pos in debug mode
 ; Reserved flags (in addition to base game):
-; $022f - $0247 : Monster item flags $01 - $18
-; $0290 - $02af : Monster item flags $19 - $2A, and 13 extras
+; $022f - $0247 : Monster item flags $01 - $19
+; $0290 - $02af : Monster item flags $1A - $2A, and some extras
 ; $02b0 - $02b1 : Statue placed in the Left/Right Hope Room
 ; $02b2 - $02b7 : DS item-get flags
+; $09a0 - $09c4 : DS visited flags
+; $09d0         : infinite inventory setting is in use
 
 
 LR_SecOnAnyFlagA:
 jsl $80b4ba    ; i.e. 3+LR_SecOnFlagA
 rtl
 LR_SetAnyFlagA:
 jsl $80b4c1    ; i.e. 3+LR_SetFlagA
@@ -169,15 +172,15 @@
 dw $02a0 : dl Config_MansionWestGateItem
 dw $ffff
 endif
 
 ; Silently gives item A, stacking if appropriate.
 LR_GiveNormalItemA8OrSec:
 {
-stz $0bfe    ; Used by Z3 mode to flag whether we're capped on a stat.
+stz $0bfe   ; whether a Z3 stat is maxed out
 php
 sep #$20
 bit #$80 : bne .IsStatOrPickup
 cmp #$32 : beq .IsOtherWorldItem
 pha
 jsl LR_GetItemAStackedCountBcd : cmp #$00 : bne .IsStackableAndHasStack
 jsl LR_GetEmptyInvSlotInYOrSec : bcs +
@@ -268,15 +271,15 @@
 plx
 bcs +
   asl $0ade
   bra ++
 ..MaxStrByDifficulty:
 db 8,4,2,1
 +:
-lda #$01 : sta $0bfe
+lda #$01 : sta $0bfe   ; stat maxed out
 ++:
 else
 inc $0ADE
 endif
 ldy #$0000
 bra .ClcAndReturn
 .IsDefJewelItem:
@@ -289,15 +292,15 @@
 plx
 bcs +
   inc $0adc
   bra ++
 ..MaxDefByDifficulty:
 db 2,2,1,0
 +:
-lda #$01 : sta $0bfe
+lda #$01 : sta $0bfe   ; stat maxed out
 ++:
 else
 inc $0ADC
 endif
 ldy #$0000
 bra .ClcAndReturn
 
@@ -315,14 +318,15 @@
 pla : jsl LR_WriteItemAToInvSlotY
 endif
   sta $0DB8
   stz $0DB9
 ldy #$FF1F
 .ClcAndReturn:
 plp
+jsr SR_SetDataForItem
 clc
 rtl
 .InvFull:
 pla : sta $0DB8
   stz $0DB9
 ldy #$FF02
 plp
@@ -346,34 +350,31 @@
   clc : adc #$0029
 +:
 sta $0db8
 lda $01,s : and #$00ff : cmp #$0087 : bcs ..IsSpecial
 ..IsNotSpecial:
 lda $01,s : and #$00ff : jsl LR_GiveNormalItemA8OrSec : bcs ..InvFull
 ..GotItem:
-cop #$BF : dw ...Text
+jsr SR_SetTextForItem
+cop #$BF : dw .TextMaybeGotItem
 stz $0db8
 stz $0bfc
+stz $0bfe
 pla
 clc
 rtl
-...Text:
-db $cd : dl .TextItsAnItem
-db $c0
 ..InvFull:
-cop #$BF : dw ...Text
+lda #$0001 : sta $0bfa   ; your inv full
+cop #$BF : dw .TextMaybeGotItem
 stz $0db8
 stz $0bfc
+stz $0bfe
 pla
 sec
 rtl
-...Text:
-db $cd : dl .TextItsAnItem
-db "But your inventory's full!"
-db $c0
 ..IsSpecial:    ; Handling for upgrades, duplicate stat items, and Heart Pieces.
 lda $01,s : cmp #$008a : bcs ..IsNotStatUpgrade
 ..IsStatUpgrade:
 jsl LR_GiveNormalItemA8OrSec
 bra ..GotItem
 ..IsNotStatUpgrade:
 cmp #$008a : beq ...LightUpgrade
@@ -431,37 +432,64 @@
 cop #$BF : dw ..Text
 clc
 rtl
 ..Text:
 db $cd : dl .TextAbilityCanNowBeUsed
 db $ca   ; not $c0 here, because we're clumsily including a $c0 upstream
 
+.TextMaybeGotItem:
+db $cd : dl .TextItsAnItem
+db $cb
+db $c5 : dw TextItemGetExtraLine, $0bfa
+db $c0
+
 .TextItsAnItem:
 db $d3
 db $c5 : dw TextItemGetSpeeds, $0bfc
 db $d6,$1d    ; "It's "
 db $c5 : dw TextItemGetArticles, $0db8
 db $c5 : dw TextItemGetNames, $0db8
-db "!",$cb
-db $c5 : dw TextZ3UpgradeMaybeMaxedOut, $0bfe
-db $cb
+db "!"
 db $ca
 .TextItsADoor:
 db $d3
 db $d5,$00
 db "Opened a door!",$cb
 db $c5 : dw TextDoorNames, $0db8
 db $ca
 .TextAbilityCanNowBeUsed:
 db $d3
 db $c5 : dw TextItemGetSpeeds, $0bfc
 db $cd : dl TextItemGetAbilityCanBeUsedIncl
 db $ca
+}
 
+; Set flags etc. as appropriate for the item. Hopefully move some of the above code into here later.
+SR_SetDataForItem:
+{
+lda $0db8 : cmp #$0024 : beq .GotAura
+rts
+.GotAura:
+cop #$CC : db $b4
+rts
+}
 
+; Text is separate from data, so we don't clobber $0bfa by e.g. receiving a MW item while opening Lance's letter.
+SR_SetTextForItem:
+{
+lda $0bfe : bne .GotMaxedOutZ3Stat
+lda $0db8 : cmp #$0024 : beq .GotAura
+stz $0bfa    ; No extra line if no special case is known
+rts
+.GotMaxedOutZ3Stat:
+lda #$0002 : sta $0bfa   ; ope, you get nothing
+rts
+.GotAura:
+lda #$0003 : sta $0bfa   ; congrats, you got shadow
+rts
 }
 
 TextItemGetNames:
 .Pointers:
 {
 dw .Null
 dw .RedJewel
@@ -1417,23 +1445,31 @@
 .Fast:
 db $d5,$00
 db $ca
 .Slow:
 db $d5,$09
 db $ca
 
-TextZ3UpgradeMaybeMaxedOut:
+TextItemGetExtraLine:
 .Pointers:
-dw .NotMaxedOut
-dw .IsMaxedOut
-.NotMaxedOut:
+dw .NoExtraLine
+dw .YourInvFull
+dw .Z3StatIsMaxedOut
+dw .ShadowsFormUnlocked
+.NoExtraLine:
 db $ca
-.IsMaxedOut:
+.YourInvFull:
+db "But your inventory's full!"
+db $ca
+.Z3StatIsMaxedOut:
 db "But you're maxed out!"
 db $ca
+.ShadowsFormUnlocked:
+db "Shadow's form unlocked!"
+db $ca
 
 TextJewelerInvLineBegin:
 db $cd : dl 0+SramTextBuffer   ; Target shall contain a 2-byte color setting followed by $ca
 db $ca
 
 TextJewelerInvItemPaddedAssumingSram:
 db $cd : dl TextJewelerInvLineBegin
@@ -1485,14 +1521,15 @@
 bra .Done
 .TwoDigitNumber:
 lda #$0002 : sta.l 6+SramTextBuffer
 .Done:
 rtl
 
 LR_SetupAndDrawJewelerInvLineA:   ; A = 1-7
+{
 pha
 jsl LR_PrepSramTextBufferForJewelerLineA
 pla : cmp #$0007 : bcs .IsLine7
 dec : bne +
   lda.l Config_Jeweler1Item
   bra .IsItemLine
 +:
@@ -1557,14 +1594,15 @@
 db $c0
 .TextNormalItem:
 db $cd : dl TextJewelerInvItemPaddedAssumingSram
 db $ca
 .TextSpecialItem:
 db $cd : dl TextJewelerInvSpecialPaddedAssumingSram
 db $ca
+}
 
 macro MIncBcd8(addr)
 lda <addr> : clc : adc.b #1 : sta <addr>
 endmacro
 SR_GrowStackForItemA:
 {
 php
@@ -1706,14 +1744,15 @@
 plp
 cmp #$0000   ; to set/clear z
 clc
 rtl
 }
 
 LR_GetEmptyInvSlotInYOrSec:
+{
 php
 sep #$20
 ldy #$0000
 if !SettingInfiniteInventory == 1
 phb
 lda #$30 : pha : plb
 .CheckInvSlotEmpty:
@@ -1736,14 +1775,15 @@
 plp
 clc
 rtl
 .InvFull:
 plp
 sec
 rtl
+}
 
 LR_WriteItemAToInvSlotY:
 php
 sep #$20
 if !SettingInfiniteInventory == 1
 phx
   phy
@@ -1853,53 +1893,67 @@
 ; Silently gives all items in the holding tank.
 LR_GiveQueuedItems:
 phx
 lda #$0000 : tax : tay
 pha
 .NextItem:
 lda.l SramInvHoldingTank,x : and #$00ff : beq ..Given
-  tay
+  phx
+    tay
+      lda $05,s : tax   ; i.e. restore .X = ActorID
+    tya
+    jsl LR_GiveNormalItemA8OrSec : bcs ..FailedToGiveItem
+  plx
   sep #$20
     lda #$00 : sta.l SramInvHoldingTank,x
   rep #$20
-  lda $03,s : tax
-  tya
-  jsl LR_GiveNormalItemA8OrSec
 ..Given:
 pla : inc : cmp #$0100 : bcs .Done
   tax
   pha
   bra .NextItem
+..FailedToGiveItem:   ; something's probably horribly wrong if we get here, but we can handle it
+plx
+pla
 .Done:
 plx
 rtl
 
-; Called during Gaia game save. After a reset, permanent SRAM will be restored as it is at this point.
+; Called during Gaia game save. After a reset, permanent "SRAM" will be restored as it is at this point.
 LR_HardenSram:
 phx
 ldx #$0000
 -:
-lda.l SramStartPermanentData,x : sta.l SramHardened,x
+lda.l SramStartPermanentDataA,x : sta.l SramHardened,x
+inx : inx
+cpx.w #(SramEndPermanentDataA-SramStartPermanentDataA) : bcc -
+ldx #$0000
+-:
+lda.l SramStartPermanentDataB,x : sta.l SramHardened+(SramEndPermanentDataA-SramStartPermanentDataA),x
 inx : inx
-cpx.w #(SramEndPermanentData-SramStartPermanentData) : bcc -
-lda #$0001 : sta.l SramHardened,x   ; Artificial, indicates that there's saved data here
+cpx.w #(SramEndPermanentDataB-SramStartPermanentDataB) : bcc -
+lda #$0001 : sta.l SramHardenedDataMarker   ; Artificial, indicates that there's saved data
 plx
 rtl
 
-; Restores the save file as usual, along with hardened SRAM.
+; Restores the save file as usual, along with hardened "SRAM".
 LR_RestoreSaveFileWithInfiniteInventoryOrSec:
 phx
 jsl $83D954 : bcs .SecAndReturn   ; Normal routine accepts save file ID in A; sets carry if file is blank.
-ldx.w #(SramEndPermanentData-SramStartPermanentData)
-lda.l SramHardened,x : cmp #$0001 : bne .ClcAndReturn
+lda.l SramHardenedDataMarker : cmp #$0001 : bne .ClcAndReturn
+ldx #$0000
+-:
+lda.l SramHardened,x : sta.l SramStartPermanentDataA,x
+inx : inx
+cpx.w #(SramEndPermanentDataA-SramStartPermanentDataA) : bcc -
 ldx #$0000
 -:
-lda.l SramHardened,x : sta.l SramStartPermanentData,x
+lda.l SramHardened+(SramEndPermanentDataA-SramStartPermanentDataA),x : sta.l SramStartPermanentDataB,x
 inx : inx
-cpx.w #2+SramEndPermanentData-SramStartPermanentData : bcc -
+cpx.w #(SramEndPermanentDataB-SramStartPermanentDataB) : bcc -
 .ClcAndReturn:
 plx
 jsl LR_UpdateItemViewFull
 clc
 rtl
 .SecAndReturn:
 plx
@@ -2193,14 +2247,33 @@
   cop #$9C : dl EDarkRoomSpotlightManager : dw $3000
 +:
 endif
 if !SettingInfiniteInventory == 1
 jsl LR_GiveQueuedItems
 jsl LR_UpdateItemViewFull
 endif
+.SetupRng:
+lda $0644 : cmp #$008a : beq ..Fanger
+  cmp #$00f5 : beq ..Fanger
+  cmp #$00dd : beq ..MummyQueen
+  cmp #$00f6 : beq ..MummyQueen
+  cmp #$00e7 : beq ..FlightToComet
+bra ..Done
+..Fanger:
+lda #$0000
+bra ..DoSetRng
+..MummyQueen:
+lda #$0001
+bra ..DoSetRng
+..FlightToComet:
+lda #$0002
+;bra ..DoSetRng
+..DoSetRng:
+jsl LR_SetGameRngIndexA
+..Done:
 lda #$1000 : tsb $12
 rtl
 
 LR_SecIfThisMapIsDark:
 if !SettingDarkRoomsLevel == 4
 ; All rooms are dark other than hardcoded exceptions.
 phx
@@ -2431,15 +2504,14 @@
 rtl
 
 
 
 ; Spawn this and set its $26 to the target DS index from TableDsMapSpawnData.
 EDarkSpaceWarper:
 {
-lda #$1000 : tsb $12   ; Ignore Earthquaker
 lda #$fff0 : tsb $065a
 lda $1010 : ora #$2000 : sta $1010
 cop #$08 : db $0C, $0C
 lda $1014 : sta $14
 lda $1016 : sta $16
 lda #$2000 : trb $10
 cop #$88 : dl $8ee000
@@ -2714,14 +2786,15 @@
 %MDsWarpTargetMenuForIds(32,33)
 ..ChooseBabel:
 %MDsWarpTargetMenuForIds(34,35)
 
 EDsWarpMenuChoseGoodLoc:
 cop #$BF : dw TextDsWarpClearScreen
 cop #$9C : dl EDarkSpaceWarper : dw $2000
+lda $0012,y : ora #$1000 : sta $0012,y   ; Make the warp ignore Earthquaker
 lda $0bf8 : sta $0026,y
   sta $0bf6
 cop #$C1
 rtl
 
 TextDsWarpClearScreen:
 db $ce
@@ -3032,14 +3105,26 @@
 db $ca
 .TextClear:
 db $c8
 db $ca
 }
 
 
+db $00 : dw $2000
+ESeaPalNpcFixer:
+cop #$D0 : db $70,$00 : dw .Die
+cop #$C2
+lda #$0101 : sta $7fc384
+  sta $7fc386
+  sta $7fc388
+  sta $7fc389
+rtl
+.Die:
+cop #$E0
+
 
 LR_DebugSubActor:
 {
 lda $09AA : tcd : tax
 cop #$BF : dw .OptionText
 cop #$BE : db $63,$01 : dw .OptionList
 .OptionList:
@@ -3541,11 +3626,32 @@
 rtl
 .SecAndReturn:
 lda #$0000
 plx
 sec
 rtl
 
+LR_SetGameRngIndexA:
+{
+; Seeds the RNG from the IOGR hash string, accepting A=0-5 for variations.
+; Unsure whether I want to round $0036 to a multiple of 2 as well.
+phx
+tax
+lda.l Config_RandoTitleScreenHashString-1,x
+ldy #$0000
+-:
+sta $0410,y
+iny : iny
+cpy #$0010 : bcc -
+;lda $0036 : lsr : bcc +
+;  inc $0036
+;+:
+plx
+rtl
+}
+
+
+
```

### Comparing `iog-randomizer-4.7.2.2/randomizer/iogr_dialogue_overflow.asr` & `iog_randomizer-5.0.0/src/iog_randomizer/randomizer/iogr_dialogue_overflow.asr`

 * *Files 1% similar despite different names*

```diff
@@ -184,14 +184,26 @@
 
 TextEdwardJailedPerson:
 db "Please... tell",$cb
 db "SmashManiac I'm waiting",$cb
 db "for him..."
 db $ca
 
+TextLongLolasMelodyInEdwards:
+db "(You softly play",$cb
+db "Lola's Melody...)"
+db $cf
+db "(But nothing happens.)"
+db $cf
+db "(Seems like Lilly's",$cb
+db "not here. You'll have",$cb
+db "to go recruit her and",$cb
+db "come back here later.)"
+db $c0
+
 
 TextGiveLillyNecklace:
 db "Lilly: Oh, you found my",$cb
 db "necklace! Thank you so",$cb
 db "much!"
 db $CF
 db $CE
@@ -253,16 +265,18 @@
 db "Mummy Queen!",$ca
 ..MQ2:
 db "Mummy Queen 2.0!",$ca
 ..SolidArm:
 db "Solid Arm!",$ca
 
 
-TextLongShadowsFormUnlocked:
-db "Shadow's form unlocked!"
+TextLongYouCantUseAura:
+db "Only Shadow can use",$cb
+db "this. You'll find him",$cb
+db "in Dark Spaces!"
 db $ca
 
 
 TextUsedRedJewelRJM:
 db $d3
 db "As the Jewel disappears,",$cb
 db "Will feels his strength",$cb
```

### Comparing `iog-randomizer-4.7.2.2/randomizer/iogr_exit_ledger.asr` & `iog_randomizer-5.0.0/src/iog_randomizer/randomizer/iogr_exit_ledger.asr`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.2/randomizer/iogr_misc_defines.asr` & `iog_randomizer-5.0.0/src/iog_randomizer/randomizer/iogr_misc_defines.asr`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 EPlayer_DoAuraBarrier = $82b97f
 EPlayer_DoPsychoDash = $82bea0
 EPlayer_DoSpinDash = $82c0a9
 LR_ParseDialogueScriptAtY = $82f048
 LR_PlaceSelfBetween04And06 = $8aa41c
 }
 
-
 ; Dark rooms
 {
 !IsMap00Dark ?= 0
 !IsMap01Dark ?= 0
 !IsMap02Dark ?= 0
 !IsMap03Dark ?= 0
 !IsMap04Dark ?= 0
@@ -444,38 +443,47 @@
 }
 
 
 ; SRAM, including infinite inventory and Multiworld
 {
 !SettingInfiniteInventory ?= 0
 
-org $306002
-SramTextBuffer:    ; For drawing complex dynamic text
-skip 100
-
-SramDarkSpaceSeenFormFlags:   ; 2 "flags" per each of 36 DSes for if Will or not-Will has been seen nearby
-skip 9
-
-warnpc $306200
-
-org $306400
-SramStartPermanentData:   ; Data between here and End will be saved by Gaia and restored after a reset
-SramInvHoldingTank:   ; Items from other worlds; MW writing directly to the inventory is unsafe
-skip $100
+org $7e0dc0
+SramStartPermanentDataA:   ; Data between here and End will be saved by Gaia and restored after a reset
 SramInvActivePageId:  ; ID of the current active inventory page
 skip 2
 SramInvItems:         ; Aliased start of the item list, which begins immediately with the top line
 SramInvTopLine:       ; First four inventory slots, which aren't paginated
 skip 4
 SramInvPages:         ; Inventory pages, 12 bytes each
 skip 12
 skip 12
 skip 12
 SramInvEndOfList:     ; End of item list
+skip 2                ; Reserved for future use
+skip 2                ; Reserved for future use
+skip 2                ; Reserved for future use
+SramInvSmallHoldingTank:   ; Items from other worlds, small WRAM buffer
+skip 16
+SramEndPermanentDataA:   ; End of data that should be considered part of the game and saved/restored
+warnpc $7e0e00
+
+
+org $306002
+SramTextBuffer:    ; For drawing complex dynamic text
+skip $100
+SramHardenedDataMarker:
+skip 2                  ; The value here will be nonzero and non-#$FFFF if there's hardened data
+warnpc $306200
+
+
+org $306400
+SramStartPermanentDataB:   ; Data between here and End will be saved by Gaia and restored after a reset
+SramInvHoldingTank:   ; Items from other worlds; MW writing directly to the inventory is unsafe
+skip $100
+SramEndPermanentDataB:   ; End of data that should be considered part of the game and saved/restored
 
-warnpc $3065fe
-org $3065fe
-SramEndPermanentData:   ; End of all data that should be considered part of the game and saved/restored
-skip 2                  ; The value here will be nonzero and non-#$FFFF if there's saved data
+warnpc $306600
+org $306600
 SramHardened:    ; Contents of SRAM inventory at last save, for restoring from a reset or crash
 
 }
```

### Comparing `iog-randomizer-4.7.2.2/randomizer/iogr_monster_defaults.asr` & `iog_randomizer-5.0.0/src/iog_randomizer/randomizer/iogr_monster_defaults.asr`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.2/randomizer/iogr_rom.py` & `iog_randomizer-5.0.0/src/iog_randomizer/randomizer/iogr_rom.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,25 @@
-import binascii, hashlib, logging, os, random, tempfile, json, copy, sys
-from typing import BinaryIO
+import copy
+import hashlib
+import json
+import logging
+import os
+import random
+import sys
 
-from .patch import Patch
+from . import asar
 from .classes import World
-#from .quintet_comp import compress as qt_compress
-from .quintet_text import encode as qt_encode
-from .errors import FileNotFoundError, OffsetError
-from .models.randomizer_data import RandomizerData
-#from .models.enums.difficulty import Difficulty
-#from .models.enums.goal import Goal
-#from .models.enums.statue_req import StatueReq
-#from .models.enums.logic import Logic
-#from .models.enums.entrance_shuffle import EntranceShuffle
-#from .models.enums.dungeon_shuffle import DungeonShuffle
-#from .models.enums.orb_rando import OrbRando
-#from .models.enums.darkrooms import DarkRooms
-#from .models.enums.enemizer import Enemizer
-#from .models.enums.flute import FluteOpt
-#from .models.enums.start_location import StartLocation
+from .errors import OffsetError
 from .models.enums import *
+from .models.randomizer_data import RandomizerData
 
-from . import asar
-
-VERSION = "4.7.2.2"
+VERSION = "5.0.0"
 MAX_RANDO_RETRIES = 50
-OUTPUT_FOLDER: str = os.path.dirname(os.path.realpath(__file__)) + os.path.sep + ".." + os.path.sep + ".." + os.path.sep + "data" + os.path.sep + "output" + os.path.sep
+OUTPUT_FOLDER: str = os.path.dirname(os.path.realpath(
+    __file__)) + os.path.sep + ".." + os.path.sep + ".." + os.path.sep + "data" + os.path.sep + "output" + os.path.sep
 
 
 def generate_filename(settings: RandomizerData, extension: str):
     def getDifficulty(difficulty):
         if difficulty.value == Difficulty.EASY.value:
             return "_E"
         if difficulty.value == Difficulty.NORMAL.value:
@@ -76,22 +67,15 @@
         if overworld_shuffle:
             affix += "W"
         if town_shuffle:
             affix += "T"
         if dungeon_shuffle:
             affix += "D"
         return affix
-    
-    #def getOrbRando(orb_rando):
-    #    if orb_rando.value == OrbRando.BASIC.value:
-    #        return "_oB"
-    #    if orb_rando.value == OrbRando.ORBSANITY.value:
-    #        return "_oX"
-    #    return ""
-    
+
     def getDarkRooms(darkrooms):
         if abs(darkrooms.value) == DarkRooms.NONE.value:
             return ""
         if abs(darkrooms.value) == DarkRooms.FEW.value:
             affix = "_drF"
         if abs(darkrooms.value) == DarkRooms.SOME.value:
             affix = "_drS"
@@ -124,15 +108,15 @@
         if enemizer.value == Enemizer.FULL.value:
             affix += "F"
         if enemizer.value == Enemizer.INSANE.value:
             affix += "I"
         if boss_shuffle:
             affix += "-B"
         return affix
-    
+
     def getFluteOpt(flute):
         if flute.value == FluteOpt.SHUFFLE.value:
             return "-fs"
         if flute.value == FluteOpt.FLUTELESS.value:
             return "-fl"
         return ""
 
@@ -143,18 +127,20 @@
 
     filename = "IoGR" + VERSION
     filename += getDifficulty(settings.difficulty)
     filename += getLogic(settings.logic)
     filename += getGoal(settings.goal, settings.statues, settings.statue_req)
     filename += getStartingLocation(settings.start_location)
     filename += getEnemizer(settings.enemizer, settings.boss_shuffle)
-    filename += getEntranceShuffle(settings.coupled_exits, settings.town_shuffle, settings.dungeon_shuffle, settings.overworld_shuffle)
+    filename += getEntranceShuffle(settings.coupled_exits, settings.town_shuffle, settings.dungeon_shuffle,
+                                   settings.overworld_shuffle)
     filename += getSwitch(settings.orb_rando, "_oX")
     filename += getDarkRooms(settings.darkrooms)
-    if (settings.open_mode or settings.firebird or settings.ohko or settings.z3 or settings.allow_glitches or settings.flute.value > 0 or settings.infinite_inventory or settings.red_jewel_madness):
+    if (
+            settings.open_mode or settings.firebird or settings.ohko or settings.z3 or settings.allow_glitches or settings.flute.value > 0 or settings.infinite_inventory or settings.red_jewel_madness):
         filename += "_v"
         filename += getSwitch(settings.open_mode, "o")
         filename += getSwitch(settings.firebird, "f")
         filename += getSwitch(settings.allow_glitches, "g")
         filename += getSwitch(settings.ohko, "1")
         filename += getSwitch(settings.z3, "z")
         filename += getSwitch(settings.infinite_inventory, "i")
@@ -175,64 +161,65 @@
         self.rom_path = rom_path
         self.output_folder = os.path.dirname(rom_path) + os.path.sep + "iogr" + os.path.sep
 
         data_file = open(self.rom_path, "rb")
         self.original_rom_data = data_file.read()
         data_file.close()
         if len(self.original_rom_data) == 0x200200:
-            self.original_rom_data = self.original_rom_data[0x200:]    # Strip the 512-byte header
+            self.original_rom_data = self.original_rom_data[0x200:]  # Strip the 512-byte header
         if len(self.original_rom_data) == 0x200000:
             # Validate a 2MB input
             basehash = hashlib.md5()
             basehash.update(self.original_rom_data)
             if basehash.hexdigest() != 'a7c7a76b4d6f6df389bd631757b91b76':
                 raise OffsetError
         elif len(self.original_rom_data) != 0x400000:
             # If caller gives a 4MB input, assume it knows what it's doing; otherwise fail
             raise OffsetError
 
-        log_file_path = os.path.dirname(rom_path) + os.path.sep + "iogr" + os.path.sep + "logs" + os.path.sep + "app.log"
+        log_file_path = os.path.dirname(
+            rom_path) + os.path.sep + "iogr" + os.path.sep + "logs" + os.path.sep + "app.log"
         if not os.path.exists(os.path.dirname(log_file_path)):
             os.makedirs(os.path.dirname(log_file_path))
 
         logging.basicConfig(filename=log_file_path, filemode='w', format='%(message)s', level=logging.DEBUG)
         self.logger = logging.getLogger("IOGR")
 
     def generate_rom(self, filename: str, settings: RandomizerData, profile_base_filepath=""):
-        self.asar_defines = { "DummyRandomizerDefine": "DummyRandomizerDefine" }
+        self.asar_defines = {"DummyRandomizerDefine": "DummyRandomizerDefine"}
 
         random.seed(settings.seed)
         if settings.race_mode:
             for i in range(random.randint(100, 1000)):
-                _ = random.randint(0,10000)
+                _ = random.randint(0, 10000)
 
         statues_required = self.__get_required_statues__(settings)
         statue_req = settings.statue_req.value
         if statue_req == StatueReq.RANDOM_CHOICE.value:
-            if random.randint(0,1):
+            if random.randint(0, 1):
                 statue_req = StatueReq.GAME_CHOICE.value
             else:
                 statue_req = StatueReq.PLAYER_CHOICE.value
 
         ##########################################################################
         #                  Generate hash code for title screen
         ##########################################################################
         hash_str = filename
         h = hashlib.sha256()
         h.update(hash_str.encode())
         hash = h.digest()
 
-        hash_dict = [ "/", ".", "[", "]", "*", ",", "+", "-", 
-                      "2", "3", "4", "5", "6", "7", "8", "9", ":", 
-            "(", ")", "?", "A", "B", "C", "D", "E", "F", "G", 
-            "H", "I", "J", "K", "L", "M", "N",      "P", "Q", "R", 
-            "S", "T", "U", "V", "W", "X", "Y", "Z", "'", "<", ">", 
-            "#", "a", "b", "c", "d", "e", "f", "g", "h", "i", 
-            "j", "k",      "m", "n", "o", "p", "q", "r", "s", "t", 
-            "u", "v", "w", "x", "y", "z", "{", "}",      "=", ";" ]
+        hash_dict = ["/", ".", "[", "]", "*", ",", "+", "-",
+                     "2", "3", "4", "5", "6", "7", "8", "9", ":",
+                     "(", ")", "?", "A", "B", "C", "D", "E", "F", "G",
+                     "H", "I", "J", "K", "L", "M", "N", "P", "Q", "R",
+                     "S", "T", "U", "V", "W", "X", "Y", "Z", "'", "<", ">",
+                     "#", "a", "b", "c", "d", "e", "f", "g", "h", "i",
+                     "j", "k", "m", "n", "o", "p", "q", "r", "s", "t",
+                     "u", "v", "w", "x", "y", "z", "{", "}", "=", ";"]
 
         hash_len = len(hash_dict)
 
         i = 0
         hash_final = ""
         while i < 6:
             key = hash[i] % hash_len
@@ -249,41 +236,41 @@
         inca_y = random.randint(0, 5)
         self.asar_defines["IncaTileX"] = inca_x
         self.asar_defines["IncaTileY"] = inca_y
 
         ##########################################################################
         #                       Randomize heiroglyph order
         ##########################################################################
-        #hieroglyph_info = {    # 2-byte text word, sprite addr, tile ID
+        # hieroglyph_info = {    # 2-byte text word, sprite addr, tile ID
         #    1: [0xc1c0, 0x81de, 0x84],
         #    2: [0xc3c2, 0x81e4, 0x85],
         #    3: [0xc5c4, 0x81ea, 0x86],
         #    4: [0xc7c6, 0x81f0, 0x8c],
         #    5: [0xc9c8, 0x81f6, 0x8d],
         #    6: [0xcbca, 0x81fc, 0x8e]
-        #}
+        # }
         hieroglyph_order = [1, 2, 3, 4, 5, 6]
         random.shuffle(hieroglyph_order)
         this_pos = 1
         while this_pos < 7:
-            this_hiero = hieroglyph_order[this_pos-1]
-            self.asar_defines["HieroOrder"+str(this_pos)] = this_hiero
-            #self.asar_defines["HieroSpritePointer"+str(this_pos)] = hieroglyph_info[this_hiero][1]
-            #self.asar_defines["HieroItemTile"+str(this_pos)] = hieroglyph_info[this_hiero][2]
-            #self.asar_defines["HieroJournalText"+str(this_pos)] = hieroglyph_info[this_hiero][0]
+            this_hiero = hieroglyph_order[this_pos - 1]
+            self.asar_defines["HieroOrder" + str(this_pos)] = this_hiero
+            # self.asar_defines["HieroSpritePointer"+str(this_pos)] = hieroglyph_info[this_hiero][1]
+            # self.asar_defines["HieroItemTile"+str(this_pos)] = hieroglyph_info[this_hiero][2]
+            # self.asar_defines["HieroJournalText"+str(this_pos)] = hieroglyph_info[this_hiero][0]
             this_pos += 1
 
         ##########################################################################
         #                          Randomize Snake Game
         ##########################################################################
-        snakes_per_sec = [0.85, 0.85, 1.175, 1.50]         # By level
+        snakes_per_sec = [0.85, 0.85, 1.175, 1.50]  # By level
         if settings.flute.value >= 1:
-            snakes_per_sec = [i/4.0 for i in snakes_per_sec]
-        snake_adj = random.uniform(0.9, 1.1)               # Varies snakes per second by +/-10%
-        snake_timer = 5 * random.randint(2,12)             # Timer between 10 and 60 sec (inc 5)
+            snakes_per_sec = [i / 4.0 for i in snakes_per_sec]
+        snake_adj = random.uniform(0.9, 1.1)  # Varies snakes per second by +/-10%
+        snake_timer = 5 * random.randint(2, 12)  # Timer between 10 and 60 sec (inc 5)
         snake_target = []
         snake_target.append(int(snake_timer * snakes_per_sec[0] * snake_adj))
         snake_target.append(int(snake_timer * snakes_per_sec[1] * snake_adj))
         snake_target.append(int(snake_timer * snakes_per_sec[2] * snake_adj))
         snake_target.append(int(snake_timer * snakes_per_sec[3] * snake_adj))
 
         snake_frames_str = format((60 * snake_timer) % 256, "02x") + format(int((60 * snake_timer) / 256), "02x")
@@ -298,75 +285,61 @@
         self.asar_defines["SnakeGameTargetEasy"] = int(snake_timer * snakes_per_sec[0] * snake_adj)
         self.asar_defines["SnakeGameTargetIntermediate"] = int(snake_timer * snakes_per_sec[1] * snake_adj)
         self.asar_defines["SnakeGameTargetAdvanced"] = int(snake_timer * snakes_per_sec[2] * snake_adj)
         self.asar_defines["SnakeGameTargetExpert"] = int(snake_timer * snakes_per_sec[3] * snake_adj)
         # The initial space forces the define to resolve as text instead of a number.
         self.asar_defines["SnakeGameTimeLimitSecondsString"] = "_" + str(snake_timer)
         self.asar_defines["SnakeGameTargetEasyString"] = "_" + str(int(snake_timer * snakes_per_sec[0] * snake_adj))
-        self.asar_defines["SnakeGameTargetIntermediateString"] = "_" + str(int(snake_timer * snakes_per_sec[1] * snake_adj))
+        self.asar_defines["SnakeGameTargetIntermediateString"] = "_" + str(
+            int(snake_timer * snakes_per_sec[1] * snake_adj))
         self.asar_defines["SnakeGameTargetAdvancedString"] = "_" + str(int(snake_timer * snakes_per_sec[2] * snake_adj))
         self.asar_defines["SnakeGameTargetExpertString"] = "_" + str(int(snake_timer * snakes_per_sec[3] * snake_adj))
 
         ##########################################################################
         #                    Randomize Jeweler Reward amounts
         ##########################################################################
         gem = []
+        gem_mod = settings.difficulty.value
         if settings.z3:
             gem.append(random.randint(1, 2))
             gem.append(random.randint(3, 4))
             gem.append(random.randint(5, 7))
             gem.append(random.randint(8, 11))
             gem.append(random.randint(12, 17))
             gem.append(random.randint(18, 23))
             gem.append(random.randint(24, 34))
-
             if settings.goal.value == Goal.RED_JEWEL_HUNT.value:
-                if settings.difficulty.value == 0:
-                    gem[6] = 24
-                elif settings.difficulty.value == 1:
-                    gem[6] = 28
-                elif settings.difficulty.value == 2:
-                    gem[6] = 31
-                elif settings.difficulty.value == 3:
-                    gem[6] = 34
+                gem[6] = [24, 28, 31, 34][gem_mod]
         else:
             gem.append(random.randint(1, 3))
             gem.append(random.randint(4, 6))
             gem.append(random.randint(7, 9))
             gem.append(random.randint(10, 14))
-            gem.append(random.randint(16, 24))
-            gem.append(random.randint(26, 34))
-            gem.append(random.randint(36, 50))
-
+            gem.append(random.randint(16, 21 + gem_mod))
+            gem.append(random.randint(23 + gem_mod, 28 + 2*gem_mod))
+            gem.append(random.randint(32 + 2*gem_mod, 38 + 4*gem_mod))
             if settings.goal.value == Goal.RED_JEWEL_HUNT.value:
-                if settings.difficulty.value == 0:
-                    gem[6] = 35
-                elif settings.difficulty.value == 1:
-                    gem[6] = 40
-                elif settings.difficulty.value == 2:
-                    gem[6] = 45
-                elif settings.difficulty.value == 3:
-                    gem[6] = 50
+                gem[6] = [35, 40, 45, 50][gem_mod]
 
         i = 1
         while i <= 7:
-            self.asar_defines["Jeweler"+str(i)+"Cost"] = gem[i-1]
+            self.asar_defines["Jeweler" + str(i) + "Cost"] = gem[i - 1]
             i += 1
 
         ##########################################################################
         #                    Randomize Mystic Statue requirement
         ##########################################################################
         statueOrder = [1, 2, 3, 4, 5, 6]
         random.shuffle(statueOrder)
         statues = []
         statues_hex = []
-        
+
         self.asar_defines["StatuesRequiredCount"] = statues_required
         for i in statueOrder:
-            self.asar_defines["Statue"+str(i)+"Required"] = 0
+            self.asar_defines["Statue" + str(i) + "Required"] = 0
 
         if statue_req == StatueReq.PLAYER_CHOICE.value:
             self.asar_defines["SettingStatuesPlayerChoice"] = 1
         else:
             self.asar_defines["SettingStatuesPlayerChoice"] = 0
             i = 0
             while i < statues_required:
@@ -401,76 +374,77 @@
         ##########################################################################
         # Edge cases:
         # - MQ2 and SA post-defeat lead to the top of Babel
         # - Babel boss and Mansion boss post-defeat lead to Dao (unless the boss is MQ2 or SA)
         # - The top of Babel leads to the dungeon of MQ2
         # - Rama Statues are required by the Mu boss, not by Vamps
         # - S exit from Vamp statue room returns to the dungeon of Vamps
-        boss_order = [*range(1,8)]
+        boss_order = [*range(1, 8)]
         if settings.boss_shuffle:
-            non_will_bosses = [5]               # Never forced to play Mummy Queen as Will
+            non_will_bosses = [5]  # Never forced to play Mummy Queen as Will
             if settings.flute.value == FluteOpt.FLUTELESS.value:
-                non_will_bosses.append(1)       # Can't beat Castoth as Will without Flute (or generous ability shuffle and lots of patience)
-            if settings.difficulty.value < 3:   # For non-Extreme seeds:
-                boss_order.remove(7)            # - Don't shuffle Solid Arm;
+                non_will_bosses.append(
+                    1)  # Can't beat Castoth as Will without Flute (or generous ability shuffle and lots of patience)
+            if settings.difficulty.value < 3:  # For non-Extreme seeds:
+                boss_order.remove(7)  # - Don't shuffle Solid Arm;
                 if settings.flute.value == FluteOpt.FLUTELESS.value:
-                    non_will_bosses.append(3)   # - Don't require fluteless Vamps.
-            if settings.difficulty.value < 2:   # Also, in Easy/Normal, can't be forced to play Vampires as Will
+                    non_will_bosses.append(3)  # - Don't require fluteless Vamps.
+            if settings.difficulty.value < 2:  # Also, in Easy/Normal, can't be forced to play Vampires as Will
                 if 3 not in non_will_bosses:
                     non_will_bosses.append(3)
             random.shuffle(non_will_bosses)
-        
+
             # Determine statue order for shuffle
             for x in non_will_bosses:
                 boss_order.remove(x)
             random.shuffle(boss_order)
-            non_will_dungeons = [0,1,2,4]   # i.e., the dungeons that don't force Will at the boss door
+            non_will_dungeons = [0, 1, 2, 4]  # i.e., the dungeons that don't force Will at the boss door
             random.shuffle(non_will_dungeons)
             non_will_dungeons = non_will_dungeons[:len(non_will_bosses)]
             non_will_dungeons.sort()
             while non_will_bosses:
                 boss = non_will_bosses.pop(0)
                 dungeon = non_will_dungeons.pop(0)
-                boss_order.insert(dungeon,boss)
+                boss_order.insert(dungeon, boss)
             if 7 not in boss_order:
                 boss_order.append(7)
-        
-            boss_music_card_labels = ["Inca","SkGn","Mu","GtWl","Pymd","Mansion","MinorDungeon"]
+
+            boss_music_card_labels = ["Inca", "SkGn", "Mu", "GtWl", "Pymd", "Mansion", "MinorDungeon"]
             # Patch music headers into new dungeons (beginner and intermediate modes)
             if settings.difficulty.value <= 1:
                 i = 0
                 while i < 6:
                     boss = boss_order[i]
-                    this_dungeon_card = "Map"+boss_music_card_labels[i]+"CardMusic"
-                    replacement_card = "DefaultMap"+boss_music_card_labels[boss-1]+"CardMusic"
-                    self.asar_defines[this_dungeon_card] = "!"+replacement_card
+                    this_dungeon_card = "Map" + boss_music_card_labels[i] + "CardMusic"
+                    replacement_card = "DefaultMap" + boss_music_card_labels[boss - 1] + "CardMusic"
+                    self.asar_defines[this_dungeon_card] = "!" + replacement_card
                     i += 1
         # Set up assembly defines for boss order
         i = 1
         while i < 8:
-            self.asar_defines["Boss"+str(i)+"Id"] = boss_order[i-1]
+            self.asar_defines["Boss" + str(i) + "Id"] = boss_order[i - 1]
             i += 1
 
         ##########################################################################
         #                   Randomize Location of Kara Portrait
         #       Sets spoiler in Lance's Letter and places portrait sprite
         ##########################################################################
         # Determine random location ID
         kara_location = random.randint(1, 5)
         self.asar_defines["KaraLocation"] = kara_location
 
         # Set Kara's location and logic mode in RAM switches (for autotracker)
         ## (hmm, I don't think tracker supports this yet?)
-        #if settings.logic.value == Logic.COMPLETABLE.value:
+        # if settings.logic.value == Logic.COMPLETABLE.value:
         #    logic_int = 0x10 + kara_location
-        #elif settings.logic.value == Logic.BEATABLE.value:
+        # elif settings.logic.value == Logic.BEATABLE.value:
         #    logic_int = 0x20 + kara_location
-        #else:
+        # else:
         #    logic_int = 0x40 + kara_location
-        self.asar_defines["AutotrackerLogicAndKaraVal"] = kara_location#logic_int
+        self.asar_defines["AutotrackerLogicAndKaraVal"] = kara_location  # logic_int
 
         ##########################################################################
         #                          Have fun with death text
         ##########################################################################
         death_list = []
         death_list.append(
             b"\x2d\x48\xa4\xac\xd6\xa3\xa3\x8e\xac\x87\x80\xa0\xa0\x84\x8d\xa3\xac\xd6\xd7\xcb\xd6\xfe\x85\xa2\x88\x84\x8d\x83\xac\xd7\x73\x88\xa3\xac\xd7\x89\xcb\x4c\x4e\x63\x64\x4b\x69\xac\x83\x84\x80\x83\x2a\x2e\xcb\xac\xac\x6d\x4c\x88\xa2\x80\x82\x8b\x84\xac\x4c\x80\xa8\xc0")
@@ -486,15 +460,16 @@
             b"\x2d\x40\x8b\x8b\xac\x83\x84\x80\xa4\x87\xa3\xac\x80\xa2\x84\xac\xa3\xa5\x83\x83\x84\x8d\xab\xac\x8d\x8e\xcb\xd6\xb8\x87\x8e\xa7\xac\x86\xa2\x80\x83\xa5\x80\x8b\xac\xa4\x87\x84\xcb\x83\xa9\x88\x8d\x86\xac\x8c\x80\xa9\xac\x81\x84\x2a\x2e\xcb\xac\xac\x6d\x4c\x88\x82\x87\x80\x84\x8b\xac\x4c\x82\x43\x8e\xa7\x84\x8b\x8b\xc0")
         death_list.append(
             b"\x2d\x43\x84\x80\xa4\x87\xac\x88\xa3\xac\xa0\x84\xa2\x87\x80\xa0\xa3\xac\x80\x8d\xcb\x8e\xa2\x83\x84\x80\x8b\xab\xac\x81\xa5\xa4\xac\x88\xa4\xac\x88\xa3\xac\x8d\x8e\xa4\xac\x80\x8d\xcb\x84\xa8\xa0\x88\x80\xa4\x88\x8e\x8d\x2a\x2e\xcb\xac\xac\x6d\x40\x8b\x84\xa8\x80\x8d\x83\xa2\x84\xac\x43\xa5\x8c\x80\xa3\xc0")
         death_list.append(
             b"\x2d\xd6\x62\xd7\x95\x8c\x80\xa4\xa4\x84\xa2\x84\x83\xac\x88\x8d\xcb\x8b\x88\x85\x84\xab\xac\xd6\xf7\x86\x80\xa6\x84\xac\x88\xa4\xcb\xa7\x84\x88\x86\x87\xa4\xab\xac\xa7\x80\xa3\xac\x83\x84\x80\xa4\x87\x2a\x2e\xcb\xac\xac\x6d\x49\x84\x85\x85\xa2\x84\xa9\xac\x44\xa5\x86\x84\x8d\x88\x83\x84\xa3\xc0")
         death_list.append(
             b"\x2d\x4d\x8e\xac\x8e\x8d\x84\xac\xd7\x6d\x8e\xa5\xa4\xac\x8e\x85\xac\xd6\xd6\xcb\xd6\xf5\x80\x8b\x88\xa6\x84\x2a\x2a\x2a\xac\x84\xa8\x82\x84\xa0\xa4\xcb\x80\xa3\xa4\xa2\x8e\x8d\x80\xa5\xa4\xa3\x2a\x2e\xcb\xac\xac\x6d\x63\xa4\x84\xa7\x80\xa2\xa4\xac\x63\xa4\x80\x85\x85\x8e\xa2\x83\xc0")
-        death_list.append(b"\x2d\x44\xa4\xac\xa4\xa5\xac\x41\xa2\xa5\xa4\x84\x0d\x2e\xcb\xac\xac\x6d\x49\xa5\x8b\x88\xa5\xa3\xac\x42\x80\x84\xa3\x80\xa2\xc0")
+        death_list.append(
+            b"\x2d\x44\xa4\xac\xa4\xa5\xac\x41\xa2\xa5\xa4\x84\x0d\x2e\xcb\xac\xac\x6d\x49\xa5\x8b\x88\xa5\xa3\xac\x42\x80\x84\xa3\x80\xa2\xc0")
         death_list.append(
             b"\x2d\x64\x8e\xac\xa4\x87\x84\xac\xa7\x88\xaa\x80\xa2\x83\xac\x83\x84\x80\xa4\x87\xac\x88\xa3\xcb\x8c\x84\xa2\x84\x8b\xa9\xac\x80\xac\x81\x84\x8b\x88\x84\x85\x2a\x2e\xcb\xac\xac\x6d\x43\x84\x84\xa0\x80\x8a\xac\x42\x87\x8e\xa0\xa2\x80\xc0")
         death_list.append(
             b"\x2d\x44\xa6\x84\xa2\xa9\xac\xd6\xdf\xa9\x8e\xa5\xac\x83\x88\x84\xab\xac\x88\xa4\xcb\x87\xa5\xa2\xa4\xa3\x2a\x2e\xcb\xac\xac\x6d\x49\x8e\xa3\x87\xac\x47\x84\x8d\x83\x84\xa2\xa3\x8e\x8d\xc0")
         death_list.append(
             b"\x2d\x48\x85\xac\x48\xac\xd6\x98\xa4\x8e\xac\x83\x88\x84\xab\xac\x8b\x84\xa4\xac\x8c\x84\xcb\x83\x88\x84\xac\x85\x88\x86\x87\xa4\x88\x8d\x86\x2a\x2e\xcb\xac\xac\x6d\x46\x80\x81\xa2\x88\x84\x8b\xac\x46\x80\xa2\x82\x88\x80\xac\x4c\x80\xa2\xa1\xa5\x84\xaa\xc0")
         death_list.append(
@@ -606,22 +581,23 @@
         death_list.append(
             b"\x2d\x4B\x88\x85\x84\xac\x8b\x84\xa6\x84\x8b\xa3\xac\x80\x8b\x8b\xac\x8c\x84\x8d\x2a\xcb\x43\x84\x80\xa4\x87\xac\xa2\x84\xa6\x84\x80\x8b\xa3\xac\xa4\x87\x84\xcb\x84\x8c\x88\x8d\x84\x8d\xa4\x2a\x2e\xcb\xac\xac\x6d\x46\x84\x8e\xa2\x86\x84\xac\x41\x84\xa2\x8d\x80\xa2\x83\xac\x63\x87\x80\xa7\xc0")
         death_list.append(
             b"\x2d\x43\x84\x80\xa4\x87\xac\x88\xa3\xac\xa4\x87\x84\xac\xa7\x88\xa3\x87\xac\x8e\x85\xcb\xa3\x8e\x8c\x84\x2b\xac\xa4\x87\x84\xac\xa2\x84\x8b\x88\x84\x85\xac\x8e\x85\xac\x8c\x80\x8d\xa9\x2b\xcb\x80\x8d\x83\xac\xa4\x87\x84\xac\x84\x8d\x83\xac\x8e\x85\xac\x80\x8b\x8b\x2a\x2e\xcb\xac\xac\x6d\x4B\xa5\x82\x88\xa5\xa3\xac\x40\x8d\x8d\x80\x84\xa5\xa3\xac\x63\x84\x8d\x84\x82\x80\xc0")
         death_list.append(
             b"\x2d\x43\x84\x80\xa4\x87\xac\xa7\x88\x8b\x8b\xac\x81\x84\xac\x80\xac\x86\xa2\x84\x80\xa4\xcb\xa2\x84\x8b\x88\x84\x85\x2a\xac\x4D\x8e\xac\x8c\x8e\xa2\x84\xcb\x88\x8d\xa4\x84\xa2\xa6\x88\x84\xa7\xa3\x2a\x2e\xcb\xac\xac\x6d\x4A\x80\xa4\x87\x80\xa2\x88\x8d\x84\xac\x47\x84\xa0\x81\xa5\xa2\x8d\xc0\xc0")
         if settings.difficulty.value >= 3:
-            death_list.append(b"\x2d\x46\x88\xa4\xac\x86\xa5\x83\xac\xa3\x82\xa2\xa5\x81\x2a\x2e\xcb\xac\xac\x6d\x41\x80\x86\xa5\xc0")
+            death_list.append(
+                b"\x2d\x46\x88\xa4\xac\x86\xa5\x83\xac\xa3\x82\xa2\xa5\x81\x2a\x2e\xcb\xac\xac\x6d\x41\x80\x86\xa5\xc0")
 
         # Will death text
         death_str = death_list[random.randint(0, len(death_list) - 1)]
         self.asar_defines["PlayerDeathText"] = ""
         i = 0
         while i < len(death_str):
-            self.asar_defines["PlayerDeathText"] += "$" + format(death_str[i],"02x")
+            self.asar_defines["PlayerDeathText"] += "$" + format(death_str[i], "02x")
             i += 1
             if i < len(death_str):
                 self.asar_defines["PlayerDeathText"] += ","
 
         ##########################################################################
         #                   Randomize item and ability placement
         ##########################################################################
@@ -629,20 +605,22 @@
         self.seed_adj = 0
         while not done:
             if self.seed_adj > MAX_RANDO_RETRIES:
                 self.logger.error("ERROR: Max number of seed adjustments exceeded")
                 raise RecursionError
             elif self.seed_adj > 0:
                 if settings.printlevel.value > -1:
-                    print("Trying again... attempt", self.seed_adj+1)
-            self.w = World(settings, statues_required, statues, statue_req, kara_location, gem, [inca_x + 1, inca_y + 1], hieroglyph_order, boss_order)
-            done = self.w.randomize(self.seed_adj, settings.printlevel.value, settings.break_on_error, settings.break_on_init)
+                    print("Trying again... attempt", self.seed_adj + 1)
+            self.w = World(settings, statues_required, statues, statue_req, kara_location, gem,
+                           [inca_x + 1, inca_y + 1], hieroglyph_order, boss_order)
+            done = self.w.randomize(self.seed_adj, settings.printlevel.value, settings.break_on_error,
+                                    settings.break_on_init)
             if profile_base_filepath != "":
                 val_messages = self.w.validate()
-                f = open(profile_base_filepath + "_" + format(self.seed_adj,"02") + ".txt","w")
+                f = open(profile_base_filepath + "_" + format(self.seed_adj, "02") + ".txt", "w")
                 f.write(generate_filename(settings, ""))
                 f.write("\n\n")
                 f.write("Error log:\n")
                 if not self.w.errorlog:
                     f.write("No errors\n")
                 else:
                     for m in self.w.errorlog:
@@ -671,37 +649,37 @@
         for wdef in self.w.asar_defines:
             self.asar_defines[wdef] = self.w.asar_defines[wdef]
 
         ##########################################################################
         #                        Randomize Ishtar puzzle
         ##########################################################################
         used_hair = False
-        for room,maxchg in [(1,10), (2,7), (3,4), (4,9)]:
+        for room, maxchg in [(1, 10), (2, 7), (3, 4), (4, 9)]:
             minchg = 1 if used_hair else 0
-            change1 = random.randint(minchg,maxchg)
+            change1 = random.randint(minchg, maxchg)
             if change1 == 0:
                 used_hair = True
                 minchg = 1
-            self.asar_defines["IshtarRoom"+str(room)+"DifferenceIndex1"] = change1
+            self.asar_defines["IshtarRoom" + str(room) + "DifferenceIndex1"] = change1
             if settings.difficulty.value >= 2:
                 change2 = change1
                 while change2 == change1:
-                    change2 = random.randint(minchg,maxchg)
+                    change2 = random.randint(minchg, maxchg)
                 if change2 == 0:
                     used_hair = True
                     minchg = 1
-                self.asar_defines["IshtarRoom"+str(room)+"DifferenceIndex2"] = change2
+                self.asar_defines["IshtarRoom" + str(room) + "DifferenceIndex2"] = change2
                 if settings.difficulty.value >= 3:
                     change3 = change2
                     while change3 == change2 or change3 == change1:
-                        change3 = random.randint(minchg,maxchg)
+                        change3 = random.randint(minchg, maxchg)
                     if change3 == 0:
                         used_hair = True
                         minchg = 1
-                    self.asar_defines["IshtarRoom"+str(room)+"DifferenceIndex3"] = change3
+                    self.asar_defines["IshtarRoom" + str(room) + "DifferenceIndex3"] = change3
 
         ##########################################################################
         #                                   Plugins
         ##########################################################################
         if self.w.goal == "Apocalypse Gaia":
             self.asar_defines["ApocalypseGaia"] = 1
         else:
@@ -747,17 +725,17 @@
         self.asar_defines["TextShadowSuperhero"] = superhero_list[rand_idx]
 
         ##########################################################################
         #            Pass all defines to assembler and return patch
         ##########################################################################
         if len(self.original_rom_data) == 0x200000:
             romdata = copy.deepcopy(self.original_rom_data) + bytearray(0x200000)
-        else:   # Caller provided a pre-expanded input
+        else:  # Caller provided a pre-expanded input
             romdata = copy.deepcopy(self.original_rom_data)
-        
+
         self.asar_defines["SettingBossShuffle"] = 1 if settings.boss_shuffle else 0
         self.asar_defines["SettingInfiniteInventory"] = 1 if settings.infinite_inventory else 0
         self.asar_defines["SettingEarlyFirebird"] = 1 if settings.firebird else 0
         self.asar_defines["SettingRedJewelHunt"] = 1 if settings.goal.value is Goal.RED_JEWEL_HUNT.value else 0
         self.asar_defines["SettingRedJewelMadness"] = 1 if settings.red_jewel_madness else 0
         self.asar_defines["SettingOpenMode"] = 1 if settings.open_mode else 0
         self.asar_defines["SettingOHKO"] = 1 if settings.ohko else 0
@@ -773,35 +751,36 @@
             self.asar_defines["InitialHp"] = 40
         elif settings.ohko:
             self.asar_defines["InitialHp"] = 1
         elif settings.z3:
             self.asar_defines["InitialHp"] = 6
         else:
             self.asar_defines["InitialHp"] = 8
-        
+
         self.asar_defines["OptionMuteMusic"] = 0
-        
+
         for d in self.asar_defines:
-            self.asar_defines[d] = str(self.asar_defines[d])   # The library requires defines to be string type.
+            self.asar_defines[d] = str(self.asar_defines[d])  # The library requires defines to be string type.
         if os.name != "nt":
             asar.init(os.path.dirname(__file__) + os.path.sep + "asar-x64.so")
-        else:    # Windows
+        else:  # Windows
             os.add_dll_directory(os.path.dirname(__file__))
-            if sys.maxsize > 2**32:    # 64-bit
+            if sys.maxsize > 2 ** 32:  # 64-bit
                 asar.init("asar-x64.dll")
-            else:    # 32-bit
+            else:  # 32-bit
                 asar.init("asar-x86.dll")
-        self.asar_patch_result = asar.patch(os.path.dirname(__file__) + os.path.sep + "iogr.asr", romdata, [], True, self.asar_defines)
-        
+        self.asar_patch_result = asar.patch(os.path.dirname(__file__) + os.path.sep + "iogr.asr", romdata, [], True,
+                                            self.asar_defines)
+
         if self.asar_patch_result[0]:
             return self.asar_patch_result
         else:
             asar_error_list = asar.geterrors()
             return [False, asar_error_list]
-    
+
     # Returns a list of dicts of the form {'index': int, 'address': int, 'data': list of ints}
     def generate_legacy_patch(self, filename: str, settings: RandomizerData):
         self.generate_rom(filename, settings)
         if not self.asar_patch_result[0]:
             return False
         legacy_patch = []
         legacy_idx = 0
@@ -820,34 +799,33 @@
     def generate_spoiler(self) -> str:
         return json.dumps(self.w.spoiler)
 
     def generate_def_dump(self) -> str:
         defkeys_sorted = []
         defs = {}
         if self.asar_patch_result[0]:
-            defs = {define: val for define,val in asar.getalldefines().items() if define[:7] not in ["Default","Monster","PlayerD","AG_Spr_","DG_Spr_"]}
+            defs = {define: val for define, val in asar.getalldefines().items() if
+                    define[:7] not in ["Default", "Monster", "PlayerD", "AG_Spr_", "DG_Spr_"]}
             defkeys_sorted = sorted(defs)
         defdump = ""
         for d in defkeys_sorted:
             defdump += "!" + d + " = " + defs[d] + "\n"
         return defdump
-    
+
     def generate_config_addrs(self) -> str:
         cfgkeys_sorted = []
         config_labels = {}
         if self.asar_patch_result[0]:
             labels = asar.getalllabels()
-            config_labels = {label: val for label,val in labels.items() if label[:7] == "Config_"}
+            config_labels = {label: val for label, val in labels.items() if label[:7] == "Config_"}
             cfgkeys_sorted = sorted(config_labels)
         addrdump = ""
         for d in cfgkeys_sorted:
-            addrdump += d + "\t" + str(int(config_labels[d])&0x3fffff) + "\n"
+            addrdump += d + "\t" + str(int(config_labels[d]) & 0x3fffff) + "\n"
         return addrdump
 
     def __get_required_statues__(self, settings: RandomizerData) -> int:
         if settings.goal.value == Goal.RED_JEWEL_HUNT.value:
             return 0
         if settings.statues.lower() == "random":
             return random.randint(0, 6)
         return int(settings.statues)
-
-
```

### Comparing `iog-randomizer-4.7.2.2/randomizer/models/enums.py` & `iog_randomizer-5.0.0/src/iog_randomizer/randomizer/models/enums.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,85 +8,96 @@
     FEWCURSED = -1
     NONE = 0
     FEW = 1
     SOME = 2
     MANY = 3
     ALL = 4
 
+
 class Difficulty(Enum):
     EASY = 0
     NORMAL = 1
     HARD = 2
     EXTREME = 3
 
+
 class DungeonShuffle(Enum):
     NONE = 0
     BASIC = 1
     CHAOS = 2
     CLUSTERED = 3
 
+
 class Enemizer(Enum):
     NONE = 0
     LIMITED = 1
     BALANCED = 2
     FULL = 3
     INSANE = 4
 
+
 class EntranceShuffle(Enum):
     NONE = 0
     COUPLED = 1
     UNCOUPLED = 2
 
+
 class FluteOpt(Enum):
     START = 0
     SHUFFLE = 1
     FLUTELESS = 2
 
+
 class Goal(Enum):
     DARK_GAIA = 0
     RED_JEWEL_HUNT = 1
     APO_GAIA = 2
     RANDOM_GAIA = 3
 
+
 class Level(Enum):
     BEGINNER = 0
     INTERMEDIATE = 1
     ADVANCED = 2
     EXPERT = 3
 
+
 class Logic(Enum):
     COMPLETABLE = 0
     BEATABLE = 1
     CHAOS = 2
 
+
 class OrbRando(Enum):
     NONE = 0
     BASIC = 1
     ORBSANITY = 2
 
+
 class Sprite(Enum):
     WILL = "will"
     BAGU = "bagu"
     INVISIBLE = "invisible"
     FREET = "freet"
     SOLAR = "solar"
     SYE = "sye"
 
+
 class StartLocation(Enum):
     SOUTH_CAPE = 0
     SAFE = 1
     UNSAFE = 2
     FORCED_UNSAFE = 3
 
+
 class StatueReq(Enum):
     GAME_CHOICE = 0
     PLAYER_CHOICE = 1
     RANDOM_CHOICE = 2
 
+
 class PrintLevel(Enum):
     SILENT = -1
     ERROR = 0
     WARN = 1
     INFO = 2
     VERBOSE = 3
-    
-
```

### Comparing `iog-randomizer-4.7.2.2/randomizer/patch.py` & `iog_randomizer-5.0.0/src/iog_randomizer/randomizer/patch.py`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.2/randomizer/quintet_comp.py` & `iog_randomizer-5.0.0/src/iog_randomizer/randomizer/quintet_comp.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,18 +14,16 @@
 # The format is described in greater detail in the decompressor.
 #
 #
 #
 # This code uses python-bitstring:
 # https://pypi.python.org/pypi/bitstring
 
-from __future__ import print_function
-from __future__ import division
-
 import sys
+
 import bitstring
 
 
 def compress(inBytes):
     # Define some useful constants.
     SEARCH_LOG2 = 8
     SEARCH_SIZE = 2 ** SEARCH_LOG2
```

### Comparing `iog-randomizer-4.7.2.2/randomizer/quintet_text.py` & `iog_randomizer-5.0.0/src/iog_randomizer/randomizer/quintet_text.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,603 +1,605 @@
 MAX_WIDTH = 26
 
 text_words = {
-    "Attack " : 	b"\xD6\x00",
-    "Angel " : 	b"\xD6\x01",
-    "After " : 	b"\xD6\x02",
-    "Aura " : 	b"\xD6\x03",
-    "Ankor " : 	b"\xD6\x04",
-    "Black " : 	b"\xD6\x05",
-    "Bill: " : 	b"\xD6\x06",
-    "Crystal " : 	b"\xD6\x07",
-    "City " : 	b"\xD6\x08",
-    "Come " : 	b"\xD6\x09",
-    "Condor's " : 	b"\xD6\x0A",
-    "Change " : 	b"\xD6\x0B",
-    "Dark " : 	b"\xD6\x0C",
-    "Don't " : 	b"\xD6\x0D",
-    "Diamond " : 	b"\xD6\x0E",
-    "Drifting, " : 	b"\xD6\x0F",
-    "Eric: " : 	b"\xD6\x10",
-    "Edward " : 	b"\xD6\x11",
-    "Even " : 	b"\xD6\x12",
-    "Elder2f " : 	b"\xD6\x13",
-    "Earth " : 	b"\xD6\x14",
-    "Freedan's " : 	b"\xD6\x15",
-    "Great " : 	b"\xD6\x16",
-    "Grandma " : 	b"\xD6\x17",
-    "Good. " : 	b"\xD6\x18",
-    "Gold " : 	b"\xD6\x19",
-    "Grandpa " : 	b"\xD6\x1A",
-    "Hieroglyph " : 	b"\xD6\x1B",
-    "Hey, " : 	b"\xD6\x1C",
-    "It's " : 	b"\xD6\x1D",
-    "Inca " : 	b"\xD6\x1E",
-    "I'll " : 	b"\xD6\x1F",
-    "I've " : 	b"\xD6\x20",
-    "Itorie " : 	b"\xD6\x21",
-    "Jewels " : 	b"\xD6\x22",
-    "Jewels! " : 	b"\xD6\x23",
-    "Just " : 	b"\xD6\x24",
-    "Kara: " : 	b"\xD6\x25",
-    "Kara " : 	b"\xD6\x26",
-    "King " : 	b"\xD6\x27",
-    "Knight " : 	b"\xD6\x28",
-    "Karen's " : 	b"\xD6\x29",
-    "Lilly: " : 	b"\xD6\x2A",
-    "Let's " : 	b"\xD6\x2B",
-    "Lilly " : 	b"\xD6\x2C",
-    "Lola's " : 	b"\xD6\x2D",
-    "Lola: " : 	b"\xD6\x2E",
-    "Mystery " : 	b"\xD6\x2F",
-    "Maybe " : 	b"\xD6\x30",
-    "Moon " : 	b"\xD6\x31",
-    "Man: " : 	b"\xD6\x32",
-    "Morris's " : 	b"\xD6\x33",
-    "Melody " : 	b"\xD6\x34",
-    "Morris: " : 	b"\xD6\x35",
-    "Neil: " : 	b"\xD6\x36",
-    "Neil's " : 	b"\xD6\x37",
-    "Only " : 	b"\xD6\x38",
-    "Once " : 	b"\xD6\x39",
-    "Oink " : 	b"\xD6\x3A",
-    "Please " : 	b"\xD6\x3B",
-    "Psycho " : 	b"\xD6\x3C",
-    "People " : 	b"\xD6\x3D",
-    "Prayer " : 	b"\xD6\x3E",
-    "Pyramid " : 	b"\xD6\x3F",
-    "Purification " : 	b"\xD6\x40",
-    "Plate " : 	b"\xD6\x41",
-    "Quit " : 	b"\xD6\x42",
-    "Rob: " : 	b"\xD6\x43",
-    "Rolek " : 	b"\xD6\x44",
-    "Soldier: " : 	b"\xD6\x45",
-    "Strange " : 	b"\xD6\x46",
-    "South " : 	b"\xD6\x47",
-    "Statue " : 	b"\xD6\x48",
-    "Somehow " : 	b"\xD6\x49",
-    "Sometimes " : 	b"\xD6\x4A",
-    "Something " : 	b"\xD6\x4B",
-    "Shadow's " : 	b"\xD6\x4C",
-    "Someone " : 	b"\xD6\x4D",
-    "This " : 	b"\xD6\x4E",
-    "Will: " : 	b"\xD6\x4F",
-    "There's " : 	b"\xD6\x50",
-    "Will's " : 	b"\xD6\x51",
-    "There " : 	b"\xD6\x52",
-    "That's " : 	b"\xD6\x53",
-    "Tower " : 	b"\xD6\x54",
-    "They " : 	b"\xD6\x55",
-    "Then " : 	b"\xD6\x56",
-    "Trip " : 	b"\xD6\x57",
-    "Thank " : 	b"\xD6\x58",
-    "Take " : 	b"\xD6\x59",
-    "Will. " : 	b"\xD6\x5A",
-    "That " : 	b"\xD6\x5B",
-    "Will, " : 	b"\xD6\x5C",
-    "They're " : 	b"\xD6\x5D",
-    "These " : 	b"\xD6\x5E",
-    "Vampire " : 	b"\xD6\x5F",
-    "Village. " : 	b"\xD6\x60",
-    "When " : 	b"\xD6\x61",
-    "What " : 	b"\xD6\x62",
-    "Well, " : 	b"\xD6\x63",
-    "What's " : 	b"\xD6\x64",
-    "Where " : 	b"\xD6\x65",
-    "Woman: " : 	b"\xD6\x66",
-    "You've " : 	b"\xD6\x67",
-    "Your " : 	b"\xD6\x68",
-    "You're " : 	b"\xD6\x69",
-    "Yes, " : 	b"\xD6\x6A",
-    "about " : 	b"\xD6\x6B",
-    "anything " : 	b"\xD6\x6C",
-    "around " : 	b"\xD6\x6D",
-    "another " : 	b"\xD6\x6E",
-    "ancient " : 	b"\xD6\x6F",
-    "been " : 	b"\xD6\x70",
-    "become " : 	b"\xD6\x71",
-    "body " : 	b"\xD6\x72",
-    "back " : 	b"\xD6\x73",
-    "before " : 	b"\xD6\x74",
-    "brought " : 	b"\xD6\x75",
-    "beautiful " : 	b"\xD6\x76",
-    "being " : 	b"\xD6\x77",
-    "can't " : 	b"\xD6\x78",
-    "come " : 	b"\xD6\x79",
-    "could " : 	b"\xD6\x7A",
-    "comet " : 	b"\xD6\x7B",
-    "company " : 	b"\xD6\x7C",
-    "children " : 	b"\xD6\x7D",
-    "constellation " : 	b"\xD6\x7E",
-    "changed " : 	b"\xD6\x7F",
-    "came " : 	b"\xD6\x80",
-    "coming " : 	b"\xD6\x81",
-    "don't " : 	b"\xD6\x82",
-    "didn't " : 	b"\xD6\x83",
-    "doesn't " : 	b"\xD6\x84",
-    "distant " : 	b"\xD6\x85",
-    "different " : 	b"\xD6\x86",
-    "demons " : 	b"\xD6\x87",
-    "destroy " : 	b"\xD6\x88",
-    "everyone " : 	b"\xD6\x89",
-    "explorer " : 	b"\xD6\x8A",
-    "everyone's " : 	b"\xD6\x8B",
-    "enemies " : 	b"\xD6\x8C",
-    "exposed " : 	b"\xD6\x8D",
-    "from " : 	b"\xD6\x8E",
-    "found " : 	b"\xD6\x8F",
-    "find " : 	b"\xD6\x90",
-    "feel " : 	b"\xD6\x91",
-    "father's " : 	b"\xD6\x92",
-    "going " : 	b"\xD6\x93",
-    "good " : 	b"\xD6\x94",
-    "great " : 	b"\xD6\x95",
-    "ground " : 	b"\xD6\x96",
-    "give " : 	b"\xD6\x97",
-    "have " : 	b"\xD6\x98",
-    "heard " : 	b"\xD6\x99",
-    "human " : 	b"\xD6\x9A",
-    "hear " : 	b"\xD6\x9B",
-    "huge " : 	b"\xD6\x9C",
-    "happened " : 	b"\xD6\x9D",
-    "hieroglyph " : 	b"\xD6\x9E",
-    "it's " : 	b"\xD6\x9F",
-    "inventory " : 	b"\xD6\xA0",
-    "into " : 	b"\xD6\xA1",
-    "inside " : 	b"\xD6\xA2",
-    "just " : 	b"\xD6\xA3",
-    "know " : 	b"\xD6\xA4",
-    "like " : 	b"\xD6\xA5",
-    "long " : 	b"\xD6\xA6",
-    "little " : 	b"\xD6\xA7",
-    "light " : 	b"\xD6\xA8",
-    "look " : 	b"\xD6\xA9",
-    "looks " : 	b"\xD6\xAA",
-    "looking " : 	b"\xD6\xAB",
-    "leave " : 	b"\xD6\xAC",
-    "labor " : 	b"\xD6\xAD",
-    "left " : 	b"\xD6\xAE",
-    "live " : 	b"\xD6\xAF",
-    "life " : 	b"\xD6\xB0",
-    "living " : 	b"\xD6\xB1",
-    "must " : 	b"\xD6\xB2",
-    "made " : 	b"\xD6\xB3",
-    "melody " : 	b"\xD6\xB4",
-    "move " : 	b"\xD6\xB5",
-    "many " : 	b"\xD6\xB6",
-    "more " : 	b"\xD6\xB7",
-    "matter " : 	b"\xD6\xB8",
-    "nothing " : 	b"\xD6\xB9",
-    "need " : 	b"\xD6\xBA",
-    "never " : 	b"\xD6\xBB",
-    "next " : 	b"\xD6\xBC",
-    "other " : 	b"\xD6\xBD",
-    "over " : 	b"\xD6\xBE",
-    "outside " : 	b"\xD6\xBF",
-    "original " : 	b"\xD6\xC0",
-    "people " : 	b"\xD6\xC1",
-    "power " : 	b"\xD6\xC2",
-    "present. " : 	b"\xD6\xC3",
-    "playing " : 	b"\xD6\xC4",
-    "raised " : 	b"\xD6\xC5",
-    "right-hand " : 	b"\xD6\xC6",
-    "strange " : 	b"\xD6\xC7",
-    "something " : 	b"\xD6\xC8",
-    "statue " : 	b"\xD6\xC9",
-    "should " : 	b"\xD6\xCA",
-    "started " : 	b"\xD6\xCB",
-    "seems " : 	b"\xD6\xCC",
-    "same " : 	b"\xD6\xCD",
-    "such " : 	b"\xD6\xCE",
-    "someone " : 	b"\xD6\xCF",
-    "some " : 	b"\xD6\xD0",
-    "save " : 	b"\xD6\xD1",
-    "statues " : 	b"\xD6\xD2",
-    "still " : 	b"\xD6\xD3",
-    "said " : 	b"\xD6\xD4",
-    "stands " : 	b"\xD6\xD5",
-    "this " : 	b"\xD6\xD6",
-    "that " : 	b"\xD6\xD7",
-    "thought " : 	b"\xD6\xD8",
-    "there " : 	b"\xD6\xD9",
-    "think " : 	b"\xD6\xDA",
-    "there's " : 	b"\xD6\xDB",
-    "through " : 	b"\xD6\xDC",
-    "tried " : 	b"\xD6\xDD",
-    "terrible " : 	b"\xD6\xDE",
-    "time " : 	b"\xD6\xDF",
-    "things " : 	b"\xD6\xE0",
-    "their " : 	b"\xD6\xE1",
-    "town " : 	b"\xD6\xE2",
-    "thing " : 	b"\xD6\xE3",
-    "these " : 	b"\xD6\xE4",
-    "temple " : 	b"\xD6\xE5",
-    "them " : 	b"\xD6\xE6",
-    "take " : 	b"\xD6\xE7",
-    "turned, " : 	b"\xD6\xE8",
-    "understand " : 	b"\xD6\xE9",
-    "under " : 	b"\xD6\xEA",
-    "underwater " : 	b"\xD6\xEB",
-    "village " : 	b"\xD6\xEC",
-    "very " : 	b"\xD6\xED",
-    "voice " : 	b"\xD6\xEE",
-    "will " : 	b"\xD6\xEF",
-    "with " : 	b"\xD6\xF0",
-    "want " : 	b"\xD6\xF1",
-    "were " : 	b"\xD6\xF2",
-    "would " : 	b"\xD6\xF3",
-    "where " : 	b"\xD6\xF4",
-    "world " : 	b"\xD6\xF5",
-    "when " : 	b"\xD6\xF6",
-    "what " : 	b"\xD6\xF7",
-    "without " : 	b"\xD6\xF8",
-    "wonder " : 	b"\xD6\xF9",
-    "won't " : 	b"\xD6\xFA",
-    "wouldn't " : 	b"\xD6\xFB",
-    "wanted " : 	b"\xD6\xFC",
-    "waiting " : 	b"\xD6\xFD",
-    "your " : 	b"\xD6\xFE",
-    "you're " : 	b"\xD6\xFF",
-    "1994 " : 	b"\xD7\x00",
-    "Actually, " : 	b"\xD7\x01",
-    "Button " : 	b"\xD7\x02",
-    "Buttons " : 	b"\xD7\x03",
-    "Back " : 	b"\xD7\x04",
-    "Child: " : 	b"\xD7\x05",
-    "Defeating " : 	b"\xD7\x06",
-    "Didn't " : 	b"\xD7\x07",
-    "Desert " : 	b"\xD7\x08",
-    "Erasquez: " : 	b"\xD7\x09",
-    "Elder " : 	b"\xD7\x0A",
-    "Earth's " : 	b"\xD7\x0B",
-    "Eric's " : 	b"\xD7\x0C",
-    "Everybody " : 	b"\xD7\x0D",
-    "Flute: " : 	b"\xD7\x0E",
-    "First " : 	b"\xD7\x0F",
-    "Firebird, " : 	b"\xD7\x10",
-    "From " : 	b"\xD7\x11",
-    "Gaia, " : 	b"\xD7\x12",
-    "Gorgon " : 	b"\xD7\x13",
-    "Have " : 	b"\xD7\x14",
-    "Hey! " : 	b"\xD7\x15",
-    "Istar's " : 	b"\xD7\x16",
-    "Ishtar's " : 	b"\xD7\x17",
-    "Lilly's " : 	b"\xD7\x18",
-    "Larai " : 	b"\xD7\x19",
-    "Looking " : 	b"\xD7\x1A",
-    "Main " : 	b"\xD7\x1B",
-    "Man's " : 	b"\xD7\x1C",
-    "Memory " : 	b"\xD7\x1D",
-    "Mountain " : 	b"\xD7\x1E",
-    "Morris " : 	b"\xD7\x1F",
-    "Many " : 	b"\xD7\x20",
-    "Native " : 	b"\xD7\x21",
-    "Native's " : 	b"\xD7\x22",
-    "Neil " : 	b"\xD7\x23",
-    "Naska " : 	b"\xD7\x24",
-    "Power " : 	b"\xD7\x25",
-    "Prison " : 	b"\xD7\x26",
-    "Play " : 	b"\xD7\x27",
-    "Panther's " : 	b"\xD7\x28",
-    "Rob's " : 	b"\xD7\x29",
-    "Recently " : 	b"\xD7\x2A",
-    "Restores " : 	b"\xD7\x2B",
-    "Right " : 	b"\xD7\x2C",
-    "Russian " : 	b"\xD7\x2D",
-    "Rofsky " : 	b"\xD7\x2E",
-    "Rearrange " : 	b"\xD7\x2F",
-    "Special " : 	b"\xD7\x30",
-    "Spin " : 	b"\xD7\x31",
-    "Seaside " : 	b"\xD7\x32",
-    "She's " : 	b"\xD7\x33",
-    "Shall " : 	b"\xD7\x34",
-    "Sorry " : 	b"\xD7\x35",
-    "Select " : 	b"\xD7\x36",
-    "Show " : 	b"\xD7\x37",
-    "Soon " : 	b"\xD7\x38",
-    "Will! " : 	b"\xD7\x39",
-    "Will... " : 	b"\xD7\x3A",
-    "Tell " : 	b"\xD7\x3B",
-    "Uses " : 	b"\xD7\x3C",
-    "Wind " : 	b"\xD7\x3D",
-    "We'll " : 	b"\xD7\x3E",
-    "We're " : 	b"\xD7\x3F",
-    "With " : 	b"\xD7\x40",
-    "We've " : 	b"\xD7\x41",
-    "Wait " : 	b"\xD7\x42",
-    "Watermia. " : 	b"\xD7\x43",
-    "always " : 	b"\xD7\x44",
-    "approaching " : 	b"\xD7\x45",
-    "animals " : 	b"\xD7\x46",
-    "almost " : 	b"\xD7\x47",
-    "also " : 	b"\xD7\x48",
-    "anything. " : 	b"\xD7\x49",
-    "abolition " : 	b"\xD7\x4A",
-    "breath " : 	b"\xD7\x4B",
-    "birthday " : 	b"\xD7\x4C",
-    "best " : 	b"\xD7\x4D",
-    "bring " : 	b"\xD7\x4E",
-    "bouquet " : 	b"\xD7\x4F",
-    "better " : 	b"\xD7\x50",
-    "behind " : 	b"\xD7\x51",
-    "change " : 	b"\xD7\x52",
-    "castle " : 	b"\xD7\x53",
-    "called " : 	b"\xD7\x54",
-    "comet's " : 	b"\xD7\x55",
-    "condition. " : 	b"\xD7\x56",
-    "care " : 	b"\xD7\x57",
-    "door " : 	b"\xD7\x58",
-    "destroyed " : 	b"\xD7\x59",
-    "disappeared " : 	b"\xD7\x5A",
-    "discovered " : 	b"\xD7\x5B",
-    "dark " : 	b"\xD7\x5C",
-    "ever " : 	b"\xD7\x5D",
-    "elevator " : 	b"\xD7\x5E",
-    "explorer. " : 	b"\xD7\x5F",
-    "eyes " : 	b"\xD7\x60",
-    "first " : 	b"\xD7\x61",
-    "fish " : 	b"\xD7\x62",
-    "followed " : 	b"\xD7\x63",
-    "fountain " : 	b"\xD7\x64",
-    "floor " : 	b"\xD7\x65",
-    "finally " : 	b"\xD7\x66",
-    "father " : 	b"\xD7\x67",
-    "flower " : 	b"\xD7\x68",
-    "forced " : 	b"\xD7\x69",
-    "forget " : 	b"\xD7\x6A",
-    "fate " : 	b"\xD7\x6B",
-    "girl " : 	b"\xD7\x6C",
-    "gets " : 	b"\xD7\x6D",
-    "guess " : 	b"\xD7\x6E",
-    "girl's " : 	b"\xD7\x6F",
-    "house " : 	b"\xD7\x70",
-    "hope " : 	b"\xD7\x71",
-    "home " : 	b"\xD7\x72",
-    "here " : 	b"\xD7\x73",
-    "here. " : 	b"\xD7\x74",
-    "home! " : 	b"\xD7\x75",
-    "happen.... " : 	b"\xD7\x76",
-    "houses " : 	b"\xD7\x77",
-    "inventing " : 	b"\xD7\x78",
-    "last " : 	b"\xD7\x79",
-    "lost " : 	b"\xD7\x7A",
-    "language. " : 	b"\xD7\x7B",
-    "list " : 	b"\xD7\x7C",
-    "life. " : 	b"\xD7\x7D",
-    "laborer " : 	b"\xD7\x7E",
-    "letter " : 	b"\xD7\x7F",
-    "looked " : 	b"\xD7\x80",
-    "lose " : 	b"\xD7\x81",
-    "left-hand " : 	b"\xD7\x82",
-    "mushrooms " : 	b"\xD7\x83",
-    "make " : 	b"\xD7\x84",
-    "mother " : 	b"\xD7\x85",
-    "merchants " : 	b"\xD7\x86",
-    "meet " : 	b"\xD7\x87",
-    "most " : 	b"\xD7\x88",
-    "only " : 	b"\xD7\x89",
-    "ocean " : 	b"\xD7\x8A",
-    "opened " : 	b"\xD7\x8B",
-    "outskirts " : 	b"\xD7\x8C",
-    "president " : 	b"\xD7\x8D",
-    "please " : 	b"\xD7\x8E",
-    "probably " : 	b"\xD7\x8F",
-    "place " : 	b"\xD7\x90",
-    "prison " : 	b"\xD7\x91",
-    "pretty " : 	b"\xD7\x92",
-    "palace " : 	b"\xD7\x93",
-    "right " : 	b"\xD7\x94",
-    "really " : 	b"\xD7\x95",
-    "returned " : 	b"\xD7\x96",
-    "running " : 	b"\xD7\x97",
-    "ruins " : 	b"\xD7\x98",
-    "right. " : 	b"\xD7\x99",
-    "ruins, " : 	b"\xD7\x9A",
-    "road " : 	b"\xD7\x9B",
-    "rest " : 	b"\xD7\x9C",
-    "stone " : 	b"\xD7\x9D",
-    "seem " : 	b"\xD7\x9E",
-    "scattered " : 	b"\xD7\x9F",
-    "seemed " : 	b"\xD7\xA0",
-    "softly " : 	b"\xD7\xA1",
-    "soldiers " : 	b"\xD7\xA2",
-    "shape " : 	b"\xD7\xA3",
-    "since " : 	b"\xD7\xA4",
-    "surprised " : 	b"\xD7\xA5",
-    "sure " : 	b"\xD7\xA6",
-    "seen " : 	b"\xD7\xA7",
-    "shouldn't " : 	b"\xD7\xA8",
-    "somewhere " : 	b"\xD7\xA9",
-    "times " : 	b"\xD7\xAA",
-    "they " : 	b"\xD7\xAB",
-    "talk " : 	b"\xD7\xAC",
-    "tell " : 	b"\xD7\xAD",
-    "townspeople " : 	b"\xD7\xAE",
-    "taken " : 	b"\xD7\xAF",
-    "they're " : 	b"\xD7\xB0",
-    "travelling " : 	b"\xD7\xB1",
-    "trying " : 	b"\xD7\xB2",
-    "turned " : 	b"\xD7\xB3",
-    "temporary " : 	b"\xD7\xB4",
-    "than " : 	b"\xD7\xB5",
-    "then " : 	b"\xD7\xB6",
-    "too, " : 	b"\xD7\xB7",
-    "thousands " : 	b"\xD7\xB8",
-    "turn " : 	b"\xD7\xB9",
-    "treasure, " : 	b"\xD7\xBA",
-    "used " : 	b"\xD7\xBB",
-    "until " : 	b"\xD7\xBC",
-    "village. " : 	b"\xD7\xBD",
-    "vampire " : 	b"\xD7\xBE",
-    "while " : 	b"\xD7\xBF",
-    "water " : 	b"\xD7\xC0",
-    "went " : 	b"\xD7\xC1",
-    "wondered " : 	b"\xD7\xC2",
-    "written " : 	b"\xD7\xC3",
-    "woman " : 	b"\xD7\xC4",
-    "wind " : 	b"\xD7\xC5",
-    "years " : 	b"\xD7\xC6",
-    "you. " : 	b"\xD7\xC7"
+    "Attack ": b"\xD6\x00",
+    "Angel ": b"\xD6\x01",
+    "After ": b"\xD6\x02",
+    "Aura ": b"\xD6\x03",
+    "Ankor ": b"\xD6\x04",
+    "Black ": b"\xD6\x05",
+    "Bill: ": b"\xD6\x06",
+    "Crystal ": b"\xD6\x07",
+    "City ": b"\xD6\x08",
+    "Come ": b"\xD6\x09",
+    "Condor's ": b"\xD6\x0A",
+    "Change ": b"\xD6\x0B",
+    "Dark ": b"\xD6\x0C",
+    "Don't ": b"\xD6\x0D",
+    "Diamond ": b"\xD6\x0E",
+    "Drifting, ": b"\xD6\x0F",
+    "Eric: ": b"\xD6\x10",
+    "Edward ": b"\xD6\x11",
+    "Even ": b"\xD6\x12",
+    "Elder2f ": b"\xD6\x13",
+    "Earth ": b"\xD6\x14",
+    "Freedan's ": b"\xD6\x15",
+    "Great ": b"\xD6\x16",
+    "Grandma ": b"\xD6\x17",
+    "Good. ": b"\xD6\x18",
+    "Gold ": b"\xD6\x19",
+    "Grandpa ": b"\xD6\x1A",
+    "Hieroglyph ": b"\xD6\x1B",
+    "Hey, ": b"\xD6\x1C",
+    "It's ": b"\xD6\x1D",
+    "Inca ": b"\xD6\x1E",
+    "I'll ": b"\xD6\x1F",
+    "I've ": b"\xD6\x20",
+    "Itorie ": b"\xD6\x21",
+    "Jewels ": b"\xD6\x22",
+    "Jewels! ": b"\xD6\x23",
+    "Just ": b"\xD6\x24",
+    "Kara: ": b"\xD6\x25",
+    "Kara ": b"\xD6\x26",
+    "King ": b"\xD6\x27",
+    "Knight ": b"\xD6\x28",
+    "Karen's ": b"\xD6\x29",
+    "Lilly: ": b"\xD6\x2A",
+    "Let's ": b"\xD6\x2B",
+    "Lilly ": b"\xD6\x2C",
+    "Lola's ": b"\xD6\x2D",
+    "Lola: ": b"\xD6\x2E",
+    "Mystery ": b"\xD6\x2F",
+    "Maybe ": b"\xD6\x30",
+    "Moon ": b"\xD6\x31",
+    "Man: ": b"\xD6\x32",
+    "Morris's ": b"\xD6\x33",
+    "Melody ": b"\xD6\x34",
+    "Morris: ": b"\xD6\x35",
+    "Neil: ": b"\xD6\x36",
+    "Neil's ": b"\xD6\x37",
+    "Only ": b"\xD6\x38",
+    "Once ": b"\xD6\x39",
+    "Oink ": b"\xD6\x3A",
+    "Please ": b"\xD6\x3B",
+    "Psycho ": b"\xD6\x3C",
+    "People ": b"\xD6\x3D",
+    "Prayer ": b"\xD6\x3E",
+    "Pyramid ": b"\xD6\x3F",
+    "Purification ": b"\xD6\x40",
+    "Plate ": b"\xD6\x41",
+    "Quit ": b"\xD6\x42",
+    "Rob: ": b"\xD6\x43",
+    "Rolek ": b"\xD6\x44",
+    "Soldier: ": b"\xD6\x45",
+    "Strange ": b"\xD6\x46",
+    "South ": b"\xD6\x47",
+    "Statue ": b"\xD6\x48",
+    "Somehow ": b"\xD6\x49",
+    "Sometimes ": b"\xD6\x4A",
+    "Something ": b"\xD6\x4B",
+    "Shadow's ": b"\xD6\x4C",
+    "Someone ": b"\xD6\x4D",
+    "This ": b"\xD6\x4E",
+    "Will: ": b"\xD6\x4F",
+    "There's ": b"\xD6\x50",
+    "Will's ": b"\xD6\x51",
+    "There ": b"\xD6\x52",
+    "That's ": b"\xD6\x53",
+    "Tower ": b"\xD6\x54",
+    "They ": b"\xD6\x55",
+    "Then ": b"\xD6\x56",
+    "Trip ": b"\xD6\x57",
+    "Thank ": b"\xD6\x58",
+    "Take ": b"\xD6\x59",
+    "Will. ": b"\xD6\x5A",
+    "That ": b"\xD6\x5B",
+    "Will, ": b"\xD6\x5C",
+    "They're ": b"\xD6\x5D",
+    "These ": b"\xD6\x5E",
+    "Vampire ": b"\xD6\x5F",
+    "Village. ": b"\xD6\x60",
+    "When ": b"\xD6\x61",
+    "What ": b"\xD6\x62",
+    "Well, ": b"\xD6\x63",
+    "What's ": b"\xD6\x64",
+    "Where ": b"\xD6\x65",
+    "Woman: ": b"\xD6\x66",
+    "You've ": b"\xD6\x67",
+    "Your ": b"\xD6\x68",
+    "You're ": b"\xD6\x69",
+    "Yes, ": b"\xD6\x6A",
+    "about ": b"\xD6\x6B",
+    "anything ": b"\xD6\x6C",
+    "around ": b"\xD6\x6D",
+    "another ": b"\xD6\x6E",
+    "ancient ": b"\xD6\x6F",
+    "been ": b"\xD6\x70",
+    "become ": b"\xD6\x71",
+    "body ": b"\xD6\x72",
+    "back ": b"\xD6\x73",
+    "before ": b"\xD6\x74",
+    "brought ": b"\xD6\x75",
+    "beautiful ": b"\xD6\x76",
+    "being ": b"\xD6\x77",
+    "can't ": b"\xD6\x78",
+    "come ": b"\xD6\x79",
+    "could ": b"\xD6\x7A",
+    "comet ": b"\xD6\x7B",
+    "company ": b"\xD6\x7C",
+    "children ": b"\xD6\x7D",
+    "constellation ": b"\xD6\x7E",
+    "changed ": b"\xD6\x7F",
+    "came ": b"\xD6\x80",
+    "coming ": b"\xD6\x81",
+    "don't ": b"\xD6\x82",
+    "didn't ": b"\xD6\x83",
+    "doesn't ": b"\xD6\x84",
+    "distant ": b"\xD6\x85",
+    "different ": b"\xD6\x86",
+    "demons ": b"\xD6\x87",
+    "destroy ": b"\xD6\x88",
+    "everyone ": b"\xD6\x89",
+    "explorer ": b"\xD6\x8A",
+    "everyone's ": b"\xD6\x8B",
+    "enemies ": b"\xD6\x8C",
+    "exposed ": b"\xD6\x8D",
+    "from ": b"\xD6\x8E",
+    "found ": b"\xD6\x8F",
+    "find ": b"\xD6\x90",
+    "feel ": b"\xD6\x91",
+    "father's ": b"\xD6\x92",
+    "going ": b"\xD6\x93",
+    "good ": b"\xD6\x94",
+    "great ": b"\xD6\x95",
+    "ground ": b"\xD6\x96",
+    "give ": b"\xD6\x97",
+    "have ": b"\xD6\x98",
+    "heard ": b"\xD6\x99",
+    "human ": b"\xD6\x9A",
+    "hear ": b"\xD6\x9B",
+    "huge ": b"\xD6\x9C",
+    "happened ": b"\xD6\x9D",
+    "hieroglyph ": b"\xD6\x9E",
+    "it's ": b"\xD6\x9F",
+    "inventory ": b"\xD6\xA0",
+    "into ": b"\xD6\xA1",
+    "inside ": b"\xD6\xA2",
+    "just ": b"\xD6\xA3",
+    "know ": b"\xD6\xA4",
+    "like ": b"\xD6\xA5",
+    "long ": b"\xD6\xA6",
+    "little ": b"\xD6\xA7",
+    "light ": b"\xD6\xA8",
+    "look ": b"\xD6\xA9",
+    "looks ": b"\xD6\xAA",
+    "looking ": b"\xD6\xAB",
+    "leave ": b"\xD6\xAC",
+    "labor ": b"\xD6\xAD",
+    "left ": b"\xD6\xAE",
+    "live ": b"\xD6\xAF",
+    "life ": b"\xD6\xB0",
+    "living ": b"\xD6\xB1",
+    "must ": b"\xD6\xB2",
+    "made ": b"\xD6\xB3",
+    "melody ": b"\xD6\xB4",
+    "move ": b"\xD6\xB5",
+    "many ": b"\xD6\xB6",
+    "more ": b"\xD6\xB7",
+    "matter ": b"\xD6\xB8",
+    "nothing ": b"\xD6\xB9",
+    "need ": b"\xD6\xBA",
+    "never ": b"\xD6\xBB",
+    "next ": b"\xD6\xBC",
+    "other ": b"\xD6\xBD",
+    "over ": b"\xD6\xBE",
+    "outside ": b"\xD6\xBF",
+    "original ": b"\xD6\xC0",
+    "people ": b"\xD6\xC1",
+    "power ": b"\xD6\xC2",
+    "present. ": b"\xD6\xC3",
+    "playing ": b"\xD6\xC4",
+    "raised ": b"\xD6\xC5",
+    "right-hand ": b"\xD6\xC6",
+    "strange ": b"\xD6\xC7",
+    "something ": b"\xD6\xC8",
+    "statue ": b"\xD6\xC9",
+    "should ": b"\xD6\xCA",
+    "started ": b"\xD6\xCB",
+    "seems ": b"\xD6\xCC",
+    "same ": b"\xD6\xCD",
+    "such ": b"\xD6\xCE",
+    "someone ": b"\xD6\xCF",
+    "some ": b"\xD6\xD0",
+    "save ": b"\xD6\xD1",
+    "statues ": b"\xD6\xD2",
+    "still ": b"\xD6\xD3",
+    "said ": b"\xD6\xD4",
+    "stands ": b"\xD6\xD5",
+    "this ": b"\xD6\xD6",
+    "that ": b"\xD6\xD7",
+    "thought ": b"\xD6\xD8",
+    "there ": b"\xD6\xD9",
+    "think ": b"\xD6\xDA",
+    "there's ": b"\xD6\xDB",
+    "through ": b"\xD6\xDC",
+    "tried ": b"\xD6\xDD",
+    "terrible ": b"\xD6\xDE",
+    "time ": b"\xD6\xDF",
+    "things ": b"\xD6\xE0",
+    "their ": b"\xD6\xE1",
+    "town ": b"\xD6\xE2",
+    "thing ": b"\xD6\xE3",
+    "these ": b"\xD6\xE4",
+    "temple ": b"\xD6\xE5",
+    "them ": b"\xD6\xE6",
+    "take ": b"\xD6\xE7",
+    "turned, ": b"\xD6\xE8",
+    "understand ": b"\xD6\xE9",
+    "under ": b"\xD6\xEA",
+    "underwater ": b"\xD6\xEB",
+    "village ": b"\xD6\xEC",
+    "very ": b"\xD6\xED",
+    "voice ": b"\xD6\xEE",
+    "will ": b"\xD6\xEF",
+    "with ": b"\xD6\xF0",
+    "want ": b"\xD6\xF1",
+    "were ": b"\xD6\xF2",
+    "would ": b"\xD6\xF3",
+    "where ": b"\xD6\xF4",
+    "world ": b"\xD6\xF5",
+    "when ": b"\xD6\xF6",
+    "what ": b"\xD6\xF7",
+    "without ": b"\xD6\xF8",
+    "wonder ": b"\xD6\xF9",
+    "won't ": b"\xD6\xFA",
+    "wouldn't ": b"\xD6\xFB",
+    "wanted ": b"\xD6\xFC",
+    "waiting ": b"\xD6\xFD",
+    "your ": b"\xD6\xFE",
+    "you're ": b"\xD6\xFF",
+    "1994 ": b"\xD7\x00",
+    "Actually, ": b"\xD7\x01",
+    "Button ": b"\xD7\x02",
+    "Buttons ": b"\xD7\x03",
+    "Back ": b"\xD7\x04",
+    "Child: ": b"\xD7\x05",
+    "Defeating ": b"\xD7\x06",
+    "Didn't ": b"\xD7\x07",
+    "Desert ": b"\xD7\x08",
+    "Erasquez: ": b"\xD7\x09",
+    "Elder ": b"\xD7\x0A",
+    "Earth's ": b"\xD7\x0B",
+    "Eric's ": b"\xD7\x0C",
+    "Everybody ": b"\xD7\x0D",
+    "Flute: ": b"\xD7\x0E",
+    "First ": b"\xD7\x0F",
+    "Firebird, ": b"\xD7\x10",
+    "From ": b"\xD7\x11",
+    "Gaia, ": b"\xD7\x12",
+    "Gorgon ": b"\xD7\x13",
+    "Have ": b"\xD7\x14",
+    "Hey! ": b"\xD7\x15",
+    "Istar's ": b"\xD7\x16",
+    "Ishtar's ": b"\xD7\x17",
+    "Lilly's ": b"\xD7\x18",
+    "Larai ": b"\xD7\x19",
+    "Looking ": b"\xD7\x1A",
+    "Main ": b"\xD7\x1B",
+    "Man's ": b"\xD7\x1C",
+    "Memory ": b"\xD7\x1D",
+    "Mountain ": b"\xD7\x1E",
+    "Morris ": b"\xD7\x1F",
+    "Many ": b"\xD7\x20",
+    "Native ": b"\xD7\x21",
+    "Native's ": b"\xD7\x22",
+    "Neil ": b"\xD7\x23",
+    "Naska ": b"\xD7\x24",
+    "Power ": b"\xD7\x25",
+    "Prison ": b"\xD7\x26",
+    "Play ": b"\xD7\x27",
+    "Panther's ": b"\xD7\x28",
+    "Rob's ": b"\xD7\x29",
+    "Recently ": b"\xD7\x2A",
+    "Restores ": b"\xD7\x2B",
+    "Right ": b"\xD7\x2C",
+    "Russian ": b"\xD7\x2D",
+    "Rofsky ": b"\xD7\x2E",
+    "Rearrange ": b"\xD7\x2F",
+    "Special ": b"\xD7\x30",
+    "Spin ": b"\xD7\x31",
+    "Seaside ": b"\xD7\x32",
+    "She's ": b"\xD7\x33",
+    "Shall ": b"\xD7\x34",
+    "Sorry ": b"\xD7\x35",
+    "Select ": b"\xD7\x36",
+    "Show ": b"\xD7\x37",
+    "Soon ": b"\xD7\x38",
+    "Will! ": b"\xD7\x39",
+    "Will... ": b"\xD7\x3A",
+    "Tell ": b"\xD7\x3B",
+    "Uses ": b"\xD7\x3C",
+    "Wind ": b"\xD7\x3D",
+    "We'll ": b"\xD7\x3E",
+    "We're ": b"\xD7\x3F",
+    "With ": b"\xD7\x40",
+    "We've ": b"\xD7\x41",
+    "Wait ": b"\xD7\x42",
+    "Watermia. ": b"\xD7\x43",
+    "always ": b"\xD7\x44",
+    "approaching ": b"\xD7\x45",
+    "animals ": b"\xD7\x46",
+    "almost ": b"\xD7\x47",
+    "also ": b"\xD7\x48",
+    "anything. ": b"\xD7\x49",
+    "abolition ": b"\xD7\x4A",
+    "breath ": b"\xD7\x4B",
+    "birthday ": b"\xD7\x4C",
+    "best ": b"\xD7\x4D",
+    "bring ": b"\xD7\x4E",
+    "bouquet ": b"\xD7\x4F",
+    "better ": b"\xD7\x50",
+    "behind ": b"\xD7\x51",
+    "change ": b"\xD7\x52",
+    "castle ": b"\xD7\x53",
+    "called ": b"\xD7\x54",
+    "comet's ": b"\xD7\x55",
+    "condition. ": b"\xD7\x56",
+    "care ": b"\xD7\x57",
+    "door ": b"\xD7\x58",
+    "destroyed ": b"\xD7\x59",
+    "disappeared ": b"\xD7\x5A",
+    "discovered ": b"\xD7\x5B",
+    "dark ": b"\xD7\x5C",
+    "ever ": b"\xD7\x5D",
+    "elevator ": b"\xD7\x5E",
+    "explorer. ": b"\xD7\x5F",
+    "eyes ": b"\xD7\x60",
+    "first ": b"\xD7\x61",
+    "fish ": b"\xD7\x62",
+    "followed ": b"\xD7\x63",
+    "fountain ": b"\xD7\x64",
+    "floor ": b"\xD7\x65",
+    "finally ": b"\xD7\x66",
+    "father ": b"\xD7\x67",
+    "flower ": b"\xD7\x68",
+    "forced ": b"\xD7\x69",
+    "forget ": b"\xD7\x6A",
+    "fate ": b"\xD7\x6B",
+    "girl ": b"\xD7\x6C",
+    "gets ": b"\xD7\x6D",
+    "guess ": b"\xD7\x6E",
+    "girl's ": b"\xD7\x6F",
+    "house ": b"\xD7\x70",
+    "hope ": b"\xD7\x71",
+    "home ": b"\xD7\x72",
+    "here ": b"\xD7\x73",
+    "here. ": b"\xD7\x74",
+    "home! ": b"\xD7\x75",
+    "happen.... ": b"\xD7\x76",
+    "houses ": b"\xD7\x77",
+    "inventing ": b"\xD7\x78",
+    "last ": b"\xD7\x79",
+    "lost ": b"\xD7\x7A",
+    "language. ": b"\xD7\x7B",
+    "list ": b"\xD7\x7C",
+    "life. ": b"\xD7\x7D",
+    "laborer ": b"\xD7\x7E",
+    "letter ": b"\xD7\x7F",
+    "looked ": b"\xD7\x80",
+    "lose ": b"\xD7\x81",
+    "left-hand ": b"\xD7\x82",
+    "mushrooms ": b"\xD7\x83",
+    "make ": b"\xD7\x84",
+    "mother ": b"\xD7\x85",
+    "merchants ": b"\xD7\x86",
+    "meet ": b"\xD7\x87",
+    "most ": b"\xD7\x88",
+    "only ": b"\xD7\x89",
+    "ocean ": b"\xD7\x8A",
+    "opened ": b"\xD7\x8B",
+    "outskirts ": b"\xD7\x8C",
+    "president ": b"\xD7\x8D",
+    "please ": b"\xD7\x8E",
+    "probably ": b"\xD7\x8F",
+    "place ": b"\xD7\x90",
+    "prison ": b"\xD7\x91",
+    "pretty ": b"\xD7\x92",
+    "palace ": b"\xD7\x93",
+    "right ": b"\xD7\x94",
+    "really ": b"\xD7\x95",
+    "returned ": b"\xD7\x96",
+    "running ": b"\xD7\x97",
+    "ruins ": b"\xD7\x98",
+    "right. ": b"\xD7\x99",
+    "ruins, ": b"\xD7\x9A",
+    "road ": b"\xD7\x9B",
+    "rest ": b"\xD7\x9C",
+    "stone ": b"\xD7\x9D",
+    "seem ": b"\xD7\x9E",
+    "scattered ": b"\xD7\x9F",
+    "seemed ": b"\xD7\xA0",
+    "softly ": b"\xD7\xA1",
+    "soldiers ": b"\xD7\xA2",
+    "shape ": b"\xD7\xA3",
+    "since ": b"\xD7\xA4",
+    "surprised ": b"\xD7\xA5",
+    "sure ": b"\xD7\xA6",
+    "seen ": b"\xD7\xA7",
+    "shouldn't ": b"\xD7\xA8",
+    "somewhere ": b"\xD7\xA9",
+    "times ": b"\xD7\xAA",
+    "they ": b"\xD7\xAB",
+    "talk ": b"\xD7\xAC",
+    "tell ": b"\xD7\xAD",
+    "townspeople ": b"\xD7\xAE",
+    "taken ": b"\xD7\xAF",
+    "they're ": b"\xD7\xB0",
+    "travelling ": b"\xD7\xB1",
+    "trying ": b"\xD7\xB2",
+    "turned ": b"\xD7\xB3",
+    "temporary ": b"\xD7\xB4",
+    "than ": b"\xD7\xB5",
+    "then ": b"\xD7\xB6",
+    "too, ": b"\xD7\xB7",
+    "thousands ": b"\xD7\xB8",
+    "turn ": b"\xD7\xB9",
+    "treasure, ": b"\xD7\xBA",
+    "used ": b"\xD7\xBB",
+    "until ": b"\xD7\xBC",
+    "village. ": b"\xD7\xBD",
+    "vampire ": b"\xD7\xBE",
+    "while ": b"\xD7\xBF",
+    "water ": b"\xD7\xC0",
+    "went ": b"\xD7\xC1",
+    "wondered ": b"\xD7\xC2",
+    "written ": b"\xD7\xC3",
+    "woman ": b"\xD7\xC4",
+    "wind ": b"\xD7\xC5",
+    "years ": b"\xD7\xC6",
+    "you. ": b"\xD7\xC7"
 }
 
 text_letters = {
-    "?" : 	b"\x0D",
-    "'" : 	b"\x0E",
-    "0" : 	b"\x20",
-    "1" : 	b"\x21",
-    "2" : 	b"\x22",
-    "3" : 	b"\x23",
-    "4" : 	b"\x24",
-    "5" : 	b"\x25",
-    "6" : 	b"\x26",
-    "7" : 	b"\x27",
-    "8" : 	b"\x28",
-    "9" : 	b"\x29",
-    "." : 	b"\x2A",
-    "," : 	b"\x2B",
-    ">" : 	b"\x2C",
-#    '"' : 	b"\x2D",
-#    '"' : 	b"\x2E",
-    ":" : 	b"\x2F",
-    "A" : 	b"\x40",
-    "B" : 	b"\x41",
-    "C" : 	b"\x42",
-    "D" : 	b"\x43",
-    "E" : 	b"\x44",
-    "F" : 	b"\x45",
-    "G" : 	b"\x46",
-    "H" : 	b"\x47",
-    "I" : 	b"\x48",
-    "J" : 	b"\x49",
-    "K" : 	b"\x4A",
-    "L" : 	b"\x4B",
-    "M" : 	b"\x4C",
-    "N" : 	b"\x4D",
-    "O" : 	b"\x4E",
-    "!" : 	b"\x4F",
-    "P" : 	b"\x60",
-    "Q" : 	b"\x61",
-    "R" : 	b"\x62",
-    "S" : 	b"\x63",
-    "T" : 	b"\x64",
-    "U" : 	b"\x65",
-    "V" : 	b"\x66",
-    "W" : 	b"\x67",
-    "X" : 	b"\x68",
-    "Y" : 	b"\x69",
-    "Z" : 	b"\x6A",
-    "/" : 	b"\x6B",
-    "*" : 	b"\x6C",
-    "-" : 	b"\x6D",
-    "(" : 	b"\x6E",
-    ")" : 	b"\x6F",
-    "a" : 	b"\x80",
-    "b" : 	b"\x81",
-    "c" : 	b"\x82",
-    "d" : 	b"\x83",
-    "e" : 	b"\x84",
-    "f" : 	b"\x85",
-    "g" : 	b"\x86",
-    "h" : 	b"\x87",
-    "i" : 	b"\x88",
-    "j" : 	b"\x89",
-    "k" : 	b"\x8A",
-    "l" : 	b"\x8B",
-    "m" : 	b"\x8C",
-    "n" : 	b"\x8D",
-    "o" : 	b"\x8E",
-    "p" : 	b"\xA0",
-    "q" : 	b"\xA1",
-    "r" : 	b"\xA2",
-    "s" : 	b"\xA3",
-    "t" : 	b"\xA4",
-    "u" : 	b"\xA5",
-    "v" : 	b"\xA6",
-    "w" : 	b"\xA7",
-    "x" : 	b"\xA8",
-    "y" : 	b"\xA9",
-    "z" : 	b"\xAA",
-    "," : 	b"\xAB",
-    " " : 	b"\xAC",
-    "|" : 	b"\xCF"    # Prompts for advance
+    "?": b"\x0D",
+    "'": b"\x0E",
+    "0": b"\x20",
+    "1": b"\x21",
+    "2": b"\x22",
+    "3": b"\x23",
+    "4": b"\x24",
+    "5": b"\x25",
+    "6": b"\x26",
+    "7": b"\x27",
+    "8": b"\x28",
+    "9": b"\x29",
+    ".": b"\x2A",
+    ",": b"\x2B",
+    ">": b"\x2C",
+    #    '"' : 	b"\x2D",
+    #    '"' : 	b"\x2E",
+    ":": b"\x2F",
+    "A": b"\x40",
+    "B": b"\x41",
+    "C": b"\x42",
+    "D": b"\x43",
+    "E": b"\x44",
+    "F": b"\x45",
+    "G": b"\x46",
+    "H": b"\x47",
+    "I": b"\x48",
+    "J": b"\x49",
+    "K": b"\x4A",
+    "L": b"\x4B",
+    "M": b"\x4C",
+    "N": b"\x4D",
+    "O": b"\x4E",
+    "!": b"\x4F",
+    "P": b"\x60",
+    "Q": b"\x61",
+    "R": b"\x62",
+    "S": b"\x63",
+    "T": b"\x64",
+    "U": b"\x65",
+    "V": b"\x66",
+    "W": b"\x67",
+    "X": b"\x68",
+    "Y": b"\x69",
+    "Z": b"\x6A",
+    "/": b"\x6B",
+    "*": b"\x6C",
+    "-": b"\x6D",
+    "(": b"\x6E",
+    ")": b"\x6F",
+    "a": b"\x80",
+    "b": b"\x81",
+    "c": b"\x82",
+    "d": b"\x83",
+    "e": b"\x84",
+    "f": b"\x85",
+    "g": b"\x86",
+    "h": b"\x87",
+    "i": b"\x88",
+    "j": b"\x89",
+    "k": b"\x8A",
+    "l": b"\x8B",
+    "m": b"\x8C",
+    "n": b"\x8D",
+    "o": b"\x8E",
+    "p": b"\xA0",
+    "q": b"\xA1",
+    "r": b"\xA2",
+    "s": b"\xA3",
+    "t": b"\xA4",
+    "u": b"\xA5",
+    "v": b"\xA6",
+    "w": b"\xA7",
+    "x": b"\xA8",
+    "y": b"\xA9",
+    "z": b"\xAA",
+    ",": b"\xAB",
+    " ": b"\xAC",
+    "|": b"\xCF"  # Prompts for advance
 }
 
 text_words_inv = {v: k for k, v in text_words.items()}
 text_letters_inv = {v: k for k, v in text_letters.items()}
 
-def get_text(addr,f,rom_offset=0):
+
+def get_text(addr, f, rom_offset=0):
     str_encoded = ""
-    f.seek(addr+rom_offset)
+    f.seek(addr + rom_offset)
     char = ""
     bytes = 0
     while char != b"\xC0" and char != b"\xCA":
         char = f.read(1)
         str_encoded += char
         bytes += 1
 
     str_decoded = ""
     i = 0
     while i < len(str_encoded):
         byte = str_encoded[i]
         i += 1
-        if byte not in [b"\xD3",b"\xC0",b"\xCA"]:
-            if byte in [b"\xD6",b"\xD7"]:
+        if byte not in [b"\xD3", b"\xC0", b"\xCA"]:
+            if byte in [b"\xD6", b"\xD7"]:
                 word = byte + str_encoded[i]
                 i += 1
                 if word in text_words_inv:
                     str_decoded += text_words_inv[word]
-                #else:
-                    #print "WARNING: Word not recognized >>", word
+                # else:
+                # print "WARNING: Word not recognized >>", word
             elif byte in text_letters_inv:
                 str_decoded += text_letters_inv[byte]
             elif byte not in [b"\xcb"]:
                 str_decoded += "?"
-                #print "WARNING: Letter not recognized >>", byte
+                # print "WARNING: Letter not recognized >>", byte
 
-    #print str_decoded
+    # print str_decoded
     return [str_decoded, bytes]
 
-def encode(unencoded_str,full_box=False):
+
+def encode(unencoded_str, full_box=False):
     words = []
     word = ""
     i = 0
     while i < len(unencoded_str):
         char = unencoded_str[i]
         if char == "|":
             words.append(word)
             words.append(char)
             word = ""
         else:
             word += char
-            if char == " " or i == len(unencoded_str)-1:
+            if char == " " or i == len(unencoded_str) - 1:
                 words.append(word)
                 word = ""
         i += 1
 
-    #print words
+    # print words
     if full_box:
         str_encoded = b"\xd3"
     else:
         str_encoded = b""
     text_width = 0
 
     for word in words:
@@ -623,9 +625,9 @@
                     str_encoded += b"\x0D"
                     print("WARNING: Character not recognized >>", char)
                 i += 1
 
     if full_box:
         str_encoded += b"\xc0"
 
-    #print str_encoded, len(str_encoded)
+    # print str_encoded, len(str_encoded)
     return str_encoded
```

### Comparing `iog-randomizer-4.7.2.2/randomizer/table_dialogue.txt` & `iog_randomizer-5.0.0/src/iog_randomizer/randomizer/table_dialogue.txt`

 * *Files identical despite different names*

### Comparing `iog-randomizer-4.7.2.2/randomizer/table_invtext.txt` & `iog_randomizer-5.0.0/src/iog_randomizer/randomizer/table_invtext.txt`

 * *Files identical despite different names*

