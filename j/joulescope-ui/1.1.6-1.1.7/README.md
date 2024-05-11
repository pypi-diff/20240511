# Comparing `tmp/joulescope_ui-1.1.6.tar.gz` & `tmp/joulescope_ui-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joulescope_ui-1.1.6.tar", last modified: Fri Apr 26 13:58:50 2024, max compression
+gzip compressed data, was "joulescope_ui-1.1.7.tar", last modified: Sat May 11 14:14:23 2024, max compression
```

## Comparing `joulescope_ui-1.1.6.tar` & `joulescope_ui-1.1.7.tar`

### file list

```diff
@@ -1,476 +1,475 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.856840 joulescope_ui-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)    53015 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    13659 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/CREDITS.html
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8926 2024-04-26 13:58:50.856840 joulescope_ui-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-26 13:58:49.000000 joulescope_ui-1.1.6/joulescope.iss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.800840 joulescope_ui-1.1.6/joulescope_ui/
--rw-r--r--   0 runner    (1001) docker     (127)    53015 2024-04-26 13:58:35.000000 joulescope_ui-1.1.6/joulescope_ui/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    13659 2024-04-26 13:58:35.000000 joulescope_ui-1.1.6/joulescope_ui/CREDITS.html
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/about.py
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/dev_signal_buffer_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.804840 joulescope_ui-1.1.6/joulescope_ui/devices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/devices/device_update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.804840 joulescope_ui-1.1.6/joulescope_ui/devices/jsdrv/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/devices/jsdrv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/devices/jsdrv/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    24052 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/devices/jsdrv/js110.py
--rw-r--r--   0 runner    (1001) docker     (127)    31966 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/devices/jsdrv/js220.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/devices/jsdrv/js220_fuse.py
--rw-r--r--   0 runner    (1001) docker     (127)    11161 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/devices/jsdrv/js220_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)    17806 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/devices/jsdrv/jsdrv_stream_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/devices/jsdrv/jsdrv_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.804840 joulescope_ui-1.1.6/joulescope_ui/devices/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/devices/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/devices/test/test_device_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/disk_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.804840 joulescope_ui-1.1.6/joulescope_ui/entry_points/
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/entry_points/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/entry_points/zip_inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/error_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    14307 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/error_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/expanding_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    11870 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/file_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/filename_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.780840 joulescope_ui-1.1.6/joulescope_ui/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.804840 joulescope_ui-1.1.6/joulescope_ui/fonts/DSEG14-Modern/
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/fonts/DSEG14-Modern/DSEG-LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.804840 joulescope_ui-1.1.6/joulescope_ui/fonts/Hack/
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/fonts/Hack/LICENSE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.804840 joulescope_ui-1.1.6/joulescope_ui/fonts/Lato/
--rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/fonts/Lato/OFL.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.804840 joulescope_ui-1.1.6/joulescope_ui/fonts/SourceCodePro/
--rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/fonts/SourceCodePro/LICENSE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.804840 joulescope_ui-1.1.6/joulescope_ui/fonts/SourceSerifPro/
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/fonts/SourceSerifPro/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (127)  3102116 2024-04-26 13:58:50.000000 joulescope_ui-1.1.6/joulescope_ui/fonts.rcc
--rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/getting_started.py
--rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/help_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/intel_graphics_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     7379 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/jls_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/jls_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/jls_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6249 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/jls_v2_annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/json_plus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.808840 joulescope_ui-1.1.6/joulescope_ui/locale/
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/locale/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.780840 joulescope_ui-1.1.6/joulescope_ui/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.808840 joulescope_ui-1.1.6/joulescope_ui/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    81477 2024-04-26 13:58:37.000000 joulescope_ui-1.1.6/joulescope_ui/locale/ar/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)   111976 2024-04-26 13:58:37.000000 joulescope_ui-1.1.6/joulescope_ui/locale/ar/LC_MESSAGES/joulescope_ui.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.780840 joulescope_ui-1.1.6/joulescope_ui/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.808840 joulescope_ui-1.1.6/joulescope_ui/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    71341 2024-04-26 13:58:37.000000 joulescope_ui-1.1.6/joulescope_ui/locale/de/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)   102241 2024-04-26 13:58:37.000000 joulescope_ui-1.1.6/joulescope_ui/locale/de/LC_MESSAGES/joulescope_ui.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.780840 joulescope_ui-1.1.6/joulescope_ui/locale/el/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.808840 joulescope_ui-1.1.6/joulescope_ui/locale/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    99006 2024-04-26 13:58:37.000000 joulescope_ui-1.1.6/joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)   129930 2024-04-26 13:58:37.000000 joulescope_ui-1.1.6/joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.780840 joulescope_ui-1.1.6/joulescope_ui/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.808840 joulescope_ui-1.1.6/joulescope_ui/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    71457 2024-04-26 13:58:37.000000 joulescope_ui-1.1.6/joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)   102311 2024-04-26 13:58:37.000000 joulescope_ui-1.1.6/joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.780840 joulescope_ui-1.1.6/joulescope_ui/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.808840 joulescope_ui-1.1.6/joulescope_ui/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    72880 2024-04-26 13:58:37.000000 joulescope_ui-1.1.6/joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)   103793 2024-04-26 13:58:37.000000 joulescope_ui-1.1.6/joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.780840 joulescope_ui-1.1.6/joulescope_ui/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.808840 joulescope_ui-1.1.6/joulescope_ui/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    72116 2024-04-26 13:58:37.000000 joulescope_ui-1.1.6/joulescope_ui/locale/it/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)   103009 2024-04-26 13:58:37.000000 joulescope_ui-1.1.6/joulescope_ui/locale/it/LC_MESSAGES/joulescope_ui.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.780840 joulescope_ui-1.1.6/joulescope_ui/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.808840 joulescope_ui-1.1.6/joulescope_ui/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    75360 2024-04-26 13:58:37.000000 joulescope_ui-1.1.6/joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)   105360 2024-04-26 13:58:37.000000 joulescope_ui-1.1.6/joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.po
--rw-r--r--   0 runner    (1001) docker     (127)    68228 2024-04-26 13:58:36.000000 joulescope_ui-1.1.6/joulescope_ui/locale/joulescope_ui.pot
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.780840 joulescope_ui-1.1.6/joulescope_ui/locale/ko/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.812840 joulescope_ui-1.1.6/joulescope_ui/locale/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    70112 2024-04-26 13:58:37.000000 joulescope_ui-1.1.6/joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)   100201 2024-04-26 13:58:37.000000 joulescope_ui-1.1.6/joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.784839 joulescope_ui-1.1.6/joulescope_ui/locale/zh/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.812840 joulescope_ui-1.1.6/joulescope_ui/locale/zh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    61187 2024-04-26 13:58:37.000000 joulescope_ui-1.1.6/joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)    91067 2024-04-26 13:58:37.000000 joulescope_ui-1.1.6/joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.po
--rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/logging_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    40925 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/mem_leak_debugger.py
--rw-r--r--   0 runner    (1001) docker     (127)     9496 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.812840 joulescope_ui-1.1.6/joulescope_ui/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9050 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/plugins/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6025 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/plugins/selector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.812840 joulescope_ui-1.1.6/joulescope_ui/plugins/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/plugins/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.812840 joulescope_ui-1.1.6/joulescope_ui/plugins/test/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/plugins/test/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.812840 joulescope_ui-1.1.6/joulescope_ui/plugins/test/plugins/p1/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/plugins/test/plugins/p1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/plugins/test/plugins/p1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/plugins/test/plugins/p1/index.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.812840 joulescope_ui-1.1.6/joulescope_ui/plugins/test/plugins/p2/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/plugins/test/plugins/p2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/plugins/test/plugins/p2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/plugins/test/plugins/p2/index.json
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/plugins/test/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/process_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    66439 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/pubsub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/pubsub_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/pubsub_callable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/pubsub_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13019 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/range_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.816840 joulescope_ui-1.1.6/joulescope_ui/range_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/range_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/range_tools/cdf.py
--rw-r--r--   0 runner    (1001) docker     (127)    10544 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/range_tools/frequency.py
--rw-r--r--   0 runner    (1001) docker     (127)     8854 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/range_tools/histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/range_tools/max_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/range_tools/plugin_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/range_tools/usb_inrush.py
--rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.816840 joulescope_ui-1.1.6/joulescope_ui/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    23260 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/resources/dmg_background.png
--rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/resources/dmg_background.svg
--rw-r--r--   0 runner    (1001) docker     (127)    48138 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/resources/dmg_background@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)   100365 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/resources/icon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.816840 joulescope_ui-1.1.6/joulescope_ui/resources/icon.iconset/
--rwxr-xr-x   0 runner    (1001) docker     (127)      968 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/resources/icon.iconset/icon_128x128.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     1510 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/resources/icon.iconset/icon_128x128@2.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/resources/icon.iconset/icon_16x16.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      550 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/resources/icon.iconset/icon_16x16@2.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     1510 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/resources/icon.iconset/icon_256x256.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     2980 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/resources/icon.iconset/icon_256x256@2.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      550 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/resources/icon.iconset/icon_32x32.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      718 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/resources/icon.iconset/icon_32x32@2.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     2980 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/resources/icon.iconset/icon_512x512.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     7537 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/resources/icon.iconset/icon_512x512@2.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      718 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/resources/icon.iconset/icon_64x64.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      968 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/resources/icon.iconset/icon_64x64@2.png
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/resources/icons.svg
--rw-r--r--   0 runner    (1001) docker     (127)    16987 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/resources/logo-large.png
--rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/resources/logo-small.png
--rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/resources/zoom.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)    22815 2024-04-26 13:58:49.000000 joulescope_ui-1.1.6/joulescope_ui/resources.rcc
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/safe_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/sanitize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/shift_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (127)    12231 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/software_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/source_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.820840 joulescope_ui-1.1.6/joulescope_ui/styles/
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/color_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/color_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6914 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/color_picker.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/color_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/font_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/font_scheme_js1.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/fonts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.824840 joulescope_ui-1.1.6/joulescope_ui/styles/js1/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/js1/arrow_down.svg
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/js1/arrow_left.svg
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/js1/arrow_right.svg
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/js1/arrow_up.svg
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/js1/branch_closed.svg
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/js1/branch_end.svg
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/js1/branch_end_open.svg
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/js1/branch_more.svg
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/js1/branch_open.svg
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/js1/branch_vline.svg
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/js1/checkbox_checked.svg
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/js1/checkbox_indeterminate.svg
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/js1/checkbox_unchecked.svg
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/js1/close.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/js1/detach.svg
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/js1/hmovetoolbar.svg
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/js1/hsepartoolbar.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/js1/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/js1/radio_checked.svg
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/js1/radio_unchecked.svg
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/js1/sizegrip.svg
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/js1/style.html
--rw-r--r--   0 runner    (1001) docker     (127)    19555 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/js1/style.qss
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/js1/tabs_menu.svg
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/js1/transparent.svg
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/js1/vmovetoolbar.svg
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/js1/vsepartoolbars.svg
--rw-r--r--   0 runner    (1001) docker     (127)    15186 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/parameter_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.824840 joulescope_ui-1.1.6/joulescope_ui/styles/system/
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/system/index.json
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/system/style.html
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/system/style.qss
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/system/zoom_all.svg
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/system/zoom_in.svg
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/system/zoom_out.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.824840 joulescope_ui-1.1.6/joulescope_ui/styles/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/test/test_color_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/test/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/styles/test/test_parameter_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.828840 joulescope_ui-1.1.6/joulescope_ui/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/test/anno1.anno.jls
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/test/test_annotation_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/test/test_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/test/test_disk_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/test/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/test/test_pubsub.py
--rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/test/test_pubsub_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)    16874 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/test/test_pubsub_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/test/test_range_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/test/test_reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/test/test_sanitize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/test/test_software_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     6608 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/test/test_source_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/test/test_time_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/test/test_tooltip.py
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/test/test_units.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/test/test_versioned_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/time_map.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-26 13:58:37.000000 joulescope_ui-1.1.6/joulescope_ui/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/tooltip.py
--rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/ui_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/units.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/versioned_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    13938 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/view.py
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widget_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.828840 joulescope_ui-1.1.6/joulescope_ui/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.828840 joulescope_ui-1.1.6/joulescope_ui/widgets/accumulator/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/accumulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/accumulator/accumulator_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.828840 joulescope_ui-1.1.6/joulescope_ui/widgets/accumulator/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/accumulator/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/accumulator/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/accumulator/styles/font_scheme_js1.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/accumulator/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/accumulator/styles/style.qss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.828840 joulescope_ui-1.1.6/joulescope_ui/widgets/clock/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/clock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/clock/clock_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.832840 joulescope_ui-1.1.6/joulescope_ui/widgets/developer/
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/developer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/developer/log_view_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/developer/profile_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/developer/publish_spy_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/developer/pubsub_explorer_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.832840 joulescope_ui-1.1.6/joulescope_ui/widgets/device_control/
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/device_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/device_control/current_limits.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/device_control/device_control_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/device_control/device_info_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    11286 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/device_control/device_update_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/device_control/fuse.py
--rw-r--r--   0 runner    (1001) docker     (127)    24811 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/device_control/js220_ctrl_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.836840 joulescope_ui-1.1.6/joulescope_ui/widgets/device_control/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/device_control/styles/active_checked.svg
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/device_control/styles/active_unchecked.svg
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/device_control/styles/closed.svg
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/device_control/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/device_control/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/device_control/styles/device_close.svg
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/device_control/styles/device_open.svg
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/device_control/styles/doc.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/device_control/styles/fuse_engaged.svg
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/device_control/styles/fuse_normal.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/device_control/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/device_control/styles/info.svg
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/device_control/styles/open.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/device_control/styles/style.qss
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/device_control/styles/target_power.svg
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/device_control/styles/target_power_off.svg
--rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/double_slider.py
--rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/draggable_list_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.836840 joulescope_ui-1.1.6/joulescope_ui/widgets/example/
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/example/example_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.836840 joulescope_ui-1.1.6/joulescope_ui/widgets/example/styles/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/example/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/example/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/example/styles/font_scheme_js1.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/example/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/example/styles/style.qss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.836840 joulescope_ui-1.1.6/joulescope_ui/widgets/flyout/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/flyout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/flyout/flyout_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.836840 joulescope_ui-1.1.6/joulescope_ui/widgets/flyout/styles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/flyout/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/flyout/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/flyout/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/flyout/styles/style.qss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.836840 joulescope_ui-1.1.6/joulescope_ui/widgets/hamburger/
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/hamburger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/hamburger/hamburger_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.836840 joulescope_ui-1.1.6/joulescope_ui/widgets/help/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/help/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/help/help_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.836840 joulescope_ui-1.1.6/joulescope_ui/widgets/jls_info/
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/jls_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/jls_info/jls_info_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.840840 joulescope_ui-1.1.6/joulescope_ui/widgets/js220_cal/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/js220_cal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22114 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/js220_cal/current_offset.png
--rw-r--r--   0 runner    (1001) docker     (127)    19681 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/js220_cal/js220_cal_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    27849 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/js220_cal/voltage_offset.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.840840 joulescope_ui-1.1.6/joulescope_ui/widgets/memory/
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11866 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/memory/memory_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.840840 joulescope_ui-1.1.6/joulescope_ui/widgets/memory/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/memory/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/memory/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/memory/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/memory/styles/style.qss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.840840 joulescope_ui-1.1.6/joulescope_ui/widgets/notes/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/notes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/notes/notes_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.840840 joulescope_ui-1.1.6/joulescope_ui/widgets/progress_bar/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/progress_bar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/progress_bar/progress_bar_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.840840 joulescope_ui-1.1.6/joulescope_ui/widgets/record_status/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/record_status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/record_status/record_status_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.840840 joulescope_ui-1.1.6/joulescope_ui/widgets/record_status/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/record_status/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/record_status/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/record_status/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/record_status/styles/record.svg
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/record_status/styles/style.qss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.840840 joulescope_ui-1.1.6/joulescope_ui/widgets/report_issue/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/report_issue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/report_issue/report_issue_dialog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.840840 joulescope_ui-1.1.6/joulescope_ui/widgets/settings/
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24258 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/settings/settings_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/settings/unique_strings_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.844840 joulescope_ui-1.1.6/joulescope_ui/widgets/sidebar/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/sidebar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10173 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/sidebar/sidebar_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.844840 joulescope_ui-1.1.6/joulescope_ui/widgets/sidebar/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/sidebar/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/sidebar/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/sidebar/styles/device.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/sidebar/styles/fuse_engaged.svg
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/sidebar/styles/fuse_normal.svg
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/sidebar/styles/help.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/sidebar/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/sidebar/styles/memory.svg
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/sidebar/styles/misc.svg
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/sidebar/styles/pause.svg
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/sidebar/styles/play.svg
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/sidebar/styles/record.svg
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/sidebar/styles/settings.svg
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/sidebar/styles/stop.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/sidebar/styles/style.qss
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/sidebar/styles/target_power.svg
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/sidebar/styles/target_power_off.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.844840 joulescope_ui-1.1.6/joulescope_ui/widgets/signal_record/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/signal_record/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/signal_record/disk_full_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     9370 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/signal_record/signal_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    13791 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/signal_record/signal_record_config_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.844840 joulescope_ui-1.1.6/joulescope_ui/widgets/statistics_record/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/statistics_record/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/statistics_record/statistics_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     9701 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/statistics_record/statistics_record_config_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/switch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.844840 joulescope_ui-1.1.6/joulescope_ui/widgets/trigger/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/trigger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/trigger/condition_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.848840 joulescope_ui-1.1.6/joulescope_ui/widgets/trigger/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/trigger/styles/active.svg
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/trigger/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/trigger/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/trigger/styles/continuous.svg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/trigger/styles/font_scheme_js1.txt
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/trigger/styles/inactive.svg
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/trigger/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/trigger/styles/searching.svg
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/trigger/styles/single.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/trigger/styles/style.qss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.848840 joulescope_ui-1.1.6/joulescope_ui/widgets/trigger/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/trigger/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/trigger/test/test_const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/trigger/test/test_duration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/trigger/test/test_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)    48890 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/trigger/trigger_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.848840 joulescope_ui-1.1.6/joulescope_ui/widgets/value/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/value/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.848840 joulescope_ui-1.1.6/joulescope_ui/widgets/value/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/value/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/value/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/value/styles/font_scheme_js1.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/value/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/value/styles/style.qss
--rw-r--r--   0 runner    (1001) docker     (127)    26634 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/value/value_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.848840 joulescope_ui-1.1.6/joulescope_ui/widgets/view_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/view_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.848840 joulescope_ui-1.1.6/joulescope_ui/widgets/view_manager/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/view_manager/styles/add.svg
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/view_manager/styles/delete.svg
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/view_manager/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/view_manager/styles/move.svg
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/view_manager/styles/reset.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/view_manager/styles/style.qss
--rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/view_manager/view_manager_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.852840 joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/annotations.md
--rw-r--r--   0 runner    (1001) docker     (127)     9848 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/axis_ticks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/interval_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/line_segments.py
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/quantities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.852840 joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/styles/
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/styles/font_scheme_js1.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/styles/marker_add1.svg
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/styles/marker_add2.svg
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/styles/marker_clear.svg
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/styles/pin_left.svg
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/styles/pin_right.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/styles/style.qss
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/styles/style_defines.txt
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/styles/trace.svg
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/styles/y_zoom_all.svg
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/styles/zoom_all.svg
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/styles/zoom_in.svg
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/styles/zoom_out.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.852840 joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/test/test_axis_ticks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/test/test_quantities.py
--rw-r--r--   0 runner    (1001) docker     (127)     8430 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/text_annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12540 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/waveform_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/waveform_source_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)   169437 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/waveform_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/y_range_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/joulescope_ui/zip_inspector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:58:50.852840 joulescope_ui-1.1.6/joulescope_ui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8926 2024-04-26 13:58:50.000000 joulescope_ui-1.1.6/joulescope_ui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17235 2024-04-26 13:58:50.000000 joulescope_ui-1.1.6/joulescope_ui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 13:58:50.000000 joulescope_ui-1.1.6/joulescope_ui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-26 13:58:50.000000 joulescope_ui-1.1.6/joulescope_ui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-26 13:58:50.000000 joulescope_ui-1.1.6/joulescope_ui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-26 13:58:50.000000 joulescope_ui-1.1.6/joulescope_ui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-26 13:58:50.856840 joulescope_ui-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8049 2024-04-26 13:58:13.000000 joulescope_ui-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.450034 joulescope_ui-1.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    53673 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13659 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/CREDITS.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8926 2024-05-11 14:14:23.450034 joulescope_ui-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-05-11 14:14:21.000000 joulescope_ui-1.1.7/joulescope.iss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.390035 joulescope_ui-1.1.7/joulescope_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)    53673 2024-05-11 14:14:11.000000 joulescope_ui-1.1.7/joulescope_ui/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13659 2024-05-11 14:14:11.000000 joulescope_ui-1.1.7/joulescope_ui/CREDITS.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/about.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/dev_signal_buffer_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.394035 joulescope_ui-1.1.7/joulescope_ui/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/devices/device_update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.394035 joulescope_ui-1.1.7/joulescope_ui/devices/jsdrv/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/devices/jsdrv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/devices/jsdrv/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24052 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/devices/jsdrv/js110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31966 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/devices/jsdrv/js220.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/devices/jsdrv/js220_fuse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11161 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/devices/jsdrv/js220_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17812 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/devices/jsdrv/jsdrv_stream_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/devices/jsdrv/jsdrv_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.394035 joulescope_ui-1.1.7/joulescope_ui/devices/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/devices/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/devices/test/test_device_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/disk_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.394035 joulescope_ui-1.1.7/joulescope_ui/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/entry_points/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/entry_points/zip_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/error_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14307 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/error_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/expanding_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11870 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/file_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/filename_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.370035 joulescope_ui-1.1.7/joulescope_ui/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.394035 joulescope_ui-1.1.7/joulescope_ui/fonts/DSEG14-Modern/
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/fonts/DSEG14-Modern/DSEG-LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.394035 joulescope_ui-1.1.7/joulescope_ui/fonts/Hack/
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/fonts/Hack/LICENSE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.394035 joulescope_ui-1.1.7/joulescope_ui/fonts/Lato/
+-rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/fonts/Lato/OFL.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.394035 joulescope_ui-1.1.7/joulescope_ui/fonts/SourceCodePro/
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/fonts/SourceCodePro/LICENSE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.394035 joulescope_ui-1.1.7/joulescope_ui/fonts/SourceSerifPro/
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/fonts/SourceSerifPro/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  3102116 2024-05-11 14:14:23.000000 joulescope_ui-1.1.7/joulescope_ui/fonts.rcc
+-rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/getting_started.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/help_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/intel_graphics_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7379 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/jls_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/jls_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/jls_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6249 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/jls_v2_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/json_plus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.398035 joulescope_ui-1.1.7/joulescope_ui/locale/
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/locale/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.370035 joulescope_ui-1.1.7/joulescope_ui/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.398035 joulescope_ui-1.1.7/joulescope_ui/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    81702 2024-05-11 14:14:13.000000 joulescope_ui-1.1.7/joulescope_ui/locale/ar/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   112244 2024-05-11 14:14:13.000000 joulescope_ui-1.1.7/joulescope_ui/locale/ar/LC_MESSAGES/joulescope_ui.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.370035 joulescope_ui-1.1.7/joulescope_ui/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.398035 joulescope_ui-1.1.7/joulescope_ui/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    71550 2024-05-11 14:14:13.000000 joulescope_ui-1.1.7/joulescope_ui/locale/de/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   102499 2024-05-11 14:14:13.000000 joulescope_ui-1.1.7/joulescope_ui/locale/de/LC_MESSAGES/joulescope_ui.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.370035 joulescope_ui-1.1.7/joulescope_ui/locale/el/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.398035 joulescope_ui-1.1.7/joulescope_ui/locale/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    99351 2024-05-11 14:14:13.000000 joulescope_ui-1.1.7/joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   130324 2024-05-11 14:14:13.000000 joulescope_ui-1.1.7/joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.370035 joulescope_ui-1.1.7/joulescope_ui/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.398035 joulescope_ui-1.1.7/joulescope_ui/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    71667 2024-05-11 14:14:13.000000 joulescope_ui-1.1.7/joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   102570 2024-05-11 14:14:13.000000 joulescope_ui-1.1.7/joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.370035 joulescope_ui-1.1.7/joulescope_ui/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.398035 joulescope_ui-1.1.7/joulescope_ui/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    73100 2024-05-11 14:14:13.000000 joulescope_ui-1.1.7/joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   104062 2024-05-11 14:14:13.000000 joulescope_ui-1.1.7/joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.370035 joulescope_ui-1.1.7/joulescope_ui/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.398035 joulescope_ui-1.1.7/joulescope_ui/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    72339 2024-05-11 14:14:13.000000 joulescope_ui-1.1.7/joulescope_ui/locale/it/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   103281 2024-05-11 14:14:13.000000 joulescope_ui-1.1.7/joulescope_ui/locale/it/LC_MESSAGES/joulescope_ui.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.370035 joulescope_ui-1.1.7/joulescope_ui/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.398035 joulescope_ui-1.1.7/joulescope_ui/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    75547 2024-05-11 14:14:13.000000 joulescope_ui-1.1.7/joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   105590 2024-05-11 14:14:13.000000 joulescope_ui-1.1.7/joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.po
+-rw-r--r--   0 runner    (1001) docker     (127)    68383 2024-05-11 14:14:12.000000 joulescope_ui-1.1.7/joulescope_ui/locale/joulescope_ui.pot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.370035 joulescope_ui-1.1.7/joulescope_ui/locale/ko/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.402035 joulescope_ui-1.1.7/joulescope_ui/locale/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    70320 2024-05-11 14:14:13.000000 joulescope_ui-1.1.7/joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   100452 2024-05-11 14:14:13.000000 joulescope_ui-1.1.7/joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.370035 joulescope_ui-1.1.7/joulescope_ui/locale/zh/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.402035 joulescope_ui-1.1.7/joulescope_ui/locale/zh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    61353 2024-05-11 14:14:13.000000 joulescope_ui-1.1.7/joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    91276 2024-05-11 14:14:13.000000 joulescope_ui-1.1.7/joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.po
+-rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/logging_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42189 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/mem_leak_debugger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9496 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.402035 joulescope_ui-1.1.7/joulescope_ui/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9050 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/plugins/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6025 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/plugins/selector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.402035 joulescope_ui-1.1.7/joulescope_ui/plugins/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/plugins/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.402035 joulescope_ui-1.1.7/joulescope_ui/plugins/test/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/plugins/test/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.402035 joulescope_ui-1.1.7/joulescope_ui/plugins/test/plugins/p1/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/plugins/test/plugins/p1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/plugins/test/plugins/p1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/plugins/test/plugins/p1/index.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.402035 joulescope_ui-1.1.7/joulescope_ui/plugins/test/plugins/p2/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/plugins/test/plugins/p2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/plugins/test/plugins/p2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/plugins/test/plugins/p2/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/plugins/test/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/process_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66497 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/pubsub_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/pubsub_callable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/pubsub_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13019 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/range_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.406035 joulescope_ui-1.1.7/joulescope_ui/range_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/range_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/range_tools/cdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10544 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/range_tools/frequency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8854 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/range_tools/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/range_tools/max_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/range_tools/plugin_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/range_tools/usb_inrush.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.406035 joulescope_ui-1.1.7/joulescope_ui/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    23260 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources/dmg_background.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources/dmg_background.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    48138 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources/dmg_background@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)   100365 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources/icon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.406035 joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      968 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_128x128.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1510 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_128x128@2.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_16x16.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      550 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_16x16@2.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1510 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_256x256.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2980 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_256x256@2.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      550 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_32x32.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      718 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_32x32@2.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2980 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_512x512.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7537 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_512x512@2.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      718 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_64x64.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      968 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_64x64@2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources/icons.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    16987 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources/logo-large.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources/logo-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources/zoom.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22815 2024-05-11 14:14:21.000000 joulescope_ui-1.1.7/joulescope_ui/resources.rcc
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/safe_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/sanitize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/shift_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12231 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/software_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/source_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.410035 joulescope_ui-1.1.7/joulescope_ui/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/color_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/color_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6914 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/color_picker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/color_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/font_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/font_scheme_js1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/fonts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.414034 joulescope_ui-1.1.7/joulescope_ui/styles/js1/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/arrow_down.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/arrow_left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/arrow_right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/arrow_up.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/branch_closed.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/branch_end.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/branch_end_open.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/branch_more.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/branch_open.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/branch_vline.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/checkbox_checked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/checkbox_indeterminate.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/checkbox_unchecked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/close.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/detach.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/hmovetoolbar.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/hsepartoolbar.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/radio_checked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/radio_unchecked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/sizegrip.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/style.html
+-rw-r--r--   0 runner    (1001) docker     (127)    19555 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/style.qss
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/tabs_menu.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/transparent.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/vmovetoolbar.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/js1/vsepartoolbars.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    15186 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/parameter_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.414034 joulescope_ui-1.1.7/joulescope_ui/styles/system/
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/system/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/system/style.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/system/style.qss
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/system/zoom_all.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/system/zoom_in.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/system/zoom_out.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.418035 joulescope_ui-1.1.7/joulescope_ui/styles/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/test/test_color_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/test/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/styles/test/test_parameter_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.418035 joulescope_ui-1.1.7/joulescope_ui/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/test/anno1.anno.jls
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/test/test_annotation_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/test/test_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/test/test_disk_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/test/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/test/test_pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/test/test_pubsub_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16874 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/test/test_pubsub_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/test/test_range_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/test/test_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/test/test_sanitize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/test/test_software_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6608 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/test/test_source_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/test/test_time_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/test/test_tooltip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/test/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/test/test_versioned_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/time_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-11 14:14:13.000000 joulescope_ui-1.1.7/joulescope_ui/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/tooltip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/ui_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/versioned_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14173 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widget_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.418035 joulescope_ui-1.1.7/joulescope_ui/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.422035 joulescope_ui-1.1.7/joulescope_ui/widgets/accumulator/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/accumulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/accumulator/accumulator_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.422035 joulescope_ui-1.1.7/joulescope_ui/widgets/accumulator/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/accumulator/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/accumulator/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/accumulator/styles/font_scheme_js1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/accumulator/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/accumulator/styles/style.qss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.422035 joulescope_ui-1.1.7/joulescope_ui/widgets/clock/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/clock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/clock/clock_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.422035 joulescope_ui-1.1.7/joulescope_ui/widgets/developer/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/developer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/developer/log_view_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/developer/profile_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/developer/publish_spy_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/developer/pubsub_explorer_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.422035 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/current_limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/device_control_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/device_info_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11286 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/device_update_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/fuse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24811 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/js220_ctrl_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.426035 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/active_checked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/active_unchecked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/closed.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/device_close.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/device_open.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/doc.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/fuse_engaged.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/fuse_normal.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/info.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/open.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/style.qss
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/target_power.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/target_power_off.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/double_slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/draggable_list_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.426035 joulescope_ui-1.1.7/joulescope_ui/widgets/example/
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/example/example_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.426035 joulescope_ui-1.1.7/joulescope_ui/widgets/example/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/example/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/example/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/example/styles/font_scheme_js1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/example/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/example/styles/style.qss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.426035 joulescope_ui-1.1.7/joulescope_ui/widgets/flyout/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/flyout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/flyout/flyout_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.430034 joulescope_ui-1.1.7/joulescope_ui/widgets/flyout/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/flyout/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/flyout/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/flyout/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/flyout/styles/style.qss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.430034 joulescope_ui-1.1.7/joulescope_ui/widgets/hamburger/
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/hamburger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/hamburger/hamburger_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.430034 joulescope_ui-1.1.7/joulescope_ui/widgets/help/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/help/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/help/help_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.430034 joulescope_ui-1.1.7/joulescope_ui/widgets/jls_info/
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/jls_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/jls_info/jls_info_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.430034 joulescope_ui-1.1.7/joulescope_ui/widgets/js220_cal/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/js220_cal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22114 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/js220_cal/current_offset.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19681 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/js220_cal/js220_cal_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27849 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/js220_cal/voltage_offset.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.430034 joulescope_ui-1.1.7/joulescope_ui/widgets/memory/
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11866 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/memory/memory_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.430034 joulescope_ui-1.1.7/joulescope_ui/widgets/memory/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/memory/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/memory/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/memory/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/memory/styles/style.qss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.430034 joulescope_ui-1.1.7/joulescope_ui/widgets/notes/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/notes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/notes/notes_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.430034 joulescope_ui-1.1.7/joulescope_ui/widgets/progress_bar/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/progress_bar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/progress_bar/progress_bar_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.430034 joulescope_ui-1.1.7/joulescope_ui/widgets/record_status/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/record_status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/record_status/record_status_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.430034 joulescope_ui-1.1.7/joulescope_ui/widgets/record_status/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/record_status/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/record_status/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/record_status/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/record_status/styles/record.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/record_status/styles/style.qss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.434034 joulescope_ui-1.1.7/joulescope_ui/widgets/report_issue/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/report_issue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/report_issue/report_issue_dialog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.434034 joulescope_ui-1.1.7/joulescope_ui/widgets/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24143 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/settings/settings_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/settings/unique_strings_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.434034 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10815 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/sidebar_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.434034 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/device.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/fuse_engaged.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/fuse_normal.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/help.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/memory.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/misc.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/pause.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/play.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/record.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/settings.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/stop.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/style.qss
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/target_power.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/target_power_off.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.434034 joulescope_ui-1.1.7/joulescope_ui/widgets/signal_record/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/signal_record/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/signal_record/disk_full_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9370 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/signal_record/signal_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13791 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/signal_record/signal_record_config_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.434034 joulescope_ui-1.1.7/joulescope_ui/widgets/statistics_record/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/statistics_record/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/statistics_record/statistics_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9701 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/statistics_record/statistics_record_config_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/switch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.438034 joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/condition_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.438034 joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/styles/active.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/styles/continuous.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/styles/font_scheme_js1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/styles/inactive.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/styles/searching.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/styles/single.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/styles/style.qss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.438034 joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/test/test_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/test/test_duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/test/test_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48890 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/trigger_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.438034 joulescope_ui-1.1.7/joulescope_ui/widgets/value/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/value/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.438034 joulescope_ui-1.1.7/joulescope_ui/widgets/value/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/value/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/value/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/value/styles/font_scheme_js1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/value/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/value/styles/style.qss
+-rw-r--r--   0 runner    (1001) docker     (127)    27149 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/value/value_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.438034 joulescope_ui-1.1.7/joulescope_ui/widgets/view_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/view_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.442034 joulescope_ui-1.1.7/joulescope_ui/widgets/view_manager/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/view_manager/styles/add.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/view_manager/styles/delete.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/view_manager/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/view_manager/styles/move.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/view_manager/styles/reset.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/view_manager/styles/style.qss
+-rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/view_manager/view_manager_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.442034 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/annotations.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9848 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/axis_ticks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/interval_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/line_segments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/quantities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.446034 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/font_scheme_js1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/marker_add1.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/marker_add2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/marker_clear.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/pin_left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/pin_right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/style.qss
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/style_defines.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/trace.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/y_zoom_all.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/zoom_all.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/zoom_in.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/zoom_out.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.446034 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/test/test_axis_ticks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/test/test_quantities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8430 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/text_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12540 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/waveform_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/waveform_source_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)   173533 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/waveform_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/y_range_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/joulescope_ui/zip_inspector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:14:23.446034 joulescope_ui-1.1.7/joulescope_ui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8926 2024-05-11 14:14:23.000000 joulescope_ui-1.1.7/joulescope_ui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17208 2024-05-11 14:14:23.000000 joulescope_ui-1.1.7/joulescope_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 14:14:23.000000 joulescope_ui-1.1.7/joulescope_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-11 14:14:23.000000 joulescope_ui-1.1.7/joulescope_ui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-11 14:14:23.000000 joulescope_ui-1.1.7/joulescope_ui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-11 14:14:23.000000 joulescope_ui-1.1.7/joulescope_ui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-11 14:14:23.450034 joulescope_ui-1.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8049 2024-05-11 14:13:48.000000 joulescope_ui-1.1.7/setup.py
```

### Comparing `joulescope_ui-1.1.6/CHANGELOG.md` & `joulescope_ui-1.1.7/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,31 @@
 
 # CHANGELOG
 
 This file contains the list of changes made to pyjoulescope_ui.
 
 ---
 
+## 1.1.7
+
+2024 May 11
+
+* Added arbitrary divisor with optional units to Value widget  #265
+* Added Flyout widget click & drag right to resize   #267
+* Deferred data directory creation  #266
+* Updated pyjls from 0.9.2 to 0.9.4 to fix unicode path handling.
+* Fixed crash on JLS file not found  #264
+* Changed to async publish for stream buffer to prevent timeouts  #269
+* Added Waveform widget keyboard shortcuts  #268
+* Improved global keyboard shortcuts to work from all windows.
+* Changed Waveform widget keyboard shortcuts to be local.
+  Fixes broken shortcuts with two Waveform widgets. Click on widget to select.
+* Improved Waveform widget undo/redo.
+
+
 ## 1.1.6
 
 2024 Apr 26
 
 * Added plugin framework with live code reload  #14
 * Restructured code to support human language translation.
 * Added AI translations: ar, de, el, es, fr, it, ja, ko, zh.
```

### Comparing `joulescope_ui-1.1.6/CREDITS.html` & `joulescope_ui-1.1.7/CREDITS.html`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/LICENSE.txt` & `joulescope_ui-1.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/PKG-INFO` & `joulescope_ui-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joulescope_ui
-Version: 1.1.6
+Version: 1.1.7
 Summary: Joulescope™ graphical user interface
 Home-page: https://www.joulescope.com
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/pyjoulescope_ui/issues
 Project-URL: Funding, https://www.joulescope.com
@@ -34,15 +34,15 @@
 License-File: LICENSE.txt
 Requires-Dist: appnope>=0.1.2
 Requires-Dist: fs
 Requires-Dist: pyjoulescope_driver<2.0.0,>=1.5.1
 Requires-Dist: joulescope<2.0.0,>=1.1.12
 Requires-Dist: markdown
 Requires-Dist: psutil
-Requires-Dist: pyjls>=0.9.2
+Requires-Dist: pyjls>=0.9.4
 Requires-Dist: pyopengl
 Requires-Dist: pywin32>=223; platform_system == "Windows"
 Requires-Dist: pyqtgraph>=0.13.3
 Requires-Dist: PySide6<7.0.0,>=6.7.0
 Requires-Dist: PySide6-QtAds<5.0.0,>=4.2.1.1
 Requires-Dist: python-dateutil>=2.7.3
 Requires-Dist: QtPy
```

### Comparing `joulescope_ui-1.1.6/README.md` & `joulescope_ui-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope.iss` & `joulescope_ui-1.1.7/joulescope.iss`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ; Script generated by the Inno Setup Script Wizard.
 ; SEE THE DOCUMENTATION FOR DETAILS ON CREATING INNO SETUP SCRIPT FILES!
 
 #define MyAppName "Joulescope"
-#define MyAppVersion "1.1.6"
-#define MyAppVersionUnderscores "1_1_6"
+#define MyAppVersion "1.1.7"
+#define MyAppVersionUnderscores "1_1_7"
 #define MyAppPublisher "Jetperch LLC"
 #define MyAppURL "https://www.joulescope.com"
 #define MyAppExeName "joulescope.exe"
 
 [Setup]
 ; NOTE: The value of AppId uniquely identifies this application.
 ; Do not use the same AppId value in installers for other applications.
```

### Comparing `joulescope_ui-1.1.6/joulescope_ui/CHANGELOG.md` & `joulescope_ui-1.1.7/joulescope_ui/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,31 @@
 
 # CHANGELOG
 
 This file contains the list of changes made to pyjoulescope_ui.
 
 ---
 
+## 1.1.7
+
+2024 May 11
+
+* Added arbitrary divisor with optional units to Value widget  #265
+* Added Flyout widget click & drag right to resize   #267
+* Deferred data directory creation  #266
+* Updated pyjls from 0.9.2 to 0.9.4 to fix unicode path handling.
+* Fixed crash on JLS file not found  #264
+* Changed to async publish for stream buffer to prevent timeouts  #269
+* Added Waveform widget keyboard shortcuts  #268
+* Improved global keyboard shortcuts to work from all windows.
+* Changed Waveform widget keyboard shortcuts to be local.
+  Fixes broken shortcuts with two Waveform widgets. Click on widget to select.
+* Improved Waveform widget undo/redo.
+
+
 ## 1.1.6
 
 2024 Apr 26
 
 * Added plugin framework with live code reload  #14
 * Restructured code to support human language translation.
 * Added AI translations: ar, de, el, es, fr, it, ja, ko, zh.
```

### Comparing `joulescope_ui-1.1.6/joulescope_ui/CREDITS.html` & `joulescope_ui-1.1.7/joulescope_ui/CREDITS.html`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/__init__.py` & `joulescope_ui-1.1.7/joulescope_ui/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/__main__.py` & `joulescope_ui-1.1.7/joulescope_ui/__main__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/about.py` & `joulescope_ui-1.1.7/joulescope_ui/about.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/api.py` & `joulescope_ui-1.1.7/joulescope_ui/api.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/app.py` & `joulescope_ui-1.1.7/joulescope_ui/app.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/capabilities.py` & `joulescope_ui-1.1.7/joulescope_ui/capabilities.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/dev_signal_buffer_source.py` & `joulescope_ui-1.1.7/joulescope_ui/dev_signal_buffer_source.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/devices/device_update.py` & `joulescope_ui-1.1.7/joulescope_ui/devices/device_update.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/devices/jsdrv/device.py` & `joulescope_ui-1.1.7/joulescope_ui/devices/jsdrv/device.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/devices/jsdrv/js110.py` & `joulescope_ui-1.1.7/joulescope_ui/devices/jsdrv/js110.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/devices/jsdrv/js220.py` & `joulescope_ui-1.1.7/joulescope_ui/devices/jsdrv/js220.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/devices/jsdrv/js220_fuse.py` & `joulescope_ui-1.1.7/joulescope_ui/devices/jsdrv/js220_fuse.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/devices/jsdrv/js220_updater.py` & `joulescope_ui-1.1.7/joulescope_ui/devices/jsdrv/js220_updater.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/devices/jsdrv/jsdrv_stream_buffer.py` & `joulescope_ui-1.1.7/joulescope_ui/devices/jsdrv/jsdrv_stream_buffer.py`

 * *Files 1% similar despite different names*

```diff
@@ -361,24 +361,24 @@
             self.pubsub.topic_add(f'{ui_signal_prefix}/{key}', meta, exists_ok=True)
         self.pubsub.publish(f'{ui_signal_prefix}/name', signal_name)
         self.pubsub.publish(f'{ui_signal_prefix}/meta', signal_meta)
         self._driver_publish(f'm/{self._id}/a/!add', buf_id)
         subtopic = device.signal_subtopics(signal, 'data')
         device_source = f'{device_path}/{subtopic}'
         buf_prefix = f'm/{self._id}/s/{buf_id:03d}'
-        self._driver_publish(f'{buf_prefix}/topic', device_source)
+        self._driver_publish(f'{buf_prefix}/topic', device_source, 0)
         self._device_subscribe(f'{buf_prefix}/info', ['pub', 'pub_retain'], self._on_device_signal_info)
         self.pubsub.publish(f'{ui_prefix}/events/signals/!add', signal_id)
 
     def on_action_remove(self, signal_id):
         self._log.info('remove %s', signal_id)
         buf_id = self._signals.pop(signal_id)[0]
         self._signals_reverse.pop(buf_id)
         self._signals_free.append(buf_id)
-        self._driver_publish(f'm/{self._id}/a/!remove', buf_id)
+        self._driver_publish(f'm/{self._id}/a/!remove', buf_id, 0)
         ui_prefix = get_topic_name(self)
         self.pubsub.publish(f'{ui_prefix}/events/signals/!remove', signal_id)
         self.pubsub.topic_remove(f'{ui_prefix}/settings/signals/{signal_id}', defer=True)
 
     def on_action_clear(self):
         self._driver_publish(f'm/{self._id}/g/!clear', 0)
```

### Comparing `joulescope_ui-1.1.6/joulescope_ui/devices/jsdrv/jsdrv_wrapper.py` & `joulescope_ui-1.1.7/joulescope_ui/devices/jsdrv/jsdrv_wrapper.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/devices/test/test_device_update.py` & `joulescope_ui-1.1.7/joulescope_ui/devices/test/test_device_update.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/disk_monitor.py` & `joulescope_ui-1.1.7/joulescope_ui/disk_monitor.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/entry_points/__init__.py` & `joulescope_ui-1.1.7/joulescope_ui/entry_points/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/entry_points/ui.py` & `joulescope_ui-1.1.7/joulescope_ui/entry_points/ui.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/entry_points/zip_inspector.py` & `joulescope_ui-1.1.7/joulescope_ui/entry_points/zip_inspector.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/error_dialog.py` & `joulescope_ui-1.1.7/joulescope_ui/error_dialog.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/error_window.py` & `joulescope_ui-1.1.7/joulescope_ui/error_window.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/expanding_widget.py` & `joulescope_ui-1.1.7/joulescope_ui/expanding_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/exporter.py` & `joulescope_ui-1.1.7/joulescope_ui/exporter.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/file_dialog.py` & `joulescope_ui-1.1.7/joulescope_ui/file_dialog.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/filename_formatter.py` & `joulescope_ui-1.1.7/joulescope_ui/filename_formatter.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/fonts/DSEG14-Modern/DSEG-LICENSE.txt` & `joulescope_ui-1.1.7/joulescope_ui/fonts/DSEG14-Modern/DSEG-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/fonts/Hack/LICENSE.md` & `joulescope_ui-1.1.7/joulescope_ui/fonts/Hack/LICENSE.md`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/fonts/Lato/OFL.txt` & `joulescope_ui-1.1.7/joulescope_ui/fonts/Lato/OFL.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/fonts/SourceCodePro/LICENSE.md` & `joulescope_ui-1.1.7/joulescope_ui/fonts/SourceCodePro/LICENSE.md`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/fonts/SourceSerifPro/OFL.txt` & `joulescope_ui-1.1.7/joulescope_ui/fonts/SourceSerifPro/OFL.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/fonts.rcc` & `joulescope_ui-1.1.7/joulescope_ui/fonts.rcc`

 * *Files 1% similar despite different names*

```diff
@@ -193814,70 +193814,70 @@
 002f5150: 0000 0000 0000 0000 0000 0080 0002 0000  ................
 002f5160: 000a 0000 0027 0000 0000 0000 0000 0000  .....'..........
 002f5170: 0050 0002 0000 000c 0000 001b 0000 0000  .P..............
 002f5180: 0000 0000 0000 0010 0002 0000 0006 0000  ................
 002f5190: 0015 0000 0000 0000 0000 0000 0030 0002  .............0..
 002f51a0: 0000 000e 0000 0007 0000 0000 0000 0000  ................
 002f51b0: 0000 071a 0004 0000 0001 0025 4f27 0000  ...........%O'..
-002f51c0: 018f 1ab3 104c 0000 07c4 0004 0000 0001  .....L..........
-002f51d0: 0029 2537 0000 018f 1ab3 1048 0000 058c  .)%7.......H....
-002f51e0: 0004 0000 0001 001c 6407 0000 018f 1ab3  ........d.......
-002f51f0: 1050 0000 05ba 0004 0000 0001 001d 95a3  .P..............
-002f5200: 0000 018f 1ab3 1058 0000 0750 0004 0000  .......X...P....
-002f5210: 0001 0026 8517 0000 018f 1ab3 1058 0000  ...&.........X..
+002f51c0: 018f 6800 b746 0000 07c4 0004 0000 0001  ..h..F..........
+002f51d0: 0029 2537 0000 018f 6800 b742 0000 058c  .)%7....h..B....
+002f51e0: 0004 0000 0001 001c 6407 0000 018f 6800  ........d.....h.
+002f51f0: b74a 0000 05ba 0004 0000 0001 001d 95a3  .J..............
+002f5200: 0000 018f 6800 b74e 0000 0750 0004 0000  ....h..N...P....
+002f5210: 0001 0026 8517 0000 018f 6800 b752 0000  ...&......h..R..
 002f5220: 07fc 0004 0000 0001 002a 5802 0000 018f  .........*X.....
-002f5230: 1ab3 104c 0000 082e 0004 0000 0001 002b  ...L...........+
-002f5240: c4d1 0000 018f 1ab3 1050 0000 062c 0004  .........P...,..
-002f5250: 0000 0001 0020 3160 0000 018f 1ab3 1054  ..... 1`.......T
+002f5230: 6800 b746 0000 082e 0004 0000 0001 002b  h..F...........+
+002f5240: c4d1 0000 018f 6800 b74a 0000 062c 0004  ......h..J...,..
+002f5250: 0000 0001 0020 3160 0000 018f 6800 b74e  ..... 1`....h..N
 002f5260: 0000 05f4 0004 0000 0001 001f 01ac 0000  ................
-002f5270: 018f 1ab3 1054 0000 078e 0004 0000 0001  .....T..........
-002f5280: 0027 bab6 0000 018f 1ab3 1054 0000 0666  .'.........T...f
-002f5290: 0004 0000 0001 0021 6449 0000 018f 1ab3  .......!dI......
-002f52a0: 1050 0000 06e6 0004 0000 0001 0023 e72d  .P...........#.-
-002f52b0: 0000 018f 1ab3 1048 0000 0862 0004 0000  .......H...b....
-002f52c0: 0001 002d 262d 0000 018f 1ab3 1054 0000  ...-&-.......T..
+002f5270: 018f 6800 b74a 0000 078e 0004 0000 0001  ..h..J..........
+002f5280: 0027 bab6 0000 018f 6800 b74e 0000 0666  .'......h..N...f
+002f5290: 0004 0000 0001 0021 6449 0000 018f 6800  .......!dI....h.
+002f52a0: b746 0000 06e6 0004 0000 0001 0023 e72d  .F...........#.-
+002f52b0: 0000 018f 6800 b742 0000 0862 0004 0000  ....h..B...b....
+002f52c0: 0001 002d 262d 0000 018f 6800 b74e 0000  ...-&-....h..N..
 002f52d0: 06a8 0004 0000 0001 0022 8ce5 0000 018f  ........."......
-002f52e0: 1ab3 104c 0000 089a 0004 0000 0001 002e  ...L............
-002f52f0: 90bc 0000 018f 1ab3 103c 0000 08d0 0004  .........<......
-002f5300: 0000 0001 002e af00 0000 018f 1ab3 103c  ...............<
+002f52e0: 6800 b746 0000 089a 0004 0000 0001 002e  h..F............
+002f52f0: 90bc 0000 018f 6800 b736 0000 08d0 0004  ......h..6......
+002f5300: 0000 0001 002e af00 0000 018f 6800 b736  ............h..6
 002f5310: 0000 097c 0004 0000 0001 002f 0ab2 0000  ...|......./....
-002f5320: 018f 1ab3 103c 0000 09b0 0004 0000 0001  .....<..........
-002f5330: 002f 293e 0000 018f 1ab3 103c 0000 090c  ./)>.......<....
-002f5340: 0004 0000 0001 002e cd3f 0000 018f 1ab3  .........?......
-002f5350: 103c 0000 094a 0004 0000 0001 002e ec32  .<...J.........2
-002f5360: 0000 018f 1ab3 103c 0000 0544 0004 0000  .......<...D....
-002f5370: 0001 001b 3ffe 0000 018f 1ab3 1064 0000  ....?........d..
+002f5320: 018f 6800 b736 0000 09b0 0004 0000 0001  ..h..6..........
+002f5330: 002f 293e 0000 018f 6800 b736 0000 090c  ./)>....h..6....
+002f5340: 0004 0000 0001 002e cd3f 0000 018f 6800  .........?....h.
+002f5350: b736 0000 094a 0004 0000 0001 002e ec32  .6...J.........2
+002f5360: 0000 018f 6800 b736 0000 0544 0004 0000  ....h..6...D....
+002f5370: 0001 001b 3ffe 0000 018f 6800 b75e 0000  ....?.....h..^..
 002f5380: 036a 0004 0000 0001 0010 f545 0000 018f  .j.........E....
-002f5390: 1ab3 105c 0000 041a 0004 0000 0001 0014  ...\............
-002f53a0: f75f 0000 018f 1ab3 1060 0000 048c 0004  ._.......`......
-002f53b0: 0000 0001 0017 6f8d 0000 018f 1ab3 1060  ......o........`
+002f5390: 6800 b756 0000 041a 0004 0000 0001 0014  h..V............
+002f53a0: f75f 0000 018f 6800 b75a 0000 048c 0004  ._....h..Z......
+002f53b0: 0000 0001 0017 6f8d 0000 018f 6800 b75a  ......o.....h..Z
 002f53c0: 0000 04c2 0004 0000 0001 0018 d613 0000  ................
-002f53d0: 018f 1ab3 105c 0000 03aa 0004 0000 0001  .....\..........
-002f53e0: 0012 1971 0000 018f 1ab3 105c 0000 03de  ...q.......\....
-002f53f0: 0004 0000 0001 0013 8810 0000 018f 1ab3  ................
-002f5400: 1064 0000 02dc 0004 0000 0001 000e c39f  .d..............
-002f5410: 0000 018f 1ab3 1060 0000 0452 0004 0000  .......`...R....
-002f5420: 0001 0016 0ed3 0000 018f 1ab3 1064 0000  .............d..
+002f53d0: 018f 6800 b756 0000 03aa 0004 0000 0001  ..h..V..........
+002f53e0: 0012 1971 0000 018f 6800 b756 0000 03de  ...q....h..V....
+002f53f0: 0004 0000 0001 0013 8810 0000 018f 6800  ..............h.
+002f5400: b75e 0000 02dc 0004 0000 0001 000e c39f  .^..............
+002f5410: 0000 018f 6800 b75a 0000 0452 0004 0000  ....h..Z...R....
+002f5420: 0001 0016 0ed3 0000 018f 6800 b75a 0000  ..........h..Z..
 002f5430: 0502 0004 0000 0001 001a 2aab 0000 018f  ..........*.....
-002f5440: 1ab3 1058 0000 031e 0004 0000 0001 000f  ...X............
-002f5450: e47b 0000 018f 1ab3 1060 0000 02a6 0004  .{.......`......
-002f5460: 0000 0001 000d 65a3 0000 018f 1ab3 1058  ......e........X
+002f5440: 6800 b752 0000 031e 0004 0000 0001 000f  h..R............
+002f5450: e47b 0000 018f 6800 b756 0000 02a6 0004  .{....h..V......
+002f5460: 0000 0001 000d 65a3 0000 018f 6800 b752  ......e.....h..R
 002f5470: 0000 01ae 0004 0000 0001 0003 6c6f 0000  ............lo..
-002f5480: 018f 1ab3 1044 0000 008e 0004 0000 0001  .....D..........
-002f5490: 0000 0000 0000 018f 1ab3 1044 0000 018a  ...........D....
-002f54a0: 0004 0000 0001 0002 e1fa 0000 018f 1ab3  ................
-002f54b0: 1044 0000 010a 0004 0000 0001 0001 72aa  .D............r.
-002f54c0: 0000 018f 1ab3 1044 0000 00e8 0004 0000  .......D........
-002f54d0: 0001 0000 f2c6 0000 018f 1ab3 1044 0000  .............D..
+002f5480: 018f 6800 b73e 0000 008e 0004 0000 0001  ..h..>..........
+002f5490: 0000 0000 0000 018f 6800 b73e 0000 018a  ........h..>....
+002f54a0: 0004 0000 0001 0002 e1fa 0000 018f 6800  ..............h.
+002f54b0: b73e 0000 010a 0004 0000 0001 0001 72aa  .>............r.
+002f54c0: 0000 018f 6800 b73e 0000 00e8 0004 0000  ....h..>........
+002f54d0: 0001 0000 f2c6 0000 018f 6800 b73e 0000  ..........h..>..
 002f54e0: 015e 0004 0000 0001 0002 7e0b 0000 018f  .^........~.....
-002f54f0: 1ab3 1048 0000 00ba 0004 0000 0001 0000  ...H............
-002f5500: 8b33 0000 018f 1ab3 1044 0000 01f0 0004  .3.......D......
-002f5510: 0000 0001 0004 74f0 0000 018f 1ab3 1048  ......t........H
+002f54f0: 6800 b742 0000 00ba 0004 0000 0001 0000  h..B............
+002f5500: 8b33 0000 018f 6800 b73e 0000 01f0 0004  .3....h..>......
+002f5510: 0000 0001 0004 74f0 0000 018f 6800 b742  ......t.....h..B
 002f5520: 0000 01ce 0004 0000 0001 0003 ee66 0000  .............f..
-002f5530: 018f 1ab3 1044 0000 0130 0004 0000 0001  .....D...0......
-002f5540: 0001 f768 0000 018f 1ab3 1044 0000 0210  ...h.......D....
-002f5550: 0004 0000 0001 0004 f353 0000 018f 1ab3  .........S......
-002f5560: 1040 0000 027a 0004 0000 0001 000b 366d  .@...z........6m
-002f5570: 0000 018f 1ab3 1040 0000 0234 0004 0000  .......@...4....
-002f5580: 0001 0007 158f 0000 018f 1ab3 103c 0000  .............<..
+002f5530: 018f 6800 b73e 0000 0130 0004 0000 0001  ..h..>...0......
+002f5540: 0001 f768 0000 018f 6800 b73e 0000 0210  ...h....h..>....
+002f5550: 0004 0000 0001 0004 f353 0000 018f 6800  .........S....h.
+002f5560: b73a 0000 027a 0004 0000 0001 000b 366d  .:...z........6m
+002f5570: 0000 018f 6800 b73a 0000 0234 0004 0000  ....h..:...4....
+002f5580: 0001 0007 158f 0000 018f 6800 b736 0000  ..........h..6..
 002f5590: 0254 0004 0000 0001 0009 2ac5 0000 018f  .T........*.....
-002f55a0: 1ab3 1044                                ...D
+002f55a0: 6800 b73e                                h..>
```

### Comparing `joulescope_ui-1.1.6/joulescope_ui/getting_started.py` & `joulescope_ui-1.1.7/joulescope_ui/getting_started.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/help_ui.py` & `joulescope_ui-1.1.7/joulescope_ui/help_ui.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/intel_graphics_dialog.py` & `joulescope_ui-1.1.7/joulescope_ui/intel_graphics_dialog.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/jls_source.py` & `joulescope_ui-1.1.7/joulescope_ui/jls_source.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/jls_v1.py` & `joulescope_ui-1.1.7/joulescope_ui/jls_v1.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/jls_v2.py` & `joulescope_ui-1.1.7/joulescope_ui/jls_v2.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/jls_v2_annotations.py` & `joulescope_ui-1.1.7/joulescope_ui/jls_v2_annotations.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/json_plus.py` & `joulescope_ui-1.1.7/joulescope_ui/json_plus.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/locale/__init__.py` & `joulescope_ui-1.1.7/joulescope_ui/locale/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/locale/ar/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.7/joulescope_ui/locale/ar/LC_MESSAGES/joulescope_ui.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.2\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-18 14:15-0400\n"
+"POT-Creation-Date: 2024-05-06 17:27-0400\n"
 "PO-Revision-Date: 2024-04-04 14:45-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: ar\n"
 "Language-Team: ar <LL@li.org>\n"
 "Plural-Forms: nplurals=6; plural=(n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
 "&& n%100<=10 ? 3 : n%100>=0 && n%100<=2 ? 4 : 5);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.14.0\n"
+"Generated-By: Babel 2.15.0\n"
 
 msgid "\"3.3 V\" uses an internally-generated 3.3V reference voltage."
 msgstr "\"3.3 فولت\" يستخدم جهدًا مرجعيًا 3.3 فولت مولدًا داخليًا."
 
 msgid "\"NaN\" sets all samples in the window to NaN."
 msgstr "\"NaN\" يضبط جميع العينات في النافذة على NaN."
 
@@ -622,14 +622,17 @@
 
 msgid ""
 "Display the number of actions processed by the publish-subscribe broker in "
 "each second."
 msgstr ""
 "عرض عدد الإجراءات التي تتم معالجتها بواسطة وسيط النشر والاشتراك في كل ثانية."
 
+msgid "Divide the quantity by this value."
+msgstr "اقسم الكمية على هذه القيمة."
+
 msgid "Do not show again"
 msgstr "لا تظهر مرة أخرى"
 
 msgid "Do not use any USB hubs, docks or adapters"
 msgstr "لا تستخدم أي محاور USB أو أرصفة أو محولات أو محولات"
 
 msgid "Dual markers"
@@ -1709,14 +1712,19 @@
 "selected)."
 msgstr ""
 "يتم تحديث القيم المعروضة عادةً مع كل بيانات إحصائية جديدة يحسبها الجهاز. عند "
 "تحديد هذا الزر، لن يتم تحديث العرض. ومع ذلك، ستستمر الإحصائيات في التراكم "
 "والتراكم (إذا تم تحديده)."
 
 msgid ""
+"The divisor is a floating point number. The number may optionally be "
+"followed by units."
+msgstr "المقسوم عليه هو رقم عائم. قد يتبع الرقم اختياريًا وحدات."
+
+msgid ""
 "The exponential decay time constant. The fuse dissipates 63.2 percent of "
 "accumulated energy in this duration."
 msgstr ""
 "ثابت زمن التضاؤل الأسي. يبدد المصهر 63.2 بالمائة من الطاقة المتراكمة في هذه "
 "المدة."
 
 msgid "The filename supports the following replacements."
@@ -1724,17 +1732,14 @@
 
 msgid "The filename with optional replacements."
 msgstr "اسم الملف مع بدائل اختيارية."
 
 msgid "The fixed default path for loading and saving files."
 msgstr "المسار الافتراضي الثابت لتحميل الملفات وحفظها."
 
-msgid "The flyout width in pixels."
-msgstr "عرض التحليق بالبكسل."
-
 msgid "The font scheme name."
 msgstr "اسم مخطط الخط."
 
 msgid "The format string"
 msgstr "سلسلة التنسيق"
 
 msgid "The fuse trips in Duration at this constant current."
```

### Comparing `joulescope_ui-1.1.6/joulescope_ui/locale/ar/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.7/joulescope_ui/locale/ar/LC_MESSAGES/joulescope_ui.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.2\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-18 14:15-0400\n"
+"POT-Creation-Date: 2024-05-06 17:27-0400\n"
 "PO-Revision-Date: 2024-04-04 14:45-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: ar <LL@li.org>\n"
 "Language: ar\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=6; plural=(n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 && n%100<=10 ? 3 : n%100>=0 && n%100<=2 ? 4 : 5);\n"
-"Generated-By: Babel 2.14.0\n"
+"Generated-By: Babel 2.15.0\n"
 
 #: about.py:24
 msgid "About the Joulescope UI"
 msgstr "حول واجهة المستخدم Joulescope UI"
 
 #: about.py:25
 msgid "Version Information"
@@ -316,27 +316,27 @@
 msgid "Email"
 msgstr "البريد الإلكتروني"
 
 #: error_window.py:103
 msgid "Description"
 msgstr "الوصف"
 
-#: error_window.py:112 widgets/waveform/waveform_widget.py:3347
+#: error_window.py:112 widgets/waveform/waveform_widget.py:3397
 msgid "Edit"
 msgstr "تحرير"
 
 #: error_window.py:113
 msgid "View as Markdown"
 msgstr "عرض كتخفيض"
 
 #: error_window.py:119
 msgid "Abort"
 msgstr "الإجهاض"
 
-#: error_window.py:120 main.py:365 widgets/settings/settings_widget.py:539
+#: error_window.py:120 main.py:363 widgets/settings/settings_widget.py:539
 msgid "View"
 msgstr "عرض"
 
 #: error_window.py:121
 msgid "Submit"
 msgstr "إرسال"
 
@@ -348,15 +348,15 @@
 msgid "Revert to previous configuration"
 msgstr "العودة إلى التكوين السابق"
 
 #: error_window.py:282
 msgid "Revert to defaults"
 msgstr "العودة إلى الإعدادات الافتراضية"
 
-#: error_window.py:283 main.py:363 main.py:409
+#: error_window.py:283 main.py:361 main.py:407
 #: widgets/js220_cal/js220_cal_widget.py:38
 msgid "Exit"
 msgstr "خروج"
 
 #: exporter.py:49 widgets/signal_record/signal_record_config_widget.py:148
 #: widgets/statistics_record/statistics_record_config_widget.py:111
 msgid "Directory"
@@ -610,162 +610,162 @@
 msgid "Do not show again"
 msgstr "لا تظهر مرة أخرى"
 
 #: intel_graphics_dialog.py:91
 msgid "Intel graphics detected"
 msgstr "تم الكشف عن رسومات إنتل"
 
-#: main.py:70 widgets/value/value_widget.py:653
+#: main.py:69 widgets/value/value_widget.py:660
 msgid "Multimeter"
 msgstr "متعدد المقاييس"
 
-#: main.py:71
+#: main.py:70
 msgid "Oscilloscope"
 msgstr "راسم الذبذبات"
 
-#: main.py:72 main.py:298 main.py:359 main.py:402
+#: main.py:71 main.py:296 main.py:357 main.py:400
 msgid "File"
 msgstr "ملف"
 
-#: main.py:82
+#: main.py:81
 msgid "The UI status bar display mode"
 msgstr "وضع عرض شريط حالة واجهة المستخدم"
 
-#: main.py:83
+#: main.py:82
 msgid ""
 "This setting controls the amount of detail shown on the status bar at the "
 "bottom of the UI window. You should usually leave this set to \"normal\" "
 "unless you want more detail concerning the UI internal operation."
 msgstr ""
 "يتحكم هذا الإعداد في مقدار التفاصيل التي تظهر على شريط الحالة في أسفل نافذة "
 "واجهة المستخدم. يجب عادةً ترك هذا الإعداد على \"عادي\" إلا إذا كنت تريد "
 "المزيد من التفاصيل المتعلقة بالتشغيل الداخلي لواجهة المستخدم."
 
-#: main.py:88 safe_mode.py:43
+#: main.py:87 safe_mode.py:43
 msgid "Normal"
 msgstr "عادي"
 
-#: main.py:89
+#: main.py:88
 msgid "Troubleshoot"
 msgstr "استكشاف الأخطاء وإصلاحها"
 
-#: main.py:95
+#: main.py:94
 msgid "Enable developer mode."
 msgstr "تمكين وضع المطور."
 
-#: main.py:108
+#: main.py:107
 msgid "PubSub utilization"
 msgstr "استخدام PubSub"
 
-#: main.py:109
+#: main.py:108
 msgid ""
 "Display the number of actions processed by the publish-subscribe broker in "
 "each second."
 msgstr ""
 "عرض عدد الإجراءات التي تتم معالجتها بواسطة وسيط النشر والاشتراك في كل ثانية."
 
-#: main.py:114
+#: main.py:113
 msgid "CPU utilization"
 msgstr "استخدام وحدة المعالجة المركزية"
 
-#: main.py:115
+#: main.py:114
 msgid ""
 "Display the CPU utilization by this application and the total CPU "
 "utilization by all applications. The value is displayed in percent."
 msgstr ""
 "عرض استخدام وحدة المعالجة المركزية بواسطة هذا التطبيق وإجمالي استخدام وحدة "
 "المعالجة المركزية بواسطة جميع التطبيقات. يتم عرض القيمة بالنسبة المئوية."
 
-#: main.py:121
+#: main.py:120
 msgid "Memory utilization"
 msgstr "استخدام الذاكرة"
 
-#: main.py:122
+#: main.py:121
 msgid ""
 "Display the memory (RAM) utilization by this application and by all "
 "applications. The value is displayed in percent."
 msgstr ""
 "عرض استخدام الذاكرة (RAM) بواسطة هذا التطبيق وجميع التطبيقات. يتم عرض القيمة"
 " بالنسبة المئوية."
 
-#: main.py:216
+#: main.py:214
 msgid "UI"
 msgstr "واجهة المستخدم"
 
-#: main.py:330
+#: main.py:328
 msgid "Help"
 msgstr "المساعدة"
 
-#: main.py:331 widgets/hamburger/hamburger_widget.py:21
+#: main.py:329 widgets/hamburger/hamburger_widget.py:21
 msgid "Getting Started"
 msgstr "الشروع في العمل"
 
-#: main.py:332
+#: main.py:330
 msgid "User's Guide"
 msgstr "دليل المستخدم"
 
-#: main.py:333 widgets/hamburger/hamburger_widget.py:22
+#: main.py:331 widgets/hamburger/hamburger_widget.py:22
 msgid "Changelog"
 msgstr "سجل التغييرات"
 
-#: main.py:334 widgets/help/help_widget.py:59
+#: main.py:332 widgets/help/help_widget.py:59
 msgid "Report Issue"
 msgstr "إصدار التقرير"
 
-#: main.py:335
+#: main.py:333
 msgid "View logs..."
 msgstr "عرض السجلات..."
 
-#: main.py:336 widgets/hamburger/hamburger_widget.py:23
+#: main.py:334 widgets/hamburger/hamburger_widget.py:23
 msgid "Credits"
 msgstr "الاعتمادات"
 
-#: main.py:337 widgets/hamburger/hamburger_widget.py:24
+#: main.py:335 widgets/hamburger/hamburger_widget.py:24
 msgid "About"
 msgstr "نبذة عن"
 
-#: main.py:360
+#: main.py:358
 msgid "Open"
 msgstr "مفتوح"
 
-#: main.py:361
+#: main.py:359
 msgid "Open recent"
 msgstr "مفتوح حديثاً"
 
-#: main.py:362 main.py:408
+#: main.py:360 main.py:406
 msgid "Clear config and exit"
 msgstr "مسح التكوين والخروج"
 
-#: main.py:366 widgets/settings/settings_widget.py:541
+#: main.py:364 widgets/settings/settings_widget.py:541
 msgid "Widgets"
 msgstr "الأدوات"
 
-#: main.py:367
+#: main.py:365
 msgid "Tools"
 msgstr "الأدوات"
 
-#: main.py:368
+#: main.py:366
 msgid "Clear Accumulators"
 msgstr "المجمعات الواضحة"
 
-#: main.py:403
+#: main.py:401
 msgid "Info"
 msgstr "معلومات"
 
-#: main.py:404 widget_tools.py:92 widgets/settings/settings_widget.py:31
+#: main.py:402 widget_tools.py:92 widgets/settings/settings_widget.py:31
 #: widgets/settings/settings_widget.py:574
 #: widgets/sidebar/sidebar_widget.py:41
 msgid "Settings"
 msgstr "الإعدادات"
 
-#: main.py:693
+#: main.py:710
 msgid "Manage"
 msgstr "إدارة"
 
-#: main.py:730
+#: main.py:747
 msgid "Select file to open"
 msgstr "حدد الملف لفتحه"
 
 #: paths.py:30 styles/manager.py:46
 msgid "The name for this widget."
 msgstr "اسم هذه الأداة"
 
@@ -904,47 +904,47 @@
 msgid "Source"
 msgstr "المصدر"
 
 #: units.py:35
 msgid "Use the application defaults"
 msgstr "استخدم الإعدادات الافتراضية للتطبيق"
 
-#: view.py:68
+#: view.py:72
 msgid "The active theme."
 msgstr "السمة النشطة"
 
-#: view.py:70
+#: view.py:74
 msgid "Joulescope standard theme"
 msgstr "سمة جولسكوب القياسية"
 
-#: view.py:70
+#: view.py:74
 msgid "System OS-specific theme"
 msgstr "سمة خاصة بنظام التشغيل"
 
-#: view.py:75
+#: view.py:79
 msgid "The color scheme name."
 msgstr "اسم نظام الألوان."
 
-#: view.py:77
+#: view.py:81
 msgid "Dark background"
 msgstr "خلفية داكنة"
 
-#: view.py:77
+#: view.py:81
 msgid "Light background"
 msgstr "خلفية ضوئية"
 
-#: view.py:81
+#: view.py:85
 msgid "The font scheme name."
 msgstr "اسم مخطط الخط."
 
-#: view.py:83
+#: view.py:87
 msgid "Joulescope standard font theme"
 msgstr "سمة خط Joulescope القياسية"
 
-#: view.py:102 widgets/view_manager/view_manager_widget.py:146
+#: view.py:106 widgets/view_manager/view_manager_widget.py:146
 msgid "New View"
 msgstr "عرض جديد"
 
 #: zip_inspector.py:23
 msgid "ZIP Inspector"
 msgstr "مفتش ZIP"
 
@@ -1058,15 +1058,15 @@
 "target device."
 msgstr ""
 "عند التمكين، يتدفق التيار بين طرفي التيار. عند تعطيله، لا يمكن للتيار أن "
 "يتدفق بين أطراف التيار. في إعدادات النظام الشائعة، يؤدي ذلك إلى تثبيط الطاقة"
 " المستهدفة، والتي يمكن استخدامها لإعادة ضبط دورة الطاقة للجهاز المستهدف."
 
 #: devices/jsdrv/js110.py:147 devices/jsdrv/js220.py:163
-#: widgets/waveform/waveform_widget.py:110
+#: widgets/waveform/waveform_widget.py:109
 msgid "Current range"
 msgstr "النطاق الحالي"
 
 #: devices/jsdrv/js110.py:149
 msgid ""
 "Configure the J110's current range. Most applications should use the "
 "default, \"auto\"."
@@ -1206,33 +1206,33 @@
 "The number of samples after the current range window used to determine the "
 "mean. This value is ignored for all other IRF types."
 msgstr ""
 "عدد العينات بعد نافذة النطاق الحالي المستخدمة لتحديد المتوسط. يتم تجاهل هذه "
 "القيمة لجميع أنواع IRF الأخرى."
 
 #: devices/jsdrv/js110.py:269 devices/jsdrv/js220.py:332
-#: widgets/device_control/fuse.py:103 widgets/waveform/waveform_widget.py:105
+#: widgets/device_control/fuse.py:103 widgets/waveform/waveform_widget.py:104
 msgid "Current"
 msgstr "التيار"
 
 #: devices/jsdrv/js110.py:270 devices/jsdrv/js220.py:333
 msgid "Enable the current signal streaming."
 msgstr "تمكين تدفق الإشارة الحالية."
 
 #: devices/jsdrv/js110.py:278 devices/jsdrv/js220.py:341
-#: widgets/waveform/waveform_widget.py:106
+#: widgets/waveform/waveform_widget.py:105
 msgid "Voltage"
 msgstr "الجهد"
 
 #: devices/jsdrv/js110.py:279 devices/jsdrv/js220.py:342
 msgid "Enable the voltage signal streaming."
 msgstr "تمكين تدفق إشارة الجهد."
 
 #: devices/jsdrv/js110.py:287 devices/jsdrv/js220.py:350
-#: widgets/waveform/waveform_widget.py:107
+#: widgets/waveform/waveform_widget.py:106
 msgid "Power"
 msgstr "الطاقة"
 
 #: devices/jsdrv/js110.py:288 devices/jsdrv/js220.py:351
 msgid "Enable the power signal streaming."
 msgstr "تمكين تدفق إشارة الطاقة."
 
@@ -1435,15 +1435,15 @@
 msgid "GPI 3"
 msgstr "GPI 3"
 
 #: devices/jsdrv/js220.py:402
 msgid "Enable the general purpose input 3 signal streaming."
 msgstr "تمكين تدفق إشارة الإدخال 3 للأغراض العامة."
 
-#: devices/jsdrv/js220.py:410 widgets/waveform/waveform_widget.py:124
+#: devices/jsdrv/js220.py:410 widgets/waveform/waveform_widget.py:123
 msgid "Trigger input"
 msgstr "مدخلات الزناد"
 
 #: devices/jsdrv/js220.py:411
 msgid "Enable the trigger input signal streaming."
 msgstr "تمكين تدفق إشارة إدخال الزناد."
 
@@ -1454,15 +1454,15 @@
 #: devices/jsdrv/jsdrv_stream_buffer.py:44
 #: devices/jsdrv/jsdrv_stream_buffer.py:93
 #: devices/jsdrv/jsdrv_stream_buffer.py:107 plugins/selector.py:58
 #: widgets/settings/settings_widget.py:85
 #: widgets/settings/settings_widget.py:266
 #: widgets/settings/settings_widget.py:364
 #: widgets/settings/settings_widget.py:431
-#: widgets/waveform/waveform_widget.py:3062
+#: widgets/waveform/waveform_widget.py:3104
 msgid "Name"
 msgstr "الاسم"
 
 #: devices/jsdrv/jsdrv_stream_buffer.py:45
 msgid "Joulescope stream buffer"
 msgstr "مخزن جولسكوب للتيار"
 
@@ -1678,15 +1678,15 @@
 
 #: widgets/accumulator/accumulator_widget.py:27
 #: widgets/value/value_widget.py:31
 msgid "The statistics data stream source."
 msgstr "مصدر تدفق البيانات الإحصائية."
 
 #: widgets/accumulator/accumulator_widget.py:32
-#: widgets/value/value_widget.py:74
+#: widgets/value/value_widget.py:81
 msgid "The signal to display."
 msgstr "الإشارة المراد عرضها."
 
 #: widgets/accumulator/accumulator_widget.py:34
 msgid "charge"
 msgstr "الشحن"
 
@@ -1769,15 +1769,15 @@
 
 #: widgets/developer/publish_spy_widget.py:20
 #: widgets/developer/publish_spy_widget.py:21
 msgid "Topic"
 msgstr "الموضوع"
 
 #: widgets/developer/publish_spy_widget.py:21
-#: widgets/settings/settings_widget.py:87 widgets/value/value_widget.py:662
+#: widgets/settings/settings_widget.py:87 widgets/value/value_widget.py:669
 msgid "Value"
 msgstr "القيمة"
 
 #: widgets/developer/publish_spy_widget.py:24
 msgid "Publish Spy"
 msgstr "نشر الجاسوس"
 
@@ -1807,15 +1807,15 @@
 
 #: widgets/device_control/device_update_dialog.py:24
 #: widgets/device_control/device_update_dialog.py:45
 msgid "Update"
 msgstr "تحديث"
 
 #: widgets/device_control/device_update_dialog.py:25
-#: widgets/value/value_widget.py:147
+#: widgets/value/value_widget.py:155
 msgid "Device"
 msgstr "الجهاز"
 
 #: widgets/device_control/device_update_dialog.py:27
 #: widgets/progress_bar/progress_bar_widget.py:59
 msgid "Progress"
 msgstr "التقدم"
@@ -2325,18 +2325,14 @@
 msgid "Click to display additional settings and actions."
 msgstr "انقر لعرض إعدادات وإجراءات إضافية."
 
 #: widgets/sidebar/sidebar_widget.py:60
 msgid "sidebar"
 msgstr "الشريط الجانبي"
 
-#: widgets/sidebar/sidebar_widget.py:68
-msgid "The flyout width in pixels."
-msgstr "عرض التحليق بالبكسل."
-
 #: widgets/signal_record/disk_full_dialog.py:19
 msgid "The disk is full"
 msgstr "القرص ممتلئ"
 
 #: widgets/signal_record/signal_record.py:57
 msgid "Could not open file for write"
 msgstr "تعذر فتح الملف للكتابة"
@@ -2363,15 +2359,15 @@
 msgid "StatisticsRecordConfig"
 msgstr "إحصائياتالتسجيلالتكوين"
 
 #: widgets/statistics_record/statistics_record_config_widget.py:123
 msgid "Time Format"
 msgstr "تنسيق الوقت"
 
-#: widgets/trigger/trigger_widget.py:41 widgets/value/value_widget.py:87
+#: widgets/trigger/trigger_widget.py:41 widgets/value/value_widget.py:94
 msgid "Select the source device"
 msgstr "حدد الجهاز المصدر"
 
 #: widgets/trigger/trigger_widget.py:42
 msgid "The device to use for the start condition and stop condition."
 msgstr "الجهاز المستخدم لحالة البدء وحالة التوقف."
 
@@ -2539,80 +2535,90 @@
 msgid "Show the statistics fields at the right."
 msgstr "عرض حقول الإحصائيات على اليمين."
 
 #: widgets/value/value_widget.py:51
 msgid "Show a leading + or - sign."
 msgstr "إظهار علامة + أو -."
 
-#: widgets/value/value_widget.py:88
+#: widgets/value/value_widget.py:62
+msgid "Divide the quantity by this value."
+msgstr "اقسم الكمية على هذه القيمة."
+
+#: widgets/value/value_widget.py:63
+msgid ""
+"The divisor is a floating point number. The number may optionally be "
+"followed by units."
+msgstr "المقسوم عليه هو رقم عائم. قد يتبع الرقم اختياريًا وحدات."
+
+#: widgets/value/value_widget.py:95
 msgid ""
 "The values displayed by this widget come from a single source device. Select"
 " the source device here."
 msgstr ""
 "تأتي القيم التي تعرضها هذه الأداة من جهاز مصدر واحد. حدد الجهاز المصدر هنا."
 
-#: widgets/value/value_widget.py:94
+#: widgets/value/value_widget.py:101
 msgid "Hold the display"
 msgstr "امسك الشاشة"
 
-#: widgets/value/value_widget.py:96
+#: widgets/value/value_widget.py:103
 msgid "When selected, prevent the display from updating."
 msgstr "عند تحديده، يمنع الشاشة من التحديث."
 
-#: widgets/value/value_widget.py:97
+#: widgets/value/value_widget.py:104
 msgid ""
 "The UI also includes a global statistics hold button on the sidebar. When "
 "the global statistics hold button is selected, this button is disabled and "
 "has no effect."
 msgstr ""
 "تتضمن واجهة المستخدم أيضًا زر تعليق الإحصائيات العامة على الشريط الجانبي. "
 "عند تحديد زر تعليق الإحصائيات العامة، يتم تعطيل هذا الزر وليس له أي تأثير."
 
-#: widgets/value/value_widget.py:100
+#: widgets/value/value_widget.py:107
 msgid ""
 "The displayed values normally update with each new statistics data computed "
 "by the device. When this button is selected, the display will not be "
 "updated. However, the statistics will continue accumulate and accrue (if "
 "selected)."
 msgstr ""
 "يتم تحديث القيم المعروضة عادةً مع كل بيانات إحصائية جديدة يحسبها الجهاز. عند"
 " تحديد هذا الزر، لن يتم تحديث العرض. ومع ذلك، ستستمر الإحصائيات في التراكم "
 "والتراكم (إذا تم تحديده)."
 
-#: widgets/value/value_widget.py:107
+#: widgets/value/value_widget.py:114
 msgid "Accrue values over time"
 msgstr "تراكم القيم بمرور الوقت"
 
-#: widgets/value/value_widget.py:109
+#: widgets/value/value_widget.py:116
 msgid ""
 "Current, voltage, and power are normally computed over a single statistics "
 "frequency interval. Press this button to accrue the values indefinitely. "
 "Press again to return to normal operation."
 msgstr ""
 "عادةً ما يتم حساب التيار والجهد والطاقة على فاصل تردد إحصائي واحد. اضغط على "
 "هذا الزر لتجميع القيم إلى أجل غير مسمى. اضغط مرة أخرى للعودة إلى التشغيل "
 "العادي."
 
-#: widgets/value/value_widget.py:113
+#: widgets/value/value_widget.py:120
 msgid ""
 "Note that this button does not affect the charge and energy accumulation. "
 "Both accumulate indefinitely regardless of this button state."
 msgstr ""
 "لاحظ أن هذا الزر لا يؤثر على تراكم الشحن والطاقة. يتراكم كلاهما إلى أجل غير "
 "مسمى بغض النظر عن حالة هذا الزر."
 
-#: widgets/value/value_widget.py:195
+#: widgets/value/value_widget.py:203
 msgid "Not present"
 msgstr "غير موجود"
 
-#: widgets/value/value_widget.py:215
+#: widgets/value/value_widget.py:223
 msgid "Hold"
 msgstr "عقد"
 
-#: widgets/value/value_widget.py:223
+#: widgets/value/value_widget.py:231
 msgid "Accrue"
 msgstr "زيادة"
 
 #: widgets/view_manager/view_manager_widget.py:108
 #: widgets/view_manager/view_manager_widget.py:174
 msgid "View Manager"
 msgstr "عرض المدير"
@@ -2658,34 +2664,34 @@
 msgstr "المثلث الأيمن"
 
 #: widgets/waveform/text_annotation.py:62
 msgid "triangle left"
 msgstr "المثلث الأيسر"
 
 #: widgets/waveform/text_annotation.py:66
-#: widgets/waveform/waveform_widget.py:3008
+#: widgets/waveform/waveform_widget.py:3050
 msgid "Manual"
 msgstr "دليل"
 
 #: widgets/waveform/text_annotation.py:67
 msgid "Centered"
 msgstr "المركز"
 
 #: widgets/waveform/text_annotation.py:99
-#: widgets/waveform/waveform_widget.py:3123
+#: widgets/waveform/waveform_widget.py:3167
 msgid "Text"
 msgstr "النص"
 
 #: widgets/waveform/text_annotation.py:107
-#: widgets/waveform/waveform_widget.py:3348
+#: widgets/waveform/waveform_widget.py:3398
 msgid "Show text"
 msgstr "إظهار النص"
 
 #: widgets/waveform/text_annotation.py:116
-#: widgets/waveform/waveform_widget.py:3360
+#: widgets/waveform/waveform_widget.py:3410
 msgid "Shape"
 msgstr "الشكل"
 
 #: widgets/waveform/text_annotation.py:126
 msgid "Y Mode"
 msgstr "الوضع Y"
 
@@ -2872,317 +2878,317 @@
 "\"default\" will use the default source which is normally configured using "
 "the Device Control widget."
 msgstr ""
 "\"افتراضي\" سيستخدم المصدر الافتراضي الذي يتم تكوينه عادةً باستخدام أداة "
 "التحكم في الجهاز."
 
 #: widgets/waveform/waveform_source_widget.py:104
-#: widgets/waveform/waveform_widget.py:402
-#: widgets/waveform/waveform_widget.py:479
+#: widgets/waveform/waveform_widget.py:401
+#: widgets/waveform/waveform_widget.py:478
 msgid "off"
 msgstr "إيقاف"
 
-#: widgets/waveform/waveform_widget.py:44
+#: widgets/waveform/waveform_widget.py:43
 msgid "Waveform"
 msgstr "الشكل الموجي"
 
-#: widgets/waveform/waveform_widget.py:120
+#: widgets/waveform/waveform_widget.py:119
 msgid "General purpose input 0"
 msgstr "مدخلات الأغراض العامة 0"
 
-#: widgets/waveform/waveform_widget.py:121
+#: widgets/waveform/waveform_widget.py:120
 msgid "General purpose input 1"
 msgstr "مدخلات الأغراض العامة 1"
 
-#: widgets/waveform/waveform_widget.py:122
+#: widgets/waveform/waveform_widget.py:121
 msgid "General purpose input 2"
 msgstr "مدخلات الأغراض العامة 2"
 
-#: widgets/waveform/waveform_widget.py:123
+#: widgets/waveform/waveform_widget.py:122
 msgid "General purpose input 3"
 msgstr "مدخلات الأغراض العامة 3"
 
-#: widgets/waveform/waveform_widget.py:358
+#: widgets/waveform/waveform_widget.py:357
 msgid "The source filter string."
 msgstr "سلسلة مرشح المصدر."
 
-#: widgets/waveform/waveform_widget.py:369
+#: widgets/waveform/waveform_widget.py:368
 msgid "The trace width."
 msgstr "عرض التتبع."
 
-#: widgets/waveform/waveform_widget.py:384
+#: widgets/waveform/waveform_widget.py:383
 msgid "The target frames per second."
 msgstr "الإطارات المستهدفة في الثانية."
 
-#: widgets/waveform/waveform_widget.py:386
+#: widgets/waveform/waveform_widget.py:385
 msgid "vsync"
 msgstr "المزامنة"
 
-#: widgets/waveform/waveform_widget.py:387
+#: widgets/waveform/waveform_widget.py:386
 msgid "20 Hz"
 msgstr "20 هرتز"
 
-#: widgets/waveform/waveform_widget.py:388
+#: widgets/waveform/waveform_widget.py:387
 msgid "10 Hz"
 msgstr "10 هرتز"
 
-#: widgets/waveform/waveform_widget.py:389
+#: widgets/waveform/waveform_widget.py:388
 msgid "5 Hz"
 msgstr "5 هرتز"
 
-#: widgets/waveform/waveform_widget.py:395
+#: widgets/waveform/waveform_widget.py:394
 msgid "The minimum interval between repaint in milliseconds."
 msgstr "الحد الأدنى للفاصل الزمني بين إعادة الطلاء بالمللي ثانية."
 
-#: widgets/waveform/waveform_widget.py:400
+#: widgets/waveform/waveform_widget.py:399
 msgid "Show the minimum and maximum extents fill."
 msgstr "إظهار الحد الأدنى والحد الأقصى لملء الحدود الدنيا والقصوى."
 
-#: widgets/waveform/waveform_widget.py:403
+#: widgets/waveform/waveform_widget.py:402
 msgid "lines"
 msgstr "الخطوط"
 
-#: widgets/waveform/waveform_widget.py:404
+#: widgets/waveform/waveform_widget.py:403
 msgid "fill 1"
 msgstr "ملء 1"
 
-#: widgets/waveform/waveform_widget.py:405
+#: widgets/waveform/waveform_widget.py:404
 msgid "fill 2"
 msgstr "ملء 2"
 
-#: widgets/waveform/waveform_widget.py:411
+#: widgets/waveform/waveform_widget.py:410
 msgid "Show the frames per second."
 msgstr "عرض الإطارات في الثانية."
 
-#: widgets/waveform/waveform_widget.py:416
+#: widgets/waveform/waveform_widget.py:415
 msgid "Show the statistics on mouse hover."
 msgstr "عرض الإحصائيات عند تحريك الماوس."
 
-#: widgets/waveform/waveform_widget.py:421
+#: widgets/waveform/waveform_widget.py:420
 msgid "Show the plot statistics on the right."
 msgstr "عرض إحصائيات الرسم على اليمين."
 
-#: widgets/waveform/waveform_widget.py:426
+#: widgets/waveform/waveform_widget.py:425
 msgid "Show frequency for dual markers and statistics."
 msgstr "عرض التردد للعلامات والإحصائيات المزدوجة."
 
-#: widgets/waveform/waveform_widget.py:431
+#: widgets/waveform/waveform_widget.py:430
 msgid "The quantities to display by default."
 msgstr "الكميات المراد عرضها افتراضيًا."
 
-#: widgets/waveform/waveform_widget.py:437
+#: widgets/waveform/waveform_widget.py:436
 msgid "The precision to display in digits."
 msgstr "دقة العرض بالأرقام."
 
-#: widgets/waveform/waveform_widget.py:443
+#: widgets/waveform/waveform_widget.py:442
 msgid "Use OpenGL rendering."
 msgstr "استخدم عرض OpenGL."
 
-#: widgets/waveform/waveform_widget.py:454
+#: widgets/waveform/waveform_widget.py:453
 msgid "Pin the left side (oldest) data so that it stays in view."
 msgstr "تثبيت بيانات الجانب الأيسر (الأقدم) بحيث تبقى في العرض."
 
-#: widgets/waveform/waveform_widget.py:459
+#: widgets/waveform/waveform_widget.py:458
 msgid "Pin the right side (newest) data so that it stays in view."
 msgstr "تثبيت بيانات الجانب الأيمن (الأحدث) بحيث تبقى في العرض."
 
-#: widgets/waveform/waveform_widget.py:464
+#: widgets/waveform/waveform_widget.py:463
 msgid "The waveform state."
 msgstr "حالة الشكل الموجي."
 
-#: widgets/waveform/waveform_widget.py:470
+#: widgets/waveform/waveform_widget.py:469
 msgid "The annotations."
 msgstr "الشروح"
 
-#: widgets/waveform/waveform_widget.py:476
+#: widgets/waveform/waveform_widget.py:475
 msgid "Control location"
 msgstr "موقع التحكم"
 
-#: widgets/waveform/waveform_widget.py:480
+#: widgets/waveform/waveform_widget.py:479
 msgid "top"
 msgstr "أعلى"
 
-#: widgets/waveform/waveform_widget.py:481
+#: widgets/waveform/waveform_widget.py:480
 msgid "bottom"
 msgstr "القاع"
 
-#: widgets/waveform/waveform_widget.py:486
+#: widgets/waveform/waveform_widget.py:485
 msgid "The signal quantity to show in the summary."
 msgstr "كمية الإشارة المراد إظهارها في الملخص."
 
-#: widgets/waveform/waveform_widget.py:492
+#: widgets/waveform/waveform_widget.py:491
 msgid "X-axis annotation mode"
 msgstr "وضع التعليق التوضيحي للمحور X"
 
-#: widgets/waveform/waveform_widget.py:495
-#: widgets/waveform/waveform_widget.py:2888
+#: widgets/waveform/waveform_widget.py:494
+#: widgets/waveform/waveform_widget.py:2930
 msgid "Absolute"
 msgstr "المطلق"
 
-#: widgets/waveform/waveform_widget.py:496
-#: widgets/waveform/waveform_widget.py:2893
+#: widgets/waveform/waveform_widget.py:495
+#: widgets/waveform/waveform_widget.py:2935
 msgid "Relative"
 msgstr "نسبي"
 
-#: widgets/waveform/waveform_widget.py:502
+#: widgets/waveform/waveform_widget.py:501
 msgid "The available subsources."
 msgstr "المصادر الفرعية المتاحة."
 
-#: widgets/waveform/waveform_widget.py:508
+#: widgets/waveform/waveform_widget.py:507
 msgid "The selected subsources for each trace."
 msgstr "المصادر الفرعية المختارة لكل تتبع."
 
-#: widgets/waveform/waveform_widget.py:514
+#: widgets/waveform/waveform_widget.py:513
 msgid "The trace priority: highest int value on top, None is off."
 msgstr "أولوية التتبع: أعلى قيمة للتيار في الأعلى، لا شيء متوقف."
 
-#: widgets/waveform/waveform_widget.py:2834
-#: widgets/waveform/waveform_widget.py:3135
+#: widgets/waveform/waveform_widget.py:2877
+#: widgets/waveform/waveform_widget.py:3179
 msgid "Save image to file"
 msgstr "حفظ الصورة في ملف"
 
-#: widgets/waveform/waveform_widget.py:2882
-#: widgets/waveform/waveform_widget.py:2951
+#: widgets/waveform/waveform_widget.py:2924
+#: widgets/waveform/waveform_widget.py:2993
 msgid "Single marker"
 msgstr "علامة واحدة"
 
-#: widgets/waveform/waveform_widget.py:2883
-#: widgets/waveform/waveform_widget.py:2952
+#: widgets/waveform/waveform_widget.py:2925
+#: widgets/waveform/waveform_widget.py:2994
 msgid "Dual markers"
 msgstr "علامات مزدوجة"
 
-#: widgets/waveform/waveform_widget.py:2885
+#: widgets/waveform/waveform_widget.py:2927
 msgid "Mode"
 msgstr "الوضع"
 
-#: widgets/waveform/waveform_widget.py:2898
-#: widgets/waveform/waveform_widget.py:2953
-#: widgets/waveform/waveform_widget.py:3111
-#: widgets/waveform/waveform_widget.py:3129
+#: widgets/waveform/waveform_widget.py:2940
+#: widgets/waveform/waveform_widget.py:2995
+#: widgets/waveform/waveform_widget.py:3155
+#: widgets/waveform/waveform_widget.py:3173
 msgid "Clear all"
 msgstr "مسح الكل"
 
-#: widgets/waveform/waveform_widget.py:2909
-#: widgets/waveform/waveform_widget.py:2998
-#: widgets/waveform/waveform_widget.py:3117
+#: widgets/waveform/waveform_widget.py:2951
+#: widgets/waveform/waveform_widget.py:3040
+#: widgets/waveform/waveform_widget.py:3161
 msgid "Annotations"
 msgstr "التعليقات التوضيحية"
 
-#: widgets/waveform/waveform_widget.py:3001
+#: widgets/waveform/waveform_widget.py:3043
 msgid "Range"
 msgstr "النطاق"
 
-#: widgets/waveform/waveform_widget.py:3005
-#: widgets/waveform/waveform_widget.py:3328
+#: widgets/waveform/waveform_widget.py:3047
+#: widgets/waveform/waveform_widget.py:3378
 msgid "Auto"
 msgstr "تلقائي"
 
-#: widgets/waveform/waveform_widget.py:3011
+#: widgets/waveform/waveform_widget.py:3053
 msgid "Exact"
 msgstr "دقيق"
 
-#: widgets/waveform/waveform_widget.py:3020
+#: widgets/waveform/waveform_widget.py:3062
 msgid "Scale"
 msgstr "المقياس"
 
-#: widgets/waveform/waveform_widget.py:3023
+#: widgets/waveform/waveform_widget.py:3065
 msgid "Linear"
 msgstr "الخطي"
 
-#: widgets/waveform/waveform_widget.py:3028
+#: widgets/waveform/waveform_widget.py:3070
 msgid "Logarithmic"
 msgstr "لوغاريتمي"
 
-#: widgets/waveform/waveform_widget.py:3036
+#: widgets/waveform/waveform_widget.py:3078
 msgid "Logarithmic zero"
 msgstr "الصفر اللوغاريتمي"
 
-#: widgets/waveform/waveform_widget.py:3050
+#: widgets/waveform/waveform_widget.py:3092
 msgid "Preferred prefix"
 msgstr "البادئة المفضلة"
 
-#: widgets/waveform/waveform_widget.py:3108
+#: widgets/waveform/waveform_widget.py:3152
 msgid "Add"
 msgstr "إضافة"
 
-#: widgets/waveform/waveform_widget.py:3109
+#: widgets/waveform/waveform_widget.py:3153
 msgid "Hide all text"
 msgstr "إخفاء كل النص"
 
-#: widgets/waveform/waveform_widget.py:3110
+#: widgets/waveform/waveform_widget.py:3154
 msgid "Show all text"
 msgstr "إظهار كل النص"
 
-#: widgets/waveform/waveform_widget.py:3118
+#: widgets/waveform/waveform_widget.py:3162
 msgid "Vertical"
 msgstr "عمودي"
 
-#: widgets/waveform/waveform_widget.py:3121
+#: widgets/waveform/waveform_widget.py:3165
 msgid "Horizontal"
 msgstr "أفقي"
 
-#: widgets/waveform/waveform_widget.py:3127
+#: widgets/waveform/waveform_widget.py:3171
 msgid "Save"
 msgstr "حفظ"
 
-#: widgets/waveform/waveform_widget.py:3132
+#: widgets/waveform/waveform_widget.py:3176
 msgid "Y-axis auto range"
 msgstr "النطاق التلقائي للمحور Y"
 
-#: widgets/waveform/waveform_widget.py:3136
+#: widgets/waveform/waveform_widget.py:3180
 msgid "Copy image to clipboard"
 msgstr "نسخ الصورة إلى الحافظة"
 
-#: widgets/waveform/waveform_widget.py:3137
+#: widgets/waveform/waveform_widget.py:3181
 msgid "Export visible data"
 msgstr "تصدير البيانات المرئية"
 
-#: widgets/waveform/waveform_widget.py:3138
+#: widgets/waveform/waveform_widget.py:3182
 msgid "Export all data"
 msgstr "تصدير جميع البيانات"
 
-#: widgets/waveform/waveform_widget.py:3304
+#: widgets/waveform/waveform_widget.py:3354
 msgid "Export"
 msgstr "التصدير"
 
-#: widgets/waveform/waveform_widget.py:3305
+#: widgets/waveform/waveform_widget.py:3355
 msgid "Analysis"
 msgstr "التحليل"
 
-#: widgets/waveform/waveform_widget.py:3313
+#: widgets/waveform/waveform_widget.py:3363
 msgid "Interval"
 msgstr "الفاصل الزمني"
 
-#: widgets/waveform/waveform_widget.py:3322
+#: widgets/waveform/waveform_widget.py:3372
 msgid "Zoom"
 msgstr "تكبير"
 
-#: widgets/waveform/waveform_widget.py:3326
+#: widgets/waveform/waveform_widget.py:3376
 msgid "Show statistics"
 msgstr "عرض الإحصائيات"
 
-#: widgets/waveform/waveform_widget.py:3331
+#: widgets/waveform/waveform_widget.py:3381
 msgid "Left"
 msgstr "يسار"
 
-#: widgets/waveform/waveform_widget.py:3334
+#: widgets/waveform/waveform_widget.py:3384
 msgid "Right"
 msgstr "صحيح"
 
-#: widgets/waveform/waveform_widget.py:3337
+#: widgets/waveform/waveform_widget.py:3387
 msgid "Off"
 msgstr "إيقاف التشغيل"
 
-#: widgets/waveform/waveform_widget.py:3340
-#: widgets/waveform/waveform_widget.py:3368
-#: widgets/waveform/waveform_widget.py:3397
+#: widgets/waveform/waveform_widget.py:3390
+#: widgets/waveform/waveform_widget.py:3418
+#: widgets/waveform/waveform_widget.py:3448
 msgid "Remove"
 msgstr "إزالة"
 
-#: widgets/waveform/waveform_widget.py:3351
+#: widgets/waveform/waveform_widget.py:3401
 msgid "Y mode"
 msgstr "الوضع Y"
 
 #: widgets/waveform/y_range_widget.py:67
 msgid "max"
 msgstr "الحد الأقصى"
```

### Comparing `joulescope_ui-1.1.6/joulescope_ui/locale/de/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.7/joulescope_ui/locale/de/LC_MESSAGES/joulescope_ui.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.2\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-18 14:15-0400\n"
+"POT-Creation-Date: 2024-05-06 17:27-0400\n"
 "PO-Revision-Date: 2024-04-04 14:45-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: de\n"
 "Language-Team: de <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.14.0\n"
+"Generated-By: Babel 2.15.0\n"
 
 msgid "\"3.3 V\" uses an internally-generated 3.3V reference voltage."
 msgstr "\"3,3 V\" verwendet eine intern erzeugte 3,3-V-Referenzspannung."
 
 msgid "\"NaN\" sets all samples in the window to NaN."
 msgstr "\"NaN\" setzt alle Proben im Fenster auf NaN."
 
@@ -661,14 +661,17 @@
 msgid ""
 "Display the number of actions processed by the publish-subscribe broker in "
 "each second."
 msgstr ""
 "Zeigt die Anzahl der Aktionen an, die der Publish-Subscribe-Broker in jeder "
 "Sekunde verarbeitet."
 
+msgid "Divide the quantity by this value."
+msgstr "Teilen Sie die Größe durch diesen Wert."
+
 msgid "Do not show again"
 msgstr "Nicht mehr anzeigen"
 
 msgid "Do not use any USB hubs, docks or adapters"
 msgstr "Verwenden Sie keine USB-Hubs, -Docks oder -Adapter"
 
 msgid "Dual markers"
@@ -1796,14 +1799,21 @@
 msgstr ""
 "Die angezeigten Werte werden normalerweise mit jeder neuen, vom Gerät "
 "berechneten Statistik aktualisiert. Wenn diese Schaltfläche ausgewählt ist, "
 "wird die Anzeige nicht aktualisiert. Die Statistiken werden jedoch weiterhin "
 "akkumuliert und auflaufen (falls ausgewählt)."
 
 msgid ""
+"The divisor is a floating point number. The number may optionally be "
+"followed by units."
+msgstr ""
+"Der Divisor ist eine Gleitkommazahl. Die Zahl kann optional von Einheiten "
+"gefolgt werden."
+
+msgid ""
 "The exponential decay time constant. The fuse dissipates 63.2 percent of "
 "accumulated energy in this duration."
 msgstr ""
 "Die exponentielle Abklingzeitkonstante. In dieser Zeitspanne baut die "
 "Sicherung 63,2 Prozent der angesammelten Energie ab."
 
 msgid "The filename supports the following replacements."
@@ -1811,17 +1821,14 @@
 
 msgid "The filename with optional replacements."
 msgstr "Der Dateiname mit optionalen Ersetzungen."
 
 msgid "The fixed default path for loading and saving files."
 msgstr "Der feste Standardpfad für das Laden und Speichern von Dateien."
 
-msgid "The flyout width in pixels."
-msgstr "Die Breite des Flyouts in Pixeln."
-
 msgid "The font scheme name."
 msgstr "Der Name des Schriftschemas."
 
 msgid "The format string"
 msgstr "Der Formatstring"
 
 msgid "The fuse trips in Duration at this constant current."
```

### Comparing `joulescope_ui-1.1.6/joulescope_ui/locale/de/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.7/joulescope_ui/locale/de/LC_MESSAGES/joulescope_ui.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.2\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-18 14:15-0400\n"
+"POT-Creation-Date: 2024-05-06 17:27-0400\n"
 "PO-Revision-Date: 2024-04-04 14:45-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: de <LL@li.org>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-"Generated-By: Babel 2.14.0\n"
+"Generated-By: Babel 2.15.0\n"
 
 #: about.py:24
 msgid "About the Joulescope UI"
 msgstr "Über die Joulescope-Benutzeroberfläche"
 
 #: about.py:25
 msgid "Version Information"
@@ -334,27 +334,27 @@
 msgid "Email"
 msgstr "E-Mail"
 
 #: error_window.py:103
 msgid "Description"
 msgstr "Beschreibung"
 
-#: error_window.py:112 widgets/waveform/waveform_widget.py:3347
+#: error_window.py:112 widgets/waveform/waveform_widget.py:3397
 msgid "Edit"
 msgstr "Bearbeiten"
 
 #: error_window.py:113
 msgid "View as Markdown"
 msgstr "Als Markdown anzeigen"
 
 #: error_window.py:119
 msgid "Abort"
 msgstr "Abbruch"
 
-#: error_window.py:120 main.py:365 widgets/settings/settings_widget.py:539
+#: error_window.py:120 main.py:363 widgets/settings/settings_widget.py:539
 msgid "View"
 msgstr "Siehe"
 
 #: error_window.py:121
 msgid "Submit"
 msgstr "einreichen"
 
@@ -366,15 +366,15 @@
 msgid "Revert to previous configuration"
 msgstr "Zur vorherigen Konfiguration zurückkehren"
 
 #: error_window.py:282
 msgid "Revert to defaults"
 msgstr "Zu Standardeinstellungen zurückkehren"
 
-#: error_window.py:283 main.py:363 main.py:409
+#: error_window.py:283 main.py:361 main.py:407
 #: widgets/js220_cal/js220_cal_widget.py:38
 msgid "Exit"
 msgstr "Ausfahrt"
 
 #: exporter.py:49 widgets/signal_record/signal_record_config_widget.py:148
 #: widgets/statistics_record/statistics_record_config_widget.py:111
 msgid "Directory"
@@ -644,164 +644,164 @@
 msgid "Do not show again"
 msgstr "Nicht mehr anzeigen"
 
 #: intel_graphics_dialog.py:91
 msgid "Intel graphics detected"
 msgstr "Intel-Grafik erkannt"
 
-#: main.py:70 widgets/value/value_widget.py:653
+#: main.py:69 widgets/value/value_widget.py:660
 msgid "Multimeter"
 msgstr "Multimeter"
 
-#: main.py:71
+#: main.py:70
 msgid "Oscilloscope"
 msgstr "Oszilloskop"
 
-#: main.py:72 main.py:298 main.py:359 main.py:402
+#: main.py:71 main.py:296 main.py:357 main.py:400
 msgid "File"
 msgstr "Datei"
 
-#: main.py:82
+#: main.py:81
 msgid "The UI status bar display mode"
 msgstr "Der UI-Statusleisten-Anzeigemodus"
 
-#: main.py:83
+#: main.py:82
 msgid ""
 "This setting controls the amount of detail shown on the status bar at the "
 "bottom of the UI window. You should usually leave this set to \"normal\" "
 "unless you want more detail concerning the UI internal operation."
 msgstr ""
 "Diese Einstellung steuert die Menge an Details, die in der Statusleiste am "
 "unteren Rand des UI-Fensters angezeigt werden. Normalerweise sollten Sie "
 "diese Einstellung auf \"normal\" belassen, es sei denn, Sie möchten mehr "
 "Details über den internen Betrieb der Benutzeroberfläche erfahren."
 
-#: main.py:88 safe_mode.py:43
+#: main.py:87 safe_mode.py:43
 msgid "Normal"
 msgstr "Normal"
 
-#: main.py:89
+#: main.py:88
 msgid "Troubleshoot"
 msgstr "Fehlersuche"
 
-#: main.py:95
+#: main.py:94
 msgid "Enable developer mode."
 msgstr "Aktivieren Sie den Entwicklermodus."
 
-#: main.py:108
+#: main.py:107
 msgid "PubSub utilization"
 msgstr "PubSub Nutzung"
 
-#: main.py:109
+#: main.py:108
 msgid ""
 "Display the number of actions processed by the publish-subscribe broker in "
 "each second."
 msgstr ""
 "Zeigt die Anzahl der Aktionen an, die der Publish-Subscribe-Broker in jeder "
 "Sekunde verarbeitet."
 
-#: main.py:114
+#: main.py:113
 msgid "CPU utilization"
 msgstr "CPU-Auslastung"
 
-#: main.py:115
+#: main.py:114
 msgid ""
 "Display the CPU utilization by this application and the total CPU "
 "utilization by all applications. The value is displayed in percent."
 msgstr ""
 "Zeigt die CPU-Auslastung durch diese Anwendung und die gesamte CPU-"
 "Auslastung durch alle Anwendungen an. Der Wert wird in Prozent angezeigt."
 
-#: main.py:121
+#: main.py:120
 msgid "Memory utilization"
 msgstr "Speicherauslastung"
 
-#: main.py:122
+#: main.py:121
 msgid ""
 "Display the memory (RAM) utilization by this application and by all "
 "applications. The value is displayed in percent."
 msgstr ""
 "Zeigt die Speicherauslastung (RAM) durch diese Anwendung und durch alle "
 "Anwendungen an. Der Wert wird in Prozent angezeigt."
 
-#: main.py:216
+#: main.py:214
 msgid "UI"
 msgstr "UI"
 
-#: main.py:330
+#: main.py:328
 msgid "Help"
 msgstr "Hilfe"
 
-#: main.py:331 widgets/hamburger/hamburger_widget.py:21
+#: main.py:329 widgets/hamburger/hamburger_widget.py:21
 msgid "Getting Started"
 msgstr "Erste Schritte"
 
-#: main.py:332
+#: main.py:330
 msgid "User's Guide"
 msgstr "Benutzerhandbuch"
 
-#: main.py:333 widgets/hamburger/hamburger_widget.py:22
+#: main.py:331 widgets/hamburger/hamburger_widget.py:22
 msgid "Changelog"
 msgstr "Changelog"
 
-#: main.py:334 widgets/help/help_widget.py:59
+#: main.py:332 widgets/help/help_widget.py:59
 msgid "Report Issue"
 msgstr "Bericht Ausgabe"
 
-#: main.py:335
+#: main.py:333
 msgid "View logs..."
 msgstr "Protokolle anzeigen..."
 
-#: main.py:336 widgets/hamburger/hamburger_widget.py:23
+#: main.py:334 widgets/hamburger/hamburger_widget.py:23
 msgid "Credits"
 msgstr "Credits"
 
-#: main.py:337 widgets/hamburger/hamburger_widget.py:24
+#: main.py:335 widgets/hamburger/hamburger_widget.py:24
 msgid "About"
 msgstr "Über"
 
-#: main.py:360
+#: main.py:358
 msgid "Open"
 msgstr "Öffnen Sie"
 
-#: main.py:361
+#: main.py:359
 msgid "Open recent"
 msgstr "Zuletzt geöffnet"
 
-#: main.py:362 main.py:408
+#: main.py:360 main.py:406
 msgid "Clear config and exit"
 msgstr "Konfiguration löschen und beenden"
 
-#: main.py:366 widgets/settings/settings_widget.py:541
+#: main.py:364 widgets/settings/settings_widget.py:541
 msgid "Widgets"
 msgstr "Widgets"
 
-#: main.py:367
+#: main.py:365
 msgid "Tools"
 msgstr "Werkzeuge"
 
-#: main.py:368
+#: main.py:366
 msgid "Clear Accumulators"
 msgstr "Klare Akkumulatoren"
 
-#: main.py:403
+#: main.py:401
 msgid "Info"
 msgstr "Info"
 
-#: main.py:404 widget_tools.py:92 widgets/settings/settings_widget.py:31
+#: main.py:402 widget_tools.py:92 widgets/settings/settings_widget.py:31
 #: widgets/settings/settings_widget.py:574
 #: widgets/sidebar/sidebar_widget.py:41
 msgid "Settings"
 msgstr "Einstellungen"
 
-#: main.py:693
+#: main.py:710
 msgid "Manage"
 msgstr "Verwalten Sie"
 
-#: main.py:730
+#: main.py:747
 msgid "Select file to open"
 msgstr "Datei zum Öffnen auswählen"
 
 #: paths.py:30 styles/manager.py:46
 msgid "The name for this widget."
 msgstr "Der Name für dieses Widget."
 
@@ -943,47 +943,47 @@
 msgid "Source"
 msgstr "Quelle"
 
 #: units.py:35
 msgid "Use the application defaults"
 msgstr "Verwenden Sie die Standardeinstellungen der Anwendung"
 
-#: view.py:68
+#: view.py:72
 msgid "The active theme."
 msgstr "Das aktive Thema."
 
-#: view.py:70
+#: view.py:74
 msgid "Joulescope standard theme"
 msgstr "Joulescope Standardthema"
 
-#: view.py:70
+#: view.py:74
 msgid "System OS-specific theme"
 msgstr "System OS-spezifisches Thema"
 
-#: view.py:75
+#: view.py:79
 msgid "The color scheme name."
 msgstr "Der Name des Farbschemas."
 
-#: view.py:77
+#: view.py:81
 msgid "Dark background"
 msgstr "Dunkler Hintergrund"
 
-#: view.py:77
+#: view.py:81
 msgid "Light background"
 msgstr "Leichter Hintergrund"
 
-#: view.py:81
+#: view.py:85
 msgid "The font scheme name."
 msgstr "Der Name des Schriftschemas."
 
-#: view.py:83
+#: view.py:87
 msgid "Joulescope standard font theme"
 msgstr "Joulescope Standard-Schriftthema"
 
-#: view.py:102 widgets/view_manager/view_manager_widget.py:146
+#: view.py:106 widgets/view_manager/view_manager_widget.py:146
 msgid "New View"
 msgstr "Neue Ansicht"
 
 #: zip_inspector.py:23
 msgid "ZIP Inspector"
 msgstr "ZIP-Prüfer"
 
@@ -1102,15 +1102,15 @@
 "Wenn aktiviert, fließt Strom zwischen den Stromanschlüssen. Wenn er "
 "deaktiviert ist, kann kein Strom zwischen den Stromanschlüssen fließen. In "
 "gängigen Systemkonfigurationen wird dadurch die Stromversorgung des "
 "Zielgeräts unterbrochen, was zum Zurücksetzen des Zielgeräts durch einen "
 "Stromzyklus verwendet werden kann."
 
 #: devices/jsdrv/js110.py:147 devices/jsdrv/js220.py:163
-#: widgets/waveform/waveform_widget.py:110
+#: widgets/waveform/waveform_widget.py:109
 msgid "Current range"
 msgstr "Strombereich"
 
 #: devices/jsdrv/js110.py:149
 msgid ""
 "Configure the J110's current range. Most applications should use the "
 "default, \"auto\"."
@@ -1259,33 +1259,33 @@
 "mean. This value is ignored for all other IRF types."
 msgstr ""
 "Die Anzahl der Abtastungen nach dem Strombereichsfenster, die zur Bestimmung"
 " des Mittelwerts verwendet wird. Dieser Wert wird für alle anderen IRF-Typen"
 " ignoriert."
 
 #: devices/jsdrv/js110.py:269 devices/jsdrv/js220.py:332
-#: widgets/device_control/fuse.py:103 widgets/waveform/waveform_widget.py:105
+#: widgets/device_control/fuse.py:103 widgets/waveform/waveform_widget.py:104
 msgid "Current"
 msgstr "Strom"
 
 #: devices/jsdrv/js110.py:270 devices/jsdrv/js220.py:333
 msgid "Enable the current signal streaming."
 msgstr "Aktivieren Sie das Stromsignal-Streaming."
 
 #: devices/jsdrv/js110.py:278 devices/jsdrv/js220.py:341
-#: widgets/waveform/waveform_widget.py:106
+#: widgets/waveform/waveform_widget.py:105
 msgid "Voltage"
 msgstr "Voltage"
 
 #: devices/jsdrv/js110.py:279 devices/jsdrv/js220.py:342
 msgid "Enable the voltage signal streaming."
 msgstr "Aktivieren Sie das Streaming von Spannungssignalen."
 
 #: devices/jsdrv/js110.py:287 devices/jsdrv/js220.py:350
-#: widgets/waveform/waveform_widget.py:107
+#: widgets/waveform/waveform_widget.py:106
 msgid "Power"
 msgstr "Strom"
 
 #: devices/jsdrv/js110.py:288 devices/jsdrv/js220.py:351
 msgid "Enable the power signal streaming."
 msgstr "Aktivieren Sie das Stromsignal-Streaming."
 
@@ -1503,15 +1503,15 @@
 msgid "GPI 3"
 msgstr "GPI 3"
 
 #: devices/jsdrv/js220.py:402
 msgid "Enable the general purpose input 3 signal streaming."
 msgstr "Aktivieren Sie den Allzweckeingang 3 Signalstreaming."
 
-#: devices/jsdrv/js220.py:410 widgets/waveform/waveform_widget.py:124
+#: devices/jsdrv/js220.py:410 widgets/waveform/waveform_widget.py:123
 msgid "Trigger input"
 msgstr "Trigger-Eingang"
 
 #: devices/jsdrv/js220.py:411
 msgid "Enable the trigger input signal streaming."
 msgstr "Aktivieren Sie das Streaming des Trigger-Eingangssignals."
 
@@ -1522,15 +1522,15 @@
 #: devices/jsdrv/jsdrv_stream_buffer.py:44
 #: devices/jsdrv/jsdrv_stream_buffer.py:93
 #: devices/jsdrv/jsdrv_stream_buffer.py:107 plugins/selector.py:58
 #: widgets/settings/settings_widget.py:85
 #: widgets/settings/settings_widget.py:266
 #: widgets/settings/settings_widget.py:364
 #: widgets/settings/settings_widget.py:431
-#: widgets/waveform/waveform_widget.py:3062
+#: widgets/waveform/waveform_widget.py:3104
 msgid "Name"
 msgstr "Name"
 
 #: devices/jsdrv/jsdrv_stream_buffer.py:45
 msgid "Joulescope stream buffer"
 msgstr "Joulescope Strompuffer"
 
@@ -1754,15 +1754,15 @@
 
 #: widgets/accumulator/accumulator_widget.py:27
 #: widgets/value/value_widget.py:31
 msgid "The statistics data stream source."
 msgstr "Die Statistik-Datenstromquelle."
 
 #: widgets/accumulator/accumulator_widget.py:32
-#: widgets/value/value_widget.py:74
+#: widgets/value/value_widget.py:81
 msgid "The signal to display."
 msgstr "Das anzuzeigende Signal."
 
 #: widgets/accumulator/accumulator_widget.py:34
 msgid "charge"
 msgstr "Ladung"
 
@@ -1845,15 +1845,15 @@
 
 #: widgets/developer/publish_spy_widget.py:20
 #: widgets/developer/publish_spy_widget.py:21
 msgid "Topic"
 msgstr "Thema"
 
 #: widgets/developer/publish_spy_widget.py:21
-#: widgets/settings/settings_widget.py:87 widgets/value/value_widget.py:662
+#: widgets/settings/settings_widget.py:87 widgets/value/value_widget.py:669
 msgid "Value"
 msgstr "Wert"
 
 #: widgets/developer/publish_spy_widget.py:24
 msgid "Publish Spy"
 msgstr "Spion veröffentlichen"
 
@@ -1883,15 +1883,15 @@
 
 #: widgets/device_control/device_update_dialog.py:24
 #: widgets/device_control/device_update_dialog.py:45
 msgid "Update"
 msgstr "aktualisieren"
 
 #: widgets/device_control/device_update_dialog.py:25
-#: widgets/value/value_widget.py:147
+#: widgets/value/value_widget.py:155
 msgid "Device"
 msgstr "Gerät"
 
 #: widgets/device_control/device_update_dialog.py:27
 #: widgets/progress_bar/progress_bar_widget.py:59
 msgid "Progress"
 msgstr "Fortschritt"
@@ -2425,18 +2425,14 @@
 msgid "Click to display additional settings and actions."
 msgstr "Klicken Sie, um zusätzliche Einstellungen und Aktionen anzuzeigen."
 
 #: widgets/sidebar/sidebar_widget.py:60
 msgid "sidebar"
 msgstr "Seitenleiste"
 
-#: widgets/sidebar/sidebar_widget.py:68
-msgid "The flyout width in pixels."
-msgstr "Die Breite des Flyouts in Pixeln."
-
 #: widgets/signal_record/disk_full_dialog.py:19
 msgid "The disk is full"
 msgstr "Die Festplatte ist voll"
 
 #: widgets/signal_record/signal_record.py:57
 msgid "Could not open file for write"
 msgstr "Datei konnte nicht zum Schreiben geöffnet werden"
@@ -2463,15 +2459,15 @@
 msgid "StatisticsRecordConfig"
 msgstr "StatistikRecordConfig"
 
 #: widgets/statistics_record/statistics_record_config_widget.py:123
 msgid "Time Format"
 msgstr "Zeitformat"
 
-#: widgets/trigger/trigger_widget.py:41 widgets/value/value_widget.py:87
+#: widgets/trigger/trigger_widget.py:41 widgets/value/value_widget.py:94
 msgid "Select the source device"
 msgstr "Wählen Sie das Quellgerät"
 
 #: widgets/trigger/trigger_widget.py:42
 msgid "The device to use for the start condition and stop condition."
 msgstr ""
 "Das Gerät, das für die Startbedingung und die Stoppbedingung zu verwenden "
@@ -2648,86 +2644,98 @@
 msgid "Show the statistics fields at the right."
 msgstr "Zeigen Sie die Statistikfelder auf der rechten Seite an."
 
 #: widgets/value/value_widget.py:51
 msgid "Show a leading + or - sign."
 msgstr "Zeigt ein führendes + oder - Zeichen."
 
-#: widgets/value/value_widget.py:88
+#: widgets/value/value_widget.py:62
+msgid "Divide the quantity by this value."
+msgstr "Teilen Sie die Größe durch diesen Wert."
+
+#: widgets/value/value_widget.py:63
+msgid ""
+"The divisor is a floating point number. The number may optionally be "
+"followed by units."
+msgstr ""
+"Der Divisor ist eine Gleitkommazahl. Die Zahl kann optional von Einheiten "
+"gefolgt werden."
+
+#: widgets/value/value_widget.py:95
 msgid ""
 "The values displayed by this widget come from a single source device. Select"
 " the source device here."
 msgstr ""
 "Die von diesem Widget angezeigten Werte stammen von einem einzigen "
 "Quellgerät. Wählen Sie hier das Quellgerät aus."
 
-#: widgets/value/value_widget.py:94
+#: widgets/value/value_widget.py:101
 msgid "Hold the display"
 msgstr "Halten Sie das Display"
 
-#: widgets/value/value_widget.py:96
+#: widgets/value/value_widget.py:103
 msgid "When selected, prevent the display from updating."
 msgstr "Wenn ausgewählt, wird die Aktualisierung der Anzeige verhindert."
 
-#: widgets/value/value_widget.py:97
+#: widgets/value/value_widget.py:104
 msgid ""
 "The UI also includes a global statistics hold button on the sidebar. When "
 "the global statistics hold button is selected, this button is disabled and "
 "has no effect."
 msgstr ""
 "Die Benutzeroberfläche enthält auch eine Schaltfläche zum Halten globaler "
 "Statistiken in der Seitenleiste. Wenn die Schaltfläche \"Globale Statistik "
 "halten\" ausgewählt ist, ist diese Schaltfläche deaktiviert und hat keine "
 "Wirkung."
 
-#: widgets/value/value_widget.py:100
+#: widgets/value/value_widget.py:107
 msgid ""
 "The displayed values normally update with each new statistics data computed "
 "by the device. When this button is selected, the display will not be "
 "updated. However, the statistics will continue accumulate and accrue (if "
 "selected)."
 msgstr ""
 "Die angezeigten Werte werden normalerweise mit jeder neuen, vom Gerät "
 "berechneten Statistik aktualisiert. Wenn diese Schaltfläche ausgewählt ist, "
 "wird die Anzeige nicht aktualisiert. Die Statistiken werden jedoch weiterhin"
 " akkumuliert und auflaufen (falls ausgewählt)."
 
-#: widgets/value/value_widget.py:107
+#: widgets/value/value_widget.py:114
 msgid "Accrue values over time"
 msgstr "Erfassen Sie Werte über die Zeit"
 
-#: widgets/value/value_widget.py:109
+#: widgets/value/value_widget.py:116
 msgid ""
 "Current, voltage, and power are normally computed over a single statistics "
 "frequency interval. Press this button to accrue the values indefinitely. "
 "Press again to return to normal operation."
 msgstr ""
 "Strom, Spannung und Leistung werden normalerweise über ein einziges "
 "statistisches Frequenzintervall berechnet. Drücken Sie diese Taste, um die "
 "Werte auf unbestimmte Zeit zu akkumulieren. Drücken Sie erneut, um zum "
 "normalen Betrieb zurückzukehren."
 
-#: widgets/value/value_widget.py:113
+#: widgets/value/value_widget.py:120
 msgid ""
 "Note that this button does not affect the charge and energy accumulation. "
 "Both accumulate indefinitely regardless of this button state."
 msgstr ""
 "Beachten Sie, dass diese Taste keinen Einfluss auf die Akkumulation von "
 "Ladung und Energie hat. Beide akkumulieren sich unabhängig vom Zustand "
 "dieser Taste auf unbestimmte Zeit."
 
-#: widgets/value/value_widget.py:195
+#: widgets/value/value_widget.py:203
 msgid "Not present"
 msgstr "Nicht vorhanden"
 
-#: widgets/value/value_widget.py:215
+#: widgets/value/value_widget.py:223
 msgid "Hold"
 msgstr "Halten"
 
-#: widgets/value/value_widget.py:223
+#: widgets/value/value_widget.py:231
 msgid "Accrue"
 msgstr "Beschleunigt"
 
 #: widgets/view_manager/view_manager_widget.py:108
 #: widgets/view_manager/view_manager_widget.py:174
 msgid "View Manager"
 msgstr "Ansicht Manager"
@@ -2773,34 +2781,34 @@
 msgstr "Dreieck rechts"
 
 #: widgets/waveform/text_annotation.py:62
 msgid "triangle left"
 msgstr "Dreieck links"
 
 #: widgets/waveform/text_annotation.py:66
-#: widgets/waveform/waveform_widget.py:3008
+#: widgets/waveform/waveform_widget.py:3050
 msgid "Manual"
 msgstr "Handbuch"
 
 #: widgets/waveform/text_annotation.py:67
 msgid "Centered"
 msgstr "Zentriert"
 
 #: widgets/waveform/text_annotation.py:99
-#: widgets/waveform/waveform_widget.py:3123
+#: widgets/waveform/waveform_widget.py:3167
 msgid "Text"
 msgstr "Text"
 
 #: widgets/waveform/text_annotation.py:107
-#: widgets/waveform/waveform_widget.py:3348
+#: widgets/waveform/waveform_widget.py:3398
 msgid "Show text"
 msgstr "Text anzeigen"
 
 #: widgets/waveform/text_annotation.py:116
-#: widgets/waveform/waveform_widget.py:3360
+#: widgets/waveform/waveform_widget.py:3410
 msgid "Shape"
 msgstr "Form"
 
 #: widgets/waveform/text_annotation.py:126
 msgid "Y Mode"
 msgstr "Y Mode"
 
@@ -3001,323 +3009,323 @@
 "\"default\" will use the default source which is normally configured using "
 "the Device Control widget."
 msgstr ""
 "\"default\" verwendet die Standardquelle, die normalerweise über das Device "
 "Control Widget konfiguriert wird."
 
 #: widgets/waveform/waveform_source_widget.py:104
-#: widgets/waveform/waveform_widget.py:402
-#: widgets/waveform/waveform_widget.py:479
+#: widgets/waveform/waveform_widget.py:401
+#: widgets/waveform/waveform_widget.py:478
 msgid "off"
 msgstr "aus"
 
-#: widgets/waveform/waveform_widget.py:44
+#: widgets/waveform/waveform_widget.py:43
 msgid "Waveform"
 msgstr "Wellenform"
 
-#: widgets/waveform/waveform_widget.py:120
+#: widgets/waveform/waveform_widget.py:119
 msgid "General purpose input 0"
 msgstr "Allzweck-Eingang 0"
 
-#: widgets/waveform/waveform_widget.py:121
+#: widgets/waveform/waveform_widget.py:120
 msgid "General purpose input 1"
 msgstr "Allzweck-Eingang 1"
 
-#: widgets/waveform/waveform_widget.py:122
+#: widgets/waveform/waveform_widget.py:121
 msgid "General purpose input 2"
 msgstr "Allzweck-Eingang 2"
 
-#: widgets/waveform/waveform_widget.py:123
+#: widgets/waveform/waveform_widget.py:122
 msgid "General purpose input 3"
 msgstr "Allzweck-Eingang 3"
 
-#: widgets/waveform/waveform_widget.py:358
+#: widgets/waveform/waveform_widget.py:357
 msgid "The source filter string."
 msgstr "Die Quellfilterkette."
 
-#: widgets/waveform/waveform_widget.py:369
+#: widgets/waveform/waveform_widget.py:368
 msgid "The trace width."
 msgstr "Die Leiterbahnbreite."
 
-#: widgets/waveform/waveform_widget.py:384
+#: widgets/waveform/waveform_widget.py:383
 msgid "The target frames per second."
 msgstr "Die angestrebten Bilder pro Sekunde."
 
-#: widgets/waveform/waveform_widget.py:386
+#: widgets/waveform/waveform_widget.py:385
 msgid "vsync"
 msgstr "vsync"
 
-#: widgets/waveform/waveform_widget.py:387
+#: widgets/waveform/waveform_widget.py:386
 msgid "20 Hz"
 msgstr "20 Hz"
 
-#: widgets/waveform/waveform_widget.py:388
+#: widgets/waveform/waveform_widget.py:387
 msgid "10 Hz"
 msgstr "10 Hz"
 
-#: widgets/waveform/waveform_widget.py:389
+#: widgets/waveform/waveform_widget.py:388
 msgid "5 Hz"
 msgstr "5 Hz"
 
-#: widgets/waveform/waveform_widget.py:395
+#: widgets/waveform/waveform_widget.py:394
 msgid "The minimum interval between repaint in milliseconds."
 msgstr ""
 "Das minimale Intervall zwischen den Wiederholungsmessungen in Millisekunden."
 
-#: widgets/waveform/waveform_widget.py:400
+#: widgets/waveform/waveform_widget.py:399
 msgid "Show the minimum and maximum extents fill."
 msgstr "Zeigt die minimale und maximale Ausdehnung an."
 
-#: widgets/waveform/waveform_widget.py:403
+#: widgets/waveform/waveform_widget.py:402
 msgid "lines"
 msgstr "Zeilen"
 
-#: widgets/waveform/waveform_widget.py:404
+#: widgets/waveform/waveform_widget.py:403
 msgid "fill 1"
 msgstr "Füllung 1"
 
-#: widgets/waveform/waveform_widget.py:405
+#: widgets/waveform/waveform_widget.py:404
 msgid "fill 2"
 msgstr "Füllung 2"
 
-#: widgets/waveform/waveform_widget.py:411
+#: widgets/waveform/waveform_widget.py:410
 msgid "Show the frames per second."
 msgstr "Zeigt die Bilder pro Sekunde an."
 
-#: widgets/waveform/waveform_widget.py:416
+#: widgets/waveform/waveform_widget.py:415
 msgid "Show the statistics on mouse hover."
 msgstr "Zeigen Sie die Statistik bei Mausbewegung an."
 
-#: widgets/waveform/waveform_widget.py:421
+#: widgets/waveform/waveform_widget.py:420
 msgid "Show the plot statistics on the right."
 msgstr "Zeigen Sie die Plot-Statistiken auf der rechten Seite an."
 
-#: widgets/waveform/waveform_widget.py:426
+#: widgets/waveform/waveform_widget.py:425
 msgid "Show frequency for dual markers and statistics."
 msgstr "Zeigt die Frequenz für duale Marker und Statistiken an."
 
-#: widgets/waveform/waveform_widget.py:431
+#: widgets/waveform/waveform_widget.py:430
 msgid "The quantities to display by default."
 msgstr "Die Größen, die standardmäßig angezeigt werden."
 
-#: widgets/waveform/waveform_widget.py:437
+#: widgets/waveform/waveform_widget.py:436
 msgid "The precision to display in digits."
 msgstr "Die Genauigkeit der Anzeige in Ziffern."
 
-#: widgets/waveform/waveform_widget.py:443
+#: widgets/waveform/waveform_widget.py:442
 msgid "Use OpenGL rendering."
 msgstr "Verwenden Sie OpenGL-Rendering."
 
-#: widgets/waveform/waveform_widget.py:454
+#: widgets/waveform/waveform_widget.py:453
 msgid "Pin the left side (oldest) data so that it stays in view."
 msgstr ""
 "Pinnen Sie die (ältesten) Daten auf der linken Seite an, damit sie im "
 "Blickfeld bleiben."
 
-#: widgets/waveform/waveform_widget.py:459
+#: widgets/waveform/waveform_widget.py:458
 msgid "Pin the right side (newest) data so that it stays in view."
 msgstr ""
 "Pinnen Sie die (neuesten) Daten auf der rechten Seite an, damit sie im "
 "Blickfeld bleiben."
 
-#: widgets/waveform/waveform_widget.py:464
+#: widgets/waveform/waveform_widget.py:463
 msgid "The waveform state."
 msgstr "Der Zustand der Wellenform."
 
-#: widgets/waveform/waveform_widget.py:470
+#: widgets/waveform/waveform_widget.py:469
 msgid "The annotations."
 msgstr "Die Anmerkungen."
 
-#: widgets/waveform/waveform_widget.py:476
+#: widgets/waveform/waveform_widget.py:475
 msgid "Control location"
 msgstr "Standort der Steuerung"
 
-#: widgets/waveform/waveform_widget.py:480
+#: widgets/waveform/waveform_widget.py:479
 msgid "top"
 msgstr "oben"
 
-#: widgets/waveform/waveform_widget.py:481
+#: widgets/waveform/waveform_widget.py:480
 msgid "bottom"
 msgstr "unten"
 
-#: widgets/waveform/waveform_widget.py:486
+#: widgets/waveform/waveform_widget.py:485
 msgid "The signal quantity to show in the summary."
 msgstr "Die Signalgröße, die in der Zusammenfassung angezeigt werden soll."
 
-#: widgets/waveform/waveform_widget.py:492
+#: widgets/waveform/waveform_widget.py:491
 msgid "X-axis annotation mode"
 msgstr "X-Achsen-Anmerkungsmodus"
 
-#: widgets/waveform/waveform_widget.py:495
-#: widgets/waveform/waveform_widget.py:2888
+#: widgets/waveform/waveform_widget.py:494
+#: widgets/waveform/waveform_widget.py:2930
 msgid "Absolute"
 msgstr "Absolut"
 
-#: widgets/waveform/waveform_widget.py:496
-#: widgets/waveform/waveform_widget.py:2893
+#: widgets/waveform/waveform_widget.py:495
+#: widgets/waveform/waveform_widget.py:2935
 msgid "Relative"
 msgstr "Relativ"
 
-#: widgets/waveform/waveform_widget.py:502
+#: widgets/waveform/waveform_widget.py:501
 msgid "The available subsources."
 msgstr "Die verfügbaren Teilquellen."
 
-#: widgets/waveform/waveform_widget.py:508
+#: widgets/waveform/waveform_widget.py:507
 msgid "The selected subsources for each trace."
 msgstr "Die ausgewählten Teilquellen für jede Messkurve."
 
-#: widgets/waveform/waveform_widget.py:514
+#: widgets/waveform/waveform_widget.py:513
 msgid "The trace priority: highest int value on top, None is off."
 msgstr ""
 "Die Priorität der Messkurve: Der höchste int-Wert steht oben, None ist aus."
 
-#: widgets/waveform/waveform_widget.py:2834
-#: widgets/waveform/waveform_widget.py:3135
+#: widgets/waveform/waveform_widget.py:2877
+#: widgets/waveform/waveform_widget.py:3179
 msgid "Save image to file"
 msgstr "Bild in Datei speichern"
 
-#: widgets/waveform/waveform_widget.py:2882
-#: widgets/waveform/waveform_widget.py:2951
+#: widgets/waveform/waveform_widget.py:2924
+#: widgets/waveform/waveform_widget.py:2993
 msgid "Single marker"
 msgstr "Einzelner Marker"
 
-#: widgets/waveform/waveform_widget.py:2883
-#: widgets/waveform/waveform_widget.py:2952
+#: widgets/waveform/waveform_widget.py:2925
+#: widgets/waveform/waveform_widget.py:2994
 msgid "Dual markers"
 msgstr "Zwei Marker"
 
-#: widgets/waveform/waveform_widget.py:2885
+#: widgets/waveform/waveform_widget.py:2927
 msgid "Mode"
 msgstr "Modus"
 
-#: widgets/waveform/waveform_widget.py:2898
-#: widgets/waveform/waveform_widget.py:2953
-#: widgets/waveform/waveform_widget.py:3111
-#: widgets/waveform/waveform_widget.py:3129
+#: widgets/waveform/waveform_widget.py:2940
+#: widgets/waveform/waveform_widget.py:2995
+#: widgets/waveform/waveform_widget.py:3155
+#: widgets/waveform/waveform_widget.py:3173
 msgid "Clear all"
 msgstr "Alles löschen"
 
-#: widgets/waveform/waveform_widget.py:2909
-#: widgets/waveform/waveform_widget.py:2998
-#: widgets/waveform/waveform_widget.py:3117
+#: widgets/waveform/waveform_widget.py:2951
+#: widgets/waveform/waveform_widget.py:3040
+#: widgets/waveform/waveform_widget.py:3161
 msgid "Annotations"
 msgstr "Anmerkungen"
 
-#: widgets/waveform/waveform_widget.py:3001
+#: widgets/waveform/waveform_widget.py:3043
 msgid "Range"
 msgstr "Range"
 
-#: widgets/waveform/waveform_widget.py:3005
-#: widgets/waveform/waveform_widget.py:3328
+#: widgets/waveform/waveform_widget.py:3047
+#: widgets/waveform/waveform_widget.py:3378
 msgid "Auto"
 msgstr "Auto"
 
-#: widgets/waveform/waveform_widget.py:3011
+#: widgets/waveform/waveform_widget.py:3053
 msgid "Exact"
 msgstr "Genau"
 
-#: widgets/waveform/waveform_widget.py:3020
+#: widgets/waveform/waveform_widget.py:3062
 msgid "Scale"
 msgstr "Skala"
 
-#: widgets/waveform/waveform_widget.py:3023
+#: widgets/waveform/waveform_widget.py:3065
 msgid "Linear"
 msgstr "Linear"
 
-#: widgets/waveform/waveform_widget.py:3028
+#: widgets/waveform/waveform_widget.py:3070
 msgid "Logarithmic"
 msgstr "Logarithmisch"
 
-#: widgets/waveform/waveform_widget.py:3036
+#: widgets/waveform/waveform_widget.py:3078
 msgid "Logarithmic zero"
 msgstr "Logarithmischer Nullpunkt"
 
-#: widgets/waveform/waveform_widget.py:3050
+#: widgets/waveform/waveform_widget.py:3092
 msgid "Preferred prefix"
 msgstr "Bevorzugte Vorsilbe"
 
-#: widgets/waveform/waveform_widget.py:3108
+#: widgets/waveform/waveform_widget.py:3152
 msgid "Add"
 msgstr "hinzufügen"
 
-#: widgets/waveform/waveform_widget.py:3109
+#: widgets/waveform/waveform_widget.py:3153
 msgid "Hide all text"
 msgstr "Alle Texte ausblenden"
 
-#: widgets/waveform/waveform_widget.py:3110
+#: widgets/waveform/waveform_widget.py:3154
 msgid "Show all text"
 msgstr "Alle Texte anzeigen"
 
-#: widgets/waveform/waveform_widget.py:3118
+#: widgets/waveform/waveform_widget.py:3162
 msgid "Vertical"
 msgstr "Vertikal"
 
-#: widgets/waveform/waveform_widget.py:3121
+#: widgets/waveform/waveform_widget.py:3165
 msgid "Horizontal"
 msgstr "Horizontal"
 
-#: widgets/waveform/waveform_widget.py:3127
+#: widgets/waveform/waveform_widget.py:3171
 msgid "Save"
 msgstr "Speichern Sie"
 
-#: widgets/waveform/waveform_widget.py:3132
+#: widgets/waveform/waveform_widget.py:3176
 msgid "Y-axis auto range"
 msgstr "Automatischer Bereich der Y-Achse"
 
-#: widgets/waveform/waveform_widget.py:3136
+#: widgets/waveform/waveform_widget.py:3180
 msgid "Copy image to clipboard"
 msgstr "Bild in die Zwischenablage kopieren"
 
-#: widgets/waveform/waveform_widget.py:3137
+#: widgets/waveform/waveform_widget.py:3181
 msgid "Export visible data"
 msgstr "Sichtbare Daten exportieren"
 
-#: widgets/waveform/waveform_widget.py:3138
+#: widgets/waveform/waveform_widget.py:3182
 msgid "Export all data"
 msgstr "Alle Daten exportieren"
 
-#: widgets/waveform/waveform_widget.py:3304
+#: widgets/waveform/waveform_widget.py:3354
 msgid "Export"
 msgstr "Exportieren"
 
-#: widgets/waveform/waveform_widget.py:3305
+#: widgets/waveform/waveform_widget.py:3355
 msgid "Analysis"
 msgstr "Analyse"
 
-#: widgets/waveform/waveform_widget.py:3313
+#: widgets/waveform/waveform_widget.py:3363
 msgid "Interval"
 msgstr "Interval"
 
-#: widgets/waveform/waveform_widget.py:3322
+#: widgets/waveform/waveform_widget.py:3372
 msgid "Zoom"
 msgstr "Zoom"
 
-#: widgets/waveform/waveform_widget.py:3326
+#: widgets/waveform/waveform_widget.py:3376
 msgid "Show statistics"
 msgstr "Statistik anzeigen"
 
-#: widgets/waveform/waveform_widget.py:3331
+#: widgets/waveform/waveform_widget.py:3381
 msgid "Left"
 msgstr "Links"
 
-#: widgets/waveform/waveform_widget.py:3334
+#: widgets/waveform/waveform_widget.py:3384
 msgid "Right"
 msgstr "Rechts"
 
-#: widgets/waveform/waveform_widget.py:3337
+#: widgets/waveform/waveform_widget.py:3387
 msgid "Off"
 msgstr "Aus"
 
-#: widgets/waveform/waveform_widget.py:3340
-#: widgets/waveform/waveform_widget.py:3368
-#: widgets/waveform/waveform_widget.py:3397
+#: widgets/waveform/waveform_widget.py:3390
+#: widgets/waveform/waveform_widget.py:3418
+#: widgets/waveform/waveform_widget.py:3448
 msgid "Remove"
 msgstr "entfernen"
 
-#: widgets/waveform/waveform_widget.py:3351
+#: widgets/waveform/waveform_widget.py:3401
 msgid "Y mode"
 msgstr "Y-Modus"
 
 #: widgets/waveform/y_range_widget.py:67
 msgid "max"
 msgstr "max"
```

### Comparing `joulescope_ui-1.1.6/joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.7/joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.2\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-18 14:15-0400\n"
+"POT-Creation-Date: 2024-05-06 17:27-0400\n"
 "PO-Revision-Date: 2024-04-04 14:45-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: el\n"
 "Language-Team: el <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.14.0\n"
+"Generated-By: Babel 2.15.0\n"
 
 msgid "\"3.3 V\" uses an internally-generated 3.3V reference voltage."
 msgstr "\"3,3 V\" χρησιμοποιεί μια εσωτερικά παραγόμενη τάση αναφοράς 3,3 V."
 
 msgid "\"NaN\" sets all samples in the window to NaN."
 msgstr "\"NaN\" θέτει όλα τα δείγματα στο παράθυρο σε NaN."
 
@@ -658,14 +658,17 @@
 msgid ""
 "Display the number of actions processed by the publish-subscribe broker in "
 "each second."
 msgstr ""
 "Εμφάνιση του αριθμού των ενεργειών που επεξεργάζεται ο μεσίτης δημοσιεύσεων-"
 "συνδρομών σε κάθε δευτερόλεπτο."
 
+msgid "Divide the quantity by this value."
+msgstr "Διαιρέστε την ποσότητα με αυτή την τιμή."
+
 msgid "Do not show again"
 msgstr "Μην εμφανίζετε ξανά"
 
 msgid "Do not use any USB hubs, docks or adapters"
 msgstr "Μην χρησιμοποιείτε διανομείς, αποβάθρες ή προσαρμογείς USB"
 
 msgid "Dual markers"
@@ -1792,14 +1795,21 @@
 msgstr ""
 "Οι εμφανιζόμενες τιμές ενημερώνονται κανονικά με κάθε νέο στατιστικό "
 "δεδομένο που υπολογίζεται από τη συσκευή. Όταν είναι επιλεγμένο αυτό το "
 "κουμπί, η οθόνη δεν θα ενημερώνεται. Ωστόσο, τα στατιστικά στοιχεία θα "
 "συνεχίσουν να συσσωρεύονται και να συσσωρεύονται (εάν επιλεγεί)."
 
 msgid ""
+"The divisor is a floating point number. The number may optionally be "
+"followed by units."
+msgstr ""
+"Ο διαιρέτης είναι ένας αριθμός κινητής υποδιαστολής. Ο αριθμός μπορεί "
+"προαιρετικά να ακολουθείται από μονάδες."
+
+msgid ""
 "The exponential decay time constant. The fuse dissipates 63.2 percent of "
 "accumulated energy in this duration."
 msgstr ""
 "Η σταθερά χρόνου εκθετικής αποσύνθεσης. Η ασφάλεια διαχέει το 63,2 % της "
 "συσσωρευμένης ενέργειας σε αυτή τη διάρκεια."
 
 msgid "The filename supports the following replacements."
@@ -1808,17 +1818,14 @@
 msgid "The filename with optional replacements."
 msgstr "Το όνομα αρχείου με προαιρετικές αντικαταστάσεις."
 
 msgid "The fixed default path for loading and saving files."
 msgstr ""
 "Η σταθερή προεπιλεγμένη διαδρομή για τη φόρτωση και την αποθήκευση αρχείων."
 
-msgid "The flyout width in pixels."
-msgstr "Το πλάτος του flyout σε pixels."
-
 msgid "The font scheme name."
 msgstr "Το όνομα του συστήματος γραμματοσειράς."
 
 msgid "The format string"
 msgstr "Η συμβολοσειρά μορφής"
 
 msgid "The fuse trips in Duration at this constant current."
```

### Comparing `joulescope_ui-1.1.6/joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.7/joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.2\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-18 14:15-0400\n"
+"POT-Creation-Date: 2024-05-06 17:27-0400\n"
 "PO-Revision-Date: 2024-04-04 14:45-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: el <LL@li.org>\n"
 "Language: el\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-"Generated-By: Babel 2.14.0\n"
+"Generated-By: Babel 2.15.0\n"
 
 #: about.py:24
 msgid "About the Joulescope UI"
 msgstr "Σχετικά με το UI του Joulescope"
 
 #: about.py:25
 msgid "Version Information"
@@ -336,27 +336,27 @@
 msgid "Email"
 msgstr "Email"
 
 #: error_window.py:103
 msgid "Description"
 msgstr "Περιγραφή"
 
-#: error_window.py:112 widgets/waveform/waveform_widget.py:3347
+#: error_window.py:112 widgets/waveform/waveform_widget.py:3397
 msgid "Edit"
 msgstr "Επεξεργασία"
 
 #: error_window.py:113
 msgid "View as Markdown"
 msgstr "Προβολή ως Markdown"
 
 #: error_window.py:119
 msgid "Abort"
 msgstr "Διακοπή"
 
-#: error_window.py:120 main.py:365 widgets/settings/settings_widget.py:539
+#: error_window.py:120 main.py:363 widgets/settings/settings_widget.py:539
 msgid "View"
 msgstr "Προβολή"
 
 #: error_window.py:121
 msgid "Submit"
 msgstr "Υποβολή"
 
@@ -368,15 +368,15 @@
 msgid "Revert to previous configuration"
 msgstr "Επιστροφή στην προηγούμενη διαμόρφωση"
 
 #: error_window.py:282
 msgid "Revert to defaults"
 msgstr "Επαναφορά στις προεπιλογές"
 
-#: error_window.py:283 main.py:363 main.py:409
+#: error_window.py:283 main.py:361 main.py:407
 #: widgets/js220_cal/js220_cal_widget.py:38
 msgid "Exit"
 msgstr "Έξοδος"
 
 #: exporter.py:49 widgets/signal_record/signal_record_config_widget.py:148
 #: widgets/statistics_record/statistics_record_config_widget.py:111
 msgid "Directory"
@@ -646,165 +646,165 @@
 msgid "Do not show again"
 msgstr "Μην εμφανίζετε ξανά"
 
 #: intel_graphics_dialog.py:91
 msgid "Intel graphics detected"
 msgstr "Ανιχνεύονται γραφικά Intel"
 
-#: main.py:70 widgets/value/value_widget.py:653
+#: main.py:69 widgets/value/value_widget.py:660
 msgid "Multimeter"
 msgstr "Πολύμετρο"
 
-#: main.py:71
+#: main.py:70
 msgid "Oscilloscope"
 msgstr "Παλμογράφος"
 
-#: main.py:72 main.py:298 main.py:359 main.py:402
+#: main.py:71 main.py:296 main.py:357 main.py:400
 msgid "File"
 msgstr "Αρχείο"
 
-#: main.py:82
+#: main.py:81
 msgid "The UI status bar display mode"
 msgstr "Ο τρόπος εμφάνισης της γραμμής κατάστασης του UI"
 
-#: main.py:83
+#: main.py:82
 msgid ""
 "This setting controls the amount of detail shown on the status bar at the "
 "bottom of the UI window. You should usually leave this set to \"normal\" "
 "unless you want more detail concerning the UI internal operation."
 msgstr ""
 "Αυτή η ρύθμιση ελέγχει την ποσότητα των λεπτομερειών που εμφανίζονται στη "
 "γραμμή κατάστασης στο κάτω μέρος του παραθύρου UI. Συνήθως θα πρέπει να την "
 "αφήνετε ρυθμισμένη στην τιμή \"normal\", εκτός αν θέλετε περισσότερες "
 "λεπτομέρειες σχετικά με την εσωτερική λειτουργία του UI."
 
-#: main.py:88 safe_mode.py:43
+#: main.py:87 safe_mode.py:43
 msgid "Normal"
 msgstr "Κανονικό"
 
-#: main.py:89
+#: main.py:88
 msgid "Troubleshoot"
 msgstr "Αντιμετώπιση προβλημάτων"
 
-#: main.py:95
+#: main.py:94
 msgid "Enable developer mode."
 msgstr "Ενεργοποίηση της λειτουργίας προγραμματιστή."
 
-#: main.py:108
+#: main.py:107
 msgid "PubSub utilization"
 msgstr "Χρήση PubSub"
 
-#: main.py:109
+#: main.py:108
 msgid ""
 "Display the number of actions processed by the publish-subscribe broker in "
 "each second."
 msgstr ""
 "Εμφάνιση του αριθμού των ενεργειών που επεξεργάζεται ο μεσίτης δημοσιεύσεων-"
 "συνδρομών σε κάθε δευτερόλεπτο."
 
-#: main.py:114
+#: main.py:113
 msgid "CPU utilization"
 msgstr "Χρήση CPU"
 
-#: main.py:115
+#: main.py:114
 msgid ""
 "Display the CPU utilization by this application and the total CPU "
 "utilization by all applications. The value is displayed in percent."
 msgstr ""
 "Εμφάνιση της χρήσης της CPU από αυτή την εφαρμογή και της συνολικής χρήσης "
 "της CPU από όλες τις εφαρμογές. Η τιμή εμφανίζεται σε ποσοστό επί τοις "
 "εκατό."
 
-#: main.py:121
+#: main.py:120
 msgid "Memory utilization"
 msgstr "Χρήση μνήμης"
 
-#: main.py:122
+#: main.py:121
 msgid ""
 "Display the memory (RAM) utilization by this application and by all "
 "applications. The value is displayed in percent."
 msgstr ""
 "Εμφάνιση της χρήσης της μνήμης (RAM) από αυτή την εφαρμογή και από όλες τις "
 "εφαρμογές. Η τιμή εμφανίζεται σε ποσοστό επί τοις εκατό."
 
-#: main.py:216
+#: main.py:214
 msgid "UI"
 msgstr "UI"
 
-#: main.py:330
+#: main.py:328
 msgid "Help"
 msgstr "Βοήθεια"
 
-#: main.py:331 widgets/hamburger/hamburger_widget.py:21
+#: main.py:329 widgets/hamburger/hamburger_widget.py:21
 msgid "Getting Started"
 msgstr "Ξεκινώντας"
 
-#: main.py:332
+#: main.py:330
 msgid "User's Guide"
 msgstr "Οδηγός χρήσης"
 
-#: main.py:333 widgets/hamburger/hamburger_widget.py:22
+#: main.py:331 widgets/hamburger/hamburger_widget.py:22
 msgid "Changelog"
 msgstr "Changelog"
 
-#: main.py:334 widgets/help/help_widget.py:59
+#: main.py:332 widgets/help/help_widget.py:59
 msgid "Report Issue"
 msgstr "Έκδοση έκθεσης"
 
-#: main.py:335
+#: main.py:333
 msgid "View logs..."
 msgstr "Προβολή αρχείων καταγραφής..."
 
-#: main.py:336 widgets/hamburger/hamburger_widget.py:23
+#: main.py:334 widgets/hamburger/hamburger_widget.py:23
 msgid "Credits"
 msgstr "Συντελεστές"
 
-#: main.py:337 widgets/hamburger/hamburger_widget.py:24
+#: main.py:335 widgets/hamburger/hamburger_widget.py:24
 msgid "About"
 msgstr "Σχετικά με το"
 
-#: main.py:360
+#: main.py:358
 msgid "Open"
 msgstr "Open"
 
-#: main.py:361
+#: main.py:359
 msgid "Open recent"
 msgstr "Ανοικτό πρόσφατα"
 
-#: main.py:362 main.py:408
+#: main.py:360 main.py:406
 msgid "Clear config and exit"
 msgstr "Εκκαθάριση ρυθμίσεων και έξοδος"
 
-#: main.py:366 widgets/settings/settings_widget.py:541
+#: main.py:364 widgets/settings/settings_widget.py:541
 msgid "Widgets"
 msgstr "Widgets"
 
-#: main.py:367
+#: main.py:365
 msgid "Tools"
 msgstr "Εργαλεία"
 
-#: main.py:368
+#: main.py:366
 msgid "Clear Accumulators"
 msgstr "Σαφείς συσσωρευτές"
 
-#: main.py:403
+#: main.py:401
 msgid "Info"
 msgstr "Πληροφορίες"
 
-#: main.py:404 widget_tools.py:92 widgets/settings/settings_widget.py:31
+#: main.py:402 widget_tools.py:92 widgets/settings/settings_widget.py:31
 #: widgets/settings/settings_widget.py:574
 #: widgets/sidebar/sidebar_widget.py:41
 msgid "Settings"
 msgstr "Ρυθμίσεις"
 
-#: main.py:693
+#: main.py:710
 msgid "Manage"
 msgstr "Διαχείριση"
 
-#: main.py:730
+#: main.py:747
 msgid "Select file to open"
 msgstr "Επιλέξτε αρχείο για άνοιγμα"
 
 #: paths.py:30 styles/manager.py:46
 msgid "The name for this widget."
 msgstr "Το όνομα για αυτό το widget."
 
@@ -947,47 +947,47 @@
 msgid "Source"
 msgstr "Πηγή"
 
 #: units.py:35
 msgid "Use the application defaults"
 msgstr "Χρήση των προεπιλογών της εφαρμογής"
 
-#: view.py:68
+#: view.py:72
 msgid "The active theme."
 msgstr "Το ενεργό θέμα."
 
-#: view.py:70
+#: view.py:74
 msgid "Joulescope standard theme"
 msgstr "Πρότυπο θέμα Joulescope"
 
-#: view.py:70
+#: view.py:74
 msgid "System OS-specific theme"
 msgstr "Ειδικό θέμα για το σύστημα OS"
 
-#: view.py:75
+#: view.py:79
 msgid "The color scheme name."
 msgstr "Το όνομα του χρωματικού σχήματος."
 
-#: view.py:77
+#: view.py:81
 msgid "Dark background"
 msgstr "Σκούρο φόντο"
 
-#: view.py:77
+#: view.py:81
 msgid "Light background"
 msgstr "Φωτεινό φόντο"
 
-#: view.py:81
+#: view.py:85
 msgid "The font scheme name."
 msgstr "Το όνομα του συστήματος γραμματοσειράς."
 
-#: view.py:83
+#: view.py:87
 msgid "Joulescope standard font theme"
 msgstr "Joulescope πρότυπο θέμα γραμματοσειράς"
 
-#: view.py:102 widgets/view_manager/view_manager_widget.py:146
+#: view.py:106 widgets/view_manager/view_manager_widget.py:146
 msgid "New View"
 msgstr "Νέα προβολή"
 
 #: zip_inspector.py:23
 msgid "ZIP Inspector"
 msgstr "Επιθεωρητής ZIP"
 
@@ -1107,15 +1107,15 @@
 "Όταν είναι ενεργοποιημένο, το ρεύμα ρέει μεταξύ των ακροδεκτών ρεύματος. "
 "Όταν είναι απενεργοποιημένο, το ρεύμα δεν μπορεί να ρέει μεταξύ των "
 "ακροδεκτών ρεύματος. Στις συνήθεις ρυθμίσεις συστημάτων, αυτό αναστέλλει την"
 " τροφοδοσία του στόχου, η οποία μπορεί να χρησιμοποιηθεί για την επαναφορά "
 "της συσκευής στόχου σε κύκλο λειτουργίας."
 
 #: devices/jsdrv/js110.py:147 devices/jsdrv/js220.py:163
-#: widgets/waveform/waveform_widget.py:110
+#: widgets/waveform/waveform_widget.py:109
 msgid "Current range"
 msgstr "Εύρος ρεύματος"
 
 #: devices/jsdrv/js110.py:149
 msgid ""
 "Configure the J110's current range. Most applications should use the "
 "default, \"auto\"."
@@ -1264,33 +1264,33 @@
 "mean. This value is ignored for all other IRF types."
 msgstr ""
 "Ο αριθμός των δειγμάτων μετά το παράθυρο εύρους ρεύματος που χρησιμοποιείται"
 " για τον προσδιορισμό του μέσου όρου. Αυτή η τιμή αγνοείται για όλους τους "
 "άλλους τύπους IRF."
 
 #: devices/jsdrv/js110.py:269 devices/jsdrv/js220.py:332
-#: widgets/device_control/fuse.py:103 widgets/waveform/waveform_widget.py:105
+#: widgets/device_control/fuse.py:103 widgets/waveform/waveform_widget.py:104
 msgid "Current"
 msgstr "Ρεύμα"
 
 #: devices/jsdrv/js110.py:270 devices/jsdrv/js220.py:333
 msgid "Enable the current signal streaming."
 msgstr "Ενεργοποίηση της ροής σημάτων ρεύματος."
 
 #: devices/jsdrv/js110.py:278 devices/jsdrv/js220.py:341
-#: widgets/waveform/waveform_widget.py:106
+#: widgets/waveform/waveform_widget.py:105
 msgid "Voltage"
 msgstr "Τάση"
 
 #: devices/jsdrv/js110.py:279 devices/jsdrv/js220.py:342
 msgid "Enable the voltage signal streaming."
 msgstr "Ενεργοποίηση της ροής σήματος τάσης."
 
 #: devices/jsdrv/js110.py:287 devices/jsdrv/js220.py:350
-#: widgets/waveform/waveform_widget.py:107
+#: widgets/waveform/waveform_widget.py:106
 msgid "Power"
 msgstr "Ισχύς"
 
 #: devices/jsdrv/js110.py:288 devices/jsdrv/js220.py:351
 msgid "Enable the power signal streaming."
 msgstr "Ενεργοποίηση της ροής σήματος ισχύος."
 
@@ -1510,15 +1510,15 @@
 msgid "GPI 3"
 msgstr "GPI 3"
 
 #: devices/jsdrv/js220.py:402
 msgid "Enable the general purpose input 3 signal streaming."
 msgstr "Ενεργοποιήστε τη ροή σήματος εισόδου γενικού σκοπού 3."
 
-#: devices/jsdrv/js220.py:410 widgets/waveform/waveform_widget.py:124
+#: devices/jsdrv/js220.py:410 widgets/waveform/waveform_widget.py:123
 msgid "Trigger input"
 msgstr "Είσοδος σκανδαλισμού"
 
 #: devices/jsdrv/js220.py:411
 msgid "Enable the trigger input signal streaming."
 msgstr "Ενεργοποίηση της ροής σήματος εισόδου σκανδαλισμού."
 
@@ -1529,15 +1529,15 @@
 #: devices/jsdrv/jsdrv_stream_buffer.py:44
 #: devices/jsdrv/jsdrv_stream_buffer.py:93
 #: devices/jsdrv/jsdrv_stream_buffer.py:107 plugins/selector.py:58
 #: widgets/settings/settings_widget.py:85
 #: widgets/settings/settings_widget.py:266
 #: widgets/settings/settings_widget.py:364
 #: widgets/settings/settings_widget.py:431
-#: widgets/waveform/waveform_widget.py:3062
+#: widgets/waveform/waveform_widget.py:3104
 msgid "Name"
 msgstr "Όνομα"
 
 #: devices/jsdrv/jsdrv_stream_buffer.py:45
 msgid "Joulescope stream buffer"
 msgstr "Απομονωτής ρεύματος Joulescope"
 
@@ -1762,15 +1762,15 @@
 
 #: widgets/accumulator/accumulator_widget.py:27
 #: widgets/value/value_widget.py:31
 msgid "The statistics data stream source."
 msgstr "Η πηγή ροής στατιστικών δεδομένων."
 
 #: widgets/accumulator/accumulator_widget.py:32
-#: widgets/value/value_widget.py:74
+#: widgets/value/value_widget.py:81
 msgid "The signal to display."
 msgstr "Το σήμα προς απεικόνιση."
 
 #: widgets/accumulator/accumulator_widget.py:34
 msgid "charge"
 msgstr "φόρτιση"
 
@@ -1854,15 +1854,15 @@
 
 #: widgets/developer/publish_spy_widget.py:20
 #: widgets/developer/publish_spy_widget.py:21
 msgid "Topic"
 msgstr "Θέμα"
 
 #: widgets/developer/publish_spy_widget.py:21
-#: widgets/settings/settings_widget.py:87 widgets/value/value_widget.py:662
+#: widgets/settings/settings_widget.py:87 widgets/value/value_widget.py:669
 msgid "Value"
 msgstr "Τιμή"
 
 #: widgets/developer/publish_spy_widget.py:24
 msgid "Publish Spy"
 msgstr "Δημοσίευση Spy"
 
@@ -1892,15 +1892,15 @@
 
 #: widgets/device_control/device_update_dialog.py:24
 #: widgets/device_control/device_update_dialog.py:45
 msgid "Update"
 msgstr "Ενημέρωση"
 
 #: widgets/device_control/device_update_dialog.py:25
-#: widgets/value/value_widget.py:147
+#: widgets/value/value_widget.py:155
 msgid "Device"
 msgstr "Συσκευή"
 
 #: widgets/device_control/device_update_dialog.py:27
 #: widgets/progress_bar/progress_bar_widget.py:59
 msgid "Progress"
 msgstr "Progress"
@@ -2433,18 +2433,14 @@
 msgid "Click to display additional settings and actions."
 msgstr "Κάντε κλικ για να εμφανίσετε πρόσθετες ρυθμίσεις και ενέργειες."
 
 #: widgets/sidebar/sidebar_widget.py:60
 msgid "sidebar"
 msgstr "sidebar"
 
-#: widgets/sidebar/sidebar_widget.py:68
-msgid "The flyout width in pixels."
-msgstr "Το πλάτος του flyout σε pixels."
-
 #: widgets/signal_record/disk_full_dialog.py:19
 msgid "The disk is full"
 msgstr "Ο δίσκος είναι γεμάτος"
 
 #: widgets/signal_record/signal_record.py:57
 msgid "Could not open file for write"
 msgstr "Δεν κατέστη δυνατό το άνοιγμα αρχείου για εγγραφή"
@@ -2471,15 +2467,15 @@
 msgid "StatisticsRecordConfig"
 msgstr "StatisticsRecordConfig"
 
 #: widgets/statistics_record/statistics_record_config_widget.py:123
 msgid "Time Format"
 msgstr "Μορφή χρόνου"
 
-#: widgets/trigger/trigger_widget.py:41 widgets/value/value_widget.py:87
+#: widgets/trigger/trigger_widget.py:41 widgets/value/value_widget.py:94
 msgid "Select the source device"
 msgstr "Επιλέξτε τη συσκευή προέλευσης"
 
 #: widgets/trigger/trigger_widget.py:42
 msgid "The device to use for the start condition and stop condition."
 msgstr ""
 "Η συσκευή που θα χρησιμοποιηθεί για τη συνθήκη εκκίνησης και τη συνθήκη "
@@ -2658,86 +2654,98 @@
 msgid "Show the statistics fields at the right."
 msgstr "Εμφανίστε τα πεδία στατιστικών στοιχείων στα δεξιά."
 
 #: widgets/value/value_widget.py:51
 msgid "Show a leading + or - sign."
 msgstr "Εμφανίζει ένα πρόσημο + ή -."
 
-#: widgets/value/value_widget.py:88
+#: widgets/value/value_widget.py:62
+msgid "Divide the quantity by this value."
+msgstr "Διαιρέστε την ποσότητα με αυτή την τιμή."
+
+#: widgets/value/value_widget.py:63
+msgid ""
+"The divisor is a floating point number. The number may optionally be "
+"followed by units."
+msgstr ""
+"Ο διαιρέτης είναι ένας αριθμός κινητής υποδιαστολής. Ο αριθμός μπορεί "
+"προαιρετικά να ακολουθείται από μονάδες."
+
+#: widgets/value/value_widget.py:95
 msgid ""
 "The values displayed by this widget come from a single source device. Select"
 " the source device here."
 msgstr ""
 "Οι τιμές που εμφανίζονται από αυτό το widget προέρχονται από μία μόνο "
 "συσκευή προέλευσης. Επιλέξτε τη συσκευή προέλευσης εδώ."
 
-#: widgets/value/value_widget.py:94
+#: widgets/value/value_widget.py:101
 msgid "Hold the display"
 msgstr "Κρατήστε την οθόνη"
 
-#: widgets/value/value_widget.py:96
+#: widgets/value/value_widget.py:103
 msgid "When selected, prevent the display from updating."
 msgstr "Όταν είναι επιλεγμένο, εμποδίζει την ενημέρωση της οθόνης."
 
-#: widgets/value/value_widget.py:97
+#: widgets/value/value_widget.py:104
 msgid ""
 "The UI also includes a global statistics hold button on the sidebar. When "
 "the global statistics hold button is selected, this button is disabled and "
 "has no effect."
 msgstr ""
 "Το UI περιλαμβάνει επίσης ένα κουμπί κράτησης συνολικών στατιστικών "
 "στοιχείων στην πλευρική γραμμή. Όταν είναι επιλεγμένο το κουμπί global "
 "statistics hold, αυτό το κουμπί είναι απενεργοποιημένο και δεν έχει καμία "
 "επίδραση."
 
-#: widgets/value/value_widget.py:100
+#: widgets/value/value_widget.py:107
 msgid ""
 "The displayed values normally update with each new statistics data computed "
 "by the device. When this button is selected, the display will not be "
 "updated. However, the statistics will continue accumulate and accrue (if "
 "selected)."
 msgstr ""
 "Οι εμφανιζόμενες τιμές ενημερώνονται κανονικά με κάθε νέο στατιστικό "
 "δεδομένο που υπολογίζεται από τη συσκευή. Όταν είναι επιλεγμένο αυτό το "
 "κουμπί, η οθόνη δεν θα ενημερώνεται. Ωστόσο, τα στατιστικά στοιχεία θα "
 "συνεχίσουν να συσσωρεύονται και να συσσωρεύονται (εάν επιλεγεί)."
 
-#: widgets/value/value_widget.py:107
+#: widgets/value/value_widget.py:114
 msgid "Accrue values over time"
 msgstr "Συγκέντρωση τιμών με την πάροδο του χρόνου"
 
-#: widgets/value/value_widget.py:109
+#: widgets/value/value_widget.py:116
 msgid ""
 "Current, voltage, and power are normally computed over a single statistics "
 "frequency interval. Press this button to accrue the values indefinitely. "
 "Press again to return to normal operation."
 msgstr ""
 "Το ρεύμα, η τάση και η ισχύς υπολογίζονται συνήθως σε ένα ενιαίο διάστημα "
 "στατιστικής συχνότητας. Πατήστε αυτό το κουμπί για να συγκεντρώσετε τις "
 "τιμές επ' αόριστον. Πατήστε το ξανά για να επιστρέψετε στην κανονική "
 "λειτουργία."
 
-#: widgets/value/value_widget.py:113
+#: widgets/value/value_widget.py:120
 msgid ""
 "Note that this button does not affect the charge and energy accumulation. "
 "Both accumulate indefinitely regardless of this button state."
 msgstr ""
 "Σημειώστε ότι αυτό το κουμπί δεν επηρεάζει τη φόρτιση και τη συσσώρευση "
 "ενέργειας. Και τα δύο συσσωρεύονται επ' αόριστον ανεξάρτητα από την "
 "κατάσταση αυτού του κουμπιού."
 
-#: widgets/value/value_widget.py:195
+#: widgets/value/value_widget.py:203
 msgid "Not present"
 msgstr "Δεν υπάρχει"
 
-#: widgets/value/value_widget.py:215
+#: widgets/value/value_widget.py:223
 msgid "Hold"
 msgstr "Hold"
 
-#: widgets/value/value_widget.py:223
+#: widgets/value/value_widget.py:231
 msgid "Accrue"
 msgstr "Αυξημένο"
 
 #: widgets/view_manager/view_manager_widget.py:108
 #: widgets/view_manager/view_manager_widget.py:174
 msgid "View Manager"
 msgstr "Διαχείριση προβολής"
@@ -2783,34 +2791,34 @@
 msgstr "τρίγωνο δεξιά"
 
 #: widgets/waveform/text_annotation.py:62
 msgid "triangle left"
 msgstr "τρίγωνο αριστερά"
 
 #: widgets/waveform/text_annotation.py:66
-#: widgets/waveform/waveform_widget.py:3008
+#: widgets/waveform/waveform_widget.py:3050
 msgid "Manual"
 msgstr "Εγχειρίδιο"
 
 #: widgets/waveform/text_annotation.py:67
 msgid "Centered"
 msgstr "Centered"
 
 #: widgets/waveform/text_annotation.py:99
-#: widgets/waveform/waveform_widget.py:3123
+#: widgets/waveform/waveform_widget.py:3167
 msgid "Text"
 msgstr "Κείμενο"
 
 #: widgets/waveform/text_annotation.py:107
-#: widgets/waveform/waveform_widget.py:3348
+#: widgets/waveform/waveform_widget.py:3398
 msgid "Show text"
 msgstr "Εμφάνιση κειμένου"
 
 #: widgets/waveform/text_annotation.py:116
-#: widgets/waveform/waveform_widget.py:3360
+#: widgets/waveform/waveform_widget.py:3410
 msgid "Shape"
 msgstr "Σχήμα"
 
 #: widgets/waveform/text_annotation.py:126
 msgid "Y Mode"
 msgstr "Λειτουργία Y"
 
@@ -3008,325 +3016,325 @@
 "\"default\" will use the default source which is normally configured using "
 "the Device Control widget."
 msgstr ""
 "\"default\" θα χρησιμοποιήσει την προεπιλεγμένη πηγή, η οποία κανονικά "
 "διαμορφώνεται χρησιμοποιώντας το widget Device Control."
 
 #: widgets/waveform/waveform_source_widget.py:104
-#: widgets/waveform/waveform_widget.py:402
-#: widgets/waveform/waveform_widget.py:479
+#: widgets/waveform/waveform_widget.py:401
+#: widgets/waveform/waveform_widget.py:478
 msgid "off"
 msgstr "off"
 
-#: widgets/waveform/waveform_widget.py:44
+#: widgets/waveform/waveform_widget.py:43
 msgid "Waveform"
 msgstr "Κυματομορφή"
 
-#: widgets/waveform/waveform_widget.py:120
+#: widgets/waveform/waveform_widget.py:119
 msgid "General purpose input 0"
 msgstr "Είσοδος γενικού σκοπού 0"
 
-#: widgets/waveform/waveform_widget.py:121
+#: widgets/waveform/waveform_widget.py:120
 msgid "General purpose input 1"
 msgstr "Είσοδος γενικού σκοπού 1"
 
-#: widgets/waveform/waveform_widget.py:122
+#: widgets/waveform/waveform_widget.py:121
 msgid "General purpose input 2"
 msgstr "Είσοδος γενικού σκοπού 2"
 
-#: widgets/waveform/waveform_widget.py:123
+#: widgets/waveform/waveform_widget.py:122
 msgid "General purpose input 3"
 msgstr "Είσοδος γενικού σκοπού 3"
 
-#: widgets/waveform/waveform_widget.py:358
+#: widgets/waveform/waveform_widget.py:357
 msgid "The source filter string."
 msgstr "Η συμβολοσειρά φίλτρων πηγής."
 
-#: widgets/waveform/waveform_widget.py:369
+#: widgets/waveform/waveform_widget.py:368
 msgid "The trace width."
 msgstr "Το πλάτος του ίχνους."
 
-#: widgets/waveform/waveform_widget.py:384
+#: widgets/waveform/waveform_widget.py:383
 msgid "The target frames per second."
 msgstr "Τα καρέ ανά δευτερόλεπτο που είναι ο στόχος."
 
-#: widgets/waveform/waveform_widget.py:386
+#: widgets/waveform/waveform_widget.py:385
 msgid "vsync"
 msgstr "vsync"
 
-#: widgets/waveform/waveform_widget.py:387
+#: widgets/waveform/waveform_widget.py:386
 msgid "20 Hz"
 msgstr "20 Hz"
 
-#: widgets/waveform/waveform_widget.py:388
+#: widgets/waveform/waveform_widget.py:387
 msgid "10 Hz"
 msgstr "10 Hz"
 
-#: widgets/waveform/waveform_widget.py:389
+#: widgets/waveform/waveform_widget.py:388
 msgid "5 Hz"
 msgstr "5 Hz"
 
-#: widgets/waveform/waveform_widget.py:395
+#: widgets/waveform/waveform_widget.py:394
 msgid "The minimum interval between repaint in milliseconds."
 msgstr ""
 "Το ελάχιστο χρονικό διάστημα μεταξύ επανεκτύπωσης σε χιλιοστά του "
 "δευτερολέπτου."
 
-#: widgets/waveform/waveform_widget.py:400
+#: widgets/waveform/waveform_widget.py:399
 msgid "Show the minimum and maximum extents fill."
 msgstr "Εμφανίζει την ελάχιστη και τη μέγιστη έκταση πλήρωσης."
 
-#: widgets/waveform/waveform_widget.py:403
+#: widgets/waveform/waveform_widget.py:402
 msgid "lines"
 msgstr "γραμμές"
 
-#: widgets/waveform/waveform_widget.py:404
+#: widgets/waveform/waveform_widget.py:403
 msgid "fill 1"
 msgstr "γέμισμα 1"
 
-#: widgets/waveform/waveform_widget.py:405
+#: widgets/waveform/waveform_widget.py:404
 msgid "fill 2"
 msgstr "γέμισμα 2"
 
-#: widgets/waveform/waveform_widget.py:411
+#: widgets/waveform/waveform_widget.py:410
 msgid "Show the frames per second."
 msgstr "Εμφάνιση των καρέ ανά δευτερόλεπτο."
 
-#: widgets/waveform/waveform_widget.py:416
+#: widgets/waveform/waveform_widget.py:415
 msgid "Show the statistics on mouse hover."
 msgstr "Εμφάνιση των στατιστικών στοιχείων κατά το πέρασμα του ποντικιού."
 
-#: widgets/waveform/waveform_widget.py:421
+#: widgets/waveform/waveform_widget.py:420
 msgid "Show the plot statistics on the right."
 msgstr "Εμφάνιση των στατιστικών στοιχείων της γραφικής παράστασης στα δεξιά."
 
-#: widgets/waveform/waveform_widget.py:426
+#: widgets/waveform/waveform_widget.py:425
 msgid "Show frequency for dual markers and statistics."
 msgstr "Εμφάνιση συχνότητας για διπλούς δείκτες και στατιστικά στοιχεία."
 
-#: widgets/waveform/waveform_widget.py:431
+#: widgets/waveform/waveform_widget.py:430
 msgid "The quantities to display by default."
 msgstr "Οι ποσότητες που θα εμφανίζονται από προεπιλογή."
 
-#: widgets/waveform/waveform_widget.py:437
+#: widgets/waveform/waveform_widget.py:436
 msgid "The precision to display in digits."
 msgstr "Η ακρίβεια για την εμφάνιση σε ψηφία."
 
-#: widgets/waveform/waveform_widget.py:443
+#: widgets/waveform/waveform_widget.py:442
 msgid "Use OpenGL rendering."
 msgstr "Χρησιμοποιήστε απόδοση OpenGL."
 
-#: widgets/waveform/waveform_widget.py:454
+#: widgets/waveform/waveform_widget.py:453
 msgid "Pin the left side (oldest) data so that it stays in view."
 msgstr ""
 "Καρφιτσώστε τα δεδομένα της αριστερής πλευράς (παλαιότερα) ώστε να "
 "παραμένουν σε προβολή."
 
-#: widgets/waveform/waveform_widget.py:459
+#: widgets/waveform/waveform_widget.py:458
 msgid "Pin the right side (newest) data so that it stays in view."
 msgstr ""
 "Καρφιτσώστε τα δεδομένα της δεξιάς πλευράς (τα νεότερα), ώστε να παραμένουν "
 "σε προβολή."
 
-#: widgets/waveform/waveform_widget.py:464
+#: widgets/waveform/waveform_widget.py:463
 msgid "The waveform state."
 msgstr "Η κατάσταση της κυματομορφής."
 
-#: widgets/waveform/waveform_widget.py:470
+#: widgets/waveform/waveform_widget.py:469
 msgid "The annotations."
 msgstr "Οι επισημάνσεις."
 
-#: widgets/waveform/waveform_widget.py:476
+#: widgets/waveform/waveform_widget.py:475
 msgid "Control location"
 msgstr "Θέση ελέγχου"
 
-#: widgets/waveform/waveform_widget.py:480
+#: widgets/waveform/waveform_widget.py:479
 msgid "top"
 msgstr "top"
 
-#: widgets/waveform/waveform_widget.py:481
+#: widgets/waveform/waveform_widget.py:480
 msgid "bottom"
 msgstr "κάτω"
 
-#: widgets/waveform/waveform_widget.py:486
+#: widgets/waveform/waveform_widget.py:485
 msgid "The signal quantity to show in the summary."
 msgstr "Η ποσότητα σήματος που θα εμφανίζεται στη σύνοψη."
 
-#: widgets/waveform/waveform_widget.py:492
+#: widgets/waveform/waveform_widget.py:491
 msgid "X-axis annotation mode"
 msgstr "Λειτουργία σχολιασμού του άξονα Χ"
 
-#: widgets/waveform/waveform_widget.py:495
-#: widgets/waveform/waveform_widget.py:2888
+#: widgets/waveform/waveform_widget.py:494
+#: widgets/waveform/waveform_widget.py:2930
 msgid "Absolute"
 msgstr "Απόλυτο"
 
-#: widgets/waveform/waveform_widget.py:496
-#: widgets/waveform/waveform_widget.py:2893
+#: widgets/waveform/waveform_widget.py:495
+#: widgets/waveform/waveform_widget.py:2935
 msgid "Relative"
 msgstr "Σχετική"
 
-#: widgets/waveform/waveform_widget.py:502
+#: widgets/waveform/waveform_widget.py:501
 msgid "The available subsources."
 msgstr "Οι διαθέσιμες υποπηγές."
 
-#: widgets/waveform/waveform_widget.py:508
+#: widgets/waveform/waveform_widget.py:507
 msgid "The selected subsources for each trace."
 msgstr "Οι επιλεγμένες υποπηγές για κάθε ίχνος."
 
-#: widgets/waveform/waveform_widget.py:514
+#: widgets/waveform/waveform_widget.py:513
 msgid "The trace priority: highest int value on top, None is off."
 msgstr ""
 "Η προτεραιότητα του ίχνους: η υψηλότερη τιμή int στην κορυφή, το None είναι "
 "απενεργοποιημένο."
 
-#: widgets/waveform/waveform_widget.py:2834
-#: widgets/waveform/waveform_widget.py:3135
+#: widgets/waveform/waveform_widget.py:2877
+#: widgets/waveform/waveform_widget.py:3179
 msgid "Save image to file"
 msgstr "Αποθήκευση εικόνας σε αρχείο"
 
-#: widgets/waveform/waveform_widget.py:2882
-#: widgets/waveform/waveform_widget.py:2951
+#: widgets/waveform/waveform_widget.py:2924
+#: widgets/waveform/waveform_widget.py:2993
 msgid "Single marker"
 msgstr "Ενιαίος δείκτης"
 
-#: widgets/waveform/waveform_widget.py:2883
-#: widgets/waveform/waveform_widget.py:2952
+#: widgets/waveform/waveform_widget.py:2925
+#: widgets/waveform/waveform_widget.py:2994
 msgid "Dual markers"
 msgstr "Διπλοί δείκτες"
 
-#: widgets/waveform/waveform_widget.py:2885
+#: widgets/waveform/waveform_widget.py:2927
 msgid "Mode"
 msgstr "Λειτουργία"
 
-#: widgets/waveform/waveform_widget.py:2898
-#: widgets/waveform/waveform_widget.py:2953
-#: widgets/waveform/waveform_widget.py:3111
-#: widgets/waveform/waveform_widget.py:3129
+#: widgets/waveform/waveform_widget.py:2940
+#: widgets/waveform/waveform_widget.py:2995
+#: widgets/waveform/waveform_widget.py:3155
+#: widgets/waveform/waveform_widget.py:3173
 msgid "Clear all"
 msgstr "Εκκαθάριση όλων"
 
-#: widgets/waveform/waveform_widget.py:2909
-#: widgets/waveform/waveform_widget.py:2998
-#: widgets/waveform/waveform_widget.py:3117
+#: widgets/waveform/waveform_widget.py:2951
+#: widgets/waveform/waveform_widget.py:3040
+#: widgets/waveform/waveform_widget.py:3161
 msgid "Annotations"
 msgstr "Σημειώσεις"
 
-#: widgets/waveform/waveform_widget.py:3001
+#: widgets/waveform/waveform_widget.py:3043
 msgid "Range"
 msgstr "Εύρος"
 
-#: widgets/waveform/waveform_widget.py:3005
-#: widgets/waveform/waveform_widget.py:3328
+#: widgets/waveform/waveform_widget.py:3047
+#: widgets/waveform/waveform_widget.py:3378
 msgid "Auto"
 msgstr "Auto"
 
-#: widgets/waveform/waveform_widget.py:3011
+#: widgets/waveform/waveform_widget.py:3053
 msgid "Exact"
 msgstr "Ακριβές"
 
-#: widgets/waveform/waveform_widget.py:3020
+#: widgets/waveform/waveform_widget.py:3062
 msgid "Scale"
 msgstr "Κλίμακα"
 
-#: widgets/waveform/waveform_widget.py:3023
+#: widgets/waveform/waveform_widget.py:3065
 msgid "Linear"
 msgstr "Γραμμική"
 
-#: widgets/waveform/waveform_widget.py:3028
+#: widgets/waveform/waveform_widget.py:3070
 msgid "Logarithmic"
 msgstr "Λογαριθμική"
 
-#: widgets/waveform/waveform_widget.py:3036
+#: widgets/waveform/waveform_widget.py:3078
 msgid "Logarithmic zero"
 msgstr "Λογαριθμικό μηδέν"
 
-#: widgets/waveform/waveform_widget.py:3050
+#: widgets/waveform/waveform_widget.py:3092
 msgid "Preferred prefix"
 msgstr "Προτιμώμενο πρόθεμα"
 
-#: widgets/waveform/waveform_widget.py:3108
+#: widgets/waveform/waveform_widget.py:3152
 msgid "Add"
 msgstr "Προσθήκη"
 
-#: widgets/waveform/waveform_widget.py:3109
+#: widgets/waveform/waveform_widget.py:3153
 msgid "Hide all text"
 msgstr "Απόκρυψη όλου του κειμένου"
 
-#: widgets/waveform/waveform_widget.py:3110
+#: widgets/waveform/waveform_widget.py:3154
 msgid "Show all text"
 msgstr "Εμφάνιση όλου του κειμένου"
 
-#: widgets/waveform/waveform_widget.py:3118
+#: widgets/waveform/waveform_widget.py:3162
 msgid "Vertical"
 msgstr "Κατακόρυφο"
 
-#: widgets/waveform/waveform_widget.py:3121
+#: widgets/waveform/waveform_widget.py:3165
 msgid "Horizontal"
 msgstr "Οριζόντια"
 
-#: widgets/waveform/waveform_widget.py:3127
+#: widgets/waveform/waveform_widget.py:3171
 msgid "Save"
 msgstr "Αποθήκευση"
 
-#: widgets/waveform/waveform_widget.py:3132
+#: widgets/waveform/waveform_widget.py:3176
 msgid "Y-axis auto range"
 msgstr "Αυτόματο εύρος του άξονα Y"
 
-#: widgets/waveform/waveform_widget.py:3136
+#: widgets/waveform/waveform_widget.py:3180
 msgid "Copy image to clipboard"
 msgstr "Αντιγραφή εικόνας στο πρόχειρο"
 
-#: widgets/waveform/waveform_widget.py:3137
+#: widgets/waveform/waveform_widget.py:3181
 msgid "Export visible data"
 msgstr "Εξαγωγή ορατών δεδομένων"
 
-#: widgets/waveform/waveform_widget.py:3138
+#: widgets/waveform/waveform_widget.py:3182
 msgid "Export all data"
 msgstr "Εξαγωγή όλων των δεδομένων"
 
-#: widgets/waveform/waveform_widget.py:3304
+#: widgets/waveform/waveform_widget.py:3354
 msgid "Export"
 msgstr "Εξαγωγή"
 
-#: widgets/waveform/waveform_widget.py:3305
+#: widgets/waveform/waveform_widget.py:3355
 msgid "Analysis"
 msgstr "Ανάλυση"
 
-#: widgets/waveform/waveform_widget.py:3313
+#: widgets/waveform/waveform_widget.py:3363
 msgid "Interval"
 msgstr "Διάστημα"
 
-#: widgets/waveform/waveform_widget.py:3322
+#: widgets/waveform/waveform_widget.py:3372
 msgid "Zoom"
 msgstr "Ζουμ"
 
-#: widgets/waveform/waveform_widget.py:3326
+#: widgets/waveform/waveform_widget.py:3376
 msgid "Show statistics"
 msgstr "Εμφάνιση στατιστικών στοιχείων"
 
-#: widgets/waveform/waveform_widget.py:3331
+#: widgets/waveform/waveform_widget.py:3381
 msgid "Left"
 msgstr "Αριστερά"
 
-#: widgets/waveform/waveform_widget.py:3334
+#: widgets/waveform/waveform_widget.py:3384
 msgid "Right"
 msgstr "Σωστό"
 
-#: widgets/waveform/waveform_widget.py:3337
+#: widgets/waveform/waveform_widget.py:3387
 msgid "Off"
 msgstr "Off"
 
-#: widgets/waveform/waveform_widget.py:3340
-#: widgets/waveform/waveform_widget.py:3368
-#: widgets/waveform/waveform_widget.py:3397
+#: widgets/waveform/waveform_widget.py:3390
+#: widgets/waveform/waveform_widget.py:3418
+#: widgets/waveform/waveform_widget.py:3448
 msgid "Remove"
 msgstr "Αφαίρεση"
 
-#: widgets/waveform/waveform_widget.py:3351
+#: widgets/waveform/waveform_widget.py:3401
 msgid "Y mode"
 msgstr "Λειτουργία Y"
 
 #: widgets/waveform/y_range_widget.py:67
 msgid "max"
 msgstr "max"
```

### Comparing `joulescope_ui-1.1.6/joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.7/joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.2\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-18 14:15-0400\n"
+"POT-Creation-Date: 2024-05-06 17:27-0400\n"
 "PO-Revision-Date: 2024-04-04 14:45-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: es\n"
 "Language-Team: es <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.14.0\n"
+"Generated-By: Babel 2.15.0\n"
 
 msgid "\"3.3 V\" uses an internally-generated 3.3V reference voltage."
 msgstr ""
 "\"3,3 V\" utiliza una tensión de referencia de 3,3 V generada internamente."
 
 msgid "\"NaN\" sets all samples in the window to NaN."
 msgstr "\"NaN\" establece todas las muestras de la ventana en NaN."
@@ -655,14 +655,17 @@
 msgid ""
 "Display the number of actions processed by the publish-subscribe broker in "
 "each second."
 msgstr ""
 "Muestra el número de acciones procesadas por el broker publish-subscribe en "
 "cada segundo."
 
+msgid "Divide the quantity by this value."
+msgstr "Divida la cantidad por este valor."
+
 msgid "Do not show again"
 msgstr "No volver a mostrar"
 
 msgid "Do not use any USB hubs, docks or adapters"
 msgstr "No utilice concentradores, bases ni adaptadores USB"
 
 msgid "Dual markers"
@@ -1783,14 +1786,21 @@
 msgstr ""
 "Los valores mostrados normalmente se actualizan con cada nuevo dato "
 "estadístico calculado por el dispositivo. Cuando se selecciona este botón, "
 "la pantalla no se actualiza. Sin embargo, las estadísticas seguirán "
 "acumulándose y acumulándose (si está seleccionado)."
 
 msgid ""
+"The divisor is a floating point number. The number may optionally be "
+"followed by units."
+msgstr ""
+"El divisor es un número de coma flotante. Opcionalmente, el número puede ir "
+"seguido de unidades."
+
+msgid ""
 "The exponential decay time constant. The fuse dissipates 63.2 percent of "
 "accumulated energy in this duration."
 msgstr ""
 "La constante de tiempo de decaimiento exponencial. El fusible disipa el "
 "63,2% de la energía acumulada en esta duración."
 
 msgid "The filename supports the following replacements."
@@ -1798,17 +1808,14 @@
 
 msgid "The filename with optional replacements."
 msgstr "El nombre del archivo con sustituciones opcionales."
 
 msgid "The fixed default path for loading and saving files."
 msgstr "La ruta fija por defecto para cargar y guardar archivos."
 
-msgid "The flyout width in pixels."
-msgstr "La anchura del flyout en píxeles."
-
 msgid "The font scheme name."
 msgstr "El nombre del esquema de fuentes."
 
 msgid "The format string"
 msgstr "La cadena de formato"
 
 msgid "The fuse trips in Duration at this constant current."
```

### Comparing `joulescope_ui-1.1.6/joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.7/joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.2\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-18 14:15-0400\n"
+"POT-Creation-Date: 2024-05-06 17:27-0400\n"
 "PO-Revision-Date: 2024-04-04 14:45-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: es <LL@li.org>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-"Generated-By: Babel 2.14.0\n"
+"Generated-By: Babel 2.15.0\n"
 
 #: about.py:24
 msgid "About the Joulescope UI"
 msgstr "Acerca de la interfaz de usuario de Joulescope"
 
 #: about.py:25
 msgid "Version Information"
@@ -335,27 +335,27 @@
 msgid "Email"
 msgstr "Correo electrónico"
 
 #: error_window.py:103
 msgid "Description"
 msgstr "Descripción"
 
-#: error_window.py:112 widgets/waveform/waveform_widget.py:3347
+#: error_window.py:112 widgets/waveform/waveform_widget.py:3397
 msgid "Edit"
 msgstr "Editar"
 
 #: error_window.py:113
 msgid "View as Markdown"
 msgstr "Ver como Markdown"
 
 #: error_window.py:119
 msgid "Abort"
 msgstr "Abortar"
 
-#: error_window.py:120 main.py:365 widgets/settings/settings_widget.py:539
+#: error_window.py:120 main.py:363 widgets/settings/settings_widget.py:539
 msgid "View"
 msgstr "Ver"
 
 #: error_window.py:121
 msgid "Submit"
 msgstr "Enviar"
 
@@ -367,15 +367,15 @@
 msgid "Revert to previous configuration"
 msgstr "Volver a la configuración anterior"
 
 #: error_window.py:282
 msgid "Revert to defaults"
 msgstr "Volver a valores predeterminados"
 
-#: error_window.py:283 main.py:363 main.py:409
+#: error_window.py:283 main.py:361 main.py:407
 #: widgets/js220_cal/js220_cal_widget.py:38
 msgid "Exit"
 msgstr "Salir de"
 
 #: exporter.py:49 widgets/signal_record/signal_record_config_widget.py:148
 #: widgets/statistics_record/statistics_record_config_widget.py:111
 msgid "Directory"
@@ -646,165 +646,165 @@
 msgid "Do not show again"
 msgstr "No volver a mostrar"
 
 #: intel_graphics_dialog.py:91
 msgid "Intel graphics detected"
 msgstr "Gráficos Intel detectados"
 
-#: main.py:70 widgets/value/value_widget.py:653
+#: main.py:69 widgets/value/value_widget.py:660
 msgid "Multimeter"
 msgstr "Multímetro"
 
-#: main.py:71
+#: main.py:70
 msgid "Oscilloscope"
 msgstr "Osciloscopio"
 
-#: main.py:72 main.py:298 main.py:359 main.py:402
+#: main.py:71 main.py:296 main.py:357 main.py:400
 msgid "File"
 msgstr "Archivo"
 
-#: main.py:82
+#: main.py:81
 msgid "The UI status bar display mode"
 msgstr ""
 "El modo de visualización de la barra de estado de la interfaz de usuario"
 
-#: main.py:83
+#: main.py:82
 msgid ""
 "This setting controls the amount of detail shown on the status bar at the "
 "bottom of the UI window. You should usually leave this set to \"normal\" "
 "unless you want more detail concerning the UI internal operation."
 msgstr ""
 "Este ajuste controla la cantidad de detalles que se muestran en la barra de "
 "estado en la parte inferior de la ventana de interfaz de usuario. "
 "Normalmente debería dejarlo en \"normal\" a menos que desee más detalles "
 "sobre el funcionamiento interno de la interfaz de usuario."
 
-#: main.py:88 safe_mode.py:43
+#: main.py:87 safe_mode.py:43
 msgid "Normal"
 msgstr "Normal"
 
-#: main.py:89
+#: main.py:88
 msgid "Troubleshoot"
 msgstr "Solución de problemas"
 
-#: main.py:95
+#: main.py:94
 msgid "Enable developer mode."
 msgstr "Activa el modo desarrollador."
 
-#: main.py:108
+#: main.py:107
 msgid "PubSub utilization"
 msgstr "Utilización de PubSub"
 
-#: main.py:109
+#: main.py:108
 msgid ""
 "Display the number of actions processed by the publish-subscribe broker in "
 "each second."
 msgstr ""
 "Muestra el número de acciones procesadas por el broker publish-subscribe en "
 "cada segundo."
 
-#: main.py:114
+#: main.py:113
 msgid "CPU utilization"
 msgstr "Utilización de la CPU"
 
-#: main.py:115
+#: main.py:114
 msgid ""
 "Display the CPU utilization by this application and the total CPU "
 "utilization by all applications. The value is displayed in percent."
 msgstr ""
 "Muestra la utilización de la CPU por esta aplicación y la utilización total "
 "de la CPU por todas las aplicaciones. El valor se muestra en porcentaje."
 
-#: main.py:121
+#: main.py:120
 msgid "Memory utilization"
 msgstr "Utilización de la memoria"
 
-#: main.py:122
+#: main.py:121
 msgid ""
 "Display the memory (RAM) utilization by this application and by all "
 "applications. The value is displayed in percent."
 msgstr ""
 "Muestra la utilización de la memoria (RAM) por esta aplicación y por todas "
 "las aplicaciones. El valor se muestra en porcentaje."
 
-#: main.py:216
+#: main.py:214
 msgid "UI"
 msgstr "INTERFAZ DE USUARIO"
 
-#: main.py:330
+#: main.py:328
 msgid "Help"
 msgstr "Ayuda"
 
-#: main.py:331 widgets/hamburger/hamburger_widget.py:21
+#: main.py:329 widgets/hamburger/hamburger_widget.py:21
 msgid "Getting Started"
 msgstr "Primeros pasos"
 
-#: main.py:332
+#: main.py:330
 msgid "User's Guide"
 msgstr "Guía del usuario"
 
-#: main.py:333 widgets/hamburger/hamburger_widget.py:22
+#: main.py:331 widgets/hamburger/hamburger_widget.py:22
 msgid "Changelog"
 msgstr "Registro de cambios"
 
-#: main.py:334 widgets/help/help_widget.py:59
+#: main.py:332 widgets/help/help_widget.py:59
 msgid "Report Issue"
 msgstr "Número de informe"
 
-#: main.py:335
+#: main.py:333
 msgid "View logs..."
 msgstr "Ver registros..."
 
-#: main.py:336 widgets/hamburger/hamburger_widget.py:23
+#: main.py:334 widgets/hamburger/hamburger_widget.py:23
 msgid "Credits"
 msgstr "Créditos"
 
-#: main.py:337 widgets/hamburger/hamburger_widget.py:24
+#: main.py:335 widgets/hamburger/hamburger_widget.py:24
 msgid "About"
 msgstr "Acerca de"
 
-#: main.py:360
+#: main.py:358
 msgid "Open"
 msgstr "Abrir"
 
-#: main.py:361
+#: main.py:359
 msgid "Open recent"
 msgstr "Abrir reciente"
 
-#: main.py:362 main.py:408
+#: main.py:360 main.py:406
 msgid "Clear config and exit"
 msgstr "Borrar configuración y salir"
 
-#: main.py:366 widgets/settings/settings_widget.py:541
+#: main.py:364 widgets/settings/settings_widget.py:541
 msgid "Widgets"
 msgstr "Widgets"
 
-#: main.py:367
+#: main.py:365
 msgid "Tools"
 msgstr "Herramientas"
 
-#: main.py:368
+#: main.py:366
 msgid "Clear Accumulators"
 msgstr "Acumuladores transparentes"
 
-#: main.py:403
+#: main.py:401
 msgid "Info"
 msgstr "Información"
 
-#: main.py:404 widget_tools.py:92 widgets/settings/settings_widget.py:31
+#: main.py:402 widget_tools.py:92 widgets/settings/settings_widget.py:31
 #: widgets/settings/settings_widget.py:574
 #: widgets/sidebar/sidebar_widget.py:41
 msgid "Settings"
 msgstr "Ajustes"
 
-#: main.py:693
+#: main.py:710
 msgid "Manage"
 msgstr "Gestione"
 
-#: main.py:730
+#: main.py:747
 msgid "Select file to open"
 msgstr "Seleccionar archivo para abrir"
 
 #: paths.py:30 styles/manager.py:46
 msgid "The name for this widget."
 msgstr "El nombre de este widget."
 
@@ -945,47 +945,47 @@
 msgid "Source"
 msgstr "Fuente"
 
 #: units.py:35
 msgid "Use the application defaults"
 msgstr "Utilizar los valores predeterminados de la aplicación"
 
-#: view.py:68
+#: view.py:72
 msgid "The active theme."
 msgstr "El tema activo."
 
-#: view.py:70
+#: view.py:74
 msgid "Joulescope standard theme"
 msgstr "Tema estándar de Joulescope"
 
-#: view.py:70
+#: view.py:74
 msgid "System OS-specific theme"
 msgstr "Tema específico del sistema operativo"
 
-#: view.py:75
+#: view.py:79
 msgid "The color scheme name."
 msgstr "El nombre de la combinación de colores."
 
-#: view.py:77
+#: view.py:81
 msgid "Dark background"
 msgstr "Fondo oscuro"
 
-#: view.py:77
+#: view.py:81
 msgid "Light background"
 msgstr "Fondo luminoso"
 
-#: view.py:81
+#: view.py:85
 msgid "The font scheme name."
 msgstr "El nombre del esquema de fuentes."
 
-#: view.py:83
+#: view.py:87
 msgid "Joulescope standard font theme"
 msgstr "Tema de fuente estándar de Joulescope"
 
-#: view.py:102 widgets/view_manager/view_manager_widget.py:146
+#: view.py:106 widgets/view_manager/view_manager_widget.py:146
 msgid "New View"
 msgstr "Nueva vista"
 
 #: zip_inspector.py:23
 msgid "ZIP Inspector"
 msgstr "Inspector ZIP"
 
@@ -1103,15 +1103,15 @@
 "Cuando está activado, la corriente fluye entre los terminales de corriente. "
 "Cuando está desactivado, la corriente no puede fluir entre los terminales de"
 " corriente. En configuraciones de sistema comunes, esto inhibe la "
 "alimentación del objetivo, que puede utilizarse para reiniciar el "
 "dispositivo objetivo."
 
 #: devices/jsdrv/js110.py:147 devices/jsdrv/js220.py:163
-#: widgets/waveform/waveform_widget.py:110
+#: widgets/waveform/waveform_widget.py:109
 msgid "Current range"
 msgstr "Rango de corriente"
 
 #: devices/jsdrv/js110.py:149
 msgid ""
 "Configure the J110's current range. Most applications should use the "
 "default, \"auto\"."
@@ -1259,33 +1259,33 @@
 "mean. This value is ignored for all other IRF types."
 msgstr ""
 "El número de muestras después de la ventana de rango de corriente utilizada "
 "para determinar la media. Este valor se ignora para todos los demás tipos de"
 " IRF."
 
 #: devices/jsdrv/js110.py:269 devices/jsdrv/js220.py:332
-#: widgets/device_control/fuse.py:103 widgets/waveform/waveform_widget.py:105
+#: widgets/device_control/fuse.py:103 widgets/waveform/waveform_widget.py:104
 msgid "Current"
 msgstr "Corriente"
 
 #: devices/jsdrv/js110.py:270 devices/jsdrv/js220.py:333
 msgid "Enable the current signal streaming."
 msgstr "Habilita la transmisión de la señal de corriente."
 
 #: devices/jsdrv/js110.py:278 devices/jsdrv/js220.py:341
-#: widgets/waveform/waveform_widget.py:106
+#: widgets/waveform/waveform_widget.py:105
 msgid "Voltage"
 msgstr "Tensión"
 
 #: devices/jsdrv/js110.py:279 devices/jsdrv/js220.py:342
 msgid "Enable the voltage signal streaming."
 msgstr "Habilita la transmisión de señales de tensión."
 
 #: devices/jsdrv/js110.py:287 devices/jsdrv/js220.py:350
-#: widgets/waveform/waveform_widget.py:107
+#: widgets/waveform/waveform_widget.py:106
 msgid "Power"
 msgstr "Potencia"
 
 #: devices/jsdrv/js110.py:288 devices/jsdrv/js220.py:351
 msgid "Enable the power signal streaming."
 msgstr "Habilita la transmisión de señales de potencia."
 
@@ -1501,15 +1501,15 @@
 msgid "GPI 3"
 msgstr "GPI 3"
 
 #: devices/jsdrv/js220.py:402
 msgid "Enable the general purpose input 3 signal streaming."
 msgstr "Habilita el flujo de señales de entrada 3 de propósito general."
 
-#: devices/jsdrv/js220.py:410 widgets/waveform/waveform_widget.py:124
+#: devices/jsdrv/js220.py:410 widgets/waveform/waveform_widget.py:123
 msgid "Trigger input"
 msgstr "Entrada de disparo"
 
 #: devices/jsdrv/js220.py:411
 msgid "Enable the trigger input signal streaming."
 msgstr "Habilita la transmisión de la señal de entrada de disparo."
 
@@ -1520,15 +1520,15 @@
 #: devices/jsdrv/jsdrv_stream_buffer.py:44
 #: devices/jsdrv/jsdrv_stream_buffer.py:93
 #: devices/jsdrv/jsdrv_stream_buffer.py:107 plugins/selector.py:58
 #: widgets/settings/settings_widget.py:85
 #: widgets/settings/settings_widget.py:266
 #: widgets/settings/settings_widget.py:364
 #: widgets/settings/settings_widget.py:431
-#: widgets/waveform/waveform_widget.py:3062
+#: widgets/waveform/waveform_widget.py:3104
 msgid "Name"
 msgstr "Nombre"
 
 #: devices/jsdrv/jsdrv_stream_buffer.py:45
 msgid "Joulescope stream buffer"
 msgstr "Búfer de corriente de Joulescope"
 
@@ -1752,15 +1752,15 @@
 
 #: widgets/accumulator/accumulator_widget.py:27
 #: widgets/value/value_widget.py:31
 msgid "The statistics data stream source."
 msgstr "La fuente de flujo de datos estadísticos."
 
 #: widgets/accumulator/accumulator_widget.py:32
-#: widgets/value/value_widget.py:74
+#: widgets/value/value_widget.py:81
 msgid "The signal to display."
 msgstr "La señal a visualizar."
 
 #: widgets/accumulator/accumulator_widget.py:34
 msgid "charge"
 msgstr "carga"
 
@@ -1844,15 +1844,15 @@
 
 #: widgets/developer/publish_spy_widget.py:20
 #: widgets/developer/publish_spy_widget.py:21
 msgid "Topic"
 msgstr "Tema"
 
 #: widgets/developer/publish_spy_widget.py:21
-#: widgets/settings/settings_widget.py:87 widgets/value/value_widget.py:662
+#: widgets/settings/settings_widget.py:87 widgets/value/value_widget.py:669
 msgid "Value"
 msgstr "Valor"
 
 #: widgets/developer/publish_spy_widget.py:24
 msgid "Publish Spy"
 msgstr "Publicar Espía"
 
@@ -1882,15 +1882,15 @@
 
 #: widgets/device_control/device_update_dialog.py:24
 #: widgets/device_control/device_update_dialog.py:45
 msgid "Update"
 msgstr "Actualización"
 
 #: widgets/device_control/device_update_dialog.py:25
-#: widgets/value/value_widget.py:147
+#: widgets/value/value_widget.py:155
 msgid "Device"
 msgstr "Dispositivo"
 
 #: widgets/device_control/device_update_dialog.py:27
 #: widgets/progress_bar/progress_bar_widget.py:59
 msgid "Progress"
 msgstr "Progreso"
@@ -2417,18 +2417,14 @@
 msgid "Click to display additional settings and actions."
 msgstr "Haga clic para ver ajustes y acciones adicionales."
 
 #: widgets/sidebar/sidebar_widget.py:60
 msgid "sidebar"
 msgstr "barra lateral"
 
-#: widgets/sidebar/sidebar_widget.py:68
-msgid "The flyout width in pixels."
-msgstr "La anchura del flyout en píxeles."
-
 #: widgets/signal_record/disk_full_dialog.py:19
 msgid "The disk is full"
 msgstr "El disco está lleno"
 
 #: widgets/signal_record/signal_record.py:57
 msgid "Could not open file for write"
 msgstr "No se pudo abrir el archivo para escribir"
@@ -2455,15 +2451,15 @@
 msgid "StatisticsRecordConfig"
 msgstr "EstadísticasRegistroConfig"
 
 #: widgets/statistics_record/statistics_record_config_widget.py:123
 msgid "Time Format"
 msgstr "Formato de tiempo"
 
-#: widgets/trigger/trigger_widget.py:41 widgets/value/value_widget.py:87
+#: widgets/trigger/trigger_widget.py:41 widgets/value/value_widget.py:94
 msgid "Select the source device"
 msgstr "Seleccione el dispositivo fuente"
 
 #: widgets/trigger/trigger_widget.py:42
 msgid "The device to use for the start condition and stop condition."
 msgstr ""
 "El dispositivo a utilizar para la condición de arranque y la condición de "
@@ -2637,85 +2633,97 @@
 msgid "Show the statistics fields at the right."
 msgstr "Muestra los campos de estadísticas a la derecha."
 
 #: widgets/value/value_widget.py:51
 msgid "Show a leading + or - sign."
 msgstr "Muestra un signo + o - inicial."
 
-#: widgets/value/value_widget.py:88
+#: widgets/value/value_widget.py:62
+msgid "Divide the quantity by this value."
+msgstr "Divida la cantidad por este valor."
+
+#: widgets/value/value_widget.py:63
+msgid ""
+"The divisor is a floating point number. The number may optionally be "
+"followed by units."
+msgstr ""
+"El divisor es un número de coma flotante. Opcionalmente, el número puede ir "
+"seguido de unidades."
+
+#: widgets/value/value_widget.py:95
 msgid ""
 "The values displayed by this widget come from a single source device. Select"
 " the source device here."
 msgstr ""
 "Los valores mostrados por este widget proceden de un único dispositivo "
 "fuente. Seleccione aquí el dispositivo de origen."
 
-#: widgets/value/value_widget.py:94
+#: widgets/value/value_widget.py:101
 msgid "Hold the display"
 msgstr "Mantener la pantalla"
 
-#: widgets/value/value_widget.py:96
+#: widgets/value/value_widget.py:103
 msgid "When selected, prevent the display from updating."
 msgstr "Cuando se selecciona, evita que la pantalla se actualice."
 
-#: widgets/value/value_widget.py:97
+#: widgets/value/value_widget.py:104
 msgid ""
 "The UI also includes a global statistics hold button on the sidebar. When "
 "the global statistics hold button is selected, this button is disabled and "
 "has no effect."
 msgstr ""
 "La interfaz de usuario también incluye un botón de retención de estadísticas"
 " globales en la barra lateral. Cuando se selecciona el botón de retención de"
 " estadísticas globales, este botón se desactiva y no tiene ningún efecto."
 
-#: widgets/value/value_widget.py:100
+#: widgets/value/value_widget.py:107
 msgid ""
 "The displayed values normally update with each new statistics data computed "
 "by the device. When this button is selected, the display will not be "
 "updated. However, the statistics will continue accumulate and accrue (if "
 "selected)."
 msgstr ""
 "Los valores mostrados normalmente se actualizan con cada nuevo dato "
 "estadístico calculado por el dispositivo. Cuando se selecciona este botón, "
 "la pantalla no se actualiza. Sin embargo, las estadísticas seguirán "
 "acumulándose y acumulándose (si está seleccionado)."
 
-#: widgets/value/value_widget.py:107
+#: widgets/value/value_widget.py:114
 msgid "Accrue values over time"
 msgstr "Acumula valores a lo largo del tiempo"
 
-#: widgets/value/value_widget.py:109
+#: widgets/value/value_widget.py:116
 msgid ""
 "Current, voltage, and power are normally computed over a single statistics "
 "frequency interval. Press this button to accrue the values indefinitely. "
 "Press again to return to normal operation."
 msgstr ""
 "La corriente, la tensión y la potencia se calculan normalmente en un único "
 "intervalo de frecuencia estadística. Pulse este botón para acumular los "
 "valores indefinidamente. Pulse de nuevo para volver al funcionamiento "
 "normal."
 
-#: widgets/value/value_widget.py:113
+#: widgets/value/value_widget.py:120
 msgid ""
 "Note that this button does not affect the charge and energy accumulation. "
 "Both accumulate indefinitely regardless of this button state."
 msgstr ""
 "Tenga en cuenta que este botón no afecta a la acumulación de carga y "
 "energía. Ambas se acumulan indefinidamente independientemente del estado de "
 "este botón."
 
-#: widgets/value/value_widget.py:195
+#: widgets/value/value_widget.py:203
 msgid "Not present"
 msgstr "No presente"
 
-#: widgets/value/value_widget.py:215
+#: widgets/value/value_widget.py:223
 msgid "Hold"
 msgstr "Mantenga"
 
-#: widgets/value/value_widget.py:223
+#: widgets/value/value_widget.py:231
 msgid "Accrue"
 msgstr "Aumento de"
 
 #: widgets/view_manager/view_manager_widget.py:108
 #: widgets/view_manager/view_manager_widget.py:174
 msgid "View Manager"
 msgstr "Administrador de vistas"
@@ -2761,34 +2769,34 @@
 msgstr "triángulo derecho"
 
 #: widgets/waveform/text_annotation.py:62
 msgid "triangle left"
 msgstr "triángulo izquierdo"
 
 #: widgets/waveform/text_annotation.py:66
-#: widgets/waveform/waveform_widget.py:3008
+#: widgets/waveform/waveform_widget.py:3050
 msgid "Manual"
 msgstr "Manual"
 
 #: widgets/waveform/text_annotation.py:67
 msgid "Centered"
 msgstr "Centrado"
 
 #: widgets/waveform/text_annotation.py:99
-#: widgets/waveform/waveform_widget.py:3123
+#: widgets/waveform/waveform_widget.py:3167
 msgid "Text"
 msgstr "Texto"
 
 #: widgets/waveform/text_annotation.py:107
-#: widgets/waveform/waveform_widget.py:3348
+#: widgets/waveform/waveform_widget.py:3398
 msgid "Show text"
 msgstr "Mostrar texto"
 
 #: widgets/waveform/text_annotation.py:116
-#: widgets/waveform/waveform_widget.py:3360
+#: widgets/waveform/waveform_widget.py:3410
 msgid "Shape"
 msgstr "Forma"
 
 #: widgets/waveform/text_annotation.py:126
 msgid "Y Mode"
 msgstr "Modo Y"
 
@@ -2986,323 +2994,323 @@
 "\"default\" will use the default source which is normally configured using "
 "the Device Control widget."
 msgstr ""
 "\"por defecto\" utilizará la fuente por defecto que normalmente se configura"
 " utilizando el widget de Control de Dispositivos."
 
 #: widgets/waveform/waveform_source_widget.py:104
-#: widgets/waveform/waveform_widget.py:402
-#: widgets/waveform/waveform_widget.py:479
+#: widgets/waveform/waveform_widget.py:401
+#: widgets/waveform/waveform_widget.py:478
 msgid "off"
 msgstr "off"
 
-#: widgets/waveform/waveform_widget.py:44
+#: widgets/waveform/waveform_widget.py:43
 msgid "Waveform"
 msgstr "Forma de onda"
 
-#: widgets/waveform/waveform_widget.py:120
+#: widgets/waveform/waveform_widget.py:119
 msgid "General purpose input 0"
 msgstr "Entrada de propósito general 0"
 
-#: widgets/waveform/waveform_widget.py:121
+#: widgets/waveform/waveform_widget.py:120
 msgid "General purpose input 1"
 msgstr "Entrada de propósito general 1"
 
-#: widgets/waveform/waveform_widget.py:122
+#: widgets/waveform/waveform_widget.py:121
 msgid "General purpose input 2"
 msgstr "Entrada de propósito general 2"
 
-#: widgets/waveform/waveform_widget.py:123
+#: widgets/waveform/waveform_widget.py:122
 msgid "General purpose input 3"
 msgstr "Entrada de propósito general 3"
 
-#: widgets/waveform/waveform_widget.py:358
+#: widgets/waveform/waveform_widget.py:357
 msgid "The source filter string."
 msgstr "La cadena de filtros de la fuente."
 
-#: widgets/waveform/waveform_widget.py:369
+#: widgets/waveform/waveform_widget.py:368
 msgid "The trace width."
 msgstr "La anchura de la traza."
 
-#: widgets/waveform/waveform_widget.py:384
+#: widgets/waveform/waveform_widget.py:383
 msgid "The target frames per second."
 msgstr "El objetivo de imágenes por segundo."
 
-#: widgets/waveform/waveform_widget.py:386
+#: widgets/waveform/waveform_widget.py:385
 msgid "vsync"
 msgstr "vsync"
 
-#: widgets/waveform/waveform_widget.py:387
+#: widgets/waveform/waveform_widget.py:386
 msgid "20 Hz"
 msgstr "20 Hz"
 
-#: widgets/waveform/waveform_widget.py:388
+#: widgets/waveform/waveform_widget.py:387
 msgid "10 Hz"
 msgstr "10 Hz"
 
-#: widgets/waveform/waveform_widget.py:389
+#: widgets/waveform/waveform_widget.py:388
 msgid "5 Hz"
 msgstr "5 Hz"
 
-#: widgets/waveform/waveform_widget.py:395
+#: widgets/waveform/waveform_widget.py:394
 msgid "The minimum interval between repaint in milliseconds."
 msgstr "El intervalo mínimo entre repintados en milisegundos."
 
-#: widgets/waveform/waveform_widget.py:400
+#: widgets/waveform/waveform_widget.py:399
 msgid "Show the minimum and maximum extents fill."
 msgstr "Muestra las extensiones mínima y máxima de llenado."
 
-#: widgets/waveform/waveform_widget.py:403
+#: widgets/waveform/waveform_widget.py:402
 msgid "lines"
 msgstr "líneas"
 
-#: widgets/waveform/waveform_widget.py:404
+#: widgets/waveform/waveform_widget.py:403
 msgid "fill 1"
 msgstr "llenar 1"
 
-#: widgets/waveform/waveform_widget.py:405
+#: widgets/waveform/waveform_widget.py:404
 msgid "fill 2"
 msgstr "llenar 2"
 
-#: widgets/waveform/waveform_widget.py:411
+#: widgets/waveform/waveform_widget.py:410
 msgid "Show the frames per second."
 msgstr "Muestra las imágenes por segundo."
 
-#: widgets/waveform/waveform_widget.py:416
+#: widgets/waveform/waveform_widget.py:415
 msgid "Show the statistics on mouse hover."
 msgstr "Muestra las estadísticas al pasar el ratón por encima."
 
-#: widgets/waveform/waveform_widget.py:421
+#: widgets/waveform/waveform_widget.py:420
 msgid "Show the plot statistics on the right."
 msgstr "Muestra las estadísticas del gráfico a la derecha."
 
-#: widgets/waveform/waveform_widget.py:426
+#: widgets/waveform/waveform_widget.py:425
 msgid "Show frequency for dual markers and statistics."
 msgstr "Muestra la frecuencia para marcadores duales y estadísticas."
 
-#: widgets/waveform/waveform_widget.py:431
+#: widgets/waveform/waveform_widget.py:430
 msgid "The quantities to display by default."
 msgstr "Las cantidades a mostrar por defecto."
 
-#: widgets/waveform/waveform_widget.py:437
+#: widgets/waveform/waveform_widget.py:436
 msgid "The precision to display in digits."
 msgstr "La precisión a mostrar en dígitos."
 
-#: widgets/waveform/waveform_widget.py:443
+#: widgets/waveform/waveform_widget.py:442
 msgid "Use OpenGL rendering."
 msgstr "Utilice el renderizado OpenGL."
 
-#: widgets/waveform/waveform_widget.py:454
+#: widgets/waveform/waveform_widget.py:453
 msgid "Pin the left side (oldest) data so that it stays in view."
 msgstr ""
 "Fije los datos del lado izquierdo (más antiguos) para que permanezcan a la "
 "vista."
 
-#: widgets/waveform/waveform_widget.py:459
+#: widgets/waveform/waveform_widget.py:458
 msgid "Pin the right side (newest) data so that it stays in view."
 msgstr ""
 "Fija los datos del lado derecho (los más nuevos) para que permanezcan a la "
 "vista."
 
-#: widgets/waveform/waveform_widget.py:464
+#: widgets/waveform/waveform_widget.py:463
 msgid "The waveform state."
 msgstr "El estado de la forma de onda."
 
-#: widgets/waveform/waveform_widget.py:470
+#: widgets/waveform/waveform_widget.py:469
 msgid "The annotations."
 msgstr "Las anotaciones."
 
-#: widgets/waveform/waveform_widget.py:476
+#: widgets/waveform/waveform_widget.py:475
 msgid "Control location"
 msgstr "Lugar de control"
 
-#: widgets/waveform/waveform_widget.py:480
+#: widgets/waveform/waveform_widget.py:479
 msgid "top"
 msgstr "top"
 
-#: widgets/waveform/waveform_widget.py:481
+#: widgets/waveform/waveform_widget.py:480
 msgid "bottom"
 msgstr "inferior"
 
-#: widgets/waveform/waveform_widget.py:486
+#: widgets/waveform/waveform_widget.py:485
 msgid "The signal quantity to show in the summary."
 msgstr "La cantidad de señal a mostrar en el resumen."
 
-#: widgets/waveform/waveform_widget.py:492
+#: widgets/waveform/waveform_widget.py:491
 msgid "X-axis annotation mode"
 msgstr "Modo de anotación en el eje X"
 
-#: widgets/waveform/waveform_widget.py:495
-#: widgets/waveform/waveform_widget.py:2888
+#: widgets/waveform/waveform_widget.py:494
+#: widgets/waveform/waveform_widget.py:2930
 msgid "Absolute"
 msgstr "Absoluto"
 
-#: widgets/waveform/waveform_widget.py:496
-#: widgets/waveform/waveform_widget.py:2893
+#: widgets/waveform/waveform_widget.py:495
+#: widgets/waveform/waveform_widget.py:2935
 msgid "Relative"
 msgstr "Relativa"
 
-#: widgets/waveform/waveform_widget.py:502
+#: widgets/waveform/waveform_widget.py:501
 msgid "The available subsources."
 msgstr "Las subfuentes disponibles."
 
-#: widgets/waveform/waveform_widget.py:508
+#: widgets/waveform/waveform_widget.py:507
 msgid "The selected subsources for each trace."
 msgstr "Las subfuentes seleccionadas para cada traza."
 
-#: widgets/waveform/waveform_widget.py:514
+#: widgets/waveform/waveform_widget.py:513
 msgid "The trace priority: highest int value on top, None is off."
 msgstr ""
 "La prioridad de la traza: el valor int más alto en la parte superior, "
 "Ninguno está desactivado."
 
-#: widgets/waveform/waveform_widget.py:2834
-#: widgets/waveform/waveform_widget.py:3135
+#: widgets/waveform/waveform_widget.py:2877
+#: widgets/waveform/waveform_widget.py:3179
 msgid "Save image to file"
 msgstr "Guardar imagen en archivo"
 
-#: widgets/waveform/waveform_widget.py:2882
-#: widgets/waveform/waveform_widget.py:2951
+#: widgets/waveform/waveform_widget.py:2924
+#: widgets/waveform/waveform_widget.py:2993
 msgid "Single marker"
 msgstr "Marcador único"
 
-#: widgets/waveform/waveform_widget.py:2883
-#: widgets/waveform/waveform_widget.py:2952
+#: widgets/waveform/waveform_widget.py:2925
+#: widgets/waveform/waveform_widget.py:2994
 msgid "Dual markers"
 msgstr "Marcadores duales"
 
-#: widgets/waveform/waveform_widget.py:2885
+#: widgets/waveform/waveform_widget.py:2927
 msgid "Mode"
 msgstr "Modo"
 
-#: widgets/waveform/waveform_widget.py:2898
-#: widgets/waveform/waveform_widget.py:2953
-#: widgets/waveform/waveform_widget.py:3111
-#: widgets/waveform/waveform_widget.py:3129
+#: widgets/waveform/waveform_widget.py:2940
+#: widgets/waveform/waveform_widget.py:2995
+#: widgets/waveform/waveform_widget.py:3155
+#: widgets/waveform/waveform_widget.py:3173
 msgid "Clear all"
 msgstr "Borrar todo"
 
-#: widgets/waveform/waveform_widget.py:2909
-#: widgets/waveform/waveform_widget.py:2998
-#: widgets/waveform/waveform_widget.py:3117
+#: widgets/waveform/waveform_widget.py:2951
+#: widgets/waveform/waveform_widget.py:3040
+#: widgets/waveform/waveform_widget.py:3161
 msgid "Annotations"
 msgstr "Anotaciones"
 
-#: widgets/waveform/waveform_widget.py:3001
+#: widgets/waveform/waveform_widget.py:3043
 msgid "Range"
 msgstr "Gama"
 
-#: widgets/waveform/waveform_widget.py:3005
-#: widgets/waveform/waveform_widget.py:3328
+#: widgets/waveform/waveform_widget.py:3047
+#: widgets/waveform/waveform_widget.py:3378
 msgid "Auto"
 msgstr "Auto"
 
-#: widgets/waveform/waveform_widget.py:3011
+#: widgets/waveform/waveform_widget.py:3053
 msgid "Exact"
 msgstr "Exacto"
 
-#: widgets/waveform/waveform_widget.py:3020
+#: widgets/waveform/waveform_widget.py:3062
 msgid "Scale"
 msgstr "Escala"
 
-#: widgets/waveform/waveform_widget.py:3023
+#: widgets/waveform/waveform_widget.py:3065
 msgid "Linear"
 msgstr "Lineal"
 
-#: widgets/waveform/waveform_widget.py:3028
+#: widgets/waveform/waveform_widget.py:3070
 msgid "Logarithmic"
 msgstr "Logarítmica"
 
-#: widgets/waveform/waveform_widget.py:3036
+#: widgets/waveform/waveform_widget.py:3078
 msgid "Logarithmic zero"
 msgstr "Cero logarítmico"
 
-#: widgets/waveform/waveform_widget.py:3050
+#: widgets/waveform/waveform_widget.py:3092
 msgid "Preferred prefix"
 msgstr "Prefijo preferido"
 
-#: widgets/waveform/waveform_widget.py:3108
+#: widgets/waveform/waveform_widget.py:3152
 msgid "Add"
 msgstr "Añadir"
 
-#: widgets/waveform/waveform_widget.py:3109
+#: widgets/waveform/waveform_widget.py:3153
 msgid "Hide all text"
 msgstr "Ocultar todo el texto"
 
-#: widgets/waveform/waveform_widget.py:3110
+#: widgets/waveform/waveform_widget.py:3154
 msgid "Show all text"
 msgstr "Mostrar todo el texto"
 
-#: widgets/waveform/waveform_widget.py:3118
+#: widgets/waveform/waveform_widget.py:3162
 msgid "Vertical"
 msgstr "Vertical"
 
-#: widgets/waveform/waveform_widget.py:3121
+#: widgets/waveform/waveform_widget.py:3165
 msgid "Horizontal"
 msgstr "Horizontal"
 
-#: widgets/waveform/waveform_widget.py:3127
+#: widgets/waveform/waveform_widget.py:3171
 msgid "Save"
 msgstr "Guardar"
 
-#: widgets/waveform/waveform_widget.py:3132
+#: widgets/waveform/waveform_widget.py:3176
 msgid "Y-axis auto range"
 msgstr "Rango automático del eje Y"
 
-#: widgets/waveform/waveform_widget.py:3136
+#: widgets/waveform/waveform_widget.py:3180
 msgid "Copy image to clipboard"
 msgstr "Copiar imagen al portapapeles"
 
-#: widgets/waveform/waveform_widget.py:3137
+#: widgets/waveform/waveform_widget.py:3181
 msgid "Export visible data"
 msgstr "Exportación de datos visibles"
 
-#: widgets/waveform/waveform_widget.py:3138
+#: widgets/waveform/waveform_widget.py:3182
 msgid "Export all data"
 msgstr "Exportar todos los datos"
 
-#: widgets/waveform/waveform_widget.py:3304
+#: widgets/waveform/waveform_widget.py:3354
 msgid "Export"
 msgstr "Exportar"
 
-#: widgets/waveform/waveform_widget.py:3305
+#: widgets/waveform/waveform_widget.py:3355
 msgid "Analysis"
 msgstr "Análisis"
 
-#: widgets/waveform/waveform_widget.py:3313
+#: widgets/waveform/waveform_widget.py:3363
 msgid "Interval"
 msgstr "Intervalo"
 
-#: widgets/waveform/waveform_widget.py:3322
+#: widgets/waveform/waveform_widget.py:3372
 msgid "Zoom"
 msgstr "Zoom"
 
-#: widgets/waveform/waveform_widget.py:3326
+#: widgets/waveform/waveform_widget.py:3376
 msgid "Show statistics"
 msgstr "Mostrar estadísticas"
 
-#: widgets/waveform/waveform_widget.py:3331
+#: widgets/waveform/waveform_widget.py:3381
 msgid "Left"
 msgstr "Izquierda"
 
-#: widgets/waveform/waveform_widget.py:3334
+#: widgets/waveform/waveform_widget.py:3384
 msgid "Right"
 msgstr "Derecha"
 
-#: widgets/waveform/waveform_widget.py:3337
+#: widgets/waveform/waveform_widget.py:3387
 msgid "Off"
 msgstr "Apagado"
 
-#: widgets/waveform/waveform_widget.py:3340
-#: widgets/waveform/waveform_widget.py:3368
-#: widgets/waveform/waveform_widget.py:3397
+#: widgets/waveform/waveform_widget.py:3390
+#: widgets/waveform/waveform_widget.py:3418
+#: widgets/waveform/waveform_widget.py:3448
 msgid "Remove"
 msgstr "Eliminar"
 
-#: widgets/waveform/waveform_widget.py:3351
+#: widgets/waveform/waveform_widget.py:3401
 msgid "Y mode"
 msgstr "Modo Y"
 
 #: widgets/waveform/y_range_widget.py:67
 msgid "max"
 msgstr "máx"
```

### Comparing `joulescope_ui-1.1.6/joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.7/joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.2\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-18 14:15-0400\n"
+"POT-Creation-Date: 2024-05-06 17:27-0400\n"
 "PO-Revision-Date: 2024-04-04 14:45-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: fr\n"
 "Language-Team: fr <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.14.0\n"
+"Generated-By: Babel 2.15.0\n"
 
 msgid "\"3.3 V\" uses an internally-generated 3.3V reference voltage."
 msgstr ""
 "\"3,3 V\" utilise une tension de référence de 3,3 V générée en interne."
 
 msgid "\"NaN\" sets all samples in the window to NaN."
 msgstr "\"NaN\" définit tous les échantillons de la fenêtre à NaN."
@@ -655,14 +655,17 @@
 msgid ""
 "Display the number of actions processed by the publish-subscribe broker in "
 "each second."
 msgstr ""
 "Affiche le nombre d'actions traitées par le courtier de publication et "
 "d'abonnement chaque seconde."
 
+msgid "Divide the quantity by this value."
+msgstr "Divisez la quantité par cette valeur."
+
 msgid "Do not show again"
 msgstr "Ne plus afficher"
 
 msgid "Do not use any USB hubs, docks or adapters"
 msgstr ""
 "N'utilisez pas de concentrateurs, de stations d'accueil ou d'adaptateurs USB."
 
@@ -1791,14 +1794,21 @@
 msgstr ""
 "Les valeurs affichées sont normalement mises à jour avec chaque nouvelle "
 "donnée statistique calculée par l'appareil. Lorsque ce bouton est "
 "sélectionné, l'affichage n'est pas mis à jour. Cependant, les statistiques "
 "continueront à s'accumuler et à se cumuler (si sélectionné)."
 
 msgid ""
+"The divisor is a floating point number. The number may optionally be "
+"followed by units."
+msgstr ""
+"Le diviseur est un nombre à virgule flottante. Le nombre peut éventuellement "
+"être suivi d'unités."
+
+msgid ""
 "The exponential decay time constant. The fuse dissipates 63.2 percent of "
 "accumulated energy in this duration."
 msgstr ""
 "La constante de temps de la décroissance exponentielle. Le fusible dissipe "
 "63,2 % de l'énergie accumulée pendant cette durée."
 
 msgid "The filename supports the following replacements."
@@ -1808,17 +1818,14 @@
 msgstr "Le nom du fichier avec des remplacements optionnels."
 
 msgid "The fixed default path for loading and saving files."
 msgstr ""
 "Le chemin fixe par défaut pour le chargement et l'enregistrement des "
 "fichiers."
 
-msgid "The flyout width in pixels."
-msgstr "La largeur du flyout en pixels."
-
 msgid "The font scheme name."
 msgstr "Le nom de la police de caractères."
 
 msgid "The format string"
 msgstr "La chaîne de format"
 
 msgid "The fuse trips in Duration at this constant current."
```

### Comparing `joulescope_ui-1.1.6/joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.7/joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.2\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-18 14:15-0400\n"
+"POT-Creation-Date: 2024-05-06 17:27-0400\n"
 "PO-Revision-Date: 2024-04-04 14:45-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: fr <LL@li.org>\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
-"Generated-By: Babel 2.14.0\n"
+"Generated-By: Babel 2.15.0\n"
 
 #: about.py:24
 msgid "About the Joulescope UI"
 msgstr "A propos de l'interface utilisateur Joulescope"
 
 #: about.py:25
 msgid "Version Information"
@@ -338,27 +338,27 @@
 msgid "Email"
 msgstr "Courriel"
 
 #: error_window.py:103
 msgid "Description"
 msgstr "Description"
 
-#: error_window.py:112 widgets/waveform/waveform_widget.py:3347
+#: error_window.py:112 widgets/waveform/waveform_widget.py:3397
 msgid "Edit"
 msgstr "Editer"
 
 #: error_window.py:113
 msgid "View as Markdown"
 msgstr "Voir comme Markdown"
 
 #: error_window.py:119
 msgid "Abort"
 msgstr "Abort"
 
-#: error_window.py:120 main.py:365 widgets/settings/settings_widget.py:539
+#: error_window.py:120 main.py:363 widgets/settings/settings_widget.py:539
 msgid "View"
 msgstr "Voir"
 
 #: error_window.py:121
 msgid "Submit"
 msgstr "Soumettre"
 
@@ -370,15 +370,15 @@
 msgid "Revert to previous configuration"
 msgstr "Revenir à la configuration précédente"
 
 #: error_window.py:282
 msgid "Revert to defaults"
 msgstr "Revenir aux valeurs par défaut"
 
-#: error_window.py:283 main.py:363 main.py:409
+#: error_window.py:283 main.py:361 main.py:407
 #: widgets/js220_cal/js220_cal_widget.py:38
 msgid "Exit"
 msgstr "Sortie"
 
 #: exporter.py:49 widgets/signal_record/signal_record_config_widget.py:148
 #: widgets/statistics_record/statistics_record_config_widget.py:111
 msgid "Directory"
@@ -649,165 +649,165 @@
 msgid "Do not show again"
 msgstr "Ne plus afficher"
 
 #: intel_graphics_dialog.py:91
 msgid "Intel graphics detected"
 msgstr "Graphique Intel détecté"
 
-#: main.py:70 widgets/value/value_widget.py:653
+#: main.py:69 widgets/value/value_widget.py:660
 msgid "Multimeter"
 msgstr "Multimètre"
 
-#: main.py:71
+#: main.py:70
 msgid "Oscilloscope"
 msgstr "Oscilloscope"
 
-#: main.py:72 main.py:298 main.py:359 main.py:402
+#: main.py:71 main.py:296 main.py:357 main.py:400
 msgid "File"
 msgstr "Fichier"
 
-#: main.py:82
+#: main.py:81
 msgid "The UI status bar display mode"
 msgstr "Le mode d'affichage de la barre d'état de l'interface utilisateur"
 
-#: main.py:83
+#: main.py:82
 msgid ""
 "This setting controls the amount of detail shown on the status bar at the "
 "bottom of the UI window. You should usually leave this set to \"normal\" "
 "unless you want more detail concerning the UI internal operation."
 msgstr ""
 "Ce paramètre contrôle la quantité de détails affichés dans la barre d'état "
 "au bas de la fenêtre de l'interface utilisateur. Vous devriez généralement "
 "laisser ce paramètre sur \"normal\" à moins que vous ne souhaitiez obtenir "
 "plus de détails sur le fonctionnement interne de l'interface utilisateur."
 
-#: main.py:88 safe_mode.py:43
+#: main.py:87 safe_mode.py:43
 msgid "Normal"
 msgstr "Normal"
 
-#: main.py:89
+#: main.py:88
 msgid "Troubleshoot"
 msgstr "Dépannage"
 
-#: main.py:95
+#: main.py:94
 msgid "Enable developer mode."
 msgstr "Active le mode développeur."
 
-#: main.py:108
+#: main.py:107
 msgid "PubSub utilization"
 msgstr "Utilisation de PubSub"
 
-#: main.py:109
+#: main.py:108
 msgid ""
 "Display the number of actions processed by the publish-subscribe broker in "
 "each second."
 msgstr ""
 "Affiche le nombre d'actions traitées par le courtier de publication et "
 "d'abonnement chaque seconde."
 
-#: main.py:114
+#: main.py:113
 msgid "CPU utilization"
 msgstr "Utilisation de l'unité centrale"
 
-#: main.py:115
+#: main.py:114
 msgid ""
 "Display the CPU utilization by this application and the total CPU "
 "utilization by all applications. The value is displayed in percent."
 msgstr ""
 "Affiche l'utilisation du processeur par cette application et l'utilisation "
 "totale du processeur par toutes les applications. La valeur est affichée en "
 "pourcentage."
 
-#: main.py:121
+#: main.py:120
 msgid "Memory utilization"
 msgstr "Utilisation de la mémoire"
 
-#: main.py:122
+#: main.py:121
 msgid ""
 "Display the memory (RAM) utilization by this application and by all "
 "applications. The value is displayed in percent."
 msgstr ""
 "Affiche l'utilisation de la mémoire (RAM) par cette application et par "
 "toutes les applications. La valeur est affichée en pourcentage."
 
-#: main.py:216
+#: main.py:214
 msgid "UI"
 msgstr "UI"
 
-#: main.py:330
+#: main.py:328
 msgid "Help"
 msgstr "Aide"
 
-#: main.py:331 widgets/hamburger/hamburger_widget.py:21
+#: main.py:329 widgets/hamburger/hamburger_widget.py:21
 msgid "Getting Started"
 msgstr "Pour commencer"
 
-#: main.py:332
+#: main.py:330
 msgid "User's Guide"
 msgstr "Guide de l'utilisateur"
 
-#: main.py:333 widgets/hamburger/hamburger_widget.py:22
+#: main.py:331 widgets/hamburger/hamburger_widget.py:22
 msgid "Changelog"
 msgstr "Changelog"
 
-#: main.py:334 widgets/help/help_widget.py:59
+#: main.py:332 widgets/help/help_widget.py:59
 msgid "Report Issue"
 msgstr "Rapport"
 
-#: main.py:335
+#: main.py:333
 msgid "View logs..."
 msgstr "Voir les journaux..."
 
-#: main.py:336 widgets/hamburger/hamburger_widget.py:23
+#: main.py:334 widgets/hamburger/hamburger_widget.py:23
 msgid "Credits"
 msgstr "Crédits"
 
-#: main.py:337 widgets/hamburger/hamburger_widget.py:24
+#: main.py:335 widgets/hamburger/hamburger_widget.py:24
 msgid "About"
 msgstr "À propos de"
 
-#: main.py:360
+#: main.py:358
 msgid "Open"
 msgstr "Ouvrir"
 
-#: main.py:361
+#: main.py:359
 msgid "Open recent"
 msgstr "Ouvert récent"
 
-#: main.py:362 main.py:408
+#: main.py:360 main.py:406
 msgid "Clear config and exit"
 msgstr "Effacer la configuration et quitter"
 
-#: main.py:366 widgets/settings/settings_widget.py:541
+#: main.py:364 widgets/settings/settings_widget.py:541
 msgid "Widgets"
 msgstr "Widgets"
 
-#: main.py:367
+#: main.py:365
 msgid "Tools"
 msgstr "Outils"
 
-#: main.py:368
+#: main.py:366
 msgid "Clear Accumulators"
 msgstr "Accumulateurs transparents"
 
-#: main.py:403
+#: main.py:401
 msgid "Info"
 msgstr "Info"
 
-#: main.py:404 widget_tools.py:92 widgets/settings/settings_widget.py:31
+#: main.py:402 widget_tools.py:92 widgets/settings/settings_widget.py:31
 #: widgets/settings/settings_widget.py:574
 #: widgets/sidebar/sidebar_widget.py:41
 msgid "Settings"
 msgstr "Paramètres"
 
-#: main.py:693
+#: main.py:710
 msgid "Manage"
 msgstr "Gérer"
 
-#: main.py:730
+#: main.py:747
 msgid "Select file to open"
 msgstr "Sélectionner le fichier à ouvrir"
 
 #: paths.py:30 styles/manager.py:46
 msgid "The name for this widget."
 msgstr "Le nom de ce widget."
 
@@ -952,47 +952,47 @@
 msgid "Source"
 msgstr "Source d'information"
 
 #: units.py:35
 msgid "Use the application defaults"
 msgstr "Utiliser les paramètres par défaut de l'application"
 
-#: view.py:68
+#: view.py:72
 msgid "The active theme."
 msgstr "Le thème actif."
 
-#: view.py:70
+#: view.py:74
 msgid "Joulescope standard theme"
 msgstr "Thème standard du Joulescope"
 
-#: view.py:70
+#: view.py:74
 msgid "System OS-specific theme"
 msgstr "Système Thème spécifique au système d'exploitation"
 
-#: view.py:75
+#: view.py:79
 msgid "The color scheme name."
 msgstr "Le nom du schéma de couleurs."
 
-#: view.py:77
+#: view.py:81
 msgid "Dark background"
 msgstr "Fond noir"
 
-#: view.py:77
+#: view.py:81
 msgid "Light background"
 msgstr "Fond clair"
 
-#: view.py:81
+#: view.py:85
 msgid "The font scheme name."
 msgstr "Le nom de la police de caractères."
 
-#: view.py:83
+#: view.py:87
 msgid "Joulescope standard font theme"
 msgstr "Thème de police standard du Joulescope"
 
-#: view.py:102 widgets/view_manager/view_manager_widget.py:146
+#: view.py:106 widgets/view_manager/view_manager_widget.py:146
 msgid "New View"
 msgstr "Nouvelle vue"
 
 #: zip_inspector.py:23
 msgid "ZIP Inspector"
 msgstr "Inspecteur ZIP"
 
@@ -1111,15 +1111,15 @@
 "Lorsqu'il est activé, le courant circule entre les bornes de courant. "
 "Lorsqu'il est désactivé, le courant ne peut pas circuler entre les bornes de"
 " courant. Dans les configurations de système courantes, cela inhibe "
 "l'alimentation de la cible, ce qui peut être utilisé pour réinitialiser le "
 "dispositif cible par cycle d'alimentation."
 
 #: devices/jsdrv/js110.py:147 devices/jsdrv/js220.py:163
-#: widgets/waveform/waveform_widget.py:110
+#: widgets/waveform/waveform_widget.py:109
 msgid "Current range"
 msgstr "Gamme de courant"
 
 #: devices/jsdrv/js110.py:149
 msgid ""
 "Configure the J110's current range. Most applications should use the "
 "default, \"auto\"."
@@ -1267,33 +1267,33 @@
 "mean. This value is ignored for all other IRF types."
 msgstr ""
 "Le nombre d'échantillons après la fenêtre de la plage de courant utilisée "
 "pour déterminer la moyenne. Cette valeur est ignorée pour tous les autres "
 "types d'IRF."
 
 #: devices/jsdrv/js110.py:269 devices/jsdrv/js220.py:332
-#: widgets/device_control/fuse.py:103 widgets/waveform/waveform_widget.py:105
+#: widgets/device_control/fuse.py:103 widgets/waveform/waveform_widget.py:104
 msgid "Current"
 msgstr "Courant"
 
 #: devices/jsdrv/js110.py:270 devices/jsdrv/js220.py:333
 msgid "Enable the current signal streaming."
 msgstr "Active le flux de signaux de courant."
 
 #: devices/jsdrv/js110.py:278 devices/jsdrv/js220.py:341
-#: widgets/waveform/waveform_widget.py:106
+#: widgets/waveform/waveform_widget.py:105
 msgid "Voltage"
 msgstr "Tension"
 
 #: devices/jsdrv/js110.py:279 devices/jsdrv/js220.py:342
 msgid "Enable the voltage signal streaming."
 msgstr "Active le flux de signaux de tension."
 
 #: devices/jsdrv/js110.py:287 devices/jsdrv/js220.py:350
-#: widgets/waveform/waveform_widget.py:107
+#: widgets/waveform/waveform_widget.py:106
 msgid "Power"
 msgstr "Puissance"
 
 #: devices/jsdrv/js110.py:288 devices/jsdrv/js220.py:351
 msgid "Enable the power signal streaming."
 msgstr "Active le flux de signaux d'alimentation."
 
@@ -1514,15 +1514,15 @@
 msgid "GPI 3"
 msgstr "GPI 3"
 
 #: devices/jsdrv/js220.py:402
 msgid "Enable the general purpose input 3 signal streaming."
 msgstr "Active le flux de signaux de l'entrée générale 3."
 
-#: devices/jsdrv/js220.py:410 widgets/waveform/waveform_widget.py:124
+#: devices/jsdrv/js220.py:410 widgets/waveform/waveform_widget.py:123
 msgid "Trigger input"
 msgstr "Entrée de déclenchement"
 
 #: devices/jsdrv/js220.py:411
 msgid "Enable the trigger input signal streaming."
 msgstr "Active le flux de signaux d'entrée de déclenchement."
 
@@ -1533,15 +1533,15 @@
 #: devices/jsdrv/jsdrv_stream_buffer.py:44
 #: devices/jsdrv/jsdrv_stream_buffer.py:93
 #: devices/jsdrv/jsdrv_stream_buffer.py:107 plugins/selector.py:58
 #: widgets/settings/settings_widget.py:85
 #: widgets/settings/settings_widget.py:266
 #: widgets/settings/settings_widget.py:364
 #: widgets/settings/settings_widget.py:431
-#: widgets/waveform/waveform_widget.py:3062
+#: widgets/waveform/waveform_widget.py:3104
 msgid "Name"
 msgstr "Nom"
 
 #: devices/jsdrv/jsdrv_stream_buffer.py:45
 msgid "Joulescope stream buffer"
 msgstr "Joulescope stream buffer"
 
@@ -1766,15 +1766,15 @@
 
 #: widgets/accumulator/accumulator_widget.py:27
 #: widgets/value/value_widget.py:31
 msgid "The statistics data stream source."
 msgstr "La source du flux de données statistiques."
 
 #: widgets/accumulator/accumulator_widget.py:32
-#: widgets/value/value_widget.py:74
+#: widgets/value/value_widget.py:81
 msgid "The signal to display."
 msgstr "Le signal à afficher."
 
 #: widgets/accumulator/accumulator_widget.py:34
 msgid "charge"
 msgstr "charge"
 
@@ -1857,15 +1857,15 @@
 
 #: widgets/developer/publish_spy_widget.py:20
 #: widgets/developer/publish_spy_widget.py:21
 msgid "Topic"
 msgstr "Sujet"
 
 #: widgets/developer/publish_spy_widget.py:21
-#: widgets/settings/settings_widget.py:87 widgets/value/value_widget.py:662
+#: widgets/settings/settings_widget.py:87 widgets/value/value_widget.py:669
 msgid "Value"
 msgstr "Valeur"
 
 #: widgets/developer/publish_spy_widget.py:24
 msgid "Publish Spy"
 msgstr "Publier l'espion"
 
@@ -1895,15 +1895,15 @@
 
 #: widgets/device_control/device_update_dialog.py:24
 #: widgets/device_control/device_update_dialog.py:45
 msgid "Update"
 msgstr "Mise à jour"
 
 #: widgets/device_control/device_update_dialog.py:25
-#: widgets/value/value_widget.py:147
+#: widgets/value/value_widget.py:155
 msgid "Device"
 msgstr "Dispositif"
 
 #: widgets/device_control/device_update_dialog.py:27
 #: widgets/progress_bar/progress_bar_widget.py:59
 msgid "Progress"
 msgstr "Progrès"
@@ -2432,18 +2432,14 @@
 msgid "Click to display additional settings and actions."
 msgstr "Cliquez pour afficher des paramètres et des actions supplémentaires."
 
 #: widgets/sidebar/sidebar_widget.py:60
 msgid "sidebar"
 msgstr "encadré"
 
-#: widgets/sidebar/sidebar_widget.py:68
-msgid "The flyout width in pixels."
-msgstr "La largeur du flyout en pixels."
-
 #: widgets/signal_record/disk_full_dialog.py:19
 msgid "The disk is full"
 msgstr "Le disque est plein"
 
 #: widgets/signal_record/signal_record.py:57
 msgid "Could not open file for write"
 msgstr "Impossible d'ouvrir le fichier en écriture"
@@ -2470,15 +2466,15 @@
 msgid "StatisticsRecordConfig"
 msgstr "StatisticsRecordConfig"
 
 #: widgets/statistics_record/statistics_record_config_widget.py:123
 msgid "Time Format"
 msgstr "Format de l'heure"
 
-#: widgets/trigger/trigger_widget.py:41 widgets/value/value_widget.py:87
+#: widgets/trigger/trigger_widget.py:41 widgets/value/value_widget.py:94
 msgid "Select the source device"
 msgstr "Sélectionner l'appareil source"
 
 #: widgets/trigger/trigger_widget.py:42
 msgid "The device to use for the start condition and stop condition."
 msgstr ""
 "Le dispositif à utiliser pour la condition de démarrage et la condition "
@@ -2653,87 +2649,99 @@
 msgid "Show the statistics fields at the right."
 msgstr "Afficher les champs de statistiques à droite."
 
 #: widgets/value/value_widget.py:51
 msgid "Show a leading + or - sign."
 msgstr "Afficher un signe + ou -."
 
-#: widgets/value/value_widget.py:88
+#: widgets/value/value_widget.py:62
+msgid "Divide the quantity by this value."
+msgstr "Divisez la quantité par cette valeur."
+
+#: widgets/value/value_widget.py:63
+msgid ""
+"The divisor is a floating point number. The number may optionally be "
+"followed by units."
+msgstr ""
+"Le diviseur est un nombre à virgule flottante. Le nombre peut éventuellement"
+" être suivi d'unités."
+
+#: widgets/value/value_widget.py:95
 msgid ""
 "The values displayed by this widget come from a single source device. Select"
 " the source device here."
 msgstr ""
 "Les valeurs affichées par ce widget proviennent d'un seul appareil source. "
 "Sélectionnez l'appareil source ici."
 
-#: widgets/value/value_widget.py:94
+#: widgets/value/value_widget.py:101
 msgid "Hold the display"
 msgstr "Tenir l'écran"
 
-#: widgets/value/value_widget.py:96
+#: widgets/value/value_widget.py:103
 msgid "When selected, prevent the display from updating."
 msgstr ""
 "Lorsque cette option est sélectionnée, elle empêche la mise à jour de "
 "l'affichage."
 
-#: widgets/value/value_widget.py:97
+#: widgets/value/value_widget.py:104
 msgid ""
 "The UI also includes a global statistics hold button on the sidebar. When "
 "the global statistics hold button is selected, this button is disabled and "
 "has no effect."
 msgstr ""
 "L'interface utilisateur comprend également un bouton de maintien des "
 "statistiques globales dans la barre latérale. Lorsque le bouton de maintien "
 "des statistiques globales est sélectionné, ce bouton est désactivé et n'a "
 "aucun effet."
 
-#: widgets/value/value_widget.py:100
+#: widgets/value/value_widget.py:107
 msgid ""
 "The displayed values normally update with each new statistics data computed "
 "by the device. When this button is selected, the display will not be "
 "updated. However, the statistics will continue accumulate and accrue (if "
 "selected)."
 msgstr ""
 "Les valeurs affichées sont normalement mises à jour avec chaque nouvelle "
 "donnée statistique calculée par l'appareil. Lorsque ce bouton est "
 "sélectionné, l'affichage n'est pas mis à jour. Cependant, les statistiques "
 "continueront à s'accumuler et à se cumuler (si sélectionné)."
 
-#: widgets/value/value_widget.py:107
+#: widgets/value/value_widget.py:114
 msgid "Accrue values over time"
 msgstr "Accumuler des valeurs au fil du temps"
 
-#: widgets/value/value_widget.py:109
+#: widgets/value/value_widget.py:116
 msgid ""
 "Current, voltage, and power are normally computed over a single statistics "
 "frequency interval. Press this button to accrue the values indefinitely. "
 "Press again to return to normal operation."
 msgstr ""
 "Le courant, la tension et la puissance sont normalement calculés sur un seul"
 " intervalle de fréquence statistique. Appuyez sur ce bouton pour accumuler "
 "les valeurs indéfiniment. Appuyez à nouveau sur ce bouton pour revenir au "
 "fonctionnement normal."
 
-#: widgets/value/value_widget.py:113
+#: widgets/value/value_widget.py:120
 msgid ""
 "Note that this button does not affect the charge and energy accumulation. "
 "Both accumulate indefinitely regardless of this button state."
 msgstr ""
 "Notez que ce bouton n'affecte pas l'accumulation de charge et d'énergie. Les"
 " deux s'accumulent indéfiniment quel que soit l'état de ce bouton."
 
-#: widgets/value/value_widget.py:195
+#: widgets/value/value_widget.py:203
 msgid "Not present"
 msgstr "Non présent"
 
-#: widgets/value/value_widget.py:215
+#: widgets/value/value_widget.py:223
 msgid "Hold"
 msgstr "Tenir"
 
-#: widgets/value/value_widget.py:223
+#: widgets/value/value_widget.py:231
 msgid "Accrue"
 msgstr "Accrue"
 
 #: widgets/view_manager/view_manager_widget.py:108
 #: widgets/view_manager/view_manager_widget.py:174
 msgid "View Manager"
 msgstr "Gestionnaire d'affichage"
@@ -2779,34 +2787,34 @@
 msgstr "triangle droit"
 
 #: widgets/waveform/text_annotation.py:62
 msgid "triangle left"
 msgstr "triangle gauche"
 
 #: widgets/waveform/text_annotation.py:66
-#: widgets/waveform/waveform_widget.py:3008
+#: widgets/waveform/waveform_widget.py:3050
 msgid "Manual"
 msgstr "Manuel"
 
 #: widgets/waveform/text_annotation.py:67
 msgid "Centered"
 msgstr "Centré"
 
 #: widgets/waveform/text_annotation.py:99
-#: widgets/waveform/waveform_widget.py:3123
+#: widgets/waveform/waveform_widget.py:3167
 msgid "Text"
 msgstr "Texte"
 
 #: widgets/waveform/text_annotation.py:107
-#: widgets/waveform/waveform_widget.py:3348
+#: widgets/waveform/waveform_widget.py:3398
 msgid "Show text"
 msgstr "Afficher le texte"
 
 #: widgets/waveform/text_annotation.py:116
-#: widgets/waveform/waveform_widget.py:3360
+#: widgets/waveform/waveform_widget.py:3410
 msgid "Shape"
 msgstr "Forme"
 
 #: widgets/waveform/text_annotation.py:126
 msgid "Y Mode"
 msgstr "Mode Y"
 
@@ -3006,323 +3014,323 @@
 "\"default\" will use the default source which is normally configured using "
 "the Device Control widget."
 msgstr ""
 "\"default\" utilisera la source par défaut qui est normalement configurée à "
 "l'aide du widget Device Control."
 
 #: widgets/waveform/waveform_source_widget.py:104
-#: widgets/waveform/waveform_widget.py:402
-#: widgets/waveform/waveform_widget.py:479
+#: widgets/waveform/waveform_widget.py:401
+#: widgets/waveform/waveform_widget.py:478
 msgid "off"
 msgstr "off"
 
-#: widgets/waveform/waveform_widget.py:44
+#: widgets/waveform/waveform_widget.py:43
 msgid "Waveform"
 msgstr "Forme d'onde"
 
-#: widgets/waveform/waveform_widget.py:120
+#: widgets/waveform/waveform_widget.py:119
 msgid "General purpose input 0"
 msgstr "Entrée générale 0"
 
-#: widgets/waveform/waveform_widget.py:121
+#: widgets/waveform/waveform_widget.py:120
 msgid "General purpose input 1"
 msgstr "Entrée d'usage général 1"
 
-#: widgets/waveform/waveform_widget.py:122
+#: widgets/waveform/waveform_widget.py:121
 msgid "General purpose input 2"
 msgstr "Entrée d'usage général 2"
 
-#: widgets/waveform/waveform_widget.py:123
+#: widgets/waveform/waveform_widget.py:122
 msgid "General purpose input 3"
 msgstr "Entrée à usage général 3"
 
-#: widgets/waveform/waveform_widget.py:358
+#: widgets/waveform/waveform_widget.py:357
 msgid "The source filter string."
 msgstr "La chaîne de filtrage de la source."
 
-#: widgets/waveform/waveform_widget.py:369
+#: widgets/waveform/waveform_widget.py:368
 msgid "The trace width."
 msgstr "La largeur de la trace."
 
-#: widgets/waveform/waveform_widget.py:384
+#: widgets/waveform/waveform_widget.py:383
 msgid "The target frames per second."
 msgstr "L'objectif en termes d'images par seconde."
 
-#: widgets/waveform/waveform_widget.py:386
+#: widgets/waveform/waveform_widget.py:385
 msgid "vsync"
 msgstr "vsync"
 
-#: widgets/waveform/waveform_widget.py:387
+#: widgets/waveform/waveform_widget.py:386
 msgid "20 Hz"
 msgstr "20 Hz"
 
-#: widgets/waveform/waveform_widget.py:388
+#: widgets/waveform/waveform_widget.py:387
 msgid "10 Hz"
 msgstr "10 Hz"
 
-#: widgets/waveform/waveform_widget.py:389
+#: widgets/waveform/waveform_widget.py:388
 msgid "5 Hz"
 msgstr "5 Hz"
 
-#: widgets/waveform/waveform_widget.py:395
+#: widgets/waveform/waveform_widget.py:394
 msgid "The minimum interval between repaint in milliseconds."
 msgstr "Intervalle minimum entre deux repeints en millisecondes."
 
-#: widgets/waveform/waveform_widget.py:400
+#: widgets/waveform/waveform_widget.py:399
 msgid "Show the minimum and maximum extents fill."
 msgstr "Affiche les remplissages minimum et maximum des étendues."
 
-#: widgets/waveform/waveform_widget.py:403
+#: widgets/waveform/waveform_widget.py:402
 msgid "lines"
 msgstr "lignes"
 
-#: widgets/waveform/waveform_widget.py:404
+#: widgets/waveform/waveform_widget.py:403
 msgid "fill 1"
 msgstr "remplir 1"
 
-#: widgets/waveform/waveform_widget.py:405
+#: widgets/waveform/waveform_widget.py:404
 msgid "fill 2"
 msgstr "remplir 2"
 
-#: widgets/waveform/waveform_widget.py:411
+#: widgets/waveform/waveform_widget.py:410
 msgid "Show the frames per second."
 msgstr "Indique le nombre d'images par seconde."
 
-#: widgets/waveform/waveform_widget.py:416
+#: widgets/waveform/waveform_widget.py:415
 msgid "Show the statistics on mouse hover."
 msgstr "Afficher les statistiques au passage de la souris."
 
-#: widgets/waveform/waveform_widget.py:421
+#: widgets/waveform/waveform_widget.py:420
 msgid "Show the plot statistics on the right."
 msgstr "Afficher les statistiques du tracé à droite."
 
-#: widgets/waveform/waveform_widget.py:426
+#: widgets/waveform/waveform_widget.py:425
 msgid "Show frequency for dual markers and statistics."
 msgstr "Fréquence d'affichage pour les marqueurs doubles et les statistiques."
 
-#: widgets/waveform/waveform_widget.py:431
+#: widgets/waveform/waveform_widget.py:430
 msgid "The quantities to display by default."
 msgstr "Les quantités à afficher par défaut."
 
-#: widgets/waveform/waveform_widget.py:437
+#: widgets/waveform/waveform_widget.py:436
 msgid "The precision to display in digits."
 msgstr "La précision à afficher en chiffres."
 
-#: widgets/waveform/waveform_widget.py:443
+#: widgets/waveform/waveform_widget.py:442
 msgid "Use OpenGL rendering."
 msgstr "Utiliser le rendu OpenGL."
 
-#: widgets/waveform/waveform_widget.py:454
+#: widgets/waveform/waveform_widget.py:453
 msgid "Pin the left side (oldest) data so that it stays in view."
 msgstr ""
 "Épingler les données de gauche (les plus anciennes) pour qu'elles restent "
 "visibles."
 
-#: widgets/waveform/waveform_widget.py:459
+#: widgets/waveform/waveform_widget.py:458
 msgid "Pin the right side (newest) data so that it stays in view."
 msgstr ""
 "Épingler les données de droite (les plus récentes) pour qu'elles restent "
 "visibles."
 
-#: widgets/waveform/waveform_widget.py:464
+#: widgets/waveform/waveform_widget.py:463
 msgid "The waveform state."
 msgstr "L'état de la forme d'onde."
 
-#: widgets/waveform/waveform_widget.py:470
+#: widgets/waveform/waveform_widget.py:469
 msgid "The annotations."
 msgstr "Les annotations."
 
-#: widgets/waveform/waveform_widget.py:476
+#: widgets/waveform/waveform_widget.py:475
 msgid "Control location"
 msgstr "Emplacement de contrôle"
 
-#: widgets/waveform/waveform_widget.py:480
+#: widgets/waveform/waveform_widget.py:479
 msgid "top"
 msgstr "haut"
 
-#: widgets/waveform/waveform_widget.py:481
+#: widgets/waveform/waveform_widget.py:480
 msgid "bottom"
 msgstr "fond"
 
-#: widgets/waveform/waveform_widget.py:486
+#: widgets/waveform/waveform_widget.py:485
 msgid "The signal quantity to show in the summary."
 msgstr "La quantité de signal à afficher dans le résumé."
 
-#: widgets/waveform/waveform_widget.py:492
+#: widgets/waveform/waveform_widget.py:491
 msgid "X-axis annotation mode"
 msgstr "Mode d'annotation de l'axe X"
 
-#: widgets/waveform/waveform_widget.py:495
-#: widgets/waveform/waveform_widget.py:2888
+#: widgets/waveform/waveform_widget.py:494
+#: widgets/waveform/waveform_widget.py:2930
 msgid "Absolute"
 msgstr "Absolu"
 
-#: widgets/waveform/waveform_widget.py:496
-#: widgets/waveform/waveform_widget.py:2893
+#: widgets/waveform/waveform_widget.py:495
+#: widgets/waveform/waveform_widget.py:2935
 msgid "Relative"
 msgstr "Relatif"
 
-#: widgets/waveform/waveform_widget.py:502
+#: widgets/waveform/waveform_widget.py:501
 msgid "The available subsources."
 msgstr "Les sous-sources disponibles."
 
-#: widgets/waveform/waveform_widget.py:508
+#: widgets/waveform/waveform_widget.py:507
 msgid "The selected subsources for each trace."
 msgstr "Les sous-sources sélectionnées pour chaque trace."
 
-#: widgets/waveform/waveform_widget.py:514
+#: widgets/waveform/waveform_widget.py:513
 msgid "The trace priority: highest int value on top, None is off."
 msgstr ""
 "La priorité de la trace : la valeur int la plus élevée est en haut, None est"
 " désactivé."
 
-#: widgets/waveform/waveform_widget.py:2834
-#: widgets/waveform/waveform_widget.py:3135
+#: widgets/waveform/waveform_widget.py:2877
+#: widgets/waveform/waveform_widget.py:3179
 msgid "Save image to file"
 msgstr "Enregistrer l'image dans un fichier"
 
-#: widgets/waveform/waveform_widget.py:2882
-#: widgets/waveform/waveform_widget.py:2951
+#: widgets/waveform/waveform_widget.py:2924
+#: widgets/waveform/waveform_widget.py:2993
 msgid "Single marker"
 msgstr "Marqueur unique"
 
-#: widgets/waveform/waveform_widget.py:2883
-#: widgets/waveform/waveform_widget.py:2952
+#: widgets/waveform/waveform_widget.py:2925
+#: widgets/waveform/waveform_widget.py:2994
 msgid "Dual markers"
 msgstr "Double marqueur"
 
-#: widgets/waveform/waveform_widget.py:2885
+#: widgets/waveform/waveform_widget.py:2927
 msgid "Mode"
 msgstr "Mode de fonctionnement"
 
-#: widgets/waveform/waveform_widget.py:2898
-#: widgets/waveform/waveform_widget.py:2953
-#: widgets/waveform/waveform_widget.py:3111
-#: widgets/waveform/waveform_widget.py:3129
+#: widgets/waveform/waveform_widget.py:2940
+#: widgets/waveform/waveform_widget.py:2995
+#: widgets/waveform/waveform_widget.py:3155
+#: widgets/waveform/waveform_widget.py:3173
 msgid "Clear all"
 msgstr "Tout effacer"
 
-#: widgets/waveform/waveform_widget.py:2909
-#: widgets/waveform/waveform_widget.py:2998
-#: widgets/waveform/waveform_widget.py:3117
+#: widgets/waveform/waveform_widget.py:2951
+#: widgets/waveform/waveform_widget.py:3040
+#: widgets/waveform/waveform_widget.py:3161
 msgid "Annotations"
 msgstr "Annotations"
 
-#: widgets/waveform/waveform_widget.py:3001
+#: widgets/waveform/waveform_widget.py:3043
 msgid "Range"
 msgstr "Gamme"
 
-#: widgets/waveform/waveform_widget.py:3005
-#: widgets/waveform/waveform_widget.py:3328
+#: widgets/waveform/waveform_widget.py:3047
+#: widgets/waveform/waveform_widget.py:3378
 msgid "Auto"
 msgstr "Auto"
 
-#: widgets/waveform/waveform_widget.py:3011
+#: widgets/waveform/waveform_widget.py:3053
 msgid "Exact"
 msgstr "Exact"
 
-#: widgets/waveform/waveform_widget.py:3020
+#: widgets/waveform/waveform_widget.py:3062
 msgid "Scale"
 msgstr "Échelle"
 
-#: widgets/waveform/waveform_widget.py:3023
+#: widgets/waveform/waveform_widget.py:3065
 msgid "Linear"
 msgstr "Linéaire"
 
-#: widgets/waveform/waveform_widget.py:3028
+#: widgets/waveform/waveform_widget.py:3070
 msgid "Logarithmic"
 msgstr "Logarithmique"
 
-#: widgets/waveform/waveform_widget.py:3036
+#: widgets/waveform/waveform_widget.py:3078
 msgid "Logarithmic zero"
 msgstr "Zéro logarithmique"
 
-#: widgets/waveform/waveform_widget.py:3050
+#: widgets/waveform/waveform_widget.py:3092
 msgid "Preferred prefix"
 msgstr "Préfixe préféré"
 
-#: widgets/waveform/waveform_widget.py:3108
+#: widgets/waveform/waveform_widget.py:3152
 msgid "Add"
 msgstr "Ajouter"
 
-#: widgets/waveform/waveform_widget.py:3109
+#: widgets/waveform/waveform_widget.py:3153
 msgid "Hide all text"
 msgstr "Cacher tout le texte"
 
-#: widgets/waveform/waveform_widget.py:3110
+#: widgets/waveform/waveform_widget.py:3154
 msgid "Show all text"
 msgstr "Afficher tous les textes"
 
-#: widgets/waveform/waveform_widget.py:3118
+#: widgets/waveform/waveform_widget.py:3162
 msgid "Vertical"
 msgstr "Vertical"
 
-#: widgets/waveform/waveform_widget.py:3121
+#: widgets/waveform/waveform_widget.py:3165
 msgid "Horizontal"
 msgstr "Horizontal"
 
-#: widgets/waveform/waveform_widget.py:3127
+#: widgets/waveform/waveform_widget.py:3171
 msgid "Save"
 msgstr "Sauvegarder"
 
-#: widgets/waveform/waveform_widget.py:3132
+#: widgets/waveform/waveform_widget.py:3176
 msgid "Y-axis auto range"
 msgstr "Plage automatique de l'axe Y"
 
-#: widgets/waveform/waveform_widget.py:3136
+#: widgets/waveform/waveform_widget.py:3180
 msgid "Copy image to clipboard"
 msgstr "Copier l'image dans le presse-papiers"
 
-#: widgets/waveform/waveform_widget.py:3137
+#: widgets/waveform/waveform_widget.py:3181
 msgid "Export visible data"
 msgstr "Export visible data"
 
-#: widgets/waveform/waveform_widget.py:3138
+#: widgets/waveform/waveform_widget.py:3182
 msgid "Export all data"
 msgstr "Exporter toutes les données"
 
-#: widgets/waveform/waveform_widget.py:3304
+#: widgets/waveform/waveform_widget.py:3354
 msgid "Export"
 msgstr "Exportation"
 
-#: widgets/waveform/waveform_widget.py:3305
+#: widgets/waveform/waveform_widget.py:3355
 msgid "Analysis"
 msgstr "Analyse"
 
-#: widgets/waveform/waveform_widget.py:3313
+#: widgets/waveform/waveform_widget.py:3363
 msgid "Interval"
 msgstr "Intervalle"
 
-#: widgets/waveform/waveform_widget.py:3322
+#: widgets/waveform/waveform_widget.py:3372
 msgid "Zoom"
 msgstr "Zoom"
 
-#: widgets/waveform/waveform_widget.py:3326
+#: widgets/waveform/waveform_widget.py:3376
 msgid "Show statistics"
 msgstr "Afficher les statistiques"
 
-#: widgets/waveform/waveform_widget.py:3331
+#: widgets/waveform/waveform_widget.py:3381
 msgid "Left"
 msgstr "Gauche"
 
-#: widgets/waveform/waveform_widget.py:3334
+#: widgets/waveform/waveform_widget.py:3384
 msgid "Right"
 msgstr "Droit"
 
-#: widgets/waveform/waveform_widget.py:3337
+#: widgets/waveform/waveform_widget.py:3387
 msgid "Off"
 msgstr "Off"
 
-#: widgets/waveform/waveform_widget.py:3340
-#: widgets/waveform/waveform_widget.py:3368
-#: widgets/waveform/waveform_widget.py:3397
+#: widgets/waveform/waveform_widget.py:3390
+#: widgets/waveform/waveform_widget.py:3418
+#: widgets/waveform/waveform_widget.py:3448
 msgid "Remove"
 msgstr "Enlever"
 
-#: widgets/waveform/waveform_widget.py:3351
+#: widgets/waveform/waveform_widget.py:3401
 msgid "Y mode"
 msgstr "Mode Y"
 
 #: widgets/waveform/y_range_widget.py:67
 msgid "max"
 msgstr "max"
```

### Comparing `joulescope_ui-1.1.6/joulescope_ui/locale/it/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.7/joulescope_ui/locale/it/LC_MESSAGES/joulescope_ui.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.4\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-18 14:15-0400\n"
+"POT-Creation-Date: 2024-05-06 17:27-0400\n"
 "PO-Revision-Date: 2024-04-18 10:43-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: it\n"
 "Language-Team: it <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.14.0\n"
+"Generated-By: Babel 2.15.0\n"
 
 msgid "\"3.3 V\" uses an internally-generated 3.3V reference voltage."
 msgstr ""
 "\"3,3 V\" utilizza una tensione di riferimento di 3,3 V generata "
 "internamente."
 
 msgid "\"NaN\" sets all samples in the window to NaN."
@@ -661,14 +661,17 @@
 msgid ""
 "Display the number of actions processed by the publish-subscribe broker in "
 "each second."
 msgstr ""
 "Visualizzare il numero di azioni elaborate dal broker publish-subscribe in "
 "ogni secondo."
 
+msgid "Divide the quantity by this value."
+msgstr "Dividere la quantità per questo valore."
+
 msgid "Do not show again"
 msgstr "Non mostrare di nuovo"
 
 msgid "Do not use any USB hubs, docks or adapters"
 msgstr "Non utilizzare hub, dock o adattatori USB."
 
 msgid "Dual markers"
@@ -1786,14 +1789,21 @@
 msgstr ""
 "I valori visualizzati si aggiornano normalmente con ogni nuovo dato "
 "statistico calcolato dal dispositivo. Quando si seleziona questo pulsante, "
 "il display non viene aggiornato. Tuttavia, le statistiche continueranno ad "
 "accumularsi (se selezionato)."
 
 msgid ""
+"The divisor is a floating point number. The number may optionally be "
+"followed by units."
+msgstr ""
+"Il divisore è un numero in virgola mobile. Il numero può essere "
+"facoltativamente seguito da unità."
+
+msgid ""
 "The exponential decay time constant. The fuse dissipates 63.2 percent of "
 "accumulated energy in this duration."
 msgstr ""
 "La costante di tempo di decadimento esponenziale. Il fusibile dissipa il "
 "63,2% dell'energia accumulata in questa durata."
 
 msgid "The filename supports the following replacements."
@@ -1802,17 +1812,14 @@
 msgid "The filename with optional replacements."
 msgstr "Il nome del file con sostituzioni opzionali."
 
 msgid "The fixed default path for loading and saving files."
 msgstr ""
 "Il percorso predefinito fisso per il caricamento e il salvataggio dei file."
 
-msgid "The flyout width in pixels."
-msgstr "Larghezza del flyout in pixel."
-
 msgid "The font scheme name."
 msgstr "Il nome dello schema di caratteri."
 
 msgid "The format string"
 msgstr "La stringa di formato"
 
 msgid "The fuse trips in Duration at this constant current."
```

### Comparing `joulescope_ui-1.1.6/joulescope_ui/locale/it/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.7/joulescope_ui/locale/it/LC_MESSAGES/joulescope_ui.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.4\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-18 14:15-0400\n"
+"POT-Creation-Date: 2024-05-06 17:27-0400\n"
 "PO-Revision-Date: 2024-04-18 10:43-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: it <LL@li.org>\n"
 "Language: it\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-"Generated-By: Babel 2.14.0\n"
+"Generated-By: Babel 2.15.0\n"
 
 #: about.py:24
 msgid "About the Joulescope UI"
 msgstr "Informazioni sull'interfaccia utente di Joulescope"
 
 #: about.py:25
 msgid "Version Information"
@@ -336,27 +336,27 @@
 msgid "Email"
 msgstr "E-mail"
 
 #: error_window.py:103
 msgid "Description"
 msgstr "Descrizione"
 
-#: error_window.py:112 widgets/waveform/waveform_widget.py:3347
+#: error_window.py:112 widgets/waveform/waveform_widget.py:3397
 msgid "Edit"
 msgstr "Modifica"
 
 #: error_window.py:113
 msgid "View as Markdown"
 msgstr "Visualizza come Markdown"
 
 #: error_window.py:119
 msgid "Abort"
 msgstr "Interruzione"
 
-#: error_window.py:120 main.py:365 widgets/settings/settings_widget.py:539
+#: error_window.py:120 main.py:363 widgets/settings/settings_widget.py:539
 msgid "View"
 msgstr "Visualizza"
 
 #: error_window.py:121
 msgid "Submit"
 msgstr "Invia"
 
@@ -368,15 +368,15 @@
 msgid "Revert to previous configuration"
 msgstr "Torna alla configurazione precedente"
 
 #: error_window.py:282
 msgid "Revert to defaults"
 msgstr "Torna alle impostazioni predefinite"
 
-#: error_window.py:283 main.py:363 main.py:409
+#: error_window.py:283 main.py:361 main.py:407
 #: widgets/js220_cal/js220_cal_widget.py:38
 msgid "Exit"
 msgstr "Uscita"
 
 #: exporter.py:49 widgets/signal_record/signal_record_config_widget.py:148
 #: widgets/statistics_record/statistics_record_config_widget.py:111
 msgid "Directory"
@@ -647,166 +647,166 @@
 msgid "Do not show again"
 msgstr "Non mostrare di nuovo"
 
 #: intel_graphics_dialog.py:91
 msgid "Intel graphics detected"
 msgstr "Rilevata la grafica Intel"
 
-#: main.py:70 widgets/value/value_widget.py:653
+#: main.py:69 widgets/value/value_widget.py:660
 msgid "Multimeter"
 msgstr "Multimetro"
 
-#: main.py:71
+#: main.py:70
 msgid "Oscilloscope"
 msgstr "Oscilloscope"
 
-#: main.py:72 main.py:298 main.py:359 main.py:402
+#: main.py:71 main.py:296 main.py:357 main.py:400
 msgid "File"
 msgstr "File"
 
-#: main.py:82
+#: main.py:81
 msgid "The UI status bar display mode"
 msgstr ""
 "Modalità di visualizzazione della barra di stato dell'interfaccia utente"
 
-#: main.py:83
+#: main.py:82
 msgid ""
 "This setting controls the amount of detail shown on the status bar at the "
 "bottom of the UI window. You should usually leave this set to \"normal\" "
 "unless you want more detail concerning the UI internal operation."
 msgstr ""
 "Questa impostazione controlla la quantità di dettagli mostrati nella barra "
 "di stato in fondo alla finestra dell'interfaccia utente. Di solito si "
 "consiglia di lasciarla impostata su \"normale\", a meno che non si vogliano "
 "maggiori dettagli sul funzionamento interno dell'interfaccia utente."
 
-#: main.py:88 safe_mode.py:43
+#: main.py:87 safe_mode.py:43
 msgid "Normal"
 msgstr "Normale"
 
-#: main.py:89
+#: main.py:88
 msgid "Troubleshoot"
 msgstr "Risoluzione dei problemi"
 
-#: main.py:95
+#: main.py:94
 msgid "Enable developer mode."
 msgstr "Attivare la modalità sviluppatore."
 
-#: main.py:108
+#: main.py:107
 msgid "PubSub utilization"
 msgstr "Utilizzo di PubSub"
 
-#: main.py:109
+#: main.py:108
 msgid ""
 "Display the number of actions processed by the publish-subscribe broker in "
 "each second."
 msgstr ""
 "Visualizzare il numero di azioni elaborate dal broker publish-subscribe in "
 "ogni secondo."
 
-#: main.py:114
+#: main.py:113
 msgid "CPU utilization"
 msgstr "Utilizzo della CPU"
 
-#: main.py:115
+#: main.py:114
 msgid ""
 "Display the CPU utilization by this application and the total CPU "
 "utilization by all applications. The value is displayed in percent."
 msgstr ""
 "Visualizza l'utilizzo della CPU da parte di questa applicazione e l'utilizzo"
 " totale della CPU da parte di tutte le applicazioni. Il valore viene "
 "visualizzato in percentuale."
 
-#: main.py:121
+#: main.py:120
 msgid "Memory utilization"
 msgstr "Utilizzo della memoria"
 
-#: main.py:122
+#: main.py:121
 msgid ""
 "Display the memory (RAM) utilization by this application and by all "
 "applications. The value is displayed in percent."
 msgstr ""
 "Visualizza l'utilizzo della memoria (RAM) da parte di questa applicazione e "
 "di tutte le applicazioni. Il valore viene visualizzato in percentuale."
 
-#: main.py:216
+#: main.py:214
 msgid "UI"
 msgstr "UI"
 
-#: main.py:330
+#: main.py:328
 msgid "Help"
 msgstr "Aiuto"
 
-#: main.py:331 widgets/hamburger/hamburger_widget.py:21
+#: main.py:329 widgets/hamburger/hamburger_widget.py:21
 msgid "Getting Started"
 msgstr "Per iniziare"
 
-#: main.py:332
+#: main.py:330
 msgid "User's Guide"
 msgstr "Guida all'uso"
 
-#: main.py:333 widgets/hamburger/hamburger_widget.py:22
+#: main.py:331 widgets/hamburger/hamburger_widget.py:22
 msgid "Changelog"
 msgstr "Changelog"
 
-#: main.py:334 widgets/help/help_widget.py:59
+#: main.py:332 widgets/help/help_widget.py:59
 msgid "Report Issue"
 msgstr "Segnala il problema"
 
-#: main.py:335
+#: main.py:333
 msgid "View logs..."
 msgstr "Visualizza i registri..."
 
-#: main.py:336 widgets/hamburger/hamburger_widget.py:23
+#: main.py:334 widgets/hamburger/hamburger_widget.py:23
 msgid "Credits"
 msgstr "Crediti"
 
-#: main.py:337 widgets/hamburger/hamburger_widget.py:24
+#: main.py:335 widgets/hamburger/hamburger_widget.py:24
 msgid "About"
 msgstr "Informazioni su"
 
-#: main.py:360
+#: main.py:358
 msgid "Open"
 msgstr "Aperto"
 
-#: main.py:361
+#: main.py:359
 msgid "Open recent"
 msgstr "Apertura recente"
 
-#: main.py:362 main.py:408
+#: main.py:360 main.py:406
 msgid "Clear config and exit"
 msgstr "Cancella la configurazione e esci"
 
-#: main.py:366 widgets/settings/settings_widget.py:541
+#: main.py:364 widgets/settings/settings_widget.py:541
 msgid "Widgets"
 msgstr "Widget"
 
-#: main.py:367
+#: main.py:365
 msgid "Tools"
 msgstr "Strumenti"
 
-#: main.py:368
+#: main.py:366
 msgid "Clear Accumulators"
 msgstr "Accumulatori chiari"
 
-#: main.py:403
+#: main.py:401
 msgid "Info"
 msgstr "Info"
 
-#: main.py:404 widget_tools.py:92 widgets/settings/settings_widget.py:31
+#: main.py:402 widget_tools.py:92 widgets/settings/settings_widget.py:31
 #: widgets/settings/settings_widget.py:574
 #: widgets/sidebar/sidebar_widget.py:41
 msgid "Settings"
 msgstr "Impostazioni"
 
-#: main.py:693
+#: main.py:710
 msgid "Manage"
 msgstr "Gestire"
 
-#: main.py:730
+#: main.py:747
 msgid "Select file to open"
 msgstr "Selezionare il file da aprire"
 
 #: paths.py:30 styles/manager.py:46
 msgid "The name for this widget."
 msgstr "Il nome di questo widget."
 
@@ -948,47 +948,47 @@
 msgid "Source"
 msgstr "Fonte"
 
 #: units.py:35
 msgid "Use the application defaults"
 msgstr "Utilizzare le impostazioni predefinite dell'applicazione"
 
-#: view.py:68
+#: view.py:72
 msgid "The active theme."
 msgstr "Il tema attivo."
 
-#: view.py:70
+#: view.py:74
 msgid "Joulescope standard theme"
 msgstr "Tema standard di Joulescope"
 
-#: view.py:70
+#: view.py:74
 msgid "System OS-specific theme"
 msgstr "Tema specifico del sistema OS"
 
-#: view.py:75
+#: view.py:79
 msgid "The color scheme name."
 msgstr "Il nome della combinazione di colori."
 
-#: view.py:77
+#: view.py:81
 msgid "Dark background"
 msgstr "Sfondo scuro"
 
-#: view.py:77
+#: view.py:81
 msgid "Light background"
 msgstr "Sfondo luminoso"
 
-#: view.py:81
+#: view.py:85
 msgid "The font scheme name."
 msgstr "Il nome dello schema di caratteri."
 
-#: view.py:83
+#: view.py:87
 msgid "Joulescope standard font theme"
 msgstr "Tema del carattere standard di Joulescope"
 
-#: view.py:102 widgets/view_manager/view_manager_widget.py:146
+#: view.py:106 widgets/view_manager/view_manager_widget.py:146
 msgid "New View"
 msgstr "Nuova vista"
 
 #: zip_inspector.py:23
 msgid "ZIP Inspector"
 msgstr "Ispettore ZIP"
 
@@ -1107,15 +1107,15 @@
 "Quando è abilitata, la corrente scorre tra i terminali di corrente. Quando è"
 " disabilitata, la corrente non può scorrere tra i terminali di corrente. "
 "Nelle comuni configurazioni di sistema, questo inibisce l'alimentazione del "
 "target, che può essere utilizzata per resettare il dispositivo di "
 "destinazione."
 
 #: devices/jsdrv/js110.py:147 devices/jsdrv/js220.py:163
-#: widgets/waveform/waveform_widget.py:110
+#: widgets/waveform/waveform_widget.py:109
 msgid "Current range"
 msgstr "Intervallo di corrente"
 
 #: devices/jsdrv/js110.py:149
 msgid ""
 "Configure the J110's current range. Most applications should use the "
 "default, \"auto\"."
@@ -1263,33 +1263,33 @@
 "mean. This value is ignored for all other IRF types."
 msgstr ""
 "Il numero di campioni dopo la finestra dell'intervallo di corrente viene "
 "utilizzato per determinare la media. Questo valore viene ignorato per tutti "
 "gli altri tipi di IRF."
 
 #: devices/jsdrv/js110.py:269 devices/jsdrv/js220.py:332
-#: widgets/device_control/fuse.py:103 widgets/waveform/waveform_widget.py:105
+#: widgets/device_control/fuse.py:103 widgets/waveform/waveform_widget.py:104
 msgid "Current"
 msgstr "Corrente"
 
 #: devices/jsdrv/js110.py:270 devices/jsdrv/js220.py:333
 msgid "Enable the current signal streaming."
 msgstr "Abilitare lo streaming del segnale di corrente."
 
 #: devices/jsdrv/js110.py:278 devices/jsdrv/js220.py:341
-#: widgets/waveform/waveform_widget.py:106
+#: widgets/waveform/waveform_widget.py:105
 msgid "Voltage"
 msgstr "Tensione"
 
 #: devices/jsdrv/js110.py:279 devices/jsdrv/js220.py:342
 msgid "Enable the voltage signal streaming."
 msgstr "Abilitare lo streaming del segnale di tensione."
 
 #: devices/jsdrv/js110.py:287 devices/jsdrv/js220.py:350
-#: widgets/waveform/waveform_widget.py:107
+#: widgets/waveform/waveform_widget.py:106
 msgid "Power"
 msgstr "Potenza"
 
 #: devices/jsdrv/js110.py:288 devices/jsdrv/js220.py:351
 msgid "Enable the power signal streaming."
 msgstr "Abilitare lo streaming del segnale di potenza."
 
@@ -1510,15 +1510,15 @@
 msgid "GPI 3"
 msgstr "GPI 3"
 
 #: devices/jsdrv/js220.py:402
 msgid "Enable the general purpose input 3 signal streaming."
 msgstr "Abilitare lo streaming del segnale dell'ingresso 3 per uso generale."
 
-#: devices/jsdrv/js220.py:410 widgets/waveform/waveform_widget.py:124
+#: devices/jsdrv/js220.py:410 widgets/waveform/waveform_widget.py:123
 msgid "Trigger input"
 msgstr "Ingresso di trigger"
 
 #: devices/jsdrv/js220.py:411
 msgid "Enable the trigger input signal streaming."
 msgstr "Abilitare lo streaming del segnale di ingresso di trigger."
 
@@ -1529,15 +1529,15 @@
 #: devices/jsdrv/jsdrv_stream_buffer.py:44
 #: devices/jsdrv/jsdrv_stream_buffer.py:93
 #: devices/jsdrv/jsdrv_stream_buffer.py:107 plugins/selector.py:58
 #: widgets/settings/settings_widget.py:85
 #: widgets/settings/settings_widget.py:266
 #: widgets/settings/settings_widget.py:364
 #: widgets/settings/settings_widget.py:431
-#: widgets/waveform/waveform_widget.py:3062
+#: widgets/waveform/waveform_widget.py:3104
 msgid "Name"
 msgstr "Nome"
 
 #: devices/jsdrv/jsdrv_stream_buffer.py:45
 msgid "Joulescope stream buffer"
 msgstr "Buffer di flusso Joulescope"
 
@@ -1763,15 +1763,15 @@
 
 #: widgets/accumulator/accumulator_widget.py:27
 #: widgets/value/value_widget.py:31
 msgid "The statistics data stream source."
 msgstr "La fonte del flusso di dati statistici."
 
 #: widgets/accumulator/accumulator_widget.py:32
-#: widgets/value/value_widget.py:74
+#: widgets/value/value_widget.py:81
 msgid "The signal to display."
 msgstr "Il segnale da visualizzare."
 
 #: widgets/accumulator/accumulator_widget.py:34
 msgid "charge"
 msgstr "carica"
 
@@ -1854,15 +1854,15 @@
 
 #: widgets/developer/publish_spy_widget.py:20
 #: widgets/developer/publish_spy_widget.py:21
 msgid "Topic"
 msgstr "Argomento"
 
 #: widgets/developer/publish_spy_widget.py:21
-#: widgets/settings/settings_widget.py:87 widgets/value/value_widget.py:662
+#: widgets/settings/settings_widget.py:87 widgets/value/value_widget.py:669
 msgid "Value"
 msgstr "Valore"
 
 #: widgets/developer/publish_spy_widget.py:24
 msgid "Publish Spy"
 msgstr "Pubblicare la spia"
 
@@ -1892,15 +1892,15 @@
 
 #: widgets/device_control/device_update_dialog.py:24
 #: widgets/device_control/device_update_dialog.py:45
 msgid "Update"
 msgstr "Aggiornamento"
 
 #: widgets/device_control/device_update_dialog.py:25
-#: widgets/value/value_widget.py:147
+#: widgets/value/value_widget.py:155
 msgid "Device"
 msgstr "Dispositivo"
 
 #: widgets/device_control/device_update_dialog.py:27
 #: widgets/progress_bar/progress_bar_widget.py:59
 msgid "Progress"
 msgstr "Progressi"
@@ -2434,18 +2434,14 @@
 msgid "Click to display additional settings and actions."
 msgstr "Fare clic per visualizzare altre impostazioni e azioni."
 
 #: widgets/sidebar/sidebar_widget.py:60
 msgid "sidebar"
 msgstr "barra laterale"
 
-#: widgets/sidebar/sidebar_widget.py:68
-msgid "The flyout width in pixels."
-msgstr "Larghezza del flyout in pixel."
-
 #: widgets/signal_record/disk_full_dialog.py:19
 msgid "The disk is full"
 msgstr "Il disco è pieno"
 
 #: widgets/signal_record/signal_record.py:57
 msgid "Could not open file for write"
 msgstr "Impossibile aprire il file per la scrittura"
@@ -2472,15 +2468,15 @@
 msgid "StatisticsRecordConfig"
 msgstr "StatisticheRegistrazioneConfig"
 
 #: widgets/statistics_record/statistics_record_config_widget.py:123
 msgid "Time Format"
 msgstr "Formato temporale"
 
-#: widgets/trigger/trigger_widget.py:41 widgets/value/value_widget.py:87
+#: widgets/trigger/trigger_widget.py:41 widgets/value/value_widget.py:94
 msgid "Select the source device"
 msgstr "Selezionare il dispositivo sorgente"
 
 #: widgets/trigger/trigger_widget.py:42
 msgid "The device to use for the start condition and stop condition."
 msgstr "Il dispositivo da utilizzare per la condizione di avvio e di arresto."
 
@@ -2652,86 +2648,98 @@
 msgid "Show the statistics fields at the right."
 msgstr "Mostrare i campi delle statistiche a destra."
 
 #: widgets/value/value_widget.py:51
 msgid "Show a leading + or - sign."
 msgstr "Mostrare un segno + o - iniziale."
 
-#: widgets/value/value_widget.py:88
+#: widgets/value/value_widget.py:62
+msgid "Divide the quantity by this value."
+msgstr "Dividere la quantità per questo valore."
+
+#: widgets/value/value_widget.py:63
+msgid ""
+"The divisor is a floating point number. The number may optionally be "
+"followed by units."
+msgstr ""
+"Il divisore è un numero in virgola mobile. Il numero può essere "
+"facoltativamente seguito da unità."
+
+#: widgets/value/value_widget.py:95
 msgid ""
 "The values displayed by this widget come from a single source device. Select"
 " the source device here."
 msgstr ""
 "I valori visualizzati da questo widget provengono da un unico dispositivo "
 "sorgente. Selezionare qui il dispositivo sorgente."
 
-#: widgets/value/value_widget.py:94
+#: widgets/value/value_widget.py:101
 msgid "Hold the display"
 msgstr "Tenere il display"
 
-#: widgets/value/value_widget.py:96
+#: widgets/value/value_widget.py:103
 msgid "When selected, prevent the display from updating."
 msgstr "Se selezionato, impedisce l'aggiornamento del display."
 
-#: widgets/value/value_widget.py:97
+#: widgets/value/value_widget.py:104
 msgid ""
 "The UI also includes a global statistics hold button on the sidebar. When "
 "the global statistics hold button is selected, this button is disabled and "
 "has no effect."
 msgstr ""
 "L'interfaccia utente comprende anche un pulsante di mantenimento delle "
 "statistiche globali nella barra laterale. Quando il pulsante di mantenimento"
 " delle statistiche globali è selezionato, questo pulsante è disabilitato e "
 "non ha alcun effetto."
 
-#: widgets/value/value_widget.py:100
+#: widgets/value/value_widget.py:107
 msgid ""
 "The displayed values normally update with each new statistics data computed "
 "by the device. When this button is selected, the display will not be "
 "updated. However, the statistics will continue accumulate and accrue (if "
 "selected)."
 msgstr ""
 "I valori visualizzati si aggiornano normalmente con ogni nuovo dato "
 "statistico calcolato dal dispositivo. Quando si seleziona questo pulsante, "
 "il display non viene aggiornato. Tuttavia, le statistiche continueranno ad "
 "accumularsi (se selezionato)."
 
-#: widgets/value/value_widget.py:107
+#: widgets/value/value_widget.py:114
 msgid "Accrue values over time"
 msgstr "Accumulare valori nel tempo"
 
-#: widgets/value/value_widget.py:109
+#: widgets/value/value_widget.py:116
 msgid ""
 "Current, voltage, and power are normally computed over a single statistics "
 "frequency interval. Press this button to accrue the values indefinitely. "
 "Press again to return to normal operation."
 msgstr ""
 "La corrente, la tensione e la potenza sono normalmente calcolate su un "
 "singolo intervallo di frequenza statistica. Premere questo pulsante per "
 "accumulare i valori a tempo indeterminato. Premere nuovamente per tornare al"
 " funzionamento normale."
 
-#: widgets/value/value_widget.py:113
+#: widgets/value/value_widget.py:120
 msgid ""
 "Note that this button does not affect the charge and energy accumulation. "
 "Both accumulate indefinitely regardless of this button state."
 msgstr ""
 "Si noti che questo pulsante non influisce sull'accumulo di carica e di "
 "energia. Entrambi si accumulano indefinitamente indipendentemente dallo "
 "stato di questo pulsante."
 
-#: widgets/value/value_widget.py:195
+#: widgets/value/value_widget.py:203
 msgid "Not present"
 msgstr "Non presente"
 
-#: widgets/value/value_widget.py:215
+#: widgets/value/value_widget.py:223
 msgid "Hold"
 msgstr "Tenere"
 
-#: widgets/value/value_widget.py:223
+#: widgets/value/value_widget.py:231
 msgid "Accrue"
 msgstr "Accumulare"
 
 #: widgets/view_manager/view_manager_widget.py:108
 #: widgets/view_manager/view_manager_widget.py:174
 msgid "View Manager"
 msgstr "Visualizza Manager"
@@ -2777,34 +2785,34 @@
 msgstr "triangolo destro"
 
 #: widgets/waveform/text_annotation.py:62
 msgid "triangle left"
 msgstr "triangolo a sinistra"
 
 #: widgets/waveform/text_annotation.py:66
-#: widgets/waveform/waveform_widget.py:3008
+#: widgets/waveform/waveform_widget.py:3050
 msgid "Manual"
 msgstr "Manuale"
 
 #: widgets/waveform/text_annotation.py:67
 msgid "Centered"
 msgstr "Centrato"
 
 #: widgets/waveform/text_annotation.py:99
-#: widgets/waveform/waveform_widget.py:3123
+#: widgets/waveform/waveform_widget.py:3167
 msgid "Text"
 msgstr "Testo"
 
 #: widgets/waveform/text_annotation.py:107
-#: widgets/waveform/waveform_widget.py:3348
+#: widgets/waveform/waveform_widget.py:3398
 msgid "Show text"
 msgstr "Mostra testo"
 
 #: widgets/waveform/text_annotation.py:116
-#: widgets/waveform/waveform_widget.py:3360
+#: widgets/waveform/waveform_widget.py:3410
 msgid "Shape"
 msgstr "Forma"
 
 #: widgets/waveform/text_annotation.py:126
 msgid "Y Mode"
 msgstr "Modalità Y"
 
@@ -3000,322 +3008,322 @@
 "\"default\" will use the default source which is normally configured using "
 "the Device Control widget."
 msgstr ""
 "\"default\" utilizzerà la sorgente predefinita, normalmente configurata "
 "tramite il widget Device Control."
 
 #: widgets/waveform/waveform_source_widget.py:104
-#: widgets/waveform/waveform_widget.py:402
-#: widgets/waveform/waveform_widget.py:479
+#: widgets/waveform/waveform_widget.py:401
+#: widgets/waveform/waveform_widget.py:478
 msgid "off"
 msgstr "off"
 
-#: widgets/waveform/waveform_widget.py:44
+#: widgets/waveform/waveform_widget.py:43
 msgid "Waveform"
 msgstr "Forma d'onda"
 
-#: widgets/waveform/waveform_widget.py:120
+#: widgets/waveform/waveform_widget.py:119
 msgid "General purpose input 0"
 msgstr "Ingresso generico 0"
 
-#: widgets/waveform/waveform_widget.py:121
+#: widgets/waveform/waveform_widget.py:120
 msgid "General purpose input 1"
 msgstr "Ingresso generico 1"
 
-#: widgets/waveform/waveform_widget.py:122
+#: widgets/waveform/waveform_widget.py:121
 msgid "General purpose input 2"
 msgstr "Ingresso generico 2"
 
-#: widgets/waveform/waveform_widget.py:123
+#: widgets/waveform/waveform_widget.py:122
 msgid "General purpose input 3"
 msgstr "Ingresso generico 3"
 
-#: widgets/waveform/waveform_widget.py:358
+#: widgets/waveform/waveform_widget.py:357
 msgid "The source filter string."
 msgstr "La stringa del filtro sorgente."
 
-#: widgets/waveform/waveform_widget.py:369
+#: widgets/waveform/waveform_widget.py:368
 msgid "The trace width."
 msgstr "La larghezza della traccia."
 
-#: widgets/waveform/waveform_widget.py:384
+#: widgets/waveform/waveform_widget.py:383
 msgid "The target frames per second."
 msgstr "I fotogrammi al secondo di riferimento."
 
-#: widgets/waveform/waveform_widget.py:386
+#: widgets/waveform/waveform_widget.py:385
 msgid "vsync"
 msgstr "vsync"
 
-#: widgets/waveform/waveform_widget.py:387
+#: widgets/waveform/waveform_widget.py:386
 msgid "20 Hz"
 msgstr "20 Hz"
 
-#: widgets/waveform/waveform_widget.py:388
+#: widgets/waveform/waveform_widget.py:387
 msgid "10 Hz"
 msgstr "10 Hz"
 
-#: widgets/waveform/waveform_widget.py:389
+#: widgets/waveform/waveform_widget.py:388
 msgid "5 Hz"
 msgstr "5 Hz"
 
-#: widgets/waveform/waveform_widget.py:395
+#: widgets/waveform/waveform_widget.py:394
 msgid "The minimum interval between repaint in milliseconds."
 msgstr "L'intervallo minimo tra un repaint e l'altro, in millisecondi."
 
-#: widgets/waveform/waveform_widget.py:400
+#: widgets/waveform/waveform_widget.py:399
 msgid "Show the minimum and maximum extents fill."
 msgstr "Mostra il riempimento delle estensioni minime e massime."
 
-#: widgets/waveform/waveform_widget.py:403
+#: widgets/waveform/waveform_widget.py:402
 msgid "lines"
 msgstr "linee"
 
-#: widgets/waveform/waveform_widget.py:404
+#: widgets/waveform/waveform_widget.py:403
 msgid "fill 1"
 msgstr "riempimento 1"
 
-#: widgets/waveform/waveform_widget.py:405
+#: widgets/waveform/waveform_widget.py:404
 msgid "fill 2"
 msgstr "riempimento 2"
 
-#: widgets/waveform/waveform_widget.py:411
+#: widgets/waveform/waveform_widget.py:410
 msgid "Show the frames per second."
 msgstr "Mostra i fotogrammi al secondo."
 
-#: widgets/waveform/waveform_widget.py:416
+#: widgets/waveform/waveform_widget.py:415
 msgid "Show the statistics on mouse hover."
 msgstr "Mostra le statistiche al passaggio del mouse."
 
-#: widgets/waveform/waveform_widget.py:421
+#: widgets/waveform/waveform_widget.py:420
 msgid "Show the plot statistics on the right."
 msgstr "Mostrare le statistiche del grafico a destra."
 
-#: widgets/waveform/waveform_widget.py:426
+#: widgets/waveform/waveform_widget.py:425
 msgid "Show frequency for dual markers and statistics."
 msgstr "Mostra la frequenza per i doppi marcatori e le statistiche."
 
-#: widgets/waveform/waveform_widget.py:431
+#: widgets/waveform/waveform_widget.py:430
 msgid "The quantities to display by default."
 msgstr "Le quantità da visualizzare per impostazione predefinita."
 
-#: widgets/waveform/waveform_widget.py:437
+#: widgets/waveform/waveform_widget.py:436
 msgid "The precision to display in digits."
 msgstr "La precisione di visualizzazione in cifre."
 
-#: widgets/waveform/waveform_widget.py:443
+#: widgets/waveform/waveform_widget.py:442
 msgid "Use OpenGL rendering."
 msgstr "Utilizzare il rendering OpenGL."
 
-#: widgets/waveform/waveform_widget.py:454
+#: widgets/waveform/waveform_widget.py:453
 msgid "Pin the left side (oldest) data so that it stays in view."
 msgstr ""
 "Appuntate i dati di sinistra (i più vecchi) in modo che rimangano in vista."
 
-#: widgets/waveform/waveform_widget.py:459
+#: widgets/waveform/waveform_widget.py:458
 msgid "Pin the right side (newest) data so that it stays in view."
 msgstr ""
 "Appuntate i dati sul lato destro (i più recenti) in modo che rimangano in "
 "vista."
 
-#: widgets/waveform/waveform_widget.py:464
+#: widgets/waveform/waveform_widget.py:463
 msgid "The waveform state."
 msgstr "Lo stato della forma d'onda."
 
-#: widgets/waveform/waveform_widget.py:470
+#: widgets/waveform/waveform_widget.py:469
 msgid "The annotations."
 msgstr "Le annotazioni."
 
-#: widgets/waveform/waveform_widget.py:476
+#: widgets/waveform/waveform_widget.py:475
 msgid "Control location"
 msgstr "Posizione di controllo"
 
-#: widgets/waveform/waveform_widget.py:480
+#: widgets/waveform/waveform_widget.py:479
 msgid "top"
 msgstr "top"
 
-#: widgets/waveform/waveform_widget.py:481
+#: widgets/waveform/waveform_widget.py:480
 msgid "bottom"
 msgstr "bottom"
 
-#: widgets/waveform/waveform_widget.py:486
+#: widgets/waveform/waveform_widget.py:485
 msgid "The signal quantity to show in the summary."
 msgstr "La quantità di segnale da mostrare nel riepilogo."
 
-#: widgets/waveform/waveform_widget.py:492
+#: widgets/waveform/waveform_widget.py:491
 msgid "X-axis annotation mode"
 msgstr "Modalità di annotazione sull'asse X"
 
-#: widgets/waveform/waveform_widget.py:495
-#: widgets/waveform/waveform_widget.py:2888
+#: widgets/waveform/waveform_widget.py:494
+#: widgets/waveform/waveform_widget.py:2930
 msgid "Absolute"
 msgstr "Assoluta"
 
-#: widgets/waveform/waveform_widget.py:496
-#: widgets/waveform/waveform_widget.py:2893
+#: widgets/waveform/waveform_widget.py:495
+#: widgets/waveform/waveform_widget.py:2935
 msgid "Relative"
 msgstr "Relativo"
 
-#: widgets/waveform/waveform_widget.py:502
+#: widgets/waveform/waveform_widget.py:501
 msgid "The available subsources."
 msgstr "Le sotto-sorgenti disponibili."
 
-#: widgets/waveform/waveform_widget.py:508
+#: widgets/waveform/waveform_widget.py:507
 msgid "The selected subsources for each trace."
 msgstr "Le sottosorgenti selezionate per ogni traccia."
 
-#: widgets/waveform/waveform_widget.py:514
+#: widgets/waveform/waveform_widget.py:513
 msgid "The trace priority: highest int value on top, None is off."
 msgstr ""
 "La priorità della traccia: il valore int più alto è in cima, nessuno è "
 "spento."
 
-#: widgets/waveform/waveform_widget.py:2834
-#: widgets/waveform/waveform_widget.py:3135
+#: widgets/waveform/waveform_widget.py:2877
+#: widgets/waveform/waveform_widget.py:3179
 msgid "Save image to file"
 msgstr "Salva l'immagine su file"
 
-#: widgets/waveform/waveform_widget.py:2882
-#: widgets/waveform/waveform_widget.py:2951
+#: widgets/waveform/waveform_widget.py:2924
+#: widgets/waveform/waveform_widget.py:2993
 msgid "Single marker"
 msgstr "Marcatore singolo"
 
-#: widgets/waveform/waveform_widget.py:2883
-#: widgets/waveform/waveform_widget.py:2952
+#: widgets/waveform/waveform_widget.py:2925
+#: widgets/waveform/waveform_widget.py:2994
 msgid "Dual markers"
 msgstr "Doppio marcatore"
 
-#: widgets/waveform/waveform_widget.py:2885
+#: widgets/waveform/waveform_widget.py:2927
 msgid "Mode"
 msgstr "Modalità"
 
-#: widgets/waveform/waveform_widget.py:2898
-#: widgets/waveform/waveform_widget.py:2953
-#: widgets/waveform/waveform_widget.py:3111
-#: widgets/waveform/waveform_widget.py:3129
+#: widgets/waveform/waveform_widget.py:2940
+#: widgets/waveform/waveform_widget.py:2995
+#: widgets/waveform/waveform_widget.py:3155
+#: widgets/waveform/waveform_widget.py:3173
 msgid "Clear all"
 msgstr "Cancella tutto"
 
-#: widgets/waveform/waveform_widget.py:2909
-#: widgets/waveform/waveform_widget.py:2998
-#: widgets/waveform/waveform_widget.py:3117
+#: widgets/waveform/waveform_widget.py:2951
+#: widgets/waveform/waveform_widget.py:3040
+#: widgets/waveform/waveform_widget.py:3161
 msgid "Annotations"
 msgstr "Annotazioni"
 
-#: widgets/waveform/waveform_widget.py:3001
+#: widgets/waveform/waveform_widget.py:3043
 msgid "Range"
 msgstr "Gamma"
 
-#: widgets/waveform/waveform_widget.py:3005
-#: widgets/waveform/waveform_widget.py:3328
+#: widgets/waveform/waveform_widget.py:3047
+#: widgets/waveform/waveform_widget.py:3378
 msgid "Auto"
 msgstr "Auto"
 
-#: widgets/waveform/waveform_widget.py:3011
+#: widgets/waveform/waveform_widget.py:3053
 msgid "Exact"
 msgstr "Esatta"
 
-#: widgets/waveform/waveform_widget.py:3020
+#: widgets/waveform/waveform_widget.py:3062
 msgid "Scale"
 msgstr "Scale"
 
-#: widgets/waveform/waveform_widget.py:3023
+#: widgets/waveform/waveform_widget.py:3065
 msgid "Linear"
 msgstr "Lineare"
 
-#: widgets/waveform/waveform_widget.py:3028
+#: widgets/waveform/waveform_widget.py:3070
 msgid "Logarithmic"
 msgstr "Logaritmico"
 
-#: widgets/waveform/waveform_widget.py:3036
+#: widgets/waveform/waveform_widget.py:3078
 msgid "Logarithmic zero"
 msgstr "Zero logaritmico"
 
-#: widgets/waveform/waveform_widget.py:3050
+#: widgets/waveform/waveform_widget.py:3092
 msgid "Preferred prefix"
 msgstr "Prefisso preferito"
 
-#: widgets/waveform/waveform_widget.py:3108
+#: widgets/waveform/waveform_widget.py:3152
 msgid "Add"
 msgstr "Aggiungere"
 
-#: widgets/waveform/waveform_widget.py:3109
+#: widgets/waveform/waveform_widget.py:3153
 msgid "Hide all text"
 msgstr "Nascondi tutto il testo"
 
-#: widgets/waveform/waveform_widget.py:3110
+#: widgets/waveform/waveform_widget.py:3154
 msgid "Show all text"
 msgstr "Mostra tutto il testo"
 
-#: widgets/waveform/waveform_widget.py:3118
+#: widgets/waveform/waveform_widget.py:3162
 msgid "Vertical"
 msgstr "Verticale"
 
-#: widgets/waveform/waveform_widget.py:3121
+#: widgets/waveform/waveform_widget.py:3165
 msgid "Horizontal"
 msgstr "Orizzontale"
 
-#: widgets/waveform/waveform_widget.py:3127
+#: widgets/waveform/waveform_widget.py:3171
 msgid "Save"
 msgstr "Risparmiare"
 
-#: widgets/waveform/waveform_widget.py:3132
+#: widgets/waveform/waveform_widget.py:3176
 msgid "Y-axis auto range"
 msgstr "Gamma automatica dell'asse Y"
 
-#: widgets/waveform/waveform_widget.py:3136
+#: widgets/waveform/waveform_widget.py:3180
 msgid "Copy image to clipboard"
 msgstr "Copia l'immagine negli appunti"
 
-#: widgets/waveform/waveform_widget.py:3137
+#: widgets/waveform/waveform_widget.py:3181
 msgid "Export visible data"
 msgstr "Esportazione di dati visibili"
 
-#: widgets/waveform/waveform_widget.py:3138
+#: widgets/waveform/waveform_widget.py:3182
 msgid "Export all data"
 msgstr "Esportazione di tutti i dati"
 
-#: widgets/waveform/waveform_widget.py:3304
+#: widgets/waveform/waveform_widget.py:3354
 msgid "Export"
 msgstr "Esportazione"
 
-#: widgets/waveform/waveform_widget.py:3305
+#: widgets/waveform/waveform_widget.py:3355
 msgid "Analysis"
 msgstr "Analisi"
 
-#: widgets/waveform/waveform_widget.py:3313
+#: widgets/waveform/waveform_widget.py:3363
 msgid "Interval"
 msgstr "Intervallo"
 
-#: widgets/waveform/waveform_widget.py:3322
+#: widgets/waveform/waveform_widget.py:3372
 msgid "Zoom"
 msgstr "Zoom"
 
-#: widgets/waveform/waveform_widget.py:3326
+#: widgets/waveform/waveform_widget.py:3376
 msgid "Show statistics"
 msgstr "Mostra le statistiche"
 
-#: widgets/waveform/waveform_widget.py:3331
+#: widgets/waveform/waveform_widget.py:3381
 msgid "Left"
 msgstr "A sinistra"
 
-#: widgets/waveform/waveform_widget.py:3334
+#: widgets/waveform/waveform_widget.py:3384
 msgid "Right"
 msgstr "A destra"
 
-#: widgets/waveform/waveform_widget.py:3337
+#: widgets/waveform/waveform_widget.py:3387
 msgid "Off"
 msgstr "Spento"
 
-#: widgets/waveform/waveform_widget.py:3340
-#: widgets/waveform/waveform_widget.py:3368
-#: widgets/waveform/waveform_widget.py:3397
+#: widgets/waveform/waveform_widget.py:3390
+#: widgets/waveform/waveform_widget.py:3418
+#: widgets/waveform/waveform_widget.py:3448
 msgid "Remove"
 msgstr "Rimuovere"
 
-#: widgets/waveform/waveform_widget.py:3351
+#: widgets/waveform/waveform_widget.py:3401
 msgid "Y mode"
 msgstr "Modalità Y"
 
 #: widgets/waveform/y_range_widget.py:67
 msgid "max"
 msgstr "max"
```

### Comparing `joulescope_ui-1.1.6/joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.7/joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.2\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-18 14:15-0400\n"
+"POT-Creation-Date: 2024-05-06 17:27-0400\n"
 "PO-Revision-Date: 2024-04-04 14:45-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: ja\n"
 "Language-Team: ja <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.14.0\n"
+"Generated-By: Babel 2.15.0\n"
 
 msgid "\"3.3 V\" uses an internally-generated 3.3V reference voltage."
 msgstr "「3.3 V」は、内部で生成された3.3V基準電圧を使用します。"
 
 msgid "\"NaN\" sets all samples in the window to NaN."
 msgstr "\"NaN \"はウィンドウ内のすべてのサンプルをNaNに設定します。"
 
@@ -633,14 +633,17 @@
 msgid ""
 "Display the number of actions processed by the publish-subscribe broker in "
 "each second."
 msgstr ""
 "パブリッシュ・サブスクライブ・ブローカーが各秒に処理したアクション数を表示し"
 "ます。"
 
+msgid "Divide the quantity by this value."
+msgstr "この値で量を割る。"
+
 msgid "Do not show again"
 msgstr "再表示しない"
 
 msgid "Do not use any USB hubs, docks or adapters"
 msgstr "USBハブ、ドック、アダプターは使用しないでください。"
 
 msgid "Dual markers"
@@ -1724,31 +1727,33 @@
 "selected)."
 msgstr ""
 "表示値は通常、デバイスによって計算された新しい統計データごとに更新されます。"
 "このボタンを選択すると、表示は更新されません。ただし、統計値は蓄積され続けま"
 "す（選択されている場合）。"
 
 msgid ""
+"The divisor is a floating point number. The number may optionally be "
+"followed by units."
+msgstr "除数は浮動小数点数です。数値の後に単位を付けることもできます。"
+
+msgid ""
 "The exponential decay time constant. The fuse dissipates 63.2 percent of "
 "accumulated energy in this duration."
 msgstr ""
 "指数関数的減衰時定数。ヒューズはこの時間内に蓄積エネルギーの63.2%を消散する。"
 
 msgid "The filename supports the following replacements."
 msgstr "ファイル名は以下の置換に対応しています。"
 
 msgid "The filename with optional replacements."
 msgstr "ファイル名。"
 
 msgid "The fixed default path for loading and saving files."
 msgstr "ファイルをロードおよび保存するための固定デフォルトパス。"
 
-msgid "The flyout width in pixels."
-msgstr "ピクセル単位のフライアウト幅。"
-
 msgid "The font scheme name."
 msgstr "フォントスキーム名。"
 
 msgid "The format string"
 msgstr "フォーマット文字列"
 
 msgid "The fuse trips in Duration at this constant current."
```

### Comparing `joulescope_ui-1.1.6/joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.7/joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.2\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-18 14:15-0400\n"
+"POT-Creation-Date: 2024-05-06 17:27-0400\n"
 "PO-Revision-Date: 2024-04-04 14:45-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: ja <LL@li.org>\n"
 "Language: ja\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"Generated-By: Babel 2.14.0\n"
+"Generated-By: Babel 2.15.0\n"
 
 #: about.py:24
 msgid "About the Joulescope UI"
 msgstr "Joulescope UIについて"
 
 #: about.py:25
 msgid "Version Information"
@@ -292,27 +292,27 @@
 msgid "Email"
 msgstr "電子メール"
 
 #: error_window.py:103
 msgid "Description"
 msgstr "商品概要"
 
-#: error_window.py:112 widgets/waveform/waveform_widget.py:3347
+#: error_window.py:112 widgets/waveform/waveform_widget.py:3397
 msgid "Edit"
 msgstr "編集"
 
 #: error_window.py:113
 msgid "View as Markdown"
 msgstr "マークダウンで表示"
 
 #: error_window.py:119
 msgid "Abort"
 msgstr "中止"
 
-#: error_window.py:120 main.py:365 widgets/settings/settings_widget.py:539
+#: error_window.py:120 main.py:363 widgets/settings/settings_widget.py:539
 msgid "View"
 msgstr "表示"
 
 #: error_window.py:121
 msgid "Submit"
 msgstr "提出"
 
@@ -324,15 +324,15 @@
 msgid "Revert to previous configuration"
 msgstr "前の設定に戻す"
 
 #: error_window.py:282
 msgid "Revert to defaults"
 msgstr "デフォルトに戻す"
 
-#: error_window.py:283 main.py:363 main.py:409
+#: error_window.py:283 main.py:361 main.py:407
 #: widgets/js220_cal/js220_cal_widget.py:38
 msgid "Exit"
 msgstr "終了"
 
 #: exporter.py:49 widgets/signal_record/signal_record_config_widget.py:148
 #: widgets/statistics_record/statistics_record_config_widget.py:111
 msgid "Directory"
@@ -562,156 +562,156 @@
 msgid "Do not show again"
 msgstr "再表示しない"
 
 #: intel_graphics_dialog.py:91
 msgid "Intel graphics detected"
 msgstr "インテル・グラフィックス検出"
 
-#: main.py:70 widgets/value/value_widget.py:653
+#: main.py:69 widgets/value/value_widget.py:660
 msgid "Multimeter"
 msgstr "マルチメーター"
 
-#: main.py:71
+#: main.py:70
 msgid "Oscilloscope"
 msgstr "オシロスコープ"
 
-#: main.py:72 main.py:298 main.py:359 main.py:402
+#: main.py:71 main.py:296 main.py:357 main.py:400
 msgid "File"
 msgstr "ファイル"
 
-#: main.py:82
+#: main.py:81
 msgid "The UI status bar display mode"
 msgstr "UIステータスバー表示モード"
 
-#: main.py:83
+#: main.py:82
 msgid ""
 "This setting controls the amount of detail shown on the status bar at the "
 "bottom of the UI window. You should usually leave this set to \"normal\" "
 "unless you want more detail concerning the UI internal operation."
 msgstr ""
 "この設定は、UIウィンドウの下部にあるステータスバーに表示される詳細の量を制御します。UI の内部動作に関する詳細が必要な場合を除き、通常は "
 "\"normal\" のままに設定してください。"
 
-#: main.py:88 safe_mode.py:43
+#: main.py:87 safe_mode.py:43
 msgid "Normal"
 msgstr "通常"
 
-#: main.py:89
+#: main.py:88
 msgid "Troubleshoot"
 msgstr "トラブルシューティング"
 
-#: main.py:95
+#: main.py:94
 msgid "Enable developer mode."
 msgstr "開発者モードを有効にします。"
 
-#: main.py:108
+#: main.py:107
 msgid "PubSub utilization"
 msgstr "パブサブ利用"
 
-#: main.py:109
+#: main.py:108
 msgid ""
 "Display the number of actions processed by the publish-subscribe broker in "
 "each second."
 msgstr "パブリッシュ・サブスクライブ・ブローカーが各秒に処理したアクション数を表示します。"
 
-#: main.py:114
+#: main.py:113
 msgid "CPU utilization"
 msgstr "CPU使用率"
 
-#: main.py:115
+#: main.py:114
 msgid ""
 "Display the CPU utilization by this application and the total CPU "
 "utilization by all applications. The value is displayed in percent."
 msgstr "このアプリケーションによるCPU使用率と、すべてのアプリケーションによるCPU使用率の合計を表示します。値はパーセントで表示されます。"
 
-#: main.py:121
+#: main.py:120
 msgid "Memory utilization"
 msgstr "メモリ使用率"
 
-#: main.py:122
+#: main.py:121
 msgid ""
 "Display the memory (RAM) utilization by this application and by all "
 "applications. The value is displayed in percent."
 msgstr "このアプリケーションおよびすべてのアプリケーションによるメモリ（RAM）使用率を表示します。値はパーセントで表示されます。"
 
-#: main.py:216
+#: main.py:214
 msgid "UI"
 msgstr "UI"
 
-#: main.py:330
+#: main.py:328
 msgid "Help"
 msgstr "ヘルプ"
 
-#: main.py:331 widgets/hamburger/hamburger_widget.py:21
+#: main.py:329 widgets/hamburger/hamburger_widget.py:21
 msgid "Getting Started"
 msgstr "はじめに"
 
-#: main.py:332
+#: main.py:330
 msgid "User's Guide"
 msgstr "ユーザーガイド"
 
-#: main.py:333 widgets/hamburger/hamburger_widget.py:22
+#: main.py:331 widgets/hamburger/hamburger_widget.py:22
 msgid "Changelog"
 msgstr "変更履歴"
 
-#: main.py:334 widgets/help/help_widget.py:59
+#: main.py:332 widgets/help/help_widget.py:59
 msgid "Report Issue"
 msgstr "報告書発行"
 
-#: main.py:335
+#: main.py:333
 msgid "View logs..."
 msgstr "ログを見る"
 
-#: main.py:336 widgets/hamburger/hamburger_widget.py:23
+#: main.py:334 widgets/hamburger/hamburger_widget.py:23
 msgid "Credits"
 msgstr "クレジット"
 
-#: main.py:337 widgets/hamburger/hamburger_widget.py:24
+#: main.py:335 widgets/hamburger/hamburger_widget.py:24
 msgid "About"
 msgstr "Joulescopeについて"
 
-#: main.py:360
+#: main.py:358
 msgid "Open"
 msgstr "オープン"
 
-#: main.py:361
+#: main.py:359
 msgid "Open recent"
 msgstr "最近のオープン"
 
-#: main.py:362 main.py:408
+#: main.py:360 main.py:406
 msgid "Clear config and exit"
 msgstr "設定をクリアして終了"
 
-#: main.py:366 widgets/settings/settings_widget.py:541
+#: main.py:364 widgets/settings/settings_widget.py:541
 msgid "Widgets"
 msgstr "ウィジェット"
 
-#: main.py:367
+#: main.py:365
 msgid "Tools"
 msgstr "ツール"
 
-#: main.py:368
+#: main.py:366
 msgid "Clear Accumulators"
 msgstr "クリアアキュムレータ"
 
-#: main.py:403
+#: main.py:401
 msgid "Info"
 msgstr "情報"
 
-#: main.py:404 widget_tools.py:92 widgets/settings/settings_widget.py:31
+#: main.py:402 widget_tools.py:92 widgets/settings/settings_widget.py:31
 #: widgets/settings/settings_widget.py:574
 #: widgets/sidebar/sidebar_widget.py:41
 msgid "Settings"
 msgstr "設定"
 
-#: main.py:693
+#: main.py:710
 msgid "Manage"
 msgstr "管理"
 
-#: main.py:730
+#: main.py:747
 msgid "Select file to open"
 msgstr "ファイルを選択して開く"
 
 #: paths.py:30 styles/manager.py:46
 msgid "The name for this widget."
 msgstr "このウィジェットの名称。"
 
@@ -850,47 +850,47 @@
 msgid "Source"
 msgstr "出典"
 
 #: units.py:35
 msgid "Use the application defaults"
 msgstr "アプリケーションのデフォルトを使用"
 
-#: view.py:68
+#: view.py:72
 msgid "The active theme."
 msgstr "アクティブなテーマ"
 
-#: view.py:70
+#: view.py:74
 msgid "Joulescope standard theme"
 msgstr "Joulescope標準テーマ"
 
-#: view.py:70
+#: view.py:74
 msgid "System OS-specific theme"
 msgstr "システムOS固有のテーマ"
 
-#: view.py:75
+#: view.py:79
 msgid "The color scheme name."
 msgstr "配色名。"
 
-#: view.py:77
+#: view.py:81
 msgid "Dark background"
 msgstr "暗い背景"
 
-#: view.py:77
+#: view.py:81
 msgid "Light background"
 msgstr "明るい背景"
 
-#: view.py:81
+#: view.py:85
 msgid "The font scheme name."
 msgstr "フォントスキーム名。"
 
-#: view.py:83
+#: view.py:87
 msgid "Joulescope standard font theme"
 msgstr "Joulescope標準フォントテーマ"
 
-#: view.py:102 widgets/view_manager/view_manager_widget.py:146
+#: view.py:106 widgets/view_manager/view_manager_widget.py:146
 msgid "New View"
 msgstr "新しいビュー"
 
 #: zip_inspector.py:23
 msgid "ZIP Inspector"
 msgstr "ZIPインスペクタ"
 
@@ -991,15 +991,15 @@
 "current cannot flow between the current terminals. In common system setups, "
 "this inhibits target power, which can be used to power cycle reset the "
 "target device."
 msgstr ""
 "有効にすると、電流端子間に電流が流れます。無効にすると、電流端子間に電流が流れなくなります。一般的なシステム・セットアップでは、これによってターゲット電源が抑制され、ターゲット・デバイスのパワー・サイクル・リセットに使用できます。"
 
 #: devices/jsdrv/js110.py:147 devices/jsdrv/js220.py:163
-#: widgets/waveform/waveform_widget.py:110
+#: widgets/waveform/waveform_widget.py:109
 msgid "Current range"
 msgstr "電流レンジ"
 
 #: devices/jsdrv/js110.py:149
 msgid ""
 "Configure the J110's current range. Most applications should use the "
 "default, \"auto\"."
@@ -1123,33 +1123,33 @@
 #: devices/jsdrv/js110.py:255
 msgid ""
 "The number of samples after the current range window used to determine the "
 "mean. This value is ignored for all other IRF types."
 msgstr "平均を決定するために使用される電流範囲ウィンドウの後のサンプル数。他のIRFタイプではこの値は無視されます。"
 
 #: devices/jsdrv/js110.py:269 devices/jsdrv/js220.py:332
-#: widgets/device_control/fuse.py:103 widgets/waveform/waveform_widget.py:105
+#: widgets/device_control/fuse.py:103 widgets/waveform/waveform_widget.py:104
 msgid "Current"
 msgstr "電流"
 
 #: devices/jsdrv/js110.py:270 devices/jsdrv/js220.py:333
 msgid "Enable the current signal streaming."
 msgstr "電流信号ストリーミングを有効にします。"
 
 #: devices/jsdrv/js110.py:278 devices/jsdrv/js220.py:341
-#: widgets/waveform/waveform_widget.py:106
+#: widgets/waveform/waveform_widget.py:105
 msgid "Voltage"
 msgstr "電圧"
 
 #: devices/jsdrv/js110.py:279 devices/jsdrv/js220.py:342
 msgid "Enable the voltage signal streaming."
 msgstr "電圧信号ストリーミングを有効にします。"
 
 #: devices/jsdrv/js110.py:287 devices/jsdrv/js220.py:350
-#: widgets/waveform/waveform_widget.py:107
+#: widgets/waveform/waveform_widget.py:106
 msgid "Power"
 msgstr "パワー"
 
 #: devices/jsdrv/js110.py:288 devices/jsdrv/js220.py:351
 msgid "Enable the power signal streaming."
 msgstr "電源信号ストリーミングを有効にします。"
 
@@ -1333,15 +1333,15 @@
 msgid "GPI 3"
 msgstr "GPI 3"
 
 #: devices/jsdrv/js220.py:402
 msgid "Enable the general purpose input 3 signal streaming."
 msgstr "汎用入力 3 信号ストリーミングを有効にします。"
 
-#: devices/jsdrv/js220.py:410 widgets/waveform/waveform_widget.py:124
+#: devices/jsdrv/js220.py:410 widgets/waveform/waveform_widget.py:123
 msgid "Trigger input"
 msgstr "トリガー入力"
 
 #: devices/jsdrv/js220.py:411
 msgid "Enable the trigger input signal streaming."
 msgstr "トリガー入力信号ストリーミングを有効にします。"
 
@@ -1352,15 +1352,15 @@
 #: devices/jsdrv/jsdrv_stream_buffer.py:44
 #: devices/jsdrv/jsdrv_stream_buffer.py:93
 #: devices/jsdrv/jsdrv_stream_buffer.py:107 plugins/selector.py:58
 #: widgets/settings/settings_widget.py:85
 #: widgets/settings/settings_widget.py:266
 #: widgets/settings/settings_widget.py:364
 #: widgets/settings/settings_widget.py:431
-#: widgets/waveform/waveform_widget.py:3062
+#: widgets/waveform/waveform_widget.py:3104
 msgid "Name"
 msgstr "名称"
 
 #: devices/jsdrv/jsdrv_stream_buffer.py:45
 msgid "Joulescope stream buffer"
 msgstr "Joulescope ストリームバッファ"
 
@@ -1568,15 +1568,15 @@
 
 #: widgets/accumulator/accumulator_widget.py:27
 #: widgets/value/value_widget.py:31
 msgid "The statistics data stream source."
 msgstr "統計データ・ストリーム・ソース。"
 
 #: widgets/accumulator/accumulator_widget.py:32
-#: widgets/value/value_widget.py:74
+#: widgets/value/value_widget.py:81
 msgid "The signal to display."
 msgstr "表示する信号。"
 
 #: widgets/accumulator/accumulator_widget.py:34
 msgid "charge"
 msgstr "チャージ"
 
@@ -1659,15 +1659,15 @@
 
 #: widgets/developer/publish_spy_widget.py:20
 #: widgets/developer/publish_spy_widget.py:21
 msgid "Topic"
 msgstr "トピック"
 
 #: widgets/developer/publish_spy_widget.py:21
-#: widgets/settings/settings_widget.py:87 widgets/value/value_widget.py:662
+#: widgets/settings/settings_widget.py:87 widgets/value/value_widget.py:669
 msgid "Value"
 msgstr "値"
 
 #: widgets/developer/publish_spy_widget.py:24
 msgid "Publish Spy"
 msgstr "スパイを公表する"
 
@@ -1697,15 +1697,15 @@
 
 #: widgets/device_control/device_update_dialog.py:24
 #: widgets/device_control/device_update_dialog.py:45
 msgid "Update"
 msgstr "更新"
 
 #: widgets/device_control/device_update_dialog.py:25
-#: widgets/value/value_widget.py:147
+#: widgets/value/value_widget.py:155
 msgid "Device"
 msgstr "デバイス"
 
 #: widgets/device_control/device_update_dialog.py:27
 #: widgets/progress_bar/progress_bar_widget.py:59
 msgid "Progress"
 msgstr "進捗状況"
@@ -2196,18 +2196,14 @@
 msgid "Click to display additional settings and actions."
 msgstr "クリックすると、追加の設定とアクションが表示されます。"
 
 #: widgets/sidebar/sidebar_widget.py:60
 msgid "sidebar"
 msgstr "サイドバー"
 
-#: widgets/sidebar/sidebar_widget.py:68
-msgid "The flyout width in pixels."
-msgstr "ピクセル単位のフライアウト幅。"
-
 #: widgets/signal_record/disk_full_dialog.py:19
 msgid "The disk is full"
 msgstr "ディスクがいっぱいです"
 
 #: widgets/signal_record/signal_record.py:57
 msgid "Could not open file for write"
 msgstr "書き込み用にファイルを開けませんでした"
@@ -2234,15 +2230,15 @@
 msgid "StatisticsRecordConfig"
 msgstr "統計レコードコンフィグ"
 
 #: widgets/statistics_record/statistics_record_config_widget.py:123
 msgid "Time Format"
 msgstr "時間フォーマット"
 
-#: widgets/trigger/trigger_widget.py:41 widgets/value/value_widget.py:87
+#: widgets/trigger/trigger_widget.py:41 widgets/value/value_widget.py:94
 msgid "Select the source device"
 msgstr "ソースデバイスを選択"
 
 #: widgets/trigger/trigger_widget.py:42
 msgid "The device to use for the start condition and stop condition."
 msgstr "開始条件および停止条件に使用するデバイス。"
 
@@ -2406,72 +2402,82 @@
 msgid "Show the statistics fields at the right."
 msgstr "右側の統計フィールドを表示します。"
 
 #: widgets/value/value_widget.py:51
 msgid "Show a leading + or - sign."
 msgstr "先頭の+または-記号を表示します。"
 
-#: widgets/value/value_widget.py:88
+#: widgets/value/value_widget.py:62
+msgid "Divide the quantity by this value."
+msgstr "この値で量を割る。"
+
+#: widgets/value/value_widget.py:63
+msgid ""
+"The divisor is a floating point number. The number may optionally be "
+"followed by units."
+msgstr "除数は浮動小数点数です。数値の後に単位を付けることもできます。"
+
+#: widgets/value/value_widget.py:95
 msgid ""
 "The values displayed by this widget come from a single source device. Select"
 " the source device here."
 msgstr "このウィジェットで表示される値は、単一のソース・デバイスからのものです。ここでソース・デバイスを選択してください。"
 
-#: widgets/value/value_widget.py:94
+#: widgets/value/value_widget.py:101
 msgid "Hold the display"
 msgstr "ディスプレイを保持する"
 
-#: widgets/value/value_widget.py:96
+#: widgets/value/value_widget.py:103
 msgid "When selected, prevent the display from updating."
 msgstr "選択すると、ディスプレイが更新されないようにします。"
 
-#: widgets/value/value_widget.py:97
+#: widgets/value/value_widget.py:104
 msgid ""
 "The UI also includes a global statistics hold button on the sidebar. When "
 "the global statistics hold button is selected, this button is disabled and "
 "has no effect."
 msgstr ""
 "UIには、サイドバーにグローバル統計ホールドボタンがあります。グローバル統計ホールドボタンが選択されている場合、このボタンは無効になり、何の効果もありません。"
 
-#: widgets/value/value_widget.py:100
+#: widgets/value/value_widget.py:107
 msgid ""
 "The displayed values normally update with each new statistics data computed "
 "by the device. When this button is selected, the display will not be "
 "updated. However, the statistics will continue accumulate and accrue (if "
 "selected)."
 msgstr ""
 "表示値は通常、デバイスによって計算された新しい統計データごとに更新されます。このボタンを選択すると、表示は更新されません。ただし、統計値は蓄積され続けます（選択されている場合）。"
 
-#: widgets/value/value_widget.py:107
+#: widgets/value/value_widget.py:114
 msgid "Accrue values over time"
 msgstr "時間の経過とともに値を蓄積"
 
-#: widgets/value/value_widget.py:109
+#: widgets/value/value_widget.py:116
 msgid ""
 "Current, voltage, and power are normally computed over a single statistics "
 "frequency interval. Press this button to accrue the values indefinitely. "
 "Press again to return to normal operation."
 msgstr ""
 "電流、電圧、電力は通常、1つの統計周波数間隔にわたって計算されます。このボタンを押すと、値が無期限に累積されます。もう一度押すと通常動作に戻ります。"
 
-#: widgets/value/value_widget.py:113
+#: widgets/value/value_widget.py:120
 msgid ""
 "Note that this button does not affect the charge and energy accumulation. "
 "Both accumulate indefinitely regardless of this button state."
 msgstr "このボタンは電荷とエネルギーの蓄積には影響しません。このボタンの状態に関係なく、どちらも無期限に蓄積されます。"
 
-#: widgets/value/value_widget.py:195
+#: widgets/value/value_widget.py:203
 msgid "Not present"
 msgstr "存在しない"
 
-#: widgets/value/value_widget.py:215
+#: widgets/value/value_widget.py:223
 msgid "Hold"
 msgstr "ホールド"
 
-#: widgets/value/value_widget.py:223
+#: widgets/value/value_widget.py:231
 msgid "Accrue"
 msgstr "増加"
 
 #: widgets/view_manager/view_manager_widget.py:108
 #: widgets/view_manager/view_manager_widget.py:174
 msgid "View Manager"
 msgstr "ビュー・マネージャー"
@@ -2517,34 +2523,34 @@
 msgstr "トライアングルライト"
 
 #: widgets/waveform/text_annotation.py:62
 msgid "triangle left"
 msgstr "左三角形"
 
 #: widgets/waveform/text_annotation.py:66
-#: widgets/waveform/waveform_widget.py:3008
+#: widgets/waveform/waveform_widget.py:3050
 msgid "Manual"
 msgstr "マニュアル"
 
 #: widgets/waveform/text_annotation.py:67
 msgid "Centered"
 msgstr "中心"
 
 #: widgets/waveform/text_annotation.py:99
-#: widgets/waveform/waveform_widget.py:3123
+#: widgets/waveform/waveform_widget.py:3167
 msgid "Text"
 msgstr "テキスト"
 
 #: widgets/waveform/text_annotation.py:107
-#: widgets/waveform/waveform_widget.py:3348
+#: widgets/waveform/waveform_widget.py:3398
 msgid "Show text"
 msgstr "テキストを表示"
 
 #: widgets/waveform/text_annotation.py:116
-#: widgets/waveform/waveform_widget.py:3360
+#: widgets/waveform/waveform_widget.py:3410
 msgid "Shape"
 msgstr "形状"
 
 #: widgets/waveform/text_annotation.py:126
 msgid "Y Mode"
 msgstr "Yモード"
 
@@ -2712,317 +2718,317 @@
 #: widgets/waveform/waveform_source_widget.py:40
 msgid ""
 "\"default\" will use the default source which is normally configured using "
 "the Device Control widget."
 msgstr "「default \"は、通常デバイス制御ウィジェットを使用して設定されるデフォルトのソースを使用します。"
 
 #: widgets/waveform/waveform_source_widget.py:104
-#: widgets/waveform/waveform_widget.py:402
-#: widgets/waveform/waveform_widget.py:479
+#: widgets/waveform/waveform_widget.py:401
+#: widgets/waveform/waveform_widget.py:478
 msgid "off"
 msgstr "オフ"
 
-#: widgets/waveform/waveform_widget.py:44
+#: widgets/waveform/waveform_widget.py:43
 msgid "Waveform"
 msgstr "波形"
 
-#: widgets/waveform/waveform_widget.py:120
+#: widgets/waveform/waveform_widget.py:119
 msgid "General purpose input 0"
 msgstr "汎用入力 0"
 
-#: widgets/waveform/waveform_widget.py:121
+#: widgets/waveform/waveform_widget.py:120
 msgid "General purpose input 1"
 msgstr "汎用入力 1"
 
-#: widgets/waveform/waveform_widget.py:122
+#: widgets/waveform/waveform_widget.py:121
 msgid "General purpose input 2"
 msgstr "汎用入力 2"
 
-#: widgets/waveform/waveform_widget.py:123
+#: widgets/waveform/waveform_widget.py:122
 msgid "General purpose input 3"
 msgstr "汎用入力 3"
 
-#: widgets/waveform/waveform_widget.py:358
+#: widgets/waveform/waveform_widget.py:357
 msgid "The source filter string."
 msgstr "ソース・フィルター・ストリング。"
 
-#: widgets/waveform/waveform_widget.py:369
+#: widgets/waveform/waveform_widget.py:368
 msgid "The trace width."
 msgstr "トレース幅。"
 
-#: widgets/waveform/waveform_widget.py:384
+#: widgets/waveform/waveform_widget.py:383
 msgid "The target frames per second."
 msgstr "目標フレーム/秒。"
 
-#: widgets/waveform/waveform_widget.py:386
+#: widgets/waveform/waveform_widget.py:385
 msgid "vsync"
 msgstr "vsync"
 
-#: widgets/waveform/waveform_widget.py:387
+#: widgets/waveform/waveform_widget.py:386
 msgid "20 Hz"
 msgstr "20 Hz"
 
-#: widgets/waveform/waveform_widget.py:388
+#: widgets/waveform/waveform_widget.py:387
 msgid "10 Hz"
 msgstr "10 Hz"
 
-#: widgets/waveform/waveform_widget.py:389
+#: widgets/waveform/waveform_widget.py:388
 msgid "5 Hz"
 msgstr "5 Hz"
 
-#: widgets/waveform/waveform_widget.py:395
+#: widgets/waveform/waveform_widget.py:394
 msgid "The minimum interval between repaint in milliseconds."
 msgstr "再描画の最小間隔（ミリ秒）。"
 
-#: widgets/waveform/waveform_widget.py:400
+#: widgets/waveform/waveform_widget.py:399
 msgid "Show the minimum and maximum extents fill."
 msgstr "最小および最大エクステントを表示します。"
 
-#: widgets/waveform/waveform_widget.py:403
+#: widgets/waveform/waveform_widget.py:402
 msgid "lines"
 msgstr "ライン"
 
-#: widgets/waveform/waveform_widget.py:404
+#: widgets/waveform/waveform_widget.py:403
 msgid "fill 1"
 msgstr "充填 1"
 
-#: widgets/waveform/waveform_widget.py:405
+#: widgets/waveform/waveform_widget.py:404
 msgid "fill 2"
 msgstr "フィル 2"
 
-#: widgets/waveform/waveform_widget.py:411
+#: widgets/waveform/waveform_widget.py:410
 msgid "Show the frames per second."
 msgstr "フレーム/秒を表示します。"
 
-#: widgets/waveform/waveform_widget.py:416
+#: widgets/waveform/waveform_widget.py:415
 msgid "Show the statistics on mouse hover."
 msgstr "マウスホバーで統計を表示します。"
 
-#: widgets/waveform/waveform_widget.py:421
+#: widgets/waveform/waveform_widget.py:420
 msgid "Show the plot statistics on the right."
 msgstr "右側にプロット統計を表示します。"
 
-#: widgets/waveform/waveform_widget.py:426
+#: widgets/waveform/waveform_widget.py:425
 msgid "Show frequency for dual markers and statistics."
 msgstr "デュアルマーカーと統計のために周波数を表示します。"
 
-#: widgets/waveform/waveform_widget.py:431
+#: widgets/waveform/waveform_widget.py:430
 msgid "The quantities to display by default."
 msgstr "デフォルトで表示する量。"
 
-#: widgets/waveform/waveform_widget.py:437
+#: widgets/waveform/waveform_widget.py:436
 msgid "The precision to display in digits."
 msgstr "桁で表示する精度。"
 
-#: widgets/waveform/waveform_widget.py:443
+#: widgets/waveform/waveform_widget.py:442
 msgid "Use OpenGL rendering."
 msgstr "OpenGLレンダリングを使用します。"
 
-#: widgets/waveform/waveform_widget.py:454
+#: widgets/waveform/waveform_widget.py:453
 msgid "Pin the left side (oldest) data so that it stays in view."
 msgstr "左側（最も古い）のデータをピン留めして、表示されたままにします。"
 
-#: widgets/waveform/waveform_widget.py:459
+#: widgets/waveform/waveform_widget.py:458
 msgid "Pin the right side (newest) data so that it stays in view."
 msgstr "右側（最新）のデータをピン留めして、表示されたままにします。"
 
-#: widgets/waveform/waveform_widget.py:464
+#: widgets/waveform/waveform_widget.py:463
 msgid "The waveform state."
 msgstr "波形の状態。"
 
-#: widgets/waveform/waveform_widget.py:470
+#: widgets/waveform/waveform_widget.py:469
 msgid "The annotations."
 msgstr "注釈"
 
-#: widgets/waveform/waveform_widget.py:476
+#: widgets/waveform/waveform_widget.py:475
 msgid "Control location"
 msgstr "制御位置"
 
-#: widgets/waveform/waveform_widget.py:480
+#: widgets/waveform/waveform_widget.py:479
 msgid "top"
 msgstr "トップ"
 
-#: widgets/waveform/waveform_widget.py:481
+#: widgets/waveform/waveform_widget.py:480
 msgid "bottom"
 msgstr "ボトム"
 
-#: widgets/waveform/waveform_widget.py:486
+#: widgets/waveform/waveform_widget.py:485
 msgid "The signal quantity to show in the summary."
 msgstr "サマリーに表示する信号量。"
 
-#: widgets/waveform/waveform_widget.py:492
+#: widgets/waveform/waveform_widget.py:491
 msgid "X-axis annotation mode"
 msgstr "X軸注釈モード"
 
-#: widgets/waveform/waveform_widget.py:495
-#: widgets/waveform/waveform_widget.py:2888
+#: widgets/waveform/waveform_widget.py:494
+#: widgets/waveform/waveform_widget.py:2930
 msgid "Absolute"
 msgstr "絶対値"
 
-#: widgets/waveform/waveform_widget.py:496
-#: widgets/waveform/waveform_widget.py:2893
+#: widgets/waveform/waveform_widget.py:495
+#: widgets/waveform/waveform_widget.py:2935
 msgid "Relative"
 msgstr "相対"
 
-#: widgets/waveform/waveform_widget.py:502
+#: widgets/waveform/waveform_widget.py:501
 msgid "The available subsources."
 msgstr "利用可能なサブソース"
 
-#: widgets/waveform/waveform_widget.py:508
+#: widgets/waveform/waveform_widget.py:507
 msgid "The selected subsources for each trace."
 msgstr "各トレースで選択されたサブソース。"
 
-#: widgets/waveform/waveform_widget.py:514
+#: widgets/waveform/waveform_widget.py:513
 msgid "The trace priority: highest int value on top, None is off."
 msgstr "トレースの優先順位：最高 int 値が一番上、None はオフ。"
 
-#: widgets/waveform/waveform_widget.py:2834
-#: widgets/waveform/waveform_widget.py:3135
+#: widgets/waveform/waveform_widget.py:2877
+#: widgets/waveform/waveform_widget.py:3179
 msgid "Save image to file"
 msgstr "画像をファイルに保存"
 
-#: widgets/waveform/waveform_widget.py:2882
-#: widgets/waveform/waveform_widget.py:2951
+#: widgets/waveform/waveform_widget.py:2924
+#: widgets/waveform/waveform_widget.py:2993
 msgid "Single marker"
 msgstr "シングルマーカー"
 
-#: widgets/waveform/waveform_widget.py:2883
-#: widgets/waveform/waveform_widget.py:2952
+#: widgets/waveform/waveform_widget.py:2925
+#: widgets/waveform/waveform_widget.py:2994
 msgid "Dual markers"
 msgstr "デュアルマーカー"
 
-#: widgets/waveform/waveform_widget.py:2885
+#: widgets/waveform/waveform_widget.py:2927
 msgid "Mode"
 msgstr "モード"
 
-#: widgets/waveform/waveform_widget.py:2898
-#: widgets/waveform/waveform_widget.py:2953
-#: widgets/waveform/waveform_widget.py:3111
-#: widgets/waveform/waveform_widget.py:3129
+#: widgets/waveform/waveform_widget.py:2940
+#: widgets/waveform/waveform_widget.py:2995
+#: widgets/waveform/waveform_widget.py:3155
+#: widgets/waveform/waveform_widget.py:3173
 msgid "Clear all"
 msgstr "すべてクリア"
 
-#: widgets/waveform/waveform_widget.py:2909
-#: widgets/waveform/waveform_widget.py:2998
-#: widgets/waveform/waveform_widget.py:3117
+#: widgets/waveform/waveform_widget.py:2951
+#: widgets/waveform/waveform_widget.py:3040
+#: widgets/waveform/waveform_widget.py:3161
 msgid "Annotations"
 msgstr "注釈"
 
-#: widgets/waveform/waveform_widget.py:3001
+#: widgets/waveform/waveform_widget.py:3043
 msgid "Range"
 msgstr "測定範囲"
 
-#: widgets/waveform/waveform_widget.py:3005
-#: widgets/waveform/waveform_widget.py:3328
+#: widgets/waveform/waveform_widget.py:3047
+#: widgets/waveform/waveform_widget.py:3378
 msgid "Auto"
 msgstr "オート"
 
-#: widgets/waveform/waveform_widget.py:3011
+#: widgets/waveform/waveform_widget.py:3053
 msgid "Exact"
 msgstr "正確"
 
-#: widgets/waveform/waveform_widget.py:3020
+#: widgets/waveform/waveform_widget.py:3062
 msgid "Scale"
 msgstr "スケール"
 
-#: widgets/waveform/waveform_widget.py:3023
+#: widgets/waveform/waveform_widget.py:3065
 msgid "Linear"
 msgstr "リニア"
 
-#: widgets/waveform/waveform_widget.py:3028
+#: widgets/waveform/waveform_widget.py:3070
 msgid "Logarithmic"
 msgstr "対数"
 
-#: widgets/waveform/waveform_widget.py:3036
+#: widgets/waveform/waveform_widget.py:3078
 msgid "Logarithmic zero"
 msgstr "対数ゼロ"
 
-#: widgets/waveform/waveform_widget.py:3050
+#: widgets/waveform/waveform_widget.py:3092
 msgid "Preferred prefix"
 msgstr "優先接頭辞"
 
-#: widgets/waveform/waveform_widget.py:3108
+#: widgets/waveform/waveform_widget.py:3152
 msgid "Add"
 msgstr "追加"
 
-#: widgets/waveform/waveform_widget.py:3109
+#: widgets/waveform/waveform_widget.py:3153
 msgid "Hide all text"
 msgstr "すべてのテキストを隠す"
 
-#: widgets/waveform/waveform_widget.py:3110
+#: widgets/waveform/waveform_widget.py:3154
 msgid "Show all text"
 msgstr "すべてのテキストを表示"
 
-#: widgets/waveform/waveform_widget.py:3118
+#: widgets/waveform/waveform_widget.py:3162
 msgid "Vertical"
 msgstr "垂直"
 
-#: widgets/waveform/waveform_widget.py:3121
+#: widgets/waveform/waveform_widget.py:3165
 msgid "Horizontal"
 msgstr "水平"
 
-#: widgets/waveform/waveform_widget.py:3127
+#: widgets/waveform/waveform_widget.py:3171
 msgid "Save"
 msgstr "節約"
 
-#: widgets/waveform/waveform_widget.py:3132
+#: widgets/waveform/waveform_widget.py:3176
 msgid "Y-axis auto range"
 msgstr "Y軸オートレンジ"
 
-#: widgets/waveform/waveform_widget.py:3136
+#: widgets/waveform/waveform_widget.py:3180
 msgid "Copy image to clipboard"
 msgstr "画像をクリップボードにコピー"
 
-#: widgets/waveform/waveform_widget.py:3137
+#: widgets/waveform/waveform_widget.py:3181
 msgid "Export visible data"
 msgstr "可視データをエクスポート"
 
-#: widgets/waveform/waveform_widget.py:3138
+#: widgets/waveform/waveform_widget.py:3182
 msgid "Export all data"
 msgstr "すべてのデータをエクスポート"
 
-#: widgets/waveform/waveform_widget.py:3304
+#: widgets/waveform/waveform_widget.py:3354
 msgid "Export"
 msgstr "輸出"
 
-#: widgets/waveform/waveform_widget.py:3305
+#: widgets/waveform/waveform_widget.py:3355
 msgid "Analysis"
 msgstr "解析"
 
-#: widgets/waveform/waveform_widget.py:3313
+#: widgets/waveform/waveform_widget.py:3363
 msgid "Interval"
 msgstr "インターバル"
 
-#: widgets/waveform/waveform_widget.py:3322
+#: widgets/waveform/waveform_widget.py:3372
 msgid "Zoom"
 msgstr "ズーム"
 
-#: widgets/waveform/waveform_widget.py:3326
+#: widgets/waveform/waveform_widget.py:3376
 msgid "Show statistics"
 msgstr "統計を表示"
 
-#: widgets/waveform/waveform_widget.py:3331
+#: widgets/waveform/waveform_widget.py:3381
 msgid "Left"
 msgstr "左"
 
-#: widgets/waveform/waveform_widget.py:3334
+#: widgets/waveform/waveform_widget.py:3384
 msgid "Right"
 msgstr "右"
 
-#: widgets/waveform/waveform_widget.py:3337
+#: widgets/waveform/waveform_widget.py:3387
 msgid "Off"
 msgstr "オフ"
 
-#: widgets/waveform/waveform_widget.py:3340
-#: widgets/waveform/waveform_widget.py:3368
-#: widgets/waveform/waveform_widget.py:3397
+#: widgets/waveform/waveform_widget.py:3390
+#: widgets/waveform/waveform_widget.py:3418
+#: widgets/waveform/waveform_widget.py:3448
 msgid "Remove"
 msgstr "削除"
 
-#: widgets/waveform/waveform_widget.py:3351
+#: widgets/waveform/waveform_widget.py:3401
 msgid "Y mode"
 msgstr "Yモード"
 
 #: widgets/waveform/y_range_widget.py:67
 msgid "max"
 msgstr "最大"
```

### Comparing `joulescope_ui-1.1.6/joulescope_ui/locale/joulescope_ui.pot` & `joulescope_ui-1.1.7/joulescope_ui/locale/joulescope_ui.pot`

 * *Files 0% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 # Copyright (C) 2024 Jetperch LLC
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #
 #, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: PROJECT 1.1.6\n"
+"Project-Id-Version: PROJECT 1.1.7\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-18 14:15-0400\n"
+"POT-Creation-Date: 2024-05-06 17:27-0400\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.14.0\n"
+"Generated-By: Babel 2.15.0\n"
 
 #: about.py:24
 msgid "About the Joulescope UI"
 msgstr ""
 
 #: about.py:25
 msgid "Version Information"
@@ -284,27 +284,27 @@
 msgid "Email"
 msgstr ""
 
 #: error_window.py:103
 msgid "Description"
 msgstr ""
 
-#: error_window.py:112 widgets/waveform/waveform_widget.py:3347
+#: error_window.py:112 widgets/waveform/waveform_widget.py:3397
 msgid "Edit"
 msgstr ""
 
 #: error_window.py:113
 msgid "View as Markdown"
 msgstr ""
 
 #: error_window.py:119
 msgid "Abort"
 msgstr ""
 
-#: error_window.py:120 main.py:365 widgets/settings/settings_widget.py:539
+#: error_window.py:120 main.py:363 widgets/settings/settings_widget.py:539
 msgid "View"
 msgstr ""
 
 #: error_window.py:121
 msgid "Submit"
 msgstr ""
 
@@ -316,15 +316,15 @@
 msgid "Revert to previous configuration"
 msgstr ""
 
 #: error_window.py:282
 msgid "Revert to defaults"
 msgstr ""
 
-#: error_window.py:283 main.py:363 main.py:409
+#: error_window.py:283 main.py:361 main.py:407
 #: widgets/js220_cal/js220_cal_widget.py:38
 msgid "Exit"
 msgstr ""
 
 #: exporter.py:49 widgets/signal_record/signal_record_config_widget.py:148
 #: widgets/statistics_record/statistics_record_config_widget.py:111
 msgid "Directory"
@@ -542,154 +542,154 @@
 msgid "Do not show again"
 msgstr ""
 
 #: intel_graphics_dialog.py:91
 msgid "Intel graphics detected"
 msgstr ""
 
-#: main.py:70 widgets/value/value_widget.py:653
+#: main.py:69 widgets/value/value_widget.py:660
 msgid "Multimeter"
 msgstr ""
 
-#: main.py:71
+#: main.py:70
 msgid "Oscilloscope"
 msgstr ""
 
-#: main.py:72 main.py:298 main.py:359 main.py:402
+#: main.py:71 main.py:296 main.py:357 main.py:400
 msgid "File"
 msgstr ""
 
-#: main.py:82
+#: main.py:81
 msgid "The UI status bar display mode"
 msgstr ""
 
-#: main.py:83
+#: main.py:82
 msgid ""
 "This setting controls the amount of detail shown on the status bar at the "
 "bottom of the UI window. You should usually leave this set to \"normal\" "
 "unless you want more detail concerning the UI internal operation."
 msgstr ""
 
-#: main.py:88 safe_mode.py:43
+#: main.py:87 safe_mode.py:43
 msgid "Normal"
 msgstr ""
 
-#: main.py:89
+#: main.py:88
 msgid "Troubleshoot"
 msgstr ""
 
-#: main.py:95
+#: main.py:94
 msgid "Enable developer mode."
 msgstr ""
 
-#: main.py:108
+#: main.py:107
 msgid "PubSub utilization"
 msgstr ""
 
-#: main.py:109
+#: main.py:108
 msgid ""
 "Display the number of actions processed by the publish-subscribe broker in "
 "each second."
 msgstr ""
 
-#: main.py:114
+#: main.py:113
 msgid "CPU utilization"
 msgstr ""
 
-#: main.py:115
+#: main.py:114
 msgid ""
 "Display the CPU utilization by this application and the total CPU "
 "utilization by all applications. The value is displayed in percent."
 msgstr ""
 
-#: main.py:121
+#: main.py:120
 msgid "Memory utilization"
 msgstr ""
 
-#: main.py:122
+#: main.py:121
 msgid ""
 "Display the memory (RAM) utilization by this application and by all "
 "applications. The value is displayed in percent."
 msgstr ""
 
-#: main.py:216
+#: main.py:214
 msgid "UI"
 msgstr ""
 
-#: main.py:330
+#: main.py:328
 msgid "Help"
 msgstr ""
 
-#: main.py:331 widgets/hamburger/hamburger_widget.py:21
+#: main.py:329 widgets/hamburger/hamburger_widget.py:21
 msgid "Getting Started"
 msgstr ""
 
-#: main.py:332
+#: main.py:330
 msgid "User's Guide"
 msgstr ""
 
-#: main.py:333 widgets/hamburger/hamburger_widget.py:22
+#: main.py:331 widgets/hamburger/hamburger_widget.py:22
 msgid "Changelog"
 msgstr ""
 
-#: main.py:334 widgets/help/help_widget.py:59
+#: main.py:332 widgets/help/help_widget.py:59
 msgid "Report Issue"
 msgstr ""
 
-#: main.py:335
+#: main.py:333
 msgid "View logs..."
 msgstr ""
 
-#: main.py:336 widgets/hamburger/hamburger_widget.py:23
+#: main.py:334 widgets/hamburger/hamburger_widget.py:23
 msgid "Credits"
 msgstr ""
 
-#: main.py:337 widgets/hamburger/hamburger_widget.py:24
+#: main.py:335 widgets/hamburger/hamburger_widget.py:24
 msgid "About"
 msgstr ""
 
-#: main.py:360
+#: main.py:358
 msgid "Open"
 msgstr ""
 
-#: main.py:361
+#: main.py:359
 msgid "Open recent"
 msgstr ""
 
-#: main.py:362 main.py:408
+#: main.py:360 main.py:406
 msgid "Clear config and exit"
 msgstr ""
 
-#: main.py:366 widgets/settings/settings_widget.py:541
+#: main.py:364 widgets/settings/settings_widget.py:541
 msgid "Widgets"
 msgstr ""
 
-#: main.py:367
+#: main.py:365
 msgid "Tools"
 msgstr ""
 
-#: main.py:368
+#: main.py:366
 msgid "Clear Accumulators"
 msgstr ""
 
-#: main.py:403
+#: main.py:401
 msgid "Info"
 msgstr ""
 
-#: main.py:404 widget_tools.py:92 widgets/settings/settings_widget.py:31
+#: main.py:402 widget_tools.py:92 widgets/settings/settings_widget.py:31
 #: widgets/settings/settings_widget.py:574
 #: widgets/sidebar/sidebar_widget.py:41
 msgid "Settings"
 msgstr ""
 
-#: main.py:693
+#: main.py:710
 msgid "Manage"
 msgstr ""
 
-#: main.py:730
+#: main.py:747
 msgid "Select file to open"
 msgstr ""
 
 #: paths.py:30 styles/manager.py:46
 msgid "The name for this widget."
 msgstr ""
 
@@ -828,47 +828,47 @@
 msgid "Source"
 msgstr ""
 
 #: units.py:35
 msgid "Use the application defaults"
 msgstr ""
 
-#: view.py:68
+#: view.py:72
 msgid "The active theme."
 msgstr ""
 
-#: view.py:70
+#: view.py:74
 msgid "Joulescope standard theme"
 msgstr ""
 
-#: view.py:70
+#: view.py:74
 msgid "System OS-specific theme"
 msgstr ""
 
-#: view.py:75
+#: view.py:79
 msgid "The color scheme name."
 msgstr ""
 
-#: view.py:77
+#: view.py:81
 msgid "Dark background"
 msgstr ""
 
-#: view.py:77
+#: view.py:81
 msgid "Light background"
 msgstr ""
 
-#: view.py:81
+#: view.py:85
 msgid "The font scheme name."
 msgstr ""
 
-#: view.py:83
+#: view.py:87
 msgid "Joulescope standard font theme"
 msgstr ""
 
-#: view.py:102 widgets/view_manager/view_manager_widget.py:146
+#: view.py:106 widgets/view_manager/view_manager_widget.py:146
 msgid "New View"
 msgstr ""
 
 #: zip_inspector.py:23
 msgid "ZIP Inspector"
 msgstr ""
 
@@ -962,15 +962,15 @@
 "When enabled, current flows between the current terminals. When disabled, "
 "current cannot flow between the current terminals. In common system setups, "
 "this inhibits target power, which can be used to power cycle reset the "
 "target device."
 msgstr ""
 
 #: devices/jsdrv/js110.py:147 devices/jsdrv/js220.py:163
-#: widgets/waveform/waveform_widget.py:110
+#: widgets/waveform/waveform_widget.py:109
 msgid "Current range"
 msgstr ""
 
 #: devices/jsdrv/js110.py:149
 msgid ""
 "Configure the J110's current range. Most applications should use the "
 "default, \"auto\"."
@@ -1086,33 +1086,33 @@
 #: devices/jsdrv/js110.py:255
 msgid ""
 "The number of samples after the current range window used to determine the "
 "mean. This value is ignored for all other IRF types."
 msgstr ""
 
 #: devices/jsdrv/js110.py:269 devices/jsdrv/js220.py:332
-#: widgets/device_control/fuse.py:103 widgets/waveform/waveform_widget.py:105
+#: widgets/device_control/fuse.py:103 widgets/waveform/waveform_widget.py:104
 msgid "Current"
 msgstr ""
 
 #: devices/jsdrv/js110.py:270 devices/jsdrv/js220.py:333
 msgid "Enable the current signal streaming."
 msgstr ""
 
 #: devices/jsdrv/js110.py:278 devices/jsdrv/js220.py:341
-#: widgets/waveform/waveform_widget.py:106
+#: widgets/waveform/waveform_widget.py:105
 msgid "Voltage"
 msgstr ""
 
 #: devices/jsdrv/js110.py:279 devices/jsdrv/js220.py:342
 msgid "Enable the voltage signal streaming."
 msgstr ""
 
 #: devices/jsdrv/js110.py:287 devices/jsdrv/js220.py:350
-#: widgets/waveform/waveform_widget.py:107
+#: widgets/waveform/waveform_widget.py:106
 msgid "Power"
 msgstr ""
 
 #: devices/jsdrv/js110.py:288 devices/jsdrv/js220.py:351
 msgid "Enable the power signal streaming."
 msgstr ""
 
@@ -1289,15 +1289,15 @@
 msgid "GPI 3"
 msgstr ""
 
 #: devices/jsdrv/js220.py:402
 msgid "Enable the general purpose input 3 signal streaming."
 msgstr ""
 
-#: devices/jsdrv/js220.py:410 widgets/waveform/waveform_widget.py:124
+#: devices/jsdrv/js220.py:410 widgets/waveform/waveform_widget.py:123
 msgid "Trigger input"
 msgstr ""
 
 #: devices/jsdrv/js220.py:411
 msgid "Enable the trigger input signal streaming."
 msgstr ""
 
@@ -1308,15 +1308,15 @@
 #: devices/jsdrv/jsdrv_stream_buffer.py:44
 #: devices/jsdrv/jsdrv_stream_buffer.py:93
 #: devices/jsdrv/jsdrv_stream_buffer.py:107 plugins/selector.py:58
 #: widgets/settings/settings_widget.py:85
 #: widgets/settings/settings_widget.py:266
 #: widgets/settings/settings_widget.py:364
 #: widgets/settings/settings_widget.py:431
-#: widgets/waveform/waveform_widget.py:3062
+#: widgets/waveform/waveform_widget.py:3104
 msgid "Name"
 msgstr ""
 
 #: devices/jsdrv/jsdrv_stream_buffer.py:45
 msgid "Joulescope stream buffer"
 msgstr ""
 
@@ -1522,15 +1522,15 @@
 
 #: widgets/accumulator/accumulator_widget.py:27
 #: widgets/value/value_widget.py:31
 msgid "The statistics data stream source."
 msgstr ""
 
 #: widgets/accumulator/accumulator_widget.py:32
-#: widgets/value/value_widget.py:74
+#: widgets/value/value_widget.py:81
 msgid "The signal to display."
 msgstr ""
 
 #: widgets/accumulator/accumulator_widget.py:34
 msgid "charge"
 msgstr ""
 
@@ -1613,15 +1613,15 @@
 
 #: widgets/developer/publish_spy_widget.py:20
 #: widgets/developer/publish_spy_widget.py:21
 msgid "Topic"
 msgstr ""
 
 #: widgets/developer/publish_spy_widget.py:21
-#: widgets/settings/settings_widget.py:87 widgets/value/value_widget.py:662
+#: widgets/settings/settings_widget.py:87 widgets/value/value_widget.py:669
 msgid "Value"
 msgstr ""
 
 #: widgets/developer/publish_spy_widget.py:24
 msgid "Publish Spy"
 msgstr ""
 
@@ -1651,15 +1651,15 @@
 
 #: widgets/device_control/device_update_dialog.py:24
 #: widgets/device_control/device_update_dialog.py:45
 msgid "Update"
 msgstr ""
 
 #: widgets/device_control/device_update_dialog.py:25
-#: widgets/value/value_widget.py:147
+#: widgets/value/value_widget.py:155
 msgid "Device"
 msgstr ""
 
 #: widgets/device_control/device_update_dialog.py:27
 #: widgets/progress_bar/progress_bar_widget.py:59
 msgid "Progress"
 msgstr ""
@@ -2137,18 +2137,14 @@
 msgid "Click to display additional settings and actions."
 msgstr ""
 
 #: widgets/sidebar/sidebar_widget.py:60
 msgid "sidebar"
 msgstr ""
 
-#: widgets/sidebar/sidebar_widget.py:68
-msgid "The flyout width in pixels."
-msgstr ""
-
 #: widgets/signal_record/disk_full_dialog.py:19
 msgid "The disk is full"
 msgstr ""
 
 #: widgets/signal_record/signal_record.py:57
 msgid "Could not open file for write"
 msgstr ""
@@ -2175,15 +2171,15 @@
 msgid "StatisticsRecordConfig"
 msgstr ""
 
 #: widgets/statistics_record/statistics_record_config_widget.py:123
 msgid "Time Format"
 msgstr ""
 
-#: widgets/trigger/trigger_widget.py:41 widgets/value/value_widget.py:87
+#: widgets/trigger/trigger_widget.py:41 widgets/value/value_widget.py:94
 msgid "Select the source device"
 msgstr ""
 
 #: widgets/trigger/trigger_widget.py:42
 msgid "The device to use for the start condition and stop condition."
 msgstr ""
 
@@ -2346,69 +2342,79 @@
 msgid "Show the statistics fields at the right."
 msgstr ""
 
 #: widgets/value/value_widget.py:51
 msgid "Show a leading + or - sign."
 msgstr ""
 
-#: widgets/value/value_widget.py:88
+#: widgets/value/value_widget.py:62
+msgid "Divide the quantity by this value."
+msgstr ""
+
+#: widgets/value/value_widget.py:63
+msgid ""
+"The divisor is a floating point number. The number may optionally be "
+"followed by units."
+msgstr ""
+
+#: widgets/value/value_widget.py:95
 msgid ""
 "The values displayed by this widget come from a single source device. Select"
 " the source device here."
 msgstr ""
 
-#: widgets/value/value_widget.py:94
+#: widgets/value/value_widget.py:101
 msgid "Hold the display"
 msgstr ""
 
-#: widgets/value/value_widget.py:96
+#: widgets/value/value_widget.py:103
 msgid "When selected, prevent the display from updating."
 msgstr ""
 
-#: widgets/value/value_widget.py:97
+#: widgets/value/value_widget.py:104
 msgid ""
 "The UI also includes a global statistics hold button on the sidebar. When "
 "the global statistics hold button is selected, this button is disabled and "
 "has no effect."
 msgstr ""
 
-#: widgets/value/value_widget.py:100
+#: widgets/value/value_widget.py:107
 msgid ""
 "The displayed values normally update with each new statistics data computed "
 "by the device. When this button is selected, the display will not be "
 "updated. However, the statistics will continue accumulate and accrue (if "
 "selected)."
 msgstr ""
 
-#: widgets/value/value_widget.py:107
+#: widgets/value/value_widget.py:114
 msgid "Accrue values over time"
 msgstr ""
 
-#: widgets/value/value_widget.py:109
+#: widgets/value/value_widget.py:116
 msgid ""
 "Current, voltage, and power are normally computed over a single statistics "
 "frequency interval. Press this button to accrue the values indefinitely. "
 "Press again to return to normal operation."
 msgstr ""
 
-#: widgets/value/value_widget.py:113
+#: widgets/value/value_widget.py:120
 msgid ""
 "Note that this button does not affect the charge and energy accumulation. "
 "Both accumulate indefinitely regardless of this button state."
 msgstr ""
 
-#: widgets/value/value_widget.py:195
+#: widgets/value/value_widget.py:203
 msgid "Not present"
 msgstr ""
 
-#: widgets/value/value_widget.py:215
+#: widgets/value/value_widget.py:223
 msgid "Hold"
 msgstr ""
 
-#: widgets/value/value_widget.py:223
+#: widgets/value/value_widget.py:231
 msgid "Accrue"
 msgstr ""
 
 #: widgets/view_manager/view_manager_widget.py:108
 #: widgets/view_manager/view_manager_widget.py:174
 msgid "View Manager"
 msgstr ""
@@ -2454,34 +2460,34 @@
 msgstr ""
 
 #: widgets/waveform/text_annotation.py:62
 msgid "triangle left"
 msgstr ""
 
 #: widgets/waveform/text_annotation.py:66
-#: widgets/waveform/waveform_widget.py:3008
+#: widgets/waveform/waveform_widget.py:3050
 msgid "Manual"
 msgstr ""
 
 #: widgets/waveform/text_annotation.py:67
 msgid "Centered"
 msgstr ""
 
 #: widgets/waveform/text_annotation.py:99
-#: widgets/waveform/waveform_widget.py:3123
+#: widgets/waveform/waveform_widget.py:3167
 msgid "Text"
 msgstr ""
 
 #: widgets/waveform/text_annotation.py:107
-#: widgets/waveform/waveform_widget.py:3348
+#: widgets/waveform/waveform_widget.py:3398
 msgid "Show text"
 msgstr ""
 
 #: widgets/waveform/text_annotation.py:116
-#: widgets/waveform/waveform_widget.py:3360
+#: widgets/waveform/waveform_widget.py:3410
 msgid "Shape"
 msgstr ""
 
 #: widgets/waveform/text_annotation.py:126
 msgid "Y Mode"
 msgstr ""
 
@@ -2648,317 +2654,317 @@
 #: widgets/waveform/waveform_source_widget.py:40
 msgid ""
 "\"default\" will use the default source which is normally configured using "
 "the Device Control widget."
 msgstr ""
 
 #: widgets/waveform/waveform_source_widget.py:104
-#: widgets/waveform/waveform_widget.py:402
-#: widgets/waveform/waveform_widget.py:479
+#: widgets/waveform/waveform_widget.py:401
+#: widgets/waveform/waveform_widget.py:478
 msgid "off"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:44
+#: widgets/waveform/waveform_widget.py:43
 msgid "Waveform"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:120
+#: widgets/waveform/waveform_widget.py:119
 msgid "General purpose input 0"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:121
+#: widgets/waveform/waveform_widget.py:120
 msgid "General purpose input 1"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:122
+#: widgets/waveform/waveform_widget.py:121
 msgid "General purpose input 2"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:123
+#: widgets/waveform/waveform_widget.py:122
 msgid "General purpose input 3"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:358
+#: widgets/waveform/waveform_widget.py:357
 msgid "The source filter string."
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:369
+#: widgets/waveform/waveform_widget.py:368
 msgid "The trace width."
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:384
+#: widgets/waveform/waveform_widget.py:383
 msgid "The target frames per second."
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:386
+#: widgets/waveform/waveform_widget.py:385
 msgid "vsync"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:387
+#: widgets/waveform/waveform_widget.py:386
 msgid "20 Hz"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:388
+#: widgets/waveform/waveform_widget.py:387
 msgid "10 Hz"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:389
+#: widgets/waveform/waveform_widget.py:388
 msgid "5 Hz"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:395
+#: widgets/waveform/waveform_widget.py:394
 msgid "The minimum interval between repaint in milliseconds."
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:400
+#: widgets/waveform/waveform_widget.py:399
 msgid "Show the minimum and maximum extents fill."
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:403
+#: widgets/waveform/waveform_widget.py:402
 msgid "lines"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:404
+#: widgets/waveform/waveform_widget.py:403
 msgid "fill 1"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:405
+#: widgets/waveform/waveform_widget.py:404
 msgid "fill 2"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:411
+#: widgets/waveform/waveform_widget.py:410
 msgid "Show the frames per second."
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:416
+#: widgets/waveform/waveform_widget.py:415
 msgid "Show the statistics on mouse hover."
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:421
+#: widgets/waveform/waveform_widget.py:420
 msgid "Show the plot statistics on the right."
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:426
+#: widgets/waveform/waveform_widget.py:425
 msgid "Show frequency for dual markers and statistics."
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:431
+#: widgets/waveform/waveform_widget.py:430
 msgid "The quantities to display by default."
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:437
+#: widgets/waveform/waveform_widget.py:436
 msgid "The precision to display in digits."
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:443
+#: widgets/waveform/waveform_widget.py:442
 msgid "Use OpenGL rendering."
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:454
+#: widgets/waveform/waveform_widget.py:453
 msgid "Pin the left side (oldest) data so that it stays in view."
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:459
+#: widgets/waveform/waveform_widget.py:458
 msgid "Pin the right side (newest) data so that it stays in view."
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:464
+#: widgets/waveform/waveform_widget.py:463
 msgid "The waveform state."
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:470
+#: widgets/waveform/waveform_widget.py:469
 msgid "The annotations."
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:476
+#: widgets/waveform/waveform_widget.py:475
 msgid "Control location"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:480
+#: widgets/waveform/waveform_widget.py:479
 msgid "top"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:481
+#: widgets/waveform/waveform_widget.py:480
 msgid "bottom"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:486
+#: widgets/waveform/waveform_widget.py:485
 msgid "The signal quantity to show in the summary."
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:492
+#: widgets/waveform/waveform_widget.py:491
 msgid "X-axis annotation mode"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:495
-#: widgets/waveform/waveform_widget.py:2888
+#: widgets/waveform/waveform_widget.py:494
+#: widgets/waveform/waveform_widget.py:2930
 msgid "Absolute"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:496
-#: widgets/waveform/waveform_widget.py:2893
+#: widgets/waveform/waveform_widget.py:495
+#: widgets/waveform/waveform_widget.py:2935
 msgid "Relative"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:502
+#: widgets/waveform/waveform_widget.py:501
 msgid "The available subsources."
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:508
+#: widgets/waveform/waveform_widget.py:507
 msgid "The selected subsources for each trace."
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:514
+#: widgets/waveform/waveform_widget.py:513
 msgid "The trace priority: highest int value on top, None is off."
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:2834
-#: widgets/waveform/waveform_widget.py:3135
+#: widgets/waveform/waveform_widget.py:2877
+#: widgets/waveform/waveform_widget.py:3179
 msgid "Save image to file"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:2882
-#: widgets/waveform/waveform_widget.py:2951
+#: widgets/waveform/waveform_widget.py:2924
+#: widgets/waveform/waveform_widget.py:2993
 msgid "Single marker"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:2883
-#: widgets/waveform/waveform_widget.py:2952
+#: widgets/waveform/waveform_widget.py:2925
+#: widgets/waveform/waveform_widget.py:2994
 msgid "Dual markers"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:2885
+#: widgets/waveform/waveform_widget.py:2927
 msgid "Mode"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:2898
-#: widgets/waveform/waveform_widget.py:2953
-#: widgets/waveform/waveform_widget.py:3111
-#: widgets/waveform/waveform_widget.py:3129
+#: widgets/waveform/waveform_widget.py:2940
+#: widgets/waveform/waveform_widget.py:2995
+#: widgets/waveform/waveform_widget.py:3155
+#: widgets/waveform/waveform_widget.py:3173
 msgid "Clear all"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:2909
-#: widgets/waveform/waveform_widget.py:2998
-#: widgets/waveform/waveform_widget.py:3117
+#: widgets/waveform/waveform_widget.py:2951
+#: widgets/waveform/waveform_widget.py:3040
+#: widgets/waveform/waveform_widget.py:3161
 msgid "Annotations"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3001
+#: widgets/waveform/waveform_widget.py:3043
 msgid "Range"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3005
-#: widgets/waveform/waveform_widget.py:3328
+#: widgets/waveform/waveform_widget.py:3047
+#: widgets/waveform/waveform_widget.py:3378
 msgid "Auto"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3011
+#: widgets/waveform/waveform_widget.py:3053
 msgid "Exact"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3020
+#: widgets/waveform/waveform_widget.py:3062
 msgid "Scale"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3023
+#: widgets/waveform/waveform_widget.py:3065
 msgid "Linear"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3028
+#: widgets/waveform/waveform_widget.py:3070
 msgid "Logarithmic"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3036
+#: widgets/waveform/waveform_widget.py:3078
 msgid "Logarithmic zero"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3050
+#: widgets/waveform/waveform_widget.py:3092
 msgid "Preferred prefix"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3108
+#: widgets/waveform/waveform_widget.py:3152
 msgid "Add"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3109
+#: widgets/waveform/waveform_widget.py:3153
 msgid "Hide all text"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3110
+#: widgets/waveform/waveform_widget.py:3154
 msgid "Show all text"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3118
+#: widgets/waveform/waveform_widget.py:3162
 msgid "Vertical"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3121
+#: widgets/waveform/waveform_widget.py:3165
 msgid "Horizontal"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3127
+#: widgets/waveform/waveform_widget.py:3171
 msgid "Save"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3132
+#: widgets/waveform/waveform_widget.py:3176
 msgid "Y-axis auto range"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3136
+#: widgets/waveform/waveform_widget.py:3180
 msgid "Copy image to clipboard"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3137
+#: widgets/waveform/waveform_widget.py:3181
 msgid "Export visible data"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3138
+#: widgets/waveform/waveform_widget.py:3182
 msgid "Export all data"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3304
+#: widgets/waveform/waveform_widget.py:3354
 msgid "Export"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3305
+#: widgets/waveform/waveform_widget.py:3355
 msgid "Analysis"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3313
+#: widgets/waveform/waveform_widget.py:3363
 msgid "Interval"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3322
+#: widgets/waveform/waveform_widget.py:3372
 msgid "Zoom"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3326
+#: widgets/waveform/waveform_widget.py:3376
 msgid "Show statistics"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3331
+#: widgets/waveform/waveform_widget.py:3381
 msgid "Left"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3334
+#: widgets/waveform/waveform_widget.py:3384
 msgid "Right"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3337
+#: widgets/waveform/waveform_widget.py:3387
 msgid "Off"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3340
-#: widgets/waveform/waveform_widget.py:3368
-#: widgets/waveform/waveform_widget.py:3397
+#: widgets/waveform/waveform_widget.py:3390
+#: widgets/waveform/waveform_widget.py:3418
+#: widgets/waveform/waveform_widget.py:3448
 msgid "Remove"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3351
+#: widgets/waveform/waveform_widget.py:3401
 msgid "Y mode"
 msgstr ""
 
 #: widgets/waveform/y_range_widget.py:67
 msgid "max"
 msgstr ""
```

### Comparing `joulescope_ui-1.1.6/joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.7/joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.2\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-18 14:15-0400\n"
+"POT-Creation-Date: 2024-05-06 17:27-0400\n"
 "PO-Revision-Date: 2024-04-04 14:45-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: ko\n"
 "Language-Team: ko <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.14.0\n"
+"Generated-By: Babel 2.15.0\n"
 
 msgid "\"3.3 V\" uses an internally-generated 3.3V reference voltage."
 msgstr "\"3.3V\"는 내부적으로 생성된 3.3V 기준 전압을 사용합니다."
 
 msgid "\"NaN\" sets all samples in the window to NaN."
 msgstr "\"NaN\"은 창에 있는 모든 샘플을 NaN으로 설정합니다."
 
@@ -620,14 +620,17 @@
 "퍼센트 단위로 표시됩니다."
 
 msgid ""
 "Display the number of actions processed by the publish-subscribe broker in "
 "each second."
 msgstr "게시-구독 브로커가 매초 처리하는 작업 수를 표시합니다."
 
+msgid "Divide the quantity by this value."
+msgstr "수량을 이 값으로 나눕니다."
+
 msgid "Do not show again"
 msgstr "다시 표시하지 않음"
 
 msgid "Do not use any USB hubs, docks or adapters"
 msgstr "USB 허브, 도크 또는 어댑터를 사용하지 마십시오."
 
 msgid "Dual markers"
@@ -1703,31 +1706,34 @@
 "selected)."
 msgstr ""
 "표시된 값은 일반적으로 장치에서 계산된 새로운 통계 데이터에 따라 업데이트됩니"
 "다. 이 버튼을 선택하면 디스플레이가 업데이트되지 않습니다. 그러나 통계는 계"
 "속 누적되어 누적됩니다(선택한 경우)."
 
 msgid ""
+"The divisor is a floating point number. The number may optionally be "
+"followed by units."
+msgstr ""
+"제수는 부동 소수점 숫자입니다. 숫자 뒤에 선택적으로 단위를 붙일 수 있습니다."
+
+msgid ""
 "The exponential decay time constant. The fuse dissipates 63.2 percent of "
 "accumulated energy in this duration."
 msgstr ""
 "지수 감쇠 시간 상수. 퓨즈는 이 기간 동안 누적된 에너지의 63.2%를 소산합니다."
 
 msgid "The filename supports the following replacements."
 msgstr "파일 이름은 다음과 같은 대체를 지원합니다."
 
 msgid "The filename with optional replacements."
 msgstr "선택적으로 대체할 수 있는 파일 이름입니다."
 
 msgid "The fixed default path for loading and saving files."
 msgstr "파일 로드 및 저장을 위한 고정된 기본 경로입니다."
 
-msgid "The flyout width in pixels."
-msgstr "픽셀 단위의 플라이아웃 너비입니다."
-
 msgid "The font scheme name."
 msgstr "글꼴 체계 이름입니다."
 
 msgid "The format string"
 msgstr "형식 문자열"
 
 msgid "The fuse trips in Duration at this constant current."
```

### Comparing `joulescope_ui-1.1.6/joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.7/joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.2\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-18 14:15-0400\n"
+"POT-Creation-Date: 2024-05-06 17:27-0400\n"
 "PO-Revision-Date: 2024-04-04 14:45-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: ko <LL@li.org>\n"
 "Language: ko\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"Generated-By: Babel 2.14.0\n"
+"Generated-By: Babel 2.15.0\n"
 
 #: about.py:24
 msgid "About the Joulescope UI"
 msgstr "줄스코프 UI 정보"
 
 #: about.py:25
 msgid "Version Information"
@@ -295,27 +295,27 @@
 msgid "Email"
 msgstr "이메일"
 
 #: error_window.py:103
 msgid "Description"
 msgstr "설명"
 
-#: error_window.py:112 widgets/waveform/waveform_widget.py:3347
+#: error_window.py:112 widgets/waveform/waveform_widget.py:3397
 msgid "Edit"
 msgstr "Edit"
 
 #: error_window.py:113
 msgid "View as Markdown"
 msgstr "마크다운으로 보기"
 
 #: error_window.py:119
 msgid "Abort"
 msgstr "Abort"
 
-#: error_window.py:120 main.py:365 widgets/settings/settings_widget.py:539
+#: error_window.py:120 main.py:363 widgets/settings/settings_widget.py:539
 msgid "View"
 msgstr "View"
 
 #: error_window.py:121
 msgid "Submit"
 msgstr "제출"
 
@@ -327,15 +327,15 @@
 msgid "Revert to previous configuration"
 msgstr "이전 구성으로 되돌리기"
 
 #: error_window.py:282
 msgid "Revert to defaults"
 msgstr "기본값으로 되돌리기"
 
-#: error_window.py:283 main.py:363 main.py:409
+#: error_window.py:283 main.py:361 main.py:407
 #: widgets/js220_cal/js220_cal_widget.py:38
 msgid "Exit"
 msgstr "Exit"
 
 #: exporter.py:49 widgets/signal_record/signal_record_config_widget.py:148
 #: widgets/statistics_record/statistics_record_config_widget.py:111
 msgid "Directory"
@@ -570,156 +570,156 @@
 msgid "Do not show again"
 msgstr "다시 표시하지 않음"
 
 #: intel_graphics_dialog.py:91
 msgid "Intel graphics detected"
 msgstr "인텔 그래픽 감지"
 
-#: main.py:70 widgets/value/value_widget.py:653
+#: main.py:69 widgets/value/value_widget.py:660
 msgid "Multimeter"
 msgstr "멀티미터"
 
-#: main.py:71
+#: main.py:70
 msgid "Oscilloscope"
 msgstr "오실로스코프"
 
-#: main.py:72 main.py:298 main.py:359 main.py:402
+#: main.py:71 main.py:296 main.py:357 main.py:400
 msgid "File"
 msgstr "파일"
 
-#: main.py:82
+#: main.py:81
 msgid "The UI status bar display mode"
 msgstr "UI 상태 표시줄 표시 모드"
 
-#: main.py:83
+#: main.py:82
 msgid ""
 "This setting controls the amount of detail shown on the status bar at the "
 "bottom of the UI window. You should usually leave this set to \"normal\" "
 "unless you want more detail concerning the UI internal operation."
 msgstr ""
 "이 설정은 UI 창 하단의 상태 표시줄에 표시되는 세부 정보의 양을 제어합니다. UI 내부 작동에 대한 자세한 정보를 원하지 않는 한 "
 "일반적으로 이 설정을 \"보통\"으로 두는 것이 좋습니다."
 
-#: main.py:88 safe_mode.py:43
+#: main.py:87 safe_mode.py:43
 msgid "Normal"
 msgstr "정상"
 
-#: main.py:89
+#: main.py:88
 msgid "Troubleshoot"
 msgstr "문제 해결"
 
-#: main.py:95
+#: main.py:94
 msgid "Enable developer mode."
 msgstr "개발자 모드를 활성화합니다."
 
-#: main.py:108
+#: main.py:107
 msgid "PubSub utilization"
 msgstr "PubSub 활용"
 
-#: main.py:109
+#: main.py:108
 msgid ""
 "Display the number of actions processed by the publish-subscribe broker in "
 "each second."
 msgstr "게시-구독 브로커가 매초 처리하는 작업 수를 표시합니다."
 
-#: main.py:114
+#: main.py:113
 msgid "CPU utilization"
 msgstr "CPU 사용률"
 
-#: main.py:115
+#: main.py:114
 msgid ""
 "Display the CPU utilization by this application and the total CPU "
 "utilization by all applications. The value is displayed in percent."
 msgstr "이 애플리케이션의 CPU 사용률과 모든 애플리케이션의 총 CPU 사용률을 표시합니다. 값은 퍼센트 단위로 표시됩니다."
 
-#: main.py:121
+#: main.py:120
 msgid "Memory utilization"
 msgstr "메모리 사용률"
 
-#: main.py:122
+#: main.py:121
 msgid ""
 "Display the memory (RAM) utilization by this application and by all "
 "applications. The value is displayed in percent."
 msgstr "이 애플리케이션 및 모든 애플리케이션의 메모리(RAM) 사용률을 표시합니다. 값은 퍼센트 단위로 표시됩니다."
 
-#: main.py:216
+#: main.py:214
 msgid "UI"
 msgstr "UI"
 
-#: main.py:330
+#: main.py:328
 msgid "Help"
 msgstr "도움말"
 
-#: main.py:331 widgets/hamburger/hamburger_widget.py:21
+#: main.py:329 widgets/hamburger/hamburger_widget.py:21
 msgid "Getting Started"
 msgstr "시작하기"
 
-#: main.py:332
+#: main.py:330
 msgid "User's Guide"
 msgstr "사용자 가이드"
 
-#: main.py:333 widgets/hamburger/hamburger_widget.py:22
+#: main.py:331 widgets/hamburger/hamburger_widget.py:22
 msgid "Changelog"
 msgstr "변경 로그"
 
-#: main.py:334 widgets/help/help_widget.py:59
+#: main.py:332 widgets/help/help_widget.py:59
 msgid "Report Issue"
 msgstr "이슈 보고"
 
-#: main.py:335
+#: main.py:333
 msgid "View logs..."
 msgstr "로그 보기..."
 
-#: main.py:336 widgets/hamburger/hamburger_widget.py:23
+#: main.py:334 widgets/hamburger/hamburger_widget.py:23
 msgid "Credits"
 msgstr "크레딧"
 
-#: main.py:337 widgets/hamburger/hamburger_widget.py:24
+#: main.py:335 widgets/hamburger/hamburger_widget.py:24
 msgid "About"
 msgstr "About"
 
-#: main.py:360
+#: main.py:358
 msgid "Open"
 msgstr "Open"
 
-#: main.py:361
+#: main.py:359
 msgid "Open recent"
 msgstr "최근 열기"
 
-#: main.py:362 main.py:408
+#: main.py:360 main.py:406
 msgid "Clear config and exit"
 msgstr "구성 지우기 및 종료"
 
-#: main.py:366 widgets/settings/settings_widget.py:541
+#: main.py:364 widgets/settings/settings_widget.py:541
 msgid "Widgets"
 msgstr "위젯"
 
-#: main.py:367
+#: main.py:365
 msgid "Tools"
 msgstr "도구"
 
-#: main.py:368
+#: main.py:366
 msgid "Clear Accumulators"
 msgstr "클리어 어큐뮬레이터"
 
-#: main.py:403
+#: main.py:401
 msgid "Info"
 msgstr "정보"
 
-#: main.py:404 widget_tools.py:92 widgets/settings/settings_widget.py:31
+#: main.py:402 widget_tools.py:92 widgets/settings/settings_widget.py:31
 #: widgets/settings/settings_widget.py:574
 #: widgets/sidebar/sidebar_widget.py:41
 msgid "Settings"
 msgstr "설정"
 
-#: main.py:693
+#: main.py:710
 msgid "Manage"
 msgstr "관리"
 
-#: main.py:730
+#: main.py:747
 msgid "Select file to open"
 msgstr "열 파일 선택"
 
 #: paths.py:30 styles/manager.py:46
 msgid "The name for this widget."
 msgstr "이 위젯의 이름입니다."
 
@@ -858,47 +858,47 @@
 msgid "Source"
 msgstr "Source"
 
 #: units.py:35
 msgid "Use the application defaults"
 msgstr "애플리케이션 기본값 사용"
 
-#: view.py:68
+#: view.py:72
 msgid "The active theme."
 msgstr "활성 테마."
 
-#: view.py:70
+#: view.py:74
 msgid "Joulescope standard theme"
 msgstr "줄스코프 표준 테마"
 
-#: view.py:70
+#: view.py:74
 msgid "System OS-specific theme"
 msgstr "시스템 OS별 테마"
 
-#: view.py:75
+#: view.py:79
 msgid "The color scheme name."
 msgstr "색 구성표 이름입니다."
 
-#: view.py:77
+#: view.py:81
 msgid "Dark background"
 msgstr "어두운 배경"
 
-#: view.py:77
+#: view.py:81
 msgid "Light background"
 msgstr "조명 배경"
 
-#: view.py:81
+#: view.py:85
 msgid "The font scheme name."
 msgstr "글꼴 체계 이름입니다."
 
-#: view.py:83
+#: view.py:87
 msgid "Joulescope standard font theme"
 msgstr "줄스코프 표준 글꼴 테마"
 
-#: view.py:102 widgets/view_manager/view_manager_widget.py:146
+#: view.py:106 widgets/view_manager/view_manager_widget.py:146
 msgid "New View"
 msgstr "새로운 보기"
 
 #: zip_inspector.py:23
 msgid "ZIP Inspector"
 msgstr "ZIP 인스펙터"
 
@@ -1004,15 +1004,15 @@
 "this inhibits target power, which can be used to power cycle reset the "
 "target device."
 msgstr ""
 "활성화되면 전류 단자 간에 전류가 흐릅니다. 비활성화하면 전류 단자 사이에 전류가 흐르지 않습니다. 일반적인 시스템 설정에서 이 기능은 "
 "목표 전력을 억제하여 목표 장치의 전원 사이클을 리셋하는 데 사용할 수 있습니다."
 
 #: devices/jsdrv/js110.py:147 devices/jsdrv/js220.py:163
-#: widgets/waveform/waveform_widget.py:110
+#: widgets/waveform/waveform_widget.py:109
 msgid "Current range"
 msgstr "전류 범위"
 
 #: devices/jsdrv/js110.py:149
 msgid ""
 "Configure the J110's current range. Most applications should use the "
 "default, \"auto\"."
@@ -1139,33 +1139,33 @@
 #: devices/jsdrv/js110.py:255
 msgid ""
 "The number of samples after the current range window used to determine the "
 "mean. This value is ignored for all other IRF types."
 msgstr "평균을 결정하는 데 사용되는 전류 범위 창 이후의 샘플 수입니다. 다른 모든 IRF 유형에서는 이 값이 무시됩니다."
 
 #: devices/jsdrv/js110.py:269 devices/jsdrv/js220.py:332
-#: widgets/device_control/fuse.py:103 widgets/waveform/waveform_widget.py:105
+#: widgets/device_control/fuse.py:103 widgets/waveform/waveform_widget.py:104
 msgid "Current"
 msgstr "전류"
 
 #: devices/jsdrv/js110.py:270 devices/jsdrv/js220.py:333
 msgid "Enable the current signal streaming."
 msgstr "전류 신호 스트리밍을 활성화합니다."
 
 #: devices/jsdrv/js110.py:278 devices/jsdrv/js220.py:341
-#: widgets/waveform/waveform_widget.py:106
+#: widgets/waveform/waveform_widget.py:105
 msgid "Voltage"
 msgstr "전압"
 
 #: devices/jsdrv/js110.py:279 devices/jsdrv/js220.py:342
 msgid "Enable the voltage signal streaming."
 msgstr "전압 신호 스트리밍을 활성화합니다."
 
 #: devices/jsdrv/js110.py:287 devices/jsdrv/js220.py:350
-#: widgets/waveform/waveform_widget.py:107
+#: widgets/waveform/waveform_widget.py:106
 msgid "Power"
 msgstr "Power"
 
 #: devices/jsdrv/js110.py:288 devices/jsdrv/js220.py:351
 msgid "Enable the power signal streaming."
 msgstr "전원 신호 스트리밍을 활성화합니다."
 
@@ -1354,15 +1354,15 @@
 msgid "GPI 3"
 msgstr "GPI 3"
 
 #: devices/jsdrv/js220.py:402
 msgid "Enable the general purpose input 3 signal streaming."
 msgstr "범용 입력 3 신호 스트리밍을 활성화합니다."
 
-#: devices/jsdrv/js220.py:410 widgets/waveform/waveform_widget.py:124
+#: devices/jsdrv/js220.py:410 widgets/waveform/waveform_widget.py:123
 msgid "Trigger input"
 msgstr "트리거 입력"
 
 #: devices/jsdrv/js220.py:411
 msgid "Enable the trigger input signal streaming."
 msgstr "트리거 입력 신호 스트리밍을 활성화합니다."
 
@@ -1373,15 +1373,15 @@
 #: devices/jsdrv/jsdrv_stream_buffer.py:44
 #: devices/jsdrv/jsdrv_stream_buffer.py:93
 #: devices/jsdrv/jsdrv_stream_buffer.py:107 plugins/selector.py:58
 #: widgets/settings/settings_widget.py:85
 #: widgets/settings/settings_widget.py:266
 #: widgets/settings/settings_widget.py:364
 #: widgets/settings/settings_widget.py:431
-#: widgets/waveform/waveform_widget.py:3062
+#: widgets/waveform/waveform_widget.py:3104
 msgid "Name"
 msgstr "이름"
 
 #: devices/jsdrv/jsdrv_stream_buffer.py:45
 msgid "Joulescope stream buffer"
 msgstr "줄스코프 스트림 버퍼"
 
@@ -1591,15 +1591,15 @@
 
 #: widgets/accumulator/accumulator_widget.py:27
 #: widgets/value/value_widget.py:31
 msgid "The statistics data stream source."
 msgstr "통계 데이터 스트림 소스."
 
 #: widgets/accumulator/accumulator_widget.py:32
-#: widgets/value/value_widget.py:74
+#: widgets/value/value_widget.py:81
 msgid "The signal to display."
 msgstr "표시할 신호."
 
 #: widgets/accumulator/accumulator_widget.py:34
 msgid "charge"
 msgstr "charge"
 
@@ -1682,15 +1682,15 @@
 
 #: widgets/developer/publish_spy_widget.py:20
 #: widgets/developer/publish_spy_widget.py:21
 msgid "Topic"
 msgstr "주제"
 
 #: widgets/developer/publish_spy_widget.py:21
-#: widgets/settings/settings_widget.py:87 widgets/value/value_widget.py:662
+#: widgets/settings/settings_widget.py:87 widgets/value/value_widget.py:669
 msgid "Value"
 msgstr "Value"
 
 #: widgets/developer/publish_spy_widget.py:24
 msgid "Publish Spy"
 msgstr "스파이 게시"
 
@@ -1720,15 +1720,15 @@
 
 #: widgets/device_control/device_update_dialog.py:24
 #: widgets/device_control/device_update_dialog.py:45
 msgid "Update"
 msgstr "업데이트"
 
 #: widgets/device_control/device_update_dialog.py:25
-#: widgets/value/value_widget.py:147
+#: widgets/value/value_widget.py:155
 msgid "Device"
 msgstr "디바이스"
 
 #: widgets/device_control/device_update_dialog.py:27
 #: widgets/progress_bar/progress_bar_widget.py:59
 msgid "Progress"
 msgstr "진행"
@@ -2217,18 +2217,14 @@
 msgid "Click to display additional settings and actions."
 msgstr "추가 설정 및 작업을 표시하려면 클릭하세요."
 
 #: widgets/sidebar/sidebar_widget.py:60
 msgid "sidebar"
 msgstr "사이드바"
 
-#: widgets/sidebar/sidebar_widget.py:68
-msgid "The flyout width in pixels."
-msgstr "픽셀 단위의 플라이아웃 너비입니다."
-
 #: widgets/signal_record/disk_full_dialog.py:19
 msgid "The disk is full"
 msgstr "디스크가 꽉 찼습니다."
 
 #: widgets/signal_record/signal_record.py:57
 msgid "Could not open file for write"
 msgstr "쓰기 위해 파일을 열 수 없습니다."
@@ -2255,15 +2251,15 @@
 msgid "StatisticsRecordConfig"
 msgstr "StatisticsRecordConfig"
 
 #: widgets/statistics_record/statistics_record_config_widget.py:123
 msgid "Time Format"
 msgstr "시간 형식"
 
-#: widgets/trigger/trigger_widget.py:41 widgets/value/value_widget.py:87
+#: widgets/trigger/trigger_widget.py:41 widgets/value/value_widget.py:94
 msgid "Select the source device"
 msgstr "소스 디바이스 선택"
 
 #: widgets/trigger/trigger_widget.py:42
 msgid "The device to use for the start condition and stop condition."
 msgstr "시작 조건 및 중지 조건에 사용할 장치입니다."
 
@@ -2429,74 +2425,84 @@
 msgid "Show the statistics fields at the right."
 msgstr "오른쪽에 통계 필드가 표시됩니다."
 
 #: widgets/value/value_widget.py:51
 msgid "Show a leading + or - sign."
 msgstr "선행 + 또는 - 기호를 표시합니다."
 
-#: widgets/value/value_widget.py:88
+#: widgets/value/value_widget.py:62
+msgid "Divide the quantity by this value."
+msgstr "수량을 이 값으로 나눕니다."
+
+#: widgets/value/value_widget.py:63
+msgid ""
+"The divisor is a floating point number. The number may optionally be "
+"followed by units."
+msgstr "제수는 부동 소수점 숫자입니다. 숫자 뒤에 선택적으로 단위를 붙일 수 있습니다."
+
+#: widgets/value/value_widget.py:95
 msgid ""
 "The values displayed by this widget come from a single source device. Select"
 " the source device here."
 msgstr "이 위젯에 표시되는 값은 단일 소스 장치에서 가져온 것입니다. 여기에서 소스 장치를 선택하세요."
 
-#: widgets/value/value_widget.py:94
+#: widgets/value/value_widget.py:101
 msgid "Hold the display"
 msgstr "디스플레이 잡기"
 
-#: widgets/value/value_widget.py:96
+#: widgets/value/value_widget.py:103
 msgid "When selected, prevent the display from updating."
 msgstr "이 옵션을 선택하면 디스플레이가 업데이트되지 않습니다."
 
-#: widgets/value/value_widget.py:97
+#: widgets/value/value_widget.py:104
 msgid ""
 "The UI also includes a global statistics hold button on the sidebar. When "
 "the global statistics hold button is selected, this button is disabled and "
 "has no effect."
 msgstr ""
 "UI에는 사이드바에 글로벌 통계 보류 버튼도 있습니다. 글로벌 통계 보류 버튼을 선택하면 이 버튼은 비활성화되며 아무런 효과가 없습니다."
 
-#: widgets/value/value_widget.py:100
+#: widgets/value/value_widget.py:107
 msgid ""
 "The displayed values normally update with each new statistics data computed "
 "by the device. When this button is selected, the display will not be "
 "updated. However, the statistics will continue accumulate and accrue (if "
 "selected)."
 msgstr ""
 "표시된 값은 일반적으로 장치에서 계산된 새로운 통계 데이터에 따라 업데이트됩니다. 이 버튼을 선택하면 디스플레이가 업데이트되지 않습니다."
 " 그러나 통계는 계속 누적되어 누적됩니다(선택한 경우)."
 
-#: widgets/value/value_widget.py:107
+#: widgets/value/value_widget.py:114
 msgid "Accrue values over time"
 msgstr "시간에 따른 값 누적"
 
-#: widgets/value/value_widget.py:109
+#: widgets/value/value_widget.py:116
 msgid ""
 "Current, voltage, and power are normally computed over a single statistics "
 "frequency interval. Press this button to accrue the values indefinitely. "
 "Press again to return to normal operation."
 msgstr ""
 "전류, 전압 및 전력은 일반적으로 단일 통계 주파수 간격에 걸쳐 계산됩니다. 이 버튼을 누르면 값이 무한정 누적됩니다. 다시 누르면 정상"
 " 작동으로 돌아갑니다."
 
-#: widgets/value/value_widget.py:113
+#: widgets/value/value_widget.py:120
 msgid ""
 "Note that this button does not affect the charge and energy accumulation. "
 "Both accumulate indefinitely regardless of this button state."
 msgstr "이 버튼은 충전 및 에너지 축적에 영향을 주지 않습니다. 둘 다 이 버튼 상태에 관계없이 무기한으로 누적됩니다."
 
-#: widgets/value/value_widget.py:195
+#: widgets/value/value_widget.py:203
 msgid "Not present"
 msgstr "현재 없음"
 
-#: widgets/value/value_widget.py:215
+#: widgets/value/value_widget.py:223
 msgid "Hold"
 msgstr "Hold"
 
-#: widgets/value/value_widget.py:223
+#: widgets/value/value_widget.py:231
 msgid "Accrue"
 msgstr "증가"
 
 #: widgets/view_manager/view_manager_widget.py:108
 #: widgets/view_manager/view_manager_widget.py:174
 msgid "View Manager"
 msgstr "뷰 관리자"
@@ -2542,34 +2548,34 @@
 msgstr "삼각형 오른쪽"
 
 #: widgets/waveform/text_annotation.py:62
 msgid "triangle left"
 msgstr "왼쪽 삼각형"
 
 #: widgets/waveform/text_annotation.py:66
-#: widgets/waveform/waveform_widget.py:3008
+#: widgets/waveform/waveform_widget.py:3050
 msgid "Manual"
 msgstr "매뉴얼"
 
 #: widgets/waveform/text_annotation.py:67
 msgid "Centered"
 msgstr "중심"
 
 #: widgets/waveform/text_annotation.py:99
-#: widgets/waveform/waveform_widget.py:3123
+#: widgets/waveform/waveform_widget.py:3167
 msgid "Text"
 msgstr "텍스트"
 
 #: widgets/waveform/text_annotation.py:107
-#: widgets/waveform/waveform_widget.py:3348
+#: widgets/waveform/waveform_widget.py:3398
 msgid "Show text"
 msgstr "텍스트 표시"
 
 #: widgets/waveform/text_annotation.py:116
-#: widgets/waveform/waveform_widget.py:3360
+#: widgets/waveform/waveform_widget.py:3410
 msgid "Shape"
 msgstr "모양"
 
 #: widgets/waveform/text_annotation.py:126
 msgid "Y Mode"
 msgstr "Y 모드"
 
@@ -2738,317 +2744,317 @@
 #: widgets/waveform/waveform_source_widget.py:40
 msgid ""
 "\"default\" will use the default source which is normally configured using "
 "the Device Control widget."
 msgstr "\"기본\"은 일반적으로 장치 제어 위젯을 사용하여 구성되는 기본 소스를 사용합니다."
 
 #: widgets/waveform/waveform_source_widget.py:104
-#: widgets/waveform/waveform_widget.py:402
-#: widgets/waveform/waveform_widget.py:479
+#: widgets/waveform/waveform_widget.py:401
+#: widgets/waveform/waveform_widget.py:478
 msgid "off"
 msgstr "off"
 
-#: widgets/waveform/waveform_widget.py:44
+#: widgets/waveform/waveform_widget.py:43
 msgid "Waveform"
 msgstr "파형"
 
-#: widgets/waveform/waveform_widget.py:120
+#: widgets/waveform/waveform_widget.py:119
 msgid "General purpose input 0"
 msgstr "범용 입력 0"
 
-#: widgets/waveform/waveform_widget.py:121
+#: widgets/waveform/waveform_widget.py:120
 msgid "General purpose input 1"
 msgstr "범용 입력 1"
 
-#: widgets/waveform/waveform_widget.py:122
+#: widgets/waveform/waveform_widget.py:121
 msgid "General purpose input 2"
 msgstr "범용 입력 2"
 
-#: widgets/waveform/waveform_widget.py:123
+#: widgets/waveform/waveform_widget.py:122
 msgid "General purpose input 3"
 msgstr "범용 입력 3"
 
-#: widgets/waveform/waveform_widget.py:358
+#: widgets/waveform/waveform_widget.py:357
 msgid "The source filter string."
 msgstr "소스 필터 문자열입니다."
 
-#: widgets/waveform/waveform_widget.py:369
+#: widgets/waveform/waveform_widget.py:368
 msgid "The trace width."
 msgstr "트레이스 폭."
 
-#: widgets/waveform/waveform_widget.py:384
+#: widgets/waveform/waveform_widget.py:383
 msgid "The target frames per second."
 msgstr "초당 목표 프레임."
 
-#: widgets/waveform/waveform_widget.py:386
+#: widgets/waveform/waveform_widget.py:385
 msgid "vsync"
 msgstr "vsync"
 
-#: widgets/waveform/waveform_widget.py:387
+#: widgets/waveform/waveform_widget.py:386
 msgid "20 Hz"
 msgstr "20 Hz"
 
-#: widgets/waveform/waveform_widget.py:388
+#: widgets/waveform/waveform_widget.py:387
 msgid "10 Hz"
 msgstr "10 Hz"
 
-#: widgets/waveform/waveform_widget.py:389
+#: widgets/waveform/waveform_widget.py:388
 msgid "5 Hz"
 msgstr "5 Hz"
 
-#: widgets/waveform/waveform_widget.py:395
+#: widgets/waveform/waveform_widget.py:394
 msgid "The minimum interval between repaint in milliseconds."
 msgstr "밀리초 단위의 최소 재도장 간격입니다."
 
-#: widgets/waveform/waveform_widget.py:400
+#: widgets/waveform/waveform_widget.py:399
 msgid "Show the minimum and maximum extents fill."
 msgstr "최소 및 최대 범위 채우기를 표시합니다."
 
-#: widgets/waveform/waveform_widget.py:403
+#: widgets/waveform/waveform_widget.py:402
 msgid "lines"
 msgstr "lines"
 
-#: widgets/waveform/waveform_widget.py:404
+#: widgets/waveform/waveform_widget.py:403
 msgid "fill 1"
 msgstr "채우기 1"
 
-#: widgets/waveform/waveform_widget.py:405
+#: widgets/waveform/waveform_widget.py:404
 msgid "fill 2"
 msgstr "채우기 2"
 
-#: widgets/waveform/waveform_widget.py:411
+#: widgets/waveform/waveform_widget.py:410
 msgid "Show the frames per second."
 msgstr "초당 프레임을 표시합니다."
 
-#: widgets/waveform/waveform_widget.py:416
+#: widgets/waveform/waveform_widget.py:415
 msgid "Show the statistics on mouse hover."
 msgstr "마우스 호버에 대한 통계를 표시합니다."
 
-#: widgets/waveform/waveform_widget.py:421
+#: widgets/waveform/waveform_widget.py:420
 msgid "Show the plot statistics on the right."
 msgstr "오른쪽에 플롯 통계가 표시됩니다."
 
-#: widgets/waveform/waveform_widget.py:426
+#: widgets/waveform/waveform_widget.py:425
 msgid "Show frequency for dual markers and statistics."
 msgstr "듀얼 마커 및 통계에 대한 주파수를 표시합니다."
 
-#: widgets/waveform/waveform_widget.py:431
+#: widgets/waveform/waveform_widget.py:430
 msgid "The quantities to display by default."
 msgstr "기본적으로 표시되는 수량입니다."
 
-#: widgets/waveform/waveform_widget.py:437
+#: widgets/waveform/waveform_widget.py:436
 msgid "The precision to display in digits."
 msgstr "숫자로 표시되는 정밀도."
 
-#: widgets/waveform/waveform_widget.py:443
+#: widgets/waveform/waveform_widget.py:442
 msgid "Use OpenGL rendering."
 msgstr "OpenGL 렌더링을 사용합니다."
 
-#: widgets/waveform/waveform_widget.py:454
+#: widgets/waveform/waveform_widget.py:453
 msgid "Pin the left side (oldest) data so that it stays in view."
 msgstr "왼쪽(가장 오래된) 데이터를 고정하여 계속 볼 수 있도록 합니다."
 
-#: widgets/waveform/waveform_widget.py:459
+#: widgets/waveform/waveform_widget.py:458
 msgid "Pin the right side (newest) data so that it stays in view."
 msgstr "오른쪽(최신) 데이터를 고정하여 계속 볼 수 있도록 합니다."
 
-#: widgets/waveform/waveform_widget.py:464
+#: widgets/waveform/waveform_widget.py:463
 msgid "The waveform state."
 msgstr "파형 상태."
 
-#: widgets/waveform/waveform_widget.py:470
+#: widgets/waveform/waveform_widget.py:469
 msgid "The annotations."
 msgstr "주석."
 
-#: widgets/waveform/waveform_widget.py:476
+#: widgets/waveform/waveform_widget.py:475
 msgid "Control location"
 msgstr "제어 위치"
 
-#: widgets/waveform/waveform_widget.py:480
+#: widgets/waveform/waveform_widget.py:479
 msgid "top"
 msgstr "top"
 
-#: widgets/waveform/waveform_widget.py:481
+#: widgets/waveform/waveform_widget.py:480
 msgid "bottom"
 msgstr "bottom"
 
-#: widgets/waveform/waveform_widget.py:486
+#: widgets/waveform/waveform_widget.py:485
 msgid "The signal quantity to show in the summary."
 msgstr "요약에 표시할 신호 양입니다."
 
-#: widgets/waveform/waveform_widget.py:492
+#: widgets/waveform/waveform_widget.py:491
 msgid "X-axis annotation mode"
 msgstr "X축 주석 모드"
 
-#: widgets/waveform/waveform_widget.py:495
-#: widgets/waveform/waveform_widget.py:2888
+#: widgets/waveform/waveform_widget.py:494
+#: widgets/waveform/waveform_widget.py:2930
 msgid "Absolute"
 msgstr "절대"
 
-#: widgets/waveform/waveform_widget.py:496
-#: widgets/waveform/waveform_widget.py:2893
+#: widgets/waveform/waveform_widget.py:495
+#: widgets/waveform/waveform_widget.py:2935
 msgid "Relative"
 msgstr "상대"
 
-#: widgets/waveform/waveform_widget.py:502
+#: widgets/waveform/waveform_widget.py:501
 msgid "The available subsources."
 msgstr "사용 가능한 하위 소스."
 
-#: widgets/waveform/waveform_widget.py:508
+#: widgets/waveform/waveform_widget.py:507
 msgid "The selected subsources for each trace."
 msgstr "각 트레이스에 대해 선택된 하위 소스."
 
-#: widgets/waveform/waveform_widget.py:514
+#: widgets/waveform/waveform_widget.py:513
 msgid "The trace priority: highest int value on top, None is off."
 msgstr "트레이스 우선순위: 가장 높은 int 값이 위에 있고 없음은 꺼져 있습니다."
 
-#: widgets/waveform/waveform_widget.py:2834
-#: widgets/waveform/waveform_widget.py:3135
+#: widgets/waveform/waveform_widget.py:2877
+#: widgets/waveform/waveform_widget.py:3179
 msgid "Save image to file"
 msgstr "파일에 이미지 저장"
 
-#: widgets/waveform/waveform_widget.py:2882
-#: widgets/waveform/waveform_widget.py:2951
+#: widgets/waveform/waveform_widget.py:2924
+#: widgets/waveform/waveform_widget.py:2993
 msgid "Single marker"
 msgstr "단일 마커"
 
-#: widgets/waveform/waveform_widget.py:2883
-#: widgets/waveform/waveform_widget.py:2952
+#: widgets/waveform/waveform_widget.py:2925
+#: widgets/waveform/waveform_widget.py:2994
 msgid "Dual markers"
 msgstr "듀얼 마커"
 
-#: widgets/waveform/waveform_widget.py:2885
+#: widgets/waveform/waveform_widget.py:2927
 msgid "Mode"
 msgstr "모드"
 
-#: widgets/waveform/waveform_widget.py:2898
-#: widgets/waveform/waveform_widget.py:2953
-#: widgets/waveform/waveform_widget.py:3111
-#: widgets/waveform/waveform_widget.py:3129
+#: widgets/waveform/waveform_widget.py:2940
+#: widgets/waveform/waveform_widget.py:2995
+#: widgets/waveform/waveform_widget.py:3155
+#: widgets/waveform/waveform_widget.py:3173
 msgid "Clear all"
 msgstr "모두 지우기"
 
-#: widgets/waveform/waveform_widget.py:2909
-#: widgets/waveform/waveform_widget.py:2998
-#: widgets/waveform/waveform_widget.py:3117
+#: widgets/waveform/waveform_widget.py:2951
+#: widgets/waveform/waveform_widget.py:3040
+#: widgets/waveform/waveform_widget.py:3161
 msgid "Annotations"
 msgstr "주석"
 
-#: widgets/waveform/waveform_widget.py:3001
+#: widgets/waveform/waveform_widget.py:3043
 msgid "Range"
 msgstr "범위"
 
-#: widgets/waveform/waveform_widget.py:3005
-#: widgets/waveform/waveform_widget.py:3328
+#: widgets/waveform/waveform_widget.py:3047
+#: widgets/waveform/waveform_widget.py:3378
 msgid "Auto"
 msgstr "Auto"
 
-#: widgets/waveform/waveform_widget.py:3011
+#: widgets/waveform/waveform_widget.py:3053
 msgid "Exact"
 msgstr "정확한"
 
-#: widgets/waveform/waveform_widget.py:3020
+#: widgets/waveform/waveform_widget.py:3062
 msgid "Scale"
 msgstr "스케일"
 
-#: widgets/waveform/waveform_widget.py:3023
+#: widgets/waveform/waveform_widget.py:3065
 msgid "Linear"
 msgstr "선형"
 
-#: widgets/waveform/waveform_widget.py:3028
+#: widgets/waveform/waveform_widget.py:3070
 msgid "Logarithmic"
 msgstr "로그"
 
-#: widgets/waveform/waveform_widget.py:3036
+#: widgets/waveform/waveform_widget.py:3078
 msgid "Logarithmic zero"
 msgstr "로그 제로"
 
-#: widgets/waveform/waveform_widget.py:3050
+#: widgets/waveform/waveform_widget.py:3092
 msgid "Preferred prefix"
 msgstr "기본 접두사"
 
-#: widgets/waveform/waveform_widget.py:3108
+#: widgets/waveform/waveform_widget.py:3152
 msgid "Add"
 msgstr "추가"
 
-#: widgets/waveform/waveform_widget.py:3109
+#: widgets/waveform/waveform_widget.py:3153
 msgid "Hide all text"
 msgstr "모든 텍스트 숨기기"
 
-#: widgets/waveform/waveform_widget.py:3110
+#: widgets/waveform/waveform_widget.py:3154
 msgid "Show all text"
 msgstr "모든 텍스트 표시"
 
-#: widgets/waveform/waveform_widget.py:3118
+#: widgets/waveform/waveform_widget.py:3162
 msgid "Vertical"
 msgstr "수직"
 
-#: widgets/waveform/waveform_widget.py:3121
+#: widgets/waveform/waveform_widget.py:3165
 msgid "Horizontal"
 msgstr "수평"
 
-#: widgets/waveform/waveform_widget.py:3127
+#: widgets/waveform/waveform_widget.py:3171
 msgid "Save"
 msgstr "저장"
 
-#: widgets/waveform/waveform_widget.py:3132
+#: widgets/waveform/waveform_widget.py:3176
 msgid "Y-axis auto range"
 msgstr "Y축 자동 범위"
 
-#: widgets/waveform/waveform_widget.py:3136
+#: widgets/waveform/waveform_widget.py:3180
 msgid "Copy image to clipboard"
 msgstr "이미지를 클립보드에 복사"
 
-#: widgets/waveform/waveform_widget.py:3137
+#: widgets/waveform/waveform_widget.py:3181
 msgid "Export visible data"
 msgstr "가시 데이터 내보내기"
 
-#: widgets/waveform/waveform_widget.py:3138
+#: widgets/waveform/waveform_widget.py:3182
 msgid "Export all data"
 msgstr "모든 데이터 내보내기"
 
-#: widgets/waveform/waveform_widget.py:3304
+#: widgets/waveform/waveform_widget.py:3354
 msgid "Export"
 msgstr "Export"
 
-#: widgets/waveform/waveform_widget.py:3305
+#: widgets/waveform/waveform_widget.py:3355
 msgid "Analysis"
 msgstr "분석"
 
-#: widgets/waveform/waveform_widget.py:3313
+#: widgets/waveform/waveform_widget.py:3363
 msgid "Interval"
 msgstr "Interval"
 
-#: widgets/waveform/waveform_widget.py:3322
+#: widgets/waveform/waveform_widget.py:3372
 msgid "Zoom"
 msgstr "줌"
 
-#: widgets/waveform/waveform_widget.py:3326
+#: widgets/waveform/waveform_widget.py:3376
 msgid "Show statistics"
 msgstr "통계 보기"
 
-#: widgets/waveform/waveform_widget.py:3331
+#: widgets/waveform/waveform_widget.py:3381
 msgid "Left"
 msgstr "왼쪽"
 
-#: widgets/waveform/waveform_widget.py:3334
+#: widgets/waveform/waveform_widget.py:3384
 msgid "Right"
 msgstr "Right"
 
-#: widgets/waveform/waveform_widget.py:3337
+#: widgets/waveform/waveform_widget.py:3387
 msgid "Off"
 msgstr "Off"
 
-#: widgets/waveform/waveform_widget.py:3340
-#: widgets/waveform/waveform_widget.py:3368
-#: widgets/waveform/waveform_widget.py:3397
+#: widgets/waveform/waveform_widget.py:3390
+#: widgets/waveform/waveform_widget.py:3418
+#: widgets/waveform/waveform_widget.py:3448
 msgid "Remove"
 msgstr "제거"
 
-#: widgets/waveform/waveform_widget.py:3351
+#: widgets/waveform/waveform_widget.py:3401
 msgid "Y mode"
 msgstr "Y 모드"
 
 #: widgets/waveform/y_range_widget.py:67
 msgid "max"
 msgstr "최대"
```

### Comparing `joulescope_ui-1.1.6/joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.7/joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.2\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-18 14:15-0400\n"
+"POT-Creation-Date: 2024-05-06 17:27-0400\n"
 "PO-Revision-Date: 2024-04-04 14:45-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: zh\n"
 "Language-Team: zh <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.14.0\n"
+"Generated-By: Babel 2.15.0\n"
 
 msgid "\"3.3 V\" uses an internally-generated 3.3V reference voltage."
 msgstr "\"3.3 V \"使用内部生成的 3.3 V 基准电压。"
 
 msgid "\"NaN\" sets all samples in the window to NaN."
 msgstr "\"NaN \"将窗口中的所有样本设置为 NaN。"
 
@@ -587,14 +587,17 @@
 msgstr "显示此应用程序和所有应用程序的内存（RAM）利用率。该值以百分比显示。"
 
 msgid ""
 "Display the number of actions processed by the publish-subscribe broker in "
 "each second."
 msgstr "显示发布-订阅代理每秒处理的操作数。"
 
+msgid "Divide the quantity by this value."
+msgstr "用这个值除以数量。"
+
 msgid "Do not show again"
 msgstr "不再显示"
 
 msgid "Do not use any USB hubs, docks or adapters"
 msgstr "请勿使用任何 USB 集线器、基座或适配器"
 
 msgid "Dual markers"
@@ -1641,30 +1644,32 @@
 "updated. However, the statistics will continue accumulate and accrue (if "
 "selected)."
 msgstr ""
 "显示值通常随设备计算的每个新统计数据更新。选择此按钮后，显示值将不会更新。但"
 "是，统计数据将继续累积（如果选择）。"
 
 msgid ""
+"The divisor is a floating point number. The number may optionally be "
+"followed by units."
+msgstr "除数是浮点数。数字后面可以选择单位。"
+
+msgid ""
 "The exponential decay time constant. The fuse dissipates 63.2 percent of "
 "accumulated energy in this duration."
 msgstr "指数衰减时间常数。保险丝在此时间内耗散了 63.2% 的累积能量。"
 
 msgid "The filename supports the following replacements."
 msgstr "文件名支持以下替换。"
 
 msgid "The filename with optional replacements."
 msgstr "可选替换的文件名。"
 
 msgid "The fixed default path for loading and saving files."
 msgstr "加载和保存文件的固定默认路径。"
 
-msgid "The flyout width in pixels."
-msgstr "飞出宽度（像素）。"
-
 msgid "The font scheme name."
 msgstr "字体方案名称。"
 
 msgid "The format string"
 msgstr "格式字符串"
 
 msgid "The fuse trips in Duration at this constant current."
```

### Comparing `joulescope_ui-1.1.6/joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.7/joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT 1.1.2\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-18 14:15-0400\n"
+"POT-Creation-Date: 2024-05-06 17:27-0400\n"
 "PO-Revision-Date: 2024-04-04 14:45-0400\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: zh <LL@li.org>\n"
 "Language: zh\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"Generated-By: Babel 2.14.0\n"
+"Generated-By: Babel 2.15.0\n"
 
 #: about.py:24
 msgid "About the Joulescope UI"
 msgstr "关于 Joulescope UI"
 
 #: about.py:25
 msgid "Version Information"
@@ -287,27 +287,27 @@
 msgid "Email"
 msgstr "电子邮件"
 
 #: error_window.py:103
 msgid "Description"
 msgstr "描述"
 
-#: error_window.py:112 widgets/waveform/waveform_widget.py:3347
+#: error_window.py:112 widgets/waveform/waveform_widget.py:3397
 msgid "Edit"
 msgstr "编辑"
 
 #: error_window.py:113
 msgid "View as Markdown"
 msgstr "以 Markdown 格式查看"
 
 #: error_window.py:119
 msgid "Abort"
 msgstr "终止"
 
-#: error_window.py:120 main.py:365 widgets/settings/settings_widget.py:539
+#: error_window.py:120 main.py:363 widgets/settings/settings_widget.py:539
 msgid "View"
 msgstr "查看"
 
 #: error_window.py:121
 msgid "Submit"
 msgstr "提交"
 
@@ -319,15 +319,15 @@
 msgid "Revert to previous configuration"
 msgstr "恢复到以前的配置"
 
 #: error_window.py:282
 msgid "Revert to defaults"
 msgstr "恢复到默认值"
 
-#: error_window.py:283 main.py:363 main.py:409
+#: error_window.py:283 main.py:361 main.py:407
 #: widgets/js220_cal/js220_cal_widget.py:38
 msgid "Exit"
 msgstr "退出"
 
 #: exporter.py:49 widgets/signal_record/signal_record_config_widget.py:148
 #: widgets/statistics_record/statistics_record_config_widget.py:111
 msgid "Directory"
@@ -551,154 +551,154 @@
 msgid "Do not show again"
 msgstr "不再显示"
 
 #: intel_graphics_dialog.py:91
 msgid "Intel graphics detected"
 msgstr "检测到英特尔显卡"
 
-#: main.py:70 widgets/value/value_widget.py:653
+#: main.py:69 widgets/value/value_widget.py:660
 msgid "Multimeter"
 msgstr "万用表"
 
-#: main.py:71
+#: main.py:70
 msgid "Oscilloscope"
 msgstr "示波器"
 
-#: main.py:72 main.py:298 main.py:359 main.py:402
+#: main.py:71 main.py:296 main.py:357 main.py:400
 msgid "File"
 msgstr "文件"
 
-#: main.py:82
+#: main.py:81
 msgid "The UI status bar display mode"
 msgstr "用户界面状态栏显示模式"
 
-#: main.py:83
+#: main.py:82
 msgid ""
 "This setting controls the amount of detail shown on the status bar at the "
 "bottom of the UI window. You should usually leave this set to \"normal\" "
 "unless you want more detail concerning the UI internal operation."
 msgstr "此设置可控制用户界面窗口底部状态栏上显示的细节数量。通常应将其设置为 \"正常\"，除非您需要更多有关用户界面内部操作的细节。"
 
-#: main.py:88 safe_mode.py:43
+#: main.py:87 safe_mode.py:43
 msgid "Normal"
 msgstr "正常"
 
-#: main.py:89
+#: main.py:88
 msgid "Troubleshoot"
 msgstr "故障排除"
 
-#: main.py:95
+#: main.py:94
 msgid "Enable developer mode."
 msgstr "启用开发人员模式。"
 
-#: main.py:108
+#: main.py:107
 msgid "PubSub utilization"
 msgstr "PubSub 利用率"
 
-#: main.py:109
+#: main.py:108
 msgid ""
 "Display the number of actions processed by the publish-subscribe broker in "
 "each second."
 msgstr "显示发布-订阅代理每秒处理的操作数。"
 
-#: main.py:114
+#: main.py:113
 msgid "CPU utilization"
 msgstr "CPU 利用率"
 
-#: main.py:115
+#: main.py:114
 msgid ""
 "Display the CPU utilization by this application and the total CPU "
 "utilization by all applications. The value is displayed in percent."
 msgstr "显示此应用程序的 CPU 利用率和所有应用程序的总 CPU 利用率。该值以百分比显示。"
 
-#: main.py:121
+#: main.py:120
 msgid "Memory utilization"
 msgstr "内存利用率"
 
-#: main.py:122
+#: main.py:121
 msgid ""
 "Display the memory (RAM) utilization by this application and by all "
 "applications. The value is displayed in percent."
 msgstr "显示此应用程序和所有应用程序的内存（RAM）利用率。该值以百分比显示。"
 
-#: main.py:216
+#: main.py:214
 msgid "UI"
 msgstr "UI"
 
-#: main.py:330
+#: main.py:328
 msgid "Help"
 msgstr "帮助"
 
-#: main.py:331 widgets/hamburger/hamburger_widget.py:21
+#: main.py:329 widgets/hamburger/hamburger_widget.py:21
 msgid "Getting Started"
 msgstr "开始使用"
 
-#: main.py:332
+#: main.py:330
 msgid "User's Guide"
 msgstr "用户指南"
 
-#: main.py:333 widgets/hamburger/hamburger_widget.py:22
+#: main.py:331 widgets/hamburger/hamburger_widget.py:22
 msgid "Changelog"
 msgstr "更新日志"
 
-#: main.py:334 widgets/help/help_widget.py:59
+#: main.py:332 widgets/help/help_widget.py:59
 msgid "Report Issue"
 msgstr "报告问题"
 
-#: main.py:335
+#: main.py:333
 msgid "View logs..."
 msgstr "查看日志..."
 
-#: main.py:336 widgets/hamburger/hamburger_widget.py:23
+#: main.py:334 widgets/hamburger/hamburger_widget.py:23
 msgid "Credits"
 msgstr "荣誉"
 
-#: main.py:337 widgets/hamburger/hamburger_widget.py:24
+#: main.py:335 widgets/hamburger/hamburger_widget.py:24
 msgid "About"
 msgstr "关于"
 
-#: main.py:360
+#: main.py:358
 msgid "Open"
 msgstr "打开"
 
-#: main.py:361
+#: main.py:359
 msgid "Open recent"
 msgstr "近期开放"
 
-#: main.py:362 main.py:408
+#: main.py:360 main.py:406
 msgid "Clear config and exit"
 msgstr "清除配置并退出"
 
-#: main.py:366 widgets/settings/settings_widget.py:541
+#: main.py:364 widgets/settings/settings_widget.py:541
 msgid "Widgets"
 msgstr "小工具"
 
-#: main.py:367
+#: main.py:365
 msgid "Tools"
 msgstr "工具"
 
-#: main.py:368
+#: main.py:366
 msgid "Clear Accumulators"
 msgstr "透明蓄电池"
 
-#: main.py:403
+#: main.py:401
 msgid "Info"
 msgstr "信息"
 
-#: main.py:404 widget_tools.py:92 widgets/settings/settings_widget.py:31
+#: main.py:402 widget_tools.py:92 widgets/settings/settings_widget.py:31
 #: widgets/settings/settings_widget.py:574
 #: widgets/sidebar/sidebar_widget.py:41
 msgid "Settings"
 msgstr "设置"
 
-#: main.py:693
+#: main.py:710
 msgid "Manage"
 msgstr "管理"
 
-#: main.py:730
+#: main.py:747
 msgid "Select file to open"
 msgstr "选择要打开的文件"
 
 #: paths.py:30 styles/manager.py:46
 msgid "The name for this widget."
 msgstr "该部件的名称。"
 
@@ -837,47 +837,47 @@
 msgid "Source"
 msgstr "来源"
 
 #: units.py:35
 msgid "Use the application defaults"
 msgstr "使用应用默认值"
 
-#: view.py:68
+#: view.py:72
 msgid "The active theme."
 msgstr "活动主题。"
 
-#: view.py:70
+#: view.py:74
 msgid "Joulescope standard theme"
 msgstr "Joulescope 标准主题"
 
-#: view.py:70
+#: view.py:74
 msgid "System OS-specific theme"
 msgstr "系统操作系统特定主题"
 
-#: view.py:75
+#: view.py:79
 msgid "The color scheme name."
 msgstr "配色方案名称。"
 
-#: view.py:77
+#: view.py:81
 msgid "Dark background"
 msgstr "深色背景"
 
-#: view.py:77
+#: view.py:81
 msgid "Light background"
 msgstr "光背景"
 
-#: view.py:81
+#: view.py:85
 msgid "The font scheme name."
 msgstr "字体方案名称。"
 
-#: view.py:83
+#: view.py:87
 msgid "Joulescope standard font theme"
 msgstr "Joulescope 标准字体主题"
 
-#: view.py:102 widgets/view_manager/view_manager_widget.py:146
+#: view.py:106 widgets/view_manager/view_manager_widget.py:146
 msgid "New View"
 msgstr "新视图"
 
 #: zip_inspector.py:23
 msgid "ZIP Inspector"
 msgstr "ZIP 检查器"
 
@@ -971,15 +971,15 @@
 "When enabled, current flows between the current terminals. When disabled, "
 "current cannot flow between the current terminals. In common system setups, "
 "this inhibits target power, which can be used to power cycle reset the "
 "target device."
 msgstr "启用时，电流在电流端子之间流动。禁用时，电流不会在电流端之间流动。在常见的系统设置中，这会抑制目标电源，可用于对目标设备进行电源循环复位。"
 
 #: devices/jsdrv/js110.py:147 devices/jsdrv/js220.py:163
-#: widgets/waveform/waveform_widget.py:110
+#: widgets/waveform/waveform_widget.py:109
 msgid "Current range"
 msgstr "电流范围"
 
 #: devices/jsdrv/js110.py:149
 msgid ""
 "Configure the J110's current range. Most applications should use the "
 "default, \"auto\"."
@@ -1098,33 +1098,33 @@
 #: devices/jsdrv/js110.py:255
 msgid ""
 "The number of samples after the current range window used to determine the "
 "mean. This value is ignored for all other IRF types."
 msgstr "用于确定平均值的电流范围窗口后的采样数目。对于所有其他 IRF 类型，该值将被忽略。"
 
 #: devices/jsdrv/js110.py:269 devices/jsdrv/js220.py:332
-#: widgets/device_control/fuse.py:103 widgets/waveform/waveform_widget.py:105
+#: widgets/device_control/fuse.py:103 widgets/waveform/waveform_widget.py:104
 msgid "Current"
 msgstr "电流"
 
 #: devices/jsdrv/js110.py:270 devices/jsdrv/js220.py:333
 msgid "Enable the current signal streaming."
 msgstr "启用电流信号流。"
 
 #: devices/jsdrv/js110.py:278 devices/jsdrv/js220.py:341
-#: widgets/waveform/waveform_widget.py:106
+#: widgets/waveform/waveform_widget.py:105
 msgid "Voltage"
 msgstr "电压"
 
 #: devices/jsdrv/js110.py:279 devices/jsdrv/js220.py:342
 msgid "Enable the voltage signal streaming."
 msgstr "启用电压信号流。"
 
 #: devices/jsdrv/js110.py:287 devices/jsdrv/js220.py:350
-#: widgets/waveform/waveform_widget.py:107
+#: widgets/waveform/waveform_widget.py:106
 msgid "Power"
 msgstr "功率"
 
 #: devices/jsdrv/js110.py:288 devices/jsdrv/js220.py:351
 msgid "Enable the power signal streaming."
 msgstr "启用电源信号流。"
 
@@ -1303,15 +1303,15 @@
 msgid "GPI 3"
 msgstr "GPI 3"
 
 #: devices/jsdrv/js220.py:402
 msgid "Enable the general purpose input 3 signal streaming."
 msgstr "启用通用输入 3 信号流。"
 
-#: devices/jsdrv/js220.py:410 widgets/waveform/waveform_widget.py:124
+#: devices/jsdrv/js220.py:410 widgets/waveform/waveform_widget.py:123
 msgid "Trigger input"
 msgstr "触发输入"
 
 #: devices/jsdrv/js220.py:411
 msgid "Enable the trigger input signal streaming."
 msgstr "启用触发输入信号流。"
 
@@ -1322,15 +1322,15 @@
 #: devices/jsdrv/jsdrv_stream_buffer.py:44
 #: devices/jsdrv/jsdrv_stream_buffer.py:93
 #: devices/jsdrv/jsdrv_stream_buffer.py:107 plugins/selector.py:58
 #: widgets/settings/settings_widget.py:85
 #: widgets/settings/settings_widget.py:266
 #: widgets/settings/settings_widget.py:364
 #: widgets/settings/settings_widget.py:431
-#: widgets/waveform/waveform_widget.py:3062
+#: widgets/waveform/waveform_widget.py:3104
 msgid "Name"
 msgstr "名称"
 
 #: devices/jsdrv/jsdrv_stream_buffer.py:45
 msgid "Joulescope stream buffer"
 msgstr "Joulescope 数据流缓冲器"
 
@@ -1537,15 +1537,15 @@
 
 #: widgets/accumulator/accumulator_widget.py:27
 #: widgets/value/value_widget.py:31
 msgid "The statistics data stream source."
 msgstr "统计数据流源。"
 
 #: widgets/accumulator/accumulator_widget.py:32
-#: widgets/value/value_widget.py:74
+#: widgets/value/value_widget.py:81
 msgid "The signal to display."
 msgstr "要显示的信号。"
 
 #: widgets/accumulator/accumulator_widget.py:34
 msgid "charge"
 msgstr "电荷"
 
@@ -1628,15 +1628,15 @@
 
 #: widgets/developer/publish_spy_widget.py:20
 #: widgets/developer/publish_spy_widget.py:21
 msgid "Topic"
 msgstr "主题"
 
 #: widgets/developer/publish_spy_widget.py:21
-#: widgets/settings/settings_widget.py:87 widgets/value/value_widget.py:662
+#: widgets/settings/settings_widget.py:87 widgets/value/value_widget.py:669
 msgid "Value"
 msgstr "值"
 
 #: widgets/developer/publish_spy_widget.py:24
 msgid "Publish Spy"
 msgstr "发布间谍"
 
@@ -1666,15 +1666,15 @@
 
 #: widgets/device_control/device_update_dialog.py:24
 #: widgets/device_control/device_update_dialog.py:45
 msgid "Update"
 msgstr "更新"
 
 #: widgets/device_control/device_update_dialog.py:25
-#: widgets/value/value_widget.py:147
+#: widgets/value/value_widget.py:155
 msgid "Device"
 msgstr "器件"
 
 #: widgets/device_control/device_update_dialog.py:27
 #: widgets/progress_bar/progress_bar_widget.py:59
 msgid "Progress"
 msgstr "进展"
@@ -2154,18 +2154,14 @@
 msgid "Click to display additional settings and actions."
 msgstr "单击可显示其他设置和操作。"
 
 #: widgets/sidebar/sidebar_widget.py:60
 msgid "sidebar"
 msgstr "侧边栏"
 
-#: widgets/sidebar/sidebar_widget.py:68
-msgid "The flyout width in pixels."
-msgstr "飞出宽度（像素）。"
-
 #: widgets/signal_record/disk_full_dialog.py:19
 msgid "The disk is full"
 msgstr "磁盘已满"
 
 #: widgets/signal_record/signal_record.py:57
 msgid "Could not open file for write"
 msgstr "无法打开文件进行写入"
@@ -2192,15 +2188,15 @@
 msgid "StatisticsRecordConfig"
 msgstr "统计记录配置"
 
 #: widgets/statistics_record/statistics_record_config_widget.py:123
 msgid "Time Format"
 msgstr "时间格式"
 
-#: widgets/trigger/trigger_widget.py:41 widgets/value/value_widget.py:87
+#: widgets/trigger/trigger_widget.py:41 widgets/value/value_widget.py:94
 msgid "Select the source device"
 msgstr "选择源器件"
 
 #: widgets/trigger/trigger_widget.py:42
 msgid "The device to use for the start condition and stop condition."
 msgstr "用于启动条件和停止条件的设备。"
 
@@ -2363,69 +2359,79 @@
 msgid "Show the statistics fields at the right."
 msgstr "显示右侧的统计字段。"
 
 #: widgets/value/value_widget.py:51
 msgid "Show a leading + or - sign."
 msgstr "显示前导 + 或 - 符号。"
 
-#: widgets/value/value_widget.py:88
+#: widgets/value/value_widget.py:62
+msgid "Divide the quantity by this value."
+msgstr "用这个值除以数量。"
+
+#: widgets/value/value_widget.py:63
+msgid ""
+"The divisor is a floating point number. The number may optionally be "
+"followed by units."
+msgstr "除数是浮点数。数字后面可以选择单位。"
+
+#: widgets/value/value_widget.py:95
 msgid ""
 "The values displayed by this widget come from a single source device. Select"
 " the source device here."
 msgstr "此 widget 显示的值来自单个源器件。在此选择源设备。"
 
-#: widgets/value/value_widget.py:94
+#: widgets/value/value_widget.py:101
 msgid "Hold the display"
 msgstr "保持显示"
 
-#: widgets/value/value_widget.py:96
+#: widgets/value/value_widget.py:103
 msgid "When selected, prevent the display from updating."
 msgstr "选中时，防止显示更新。"
 
-#: widgets/value/value_widget.py:97
+#: widgets/value/value_widget.py:104
 msgid ""
 "The UI also includes a global statistics hold button on the sidebar. When "
 "the global statistics hold button is selected, this button is disabled and "
 "has no effect."
 msgstr "用户界面侧边栏上还有一个全局统计保持按钮。选择全局统计保持按钮后，该按钮将被禁用，没有任何作用。"
 
-#: widgets/value/value_widget.py:100
+#: widgets/value/value_widget.py:107
 msgid ""
 "The displayed values normally update with each new statistics data computed "
 "by the device. When this button is selected, the display will not be "
 "updated. However, the statistics will continue accumulate and accrue (if "
 "selected)."
 msgstr "显示值通常随设备计算的每个新统计数据更新。选择此按钮后，显示值将不会更新。但是，统计数据将继续累积（如果选择）。"
 
-#: widgets/value/value_widget.py:107
+#: widgets/value/value_widget.py:114
 msgid "Accrue values over time"
 msgstr "随时间累积值"
 
-#: widgets/value/value_widget.py:109
+#: widgets/value/value_widget.py:116
 msgid ""
 "Current, voltage, and power are normally computed over a single statistics "
 "frequency interval. Press this button to accrue the values indefinitely. "
 "Press again to return to normal operation."
 msgstr "电流、电压和功率通常在单个统计频率间隔内计算。按下此按钮可无限累积数值。再次按下则返回正常操作。"
 
-#: widgets/value/value_widget.py:113
+#: widgets/value/value_widget.py:120
 msgid ""
 "Note that this button does not affect the charge and energy accumulation. "
 "Both accumulate indefinitely regardless of this button state."
 msgstr "请注意，该按钮不会影响电荷和能量的累积。无论按钮状态如何，两者都会无限累积。"
 
-#: widgets/value/value_widget.py:195
+#: widgets/value/value_widget.py:203
 msgid "Not present"
 msgstr "不存在"
 
-#: widgets/value/value_widget.py:215
+#: widgets/value/value_widget.py:223
 msgid "Hold"
 msgstr "保持"
 
-#: widgets/value/value_widget.py:223
+#: widgets/value/value_widget.py:231
 msgid "Accrue"
 msgstr "增加"
 
 #: widgets/view_manager/view_manager_widget.py:108
 #: widgets/view_manager/view_manager_widget.py:174
 msgid "View Manager"
 msgstr "查看管理器"
@@ -2471,34 +2477,34 @@
 msgstr "右三角"
 
 #: widgets/waveform/text_annotation.py:62
 msgid "triangle left"
 msgstr "左三角形"
 
 #: widgets/waveform/text_annotation.py:66
-#: widgets/waveform/waveform_widget.py:3008
+#: widgets/waveform/waveform_widget.py:3050
 msgid "Manual"
 msgstr "手册"
 
 #: widgets/waveform/text_annotation.py:67
 msgid "Centered"
 msgstr "居中"
 
 #: widgets/waveform/text_annotation.py:99
-#: widgets/waveform/waveform_widget.py:3123
+#: widgets/waveform/waveform_widget.py:3167
 msgid "Text"
 msgstr "文本"
 
 #: widgets/waveform/text_annotation.py:107
-#: widgets/waveform/waveform_widget.py:3348
+#: widgets/waveform/waveform_widget.py:3398
 msgid "Show text"
 msgstr "显示文本"
 
 #: widgets/waveform/text_annotation.py:116
-#: widgets/waveform/waveform_widget.py:3360
+#: widgets/waveform/waveform_widget.py:3410
 msgid "Shape"
 msgstr "形状"
 
 #: widgets/waveform/text_annotation.py:126
 msgid "Y Mode"
 msgstr "Y 模式"
 
@@ -2665,317 +2671,317 @@
 #: widgets/waveform/waveform_source_widget.py:40
 msgid ""
 "\"default\" will use the default source which is normally configured using "
 "the Device Control widget."
 msgstr "\"默认 \"将使用默认源，该源通常使用设备控制 widget 进行配置。"
 
 #: widgets/waveform/waveform_source_widget.py:104
-#: widgets/waveform/waveform_widget.py:402
-#: widgets/waveform/waveform_widget.py:479
+#: widgets/waveform/waveform_widget.py:401
+#: widgets/waveform/waveform_widget.py:478
 msgid "off"
 msgstr "关闭"
 
-#: widgets/waveform/waveform_widget.py:44
+#: widgets/waveform/waveform_widget.py:43
 msgid "Waveform"
 msgstr "波形"
 
-#: widgets/waveform/waveform_widget.py:120
+#: widgets/waveform/waveform_widget.py:119
 msgid "General purpose input 0"
 msgstr "通用输入 0"
 
-#: widgets/waveform/waveform_widget.py:121
+#: widgets/waveform/waveform_widget.py:120
 msgid "General purpose input 1"
 msgstr "通用输入 1"
 
-#: widgets/waveform/waveform_widget.py:122
+#: widgets/waveform/waveform_widget.py:121
 msgid "General purpose input 2"
 msgstr "通用输入 2"
 
-#: widgets/waveform/waveform_widget.py:123
+#: widgets/waveform/waveform_widget.py:122
 msgid "General purpose input 3"
 msgstr "通用输入 3"
 
-#: widgets/waveform/waveform_widget.py:358
+#: widgets/waveform/waveform_widget.py:357
 msgid "The source filter string."
 msgstr "源滤波器串。"
 
-#: widgets/waveform/waveform_widget.py:369
+#: widgets/waveform/waveform_widget.py:368
 msgid "The trace width."
 msgstr "轨迹宽度。"
 
-#: widgets/waveform/waveform_widget.py:384
+#: widgets/waveform/waveform_widget.py:383
 msgid "The target frames per second."
 msgstr "目标帧/秒。"
 
-#: widgets/waveform/waveform_widget.py:386
+#: widgets/waveform/waveform_widget.py:385
 msgid "vsync"
 msgstr "vsync"
 
-#: widgets/waveform/waveform_widget.py:387
+#: widgets/waveform/waveform_widget.py:386
 msgid "20 Hz"
 msgstr "20 赫兹"
 
-#: widgets/waveform/waveform_widget.py:388
+#: widgets/waveform/waveform_widget.py:387
 msgid "10 Hz"
 msgstr "10 赫兹"
 
-#: widgets/waveform/waveform_widget.py:389
+#: widgets/waveform/waveform_widget.py:388
 msgid "5 Hz"
 msgstr "5 赫兹"
 
-#: widgets/waveform/waveform_widget.py:395
+#: widgets/waveform/waveform_widget.py:394
 msgid "The minimum interval between repaint in milliseconds."
 msgstr "以毫秒为单位的最小重绘间隔。"
 
-#: widgets/waveform/waveform_widget.py:400
+#: widgets/waveform/waveform_widget.py:399
 msgid "Show the minimum and maximum extents fill."
 msgstr "显示填充的最小和最大范围。"
 
-#: widgets/waveform/waveform_widget.py:403
+#: widgets/waveform/waveform_widget.py:402
 msgid "lines"
 msgstr "线路"
 
-#: widgets/waveform/waveform_widget.py:404
+#: widgets/waveform/waveform_widget.py:403
 msgid "fill 1"
 msgstr "填充 1"
 
-#: widgets/waveform/waveform_widget.py:405
+#: widgets/waveform/waveform_widget.py:404
 msgid "fill 2"
 msgstr "填充 2"
 
-#: widgets/waveform/waveform_widget.py:411
+#: widgets/waveform/waveform_widget.py:410
 msgid "Show the frames per second."
 msgstr "显示每秒帧数。"
 
-#: widgets/waveform/waveform_widget.py:416
+#: widgets/waveform/waveform_widget.py:415
 msgid "Show the statistics on mouse hover."
 msgstr "鼠标悬停时显示统计数据。"
 
-#: widgets/waveform/waveform_widget.py:421
+#: widgets/waveform/waveform_widget.py:420
 msgid "Show the plot statistics on the right."
 msgstr "在右侧显示绘图统计数据。"
 
-#: widgets/waveform/waveform_widget.py:426
+#: widgets/waveform/waveform_widget.py:425
 msgid "Show frequency for dual markers and statistics."
 msgstr "显示频率，用于双重标记和统计。"
 
-#: widgets/waveform/waveform_widget.py:431
+#: widgets/waveform/waveform_widget.py:430
 msgid "The quantities to display by default."
 msgstr "默认显示的量。"
 
-#: widgets/waveform/waveform_widget.py:437
+#: widgets/waveform/waveform_widget.py:436
 msgid "The precision to display in digits."
 msgstr "以位数显示的精度。"
 
-#: widgets/waveform/waveform_widget.py:443
+#: widgets/waveform/waveform_widget.py:442
 msgid "Use OpenGL rendering."
 msgstr "使用 OpenGL 渲染。"
 
-#: widgets/waveform/waveform_widget.py:454
+#: widgets/waveform/waveform_widget.py:453
 msgid "Pin the left side (oldest) data so that it stays in view."
 msgstr "钉住左侧（最旧）数据，使其保持在视图中。"
 
-#: widgets/waveform/waveform_widget.py:459
+#: widgets/waveform/waveform_widget.py:458
 msgid "Pin the right side (newest) data so that it stays in view."
 msgstr "钉住右侧（最新）数据，使其保持在视图中。"
 
-#: widgets/waveform/waveform_widget.py:464
+#: widgets/waveform/waveform_widget.py:463
 msgid "The waveform state."
 msgstr "波形状态。"
 
-#: widgets/waveform/waveform_widget.py:470
+#: widgets/waveform/waveform_widget.py:469
 msgid "The annotations."
 msgstr "注释。"
 
-#: widgets/waveform/waveform_widget.py:476
+#: widgets/waveform/waveform_widget.py:475
 msgid "Control location"
 msgstr "控制位置"
 
-#: widgets/waveform/waveform_widget.py:480
+#: widgets/waveform/waveform_widget.py:479
 msgid "top"
 msgstr "顶部"
 
-#: widgets/waveform/waveform_widget.py:481
+#: widgets/waveform/waveform_widget.py:480
 msgid "bottom"
 msgstr "底部"
 
-#: widgets/waveform/waveform_widget.py:486
+#: widgets/waveform/waveform_widget.py:485
 msgid "The signal quantity to show in the summary."
 msgstr "要在摘要中显示的信号量。"
 
-#: widgets/waveform/waveform_widget.py:492
+#: widgets/waveform/waveform_widget.py:491
 msgid "X-axis annotation mode"
 msgstr "X 轴注释模式"
 
-#: widgets/waveform/waveform_widget.py:495
-#: widgets/waveform/waveform_widget.py:2888
+#: widgets/waveform/waveform_widget.py:494
+#: widgets/waveform/waveform_widget.py:2930
 msgid "Absolute"
 msgstr "绝对值"
 
-#: widgets/waveform/waveform_widget.py:496
-#: widgets/waveform/waveform_widget.py:2893
+#: widgets/waveform/waveform_widget.py:495
+#: widgets/waveform/waveform_widget.py:2935
 msgid "Relative"
 msgstr "相对值"
 
-#: widgets/waveform/waveform_widget.py:502
+#: widgets/waveform/waveform_widget.py:501
 msgid "The available subsources."
 msgstr "可用的子源。"
 
-#: widgets/waveform/waveform_widget.py:508
+#: widgets/waveform/waveform_widget.py:507
 msgid "The selected subsources for each trace."
 msgstr "每个跟踪所选的子源。"
 
-#: widgets/waveform/waveform_widget.py:514
+#: widgets/waveform/waveform_widget.py:513
 msgid "The trace priority: highest int value on top, None is off."
 msgstr "跟踪优先级：最高 int 值在顶部，无则关闭。"
 
-#: widgets/waveform/waveform_widget.py:2834
-#: widgets/waveform/waveform_widget.py:3135
+#: widgets/waveform/waveform_widget.py:2877
+#: widgets/waveform/waveform_widget.py:3179
 msgid "Save image to file"
 msgstr "将图像保存到文件"
 
-#: widgets/waveform/waveform_widget.py:2882
-#: widgets/waveform/waveform_widget.py:2951
+#: widgets/waveform/waveform_widget.py:2924
+#: widgets/waveform/waveform_widget.py:2993
 msgid "Single marker"
 msgstr "单标记"
 
-#: widgets/waveform/waveform_widget.py:2883
-#: widgets/waveform/waveform_widget.py:2952
+#: widgets/waveform/waveform_widget.py:2925
+#: widgets/waveform/waveform_widget.py:2994
 msgid "Dual markers"
 msgstr "双标记"
 
-#: widgets/waveform/waveform_widget.py:2885
+#: widgets/waveform/waveform_widget.py:2927
 msgid "Mode"
 msgstr "模式"
 
-#: widgets/waveform/waveform_widget.py:2898
-#: widgets/waveform/waveform_widget.py:2953
-#: widgets/waveform/waveform_widget.py:3111
-#: widgets/waveform/waveform_widget.py:3129
+#: widgets/waveform/waveform_widget.py:2940
+#: widgets/waveform/waveform_widget.py:2995
+#: widgets/waveform/waveform_widget.py:3155
+#: widgets/waveform/waveform_widget.py:3173
 msgid "Clear all"
 msgstr "全部清除"
 
-#: widgets/waveform/waveform_widget.py:2909
-#: widgets/waveform/waveform_widget.py:2998
-#: widgets/waveform/waveform_widget.py:3117
+#: widgets/waveform/waveform_widget.py:2951
+#: widgets/waveform/waveform_widget.py:3040
+#: widgets/waveform/waveform_widget.py:3161
 msgid "Annotations"
 msgstr "注释"
 
-#: widgets/waveform/waveform_widget.py:3001
+#: widgets/waveform/waveform_widget.py:3043
 msgid "Range"
 msgstr "范围"
 
-#: widgets/waveform/waveform_widget.py:3005
-#: widgets/waveform/waveform_widget.py:3328
+#: widgets/waveform/waveform_widget.py:3047
+#: widgets/waveform/waveform_widget.py:3378
 msgid "Auto"
 msgstr "自动"
 
-#: widgets/waveform/waveform_widget.py:3011
+#: widgets/waveform/waveform_widget.py:3053
 msgid "Exact"
 msgstr "精确"
 
-#: widgets/waveform/waveform_widget.py:3020
+#: widgets/waveform/waveform_widget.py:3062
 msgid "Scale"
 msgstr "规模"
 
-#: widgets/waveform/waveform_widget.py:3023
+#: widgets/waveform/waveform_widget.py:3065
 msgid "Linear"
 msgstr "线性"
 
-#: widgets/waveform/waveform_widget.py:3028
+#: widgets/waveform/waveform_widget.py:3070
 msgid "Logarithmic"
 msgstr "对数"
 
-#: widgets/waveform/waveform_widget.py:3036
+#: widgets/waveform/waveform_widget.py:3078
 msgid "Logarithmic zero"
 msgstr "对数零"
 
-#: widgets/waveform/waveform_widget.py:3050
+#: widgets/waveform/waveform_widget.py:3092
 msgid "Preferred prefix"
 msgstr "首选前缀"
 
-#: widgets/waveform/waveform_widget.py:3108
+#: widgets/waveform/waveform_widget.py:3152
 msgid "Add"
 msgstr "添加"
 
-#: widgets/waveform/waveform_widget.py:3109
+#: widgets/waveform/waveform_widget.py:3153
 msgid "Hide all text"
 msgstr "隐藏所有文本"
 
-#: widgets/waveform/waveform_widget.py:3110
+#: widgets/waveform/waveform_widget.py:3154
 msgid "Show all text"
 msgstr "显示所有文本"
 
-#: widgets/waveform/waveform_widget.py:3118
+#: widgets/waveform/waveform_widget.py:3162
 msgid "Vertical"
 msgstr "垂直"
 
-#: widgets/waveform/waveform_widget.py:3121
+#: widgets/waveform/waveform_widget.py:3165
 msgid "Horizontal"
 msgstr "水平"
 
-#: widgets/waveform/waveform_widget.py:3127
+#: widgets/waveform/waveform_widget.py:3171
 msgid "Save"
 msgstr "保存"
 
-#: widgets/waveform/waveform_widget.py:3132
+#: widgets/waveform/waveform_widget.py:3176
 msgid "Y-axis auto range"
 msgstr "Y 轴自动量程"
 
-#: widgets/waveform/waveform_widget.py:3136
+#: widgets/waveform/waveform_widget.py:3180
 msgid "Copy image to clipboard"
 msgstr "将图像复制到剪贴板"
 
-#: widgets/waveform/waveform_widget.py:3137
+#: widgets/waveform/waveform_widget.py:3181
 msgid "Export visible data"
 msgstr "导出可见数据"
 
-#: widgets/waveform/waveform_widget.py:3138
+#: widgets/waveform/waveform_widget.py:3182
 msgid "Export all data"
 msgstr "导出所有数据"
 
-#: widgets/waveform/waveform_widget.py:3304
+#: widgets/waveform/waveform_widget.py:3354
 msgid "Export"
 msgstr "出口"
 
-#: widgets/waveform/waveform_widget.py:3305
+#: widgets/waveform/waveform_widget.py:3355
 msgid "Analysis"
 msgstr "分析"
 
-#: widgets/waveform/waveform_widget.py:3313
+#: widgets/waveform/waveform_widget.py:3363
 msgid "Interval"
 msgstr "间隔"
 
-#: widgets/waveform/waveform_widget.py:3322
+#: widgets/waveform/waveform_widget.py:3372
 msgid "Zoom"
 msgstr "放大"
 
-#: widgets/waveform/waveform_widget.py:3326
+#: widgets/waveform/waveform_widget.py:3376
 msgid "Show statistics"
 msgstr "显示统计数据"
 
-#: widgets/waveform/waveform_widget.py:3331
+#: widgets/waveform/waveform_widget.py:3381
 msgid "Left"
 msgstr "左侧"
 
-#: widgets/waveform/waveform_widget.py:3334
+#: widgets/waveform/waveform_widget.py:3384
 msgid "Right"
 msgstr "正确"
 
-#: widgets/waveform/waveform_widget.py:3337
+#: widgets/waveform/waveform_widget.py:3387
 msgid "Off"
 msgstr "关闭"
 
-#: widgets/waveform/waveform_widget.py:3340
-#: widgets/waveform/waveform_widget.py:3368
-#: widgets/waveform/waveform_widget.py:3397
+#: widgets/waveform/waveform_widget.py:3390
+#: widgets/waveform/waveform_widget.py:3418
+#: widgets/waveform/waveform_widget.py:3448
 msgid "Remove"
 msgstr "删除"
 
-#: widgets/waveform/waveform_widget.py:3351
+#: widgets/waveform/waveform_widget.py:3401
 msgid "Y mode"
 msgstr "Y 模式"
 
 #: widgets/waveform/y_range_widget.py:67
 msgid "max"
 msgstr "最大值"
```

### Comparing `joulescope_ui-1.1.6/joulescope_ui/logging_util.py` & `joulescope_ui-1.1.7/joulescope_ui/logging_util.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/main.py` & `joulescope_ui-1.1.7/joulescope_ui/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 # https://wiki.qt.io/Gallery_of_Qt_CSS_Based_Styles
 
 from joulescope_ui import pubsub_singleton, N_, get_topic_name, get_instance, \
     tooltip_format, CAPABILITIES, Metadata, __version__
 from joulescope_ui.locale import locale_get
 from joulescope_ui.pubsub import UNDO_TOPIC, REDO_TOPIC, is_pubsub_registered
 from joulescope_ui.pubsub_aggregator import PubsubAggregator
-from joulescope_ui.shortcuts import Shortcuts
 from joulescope_ui.widgets import *   # registers all built-in widgets
 from joulescope_ui import logging_util
 from joulescope_ui.plugins import PluginManager
 from joulescope_ui.reporter import create as reporter_create
 from joulescope_ui.safe_mode import safe_mode_dialog
 from joulescope_ui.styles.manager import style_settings
 from joulescope_ui.process_monitor import ProcessMonitor
@@ -208,15 +207,14 @@
         self._filename = filename
         self._resync_event = None
         super(MainWindow, self).__init__()
         self.setWindowTitle(_UI_WINDOW_TITLE if filename is None else _JLS_WINDOW_TITLE)
         self._dialog = None
         self._pend_queue = []
         self._software_update_status = None
-        self._shortcuts = Shortcuts(self)
         self.SETTINGS = style_settings(N_('UI'))
         for key, value in _SETTINGS.items():
             self.SETTINGS[key] = value
         self._app = App().register(mode='normal' if filename is None else 'file_viewer')
         self._paths = Paths().register()
         self.resize(800, 600)
         self._icon = QtGui.QIcon()
@@ -415,17 +413,26 @@
         self.pubsub.publish('registry/style/settings/enable', True)
         self.pubsub.publish('registry/style/actions/!render', None)
         pubsub_singleton.process()
 
         self._process_monitor = ProcessMonitor(self)
         self._process_monitor.update.connect(self._on_process_monitor)
 
-        self._shortcuts.add(QtGui.QKeySequence.Undo, UNDO_TOPIC, None)
-        self._shortcuts.add(QtGui.QKeySequence.Redo, REDO_TOPIC, None)
-        self._shortcuts.add(QtCore.Qt.Key_Space, 'registry/app/settings/signal_stream_enable', '__toggle__')
+        self._keys = {
+            (QtCore.Qt.Key_Space, QtCore.Qt.KeyboardModifier.NoModifier):
+                ('registry/app/settings/signal_stream_enable', '__toggle__'),
+            (QtCore.Qt.Key_O, QtCore.Qt.KeyboardModifier.ControlModifier):
+                ('registry/ui/actions/!file_open_request', None),
+            (QtCore.Qt.Key_Q, QtCore.Qt.KeyboardModifier.ControlModifier): ('registry/ui/actions/!close', ''),
+            (QtCore.Qt.Key_Z, QtCore.Qt.KeyboardModifier.ControlModifier): (UNDO_TOPIC, None),
+            (QtCore.Qt.Key_Z, QtCore.Qt.KeyboardModifier.ControlModifier | QtCore.Qt.KeyboardModifier.ShiftModifier):
+                (REDO_TOPIC, None),
+        }
+        if sys.platform.startswith('win'):
+            self._keys[(QtCore.Qt.Key_Y, QtCore.Qt.KeyboardModifier.ControlModifier)] = (REDO_TOPIC, None)
 
         if filename is None:
             self.setAcceptDrops(True)
         self.show()
 
         self.pubsub.publish(UNDO_TOPIC, 'clear', defer=True)
         self.pubsub.publish(REDO_TOPIC, 'clear', defer=True)
@@ -441,14 +448,24 @@
         self.pubsub.register(DiskMonitor)
         self.pubsub.register(DiskMonitor(), 'DiskMonitor:0')
 
         self._blink_timer = QtCore.QTimer(self)
         self._blink_timer.timeout.connect(self._on_blink_timer)
         self._blink_timer.start(250)
 
+    def on_action_key_press(self, event: QtGui.QKeyEvent):
+        ev = event.key(), event.modifiers()
+        self._log.info(f'on_action_key_press: {ev}')
+        action = self._keys.get(ev)
+        if action is not None:
+            self.pubsub.publish(action[0], action[1])
+
+    def keyPressEvent(self, event: QtGui.QKeyEvent) -> None:
+        self.on_action_key_press(event)
+
     def _startup_display_maybe(self):
         # display changelog on version change
         topic = f'{self.topic}/settings/changelog_version_show'
         changelog_version_show = self.pubsub.query(topic, default=None)
         self.pubsub.publish(topic, __version__)
         if changelog_version_show is None:
             self.pubsub.publish(topic, __version__)
@@ -916,14 +933,21 @@
             if safe_mode_config['action'] == 'report_issue':
                 raise RuntimeError('Safe mode report issue')
             elif safe_mode_config['action'] == 'close':
                 action_close = True
 
         try:
             if not action_close:
+                try:
+                    p1 = pubsub_singleton.query('common/settings/paths/data')
+                    p2 = pubsub_singleton.query('registry/paths/settings/path', default=p1)
+                    if p1 == p2:
+                        os.makedirs(p1, exist_ok=True)
+                except Exception:
+                    _log.warning(f'Could not create data path {p1} {p2}')
                 resources = load_resources()
                 fonts = load_fonts()
                 appnope.nope()
 
                 ui = MainWindow(filename=filename, is_config_load=is_config_load)
                 pubsub_singleton.notify_fn = ui.resync_request
                 try:
```

### Comparing `joulescope_ui-1.1.6/joulescope_ui/mem_leak_debugger.py` & `joulescope_ui-1.1.7/joulescope_ui/mem_leak_debugger.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/metadata.py` & `joulescope_ui-1.1.7/joulescope_ui/metadata.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/paths.py` & `joulescope_ui-1.1.7/joulescope_ui/paths.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/plugins/__init__.py` & `joulescope_ui-1.1.7/joulescope_ui/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/plugins/manager.py` & `joulescope_ui-1.1.7/joulescope_ui/plugins/manager.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/plugins/selector.py` & `joulescope_ui-1.1.7/joulescope_ui/plugins/selector.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/plugins/test/plugins/p1/__init__.py` & `joulescope_ui-1.1.7/joulescope_ui/plugins/test/plugins/p1/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/plugins/test/test_manager.py` & `joulescope_ui-1.1.7/joulescope_ui/plugins/test/test_manager.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/process_monitor.py` & `joulescope_ui-1.1.7/joulescope_ui/process_monitor.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/profile.py` & `joulescope_ui-1.1.7/joulescope_ui/profile.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/pubsub.py` & `joulescope_ui-1.1.7/joulescope_ui/pubsub.py`

 * *Files 0% similar despite different names*

```diff
@@ -439,15 +439,14 @@
             app_path = os.path.join(os.path.expanduser('~'), 'Library', 'Application Support', self._app)
         elif 'linux' in sys.platform:
             user_path = os.path.join(os.path.expanduser('~'), 'Documents', self._app)
             app_path = os.path.join(os.path.expanduser('~'), '.' + self._app)
         else:
             raise RuntimeError('unsupported platform')
 
-        os.makedirs(user_path, exist_ok=True)
         self.topic_add('common/actions/profile', 'node', 'Profile actions')
         self.topic_add('common/settings/profile', 'node', 'Profile settings')
 
         self.topic_add('common/settings/paths', 'node', 'Common directory and file paths')
         self.topic_add('common/settings/paths/app', 'str', 'Base application directory', default=app_path)
         self.topic_add('common/settings/paths/config', 'str', 'Config directory', default=os.path.join(app_path, 'config'))
         self.topic_add('common/settings/paths/log', 'str', 'Log directory', default=os.path.join(app_path, 'log'))
@@ -1053,21 +1052,22 @@
         :param obj: The class type or instance to register.
         :param unique_id: The unique_id to use for this class.
             None (default) determines a suitable unique_id.
             For classes, the class name.
             For instances, a randomly generated value.
         :type unique_id: str, optional
         :param parent: The optional parent unique_id, topic, or object.
+        :return: False on failure, True on success.
         """
         pubsub_attr = _pubsub_attr_name(obj)
         if pubsub_attr in obj.__dict__ and len(obj.__dict__[pubsub_attr]):
             self._log.info('Duplicate registration for %s', obj)
             if parent is not None:
                 self._parent_add(obj, parent)
-            return
+            return False
         if unique_id is None:
             if isinstance(obj, type):
                 # Use the unqualified class name
                 # This keeps the string short & readable, but names must avoid collisions.
                 unique_id = obj.__name__
             else:
                 cls_unique_id = getattr(obj.__class__, 'unique_id', obj.__class__.__name__)
@@ -1139,18 +1139,20 @@
         except Exception:
             register_abort = True
             self._log.exception('register(unique_id=%s) callback failed', unique_id)
         self._register_capabilities(obj, unique_id)
         self._log.info('register(unique_id=%s) done %s', unique_id, 'ABORT' if register_abort else '')
         if register_abort:
             self.unregister(obj, delete=True)
-            raise RuntimeError(f'register(unique_id={unique_id}) aborted')
+            self._log.error(f'register(unique_id={unique_id}) aborted')
+            return False
         else:
             getattr(obj, pubsub_attr)['is_registered'] = True
             self._registry_add(unique_id)
+            return True
 
     def _parent_add(self, obj, parent=None):
         if parent is None:
             self._parent_remove(obj)
             return
         unique_id = get_unique_id(obj)
         self.publish(f'{get_topic_name(obj)}/parent', get_unique_id(parent))
```

### Comparing `joulescope_ui-1.1.6/joulescope_ui/pubsub_aggregator.py` & `joulescope_ui-1.1.7/joulescope_ui/pubsub_aggregator.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/pubsub_callable.py` & `joulescope_ui-1.1.7/joulescope_ui/pubsub_callable.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/pubsub_proxy.py` & `joulescope_ui-1.1.7/joulescope_ui/pubsub_proxy.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/range_tool.py` & `joulescope_ui-1.1.7/joulescope_ui/range_tool.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/range_tools/__init__.py` & `joulescope_ui-1.1.7/joulescope_ui/range_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/range_tools/cdf.py` & `joulescope_ui-1.1.7/joulescope_ui/range_tools/cdf.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/range_tools/frequency.py` & `joulescope_ui-1.1.7/joulescope_ui/range_tools/frequency.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/range_tools/histogram.py` & `joulescope_ui-1.1.7/joulescope_ui/range_tools/histogram.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/range_tools/max_window.py` & `joulescope_ui-1.1.7/joulescope_ui/range_tools/max_window.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/range_tools/plugin_helpers.py` & `joulescope_ui-1.1.7/joulescope_ui/range_tools/plugin_helpers.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/range_tools/usb_inrush.py` & `joulescope_ui-1.1.7/joulescope_ui/range_tools/usb_inrush.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/reporter.py` & `joulescope_ui-1.1.7/joulescope_ui/reporter.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/resources/dmg_background.png` & `joulescope_ui-1.1.7/joulescope_ui/resources/dmg_background.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/resources/dmg_background.svg` & `joulescope_ui-1.1.7/joulescope_ui/resources/dmg_background.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/resources/dmg_background@2x.png` & `joulescope_ui-1.1.7/joulescope_ui/resources/dmg_background@2x.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/resources/icon.ico` & `joulescope_ui-1.1.7/joulescope_ui/resources/icon.ico`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/resources/icon.iconset/icon_128x128.png` & `joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_128x128.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/resources/icon.iconset/icon_128x128@2.png` & `joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_128x128@2.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/resources/icon.iconset/icon_16x16@2.png` & `joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_16x16@2.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/resources/icon.iconset/icon_256x256.png` & `joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_256x256.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/resources/icon.iconset/icon_256x256@2.png` & `joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_256x256@2.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/resources/icon.iconset/icon_32x32.png` & `joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_32x32.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/resources/icon.iconset/icon_32x32@2.png` & `joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_32x32@2.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/resources/icon.iconset/icon_512x512.png` & `joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_512x512.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/resources/icon.iconset/icon_512x512@2.png` & `joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_512x512@2.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/resources/icon.iconset/icon_64x64.png` & `joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_64x64.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/resources/icon.iconset/icon_64x64@2.png` & `joulescope_ui-1.1.7/joulescope_ui/resources/icon.iconset/icon_64x64@2.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/resources/icons.svg` & `joulescope_ui-1.1.7/joulescope_ui/resources/icons.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/resources/logo-large.png` & `joulescope_ui-1.1.7/joulescope_ui/resources/logo-large.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/resources/logo-small.png` & `joulescope_ui-1.1.7/joulescope_ui/resources/logo-small.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/resources/zoom.svg` & `joulescope_ui-1.1.7/joulescope_ui/resources/zoom.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/resources.py` & `joulescope_ui-1.1.7/joulescope_ui/resources.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/resources.rcc` & `joulescope_ui-1.1.7/joulescope_ui/resources.rcc`

 * *Files 2% similar despite different names*

```diff
@@ -1416,11 +1416,11 @@
 00005870: 5f00 3600 3400 7800 3600 3400 2e00 6900  _.6.4.x.6.4...i.
 00005880: 6300 6f00 0e03 14ce 8700 6c00 6f00 6700  c.o.......l.o.g.
 00005890: 6f00 2d00 6c00 6100 7200 6700 6500 2e00  o.-.l.a.r.g.e...
 000058a0: 7000 6e00 6700 0e0f ebc7 e700 6c00 6f00  p.n.g.......l.o.
 000058b0: 6700 6f00 2d00 7300 6d00 6100 6c00 6c00  g.o.-.s.m.a.l.l.
 000058c0: 2e00 7000 6e00 6700 0000 0000 0200 0000  ..p.n.g.........
 000058d0: 0300 0000 0100 0000 0000 0000 0000 0000  ................
-000058e0: 2200 0000 0000 0100 0001 9900 0001 8f1a  "...............
-000058f0: b310 6c00 0000 0000 0400 0000 0100 0000  ..l.............
-00005900: 0000 0001 8f1a b310 6c00 0000 4400 0000  ........l...D...
-00005910: 0000 0100 0043 f800 0001 8f1a b310 6c    .....C........l
+000058e0: 2200 0000 0000 0100 0001 9900 0001 8f68  "..............h
+000058f0: 00b7 6600 0000 0000 0400 0000 0100 0000  ..f.............
+00005900: 0000 0001 8f68 00b7 6600 0000 4400 0000  .....h..f...D...
+00005910: 0000 0100 0043 f800 0001 8f68 00b7 66    .....C.....h..f
```

### Comparing `joulescope_ui-1.1.6/joulescope_ui/safe_mode.py` & `joulescope_ui-1.1.7/joulescope_ui/safe_mode.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/sanitize.py` & `joulescope_ui-1.1.7/joulescope_ui/sanitize.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/shift_key.py` & `joulescope_ui-1.1.7/joulescope_ui/shift_key.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/software_update.py` & `joulescope_ui-1.1.7/joulescope_ui/software_update.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/source_selector.py` & `joulescope_ui-1.1.7/joulescope_ui/source_selector.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/styles/README.md` & `joulescope_ui-1.1.7/joulescope_ui/styles/README.md`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/styles/__init__.py` & `joulescope_ui-1.1.7/joulescope_ui/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/styles/color_editor.py` & `joulescope_ui-1.1.7/joulescope_ui/styles/color_editor.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/styles/color_file.py` & `joulescope_ui-1.1.7/joulescope_ui/styles/color_file.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/styles/color_picker.py` & `joulescope_ui-1.1.7/joulescope_ui/styles/color_picker.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/styles/color_scheme.py` & `joulescope_ui-1.1.7/joulescope_ui/styles/color_scheme.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/styles/color_scheme_dark.txt` & `joulescope_ui-1.1.7/joulescope_ui/styles/color_scheme_dark.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/styles/color_scheme_light.txt` & `joulescope_ui-1.1.7/joulescope_ui/styles/color_scheme_light.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/styles/font_scheme.py` & `joulescope_ui-1.1.7/joulescope_ui/styles/font_scheme.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/styles/fonts.py` & `joulescope_ui-1.1.7/joulescope_ui/styles/fonts.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/styles/js1/detach.svg` & `joulescope_ui-1.1.7/joulescope_ui/styles/js1/detach.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/styles/js1/index.json` & `joulescope_ui-1.1.7/joulescope_ui/styles/js1/index.json`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/styles/js1/style.qss` & `joulescope_ui-1.1.7/joulescope_ui/styles/js1/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/styles/js1/vmovetoolbar.svg` & `joulescope_ui-1.1.7/joulescope_ui/styles/js1/vmovetoolbar.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/styles/js1/vsepartoolbars.svg` & `joulescope_ui-1.1.7/joulescope_ui/styles/js1/vsepartoolbars.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/styles/manager.py` & `joulescope_ui-1.1.7/joulescope_ui/styles/manager.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/styles/parameter_file.py` & `joulescope_ui-1.1.7/joulescope_ui/styles/parameter_file.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/styles/system/style.qss` & `joulescope_ui-1.1.7/joulescope_ui/styles/system/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/styles/system/zoom_all.svg` & `joulescope_ui-1.1.7/joulescope_ui/styles/system/zoom_all.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/styles/test/test_color_file.py` & `joulescope_ui-1.1.7/joulescope_ui/styles/test/test_color_file.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/styles/test/test_manager.py` & `joulescope_ui-1.1.7/joulescope_ui/styles/test/test_manager.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/styles/test/test_parameter_file.py` & `joulescope_ui-1.1.7/joulescope_ui/styles/test/test_parameter_file.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/test/anno1.anno.jls` & `joulescope_ui-1.1.7/joulescope_ui/test/anno1.anno.jls`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/test/test_annotation_load.py` & `joulescope_ui-1.1.7/joulescope_ui/test/test_annotation_load.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/test/test_capabilities.py` & `joulescope_ui-1.1.7/joulescope_ui/test/test_capabilities.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/test/test_disk_monitor.py` & `joulescope_ui-1.1.7/joulescope_ui/test/test_disk_monitor.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/test/test_metadata.py` & `joulescope_ui-1.1.7/joulescope_ui/test/test_metadata.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/test/test_pubsub.py` & `joulescope_ui-1.1.7/joulescope_ui/test/test_pubsub.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/test/test_pubsub_aggregator.py` & `joulescope_ui-1.1.7/joulescope_ui/test/test_pubsub_aggregator.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/test/test_pubsub_registry.py` & `joulescope_ui-1.1.7/joulescope_ui/test/test_pubsub_registry.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/test/test_range_tool.py` & `joulescope_ui-1.1.7/joulescope_ui/test/test_range_tool.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/test/test_reporter.py` & `joulescope_ui-1.1.7/joulescope_ui/test/test_reporter.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/test/test_sanitize.py` & `joulescope_ui-1.1.7/joulescope_ui/test/test_sanitize.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/test/test_software_update.py` & `joulescope_ui-1.1.7/joulescope_ui/test/test_software_update.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/test/test_source_selector.py` & `joulescope_ui-1.1.7/joulescope_ui/test/test_source_selector.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/test/test_time_map.py` & `joulescope_ui-1.1.7/joulescope_ui/test/test_time_map.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/test/test_tooltip.py` & `joulescope_ui-1.1.7/joulescope_ui/test/test_tooltip.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/test/test_units.py` & `joulescope_ui-1.1.7/joulescope_ui/test/test_units.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/test/test_versioned_file.py` & `joulescope_ui-1.1.7/joulescope_ui/test/test_versioned_file.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/time_map.py` & `joulescope_ui-1.1.7/joulescope_ui/time_map.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/tokens.py` & `joulescope_ui-1.1.7/joulescope_ui/tokens.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/tooltip.py` & `joulescope_ui-1.1.7/joulescope_ui/tooltip.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/ui_util.py` & `joulescope_ui-1.1.7/joulescope_ui/ui_util.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/units.py` & `joulescope_ui-1.1.7/joulescope_ui/units.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/urls.py` & `joulescope_ui-1.1.7/joulescope_ui/urls.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/versioned_file.py` & `joulescope_ui-1.1.7/joulescope_ui/versioned_file.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/view.py` & `joulescope_ui-1.1.7/joulescope_ui/view.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 
 from . import pubsub_singleton, register, N_, sanitize, \
     get_topic_name, get_unique_id, get_instance
 from joulescope_ui.pubsub import pubsub_attr
 from .styles.manager import style_settings
-from PySide6 import QtCore, QtWidgets
+from PySide6 import QtCore, QtGui, QtWidgets
 import PySide6QtAds as QtAds
 import logging
 import weakref
 
 
 _log = logging.getLogger(__name__)
 
@@ -45,14 +45,18 @@
             QtAds.CDockWidget.DockWidgetForceCloseWithArea |
             0)
         self.closeRequested.connect(self._on_close_request)
 
     def _on_setting_name(self, value):
         self.setWindowTitle(value)
 
+    def keyPressEvent(self, event: QtGui.QKeyEvent):
+        # unhandled by widget.  Send to global key press processor.
+        pubsub_singleton.publish('registry/ui/actions/!key_press', event)
+
     @QtCore.Slot()
     def _on_close_request(self):
         widget = self.widget()
         _log.info('close %s', get_unique_id(widget))
         pubsub_singleton.publish('registry/view/actions/!widget_close', get_topic_name(widget))
 
 
@@ -214,15 +218,16 @@
         if isinstance(spec, type):
             obj = spec(*args, **kwargs)
         else:
             obj = spec
         if obj is None:
             _log.warning('Could not open %s', spec)
             return
-        pubsub_singleton.register(obj, unique_id=unique_id, parent=self)
+        if not pubsub_singleton.register(obj, unique_id=unique_id, parent=self):
+            return None
         unique_id = obj.unique_id
         obj.setObjectName(unique_id)
         obj.destroyed.connect(self._on_destroyed)
         dock_widget = DockWidget(obj)
         dock_widget.destroyed.connect(self._on_destroyed)
         pubsub_attr(obj)['dock_widget'] = weakref.ref(dock_widget)
         tab_widget = dock_widget.tabWidget()
```

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widget_tools.py` & `joulescope_ui-1.1.7/joulescope_ui/widget_tools.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/__init__.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/accumulator/__init__.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/accumulator/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/accumulator/accumulator_widget.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/accumulator/accumulator_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/accumulator/styles/style.qss` & `joulescope_ui-1.1.7/joulescope_ui/widgets/accumulator/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/clock/__init__.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/clock/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/clock/clock_widget.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/clock/clock_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/developer/__init__.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/developer/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/developer/log_view_widget.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/developer/log_view_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/developer/profile_widget.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/developer/profile_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/developer/publish_spy_widget.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/developer/publish_spy_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/developer/pubsub_explorer_widget.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/developer/pubsub_explorer_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/device_control/__init__.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/device_control/current_limits.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/current_limits.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/device_control/device_control_widget.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/device_control_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/device_control/device_info_dialog.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/device_info_dialog.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/device_control/device_update_dialog.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/device_update_dialog.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/device_control/fuse.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/fuse.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/device_control/js220_ctrl_widget.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/js220_ctrl_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/device_control/styles/device_open.svg` & `joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/device_open.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/device_control/styles/fuse_engaged.svg` & `joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/fuse_engaged.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/device_control/styles/fuse_normal.svg` & `joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/fuse_normal.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/device_control/styles/index.json` & `joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/index.json`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/device_control/styles/info.svg` & `joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/info.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/device_control/styles/style.qss` & `joulescope_ui-1.1.7/joulescope_ui/widgets/device_control/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/double_slider.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/double_slider.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/draggable_list_widget.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/draggable_list_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/example/__init__.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/example/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/example/example_widget.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/example/example_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/flyout/__init__.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/flyout/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/flyout/flyout_widget.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/flyout/flyout_widget.py`

 * *Files 26% similar despite different names*

```diff
@@ -22,35 +22,43 @@
 _ANIMATION_DURATION_MS = 500
 
 
 @register
 @styled_widget(N_('flyout'))
 class FlyoutWidget(QtWidgets.QScrollArea):
 
+    width_changed = QtCore.Signal(int)
+
     def __init__(self, parent, sidebar):
         self._sidebar = sidebar
         super().__init__(parent)
         self._log = logging.getLogger(__name__)
         self.setObjectName('flyout1')
         self.setGeometry(50, 0, 0, 100)  # unused, see on_sidebar_geometry() and sidebar setting "flyout_width"
         self.setWidgetResizable(True)
         self.setHorizontalScrollBarPolicy(QtGui.Qt.ScrollBarPolicy.ScrollBarAlwaysOff)
+        self._resize_active = None
         self.show()
         self.animations = []
+        self._CURSOR_ARROW = QtGui.QCursor(QtGui.Qt.ArrowCursor)
+        self._CURSOR_SIZE_HOR = QtGui.QCursor(QtGui.Qt.SizeHorCursor)
+        self.setMouseTracking(True)
 
     def flyout_widget_set(self, widget, width=0):
         for a in self.animations:
             a.stop()
         self.animations.clear()
         if widget is not None:
             w = self.takeWidget()
             if w is not None:
                 w.hide()
+                w.setMouseTracking(False)
             self.setWidget(widget)
             widget.show()
+            widget.setMouseTracking(True)
 
         x_start = self.width()
         x_end = width
         self._log.info(f'animate: {x_start} -> {x_end}')
         for p in [b'minimumWidth', b'maximumWidth']:
             a = QtCore.QPropertyAnimation(self, p)
             a.setDuration(_ANIMATION_DURATION_MS)
@@ -63,22 +71,52 @@
 
     @QtCore.Slot()
     def _on_animation_finished(self):
         if self.width() == 0:
             w = self.takeWidget()
             if w is not None:
                 w.hide()
+        for a in self.animations:
+            a.stop()
         self.animations.clear()
 
     def on_sidebar_geometry(self, r):
         width = self.width()
         self.setGeometry(r.right() + 3, r.y(), width, r.height())
-        self.repaint()
+        self.update()
 
     def leaveEvent(self, event: QtCore.QEvent):
         if self.width() == 0:
             return
         pos = self.mapFromGlobal(QtGui.QCursor.pos())
         if (pos.x() + 1) >= self.width():
             if len(self.animations) == 0 or self.animations[-1].endValue() != 0:
                 self._sidebar.on_cmd_show(None)
         return super().leaveEvent(event)
+
+    def mouseMoveEvent(self, event: QtGui.QMouseEvent):
+        if self.width() == 0:
+            return
+        x = event.position().x()
+        if self._resize_active is not None:
+            w = max(100, x - self._resize_active)
+            self.setMinimumWidth(w)
+            self.setMaximumWidth(w)
+            self.update()
+        elif x >= (self.width() - 5):
+            self.setCursor(self._CURSOR_SIZE_HOR)
+        else:
+            self.setCursor(self._CURSOR_ARROW)
+        event.accept()
+
+    def mousePressEvent(self, event):
+        if self.width() == 0:
+            return
+        x = event.position().x()
+        if x >= (self.width() - 5):
+            self._resize_active = x - self.width()
+        return super().mousePressEvent(event)
+
+    def mouseReleaseEvent(self, event):
+        if self._resize_active is not None:
+            self.width_changed.emit(self.width())
+            self._resize_active = None
```

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/flyout/styles/style.qss` & `joulescope_ui-1.1.7/joulescope_ui/widgets/flyout/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/hamburger/__init__.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/hamburger/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/hamburger/hamburger_widget.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/hamburger/hamburger_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/help/__init__.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/help/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/help/help_widget.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/help/help_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/jls_info/__init__.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/jls_info/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/jls_info/jls_info_widget.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/jls_info/jls_info_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/js220_cal/__init__.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/js220_cal/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/js220_cal/current_offset.png` & `joulescope_ui-1.1.7/joulescope_ui/widgets/js220_cal/current_offset.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/js220_cal/js220_cal_widget.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/js220_cal/js220_cal_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/js220_cal/voltage_offset.png` & `joulescope_ui-1.1.7/joulescope_ui/widgets/js220_cal/voltage_offset.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/memory/__init__.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/memory/memory_widget.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/memory/memory_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/memory/styles/style.qss` & `joulescope_ui-1.1.7/joulescope_ui/widgets/memory/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/notes/__init__.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/notes/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/notes/notes_widget.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/notes/notes_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/progress_bar/__init__.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/progress_bar/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/progress_bar/progress_bar_widget.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/progress_bar/progress_bar_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/record_status/__init__.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/record_status/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/record_status/record_status_widget.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/record_status/record_status_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/record_status/styles/index.json` & `joulescope_ui-1.1.7/joulescope_ui/widgets/record_status/styles/index.json`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/record_status/styles/style.qss` & `joulescope_ui-1.1.7/joulescope_ui/widgets/record_status/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/report_issue/__init__.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/report_issue/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/report_issue/report_issue_dialog.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/report_issue/report_issue_dialog.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/settings/__init__.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/settings/settings_widget.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/settings/settings_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -624,13 +624,11 @@
         for c in [REGISTRY_MANAGER_TOPICS.REGISTRY_ADD, REGISTRY_MANAGER_TOPICS.REGISTRY_REMOVE]:
             self.pubsub.subscribe(c, self._on_populate, ['pub'])
 
     @staticmethod
     def on_cls_action_edit(pubsub, topic, value):
         w = SettingsWidget()
         w.view_skip_undo = True
-        active_view = pubsub.query('registry/view/settings/active')
-        pubsub.register(w, parent=active_view)
         pubsub.publish('registry/view/actions/!widget_open',
                        {'value': w, 'floating': True})
         pubsub.publish(f'{get_topic_name(w)}/settings/target',
                        get_unique_id(value))
```

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/settings/unique_strings_widget.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/settings/unique_strings_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/sidebar/__init__.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/sidebar/sidebar_widget.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/sidebar_widget.py`

 * *Files 13% similar despite different names*

```diff
@@ -59,18 +59,21 @@
 @register
 @styled_widget(N_('sidebar'))
 class SideBar(QtWidgets.QWidget):
 
     # Note: does NOT implement widget CAPABILITY, since not instantiable by user or available as a dock widget.
 
     SETTINGS = {
-        'flyout_width': {
-            'dtype': 'int',
-            'brief': N_('The flyout width in pixels.'),
-            'default': 300,
+        'flyout_widths': {
+            'dtype': 'obj',
+            'brief': 'The flyout width for each widget in pixels.',
+            'default': {
+                'settings': 500,
+                '__default__': 300,
+            },
         },
     }
 
     def __init__(self, parent):
         super().__init__(parent)
         self.setObjectName('side_bar_icons')
         size_policy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
@@ -78,14 +81,15 @@
         self.setSizePolicy(size_policy)
         self._style_cache = None
         self._selected_area = None
         self._selected_area_brush = QtGui.QBrush
         self._buttons = {}
         self._buttons_blink = {}
         self._flyout: FlyoutWidget = None
+        self._flyout_active_name = None
 
         self._layout = QtWidgets.QVBoxLayout(self)
         self._layout.setSpacing(6)
         self._layout.setContentsMargins(3, 3, 3, 3)
 
     def _on_fuse_button_pressed(self):
         self.pubsub.publish('registry/app/actions/!fuse_clear_all', None)
@@ -98,25 +102,26 @@
         b.pressed.connect(self._on_fuse_button_pressed)
         self._add_blink_button('signal_play', 'signal_stream_enable')
         self._add_blink_button('signal_record', 'signal_stream_record')
         self._add_blink_button('statistics_play', 'statistics_stream_enable')
         self._add_blink_button('statistics_record', 'statistics_stream_record')
         self._add_button('device', _DEVICE_TOOLTIP, 'DeviceControlWidget', 'device_control_widget:flyout')
         self._add_button('memory', _MEMORY_TOOLTIP, 'MemoryWidget', 'memory_widget:flyout')
-        self._add_button('settings', _SETTINGS_TOOLTIP, 'settings', 'settings:flyout', width=500)
+        self._add_button('settings', _SETTINGS_TOOLTIP, 'settings', 'settings:flyout')
         self._spacer = QtWidgets.QSpacerItem(10, 0,
                                              QtWidgets.QSizePolicy.Minimum,
                                              QtWidgets.QSizePolicy.Expanding)
         self._layout.addItem(self._spacer)
         self._add_button('help', _HELP_TOOLTIP, 'HelpWidget', 'help_widget:flyout')
         self._add_button('misc', _MISC_TOOLTIP, 'HamburgerWidget', 'hamburger_widget:flyout')
 
         self.pubsub.subscribe('registry/ui/events/blink_slow', self._on_blink, ['pub', 'retain'])
         self.pubsub.subscribe(_STATISTIC_STREAM_SOURCE_TOPIC, self._on_statistics_stream_source_list, ['pub', 'retain'])
         self.pubsub.subscribe(_SIGNAL_STREAM_SOURCE_TOPIC, self._on_signal_stream_source_list, ['pub', 'retain'])
+        self._flyout.width_changed.connect(self.on_flyout_width_changed)
 
     def mousePressEvent(self, event):
         if event.button() == QtCore.Qt.LeftButton:
             self.on_cmd_show(None)
             event.accept()
 
     def _on_settings_pressed(self, checked):
@@ -158,26 +163,25 @@
 
         self.pubsub.subscribe(topic, update_from_pubsub, ['pub', 'retain'])
         if not bool(skip_connect):
             adapter = CallableSlotAdapter(button, lambda checked: self.pubsub.publish(topic, bool(checked)))
             button.toggled.connect(adapter.slot)
         return button
 
-    def _add_button(self, name, tooltip, clz=None, unique_id=None, width=None):
+    def _add_button(self, name, tooltip, clz=None, unique_id=None):
         button = QtWidgets.QPushButton(self)
         button.setObjectName(name)
         button.setFlat(True)
         button.setFixedSize(32, 32)
         button.setToolTip(tooltip)
         self._buttons[name] = {
             'name': name,
             'button': button,
             'class': clz,
             'unique_id': unique_id,
-            'width': 300 if width is None else int(width),
         }
         if clz is not None:
             button.setProperty('selected', False)
             adapter = CallableSlotAdapter(button, lambda: self.on_cmd_show(name))
             button.clicked.connect(adapter.slot)
         self._layout.addWidget(button)
         return button
@@ -188,29 +192,42 @@
             if disabling:
                 b.setProperty('disabling', False)
             if b.isEnabled() or disabling:
                 b.setProperty('blink', value and not disabling)
                 b.style().unpolish(b)
                 b.style().polish(b)
 
+    @QtCore.Slot(int)
+    def on_flyout_width_changed(self, width: int):
+        if self._flyout_active_name is None:
+            return
+        name = self._flyout_active_name
+        if name not in self.flyout_widths:
+            name = '__default__'
+        self.flyout_widths[name] = width
+
     def on_cmd_show(self, name):
         w = self._buttons.get(name, {}).get('widget')
         if name is None or (w is not None and w == self._flyout.widget()):
+            self._flyout_active_name = None
             self._flyout.flyout_widget_set(None)
             self._selected_area = None
         else:
+            self._flyout_active_name = name
             v = self._buttons[name]
             if v.get('widget') is None:
                 clz = get_instance(v['class'])
                 w = clz(parent=self._flyout)
                 w.setContentsMargins(5, 5, 5, 5)
                 self.pubsub.register(w, v['unique_id'], parent='flyout:0')
                 v['widget'] = w
                 self.pubsub.publish(f'registry/style/actions/!render', w)
-            self._flyout.flyout_widget_set(v['widget'], v['width'])
+            width = self.flyout_widths.get('__default__', 300)
+            width = self.flyout_widths.get(self._flyout_active_name, width)
+            self._flyout.flyout_widget_set(v['widget'], width)
             self._selected_area = v['button'].geometry()
         self.update()
 
     def paintEvent(self, event):
         s = self._style
         if s is None:
             return
```

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/sidebar/styles/color_scheme_dark.txt` & `joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/color_scheme_dark.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/sidebar/styles/color_scheme_light.txt` & `joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/color_scheme_light.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/sidebar/styles/fuse_engaged.svg` & `joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/fuse_engaged.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/sidebar/styles/fuse_normal.svg` & `joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/fuse_normal.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/sidebar/styles/index.json` & `joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/index.json`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/sidebar/styles/style.qss` & `joulescope_ui-1.1.7/joulescope_ui/widgets/sidebar/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/signal_record/__init__.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/signal_record/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/signal_record/disk_full_dialog.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/signal_record/disk_full_dialog.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/signal_record/signal_record.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/signal_record/signal_record.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/signal_record/signal_record_config_widget.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/signal_record/signal_record_config_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/statistics_record/__init__.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/statistics_record/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/statistics_record/statistics_record.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/statistics_record/statistics_record.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/statistics_record/statistics_record_config_widget.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/statistics_record/statistics_record_config_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/switch.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/switch.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/trigger/__init__.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/trigger/condition_detector.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/condition_detector.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/trigger/styles/continuous.svg` & `joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/styles/continuous.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/trigger/styles/index.json` & `joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/styles/index.json`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/trigger/styles/searching.svg` & `joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/styles/searching.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/trigger/styles/style.qss` & `joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/trigger/test/test_const.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/test/test_const.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/trigger/test/test_duration.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/test/test_duration.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/trigger/test/test_edge.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/test/test_edge.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/trigger/trigger_widget.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/trigger/trigger_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/value/__init__.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/value/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/value/value_widget.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/value/value_widget.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from PySide6 import QtWidgets, QtGui, QtCore
 from joulescope_ui import CAPABILITIES, register, N_, P_, get_topic_name, tooltip_format
 from joulescope_ui.widget_tools import settings_action_create, context_menu_show
 from joulescope_ui.styles import styled_widget, color_as_qcolor, font_as_qfont
-from joulescope_ui.units import UNITS_SETTING, convert_units, unit_prefix, three_sig_figs
+from joulescope_ui.units import RE_IS_NUMBER, UNITS_SETTING, convert_units, unit_prefix, three_sig_figs
 from joulescope_ui.ui_util import comboBoxConfig, comboBoxSelectItemByText
 from joulescope_ui.source_selector import SourceSelector
 import datetime
 import numpy as np
 import copy
 import logging
 
@@ -53,14 +53,21 @@
     },
     'show_titles': {
         'dtype': 'bool',
         'brief': N_('Show the statistics section title for each signal.'),
         'default': True,
     },
     'units': UNITS_SETTING,
+    'divisor': {
+        'dtype': 'str',
+        'brief': N_('Divide the quantity by this value.'),
+        'detail': N_('The divisor is a floating point number. '
+                     + 'The number may optionally be followed by units.'),
+        'default': '',
+    },
 }
 
 
 def _settings_alter(**kwargs):
     d = copy.deepcopy(SETTINGS)
     for key, default in kwargs.items():
         d[key]['default'] = default
@@ -111,14 +118,15 @@
         this button to accrue the values indefinitely.
         Press again to return to normal operation."""),
         N_("""Note that this button does not affect the charge and energy
         accumulation.  Both accumulate indefinitely regardless of
         this button state.""")
     ]))
 
+
 def duration_to_str(value):
     if value > 60:
         h = int(value // 3600)
         value -= h * 3600
         m = int(value // 60)
         value -= m * 60
         s = int(value // 1)
@@ -294,50 +302,87 @@
     def paintEvent(self, event):
         fields = [field for field in self._fields if field != self._main]
         parent: ValueWidget = self.parent()
         resolved = parent.source_selector.resolved()
         if resolved is None or parent.style_obj is None:
             return
 
+        self._geometry = {}
         painter = QtGui.QPainter(self)
         v = parent.style_obj['vars']
         x_border, y_border = 10, 10
         y_sep = 6
         number_example = '8.88888'
 
+        divisor_str = parent.divisor
+        divisor = 1.0
+        divisor_units = ''
+        if divisor_str is not None:
+            match = RE_IS_NUMBER.match(divisor_str)
+            if match:
+                divisor = float(match.group(1))
+                divisor_units = match.group(2).strip()
+                if divisor_units:
+                    divisor_units = f'/{divisor_units}'
+
         background_color = color_as_qcolor(v['value.background'])
         background_brush = QtGui.QBrush(background_color)
 
         title_color = color_as_qcolor(v['value.title_color'])
         title_font = font_as_qfont(v['value.title_font'])
         title_font_metrics = QtGui.QFontMetrics(title_font)
         title_space = np.ceil(title_font_metrics.ascent() * 0.05)
         title_height = title_font_metrics.height() + title_space if parent.show_titles else 0
 
         main_color = color_as_qcolor(v['value.main_color'])
         main_font = font_as_qfont(v['value.main_font'])
         main_font_metrics = QtGui.QFontMetrics(main_font)
         main_number_width = main_font_metrics.boundingRect(number_example).width()
-        main_char_width = _width(main_font_metrics)
-        main_text_width = main_font_metrics.boundingRect('W').width()
+        main_num_char_width = _width(main_font_metrics)
+        main_txt_char_width = main_font_metrics.boundingRect('W').width()
+        main_units_width = main_font_metrics.boundingRect('W').width()
+        main_divisor_width = main_font_metrics.boundingRect(divisor_units).width()
 
         stats_color = color_as_qcolor(v['value.stats_color'])
         stats_font = font_as_qfont(v['value.stats_font'])
         stats_font_metrics = QtGui.QFontMetrics(stats_font)
         stats_number_width = stats_font_metrics.boundingRect(number_example).width()
         stats_char_width = _width(stats_font_metrics)
         stats_field_width_max = max([stats_font_metrics.boundingRect(field).width() for field in self._fields])
         stats_space = np.ceil(stats_font_metrics.ascent() * 0.05)
 
         line_color = color_as_qcolor(v['value.line_color'])
 
-        x_max = x_border + main_char_width + main_number_width + main_char_width // 2 + main_text_width * 2 + x_border
+        x_width = [
+            ('margin.left', x_border),
+            ('main.sign', main_num_char_width),
+            ('main.number', main_number_width),
+            ('main.sep1', main_num_char_width // 2),
+            ('main.prefix', main_txt_char_width),
+            ('main.units', main_units_width),
+            ('main.divisor', main_divisor_width),
+        ]
         if parent.show_fields and len(fields):
-            x_max += (main_text_width // 2 + stats_char_width + stats_number_width +
-                      stats_char_width + stats_field_width_max)
+            x_width.extend([
+                ('stats.sep0', main_txt_char_width // 2),
+                ('stats.sign', stats_char_width),
+                ('stats.number', stats_number_width),
+                ('stats.sep1', stats_char_width),
+                ('stats.text', stats_field_width_max),
+            ])
+        x_width.append(('margin.right', x_border))
+        x_pos_list = []
+        x_pos_dict = {}
+        x1 = 0
+        for x_loc, x_w in x_width:
+            x0, x1 = x1, int(x1 + x_w)
+            x_pos_list.append((x_loc, x0, x1))
+            x_pos_dict[x_loc] = (x0, x1)
+        x_max = x_pos_list[-1][-1]
+
         field_count = len(fields) if parent.show_fields else 0
         y1 = title_height + main_font_metrics.height()
         y2 = stats_font_metrics.height() * field_count
         if field_count > 1:
             y2 += (field_count - 1) * stats_space
         y_signal = max(y1, y2)
         signal_len = len(self._signals)
@@ -357,33 +402,22 @@
             a_start, a_end = self._statistics['time']['accum_samples']['value']
             sample_freq = self._statistics['time']['sample_freq']['value']
             a_duration = (a_end - a_start) / sample_freq
             a_duration_txt = duration_to_str(a_duration)
 
         painter.fillRect(0, 0, x_max, y_max, background_brush)
 
-        self._geometry = {
-            'y_border': y_border,
-            'y_signal': y_signal,
-            'y_sep': y_sep,
-            'y_stats_space': stats_space,
-            'y_stats': stats_font_metrics.height(),
-            'x_stats': None,
-            'fields': {},  # signal_idx -> list of available fields
-            'values': {},  # signal_idx -> field_name -> value
-        }
-
         for idx, signal_name in enumerate(self._signals):
             y = y_border + idx * (y_signal + y_sep)
             if idx != 0:
                 y_line = y - y_sep // 2
                 painter.setPen(line_color)
                 painter.drawLine(x_border, y_line, x_max - x_border, y_line)
             y_start = y
-            x = x_border
+            x = x_pos_dict['margin.left'][1]
 
             if parent.show_titles:
                 painter.setPen(title_color)
                 painter.setFont(title_font)
                 y += title_font_metrics.ascent()
                 signal_title_parts = [resolved, signal_name]
                 if self._statistics is not None:
@@ -398,127 +432,100 @@
             painter.setPen(main_color)
             painter.setFont(main_font)
             y += main_font_metrics.ascent() + (y_signal - title_height - main_font_metrics.height()) // 2
 
             if signal_name in self._statistics['accumulators']:
                 signal = self._statistics['accumulators'][signal_name]
                 fields = ['accumulate_duration']
-                signal_value, signal_units = convert_units(signal['value'], signal['units'], parent.units)
+                signal_value, signal_units = convert_units(signal['value'] / divisor, signal['units'], parent.units)
                 _, prefix, scale = unit_prefix(signal_value)
+                scale *= divisor
             else:
                 signal = self._statistics['signals'][signal_name]
                 fields = fields if parent.show_fields else []
                 fields_all = [self._main] + fields
                 max_value = max([abs(signal[s]['value']) for s in fields_all])
-                _, prefix, scale = unit_prefix(max_value)
+                _, prefix, scale = unit_prefix(max_value / divisor)
                 signal_value = signal[self._main]['value']
                 signal_units = signal[self._main]['units']
+                scale *= divisor
             if len(prefix) != 1:
                 prefix = ' '
             v_str = ('%+6f' % (signal_value / scale))[:8]
             v_str_idx = 1
             if v_str[0] == '-' or parent.show_sign:
                 painter.drawText(x, y, v_str[0])
                 v_str_idx = 0
-            x += main_char_width
-            painter.drawText(x, y, v_str[1:])
-            x += main_number_width + main_char_width // 2
-            w1 = main_font_metrics.boundingRect(signal_units).width()
-            w2 = main_font_metrics.boundingRect(prefix + signal_units).width()
-            x_offset = int(main_text_width * 1.5 - w1 / 2)
-            painter.drawText(x + x_offset - (w2 - w1), y, prefix)
-            painter.drawText(x + x_offset, y, signal_units)
-            x += 2 * main_text_width
-            self._geometry['values'][idx] = {'avg': f'{v_str[v_str_idx:]} {prefix}{signal_units}'}
+            painter.drawText(x_pos_dict['main.number'][0], y, v_str[1:])
+            x0, x1 = x_pos_dict['main.units']
+            xk = x0 + ((x1 - x0) - main_font_metrics.boundingRect(signal_units).width()) // 2
+            painter.drawText(xk - main_font_metrics.horizontalAdvance(prefix), y, prefix)
+            painter.drawText(xk, y, f'{signal_units}')
+            if divisor_units:
+                painter.drawText(x_pos_dict['main.divisor'][0], y, divisor_units)
+            units = f'{prefix}{signal_units}{divisor_units}'
+            p0 = x_pos_dict['main.sign'][0], y_start
+            p1 = x_pos_dict['main.divisor'][1], y
+            self._geometry[(signal_name, 'avg')] = (p0, p1, f'{v_str[v_str_idx:]} {units}')
 
             painter.setPen(stats_color)
             painter.setFont(stats_font)
             y = y_start + (y_signal - y2) // 2
-            x += main_text_width // 2
-            x_start = x
-            self._geometry['fields'][idx] = fields
 
             for field_idx, stat in enumerate(fields):
+                y0 = y
                 if field_idx == 0:
                     y += stats_space
                 y += stats_font_metrics.ascent()
-                x = x_start
-                self._geometry['x_stats'] = x
+                x0 = x_pos_dict['stats.sign'][0]
+                x1 = x_pos_dict['stats.number'][0]
+                x2, x3 = x_pos_dict['stats.text']
                 if stat == 'accumulate_duration':
-                    painter.drawText(x, y, a_duration_txt)
+                    painter.drawText(x0, y, a_duration_txt)
+                    self._geometry[(signal_name, 'duration')] = ((x0, y0), (x3, y), a_duration_txt)
                 else:
                     v_str = ('%+6f' % (signal[stat]['value'] / scale))[:8]
                     v_str_idx = 1
                     if v_str[0] == '-' or parent.show_sign:
-                        painter.drawText(x, y, v_str[0])
+                        painter.drawText(x0, y, v_str[0])
                         v_str_idx = 0
                     x += stats_char_width
-                    painter.drawText(x, y, v_str[1:])
+                    painter.drawText(x1, y, v_str[1:])
                     x += stats_number_width + stats_char_width
-                    painter.drawText(x, y, stat)
-                    self._geometry['values'][idx][stat] = f'{v_str[v_str_idx:]} {prefix}{signal_units}'
+                    painter.drawText(x2, y, stat)
+                    self._geometry[(signal_name, stat)] = ((x0, y0), (x3, y), f'{v_str[v_str_idx:]} {units} {stat}')
                 y += stats_font_metrics.descent()
 
         #color = color_as_qcolor('#ff000040')
         #painter.setPen(color)
         #painter.drawRect(x_border, y_border, x_max - x_border, y - y_border)
         painter.end()
 
-    def _pos_to_item(self, x, y):
+    def _pos_to_str(self, x, y):
         if self._geometry is None:
             return None
-        if y < self._geometry['y_border']:
-            return None
-        y -= self._geometry['y_border']
-        y_signal = self._geometry['y_signal']
-        y_sep = self._geometry['y_sep']
-        y_height = y_signal + y_sep
-        idx = int(y // y_height)
-        if idx >= len(self._signals):
-            return None
-        z = y - idx * y_height
-        if z > y_signal:  # in separator
-            return None
-        x_stats = self._geometry.get('x_stats')
-        result = {
-            'signal_idx': idx,
-        }
-        if x_stats is not None and x >= x_stats:
-            fields = self._geometry['fields'][idx]
-            y_stats_space = self._geometry['y_stats_space']
-            y_stats = self._geometry['y_stats']
-            if z < y_stats_space:
-                return None
-            k = int(z // y_stats)
-            if k >= len(fields):
-                return None
-            result['field'] = fields[k]
-        else:
-            result['field'] = 'avg'
-        return result
+        for p0, p1, s in self._geometry.values():
+            if p0[0] <= x < p1[0] and p0[1] <= y < p1[1]:
+                return s
+        return None
 
     def mouseMoveEvent(self, event: QtGui.QMouseEvent):
         event.accept()
 
     def mousePressEvent(self, event):
         if event.button() != QtCore.Qt.LeftButton:
             return super().mousePressEvent(event)
         if self._geometry is None:
             return
         x, y = event.position().x(), event.position().y()
-        item = self._pos_to_item(x, y)
-        if item is None:
-            return
-        try:
-            value = self._geometry['values'][item['signal_idx']][item['field']]
-        except KeyError:
-            return
-        self._log.info('copy value to clipboard: %s', value)
-        self._clipboard = value
-        QtWidgets.QApplication.clipboard().setText(self._clipboard)
+        s = self._pos_to_str(x, y)
+        if s is not None:
+            self._log.info('copy value to clipboard: %s', s)
+            self._clipboard = s
+            QtWidgets.QApplication.clipboard().setText(self._clipboard)
 
 
 class _BaseWidget(QtWidgets.QWidget):
     CAPABILITIES = ['widget@', CAPABILITIES.STATISTIC_STREAM_SINK]
 
     def __init__(self, parent=None):
         self._log = logging.getLogger(__name__ + '.base')
```

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/view_manager/__init__.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/view_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/view_manager/styles/style.qss` & `joulescope_ui-1.1.7/joulescope_ui/widgets/view_manager/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/view_manager/view_manager_widget.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/view_manager/view_manager_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/__init__.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/annotations.md` & `joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/annotations.md`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/axis_ticks.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/axis_ticks.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/interval_widget.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/interval_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/line_segments.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/line_segments.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/quantities.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/quantities.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/styles/color_scheme_dark.txt` & `joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/color_scheme_dark.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/styles/color_scheme_light.txt` & `joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/color_scheme_light.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/styles/index.json` & `joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/index.json`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/styles/style.qss` & `joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/styles/y_zoom_all.svg` & `joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/y_zoom_all.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/styles/zoom_all.svg` & `joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/styles/zoom_all.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/test/test_axis_ticks.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/test/test_axis_ticks.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/test/test_quantities.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/test/test_quantities.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/text_annotation.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/text_annotation.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/waveform_control.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/waveform_control.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/waveform_source_widget.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/waveform_source_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/waveform_widget.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/waveform_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from PySide6 import QtWidgets, QtGui, QtCore, QtOpenGLWidgets
 from OpenGL import GL as gl
 from joulescope_ui import CAPABILITIES, register, N_, get_topic_name, get_instance, time64
-from joulescope_ui.shortcuts import Shortcuts
 from joulescope_ui.styles import styled_widget, color_as_qcolor, color_as_string, font_as_qfont
 from joulescope_ui.widget_tools import CallableAction, CallableSlotAdapter, settings_action_create, context_menu_show
 from joulescope_ui.exporter import TO_JLS_SIGNAL_NAME
 from .quantities import X_QUANTITY_OPTIONS, PRECISION_OPTIONS, quantities_format
 from .quantities import si_format as quantities_si_format
 from .line_segments import PointsF
 from .text_annotation import TextAnnotationDialog, SHAPES_DEF, Y_POSITION_MODE
@@ -528,14 +527,15 @@
         self._log = logging.getLogger(__name__)
         self._kwargs = kwargs
         self._style_cache = None
         self._summary_data = None
         self._default_source = None
 
         super().__init__(parent)
+        self.setFocusPolicy(QtGui.Qt.FocusPolicy.StrongFocus)
 
         # manage repainting
         self.__repaint_request = False
         self._paint_state = PaintState.IDLE
         self._paint_timer = QtCore.QTimer(self)
         self._paint_timer.setTimerType(QtGui.Qt.PreciseTimer)
         self._paint_timer.setSingleShot(True)
@@ -546,15 +546,15 @@
         self._NO_BRUSH = QtGui.QBrush(QtGui.Qt.NoBrush)  # prevent memory leak
         self._CURSOR_ARROW = QtGui.QCursor(QtGui.Qt.ArrowCursor)
         self._CURSOR_SIZE_VER = QtGui.QCursor(QtGui.Qt.SizeVerCursor)
         self._CURSOR_SIZE_HOR = QtGui.QCursor(QtGui.Qt.SizeHorCursor)
         self._CURSOR_CROSS = QtGui.QCursor(QtGui.Qt.CrossCursor)
 
         self._dialog = None
-        self._shortcuts = Shortcuts(self)
+        self._keymap = {}
         self._x_map = TimeMap()
         self._x_summary_map = TimeMap()
         self._mouse_pos = None
         self._mouse_pos_start = None
         self._wheel_accum_degrees = np.zeros(2, dtype=np.float64)
         self._margin = _MARGIN
 
@@ -764,14 +764,16 @@
             return False
         return True
 
     def on_pubsub_register(self):
         self._trace_widget.on_pubsub_register(self.pubsub)
         source_filter = self._source_filter_set()
         is_device = source_filter in [None, '', 'JsdrvStreamBuffer:001']
+        if not is_device and get_topic_name(source_filter) not in self.pubsub:
+            raise RuntimeError(f'Source not found {source_filter}')
         if self.state is None:
             self.state = copy.deepcopy(_STATE_DEFAULT)
             if not is_device:
                 self.name = self._kwargs.get('name', _NAME)
         if self.annotations is None:
             self.annotations = {
                 'next_id': 0,
@@ -801,44 +803,85 @@
             plot.setdefault('prefix_preferred', 'auto')
             if 'label' not in plot:
                 plot['label'] = '' if ('integral' in plot) else plot['quantity']
         self.pubsub.subscribe('registry_manager/capabilities/signal_buffer.source/list',
                               self._on_source_list, ['pub', 'retain'])
         topic = get_topic_name(self)
         self._control.on_pubsub_register(self.pubsub, topic, source_filter)
-        self._shortcuts_add()
         self.pubsub.subscribe('registry/app/settings/units', self._update_on_publish, ['pub'])
         self.pubsub.subscribe('registry/app/settings/defaults/signal_buffer_source',
                               self._on_default_signal_buffer_source, ['pub', 'retain'])
 
+        NoMod = QtCore.Qt.KeyboardModifier.NoModifier
+        self._keymap = {
+            (QtCore.Qt.Key_Asterisk, NoMod): (f'{self.topic}/actions/!x_zoom_all', None),
+            (QtCore.Qt.Key_Left, NoMod): (f'{self.topic}/actions/!x_pan', -1),
+            (QtCore.Qt.Key_Right, NoMod): (f'{self.topic}/actions/!x_pan', 1),
+            (QtCore.Qt.Key_Up, NoMod): (f'{self.topic}/actions/!x_zoom', [1, None]),
+            (QtCore.Qt.Key_Down, NoMod): (f'{self.topic}/actions/!x_zoom', [-1, None]),
+            (QtCore.Qt.Key_Plus, NoMod): (f'{self.topic}/actions/!x_zoom', [1, None]),
+            (QtCore.Qt.Key_Minus, NoMod): (f'{self.topic}/actions/!x_zoom', [-1, None]),
+            (QtCore.Qt.Key_Delete, NoMod): (f'{self.topic}/actions/!annotations', ['clear_all']),
+            (QtCore.Qt.Key_Backspace, NoMod): (f'{self.topic}/actions/!annotations', ['clear_all']),
+            (QtCore.Qt.Key_A, QtCore.Qt.KeyboardModifier.ControlModifier):
+                (f'{self.topic}/actions/!viewport', ['pinned']),
+            (QtCore.Qt.Key_D, NoMod): (f'{self.topic}/actions/!x_markers', 'add_dual'),
+            (QtCore.Qt.Key_S, NoMod): (f'{self.topic}/actions/!x_markers', 'add_single'),
+            (QtCore.Qt.Key_1, NoMod): (f'{self.topic}/actions/!x_markers', ['select', 0]),
+            (QtCore.Qt.Key_2, NoMod): (f'{self.topic}/actions/!x_markers', ['select', 1]),
+            (QtCore.Qt.Key_3, NoMod): (f'{self.topic}/actions/!x_markers', ['select', 2]),
+            (QtCore.Qt.Key_4, NoMod): (f'{self.topic}/actions/!x_markers', ['select', 3]),
+            (QtCore.Qt.Key_5, NoMod): (f'{self.topic}/actions/!x_markers', ['select', 4]),
+            (QtCore.Qt.Key_6, NoMod): (f'{self.topic}/actions/!x_markers', ['select', 5]),
+            (QtCore.Qt.Key_7, NoMod): (f'{self.topic}/actions/!x_markers', ['select', 6]),
+            (QtCore.Qt.Key_8, NoMod): (f'{self.topic}/actions/!x_markers', ['select', 7]),
+            (QtCore.Qt.Key_9, NoMod): (f'{self.topic}/actions/!x_markers', ['select', 8]),
+            (QtCore.Qt.Key_Space, QtCore.Qt.KeyboardModifier.ShiftModifier):
+                (f'{self.topic}/actions/!viewport', ['toggle']),
+        }
+
         self._repaint_request = True
         self._paint_state = PaintState.READY
         self._paint_timer.start(1)
 
+    def on_action_viewport(self, topic, value):
+        cmd = value[0]
+        t1 = f'{self.topic}/settings/pin_right'
+        t2 = f'{self.topic}/settings/pin_left'
+        v1 = self.pubsub.query(t1)
+        v2 = self.pubsub.query(t2)
+        if cmd == 'toggle':
+            cmd = 'unpinned' if v1 else 'pinned'
+        if cmd == 'pinned':
+            self.pubsub.publish(t1, True)
+            self.pubsub.publish(t2, True)
+        elif cmd == 'unpinned':
+            self.pubsub.publish(t1, False)
+            self.pubsub.publish(t2, False)
+        elif cmd == 'undo':
+            self.pubsub.publish(t1, value[1])
+            self.pubsub.publish(t2, value[2])
+        return topic, ['undo', v1, v2]
+
     def _update_on_publish(self):
         self._repaint_request = True
 
     def _on_default_signal_buffer_source(self, value):
         self._default_source = value
         self._repaint_request = True
 
-    def _shortcuts_add(self):
-        topic = get_topic_name(self)
-        self._shortcuts.add(QtCore.Qt.Key_Asterisk, f'{topic}/actions/!x_zoom_all')
-        # self._shortcuts.add(QtCore.Qt.Key_Delete,  # clear annotations
-        # self._shortcuts.add(QtCore.Qt.Key_Backspace, # clear annotations
-        self._shortcuts.add(QtCore.Qt.Key_Left, f'{topic}/actions/!x_pan', -1)
-        self._shortcuts.add(QtCore.Qt.Key_Right, f'{topic}/actions/!x_pan', 1)
-        self._shortcuts.add(QtCore.Qt.Key_Up, f'{topic}/actions/!x_zoom', [1, None])
-        self._shortcuts.add(QtCore.Qt.Key_Down, f'{topic}/actions/!x_zoom', [-1, None])
-        self._shortcuts.add(QtCore.Qt.Key_Plus, f'{topic}/actions/!x_zoom', [1, None])
-        self._shortcuts.add(QtCore.Qt.Key_Minus, f'{topic}/actions/!x_zoom', [-1, None])
+    def keyPressEvent(self, event: QtGui.QKeyEvent):
+        v = self._keymap.get((event.key(), event.modifiers()))
+        if v is None:
+            super().keyPressEvent(event)
+        else:
+            self._log.info(f'key {event.key()} -> publish {v}')
+            self.pubsub.publish(*v)
 
     def on_pubsub_unregister(self):
-        self._shortcuts.clear()
         self._paint_timer.stop()
         self._paint_state = PaintState.IDLE
 
     def on_pubsub_delete(self):
         for topic, value in self.pubsub.query(f'{self.topic}/settings/close_actions', default=[]):
             self._log.info('waveform close: %s %s', topic, value)
             self.pubsub.publish(topic, value)
@@ -2859,16 +2902,15 @@
             else:
                 self._mouse_action = None
         else:
             self._mouse_action = None
 
     def _on_menu_x_marker(self, action):
         pos = self._x_map.counter_to_time64(self._mouse_pos[0])
-        topic = get_topic_name(self)
-        self.pubsub.publish(f'{topic}/actions/!x_markers', [action, pos, None])
+        self.pubsub.publish(f'{self.topic}/actions/!x_markers', [action, pos, None])
 
     @QtCore.Slot()
     def _on_menu_x_marker_add_single(self):
         self._on_menu_x_marker('add_single')
 
     @QtCore.Slot()
     def _on_menu_x_marker_add_dual(self):
@@ -2929,15 +2971,15 @@
         return self.state['plots'][plot_index]
 
     def _on_menu_y_marker(self, action):
         plot = self._lookup_plot()
         if plot is not None:
             pos = self._y_pixel_to_value(plot, self._mouse_pos[1])
             topic = get_topic_name(self)
-            self.pubsub.publish(f'{topic}/actions/!y_markers', [action, plot, pos, None])
+            self.pubsub.publish(f'{topic}/actions/!y_markers', [action, plot['index'], pos, None])
 
     @QtCore.Slot()
     def _on_menu_y_marker_add_single(self):
         self._on_menu_y_marker('add_single')
 
     @QtCore.Slot()
     def _on_menu_y_marker_add_dual(self):
@@ -3096,17 +3138,19 @@
             if source.startswith('JlsSource'):
                 path = self.pubsub.query(f'{get_topic_name(source)}/settings/path')
                 path_base, path_ext = os.path.splitext(path)
                 anno_path = f'{path_base}.anno{path_ext}'
                 self.on_callback_annotation_save({'path': anno_path})
 
     def _on_menu_annotations_clear_all(self, checked=False):
-        self._on_menu_x_marker('clear_all')
-        self._on_menu_y_marker('clear_all')
-        self._on_menu_text_annotation('clear_all')
+        value = ['clear_all']
+        plot = self._lookup_plot()
+        if plot is not None:
+            value.append(plot['index'])
+        self.pubsub.publish(f'{self.topic}/actions/!annotations', value)
 
     def _menu_add_text_annotations(self, menu: QtWidgets.QMenu):
         CallableAction(menu, N_('Add'), lambda: self._on_menu_text_annotation('add'))
         CallableAction(menu, N_('Hide all text'), lambda: self._on_menu_text_annotation('text_hide_all'))
         CallableAction(menu, N_('Show all text'), lambda: self._on_menu_text_annotation('text_show_all'))
         CallableAction(menu, N_('Clear all'), lambda: self._on_menu_text_annotation('clear_all'))
 
@@ -3267,18 +3311,24 @@
 
     def _construct_analysis_menu_action(self, menu, unique_id, idx):
         cls = get_instance(unique_id)
         CallableAction(menu, cls.NAME, lambda: self._on_range_tool(unique_id, idx))
 
     def _on_x_marker_zoom(self, marker_idx, zoom_level):
         m = self._annotation_lookup(marker_idx)
-        z0, z1 = m['pos1'], m['pos2']
-        zc = (z1 + z0) / 2
-        zd = abs(z1 - z0) / (2 * float(zoom_level))
-        z0, z1 = int(zc - zd), int(zc + zd)
+        if m['dtype'] == 'dual':
+            z0, z1 = m['pos1'], m['pos2']
+            zc = (z1 + z0) / 2
+            zd = abs(z1 - z0) / (2 * float(zoom_level))
+            z0, z1 = int(zc - zd), int(zc + zd)
+        else:
+            x0, x1 = self.x_range
+            xd = (x1 - x0) // 2
+            p = m['pos1']
+            z0, z1 = p - xd, p + xd
         self.pubsub.publish(f'{self.topic}/actions/!x_zoom_to', [z0, z1])
 
     def _construct_x_marker_zoom_menu_action(self, menu, idx, zoom_level):
         CallableAction(menu, f'{zoom_level}%', lambda: self._on_x_marker_zoom(idx, zoom_level / 100.0))
 
     def _on_x_interval(self, m, pos_text, interval):
         other_pos = 'pos2' if pos_text == 'pos1' else 'pos1'
@@ -3361,15 +3411,16 @@
         shape_group = QtGui.QActionGroup(shape)
 
         def shape_item(index, name):
             CallableAction(shape_group, name,
                            lambda: self._on_text_annotation_shape(a['id'], index),
                            checkable=True, checked=(a['shape'] == index))
         [shape_item(index, value[1]) for index, value in enumerate(SHAPES_DEF)]
-        CallableAction(menu, N_('Remove'), lambda: self._on_text_annotation_remove(a['id']))
+        CallableAction(menu, N_('Remove'), lambda: self.pubsub.publish(f'{self.topic}/actions/!text_annotation',
+                                                                       ['remove', a['id']]))
         return context_menu_show(menu, event)
 
     def _on_text_annotation_edit(self, a_id):
         a = self._annotation_lookup(a_id)
         TextAnnotationDialog(self, self.unique_id, a).show()
 
     def _on_text_annotation_show(self, a_id, value):
@@ -3392,15 +3443,15 @@
         self._text_annotation_remove(a)
 
     def _menu_y_marker_single(self, item, event: QtGui.QMouseEvent):
         m, m_pos = self._item_parse_y_marker(item)
         menu = QtWidgets.QMenu('Waveform y_marker context menu', self)
         CallableAction(menu, N_('Remove'),
                        lambda: self.pubsub.publish(f'{get_topic_name(self)}/actions/!y_markers',
-                                                   ['remove', m['plot_index'], m['id']]))
+                                                   ['remove', m['id']]))
         return context_menu_show(menu, event)
 
     def _menu_summary_quantity(self, menu, quantity, name):
         def action():
             self.summary_quantity = quantity
         return CallableAction(menu, name, action)
 
@@ -3518,14 +3569,15 @@
             add_single, add_dual, clear_all.  The commands are:
             * ['add_single', pos]
             * ['add_dual', center, None]
             * ['add_dual', pos1, pos2]
             * ['clear_all']
             * ['remove', marker_id, ...]
             * ['add', marker_obj, ...]  # for undo remove
+            * ['select', marker_id]
         """
         self._log.info('x_markers %s', value)
         value = _marker_action_string_to_command(value)
         cmd = value[0]
         self._repaint_request = True
         if cmd == 'remove':
             m = self._x_marker_remove(value[1])
@@ -3538,15 +3590,20 @@
             return [topic, ['remove', m['id']]]
         elif cmd == 'add':
             for m in value[1:]:
                 self._x_marker_add(m)
             return [topic, ['remove'] + value[1:]]
         elif cmd == 'clear_all':
             self.annotations['x'], rv = OrderedDict(), self.annotations['x']
-            return None
+            return [topic, ['add'] + list(rv.values())]
+        elif cmd == 'select':
+            try:
+                self._on_x_marker_zoom(value[1], 0.75)
+            except KeyError:
+                pass
         else:
             raise NotImplementedError(f'Unsupported marker action {value}')
 
     def _y_marker_position(self, plot, yi):
         yi = self._y_transform_fwd(plot, yi)
         yi_init = yi
         y0, y1 = plot['range']
@@ -3653,42 +3710,50 @@
         :param value: Either the action string or [action, args...].
             Action strings that do not require arguments include:
             add_single, add_dual, clear_all.  The commands are:
             * ['add_single', plot, pos]
             * ['add_dual', plot, center, None]
             * ['add_dual', plot, pos1, pos2]
             * ['clear_all', plot]
-            * ['remove', plot, marker_id, ...]
-            * ['add', plot, marker_obj, ...]  # for undo remove
+            * ['remove', marker_id, ...]
+            * ['add', marker_obj, ...]  # for undo remove
 
             In all cases, plot can be the plot index or plot object.
         """
         self._log.info('y_markers %s', value)
         value = _marker_action_string_to_command(value)
         cmd = value[0]
-        plot = self._plot_get(value[1])
-        plot_index = plot['index']
         self._repaint_request = True
         if cmd == 'remove':
-            for m in value[2:]:
-                self._y_marker_remove(m)
-            return [topic, ['add', plot_index] + value[2:]]
+            undo = ['add']
+            for m in value[1:]:
+                undo.append(self._y_marker_remove(m))
+            return [topic, undo]
         elif cmd == 'add_single':
+            plot = self._plot_get(value[1])
             m = self._y_marker_add_single(plot, value[2])
-            return [topic, ['remove', plot_index, m['id']]]
+            return [topic, ['remove', m['id']]]
         elif cmd == 'add_dual':
+            plot = self._plot_get(value[1])
             m = self._y_marker_add_dual(plot, value[2], value[3])
-            return [topic, ['remove', plot_index, m['id']]]
+            return [topic, ['remove', m['id']]]
         elif cmd == 'add':
-            for m in value[2:]:
+            for m in value[1:]:
                 self._y_marker_add(m)
-            return [topic, ['remove', plot_index] + value[2:]]
+            return [topic, ['remove'] + value[1:]]
         elif cmd == 'clear_all':
-            self.annotations['y'][plot_index], items = OrderedDict(), self.annotations['y'][plot_index]
-            return [topic, ['add', list(items.values())]]
+            if len(value) == 1:
+                plot_ids = [p['index'] for p in self.state['plots']]
+            else:
+                plot_ids = [value[1]]
+            all_items = []
+            for plot_index in plot_ids:
+                self.annotations['y'][plot_index], items = OrderedDict(), self.annotations['y'][plot_index]
+                all_items.extend(items.values())
+            return [topic, ['add'] + all_items]
         else:
             raise NotImplementedError(f'Unsupported marker action {value}')
 
     def _text_annotation_add(self, a):
         plot_index = a['plot_index']
         if 'id' not in a:
             a['id'] = self._annotation_next_id('text', plot_index)
@@ -3715,14 +3780,15 @@
         elif idx_len > 1:
             self._log.warning('_text_annotation_remove but too many entries')
         else:
             x_lookup[idx[0]:-1, :] = x_lookup[(idx[0] + 1):, :]
             entry['x_lookup_length'] -= 1
         del self.annotations['text'][a['plot_index']]['items'][a_id]
         self._repaint_request = True
+        return a
 
     def on_callback_annotation_save(self, value):
         """Export callback to save annotations.
 
         :param value: The value dict with keys (see _on_x_export):
             * x_range: The (x0, x1) time64 range.  Use extents if not provided.
             * signals: The list of signals to export.
@@ -3805,21 +3871,22 @@
         """
         self._log.info('text_annotation %s', value)
         action = value[0]
         self._repaint_request = True
         if action == 'add':
             for a in value[1:]:
                 self._text_annotation_add(a)
-            return [topic, ['remove', a]]
+            return [topic, ['remove'] + value[1:]]
         elif action == 'update':
             pass  # text_annotation entry modified in place
         elif action == 'remove':
+            undo = ['add']
             for a in value[1:]:
-                self._text_annotation_remove(a)
-            return [topic, ['add', a]]
+                undo.append(self._text_annotation_remove(a))
+            return [topic, undo]
         elif action in ['text_hide_all', 'text_show_all']:
             show = (action == 'text_show_all')
             if len(value) == 1:
                 plot_ids = [p['index'] for p in self.state['plots']]
             else:
                 plot_ids = value[1:]
             for plot_id in plot_ids:
@@ -3835,18 +3902,37 @@
             all_items = []
             for plot_id in plot_ids:
                 entry = self.annotations['text'][plot_id]
                 self.annotations['text'][plot_id]['items'], items = OrderedDict(), self.annotations['text'][plot_id]['items']
                 entry['x_lookup_length'] = 0
                 entry['x_lookup'][:, 0] = np.iinfo(np.int64).max
                 all_items.extend(items.values())
-            return [topic, ['add', all_items]]
+            return [topic, ['add'] + all_items]
         else:
             raise ValueError(f'unsupported text_annotation action {action}')
 
+    def on_action_annotations(self, topic, value):
+        cmd = value[0]
+        if cmd == 'clear_all':
+            undo = [
+                'undo',
+                self.on_action_x_markers(f'{self.topic}/actions/!x_markers', ['clear_all']),
+                self.on_action_y_markers(f'{self.topic}/actions/!y_markers', ['clear_all'] + value[1:]),
+                self.on_action_text_annotation(f'{self.topic}/actions/!text_annotation', ['clear_all'] + value[1:]),
+            ]
+            return [topic, undo]
+        elif cmd == 'undo':
+            undo = [
+                'undo',
+                self.on_action_x_markers(*value[1]),
+                self.on_action_y_markers(*value[2]),
+                self.on_action_text_annotation(*value[3]),
+            ]
+            return [topic, undo]
+
     def on_action_x_range(self, topic, value):
         """Set the x-axis range.
 
         :param topic: The topic name.
         :param value: The [x_min, x_max] range.
         """
         e0, e1 = self._extents()
```

### Comparing `joulescope_ui-1.1.6/joulescope_ui/widgets/waveform/y_range_widget.py` & `joulescope_ui-1.1.7/joulescope_ui/widgets/waveform/y_range_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui/zip_inspector.py` & `joulescope_ui-1.1.7/joulescope_ui/zip_inspector.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/joulescope_ui.egg-info/PKG-INFO` & `joulescope_ui-1.1.7/joulescope_ui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joulescope_ui
-Version: 1.1.6
+Version: 1.1.7
 Summary: Joulescope™ graphical user interface
 Home-page: https://www.joulescope.com
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/pyjoulescope_ui/issues
 Project-URL: Funding, https://www.joulescope.com
@@ -34,15 +34,15 @@
 License-File: LICENSE.txt
 Requires-Dist: appnope>=0.1.2
 Requires-Dist: fs
 Requires-Dist: pyjoulescope_driver<2.0.0,>=1.5.1
 Requires-Dist: joulescope<2.0.0,>=1.1.12
 Requires-Dist: markdown
 Requires-Dist: psutil
-Requires-Dist: pyjls>=0.9.2
+Requires-Dist: pyjls>=0.9.4
 Requires-Dist: pyopengl
 Requires-Dist: pywin32>=223; platform_system == "Windows"
 Requires-Dist: pyqtgraph>=0.13.3
 Requires-Dist: PySide6<7.0.0,>=6.7.0
 Requires-Dist: PySide6-QtAds<5.0.0,>=4.2.1.1
 Requires-Dist: python-dateutil>=2.7.3
 Requires-Dist: QtPy
```

### Comparing `joulescope_ui-1.1.6/joulescope_ui.egg-info/SOURCES.txt` & `joulescope_ui-1.1.7/joulescope_ui.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 joulescope_ui/range_tool.py
 joulescope_ui/reporter.py
 joulescope_ui/resources.py
 joulescope_ui/resources.rcc
 joulescope_ui/safe_mode.py
 joulescope_ui/sanitize.py
 joulescope_ui/shift_key.py
-joulescope_ui/shortcuts.py
 joulescope_ui/software_update.py
 joulescope_ui/source_selector.py
 joulescope_ui/time_map.py
 joulescope_ui/tokens.py
 joulescope_ui/tooltip.py
 joulescope_ui/ui_util.py
 joulescope_ui/units.py
```

### Comparing `joulescope_ui-1.1.6/pyproject.toml` & `joulescope_ui-1.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.6/setup.py` & `joulescope_ui-1.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,15 +197,15 @@
     install_requires=[
         'appnope>=0.1.2',
         'fs',
         'pyjoulescope_driver>=1.5.1,<2.0.0',
         'joulescope>=1.1.12,<2.0.0',
         'markdown',
         'psutil',
-        'pyjls>=0.9.2',
+        'pyjls>=0.9.4',
         'pyopengl',
         "pywin32>=223; platform_system == 'Windows'",
         'pyqtgraph>=0.13.3',
         'PySide6>=6.7.0,<7.0.0',
         'PySide6-QtAds>=4.2.1.1,<5.0.0',
         'python-dateutil>=2.7.3',
         'QtPy',
```

