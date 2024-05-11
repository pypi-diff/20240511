# Comparing `tmp/musical_games-0.8.3.tar.gz` & `tmp/musical_games-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musical_games-0.8.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "musical_games-0.8.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `musical_games-0.8.3.tar` & `musical_games-0.8.4.tar`

### file list

```diff
@@ -1,115 +1,115 @@
--rw-r--r--   0        0        0      511 2024-04-07 08:37:11.575406 musical_games-0.8.3/.coveragerc
--rw-r--r--   0        0        0      292 2016-07-03 13:55:58.881844 musical_games-0.8.3/.editorconfig
--rw-r--r--   0        0        0    10359 2024-04-07 08:37:38.227407 musical_games-0.8.3/.gitchangelog.rc
--rw-r--r--   0        0        0      271 2018-09-16 09:02:35.270504 musical_games-0.8.3/.gitchangelog.tpl
--rw-r--r--   0        0        0     1166 2024-04-07 08:37:55.851407 musical_games-0.8.3/.gitignore
--rw-r--r--   0        0        0      419 2024-04-07 08:38:05.135407 musical_games-0.8.3/.travis.yml
--rw-r--r--   0        0        0     2067 2024-05-04 19:06:22.708059 musical_games-0.8.3/CHANGELOG.rst
--rw-r--r--   0        0        0     7707 2016-07-03 13:55:58.881844 musical_games-0.8.3/LICENSE
--rw-r--r--   0        0        0     4770 2024-04-13 15:08:13.743551 musical_games-0.8.3/Makefile
--rw-r--r--   0        0        0     3103 2024-04-13 13:04:50.799749 musical_games-0.8.3/README.rst
--rw-r--r--   0        0        0     6790 2016-07-03 13:55:58.881844 musical_games-0.8.3/docs/Makefile
--rw-r--r--   0        0        0      154 2018-08-01 14:00:31.251630 musical_games-0.8.3/docs/authors.rst
--rwxr-xr-x   0        0        0     7987 2024-04-09 10:08:14.002483 musical_games-0.8.3/docs/conf.py
--rw-r--r--   0        0        0     3219 2018-08-01 14:00:31.247630 musical_games-0.8.3/docs/contributing.rst
--rw-r--r--   0        0        0      119 2018-08-01 14:00:31.251630 musical_games-0.8.3/docs/history.rst
--rw-r--r--   0        0        0      516 2018-08-01 14:00:31.247630 musical_games-0.8.3/docs/index.rst
--rw-r--r--   0        0        0      209 2018-08-01 14:00:31.247630 musical_games-0.8.3/docs/installation.rst
--rw-r--r--   0        0        0     6473 2016-07-03 13:55:58.881844 musical_games-0.8.3/docs/make.bat
--rw-r--r--   0        0        0       76 2018-08-01 14:00:31.247630 musical_games-0.8.3/docs/modules.rst
--rw-r--r--   0        0        0      962 2018-08-01 14:00:31.251630 musical_games-0.8.3/docs/musical_games.converters.rst
--rw-r--r--   0        0        0     1387 2018-08-01 14:00:31.247630 musical_games-0.8.3/docs/musical_games.dice_games.lilypond.rst
--rw-r--r--   0        0        0     1276 2018-08-01 14:00:31.247630 musical_games-0.8.3/docs/musical_games.dice_games.rst
--rw-r--r--   0        0        0      749 2018-08-01 14:00:31.247630 musical_games-0.8.3/docs/musical_games.rst
--rw-r--r--   0        0        0       27 2018-08-01 14:00:31.247630 musical_games-0.8.3/docs/readme.rst
--rw-r--r--   0        0        0       87 2018-08-01 14:00:31.247630 musical_games-0.8.3/docs/usage.rst
--rwxr-xr-x   0        0        0      191 2024-04-09 10:08:14.006483 musical_games-0.8.3/musical_games/__init__.py
--rw-r--r--   0        0        0      518 2024-04-09 10:08:14.002483 musical_games-0.8.3/musical_games/__version__.py
--rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.8.3/musical_games/data/__init__.py
--rw-r--r--   0        0        0      140 2024-04-09 14:44:21.674751 musical_games-0.8.3/musical_games/data/dice_games/__init__.py
--rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.8.3/musical_games/data/dice_games/cpe_bach_counterpoint/__init__.py
--rw-r--r--   0        0        0     2435 2024-04-13 12:41:41.563787 musical_games-0.8.3/musical_games/data/dice_games/cpe_bach_counterpoint/bars.csv
--rw-r--r--   0        0        0      882 2024-04-13 12:41:41.563787 musical_games-0.8.3/musical_games/data/dice_games/cpe_bach_counterpoint/bars_bass.csv
--rw-r--r--   0        0        0     1407 2024-04-13 12:41:41.563787 musical_games-0.8.3/musical_games/data/dice_games/cpe_bach_counterpoint/bars_treble.csv
--rw-r--r--   0        0        0     1426 2024-05-01 10:00:27.942474 musical_games-0.8.3/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     1773 2024-05-01 10:01:07.542475 musical_games-0.8.3/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     2987 2024-05-04 11:52:35.602498 musical_games-0.8.3/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0      524 2024-05-01 10:01:25.466475 musical_games-0.8.3/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_bar.ly
--rw-r--r--   0        0        0      623 2024-05-01 10:01:48.778476 musical_games-0.8.3/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_dice_table_element.ly
--rw-r--r--   0        0        0      140 2024-04-30 09:20:04.502864 musical_games-0.8.3/musical_games/data/dice_games/gerlach_scottish_dance/__init__.py
--rw-r--r--   0        0        0     2217 2024-05-01 12:32:39.650622 musical_games-0.8.3/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     8375 2024-05-03 10:05:04.980883 musical_games-0.8.3/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     6391 2024-05-04 11:52:35.590498 musical_games-0.8.3/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0     1208 2024-05-01 12:32:39.650622 musical_games-0.8.3/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/single_bar.ly
--rw-r--r--   0        0        0     2344 2024-05-01 12:32:39.650622 musical_games-0.8.3/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/single_dice_table_element.ly
--rw-r--r--   0        0        0    18686 2024-05-01 09:40:49.846455 musical_games-0.8.3/musical_games/data/dice_games/gerlach_scottish_dance/scottish_dance_bars.csv
--rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.8.3/musical_games/data/dice_games/kirnberger_menuet_trio/__init__.py
--rw-r--r--   0        0        0     2515 2024-05-01 10:02:26.562476 musical_games-0.8.3/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     6430 2024-05-01 10:02:36.282477 musical_games-0.8.3/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     4303 2024-05-04 11:52:35.610498 musical_games-0.8.3/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0     1115 2024-05-01 10:04:40.982478 musical_games-0.8.3/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_bar.ly
--rw-r--r--   0        0        0     1313 2024-05-01 10:04:40.990478 musical_games-0.8.3/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_dice_table_element.ly
--rw-r--r--   0        0        0     5346 2024-04-16 05:05:56.478852 musical_games-0.8.3/musical_games/data/dice_games/kirnberger_menuet_trio/menuet_bars.csv
--rw-r--r--   0        0        0     3901 2024-04-13 12:41:41.563787 musical_games-0.8.3/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_lh.txt
--rw-r--r--   0        0        0     2059 2024-04-13 12:41:41.563787 musical_games-0.8.3/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_rh.txt
--rw-r--r--   0        0        0      154 2024-04-13 12:41:41.563787 musical_games-0.8.3/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/readme
--rw-r--r--   0        0        0     9117 2024-04-13 12:41:41.563787 musical_games-0.8.3/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_lh.txt
--rw-r--r--   0        0        0     2453 2024-04-13 12:41:41.563787 musical_games-0.8.3/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_rh.txt
--rw-r--r--   0        0        0    10956 2024-04-13 12:41:41.563787 musical_games-0.8.3/musical_games/data/dice_games/kirnberger_menuet_trio/trio_bars.csv
--rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.8.3/musical_games/data/dice_games/kirnberger_polonaise/__init__.py
--rw-r--r--   0        0        0     2867 2024-05-01 10:06:57.106481 musical_games-0.8.3/musical_games/data/dice_games/kirnberger_polonaise/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     4350 2024-05-01 10:06:57.126481 musical_games-0.8.3/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     3773 2024-05-04 11:54:20.298500 musical_games-0.8.3/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0     1634 2024-05-01 10:06:57.134481 musical_games-0.8.3/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_bar.ly
--rw-r--r--   0        0        0     2046 2024-05-01 10:06:57.086481 musical_games-0.8.3/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_dice_table_element.ly
--rw-r--r--   0        0        0    32523 2024-04-13 12:41:41.563787 musical_games-0.8.3/musical_games/data/dice_games/kirnberger_polonaise/polonaise_bars.csv
--rw-r--r--   0        0        0      140 2024-04-16 05:05:56.478852 musical_games-0.8.3/musical_games/data/dice_games/mozart_contredanse/__init__.py
--rw-r--r--   0        0        0     8219 2024-05-04 12:42:02.922546 musical_games-0.8.3/musical_games/data/dice_games/mozart_contredanse/contredanse_bars.csv
--rw-r--r--   0        0        0     1439 2024-05-04 12:39:21.850544 musical_games-0.8.3/musical_games/data/dice_games/mozart_contredanse/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     2929 2024-05-04 12:41:06.802545 musical_games-0.8.3/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     4138 2024-05-04 12:41:06.842545 musical_games-0.8.3/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0      892 2024-05-04 12:41:06.822545 musical_games-0.8.3/musical_games/data/dice_games/mozart_contredanse/lilypond/single_bar.ly
--rw-r--r--   0        0        0     1090 2024-05-04 12:41:06.854545 musical_games-0.8.3/musical_games/data/dice_games/mozart_contredanse/lilypond/single_dice_table_element.ly
--rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.8.3/musical_games/data/dice_games/mozart_waltz/__init__.py
--rw-r--r--   0        0        0     1421 2024-05-04 12:21:30.450526 musical_games-0.8.3/musical_games/data/dice_games/mozart_waltz/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     2847 2024-05-04 12:35:43.522540 musical_games-0.8.3/musical_games/data/dice_games/mozart_waltz/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     4087 2024-05-04 12:35:43.510540 musical_games-0.8.3/musical_games/data/dice_games/mozart_waltz/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0      892 2024-05-04 12:22:16.662527 musical_games-0.8.3/musical_games/data/dice_games/mozart_waltz/lilypond/single_bar.ly
--rw-r--r--   0        0        0     1090 2024-05-04 12:41:06.830545 musical_games-0.8.3/musical_games/data/dice_games/mozart_waltz/lilypond/single_dice_table_element.ly
--rw-r--r--   0        0        0     9398 2024-05-04 12:21:02.330526 musical_games-0.8.3/musical_games/data/dice_games/mozart_waltz/waltz_bars.csv
--rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.8.3/musical_games/data/dice_games/stadler_menuet_trio/__init__.py
--rw-r--r--   0        0        0     2534 2024-05-01 10:10:19.634484 musical_games-0.8.3/musical_games/data/dice_games/stadler_menuet_trio/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     6430 2024-05-01 10:11:25.454485 musical_games-0.8.3/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     4406 2024-05-04 11:52:35.630499 musical_games-0.8.3/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0     1115 2024-05-01 10:11:25.482485 musical_games-0.8.3/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_bar.ly
--rw-r--r--   0        0        0     1313 2024-05-01 10:11:25.494485 musical_games-0.8.3/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_dice_table_element.ly
--rw-r--r--   0        0        0    13676 2024-04-13 12:47:13.523778 musical_games-0.8.3/musical_games/data/dice_games/stadler_menuet_trio/menuet_bars.csv
--rw-r--r--   0        0        0     7653 2024-04-13 12:47:50.671777 musical_games-0.8.3/musical_games/data/dice_games/stadler_menuet_trio/trio_bars.csv
--rw-r--r--   0        0        0     2104 2024-05-01 12:32:39.650622 musical_games-0.8.3/musical_games/data/lilypond_utils/clef_changes.ly
--rw-r--r--   0        0        0      140 2024-04-09 12:20:58.102612 musical_games-0.8.3/musical_games/dice_games/__init__.py
--rw-r--r--   0        0        0    46961 2024-05-04 19:01:22.376069 musical_games-0.8.3/musical_games/dice_games/base.py
--rw-r--r--   0        0        0     2614 2024-04-13 13:00:55.979755 musical_games-0.8.3/musical_games/dice_games/data_csv.py
--rw-r--r--   0        0        0    17130 2024-05-04 12:38:10.242543 musical_games-0.8.3/musical_games/dice_games/dice_games.py
--rw-r--r--   0        0        0      116 2024-04-09 10:08:14.006483 musical_games-0.8.3/musical_games/external/__init__.py
--rw-r--r--   0        0        0     2969 2024-04-09 10:08:14.006483 musical_games-0.8.3/musical_games/external/base.py
--rw-r--r--   0        0        0      411 2024-04-09 10:08:14.006483 musical_games-0.8.3/musical_games/external/exceptions.py
--rw-r--r--   0        0        0      972 2024-04-09 10:08:14.006483 musical_games-0.8.3/musical_games/external/images.py
--rw-r--r--   0        0        0     3595 2024-04-15 05:04:22.919891 musical_games-0.8.3/musical_games/external/lilypond.py
--rw-r--r--   0        0        0     4729 2024-04-09 10:11:56.454487 musical_games-0.8.3/musical_games/external/midi_converters.py
--rw-r--r--   0        0        0     1142 2024-04-09 10:08:14.006483 musical_games-0.8.3/musical_games/external/utils.py
--rw-r--r--   0        0        0     2954 2024-04-09 10:11:56.486487 musical_games-0.8.3/musical_games/external/wav_converters.py
--rw-r--r--   0        0        0     4835 2024-04-18 13:39:38.231087 musical_games-0.8.3/musical_games/utils.py
--rw-r--r--   0        0        0     1117 2024-05-04 19:06:22.588059 musical_games-0.8.3/pyproject.toml
--rw-r--r--   0        0        0      116 2024-04-09 10:08:14.002483 musical_games-0.8.3/scripts/__init__.py
--rw-r--r--   0        0        0     1995 2024-05-04 18:52:13.860087 musical_games-0.8.3/scripts/demo_cpe_bach.py
--rw-r--r--   0        0        0     2364 2024-05-04 18:42:05.516108 musical_games-0.8.3/scripts/demo_gerlach_scottish_dance.py
--rw-r--r--   0        0        0     2228 2024-05-04 18:39:35.968113 musical_games-0.8.3/scripts/demo_kirnberger_meneut_trio.py
--rw-r--r--   0        0        0     1896 2024-05-04 18:37:37.884117 musical_games-0.8.3/scripts/demo_kirnberger_polonaise.py
--rw-r--r--   0        0        0     1898 2024-05-04 18:42:20.816107 musical_games-0.8.3/scripts/demo_mozart_contredanse.py
--rw-r--r--   0        0        0     1852 2024-05-04 12:36:25.506541 musical_games-0.8.3/scripts/demo_mozart_waltz.py
--rw-r--r--   0        0        0     2329 2024-04-18 13:39:38.231087 musical_games-0.8.3/scripts/demo_stadler_meneut_trio.py
--rw-r--r--   0        0        0    26645 2024-04-30 09:20:04.502864 musical_games-0.8.3/scripts/lilypond_copy.py
--rw-r--r--   0        0        0    29517 2024-04-30 09:20:04.502864 musical_games-0.8.3/scripts/lilypond_copy2.py
--rwxr-xr-x   0        0        0       24 2024-04-09 10:08:14.002483 musical_games-0.8.3/tests/__init__.py
--rw-r--r--   0        0        0     1061 2024-04-07 08:43:49.135413 musical_games-0.8.3/tox.ini
--rw-r--r--   0        0        0     4186 1970-01-01 00:00:00.000000 musical_games-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0      511 2024-04-07 08:37:11.575406 musical_games-0.8.4/.coveragerc
+-rw-r--r--   0        0        0      292 2016-07-03 13:55:58.881844 musical_games-0.8.4/.editorconfig
+-rw-r--r--   0        0        0    10359 2024-04-07 08:37:38.227407 musical_games-0.8.4/.gitchangelog.rc
+-rw-r--r--   0        0        0      271 2018-09-16 09:02:35.270504 musical_games-0.8.4/.gitchangelog.tpl
+-rw-r--r--   0        0        0     1166 2024-04-07 08:37:55.851407 musical_games-0.8.4/.gitignore
+-rw-r--r--   0        0        0      419 2024-04-07 08:38:05.135407 musical_games-0.8.4/.travis.yml
+-rw-r--r--   0        0        0     2171 2024-05-11 18:11:00.295832 musical_games-0.8.4/CHANGELOG.rst
+-rw-r--r--   0        0        0     7707 2016-07-03 13:55:58.881844 musical_games-0.8.4/LICENSE
+-rw-r--r--   0        0        0     4770 2024-04-13 15:08:13.743551 musical_games-0.8.4/Makefile
+-rw-r--r--   0        0        0     3103 2024-04-13 13:04:50.799749 musical_games-0.8.4/README.rst
+-rw-r--r--   0        0        0     6790 2016-07-03 13:55:58.881844 musical_games-0.8.4/docs/Makefile
+-rw-r--r--   0        0        0      154 2018-08-01 14:00:31.251630 musical_games-0.8.4/docs/authors.rst
+-rwxr-xr-x   0        0        0     7987 2024-04-09 10:08:14.002483 musical_games-0.8.4/docs/conf.py
+-rw-r--r--   0        0        0     3219 2018-08-01 14:00:31.247630 musical_games-0.8.4/docs/contributing.rst
+-rw-r--r--   0        0        0      119 2018-08-01 14:00:31.251630 musical_games-0.8.4/docs/history.rst
+-rw-r--r--   0        0        0      516 2018-08-01 14:00:31.247630 musical_games-0.8.4/docs/index.rst
+-rw-r--r--   0        0        0      209 2018-08-01 14:00:31.247630 musical_games-0.8.4/docs/installation.rst
+-rw-r--r--   0        0        0     6473 2016-07-03 13:55:58.881844 musical_games-0.8.4/docs/make.bat
+-rw-r--r--   0        0        0       76 2018-08-01 14:00:31.247630 musical_games-0.8.4/docs/modules.rst
+-rw-r--r--   0        0        0      962 2018-08-01 14:00:31.251630 musical_games-0.8.4/docs/musical_games.converters.rst
+-rw-r--r--   0        0        0     1387 2018-08-01 14:00:31.247630 musical_games-0.8.4/docs/musical_games.dice_games.lilypond.rst
+-rw-r--r--   0        0        0     1276 2018-08-01 14:00:31.247630 musical_games-0.8.4/docs/musical_games.dice_games.rst
+-rw-r--r--   0        0        0      749 2018-08-01 14:00:31.247630 musical_games-0.8.4/docs/musical_games.rst
+-rw-r--r--   0        0        0       27 2018-08-01 14:00:31.247630 musical_games-0.8.4/docs/readme.rst
+-rw-r--r--   0        0        0       87 2018-08-01 14:00:31.247630 musical_games-0.8.4/docs/usage.rst
+-rwxr-xr-x   0        0        0      191 2024-04-09 10:08:14.006483 musical_games-0.8.4/musical_games/__init__.py
+-rw-r--r--   0        0        0      518 2024-04-09 10:08:14.002483 musical_games-0.8.4/musical_games/__version__.py
+-rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.8.4/musical_games/data/__init__.py
+-rw-r--r--   0        0        0      140 2024-04-09 14:44:21.674751 musical_games-0.8.4/musical_games/data/dice_games/__init__.py
+-rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.8.4/musical_games/data/dice_games/cpe_bach_counterpoint/__init__.py
+-rw-r--r--   0        0        0     2435 2024-04-13 12:41:41.563787 musical_games-0.8.4/musical_games/data/dice_games/cpe_bach_counterpoint/bars.csv
+-rw-r--r--   0        0        0      882 2024-04-13 12:41:41.563787 musical_games-0.8.4/musical_games/data/dice_games/cpe_bach_counterpoint/bars_bass.csv
+-rw-r--r--   0        0        0     1407 2024-04-13 12:41:41.563787 musical_games-0.8.4/musical_games/data/dice_games/cpe_bach_counterpoint/bars_treble.csv
+-rw-r--r--   0        0        0     1426 2024-05-01 10:00:27.942474 musical_games-0.8.4/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     1773 2024-05-01 10:01:07.542475 musical_games-0.8.4/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     2987 2024-05-04 11:52:35.602498 musical_games-0.8.4/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0      524 2024-05-01 10:01:25.466475 musical_games-0.8.4/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_bar.ly
+-rw-r--r--   0        0        0      623 2024-05-01 10:01:48.778476 musical_games-0.8.4/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0      140 2024-04-30 09:20:04.502864 musical_games-0.8.4/musical_games/data/dice_games/gerlach_scottish_dance/__init__.py
+-rw-r--r--   0        0        0     2202 2024-05-11 18:10:52.999832 musical_games-0.8.4/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     7443 2024-05-11 18:10:52.999832 musical_games-0.8.4/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     5795 2024-05-11 18:10:52.999832 musical_games-0.8.4/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0     1208 2024-05-01 12:32:39.650622 musical_games-0.8.4/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     2193 2024-05-11 18:10:52.999832 musical_games-0.8.4/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0    18695 2024-05-11 18:10:52.999832 musical_games-0.8.4/musical_games/data/dice_games/gerlach_scottish_dance/scottish_dance_bars.csv
+-rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/__init__.py
+-rw-r--r--   0        0        0     2515 2024-05-01 10:02:26.562476 musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     6430 2024-05-01 10:02:36.282477 musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     4303 2024-05-04 11:52:35.610498 musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0     1115 2024-05-01 10:04:40.982478 musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     1313 2024-05-01 10:04:40.990478 musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0     5346 2024-04-16 05:05:56.478852 musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/menuet_bars.csv
+-rw-r--r--   0        0        0     3901 2024-04-13 12:41:41.563787 musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_lh.txt
+-rw-r--r--   0        0        0     2059 2024-04-13 12:41:41.563787 musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_rh.txt
+-rw-r--r--   0        0        0      154 2024-04-13 12:41:41.563787 musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/readme
+-rw-r--r--   0        0        0     9117 2024-04-13 12:41:41.563787 musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_lh.txt
+-rw-r--r--   0        0        0     2453 2024-04-13 12:41:41.563787 musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_rh.txt
+-rw-r--r--   0        0        0    10956 2024-04-13 12:41:41.563787 musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/trio_bars.csv
+-rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.8.4/musical_games/data/dice_games/kirnberger_polonaise/__init__.py
+-rw-r--r--   0        0        0     2867 2024-05-01 10:06:57.106481 musical_games-0.8.4/musical_games/data/dice_games/kirnberger_polonaise/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     4350 2024-05-01 10:06:57.126481 musical_games-0.8.4/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     3773 2024-05-04 11:54:20.298500 musical_games-0.8.4/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0     1634 2024-05-01 10:06:57.134481 musical_games-0.8.4/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     2046 2024-05-01 10:06:57.086481 musical_games-0.8.4/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0    32523 2024-04-13 12:41:41.563787 musical_games-0.8.4/musical_games/data/dice_games/kirnberger_polonaise/polonaise_bars.csv
+-rw-r--r--   0        0        0      140 2024-04-16 05:05:56.478852 musical_games-0.8.4/musical_games/data/dice_games/mozart_contredanse/__init__.py
+-rw-r--r--   0        0        0     8219 2024-05-04 12:42:02.922546 musical_games-0.8.4/musical_games/data/dice_games/mozart_contredanse/contredanse_bars.csv
+-rw-r--r--   0        0        0     1439 2024-05-04 12:39:21.850544 musical_games-0.8.4/musical_games/data/dice_games/mozart_contredanse/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     2929 2024-05-04 12:41:06.802545 musical_games-0.8.4/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     4138 2024-05-04 12:41:06.842545 musical_games-0.8.4/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0      892 2024-05-04 12:41:06.822545 musical_games-0.8.4/musical_games/data/dice_games/mozart_contredanse/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     1090 2024-05-04 12:41:06.854545 musical_games-0.8.4/musical_games/data/dice_games/mozart_contredanse/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.8.4/musical_games/data/dice_games/mozart_waltz/__init__.py
+-rw-r--r--   0        0        0     1421 2024-05-04 12:21:30.450526 musical_games-0.8.4/musical_games/data/dice_games/mozart_waltz/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     2847 2024-05-04 12:35:43.522540 musical_games-0.8.4/musical_games/data/dice_games/mozart_waltz/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     4087 2024-05-04 12:35:43.510540 musical_games-0.8.4/musical_games/data/dice_games/mozart_waltz/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0      892 2024-05-04 12:22:16.662527 musical_games-0.8.4/musical_games/data/dice_games/mozart_waltz/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     1090 2024-05-04 12:41:06.830545 musical_games-0.8.4/musical_games/data/dice_games/mozart_waltz/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0     9398 2024-05-04 12:21:02.330526 musical_games-0.8.4/musical_games/data/dice_games/mozart_waltz/waltz_bars.csv
+-rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.8.4/musical_games/data/dice_games/stadler_menuet_trio/__init__.py
+-rw-r--r--   0        0        0     2534 2024-05-01 10:10:19.634484 musical_games-0.8.4/musical_games/data/dice_games/stadler_menuet_trio/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     6430 2024-05-01 10:11:25.454485 musical_games-0.8.4/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     4406 2024-05-04 11:52:35.630499 musical_games-0.8.4/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0     1115 2024-05-01 10:11:25.482485 musical_games-0.8.4/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     1313 2024-05-01 10:11:25.494485 musical_games-0.8.4/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0    13676 2024-04-13 12:47:13.523778 musical_games-0.8.4/musical_games/data/dice_games/stadler_menuet_trio/menuet_bars.csv
+-rw-r--r--   0        0        0     7653 2024-04-13 12:47:50.671777 musical_games-0.8.4/musical_games/data/dice_games/stadler_menuet_trio/trio_bars.csv
+-rw-r--r--   0        0        0     2519 2024-05-11 18:10:52.999832 musical_games-0.8.4/musical_games/data/lilypond_utils/clef_changes.ly
+-rw-r--r--   0        0        0      140 2024-04-09 12:20:58.102612 musical_games-0.8.4/musical_games/dice_games/__init__.py
+-rw-r--r--   0        0        0    46961 2024-05-04 19:01:22.376069 musical_games-0.8.4/musical_games/dice_games/base.py
+-rw-r--r--   0        0        0     2614 2024-04-13 13:00:55.979755 musical_games-0.8.4/musical_games/dice_games/data_csv.py
+-rw-r--r--   0        0        0    17130 2024-05-04 12:38:10.242543 musical_games-0.8.4/musical_games/dice_games/dice_games.py
+-rw-r--r--   0        0        0      116 2024-04-09 10:08:14.006483 musical_games-0.8.4/musical_games/external/__init__.py
+-rw-r--r--   0        0        0     2969 2024-04-09 10:08:14.006483 musical_games-0.8.4/musical_games/external/base.py
+-rw-r--r--   0        0        0      411 2024-04-09 10:08:14.006483 musical_games-0.8.4/musical_games/external/exceptions.py
+-rw-r--r--   0        0        0      972 2024-04-09 10:08:14.006483 musical_games-0.8.4/musical_games/external/images.py
+-rw-r--r--   0        0        0     3595 2024-04-15 05:04:22.919891 musical_games-0.8.4/musical_games/external/lilypond.py
+-rw-r--r--   0        0        0     4729 2024-04-09 10:11:56.454487 musical_games-0.8.4/musical_games/external/midi_converters.py
+-rw-r--r--   0        0        0     1142 2024-04-09 10:08:14.006483 musical_games-0.8.4/musical_games/external/utils.py
+-rw-r--r--   0        0        0     2954 2024-04-09 10:11:56.486487 musical_games-0.8.4/musical_games/external/wav_converters.py
+-rw-r--r--   0        0        0     4835 2024-04-18 13:39:38.231087 musical_games-0.8.4/musical_games/utils.py
+-rw-r--r--   0        0        0     1117 2024-05-11 18:11:00.171832 musical_games-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0      116 2024-04-09 10:08:14.002483 musical_games-0.8.4/scripts/__init__.py
+-rw-r--r--   0        0        0     1995 2024-05-04 18:52:13.860087 musical_games-0.8.4/scripts/demo_cpe_bach.py
+-rw-r--r--   0        0        0     2402 2024-05-11 18:10:52.999832 musical_games-0.8.4/scripts/demo_gerlach_scottish_dance.py
+-rw-r--r--   0        0        0     2228 2024-05-04 18:39:35.968113 musical_games-0.8.4/scripts/demo_kirnberger_meneut_trio.py
+-rw-r--r--   0        0        0     1896 2024-05-04 18:37:37.884117 musical_games-0.8.4/scripts/demo_kirnberger_polonaise.py
+-rw-r--r--   0        0        0     1898 2024-05-04 18:42:20.816107 musical_games-0.8.4/scripts/demo_mozart_contredanse.py
+-rw-r--r--   0        0        0     1852 2024-05-04 12:36:25.506541 musical_games-0.8.4/scripts/demo_mozart_waltz.py
+-rw-r--r--   0        0        0     2329 2024-04-18 13:39:38.231087 musical_games-0.8.4/scripts/demo_stadler_meneut_trio.py
+-rw-r--r--   0        0        0    26645 2024-04-30 09:20:04.502864 musical_games-0.8.4/scripts/lilypond_copy.py
+-rw-r--r--   0        0        0    29517 2024-04-30 09:20:04.502864 musical_games-0.8.4/scripts/lilypond_copy2.py
+-rwxr-xr-x   0        0        0       24 2024-04-09 10:08:14.002483 musical_games-0.8.4/tests/__init__.py
+-rw-r--r--   0        0        0     1061 2024-04-07 08:43:49.135413 musical_games-0.8.4/tox.ini
+-rw-r--r--   0        0        0     4186 1970-01-01 00:00:00.000000 musical_games-0.8.4/PKG-INFO
```

