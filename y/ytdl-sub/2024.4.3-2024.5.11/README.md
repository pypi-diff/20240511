# Comparing `tmp/ytdl-sub-2024.4.3.tar.gz` & `tmp/ytdl_sub-2024.5.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytdl-sub-2024.4.3.tar", last modified: Wed Apr  3 00:34:23 2024, max compression
+gzip compressed data, was "ytdl_sub-2024.5.11.tar", last modified: Sat May 11 02:58:38 2024, max compression
```

## Comparing `ytdl-sub-2024.4.3.tar` & `ytdl_sub-2024.5.11.tar`

### file list

```diff
@@ -1,195 +1,195 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.359598 ytdl-sub-2024.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10768 2024-04-03 00:34:23.359598 ytdl-sub-2024.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-03 00:34:23.359598 ytdl-sub-2024.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.327597 ytdl-sub-2024.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.331597 ytdl-sub-2024.4.3/src/ytdl_sub/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.331597 ytdl-sub-2024.4.3/src/ytdl_sub/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9286 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/cli/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/cli/output_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/cli/output_transaction_log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.331597 ytdl-sub-2024.4.3/src/ytdl_sub/cli/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/cli/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8960 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/cli/parsers/dl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/cli/parsers/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.335597 ytdl-sub-2024.4.3/src/ytdl_sub/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/config_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     8985 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/config_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/overrides.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.335597 ytdl-sub-2024.4.3/src/ytdl_sub/config/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/plugin/plugin_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/plugin/plugin_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/plugin/preset_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/preset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11074 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/preset_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.335597 ytdl-sub-2024.4.3/src/ytdl_sub/config/validators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/validators/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     8515 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/validators/variable_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.335597 ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.335597 ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/info_json/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/info_json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/info_json/info_json_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/source_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.335597 ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/url/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/url/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20678 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/url/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    12438 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/url/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/ytdl_options_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    10134 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/ytdlp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.339598 ytdl-sub-2024.4.3/src/ytdl_sub/entries/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/entries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/entries/base_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     9628 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/entries/entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     8410 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/entries/entry_parent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.339598 ytdl-sub-2024.4.3/src/ytdl_sub/entries/script/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/entries/script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/entries/script/custom_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/entries/script/function_scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)    42267 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/entries/script/variable_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/entries/script/variable_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.339598 ytdl-sub-2024.4.3/src/ytdl_sub/entries/variables/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/entries/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/entries/variables/override_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.343598 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/audio_extract.py
--rw-r--r--   0 runner    (1001) docker     (127)    14565 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/chapters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/date_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/embed_thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/file_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/filter_exclude.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/filter_include.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/format.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.343598 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/internal/view.py
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/match_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/music_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     9418 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/nfo_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/output_directory_nfo_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    18653 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/regex.py
--rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/split_by_chapters.py
--rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/throttle_protection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/video_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.343598 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.343598 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/helpers/download_deletion_options.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/helpers/media_quality.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/helpers/players.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    23681 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/helpers/url.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/helpers/url_bilateral.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.343598 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/internal/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/internal/view.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.343598 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music/albums_from_chapters.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music/albums_from_playlists.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music/other_websites.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music/singles.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.343598 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music_videos/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music_videos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music_videos/music_video_base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music_videos/music_videos.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.347598 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/tv_show/
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    34839 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.347598 ytdl-sub-2024.4.3/src/ytdl_sub/script/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.347598 ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/array_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/boolean_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/conditional_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/date_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/error_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/json_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/map_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/numeric_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/regex_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/string_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    21712 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    22535 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/script_output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.347598 ytdl-sub-2024.4.3/src/ytdl_sub/script/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/types/array.py
--rw-r--r--   0 runner    (1001) docker     (127)    11506 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/types/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/types/map.py
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/types/resolvable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/types/syntax_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/types/variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/types/variable_dependency.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.351598 ytdl-sub-2024.4.3/src/ytdl_sub/script/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/utils/exception_formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/utils/name_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9293 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/utils/type_checking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.351598 ytdl-sub-2024.4.3/src/ytdl_sub/subscriptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/subscriptions/base_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/subscriptions/subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)    16254 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/subscriptions/subscription_download.py
--rw-r--r--   0 runner    (1001) docker     (127)    12923 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/subscriptions/subscription_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/subscriptions/subscription_ytdl_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.351598 ytdl-sub-2024.4.3/src/ytdl_sub/thread/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/thread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/thread/log_entries_downloaded_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.355598 ytdl-sub-2024.4.3/src/ytdl_sub/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8469 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/chapters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/ffmpeg.py
--rw-r--r--   0 runner    (1001) docker     (127)    16310 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/file_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/file_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/scriptable.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/xml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.355598 ytdl-sub-2024.4.3/src/ytdl_sub/validators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/validators/audo_codec_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/validators/file_path_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/validators/nfo_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/validators/regex_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/validators/source_variable_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/validators/strict_dict_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/validators/string_datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     9137 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/validators/string_formatter_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/validators/string_select_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9307 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/validators/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.355598 ytdl-sub-2024.4.3/src/ytdl_sub/ytdl_additions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/ytdl_additions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23454 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.355598 ytdl-sub-2024.4.3/src/ytdl_sub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10768 2024-04-03 00:34:23.000000 ytdl-sub-2024.4.3/src/ytdl_sub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-04-03 00:34:23.000000 ytdl-sub-2024.4.3/src/ytdl_sub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 00:34:23.000000 ytdl-sub-2024.4.3/src/ytdl_sub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-03 00:34:23.000000 ytdl-sub-2024.4.3/src/ytdl_sub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-03 00:34:23.000000 ytdl-sub-2024.4.3/src/ytdl_sub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 00:34:23.000000 ytdl-sub-2024.4.3/src/ytdl_sub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.905420 ytdl_sub-2024.5.11/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    51272 2024-05-11 02:58:38.905420 ytdl_sub-2024.5.11/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 02:58:38.905420 ytdl_sub-2024.5.11/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.873420 ytdl_sub-2024.5.11/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.877420 ytdl_sub-2024.5.11/src/ytdl_sub/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.877420 ytdl_sub-2024.5.11/src/ytdl_sub/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9286 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/cli/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/cli/output_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/cli/output_transaction_log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.877420 ytdl_sub-2024.5.11/src/ytdl_sub/cli/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/cli/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8960 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/cli/parsers/dl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/cli/parsers/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.881420 ytdl_sub-2024.5.11/src/ytdl_sub/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/config/config_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9123 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/config/config_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/config/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/config/overrides.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.881420 ytdl_sub-2024.5.11/src/ytdl_sub/config/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/config/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/config/plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/config/plugin/plugin_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/config/plugin/plugin_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/config/plugin/preset_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/config/preset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11074 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/config/preset_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.881420 ytdl_sub-2024.5.11/src/ytdl_sub/config/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/config/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/config/validators/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8516 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/config/validators/variable_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.881420 ytdl_sub-2024.5.11/src/ytdl_sub/downloaders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/downloaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.881420 ytdl_sub-2024.5.11/src/ytdl_sub/downloaders/info_json/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/downloaders/info_json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/downloaders/info_json/info_json_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/downloaders/source_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.881420 ytdl_sub-2024.5.11/src/ytdl_sub/downloaders/url/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/downloaders/url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20577 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/downloaders/url/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12438 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/downloaders/url/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/downloaders/ytdl_options_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10134 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/downloaders/ytdlp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.881420 ytdl_sub-2024.5.11/src/ytdl_sub/entries/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/entries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/entries/base_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9628 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/entries/entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8410 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/entries/entry_parent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.885420 ytdl_sub-2024.5.11/src/ytdl_sub/entries/script/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/entries/script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/entries/script/custom_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/entries/script/function_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42312 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/entries/script/variable_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/entries/script/variable_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.885420 ytdl_sub-2024.5.11/src/ytdl_sub/entries/variables/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/entries/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/entries/variables/override_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.889420 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/audio_extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14569 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/date_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/embed_thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/file_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/filter_exclude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/filter_include.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.889420 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/internal/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/match_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/music_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9418 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/nfo_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/output_directory_nfo_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18653 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/split_by_chapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/throttle_protection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/video_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.889420 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.889420 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/helpers/download_deletion_options.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/helpers/media_quality.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/helpers/players.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    23681 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/helpers/url.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/helpers/url_bilateral.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.889420 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/internal/view.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.889420 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/music/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/music/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/music/albums_from_chapters.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/music/albums_from_playlists.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/music/other_websites.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/music/singles.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.889420 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/music_videos/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/music_videos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/music_videos/music_video_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/music_videos/music_videos.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.893420 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/tv_show/
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    34839 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.893420 ytdl_sub-2024.5.11/src/ytdl_sub/script/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.893420 ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/array_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/boolean_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/conditional_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/date_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/error_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/json_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/map_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/numeric_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/regex_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/string_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21725 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22535 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/script_output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.897420 ytdl_sub-2024.5.11/src/ytdl_sub/script/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/types/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11506 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/types/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/types/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/types/resolvable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/types/syntax_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/types/variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/types/variable_dependency.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.897420 ytdl_sub-2024.5.11/src/ytdl_sub/script/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/utils/exception_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/utils/name_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9293 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/utils/type_checking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.897420 ytdl_sub-2024.5.11/src/ytdl_sub/subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/subscriptions/base_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/subscriptions/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16237 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/subscriptions/subscription_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12929 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/subscriptions/subscription_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/subscriptions/subscription_ytdl_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.897420 ytdl_sub-2024.5.11/src/ytdl_sub/thread/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/thread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/thread/log_entries_downloaded_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.901420 ytdl_sub-2024.5.11/src/ytdl_sub/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8469 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/utils/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/utils/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/utils/ffmpeg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16310 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/utils/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/utils/file_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/utils/file_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/utils/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/utils/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/utils/scriptable.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/utils/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/utils/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/utils/thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/utils/xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/utils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.901420 ytdl_sub-2024.5.11/src/ytdl_sub/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/validators/audo_codec_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/validators/file_path_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/validators/nfo_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/validators/regex_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/validators/source_variable_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/validators/strict_dict_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/validators/string_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9068 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/validators/string_formatter_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/validators/string_select_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9352 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/validators/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.905420 ytdl_sub-2024.5.11/src/ytdl_sub/ytdl_additions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/ytdl_additions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23454 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.905420 ytdl_sub-2024.5.11/src/ytdl_sub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    51272 2024-05-11 02:58:38.000000 ytdl_sub-2024.5.11/src/ytdl_sub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6635 2024-05-11 02:58:38.000000 ytdl_sub-2024.5.11/src/ytdl_sub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 02:58:38.000000 ytdl_sub-2024.5.11/src/ytdl_sub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-11 02:58:38.000000 ytdl_sub-2024.5.11/src/ytdl_sub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-11 02:58:38.000000 ytdl_sub-2024.5.11/src/ytdl_sub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-11 02:58:38.000000 ytdl_sub-2024.5.11/src/ytdl_sub.egg-info/top_level.txt
```

### Comparing `ytdl-sub-2024.4.3/LICENSE` & `ytdl_sub-2024.5.11/LICENSE`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/PKG-INFO` & `ytdl_sub-2024.5.11/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,47 +1,7 @@
-Metadata-Version: 2.1
-Name: ytdl-sub
-Version: 2024.4.3
-Summary: Automate downloading and metadata generation with YoutubeDL
-Home-page: https://github.com/jmbannon/ytdl-sub
-Author: Jesse Bannon
-Author-email: use_github_issues@nope.com
-License: GNUv3
-Platform: Unix
-Classifier: Topic :: Multimedia :: Sound/Audio
-Classifier: Topic :: Multimedia :: Video
-Classifier: License :: Public Domain
-Classifier: Environment :: Console
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: yt-dlp==2024.3.10
-Requires-Dist: argparse==1.4.0
-Requires-Dist: colorama==0.4.6
-Requires-Dist: mergedeep==1.3.4
-Requires-Dist: mediafile==0.12.0
-Requires-Dist: PyYAML==5.3.1
-Provides-Extra: test
-Requires-Dist: coverage[toml]==6.3.2; extra == "test"
-Requires-Dist: pytest==7.1.1; extra == "test"
-Requires-Dist: pytest-rerunfailures==12.0; extra == "test"
-Provides-Extra: lint
-Requires-Dist: black==22.3.0; extra == "lint"
-Requires-Dist: isort==5.10.1; extra == "lint"
-Requires-Dist: pylint==2.13.5; extra == "lint"
-Provides-Extra: docs
-Requires-Dist: sphinx==7.2.6; extra == "docs"
-Requires-Dist: sphinx-rtd-theme==2.0.0; extra == "docs"
-Requires-Dist: sphinx-book-theme==1.1.0; extra == "docs"
-Provides-Extra: build
-Requires-Dist: build; extra == "build"
-Requires-Dist: twine; extra == "build"
-Requires-Dist: pyinstaller; extra == "build"
-
 # ytdl-sub
 ## Automate downloading and metadata generation with YoutubeDL.
 [<img src="https://img.shields.io/badge/readthedocs-link-blue?logo=readthedocs">](https://ytdl-sub.readthedocs.io/en/latest/index.html)
 [<img src="https://img.shields.io/discord/994270357957648404?logo=Discord">](https://discord.gg/v8j9RAHb4k)
 [![codecov](https://img.shields.io/codecov/c/github/jmbannon/ytdl-sub)](https://app.codecov.io/gh/jmbannon/ytdl-sub)
 ![Code Qaulity](https://img.shields.io/badge/pylint-10%2F10-brightgreen)
 ![Checks](https://img.shields.io/github/checks-status/jmbannon/ytdl-sub/master)
```

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/cli/entrypoint.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/cli/output_summary.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/cli/output_summary.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/cli/output_transaction_log.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/cli/output_transaction_log.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/cli/parsers/dl.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/cli/parsers/dl.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/cli/parsers/main.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/cli/parsers/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,14 +146,16 @@
 parser = argparse.ArgumentParser(
     description="ytdl-sub: Automate download and adding metadata with YoutubeDL",
 )
 parser.add_argument("-v", "--version", action="version", version="%(prog)s " + __local_version__)
 _add_shared_arguments(parser, suppress_defaults=False)
 
 subparsers = parser.add_subparsers(dest="subparser")
