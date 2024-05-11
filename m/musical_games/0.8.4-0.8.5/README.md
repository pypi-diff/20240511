# Comparing `tmp/musical_games-0.8.4.tar.gz` & `tmp/musical_games-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musical_games-0.8.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "musical_games-0.8.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `musical_games-0.8.4.tar` & `musical_games-0.8.5.tar`

### file list

```diff
@@ -1,115 +1,115 @@
--rw-r--r--   0        0        0      511 2024-04-07 08:37:11.575406 musical_games-0.8.4/.coveragerc
--rw-r--r--   0        0        0      292 2016-07-03 13:55:58.881844 musical_games-0.8.4/.editorconfig
--rw-r--r--   0        0        0    10359 2024-04-07 08:37:38.227407 musical_games-0.8.4/.gitchangelog.rc
--rw-r--r--   0        0        0      271 2018-09-16 09:02:35.270504 musical_games-0.8.4/.gitchangelog.tpl
--rw-r--r--   0        0        0     1166 2024-04-07 08:37:55.851407 musical_games-0.8.4/.gitignore
--rw-r--r--   0        0        0      419 2024-04-07 08:38:05.135407 musical_games-0.8.4/.travis.yml
--rw-r--r--   0        0        0     2171 2024-05-11 18:11:00.295832 musical_games-0.8.4/CHANGELOG.rst
--rw-r--r--   0        0        0     7707 2016-07-03 13:55:58.881844 musical_games-0.8.4/LICENSE
--rw-r--r--   0        0        0     4770 2024-04-13 15:08:13.743551 musical_games-0.8.4/Makefile
--rw-r--r--   0        0        0     3103 2024-04-13 13:04:50.799749 musical_games-0.8.4/README.rst
--rw-r--r--   0        0        0     6790 2016-07-03 13:55:58.881844 musical_games-0.8.4/docs/Makefile
--rw-r--r--   0        0        0      154 2018-08-01 14:00:31.251630 musical_games-0.8.4/docs/authors.rst
--rwxr-xr-x   0        0        0     7987 2024-04-09 10:08:14.002483 musical_games-0.8.4/docs/conf.py
--rw-r--r--   0        0        0     3219 2018-08-01 14:00:31.247630 musical_games-0.8.4/docs/contributing.rst
--rw-r--r--   0        0        0      119 2018-08-01 14:00:31.251630 musical_games-0.8.4/docs/history.rst
--rw-r--r--   0        0        0      516 2018-08-01 14:00:31.247630 musical_games-0.8.4/docs/index.rst
--rw-r--r--   0        0        0      209 2018-08-01 14:00:31.247630 musical_games-0.8.4/docs/installation.rst
--rw-r--r--   0        0        0     6473 2016-07-03 13:55:58.881844 musical_games-0.8.4/docs/make.bat
--rw-r--r--   0        0        0       76 2018-08-01 14:00:31.247630 musical_games-0.8.4/docs/modules.rst
--rw-r--r--   0        0        0      962 2018-08-01 14:00:31.251630 musical_games-0.8.4/docs/musical_games.converters.rst
--rw-r--r--   0        0        0     1387 2018-08-01 14:00:31.247630 musical_games-0.8.4/docs/musical_games.dice_games.lilypond.rst
--rw-r--r--   0        0        0     1276 2018-08-01 14:00:31.247630 musical_games-0.8.4/docs/musical_games.dice_games.rst
--rw-r--r--   0        0        0      749 2018-08-01 14:00:31.247630 musical_games-0.8.4/docs/musical_games.rst
--rw-r--r--   0        0        0       27 2018-08-01 14:00:31.247630 musical_games-0.8.4/docs/readme.rst
--rw-r--r--   0        0        0       87 2018-08-01 14:00:31.247630 musical_games-0.8.4/docs/usage.rst
--rwxr-xr-x   0        0        0      191 2024-04-09 10:08:14.006483 musical_games-0.8.4/musical_games/__init__.py
--rw-r--r--   0        0        0      518 2024-04-09 10:08:14.002483 musical_games-0.8.4/musical_games/__version__.py
--rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.8.4/musical_games/data/__init__.py
--rw-r--r--   0        0        0      140 2024-04-09 14:44:21.674751 musical_games-0.8.4/musical_games/data/dice_games/__init__.py
--rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.8.4/musical_games/data/dice_games/cpe_bach_counterpoint/__init__.py
--rw-r--r--   0        0        0     2435 2024-04-13 12:41:41.563787 musical_games-0.8.4/musical_games/data/dice_games/cpe_bach_counterpoint/bars.csv
--rw-r--r--   0        0        0      882 2024-04-13 12:41:41.563787 musical_games-0.8.4/musical_games/data/dice_games/cpe_bach_counterpoint/bars_bass.csv
--rw-r--r--   0        0        0     1407 2024-04-13 12:41:41.563787 musical_games-0.8.4/musical_games/data/dice_games/cpe_bach_counterpoint/bars_treble.csv
--rw-r--r--   0        0        0     1426 2024-05-01 10:00:27.942474 musical_games-0.8.4/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     1773 2024-05-01 10:01:07.542475 musical_games-0.8.4/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     2987 2024-05-04 11:52:35.602498 musical_games-0.8.4/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0      524 2024-05-01 10:01:25.466475 musical_games-0.8.4/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_bar.ly
--rw-r--r--   0        0        0      623 2024-05-01 10:01:48.778476 musical_games-0.8.4/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_dice_table_element.ly
--rw-r--r--   0        0        0      140 2024-04-30 09:20:04.502864 musical_games-0.8.4/musical_games/data/dice_games/gerlach_scottish_dance/__init__.py
--rw-r--r--   0        0        0     2202 2024-05-11 18:10:52.999832 musical_games-0.8.4/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     7443 2024-05-11 18:10:52.999832 musical_games-0.8.4/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     5795 2024-05-11 18:10:52.999832 musical_games-0.8.4/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0     1208 2024-05-01 12:32:39.650622 musical_games-0.8.4/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/single_bar.ly
--rw-r--r--   0        0        0     2193 2024-05-11 18:10:52.999832 musical_games-0.8.4/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/single_dice_table_element.ly
--rw-r--r--   0        0        0    18695 2024-05-11 18:10:52.999832 musical_games-0.8.4/musical_games/data/dice_games/gerlach_scottish_dance/scottish_dance_bars.csv
--rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/__init__.py
--rw-r--r--   0        0        0     2515 2024-05-01 10:02:26.562476 musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     6430 2024-05-01 10:02:36.282477 musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     4303 2024-05-04 11:52:35.610498 musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0     1115 2024-05-01 10:04:40.982478 musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_bar.ly
--rw-r--r--   0        0        0     1313 2024-05-01 10:04:40.990478 musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_dice_table_element.ly
--rw-r--r--   0        0        0     5346 2024-04-16 05:05:56.478852 musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/menuet_bars.csv
--rw-r--r--   0        0        0     3901 2024-04-13 12:41:41.563787 musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_lh.txt
--rw-r--r--   0        0        0     2059 2024-04-13 12:41:41.563787 musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_rh.txt
--rw-r--r--   0        0        0      154 2024-04-13 12:41:41.563787 musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/readme
--rw-r--r--   0        0        0     9117 2024-04-13 12:41:41.563787 musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_lh.txt
--rw-r--r--   0        0        0     2453 2024-04-13 12:41:41.563787 musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_rh.txt
--rw-r--r--   0        0        0    10956 2024-04-13 12:41:41.563787 musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/trio_bars.csv
--rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.8.4/musical_games/data/dice_games/kirnberger_polonaise/__init__.py
--rw-r--r--   0        0        0     2867 2024-05-01 10:06:57.106481 musical_games-0.8.4/musical_games/data/dice_games/kirnberger_polonaise/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     4350 2024-05-01 10:06:57.126481 musical_games-0.8.4/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     3773 2024-05-04 11:54:20.298500 musical_games-0.8.4/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0     1634 2024-05-01 10:06:57.134481 musical_games-0.8.4/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_bar.ly
--rw-r--r--   0        0        0     2046 2024-05-01 10:06:57.086481 musical_games-0.8.4/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_dice_table_element.ly
--rw-r--r--   0        0        0    32523 2024-04-13 12:41:41.563787 musical_games-0.8.4/musical_games/data/dice_games/kirnberger_polonaise/polonaise_bars.csv
--rw-r--r--   0        0        0      140 2024-04-16 05:05:56.478852 musical_games-0.8.4/musical_games/data/dice_games/mozart_contredanse/__init__.py
--rw-r--r--   0        0        0     8219 2024-05-04 12:42:02.922546 musical_games-0.8.4/musical_games/data/dice_games/mozart_contredanse/contredanse_bars.csv
--rw-r--r--   0        0        0     1439 2024-05-04 12:39:21.850544 musical_games-0.8.4/musical_games/data/dice_games/mozart_contredanse/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     2929 2024-05-04 12:41:06.802545 musical_games-0.8.4/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     4138 2024-05-04 12:41:06.842545 musical_games-0.8.4/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0      892 2024-05-04 12:41:06.822545 musical_games-0.8.4/musical_games/data/dice_games/mozart_contredanse/lilypond/single_bar.ly
--rw-r--r--   0        0        0     1090 2024-05-04 12:41:06.854545 musical_games-0.8.4/musical_games/data/dice_games/mozart_contredanse/lilypond/single_dice_table_element.ly
--rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.8.4/musical_games/data/dice_games/mozart_waltz/__init__.py
--rw-r--r--   0        0        0     1421 2024-05-04 12:21:30.450526 musical_games-0.8.4/musical_games/data/dice_games/mozart_waltz/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     2847 2024-05-04 12:35:43.522540 musical_games-0.8.4/musical_games/data/dice_games/mozart_waltz/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     4087 2024-05-04 12:35:43.510540 musical_games-0.8.4/musical_games/data/dice_games/mozart_waltz/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0      892 2024-05-04 12:22:16.662527 musical_games-0.8.4/musical_games/data/dice_games/mozart_waltz/lilypond/single_bar.ly
--rw-r--r--   0        0        0     1090 2024-05-04 12:41:06.830545 musical_games-0.8.4/musical_games/data/dice_games/mozart_waltz/lilypond/single_dice_table_element.ly
--rw-r--r--   0        0        0     9398 2024-05-04 12:21:02.330526 musical_games-0.8.4/musical_games/data/dice_games/mozart_waltz/waltz_bars.csv
--rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.8.4/musical_games/data/dice_games/stadler_menuet_trio/__init__.py
--rw-r--r--   0        0        0     2534 2024-05-01 10:10:19.634484 musical_games-0.8.4/musical_games/data/dice_games/stadler_menuet_trio/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     6430 2024-05-01 10:11:25.454485 musical_games-0.8.4/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     4406 2024-05-04 11:52:35.630499 musical_games-0.8.4/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0     1115 2024-05-01 10:11:25.482485 musical_games-0.8.4/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_bar.ly
--rw-r--r--   0        0        0     1313 2024-05-01 10:11:25.494485 musical_games-0.8.4/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_dice_table_element.ly
--rw-r--r--   0        0        0    13676 2024-04-13 12:47:13.523778 musical_games-0.8.4/musical_games/data/dice_games/stadler_menuet_trio/menuet_bars.csv
--rw-r--r--   0        0        0     7653 2024-04-13 12:47:50.671777 musical_games-0.8.4/musical_games/data/dice_games/stadler_menuet_trio/trio_bars.csv
--rw-r--r--   0        0        0     2519 2024-05-11 18:10:52.999832 musical_games-0.8.4/musical_games/data/lilypond_utils/clef_changes.ly
--rw-r--r--   0        0        0      140 2024-04-09 12:20:58.102612 musical_games-0.8.4/musical_games/dice_games/__init__.py
--rw-r--r--   0        0        0    46961 2024-05-04 19:01:22.376069 musical_games-0.8.4/musical_games/dice_games/base.py
--rw-r--r--   0        0        0     2614 2024-04-13 13:00:55.979755 musical_games-0.8.4/musical_games/dice_games/data_csv.py
--rw-r--r--   0        0        0    17130 2024-05-04 12:38:10.242543 musical_games-0.8.4/musical_games/dice_games/dice_games.py
--rw-r--r--   0        0        0      116 2024-04-09 10:08:14.006483 musical_games-0.8.4/musical_games/external/__init__.py
--rw-r--r--   0        0        0     2969 2024-04-09 10:08:14.006483 musical_games-0.8.4/musical_games/external/base.py
--rw-r--r--   0        0        0      411 2024-04-09 10:08:14.006483 musical_games-0.8.4/musical_games/external/exceptions.py
--rw-r--r--   0        0        0      972 2024-04-09 10:08:14.006483 musical_games-0.8.4/musical_games/external/images.py
--rw-r--r--   0        0        0     3595 2024-04-15 05:04:22.919891 musical_games-0.8.4/musical_games/external/lilypond.py
--rw-r--r--   0        0        0     4729 2024-04-09 10:11:56.454487 musical_games-0.8.4/musical_games/external/midi_converters.py
--rw-r--r--   0        0        0     1142 2024-04-09 10:08:14.006483 musical_games-0.8.4/musical_games/external/utils.py
--rw-r--r--   0        0        0     2954 2024-04-09 10:11:56.486487 musical_games-0.8.4/musical_games/external/wav_converters.py
--rw-r--r--   0        0        0     4835 2024-04-18 13:39:38.231087 musical_games-0.8.4/musical_games/utils.py
--rw-r--r--   0        0        0     1117 2024-05-11 18:11:00.171832 musical_games-0.8.4/pyproject.toml
--rw-r--r--   0        0        0      116 2024-04-09 10:08:14.002483 musical_games-0.8.4/scripts/__init__.py
--rw-r--r--   0        0        0     1995 2024-05-04 18:52:13.860087 musical_games-0.8.4/scripts/demo_cpe_bach.py
--rw-r--r--   0        0        0     2402 2024-05-11 18:10:52.999832 musical_games-0.8.4/scripts/demo_gerlach_scottish_dance.py
--rw-r--r--   0        0        0     2228 2024-05-04 18:39:35.968113 musical_games-0.8.4/scripts/demo_kirnberger_meneut_trio.py
--rw-r--r--   0        0        0     1896 2024-05-04 18:37:37.884117 musical_games-0.8.4/scripts/demo_kirnberger_polonaise.py
--rw-r--r--   0        0        0     1898 2024-05-04 18:42:20.816107 musical_games-0.8.4/scripts/demo_mozart_contredanse.py
--rw-r--r--   0        0        0     1852 2024-05-04 12:36:25.506541 musical_games-0.8.4/scripts/demo_mozart_waltz.py
--rw-r--r--   0        0        0     2329 2024-04-18 13:39:38.231087 musical_games-0.8.4/scripts/demo_stadler_meneut_trio.py
--rw-r--r--   0        0        0    26645 2024-04-30 09:20:04.502864 musical_games-0.8.4/scripts/lilypond_copy.py
--rw-r--r--   0        0        0    29517 2024-04-30 09:20:04.502864 musical_games-0.8.4/scripts/lilypond_copy2.py
--rwxr-xr-x   0        0        0       24 2024-04-09 10:08:14.002483 musical_games-0.8.4/tests/__init__.py
--rw-r--r--   0        0        0     1061 2024-04-07 08:43:49.135413 musical_games-0.8.4/tox.ini
--rw-r--r--   0        0        0     4186 1970-01-01 00:00:00.000000 musical_games-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0      511 2024-04-07 08:37:11.575406 musical_games-0.8.5/.coveragerc
+-rw-r--r--   0        0        0      292 2016-07-03 13:55:58.881844 musical_games-0.8.5/.editorconfig
+-rw-r--r--   0        0        0    10359 2024-04-07 08:37:38.227407 musical_games-0.8.5/.gitchangelog.rc
+-rw-r--r--   0        0        0      271 2018-09-16 09:02:35.270504 musical_games-0.8.5/.gitchangelog.tpl
+-rw-r--r--   0        0        0     1166 2024-04-07 08:37:55.851407 musical_games-0.8.5/.gitignore
+-rw-r--r--   0        0        0      419 2024-04-07 08:38:05.135407 musical_games-0.8.5/.travis.yml
+-rw-r--r--   0        0        0     2262 2024-05-11 18:34:01.567795 musical_games-0.8.5/CHANGELOG.rst
+-rw-r--r--   0        0        0     7707 2016-07-03 13:55:58.881844 musical_games-0.8.5/LICENSE
+-rw-r--r--   0        0        0     4770 2024-04-13 15:08:13.743551 musical_games-0.8.5/Makefile
+-rw-r--r--   0        0        0     3103 2024-04-13 13:04:50.799749 musical_games-0.8.5/README.rst
+-rw-r--r--   0        0        0     6790 2016-07-03 13:55:58.881844 musical_games-0.8.5/docs/Makefile
+-rw-r--r--   0        0        0      154 2018-08-01 14:00:31.251630 musical_games-0.8.5/docs/authors.rst
+-rwxr-xr-x   0        0        0     7987 2024-04-09 10:08:14.002483 musical_games-0.8.5/docs/conf.py
+-rw-r--r--   0        0        0     3219 2018-08-01 14:00:31.247630 musical_games-0.8.5/docs/contributing.rst
+-rw-r--r--   0        0        0      119 2018-08-01 14:00:31.251630 musical_games-0.8.5/docs/history.rst
+-rw-r--r--   0        0        0      516 2018-08-01 14:00:31.247630 musical_games-0.8.5/docs/index.rst
+-rw-r--r--   0        0        0      209 2018-08-01 14:00:31.247630 musical_games-0.8.5/docs/installation.rst
+-rw-r--r--   0        0        0     6473 2016-07-03 13:55:58.881844 musical_games-0.8.5/docs/make.bat
+-rw-r--r--   0        0        0       76 2018-08-01 14:00:31.247630 musical_games-0.8.5/docs/modules.rst
+-rw-r--r--   0        0        0      962 2018-08-01 14:00:31.251630 musical_games-0.8.5/docs/musical_games.converters.rst
+-rw-r--r--   0        0        0     1387 2018-08-01 14:00:31.247630 musical_games-0.8.5/docs/musical_games.dice_games.lilypond.rst
+-rw-r--r--   0        0        0     1276 2018-08-01 14:00:31.247630 musical_games-0.8.5/docs/musical_games.dice_games.rst
+-rw-r--r--   0        0        0      749 2018-08-01 14:00:31.247630 musical_games-0.8.5/docs/musical_games.rst
+-rw-r--r--   0        0        0       27 2018-08-01 14:00:31.247630 musical_games-0.8.5/docs/readme.rst
+-rw-r--r--   0        0        0       87 2018-08-01 14:00:31.247630 musical_games-0.8.5/docs/usage.rst
+-rwxr-xr-x   0        0        0      191 2024-04-09 10:08:14.006483 musical_games-0.8.5/musical_games/__init__.py
+-rw-r--r--   0        0        0      518 2024-04-09 10:08:14.002483 musical_games-0.8.5/musical_games/__version__.py
+-rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.8.5/musical_games/data/__init__.py
+-rw-r--r--   0        0        0      140 2024-04-09 14:44:21.674751 musical_games-0.8.5/musical_games/data/dice_games/__init__.py
+-rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.8.5/musical_games/data/dice_games/cpe_bach_counterpoint/__init__.py
+-rw-r--r--   0        0        0     2435 2024-04-13 12:41:41.563787 musical_games-0.8.5/musical_games/data/dice_games/cpe_bach_counterpoint/bars.csv
+-rw-r--r--   0        0        0      882 2024-04-13 12:41:41.563787 musical_games-0.8.5/musical_games/data/dice_games/cpe_bach_counterpoint/bars_bass.csv
+-rw-r--r--   0        0        0     1407 2024-04-13 12:41:41.563787 musical_games-0.8.5/musical_games/data/dice_games/cpe_bach_counterpoint/bars_treble.csv
+-rw-r--r--   0        0        0     1426 2024-05-01 10:00:27.942474 musical_games-0.8.5/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     1773 2024-05-01 10:01:07.542475 musical_games-0.8.5/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     2987 2024-05-04 11:52:35.602498 musical_games-0.8.5/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0      524 2024-05-01 10:01:25.466475 musical_games-0.8.5/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_bar.ly
+-rw-r--r--   0        0        0      623 2024-05-01 10:01:48.778476 musical_games-0.8.5/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0      140 2024-04-30 09:20:04.502864 musical_games-0.8.5/musical_games/data/dice_games/gerlach_scottish_dance/__init__.py
+-rw-r--r--   0        0        0     2202 2024-05-11 18:10:52.999832 musical_games-0.8.5/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     7480 2024-05-11 18:33:48.383795 musical_games-0.8.5/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     5795 2024-05-11 18:10:52.999832 musical_games-0.8.5/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0     1208 2024-05-01 12:32:39.650622 musical_games-0.8.5/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     2193 2024-05-11 18:10:52.999832 musical_games-0.8.5/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0    18695 2024-05-11 18:10:52.999832 musical_games-0.8.5/musical_games/data/dice_games/gerlach_scottish_dance/scottish_dance_bars.csv
+-rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.8.5/musical_games/data/dice_games/kirnberger_menuet_trio/__init__.py
+-rw-r--r--   0        0        0     2515 2024-05-01 10:02:26.562476 musical_games-0.8.5/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     6430 2024-05-01 10:02:36.282477 musical_games-0.8.5/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     4303 2024-05-04 11:52:35.610498 musical_games-0.8.5/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0     1115 2024-05-01 10:04:40.982478 musical_games-0.8.5/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     1313 2024-05-01 10:04:40.990478 musical_games-0.8.5/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0     5346 2024-04-16 05:05:56.478852 musical_games-0.8.5/musical_games/data/dice_games/kirnberger_menuet_trio/menuet_bars.csv
+-rw-r--r--   0        0        0     3901 2024-04-13 12:41:41.563787 musical_games-0.8.5/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_lh.txt
+-rw-r--r--   0        0        0     2059 2024-04-13 12:41:41.563787 musical_games-0.8.5/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_rh.txt
+-rw-r--r--   0        0        0      154 2024-04-13 12:41:41.563787 musical_games-0.8.5/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/readme
+-rw-r--r--   0        0        0     9117 2024-04-13 12:41:41.563787 musical_games-0.8.5/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_lh.txt
+-rw-r--r--   0        0        0     2453 2024-04-13 12:41:41.563787 musical_games-0.8.5/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_rh.txt
+-rw-r--r--   0        0        0    10956 2024-04-13 12:41:41.563787 musical_games-0.8.5/musical_games/data/dice_games/kirnberger_menuet_trio/trio_bars.csv
+-rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.8.5/musical_games/data/dice_games/kirnberger_polonaise/__init__.py
+-rw-r--r--   0        0        0     2867 2024-05-01 10:06:57.106481 musical_games-0.8.5/musical_games/data/dice_games/kirnberger_polonaise/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     4350 2024-05-01 10:06:57.126481 musical_games-0.8.5/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     3773 2024-05-04 11:54:20.298500 musical_games-0.8.5/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0     1634 2024-05-01 10:06:57.134481 musical_games-0.8.5/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     2046 2024-05-01 10:06:57.086481 musical_games-0.8.5/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0    32523 2024-04-13 12:41:41.563787 musical_games-0.8.5/musical_games/data/dice_games/kirnberger_polonaise/polonaise_bars.csv
+-rw-r--r--   0        0        0      140 2024-04-16 05:05:56.478852 musical_games-0.8.5/musical_games/data/dice_games/mozart_contredanse/__init__.py
+-rw-r--r--   0        0        0     8219 2024-05-04 12:42:02.922546 musical_games-0.8.5/musical_games/data/dice_games/mozart_contredanse/contredanse_bars.csv
+-rw-r--r--   0        0        0     1439 2024-05-04 12:39:21.850544 musical_games-0.8.5/musical_games/data/dice_games/mozart_contredanse/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     2929 2024-05-04 12:41:06.802545 musical_games-0.8.5/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     4138 2024-05-04 12:41:06.842545 musical_games-0.8.5/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0      892 2024-05-04 12:41:06.822545 musical_games-0.8.5/musical_games/data/dice_games/mozart_contredanse/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     1090 2024-05-04 12:41:06.854545 musical_games-0.8.5/musical_games/data/dice_games/mozart_contredanse/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.8.5/musical_games/data/dice_games/mozart_waltz/__init__.py
+-rw-r--r--   0        0        0     1421 2024-05-04 12:21:30.450526 musical_games-0.8.5/musical_games/data/dice_games/mozart_waltz/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     2847 2024-05-04 12:35:43.522540 musical_games-0.8.5/musical_games/data/dice_games/mozart_waltz/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     4087 2024-05-04 12:35:43.510540 musical_games-0.8.5/musical_games/data/dice_games/mozart_waltz/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0      892 2024-05-04 12:22:16.662527 musical_games-0.8.5/musical_games/data/dice_games/mozart_waltz/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     1090 2024-05-04 12:41:06.830545 musical_games-0.8.5/musical_games/data/dice_games/mozart_waltz/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0     9398 2024-05-04 12:21:02.330526 musical_games-0.8.5/musical_games/data/dice_games/mozart_waltz/waltz_bars.csv
+-rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.8.5/musical_games/data/dice_games/stadler_menuet_trio/__init__.py
+-rw-r--r--   0        0        0     2534 2024-05-01 10:10:19.634484 musical_games-0.8.5/musical_games/data/dice_games/stadler_menuet_trio/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     6430 2024-05-01 10:11:25.454485 musical_games-0.8.5/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     4406 2024-05-04 11:52:35.630499 musical_games-0.8.5/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0     1115 2024-05-01 10:11:25.482485 musical_games-0.8.5/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     1313 2024-05-01 10:11:25.494485 musical_games-0.8.5/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0    13676 2024-04-13 12:47:13.523778 musical_games-0.8.5/musical_games/data/dice_games/stadler_menuet_trio/menuet_bars.csv
+-rw-r--r--   0        0        0     7653 2024-04-13 12:47:50.671777 musical_games-0.8.5/musical_games/data/dice_games/stadler_menuet_trio/trio_bars.csv
+-rw-r--r--   0        0        0     2519 2024-05-11 18:10:52.999832 musical_games-0.8.5/musical_games/data/lilypond_utils/clef_changes.ly
+-rw-r--r--   0        0        0      140 2024-04-09 12:20:58.102612 musical_games-0.8.5/musical_games/dice_games/__init__.py
+-rw-r--r--   0        0        0    46961 2024-05-04 19:01:22.376069 musical_games-0.8.5/musical_games/dice_games/base.py
+-rw-r--r--   0        0        0     2614 2024-04-13 13:00:55.979755 musical_games-0.8.5/musical_games/dice_games/data_csv.py
+-rw-r--r--   0        0        0    17130 2024-05-04 12:38:10.242543 musical_games-0.8.5/musical_games/dice_games/dice_games.py
+-rw-r--r--   0        0        0      116 2024-04-09 10:08:14.006483 musical_games-0.8.5/musical_games/external/__init__.py
+-rw-r--r--   0        0        0     2969 2024-04-09 10:08:14.006483 musical_games-0.8.5/musical_games/external/base.py
+-rw-r--r--   0        0        0      411 2024-04-09 10:08:14.006483 musical_games-0.8.5/musical_games/external/exceptions.py
+-rw-r--r--   0        0        0      972 2024-04-09 10:08:14.006483 musical_games-0.8.5/musical_games/external/images.py
+-rw-r--r--   0        0        0     3595 2024-04-15 05:04:22.919891 musical_games-0.8.5/musical_games/external/lilypond.py
+-rw-r--r--   0        0        0     4729 2024-04-09 10:11:56.454487 musical_games-0.8.5/musical_games/external/midi_converters.py
+-rw-r--r--   0        0        0     1142 2024-04-09 10:08:14.006483 musical_games-0.8.5/musical_games/external/utils.py
+-rw-r--r--   0        0        0     2954 2024-04-09 10:11:56.486487 musical_games-0.8.5/musical_games/external/wav_converters.py
+-rw-r--r--   0        0        0     4835 2024-04-18 13:39:38.231087 musical_games-0.8.5/musical_games/utils.py
+-rw-r--r--   0        0        0     1117 2024-05-11 18:33:53.263795 musical_games-0.8.5/pyproject.toml
+-rw-r--r--   0        0        0      116 2024-04-09 10:08:14.002483 musical_games-0.8.5/scripts/__init__.py
+-rw-r--r--   0        0        0     1995 2024-05-04 18:52:13.860087 musical_games-0.8.5/scripts/demo_cpe_bach.py
+-rw-r--r--   0        0        0     2364 2024-05-11 18:33:48.383795 musical_games-0.8.5/scripts/demo_gerlach_scottish_dance.py
+-rw-r--r--   0        0        0     2228 2024-05-04 18:39:35.968113 musical_games-0.8.5/scripts/demo_kirnberger_meneut_trio.py
+-rw-r--r--   0        0        0     1896 2024-05-04 18:37:37.884117 musical_games-0.8.5/scripts/demo_kirnberger_polonaise.py
+-rw-r--r--   0        0        0     1898 2024-05-04 18:42:20.816107 musical_games-0.8.5/scripts/demo_mozart_contredanse.py
+-rw-r--r--   0        0        0     1852 2024-05-04 12:36:25.506541 musical_games-0.8.5/scripts/demo_mozart_waltz.py
+-rw-r--r--   0        0        0     2329 2024-04-18 13:39:38.231087 musical_games-0.8.5/scripts/demo_stadler_meneut_trio.py
+-rw-r--r--   0        0        0    26645 2024-04-30 09:20:04.502864 musical_games-0.8.5/scripts/lilypond_copy.py
+-rw-r--r--   0        0        0    29517 2024-04-30 09:20:04.502864 musical_games-0.8.5/scripts/lilypond_copy2.py
+-rwxr-xr-x   0        0        0       24 2024-04-09 10:08:14.002483 musical_games-0.8.5/tests/__init__.py
+-rw-r--r--   0        0        0     1061 2024-04-07 08:43:49.135413 musical_games-0.8.5/tox.ini
+-rw-r--r--   0        0        0     4186 1970-01-01 00:00:00.000000 musical_games-0.8.5/PKG-INFO
```