### Comparing `musical_games-0.8.3/.gitchangelog.rc` & `musical_games-0.8.4/.gitchangelog.rc`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/.gitignore` & `musical_games-0.8.4/.gitignore`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/CHANGELOG.rst` & `musical_games-0.8.4/CHANGELOG.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 *********
 Changelog
 *********
 
+v0.8.4 (2024-05-11)
+===================
+
+Changed
+-------
+- Updated Gerlach bar 64 to be in the g-key.
+
+
 v0.8.3 (2024-05-04)
 ===================
 
 Fixed
 -----
 - Fixed the max dice value property.
```

### Comparing `musical_games-0.8.3/LICENSE` & `musical_games-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/Makefile` & `musical_games-0.8.4/Makefile`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/README.rst` & `musical_games-0.8.4/README.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/docs/Makefile` & `musical_games-0.8.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/docs/conf.py` & `musical_games-0.8.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/docs/contributing.rst` & `musical_games-0.8.4/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/docs/index.rst` & `musical_games-0.8.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/docs/make.bat` & `musical_games-0.8.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/docs/musical_games.converters.rst` & `musical_games-0.8.4/docs/musical_games.converters.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/docs/musical_games.dice_games.lilypond.rst` & `musical_games-0.8.4/docs/musical_games.dice_games.lilypond.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/docs/musical_games.dice_games.rst` & `musical_games-0.8.4/docs/musical_games.dice_games.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/docs/musical_games.rst` & `musical_games-0.8.4/docs/musical_games.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/__version__.py` & `musical_games-0.8.4/musical_games/__version__.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/cpe_bach_counterpoint/bars.csv` & `musical_games-0.8.4/musical_games/data/dice_games/cpe_bach_counterpoint/bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/cpe_bach_counterpoint/bars_bass.csv` & `musical_games-0.8.4/musical_games/data/dice_games/cpe_bach_counterpoint/bars_bass.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/cpe_bach_counterpoint/bars_treble.csv` & `musical_games-0.8.4/musical_games/data/dice_games/cpe_bach_counterpoint/bars_treble.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/bar_overview.ly` & `musical_games-0.8.4/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/bar_overview.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_midi.ly` & `musical_games-0.8.4/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_midi.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_pdf.ly` & `musical_games-0.8.4/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_pdf.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_bar.ly` & `musical_games-0.8.4/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_bar.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_dice_table_element.ly` & `musical_games-0.8.4/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_dice_table_element.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/bar_overview.ly` & `musical_games-0.8.4/musical_games/data/dice_games/mozart_contredanse/lilypond/bar_overview.ly`

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,57 @@
 \version "2.22.1"
 \paper {
     print-all-headers = ##t
+
     \BLOCK{ if render_settings['single_page'] }
         system-system-spacing = #'((basic-distance . 15))
-        paper-height = 1600\mm  %% default is 297 for a4
+        paper-height = 1200\mm  %% default is 297 for a4
     \BLOCK{ endif }
 }
 \header{
-    title = "Scottish dance"
-    composer = "Gerlach"
+    title = "Contredanse"
+    composer = "Mozart"
     tagline = ##f
 }
 \score {
     \header {
-        piece = \markup { \fontsize #1 "Scottish dance & Trio" }
-        composer = ""
+        piece = \markup { \fontsize #1 "" }
         title = ""
+        composer = ""
     }
     \new PianoStaff
     <<
         \new Staff
         <<
             {
                 \override Score.BarNumber.break-visibility = ##(#t #t #t)
-                \key c \major
+                \key c\major
             }
             {
                 \clef treble
                 \time 2/4
-                \BLOCK{ for bar in bar_collections['dance'].get_bars('piano_right_hand').values() }
+                \BLOCK{ for bar in bar_collections['contredanse'].get_bars('piano_right_hand').values() }
                     \VAR{bar.lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|"
             }
         >>
         \new Staff
         <<
             {
                 \override Score.BarNumber.break-visibility = ##(#t #t #t)
-                \key c \major
+                \key c\major
             }
             {
                 \clef bass
                 \time 2/4
-                \BLOCK{ for bar_ind, bar in bar_collections['dance'].get_bars('piano_left_hand').items() }
-                    \BLOCK{ if bar.lilypond_str.startswith('\clef') }
-                        \set Staff.forceClef = ##t
-                        \VAR{bar.lilypond_str}
-                        \BLOCK{ if not bar_collections['dance'].get_bars('piano_left_hand')[bar_ind + 1].lilypond_str.startswith('\clef') }
-                            \once \override Score.BreakAlignment #'break-align-orders = #(make-vector 3 '(span-bar breathing-sign staff-bar key clef time-signature))
-                            \once \override Staff.Clef.stencil = #(lambda (grob) (bracketify-stencil (ly:clef::print grob) Y 0.2 0.2 0.1))
-                            \clef "bass"
-                        \BLOCK{ endif }
-                    \BLOCK{ else }
+                \BLOCK{ for bar_ind, bar in bar_collections['contredanse'].get_bars('piano_left_hand').items() }
                     \VAR{bar.lilypond_str}
-                    \BLOCK{endif}
                 \BLOCK{ endfor }
                 \bar "|"
             }
         >>
     >>
     \layout {
         indent = #0
     }
 }
-
```

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/composition_pdf.ly` & `musical_games-0.8.4/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/composition_pdf.ly`

 * *Files 15% similar despite different names*

```diff
@@ -9,14 +9,17 @@
     \BLOCK{ endif }
 }
 \header{
     title = "Scottish Dance - Dance and Trio"
     composer = "Gerlach"
     tagline = ##f
 }
+
+\BLOCK{ include 'clef_changes.ly' }
+
 \score {
     \header {
         piece = \markup { \fontsize #1 "Scottish Dance" }
         title = ""
         composer = ""
     }
     \new PianoStaff
@@ -113,37 +116,35 @@
             {
                 \clef bass
                 \time 2/4
 		        \repeat volta 2{
 		            \BLOCK{ for bar_index in range(8) }
 		                \BLOCK{ set bar = composition_bars['trio'][bar_index].get_bar('piano_left_hand') }
 		                \BLOCK{ if bar.lilypond_str.startswith('\clef') }
-                            \once \override Score.BreakAlignment #'break-align-orders = #(make-vector 3 '(span-bar breathing-sign staff-bar key clef time-signature))
+                            \clefAfterBarOnce
+                            \set Staff.forceClef = ##t
                             \VAR{bar.lilypond_str}
                             \BLOCK{ if bar_index != 7 and not composition_bars['trio'][bar_index + 1].get_bar('piano_left_hand').lilypond_str.startswith('\clef') }
-                                \once \override Score.BreakAlignment #'break-align-orders = #(make-vector 3 '(span-bar breathing-sign staff-bar key clef time-signature))
-                                \once \override Staff.Clef.stencil = #(lambda (grob) (bracketify-stencil (ly:clef::print grob) Y 0.2 0.2 0.1))
-                                \clef "bass"
+                                \set Staff.forceClef = ##t \clefAfterBarOnce \clefBracketed "bass"
                             \BLOCK{ endif }
                         \BLOCK{ else }
                         \VAR{bar.lilypond_str}
                         \BLOCK{endif}
     		        \BLOCK{ endfor }
 	        	}
 	        	\clef bass
 		        \repeat volta 2{
     		        \BLOCK{ for bar_index in range(8, 16) }
     		            \BLOCK{ set bar = composition_bars['trio'][bar_index].get_bar('piano_left_hand') }
 		                \BLOCK{ if bar.lilypond_str.startswith('\clef') }
-		                    \once \override Score.BreakAlignment #'break-align-orders = #(make-vector 3 '(span-bar breathing-sign staff-bar key clef time-signature))
+		                    \clefAfterBarOnce
+		                    \set Staff.forceClef = ##t
 		                    \VAR{bar.lilypond_str}
-                            \BLOCK{ if not composition_bars['trio'][bar_index + 1].get_bar('piano_left_hand').lilypond_str.startswith('\clef') }
-                                \once \override Score.BreakAlignment #'break-align-orders = #(make-vector 3 '(span-bar breathing-sign staff-bar key clef time-signature))
-                                \once \override Staff.Clef.stencil = #(lambda (grob) (bracketify-stencil (ly:clef::print grob) Y 0.2 0.2 0.1))
-                                \clef "bass"
+                            \BLOCK{ if bar_index != 15 and not composition_bars['trio'][bar_index + 1].get_bar('piano_left_hand').lilypond_str.startswith('\clef') }
+                                \set Staff.forceClef = ##t \clefAfterBarOnce \clefBracketed "bass"
                             \BLOCK{ endif }
                         \BLOCK{ else }
                         \VAR{bar.lilypond_str}
                         \BLOCK{endif}
     		        \BLOCK{ endfor }
 	        	}
 		        \once \override Score.RehearsalMark #'self-alignment-X = #right \mark \markup {\fontsize #-1 \italic "D.C. al Fine"}
```

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/single_bar.ly` & `musical_games-0.8.4/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/single_bar.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/single_dice_table_element.ly` & `musical_games-0.8.4/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/single_dice_table_element.ly`

 * *Files 17% similar despite different names*

```diff
@@ -42,21 +42,22 @@
                     \clef bass
                 \BLOCK{ endif }
                 \time 2/4
 
                 \BLOCK{ for synchronous_bar in synchronous_bars }
                 \BLOCK{ set bar = synchronous_bar.get_bar('piano_left_hand') }
                 \BLOCK{ set has_next = loop.index0 != synchronous_bars|length - 1 }
+                \BLOCK{ if has_next }
+                \BLOCK{ set next_bar = synchronous_bars[loop.index0 + 1].get_bar('piano_left_hand') }
+                \BLOCK{ endif }
                 \BLOCK{ if bar.lilypond_str.startswith('\clef') }
                     \set Staff.forceClef = ##t
                     \VAR{ bar.lilypond_str }
-                    \BLOCK{ if has_next and not synchronous_bars[loop.index0 + 1].get_bar('piano_left_hand').lilypond_str.startswith('\clef') }
-                        \once \override Score.BreakAlignment #'break-align-orders = #(make-vector 3 '(span-bar breathing-sign staff-bar key clef time-signature))
-                        \once \override Staff.Clef.stencil = #(lambda (grob) (bracketify-stencil (ly:clef::print grob) Y 0.2 0.2 0.1))
-                        \clef "bass"
+                    \BLOCK{ if has_next and not next_bar.lilypond_str.startswith('\clef') }
+                       \clefAfterBarOnce \clefBracketed "bass"
                     \BLOCK{ endif }
                 \BLOCK{ else }
                     \VAR{ bar.lilypond_str }
                 \BLOCK{endif}
                 \BLOCK{ endfor }
                 \bar "|."
             }
```

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/gerlach_scottish_dance/scottish_dance_bars.csv` & `musical_games-0.8.4/musical_games/data/dice_games/gerlach_scottish_dance/scottish_dance_bars.csv`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 "12","<e'' g''>8 [<g' c''>8] <c'' e''>4","c8 [e'8] c'4"
 "13","<a' c''>4 <g' cis''>4","<f f'>4 <a e'>8 [es'8]"
 "14","e''16 [d''16 cis''16 e''16] d''4","{<<{\voiceOne r8 <b d'>8 <b d'>8 [<b d'>8]} \new Voice {\voiceTwo g2}>>}"
 "15","<e' g'>8 [<f' a'>16 <e' g'>16] <e' g'>8 [<e' c''>8]","{<<{\voiceOne r8 c'8 c'8 [c'8]} \new Voice {\voiceTwo c2}>>}"
 "16","g''16 [a''16 b''16 c'''16] d'''8 [g''8]","\clef ""treble"" {<<{\voiceOne r8 <f' g'>8 <f' g'>8 [<f' g'>8]} \new Voice {\voiceTwo b2}>>}"
 "17","e''8 [\grace{dis''8} e''8] e'4","<e gis b>8 [\grace{dis'8} e'8] e4"
 "18","\ottava #1 d'''16 [cis'''16 d'''16 e'''16] f'''8 [a''8] \ottava #0","\clef ""bass"" {<<{\voiceOne r8 <d' f'>8 <d' f'>8 [<d' f'>8]} \new Voice {\voiceTwo d4 s4}>>}"
-"19","d'''8 [a''8] b''8 [e'''8]","<fis c' d'>4 <g b d'>8 [<gis b d'>8] |"
+"19","d'''8 [a''8] b''8 [e'''8]","<fis c' d'>4 <g b d'>8 [<gis b d'>8]"
 "20","g''16 [fis''16 fis''16 e'''16] e'''16 [d'''16 c'''16 a''16]","{<<{\voiceOne r8 <a c'>8 <a c'>8 [<fis d'>8]} \new Voice {\voiceTwo d2}>>}"
 "21","e''8 [d''8] a''16 [g''16 f''16 d''16]","{<<{\voiceOne r8 <b f'>8 r8 <b f'>8} \new Voice {\voiceTwo g4 g4}>>}"
 "22","c'''8 [d'''16 es'''16] g''8 [e''8]","<fis a c' es'>4 <g c' e'>4"
 "23","e''8 [b'8] gis''8 [e''8]","g8 [<d' e'>8] b8 [<d' e'>8]"
 "24","c'''8 [bes''8] g''8 [e''8]","g8 [<c' e'>8] bes8 [<c' g'>8]"
 "25","e''8 [c''8] g''8 [e''8]","{<<{\voiceOne r8 <bes c'>8 <bes c'>8 [<bes c'>8]} \new Voice {\voiceTwo c2}>>}"
 "26","a'8 [c''8] e''8 [a''8]","a8 [c'8] e'8 [a'8]"
@@ -33,15 +33,15 @@
 "32","<g' c'' e''>4 <g' b' d''>8 r8","g2"
 "33","g''8 [b'8] fis''8 [a'8]","e8 [<g b>8] b,8 [<fis b>8]"
 "34","a''8 [<c'' a''>8] <a' a''>4","<a c'>8 [<a e'>8] <a c'>4"
 "35","c''16 [d''16 e''16 c''16] a'8 [a''8]","{<<{\voiceOne r8 <c' e'>8 <c' e'>8 [<c' e'>8]} \new Voice {\voiceTwo a2}>>}"
 "36","a''8 [f''8] d''8 [c''8]","<f a d'>4 <fis a d'>4"
 "37","a''16 [f''16 e''16 d''16] c''16 [g''16 b'16 d''16]","f8 [<a d'>8] <g c' e'>8 [<g b f'>8]"
 "38","f''16 [e''16 f''16 g''16] a''8 [a''8]","{<<{\voiceOne r8 <a c'>8 <a c'>8 [<a c'>8]} \new Voice {\voiceTwo f2}>>}"
-"39","{<<{\voiceOne e''8 [f''16 e''16] dis''8 [e''8]} \new Voice {\voiceTwo | c''2}>>}","c8 [g8] <c' e'>8 [g8] |"
+"39","{<<{\voiceOne e''8 [f''16 e''16] dis''8 [e''8]} \new Voice {\voiceTwo c''2}>>}","c8 [g8] <c' e'>8 [g8]"
 "40","<e' g'>8 [<f' a'>16 <e' g'>16] <e' c''>8 [<c'' e''>8]","{<<{\voiceOne r8 c'8 c'8 [c'8]} \new Voice {\voiceTwo c2}>>}"
 "41","gis'16 [a'16 b'16 gis'16] e'8 [e''8]","{<<{\voiceOne r8 <b d'>8 <b d'>8 [<b d'>8]} \new Voice {\voiceTwo e2}>>}"
 "42","a''8 [gis''16 a''16] bes''8 [a''8]","\clef ""bass"" {<<{\voiceOne r8 <cis' e'>8 <cis' g'>8 [<cis' g'>8]} \new Voice {\voiceTwo a4 s4}>>}"
 "43","a'8 [bes'16 b'16] \tuplet 3/2 {c''8 [f''8 a'8]}","{<<{\voiceOne r8 <c' f'>8 <c' f'>8 [<c' f'>8]} \new Voice {\voiceTwo f2}>>}"
 "44","c'''8 [d''8] b''8 [d''8]","{<<{\voiceOne r8 <fis c'>8 r8 b8} \new Voice {\voiceTwo d4 g4}>>}"
 "45","b'8 [d''8] g''8 [b''8]","{<<{\voiceOne r8 <b d'>8 <b d'>8 [<b d'>8]} \new Voice {\voiceTwo g2}>>}"
 "46","c''8 [e''8] g'4","c8 [<c' e'>8] <c' e'>8 [<c' e'>8]"
@@ -53,35 +53,35 @@
 "52","c''8 [c'''8] c''4","<c' e'>8 [<e' g'>8] <c' e'>4"
 "53","f''8 [a''8] f''4","<f a>8 [c'8] <f a>4"
 "54","{<<{\voiceOne b''8 [d'''16 b''16] a''8 [gis''8]} \new Voice {\voiceTwo d''4 c''8 [b'8]}>>}","{<<{\voiceOne r8 f'8 e'8 [d'8]} \new Voice {\voiceTwo f4 e8 [e8]}>>}"
 "55","{<<{\voiceOne d''8 [e''16 d''16] d''8 [g''8]} \new Voice {\voiceTwo f'4 f'4}>>}","{<<{\voiceOne r8 b8 b8 [b8]} \new Voice {\voiceTwo g2}>>}"
 "56","a''8 [e''8] cis'''8 [e'''8]","{<<{\voiceOne r8 <cis' g'>8 <cis' g'>8 [<cis' g'>8]} \new Voice {\voiceTwo a2}>>}"
 "57","bes'8 [c''16 e''16] g''4","c8 [<c' e'>8] <c' e'>8 [<c' e'>8]"
 "58","g''8 [d'''16 dis'''16] e'''8 [g''8]","<g b f'>4 <g c' e'>4"
-"59","c''16 [d''16 e''16 d''16] c''4","<g c' e'>8 [<g b f'>8] <c' e'>4 |"
+"59","c''16 [d''16 e''16 d''16] c''4","<g c' e'>8 [<g b f'>8] <c' e'>4"
 "60","a'8 [d''16 e''16] f''16 [g''16 a''8]","f8 [a8] d'8 [f'8]"
 "61","b''8 [f''16 b''16] d'''8 [f'''8]","{<<{\voiceOne r8 <f b>8 <f b>8 [<f b>8]} \new Voice {\voiceTwo d2}>>}"
 "62","g''8 [fis''16 g''16] as''8 [f''16 d''16]","<bes d' g'>4 <bes d' f'>4"
 "63","c'''8 [a''8] f'''8 [a''8]","a8 [<c' f'>8] f8 [<c' f'>8]"
-"64","f''8 [<c'' a''>8] <a' f''>4","<a, c>8 [e,8] a,,4"
+"64","f''8 [<c'' a''>8] <a' f''>4","\clefBracketed ""treble"" <f' a'>8 [c'8] f4"
 "65","e'8 [c''16 e'16] g'8 [e''8]","{<<{\voiceOne r8 <g c'>8 <g c'>8 [<g c'>8]} \new Voice {\voiceTwo c2}>>}"
 "66","g''16 [f''16 f''16 d'''16] d'''8 [f''8]","{<<{\voiceOne r8 <b d'>8 <b d'>8 [<b d'>8]} \new Voice {\voiceTwo g2}>>}"
 "67","c'''8 [d'''16 e'''16] f'''8 [a''8]","<g bes c'>4 <f a c'>4"
 "68","\ottava #1 d'''8 [c'''8] bes''8 [a''8] \ottava #0","{<<{\voiceOne r8 f'8 r8 f'8} \new Voice {\voiceTwo c'4 d'4}>>}"
 "69","c'''16 [bes''16 a''16 g''16] a''8 [f''8]","{<<{\voiceOne r8 <bes e'>8 r8 <a c'>8} \new Voice {\voiceTwo c4 f4}>>}"
 "70","g''8 [<b' g''>8] <b' g''>4","<g b>8 [g8] g,4"
 "71","d''8 [e''16 d''16] c'''8 [a''8]","{<<{\voiceOne r8 <a d'>8 <a d'>8 [<a d'>8]} \new Voice {\voiceTwo fis2}>>}"
 "72","a''8 [f''16 d''16] c''16 [g''16 b'16 d''16]","f8 [<a d'>8] <g c' e'>8 [<g b f'>8]"
 "73","\ottava #1 a''16 [b''16 c'''16 d'''16] e'''8 [gis''8] \ottava #0","e8 [<c' e'>8] e8 [<b d'>8]"
 "74","\ottava #1 d'''8 [c'''8] a''8 [e''8] \ottava #0","{<<{\voiceOne r8 <c' e'>8 r8 <c' e'>8} \new Voice {\voiceTwo a4 a4}>>}"
 "75","e''8 [e''16 d''16] a''8 [d''8]","{<<{\voiceOne r8 <c' d'>8 <c' d'>8 [<c' d'>8]} \new Voice {\voiceTwo fis2}>>}"
 "76","a''16 [gis''16 a''16 b''16] c'''4","a8 [<c' e'>8] <c' e'>8 [<c' e'>8]"
 "77","<e' c''>8 [<e' c''>8] <f' d''>8 [<g' e''>8]","c8 [c'8] <b c'>8 [<bes c'>8]"
 "78","e''16 [d''16 cis''16 d''16] a''8 [d''8]","fis8 [<a d'>8] fis8 [<c' d'>8]"
-"79","c''8 [a'8] a''8 [e''8] |","{<<{\voiceOne r8 <c' e'>8 <c' e'>8 [<c' e'>8]} \new Voice {\voiceTwo a2}>>}"
+"79","c''8 [a'8] a''8 [e''8]","{<<{\voiceOne r8 <c' e'>8 <c' e'>8 [<c' e'>8]} \new Voice {\voiceTwo a2}>>}"
 "80","a''16 [g''16 f''16 e''16] f''8 [d''8]","d8 [<d' f'>8] <d' f'>8 [<d' f'>8]"
 "81","\ottava #1 c'''16 [d'''16 e'''16 f'''16] g'''8 [c'''8] \ottava #0","{<<{\voiceOne r8 <c' e'>8 <c' e'>8 [<c' e'>8]} \new Voice {\voiceTwo g2}>>}"
 "82","\grace{ais''8} b''4 \grace{ais''8} b''8 [e'''8]","\grace{s8} e8 [<gis d'>8] gis8 [<d' e'>8]"
 "83","a''2","{<<{\voiceOne r8 <c' e'>8 <c' e'>8 [<c' e'>8]} \new Voice {\voiceTwo a2}>>}"
 "84","c''8 [e''8] a'8 [a''8]","{<<{\voiceOne r8 <c' e'>8 <c' e'>8 [<c' e'>8]} \new Voice {\voiceTwo a2}>>}"
 "85","{<<{\voiceOne d''16 [cis''16 d''16 e''16] f''8 [d''8]} \new Voice {\voiceTwo f'4 r4}>>}","bes,8 [<bes d'>8] <bes d'>8 [<bes d'>8]"
 "86","c'''8 [a''8] b''8 [c'''8]","<a c'>8 [<fis a d'>8] <g b f'>8 [<a c' e'>8]"
@@ -133,15 +133,15 @@
 "132","a''8 [f'''8] c'''8 [a''8]","{<<{\voiceOne r8 <c' f'>8 <c' f'>8 [<c' f'>8]} \new Voice {\voiceTwo f2}>>}"
 "133","gis'8 [b'8] e''8 [gis''8]","{<<{\voiceOne r8 <gis d'>8 <b e'>8 [<b e'>8]} \new Voice {\voiceTwo e2}>>}"
 "134","R2","{<<{\voiceOne a4 c'8 [e'8]} \new Voice {\voiceTwo a,4 c8 [e8]}>>}"
 "135","g''8 [fis''16 g''16] a''16 [g''16 f''16 d''16]","{<<{\voiceOne r8 <b d'>8 <b f'>8 [<b f'>8]} \new Voice {\voiceTwo g2}>>}"
 "136","e''8 [e'8] e'4","<e g b>8 [<e g c'>8] <e g>4"
 "137","{<<{\voiceOne d''8 [bes''16 d'''16] c'''8 [e''8]} \new Voice {\voiceTwo r8 <d' g'>8 r8 <g' bes'>8}>>}","bes4 c'4"
 "138","a''16 [bes''16 c'''16 d'''16] bes''8 [g''8]","{<<{\voiceOne r8 <a d'>8 r8 <bes d'>8} \new Voice {\voiceTwo fis4 g4}>>}"
-"139","b''8 [a''8] g''4","<g b d'>8 [<fis c' d'>8] <g b f'>4 |"
+"139","b''8 [a''8] g''4","<g b d'>8 [<fis c' d'>8] <g b f'>4"
 "140","bes''8 [c'''16 bes''16] a''8 [f''8]","{<<{\voiceOne r8 <c' e'>8 r8 <a c'>8} \new Voice {\voiceTwo g4 f4}>>}"
 "141","b''16 [a''16 gis''16 fis''16] e''8 [b''8]","{<<{\voiceOne r8 <gis d'>8 <gis d'>8 [<gis d'>8]} \new Voice {\voiceTwo e2}>>}"
 "142","\grace{b''8} c'''8 [b''16 a''16] c'''8 [b''16 a''16]","\grace{s8} {<<{\voiceOne r8 <c' es'>8 r8 <c' es'>8} \new Voice {\voiceTwo fis4 f4}>>}"
 "143","{<<{\voiceOne a''8 [g''8] f''8 [d''8]} \new Voice {\voiceTwo b'2}>>}","g,8 [g8] <d' f'>8 [g8]"
 "144","e''16 [dis''16 e''16 gis''16] b''8 [e''8]","{<<{\voiceOne r8 <b e'>8 r8 <d' e'>8} \new Voice {\voiceTwo gis4 gis4}>>}"
 "145","d'''8 [e'''16 f'''16] f'''8 [g''8]","<gis b f'>4 <g b f'>4"
 "146","e'''8. [d'''16] b''8 [c'''8]","{<<{\voiceOne r8 <b e'>8 <b e'>8 [<b e'>8]} \new Voice {\voiceTwo gis2}>>}"
@@ -163,25 +163,25 @@
 "162","\ottava #1 d'''8 [c'''8] a''8 [a''8] \ottava #0","a8 [<c' e'>8] f8 [<c' d'>8]"
 "163","g''8 [\grace{b''8} c'''8] c'''8 [c''8]","<c e g>8 [c'8] c'8 [c8]"
 "164","f'''4 d'''8 [a''8]","d8 [<d' f'>8] <d' f'>8 [<d' f'>8]"
 "165","c'''8 [a'16 b'16] c''16 [c''16 c''16 d''16]","<a, a>8 [<c' e'>8] a8 [<c' e'>8]"
 "166","a''8. [g''16] e''8 [f''8]","{<<{\voiceOne r8 <cis' g'>8 <cis' g'>8 [<cis' g'>8]} \new Voice {\voiceTwo a2}>>}"
 "167","\ottava #1 a''16 [b''16 c'''16 d'''16] e'''8 [a''8] \ottava #0","{<<{\voiceOne r8 <c' e'>8 <c' e'>8 [<c' e'>8]} \new Voice {\voiceTwo a2}>>}"
 "168","a''16 [g''16 fis''16 g''16] a''8 [b''8]","{<<{\voiceOne r8 <b f'>8 <d' f'>8 [<d' f'>8]} \new Voice {\voiceTwo g2}>>}"
-"169","g''8 [fis''16 g''16] c'''8 [e''8]","<g b f'>4 <g c' e'>8 [<g bes c'>8] |"
+"169","g''8 [fis''16 g''16] c'''8 [e''8]","<g b f'>4 <g c' e'>8 [<g bes c'>8]"
 "170","a''8 [f'''8] c'''8 [a''8]","f8 [<a f'>8] a8 [<c' f'>8]"
 "171","c'''4 r4","<c' e'>8 [g'8] <c' e'>4"
 "172","gis''8 [e'''8] c'''8 [a''8]","{<<{\voiceOne r8 <gis e'>8 r8 <c' e'>8} \new Voice {\voiceTwo e4 a4}>>}"
 "173","e'''8 [d'''8] c'''4","{<<{\voiceOne g8 [f8] e4} \new Voice {\voiceTwo c2}>>}"
 "174","{<<{\voiceOne c'''8. [bes''16] a''8 [a''8]} \new Voice {\voiceTwo c''4 c''8 [c''8]}>>}","{<<{\voiceOne r8 <c' e'>8 r8 <c' f'>8} \new Voice {\voiceTwo g4 f4}>>}"
 "175","f''16 [e''16 e''16 c'''16] c'''8 [e''8]","{<<{\voiceOne r8 <c' e'>8 r8 <c' e'>8} \new Voice {\voiceTwo g4 a4}>>}"
 "176","<a' f''>8 [<c'' a''>8] <a' f''>4","a'8 [f'8] f4"
 "177","\ottava #1 g''16 [fis''16 g''16 d'''16] c'''16 [bes''16 g''16 e''16] \ottava #0","\clef ""treble"" {<<{\voiceOne r8 <d' g'>8 r8 <g' bes'>8} \new Voice {\voiceTwo bes4 c'4}>>}"
 "178","cis''8 [a''8] a'4","\clef ""treble"" <a a'>4 a4"
-"179","c'''8 [b''16 c'''16] e'''16 [d'''16 bes''16 g''16] |","{<<{\voiceOne r8 <c' e'>8 <c' e'>8 [<c' e'>8]} \new Voice {\voiceTwo g2}>>}"
+"179","c'''8 [b''16 c'''16] e'''16 [d'''16 bes''16 g''16]","{<<{\voiceOne r8 <c' e'>8 <c' e'>8 [<c' e'>8]} \new Voice {\voiceTwo g2}>>}"
 "180","bes''16 [a''16 gis''16 a''16] f''4","{<<{\voiceOne r8 <c' f'>8 r8 <c' f'>8} \new Voice {\voiceTwo f4 a4}>>}"
 "181","\grace{b'8} c''4 \grace{b'8} c''4","\grace{s8} {<<{\voiceOne r8 <a f'>8 <a f'>8 [<a f'>8]} \new Voice {\voiceTwo f2}>>}"
 "182","c'''8 [b''8] a''4","{<<{\voiceOne <c' e'>8 [d'8] c'4} \new Voice {\voiceTwo a2}>>}"
 "183","c''16 [d''16 e''16 f''16] g''8 [bes''8]","{<<{\voiceOne r8 <c' e'>8 r8 <c' e'>8} \new Voice {\voiceTwo bes4 g4}>>}"
 "184","c''8 [b'8] a'4","{<<{\voiceOne e'8 [d'8] c'4} \new Voice {\voiceTwo a2}>>}"
 "185","bes''8 [c'''16 d'''16] c'''8 [f''8]","<g c' e'>4 <a c' f'>4"
 "186","\tuplet 3/2 {d''8 [f''8 a''8]} a''4","d8 [<d' f'>8] <d' f'>8 [<d' f'>8]"
```

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/bar_overview.ly` & `musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/bar_overview.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_midi.ly` & `musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_midi.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_pdf.ly` & `musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_pdf.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_bar.ly` & `musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_bar.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_dice_table_element.ly` & `musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_dice_table_element.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/kirnberger_menuet_trio/menuet_bars.csv` & `musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/menuet_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_lh.txt` & `musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_lh.txt`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_rh.txt` & `musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_rh.txt`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_lh.txt` & `musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_lh.txt`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_rh.txt` & `musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_rh.txt`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/kirnberger_menuet_trio/trio_bars.csv` & `musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/trio_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/kirnberger_polonaise/lilypond/bar_overview.ly` & `musical_games-0.8.4/musical_games/data/dice_games/kirnberger_polonaise/lilypond/bar_overview.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_midi.ly` & `musical_games-0.8.4/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_midi.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_pdf.ly` & `musical_games-0.8.4/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_pdf.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_bar.ly` & `musical_games-0.8.4/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_bar.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_dice_table_element.ly` & `musical_games-0.8.4/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_dice_table_element.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/kirnberger_polonaise/polonaise_bars.csv` & `musical_games-0.8.4/musical_games/data/dice_games/kirnberger_polonaise/polonaise_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/mozart_contredanse/contredanse_bars.csv` & `musical_games-0.8.4/musical_games/data/dice_games/mozart_contredanse/contredanse_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/mozart_contredanse/lilypond/bar_overview.ly` & `musical_games-0.8.4/musical_games/data/dice_games/mozart_waltz/lilypond/bar_overview.ly`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
     \BLOCK{ if render_settings['single_page'] }
         system-system-spacing = #'((basic-distance . 15))
         paper-height = 1200\mm  %% default is 297 for a4
     \BLOCK{ endif }
 }
 \header{
-    title = "Contredanse"
+    title = "Waltz"
     composer = "Mozart"
     tagline = ##f
 }
 \score {
     \header {
         piece = \markup { \fontsize #1 "" }
         title = ""
@@ -24,31 +24,31 @@
         <<
             {
                 \override Score.BarNumber.break-visibility = ##(#t #t #t)
                 \key c\major
             }
             {
                 \clef treble
-                \time 2/4
-                \BLOCK{ for bar in bar_collections['contredanse'].get_bars('piano_right_hand').values() }
+                \time 3/8
+                \BLOCK{ for bar in bar_collections['waltz'].get_bars('piano_right_hand').values() }
                     \VAR{bar.lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|"
             }
         >>
         \new Staff
         <<
             {
                 \override Score.BarNumber.break-visibility = ##(#t #t #t)
                 \key c\major
             }
             {
                 \clef bass
-                \time 2/4
-                \BLOCK{ for bar_ind, bar in bar_collections['contredanse'].get_bars('piano_left_hand').items() }
+                \time 3/8
+                \BLOCK{ for bar_ind, bar in bar_collections['waltz'].get_bars('piano_left_hand').items() }
                     \VAR{bar.lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|"
             }
         >>
     >>
     \layout {
```

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_midi.ly` & `musical_games-0.8.4/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_midi.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_pdf.ly` & `musical_games-0.8.4/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_pdf.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/mozart_contredanse/lilypond/single_bar.ly` & `musical_games-0.8.4/musical_games/data/dice_games/mozart_contredanse/lilypond/single_bar.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/mozart_contredanse/lilypond/single_dice_table_element.ly` & `musical_games-0.8.4/musical_games/data/dice_games/mozart_contredanse/lilypond/single_dice_table_element.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/mozart_waltz/lilypond/bar_overview.ly` & `musical_games-0.8.4/musical_games/data/dice_games/stadler_menuet_trio/lilypond/bar_overview.ly`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,99 @@
 \version "2.22.1"
 \paper {
     print-all-headers = ##t
-
     \BLOCK{ if render_settings['single_page'] }
         system-system-spacing = #'((basic-distance . 15))
-        paper-height = 1200\mm  %% default is 297 for a4
+        paper-height = 2800\mm  %% default is 297 for a4
     \BLOCK{ endif }
 }
 \header{
-    title = "Waltz"
-    composer = "Mozart"
+    title = "Menuet and Trio"
+    composer = "Stadler"
     tagline = ##f
 }
 \score {
     \header {
-        piece = \markup { \fontsize #1 "" }
-        title = ""
+        piece = \markup { \fontsize #1 "Menuet" }
         composer = ""
+        title = ""
     }
     \new PianoStaff
     <<
         \new Staff
         <<
             {
                 \override Score.BarNumber.break-visibility = ##(#t #t #t)
-                \key c\major
+                \key d\major
             }
             {
                 \clef treble
-                \time 3/8
-                \BLOCK{ for bar in bar_collections['waltz'].get_bars('piano_right_hand').values() }
+                \time 3/4
+                \BLOCK{ for bar in bar_collections['menuet'].get_bars('piano_right_hand').values() }
                     \VAR{bar.lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|"
             }
         >>
         \new Staff
         <<
             {
                 \override Score.BarNumber.break-visibility = ##(#t #t #t)
-                \key c\major
+                \key d\major
             }
             {
                 \clef bass
-                \time 3/8
-                \BLOCK{ for bar_ind, bar in bar_collections['waltz'].get_bars('piano_left_hand').items() }
+                \time 3/4
+                \BLOCK{ for bar in bar_collections['menuet'].get_bars('piano_left_hand').values() }
                     \VAR{bar.lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|"
             }
         >>
     >>
     \layout {
         indent = #0
     }
 }
+\score {
+    \header {
+        piece = \markup { \fontsize #1 "Trio" }
+        title = ""
+        composer = ""
+    }
+    \new PianoStaff
+    <<
+        \new Staff
+        <<
+            {
+                \override Score.BarNumber.break-visibility = ##(#t #t #t)
+                \key g\major
+            }
+            {
+                \clef treble
+                \time 3/4
+                \BLOCK{ for bar in bar_collections['trio'].get_bars('piano_right_hand').values() }
+                    \VAR{bar.lilypond_str}
+                \BLOCK{ endfor }
+                \bar "|"
+            }
+        >>
+        \new Staff
+        <<
+            {
+                \override Score.BarNumber.break-visibility = ##(#t #t #t)
+                \key g\major
+            }
+            {
+                \clef bass
+                \time 3/4
+                \BLOCK{ for bar in bar_collections['trio'].get_bars('piano_left_hand').values() }
+                    \VAR{bar.lilypond_str}
+                \BLOCK{ endfor }
+                \bar "|"
+            }
+        >>
+    >>
+    \layout {
+        indent = 0\mm
+    }
+}
```

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/mozart_waltz/lilypond/composition_midi.ly` & `musical_games-0.8.4/musical_games/data/dice_games/mozart_waltz/lilypond/composition_midi.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/mozart_waltz/lilypond/composition_pdf.ly` & `musical_games-0.8.4/musical_games/data/dice_games/mozart_waltz/lilypond/composition_pdf.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/mozart_waltz/lilypond/single_bar.ly` & `musical_games-0.8.4/musical_games/data/dice_games/mozart_waltz/lilypond/single_bar.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/mozart_waltz/lilypond/single_dice_table_element.ly` & `musical_games-0.8.4/musical_games/data/dice_games/mozart_waltz/lilypond/single_dice_table_element.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/mozart_waltz/waltz_bars.csv` & `musical_games-0.8.4/musical_games/data/dice_games/mozart_waltz/waltz_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/stadler_menuet_trio/lilypond/bar_overview.ly` & `musical_games-0.8.4/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_bar.ly`

 * *Files 25% similar despite different names*

```diff
@@ -1,99 +1,50 @@
 \version "2.22.1"
 \paper {
-    print-all-headers = ##t
-    \BLOCK{ if render_settings['single_page'] }
-        system-system-spacing = #'((basic-distance . 15))
-        paper-height = 2800\mm  %% default is 297 for a4
-    \BLOCK{ endif }
+    print-all-headers = ##f
+    paper-height = 50\mm
+    paper-width = 100\mm
 }
 \header{
-    title = "Menuet and Trio"
-    composer = "Stadler"
+    title = ""
     tagline = ##f
 }
 \score {
-    \header {
-        piece = \markup { \fontsize #1 "Menuet" }
-        composer = ""
-        title = ""
-    }
-    \new PianoStaff
-    <<
-        \new Staff
-        <<
-            {
-                \override Score.BarNumber.break-visibility = ##(#t #t #t)
-                \key d\major
-            }
-            {
-                \clef treble
-                \time 3/4
-                \BLOCK{ for bar in bar_collections['menuet'].get_bars('piano_right_hand').values() }
-                    \VAR{bar.lilypond_str}
-                \BLOCK{ endfor }
-                \bar "|"
-            }
-        >>
-        \new Staff
-        <<
-            {
-                \override Score.BarNumber.break-visibility = ##(#t #t #t)
-                \key d\major
-            }
-            {
-                \clef bass
-                \time 3/4
-                \BLOCK{ for bar in bar_collections['menuet'].get_bars('piano_left_hand').values() }
-                    \VAR{bar.lilypond_str}
-                \BLOCK{ endfor }
-                \bar "|"
-            }
-        >>
-    >>
-    \layout {
-        indent = #0
-    }
-}
-\score {
-    \header {
-        piece = \markup { \fontsize #1 "Trio" }
-        title = ""
-        composer = ""
-    }
     \new PianoStaff
     <<
         \new Staff
         <<
             {
-                \override Score.BarNumber.break-visibility = ##(#t #t #t)
-                \key g\major
+                \BLOCK{ if table_name == 'menuet' }
+                    \key d\major
+                \BLOCK{ else }
+                    \key g\major
+                \BLOCK{ endif }
             }
             {
                 \clef treble
                 \time 3/4
-                \BLOCK{ for bar in bar_collections['trio'].get_bars('piano_right_hand').values() }
-                    \VAR{bar.lilypond_str}
-                \BLOCK{ endfor }
-                \bar "|"
+                \VAR{ synchronous_bar.get_bar('piano_right_hand').lilypond_str }
+                \bar "|."
             }
         >>
         \new Staff
         <<
             {
-                \override Score.BarNumber.break-visibility = ##(#t #t #t)
-                \key g\major
+                \BLOCK{ if table_name == 'menuet' }
+                    \key d\major
+                \BLOCK{ else }
+                    \key g\major
+                \BLOCK{ endif }
             }
             {
                 \clef bass
                 \time 3/4
-                \BLOCK{ for bar in bar_collections['trio'].get_bars('piano_left_hand').values() }
-                    \VAR{bar.lilypond_str}
-                \BLOCK{ endfor }
-                \bar "|"
+                \VAR{ synchronous_bar.get_bar('piano_left_hand').lilypond_str }
+                \bar "|."
             }
         >>
     >>
     \layout {
         indent = 0\mm
     }
 }
```

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_midi.ly` & `musical_games-0.8.4/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_midi.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_pdf.ly` & `musical_games-0.8.4/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_pdf.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_bar.ly` & `musical_games-0.8.4/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_dice_table_element.ly`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,17 @@
                 \BLOCK{ else }
                     \key g\major
                 \BLOCK{ endif }
             }
             {
                 \clef treble
                 \time 3/4
+                \BLOCK{ for synchronous_bar in synchronous_bars }
                 \VAR{ synchronous_bar.get_bar('piano_right_hand').lilypond_str }
+                \BLOCK{ endfor }
                 \bar "|."
             }
         >>
         \new Staff
         <<
             {
                 \BLOCK{ if table_name == 'menuet' }
@@ -35,15 +37,17 @@
                 \BLOCK{ else }
                     \key g\major
                 \BLOCK{ endif }
             }
             {
                 \clef bass
                 \time 3/4
+                \BLOCK{ for synchronous_bar in synchronous_bars }
                 \VAR{ synchronous_bar.get_bar('piano_left_hand').lilypond_str }
+                \BLOCK{ endfor }
                 \bar "|."
             }
         >>
     >>
     \layout {
         indent = 0\mm
     }
```

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/stadler_menuet_trio/menuet_bars.csv` & `musical_games-0.8.4/musical_games/data/dice_games/stadler_menuet_trio/menuet_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/data/dice_games/stadler_menuet_trio/trio_bars.csv` & `musical_games-0.8.4/musical_games/data/dice_games/stadler_menuet_trio/trio_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/data/lilypond_utils/clef_changes.ly` & `musical_games-0.8.4/musical_games/data/lilypond_utils/clef_changes.ly`

 * *Files 12% similar despite different names*

```diff
@@ -54,7 +54,18 @@
     \hspace #1.2
     \raise #1
     \musicglyph "clefs.F_change"
   }
   \once \override Staff.TimeSignature.stencil = #(lambda (grob)
     (append-markup grob (ly:time-signature::print grob)))
 }
+
+
+clefAfterBarOnce = {
+    \once \override Score.BreakAlignment #'break-align-orders = #(make-vector 3 '(span-bar breathing-sign staff-bar key clef time-signature))
+}
+
+% A function for clef changes defined by the editor
+clefBracketed = #(define-music-function (clef) (string?) #{
+    \once \override Staff.Clef.stencil = #(lambda (grob) (bracketify-stencil (ly:clef::print grob) Y 0.2 0.2 0.1))
+    \clef #clef
+#})
```

### Comparing `musical_games-0.8.3/musical_games/dice_games/base.py` & `musical_games-0.8.4/musical_games/dice_games/base.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/dice_games/data_csv.py` & `musical_games-0.8.4/musical_games/dice_games/data_csv.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/dice_games/dice_games.py` & `musical_games-0.8.4/musical_games/dice_games/dice_games.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/external/base.py` & `musical_games-0.8.4/musical_games/external/base.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/external/images.py` & `musical_games-0.8.4/musical_games/external/images.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/external/lilypond.py` & `musical_games-0.8.4/musical_games/external/lilypond.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/external/midi_converters.py` & `musical_games-0.8.4/musical_games/external/midi_converters.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/external/utils.py` & `musical_games-0.8.4/musical_games/external/utils.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/external/wav_converters.py` & `musical_games-0.8.4/musical_games/external/wav_converters.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/musical_games/utils.py` & `musical_games-0.8.4/musical_games/utils.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/pyproject.toml` & `musical_games-0.8.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "musical_games"
 description = "Implementation of musical dice games from the 18th century."
 readme = "README.rst"
-version = "0.8.3"
+version = "0.8.4"
 requires-python = ">=3.11"
 keywords = ["Musical games", "Dice games", "Piano music"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Education",
     "Intended Audience :: Science/Research",
```

### Comparing `musical_games-0.8.3/scripts/demo_cpe_bach.py` & `musical_games-0.8.4/scripts/demo_cpe_bach.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/scripts/demo_gerlach_scottish_dance.py` & `musical_games-0.8.4/scripts/demo_mozart_waltz.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,45 @@
 __author__ = 'Robbert Harms'
 __date__ = '2021-03-09'
 __maintainer__ = 'Robbert Harms'
 __email__ = 'robbert@xkls.nl'
 __licence__ = 'LGPL v3'
 
 from pathlib import Path
-from musical_games.dice_games.dice_games import GerlachScottishDance
+
+from musical_games.dice_games.dice_games import MozartWaltz
 from musical_games.utils import auto_convert_lilypond_file
 
 out_dir = Path('/tmp/test')
 
-dice_game = GerlachScottishDance()
+dice_game = MozartWaltz()
 
 dice_game.compile_bars_overview(single_page=True).to_file(out_dir / 'overview.ly')
 auto_convert_lilypond_file(out_dir / 'overview.ly')
 
-dice_game.compile_single_bar('dance', 6).to_file(out_dir / 'bar_dance_6.ly')
-auto_convert_lilypond_file(out_dir / 'bar_dance_6.ly')
-dice_game.compile_single_bar('trio', 158).to_file(out_dir / 'bar_trio_158.ly')
-auto_convert_lilypond_file(out_dir / 'bar_trio_158.ly')
-
-dice_game.compile_single_dice_table_element('dance',
-                                            dice_game.get_dice_tables()['dance'].get_elements()[0]).to_file(
-    out_dir / 'single_dice_table_element_dance_0.ly')
-auto_convert_lilypond_file(out_dir / 'single_dice_table_element_dance_0.ly')
-
-dice_game.compile_single_dice_table_element('trio',
-                                            dice_game.get_dice_tables()['trio'].get_element(3, 7)).to_file(
-    out_dir / 'single_dice_table_element_trio_3_7.ly')
-auto_convert_lilypond_file(out_dir / 'single_dice_table_element_trio_3_7.ly')
+dice_game.compile_single_bar('waltz', 5).to_file(out_dir / 'bar_waltz_1.ly')
+auto_convert_lilypond_file(out_dir / 'bar_waltz_1.ly')
+
+dice_game.compile_single_dice_table_element('waltz',
+                                            dice_game.get_dice_tables()['waltz'].get_elements()[0]).to_file(
+    out_dir / 'single_dice_table_element_waltz_0.ly')
+auto_convert_lilypond_file(out_dir / 'single_dice_table_element_waltz_0.ly')
 
-print(dice_game.get_duplicate_dice_table_elements('dance'))
-print(dice_game.get_duplicate_dice_table_elements('trio'))
+print(dice_game.get_duplicate_dice_table_elements('waltz'))
 print(dice_game.count_unique_compositions(count_duplicates=True))
 print(dice_game.count_unique_compositions(count_duplicates=False))
 
-bar_selection = dice_game.get_random_bar_selection(seed=1)
-
-dice_game.compile_composition_score(bar_selection,
+dice_game.compile_composition_score(dice_game.get_random_bar_selection(seed=1, shuffle_staffs=False),
                                     comment='Test', single_page=True).to_file(out_dir / 'composition_pdf.ly')
 auto_convert_lilypond_file(out_dir / 'composition_pdf.ly')
 
 midi_settings = dice_game.get_default_midi_settings()
-my_midi_settings = midi_settings.with_updated_instrument('flute', 'dance', 'piano_right_hand')
+my_midi_settings = midi_settings.with_updated_instrument('flute', 'waltz', 'piano_right_hand')
 
-dice_game.compile_composition_audio(bar_selection,
-                                    midi_settings=my_midi_settings).to_file(out_dir / 'composition_midi.ly')
+dice_game.compile_composition_audio(
+    dice_game.get_random_bar_selection(seed=0),
+    midi_settings=my_midi_settings).to_file(out_dir / 'composition_midi.ly')
 
 auto_convert_lilypond_file(
     out_dir / 'composition_midi.ly',
     soundfont=Path('/home/robbert/programming/python/opus_infinity.org/soundfonts/Musyng_Kite.sf2'))
```

### Comparing `musical_games-0.8.3/scripts/demo_kirnberger_meneut_trio.py` & `musical_games-0.8.4/scripts/demo_kirnberger_meneut_trio.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/scripts/demo_kirnberger_polonaise.py` & `musical_games-0.8.4/scripts/demo_kirnberger_polonaise.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/scripts/demo_mozart_contredanse.py` & `musical_games-0.8.4/scripts/demo_mozart_contredanse.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/scripts/demo_mozart_waltz.py` & `musical_games-0.8.4/scripts/demo_gerlach_scottish_dance.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,53 @@
 __author__ = 'Robbert Harms'
 __date__ = '2021-03-09'
 __maintainer__ = 'Robbert Harms'
 __email__ = 'robbert@xkls.nl'
 __licence__ = 'LGPL v3'
 
 from pathlib import Path
-
-from musical_games.dice_games.dice_games import MozartWaltz
+from musical_games.dice_games.dice_games import GerlachScottishDance
 from musical_games.utils import auto_convert_lilypond_file
 
 out_dir = Path('/tmp/test')
 
-dice_game = MozartWaltz()
-
-dice_game.compile_bars_overview(single_page=True).to_file(out_dir / 'overview.ly')
-auto_convert_lilypond_file(out_dir / 'overview.ly')
-
-dice_game.compile_single_bar('waltz', 5).to_file(out_dir / 'bar_waltz_1.ly')
-auto_convert_lilypond_file(out_dir / 'bar_waltz_1.ly')
+dice_game = GerlachScottishDance()
 
-dice_game.compile_single_dice_table_element('waltz',
-                                            dice_game.get_dice_tables()['waltz'].get_elements()[0]).to_file(
-    out_dir / 'single_dice_table_element_waltz_0.ly')
-auto_convert_lilypond_file(out_dir / 'single_dice_table_element_waltz_0.ly')
+# dice_game.compile_bars_overview(single_page=True).to_file(out_dir / 'overview.ly')
+# auto_convert_lilypond_file(out_dir / 'overview.ly')
 
-print(dice_game.get_duplicate_dice_table_elements('waltz'))
-print(dice_game.count_unique_compositions(count_duplicates=True))
-print(dice_game.count_unique_compositions(count_duplicates=False))
+# dice_game.compile_single_bar('dance', 6).to_file(out_dir / 'bar_dance_6.ly')
+# auto_convert_lilypond_file(out_dir / 'bar_dance_6.ly')
+# dice_game.compile_single_bar('trio', 158).to_file(out_dir / 'bar_trio_158.ly')
+# auto_convert_lilypond_file(out_dir / 'bar_trio_158.ly')
+
+# dice_game.compile_single_dice_table_element('dance',
+#                                             dice_game.get_dice_tables()['dance'].get_elements()[0]).to_file(
+#     out_dir / 'single_dice_table_element_dance_0.ly')
+# auto_convert_lilypond_file(out_dir / 'single_dice_table_element_dance_0.ly')
+#
+# dice_game.compile_single_dice_table_element('trio',
+#                                             dice_game.get_dice_tables()['trio'].get_element(3, 7)).to_file(
+#     out_dir / 'single_dice_table_element_trio_3_7.ly')
+# auto_convert_lilypond_file(out_dir / 'single_dice_table_element_trio_3_7.ly')
+
+# print(dice_game.get_duplicate_dice_table_elements('dance'))
+# print(dice_game.get_duplicate_dice_table_elements('trio'))
+# print(dice_game.count_unique_compositions(count_duplicates=True))
+# print(dice_game.count_unique_compositions(count_duplicates=False))
+#
+bar_selection = dice_game.get_random_bar_selection(seed=2)
 
-dice_game.compile_composition_score(dice_game.get_random_bar_selection(seed=1, shuffle_staffs=False),
+dice_game.compile_composition_score(bar_selection,
                                     comment='Test', single_page=True).to_file(out_dir / 'composition_pdf.ly')
 auto_convert_lilypond_file(out_dir / 'composition_pdf.ly')
 
 midi_settings = dice_game.get_default_midi_settings()
-my_midi_settings = midi_settings.with_updated_instrument('flute', 'waltz', 'piano_right_hand')
+my_midi_settings = midi_settings.with_updated_instrument('flute', 'dance', 'piano_right_hand')
 
-dice_game.compile_composition_audio(
-    dice_game.get_random_bar_selection(seed=0),
-    midi_settings=my_midi_settings).to_file(out_dir / 'composition_midi.ly')
+dice_game.compile_composition_audio(bar_selection,
+                                    midi_settings=my_midi_settings).to_file(out_dir / 'composition_midi.ly')
 
 auto_convert_lilypond_file(
     out_dir / 'composition_midi.ly',
     soundfont=Path('/home/robbert/programming/python/opus_infinity.org/soundfonts/Musyng_Kite.sf2'))
```

### Comparing `musical_games-0.8.3/scripts/demo_stadler_meneut_trio.py` & `musical_games-0.8.4/scripts/demo_stadler_meneut_trio.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/scripts/lilypond_copy.py` & `musical_games-0.8.4/scripts/lilypond_copy.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/scripts/lilypond_copy2.py` & `musical_games-0.8.4/scripts/lilypond_copy2.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/tox.ini` & `musical_games-0.8.4/tox.ini`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.3/PKG-INFO` & `musical_games-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musical_games
-Version: 0.8.3
+Version: 0.8.4
 Summary: Implementation of musical dice games from the 18th century.
 Keywords: Musical games,Dice games,Piano music
 Author-email: Robbert Harms <robbert@xkls.nl>
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