+
+
 ###################################################################################################
 # SUBSCRIPTION PARSER
 class SubArguments:
     UPDATE_WITH_INFO_JSON = CLIArgument(
         short="-u",
         long="--update-with-info-json",
     )
```

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/config/config_file.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/config/config_file.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/config/config_validator.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/config/config_validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import os
+import posixpath
 from typing import Any
 from typing import Dict
 from typing import Optional
 
 from mergedeep import mergedeep
 from yt_dlp.utils import datetime_from_str
 
@@ -143,15 +145,16 @@
 
     @property
     def working_directory(self) -> str:
         """
         The directory to temporarily store downloaded files before moving them into their final
         directory. Defaults to .ytdl-sub-working-directory
         """
-        return self._working_directory.value
+        # Expands tildas to actual paths, use native os sep
+        return os.path.expanduser(self._working_directory.value.replace(posixpath.sep, os.sep))
 
     @property
     def umask(self) -> Optional[str]:
         """
         Umask (octal format) to apply to every created file. Defaults to "022".
         """
         return self._umask.value
```

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/config/defaults.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/config/defaults.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/config/overrides.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/config/overrides.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/config/plugin/plugin.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/config/plugin/plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,44 +5,44 @@
 from typing import Generic
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Type
 
 from ytdl_sub.config.overrides import Overrides