### Comparing `musical_games-0.8.4/.gitchangelog.rc` & `musical_games-0.8.5/.gitchangelog.rc`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/.gitignore` & `musical_games-0.8.5/.gitignore`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/CHANGELOG.rst` & `musical_games-0.8.5/CHANGELOG.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 *********
 Changelog
 *********
 
+v0.8.5 (2024-05-11)
+===================
+
+Fixed
+-----
+- Fixed midi generation in Gerlach.
+
+
 v0.8.4 (2024-05-11)
 ===================
 
 Changed
 -------
 - Updated Gerlach bar 64 to be in the g-key.
```

### Comparing `musical_games-0.8.4/LICENSE` & `musical_games-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/Makefile` & `musical_games-0.8.5/Makefile`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/README.rst` & `musical_games-0.8.5/README.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/docs/Makefile` & `musical_games-0.8.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/docs/conf.py` & `musical_games-0.8.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/docs/contributing.rst` & `musical_games-0.8.5/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/docs/index.rst` & `musical_games-0.8.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/docs/make.bat` & `musical_games-0.8.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/docs/musical_games.converters.rst` & `musical_games-0.8.5/docs/musical_games.converters.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/docs/musical_games.dice_games.lilypond.rst` & `musical_games-0.8.5/docs/musical_games.dice_games.lilypond.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/docs/musical_games.dice_games.rst` & `musical_games-0.8.5/docs/musical_games.dice_games.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/docs/musical_games.rst` & `musical_games-0.8.5/docs/musical_games.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/__version__.py` & `musical_games-0.8.5/musical_games/__version__.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/cpe_bach_counterpoint/bars.csv` & `musical_games-0.8.5/musical_games/data/dice_games/cpe_bach_counterpoint/bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/cpe_bach_counterpoint/bars_bass.csv` & `musical_games-0.8.5/musical_games/data/dice_games/cpe_bach_counterpoint/bars_bass.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/cpe_bach_counterpoint/bars_treble.csv` & `musical_games-0.8.5/musical_games/data/dice_games/cpe_bach_counterpoint/bars_treble.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/bar_overview.ly` & `musical_games-0.8.5/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/bar_overview.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_midi.ly` & `musical_games-0.8.5/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_midi.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_pdf.ly` & `musical_games-0.8.5/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_pdf.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_bar.ly` & `musical_games-0.8.5/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_bar.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_dice_table_element.ly` & `musical_games-0.8.5/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_dice_table_element.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/bar_overview.ly` & `musical_games-0.8.5/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/bar_overview.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/composition_midi.ly` & `musical_games-0.8.5/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/composition_midi.ly`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 \version "2.22.1"
 \include "articulate.ly"
 
+\BLOCK{ include 'clef_changes.ly' }
+
 % dance with repeats
 \score {
     \unfoldRepeats
     \articulate
     \new GrandStaff
     <<
         \new Staff
```

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/composition_pdf.ly` & `musical_games-0.8.5/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/composition_pdf.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/single_bar.ly` & `musical_games-0.8.5/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/single_bar.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/single_dice_table_element.ly` & `musical_games-0.8.5/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/single_dice_table_element.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/gerlach_scottish_dance/scottish_dance_bars.csv` & `musical_games-0.8.5/musical_games/data/dice_games/gerlach_scottish_dance/scottish_dance_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/bar_overview.ly` & `musical_games-0.8.5/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/bar_overview.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_midi.ly` & `musical_games-0.8.5/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_midi.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_pdf.ly` & `musical_games-0.8.5/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_pdf.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_bar.ly` & `musical_games-0.8.5/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_bar.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_dice_table_element.ly` & `musical_games-0.8.5/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_dice_table_element.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/menuet_bars.csv` & `musical_games-0.8.5/musical_games/data/dice_games/kirnberger_menuet_trio/menuet_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_lh.txt` & `musical_games-0.8.5/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_lh.txt`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_rh.txt` & `musical_games-0.8.5/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_rh.txt`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_lh.txt` & `musical_games-0.8.5/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_lh.txt`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_rh.txt` & `musical_games-0.8.5/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_rh.txt`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/kirnberger_menuet_trio/trio_bars.csv` & `musical_games-0.8.5/musical_games/data/dice_games/kirnberger_menuet_trio/trio_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/kirnberger_polonaise/lilypond/bar_overview.ly` & `musical_games-0.8.5/musical_games/data/dice_games/kirnberger_polonaise/lilypond/bar_overview.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_midi.ly` & `musical_games-0.8.5/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_midi.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_pdf.ly` & `musical_games-0.8.5/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_pdf.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_bar.ly` & `musical_games-0.8.5/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_bar.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_dice_table_element.ly` & `musical_games-0.8.5/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_dice_table_element.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/kirnberger_polonaise/polonaise_bars.csv` & `musical_games-0.8.5/musical_games/data/dice_games/kirnberger_polonaise/polonaise_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/mozart_contredanse/contredanse_bars.csv` & `musical_games-0.8.5/musical_games/data/dice_games/mozart_contredanse/contredanse_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/mozart_contredanse/lilypond/bar_overview.ly` & `musical_games-0.8.5/musical_games/data/dice_games/mozart_contredanse/lilypond/bar_overview.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_midi.ly` & `musical_games-0.8.5/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_midi.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_pdf.ly` & `musical_games-0.8.5/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_pdf.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/mozart_contredanse/lilypond/single_bar.ly` & `musical_games-0.8.5/musical_games/data/dice_games/mozart_contredanse/lilypond/single_bar.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/mozart_contredanse/lilypond/single_dice_table_element.ly` & `musical_games-0.8.5/musical_games/data/dice_games/mozart_contredanse/lilypond/single_dice_table_element.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/mozart_waltz/lilypond/bar_overview.ly` & `musical_games-0.8.5/musical_games/data/dice_games/mozart_waltz/lilypond/bar_overview.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/mozart_waltz/lilypond/composition_midi.ly` & `musical_games-0.8.5/musical_games/data/dice_games/mozart_waltz/lilypond/composition_midi.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/mozart_waltz/lilypond/composition_pdf.ly` & `musical_games-0.8.5/musical_games/data/dice_games/mozart_waltz/lilypond/composition_pdf.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/mozart_waltz/lilypond/single_bar.ly` & `musical_games-0.8.5/musical_games/data/dice_games/mozart_waltz/lilypond/single_bar.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/mozart_waltz/lilypond/single_dice_table_element.ly` & `musical_games-0.8.5/musical_games/data/dice_games/mozart_waltz/lilypond/single_dice_table_element.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/mozart_waltz/waltz_bars.csv` & `musical_games-0.8.5/musical_games/data/dice_games/mozart_waltz/waltz_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/stadler_menuet_trio/lilypond/bar_overview.ly` & `musical_games-0.8.5/musical_games/data/dice_games/stadler_menuet_trio/lilypond/bar_overview.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_midi.ly` & `musical_games-0.8.5/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_midi.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_pdf.ly` & `musical_games-0.8.5/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_pdf.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_bar.ly` & `musical_games-0.8.5/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_bar.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_dice_table_element.ly` & `musical_games-0.8.5/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_dice_table_element.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/stadler_menuet_trio/menuet_bars.csv` & `musical_games-0.8.5/musical_games/data/dice_games/stadler_menuet_trio/menuet_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/dice_games/stadler_menuet_trio/trio_bars.csv` & `musical_games-0.8.5/musical_games/data/dice_games/stadler_menuet_trio/trio_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/data/lilypond_utils/clef_changes.ly` & `musical_games-0.8.5/musical_games/data/lilypond_utils/clef_changes.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/dice_games/base.py` & `musical_games-0.8.5/musical_games/dice_games/base.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/dice_games/data_csv.py` & `musical_games-0.8.5/musical_games/dice_games/data_csv.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/dice_games/dice_games.py` & `musical_games-0.8.5/musical_games/dice_games/dice_games.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/external/base.py` & `musical_games-0.8.5/musical_games/external/base.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/external/images.py` & `musical_games-0.8.5/musical_games/external/images.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/external/lilypond.py` & `musical_games-0.8.5/musical_games/external/lilypond.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/external/midi_converters.py` & `musical_games-0.8.5/musical_games/external/midi_converters.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/external/utils.py` & `musical_games-0.8.5/musical_games/external/utils.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/external/wav_converters.py` & `musical_games-0.8.5/musical_games/external/wav_converters.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/musical_games/utils.py` & `musical_games-0.8.5/musical_games/utils.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/pyproject.toml` & `musical_games-0.8.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "musical_games"
 description = "Implementation of musical dice games from the 18th century."
 readme = "README.rst"
-version = "0.8.4"
+version = "0.8.5"
 requires-python = ">=3.11"
 keywords = ["Musical games", "Dice games", "Piano music"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Education",
     "Intended Audience :: Science/Research",
```

### Comparing `musical_games-0.8.4/scripts/demo_cpe_bach.py` & `musical_games-0.8.5/scripts/demo_cpe_bach.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/scripts/demo_gerlach_scottish_dance.py` & `musical_games-0.8.5/scripts/demo_gerlach_scottish_dance.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,38 +8,38 @@
 from musical_games.dice_games.dice_games import GerlachScottishDance
 from musical_games.utils import auto_convert_lilypond_file
 
 out_dir = Path('/tmp/test')
 
 dice_game = GerlachScottishDance()
 
-# dice_game.compile_bars_overview(single_page=True).to_file(out_dir / 'overview.ly')
-# auto_convert_lilypond_file(out_dir / 'overview.ly')
+dice_game.compile_bars_overview(single_page=True).to_file(out_dir / 'overview.ly')
+auto_convert_lilypond_file(out_dir / 'overview.ly')
 
-# dice_game.compile_single_bar('dance', 6).to_file(out_dir / 'bar_dance_6.ly')
-# auto_convert_lilypond_file(out_dir / 'bar_dance_6.ly')
-# dice_game.compile_single_bar('trio', 158).to_file(out_dir / 'bar_trio_158.ly')
-# auto_convert_lilypond_file(out_dir / 'bar_trio_158.ly')
-
-# dice_game.compile_single_dice_table_element('dance',
-#                                             dice_game.get_dice_tables()['dance'].get_elements()[0]).to_file(
-#     out_dir / 'single_dice_table_element_dance_0.ly')
-# auto_convert_lilypond_file(out_dir / 'single_dice_table_element_dance_0.ly')
-#
-# dice_game.compile_single_dice_table_element('trio',
-#                                             dice_game.get_dice_tables()['trio'].get_element(3, 7)).to_file(
-#     out_dir / 'single_dice_table_element_trio_3_7.ly')
-# auto_convert_lilypond_file(out_dir / 'single_dice_table_element_trio_3_7.ly')
-
-# print(dice_game.get_duplicate_dice_table_elements('dance'))
-# print(dice_game.get_duplicate_dice_table_elements('trio'))
-# print(dice_game.count_unique_compositions(count_duplicates=True))
-# print(dice_game.count_unique_compositions(count_duplicates=False))
-#
-bar_selection = dice_game.get_random_bar_selection(seed=2)
+dice_game.compile_single_bar('dance', 6).to_file(out_dir / 'bar_dance_6.ly')
+auto_convert_lilypond_file(out_dir / 'bar_dance_6.ly')
+dice_game.compile_single_bar('trio', 158).to_file(out_dir / 'bar_trio_158.ly')
+auto_convert_lilypond_file(out_dir / 'bar_trio_158.ly')
+
+dice_game.compile_single_dice_table_element('dance',
+                                            dice_game.get_dice_tables()['dance'].get_elements()[0]).to_file(
+    out_dir / 'single_dice_table_element_dance_0.ly')
+auto_convert_lilypond_file(out_dir / 'single_dice_table_element_dance_0.ly')
+
+dice_game.compile_single_dice_table_element('trio',
+                                            dice_game.get_dice_tables()['trio'].get_element(3, 7)).to_file(
+    out_dir / 'single_dice_table_element_trio_3_7.ly')
+auto_convert_lilypond_file(out_dir / 'single_dice_table_element_trio_3_7.ly')
+
+print(dice_game.get_duplicate_dice_table_elements('dance'))
+print(dice_game.get_duplicate_dice_table_elements('trio'))
+print(dice_game.count_unique_compositions(count_duplicates=True))
+print(dice_game.count_unique_compositions(count_duplicates=False))
+
+bar_selection = dice_game.get_random_bar_selection(seed=1)
 
 dice_game.compile_composition_score(bar_selection,
                                     comment='Test', single_page=True).to_file(out_dir / 'composition_pdf.ly')
 auto_convert_lilypond_file(out_dir / 'composition_pdf.ly')
 
 midi_settings = dice_game.get_default_midi_settings()
 my_midi_settings = midi_settings.with_updated_instrument('flute', 'dance', 'piano_right_hand')
```

### Comparing `musical_games-0.8.4/scripts/demo_kirnberger_meneut_trio.py` & `musical_games-0.8.5/scripts/demo_kirnberger_meneut_trio.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/scripts/demo_kirnberger_polonaise.py` & `musical_games-0.8.5/scripts/demo_kirnberger_polonaise.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/scripts/demo_mozart_contredanse.py` & `musical_games-0.8.5/scripts/demo_mozart_contredanse.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/scripts/demo_mozart_waltz.py` & `musical_games-0.8.5/scripts/demo_mozart_waltz.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/scripts/demo_stadler_meneut_trio.py` & `musical_games-0.8.5/scripts/demo_stadler_meneut_trio.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/scripts/lilypond_copy.py` & `musical_games-0.8.5/scripts/lilypond_copy.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/scripts/lilypond_copy2.py` & `musical_games-0.8.5/scripts/lilypond_copy2.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/tox.ini` & `musical_games-0.8.5/tox.ini`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.4/PKG-INFO` & `musical_games-0.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musical_games
-Version: 0.8.4
+Version: 0.8.5
 Summary: Implementation of musical dice games from the 18th century.
 Keywords: Musical games,Dice games,Piano music
 Author-email: Robbert Harms <robbert@xkls.nl>
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