+from ytdl_sub.config.validators.options import OptionsValidatorT
 from ytdl_sub.config.validators.options import ToggleableOptionsDictValidator
-from ytdl_sub.config.validators.options import TOptionsValidator
 from ytdl_sub.entries.entry import Entry
 from ytdl_sub.utils.file_handler import FileMetadata
 from ytdl_sub.utils.script import ScriptUtils
 from ytdl_sub.ytdl_additions.enhanced_download_archive import DownloadArchiver
 from ytdl_sub.ytdl_additions.enhanced_download_archive import EnhancedDownloadArchive
 
-# pylint: disable=no-self-use,unused-argument
+# pylint: disable=unused-argument
 
 
-class BasePlugin(DownloadArchiver, Generic[TOptionsValidator], ABC):
+class BasePlugin(DownloadArchiver, Generic[OptionsValidatorT], ABC):
     """
     Shared code amongst all SourcePlugins (downloaders) and Plugins (post-download modification)
     """
 
-    plugin_options_type: Type[TOptionsValidator]
+    plugin_options_type: Type[OptionsValidatorT]
 
     def __init__(
         self,
-        options: TOptionsValidator,
+        options: OptionsValidatorT,
         overrides: Overrides,
         enhanced_download_archive: EnhancedDownloadArchive,
     ):
         DownloadArchiver.__init__(self=self, enhanced_download_archive=enhanced_download_archive)
         self.plugin_options = options
         self.overrides = overrides
 
 
-class Plugin(BasePlugin[TOptionsValidator], Generic[TOptionsValidator], ABC):
+class Plugin(BasePlugin[OptionsValidatorT], Generic[OptionsValidatorT], ABC):
     """
     Class to define the new plugin functionality
     """
 
     @cached_property
     def is_enabled(self) -> bool:
         """
@@ -117,15 +117,15 @@
 
     def post_process_subscription(self):
         """
         After all downloaded files have been post-processed, apply a subscription-wide post process
         """
 
 
-class SplitPlugin(Plugin[TOptionsValidator], Generic[TOptionsValidator], ABC):
+class SplitPlugin(Plugin[OptionsValidatorT], Generic[OptionsValidatorT], ABC):
     """
     Plugin that splits entries into zero or more entries
     """
 
     @abstractmethod
     def split(self, entry: Entry) -> List[Tuple[Entry, FileMetadata]]:
         """
```

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/config/plugin/plugin_mapping.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/config/plugin/plugin_mapping.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/config/plugin/preset_plugins.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/config/plugin/preset_plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Type
 
 from ytdl_sub.config.plugin.plugin import Plugin
 from ytdl_sub.config.validators.options import OptionsValidator
-from ytdl_sub.config.validators.options import TOptionsValidator
+from ytdl_sub.config.validators.options import OptionsValidatorT
 
 
 class PresetPlugins:
     def __init__(self):
         self.plugin_types: List[Type[Plugin]] = []
         self.plugin_options: List[OptionsValidator] = []
 
@@ -25,15 +25,15 @@
         """
         Returns
         -------
         Plugin and PluginOptions zipped
         """
         return list(zip(self.plugin_types, self.plugin_options))
 
-    def get(self, plugin_type: Type[TOptionsValidator]) -> Optional[TOptionsValidator]:
+    def get(self, plugin_type: Type[OptionsValidatorT]) -> Optional[OptionsValidatorT]:
         """
         Parameters
         ----------
         plugin_type
             Fetch the plugin options for this type
 
         Returns
```

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/config/preset.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/config/preset.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/config/preset_options.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/config/preset_options.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/config/validators/options.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/config/validators/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 from ytdl_sub.config.plugin.plugin_operation import PluginOperation
 from ytdl_sub.utils.exceptions import ValidationException
 from ytdl_sub.validators.strict_dict_validator import StrictDictValidator
 from ytdl_sub.validators.string_formatter_validators import OverridesBooleanFormatterValidator
 from ytdl_sub.validators.validators import Validator
 
-# pylint: disable=no-self-use
 # pylint: disable=unused-argument
 
 
 class OptionsValidator(Validator, ABC):
     """
     Abstract class that validates options for preset sections (plugins, downloaders)
     """
@@ -49,15 +48,15 @@
     ) -> Dict[PluginOperation, Set[str]]:
         """
         If the plugin adds source variables, list them here.
         """
         return {}
 
 
-TOptionsValidator = TypeVar("TOptionsValidator", bound=OptionsValidator)
+OptionsValidatorT = TypeVar("OptionsValidatorT", bound=OptionsValidator)
 
 
 class OptionsDictValidator(StrictDictValidator, OptionsValidator, ABC):
     pass
 
 
 class ToggleableOptionsDictValidator(OptionsDictValidator):
```

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/config/validators/variable_validation.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/config/validators/variable_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from ytdl_sub.validators.string_formatter_validators import validate_formatters
 
 # Entry variables to mock during validation
 _DUMMY_ENTRY_VARIABLES: Dict[str, str] = {
     name: to_variable_dependency_format_string(
         # pylint: disable=protected-access
         script=BASE_SCRIPT,
-        parsed_format_string=BASE_SCRIPT._variables[name]
+        parsed_format_string=BASE_SCRIPT._variables[name],
         # pylint: enable=protected-access
     )
     for name in BASE_SCRIPT.variable_names
 }
 
 
 def _add_dummy_variables(variables: Iterable[str]) -> Dict[str, str]:
```

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/info_json/info_json_downloader.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/downloaders/info_json/info_json_downloader.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/source_plugin.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/downloaders/source_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,41 +7,41 @@
 from typing import Optional
 from typing import Type
 from typing import final
 
 from ytdl_sub.config.overrides import Overrides
 from ytdl_sub.config.plugin.plugin import BasePlugin
 from ytdl_sub.config.plugin.plugin import Plugin
-from ytdl_sub.config.validators.options import TOptionsValidator
+from ytdl_sub.config.validators.options import OptionsValidatorT
 from ytdl_sub.downloaders.ytdl_options_builder import YTDLOptionsBuilder
 from ytdl_sub.entries.entry import Entry
 from ytdl_sub.ytdl_additions.enhanced_download_archive import EnhancedDownloadArchive
 
 
-class SourcePluginExtension(Plugin[TOptionsValidator], Generic[TOptionsValidator], ABC):
+class SourcePluginExtension(Plugin[OptionsValidatorT], Generic[OptionsValidatorT], ABC):
     """
     Plugins that get added automatically by using a downloader. Downloader options
     are the plugin options.
     """
 
     @final
     def ytdl_options(self) -> Optional[Dict]:
         """
         SourcePluginExtensions are intended to run after downloading. ytdl_options at that point
         are not needed.
         """
         return None
 
 
-class SourcePlugin(BasePlugin[TOptionsValidator], Generic[TOptionsValidator], ABC):
+class SourcePlugin(BasePlugin[OptionsValidatorT], Generic[OptionsValidatorT], ABC):
     plugin_extensions: List[Type[SourcePluginExtension]] = []
 
     def __init__(
         self,
-        options: TOptionsValidator,
+        options: OptionsValidatorT,
         enhanced_download_archive: EnhancedDownloadArchive,
         download_ytdl_options: YTDLOptionsBuilder,
         metadata_ytdl_options: YTDLOptionsBuilder,
         overrides: Overrides,
     ):
         super().__init__(
             options=options,
```

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/url/downloader.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/downloaders/url/downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,17 +244,19 @@
         -------
         YTLD options dict for downloading
         """
         return (
             self._download_ytdl_options_builder.clone()
             .add(self.ytdl_option_defaults(), before=True)
             .add(
-                self.plugin_options.urls.list[url_idx].ytdl_options.dict
-                if url_idx is not None
-                else None,
+                (
+                    self.plugin_options.urls.list[url_idx].ytdl_options.dict
+                    if url_idx is not None
+                    else None
+                ),
                 before=True,
             )
             .to_dict()
         )
 
     def metadata_ytdl_options(self, ytdl_option_overrides: Dict) -> Dict:
         """
@@ -348,17 +350,19 @@
 
     def _extract_entry_info_with_retry(self, entry: Entry) -> Entry:
         download_entry_dict = YTDLP.extract_info_with_retry(
             ytdl_options_overrides=self.download_ytdl_options(
                 url_idx=entry.get(v.ytdl_sub_input_url_index, int)
             ),
             is_downloaded_fn=None if self.is_dry_run else entry.is_downloaded,
-            is_thumbnail_downloaded_fn=None
-            if (self.is_dry_run or not self.is_entry_thumbnails_enabled)
-            else entry.is_thumbnail_downloaded_via_ytdlp,
+            is_thumbnail_downloaded_fn=(
+                None
+                if (self.is_dry_run or not self.is_entry_thumbnails_enabled)
+                else entry.is_thumbnail_downloaded_via_ytdlp
+            ),
             url=entry.webpage_url,
         )
         return Entry(
             download_entry_dict,
             working_directory=self.working_directory,
         )
 
@@ -389,25 +393,23 @@
             self._mark_downloaded(entries_to_iter[idx])
 
             entries_to_iter[idx] = None
 
     def _iterate_parent_entry(
         self, parent: EntryParent, download_reversed: bool
     ) -> Iterator[Entry]:
-        for entry_child in self._iterate_child_entries(
+        yield from self._iterate_child_entries(
             entries=parent.entry_children(), download_reversed=download_reversed
-        ):
-            yield entry_child
+        )
 
         # Recursion the parent's parent entries
         for parent_child in reversed(parent.parent_children()):
-            for entry_child in self._iterate_parent_entry(
+            yield from self._iterate_parent_entry(
                 parent=parent_child, download_reversed=download_reversed
-            ):
-                yield entry_child
+            )
 
     def _download_url_metadata(
         self, url: str, include_sibling_metadata: bool, ytdl_options_overrides: Dict
     ) -> Tuple[List[EntryParent], List[Entry]]:
         """
         Downloads only info.json files and forms EntryParent trees
         """
@@ -441,23 +443,21 @@
     ) -> Iterator[Entry]:
         """
         Downloads the leaf entries from EntryParent trees
         """
         # Delete info json files afterwards so other collection URLs do not use them
         with self._separate_download_archives(clear_info_json_files=True):
             for parent in parents:
-                for entry_child in self._iterate_parent_entry(
+                yield from self._iterate_parent_entry(
                     parent=parent, download_reversed=download_reversed
-                ):
-                    yield entry_child
+                )
 
-            for orphan in self._iterate_child_entries(
+            yield from self._iterate_child_entries(
                 entries=orphans, download_reversed=download_reversed
-            ):
-                yield orphan
+            )
 
     def _download_metadata(self, url: str, validator: UrlValidator) -> Iterable[Entry]:
         metadata_ytdl_options = self.metadata_ytdl_options(
             ytdl_option_overrides=validator.ytdl_options.dict
         )
         download_reversed = ScriptUtils.bool_formatter_output(
             self.overrides.apply_formatter(validator.download_reverse)
@@ -471,20 +471,19 @@
 
         # TODO: Encapsulate this logic into its own class
         self._url_state = URLDownloadState(
             entries_total=sum(parent.num_children() for parent in parents) + len(orphan_entries)
         )
 
         download_logger.info("Beginning downloads for %s", url)
-        for entry in self._iterate_entries(
+        yield from self._iterate_entries(
             parents=parents,
             orphans=orphan_entries,
             download_reversed=download_reversed,
-        ):
-            yield entry
+        )
 
     def download_metadata(self) -> Iterable[Entry]:
         """The function to perform the download of all media entries"""
         # download the bottom-most urls first since they are top-priority
         for idx, url_validator in reversed(list(enumerate(self.collection.urls.list))):
             # URLs can be empty. If they are, then skip
             if not (url := self.overrides.apply_formatter(url_validator.url)):
```

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/url/validators.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/downloaders/url/validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/ytdl_options_builder.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/downloaders/ytdl_options_builder.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/ytdlp.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/downloaders/ytdlp.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/entries/base_entry.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/entries/base_entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from yt_dlp.utils import sanitize_filename
 
 from ytdl_sub.entries.script.variable_definitions import VARIABLES
 from ytdl_sub.entries.script.variable_definitions import VariableDefinitions
 
 v: VariableDefinitions = VARIABLES
 
-TBaseEntry = TypeVar("TBaseEntry", bound="BaseEntry")
+BaseEntryT = TypeVar("BaseEntryT", bound="BaseEntry")
 
 
 class BaseEntry(ABC):
     """
     Abstract entry object to represent anything download from ytdl (playlist metadata, media, etc).
     """
 
@@ -136,39 +136,39 @@
         Returns
         -------
         Entry's downloaded info json file path
         """
         return str(Path(self.working_directory()) / self.get_download_info_json_name())
 
     @final
-    def to_type(self, entry_type: Type[TBaseEntry]) -> TBaseEntry:
+    def to_type(self, entry_type: Type[BaseEntryT]) -> BaseEntryT:
         """
         Returns
         -------
         Converted EntryParent to Entry-like class
         """
         return entry_type(entry_dict=self._kwargs, working_directory=self._working_directory)
 
     @classmethod
-    def is_entry_parent(cls, entry_dict: Dict | TBaseEntry):
+    def is_entry_parent(cls, entry_dict: Dict | BaseEntryT):
         """
         Returns
         -------
         True if it is a parent. False otherwise
         """
         entry_type: Optional[str] = None
         if isinstance(entry_dict, cls):
             entry_type = entry_dict._kwargs_get("_type")
         if isinstance(entry_dict, dict):
             entry_type = entry_dict.get("_type")
 
         return entry_type == "playlist"
 
     @classmethod
-    def is_entry(cls, entry_dict: Dict | TBaseEntry):
+    def is_entry(cls, entry_dict: Dict | BaseEntryT):
         """
         Returns
         -------
         True if it is an entry. False otherwise
         """
         entry_ext: Optional[str] = None
         if isinstance(entry_dict, cls):
```

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/entries/entry.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/entries/entry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/entries/entry_parent.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/entries/entry_parent.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Set
 from urllib.parse import urlparse
 
 from ytdl_sub.entries.base_entry import BaseEntry
-from ytdl_sub.entries.base_entry import TBaseEntry
+from ytdl_sub.entries.base_entry import BaseEntryT
 from ytdl_sub.entries.entry import Entry
 from ytdl_sub.entries.script.variable_definitions import VARIABLES
 from ytdl_sub.entries.script.variable_definitions import VariableDefinitions
 from ytdl_sub.entries.script.variable_types import MetadataVariable
 
 v: VariableDefinitions = VARIABLES
 
 
 # pylint: disable=protected-access
 
 
 class EntryParent(BaseEntry):
     @classmethod
-    def _sort_entries(cls, entries: List[TBaseEntry]) -> List[TBaseEntry]:
+    def _sort_entries(cls, entries: List[BaseEntryT]) -> List[BaseEntryT]:
         """Try sorting by playlist_id first, then fall back to uid"""
         return sorted(
             entries,
             key=lambda ent: (ent._kwargs_get(v.playlist_index.metadata_key, math.inf), ent.uid),
         )
 
     def __init__(self, entry_dict: Dict, working_directory: str):
```

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/entries/script/custom_functions.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/entries/script/custom_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,17 +32,17 @@
             value = String(value.value.replace("{", "｛").replace("}", "｝"))
         return value
 
     @staticmethod
     def to_native_filepath(filepath: String) -> String:
         """
         Convert any unix-based path separators ('/') with the OS's native
-        separator.
+        separator. In addition, expand ~ to absolute directories.
         """
-        return String(filepath.value.replace(posixpath.sep, os.sep))
+        return String(os.path.expanduser(filepath.value.replace(posixpath.sep, os.sep)))
 
     @staticmethod
     def truncate_filepath_if_too_long(filepath: String) -> String:
         """
         If a file-path is too long for the OS, this function will truncate it while preserving
         the extension.
         """
```

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/entries/script/function_scripts.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/entries/script/function_scripts.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/entries/script/variable_definitions.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/entries/script/variable_definitions.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from ytdl_sub.entries.script.variable_types import StringVariable
 from ytdl_sub.entries.script.variable_types import Variable
 
 # This file contains mixins to a BaseEntry subclass. Ignore pylint's "no kwargs member" suggestion
 # pylint: disable=no-member
 # pylint: disable=too-many-public-methods
 # pylint: disable=too-many-lines
+# pylint: disable=method-cache-max-size-none
 
 
 class MetadataVariableDefinitions(ABC):
     @cached_property
     def entry_metadata(self: "VariableDefinitions") -> MapVariable:
         """
         :description:
```

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/entries/script/variable_types.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/entries/script/variable_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 from ytdl_sub.script.types.resolvable import Integer
 from ytdl_sub.script.types.resolvable import String
 
 ENTRY_METADATA_VARIABLE_NAME = "entry_metadata"
 PLAYLIST_METADATA_VARIABLE_NAME = "playlist_metadata"
 SOURCE_METADATA_VARIABLE_NAME = "source_metadata"
 
-TMetadataVariable = TypeVar("TMetadataVariable", bound="MetadataVariable")
-TVariable = TypeVar("TVariable", bound="Variable")
+MetadataVariableT = TypeVar("MetadataVariableT", bound="MetadataVariable")
+VariableT = TypeVar("VariableT", bound="Variable")
 
 
 def _get(
     cast: str,
     metadata_variable_name: str,
     metadata_key: str,
     variable_name: Optional[str],
-    default: Optional[TVariable | str | int | Dict | List],
-    as_type: Type[TMetadataVariable],
-) -> TMetadataVariable:
+    default: Optional[VariableT | str | int | Dict | List],
+    as_type: Type[MetadataVariableT],
+) -> MetadataVariableT:
     if default is None:
         # TODO: assert with good error message if key DNE
         out = f"%map_get({metadata_variable_name}, '{metadata_key}')"
     elif isinstance(default, Variable):
         args = f"{metadata_variable_name}, '{metadata_key}', {default.variable_name}"
         out = f"%map_get_non_empty({args})"
     elif isinstance(default, str):
```

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/entries/variables/override_variables.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/entries/variables/override_variables.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/main.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/main.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/audio_extract.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/plugins/audio_extract.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/chapters.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/plugins/chapters.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,21 +259,21 @@
 
         if self._is_removing_chapters:
             remove_chapters_post_processor = {
                 "key": "ModifyChapters",
                 "force_keyframes": self.plugin_options.force_key_frames,
             }
             if self.plugin_options.remove_sponsorblock_categories is not None:
-                remove_chapters_post_processor[
-                    "remove_sponsor_segments"
-                ] = self.plugin_options.remove_sponsorblock_categories
+                remove_chapters_post_processor["remove_sponsor_segments"] = (
+                    self.plugin_options.remove_sponsorblock_categories
+                )
             if self.plugin_options.remove_chapters_regex is not None:
-                remove_chapters_post_processor[
-                    "remove_chapters_patterns"
-                ] = self.plugin_options.remove_chapters_regex
+                remove_chapters_post_processor["remove_chapters_patterns"] = (
+                    self.plugin_options.remove_chapters_regex
+                )
 
             if self.plugin_options.embed_chapters:
                 builder.add(
                     {
                         # re-add chapters
                         "postprocessors": [
                             remove_chapters_post_processor,
```

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/date_range.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/plugins/date_range.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/embed_thumbnail.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/plugins/embed_thumbnail.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/file_convert.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/plugins/file_convert.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/filter_exclude.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/plugins/filter_exclude.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/filter_include.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/plugins/filter_include.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/format.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/plugins/format.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/internal/view.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/plugins/internal/view.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/match_filters.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/plugins/match_filters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/music_tags.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/plugins/music_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/nfo_tags.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/plugins/nfo_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/output_directory_nfo_tags.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/plugins/output_directory_nfo_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/regex.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/plugins/regex.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/split_by_chapters.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/plugins/split_by_chapters.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,17 +155,17 @@
         timestamp_begin = chapters.timestamps[idx].readable_str
         timestamp_end = Timestamp(new_entry.get(v.duration, int)).readable_str
         if idx + 1 < len(chapters.timestamps):
             timestamp_end = chapters.timestamps[idx + 1].readable_str
 
         metadata_value_dict = {}
         if self.is_dry_run:
-            metadata_value_dict[
-                "Warning"
-            ] = "Dry-run assumes embedded chapters with no modifications"
+            metadata_value_dict["Warning"] = (
+                "Dry-run assumes embedded chapters with no modifications"
+            )
 
         metadata_value_dict["Source Title"] = new_entry.title
         metadata_value_dict["Segment"] = f"{timestamp_begin} - {timestamp_end}"
 
         metadata = FileMetadata.from_dict(
             value_dict=metadata_value_dict,
             title="From Chapter Split",
```

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/subtitles.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/plugins/subtitles.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/throttle_protection.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/plugins/throttle_protection.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/video_tags.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/plugins/video_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/__init__.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/helpers/download_deletion_options.yaml` & `ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/helpers/download_deletion_options.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/helpers/media_quality.yaml` & `ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/helpers/media_quality.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/helpers/players.yaml` & `ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/helpers/players.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/helpers/url.yaml` & `ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/helpers/url.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/helpers/url_bilateral.yaml` & `ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/helpers/url_bilateral.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music/albums_from_chapters.yaml` & `ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/music/albums_from_chapters.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music/albums_from_playlists.yaml` & `ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/music/albums_from_playlists.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music/other_websites.yaml` & `ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/music/other_websites.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music/singles.yaml` & `ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/music/singles.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music_videos/music_video_base.yaml` & `ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/music_videos/music_video_base.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music_videos/music_videos.yaml` & `ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/music_videos/music_videos.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml` & `ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml` & `ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml` & `ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml` & `ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/__init__.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/array_functions.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/array_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/boolean_functions.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/boolean_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/conditional_functions.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/conditional_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/error_functions.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/error_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/json_functions.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/json_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/map_functions.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/map_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/numeric_functions.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/numeric_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/regex_functions.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/regex_functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,7 +48,17 @@
     @staticmethod
     def regex_capture_groups(regex: String) -> Integer:
         """
         :description:
           Returns number of capture groups in regex
         """
         return Integer(re.compile(regex.value).groups)
+
+    @staticmethod
+    def regex_sub(regex: String, replacement: String, string: String) -> String:
+        """
+        :description:
+          Returns the string obtained by replacing the leftmost non-overlapping occurrences of the
+          pattern in string by the replacement string. The replacement string can reference the
+          match groups via backslash escapes. Callables as replacement argument are not supported.
+        """
+        return String(re.sub(regex.value, replacement.value, string.value))
```

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/string_functions.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/string_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/script/parser.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/script/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,15 +243,15 @@
 
     def _parse_numeric(self) -> Integer | Float:
         numeric_string = ""
 
         if self._read(increment_pos=False) == "-":
             numeric_string += "-"
             self._pos += 1
-        if has_decimal := (self._read(increment_pos=False) == "."):
+        if has_decimal := self._read(increment_pos=False) == ".":
             numeric_string += "."
             self._pos += 1
 
         while ch := self._read(increment_pos=False):
             if ch == "-":
                 raise NUMERICS_INVALID_CHAR
 
@@ -500,15 +500,17 @@
                     raise MAP_KEY_NOT_HASHABLE
                 if len(value_args) > 1:
                     raise MAP_KEY_MULTIPLE_VALUES
 
                 output[key] = value_args[0]
                 key = None
             else:
-                raise UNREACHABLE
+                break
+
+        raise UNREACHABLE
 
     def _parse_main_loop(self, ch: str) -> bool:
         if ch == "\\" and self._read(increment_pos=False) in {"{", "}"}:
             # Escape brackets are \{ and \}, only add the second char
             self._literal_str += self._read()
             return True
         if ch == "}":
```

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/script/script.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/script/script.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/script/script_output.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/script/script_output.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/script/types/array.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/script/types/array.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/script/types/function.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/script/types/function.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/script/types/map.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/script/types/map.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/script/types/resolvable.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/script/types/resolvable.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/script/types/syntax_tree.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/script/types/syntax_tree.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/script/types/variable.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/script/types/variable.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/script/types/variable_dependency.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/script/types/variable_dependency.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/script/utils/exception_formatters.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/script/utils/exception_formatters.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 from ytdl_sub.script.types.resolvable import BuiltInFunctionType
 from ytdl_sub.script.utils.exceptions import IncompatibleFunctionArguments
 from ytdl_sub.script.utils.exceptions import UserException
 from ytdl_sub.script.utils.type_checking import FunctionSpec
 from ytdl_sub.script.utils.type_checking import is_union
 
-TUserException = TypeVar("TUserException", bound=UserException)
+UserExceptionT = TypeVar("UserExceptionT", bound=UserException)
 
 
 class ParserExceptionFormatter:
-    def __init__(self, text: str, start: int, end: int, exception: TUserException):
+    def __init__(self, text: str, start: int, end: int, exception: UserExceptionT):
         self._text = text
         self._start = start
         self._end = end
         self._exception = exception
 
     def _exception_text(self, border: int):
         """
@@ -74,15 +74,15 @@
             if idx == true_start_line:
                 to_return.append(f">>> {split_text[idx][min_leading_spaces:]}")
             else:
                 to_return.append(f"    {split_text[idx][min_leading_spaces:]}")
 
         return "\n" + "\n".join(to_return)
 
-    def highlight(self) -> TUserException:
+    def highlight(self) -> UserExceptionT:
         """
         Returns
         -------
         Exception with human-readable error highlighting for invalid syntax
         """
         if self._is_multi_line:
             invalid_syntax = self._exception_text_lines(border_lines=3)
```

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/script/utils/exceptions.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/script/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/script/utils/name_validation.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/script/utils/name_validation.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/script/utils/type_checking.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/script/utils/type_checking.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from ytdl_sub.script.types.resolvable import LambdaTwo
 from ytdl_sub.script.types.resolvable import NamedCustomFunction
 from ytdl_sub.script.types.resolvable import NamedType
 from ytdl_sub.script.types.resolvable import Resolvable
 from ytdl_sub.script.types.variable import Variable
 from ytdl_sub.script.utils.exceptions import UNREACHABLE
 
-TLambda = TypeVar("TLambda", bound=Lambda)
+LambdaT = TypeVar("LambdaT", bound=Lambda)
 
 
 def is_union(arg_type: Type) -> bool:
     """
     Returns
     -------
     True if typing is Union. False otherwise.
@@ -208,15 +208,15 @@
         if LambdaTwo in (self.args or []):
             return LambdaTwo
         if Lambda in (self.args or []):
             return Lambda
         return None
 
     @property
-    def is_lambda_like(self) -> Optional[Type[TLambda]]:
+    def is_lambda_like(self) -> Optional[Type[LambdaT]]:
         """
         Returns
         -------
         True if the function is a Lambda type (including reduce).
         """
         if l_type := self.is_lambda_reduce_function:
             return l_type
```

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/subscriptions/base_subscription.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/subscriptions/base_subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,21 +70,21 @@
         # Add overrides pre-archive
         self.overrides.add(
             {
                 SubscriptionVariables.subscription_name(): self.name,
             }
         )
 
-        self._enhanced_download_archive: Optional[
-            EnhancedDownloadArchive
-        ] = _initialize_download_archive(
-            output_options=self.output_options,
-            overrides=self.overrides,
-            working_directory=self.working_directory,
-            output_directory=self.output_directory,
+        self._enhanced_download_archive: Optional[EnhancedDownloadArchive] = (
+            _initialize_download_archive(
+                output_options=self.output_options,
+                overrides=self.overrides,
+                working_directory=self.working_directory,
+                output_directory=self.output_directory,
+            )
         )
 
         # Add post-archive variables
         self.overrides.add(
             {
                 SubscriptionVariables.subscription_has_download_archive(): f"""{{
                         %bool({self.download_archive.num_entries > 0})
```

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/subscriptions/subscription.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/subscriptions/subscription.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/subscriptions/subscription_download.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/subscriptions/subscription_download.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,16 +122,16 @@
         os.makedirs(self.working_directory, exist_ok=True)
 
         try:
             yield
         except Exception as exc:
             self._delete_working_directory(is_error=True)
             raise exc
-        else:
-            self._delete_working_directory()
+
+        self._delete_working_directory()
 
     @contextlib.contextmanager
     def _maintain_archive_file(self):
         """
         Context manager to initialize the enhanced download archive
         """
         if self.maintain_download_archive:
```

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/subscriptions/subscription_validators.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/subscriptions/subscription_validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,17 +139,17 @@
             name=name,
             value=value,
             subscription_name=subscription_name,
             config=config,
             presets=presets,
             indent_overrides=indent_overrides,
         )
-        self._overrides_to_add[
-            SubscriptionVariables.subscription_value().variable_name
-        ] = self.value
+        self._overrides_to_add[SubscriptionVariables.subscription_value().variable_name] = (
+            self.value
+        )
 
 
 class SubscriptionListValuesValidator(SubscriptionLeafValidator, StringListValidator):
     def __init__(
         self,
         name,
         value,
@@ -166,17 +166,17 @@
             presets=presets,
             indent_overrides=indent_overrides,
         )
 
         for idx, list_value in enumerate(self.list):
             # Write the first list value into subscription_value as well
             if idx == 0:
-                self._overrides_to_add[
-                    SubscriptionVariables.subscription_value().variable_name
-                ] = list_value.value
+                self._overrides_to_add[SubscriptionVariables.subscription_value().variable_name] = (
+                    list_value.value
+                )
 
             self._overrides_to_add[
                 SubscriptionVariables.subscription_value_i(index=idx).variable_name
             ] = list_value.value
 
 
 class SubscriptionWithOverridesValidator(SubscriptionLeafValidator, DictFormatterValidator):
@@ -215,17 +215,17 @@
             name=name,
             value=value,
             subscription_name=subscription_name,
             config=config,
             presets=presets,
             indent_overrides=indent_overrides,
         )
-        self._overrides_to_add[
-            SubscriptionVariables.subscription_map().variable_name
-        ] = ScriptUtils.to_script(self.dict)
+        self._overrides_to_add[SubscriptionVariables.subscription_map().variable_name] = (
+            ScriptUtils.to_script(self.dict)
+        )
 
 
 class SubscriptionValidator(SubscriptionOutput):
     """
     Top-level subscription validator
     """
```

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/subscriptions/subscription_ytdl_options.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/subscriptions/subscription_ytdl_options.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/thread/log_entries_downloaded_listener.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/thread/log_entries_downloaded_listener.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/utils/chapters.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/utils/chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/utils/datetime.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/utils/exceptions.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/utils/ffmpeg.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/utils/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/utils/file_handler.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/utils/file_handler.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/utils/file_lock.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/utils/file_lock.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/utils/file_path.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/utils/file_path.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/utils/logger.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/utils/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,17 +209,18 @@
                         yield
             finally:
                 redirect_stream.flush()
 
     @classmethod
     def _append_to_error_log(cls):
         # Any time an exception occurs, dump all debug logs into the error log
-        with open(cls.debug_log_filename(), mode="r", encoding="utf-8") as debug_logs, open(
-            cls.error_log_filename(), mode="a", encoding="utf-8"
-        ) as error_logs:
+        with (
+            open(cls.debug_log_filename(), mode="r", encoding="utf-8") as debug_logs,
+            open(cls.error_log_filename(), mode="a", encoding="utf-8") as error_logs,
+        ):
             error_logs.writelines(debug_logs.readlines())
 
     @classmethod
     def log_exception(cls, exception: Exception, log_filepath: Optional[Path] = None):
         """
         Logs an exception based on the exception type. Will transfer all
         debug logs into the error log file. This allows for subscriptions to only write to the
```

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/utils/retry.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/utils/retry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/utils/script.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/utils/script.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/utils/scriptable.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/utils/scriptable.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/utils/thumbnail.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/utils/thumbnail.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/utils/xml.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/utils/xml.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/utils/yaml.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/validators/audo_codec_validator.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/validators/audo_codec_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/validators/file_path_validators.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/validators/file_path_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/validators/nfo_validators.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/validators/nfo_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/validators/regex_validator.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/validators/regex_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/validators/source_variable_validator.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/validators/source_variable_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/validators/strict_dict_validator.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/validators/strict_dict_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/validators/string_datetime.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/validators/string_datetime.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/validators/string_formatter_validators.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/validators/string_formatter_validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,26 +59,22 @@
         """
         Returns
         -------
         The literal format string, unformatted.
         """
         return self._value
 
-    # pylint: disable=no-self-use
-
     def post_process(self, resolved: str) -> str:
         """
         Returns
         -------
         Apply any post processing to the resolved value
         """
         return resolved
 
-    # pylint: enable=no-self-use
-
 
 # pylint: disable=line-too-long
 class OverridesStringFormatterValidator(StringFormatterValidator):
     """
     String that can `only` use :class:`overrides <ytdl_sub.config.preset_options.Overrides>`.
 
     Used in fields that do not touch the downloaded files themselves, but instead, `single`
```

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/validators/string_select_validator.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/validators/string_select_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/validators/validators.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/validators/validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,14 +165,15 @@
 
 
 class ListValidator(Validator, ABC, Generic[ValidatorT]):
     """
     Validates a list of objects to validate
     """
 
+    # pylint: disable=used-before-assignment
     _expected_value_type = list
     _expected_value_type_name = "list"
 
     _inner_list_type: Type[ValidatorT]
 
     def __init__(self, name, value):
         # If the value isn't actually a list, but a single value with the same type as the
```

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py` & `ytdl_sub-2024.5.11/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.3/src/ytdl_sub.egg-info/SOURCES.txt` & `ytdl_sub-2024.5.11/src/ytdl_sub.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 README.md
 pyproject.toml
-setup.cfg
 src/ytdl_sub/__init__.py
 src/ytdl_sub/main.py
 src/ytdl_sub.egg-info/PKG-INFO
 src/ytdl_sub.egg-info/SOURCES.txt
 src/ytdl_sub.egg-info/dependency_links.txt
 src/ytdl_sub.egg-info/entry_points.txt
 src/ytdl_sub.egg-info/requires.txt
```

