# Comparing `tmp/janim-0.5.2.tar.gz` & `tmp/janim-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "janim-0.5.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "janim-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `janim-0.5.2.tar` & `janim-1.0.0.tar`

### file list

```diff
@@ -1,97 +1,99 @@
--rw-r--r--   0        0        0      164 2024-03-08 02:47:13.175046 janim-0.5.2/.gitignore
--rw-r--r--   0        0        0     1053 2024-04-17 15:49:03.633620 janim-0.5.2/.readthedocs.yaml
--rw-r--r--   0        0        0      398 2024-03-07 03:42:49.399574 janim-0.5.2/.vscode/settings.json
--rw-r--r--   0        0        0      403 2023-10-12 06:08:14.650702 janim-0.5.2/.vscode/tasks.json
--rw-r--r--   0        0        0     1085 2023-08-02 08:54:33.983910 janim-0.5.2/LICENSE
--rw-r--r--   0        0        0      966 2024-03-08 14:50:49.538193 janim-0.5.2/README.md
--rw-r--r--   0        0        0       71 2024-04-17 15:51:46.338095 janim-0.5.2/janim/__init__.py
--rw-r--r--   0        0        0     3147 2024-04-17 03:59:08.847168 janim-0.5.2/janim/__main__.py
--rw-r--r--   0        0        0     4095 2024-04-17 03:59:08.847168 janim-0.5.2/janim/anims/animation.py
--rw-r--r--   0        0        0     5417 2024-04-17 03:59:08.848161 janim-0.5.2/janim/anims/composition.py
--rw-r--r--   0        0        0     5922 2024-04-17 03:59:08.848161 janim-0.5.2/janim/anims/creation.py
--rw-r--r--   0        0        0      855 2024-02-20 13:10:29.944561 janim-0.5.2/janim/anims/display.py
--rw-r--r--   0        0        0     3293 2024-03-14 06:39:26.710299 janim-0.5.2/janim/anims/fading.py
--rw-r--r--   0        0        0     1484 2024-04-17 03:59:08.849160 janim-0.5.2/janim/anims/rotation.py
--rw-r--r--   0        0        0    27295 2024-04-17 15:49:03.638608 janim-0.5.2/janim/anims/timeline.py
--rw-r--r--   0        0        0     8590 2024-04-17 03:59:08.850373 janim-0.5.2/janim/anims/transform.py
--rw-r--r--   0        0        0     9432 2024-03-14 08:01:57.787600 janim-0.5.2/janim/anims/updater.py
--rw-r--r--   0        0        0     4495 2024-04-16 10:46:40.397643 janim-0.5.2/janim/camera/camera.py
--rw-r--r--   0        0        0     2744 2024-03-05 11:28:56.434384 janim-0.5.2/janim/camera/camera_info.py
--rw-r--r--   0        0        0     6703 2024-04-17 03:59:08.851151 janim-0.5.2/janim/cli.py
--rw-r--r--   0        0        0     8265 2024-04-17 03:59:08.851151 janim-0.5.2/janim/components/component.py
--rw-r--r--   0        0        0     2326 2024-03-14 06:39:26.718305 janim-0.5.2/janim/components/data.py
--rw-r--r--   0        0        0     2517 2024-03-26 14:54:35.911658 janim-0.5.2/janim/components/depth.py
--rw-r--r--   0        0        0     1279 2024-03-05 11:28:56.434384 janim-0.5.2/janim/components/image.py
--rw-r--r--   0        0        0    31519 2024-03-26 14:54:35.911658 janim-0.5.2/janim/components/points.py
--rw-r--r--   0        0        0     3024 2024-03-14 12:12:39.400689 janim-0.5.2/janim/components/radius.py
--rw-r--r--   0        0        0     8633 2024-03-26 14:54:35.912656 janim-0.5.2/janim/components/rgbas.py
--rw-r--r--   0        0        0    23584 2024-03-26 14:54:35.916644 janim-0.5.2/janim/components/vpoints.py
--rw-r--r--   0        0        0      171 2024-02-20 13:10:29.968656 janim-0.5.2/janim/constants/__init__.py
--rw-r--r--   0        0        0      169 2024-01-12 15:55:35.365552 janim-0.5.2/janim/constants/alignment.py
--rw-r--r--   0        0        0     1333 2024-02-20 13:10:29.970716 janim-0.5.2/janim/constants/colors.py
--rw-r--r--   0        0        0      483 2024-03-05 11:28:56.458376 janim-0.5.2/janim/constants/coord.py
--rw-r--r--   0        0        0      179 2024-01-12 15:55:05.570414 janim-0.5.2/janim/constants/degrees.py
--rw-r--r--   0        0        0     4806 2024-04-17 03:59:08.852148 janim-0.5.2/janim/examples.py
--rw-r--r--   0        0        0     1721 2024-03-14 06:39:26.734309 janim-0.5.2/janim/exception.py
--rw-r--r--   0        0        0    39740 2024-04-17 15:49:03.641638 janim-0.5.2/janim/gui/anim_viewer.py
--rw-r--r--   0        0        0      330 2024-02-20 13:10:29.974744 janim-0.5.2/janim/gui/application.py
--rw-r--r--   0        0        0      797 2024-04-17 03:59:08.853145 janim-0.5.2/janim/gui/audio_player.py
--rw-r--r--   0        0        0     3181 2024-02-20 13:10:29.978729 janim-0.5.2/janim/gui/export.png
--rw-r--r--   0        0        0     1258 2024-02-20 13:10:29.978729 janim-0.5.2/janim/gui/fixed_ratio_widget.py
--rw-r--r--   0        0        0      845 2024-04-17 03:59:08.854142 janim-0.5.2/janim/gui/glwidget.py
--rw-r--r--   0        0        0      903 2024-04-17 03:59:08.854142 janim-0.5.2/janim/gui/precise_timer.py
--rw-r--r--   0        0        0     5278 2024-03-26 14:54:35.926619 janim-0.5.2/janim/gui/richtext_editor.py
--rw-r--r--   0        0        0     8892 2024-03-14 06:39:26.742300 janim-0.5.2/janim/gui/selector.py
--rw-r--r--   0        0        0     1564 2024-04-17 03:59:08.854142 janim-0.5.2/janim/imports.py
--rw-r--r--   0        0        0     4744 2024-04-17 03:59:08.855140 janim-0.5.2/janim/items/audio.py
--rw-r--r--   0        0        0     4862 2024-03-08 02:47:13.255043 janim-0.5.2/janim/items/boolean_ops.py
--rw-r--r--   0        0        0     8823 2024-03-26 14:54:35.934597 janim-0.5.2/janim/items/coordinate/coordinate_systems.py
--rw-r--r--   0        0        0     2165 2024-03-26 14:54:35.938586 janim-0.5.2/janim/items/coordinate/functions.py
--rw-r--r--   0        0        0     8330 2024-03-26 14:54:35.942576 janim-0.5.2/janim/items/coordinate/number_line.py
--rw-r--r--   0        0        0     8792 2024-03-23 03:08:17.235541 janim-0.5.2/janim/items/geometry/arc.py
--rw-r--r--   0        0        0     6497 2024-03-26 14:54:35.947562 janim-0.5.2/janim/items/geometry/arrow.py
--rw-r--r--   0        0        0     8130 2024-04-12 02:55:45.180361 janim-0.5.2/janim/items/geometry/line.py
--rw-r--r--   0        0        0     5379 2024-03-14 06:39:26.922045 janim-0.5.2/janim/items/geometry/polygon.py
--rw-r--r--   0        0        0     5315 2024-03-05 11:28:56.482378 janim-0.5.2/janim/items/image_item.py
--rw-r--r--   0        0        0    19385 2024-03-24 09:07:24.006701 janim-0.5.2/janim/items/item.py
--rw-r--r--   0        0        0     3397 2024-03-14 06:39:26.922045 janim-0.5.2/janim/items/points.py
--rw-r--r--   0        0        0     7379 2024-03-26 14:54:35.952548 janim-0.5.2/janim/items/relation.py
--rw-r--r--   0        0        0     6290 2024-03-14 06:39:26.922045 janim-0.5.2/janim/items/svg/brace.py
--rw-r--r--   0        0        0     1736 2024-03-14 06:39:26.930042 janim-0.5.2/janim/items/svg/brace.svg
--rw-r--r--   0        0        0     4072 2024-04-17 03:59:08.855140 janim-0.5.2/janim/items/svg/svg_item.py
--rw-r--r--   0        0        0     3090 2024-04-17 03:59:08.856138 janim-0.5.2/janim/items/svg/typst.py
--rw-r--r--   0        0        0       40 2024-03-05 11:28:56.482378 janim-0.5.2/janim/items/svg/typst_template.typ
--rw-r--r--   0        0        0    15651 2024-04-17 03:59:08.856138 janim-0.5.2/janim/items/text/text.py
--rw-r--r--   0        0        0     1064 2024-03-14 06:39:26.938042 janim-0.5.2/janim/items/value_tracker.py
--rw-r--r--   0        0        0     5487 2024-03-26 14:54:35.961526 janim-0.5.2/janim/items/vitem.py
--rw-r--r--   0        0        0      271 2024-01-17 04:53:39.682291 janim-0.5.2/janim/logger.py
--rw-r--r--   0        0        0     3054 2024-03-06 03:25:06.445058 janim-0.5.2/janim/render/base.py
--rw-r--r--   0        0        0     8944 2024-03-06 03:27:12.375792 janim-0.5.2/janim/render/impl.py
--rw-r--r--   0        0        0      448 2024-02-20 13:10:30.002762 janim-0.5.2/janim/render/shaders/dotcloud.frag.glsl
--rw-r--r--   0        0        0     1250 2024-04-01 15:20:38.430742 janim-0.5.2/janim/render/shaders/dotcloud.geom.glsl
--rw-r--r--   0        0        0      325 2024-02-20 13:10:30.006723 janim-0.5.2/janim/render/shaders/dotcloud.vert.glsl
--rw-r--r--   0        0        0      180 2024-03-05 11:28:56.506406 janim-0.5.2/janim/render/shaders/image.frag.glsl
--rw-r--r--   0        0        0      350 2024-03-05 11:28:56.506406 janim-0.5.2/janim/render/shaders/image.vert.glsl
--rw-r--r--   0        0        0     6950 2024-04-12 03:01:12.197148 janim-0.5.2/janim/render/shaders/vitem.frag.glsl
--rw-r--r--   0        0        0      203 2024-02-20 13:10:30.010722 janim-0.5.2/janim/render/shaders/vitem.vert.glsl
--rw-r--r--   0        0        0      857 2024-03-05 11:28:56.514381 janim-0.5.2/janim/render/texture.py
--rw-r--r--   0        0        0     6787 2024-04-17 03:59:08.857134 janim-0.5.2/janim/render/writer.py
--rw-r--r--   0        0        0      950 2024-03-14 06:39:26.962043 janim-0.5.2/janim/typing.py
--rw-r--r--   0        0        0    17207 2024-03-26 14:54:35.966511 janim-0.5.2/janim/utils/bezier.py
--rw-r--r--   0        0        0     4156 2024-04-17 03:59:08.858135 janim-0.5.2/janim/utils/config.py
--rw-r--r--   0        0        0      215 2024-02-20 13:10:30.018725 janim-0.5.2/janim/utils/data.py
--rw-r--r--   0        0        0      637 2024-03-26 14:54:35.970502 janim-0.5.2/janim/utils/dict_ops.py
--rw-r--r--   0        0        0      657 2024-04-17 03:59:08.858135 janim-0.5.2/janim/utils/file_ops.py
--rw-r--r--   0        0        0     2406 2024-04-17 03:59:08.859133 janim-0.5.2/janim/utils/font.py
--rw-r--r--   0        0        0     6369 2024-03-05 11:28:56.522384 janim-0.5.2/janim/utils/font_manager.py
--rw-r--r--   0        0        0     5973 2024-03-05 11:28:56.530408 janim-0.5.2/janim/utils/iterables.py
--rw-r--r--   0        0        0     1870 2024-02-20 13:10:30.022729 janim-0.5.2/janim/utils/paths.py
--rw-r--r--   0        0        0     2705 2024-01-31 12:46:51.074078 janim-0.5.2/janim/utils/rate_functions.py
--rw-r--r--   0        0        0     2008 2024-02-20 13:10:30.022729 janim-0.5.2/janim/utils/refresh.py
--rw-r--r--   0        0        0     8918 2024-03-07 06:40:50.078686 janim-0.5.2/janim/utils/signal.py
--rw-r--r--   0        0        0     2000 2024-03-05 11:28:56.538410 janim-0.5.2/janim/utils/simple_functions.py
--rw-r--r--   0        0        0    10068 2024-03-08 02:47:13.319071 janim-0.5.2/janim/utils/space_ops.py
--rw-r--r--   0        0        0     1108 2024-04-17 03:59:08.859133 janim-0.5.2/janim/utils/unique_nparray.py
--rw-r--r--   0        0        0    22970 2024-03-08 02:47:13.327041 janim-0.5.2/logo.png
--rw-r--r--   0        0        0     1018 2024-04-17 04:51:28.717344 janim-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     1997 1970-01-01 00:00:00.000000 janim-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0      165 2024-04-29 03:02:09.985896 janim-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1053 2024-04-17 15:49:03.633620 janim-1.0.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      413 2024-04-28 10:20:10.624911 janim-1.0.0/.vscode/settings.json
+-rw-r--r--   0        0        0      403 2023-10-12 06:08:14.650702 janim-1.0.0/.vscode/tasks.json
+-rw-r--r--   0        0        0     1085 2023-08-02 08:54:33.983910 janim-1.0.0/LICENSE
+-rw-r--r--   0        0        0      966 2024-03-08 14:50:49.538193 janim-1.0.0/README.md
+-rw-r--r--   0        0        0       71 2024-05-11 03:15:47.840567 janim-1.0.0/janim/__init__.py
+-rw-r--r--   0        0        0     3147 2024-04-17 03:59:08.847168 janim-1.0.0/janim/__main__.py
+-rw-r--r--   0        0        0     4099 2024-05-10 15:16:50.978563 janim-1.0.0/janim/anims/animation.py
+-rw-r--r--   0        0        0     6349 2024-05-10 15:15:49.989394 janim-1.0.0/janim/anims/composition.py
+-rw-r--r--   0        0        0     5861 2024-04-29 03:02:09.993849 janim-1.0.0/janim/anims/creation.py
+-rw-r--r--   0        0        0      721 2024-04-29 03:02:09.993849 janim-1.0.0/janim/anims/display.py
+-rw-r--r--   0        0        0     3246 2024-04-29 03:02:09.993849 janim-1.0.0/janim/anims/fading.py
+-rw-r--r--   0        0        0     3458 2024-05-10 01:15:31.092973 janim-1.0.0/janim/anims/growing.py
+-rw-r--r--   0        0        0     9094 2024-05-11 01:59:04.880227 janim-1.0.0/janim/anims/indication.py
+-rw-r--r--   0        0        0     1525 2024-05-11 01:34:20.294913 janim-1.0.0/janim/anims/rotation.py
+-rw-r--r--   0        0        0    24756 2024-05-11 02:53:28.238786 janim-1.0.0/janim/anims/timeline.py
+-rw-r--r--   0        0        0     8894 2024-04-29 03:02:10.001840 janim-1.0.0/janim/anims/transform.py
+-rw-r--r--   0        0        0     9918 2024-05-10 15:49:08.746418 janim-1.0.0/janim/anims/updater.py
+-rw-r--r--   0        0        0     4505 2024-04-29 03:02:10.001840 janim-1.0.0/janim/camera/camera.py
+-rw-r--r--   0        0        0     2744 2024-03-05 11:28:56.434384 janim-1.0.0/janim/camera/camera_info.py
+-rw-r--r--   0        0        0     6808 2024-04-28 10:19:08.668987 janim-1.0.0/janim/cli.py
+-rw-r--r--   0        0        0     9221 2024-05-09 02:33:32.575199 janim-1.0.0/janim/components/component.py
+-rw-r--r--   0        0        0     2408 2024-04-29 03:02:10.001840 janim-1.0.0/janim/components/data.py
+-rw-r--r--   0        0        0     2609 2024-05-10 14:02:00.852109 janim-1.0.0/janim/components/depth.py
+-rw-r--r--   0        0        0     1284 2024-04-29 03:02:10.001840 janim-1.0.0/janim/components/image.py
+-rw-r--r--   0        0        0    30900 2024-05-10 09:03:24.673167 janim-1.0.0/janim/components/points.py
+-rw-r--r--   0        0        0     2833 2024-04-29 04:16:18.595714 janim-1.0.0/janim/components/radius.py
+-rw-r--r--   0        0        0     7922 2024-05-10 15:58:49.637620 janim-1.0.0/janim/components/rgbas.py
+-rw-r--r--   0        0        0    22599 2024-05-10 01:20:31.753161 janim-1.0.0/janim/components/vpoints.py
+-rw-r--r--   0        0        0      245 2024-05-09 02:35:19.291617 janim-1.0.0/janim/constants/__init__.py
+-rw-r--r--   0        0        0      169 2024-01-12 15:55:35.365552 janim-1.0.0/janim/constants/alignment.py
+-rw-r--r--   0        0        0     1333 2024-02-20 13:10:29.970716 janim-1.0.0/janim/constants/colors.py
+-rw-r--r--   0        0        0      483 2024-03-05 11:28:56.458376 janim-1.0.0/janim/constants/coord.py
+-rw-r--r--   0        0        0      179 2024-01-12 15:55:05.570414 janim-1.0.0/janim/constants/degrees.py
+-rw-r--r--   0        0        0     4783 2024-04-29 03:02:10.009835 janim-1.0.0/janim/examples.py
+-rw-r--r--   0        0        0     1723 2024-04-29 03:02:10.009835 janim-1.0.0/janim/exception.py
+-rw-r--r--   0        0        0    40949 2024-05-09 06:44:12.976369 janim-1.0.0/janim/gui/anim_viewer.py
+-rw-r--r--   0        0        0      330 2024-02-20 13:10:29.974744 janim-1.0.0/janim/gui/application.py
+-rw-r--r--   0        0        0      797 2024-04-17 03:59:08.853145 janim-1.0.0/janim/gui/audio_player.py
+-rw-r--r--   0        0        0     3181 2024-02-20 13:10:29.978729 janim-1.0.0/janim/gui/export.png
+-rw-r--r--   0        0        0     1258 2024-02-20 13:10:29.978729 janim-1.0.0/janim/gui/fixed_ratio_widget.py
+-rw-r--r--   0        0        0      845 2024-04-17 03:59:08.854142 janim-1.0.0/janim/gui/glwidget.py
+-rw-r--r--   0        0        0      903 2024-04-24 02:36:54.042754 janim-1.0.0/janim/gui/precise_timer.py
+-rw-r--r--   0        0        0     5278 2024-03-26 14:54:35.926619 janim-1.0.0/janim/gui/richtext_editor.py
+-rw-r--r--   0        0        0     8331 2024-04-29 03:02:10.017837 janim-1.0.0/janim/gui/selector.py
+-rw-r--r--   0        0        0     1679 2024-05-10 01:25:26.525873 janim-1.0.0/janim/imports.py
+-rw-r--r--   0        0        0     5727 2024-05-11 02:59:56.767613 janim-1.0.0/janim/items/audio.py
+-rw-r--r--   0        0        0     4862 2024-03-08 02:47:13.255043 janim-1.0.0/janim/items/boolean_ops.py
+-rw-r--r--   0        0        0     8745 2024-05-10 13:55:21.394170 janim-1.0.0/janim/items/coordinate/coordinate_systems.py
+-rw-r--r--   0        0        0     2165 2024-05-09 02:35:32.318443 janim-1.0.0/janim/items/coordinate/functions.py
+-rw-r--r--   0        0        0     8330 2024-03-26 14:54:35.942576 janim-1.0.0/janim/items/coordinate/number_line.py
+-rw-r--r--   0        0        0     8784 2024-04-28 10:29:47.798293 janim-1.0.0/janim/items/geometry/arc.py
+-rw-r--r--   0        0        0     6729 2024-05-11 01:59:17.314024 janim-1.0.0/janim/items/geometry/arrow.py
+-rw-r--r--   0        0        0     7917 2024-04-29 03:02:10.017837 janim-1.0.0/janim/items/geometry/line.py
+-rw-r--r--   0        0        0     5239 2024-05-10 14:00:42.241727 janim-1.0.0/janim/items/geometry/polygon.py
+-rw-r--r--   0        0        0     5277 2024-05-10 09:01:57.035941 janim-1.0.0/janim/items/image_item.py
+-rw-r--r--   0        0        0    18848 2024-05-11 01:35:54.138307 janim-1.0.0/janim/items/item.py
+-rw-r--r--   0        0        0     3262 2024-05-06 03:29:21.974646 janim-1.0.0/janim/items/points.py
+-rw-r--r--   0        0        0     7660 2024-05-06 05:14:45.063804 janim-1.0.0/janim/items/relation.py
+-rw-r--r--   0        0        0     2071 2024-04-28 10:20:10.634879 janim-1.0.0/janim/items/shape_matchers.py
+-rw-r--r--   0        0        0     5955 2024-04-29 03:38:28.528237 janim-1.0.0/janim/items/svg/brace.py
+-rw-r--r--   0        0        0     1736 2024-03-14 06:39:26.930042 janim-1.0.0/janim/items/svg/brace.svg
+-rw-r--r--   0        0        0     4377 2024-05-09 02:42:00.017699 janim-1.0.0/janim/items/svg/svg_item.py
+-rw-r--r--   0        0        0     3090 2024-04-17 03:59:08.856138 janim-1.0.0/janim/items/svg/typst.py
+-rw-r--r--   0        0        0       40 2024-05-09 06:47:34.328454 janim-1.0.0/janim/items/svg/typst_template.typ
+-rw-r--r--   0        0        0    16153 2024-05-09 03:09:50.338506 janim-1.0.0/janim/items/text/text.py
+-rw-r--r--   0        0        0     1094 2024-04-29 03:02:10.025824 janim-1.0.0/janim/items/value_tracker.py
+-rw-r--r--   0        0        0     5357 2024-05-06 03:22:50.462994 janim-1.0.0/janim/items/vitem.py
+-rw-r--r--   0        0        0      271 2024-01-17 04:53:39.682291 janim-1.0.0/janim/logger.py
+-rw-r--r--   0        0        0     3054 2024-04-29 03:26:21.783167 janim-1.0.0/janim/render/base.py
+-rw-r--r--   0        0        0     8845 2024-04-29 03:02:10.025824 janim-1.0.0/janim/render/impl.py
+-rw-r--r--   0        0        0      448 2024-02-20 13:10:30.002762 janim-1.0.0/janim/render/shaders/dotcloud.frag.glsl
+-rw-r--r--   0        0        0     1250 2024-04-01 15:20:38.430742 janim-1.0.0/janim/render/shaders/dotcloud.geom.glsl
+-rw-r--r--   0        0        0      325 2024-02-20 13:10:30.006723 janim-1.0.0/janim/render/shaders/dotcloud.vert.glsl
+-rw-r--r--   0        0        0      180 2024-03-05 11:28:56.506406 janim-1.0.0/janim/render/shaders/image.frag.glsl
+-rw-r--r--   0        0        0      350 2024-03-05 11:28:56.506406 janim-1.0.0/janim/render/shaders/image.vert.glsl
+-rw-r--r--   0        0        0     6950 2024-04-12 03:01:12.197148 janim-1.0.0/janim/render/shaders/vitem.frag.glsl
+-rw-r--r--   0        0        0      203 2024-02-20 13:10:30.010722 janim-1.0.0/janim/render/shaders/vitem.vert.glsl
+-rw-r--r--   0        0        0     1013 2024-05-10 08:16:24.365275 janim-1.0.0/janim/render/texture.py
+-rw-r--r--   0        0        0     6787 2024-04-17 03:59:08.857134 janim-1.0.0/janim/render/writer.py
+-rw-r--r--   0        0        0      964 2024-04-29 03:02:10.025824 janim-1.0.0/janim/typing.py
+-rw-r--r--   0        0        0    17207 2024-03-26 14:54:35.966511 janim-1.0.0/janim/utils/bezier.py
+-rw-r--r--   0        0        0     5515 2024-05-11 02:51:12.477563 janim-1.0.0/janim/utils/config.py
+-rw-r--r--   0        0        0     5786 2024-04-29 03:02:10.025824 janim-1.0.0/janim/utils/data.py
+-rw-r--r--   0        0        0      637 2024-03-26 14:54:35.970502 janim-1.0.0/janim/utils/dict_ops.py
+-rw-r--r--   0        0        0     2483 2024-04-28 10:19:08.704857 janim-1.0.0/janim/utils/file_ops.py
+-rw-r--r--   0        0        0     2907 2024-04-29 03:59:03.952932 janim-1.0.0/janim/utils/font.py
+-rw-r--r--   0        0        0     6369 2024-03-05 11:28:56.522384 janim-1.0.0/janim/utils/font_manager.py
+-rw-r--r--   0        0        0     5973 2024-03-05 11:28:56.530408 janim-1.0.0/janim/utils/iterables.py
+-rw-r--r--   0        0        0     1870 2024-02-20 13:10:30.022729 janim-1.0.0/janim/utils/paths.py
+-rw-r--r--   0        0        0     2705 2024-01-31 12:46:51.074078 janim-1.0.0/janim/utils/rate_functions.py
+-rw-r--r--   0        0        0     2651 2024-05-06 04:42:35.799305 janim-1.0.0/janim/utils/refresh.py
+-rw-r--r--   0        0        0     8342 2024-04-29 08:39:07.489731 janim-1.0.0/janim/utils/signal.py
+-rw-r--r--   0        0        0     2000 2024-03-05 11:28:56.538410 janim-1.0.0/janim/utils/simple_functions.py
+-rw-r--r--   0        0        0    10068 2024-03-08 02:47:13.319071 janim-1.0.0/janim/utils/space_ops.py
+-rw-r--r--   0        0        0    22970 2024-03-08 02:47:13.327041 janim-1.0.0/logo.png
+-rw-r--r--   0        0        0     1018 2024-04-17 04:51:28.717344 janim-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1997 1970-01-01 00:00:00.000000 janim-1.0.0/PKG-INFO
```

### Comparing `janim-0.5.2/.readthedocs.yaml` & `janim-1.0.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `janim-0.5.2/LICENSE` & `janim-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `janim-0.5.2/README.md` & `janim-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `janim-0.5.2/janim/__main__.py` & `janim-1.0.0/janim/__main__.py`

 * *Files identical despite different names*

### Comparing `janim-0.5.2/janim/anims/animation.py` & `janim-1.0.0/janim/anims/animation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 from contextvars import ContextVar
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Callable
 
-from janim.components.depth import Cmpt_Depth
 from janim.utils.rate_functions import RateFunc, smooth
 
 if TYPE_CHECKING:   # pragma: no cover
     from janim.anims.composition import AnimGroup
+    from janim.components.depth import Cmpt_Depth
 
 
 @dataclass
 class TimeRange:
     at: float
     duration: float
```

### Comparing `janim-0.5.2/janim/anims/creation.py` & `janim-1.0.0/janim/anims/creation.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         bound_func: Callable[[UpdaterParams], tuple[int, int]],
         *,
         auto_close_path: bool = False,
         become_at_end: bool = False,
         root_only: bool = False,
         **kwargs
     ):
-        def func(data: Item.Data, p: UpdaterParams) -> None:
+        def func(data: Item, p: UpdaterParams) -> None:
             cmpt = data.components.get('points', None)
             if cmpt is None or not isinstance(cmpt, Cmpt_VPoints):
                 return  # pragma: no cover
             if not cmpt.has():
                 return  # pragma: no cover
 
             if not auto_close_path:
@@ -43,15 +43,15 @@
                 begin_indices = np.array([0, *[indice + 2 for indice in end_indices[:-1]]])
 
                 points = cmpt.get()
                 cond1 = np.isclose(points[begin_indices], points[end_indices]).all(axis=1)
 
                 cmpt.pointwise_become_partial(cmpt, *bound_func(p))
 
-                points = cmpt.get()
+                points = cmpt.get().copy()
                 cond2 = ~np.isclose(points[begin_indices], points[end_indices]).all(axis=1)
                 where = np.where(cond1 & cond2)[0]
 
                 if len(where) == 0:
                     return
 
                 end_indices = end_indices[where]
@@ -121,32 +121,32 @@
             become_at_end=become_at_end,
             root_only=root_only,
             **kwargs
         )
         self.stroke_radius = stroke_radius
         self.stroke_color = stroke_color
 
-    def create_extra_data(self, data: Item.Data[VItem]) -> tuple | None:
-        if not isinstance(data.item, VItem):
+    def create_extra_data(self, data: Item) -> VItem | None:
+        if not isinstance(data, VItem):
             return None     # pragma: no cover
-        data_copy = data._copy(data)
-        data_copy.cmpt.radius.set(self.stroke_radius)
-        data_copy.cmpt.stroke.set(self.stroke_color, 1)
-        data_copy.cmpt.fill.set(alpha=0)
-        return (data_copy, )
+        data_copy = data.store()
+        data_copy.radius.set(self.stroke_radius)
+        data_copy.stroke.set(self.stroke_color, 1)
+        data_copy.fill.set(alpha=0)
+        return data_copy
 
-    def updater(self, data: Item.Data[VItem], p: UpdaterParams) -> None:
+    def updater(self, data: VItem, p: UpdaterParams) -> None:
         if p.extra_data is None:
             return  # pragma: no cover
-        outline, = p.extra_data
+        outline = p.extra_data
         index, subalpha = integer_interpolate(0, 2, p.alpha)
 
         if index == 0:
-            data._restore(outline)
-            data.cmpt.points.pointwise_become_partial(data.cmpt.points, 0, subalpha)
+            data.restore(outline)
+            data.points.pointwise_become_partial(data.points, 0, subalpha)
         else:
             data.interpolate(outline, data, subalpha)
 
 
 class Write(DrawBorderThenFill):
     '''
     显示书写过程（对每个子物件应用 :class:`DrawBorderThenFill`）
```

### Comparing `janim-0.5.2/janim/anims/fading.py` & `janim-1.0.0/janim/anims/fading.py`

 * *Files 11% similar despite different names*

```diff
@@ -40,40 +40,40 @@
         if about_point is None and scale != 1.0:
             cmpt = item(Points).points
             box = cmpt.self_box if root_only else cmpt.box
             about_point = box.get(about_edge)
         self.about_point = about_point
 
     @abstractmethod
-    def updater(self, data: Item.Data, p: UpdaterParams) -> None:
+    def updater(self, data: Item, p: UpdaterParams) -> None:
         pass
 
 
 class FadeIn(Fade):
     '''
     淡入
 
     - 可以使用 ``shift`` 指定淡入位移
     - 可以使用 ``scale`` 指定淡入缩放
     '''
-    def updater(self, data: Item.Data[Points], p: UpdaterParams) -> None:
-        if not isinstance(data.item, Points):
+    def updater(self, data: Item, p: UpdaterParams) -> None:
+        if not isinstance(data, Points):
             return
 
         for cmpt in data.components.values():
             if not isinstance(cmpt, Cmpt_Rgbas):
                 continue
-            rgbas = cmpt.get()
+            rgbas = cmpt.get().copy()
             rgbas[:, 3] *= p.alpha
             cmpt.set_rgbas(rgbas)
 
         if np.any(self.shift != ORIGIN):
-            data.cmpt.points.shift((1 - p.alpha) * -self.shift)
+            data.points.shift((1 - p.alpha) * -self.shift)
         if self.scale != 1.0:
-            data.cmpt.points.scale(
+            data.points.scale(
                 (1 - p.alpha) * 1 / self.scale + p.alpha,
                 about_point=self.about_point
             )
 
 
 class FadeOut(Fade):
     '''
@@ -94,25 +94,25 @@
             item,
             shift,
             scale,
             show_at_end=show_at_end,
             **kwargs
         )
 
-    def updater(self, data: Item.Data[Points], p: UpdaterParams) -> None:
-        if not isinstance(data.item, Points):
+    def updater(self, data: Item, p: UpdaterParams) -> None:
+        if not isinstance(data, Points):
             return
 
         for cmpt in data.components.values():
             if not isinstance(cmpt, Cmpt_Rgbas):
                 continue
-            rgbas = cmpt.get()
+            rgbas = cmpt.get().copy()
             rgbas[:, 3] *= 1 - p.alpha
             cmpt.set_rgbas(rgbas)
 
         if np.any(self.shift != ORIGIN):
-            data.cmpt.points.shift(p.alpha * self.shift)
+            data.points.shift(p.alpha * self.shift)
         if self.scale != 1.0:
-            data.cmpt.points.scale(
+            data.points.scale(
                 p.alpha * self.scale + (1 - p.alpha),
                 about_point=self.about_point
             )
```

### Comparing `janim-0.5.2/janim/anims/rotation.py` & `janim-1.0.0/janim/anims/rotation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 
 from janim.anims.updater import DataUpdater, UpdaterParams
+from janim.components.points import Cmpt_Points
+from janim.constants import ORIGIN, OUT
 from janim.items.item import Item
 from janim.items.points import Points
-from janim.components.points import Cmpt_Points
 from janim.typing import Vect
 from janim.utils.rate_functions import linear
-from janim.constants import ORIGIN
 
 
 class Rotate(DataUpdater):
     '''
     旋转，默认对角度进行平滑插值
     '''
     label_color = (64, 181, 126)
 
     def __init__(
         self,
         item: Item,
         angle: float,
         *,
+        axis: Vect = OUT,
         about_point: Vect | None = None,
         about_edge: Vect = ORIGIN,
         root_only: bool = False,
         **kwargs
     ):
         if about_point is None:
             box = item.astype(Points).points.self_box if root_only else item.astype(Points).points.box
             about_point = box.get(about_edge)
 
-        def func(data: Item.Data, p: UpdaterParams) -> None:
+        def func(data: Item, p: UpdaterParams) -> None:
             points = data.components.get('points', None)
             if points is None or not isinstance(points, Cmpt_Points):
                 return  # pragma: no cover
-            points.rotate(p.alpha * angle, about_point=about_point, root_only=True)
+            points.rotate(p.alpha * angle, axis=axis, about_point=about_point, root_only=True)
 
         super().__init__(item, func, root_only=root_only, **kwargs)
 
 
 class Rotating(Rotate):
     '''
     旋转，默认对角度进行线性插值
     '''
-    def __init__(self, item: Points, angle: float, rate_func=linear, **kwargs):
+    def __init__(self, item: Points, angle: float, *, rate_func=linear, **kwargs):
         super().__init__(item, angle, rate_func=rate_func, **kwargs)
```

### Comparing `janim-0.5.2/janim/anims/transform.py` & `janim-1.0.0/janim/anims/transform.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 from __future__ import annotations
 
 from collections import defaultdict
-from typing import TYPE_CHECKING, Self
+from typing import Self
 
 from janim.anims.animation import Animation, RenderCall
 from janim.components.component import Component
-from janim.constants import OUT
-from janim.items.item import Item
+from janim.constants import ANIM_END_DELTA, OUT
+from janim.items.item import DynamicItem, Item
 from janim.logger import log
 from janim.typing import Vect
 from janim.utils.data import AlignedData
 from janim.utils.paths import PathFunc, path_along_arc, straight_path
 
-if TYPE_CHECKING:
-    from janim.anims.timeline import DynamicData    # pragma: no cover
-
 
 class Transform(Animation):
     label_color = (208, 171, 67)
 
     def __init__(
         self,
         src_item: Item,
@@ -45,14 +42,20 @@
         self.hide_src = hide_src
         self.show_target = show_target
 
         self.root_only = root_only
 
         self.init_path_func()
 
+        for item in src_item.walk_self_and_descendants(root_only):
+            self.timeline.track(item)
+        if target_item is not src_item:
+            for item in target_item.walk_self_and_descendants(root_only):
+                self.timeline.track(item)
+
     def init_path_func(self) -> None:
         '''
         根据传入对象的 ``path_arc`` ``path_arc_axis`` ``path_func`` ，建立 ``self.path_func``
 
         不需要手动调用
         '''
         if self.path_func is not None:
@@ -66,38 +69,38 @@
                 self.path_arc_axis
             )
 
     def anim_init(self) -> None:
         '''
         进行物件数据的对齐
         '''
-        self.aligned: dict[tuple[Item, Item], AlignedData[Item.Data[Item]]] = {}
+        self.aligned: dict[tuple[Item, Item], AlignedData[Item]] = {}
         begin_times: defaultdict[Item, int] = defaultdict(int)
         end_times: defaultdict[Item, int] = defaultdict(int)
 
         # 对齐物件
         def align(item1: Item, item2: Item, recurse: bool) -> None:
             tpl = (item1, item2)
             if tpl in self.aligned:
                 return
 
-            data1 = self.timeline.get_stored_data_at_right(item1, self.global_range.at, skip_dynamic_data=True)
-            data2 = self.timeline.get_stored_data_at_left(item2, self.global_range.end, skip_dynamic_data=True)
+            data1 = item1.current(as_time=self.global_range.at, skip_dynamic=True)
+            data2 = item2.current(as_time=self.global_range.end, skip_dynamic=True)
             aligned = self.aligned[tpl] = data1.align_for_interpolate(data1, data2)
             begin_times[item1] += 1
             end_times[item2] += 1
 
             if recurse:
-                if bool(data1.children) != bool(data2.children):
+                if bool(data1.get_children()) != bool(data2.get_children()):
                     spec1 = f'<"{item1.__class__.__name__}" {id(item1):X}>'
                     spec2 = f'<"{item2.__class__.__name__}" {id(item2):X}>'
                     log.warning(f'{spec1} 和 {spec2} 的子物件无法对齐，因为二者的子物件必须同时为空或同时存在，'
-                                f'但是二者的子物件数量分别是 {len(data1.children)} 和 {len(data2.children)}')
+                                f'但是二者的子物件数量分别是 {len(data1.get_children())} 和 {len(data2.get_children())}')
                 else:
-                    for child1, child2 in zip(aligned.data1.children, aligned.data2.children):
+                    for child1, child2 in zip(aligned.data1.stored_children, aligned.data2.stored_children):
                         align(child1, child2, True)
 
         align(self.src_item, self.target_item, not self.root_only)
 
         # 因为对齐后，可能会有多个一样的物件重叠在一起
         # 所以这里需要拆分这些物件的透明度，使得重叠在一起的相同物件在颜色混合后仍表现为原有的样子
         # 这样在动画进行时和进行前后之间就不会有突兀的切换
@@ -109,15 +112,15 @@
             times = end_times.get(end, 0)
             if times >= 2:
                 aligned.data2.apart_alpha(times)
 
         # 设置 RenderCall
         self.set_render_call_list([
             RenderCall(
-                aligned.data1.cmpt.depth,
+                aligned.union.depth,
                 aligned.union.render
             )
             for aligned in self.aligned.values()
         ])
 
         # 在动画开始时自动隐藏源对象，在动画结束时自动显示目标对象
         # 可以将 ``hide_src`` 和 ``show_target`` 置为 ``False`` 以禁用
@@ -148,42 +151,41 @@
 
         self.timeline.detect_changes(item.walk_self_and_descendants())
 
     def do(self, func) -> Self:
         func(self.src_item)
         return self
 
-    def wrap_data(self, item: Item) -> DynamicData:
+    def wrap_dynamic(self, item: Item) -> DynamicItem:
         '''
-        以供传入 :meth:`~.Timeline.register_dynamic_data` 使用
+        以供传入 :meth:`~.Component.register_dynamic` 使用
         '''
-        def wrapper(global_t: float) -> Item.Data:
+        def wrapper(global_t: float) -> Component:
             aligned = self.aligned[(item, item)]
             alpha = self.get_alpha_on_global_t(global_t)
 
-            union_copy = aligned.union._copy(aligned.union)
+            union_copy = aligned.union.store()
             union_copy.interpolate(aligned.data1, aligned.data2, alpha, path_func=self.path_func)
+            union_copy.stored_children = aligned.data1.stored_children.copy()
 
             return union_copy
 
         return wrapper
 
     def anim_pre_init(self) -> None:
-        from janim.anims.timeline import ANIM_END_DELTA
-
-        self.timeline.register_dynamic_data(self.src_item, self.wrap_data(self.src_item), self.global_range.at)
-        if not self.root_only:
-            for item in self.src_item.descendants():
-                # if (item, item) not in self.aligned:
-                #     continue
-
-                self.timeline.register_dynamic_data(item, self.wrap_data(item), self.global_range.at)
-
-        self.timeline.detect_changes(self.src_item.walk_self_and_descendants(),
-                                     as_time=self.global_range.end - ANIM_END_DELTA)
+        for item in self.src_item.walk_self_and_descendants(self.root_only):
+            ih = self.timeline.items_history[item]
+            history_wo_dnmc = ih.history_without_dynamic
+            not_changed = history_wo_dnmc.has_record() and history_wo_dnmc.latest().data.not_changed(item)
+            self.timeline.register_dynamic(item,
+                                           self.wrap_dynamic(item),
+                                           None if not_changed else item.store(),
+                                           self.global_range.at,
+                                           self.global_range.end - ANIM_END_DELTA,
+                                           not_changed)
 
     def anim_on_alpha(self, alpha: float) -> None:
         if alpha == self.current_alpha:
             return
         self.current_alpha = alpha
         super().anim_on_alpha(alpha)
```

### Comparing `janim-0.5.2/janim/anims/updater.py` & `janim-1.0.0/janim/anims/updater.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 
 import inspect
 from contextvars import ContextVar
 from dataclasses import dataclass
 from typing import Any, Callable, Self
 
 from janim.anims.animation import Animation, RenderCall, TimeRange
-from janim.anims.timeline import ANIM_END_DELTA, DynamicData
+from janim.constants import ANIM_END_DELTA
 from janim.exception import UpdaterError
-from janim.items.item import Item
+from janim.items.item import Item, DynamicItem
 from janim.utils.simple_functions import clip
 
 
 @dataclass
 class UpdaterParams:
     '''
     ``Updater`` 调用时会传递的参数，用于标注时间信息以及动画进度
     '''
+    updater: DataUpdater | ItemUpdater
     global_t: float
     alpha: float
     range: TimeRange
     extra_data: tuple | None
 
     def __enter__(self) -> Self:
         self.token = updater_params_ctx.set(self)
@@ -28,14 +29,16 @@
 
     def __exit__(self, exc_type, exc_value, tb):
         updater_params_ctx.reset(self.token)
 
 
 updater_params_ctx: ContextVar[UpdaterParams] = ContextVar('updater_params_ctx')
 
+type DataUpdaterFn[T] = Callable[[T, UpdaterParams], Any]
+
 
 class DataUpdater[T: Item](Animation):
     '''
     以时间为参数对物件的数据进行修改
 
     例如：
 
@@ -45,37 +48,34 @@
             def construct(self) -> None:
                 rect = Rect()
                 rect.points.to_border(LEFT)
 
                 self.play(
                     DataUpdater(
                         rect,
-                        lambda data, p: data.cmpt.points.rotate(p.alpha * 180 * DEGREES).shift(p.alpha * 6 * RIGHT)
+                        lambda data, p: data.points.rotate(p.alpha * 180 * DEGREES).shift(p.alpha * 6 * RIGHT)
                     )
                 )
 
-
     会产生一个“矩形从左侧旋转着移动到右侧”的动画
 
-    注：使用 ``data.cmpt`` 即可访问物件的组件，例如物件的组件方法 ``item.points.xxx`` 对于数据来说则是通过 ``data.cmpt.points.xxx`` 来调用
-
     另见：:class:`~.UpdaterExample`
     '''
     label_color = (49, 155, 191)
 
     @dataclass
     class DataGroup:
-        orig_data: Item.Data[Item]
-        data: Item.Data[Item]
-        extra_data: tuple | None
+        orig_data: Item
+        data: Item
+        extra_data: Any | None
 
     def __init__(
         self,
         item: T,
-        func: Callable[[Item.Data[T], UpdaterParams], Any],
+        func: DataUpdaterFn[T],
         *,
         lag_ratio: float = 0,
         hide_at_begin: bool = True,
         show_at_end: bool = True,
         become_at_end: bool = True,
         skip_null_items: bool = True,
         root_only: bool = True,
@@ -87,69 +87,82 @@
         self.lag_ratio = lag_ratio
         self.hide_at_begin = hide_at_begin
         self.show_at_end = show_at_end
         self.become_at_end = become_at_end
         self.skip_null_items = skip_null_items
         self.root_only = root_only
 
-    def create_extra_data(self, data: Item.Data) -> tuple | None:
+        self.post_updaters: list[DataUpdaterFn[T]] = []
+
+        for subitem in item.walk_self_and_descendants(root_only):
+            self.timeline.track(subitem)
+
+    def add_post_updater(self, updater: DataUpdaterFn[T]) -> Self:
+        self.post_updaters.append(updater)
+        return self
+
+    def call(self, data: T, p: UpdaterParams) -> None:
+        self.func(data, p)
+        for updater in self.post_updaters:
+            updater(data, p)
+
+    def create_extra_data(self, data: Item) -> Any | None:
         return None
 
-    def wrap_data(self, updater_data: DataUpdater.DataGroup) -> DynamicData:
+    def wrap_dynamic(self, updater_data: DataUpdater.DataGroup) -> DynamicItem:
         '''
         以供传入 :meth:`~.Timeline.register_dynamic_data` 使用
         '''
-        def wrapper(global_t: float) -> Item.Data:
+        def wrapper(global_t: float) -> Item:
             alpha = self.get_alpha_on_global_t(global_t)
-            data_copy = updater_data.orig_data._copy(updater_data.orig_data)
+            data_copy = updater_data.orig_data.store()
 
-            with UpdaterParams(global_t,
+            with UpdaterParams(self,
+                               global_t,
                                alpha,
                                self.global_range,
                                updater_data.extra_data) as params:
-                self.func(data_copy, params)
+                self.call(data_copy, params)
 
             return data_copy
+
         return wrapper
 
     def anim_init(self) -> None:
-        def build_data(data: Item.Data) -> DataUpdater.DataGroup:
-            return DataUpdater.DataGroup(data, data._copy(data), self.create_extra_data(data))
+        def build_data(data: Item) -> DataUpdater.DataGroup:
+            return DataUpdater.DataGroup(data, data.store(), self.create_extra_data(data))
 
         self.datas: dict[Item, DataUpdater.DataGroup] = {
             item: build_data(
-                self.timeline.get_stored_data_at_right(
-                    item,
-                    self.global_range.at,
-                    skip_dynamic_data=True
-                )
-            )
-            for item in (
-                [self.item]
-                if self.root_only
-                else self.item.walk_self_and_descendants()
+                item.current(as_time=self.global_range.at,
+                             skip_dynamic=True)
             )
+            for item in self.item.walk_self_and_descendants(self.root_only)
             if not self.skip_null_items or not item.is_null()
         }
 
         for item, updater_data in self.datas.items():
             if self.become_at_end:
-                with UpdaterParams(self.global_range.end,
+                with UpdaterParams(self,
+                                   self.global_range.end,
                                    1,
                                    self.global_range,
                                    updater_data.extra_data) as params:
-                    self.func(item.ref_data(), params)
-            self.timeline.register_dynamic_data(item, self.wrap_data(updater_data), self.global_range.at)
+                    self.call(item, params)
 
-        self.timeline.detect_changes([self.item] if self.root_only else self.item.walk_self_and_descendants(),
-                                     as_time=self.global_range.end - ANIM_END_DELTA)
+            self.timeline.register_dynamic(item,
+                                           self.wrap_dynamic(updater_data),
+                                           item.store() if self.become_at_end else None,
+                                           self.global_range.at,
+                                           self.global_range.end - ANIM_END_DELTA,
+                                           not self.become_at_end)
 
         self.set_render_call_list([
             RenderCall(
-                updater_data.data.cmpt.depth,
+                updater_data.data.depth,
                 updater_data.data.render
             )
             for updater_data in self.datas.values()
         ])
 
         # 在动画开始时自动隐藏，在动画结束时自动显示
         # 可以将 ``hide_on_begin`` 和 ``show_on_end`` 置为 ``False`` 以禁用
@@ -158,21 +171,22 @@
         if self.show_at_end:
             self.timeline.schedule(self.global_range.end, self.item.show, root_only=self.root_only)
 
     def anim_on_alpha(self, alpha: float) -> None:
         global_t = self.global_t_ctx.get()
         for i, updater_data in enumerate(self.datas.values()):
             sub_alpha = self.get_sub_alpha(alpha, i)
-            updater_data.data._restore(updater_data.orig_data)
+            updater_data.data.restore(updater_data.orig_data)
 
-            with UpdaterParams(global_t,
+            with UpdaterParams(self,
+                               global_t,
                                sub_alpha,
                                self.global_range,
                                updater_data.extra_data) as params:
-                self.func(updater_data.data, params)
+                self.call(updater_data.data, params)
 
     def get_sub_alpha(
         self,
         alpha: float,
         index: int
     ) -> float:
         '''依据 ``lag_ratio`` 得到特定子物件的 ``sub_alpha``'''
@@ -180,14 +194,15 @@
         lag_ratio = self.lag_ratio
         full_length = (len(self.datas) - 1) * lag_ratio + 1
         value = alpha * full_length
         lower = index * lag_ratio
         return clip((value - lower), 0, 1)
 
 
+# TODO: optimize
 class ItemUpdater(Animation):
     '''
     以时间为参数显示物件
 
     也就是说，在 :class:`ItemUpdater` 执行时，对于每帧，都会执行 ``func``，并显示 ``func`` 返回的物件
 
     在默认情况下：
@@ -218,14 +233,16 @@
         self.become_at_end = become_at_end
 
     def call(self, p: UpdaterParams) -> Item:
         ret = self.func(p)
         if not isinstance(ret, Item):
             raise UpdaterError(f'传入 ItemUpdater 的函数必须以一个物件作为返回值，而返回的是 {ret}，'
                                f'函数定义于 {inspect.getfile(self.func)}:{inspect.getsourcelines(self.func)[1]}')
+        for item in ret.walk_self_and_descendants():
+            item.is_temporary = True
         return ret
 
     def anim_init(self) -> None:
         if self.item is None:
             return
 
         # 在动画开始时自动隐藏，在动画结束时自动显示
@@ -236,26 +253,27 @@
             self.timeline.schedule(self.global_range.end, self.item.show)
 
         # 在动画结束后，自动使用动画最后一帧的物件替换原有的
         if self.become_at_end:
             self.timeline.schedule(self.global_range.end, self.scheduled_become)
 
     def scheduled_become(self) -> None:
-        with UpdaterParams(self.global_range.end,
+        with UpdaterParams(self,
+                           self.global_range.end,
                            1,
                            self.global_range,
                            None) as params:
             self.item.become(self.call(params))
 
     def anim_on_alpha(self, alpha: float) -> None:
         global_t = self.global_t_ctx.get()
 
-        with UpdaterParams(global_t, alpha, self.global_range, None) as params:
+        with UpdaterParams(self, global_t, alpha, self.global_range, None) as params:
             dynamic = self.call(params)
 
         self.set_render_call_list([
             RenderCall(
                 sub.depth,
-                sub.ref_data().render
+                sub.render
             )
             for sub in dynamic.walk_self_and_descendants()
         ])
```

### Comparing `janim-0.5.2/janim/camera/camera.py` & `janim-1.0.0/janim/camera/camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,16 +48,16 @@
         self.size = other.size
         self.fov = other.fov
         # 有无更好的复制方法？
         self.orientation = Rotation.from_rotvec(other.orientation.as_rotvec())
 
         return self
 
-    def __eq__(self, other: Cmpt_CameraPoints) -> Self:
-        if not super().__eq__(other):
+    def not_changed(self, other: Cmpt_CameraPoints) -> Self:
+        if not super().not_changed(other):
             return False
         if np.any(self.size != other.size) or self.fov != other.fov:
             return False
         return np.all(self.orientation.as_quat() == other.orientation.as_quat())
 
     def interpolate(
         self,
```

### Comparing `janim-0.5.2/janim/camera/camera_info.py` & `janim-1.0.0/janim/camera/camera_info.py`

 * *Files identical despite different names*

### Comparing `janim-0.5.2/janim/cli.py` & `janim-1.0.0/janim/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import importlib.machinery
+import inspect
 import os
 import platform
 import subprocess as sp
 import time
 from argparse import Namespace
 
 from janim.anims.timeline import Timeline
@@ -77,16 +78,17 @@
 
     both = not args.video and not args.audio
 
     log.info('======')
 
     for anim in built:
         name = anim.timeline.__class__.__name__
+        relative_path = os.path.dirname(inspect.getfile(anim.timeline.__class__))
 
-        output_dir = os.path.normpath(anim.cfg.output_dir)
+        output_dir = os.path.normpath(anim.cfg.formated_output_dir(relative_path))
         if not os.path.exists(output_dir):
             os.makedirs(output_dir)
 
         if both or args.video:
             log.info(f'fps={anim.cfg.fps}')
             log.info(f'resolution="{anim.cfg.pixel_width}x{anim.cfg.pixel_height}"')
             log.info(f'format="{args.format}"')
@@ -94,24 +96,24 @@
             log.info(f'audio_format="{args.audio_format}"')
             log.info(f'audio_framerate="{anim.cfg.audio_framerate}"')
         log.info(f'output_dir="{output_dir}"')
 
         if both or args.video:
             writer = VideoWriter(anim)
             writer.write_all(
-                os.path.join(anim.cfg.output_dir,
+                os.path.join(output_dir,
                              f'{name}.{args.format}')
             )
             if args.open and anim is built[-1]:
                 open_file(writer.final_file_path)
 
         if (both or args.audio) and anim.timeline.has_audio():
             writer = AudioWriter(anim)
             writer.write_all(
-                os.path.join(anim.cfg.output_dir,
+                os.path.join(output_dir,
                              f'{name}.{args.audio_format}')
             )
 
     log.info('======')
 
 
 def modify_default_config(args: Namespace) -> None:
```

### Comparing `janim-0.5.2/janim/components/component.py` & `janim-1.0.0/janim/components/component.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import copy
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, Callable, Self, overload
+from typing import TYPE_CHECKING, Callable, Generator, Self, overload
 
 import janim.utils.refresh as refresh
 from janim.exception import CmptGroupLookupError
 from janim.utils.data import AlignedData
 
 if TYPE_CHECKING:   # pragma: no cover
     from janim.items.item import Item
@@ -18,15 +18,15 @@
         name: str,
         bases: tuple[type, ...],
         attrdict: dict,
         *,
         impl=False,     # 若 impl=True，则会跳过下面的检查
     ):
         if not impl:
-            for key in ('copy', 'become', '__eq__'):
+            for key in ('copy', 'become', 'not_changed'):
                 if not callable(attrdict.get(key, None)):
                     raise AttributeError(f'Component 的每一个子类都必须继承并实现 `{key}` 方法，而 {name} 没有')
         return super().__new__(cls, name, bases, attrdict)
 
 
 class Component[ItemT](refresh.Refreshable, metaclass=_CmptMeta):
     @dataclass
@@ -58,40 +58,32 @@
             # item.cmpt2.bind_info 与 BindInfo(MyItem, item, 'cmpt2') 一致
 
             item2 = MyItem2()
 
             # item2.cmpt1.bind_info 与 BindInfo(MyItem, item2, 'cmpt1') 一致
             # item2.cmpt3.bind_info 与 BindInfo(MyItem2, item2, 'cmpt3') 一致
         '''
-        decl_cls: type
+        decl_cls: type[Item]
         at_item: Item
         key: str
 
     def __init__(self) -> None:
         super().__init__()
-
         self.bind: Component.BindInfo | None = None
 
-    def init_bind(self, bind: BindInfo):
+    def init_bind(self, bind: BindInfo) -> None:
         '''
         用于 ``Item._init_components``
 
         子类可以继承该函数，进行与所在物件相关的处理
         '''
         self.bind = bind
 
-    def copy(self) -> Self:
-        cmpt_copy = copy.copy(self)
-        cmpt_copy.bind = None
-        cmpt_copy.reset_refresh()
-        return cmpt_copy
-
-    def become(self, other) -> Self: ...
-
-    def __eq__(self, other) -> bool: ...
+    def fallback_check(self) -> bool:
+        return self.bind is not None and self.bind.at_item.stored
 
     def mark_refresh(self, func: Callable | str, *, recurse_up=False, recurse_down=False) -> Self:
         '''
         详见： :meth:`~.Item.broadcast_refresh_of_component`
         '''
         super().mark_refresh(func)
 
@@ -99,30 +91,66 @@
             self.bind.at_item.broadcast_refresh_of_component(
                 self,
                 func,
                 recurse_up=recurse_up,
                 recurse_down=recurse_down
             )
 
+    def copy(self) -> Self:
+        cmpt_copy = copy.copy(self)
+        # cmpt_copy.bind = None
+        cmpt_copy.reset_refresh()
+        return cmpt_copy
+
+    def become(self, other) -> Self: ...
+
+    def not_changed(self, other) -> bool: ...
+
     def get_same_cmpt(self, item: Item) -> Self:
         return self.get_same_cmpt_if_exists(item) or getattr(item.astype(self.bind.decl_cls), self.bind.key)
 
     def get_same_cmpt_without_mock(self, item: Item) -> Self | None:
-        # TODO: refactor
         return item.components.get(self.bind.key, None)
 
     def get_same_cmpt_if_exists(self, item: Item) -> Self | None:
         cmpt = item.components.get(self.bind.key, None)
         if cmpt is not None:
             return cmpt
-        cmpt = item._astype_mock_cmpt.get(self.bind.key, None)
-        return cmpt
+
+        return item._astype_mock_cmpt.get(self.bind.key, None)
+
+    def walk_same_cmpt_of_self_and_descendants_without_mock(
+        self,
+        root_only: bool = False,
+        *,
+        timed: bool = False
+    ) -> Generator[Self, None, None]:
+        yield self
+        if root_only or self.bind is None:
+            return
+
+        item = self.bind.at_item
+        walk = None
+        if not item.stored:
+            walk = item.walk_descendants(self.bind.decl_cls)
+        elif timed:
+            walk = item._walk_lst(self.bind.decl_cls, item._current_family(up=False))
+
+        if walk is not None:
+            for item in walk:
+                cmpt = self.get_same_cmpt_without_mock(item)
+                if cmpt is None:
+                    continue
+                yield cmpt
 
     @property
     def r(self) -> ItemT:
+        '''
+        所位于的物件，便于链式调用同物件下其它的组件
+        '''
         return self.bind.at_item
 
 
 class CmptInfo[T]:
     '''
     在类中定义组件需要使用该类
 
@@ -179,23 +207,23 @@
         }
 
         return cmpt_copy
 
     def become(self, other) -> Self:    # pragma: no cover
         return self
 
-    def __eq__(self, other: _CmptGroup) -> bool:
-        for key in self.objects.keys():
-            if self.objects[key] != other.objects[key]:
+    def not_changed(self, other: _CmptGroup) -> bool:
+        for key, obj in self.objects.items():
+            if not obj.not_changed(other.objects[key]):
                 return False
 
         return True
 
     @classmethod
-    def align(cls, cmpt1: _CmptGroup, cmpt2: _CmptGroup, aligned: AlignedData[Item.Data]):
+    def align(cls, cmpt1: _CmptGroup, cmpt2: _CmptGroup, aligned: AlignedData[Item]):
         cmpt1_copy = cmpt1.copy(new_cmpts=aligned.data1.components)
         cmpt2_copy = cmpt2.copy(new_cmpts=aligned.data2.components)
         cmpt_union = cmpt1.copy(new_cmpts=aligned.union.components)
         return AlignedData(cmpt1_copy, cmpt2_copy, cmpt_union)
 
     def _find_objects(self) -> None:
         self.objects: dict[str, Component] = {}
@@ -210,20 +238,20 @@
         for key, val in self.bind.decl_cls.__dict__.get(CLS_CMPTINFO_NAME, {}).items():
             if val is cmpt_info:
                 return key
 
         raise CmptGroupLookupError('CmptGroup 必须要与传入的内容在同一个类的定义中')
 
     def __getattr__(self, name: str):
-        objects = []
-        methods = []
-
         if name == 'objects':
             raise AttributeError()
 
+        objects = []
+        methods = []
+
         for obj in self.objects.values():
             if not hasattr(obj, name):
                 continue
 
             attr = getattr(obj, name)
             if not callable(attr):
                 continue
```

### Comparing `janim-0.5.2/janim/components/data.py` & `janim-1.0.0/janim/components/data.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,42 +2,42 @@
 
 from typing import Callable, Self
 
 from janim.components.component import Component
 from janim.utils.data import AlignedData
 
 type CopyFn[T] = Callable[[T], T]
-type EqFn[T] = Callable[[T, T], bool]
+type MaybeSameFn[T] = Callable[[T, T], bool]
 type InterpolateFn[T] = Callable[[T, T, float], T]
 
 
 class Cmpt_Data[ItemT, T](Component[ItemT]):
     '''
     详见 :class:`~.ValueTracker`
     '''
     def __init__(self):
         self.copy_func: CopyFn[T] = None
-        self.eq_func: EqFn[T] = None
+        self.maybe_same_func: MaybeSameFn[T] = None
         self.interpolate_func: InterpolateFn[T] = None
 
     def copy(self) -> Self:
         cmpt_copy = super().copy()
 
         assert self.copy_func is not None
         cmpt_copy.set(self.copy_func(self.value))
 
         return cmpt_copy
 
     def become(self, other: Cmpt_Data) -> Self:
         self.set(other.copy_func(other.value))
         return self
 
-    def __eq__(self, other: Cmpt_Data) -> bool:
-        assert self.eq_func is not None
-        return self.eq_func(self.value, other.value)
+    def not_changed(self, other: Cmpt_Data) -> bool:
+        assert self.maybe_same_func is not None
+        return self.maybe_same_func(self.value, other.value)
 
     @classmethod
     def align_for_interpolate(cls, cmpt1: Cmpt_Data, cmpt2: Cmpt_Data) -> AlignedData[Self]:
         cmpt1_copy = cmpt1.copy()
         cmpt2_copy = cmpt2.copy()
         return AlignedData(cmpt1_copy, cmpt2_copy, cmpt1_copy.copy())
 
@@ -61,17 +61,17 @@
     def get(self) -> T:
         '''得到当前数据'''
         return self.value
 
     def set_func(
         self,
         copy_func: CopyFn[T] | None = None,
-        eq_func: EqFn[T] | None = None,
+        maybe_same_func: MaybeSameFn[T] | None = None,
         interpolate_func: InterpolateFn[T] | None = None
     ) -> Self:
         if copy_func is not None:
             self.copy_func = copy_func
-        if eq_func is not None:
-            self.eq_func = eq_func
+        if maybe_same_func is not None:
+            self.maybe_same_func = maybe_same_func
         if interpolate_func is not None:
             self.interpolate_func = interpolate_func
         return self
```

### Comparing `janim-0.5.2/janim/components/depth.py` & `janim-1.0.0/janim/components/depth.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,25 +34,26 @@
     d2、d3、d1
 
     也就是 d3 会盖住 d2；d1 会盖住 d2 和 d3
     '''
     _counter: defaultdict[float, int] = defaultdict(int)
 
     def __init__(self, value: float, order: int | None = None):
+        super().__init__()
         self.set(value, order=order)
 
     def copy(self) -> Self:
         # Component.copy 中的 copy.copy(self) 已将 _value 和 _order 拷贝
         return super().copy()
 
     def become(self, other: Cmpt_Depth) -> Self:
         self.set(*other.get_raw())
         return self
 
-    def __eq__(self, other: Cmpt_Depth) -> bool:
+    def not_changed(self, other: Cmpt_Depth) -> bool:
         return self._depth == other._depth and self._order == other._order
 
     def __lt__(self, other: Cmpt_Depth) -> bool:
         if self._depth != other._depth:
             return self._depth < other._depth
         return self._order < other._order
 
@@ -63,14 +64,17 @@
         self._depth = value
         if order is None:
             order = self._counter[value]
             self._counter[value] -= 1
         self._order = order
         return self
 
+    def get(self) -> float:
+        return self._depth
+
     def get_raw(self) -> tuple[float, int]:
         '''
         返回元组 ``(depth, order)``
         '''
         return (self._depth, self._order)
 
     def arrange(self, depth: float | None = None) -> Self:
```

### Comparing `janim-0.5.2/janim/components/image.py` & `janim-1.0.0/janim/components/image.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         # self.min_mag_filter 已通过父方法 copy.copy 复制
         return super().copy()
 
     def become(self, other: Cmpt_Image) -> Self:
         self.set(other.img, other.min_mag_filter)
         return self
 
-    def __eq__(self, other: Cmpt_Image) -> bool:
+    def not_changed(self, other: Cmpt_Image) -> bool:
         return id(self.img) == id(other.img) and self.min_mag_filter == other.min_mag_filter
 
     def set(self, img: Image.Image | None, min_mag_filter: int | None) -> Self:
         '''
         设置 PIL 图像
         '''
         if img is not None:
```

### Comparing `janim-0.5.2/janim/components/points.py` & `janim-1.0.0/janim/components/points.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,35 +11,36 @@
                              DEFAULT_ITEM_TO_ITEM_BUFF, DOWN, IN, LEFT,
                              MED_SMALL_BUFF, ORIGIN, OUT, PI, RIGHT, UP)
 from janim.exception import InvaildMatrixError, PointError
 from janim.items.item import Item
 from janim.typing import Vect, VectArray
 from janim.utils.bezier import integer_interpolate, interpolate
 from janim.utils.config import Config
-from janim.utils.data import AlignedData
+from janim.utils.data import AlignedData, Array
 from janim.utils.iterables import resize_and_repeatedly_extend
 from janim.utils.paths import PathFunc, straight_path
 from janim.utils.signal import Signal
 from janim.utils.space_ops import angle_of_vector, get_norm, rotation_matrix
-from janim.utils.unique_nparray import UniqueNparray
 
 type PointsFn = Callable[[np.ndarray], VectArray]
 type PointFn = Callable[[np.ndarray], Vect]
 type ComplexFn = Callable[[complex], complex]
 
+DEFAULT_POINTS_DATA = np.zeros((0, 3))
+
 
 class Cmpt_Points[ItemT](Component[ItemT]):
     resize_func = staticmethod(resize_and_repeatedly_extend)
     ''''''
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-        self._points = UniqueNparray()
-        self.clear()
+        self._points = Array()
+        self._points.data = DEFAULT_POINTS_DATA
 
     def init_bind(self, bind: Component.BindInfo):
         super().init_bind(bind)
 
         item = bind.at_item
 
         item.__class__.children_changed.connect_refresh(item, self, Cmpt_Points.box.fget)
@@ -50,15 +51,15 @@
         return cmpt_copy
 
     def become(self, other: Cmpt_Points) -> Self:
         self._points = other._points.copy()
         Cmpt_Points.set.emit(self)
         return self
 
-    def __eq__(self, other: Cmpt_Points) -> bool:
+    def not_changed(self, other: Cmpt_Points) -> bool:
         return self._points.is_share(other._points)
 
     @classmethod
     def align_for_interpolate(cls, cmpt1: Cmpt_Points, cmpt2: Cmpt_Points) -> AlignedData[Self]:
         len1, len2 = len(cmpt1.get()), len(cmpt2.get())
 
         cmpt1_copy = cmpt1.copy()
@@ -75,15 +76,15 @@
         self,
         cmpt1: Self,
         cmpt2: Self,
         alpha: float,
         *,
         path_func: PathFunc = straight_path
     ) -> None:
-        if cmpt1 == cmpt2:
+        if cmpt1.not_changed(cmpt2):
             return
 
         self.set(path_func(cmpt1.get(), cmpt2.get(), alpha))
 
     # region 点数据 | Points
 
     def get(self) -> np.ndarray:
@@ -92,23 +93,18 @@
         '''
         return self._points.data
 
     def get_all(self) -> np.ndarray:
         '''
         得到自己以及后代物件的所有点坐标数据
         '''
-        point_datas = [self.get()]
-
-        if self.bind is not None:
-            for item in self.bind.at_item.walk_descendants(self.bind.decl_cls):
-                cmpt = self.get_same_cmpt_without_mock(item)
-                if cmpt is None:
-                    continue
-                point_datas.append(cmpt.get())
-
+        point_datas = [
+            cmpt.get()
+            for cmpt in self.walk_same_cmpt_of_self_and_descendants_without_mock(timed=True)
+        ]
         return np.vstack(point_datas)
 
     @Signal
     def set(self, points: VectArray) -> Self:
         '''
         设置点坐标数据，每个坐标点都有三个分量
 
@@ -130,15 +126,15 @@
             Cmpt_Points.set.emit(self, key='count')
         Cmpt_Points.set.emit(self)
 
         return self
 
     def clear(self) -> Self:
         '''清除点'''
-        self.set(np.zeros((0, 3)))
+        self.set(DEFAULT_POINTS_DATA)
         return self
 
     def extend(self, points: VectArray) -> Self:
         '''
         追加点坐标数据，每个坐标点都有三个分量
 
         使用形如 ``.append([[1.5, 3, 2], [2, 1.5, 0]])`` 的形式
@@ -173,31 +169,31 @@
         return self.count() > 0
 
     def get_start(self) -> np.ndarray:
         '''
         得到 ``points`` 的第一个点
         '''
         self._raise_error_if_no_points()
-        return self._points._data[0].copy()
+        return self._points.data[0]
 
     def get_end(self) -> np.ndarray:
         '''
         得到 ``points`` 的最后一个点
         '''
         self._raise_error_if_no_points()
-        return self._points._data[-1].copy()
+        return self._points.data[-1]
 
     def get_start_and_end(self) -> tuple[np.ndarray, np.ndarray]:
         '''
         得到 ``points`` 的第一个和最后一个点
         '''
         return (self.get_start(), self.get_end())
 
     def point_from_proportion(self, alpha: float) -> np.ndarray:
-        points = self._points._data
+        points = self._points.data
         i, subalpha = integer_interpolate(0, len(points) - 1, alpha)
         return interpolate(points[i], points[i + 1], subalpha)
 
     def pfp(self, alpha) -> np.ndarray:
         '''``point_from_proportion`` 的缩写'''
         return self.point_from_proportion(alpha)
 
@@ -209,32 +205,24 @@
 
     # endregion
 
     # region 边界框 | Bounding box
 
     @property
     @set.self_refresh_with_recurse(recurse_up=True)
-    @refresh.register
+    @refresh.register(fallback_check=Component.fallback_check)
     def box(self) -> BoundingBox:
         '''
         表示物件（包括后代物件）的矩形包围框
         '''
-        box_datas = []
-
-        if self.has():
-            box_datas.append(self.self_box.data)
-
-        if self.bind is not None:
-            for item in self.bind.at_item.walk_descendants(self.bind.decl_cls):
-                cmpt = self.get_same_cmpt_without_mock(item)
-                if cmpt is None or not cmpt.has():
-                    continue
-
-                box_datas.append(cmpt.self_box.data)
-
+        box_datas = [
+            cmpt.self_box.data
+            for cmpt in self.walk_same_cmpt_of_self_and_descendants_without_mock(timed=True)
+            if cmpt.has()
+        ]
         return self.BoundingBox(np.vstack(box_datas) if box_datas else [])
 
     @property
     @set.self_refresh()
     @refresh.register
     def self_box(self) -> BoundingBox:
         '''
@@ -382,46 +370,36 @@
     @Signal
     def apply_points_fn(
         self,
         func: PointsFn,
         *,
         about_point: Vect | None = None,
         about_edge: Vect | None = ORIGIN,
-        root_only: bool = False,
+        root_only: bool = False
     ) -> Self:
         '''
         将所有点作为单独的一个参数传入 ``func``，并将 ``func`` 返回的结果作为新的点坐标数据
 
         视 ``about_point`` 为原点，若其为 ``None``，则将物件在 ``about_edge`` 方向上的边界作为 ``about_point``
         '''
         if about_point is None and about_edge is not None:
             if root_only:
                 about_point = self.self_box.get(about_edge)
             else:
                 about_point = self.box.get(about_edge)
 
-        def apply(cmpt: Cmpt_Points):
+        for cmpt in self.walk_same_cmpt_of_self_and_descendants_without_mock(root_only):
             if cmpt.has():
                 if about_point is None:
                     cmpt.set(func(cmpt.get()))
                 else:
                     cmpt.set(func(cmpt.get() - about_point) + about_point)
 
             Cmpt_Points.apply_points_fn.emit(cmpt, func, about_point)
 
-        apply(self)
-
-        if not root_only and self.bind is not None:
-            for item in self.bind.at_item.walk_descendants(self.bind.decl_cls):
-                cmpt = self.get_same_cmpt_without_mock(item)
-                if cmpt is None:
-                    continue
-
-                apply(cmpt)
-
         return self
 
     def apply_point_fn(
         self,
         func: PointFn,
         *,
         about_point: Vect | None = ORIGIN,
```

### Comparing `janim-0.5.2/janim/components/radius.py` & `janim-1.0.0/janim/components/radius.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,40 +2,39 @@
 
 from typing import Iterable, Self
 
 import numpy as np
 
 from janim.components.component import Component
 from janim.utils.bezier import interpolate
-from janim.utils.data import AlignedData
+from janim.utils.data import AlignedData, Array
 from janim.utils.iterables import resize_with_interpolation
-from janim.utils.unique_nparray import UniqueNparray
 
 
 class Cmpt_Radius[ItemT](Component[ItemT]):
     '''
     半径组件，被用于 :class:`DotCloud` 的点半径，以及 :class:`VItem` 的轮廓线粗细
     '''
     def __init__(self, default_radius: float, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.default_radius = default_radius
 
-        self._radii = UniqueNparray()
-        self.clear()
+        self._radii = Array()
+        self._radii.data = np.full(1, self.default_radius)
 
     def copy(self) -> Self:
         cmpt_copy = super().copy()
         cmpt_copy._radii = self._radii.copy()
         return cmpt_copy
 
     def become(self, other: Cmpt_Radius) -> Self:
         self.set(other.get())
         return self
 
-    def __eq__(self, other: Cmpt_Radius) -> bool:
+    def not_changed(self, other: Cmpt_Radius) -> bool:
         return self._radii.is_share(other._radii)
 
     @classmethod
     def align_for_interpolate(cls, cmpt1: Cmpt_Radius, cmpt2: Cmpt_Radius):
         len1, len2 = len(cmpt1.get()), len(cmpt2.get())
 
         cmpt1_copy = cmpt1.copy()
@@ -45,15 +44,15 @@
             cmpt1_copy.resize(len2)
         elif len1 > len2:
             cmpt1_copy.resize(len1)
 
         return AlignedData(cmpt1_copy, cmpt2_copy, cmpt1_copy.copy())
 
     def interpolate(self, cmpt1: Cmpt_Radius, cmpt2: Cmpt_Radius, alpha: float, *, path_func=None) -> None:
-        if cmpt1 == cmpt2:
+        if cmpt1.not_changed(cmpt2):
             return
 
         self.set(interpolate(cmpt1.get(), cmpt2.get(), alpha))
 
     # region 半径数据 | Radii
 
     def get(self) -> np.ndarray:
@@ -69,23 +68,19 @@
         root_only: bool = False,
     ) -> Self:
         '''
         设置半径数据
         '''
         if not isinstance(radius, Iterable):
             radius = [radius]
-        radii = np.array(radius)
+        radii = Array()
+        radii.data = radius
 
-        self._radii.data = radii
-        if not root_only and self.bind is not None:
-            for item in self.bind.at_item.walk_descendants(self.bind.decl_cls):
-                cmpt = self.get_same_cmpt_without_mock(item)
-                if cmpt is None:
-                    continue
-                cmpt._radii._data = radii
+        for cmpt in self.walk_same_cmpt_of_self_and_descendants_without_mock(root_only):
+            cmpt._radii.data = radii
 
         return self
 
     def clear(self) -> Self:
         '''
         将半径数据重置为默认值
         '''
```

### Comparing `janim-0.5.2/janim/components/rgbas.py` & `janim-1.0.0/janim/components/rgbas.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,39 +4,40 @@
 
 import numpy as np
 from colour import Color
 
 from janim.components.component import Component
 from janim.typing import Alpha, AlphaArray, ColorArray, JAnimColor, RgbaArray
 from janim.utils.bezier import interpolate
-from janim.utils.data import AlignedData
+from janim.utils.data import AlignedData, Array
 from janim.utils.iterables import resize_with_interpolation
-from janim.utils.unique_nparray import UniqueNparray
+
+DEFAULT_RGBAS_DATA = np.full((1, 4), 1)
 
 
 class Cmpt_Rgbas[ItemT](Component[ItemT]):
     '''
     颜色组件
     '''
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-        self._rgbas = UniqueNparray()
-        self.clear()
+        self._rgbas = Array()
+        self._rgbas.data = DEFAULT_RGBAS_DATA
 
     def copy(self) -> Self:
         cmpt_copy = super().copy()
         cmpt_copy._rgbas = self._rgbas.copy()
         return cmpt_copy
 
     def become(self, other: Cmpt_Rgbas) -> Self:
         self.set(other.get())
         return self
 
-    def __eq__(self, other: Cmpt_Rgbas) -> bool:
+    def not_changed(self, other: Cmpt_Rgbas) -> bool:
         return self._rgbas.is_share(other._rgbas)
 
     @classmethod
     def align_for_interpolate(cls, cmpt1: Cmpt_Rgbas, cmpt2: Cmpt_Rgbas):
         len1, len2 = len(cmpt1.get()), len(cmpt2.get())
 
         cmpt1_copy = cmpt1.copy()
@@ -46,15 +47,15 @@
             cmpt1_copy.resize(len2)
         elif len1 > len2:
             cmpt1_copy.resize(len1)
 
         return AlignedData(cmpt1_copy, cmpt2_copy, cmpt1_copy.copy())
 
     def interpolate(self, cmpt1: Cmpt_Rgbas, cmpt2: Cmpt_Rgbas, alpha: float, *, path_func=None) -> None:
-        if cmpt1 == cmpt2:
+        if cmpt1.not_changed(cmpt2):
             return
 
         self.set(interpolate(cmpt1.get(), cmpt2.get(), alpha))
 
     # region 颜色数据 | Colors
 
     def get(self) -> np.ndarray:
@@ -144,54 +145,41 @@
             alpha = [alpha]
 
         if alpha is None and not isinstance(color[0], str) and len(color[0]) == 4:
             rgbas = self.format_rgbas(color)
 
             self.set_rgbas(rgbas)
 
-            if not root_only and self.bind is not None:
-                for item in self.bind.at_item.walk_descendants(self.bind.decl_cls):
-                    cmpt = self.get_same_cmpt_without_mock(item)
-                    if cmpt is None:
-                        continue
-                    cmpt.set_rgbas(rgbas)
+            for cmpt in self.walk_same_cmpt_of_self_and_descendants_without_mock(root_only):
+                cmpt.set_rgbas(rgbas)
+
         else:
             if color is not None:
                 color = self.format_colors(color)
             if alpha is not None:
                 alpha = self.format_alphas(alpha)
 
-            def set_to(cmpt: Cmpt_Rgbas):
+            for cmpt in self.walk_same_cmpt_of_self_and_descendants_without_mock(root_only):
                 cmpt_color = cmpt.get()[:, :3] if color is None else color
                 cmpt_alpha = cmpt.get()[:, 3] if alpha is None else alpha
                 length = max(len(cmpt_color), len(cmpt_alpha))
 
                 rgbas = np.hstack([
                     resize_with_interpolation(cmpt_color.astype(float), length),
                     resize_with_interpolation(cmpt_alpha.astype(float), length).reshape((length, 1))
                 ])
                 cmpt.set_rgbas(rgbas)
 
-            set_to(self)
-
-            if not root_only and self.bind is not None:
-                for item in self.bind.at_item.walk_descendants(self.bind.decl_cls):
-                    cmpt = self.get_same_cmpt_without_mock(item)
-                    if cmpt is None:
-                        continue
-
-                    set_to(cmpt)
-
         return self
 
     def clear(self) -> Self:
         '''
         将颜色数据重置为默认值
         '''
-        self.set(np.full((1, 4), 1))
+        self.set(DEFAULT_RGBAS_DATA)
         return self
 
     def reverse(self) -> Self:
         self.set_rgbas(self.get()[::-1])
         return self
 
     def resize(self, length: int) -> Self:
@@ -201,36 +189,26 @@
     def count(self) -> int:
         return len(self.get())
 
     def apart_alpha(self, n: int) -> Self:
         '''
         对每一个颜色数据应用 :func:`~.apart_alpha`
         '''
-        rgbas = self.get()
+        rgbas = self.get().copy()
         for i in range(len(rgbas)):
             rgbas[i, 3] = apart_alpha(rgbas[i, 3], n)
         self.set_rgbas(rgbas)
         return self
 
     def fade(self, factor: float | Iterable[float], *, root_only: bool = False) -> Self:
-        def fade_on(cmpt: Cmpt_Rgbas):
-            rgbas = cmpt.get()
+        for cmpt in self.walk_same_cmpt_of_self_and_descendants_without_mock(root_only):
+            rgbas = cmpt.get().copy()
             rgbas[:, 3] *= 1 - factor
             cmpt.set_rgbas(rgbas)
 
-        fade_on(self)
-
-        if not root_only and self.bind is not None:
-            for item in self.bind.at_item.walk_descendants(self.bind.decl_cls):
-                cmpt = self.get_same_cmpt_without_mock(item)
-                if cmpt is None:
-                    continue
-
-                fade_on(cmpt)
-
         return self
 
     # endregion
 
 
 def merge_alpha(alpha: float, n: int) -> float:
     '''
```

### Comparing `janim-0.5.2/janim/components/vpoints.py` & `janim-1.0.0/janim/components/vpoints.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
                                 integer_interpolate, inverse_interpolate,
                                 partial_quadratic_bezier_points,
                                 smooth_quadratic_path)
 from janim.utils.data import AlignedData
 from janim.utils.space_ops import get_norm, get_unit_normal
 
 
-class Cmpt_VPoints[ItemT](Cmpt_Points[ItemT]):
+class Cmpt_VPoints[ItemT](Cmpt_Points[ItemT], impl=True):
     '''
     曲线点坐标数据
 
     - 每三个点表示一段二阶贝塞尔曲线，并且前后相接的曲线共用公共点。
 
       例如对于点坐标列表 ``[a, b, c, d, e, f, g]``，则表示这些曲线：``[a, b, c]`` ``[c, d, e]`` ``[e, f, g]``
 
@@ -37,71 +37,56 @@
 
       只有闭合的子路径，才能够进行填充色的渲染
     '''
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.make_smooth_after_applying_functions = False
 
-    def copy(self) -> Self:
-        return super().copy()
-
-    def become(self, other: Cmpt_VPoints) -> Self:
-        super().become(other)
-        return self
-
-    def __eq__(self, other: Cmpt_VPoints) -> bool:
-        return super().__eq__(other)
-
     def set(self, points: VectArray) -> Self:
         if len(points) != 0 and len(points) % 2 == 0:
             log.warning(f'设置的点数量为 {len(points)}，不是奇数，最后一个点被忽略')
             points = points[:-1]
         super().set(points)
         return self
 
     def apply_points_fn(
         self,
         func: PointsFn,
         *,
         about_point: Vect | None = None,
         about_edge: Vect | None = ORIGIN,
-        root_only: bool = False,
+        root_only: bool = False
     ) -> Self:
         super().apply_points_fn(
             func,
             about_point=about_point,
             about_edge=about_edge,
             root_only=root_only
         )
-        if root_only or self.bind is None:
-            if self.make_smooth_after_applying_functions:
-                self.make_approximately_smooth()
-        else:
-            for item in self.bind.at_item.walk_self_and_descendants():
-                cmpt = self.get_same_cmpt_without_mock(item)
-                if not isinstance(cmpt, Cmpt_VPoints) or not cmpt.make_smooth_after_applying_functions:
-                    continue
-                cmpt.make_approximately_smooth()
+        for cmpt in self.walk_same_cmpt_of_self_and_descendants_without_mock(root_only):
+            if not isinstance(cmpt, Cmpt_VPoints) or not cmpt.make_smooth_after_applying_functions:
+                continue
+            cmpt.make_approximately_smooth()
 
         return self
 
     # region align
 
     @classmethod
     def align_for_interpolate(cls, cmpt1: Cmpt_VPoints, cmpt2: Cmpt_VPoints) -> AlignedData[Self]:
         cmpt1_copy = cmpt1.copy()
         cmpt2_copy = cmpt2.copy()
 
-        if cmpt1_copy == cmpt2_copy:
+        if cmpt1_copy.not_changed(cmpt2_copy):
             return AlignedData(cmpt1_copy, cmpt2_copy, cmpt1_copy.copy())
 
         if not cmpt1_copy.has():
-            cmpt1_copy.set([cmpt2.box.center])
+            cmpt1_copy.set([cmpt2.self_box.center])
         if not cmpt2_copy.has():
-            cmpt2_copy.set([cmpt1.box.center])
+            cmpt2_copy.set([cmpt1.self_box.center])
 
         subpaths1 = cmpt1_copy.get_subpaths()
         subpaths2 = cmpt2_copy.get_subpaths()
 
         # 如果都只有单个路径，直接对齐就可以了
         # 否则进行路径之间的配对，以便对齐数据
         if len(subpaths1) == len(subpaths2) == 1:
@@ -240,29 +225,20 @@
             alphas = np.linspace(0, 1, n_inserts + 2)
             for a1, a2 in zip(alphas, alphas[1:]):
                 new_points.extend(partial_quadratic_bezier_points(tup, a1, a2)[1:])
 
         return np.vstack(new_points)
 
     def insert_n_curves(self, n: int, root_only=False) -> Self:
-        def apply(cmpt: Cmpt_VPoints) -> None:
-            if cmpt.curves_count() == 0:
-                return
+        for cmpt in self.walk_same_cmpt_of_self_and_descendants_without_mock(root_only):
+            if not isinstance(cmpt, Cmpt_VPoints) or cmpt.curves_count() == 0:
+                continue
             points = cmpt.insert_n_curves_to_point_list(n, cmpt.get())
             cmpt.set(points)
 
-        if root_only or self.bind is None:
-            apply(self)
-        else:
-            for item in self.bind.at_item.walk_self_and_descendants():
-                cmpt = self.get_same_cmpt_without_mock(item)
-                if not isinstance(cmpt, Cmpt_VPoints):
-                    continue
-                apply(cmpt)
-
         return self
 
     # endregion
 
     # region anchors and handles
 
     def get_anchors(self) -> np.ndarray:
@@ -275,38 +251,38 @@
         '''
         得到曲线的控制点
         '''
         return self.get()[1::2]
 
     @property
     def start_direction(self) -> np.ndarray:
-        points = self._points._data
+        points = self._points.data
         start = points[0]
         for pos in points[1:]:
             if not np.isclose(start, pos).all():
                 return pos - start
         return RIGHT
 
     @property
     def end_direction(self) -> np.ndarray:
-        points = self._points._data
+        points = self._points.data
         end = points[-1]
         for pos in points[-2::-1]:
             if not np.isclose(end, pos).all():
                 return end - pos
         return RIGHT
 
     def close_path(self) -> Self:
         self._raise_error_if_no_points()
         indices = self.get_subpath_end_indices()
         end = self.get_end()
         if len(indices) == 1:
             point = self.get_start()
         else:
-            point = self._points._data[indices[-2] + 2]
+            point = self._points.data[indices[-2] + 2]
         self.extend([(end + point) * 0.5, point])
         return self
 
     @staticmethod
     def get_bezier_tuples_from_points(points: VectArray) -> Iterable[np.ndarray]:
         '''
         由 ``points`` 得到由每一组贝塞尔曲线控制点组成的列表
@@ -330,15 +306,15 @@
 
     def get_nth_curve_points(self, n: int) -> VectArray:
         '''
         得到第 ``n`` 组的贝塞尔曲线控制点 (从 0 开始计数)
         '''
         if n < 0 or n >= self.curves_count():
             raise PointError(f'n 必须是 0~{self.curves_count() - 1} 的值，{n} 无效')
-        return self._points._data[2 * n: 2 * n + 3].copy()
+        return self._points.data[2 * n: 2 * n + 3]
 
     def get_nth_curve_function(self, n: int) -> Callable[[float], np.ndarray]:
         '''
         返回值是第 ``n`` 组贝塞尔曲线的描点函数，传入 [0, 1] 之间的值，得到对应的在曲线上的点
         '''
         return bezier(self.get_nth_curve_points(n))
 
@@ -470,57 +446,52 @@
     def change_anchor_mode(self, mode: AnchorMode) -> Self:
         if not self.has():
             return self
 
         subpaths = self.get_subpaths()
         self.clear()
         for subpath in subpaths:
+            new_subpath = subpath.copy()
             anchors = subpath[::2]
             match mode:
                 case AnchorMode.Jagged:
-                    subpath[1::2] = 0.5 * (anchors[:-1] + anchors[1:])
+                    new_subpath[1::2] = 0.5 * (anchors[:-1] + anchors[1:])
                 case AnchorMode.ApproxSmooth:
-                    subpath[1::2] = approx_smooth_quadratic_bezier_handles(anchors)
+                    new_subpath[1::2] = approx_smooth_quadratic_bezier_handles(anchors)
                 case AnchorMode.TrueSmooth:
-                    subpath = smooth_quadratic_path(anchors)
-            self.add_subpath(subpath)
+                    new_subpath = smooth_quadratic_path(anchors)
+            self.add_subpath(new_subpath)
         return self
 
     def make_smooth(self, approx=False, root_only=False) -> Self:
         '''
         Edits the path so as to pass smoothly through all
         the current anchor points.
 
         If approx is False, this may increase the total
         number of points.
         '''
         mode = AnchorMode.ApproxSmooth if approx else AnchorMode.TrueSmooth
-        if root_only or self.bind is None:
-            self.change_anchor_mode(mode)
-        else:
-            for item in self.bind.at_item.walk_self_and_descendants():
-                cmpt = self.get_same_cmpt_without_mock(item)
-                if not isinstance(cmpt, Cmpt_VPoints):
-                    continue
-                cmpt.change_anchor_mode(mode)
+        for cmpt in self.walk_same_cmpt_of_self_and_descendants_without_mock(root_only):
+            if not isinstance(cmpt, Cmpt_VPoints):
+                continue
+            cmpt.change_anchor_mode(mode)
+
         return self
 
     def make_approximately_smooth(self, root_only=False) -> Self:
         self.make_smooth(approx=True, root_only=root_only)
         return self
 
     def make_jagged(self, root_only=False) -> Self:
-        if root_only or self.bind is None:
-            self.change_anchor_mode(AnchorMode.Jagged)
-        else:
-            for item in self.bind.at_item.walk_self_and_descendants():
-                cmpt = self.get_same_cmpt_without_mock(item)
-                if not isinstance(cmpt, Cmpt_VPoints):
-                    continue
-                cmpt.change_anchor_mode(AnchorMode.Jagged)
+        for cmpt in self.walk_same_cmpt_of_self_and_descendants_without_mock(root_only):
+            if not isinstance(cmpt, Cmpt_VPoints):
+                continue
+            cmpt.change_anchor_mode(AnchorMode.Jagged)
+
         return self
 
     # endregion
 
     # region unit_normal
 
     @staticmethod
```

### Comparing `janim-0.5.2/janim/constants/colors.py` & `janim-1.0.0/janim/constants/colors.py`

 * *Files identical despite different names*

### Comparing `janim-0.5.2/janim/examples.py` & `janim-1.0.0/janim/examples.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         self.play(Rotate(item1, -90 * DEGREES))
         self.forward(0.5)
 
         item2 = VItem(LEFT, UP, RIGHT, DOWN, LEFT)
         item2.color.set(BLUE)
         item2.fill.set(alpha=0.2)
 
-        state = self.camera.store_data()
+        state = self.camera.copy()
         self.play(self.camera.anim.points.scale(0.5))
         self.play(self.camera.anim.become(state))
 
         self.play(
             Transform(item1, item2),
             duration=2
         )
@@ -127,36 +127,35 @@
 
 class UpdaterExample(Timeline):
     def construct(self) -> None:
         square = Square(fill_color=BLUE_E, fill_alpha=1).show()
         brace = Brace(square, UP).show()
 
         def text_updater(p: UpdaterParams):
-            cmpt = self.t2d(brace).cmpt.points
+            cmpt = brace.current().points
             return cmpt.create_text(f'Width = {cmpt.brace_length:.2f}')
 
         self.prepare(
             DataUpdater(
                 brace,
-                lambda data, p: data.cmpt.points.match(self.t2d(square))
+                lambda data, p: data.points.match(square.current())
             ),
             ItemUpdater(None, text_updater),
             duration=10
         )
         self.forward()
         self.play(square.anim.points.scale(2))
         self.play(square.anim.points.scale(0.5))
         self.play(square.anim.points.set_width(5, stretch=True))
 
         w0 = square.points.box.width
 
         self.play(
             DataUpdater(
                 square,
-                lambda data, p: data.cmpt.points.set_width(
+                lambda data, p: data.points.set_width(
                     w0 + 0.5 * w0 * math.sin(p.alpha * p.range.duration)
                 )
             ),
             duration=5
         )
         self.forward()
-
```

### Comparing `janim-0.5.2/janim/exception.py` & `janim-1.0.0/janim/exception.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,16 +40,16 @@
     会直接以 ``exit_code`` 退出，不输出 ``traceback`` 信息
     '''
     exit_code: int
 
 
 class TimelineError(JAnimException): ...
 class TimelineLookupError(TimelineError): ...
-class StoreFailedError(TimelineError): ...
-class StoreNotFoundError(TimelineError): ...
+class RecordFailedError(TimelineError): ...
+class RecordNotFoundError(TimelineError): ...
 class NotAnimationError(TimelineError): ...
 
 
 class UpdaterError(JAnimException): ...
 
 
 class CmptGroupLookupError(JAnimException): ...
```

### Comparing `janim-0.5.2/janim/gui/anim_viewer.py` & `janim-1.0.0/janim/gui/anim_viewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 try:
-    import PySide6
+    import PySide6  # noqa: F401
 except ImportError:
     print('使用 GUI 界面时需要安装额外模块，但是未安装')
     print('你可以使用 pip install janim[gui] 进行安装，并确保你安装在了正确的 Python 版本中')
 
     from janim.exception import EXITCODE_PYSIDE6_NOT_FOUND, ExitException
     raise ExitException(EXITCODE_PYSIDE6_NOT_FOUND)
 
 import importlib.machinery
 import inspect
 import json
+import math
 import os
 import sys
 import time
 import traceback
 from bisect import bisect
 from dataclasses import dataclass
 
@@ -35,14 +36,15 @@
 from janim.gui.fixed_ratio_widget import FixedRatioWidget
 from janim.gui.glwidget import GLWidget
 from janim.gui.precise_timer import PreciseTimer
 from janim.gui.richtext_editor import RichTextEditor
 from janim.gui.selector import Selector
 from janim.logger import log
 from janim.render.writer import VideoWriter
+from janim.utils.bezier import interpolate
 from janim.utils.file_ops import get_janim_dir
 from janim.utils.simple_functions import clip
 
 TIMELINE_VIEW_MIN_DURATION = 0.5
 
 
 class AnimViewer(QMainWindow):
@@ -365,14 +367,15 @@
         self.setWindowFlag(Qt.WindowType.WindowStaysOnTopHint, flag)
         if visible:
             self.setVisible(True)
 
     def on_rebuild_triggered(self) -> None:
         module = inspect.getmodule(self.anim.timeline)
         progress = self.timeline_view.progress()
+        preview_fps = self.anim.cfg.preview_fps
 
         loader = importlib.machinery.SourceFileLoader(module.__name__, module.__file__)
         module = loader.load_module()
         timeline_class: type[Timeline] = getattr(module, self.anim.timeline.__class__.__name__)
 
         try:
             self.anim: TimelineAnim = timeline_class().build()
@@ -394,14 +397,16 @@
                     *client
                 )
 
             time = self.timeline_view.progress_to_time(self.timeline_view.progress())
             self.send_lineno(self.anim.timeline.get_lineno_at_time(time))
 
         self.setup_audio_player()
+        self.play_timer.duration = 1 / self.anim.cfg.preview_fps
+        progress = int(progress * self.anim.cfg.preview_fps / preview_fps)
 
         self.anim.anim_on(self.timeline_view.progress_to_time(progress))
 
         self.glw.anim = self.anim
         self.glw.update()
 
         range = self.timeline_view.range
@@ -437,15 +442,17 @@
             self.fps_label.setText(f'Preview FPS: {self.fps_counter}/{self.anim.cfg.preview_fps}')
             self.fps_counter = 0
             self.fps_record_start = cur
 
     def on_export_clicked(self) -> None:
         self.play_timer.stop()
 
-        output_dir = self.anim.cfg.output_dir
+        relative_path = os.path.dirname(inspect.getfile(self.anim.timeline.__class__))
+
+        output_dir = self.anim.cfg.formated_output_dir(relative_path)
         if not os.path.exists(output_dir):
             os.makedirs(output_dir)
 
         file_path = QFileDialog.getSaveFileName(
             self,
             '',
             os.path.join(output_dir, f'{self.anim.timeline.__class__.__name__}.mp4'),
@@ -625,19 +632,37 @@
                       range.width,
                       self.label_height).contains(pos):
                 self.hover_at_anim(pos, info.anim)
 
     def hover_at_audio(self, pos: QPoint, info: Timeline.PlayAudioInfo) -> None:
         msg_lst = [
             f'{round(info.range.at, 2)}s ~ {round(info.range.end, 2)}s',
-            info.audio.filepath
+            info.audio.file_path
         ]
         if info.clip_range != TimeRange(0, info.audio.duration()):
             msg_lst.append(f'Clip: {round(info.clip_range.at, 2)}s ~ {round(info.clip_range.end, 2)}s')
 
+        data = info.audio._samples.data
+        indices = np.where(data > np.iinfo(np.int16).max * 0.02)[0]
+        if len(indices) != 0:
+            diff_end_indices = np.where(np.diff(indices) > info.audio.framerate * 0.15)[0]
+
+            starts = [indices[0], *indices[diff_end_indices + 1]]
+            ends = [*indices[diff_end_indices], indices[-1]]
+
+            starts = interpolate(0, info.audio.duration(), np.array(starts) / len(data))
+            ends = interpolate(0, info.audio.duration(), np.array(ends) / len(data))
+
+            clips = ', '.join(
+                f'{math.floor(start * 10) / 10}s ~ {math.ceil(end * 10) / 10}s'
+                for start, end in zip(starts, ends)
+            )
+
+            msg_lst.append(f'Recommended clip: {clips}')
+
         label = QLabel('\n'.join(msg_lst))
         chart_view = self.create_audio_chart(info, near=round(self.pixel_to_time(pos.x())))
 
         layout = QVBoxLayout()
         layout.addWidget(label)
         layout.addWidget(chart_view)
 
@@ -657,35 +682,35 @@
 
         clip_begin = info.clip_range.at
         clip_end = info.clip_range.end
         if near is not None:
             clip_begin = max(clip_begin, near - info.range.at - 4)
             clip_end = min(clip_end, near - info.range.at + 4)
 
-        range_begin = clip_begin + info.range.at
-        range_end = clip_end + info.range.at
+        range_begin = info.range.at + (clip_begin - info.clip_range.at)
+        range_end = range_begin + (clip_end - clip_begin)
 
         begin = int(clip_begin * audio.framerate)
         end = int(clip_end * audio.framerate)
 
         left_blank = max(0, -begin)
         right_blank = max(0, end - audio.sample_count())
 
-        data = audio._samples._data[max(0, begin): min(end, audio.sample_count())]
+        data = audio._samples.data[max(0, begin): min(end, audio.sample_count())]
 
         if left_blank != 0 or right_blank != 0:
             data = np.concatenate([
                 np.zeros(left_blank, dtype=np.int16),
                 data,
                 np.zeros(right_blank, dtype=np.int16)
             ])
 
         unit = audio.framerate // self.anim.cfg.fps
 
-        data = np.max(
+        data: np.ndarray = np.max(
             np.abs(
                 data[:len(data) // unit * unit].reshape(-1, unit)
             ),
             axis=1
         ) / np.iinfo(np.int16).max
 
         times = np.linspace(range_begin,
@@ -822,15 +847,15 @@
             self.set_range(
                 self.range.at + shift,
                 self.range.duration
             )
 
             self.update()
 
-    def set_progress(self, progress: float) -> None:
+    def set_progress(self, progress: int) -> None:
         progress = clip(progress, 0, self._maximum)
         if progress != self._progress:
             self._progress = progress
 
             pixel_at = self.progress_to_pixel(progress)
             minimum = self.play_space
             maximum = self.width() - self.play_space
```

### Comparing `janim-0.5.2/janim/gui/audio_player.py` & `janim-1.0.0/janim/gui/audio_player.py`

 * *Files identical despite different names*

### Comparing `janim-0.5.2/janim/gui/export.png` & `janim-1.0.0/janim/gui/export.png`

 * *Files identical despite different names*

### Comparing `janim-0.5.2/janim/gui/fixed_ratio_widget.py` & `janim-1.0.0/janim/gui/fixed_ratio_widget.py`

 * *Files identical despite different names*

### Comparing `janim-0.5.2/janim/gui/glwidget.py` & `janim-1.0.0/janim/gui/glwidget.py`

 * *Files identical despite different names*

### Comparing `janim-0.5.2/janim/gui/precise_timer.py` & `janim-1.0.0/janim/gui/precise_timer.py`

 * *Files identical despite different names*

### Comparing `janim-0.5.2/janim/gui/richtext_editor.py` & `janim-1.0.0/janim/gui/richtext_editor.py`

 * *Files identical despite different names*

### Comparing `janim-0.5.2/janim/gui/selector.py` & `janim-1.0.0/janim/gui/selector.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,556 +1,521 @@
 00000000: 0d0a 6672 6f6d 2064 6174 6163 6c61 7373  ..from dataclass
 00000010: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
 00000020: 6173 730d 0a66 726f 6d20 7479 7069 6e67  ass..from typing
 00000030: 2069 6d70 6f72 7420 5459 5045 5f43 4845   import TYPE_CHE
-00000040: 434b 494e 470d 0a0d 0a69 6d70 6f72 7420  CKING....import 
-00000050: 6e75 6d70 7920 6173 206e 700d 0a66 726f  numpy as np..fro
-00000060: 6d20 5079 5369 6465 362e 5174 436f 7265  m PySide6.QtCore
-00000070: 2069 6d70 6f72 7420 5145 7665 6e74 2c20   import QEvent, 
-00000080: 514f 626a 6563 742c 2051 506f 696e 7446  QObject, QPointF
-00000090: 2c20 5152 6563 7446 2c20 5174 0d0a 6672  , QRectF, Qt..fr
-000000a0: 6f6d 2050 7953 6964 6536 2e51 7447 7569  om PySide6.QtGui
-000000b0: 2069 6d70 6f72 7420 5143 6f6c 6f72 2c20   import QColor, 
-000000c0: 514d 6f75 7365 4576 656e 742c 2051 5061  QMouseEvent, QPa
-000000d0: 696e 7465 722c 2051 5061 696e 7445 7665  inter, QPaintEve
-000000e0: 6e74 0d0a 0d0a 6672 6f6d 206a 616e 696d  nt....from janim
-000000f0: 2e61 6e69 6d73 2e64 6973 706c 6179 2069  .anims.display i
-00000100: 6d70 6f72 7420 4469 7370 6c61 790d 0a66  mport Display..f
-00000110: 726f 6d20 6a61 6e69 6d2e 636f 6d70 6f6e  rom janim.compon
-00000120: 656e 7473 2e70 6f69 6e74 7320 696d 706f  ents.points impo
-00000130: 7274 2043 6d70 745f 506f 696e 7473 0d0a  rt Cmpt_Points..
-00000140: 6672 6f6d 206a 616e 696d 2e69 7465 6d73  from janim.items
-00000150: 2e69 7465 6d20 696d 706f 7274 2049 7465  .item import Ite
-00000160: 6d0d 0a66 726f 6d20 6a61 6e69 6d2e 6974  m..from janim.it
-00000170: 656d 732e 706f 696e 7473 2069 6d70 6f72  ems.points impor
-00000180: 7420 506f 696e 7473 0d0a 0d0a 6966 2054  t Points....if T
-00000190: 5950 455f 4348 4543 4b49 4e47 3a0d 0a20  YPE_CHECKING:.. 
-000001a0: 2020 2066 726f 6d20 6a61 6e69 6d2e 6775     from janim.gu
-000001b0: 692e 616e 696d 5f76 6965 7765 7220 696d  i.anim_viewer im
-000001c0: 706f 7274 2041 6e69 6d56 6965 7765 720d  port AnimViewer.
-000001d0: 0a0d 0a0d 0a63 6c61 7373 2053 656c 6563  .....class Selec
-000001e0: 746f 7228 514f 626a 6563 7429 3a0d 0a20  tor(QObject):.. 
-000001f0: 2020 2027 2727 0d0a 2020 2020 e5ad 90e7     '''..    ....
-00000200: 89a9 e4bb b6e9 8089 e68b a9e5 b7a5 e585  ................
-00000210: b70d 0a20 2020 2027 2727 0d0a 2020 2020  ...    '''..    
-00000220: 4064 6174 6163 6c61 7373 0d0a 2020 2020  @dataclass..    
-00000230: 636c 6173 7320 5365 6c65 6374 6564 4974  class SelectedIt
-00000240: 656d 3a0d 0a20 2020 2020 2020 2069 7465  em:..        ite
-00000250: 6d3a 2049 7465 6d0d 0a20 2020 2020 2020  m: Item..       
-00000260: 206d 696e 5f67 6c78 3a20 666c 6f61 740d   min_glx: float.
-00000270: 0a20 2020 2020 2020 206d 696e 5f67 6c79  .        min_gly
-00000280: 3a20 666c 6f61 740d 0a20 2020 2020 2020  : float..       
-00000290: 206d 6178 5f67 6c78 3a20 666c 6f61 740d   max_glx: float.
-000002a0: 0a20 2020 2020 2020 206d 6178 5f67 6c79  .        max_gly
-000002b0: 3a20 666c 6f61 740d 0a0d 0a20 2020 2064  : float....    d
-000002c0: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-000002d0: 2c20 7061 7265 6e74 3a20 2741 6e69 6d56  , parent: 'AnimV
-000002e0: 6965 7765 7227 2920 2d3e 204e 6f6e 653a  iewer') -> None:
-000002f0: 0d0a 2020 2020 2020 2020 7375 7065 7228  ..        super(
-00000300: 292e 5f5f 696e 6974 5f5f 2870 6172 656e  ).__init__(paren
-00000310: 7429 0d0a 2020 2020 2020 2020 7365 6c66  t)..        self
-00000320: 2e76 6965 7765 7220 3d20 7061 7265 6e74  .viewer = parent
-00000330: 0d0a 0d0a 2020 2020 2020 2020 7365 6c66  ....        self
-00000340: 2e76 6965 7765 722e 676c 772e 696e 7374  .viewer.glw.inst
-00000350: 616c 6c45 7665 6e74 4669 6c74 6572 2873  allEventFilter(s
-00000360: 656c 6629 0d0a 2020 2020 2020 2020 7365  elf)..        se
-00000370: 6c66 2e76 6965 7765 722e 6f76 6572 6c61  lf.viewer.overla
-00000380: 792e 696e 7374 616c 6c45 7665 6e74 4669  y.installEventFi
-00000390: 6c74 6572 2873 656c 6629 0d0a 0d0a 2020  lter(self)....  
-000003a0: 2020 2020 2020 7365 6c66 2e63 6c65 6172        self.clear
-000003b0: 2829 0d0a 0d0a 2020 2020 6465 6620 636c  ()....    def cl
-000003c0: 6561 7228 7365 6c66 2920 2d3e 204e 6f6e  ear(self) -> Non
-000003d0: 653a 0d0a 2020 2020 2020 2020 7365 6c66  e:..        self
-000003e0: 2e63 7572 7265 6e74 3a20 5365 6c65 6374  .current: Select
-000003f0: 6f72 2e53 656c 6563 7465 6449 7465 6d20  or.SelectedItem 
-00000400: 7c20 4e6f 6e65 203d 204e 6f6e 650d 0a20  | None = None.. 
-00000410: 2020 2020 2020 2073 656c 662e 6368 696c         self.chil
-00000420: 6472 656e 3a20 6c69 7374 5b53 656c 6563  dren: list[Selec
-00000430: 746f 722e 5365 6c65 6374 6564 4974 656d  tor.SelectedItem
-00000440: 5d20 3d20 5b5d 0d0a 2020 2020 2020 2020  ] = []..        
-00000450: 7365 6c66 2e73 656c 6563 7465 645f 6368  self.selected_ch
-00000460: 696c 6472 656e 3a20 6c69 7374 5b53 656c  ildren: list[Sel
-00000470: 6563 746f 722e 5365 6c65 6374 6564 4974  ector.SelectedIt
-00000480: 656d 5d20 3d20 5b5d 0d0a 2020 2020 2020  em] = []..      
-00000490: 2020 7365 6c66 2e76 6965 7765 722e 6f76    self.viewer.ov
-000004a0: 6572 6c61 792e 7570 6461 7465 2829 0d0a  erlay.update()..
-000004b0: 0d0a 2020 2020 6465 6620 676c 785f 746f  ..    def glx_to
-000004c0: 5f6f 7665 726c 6179 5f78 2873 656c 662c  _overlay_x(self,
-000004d0: 2067 6c78 3a20 666c 6f61 7429 202d 3e20   glx: float) -> 
-000004e0: 666c 6f61 743a 0d0a 2020 2020 2020 2020  float:..        
-000004f0: 7265 7475 726e 2028 676c 7820 2b20 3129  return (glx + 1)
-00000500: 202f 2032 202a 2073 656c 662e 7669 6577   / 2 * self.view
-00000510: 6572 2e6f 7665 726c 6179 2e77 6964 7468  er.overlay.width
-00000520: 2829 0d0a 0d0a 2020 2020 6465 6620 676c  ()....    def gl
-00000530: 795f 746f 5f6f 7665 726c 6179 5f79 2873  y_to_overlay_y(s
-00000540: 656c 662c 2067 6c79 3a20 666c 6f61 7429  elf, gly: float)
-00000550: 202d 3e20 666c 6f61 743a 0d0a 2020 2020   -> float:..    
-00000560: 2020 2020 7265 7475 726e 2028 2d67 6c79      return (-gly
-00000570: 202b 2031 2920 2f20 3220 2a20 7365 6c66   + 1) / 2 * self
-00000580: 2e76 6965 7765 722e 6f76 6572 6c61 792e  .viewer.overlay.
-00000590: 6865 6967 6874 2829 0d0a 0d0a 2020 2020  height()....    
-000005a0: 6465 6620 6765 745f 706f 696e 7473 5f62  def get_points_b
-000005b0: 6f78 5f6f 665f 7469 6d65 2873 656c 662c  ox_of_time(self,
-000005c0: 2069 7465 6d3a 2049 7465 6d2c 2074 3a20   item: Item, t: 
-000005d0: 666c 6f61 7429 202d 3e20 436d 7074 5f50  float) -> Cmpt_P
-000005e0: 6f69 6e74 732e 426f 756e 6469 6e67 426f  oints.BoundingBo
-000005f0: 783a 0d0a 2020 2020 2020 2020 626f 785f  x:..        box_
-00000600: 6461 7461 7320 3d20 5b0d 0a20 2020 2020  datas = [..     
-00000610: 2020 2020 2020 2073 656c 662e 7669 6577         self.view
-00000620: 6572 2e61 6e69 6d2e 7469 6d65 6c69 6e65  er.anim.timeline
-00000630: 2e67 6574 5f73 746f 7265 645f 6461 7461  .get_stored_data
-00000640: 5f61 745f 7269 6768 7428 0d0a 2020 2020  _at_right(..    
-00000650: 2020 2020 2020 2020 2020 2020 7375 622c              sub,
-00000660: 2074 2c20 736b 6970 5f64 796e 616d 6963   t, skip_dynamic
-00000670: 5f64 6174 613d 5472 7565 0d0a 2020 2020  _data=True..    
-00000680: 2020 2020 2020 2020 292e 636d 7074 2e70          ).cmpt.p
-00000690: 6f69 6e74 732e 7365 6c66 5f62 6f78 2e64  oints.self_box.d
-000006a0: 6174 610d 0a0d 0a20 2020 2020 2020 2020  ata....         
-000006b0: 2020 2066 6f72 2073 7562 2069 6e20 6974     for sub in it
-000006c0: 656d 2e77 616c 6b5f 7365 6c66 5f61 6e64  em.walk_self_and
-000006d0: 5f64 6573 6365 6e64 616e 7473 2829 0d0a  _descendants()..
-000006e0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-000006f0: 7369 6e73 7461 6e63 6528 7375 622c 2050  sinstance(sub, P
-00000700: 6f69 6e74 7329 2061 6e64 2073 7562 2e70  oints) and sub.p
-00000710: 6f69 6e74 732e 6861 7328 290d 0a20 2020  oints.has()..   
-00000720: 2020 2020 205d 0d0a 2020 2020 2020 2020       ]..        
-00000730: 7265 7475 726e 2043 6d70 745f 506f 696e  return Cmpt_Poin
-00000740: 7473 2e42 6f75 6e64 696e 6742 6f78 286e  ts.BoundingBox(n
-00000750: 702e 7673 7461 636b 2862 6f78 5f64 6174  p.vstack(box_dat
-00000760: 6173 2920 6966 2062 6f78 5f64 6174 6173  as) if box_datas
-00000770: 2065 6c73 6520 5b5d 290d 0a0d 0a20 2020   else [])....   
-00000780: 2064 6566 2065 7665 6e74 4669 6c74 6572   def eventFilter
-00000790: 2873 656c 662c 2077 6174 6368 6564 3a20  (self, watched: 
-000007a0: 514f 626a 6563 742c 2065 7665 6e74 3a20  QObject, event: 
-000007b0: 5145 7665 6e74 2920 2d3e 2062 6f6f 6c3a  QEvent) -> bool:
-000007c0: 0d0a 2020 2020 2020 2020 6966 2077 6174  ..        if wat
-000007d0: 6368 6564 2069 7320 7365 6c66 2e76 6965  ched is self.vie
-000007e0: 7765 722e 676c 773a 0d0a 2020 2020 2020  wer.glw:..      
-000007f0: 2020 2020 2020 6966 2065 7665 6e74 2e74        if event.t
-00000800: 7970 6528 2920 696e 2028 5145 7665 6e74  ype() in (QEvent
-00000810: 2e54 7970 652e 4d6f 7573 6542 7574 746f  .Type.MouseButto
-00000820: 6e50 7265 7373 2c20 5145 7665 6e74 2e54  nPress, QEvent.T
-00000830: 7970 652e 4d6f 7573 6542 7574 746f 6e44  ype.MouseButtonD
-00000840: 626c 436c 6963 6b29 3a0d 0a20 2020 2020  blClick):..     
-00000850: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00000860: 6f6e 5f67 6c77 5f6d 6f75 7365 5f70 7265  on_glw_mouse_pre
-00000870: 7373 2865 7665 6e74 290d 0a20 2020 2020  ss(event)..     
-00000880: 2020 2020 2020 2069 6620 6576 656e 742e         if event.
-00000890: 7479 7065 2829 203d 3d20 5145 7665 6e74  type() == QEvent
-000008a0: 2e54 7970 652e 4d6f 7573 654d 6f76 653a  .Type.MouseMove:
-000008b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000008c0: 2020 7365 6c66 2e6f 6e5f 676c 775f 6d6f    self.on_glw_mo
-000008d0: 7573 655f 6d6f 7665 2865 7665 6e74 290d  use_move(event).
-000008e0: 0a0d 0a20 2020 2020 2020 2069 6620 7761  ...        if wa
-000008f0: 7463 6865 6420 6973 2073 656c 662e 7669  tched is self.vi
-00000900: 6577 6572 2e6f 7665 726c 6179 3a0d 0a20  ewer.overlay:.. 
-00000910: 2020 2020 2020 2020 2020 2069 6620 6576             if ev
-00000920: 656e 742e 7479 7065 2829 203d 3d20 5145  ent.type() == QE
-00000930: 7665 6e74 2e54 7970 652e 5061 696e 743a  vent.Type.Paint:
-00000940: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000950: 2020 7365 6c66 2e6f 6e5f 6f76 6572 6c61    self.on_overla
-00000960: 795f 7061 696e 7428 6576 656e 7429 0d0a  y_paint(event)..
-00000970: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00000980: 2073 7570 6572 2829 2e65 7665 6e74 4669   super().eventFi
-00000990: 6c74 6572 2877 6174 6368 6564 2c20 6576  lter(watched, ev
-000009a0: 656e 7429 0d0a 0d0a 2020 2020 6465 6620  ent)....    def 
-000009b0: 6f6e 5f67 6c77 5f6d 6f75 7365 5f70 7265  on_glw_mouse_pre
-000009c0: 7373 2873 656c 662c 2065 7665 6e74 3a20  ss(self, event: 
-000009d0: 514d 6f75 7365 4576 656e 7429 202d 3e20  QMouseEvent) -> 
-000009e0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2069  None:..        i
-000009f0: 6620 6576 656e 742e 6d6f 6469 6669 6572  f event.modifier
-00000a00: 7328 2920 2620 5174 2e4b 6579 626f 6172  s() & Qt.Keyboar
-00000a10: 644d 6f64 6966 6965 722e 436f 6e74 726f  dModifier.Contro
-00000a20: 6c4d 6f64 6966 6965 723a 0d0a 2020 2020  lModifier:..    
-00000a30: 2020 2020 2020 2020 6d61 7463 6820 6576          match ev
-00000a40: 656e 742e 6275 7474 6f6e 2829 3a0d 0a20  ent.button():.. 
-00000a50: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00000a60: 6173 6520 5174 2e4d 6f75 7365 4275 7474  ase Qt.MouseButt
-00000a70: 6f6e 2e4c 6566 7442 7574 746f 6e3a 0d0a  on.LeftButton:..
-00000a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a90: 2020 2020 7365 6c66 2e73 656c 6563 745f      self.select_
-00000aa0: 7061 7265 6e74 5f69 7465 6d28 6576 656e  parent_item(even
-00000ab0: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
-00000ac0: 2020 2020 6361 7365 2051 742e 4d6f 7573      case Qt.Mous
-00000ad0: 6542 7574 746f 6e2e 5269 6768 7442 7574  eButton.RightBut
-00000ae0: 746f 6e3a 0d0a 2020 2020 2020 2020 2020  ton:..          
-00000af0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-00000b00: 656c 6574 654c 6174 6572 2829 0d0a 2020  eleteLater()..  
-00000b10: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00000b20: 2020 2020 2020 2020 206d 6174 6368 2065           match e
-00000b30: 7665 6e74 2e62 7574 746f 6e28 293a 0d0a  vent.button():..
-00000b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b50: 6361 7365 2051 742e 4d6f 7573 6542 7574  case Qt.MouseBut
-00000b60: 746f 6e2e 4c65 6674 4275 7474 6f6e 3a0d  ton.LeftButton:.
-00000b70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000b80: 2020 2020 2073 656c 662e 7365 6c65 6374       self.select
-00000b90: 5f63 6869 6c64 5f69 7465 6d28 6576 656e  _child_item(even
-00000ba0: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
-00000bb0: 2020 2020 6361 7365 2051 742e 4d6f 7573      case Qt.Mous
-00000bc0: 6542 7574 746f 6e2e 5269 6768 7442 7574  eButton.RightBut
-00000bd0: 746f 6e3a 0d0a 2020 2020 2020 2020 2020  ton:..          
-00000be0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-00000bf0: 656d 6f76 655f 6368 696c 645f 6974 656d  emove_child_item
-00000c00: 2865 7665 6e74 290d 0a0d 0a20 2020 2020  (event)....     
-00000c10: 2020 2073 656c 662e 7669 6577 6572 2e6f     self.viewer.o
-00000c20: 7665 726c 6179 2e75 7064 6174 6528 290d  verlay.update().
-00000c30: 0a0d 0a20 2020 2064 6566 206f 6e5f 676c  ...    def on_gl
-00000c40: 775f 6d6f 7573 655f 6d6f 7665 2873 656c  w_mouse_move(sel
-00000c50: 662c 2065 7665 6e74 3a20 514d 6f75 7365  f, event: QMouse
-00000c60: 4576 656e 7429 202d 3e20 4e6f 6e65 3a0d  Event) -> None:.
-00000c70: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00000c80: 6576 656e 742e 6d6f 6469 6669 6572 7328  event.modifiers(
-00000c90: 2920 2620 5174 2e4b 6579 626f 6172 644d  ) & Qt.KeyboardM
-00000ca0: 6f64 6966 6965 722e 436f 6e74 726f 6c4d  odifier.ControlM
-00000cb0: 6f64 6966 6965 723a 0d0a 2020 2020 2020  odifier:..      
-00000cc0: 2020 2020 2020 6d61 7463 6820 6576 656e        match even
-00000cd0: 742e 6275 7474 6f6e 7328 293a 0d0a 2020  t.buttons():..  
-00000ce0: 2020 2020 2020 2020 2020 2020 2020 6361                ca
-00000cf0: 7365 2051 742e 4d6f 7573 6542 7574 746f  se Qt.MouseButto
-00000d00: 6e2e 4c65 6674 4275 7474 6f6e 3a0d 0a20  n.LeftButton:.. 
-00000d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d20: 2020 2073 656c 662e 7365 6c65 6374 5f63     self.select_c
-00000d30: 6869 6c64 5f69 7465 6d28 6576 656e 7429  hild_item(event)
-00000d40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000d50: 2020 6361 7365 2051 742e 4d6f 7573 6542    case Qt.MouseB
-00000d60: 7574 746f 6e2e 5269 6768 7442 7574 746f  utton.RightButto
-00000d70: 6e3a 0d0a 2020 2020 2020 2020 2020 2020  n:..            
-00000d80: 2020 2020 2020 2020 7365 6c66 2e72 656d          self.rem
-00000d90: 6f76 655f 6368 696c 645f 6974 656d 2865  ove_child_item(e
-00000da0: 7665 6e74 290d 0a0d 0a20 2020 2020 2020  vent)....       
-00000db0: 2020 2020 2073 656c 662e 7669 6577 6572       self.viewer
-00000dc0: 2e6f 7665 726c 6179 2e75 7064 6174 6528  .overlay.update(
-00000dd0: 290d 0a0d 0a20 2020 2064 6566 2073 656c  )....    def sel
-00000de0: 6563 745f 7061 7265 6e74 5f69 7465 6d28  ect_parent_item(
-00000df0: 7365 6c66 2c20 6576 656e 743a 2051 4d6f  self, event: QMo
-00000e00: 7573 6545 7665 6e74 2920 2d3e 204e 6f6e  useEvent) -> Non
-00000e10: 653a 0d0a 2020 2020 2020 2020 7365 6c66  e:..        self
-00000e20: 2e63 6869 6c64 7265 6e2e 636c 6561 7228  .children.clear(
-00000e30: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00000e40: 7365 6c65 6374 6564 5f63 6869 6c64 7265  selected_childre
-00000e50: 6e2e 636c 6561 7228 290d 0a0d 0a20 2020  n.clear()....   
-00000e60: 2020 2020 2078 2c20 7920 3d20 6576 656e       x, y = even
-00000e70: 742e 706f 7369 7469 6f6e 2829 2e74 6f54  t.position().toT
-00000e80: 7570 6c65 2829 0d0a 2020 2020 2020 2020  uple()..        
-00000e90: 676c 7820 3d20 7820 2f20 7365 6c66 2e76  glx = x / self.v
-00000ea0: 6965 7765 722e 676c 772e 7769 6474 6828  iewer.glw.width(
-00000eb0: 2920 2a20 3220 2d20 310d 0a20 2020 2020  ) * 2 - 1..     
-00000ec0: 2020 2067 6c79 203d 2079 202f 2073 656c     gly = y / sel
-00000ed0: 662e 7669 6577 6572 2e67 6c77 2e68 6569  f.viewer.glw.hei
-00000ee0: 6768 7428 2920 2a20 2d32 202b 2031 0d0a  ght() * -2 + 1..
-00000ef0: 0d0a 2020 2020 2020 2020 616e 696d 203d  ..        anim =
-00000f00: 2073 656c 662e 7669 6577 6572 2e61 6e69   self.viewer.ani
-00000f10: 6d0d 0a20 2020 2020 2020 2067 6c6f 6261  m..        globa
-00000f20: 6c5f 7420 3d20 616e 696d 2e5f 7469 6d65  l_t = anim._time
-00000f30: 0d0a 2020 2020 2020 2020 6361 6d65 7261  ..        camera
-00000f40: 5f69 6e66 6f20 3d20 616e 696d 2e74 696d  _info = anim.tim
-00000f50: 656c 696e 652e 6765 745f 7374 6f72 6564  eline.get_stored
-00000f60: 5f64 6174 615f 6174 5f72 6967 6874 2861  _data_at_right(a
-00000f70: 6e69 6d2e 7469 6d65 6c69 6e65 2e63 616d  nim.timeline.cam
-00000f80: 6572 612c 2067 6c6f 6261 6c5f 7429 2e63  era, global_t).c
-00000f90: 6d70 742e 706f 696e 7473 2e69 6e66 6f0d  mpt.points.info.
-00000fa0: 0a0d 0a20 2020 2020 2020 2066 6f75 6e64  ...        found
-00000fb0: 3a20 6c69 7374 5b53 656c 6563 746f 722e  : list[Selector.
-00000fc0: 5365 6c65 6374 6564 4974 656d 5d20 3d20  SelectedItem] = 
-00000fd0: 5b5d 0d0a 0d0a 2020 2020 2020 2020 666f  []....        fo
-00000fe0: 7220 6469 7370 6c61 7920 696e 2061 6e69  r display in ani
-00000ff0: 6d2e 6469 7370 6c61 795f 616e 696d 2e61  m.display_anim.a
-00001000: 6e69 6d73 3a0d 0a20 2020 2020 2020 2020  nims:..         
-00001010: 2020 2064 6973 706c 6179 3a20 4469 7370     display: Disp
-00001020: 6c61 790d 0a20 2020 2020 2020 2020 2020  lay..           
-00001030: 2069 6620 6e6f 7420 6469 7370 6c61 792e   if not display.
-00001040: 676c 6f62 616c 5f72 616e 6765 2e61 7420  global_range.at 
-00001050: 3c3d 2067 6c6f 6261 6c5f 7420 3c20 6469  <= global_t < di
-00001060: 7370 6c61 792e 676c 6f62 616c 5f72 616e  splay.global_ran
-00001070: 6765 2e65 6e64 3a0d 0a20 2020 2020 2020  ge.end:..       
-00001080: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-00001090: 650d 0a0d 0a20 2020 2020 2020 2020 2020  e....           
-000010a0: 2062 6f78 203d 2073 656c 662e 6765 745f   box = self.get_
-000010b0: 706f 696e 7473 5f62 6f78 5f6f 665f 7469  points_box_of_ti
-000010c0: 6d65 2864 6973 706c 6179 2e69 7465 6d2c  me(display.item,
-000010d0: 2067 6c6f 6261 6c5f 7429 0d0a 0d0a 2020   global_t)....  
-000010e0: 2020 2020 2020 2020 2020 6d61 7070 6564            mapped
-000010f0: 203d 2063 616d 6572 615f 696e 666f 2e6d   = camera_info.m
-00001100: 6170 5f70 6f69 6e74 7328 626f 782e 6765  ap_points(box.ge
-00001110: 745f 636f 726e 6572 7328 2929 0d0a 2020  t_corners())..  
-00001120: 2020 2020 2020 2020 2020 6d69 6e5f 676c            min_gl
-00001130: 782c 206d 696e 5f67 6c79 203d 206d 6170  x, min_gly = map
-00001140: 7065 642e 6d69 6e28 6178 6973 3d30 290d  ped.min(axis=0).
-00001150: 0a20 2020 2020 2020 2020 2020 206d 6178  .            max
-00001160: 5f67 6c78 2c20 6d61 785f 676c 7920 3d20  _glx, max_gly = 
-00001170: 6d61 7070 6564 2e6d 6178 2861 7869 733d  mapped.max(axis=
-00001180: 3029 0d0a 2020 2020 2020 2020 2020 2020  0)..            
-00001190: 6966 206e 6f74 206d 696e 5f67 6c78 203c  if not min_glx <
-000011a0: 3d20 676c 7820 3c3d 206d 6178 5f67 6c78  = glx <= max_glx
-000011b0: 206f 7220 6e6f 7420 6d69 6e5f 676c 7920   or not min_gly 
-000011c0: 3c3d 2067 6c79 203c 3d20 6d61 785f 676c  <= gly <= max_gl
-000011d0: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
-000011e0: 2020 2020 636f 6e74 696e 7565 0d0a 0d0a      continue....
-000011f0: 2020 2020 2020 2020 2020 2020 666f 756e              foun
-00001200: 642e 6170 7065 6e64 2853 656c 6563 746f  d.append(Selecto
-00001210: 722e 5365 6c65 6374 6564 4974 656d 2864  r.SelectedItem(d
-00001220: 6973 706c 6179 2e69 7465 6d2c 206d 696e  isplay.item, min
-00001230: 5f67 6c78 2c20 6d69 6e5f 676c 792c 206d  _glx, min_gly, m
-00001240: 6178 5f67 6c78 2c20 6d61 785f 676c 7929  ax_glx, max_gly)
-00001250: 290d 0a0d 0a20 2020 2020 2020 2069 6620  )....        if 
-00001260: 6e6f 7420 666f 756e 643a 0d0a 2020 2020  not found:..    
-00001270: 2020 2020 2020 2020 7365 6c66 2e63 7572          self.cur
-00001280: 7265 6e74 203d 204e 6f6e 650d 0a20 2020  rent = None..   
-00001290: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-000012a0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000012b0: 6375 7272 656e 7420 6973 204e 6f6e 6520  current is None 
-000012c0: 6f72 2073 656c 662e 6375 7272 656e 7420  or self.current 
-000012d0: 6e6f 7420 696e 2066 6f75 6e64 3a0d 0a20  not in found:.. 
-000012e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000012f0: 656c 662e 6375 7272 656e 7420 3d20 666f  elf.current = fo
-00001300: 756e 645b 305d 0d0a 2020 2020 2020 2020  und[0]..        
-00001310: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00001320: 2020 2020 2020 2020 2020 2069 6478 203d             idx =
-00001330: 2066 6f75 6e64 2e69 6e64 6578 2873 656c   found.index(sel
-00001340: 662e 6375 7272 656e 7429 0d0a 2020 2020  f.current)..    
-00001350: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00001360: 2e63 7572 7265 6e74 203d 2066 6f75 6e64  .current = found
-00001370: 5b28 6964 7820 2b20 3129 2025 206c 656e  [(idx + 1) % len
-00001380: 2866 6f75 6e64 295d 0d0a 0d0a 2020 2020  (found)]....    
-00001390: 2020 2020 2020 2020 666f 7220 6974 656d          for item
-000013a0: 2069 6e20 7365 6c66 2e63 7572 7265 6e74   in self.current
-000013b0: 2e69 7465 6d2e 6368 696c 6472 656e 3a0d  .item.children:.
-000013c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000013d0: 2062 6f78 203d 2073 656c 662e 6765 745f   box = self.get_
-000013e0: 706f 696e 7473 5f62 6f78 5f6f 665f 7469  points_box_of_ti
-000013f0: 6d65 2869 7465 6d2c 2067 6c6f 6261 6c5f  me(item, global_
-00001400: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
-00001410: 2020 2020 6d61 7070 6564 203d 2063 616d      mapped = cam
-00001420: 6572 615f 696e 666f 2e6d 6170 5f70 6f69  era_info.map_poi
-00001430: 6e74 7328 626f 782e 6765 745f 636f 726e  nts(box.get_corn
-00001440: 6572 7328 2929 0d0a 2020 2020 2020 2020  ers())..        
-00001450: 2020 2020 2020 2020 7365 6c66 2e63 6869          self.chi
-00001460: 6c64 7265 6e2e 6170 7065 6e64 2853 656c  ldren.append(Sel
-00001470: 6563 746f 722e 5365 6c65 6374 6564 4974  ector.SelectedIt
-00001480: 656d 2869 7465 6d2c 202a 6d61 7070 6564  em(item, *mapped
-00001490: 2e6d 696e 2861 7869 733d 3029 2c20 2a6d  .min(axis=0), *m
-000014a0: 6170 7065 642e 6d61 7828 6178 6973 3d30  apped.max(axis=0
-000014b0: 2929 290d 0a0d 0a20 2020 2064 6566 2073  )))....    def s
-000014c0: 656c 6563 745f 6368 696c 645f 6974 656d  elect_child_item
-000014d0: 2873 656c 662c 2065 7665 6e74 3a20 514d  (self, event: QM
-000014e0: 6f75 7365 4576 656e 7429 202d 3e20 4e6f  ouseEvent) -> No
-000014f0: 6e65 3a0d 0a20 2020 2020 2020 2078 2c20  ne:..        x, 
-00001500: 7920 3d20 6576 656e 742e 706f 7369 7469  y = event.positi
-00001510: 6f6e 2829 2e74 6f54 7570 6c65 2829 0d0a  on().toTuple()..
-00001520: 2020 2020 2020 2020 676c 7820 3d20 7820          glx = x 
-00001530: 2f20 7365 6c66 2e76 6965 7765 722e 676c  / self.viewer.gl
-00001540: 772e 7769 6474 6828 2920 2a20 3220 2d20  w.width() * 2 - 
-00001550: 310d 0a20 2020 2020 2020 2067 6c79 203d  1..        gly =
-00001560: 2079 202f 2073 656c 662e 7669 6577 6572   y / self.viewer
-00001570: 2e67 6c77 2e68 6569 6768 7428 2920 2a20  .glw.height() * 
-00001580: 2d32 202b 2031 0d0a 0d0a 2020 2020 2020  -2 + 1....      
-00001590: 2020 666f 7220 6368 696c 6420 696e 2073    for child in s
-000015a0: 656c 662e 6368 696c 6472 656e 3a0d 0a20  elf.children:.. 
-000015b0: 2020 2020 2020 2020 2020 2069 6620 6368             if ch
-000015c0: 696c 6420 696e 2073 656c 662e 7365 6c65  ild in self.sele
-000015d0: 6374 6564 5f63 6869 6c64 7265 6e3a 0d0a  cted_children:..
-000015e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015f0: 636f 6e74 696e 7565 0d0a 2020 2020 2020  continue..      
-00001600: 2020 2020 2020 6966 206e 6f74 2063 6869        if not chi
-00001610: 6c64 2e6d 696e 5f67 6c78 203c 3d20 676c  ld.min_glx <= gl
-00001620: 7820 3c3d 2063 6869 6c64 2e6d 6178 5f67  x <= child.max_g
-00001630: 6c78 206f 7220 6e6f 7420 6368 696c 642e  lx or not child.
-00001640: 6d69 6e5f 676c 7920 3c3d 2067 6c79 203c  min_gly <= gly <
-00001650: 3d20 6368 696c 642e 6d61 785f 676c 793a  = child.max_gly:
-00001660: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001670: 2020 636f 6e74 696e 7565 0d0a 2020 2020    continue..    
-00001680: 2020 2020 2020 2020 7365 6c66 2e73 656c          self.sel
-00001690: 6563 7465 645f 6368 696c 6472 656e 2e61  ected_children.a
-000016a0: 7070 656e 6428 6368 696c 6429 0d0a 0d0a  ppend(child)....
-000016b0: 2020 2020 6465 6620 7265 6d6f 7665 5f63      def remove_c
-000016c0: 6869 6c64 5f69 7465 6d28 7365 6c66 2c20  hild_item(self, 
-000016d0: 6576 656e 743a 2051 4d6f 7573 6545 7665  event: QMouseEve
-000016e0: 6e74 2920 2d3e 204e 6f6e 653a 0d0a 2020  nt) -> None:..  
-000016f0: 2020 2020 2020 782c 2079 203d 2065 7665        x, y = eve
-00001700: 6e74 2e70 6f73 6974 696f 6e28 292e 746f  nt.position().to
-00001710: 5475 706c 6528 290d 0a20 2020 2020 2020  Tuple()..       
-00001720: 2067 6c78 203d 2078 202f 2073 656c 662e   glx = x / self.
-00001730: 7669 6577 6572 2e67 6c77 2e77 6964 7468  viewer.glw.width
-00001740: 2829 202a 2032 202d 2031 0d0a 2020 2020  () * 2 - 1..    
-00001750: 2020 2020 676c 7920 3d20 7920 2f20 7365      gly = y / se
-00001760: 6c66 2e76 6965 7765 722e 676c 772e 6865  lf.viewer.glw.he
-00001770: 6967 6874 2829 202a 202d 3220 2b20 310d  ight() * -2 + 1.
-00001780: 0a0d 0a20 2020 2020 2020 2066 6f72 2063  ...        for c
-00001790: 6869 6c64 2069 6e20 7365 6c66 2e73 656c  hild in self.sel
-000017a0: 6563 7465 645f 6368 696c 6472 656e 3a0d  ected_children:.
-000017b0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000017c0: 6e6f 7420 6368 696c 642e 6d69 6e5f 676c  not child.min_gl
-000017d0: 7820 3c3d 2067 6c78 203c 3d20 6368 696c  x <= glx <= chil
-000017e0: 642e 6d61 785f 676c 7820 6f72 206e 6f74  d.max_glx or not
-000017f0: 2063 6869 6c64 2e6d 696e 5f67 6c79 203c   child.min_gly <
-00001800: 3d20 676c 7920 3c3d 2063 6869 6c64 2e6d  = gly <= child.m
-00001810: 6178 5f67 6c79 3a0d 0a20 2020 2020 2020  ax_gly:..       
-00001820: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-00001830: 650d 0a20 2020 2020 2020 2020 2020 2073  e..            s
-00001840: 656c 662e 7365 6c65 6374 6564 5f63 6869  elf.selected_chi
-00001850: 6c64 7265 6e2e 7265 6d6f 7665 2863 6869  ldren.remove(chi
-00001860: 6c64 290d 0a0d 0a20 2020 2064 6566 206f  ld)....    def o
-00001870: 6e5f 6f76 6572 6c61 795f 7061 696e 7428  n_overlay_paint(
-00001880: 7365 6c66 2c20 6576 656e 743a 2051 5061  self, event: QPa
-00001890: 696e 7445 7665 6e74 2920 2d3e 204e 6f6e  intEvent) -> Non
-000018a0: 653a 0d0a 2020 2020 2020 2020 7265 6374  e:..        rect
-000018b0: 203d 2073 656c 662e 7669 6577 6572 2e6f   = self.viewer.o
-000018c0: 7665 726c 6179 2e72 6563 7428 292e 6164  verlay.rect().ad
-000018d0: 6a75 7374 6564 2832 2c20 322c 202d 322c  justed(2, 2, -2,
-000018e0: 202d 3229 0d0a 0d0a 2020 2020 2020 2020   -2)....        
-000018f0: 7020 3d20 5150 6169 6e74 6572 2873 656c  p = QPainter(sel
-00001900: 662e 7669 6577 6572 2e6f 7665 726c 6179  f.viewer.overlay
-00001910: 290d 0a0d 0a20 2020 2020 2020 2072 616e  )....        ran
-00001920: 6765 733a 206c 6973 745b 7475 706c 655b  ges: list[tuple[
-00001930: 666c 6f61 742c 2066 6c6f 6174 5d5d 203d  float, float]] =
-00001940: 205b 5d0d 0a20 2020 2020 2020 2069 6620   []..        if 
-00001950: 7365 6c66 2e73 656c 6563 7465 645f 6368  self.selected_ch
-00001960: 696c 6472 656e 3a0d 0a20 2020 2020 2020  ildren:..       
-00001970: 2020 2020 2072 616e 6765 5f73 7461 7274       range_start
-00001980: 203d 204e 6f6e 650d 0a20 2020 2020 2020   = None..       
-00001990: 2020 2020 2072 616e 6765 5f65 6e64 203d       range_end =
-000019a0: 204e 6f6e 650d 0a0d 0a20 2020 2020 2020   None....       
-000019b0: 2020 2020 2066 6f72 2069 2c20 6368 696c       for i, chil
-000019c0: 6420 696e 2065 6e75 6d65 7261 7465 2873  d in enumerate(s
-000019d0: 656c 662e 6368 696c 6472 656e 293a 0d0a  elf.children):..
-000019e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019f0: 6966 2063 6869 6c64 2069 6e20 7365 6c66  if child in self
-00001a00: 2e73 656c 6563 7465 645f 6368 696c 6472  .selected_childr
-00001a10: 656e 3a0d 0a20 2020 2020 2020 2020 2020  en:..           
-00001a20: 2020 2020 2020 2020 2069 6620 7261 6e67           if rang
-00001a30: 655f 7374 6172 7420 6973 204e 6f6e 653a  e_start is None:
-00001a40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001a50: 2020 2020 2020 2020 2020 7261 6e67 655f            range_
-00001a60: 7374 6172 7420 3d20 690d 0a20 2020 2020  start = i..     
-00001a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a80: 2020 2072 616e 6765 5f65 6e64 203d 2069     range_end = i
-00001a90: 202b 2031 0d0a 2020 2020 2020 2020 2020   + 1..          
-00001aa0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00001ab0: 6e74 696e 7565 0d0a 0d0a 2020 2020 2020  ntinue....      
-00001ac0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00001ad0: 2069 203d 3d20 7261 6e67 655f 656e 643a   i == range_end:
-00001ae0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001af0: 2020 2020 2020 2020 2020 7261 6e67 655f            range_
-00001b00: 656e 6420 2b3d 2031 0d0a 2020 2020 2020  end += 1..      
-00001b10: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00001b20: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00001b30: 2020 2020 2020 2020 2020 2020 2072 616e               ran
-00001b40: 6765 732e 6170 7065 6e64 2828 7261 6e67  ges.append((rang
-00001b50: 655f 7374 6172 742c 2072 616e 6765 5f65  e_start, range_e
-00001b60: 6e64 2929 0d0a 2020 2020 2020 2020 2020  nd))..          
-00001b70: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-00001b80: 6e67 655f 7374 6172 7420 3d20 690d 0a20  nge_start = i.. 
-00001b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ba0: 2020 2020 2020 2072 616e 6765 5f65 6e64         range_end
-00001bb0: 203d 2069 202b 2031 0d0a 2020 2020 2020   = i + 1..      
-00001bc0: 2020 2020 2020 7261 6e67 6573 2e61 7070        ranges.app
-00001bd0: 656e 6428 2872 616e 6765 5f73 7461 7274  end((range_start
-00001be0: 2c20 7261 6e67 655f 656e 6429 290d 0a0d  , range_end))...
-00001bf0: 0a20 2020 2020 2020 2074 7874 5f6c 6973  .        txt_lis
-00001c00: 7420 3d20 5b0d 0a20 2020 2020 2020 2020  t = [..         
-00001c10: 2020 2027 e5ad 90e7 89a9 e4bb b6e9 8089     '............
-00001c20: e68b a9e5 b7a5 e585 b7ef bc88 4374 726c  ............Ctrl
-00001c30: 2be5 b7a6 e994 ae3a 20e9 8089 e68b a9e7  +......: .......
-00001c40: 88b6 e789 a9e4 bbb6 efbc 8ce5 b7a6 e994  ................
-00001c50: ae3a 20e9 8089 e68b a9e5 ad90 e789 a9e4  .: .............
-00001c60: bbb6 efbc 8ce5 8fb3 e994 ae3a 20e5 8f96  ...........: ...
-00001c70: e6b6 88e9 8089 e68b a9e5 ad90 e789 a9e4  ................
-00001c80: bbb6 efbc 8c43 7472 6c2b e58f b3e9 94ae  .....Ctrl+......
-00001c90: 3a20 e980 80e5 87ba efbc 8927 2c0d 0a20  : .........',.. 
-00001ca0: 2020 2020 2020 2020 2020 2027 e980 89e4             '....
-00001cb0: b8ad e788 b6e7 89a9 e4bb b63a 2027 202b  ...........: ' +
-00001cc0: 2028 0d0a 2020 2020 2020 2020 2020 2020   (..            
-00001cd0: 2020 2020 27e6 97a0 270d 0a20 2020 2020      '...'..     
-00001ce0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00001cf0: 6c66 2e63 7572 7265 6e74 2069 7320 4e6f  lf.current is No
-00001d00: 6e65 0d0a 2020 2020 2020 2020 2020 2020  ne..            
-00001d10: 2020 2020 656c 7365 2066 277b 7365 6c66      else f'{self
-00001d20: 2e63 7572 7265 6e74 2e69 7465 6d2e 5f5f  .current.item.__
-00001d30: 636c 6173 735f 5f2e 5f5f 6e61 6d65 5f5f  class__.__name__
-00001d40: 7d20 6174 207b 6964 2873 656c 662e 6375  } at {id(self.cu
-00001d50: 7272 656e 742e 6974 656d 293a 587d 270d  rrent.item):X}'.
-00001d60: 0a20 2020 2020 2020 2020 2020 2029 2c0d  .            ),.
-00001d70: 0a20 2020 2020 2020 2020 2020 2027 e980  .            '..
-00001d80: 89e4 b8ad e5ad 90e7 89a9 e4bb b63a 2027  .............: '
-00001d90: 202b 2027 2c20 272e 6a6f 696e 280d 0a20   + ', '.join(.. 
-00001da0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-00001db0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001dc0: 2020 2020 2020 6627 5b7b 7261 6e67 655b        f'[{range[
-00001dd0: 305d 7d5d 270d 0a20 2020 2020 2020 2020  0]}]'..         
-00001de0: 2020 2020 2020 2020 2020 2069 6620 7261             if ra
-00001df0: 6e67 655b 305d 202b 2031 203d 3d20 7261  nge[0] + 1 == ra
-00001e00: 6e67 655b 315d 0d0a 2020 2020 2020 2020  nge[1]..        
-00001e10: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00001e20: 2066 275b 7b72 616e 6765 5b30 5d7d 3a7b   f'[{range[0]}:{
-00001e30: 7261 6e67 655b 315d 7d5d 270d 0a20 2020  range[1]}]'..   
-00001e40: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
-00001e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e60: 666f 7220 7261 6e67 6520 696e 2072 616e  for range in ran
-00001e70: 6765 730d 0a20 2020 2020 2020 2020 2020  ges..           
-00001e80: 2029 0d0a 2020 2020 2020 2020 5d0d 0a0d   )..        ]...
-00001e90: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00001ea0: 2e63 7572 7265 6e74 2069 7320 6e6f 7420  .current is not 
-00001eb0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-00001ec0: 2020 2070 2e73 6574 4272 7573 6828 5143     p.setBrush(QC
-00001ed0: 6f6c 6f72 2831 3935 2c20 3133 312c 2031  olor(195, 131, 1
-00001ee0: 392c 2033 3229 290d 0a20 2020 2020 2020  9, 32))..       
-00001ef0: 2020 2020 2070 2e73 6574 5065 6e28 5143       p.setPen(QC
-00001f00: 6f6c 6f72 2831 3935 2c20 3133 312c 2031  olor(195, 131, 1
-00001f10: 3929 290d 0a20 2020 2020 2020 2020 2020  9))..           
-00001f20: 2070 2e64 7261 7752 6563 7428 0d0a 2020   p.drawRect(..  
-00001f30: 2020 2020 2020 2020 2020 2020 2020 5152                QR
-00001f40: 6563 7446 280d 0a20 2020 2020 2020 2020  ectF(..         
-00001f50: 2020 2020 2020 2020 2020 2051 506f 696e             QPoin
-00001f60: 7446 2873 656c 662e 676c 785f 746f 5f6f  tF(self.glx_to_o
-00001f70: 7665 726c 6179 5f78 2873 656c 662e 6375  verlay_x(self.cu
-00001f80: 7272 656e 742e 6d69 6e5f 676c 7829 2c20  rrent.min_glx), 
-00001f90: 7365 6c66 2e67 6c79 5f74 6f5f 6f76 6572  self.gly_to_over
-00001fa0: 6c61 795f 7928 7365 6c66 2e63 7572 7265  lay_y(self.curre
-00001fb0: 6e74 2e6d 696e 5f67 6c79 2929 2c0d 0a20  nt.min_gly)),.. 
-00001fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fd0: 2020 2051 506f 696e 7446 2873 656c 662e     QPointF(self.
-00001fe0: 676c 785f 746f 5f6f 7665 726c 6179 5f78  glx_to_overlay_x
-00001ff0: 2873 656c 662e 6375 7272 656e 742e 6d61  (self.current.ma
-00002000: 785f 676c 7829 2c20 7365 6c66 2e67 6c79  x_glx), self.gly
-00002010: 5f74 6f5f 6f76 6572 6c61 795f 7928 7365  _to_overlay_y(se
-00002020: 6c66 2e63 7572 7265 6e74 2e6d 6178 5f67  lf.current.max_g
-00002030: 6c79 2929 0d0a 2020 2020 2020 2020 2020  ly))..          
-00002040: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-00002050: 2020 2020 2029 0d0a 0d0a 2020 2020 2020       )....      
-00002060: 2020 2020 2020 702e 7365 7442 7275 7368        p.setBrush
-00002070: 2851 436f 6c6f 7228 3139 342c 2031 3032  (QColor(194, 102
-00002080: 2c20 3231 392c 2036 3429 290d 0a20 2020  , 219, 64))..   
-00002090: 2020 2020 2020 2020 2070 2e73 6574 5065           p.setPe
-000020a0: 6e28 5143 6f6c 6f72 2831 3934 2c20 3130  n(QColor(194, 10
-000020b0: 322c 2032 3139 2929 0d0a 2020 2020 2020  2, 219))..      
-000020c0: 2020 2020 2020 666f 7220 6368 696c 6420        for child 
-000020d0: 696e 2073 656c 662e 7365 6c65 6374 6564  in self.selected
-000020e0: 5f63 6869 6c64 7265 6e3a 0d0a 2020 2020  _children:..    
-000020f0: 2020 2020 2020 2020 2020 2020 702e 6472              p.dr
-00002100: 6177 5265 6374 280d 0a20 2020 2020 2020  awRect(..       
-00002110: 2020 2020 2020 2020 2020 2020 2051 5265               QRe
-00002120: 6374 4628 0d0a 2020 2020 2020 2020 2020  ctF(..          
-00002130: 2020 2020 2020 2020 2020 2020 2020 5150                QP
-00002140: 6f69 6e74 4628 7365 6c66 2e67 6c78 5f74  ointF(self.glx_t
-00002150: 6f5f 6f76 6572 6c61 795f 7828 6368 696c  o_overlay_x(chil
-00002160: 642e 6d69 6e5f 676c 7829 2c20 7365 6c66  d.min_glx), self
-00002170: 2e67 6c79 5f74 6f5f 6f76 6572 6c61 795f  .gly_to_overlay_
-00002180: 7928 6368 696c 642e 6d69 6e5f 676c 7929  y(child.min_gly)
-00002190: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-000021a0: 2020 2020 2020 2020 2020 2020 5150 6f69              QPoi
-000021b0: 6e74 4628 7365 6c66 2e67 6c78 5f74 6f5f  ntF(self.glx_to_
-000021c0: 6f76 6572 6c61 795f 7828 6368 696c 642e  overlay_x(child.
-000021d0: 6d61 785f 676c 7829 2c20 7365 6c66 2e67  max_glx), self.g
-000021e0: 6c79 5f74 6f5f 6f76 6572 6c61 795f 7928  ly_to_overlay_y(
-000021f0: 6368 696c 642e 6d61 785f 676c 7929 290d  child.max_gly)).
-00002200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002210: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-00002220: 2020 2020 2020 2020 290d 0a0d 0a20 2020          )....   
-00002230: 2020 2020 2070 2e73 6574 5065 6e28 5174       p.setPen(Qt
-00002240: 2e47 6c6f 6261 6c43 6f6c 6f72 2e77 6869  .GlobalColor.whi
-00002250: 7465 290d 0a20 2020 2020 2020 2070 2e64  te)..        p.d
-00002260: 7261 7754 6578 7428 7265 6374 2c20 5174  rawText(rect, Qt
-00002270: 2e41 6c69 676e 6d65 6e74 466c 6167 2e41  .AlignmentFlag.A
-00002280: 6c69 676e 4c65 6674 207c 2051 742e 416c  lignLeft | Qt.Al
-00002290: 6967 6e6d 656e 7446 6c61 672e 416c 6967  ignmentFlag.Alig
-000022a0: 6e54 6f70 2c20 275c 6e27 2e6a 6f69 6e28  nTop, '\n'.join(
-000022b0: 7478 745f 6c69 7374 2929 0d0a            txt_list))..
+00000040: 434b 494e 470d 0a0d 0a66 726f 6d20 5079  CKING....from Py
+00000050: 5369 6465 362e 5174 436f 7265 2069 6d70  Side6.QtCore imp
+00000060: 6f72 7420 5145 7665 6e74 2c20 514f 626a  ort QEvent, QObj
+00000070: 6563 742c 2051 506f 696e 7446 2c20 5152  ect, QPointF, QR
+00000080: 6563 7446 2c20 5174 0d0a 6672 6f6d 2050  ectF, Qt..from P
+00000090: 7953 6964 6536 2e51 7447 7569 2069 6d70  ySide6.QtGui imp
+000000a0: 6f72 7420 5143 6f6c 6f72 2c20 514d 6f75  ort QColor, QMou
+000000b0: 7365 4576 656e 742c 2051 5061 696e 7465  seEvent, QPainte
+000000c0: 722c 2051 5061 696e 7445 7665 6e74 0d0a  r, QPaintEvent..
+000000d0: 0d0a 6672 6f6d 206a 616e 696d 2e61 6e69  ..from janim.ani
+000000e0: 6d73 2e64 6973 706c 6179 2069 6d70 6f72  ms.display impor
+000000f0: 7420 4469 7370 6c61 790d 0a66 726f 6d20  t Display..from 
+00000100: 6a61 6e69 6d2e 6974 656d 732e 6974 656d  janim.items.item
+00000110: 2069 6d70 6f72 7420 4974 656d 0d0a 6672   import Item..fr
+00000120: 6f6d 206a 616e 696d 2e69 7465 6d73 2e70  om janim.items.p
+00000130: 6f69 6e74 7320 696d 706f 7274 2050 6f69  oints import Poi
+00000140: 6e74 730d 0a0d 0a69 6620 5459 5045 5f43  nts....if TYPE_C
+00000150: 4845 434b 494e 473a 0d0a 2020 2020 6672  HECKING:..    fr
+00000160: 6f6d 206a 616e 696d 2e67 7569 2e61 6e69  om janim.gui.ani
+00000170: 6d5f 7669 6577 6572 2069 6d70 6f72 7420  m_viewer import 
+00000180: 416e 696d 5669 6577 6572 0d0a 0d0a 0d0a  AnimViewer......
+00000190: 636c 6173 7320 5365 6c65 6374 6f72 2851  class Selector(Q
+000001a0: 4f62 6a65 6374 293a 0d0a 2020 2020 2727  Object):..    ''
+000001b0: 270d 0a20 2020 20e5 ad90 e789 a9e4 bbb6  '..    .........
+000001c0: e980 89e6 8ba9 e5b7 a5e5 85b7 0d0a 2020  ..............  
+000001d0: 2020 2727 270d 0a20 2020 2040 6461 7461    '''..    @data
+000001e0: 636c 6173 730d 0a20 2020 2063 6c61 7373  class..    class
+000001f0: 2053 656c 6563 7465 6449 7465 6d3a 0d0a   SelectedItem:..
+00000200: 2020 2020 2020 2020 6974 656d 3a20 4974          item: It
+00000210: 656d 0d0a 2020 2020 2020 2020 6d69 6e5f  em..        min_
+00000220: 676c 783a 2066 6c6f 6174 0d0a 2020 2020  glx: float..    
+00000230: 2020 2020 6d69 6e5f 676c 793a 2066 6c6f      min_gly: flo
+00000240: 6174 0d0a 2020 2020 2020 2020 6d61 785f  at..        max_
+00000250: 676c 783a 2066 6c6f 6174 0d0a 2020 2020  glx: float..    
+00000260: 2020 2020 6d61 785f 676c 793a 2066 6c6f      max_gly: flo
+00000270: 6174 0d0a 0d0a 2020 2020 6465 6620 5f5f  at....    def __
+00000280: 696e 6974 5f5f 2873 656c 662c 2070 6172  init__(self, par
+00000290: 656e 743a 2027 416e 696d 5669 6577 6572  ent: 'AnimViewer
+000002a0: 2729 202d 3e20 4e6f 6e65 3a0d 0a20 2020  ') -> None:..   
+000002b0: 2020 2020 2073 7570 6572 2829 2e5f 5f69       super().__i
+000002c0: 6e69 745f 5f28 7061 7265 6e74 290d 0a20  nit__(parent).. 
+000002d0: 2020 2020 2020 2073 656c 662e 7669 6577         self.view
+000002e0: 6572 203d 2070 6172 656e 740d 0a0d 0a20  er = parent.... 
+000002f0: 2020 2020 2020 2073 656c 662e 7669 6577         self.view
+00000300: 6572 2e67 6c77 2e69 6e73 7461 6c6c 4576  er.glw.installEv
+00000310: 656e 7446 696c 7465 7228 7365 6c66 290d  entFilter(self).
+00000320: 0a20 2020 2020 2020 2073 656c 662e 7669  .        self.vi
+00000330: 6577 6572 2e6f 7665 726c 6179 2e69 6e73  ewer.overlay.ins
+00000340: 7461 6c6c 4576 656e 7446 696c 7465 7228  tallEventFilter(
+00000350: 7365 6c66 290d 0a0d 0a20 2020 2020 2020  self)....       
+00000360: 2073 656c 662e 636c 6561 7228 290d 0a0d   self.clear()...
+00000370: 0a20 2020 2064 6566 2063 6c65 6172 2873  .    def clear(s
+00000380: 656c 6629 202d 3e20 4e6f 6e65 3a0d 0a20  elf) -> None:.. 
+00000390: 2020 2020 2020 2073 656c 662e 6375 7272         self.curr
+000003a0: 656e 743a 2053 656c 6563 746f 722e 5365  ent: Selector.Se
+000003b0: 6c65 6374 6564 4974 656d 207c 204e 6f6e  lectedItem | Non
+000003c0: 6520 3d20 4e6f 6e65 0d0a 2020 2020 2020  e = None..      
+000003d0: 2020 7365 6c66 2e63 6869 6c64 7265 6e3a    self.children:
+000003e0: 206c 6973 745b 5365 6c65 6374 6f72 2e53   list[Selector.S
+000003f0: 656c 6563 7465 6449 7465 6d5d 203d 205b  electedItem] = [
+00000400: 5d0d 0a20 2020 2020 2020 2073 656c 662e  ]..        self.
+00000410: 7365 6c65 6374 6564 5f63 6869 6c64 7265  selected_childre
+00000420: 6e3a 206c 6973 745b 5365 6c65 6374 6f72  n: list[Selector
+00000430: 2e53 656c 6563 7465 6449 7465 6d5d 203d  .SelectedItem] =
+00000440: 205b 5d0d 0a20 2020 2020 2020 2073 656c   []..        sel
+00000450: 662e 7669 6577 6572 2e6f 7665 726c 6179  f.viewer.overlay
+00000460: 2e75 7064 6174 6528 290d 0a0d 0a20 2020  .update()....   
+00000470: 2064 6566 2067 6c78 5f74 6f5f 6f76 6572   def glx_to_over
+00000480: 6c61 795f 7828 7365 6c66 2c20 676c 783a  lay_x(self, glx:
+00000490: 2066 6c6f 6174 2920 2d3e 2066 6c6f 6174   float) -> float
+000004a0: 3a0d 0a20 2020 2020 2020 2072 6574 7572  :..        retur
+000004b0: 6e20 2867 6c78 202b 2031 2920 2f20 3220  n (glx + 1) / 2 
+000004c0: 2a20 7365 6c66 2e76 6965 7765 722e 6f76  * self.viewer.ov
+000004d0: 6572 6c61 792e 7769 6474 6828 290d 0a0d  erlay.width()...
+000004e0: 0a20 2020 2064 6566 2067 6c79 5f74 6f5f  .    def gly_to_
+000004f0: 6f76 6572 6c61 795f 7928 7365 6c66 2c20  overlay_y(self, 
+00000500: 676c 793a 2066 6c6f 6174 2920 2d3e 2066  gly: float) -> f
+00000510: 6c6f 6174 3a0d 0a20 2020 2020 2020 2072  loat:..        r
+00000520: 6574 7572 6e20 282d 676c 7920 2b20 3129  eturn (-gly + 1)
+00000530: 202f 2032 202a 2073 656c 662e 7669 6577   / 2 * self.view
+00000540: 6572 2e6f 7665 726c 6179 2e68 6569 6768  er.overlay.heigh
+00000550: 7428 290d 0a0d 0a20 2020 2064 6566 2065  t()....    def e
+00000560: 7665 6e74 4669 6c74 6572 2873 656c 662c  ventFilter(self,
+00000570: 2077 6174 6368 6564 3a20 514f 626a 6563   watched: QObjec
+00000580: 742c 2065 7665 6e74 3a20 5145 7665 6e74  t, event: QEvent
+00000590: 2920 2d3e 2062 6f6f 6c3a 0d0a 2020 2020  ) -> bool:..    
+000005a0: 2020 2020 6966 2077 6174 6368 6564 2069      if watched i
+000005b0: 7320 7365 6c66 2e76 6965 7765 722e 676c  s self.viewer.gl
+000005c0: 773a 0d0a 2020 2020 2020 2020 2020 2020  w:..            
+000005d0: 6966 2065 7665 6e74 2e74 7970 6528 2920  if event.type() 
+000005e0: 696e 2028 5145 7665 6e74 2e54 7970 652e  in (QEvent.Type.
+000005f0: 4d6f 7573 6542 7574 746f 6e50 7265 7373  MouseButtonPress
+00000600: 2c20 5145 7665 6e74 2e54 7970 652e 4d6f  , QEvent.Type.Mo
+00000610: 7573 6542 7574 746f 6e44 626c 436c 6963  useButtonDblClic
+00000620: 6b29 3a0d 0a20 2020 2020 2020 2020 2020  k):..           
+00000630: 2020 2020 2073 656c 662e 6f6e 5f67 6c77       self.on_glw
+00000640: 5f6d 6f75 7365 5f70 7265 7373 2865 7665  _mouse_press(eve
+00000650: 6e74 290d 0a20 2020 2020 2020 2020 2020  nt)..           
+00000660: 2069 6620 6576 656e 742e 7479 7065 2829   if event.type()
+00000670: 203d 3d20 5145 7665 6e74 2e54 7970 652e   == QEvent.Type.
+00000680: 4d6f 7573 654d 6f76 653a 0d0a 2020 2020  MouseMove:..    
+00000690: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000006a0: 2e6f 6e5f 676c 775f 6d6f 7573 655f 6d6f  .on_glw_mouse_mo
+000006b0: 7665 2865 7665 6e74 290d 0a0d 0a20 2020  ve(event)....   
+000006c0: 2020 2020 2069 6620 7761 7463 6865 6420       if watched 
+000006d0: 6973 2073 656c 662e 7669 6577 6572 2e6f  is self.viewer.o
+000006e0: 7665 726c 6179 3a0d 0a20 2020 2020 2020  verlay:..       
+000006f0: 2020 2020 2069 6620 6576 656e 742e 7479       if event.ty
+00000700: 7065 2829 203d 3d20 5145 7665 6e74 2e54  pe() == QEvent.T
+00000710: 7970 652e 5061 696e 743a 0d0a 2020 2020  ype.Paint:..    
+00000720: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00000730: 2e6f 6e5f 6f76 6572 6c61 795f 7061 696e  .on_overlay_pain
+00000740: 7428 6576 656e 7429 0d0a 0d0a 2020 2020  t(event)....    
+00000750: 2020 2020 7265 7475 726e 2073 7570 6572      return super
+00000760: 2829 2e65 7665 6e74 4669 6c74 6572 2877  ().eventFilter(w
+00000770: 6174 6368 6564 2c20 6576 656e 7429 0d0a  atched, event)..
+00000780: 0d0a 2020 2020 6465 6620 6f6e 5f67 6c77  ..    def on_glw
+00000790: 5f6d 6f75 7365 5f70 7265 7373 2873 656c  _mouse_press(sel
+000007a0: 662c 2065 7665 6e74 3a20 514d 6f75 7365  f, event: QMouse
+000007b0: 4576 656e 7429 202d 3e20 4e6f 6e65 3a0d  Event) -> None:.
+000007c0: 0a20 2020 2020 2020 2069 6620 6576 656e  .        if even
+000007d0: 742e 6d6f 6469 6669 6572 7328 2920 2620  t.modifiers() & 
+000007e0: 5174 2e4b 6579 626f 6172 644d 6f64 6966  Qt.KeyboardModif
+000007f0: 6965 722e 436f 6e74 726f 6c4d 6f64 6966  ier.ControlModif
+00000800: 6965 723a 0d0a 2020 2020 2020 2020 2020  ier:..          
+00000810: 2020 6d61 7463 6820 6576 656e 742e 6275    match event.bu
+00000820: 7474 6f6e 2829 3a0d 0a20 2020 2020 2020  tton():..       
+00000830: 2020 2020 2020 2020 2063 6173 6520 5174           case Qt
+00000840: 2e4d 6f75 7365 4275 7474 6f6e 2e4c 6566  .MouseButton.Lef
+00000850: 7442 7574 746f 6e3a 0d0a 2020 2020 2020  tButton:..      
+00000860: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00000870: 6c66 2e73 656c 6563 745f 7061 7265 6e74  lf.select_parent
+00000880: 5f69 7465 6d28 6576 656e 7429 0d0a 2020  _item(event)..  
+00000890: 2020 2020 2020 2020 2020 2020 2020 6361                ca
+000008a0: 7365 2051 742e 4d6f 7573 6542 7574 746f  se Qt.MouseButto
+000008b0: 6e2e 5269 6768 7442 7574 746f 6e3a 0d0a  n.RightButton:..
+000008c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008d0: 2020 2020 7365 6c66 2e64 656c 6574 654c      self.deleteL
+000008e0: 6174 6572 2829 0d0a 2020 2020 2020 2020  ater()..        
+000008f0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00000900: 2020 206d 6174 6368 2065 7665 6e74 2e62     match event.b
+00000910: 7574 746f 6e28 293a 0d0a 2020 2020 2020  utton():..      
+00000920: 2020 2020 2020 2020 2020 6361 7365 2051            case Q
+00000930: 742e 4d6f 7573 6542 7574 746f 6e2e 4c65  t.MouseButton.Le
+00000940: 6674 4275 7474 6f6e 3a0d 0a20 2020 2020  ftButton:..     
+00000950: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00000960: 656c 662e 7365 6c65 6374 5f63 6869 6c64  elf.select_child
+00000970: 5f69 7465 6d28 6576 656e 7429 0d0a 2020  _item(event)..  
+00000980: 2020 2020 2020 2020 2020 2020 2020 6361                ca
+00000990: 7365 2051 742e 4d6f 7573 6542 7574 746f  se Qt.MouseButto
+000009a0: 6e2e 5269 6768 7442 7574 746f 6e3a 0d0a  n.RightButton:..
+000009b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009c0: 2020 2020 7365 6c66 2e72 656d 6f76 655f      self.remove_
+000009d0: 6368 696c 645f 6974 656d 2865 7665 6e74  child_item(event
+000009e0: 290d 0a0d 0a20 2020 2020 2020 2073 656c  )....        sel
+000009f0: 662e 7669 6577 6572 2e6f 7665 726c 6179  f.viewer.overlay
+00000a00: 2e75 7064 6174 6528 290d 0a0d 0a20 2020  .update()....   
+00000a10: 2064 6566 206f 6e5f 676c 775f 6d6f 7573   def on_glw_mous
+00000a20: 655f 6d6f 7665 2873 656c 662c 2065 7665  e_move(self, eve
+00000a30: 6e74 3a20 514d 6f75 7365 4576 656e 7429  nt: QMouseEvent)
+00000a40: 202d 3e20 4e6f 6e65 3a0d 0a20 2020 2020   -> None:..     
+00000a50: 2020 2069 6620 6e6f 7420 6576 656e 742e     if not event.
+00000a60: 6d6f 6469 6669 6572 7328 2920 2620 5174  modifiers() & Qt
+00000a70: 2e4b 6579 626f 6172 644d 6f64 6966 6965  .KeyboardModifie
+00000a80: 722e 436f 6e74 726f 6c4d 6f64 6966 6965  r.ControlModifie
+00000a90: 723a 0d0a 2020 2020 2020 2020 2020 2020  r:..            
+00000aa0: 6d61 7463 6820 6576 656e 742e 6275 7474  match event.butt
+00000ab0: 6f6e 7328 293a 0d0a 2020 2020 2020 2020  ons():..        
+00000ac0: 2020 2020 2020 2020 6361 7365 2051 742e          case Qt.
+00000ad0: 4d6f 7573 6542 7574 746f 6e2e 4c65 6674  MouseButton.Left
+00000ae0: 4275 7474 6f6e 3a0d 0a20 2020 2020 2020  Button:..       
+00000af0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00000b00: 662e 7365 6c65 6374 5f63 6869 6c64 5f69  f.select_child_i
+00000b10: 7465 6d28 6576 656e 7429 0d0a 2020 2020  tem(event)..    
+00000b20: 2020 2020 2020 2020 2020 2020 6361 7365              case
+00000b30: 2051 742e 4d6f 7573 6542 7574 746f 6e2e   Qt.MouseButton.
+00000b40: 5269 6768 7442 7574 746f 6e3a 0d0a 2020  RightButton:..  
+00000b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b60: 2020 7365 6c66 2e72 656d 6f76 655f 6368    self.remove_ch
+00000b70: 696c 645f 6974 656d 2865 7665 6e74 290d  ild_item(event).
+00000b80: 0a0d 0a20 2020 2020 2020 2020 2020 2073  ...            s
+00000b90: 656c 662e 7669 6577 6572 2e6f 7665 726c  elf.viewer.overl
+00000ba0: 6179 2e75 7064 6174 6528 290d 0a0d 0a20  ay.update().... 
+00000bb0: 2020 2064 6566 2073 656c 6563 745f 7061     def select_pa
+00000bc0: 7265 6e74 5f69 7465 6d28 7365 6c66 2c20  rent_item(self, 
+00000bd0: 6576 656e 743a 2051 4d6f 7573 6545 7665  event: QMouseEve
+00000be0: 6e74 2920 2d3e 204e 6f6e 653a 0d0a 2020  nt) -> None:..  
+00000bf0: 2020 2020 2020 7365 6c66 2e63 6869 6c64        self.child
+00000c00: 7265 6e2e 636c 6561 7228 290d 0a20 2020  ren.clear()..   
+00000c10: 2020 2020 2073 656c 662e 7365 6c65 6374       self.select
+00000c20: 6564 5f63 6869 6c64 7265 6e2e 636c 6561  ed_children.clea
+00000c30: 7228 290d 0a0d 0a20 2020 2020 2020 2078  r()....        x
+00000c40: 2c20 7920 3d20 6576 656e 742e 706f 7369  , y = event.posi
+00000c50: 7469 6f6e 2829 2e74 6f54 7570 6c65 2829  tion().toTuple()
+00000c60: 0d0a 2020 2020 2020 2020 676c 7820 3d20  ..        glx = 
+00000c70: 7820 2f20 7365 6c66 2e76 6965 7765 722e  x / self.viewer.
+00000c80: 676c 772e 7769 6474 6828 2920 2a20 3220  glw.width() * 2 
+00000c90: 2d20 310d 0a20 2020 2020 2020 2067 6c79  - 1..        gly
+00000ca0: 203d 2079 202f 2073 656c 662e 7669 6577   = y / self.view
+00000cb0: 6572 2e67 6c77 2e68 6569 6768 7428 2920  er.glw.height() 
+00000cc0: 2a20 2d32 202b 2031 0d0a 0d0a 2020 2020  * -2 + 1....    
+00000cd0: 2020 2020 616e 696d 203d 2073 656c 662e      anim = self.
+00000ce0: 7669 6577 6572 2e61 6e69 6d0d 0a20 2020  viewer.anim..   
+00000cf0: 2020 2020 2067 6c6f 6261 6c5f 7420 3d20       global_t = 
+00000d00: 616e 696d 2e5f 7469 6d65 0d0a 2020 2020  anim._time..    
+00000d10: 2020 2020 6361 6d65 7261 5f69 6e66 6f20      camera_info 
+00000d20: 3d20 616e 696d 2e74 696d 656c 696e 652e  = anim.timeline.
+00000d30: 6361 6d65 7261 2e63 7572 7265 6e74 2861  camera.current(a
+00000d40: 735f 7469 6d65 3d67 6c6f 6261 6c5f 7429  s_time=global_t)
+00000d50: 2e70 6f69 6e74 732e 696e 666f 0d0a 0d0a  .points.info....
+00000d60: 2020 2020 2020 2020 666f 756e 643a 206c          found: l
+00000d70: 6973 745b 5365 6c65 6374 6f72 2e53 656c  ist[Selector.Sel
+00000d80: 6563 7465 6449 7465 6d5d 203d 205b 5d0d  ectedItem] = [].
+00000d90: 0a0d 0a20 2020 2020 2020 2066 6f72 2064  ...        for d
+00000da0: 6973 706c 6179 2069 6e20 616e 696d 2e64  isplay in anim.d
+00000db0: 6973 706c 6179 5f61 6e69 6d2e 616e 696d  isplay_anim.anim
+00000dc0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00000dd0: 6469 7370 6c61 793a 2044 6973 706c 6179  display: Display
+00000de0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00000df0: 206e 6f74 2064 6973 706c 6179 2e67 6c6f   not display.glo
+00000e00: 6261 6c5f 7261 6e67 652e 6174 203c 3d20  bal_range.at <= 
+00000e10: 676c 6f62 616c 5f74 203c 2064 6973 706c  global_t < displ
+00000e20: 6179 2e67 6c6f 6261 6c5f 7261 6e67 652e  ay.global_range.
+00000e30: 656e 643a 0d0a 2020 2020 2020 2020 2020  end:..          
+00000e40: 2020 2020 2020 636f 6e74 696e 7565 0d0a        continue..
+00000e50: 0d0a 2020 2020 2020 2020 2020 2020 626f  ..            bo
+00000e60: 7820 3d20 6469 7370 6c61 792e 6974 656d  x = display.item
+00000e70: 2e63 7572 7265 6e74 2861 735f 7469 6d65  .current(as_time
+00000e80: 3d67 6c6f 6261 6c5f 7429 2850 6f69 6e74  =global_t)(Point
+00000e90: 7329 2e70 6f69 6e74 732e 626f 780d 0a0d  s).points.box...
+00000ea0: 0a20 2020 2020 2020 2020 2020 206d 6170  .            map
+00000eb0: 7065 6420 3d20 6361 6d65 7261 5f69 6e66  ped = camera_inf
+00000ec0: 6f2e 6d61 705f 706f 696e 7473 2862 6f78  o.map_points(box
+00000ed0: 2e67 6574 5f63 6f72 6e65 7273 2829 290d  .get_corners()).
+00000ee0: 0a20 2020 2020 2020 2020 2020 206d 696e  .            min
+00000ef0: 5f67 6c78 2c20 6d69 6e5f 676c 7920 3d20  _glx, min_gly = 
+00000f00: 6d61 7070 6564 2e6d 696e 2861 7869 733d  mapped.min(axis=
+00000f10: 3029 0d0a 2020 2020 2020 2020 2020 2020  0)..            
+00000f20: 6d61 785f 676c 782c 206d 6178 5f67 6c79  max_glx, max_gly
+00000f30: 203d 206d 6170 7065 642e 6d61 7828 6178   = mapped.max(ax
+00000f40: 6973 3d30 290d 0a20 2020 2020 2020 2020  is=0)..         
+00000f50: 2020 2069 6620 6e6f 7420 6d69 6e5f 676c     if not min_gl
+00000f60: 7820 3c3d 2067 6c78 203c 3d20 6d61 785f  x <= glx <= max_
+00000f70: 676c 7820 6f72 206e 6f74 206d 696e 5f67  glx or not min_g
+00000f80: 6c79 203c 3d20 676c 7920 3c3d 206d 6178  ly <= gly <= max
+00000f90: 5f67 6c79 3a0d 0a20 2020 2020 2020 2020  _gly:..         
+00000fa0: 2020 2020 2020 2063 6f6e 7469 6e75 650d         continue.
+00000fb0: 0a0d 0a20 2020 2020 2020 2020 2020 2066  ...            f
+00000fc0: 6f75 6e64 2e61 7070 656e 6428 5365 6c65  ound.append(Sele
+00000fd0: 6374 6f72 2e53 656c 6563 7465 6449 7465  ctor.SelectedIte
+00000fe0: 6d28 6469 7370 6c61 792e 6974 656d 2c20  m(display.item, 
+00000ff0: 6d69 6e5f 676c 782c 206d 696e 5f67 6c79  min_glx, min_gly
+00001000: 2c20 6d61 785f 676c 782c 206d 6178 5f67  , max_glx, max_g
+00001010: 6c79 2929 0d0a 0d0a 2020 2020 2020 2020  ly))....        
+00001020: 6966 206e 6f74 2066 6f75 6e64 3a0d 0a20  if not found:.. 
+00001030: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00001040: 6375 7272 656e 7420 3d20 4e6f 6e65 0d0a  current = None..
+00001050: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00001060: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00001070: 6c66 2e63 7572 7265 6e74 2069 7320 4e6f  lf.current is No
+00001080: 6e65 206f 7220 7365 6c66 2e63 7572 7265  ne or self.curre
+00001090: 6e74 206e 6f74 2069 6e20 666f 756e 643a  nt not in found:
+000010a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000010b0: 2020 7365 6c66 2e63 7572 7265 6e74 203d    self.current =
+000010c0: 2066 6f75 6e64 5b30 5d0d 0a20 2020 2020   found[0]..     
+000010d0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+000010e0: 2020 2020 2020 2020 2020 2020 2020 6964                id
+000010f0: 7820 3d20 666f 756e 642e 696e 6465 7828  x = found.index(
+00001100: 7365 6c66 2e63 7572 7265 6e74 290d 0a20  self.current).. 
+00001110: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00001120: 656c 662e 6375 7272 656e 7420 3d20 666f  elf.current = fo
+00001130: 756e 645b 2869 6478 202b 2031 2920 2520  und[(idx + 1) % 
+00001140: 6c65 6e28 666f 756e 6429 5d0d 0a0d 0a20  len(found)].... 
+00001150: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+00001160: 7465 6d20 696e 2073 656c 662e 6375 7272  tem in self.curr
+00001170: 656e 742e 6974 656d 2e67 6574 5f63 6869  ent.item.get_chi
+00001180: 6c64 7265 6e28 293a 0d0a 2020 2020 2020  ldren():..      
+00001190: 2020 2020 2020 2020 2020 626f 7820 3d20            box = 
+000011a0: 6974 656d 2e63 7572 7265 6e74 2861 735f  item.current(as_
+000011b0: 7469 6d65 3d67 6c6f 6261 6c5f 7429 2850  time=global_t)(P
+000011c0: 6f69 6e74 7329 2e70 6f69 6e74 732e 626f  oints).points.bo
+000011d0: 780d 0a20 2020 2020 2020 2020 2020 2020  x..             
+000011e0: 2020 206d 6170 7065 6420 3d20 6361 6d65     mapped = came
+000011f0: 7261 5f69 6e66 6f2e 6d61 705f 706f 696e  ra_info.map_poin
+00001200: 7473 2862 6f78 2e67 6574 5f63 6f72 6e65  ts(box.get_corne
+00001210: 7273 2829 290d 0a20 2020 2020 2020 2020  rs())..         
+00001220: 2020 2020 2020 2073 656c 662e 6368 696c         self.chil
+00001230: 6472 656e 2e61 7070 656e 6428 5365 6c65  dren.append(Sele
+00001240: 6374 6f72 2e53 656c 6563 7465 6449 7465  ctor.SelectedIte
+00001250: 6d28 6974 656d 2c20 2a6d 6170 7065 642e  m(item, *mapped.
+00001260: 6d69 6e28 6178 6973 3d30 292c 202a 6d61  min(axis=0), *ma
+00001270: 7070 6564 2e6d 6178 2861 7869 733d 3029  pped.max(axis=0)
+00001280: 2929 0d0a 0d0a 2020 2020 6465 6620 7365  ))....    def se
+00001290: 6c65 6374 5f63 6869 6c64 5f69 7465 6d28  lect_child_item(
+000012a0: 7365 6c66 2c20 6576 656e 743a 2051 4d6f  self, event: QMo
+000012b0: 7573 6545 7665 6e74 2920 2d3e 204e 6f6e  useEvent) -> Non
+000012c0: 653a 0d0a 2020 2020 2020 2020 782c 2079  e:..        x, y
+000012d0: 203d 2065 7665 6e74 2e70 6f73 6974 696f   = event.positio
+000012e0: 6e28 292e 746f 5475 706c 6528 290d 0a20  n().toTuple().. 
+000012f0: 2020 2020 2020 2067 6c78 203d 2078 202f         glx = x /
+00001300: 2073 656c 662e 7669 6577 6572 2e67 6c77   self.viewer.glw
+00001310: 2e77 6964 7468 2829 202a 2032 202d 2031  .width() * 2 - 1
+00001320: 0d0a 2020 2020 2020 2020 676c 7920 3d20  ..        gly = 
+00001330: 7920 2f20 7365 6c66 2e76 6965 7765 722e  y / self.viewer.
+00001340: 676c 772e 6865 6967 6874 2829 202a 202d  glw.height() * -
+00001350: 3220 2b20 310d 0a0d 0a20 2020 2020 2020  2 + 1....       
+00001360: 2066 6f72 2063 6869 6c64 2069 6e20 7365   for child in se
+00001370: 6c66 2e63 6869 6c64 7265 6e3a 0d0a 2020  lf.children:..  
+00001380: 2020 2020 2020 2020 2020 6966 2063 6869            if chi
+00001390: 6c64 2069 6e20 7365 6c66 2e73 656c 6563  ld in self.selec
+000013a0: 7465 645f 6368 696c 6472 656e 3a0d 0a20  ted_children:.. 
+000013b0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000013c0: 6f6e 7469 6e75 650d 0a20 2020 2020 2020  ontinue..       
+000013d0: 2020 2020 2069 6620 6e6f 7420 6368 696c       if not chil
+000013e0: 642e 6d69 6e5f 676c 7820 3c3d 2067 6c78  d.min_glx <= glx
+000013f0: 203c 3d20 6368 696c 642e 6d61 785f 676c   <= child.max_gl
+00001400: 7820 6f72 206e 6f74 2063 6869 6c64 2e6d  x or not child.m
+00001410: 696e 5f67 6c79 203c 3d20 676c 7920 3c3d  in_gly <= gly <=
+00001420: 2063 6869 6c64 2e6d 6178 5f67 6c79 3a0d   child.max_gly:.
+00001430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001440: 2063 6f6e 7469 6e75 650d 0a20 2020 2020   continue..     
+00001450: 2020 2020 2020 2073 656c 662e 7365 6c65         self.sele
+00001460: 6374 6564 5f63 6869 6c64 7265 6e2e 6170  cted_children.ap
+00001470: 7065 6e64 2863 6869 6c64 290d 0a0d 0a20  pend(child).... 
+00001480: 2020 2064 6566 2072 656d 6f76 655f 6368     def remove_ch
+00001490: 696c 645f 6974 656d 2873 656c 662c 2065  ild_item(self, e
+000014a0: 7665 6e74 3a20 514d 6f75 7365 4576 656e  vent: QMouseEven
+000014b0: 7429 202d 3e20 4e6f 6e65 3a0d 0a20 2020  t) -> None:..   
+000014c0: 2020 2020 2078 2c20 7920 3d20 6576 656e       x, y = even
+000014d0: 742e 706f 7369 7469 6f6e 2829 2e74 6f54  t.position().toT
+000014e0: 7570 6c65 2829 0d0a 2020 2020 2020 2020  uple()..        
+000014f0: 676c 7820 3d20 7820 2f20 7365 6c66 2e76  glx = x / self.v
+00001500: 6965 7765 722e 676c 772e 7769 6474 6828  iewer.glw.width(
+00001510: 2920 2a20 3220 2d20 310d 0a20 2020 2020  ) * 2 - 1..     
+00001520: 2020 2067 6c79 203d 2079 202f 2073 656c     gly = y / sel
+00001530: 662e 7669 6577 6572 2e67 6c77 2e68 6569  f.viewer.glw.hei
+00001540: 6768 7428 2920 2a20 2d32 202b 2031 0d0a  ght() * -2 + 1..
+00001550: 0d0a 2020 2020 2020 2020 666f 7220 6368  ..        for ch
+00001560: 696c 6420 696e 2073 656c 662e 7365 6c65  ild in self.sele
+00001570: 6374 6564 5f63 6869 6c64 7265 6e3a 0d0a  cted_children:..
+00001580: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00001590: 6f74 2063 6869 6c64 2e6d 696e 5f67 6c78  ot child.min_glx
+000015a0: 203c 3d20 676c 7820 3c3d 2063 6869 6c64   <= glx <= child
+000015b0: 2e6d 6178 5f67 6c78 206f 7220 6e6f 7420  .max_glx or not 
+000015c0: 6368 696c 642e 6d69 6e5f 676c 7920 3c3d  child.min_gly <=
+000015d0: 2067 6c79 203c 3d20 6368 696c 642e 6d61   gly <= child.ma
+000015e0: 785f 676c 793a 0d0a 2020 2020 2020 2020  x_gly:..        
+000015f0: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
+00001600: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00001610: 6c66 2e73 656c 6563 7465 645f 6368 696c  lf.selected_chil
+00001620: 6472 656e 2e72 656d 6f76 6528 6368 696c  dren.remove(chil
+00001630: 6429 0d0a 0d0a 2020 2020 6465 6620 6f6e  d)....    def on
+00001640: 5f6f 7665 726c 6179 5f70 6169 6e74 2873  _overlay_paint(s
+00001650: 656c 662c 2065 7665 6e74 3a20 5150 6169  elf, event: QPai
+00001660: 6e74 4576 656e 7429 202d 3e20 4e6f 6e65  ntEvent) -> None
+00001670: 3a0d 0a20 2020 2020 2020 2072 6563 7420  :..        rect 
+00001680: 3d20 7365 6c66 2e76 6965 7765 722e 6f76  = self.viewer.ov
+00001690: 6572 6c61 792e 7265 6374 2829 2e61 646a  erlay.rect().adj
+000016a0: 7573 7465 6428 322c 2032 2c20 2d32 2c20  usted(2, 2, -2, 
+000016b0: 2d32 290d 0a0d 0a20 2020 2020 2020 2070  -2)....        p
+000016c0: 203d 2051 5061 696e 7465 7228 7365 6c66   = QPainter(self
+000016d0: 2e76 6965 7765 722e 6f76 6572 6c61 7929  .viewer.overlay)
+000016e0: 0d0a 0d0a 2020 2020 2020 2020 7261 6e67  ....        rang
+000016f0: 6573 3a20 6c69 7374 5b74 7570 6c65 5b66  es: list[tuple[f
+00001700: 6c6f 6174 2c20 666c 6f61 745d 5d20 3d20  loat, float]] = 
+00001710: 5b5d 0d0a 2020 2020 2020 2020 6966 2073  []..        if s
+00001720: 656c 662e 7365 6c65 6374 6564 5f63 6869  elf.selected_chi
+00001730: 6c64 7265 6e3a 0d0a 2020 2020 2020 2020  ldren:..        
+00001740: 2020 2020 7261 6e67 655f 7374 6172 7420      range_start 
+00001750: 3d20 4e6f 6e65 0d0a 2020 2020 2020 2020  = None..        
+00001760: 2020 2020 7261 6e67 655f 656e 6420 3d20      range_end = 
+00001770: 4e6f 6e65 0d0a 0d0a 2020 2020 2020 2020  None....        
+00001780: 2020 2020 666f 7220 692c 2063 6869 6c64      for i, child
+00001790: 2069 6e20 656e 756d 6572 6174 6528 7365   in enumerate(se
+000017a0: 6c66 2e63 6869 6c64 7265 6e29 3a0d 0a20  lf.children):.. 
+000017b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000017c0: 6620 6368 696c 6420 696e 2073 656c 662e  f child in self.
+000017d0: 7365 6c65 6374 6564 5f63 6869 6c64 7265  selected_childre
+000017e0: 6e3a 0d0a 2020 2020 2020 2020 2020 2020  n:..            
+000017f0: 2020 2020 2020 2020 6966 2072 616e 6765          if range
+00001800: 5f73 7461 7274 2069 7320 4e6f 6e65 3a0d  _start is None:.
+00001810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001820: 2020 2020 2020 2020 2072 616e 6765 5f73           range_s
+00001830: 7461 7274 203d 2069 0d0a 2020 2020 2020  tart = i..      
+00001840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001850: 2020 7261 6e67 655f 656e 6420 3d20 6920    range_end = i 
+00001860: 2b20 310d 0a20 2020 2020 2020 2020 2020  + 1..           
+00001870: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+00001880: 7469 6e75 650d 0a0d 0a20 2020 2020 2020  tinue....       
+00001890: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000018a0: 6920 3d3d 2072 616e 6765 5f65 6e64 3a0d  i == range_end:.
+000018b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000018c0: 2020 2020 2020 2020 2072 616e 6765 5f65           range_e
+000018d0: 6e64 202b 3d20 310d 0a20 2020 2020 2020  nd += 1..       
+000018e0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+000018f0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00001900: 2020 2020 2020 2020 2020 2020 7261 6e67              rang
+00001910: 6573 2e61 7070 656e 6428 2872 616e 6765  es.append((range
+00001920: 5f73 7461 7274 2c20 7261 6e67 655f 656e  _start, range_en
+00001930: 6429 290d 0a20 2020 2020 2020 2020 2020  d))..           
+00001940: 2020 2020 2020 2020 2020 2020 2072 616e               ran
+00001950: 6765 5f73 7461 7274 203d 2069 0d0a 2020  ge_start = i..  
+00001960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001970: 2020 2020 2020 7261 6e67 655f 656e 6420        range_end 
+00001980: 3d20 6920 2b20 310d 0a20 2020 2020 2020  = i + 1..       
+00001990: 2020 2020 2072 616e 6765 732e 6170 7065       ranges.appe
+000019a0: 6e64 2828 7261 6e67 655f 7374 6172 742c  nd((range_start,
+000019b0: 2072 616e 6765 5f65 6e64 2929 0d0a 0d0a   range_end))....
+000019c0: 2020 2020 2020 2020 7478 745f 6c69 7374          txt_list
+000019d0: 203d 205b 0d0a 2020 2020 2020 2020 2020   = [..          
+000019e0: 2020 27e5 ad90 e789 a9e4 bbb6 e980 89e6    '.............
+000019f0: 8ba9 e5b7 a5e5 85b7 efbc 8843 7472 6c2b  ...........Ctrl+
+00001a00: e5b7 a6e9 94ae 3a20 e980 89e6 8ba9 e788  ......: ........
+00001a10: b6e7 89a9 e4bb b6ef bc8c e5b7 a6e9 94ae  ................
+00001a20: 3a20 e980 89e6 8ba9 e5ad 90e7 89a9 e4bb  : ..............
+00001a30: b6ef bc8c e58f b3e9 94ae 3a20 e58f 96e6  ..........: ....
+00001a40: b688 e980 89e6 8ba9 e5ad 90e7 89a9 e4bb  ................
+00001a50: b6ef bc8c 4374 726c 2be5 8fb3 e994 ae3a  ....Ctrl+......:
+00001a60: 20e9 8080 e587 baef bc89 272c 0d0a 2020   .........',..  
+00001a70: 2020 2020 2020 2020 2020 27e9 8089 e4b8            '.....
+00001a80: ade7 88b6 e789 a9e4 bbb6 3a20 2720 2b20  ..........: ' + 
+00001a90: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+00001aa0: 2020 2027 e697 a027 0d0a 2020 2020 2020     '...'..      
+00001ab0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00001ac0: 662e 6375 7272 656e 7420 6973 204e 6f6e  f.current is Non
+00001ad0: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
+00001ae0: 2020 2065 6c73 6520 6627 7b73 656c 662e     else f'{self.
+00001af0: 6375 7272 656e 742e 6974 656d 2e5f 5f63  current.item.__c
+00001b00: 6c61 7373 5f5f 2e5f 5f6e 616d 655f 5f7d  lass__.__name__}
+00001b10: 2061 7420 7b69 6428 7365 6c66 2e63 7572   at {id(self.cur
+00001b20: 7265 6e74 2e69 7465 6d29 3a58 7d27 0d0a  rent.item):X}'..
+00001b30: 2020 2020 2020 2020 2020 2020 292c 0d0a              ),..
+00001b40: 2020 2020 2020 2020 2020 2020 27e9 8089              '...
+00001b50: e4b8 ade5 ad90 e789 a9e4 bbb6 3a20 2720  ............: ' 
+00001b60: 2b20 272c 2027 2e6a 6f69 6e28 0d0a 2020  + ', '.join(..  
+00001b70: 2020 2020 2020 2020 2020 2020 2020 280d                (.
+00001b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001b90: 2020 2020 2066 275b 7b72 616e 6765 5b30       f'[{range[0
+00001ba0: 5d7d 5d27 0d0a 2020 2020 2020 2020 2020  ]}]'..          
+00001bb0: 2020 2020 2020 2020 2020 6966 2072 616e            if ran
+00001bc0: 6765 5b30 5d20 2b20 3120 3d3d 2072 616e  ge[0] + 1 == ran
+00001bd0: 6765 5b31 5d0d 0a20 2020 2020 2020 2020  ge[1]..         
+00001be0: 2020 2020 2020 2020 2020 2065 6c73 6520             else 
+00001bf0: 6627 5b7b 7261 6e67 655b 305d 7d3a 7b72  f'[{range[0]}:{r
+00001c00: 616e 6765 5b31 5d7d 5d27 0d0a 2020 2020  ange[1]}]'..    
+00001c10: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
+00001c20: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00001c30: 6f72 2072 616e 6765 2069 6e20 7261 6e67  or range in rang
+00001c40: 6573 0d0a 2020 2020 2020 2020 2020 2020  es..            
+00001c50: 290d 0a20 2020 2020 2020 205d 0d0a 0d0a  )..        ]....
+00001c60: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00001c70: 6375 7272 656e 7420 6973 206e 6f74 204e  current is not N
+00001c80: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+00001c90: 2020 702e 7365 7442 7275 7368 2851 436f    p.setBrush(QCo
+00001ca0: 6c6f 7228 3139 352c 2031 3331 2c20 3139  lor(195, 131, 19
+00001cb0: 2c20 3332 2929 0d0a 2020 2020 2020 2020  , 32))..        
+00001cc0: 2020 2020 702e 7365 7450 656e 2851 436f      p.setPen(QCo
+00001cd0: 6c6f 7228 3139 352c 2031 3331 2c20 3139  lor(195, 131, 19
+00001ce0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00001cf0: 702e 6472 6177 5265 6374 280d 0a20 2020  p.drawRect(..   
+00001d00: 2020 2020 2020 2020 2020 2020 2051 5265               QRe
+00001d10: 6374 4628 0d0a 2020 2020 2020 2020 2020  ctF(..          
+00001d20: 2020 2020 2020 2020 2020 5150 6f69 6e74            QPoint
+00001d30: 4628 7365 6c66 2e67 6c78 5f74 6f5f 6f76  F(self.glx_to_ov
+00001d40: 6572 6c61 795f 7828 7365 6c66 2e63 7572  erlay_x(self.cur
+00001d50: 7265 6e74 2e6d 696e 5f67 6c78 292c 2073  rent.min_glx), s
+00001d60: 656c 662e 676c 795f 746f 5f6f 7665 726c  elf.gly_to_overl
+00001d70: 6179 5f79 2873 656c 662e 6375 7272 656e  ay_y(self.curren
+00001d80: 742e 6d69 6e5f 676c 7929 292c 0d0a 2020  t.min_gly)),..  
+00001d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001da0: 2020 5150 6f69 6e74 4628 7365 6c66 2e67    QPointF(self.g
+00001db0: 6c78 5f74 6f5f 6f76 6572 6c61 795f 7828  lx_to_overlay_x(
+00001dc0: 7365 6c66 2e63 7572 7265 6e74 2e6d 6178  self.current.max
+00001dd0: 5f67 6c78 292c 2073 656c 662e 676c 795f  _glx), self.gly_
+00001de0: 746f 5f6f 7665 726c 6179 5f79 2873 656c  to_overlay_y(sel
+00001df0: 662e 6375 7272 656e 742e 6d61 785f 676c  f.current.max_gl
+00001e00: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
+00001e10: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+00001e20: 2020 2020 290d 0a0d 0a20 2020 2020 2020      )....       
+00001e30: 2020 2020 2070 2e73 6574 4272 7573 6828       p.setBrush(
+00001e40: 5143 6f6c 6f72 2831 3934 2c20 3130 322c  QColor(194, 102,
+00001e50: 2032 3139 2c20 3634 2929 0d0a 2020 2020   219, 64))..    
+00001e60: 2020 2020 2020 2020 702e 7365 7450 656e          p.setPen
+00001e70: 2851 436f 6c6f 7228 3139 342c 2031 3032  (QColor(194, 102
+00001e80: 2c20 3231 3929 290d 0a20 2020 2020 2020  , 219))..       
+00001e90: 2020 2020 2066 6f72 2063 6869 6c64 2069       for child i
+00001ea0: 6e20 7365 6c66 2e73 656c 6563 7465 645f  n self.selected_
+00001eb0: 6368 696c 6472 656e 3a0d 0a20 2020 2020  children:..     
+00001ec0: 2020 2020 2020 2020 2020 2070 2e64 7261             p.dra
+00001ed0: 7752 6563 7428 0d0a 2020 2020 2020 2020  wRect(..        
+00001ee0: 2020 2020 2020 2020 2020 2020 5152 6563              QRec
+00001ef0: 7446 280d 0a20 2020 2020 2020 2020 2020  tF(..           
+00001f00: 2020 2020 2020 2020 2020 2020 2051 506f               QPo
+00001f10: 696e 7446 2873 656c 662e 676c 785f 746f  intF(self.glx_to
+00001f20: 5f6f 7665 726c 6179 5f78 2863 6869 6c64  _overlay_x(child
+00001f30: 2e6d 696e 5f67 6c78 292c 2073 656c 662e  .min_glx), self.
+00001f40: 676c 795f 746f 5f6f 7665 726c 6179 5f79  gly_to_overlay_y
+00001f50: 2863 6869 6c64 2e6d 696e 5f67 6c79 2929  (child.min_gly))
+00001f60: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00001f70: 2020 2020 2020 2020 2020 2051 506f 696e             QPoin
+00001f80: 7446 2873 656c 662e 676c 785f 746f 5f6f  tF(self.glx_to_o
+00001f90: 7665 726c 6179 5f78 2863 6869 6c64 2e6d  verlay_x(child.m
+00001fa0: 6178 5f67 6c78 292c 2073 656c 662e 676c  ax_glx), self.gl
+00001fb0: 795f 746f 5f6f 7665 726c 6179 5f79 2863  y_to_overlay_y(c
+00001fc0: 6869 6c64 2e6d 6178 5f67 6c79 2929 0d0a  hild.max_gly))..
+00001fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001fe0: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
+00001ff0: 2020 2020 2020 2029 0d0a 0d0a 2020 2020         )....    
+00002000: 2020 2020 702e 7365 7450 656e 2851 742e      p.setPen(Qt.
+00002010: 476c 6f62 616c 436f 6c6f 722e 7768 6974  GlobalColor.whit
+00002020: 6529 0d0a 2020 2020 2020 2020 702e 6472  e)..        p.dr
+00002030: 6177 5465 7874 2872 6563 742c 2051 742e  awText(rect, Qt.
+00002040: 416c 6967 6e6d 656e 7446 6c61 672e 416c  AlignmentFlag.Al
+00002050: 6967 6e4c 6566 7420 7c20 5174 2e41 6c69  ignLeft | Qt.Ali
+00002060: 676e 6d65 6e74 466c 6167 2e41 6c69 676e  gnmentFlag.Align
+00002070: 546f 702c 2027 5c6e 272e 6a6f 696e 2874  Top, '\n'.join(t
+00002080: 7874 5f6c 6973 7429 290d 0a              xt_list))..
```

### Comparing `janim-0.5.2/janim/imports.py` & `janim-1.0.0/janim/imports.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 # flake8: noqa
 import janim.items.boolean_ops as boolean_ops
 from janim.anims.composition import *
 from janim.anims.creation import *
 from janim.anims.display import *
 from janim.anims.fading import *
+from janim.anims.growing import *
+from janim.anims.indication import *
 from janim.anims.rotation import *
 from janim.anims.timeline import *
 from janim.anims.transform import *
 from janim.anims.updater import *
 from janim.camera.camera import *
 from janim.camera.camera_info import *
 from janim.components.rgbas import apart_alpha, merge_alpha
@@ -22,14 +24,15 @@
 from janim.items.geometry.arc import *
 from janim.items.geometry.arrow import *
 from janim.items.geometry.line import *
 from janim.items.geometry.polygon import *
 from janim.items.image_item import *
 from janim.items.item import *
 from janim.items.points import *
+from janim.items.shape_matchers import *
 from janim.items.svg.brace import *
 from janim.items.svg.svg_item import *
 from janim.items.svg.typst import *
 from janim.items.text.text import *
 from janim.items.value_tracker import *
 from janim.items.vitem import *
 from janim.utils.bezier import *
```

### Comparing `janim-0.5.2/janim/items/audio.py` & `janim-1.0.0/janim/items/audio.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,295 +3,356 @@
 00000020: 696f 6e73 0d0a 0d0a 696d 706f 7274 2063  ions....import c
 00000030: 6f70 790d 0a69 6d70 6f72 7420 6f73 0d0a  opy..import os..
 00000040: 696d 706f 7274 2073 7562 7072 6f63 6573  import subproces
 00000050: 7320 6173 2073 700d 0a66 726f 6d20 7479  s as sp..from ty
 00000060: 7069 6e67 2069 6d70 6f72 7420 4974 6572  ping import Iter
 00000070: 6162 6c65 2c20 5365 6c66 0d0a 0d0a 696d  able, Self....im
 00000080: 706f 7274 206e 756d 7079 2061 7320 6e70  port numpy as np
-00000090: 0d0a 0d0a 6672 6f6d 206a 616e 696d 2e65  ....from janim.e
-000000a0: 7863 6570 7469 6f6e 2069 6d70 6f72 7420  xception import 
-000000b0: 4558 4954 434f 4445 5f46 464d 5045 475f  EXITCODE_FFMPEG_
-000000c0: 4e4f 545f 464f 554e 442c 2045 7869 7445  NOT_FOUND, ExitE
-000000d0: 7863 6570 7469 6f6e 0d0a 6672 6f6d 206a  xception..from j
-000000e0: 616e 696d 2e6c 6f67 6765 7220 696d 706f  anim.logger impo
-000000f0: 7274 206c 6f67 0d0a 6672 6f6d 206a 616e  rt log..from jan
-00000100: 696d 2e75 7469 6c73 2e63 6f6e 6669 6720  im.utils.config 
-00000110: 696d 706f 7274 2043 6f6e 6669 670d 0a66  import Config..f
-00000120: 726f 6d20 6a61 6e69 6d2e 7574 696c 732e  rom janim.utils.
-00000130: 6974 6572 6162 6c65 7320 696d 706f 7274  iterables import
-00000140: 2072 6573 697a 655f 7769 7468 5f69 6e74   resize_with_int
-00000150: 6572 706f 6c61 7469 6f6e 0d0a 6672 6f6d  erpolation..from
-00000160: 206a 616e 696d 2e75 7469 6c73 2e73 696d   janim.utils.sim
-00000170: 706c 655f 6675 6e63 7469 6f6e 7320 696d  ple_functions im
-00000180: 706f 7274 2063 6c69 700d 0a66 726f 6d20  port clip..from 
-00000190: 6a61 6e69 6d2e 7574 696c 732e 756e 6971  janim.utils.uniq
-000001a0: 7565 5f6e 7061 7272 6179 2069 6d70 6f72  ue_nparray impor
-000001b0: 7420 556e 6971 7565 4e70 6172 7261 790d  t UniqueNparray.
-000001c0: 0a0d 0a0d 0a63 6c61 7373 2041 7564 696f  .....class Audio
-000001d0: 3a0d 0a20 2020 2027 2727 0d0a 2020 2020  :..    '''..    
-000001e0: e4b8 8de5 bbba e8ae aee4 bdbf e794 a8e8  ................
-000001f0: afa5 e7b1 bbe5 a484 e790 86e5 a49a e5a3  ................
-00000200: b0e9 8193 e99f b3e9 a291 efbc 8ce5 9ba0  ................
-00000210: e4b8 bae8 afa5 e7b1 bbe8 afbb e58f 96e6  ................
-00000220: 97b6 e4bb 85e4 bf9d e795 99e5 8d95 e5a3  ................
-00000230: b0e9 8193 0d0a 2020 2020 2727 270d 0a20  ......    '''.. 
-00000240: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00000250: 7365 6c66 2c20 6669 6c65 7061 7468 3a20  self, filepath: 
-00000260: 7374 722c 2062 6567 696e 3a20 666c 6f61  str, begin: floa
-00000270: 7420 3d20 2d31 2c20 656e 643a 2066 6c6f  t = -1, end: flo
-00000280: 6174 203d 202d 312c 202a 2a6b 7761 7267  at = -1, **kwarg
-00000290: 7329 3a0d 0a20 2020 2020 2020 2073 7570  s):..        sup
-000002a0: 6572 2829 2e5f 5f69 6e69 745f 5f28 2a2a  er().__init__(**
-000002b0: 6b77 6172 6773 290d 0a20 2020 2020 2020  kwargs)..       
-000002c0: 2073 656c 662e 5f73 616d 706c 6573 203d   self._samples =
-000002d0: 2055 6e69 7175 654e 7061 7272 6179 2864   UniqueNparray(d
-000002e0: 7479 7065 3d6e 702e 696e 7431 3629 0d0a  type=np.int16)..
-000002f0: 2020 2020 2020 2020 7365 6c66 2e66 7261          self.fra
-00000300: 6d65 7261 7465 203d 2030 0d0a 2020 2020  merate = 0..    
-00000310: 2020 2020 7365 6c66 2e66 696c 6570 6174      self.filepat
-00000320: 6820 3d20 2727 0d0a 2020 2020 2020 2020  h = ''..        
-00000330: 7365 6c66 2e66 696c 656e 616d 6520 3d20  self.filename = 
-00000340: 2727 0d0a 2020 2020 2020 2020 7365 6c66  ''..        self
-00000350: 2e72 6561 6428 6669 6c65 7061 7468 2c20  .read(filepath, 
-00000360: 6265 6769 6e2c 2065 6e64 290d 0a0d 0a20  begin, end).... 
-00000370: 2020 2064 6566 2063 6f70 7928 7365 6c66     def copy(self
-00000380: 2920 2d3e 2053 656c 663a 0d0a 2020 2020  ) -> Self:..    
-00000390: 2020 2020 636f 7079 5f61 7564 696f 203d      copy_audio =
-000003a0: 2063 6f70 792e 636f 7079 2873 656c 6629   copy.copy(self)
-000003b0: 0d0a 2020 2020 2020 2020 636f 7079 5f61  ..        copy_a
-000003c0: 7564 696f 2e5f 7361 6d70 6c65 7320 3d20  udio._samples = 
-000003d0: 7365 6c66 2e5f 7361 6d70 6c65 732e 636f  self._samples.co
-000003e0: 7079 2829 0d0a 2020 2020 2020 2020 7265  py()..        re
-000003f0: 7475 726e 2063 6f70 795f 6175 6469 6f0d  turn copy_audio.
-00000400: 0a0d 0a20 2020 2064 6566 2072 6561 6428  ...    def read(
-00000410: 0d0a 2020 2020 2020 2020 7365 6c66 2c0d  ..        self,.
-00000420: 0a20 2020 2020 2020 2066 696c 6570 6174  .        filepat
-00000430: 683a 2073 7472 2c0d 0a20 2020 2020 2020  h: str,..       
-00000440: 2062 6567 696e 3a20 666c 6f61 7420 3d20   begin: float = 
-00000450: 2d31 2c0d 0a20 2020 2020 2020 2065 6e64  -1,..        end
-00000460: 3a20 666c 6f61 7420 3d20 2d31 0d0a 2020  : float = -1..  
-00000470: 2020 2920 2d3e 2053 656c 663a 0d0a 2020    ) -> Self:..  
-00000480: 2020 2020 2020 2727 270d 0a20 2020 2020        '''..     
-00000490: 2020 20e4 bb8e e696 87e4 bbb6 e4b8 ade8     .............
-000004a0: afbb e58f 96e9 9fb3 e9a2 910d 0a0d 0a20  ............... 
-000004b0: 2020 2020 2020 20e5 8faf e4bb a5e6 8c87         .........
-000004c0: e5ae 9a20 6060 6265 6769 6e60 6020 e592  ... ``begin`` ..
-000004d0: 8c20 6060 656e 6460 6020 e69d a5e6 88aa  . ``end`` ......
-000004e0: e58f 96e9 9fb3 e9a2 91e7 9a84 e4b8 80e9  ................
-000004f0: 83a8 e588 860d 0a20 2020 2020 2020 2027  .......        '
-00000500: 2727 0d0a 2020 2020 2020 2020 636f 6d6d  ''..        comm
-00000510: 616e 6420 3d20 5b0d 0a20 2020 2020 2020  and = [..       
-00000520: 2020 2020 2043 6f6e 6669 672e 6765 742e       Config.get.
-00000530: 6666 6d70 6567 5f62 696e 2c0d 0a20 2020  ffmpeg_bin,..   
-00000540: 2020 2020 2020 2020 2027 2d76 6e27 2c0d           '-vn',.
-00000550: 0a20 2020 2020 2020 2020 2020 2027 2d69  .            '-i
-00000560: 272c 2066 696c 6570 6174 682c 0d0a 2020  ', filepath,..  
-00000570: 2020 2020 2020 5d0d 0a20 2020 2020 2020        ]..       
-00000580: 2069 6620 6265 6769 6e20 213d 202d 313a   if begin != -1:
-00000590: 0d0a 2020 2020 2020 2020 2020 2020 636f  ..            co
-000005a0: 6d6d 616e 6420 2b3d 205b 272d 7373 272c  mmand += ['-ss',
-000005b0: 2073 7472 2862 6567 696e 295d 2020 2320   str(begin)]  # 
-000005c0: 636c 6970 2066 726f 6d0d 0a20 2020 2020  clip from..     
-000005d0: 2020 2069 6620 656e 6420 213d 202d 313a     if end != -1:
-000005e0: 0d0a 2020 2020 2020 2020 2020 2020 636f  ..            co
-000005f0: 6d6d 616e 6420 2b3d 205b 272d 746f 272c  mmand += ['-to',
-00000600: 2073 7472 2865 6e64 295d 2020 2020 2320   str(end)]    # 
-00000610: 636c 6970 2074 6f0d 0a0d 0a20 2020 2020  clip to....     
-00000620: 2020 2063 6f6d 6d61 6e64 202b 3d20 5b0d     command += [.
-00000630: 0a20 2020 2020 2020 2020 2020 2027 2d66  .            '-f
-00000640: 272c 2027 7331 366c 6527 2c0d 0a20 2020  ', 's16le',..   
-00000650: 2020 2020 2020 2020 2027 2d61 636f 6465           '-acode
-00000660: 6327 2c20 2770 636d 5f73 3136 6c65 272c  c', 'pcm_s16le',
-00000670: 0d0a 2020 2020 2020 2020 2020 2020 272d  ..            '-
-00000680: 6172 272c 2073 7472 2843 6f6e 6669 672e  ar', str(Config.
-00000690: 6765 742e 6175 6469 6f5f 6672 616d 6572  get.audio_framer
-000006a0: 6174 6529 2c20 2020 2020 2320 6672 616d  ate),     # fram
-000006b0: 6572 6174 6520 2620 7361 6d70 6c65 7261  erate & samplera
-000006c0: 7465 0d0a 2020 2020 2020 2020 2020 2020  te..            
-000006d0: 272d 6163 272c 2027 3127 2c0d 0a20 2020  '-ac', '1',..   
-000006e0: 2020 2020 2020 2020 2027 2d6c 6f67 6c65           '-logle
-000006f0: 7665 6c27 2c20 2765 7272 6f72 272c 0d0a  vel', 'error',..
-00000700: 2020 2020 2020 2020 2020 2020 272d 272c              '-',
-00000710: 2020 2020 2320 6f75 7470 7574 2074 6f20      # output to 
-00000720: 6120 7069 7065 0d0a 2020 2020 2020 2020  a pipe..        
-00000730: 5d0d 0a0d 0a20 2020 2020 2020 2074 7279  ]....        try
-00000740: 3a0d 0a20 2020 2020 2020 2020 2020 2023  :..            #
-00000750: 2054 4f44 4f3a 2073 7570 706f 7274 206d   TODO: support m
-00000760: 6f72 6520 7361 6d70 7769 6474 680d 0a20  ore sampwidth.. 
-00000770: 2020 2020 2020 2020 2020 2023 2054 4f44             # TOD
-00000780: 4f3a 2066 6978 2042 7974 654f 7264 6572  O: fix ByteOrder
-00000790: 0d0a 2020 2020 2020 2020 2020 2020 7769  ..            wi
-000007a0: 7468 2073 702e 506f 7065 6e28 636f 6d6d  th sp.Popen(comm
-000007b0: 616e 642c 2073 7464 6f75 743d 7370 2e50  and, stdout=sp.P
-000007c0: 4950 4529 2061 7320 7265 6164 696e 675f  IPE) as reading_
-000007d0: 7072 6f63 6573 733a 0d0a 2020 2020 2020  process:..      
-000007e0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-000007f0: 7361 6d70 6c65 732e 6461 7461 203d 206e  samples.data = n
-00000800: 702e 6672 6f6d 6275 6666 6572 2872 6561  p.frombuffer(rea
-00000810: 6469 6e67 5f70 726f 6365 7373 2e73 7464  ding_process.std
-00000820: 6f75 742e 7265 6164 2829 2c20 6474 7970  out.read(), dtyp
-00000830: 653d 6e70 2e69 6e74 3136 290d 0a20 2020  e=np.int16)..   
-00000840: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00000850: 662e 6672 616d 6572 6174 6520 3d20 436f  f.framerate = Co
-00000860: 6e66 6967 2e67 6574 2e61 7564 696f 5f66  nfig.get.audio_f
-00000870: 7261 6d65 7261 7465 0d0a 2020 2020 2020  ramerate..      
-00000880: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
-00000890: 696c 6570 6174 6820 3d20 6669 6c65 7061  ilepath = filepa
-000008a0: 7468 0d0a 2020 2020 2020 2020 2020 2020  th..            
-000008b0: 2020 2020 7365 6c66 2e66 696c 656e 616d      self.filenam
-000008c0: 6520 3d20 6f73 2e70 6174 682e 6261 7365  e = os.path.base
-000008d0: 6e61 6d65 2866 696c 6570 6174 6829 0d0a  name(filepath)..
-000008e0: 0d0a 2020 2020 2020 2020 6578 6365 7074  ..        except
-000008f0: 2046 696c 654e 6f74 466f 756e 6445 7272   FileNotFoundErr
-00000900: 6f72 3a0d 0a20 2020 2020 2020 2020 2020  or:..           
-00000910: 206c 6f67 2e65 7272 6f72 2827 e697 a0e6   log.error('....
-00000920: b395 e8af bbe5 8f96 e99f b3e9 a291 efbc  ................
-00000930: 8ce9 9c80 e8a6 81e5 ae89 e8a3 8520 6666  ............. ff
-00000940: 6d70 6567 20e5 b9b6 e5b0 86e5 85b6 e6b7  mpeg ...........
-00000950: bbe5 8aa0 e588 b0e7 8eaf e5a2 83e5 8f98  ................
-00000960: e987 8fe4 b8ad 2729 0d0a 2020 2020 2020  ......')..      
-00000970: 2020 2020 2020 7261 6973 6520 4578 6974        raise Exit
-00000980: 4578 6365 7074 696f 6e28 4558 4954 434f  Exception(EXITCO
-00000990: 4445 5f46 464d 5045 475f 4e4f 545f 464f  DE_FFMPEG_NOT_FO
-000009a0: 554e 4429 0d0a 0d0a 2020 2020 2020 2020  UND)....        
-000009b0: 7265 7475 726e 2073 656c 660d 0a0d 0a20  return self.... 
-000009c0: 2020 2064 6566 2073 616d 706c 655f 636f     def sample_co
-000009d0: 756e 7428 7365 6c66 2920 2d3e 2069 6e74  unt(self) -> int
-000009e0: 3a0d 0a20 2020 2020 2020 2027 2727 0d0a  :..        '''..
-000009f0: 2020 2020 2020 2020 e689 80e6 9c89 e987          ........
-00000a00: 87e6 a0b7 e782 b9e7 9a84 e695 b0e9 878f  ................
-00000a10: 0d0a 2020 2020 2020 2020 2727 270d 0a20  ..        '''.. 
-00000a20: 2020 2020 2020 2072 6574 7572 6e20 6c65         return le
-00000a30: 6e28 7365 6c66 2e5f 7361 6d70 6c65 732e  n(self._samples.
-00000a40: 5f64 6174 6129 0d0a 0d0a 2020 2020 6465  _data)....    de
-00000a50: 6620 6475 7261 7469 6f6e 2873 656c 6629  f duration(self)
-00000a60: 202d 3e20 666c 6f61 743a 0d0a 2020 2020   -> float:..    
-00000a70: 2020 2020 2727 270d 0a20 2020 2020 2020      '''..       
-00000a80: 20e6 8c81 e7bb ade6 97b6 e997 b40d 0a20   .............. 
-00000a90: 2020 2020 2020 2027 2727 0d0a 2020 2020         '''..    
-00000aa0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00000ab0: 7361 6d70 6c65 5f63 6f75 6e74 2829 202f  sample_count() /
-00000ac0: 2073 656c 662e 6672 616d 6572 6174 650d   self.framerate.
-00000ad0: 0a0d 0a20 2020 2064 6566 2063 6c69 7028  ...    def clip(
-00000ae0: 7365 6c66 2c20 6265 6769 6e3a 2066 6c6f  self, begin: flo
-00000af0: 6174 203d 2030 2c20 656e 643a 2066 6c6f  at = 0, end: flo
-00000b00: 6174 203d 202d 3129 202d 3e20 5365 6c66  at = -1) -> Self
-00000b10: 3a0d 0a20 2020 2020 2020 2027 2727 0d0a  :..        '''..
-00000b20: 2020 2020 2020 2020 e8a3 81e5 89aa e99f          ........
-00000b30: b3e9 a291 0d0a 0d0a 2020 2020 2020 2020  ........        
-00000b40: 2d20 e4bf 9de7 9599 2060 6062 6567 696e  - ...... ``begin
-00000b50: 6060 20e5 88b0 2060 6065 6e64 6060 20e4  `` ... ``end`` .
-00000b60: b98b e997 b4e7 9a84 e983 a8e5 8886 0d0a  ................
-00000b70: 2020 2020 2020 2020 2d20 e88b a520 6060          - ... ``
-00000b80: 6265 6769 6e60 6020 e7bc bae7 9c81 efbc  begin`` ........
-00000b90: 8ce5 8899 e8a1 a8e7 a4ba e4bb 8ee6 9c80  ................
-00000ba0: e5bc 80e5 a78b 0d0a 2020 2020 2020 2020  ........        
-00000bb0: 2d20 e88b a520 6060 656e 6460 6020 e7bc  - ... ``end`` ..
-00000bc0: bae7 9c81 2860 602d 3160 6029 efbc 8ce5  ....(``-1``)....
-00000bd0: 8899 e8a1 a8e7 a4ba e588 b0e6 9c80 e69c  ................
-00000be0: abe5 b0be 0d0a 2020 2020 2020 2020 2727  ......        ''
-00000bf0: 270d 0a20 2020 2020 2020 2066 7261 6d65  '..        frame
-00000c00: 5f62 6567 696e 203d 2063 6c69 7028 696e  _begin = clip(in
-00000c10: 7428 6265 6769 6e20 2a20 7365 6c66 2e66  t(begin * self.f
-00000c20: 7261 6d65 7261 7465 292c 2030 2c20 7365  ramerate), 0, se
-00000c30: 6c66 2e73 616d 706c 655f 636f 756e 7428  lf.sample_count(
-00000c40: 2929 0d0a 2020 2020 2020 2020 6966 2065  ))..        if e
-00000c50: 6e64 203d 3d20 2d31 3a0d 0a20 2020 2020  nd == -1:..     
-00000c60: 2020 2020 2020 2066 7261 6d65 5f65 6e64         frame_end
-00000c70: 203d 2073 656c 662e 7361 6d70 6c65 5f63   = self.sample_c
-00000c80: 6f75 6e74 2829 0d0a 2020 2020 2020 2020  ount()..        
-00000c90: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00000ca0: 2020 2066 7261 6d65 5f65 6e64 203d 2063     frame_end = c
-00000cb0: 6c69 7028 696e 7428 656e 6420 2a20 7365  lip(int(end * se
-00000cc0: 6c66 2e66 7261 6d65 7261 7465 292c 2030  lf.framerate), 0
-00000cd0: 2c20 7365 6c66 2e73 616d 706c 655f 636f  , self.sample_co
-00000ce0: 756e 7428 2929 0d0a 2020 2020 2020 2020  unt())..        
-00000cf0: 7365 6c66 2e5f 7361 6d70 6c65 732e 6461  self._samples.da
-00000d00: 7461 203d 2073 656c 662e 5f73 616d 706c  ta = self._sampl
-00000d10: 6573 2e5f 6461 7461 5b66 7261 6d65 5f62  es._data[frame_b
-00000d20: 6567 696e 3a66 7261 6d65 5f65 6e64 5d0d  egin:frame_end].
-00000d30: 0a0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
-00000d40: 6e20 7365 6c66 0d0a 0d0a 2020 2020 6465  n self....    de
-00000d50: 6620 6d75 6c28 7365 6c66 2c20 7661 6c75  f mul(self, valu
-00000d60: 653a 2066 6c6f 6174 207c 2049 7465 7261  e: float | Itera
-00000d70: 626c 655b 666c 6f61 745d 2920 2d3e 2053  ble[float]) -> S
-00000d80: 656c 663a 0d0a 2020 2020 2020 2020 2727  elf:..        ''
-00000d90: 270d 0a20 2020 2020 2020 20e4 b998 e4bb  '..        .....
-00000da0: a5e7 bb99 e5ae 9ae7 9a84 2060 6076 616c  .......... ``val
-00000db0: 7565 6060 efbc 8c60 6076 616c 7565 6060  ue``...``value``
-00000dc0: 20e5 8faf e4bb a5e5 90ab e69c 89e5 a49a   ...............
-00000dd0: e4b8 aae5 8583 e7b4 a0ef bc88 e6af 94e5  ................
-00000de0: a682 e4b8 80e4 b8aa e588 97e8 a1a8 efbc  ................
-00000df0: 890d 0a0d 0a20 2020 2020 2020 20e4 be8b  .....        ...
-00000e00: e5a6 82ef bc9a 0d0a 0d0a 2020 2020 2020  ..........      
-00000e10: 2020 2d20 6060 6175 6469 6f2e 6d75 6c28    - ``audio.mul(
-00000e20: 302e 3529 6060 20e5 8faf e4bb a5e4 bdbf  0.5)`` .........
-00000e30: e99f b3e9 ab98 e587 8fe5 8d8a 0d0a 2020  ..............  
-00000e40: 2020 2020 2020 2d20 6060 6175 6469 6f2e        - ``audio.
-00000e50: 6d75 6c28 5b31 2c20 305d 2960 6020 e58f  mul([1, 0])`` ..
-00000e60: afe4 bba5 e4bd bfe5 bc80 e5a7 8be6 97b6  ................
-00000e70: e69c 80e5 bcba efbc 8ce7 bb93 e69d 9fe6  ................
-00000e80: 97b6 e69c 80e5 bcb1 0d0a 2020 2020 2020  ..........      
-00000e90: 2020 2d20 6060 6175 6469 6f2e 6d75 6c28    - ``audio.mul(
-00000ea0: 6e70 2e73 696e 286e 702e 6c69 6e73 7061  np.sin(np.linspa
-00000eb0: 6365 2830 2c20 3220 2a20 6e70 2e70 692c  ce(0, 2 * np.pi,
-00000ec0: 2061 7564 696f 2e73 616d 706c 655f 636f   audio.sample_co
-00000ed0: 756e 7428 2929 2929 6060 20e5 8faf e4bb  unt())))`` .....
-00000ee0: a5e4 bdbf e99f b3e9 ab98 e99a 8fe6 97b6  ................
-00000ef0: e997 b4e4 b998 e4bb a520 7369 6e20 e587  ......... sin ..
-00000f00: bde6 95b0 e79a 84e4 b880 e4b8 aae5 91a8  ................
-00000f10: e69c 9f0d 0a20 2020 2020 2020 2027 2727  .....        '''
-00000f20: 0d0a 2020 2020 2020 2020 6966 2069 7369  ..        if isi
-00000f30: 6e73 7461 6e63 6528 7661 6c75 652c 2049  nstance(value, I
-00000f40: 7465 7261 626c 6529 3a0d 0a20 2020 2020  terable):..     
-00000f50: 2020 2020 2020 2076 616c 7565 203d 2072         value = r
-00000f60: 6573 697a 655f 7769 7468 5f69 6e74 6572  esize_with_inter
-00000f70: 706f 6c61 7469 6f6e 2876 616c 7565 2c20  polation(value, 
-00000f80: 7365 6c66 2e73 616d 706c 655f 636f 756e  self.sample_coun
-00000f90: 7428 2929 0d0a 2020 2020 2020 2020 7365  t())..        se
-00000fa0: 6c66 2e5f 7361 6d70 6c65 732e 6461 7461  lf._samples.data
-00000fb0: 203d 2073 656c 662e 5f73 616d 706c 6573   = self._samples
-00000fc0: 2e64 6174 6120 2a20 7661 6c75 650d 0a0d  .data * value...
-00000fd0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00000fe0: 7365 6c66 0d0a 0d0a 2020 2020 6465 6620  self....    def 
-00000ff0: 6661 6465 5f69 6e28 7365 6c66 2c20 6475  fade_in(self, du
-00001000: 7261 7469 6f6e 3a20 666c 6f61 7429 202d  ration: float) -
-00001010: 3e20 5365 6c66 3a0d 0a20 2020 2020 2020  > Self:..       
-00001020: 2027 2727 0d0a 2020 2020 2020 2020 e5ba   '''..        ..
-00001030: 94e7 94a8 2060 6064 7572 6174 696f 6e60  .... ``duration`
-00001040: 6020 e7a7 92e7 9a84 e6b7 a1e5 85a5 0d0a  ` ..............
-00001050: 2020 2020 2020 2020 2727 270d 0a20 2020          '''..   
-00001060: 2020 2020 2066 7261 6d65 7320 3d20 696e       frames = in
-00001070: 7428 7365 6c66 2e66 7261 6d65 7261 7465  t(self.framerate
-00001080: 202a 2064 7572 6174 696f 6e29 0d0a 2020   * duration)..  
-00001090: 2020 2020 2020 6461 7461 203d 2073 656c        data = sel
-000010a0: 662e 5f73 616d 706c 6573 2e64 6174 610d  f._samples.data.
-000010b0: 0a20 2020 2020 2020 2064 6174 615b 3a66  .        data[:f
-000010c0: 7261 6d65 735d 203d 2028 6461 7461 5b3a  rames] = (data[:
-000010d0: 6672 616d 6573 5d20 2a20 6e70 2e6c 696e  frames] * np.lin
-000010e0: 7370 6163 6528 302c 2031 2c20 6672 616d  space(0, 1, fram
-000010f0: 6573 2929 2e61 7374 7970 6528 6e70 2e69  es)).astype(np.i
-00001100: 6e74 3136 290d 0a20 2020 2020 2020 2073  nt16)..        s
-00001110: 656c 662e 5f73 616d 706c 6573 2e64 6174  elf._samples.dat
-00001120: 6120 3d20 6461 7461 0d0a 0d0a 2020 2020  a = data....    
-00001130: 2020 2020 7265 7475 726e 2073 656c 660d      return self.
-00001140: 0a0d 0a20 2020 2064 6566 2066 6164 655f  ...    def fade_
-00001150: 6f75 7428 7365 6c66 2c20 6475 7261 7469  out(self, durati
-00001160: 6f6e 3a20 666c 6f61 7429 202d 3e20 5365  on: float) -> Se
-00001170: 6c66 3a0d 0a20 2020 2020 2020 2027 2727  lf:..        '''
-00001180: 0d0a 2020 2020 2020 2020 e5ba 94e7 94a8  ..        ......
-00001190: 2060 6064 7572 6174 696f 6e60 6020 e7a7   ``duration`` ..
-000011a0: 92e7 9a84 e6b7 a1e5 87ba 0d0a 2020 2020  ............    
-000011b0: 2020 2020 2727 270d 0a20 2020 2020 2020      '''..       
-000011c0: 2066 7261 6d65 7320 3d20 696e 7428 7365   frames = int(se
-000011d0: 6c66 2e66 7261 6d65 7261 7465 202a 2064  lf.framerate * d
-000011e0: 7572 6174 696f 6e29 0d0a 2020 2020 2020  uration)..      
-000011f0: 2020 6461 7461 203d 2073 656c 662e 5f73    data = self._s
-00001200: 616d 706c 6573 2e64 6174 610d 0a20 2020  amples.data..   
-00001210: 2020 2020 2064 6174 615b 2d66 7261 6d65       data[-frame
-00001220: 733a 5d20 3d20 2864 6174 615b 2d66 7261  s:] = (data[-fra
-00001230: 6d65 733a 5d20 2a20 6e70 2e6c 696e 7370  mes:] * np.linsp
-00001240: 6163 6528 312c 2030 2c20 6672 616d 6573  ace(1, 0, frames
-00001250: 2929 2e61 7374 7970 6528 6e70 2e69 6e74  )).astype(np.int
-00001260: 3136 290d 0a20 2020 2020 2020 2073 656c  16)..        sel
-00001270: 662e 5f73 616d 706c 6573 2e64 6174 6120  f._samples.data 
-00001280: 3d20 6461 7461 0d0a                      = data..
+00000090: 0d0a 6672 6f6d 206a 616e 696d 2e65 7863  ..from janim.exc
+000000a0: 6570 7469 6f6e 2069 6d70 6f72 7420 4558  eption import EX
+000000b0: 4954 434f 4445 5f46 464d 5045 475f 4e4f  ITCODE_FFMPEG_NO
+000000c0: 545f 464f 554e 442c 2045 7869 7445 7863  T_FOUND, ExitExc
+000000d0: 6570 7469 6f6e 0d0a 6672 6f6d 206a 616e  eption..from jan
+000000e0: 696d 2e6c 6f67 6765 7220 696d 706f 7274  im.logger import
+000000f0: 206c 6f67 0d0a 6672 6f6d 206a 616e 696d   log..from janim
+00000100: 2e75 7469 6c73 2e63 6f6e 6669 6720 696d  .utils.config im
+00000110: 706f 7274 2043 6f6e 6669 670d 0a66 726f  port Config..fro
+00000120: 6d20 6a61 6e69 6d2e 7574 696c 732e 6461  m janim.utils.da
+00000130: 7461 2069 6d70 6f72 7420 4172 7261 790d  ta import Array.
+00000140: 0a66 726f 6d20 6a61 6e69 6d2e 7574 696c  .from janim.util
+00000150: 732e 6669 6c65 5f6f 7073 2069 6d70 6f72  s.file_ops impor
+00000160: 7420 6669 6e64 5f66 696c 650d 0a66 726f  t find_file..fro
+00000170: 6d20 6a61 6e69 6d2e 7574 696c 732e 6974  m janim.utils.it
+00000180: 6572 6162 6c65 7320 696d 706f 7274 2072  erables import r
+00000190: 6573 697a 655f 7769 7468 5f69 6e74 6572  esize_with_inter
+000001a0: 706f 6c61 7469 6f6e 0d0a 6672 6f6d 206a  polation..from j
+000001b0: 616e 696d 2e75 7469 6c73 2e73 696d 706c  anim.utils.simpl
+000001c0: 655f 6675 6e63 7469 6f6e 7320 696d 706f  e_functions impo
+000001d0: 7274 2063 6c69 700d 0a0d 0a0d 0a63 6c61  rt clip......cla
+000001e0: 7373 2041 7564 696f 3a0d 0a20 2020 2027  ss Audio:..    '
+000001f0: 2727 0d0a 2020 2020 e4b8 8de5 bbba e8ae  ''..    ........
+00000200: aee4 bdbf e794 a8e8 afa5 e7b1 bbe5 a484  ................
+00000210: e790 86e5 a49a e5a3 b0e9 8193 e99f b3e9  ................
+00000220: a291 efbc 8ce5 9ba0 e4b8 bae8 afa5 e7b1  ................
+00000230: bbe8 afbb e58f 96e6 97b6 e4bb 85e4 bf9d  ................
+00000240: e795 99e5 8d95 e5a3 b0e9 8193 0d0a 2020  ..............  
+00000250: 2020 2727 270d 0a0d 0a20 2020 2061 7564    '''....    aud
+00000260: 696f 5f63 6163 6865 5f6d 6170 3a20 6469  io_cache_map: di
+00000270: 6374 5b74 7570 6c65 2c20 7475 706c 655b  ct[tuple, tuple[
+00000280: 6e70 2e6e 6461 7272 6179 2c20 696e 742c  np.ndarray, int,
+00000290: 2073 7472 2c20 7374 725d 5d20 3d20 7b7d   str, str]] = {}
+000002a0: 0d0a 0d0a 2020 2020 6465 6620 5f5f 696e  ....    def __in
+000002b0: 6974 5f5f 2873 656c 662c 2066 696c 655f  it__(self, file_
+000002c0: 7061 7468 3a20 7374 722c 2062 6567 696e  path: str, begin
+000002d0: 3a20 666c 6f61 7420 3d20 2d31 2c20 656e  : float = -1, en
+000002e0: 643a 2066 6c6f 6174 203d 202d 312c 202a  d: float = -1, *
+000002f0: 2a6b 7761 7267 7329 3a0d 0a20 2020 2020  *kwargs):..     
+00000300: 2020 2073 7570 6572 2829 2e5f 5f69 6e69     super().__ini
+00000310: 745f 5f28 2a2a 6b77 6172 6773 290d 0a20  t__(**kwargs).. 
+00000320: 2020 2020 2020 2073 656c 662e 5f73 616d         self._sam
+00000330: 706c 6573 203d 2041 7272 6179 2864 7479  ples = Array(dty
+00000340: 7065 3d6e 702e 696e 7431 3629 0d0a 2020  pe=np.int16)..  
+00000350: 2020 2020 2020 7365 6c66 2e66 7261 6d65        self.frame
+00000360: 7261 7465 203d 2030 0d0a 2020 2020 2020  rate = 0..      
+00000370: 2020 7365 6c66 2e66 696c 655f 7061 7468    self.file_path
+00000380: 203d 2027 270d 0a20 2020 2020 2020 2073   = ''..        s
+00000390: 656c 662e 6669 6c65 6e61 6d65 203d 2027  elf.filename = '
+000003a0: 270d 0a20 2020 2020 2020 2073 656c 662e  '..        self.
+000003b0: 7265 6164 2866 696c 655f 7061 7468 2c20  read(file_path, 
+000003c0: 6265 6769 6e2c 2065 6e64 290d 0a0d 0a20  begin, end).... 
+000003d0: 2020 2064 6566 2063 6f70 7928 7365 6c66     def copy(self
+000003e0: 2920 2d3e 2053 656c 663a 0d0a 2020 2020  ) -> Self:..    
+000003f0: 2020 2020 636f 7079 5f61 7564 696f 203d      copy_audio =
+00000400: 2063 6f70 792e 636f 7079 2873 656c 6629   copy.copy(self)
+00000410: 0d0a 2020 2020 2020 2020 636f 7079 5f61  ..        copy_a
+00000420: 7564 696f 2e5f 7361 6d70 6c65 7320 3d20  udio._samples = 
+00000430: 7365 6c66 2e5f 7361 6d70 6c65 732e 636f  self._samples.co
+00000440: 7079 2829 0d0a 2020 2020 2020 2020 7265  py()..        re
+00000450: 7475 726e 2063 6f70 795f 6175 6469 6f0d  turn copy_audio.
+00000460: 0a0d 0a20 2020 2064 6566 2072 6561 6428  ...    def read(
+00000470: 0d0a 2020 2020 2020 2020 7365 6c66 2c0d  ..        self,.
+00000480: 0a20 2020 2020 2020 2066 696c 655f 7061  .        file_pa
+00000490: 7468 3a20 7374 722c 0d0a 2020 2020 2020  th: str,..      
+000004a0: 2020 6265 6769 6e3a 2066 6c6f 6174 203d    begin: float =
+000004b0: 202d 312c 0d0a 2020 2020 2020 2020 656e   -1,..        en
+000004c0: 643a 2066 6c6f 6174 203d 202d 310d 0a20  d: float = -1.. 
+000004d0: 2020 2029 202d 3e20 5365 6c66 3a0d 0a20     ) -> Self:.. 
+000004e0: 2020 2020 2020 2027 2727 0d0a 2020 2020         '''..    
+000004f0: 2020 2020 e4bb 8ee6 9687 e4bb b6e4 b8ad      ............
+00000500: e8af bbe5 8f96 e99f b3e9 a291 0d0a 0d0a  ................
+00000510: 2020 2020 2020 2020 e58f afe4 bba5 e68c          ........
+00000520: 87e5 ae9a 2060 6062 6567 696e 6060 20e5  .... ``begin`` .
+00000530: 928c 2060 6065 6e64 6060 20e6 9da5 e688  .. ``end`` .....
+00000540: aae5 8f96 e99f b3e9 a291 e79a 84e4 b880  ................
+00000550: e983 a8e5 8886 0d0a 2020 2020 2020 2020  ........        
+00000560: 2727 270d 0a20 2020 2020 2020 2074 7279  '''..        try
+00000570: 3a0d 0a20 2020 2020 2020 2020 2020 2066  :..            f
+00000580: 696c 655f 7061 7468 203d 2066 696e 645f  ile_path = find_
+00000590: 6669 6c65 2866 696c 655f 7061 7468 290d  file(file_path).
+000005a0: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+000005b0: 4669 6c65 4e6f 7446 6f75 6e64 4572 726f  FileNotFoundErro
+000005c0: 723a 0d0a 2020 2020 2020 2020 2020 2020  r:..            
+000005d0: 6c6f 672e 7761 726e 696e 6728 6627 e697  log.warning(f'..
+000005e0: a0e6 b395 e689 bee5 88b0 e99f b3e9 a291  ................
+000005f0: 2022 7b66 696c 655f 7061 7468 7d22 efbc   "{file_path}"..
+00000600: 8ce5 b7b2 e4bd bfe7 94a8 2038 7320 e79a  .......... 8s ..
+00000610: 84e7 a9ba e799 bde9 9fb3 e9a2 91e4 bba3  ................
+00000620: e69b bf27 290d 0a20 2020 2020 2020 2020  ...')..         
+00000630: 2020 2073 656c 662e 5f73 616d 706c 6573     self._samples
+00000640: 2e64 6174 6120 3d20 6e70 2e7a 6572 6f73  .data = np.zeros
+00000650: 2843 6f6e 6669 672e 6765 742e 6175 6469  (Config.get.audi
+00000660: 6f5f 6672 616d 6572 6174 6520 2a20 3829  o_framerate * 8)
+00000670: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00000680: 6c66 2e66 7261 6d65 7261 7465 203d 2043  lf.framerate = C
+00000690: 6f6e 6669 672e 6765 742e 6175 6469 6f5f  onfig.get.audio_
+000006a0: 6672 616d 6572 6174 650d 0a20 2020 2020  framerate..     
+000006b0: 2020 2020 2020 2073 656c 662e 6669 6c65         self.file
+000006c0: 5f70 6174 6820 3d20 6669 6c65 5f70 6174  _path = file_pat
+000006d0: 680d 0a20 2020 2020 2020 2020 2020 2073  h..            s
+000006e0: 656c 662e 6669 6c65 6e61 6d65 203d 206f  elf.filename = o
+000006f0: 732e 7061 7468 2e62 6173 656e 616d 6528  s.path.basename(
+00000700: 6669 6c65 5f70 6174 6829 0d0a 2020 2020  file_path)..    
+00000710: 2020 2020 2020 2020 7265 7475 726e 0d0a          return..
+00000720: 0d0a 2020 2020 2020 2020 6d74 696d 6520  ..        mtime 
+00000730: 3d20 6f73 2e70 6174 682e 6765 746d 7469  = os.path.getmti
+00000740: 6d65 2866 696c 655f 7061 7468 290d 0a20  me(file_path).. 
+00000750: 2020 2020 2020 206e 616d 6520 3d20 6f73         name = os
+00000760: 2e70 6174 682e 7370 6c69 7465 7874 286f  .path.splitext(o
+00000770: 732e 7061 7468 2e62 6173 656e 616d 6528  s.path.basename(
+00000780: 6669 6c65 5f70 6174 6829 295b 305d 0d0a  file_path))[0]..
+00000790: 2020 2020 2020 2020 6b65 7920 3d20 286e          key = (n
+000007a0: 616d 652c 206d 7469 6d65 2c20 6265 6769  ame, mtime, begi
+000007b0: 6e2c 2065 6e64 290d 0a0d 0a20 2020 2020  n, end)....     
+000007c0: 2020 2063 6163 6865 6420 3d20 7365 6c66     cached = self
+000007d0: 2e61 7564 696f 5f63 6163 6865 5f6d 6170  .audio_cache_map
+000007e0: 2e67 6574 286b 6579 2c20 4e6f 6e65 290d  .get(key, None).
+000007f0: 0a20 2020 2020 2020 2069 6620 6361 6368  .        if cach
+00000800: 6564 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ed is not None:.
+00000810: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00000820: 662e 5f73 616d 706c 6573 2e64 6174 612c  f._samples.data,
+00000830: 2073 656c 662e 6672 616d 6572 6174 652c   self.framerate,
+00000840: 2073 656c 662e 6669 6c65 5f70 6174 682c   self.file_path,
+00000850: 2073 656c 662e 6669 6c65 6e61 6d65 203d   self.filename =
+00000860: 2063 6163 6865 640d 0a20 2020 2020 2020   cached..       
+00000870: 2020 2020 2072 6574 7572 6e0d 0a0d 0a20       return.... 
+00000880: 2020 2020 2020 2063 6f6d 6d61 6e64 203d         command =
+00000890: 205b 0d0a 2020 2020 2020 2020 2020 2020   [..            
+000008a0: 436f 6e66 6967 2e67 6574 2e66 666d 7065  Config.get.ffmpe
+000008b0: 675f 6269 6e2c 0d0a 2020 2020 2020 2020  g_bin,..        
+000008c0: 2020 2020 272d 766e 272c 0d0a 2020 2020      '-vn',..    
+000008d0: 2020 2020 2020 2020 272d 6927 2c20 6669          '-i', fi
+000008e0: 6c65 5f70 6174 682c 0d0a 2020 2020 2020  le_path,..      
+000008f0: 2020 5d0d 0a20 2020 2020 2020 2069 6620    ]..        if 
+00000900: 6265 6769 6e20 213d 202d 313a 0d0a 2020  begin != -1:..  
+00000910: 2020 2020 2020 2020 2020 636f 6d6d 616e            comman
+00000920: 6420 2b3d 205b 272d 7373 272c 2073 7472  d += ['-ss', str
+00000930: 2862 6567 696e 295d 2020 2320 636c 6970  (begin)]  # clip
+00000940: 2066 726f 6d0d 0a20 2020 2020 2020 2069   from..        i
+00000950: 6620 656e 6420 213d 202d 313a 0d0a 2020  f end != -1:..  
+00000960: 2020 2020 2020 2020 2020 636f 6d6d 616e            comman
+00000970: 6420 2b3d 205b 272d 746f 272c 2073 7472  d += ['-to', str
+00000980: 2865 6e64 295d 2020 2020 2320 636c 6970  (end)]    # clip
+00000990: 2074 6f0d 0a0d 0a20 2020 2020 2020 2063   to....        c
+000009a0: 6f6d 6d61 6e64 202b 3d20 5b0d 0a20 2020  ommand += [..   
+000009b0: 2020 2020 2020 2020 2027 2d66 272c 2027           '-f', '
+000009c0: 7331 366c 6527 2c0d 0a20 2020 2020 2020  s16le',..       
+000009d0: 2020 2020 2027 2d61 636f 6465 6327 2c20       '-acodec', 
+000009e0: 2770 636d 5f73 3136 6c65 272c 0d0a 2020  'pcm_s16le',..  
+000009f0: 2020 2020 2020 2020 2020 272d 6172 272c            '-ar',
+00000a00: 2073 7472 2843 6f6e 6669 672e 6765 742e   str(Config.get.
+00000a10: 6175 6469 6f5f 6672 616d 6572 6174 6529  audio_framerate)
+00000a20: 2c20 2020 2020 2320 6672 616d 6572 6174  ,     # framerat
+00000a30: 6520 2620 7361 6d70 6c65 7261 7465 0d0a  e & samplerate..
+00000a40: 2020 2020 2020 2020 2020 2020 272d 6163              '-ac
+00000a50: 272c 2027 3127 2c0d 0a20 2020 2020 2020  ', '1',..       
+00000a60: 2020 2020 2027 2d6c 6f67 6c65 7665 6c27       '-loglevel'
+00000a70: 2c20 2765 7272 6f72 272c 0d0a 2020 2020  , 'error',..    
+00000a80: 2020 2020 2020 2020 272d 272c 2020 2020          '-',    
+00000a90: 2320 6f75 7470 7574 2074 6f20 6120 7069  # output to a pi
+00000aa0: 7065 0d0a 2020 2020 2020 2020 5d0d 0a0d  pe..        ]...
+00000ab0: 0a20 2020 2020 2020 2074 7279 3a0d 0a20  .        try:.. 
+00000ac0: 2020 2020 2020 2020 2020 2023 2054 4f44             # TOD
+00000ad0: 4f3a 2073 7570 706f 7274 206d 6f72 6520  O: support more 
+00000ae0: 7361 6d70 7769 6474 680d 0a20 2020 2020  sampwidth..     
+00000af0: 2020 2020 2020 2023 2054 4f44 4f3a 2066         # TODO: f
+00000b00: 6978 2042 7974 654f 7264 6572 0d0a 2020  ix ByteOrder..  
+00000b10: 2020 2020 2020 2020 2020 7769 7468 2073            with s
+00000b20: 702e 506f 7065 6e28 636f 6d6d 616e 642c  p.Popen(command,
+00000b30: 2073 7464 6f75 743d 7370 2e50 4950 4529   stdout=sp.PIPE)
+00000b40: 2061 7320 7265 6164 696e 675f 7072 6f63   as reading_proc
+00000b50: 6573 733a 0d0a 2020 2020 2020 2020 2020  ess:..          
+00000b60: 2020 2020 2020 6461 7461 203d 206e 702e        data = np.
+00000b70: 6672 6f6d 6275 6666 6572 2872 6561 6469  frombuffer(readi
+00000b80: 6e67 5f70 726f 6365 7373 2e73 7464 6f75  ng_process.stdou
+00000b90: 742e 7265 6164 2829 2c20 6474 7970 653d  t.read(), dtype=
+00000ba0: 6e70 2e69 6e74 3136 290d 0a0d 0a20 2020  np.int16)....   
+00000bb0: 2020 2020 2065 7863 6570 7420 4669 6c65       except File
+00000bc0: 4e6f 7446 6f75 6e64 4572 726f 723a 0d0a  NotFoundError:..
+00000bd0: 2020 2020 2020 2020 2020 2020 6c6f 672e              log.
+00000be0: 6572 726f 7228 27e6 97a0 e6b3 95e8 afbb  error('.........
+00000bf0: e58f 96e9 9fb3 e9a2 91ef bc8c e99c 80e8  ................
+00000c00: a681 e5ae 89e8 a385 2066 666d 7065 6720  ........ ffmpeg 
+00000c10: e5b9 b6e5 b086 e585 b6e6 b7bb e58a a0e5  ................
+00000c20: 88b0 e78e afe5 a283 e58f 98e9 878f e4b8  ................
+00000c30: ad27 290d 0a20 2020 2020 2020 2020 2020  .')..           
+00000c40: 2072 6169 7365 2045 7869 7445 7863 6570   raise ExitExcep
+00000c50: 7469 6f6e 2845 5849 5443 4f44 455f 4646  tion(EXITCODE_FF
+00000c60: 4d50 4547 5f4e 4f54 5f46 4f55 4e44 290d  MPEG_NOT_FOUND).
+00000c70: 0a0d 0a20 2020 2020 2020 2073 656c 662e  ...        self.
+00000c80: 5f73 616d 706c 6573 2e64 6174 6120 3d20  _samples.data = 
+00000c90: 6461 7461 0d0a 2020 2020 2020 2020 7365  data..        se
+00000ca0: 6c66 2e66 7261 6d65 7261 7465 203d 2043  lf.framerate = C
+00000cb0: 6f6e 6669 672e 6765 742e 6175 6469 6f5f  onfig.get.audio_
+00000cc0: 6672 616d 6572 6174 650d 0a20 2020 2020  framerate..     
+00000cd0: 2020 2073 656c 662e 6669 6c65 5f70 6174     self.file_pat
+00000ce0: 6820 3d20 6669 6c65 5f70 6174 680d 0a20  h = file_path.. 
+00000cf0: 2020 2020 2020 2073 656c 662e 6669 6c65         self.file
+00000d00: 6e61 6d65 203d 206f 732e 7061 7468 2e62  name = os.path.b
+00000d10: 6173 656e 616d 6528 6669 6c65 5f70 6174  asename(file_pat
+00000d20: 6829 0d0a 2020 2020 2020 2020 7365 6c66  h)..        self
+00000d30: 2e61 7564 696f 5f63 6163 6865 5f6d 6170  .audio_cache_map
+00000d40: 5b6b 6579 5d20 3d20 2864 6174 612c 2073  [key] = (data, s
+00000d50: 656c 662e 6672 616d 6572 6174 652c 2073  elf.framerate, s
+00000d60: 656c 662e 6669 6c65 5f70 6174 682c 2073  elf.file_path, s
+00000d70: 656c 662e 6669 6c65 6e61 6d65 290d 0a0d  elf.filename)...
+00000d80: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00000d90: 7365 6c66 0d0a 0d0a 2020 2020 6465 6620  self....    def 
+00000da0: 7361 6d70 6c65 5f63 6f75 6e74 2873 656c  sample_count(sel
+00000db0: 6629 202d 3e20 696e 743a 0d0a 2020 2020  f) -> int:..    
+00000dc0: 2020 2020 2727 270d 0a20 2020 2020 2020      '''..       
+00000dd0: 20e6 8980 e69c 89e9 8787 e6a0 b7e7 82b9   ...............
+00000de0: e79a 84e6 95b0 e987 8f0d 0a20 2020 2020  ...........     
+00000df0: 2020 2027 2727 0d0a 2020 2020 2020 2020     '''..        
+00000e00: 7265 7475 726e 206c 656e 2873 656c 662e  return len(self.
+00000e10: 5f73 616d 706c 6573 2e64 6174 6129 0d0a  _samples.data)..
+00000e20: 0d0a 2020 2020 6465 6620 6475 7261 7469  ..    def durati
+00000e30: 6f6e 2873 656c 6629 202d 3e20 666c 6f61  on(self) -> floa
+00000e40: 743a 0d0a 2020 2020 2020 2020 2727 270d  t:..        '''.
+00000e50: 0a20 2020 2020 2020 20e6 8c81 e7bb ade6  .        .......
+00000e60: 97b6 e997 b40d 0a20 2020 2020 2020 2027  .......        '
+00000e70: 2727 0d0a 2020 2020 2020 2020 7265 7475  ''..        retu
+00000e80: 726e 2073 656c 662e 7361 6d70 6c65 5f63  rn self.sample_c
+00000e90: 6f75 6e74 2829 202f 2073 656c 662e 6672  ount() / self.fr
+00000ea0: 616d 6572 6174 650d 0a0d 0a20 2020 2064  amerate....    d
+00000eb0: 6566 2063 6c69 7028 7365 6c66 2c20 6265  ef clip(self, be
+00000ec0: 6769 6e3a 2066 6c6f 6174 203d 2030 2c20  gin: float = 0, 
+00000ed0: 656e 643a 2066 6c6f 6174 203d 202d 3129  end: float = -1)
+00000ee0: 202d 3e20 5365 6c66 3a0d 0a20 2020 2020   -> Self:..     
+00000ef0: 2020 2027 2727 0d0a 2020 2020 2020 2020     '''..        
+00000f00: e8a3 81e5 89aa e99f b3e9 a291 0d0a 0d0a  ................
+00000f10: 2020 2020 2020 2020 2d20 e4bf 9de7 9599          - ......
+00000f20: 2060 6062 6567 696e 6060 20e5 88b0 2060   ``begin`` ... `
+00000f30: 6065 6e64 6060 20e4 b98b e997 b4e7 9a84  `end`` .........
+00000f40: e983 a8e5 8886 0d0a 2020 2020 2020 2020  ........        
+00000f50: 2d20 e88b a520 6060 6265 6769 6e60 6020  - ... ``begin`` 
+00000f60: e7bc bae7 9c81 efbc 8ce5 8899 e8a1 a8e7  ................
+00000f70: a4ba e4bb 8ee6 9c80 e5bc 80e5 a78b 0d0a  ................
+00000f80: 2020 2020 2020 2020 2d20 e88b a520 6060          - ... ``
+00000f90: 656e 6460 6020 e7bc bae7 9c81 2860 602d  end`` ......(``-
+00000fa0: 3160 6029 efbc 8ce5 8899 e8a1 a8e7 a4ba  1``)............
+00000fb0: e588 b0e6 9c80 e69c abe5 b0be 0d0a 2020  ..............  
+00000fc0: 2020 2020 2020 2727 270d 0a20 2020 2020        '''..     
+00000fd0: 2020 2066 7261 6d65 5f62 6567 696e 203d     frame_begin =
+00000fe0: 2063 6c69 7028 696e 7428 6265 6769 6e20   clip(int(begin 
+00000ff0: 2a20 7365 6c66 2e66 7261 6d65 7261 7465  * self.framerate
+00001000: 292c 2030 2c20 7365 6c66 2e73 616d 706c  ), 0, self.sampl
+00001010: 655f 636f 756e 7428 2929 0d0a 2020 2020  e_count())..    
+00001020: 2020 2020 6966 2065 6e64 203d 3d20 2d31      if end == -1
+00001030: 3a0d 0a20 2020 2020 2020 2020 2020 2066  :..            f
+00001040: 7261 6d65 5f65 6e64 203d 2073 656c 662e  rame_end = self.
+00001050: 7361 6d70 6c65 5f63 6f75 6e74 2829 0d0a  sample_count()..
+00001060: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00001070: 2020 2020 2020 2020 2020 2066 7261 6d65             frame
+00001080: 5f65 6e64 203d 2063 6c69 7028 696e 7428  _end = clip(int(
+00001090: 656e 6420 2a20 7365 6c66 2e66 7261 6d65  end * self.frame
+000010a0: 7261 7465 292c 2030 2c20 7365 6c66 2e73  rate), 0, self.s
+000010b0: 616d 706c 655f 636f 756e 7428 2929 0d0a  ample_count())..
+000010c0: 2020 2020 2020 2020 7365 6c66 2e5f 7361          self._sa
+000010d0: 6d70 6c65 732e 6461 7461 203d 2073 656c  mples.data = sel
+000010e0: 662e 5f73 616d 706c 6573 2e64 6174 615b  f._samples.data[
+000010f0: 6672 616d 655f 6265 6769 6e3a 6672 616d  frame_begin:fram
+00001100: 655f 656e 645d 0d0a 0d0a 2020 2020 2020  e_end]....      
+00001110: 2020 7265 7475 726e 2073 656c 660d 0a0d    return self...
+00001120: 0a20 2020 2064 6566 206d 756c 2873 656c  .    def mul(sel
+00001130: 662c 2076 616c 7565 3a20 666c 6f61 7420  f, value: float 
+00001140: 7c20 4974 6572 6162 6c65 5b66 6c6f 6174  | Iterable[float
+00001150: 5d29 202d 3e20 5365 6c66 3a0d 0a20 2020  ]) -> Self:..   
+00001160: 2020 2020 2027 2727 0d0a 2020 2020 2020       '''..      
+00001170: 2020 e4b9 98e4 bba5 e7bb 99e5 ae9a e79a    ..............
+00001180: 8420 6060 7661 6c75 6560 60ef bc8c 6060  . ``value``...``
+00001190: 7661 6c75 6560 6020 e58f afe4 bba5 e590  value`` ........
+000011a0: abe6 9c89 e5a4 9ae4 b8aa e585 83e7 b4a0  ................
+000011b0: efbc 88e6 af94 e5a6 82e4 b880 e4b8 aae5  ................
+000011c0: 8897 e8a1 a8ef bc89 0d0a 0d0a 2020 2020  ............    
+000011d0: 2020 2020 e4be 8be5 a682 efbc 9a0d 0a0d      ............
+000011e0: 0a20 2020 2020 2020 202d 2060 6061 7564  .        - ``aud
+000011f0: 696f 2e6d 756c 2830 2e35 2960 6020 e58f  io.mul(0.5)`` ..
+00001200: afe4 bba5 e4bd bfe9 9fb3 e9ab 98e5 878f  ................
+00001210: e58d 8a0d 0a20 2020 2020 2020 202d 2060  .....        - `
+00001220: 6061 7564 696f 2e6d 756c 285b 312c 2030  `audio.mul([1, 0
+00001230: 5d29 6060 20e5 8faf e4bb a5e4 bdbf e5bc  ])`` ...........
+00001240: 80e5 a78b e697 b6e6 9c80 e5bc baef bc8c  ................
+00001250: e7bb 93e6 9d9f e697 b6e6 9c80 e5bc b10d  ................
+00001260: 0a20 2020 2020 2020 202d 2060 6061 7564  .        - ``aud
+00001270: 696f 2e6d 756c 286e 702e 7369 6e28 6e70  io.mul(np.sin(np
+00001280: 2e6c 696e 7370 6163 6528 302c 2032 202a  .linspace(0, 2 *
+00001290: 206e 702e 7069 2c20 6175 6469 6f2e 7361   np.pi, audio.sa
+000012a0: 6d70 6c65 5f63 6f75 6e74 2829 2929 2960  mple_count())))`
+000012b0: 6020 e58f afe4 bba5 e4bd bfe9 9fb3 e9ab  ` ..............
+000012c0: 98e9 9a8f e697 b6e9 97b4 e4b9 98e4 bba5  ................
+000012d0: 2073 696e 20e5 87bd e695 b0e7 9a84 e4b8   sin ...........
+000012e0: 80e4 b8aa e591 a8e6 9c9f 0d0a 2020 2020  ............    
+000012f0: 2020 2020 2727 270d 0a20 2020 2020 2020      '''..       
+00001300: 2069 6620 6973 696e 7374 616e 6365 2876   if isinstance(v
+00001310: 616c 7565 2c20 4974 6572 6162 6c65 293a  alue, Iterable):
+00001320: 0d0a 2020 2020 2020 2020 2020 2020 7661  ..            va
+00001330: 6c75 6520 3d20 7265 7369 7a65 5f77 6974  lue = resize_wit
+00001340: 685f 696e 7465 7270 6f6c 6174 696f 6e28  h_interpolation(
+00001350: 7661 6c75 652c 2073 656c 662e 7361 6d70  value, self.samp
+00001360: 6c65 5f63 6f75 6e74 2829 290d 0a20 2020  le_count())..   
+00001370: 2020 2020 2073 656c 662e 5f73 616d 706c       self._sampl
+00001380: 6573 2e64 6174 6120 3d20 7365 6c66 2e5f  es.data = self._
+00001390: 7361 6d70 6c65 732e 6461 7461 202a 2076  samples.data * v
+000013a0: 616c 7565 0d0a 0d0a 2020 2020 2020 2020  alue....        
+000013b0: 7265 7475 726e 2073 656c 660d 0a0d 0a20  return self.... 
+000013c0: 2020 2064 6566 2066 6164 655f 696e 2873     def fade_in(s
+000013d0: 656c 662c 2064 7572 6174 696f 6e3a 2066  elf, duration: f
+000013e0: 6c6f 6174 2920 2d3e 2053 656c 663a 0d0a  loat) -> Self:..
+000013f0: 2020 2020 2020 2020 2727 270d 0a20 2020          '''..   
+00001400: 2020 2020 20e5 ba94 e794 a820 6060 6475       ...... ``du
+00001410: 7261 7469 6f6e 6060 20e7 a792 e79a 84e6  ration`` .......
+00001420: b7a1 e585 a50d 0a20 2020 2020 2020 2027  .......        '
+00001430: 2727 0d0a 2020 2020 2020 2020 6672 616d  ''..        fram
+00001440: 6573 203d 2069 6e74 2873 656c 662e 6672  es = int(self.fr
+00001450: 616d 6572 6174 6520 2a20 6475 7261 7469  amerate * durati
+00001460: 6f6e 290d 0a20 2020 2020 2020 2064 6174  on)..        dat
+00001470: 6120 3d20 7365 6c66 2e5f 7361 6d70 6c65  a = self._sample
+00001480: 732e 6461 7461 0d0a 2020 2020 2020 2020  s.data..        
+00001490: 6461 7461 5b3a 6672 616d 6573 5d20 3d20  data[:frames] = 
+000014a0: 2864 6174 615b 3a66 7261 6d65 735d 202a  (data[:frames] *
+000014b0: 206e 702e 6c69 6e73 7061 6365 2830 2c20   np.linspace(0, 
+000014c0: 312c 2066 7261 6d65 7329 292e 6173 7479  1, frames)).asty
+000014d0: 7065 286e 702e 696e 7431 3629 0d0a 2020  pe(np.int16)..  
+000014e0: 2020 2020 2020 7365 6c66 2e5f 7361 6d70        self._samp
+000014f0: 6c65 732e 6461 7461 203d 2064 6174 610d  les.data = data.
+00001500: 0a0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
+00001510: 6e20 7365 6c66 0d0a 0d0a 2020 2020 6465  n self....    de
+00001520: 6620 6661 6465 5f6f 7574 2873 656c 662c  f fade_out(self,
+00001530: 2064 7572 6174 696f 6e3a 2066 6c6f 6174   duration: float
+00001540: 2920 2d3e 2053 656c 663a 0d0a 2020 2020  ) -> Self:..    
+00001550: 2020 2020 2727 270d 0a20 2020 2020 2020      '''..       
+00001560: 20e5 ba94 e794 a820 6060 6475 7261 7469   ...... ``durati
+00001570: 6f6e 6060 20e7 a792 e79a 84e6 b7a1 e587  on`` ...........
+00001580: ba0d 0a20 2020 2020 2020 2027 2727 0d0a  ...        '''..
+00001590: 2020 2020 2020 2020 6672 616d 6573 203d          frames =
+000015a0: 2069 6e74 2873 656c 662e 6672 616d 6572   int(self.framer
+000015b0: 6174 6520 2a20 6475 7261 7469 6f6e 290d  ate * duration).
+000015c0: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
+000015d0: 7365 6c66 2e5f 7361 6d70 6c65 732e 6461  self._samples.da
+000015e0: 7461 0d0a 2020 2020 2020 2020 6461 7461  ta..        data
+000015f0: 5b2d 6672 616d 6573 3a5d 203d 2028 6461  [-frames:] = (da
+00001600: 7461 5b2d 6672 616d 6573 3a5d 202a 206e  ta[-frames:] * n
+00001610: 702e 6c69 6e73 7061 6365 2831 2c20 302c  p.linspace(1, 0,
+00001620: 2066 7261 6d65 7329 292e 6173 7479 7065   frames)).astype
+00001630: 286e 702e 696e 7431 3629 0d0a 2020 2020  (np.int16)..    
+00001640: 2020 2020 7365 6c66 2e5f 7361 6d70 6c65      self._sample
+00001650: 732e 6461 7461 203d 2064 6174 610d 0a    s.data = data..
```

### Comparing `janim-0.5.2/janim/items/boolean_ops.py` & `janim-1.0.0/janim/items/boolean_ops.py`

 * *Files identical despite different names*

### Comparing `janim-0.5.2/janim/items/coordinate/coordinate_systems.py` & `janim-1.0.0/janim/items/coordinate/coordinate_systems.py`

 * *Files 6% similar despite different names*

```diff
@@ -140,39 +140,33 @@
             t_range=tuple(t_range),
             **kwargs
         )
 
         if bind:
             Cmpt_Points.apply_points_fn.connect(
                 self.points,
-                lambda func, about_point: graph.points.apply_points_fn(func, about_point=about_point)
+                lambda func, about_point: graph.points.apply_points_fn(func,
+                                                                       about_point=about_point,
+                                                                       about_edge=None)
             )
 
         return graph
 
 
 class CmptVPoints_NumberPlaneImpl(Cmpt_VPoints, impl=True):
     def prepare_for_nonlinear_transform(self, num_inserted_curves: int = 50, *, root_only=False) -> Self:
-        def apply(cmpt: Cmpt_VPoints):
-            if not cmpt.has():
-                return
+        for cmpt in self.walk_same_cmpt_of_self_and_descendants_without_mock(root_only):
+            if not isinstance(cmpt, Cmpt_VPoints) or not cmpt.has():
+                continue
+
             curves_count = cmpt.curves_count()
             if num_inserted_curves > curves_count:
                 cmpt.insert_n_curves(num_inserted_curves - curves_count)
             cmpt.make_smooth_after_applying_functions = True
 
-        if root_only or self.bind is None:
-            apply(self)
-        else:
-            for item in self.bind.at_item.walk_self_and_descendants():
-                cmpt = self.get_same_cmpt_without_mock(item)
-                if not isinstance(cmpt, Cmpt_VPoints):
-                    continue
-                apply(cmpt)
-
         return self
 
 
 class NumberPlane(Axes):
     points = CmptInfo(CmptVPoints_NumberPlaneImpl)
 
     axis_config_d: dict = dict(
@@ -222,16 +216,16 @@
             self.faded_line_style = style
 
         x_lines1, x_lines2 = self.get_lines_parallel_to_axis(self.x_axis, self.y_axis)
         y_lines1, y_lines2 = self.get_lines_parallel_to_axis(self.y_axis, self.x_axis)
         self.background_lines = Group(*x_lines1, *y_lines1)
         self.faded_lines = Group(*x_lines2, *y_lines2)
 
-        self.background_lines.digest_styles(self.background_line_style)
-        self.faded_lines.digest_styles(self.faded_line_style)
+        self.background_lines.digest_styles(**self.background_line_style)
+        self.faded_lines.digest_styles(**self.faded_line_style)
 
         self.add(
             self.faded_lines,
             self.background_lines,
             insert=True
         )
         self.depth.arrange()
```

### Comparing `janim-0.5.2/janim/items/coordinate/functions.py` & `janim-1.0.0/janim/items/coordinate/functions.py`

 * *Files identical despite different names*

### Comparing `janim-0.5.2/janim/items/coordinate/number_line.py` & `janim-1.0.0/janim/items/coordinate/number_line.py`

 * *Files identical despite different names*

### Comparing `janim-0.5.2/janim/items/geometry/arc.py` & `janim-1.0.0/janim/items/geometry/arc.py`

 * *Files 3% similar despite different names*

```diff
@@ -187,21 +187,21 @@
     点，半径默认为 ``0.08``
     '''
     def __init__(
         self,
         point: np.ndarray = ORIGIN,
         radius: float = DEFAULT_DOT_RADIUS,
         *,
-        stroke_radius: float | Iterable[float] | None = 0,
+        stroke_alpha: Alpha | AlphaArray | None = 0,
         fill_alpha: Alpha | AlphaArray | None = 1.0,
         **kwargs
     ) -> None:
         super().__init__(
             radius=radius,
-            stroke_radius=stroke_radius,
+            stroke_alpha=stroke_alpha,
             fill_alpha=fill_alpha,
             **kwargs
         )
         self.points.move_to(point)
 
 
 class SmallDot(Dot):
```

### Comparing `janim-0.5.2/janim/items/geometry/arrow.py` & `janim-1.0.0/janim/items/geometry/arrow.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,38 +69,38 @@
         self.rotate_about_anchor(angle)
 
     def get_center_anchor(self) -> np.ndarray:
         '''
         根据设定的 ``center_anchor`` 得到原点位置，
         请参考 :class:`ArrowTip.CenterAnchor`
         '''
-        points = self.points._points._data
+        points = self.points._points.data
         if self.center_anchor == CenterAnchor.Back:
             return points[3]
         if self.center_anchor == CenterAnchor.Center:
             return midpoint(points[0], points[3])
         # if self.center_anchor == CenterAnchor.Front:
         return points[0]
 
     @property
     def direction(self) -> np.ndarray:
         '''得到箭头的方向（单位向量）'''
-        points = self.points._points._data
+        points = self.points._points.data
         return normalize(points[0] - points[3])
 
     @property
     def body_length(self) -> float:
         '''得到箭头的长度'''
-        points = self.points._points._data
+        points = self.points._points.data
         return get_norm(points[0] - points[3])
 
     @property
     def back_width(self) -> float:
         '''得到箭头的宽度'''
-        points = self.points._points._data
+        points = self.points._points.data
         return get_norm(points[4] - points[2])
 
     def rotate_about_anchor(self, angle: float) -> Self:
         '''相对于原点位置进行旋转'''
         self.points.rotate(angle, about_point=self.get_center_anchor())
 
     def move_anchor_to(self, pos: np.ndarray) -> Self:
@@ -135,17 +135,20 @@
         self.init_tips(tip_kwargs)
         self.place_tip()
 
     def init_tips(self, tip_kwargs: dict) -> None:
         self.tip = self.add_tip(**tip_kwargs)
         self.tip_orig_body_length = self.tip.body_length
 
-    def copy(self) -> Self:
-        copy_item = super().copy()
-        copy_item.tip = copy_item[0]
+    def copy(self, *, root_only=False) -> Self:
+        copy_item = super().copy(root_only=root_only)
+        if root_only:
+            copy_item.tip = None
+        else:
+            copy_item.tip = copy_item[0]
         return copy_item
 
     def _place_tip(
         self,
         tip: ArrowTip,
         target: np.ndarray,
         target_direction: np.ndarray
@@ -194,17 +197,20 @@
     def __init__(self, *args, tip_kwargs: dict = {}, **kwargs) -> None:
         super().__init__(*args, tip_kwargs=tip_kwargs, **kwargs)
 
     def init_tips(self, tip_kwargs: dict) -> None:
         super().init_tips(tip_kwargs)
         self.start_tip = self.add_tip(0, True, **tip_kwargs)
 
-    def copy(self) -> Self:
-        copy_item = super().copy()
-        copy_item.start_tip = copy_item[1]
+    def copy(self, *, root_only=False) -> Self:
+        copy_item = super().copy(root_only=root_only)
+        if root_only:
+            copy_item.start_tip = None
+        else:
+            copy_item.start_tip = copy_item[1]
         return copy_item
 
     def place_tip(self) -> Self:
         super().place_tip()
         self._place_tip(self.start_tip, self.points.get_start(), -self.points.start_direction)
         return self
```

### Comparing `janim-0.5.2/janim/items/geometry/line.py` & `janim-1.0.0/janim/items/geometry/line.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,23 +4,22 @@
 from typing import Self
 
 import numpy as np
 
 from janim.components.component import CmptInfo
 from janim.components.vpoints import Cmpt_VPoints
 from janim.constants import LEFT, ORIGIN, RIGHT, UP
-from janim.items.item import Item
 from janim.items.points import Points
 from janim.items.vitem import VItem
 from janim.typing import Vect
 from janim.utils.bezier import PathBuilder
 from janim.utils.simple_functions import clip
 from janim.utils.space_ops import angle_of_vector, get_norm, normalize
 
-type SupportsPointify = Vect | Points | Item.Data[Item]
+type SupportsPointify = Vect | Points
 
 
 class Cmpt_VPoints_LineImpl[ItemT](Cmpt_VPoints[ItemT]):
     '''
     在线段中，对 :class:`~.Cmpt_VPoints` 的进一步实现
     '''
     def copy(self) -> Self:
@@ -34,16 +33,16 @@
         super().become(other)
         self.start = other.start.copy()
         self.end = other.end.copy()
         self.buff = other.buff
         self.path_arc = other.path_arc
         return self
 
-    def __eq__(self, other) -> bool:
-        return super().__eq__(other)
+    def not_changed(self, other) -> bool:
+        return super().not_changed(other)
 
     def put_start_and_end_on(self, start: Vect, end: Vect) -> Self:
         curr_start, curr_end = self.get_start_and_end()
         if np.isclose(curr_start, curr_end).all():
             # Handle null lines more gracefully
             self.update_points_by_attrs(start, end, buff=0, path_arc=self.path_arc)
             return self
@@ -116,26 +115,23 @@
         return (
             Cmpt_VPoints_LineImpl.pointify(start, vect),
             Cmpt_VPoints_LineImpl.pointify(end, -vect)
         )
 
     @staticmethod
     def pointify(
-        item_or_data_or_point: Vect | Points | Item.Data[Points],
+        item_or_data_or_point: SupportsPointify,
         direction: Vect | None = None
     ) -> np.ndarray:
         """
         Take an argument passed into Line (or subclass) and turn
         it into a 3d point.
         """
-        if isinstance(item_or_data_or_point, (Points, Item.Data)):
-            if isinstance(item_or_data_or_point, Points):
-                cmpt = item_or_data_or_point.points
-            else:
-                cmpt = item_or_data_or_point.cmpt.points
+        if isinstance(item_or_data_or_point, Points):
+            cmpt = item_or_data_or_point.points
 
             if direction is None:
                 return cmpt.box.center
             else:
                 return cmpt.box.get_continuous(direction)
         else:
             point = item_or_data_or_point
```

### Comparing `janim-0.5.2/janim/items/geometry/polygon.py` & `janim-1.0.0/janim/items/geometry/polygon.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 
 from typing import Iterable, Self, overload
 
 import numpy as np
 
-from janim.anims.timeline import Timeline
 from janim.constants import DL, DR, PI, RIGHT, UL, UR
 from janim.items.geometry.arc import ArcBetweenPoints
 from janim.items.vitem import VItem
 from janim.typing import Vect, VectArray
 from janim.utils.bezier import PathBuilder
 from janim.utils.iterables import adjacent_n_tuples
 from janim.utils.space_ops import (angle_between_vectors, compass_directions,
@@ -47,30 +46,29 @@
         if radius is None:
             radius = 0.25 * min_edge_length
         else:
             radius = min(radius, 0.5 * min_edge_length)
         vertices = self.get_vertices()
         arcs: list[ArcBetweenPoints] = []
 
-        with Timeline.CtxBlocker():
-            for v1, v2, v3 in adjacent_n_tuples(vertices, 3):
-                vect1 = normalize(v2 - v1)
-                vect2 = normalize(v3 - v2)
-                angle = angle_between_vectors(vect1, vect2)
-                # Distance between vertex and start of the arc
-                cut_off_length = radius * np.tan(angle / 2)
-                # Negative radius gives concave curves
-                sign = float(np.sign(radius * cross2d(vect1, vect2)))
-                arc = ArcBetweenPoints(
-                    v2 - vect1 * cut_off_length,
-                    v2 + vect2 * cut_off_length,
-                    angle=sign * angle,
-                    n_components=2,
-                )
-                arcs.append(arc)
+        for v1, v2, v3 in adjacent_n_tuples(vertices, 3):
+            vect1 = normalize(v2 - v1)
+            vect2 = normalize(v3 - v2)
+            angle = angle_between_vectors(vect1, vect2)
+            # Distance between vertex and start of the arc
+            cut_off_length = radius * np.tan(angle / 2)
+            # Negative radius gives concave curves
+            sign = float(np.sign(radius * cross2d(vect1, vect2)))
+            arc = ArcBetweenPoints(
+                v2 - vect1 * cut_off_length,
+                v2 + vect2 * cut_off_length,
+                angle=sign * angle,
+                n_components=2,
+            )
+            arcs.append(arc)
 
         builder = PathBuilder(start_point=arcs[-1].points.get_end())
         for arc in arcs:
             if not np.isclose(builder.end_point, arc.points.get_start()).all():
                 builder.line_to(arc.points.get_start())
             builder.append(arc.points.get()[1:])
         self.points.set(builder.get())
```

### Comparing `janim-0.5.2/janim/items/image_item.py` & `janim-1.0.0/janim/items/image_item.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,60 +46,63 @@
 
         img = get_img_from_file(file_path)
         self.image.set(img, min_mag_filter)
 
         if height is None:
             self.points.set_size(
                 img.width * Config.get.pixel_to_frame_ratio,
-                img.height * Config.get.pixel_to_frame_ratio)
+                img.height * Config.get.pixel_to_frame_ratio
+            )
         else:
             self.points.set_size(
                 height * img.width / img.height,
                 height
             )
 
     def get_orig(self) -> np.ndarray:
         '''图像的左上角'''
-        return self.points[0]
+        return self.points.get()[0]
 
     def get_horizontal_vect(self) -> np.ndarray:
         '''
         从图像的左上角指向右上角的向量
         '''
-        return self.points[2] - self.points[0]
+        points = self.points.get()
+        return points[2] - points[0]
 
     def get_horizontal_dist(self) -> float:
         '''
         :meth:`get_horizontal_vect` 的长度
         '''
         return get_norm(self.get_horizontal_vect())
 
     def get_vertical_vect(self) -> np.ndarray:
         '''
         从图像的左上角指向左下角的向量
         '''
-        return self.points[1] - self.points[0]
+        points = self.points.get()
+        return points[1] - points[0]
 
     def get_vertical_dist(self) -> float:
         '''
         :meth:`get_vertical_vect` 的长度
         '''
         return get_norm(self.get_vertical_vect())
 
     def pixel_to_rgba(self, x: int, y: int) -> np.ndarray:
         '''
         根据像素坐标得到颜色
         '''
         img = self.image.get()
         width, height = img.size
         return np.array(
-            img.getpixel(
+            img.getpixel((
                 clip(x, 0, width - 1),
                 clip(y, 0, height - 1)
-            )
+            ))
         ) / 255
 
     def point_to_rgba(self, point: np.ndarray, clamp_to_edge: bool = False) -> np.ndarray:
         '''
         通过空间坐标获得对应的像素颜色
         '''
         hor = self.get_horizontal_vect()
@@ -133,29 +136,27 @@
         hor = self.get_horizontal_vect()
         ver = self.get_vertical_vect()
         orig = self.get_orig()
         width, height = self.image.get().size
 
         return orig + hor * x / width + ver * y / height
 
-    class Data(Item.Data['ImageItem']):
-
-        @classmethod
-        def align_for_interpolate(
-            cls,
-            data1: ImageItem.Data,
-            data2: ImageItem.Data,
-        ) -> AlignedData[ImageItem.Data]:
-            aligned = super().align_for_interpolate(data1, data2)
-
-            for data in (aligned.data1, aligned.data2):
-                points_count = data.cmpt.points.count()
-                data.cmpt.color.resize(points_count)
+    @classmethod
+    def align_for_interpolate(
+        cls,
+        item1: ImageItem,
+        item2: ImageItem,
+    ) -> AlignedData[ImageItem]:
+        aligned = super().align_for_interpolate(item1, item2)
+
+        for data in (aligned.data1, aligned.data2):
+            points_count = data.points.count()
+            data.color.resize(points_count)
 
-            return aligned
+        return aligned
 
 
 class PixelImageItem(ImageItem):
     '''
     图像物件
 
     与 :class:`ImageItem` 基本一致，只是在图像被放大显示时不进行平滑插值处理，使得像素清晰
```

### Comparing `janim-0.5.2/janim/items/item.py` & `janim-1.0.0/janim/items/item.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 from janim.utils.data import AlignedData
 from janim.utils.iterables import resize_preserving_order
 from janim.utils.paths import PathFunc, straight_path
 
 if TYPE_CHECKING:
     from janim.items.points import Group
 
+type DynamicItem = Callable[[float], Item]
+
 CLS_CMPTINFO_NAME = '__cls_cmptinfo'
 CLS_STYLES_NAME = '__cls_styles'
 ALL_STYLES_NAME = '__all_styles'
 
 
 class _ItemMeta(type):
     '''
@@ -64,37 +66,52 @@
 
 class Item(Relation['Item'], metaclass=_ItemMeta):
     renderer_cls = Renderer
     '''
     覆盖该值以在子类中使用特定的渲染器
     '''
 
+    global_renderer: Renderer | None = None
+    '''
+    共用的渲染器，用于 ``is_temporary=True`` 的物件
+    '''
+
     depth = CmptInfo(Cmpt_Depth[Self], 0)
 
     def __init__(
         self,
         *args,
         depth: float | None = None,
-        children: list[Item] = [],
+        children: list[Item] | None = None,
         **kwargs
     ):
         super().__init__(*args)
 
+        self.stored: bool = False
+        self.stored_parents: list[Item] | None = None
+        self.stored_children: list[Item] | None = None
+
+        # 如果 is_temporary 为 True，则不会另外创建渲染器，而是使用共用的渲染器
+        self.is_temporary: bool = False
+
+        from janim.anims.timeline import Timeline
+        self.timeline = Timeline.get_context(raise_exc=False)
+
         self._init_components()
         if depth is not None:
             self.depth.set(depth)
 
         self._astype: type[Item] | None = None
         self._astype_mock_cmpt: dict[str, Component] = {}
 
-        self.add(*children)
+        self.renderer: Renderer | None = None
 
-        self.digest_styles(kwargs)
-
-        self.register_to_timeline(raise_exc=False)
+        if children is not None:
+            self.add(*children)
+        self.digest_styles(**kwargs)
 
     @dataclass
     class _CmptInitData:
         info: CmptInfo[CmptInfo]
         decl_cls: type[Item]
 
     def _init_components(self) -> None:
@@ -121,19 +138,17 @@
 
         for key, data in datas.items():
             obj = data.info.create()
             obj.init_bind(Component.BindInfo(data.decl_cls, self, key))
 
             self.__dict__[key] = self.components[key] = obj
 
-    def register_to_timeline(self, *, raise_exc=True) -> None:
-        from janim.anims.timeline import Timeline
-        timeline = Timeline.get_context(raise_exc=raise_exc)
-        if timeline:
-            timeline.register(self)
+    def set_component(self, key: str, cmpt: Component) -> None:
+        setattr(self, key, cmpt)
+        self.components[key] = cmpt
 
     def broadcast_refresh_of_component(
         self,
         cmpt: Component,
         func: Callable | str,
         *,
         recurse_up=False,
@@ -161,15 +176,18 @@
 
         if recurse_up:
             mark(self.ancestors())
 
         if recurse_down:
             mark(self.descendants())
 
-    def digest_styles(self, styles: dict[str, Any]):
+    def digest_styles(self, **styles):
+        '''
+        设置物件以及子物件的样式
+        '''
         flags = dict.fromkeys(styles.keys(), False)
         for item in self.walk_self_and_descendants():
             available_styles = item.get_available_styles()
             apply_styles = {
                 key: style
                 for key, style in styles.items()
                 if key in available_styles
@@ -182,15 +200,24 @@
             if not flag:
                 log.warning(f'传入参数 "{key}" 没有匹配任何的样式设置，且没有被任何地方使用')
 
     @classmethod
     def get_available_styles(cls) -> list[str]:
         return getattr(cls, ALL_STYLES_NAME)
 
-    def set_style(self, **kwargs) -> Self:
+    def set_style(
+        self,
+        depth: float | None = None,
+        **kwargs
+    ) -> Self:
+        '''
+        设置物件自身的样式，不影响子物件
+        '''
+        if depth is not None:
+            self.depth.set(depth)
         return self
 
     def do(self, func: Callable[[Self], Any]) -> Self:
         '''
         使用 ``func`` 对物件进行操作，并返回 ``self`` 以方便链式调用
         '''
         func(self)
@@ -253,15 +280,15 @@
         '''
         复制 n 个自身，并作为一个 :class:`Group` 返回
 
         可以将 ``item * n`` 作为该方法的简写
         '''
         from janim.items.points import Group
         return Group(
-            *(self.copy() for _ in range(n))
+            *(self.copy() for i in range(n))
         )
 
     # region astype
 
     def astype[T](self, cls: type[T]) -> T:
         '''
         使得可以调用当前物件中没有的组件
@@ -331,221 +358,89 @@
         self._astype_mock_cmpt[name] = cmpt
         return cmpt
 
     # endregion
 
     # region data
 
-    class Data[ItemT: 'Item']:
-        def __init__(
-            self,
-            item: ItemT,
-            components: dict[str, Component],
-            parents: list[Item],
-            children: list[Item],
-        ):
-            self.item = item
-            self.components = components
-            self.parents = parents
-            self.children = children
-
-            self.renderer = None
-
-        @classmethod
-        def _store[U: 'Item'](cls, item: U) -> Self[U]:
-            return cls._copy(cls._ref(item))
-
-        @classmethod
-        def _ref[U: 'Item'](cls, item: U) -> Self[U]:
-            return cls(
-                item,
-                item.components,
-                item.parents,
-                item.children
-            )
-
-        @classmethod
-        def _copy[U: 'Item'](cls, data: Self[U]) -> Self[U]:
-            components: dict[str, Component] = {}
-
-            for key, cmpt in data.components.items():
-                if isinstance(cmpt, _CmptGroup):
-                    # 因为现在的 Python 版本中，dict 取键值保留原序
-                    # 所以 new_cmpts 肯定有 _CmptGroup 所需要的
-                    components[key] = cmpt.copy(new_cmpts=components)
-                else:
-                    components[key] = cmpt.copy()
-
-            parents = data.parents.copy()
-            children = data.children.copy()
-
-            return cls(data.item, components, parents, children)
-
-        def _restore(self, data: Item.Data) -> None:
-            for key in self.components.keys() | data.components.keys():
-                self.components[key].become(data.components[key])
-
-            self.parents.clear()
-            self.parents.extend(data.parents)
-
-            self.children.clear()
-            self.children.extend(data.children)
-
-        def is_changed(self) -> bool:
-            '''
-            检查该数据与 ``item`` 现在的数据是否产生差异
-
-            注：仅检查自身数据，不检查子物件的数据
-            '''
-            for stored_cmpt, item_cmpt in zip(self.components.values(), self.item.components.values()):
-                if stored_cmpt != item_cmpt:
-                    return True
-
-            return self.parents != self.item.parents or self.children != self.item.children
-
-        class _CmptGetter:
-            def __init__(self, data: Item.Data):
-                self._data = data
-
-            def __getattr__(self, name: str):
-                cmpt = self._data.components.get(name, None)
-                if cmpt is None:
-                    raise AttributeError(f"'{self._data.item.__class__.__name__}' 没有叫作 '{name}' 的组件")
-
-                return cmpt
-
-        @property
-        def cmpt(self) -> ItemT:
-            '''
-            将 ``.component['key']`` 简化为 ``.cmpt.key`` 且方便代码提示
-            '''
-            return Item.Data._CmptGetter(self)
-
-        @classmethod
-        def align_for_interpolate(
-            cls,
-            data1: Item.Data,
-            data2: Item.Data,
-        ) -> AlignedData[Self]:
-            aligned = AlignedData(*[
-                cls(data1.item, {}, [], [])
-                for _ in range(3)
-            ])
-
-            # align components
-            for key, cmpt1 in data1.components.items():
-                cmpt2 = data2.components.get(key, None)
-
-                if isinstance(cmpt1, _CmptGroup) and isinstance(cmpt2, _CmptGroup):
-                    cmpt_aligned = cmpt1.align(cmpt1, cmpt2, aligned)
-
-                elif cmpt2 is None or not isinstance(cmpt1, SupportsInterpolate):
-                    cmpt_aligned = AlignedData(cmpt1, cmpt1, cmpt1)
-                else:
-                    cmpt_aligned = cmpt1.align_for_interpolate(cmpt1, cmpt2)
-
-                aligned.data1.components[key] = cmpt_aligned.data1
-                aligned.data2.components[key] = cmpt_aligned.data2
-                aligned.union.components[key] = cmpt_aligned.union
+    def get_parents(self):
+        return self.stored_parents if self.stored else self.parents
 
-            # align children
-            max_len = max(len(data1.children), len(data2.children))
-            aligned.data1.children = resize_preserving_order(data1.children, max_len)
-            aligned.data2.children = resize_preserving_order(data2.children, max_len)
+    def get_children(self):
+        return self.stored_children if self.stored else self.children
 
-            return aligned
-
-        def interpolate(
-            self,
-            data1: Item.Data,
-            data2: Item.Data,
-            alpha: float,
-            *,
-            path_func: PathFunc = straight_path,
-        ) -> None:
-            for key, cmpt in self.components.items():
-                cmpt1 = data1.components[key]
-                cmpt2 = data2.components[key]
-
-                if not isinstance(cmpt, SupportsInterpolate):
-                    continue
-
-                cmpt.interpolate(cmpt1, cmpt2, alpha, path_func=path_func)
-
-        def apart_alpha(self, n: int) -> None:
-            for cmpt in self.components.values():
-                if isinstance(cmpt, SupportsApartAlpha):
-                    cmpt.apart_alpha(n)
-
-        def create_renderer(self) -> None:
-            self.renderer = self.item.renderer_cls()
-
-        def render(self) -> None:
-            if self.renderer is None:
-                self.create_renderer()
-
-            if not self.renderer.initialized:
-                self.renderer.init()
-                self.renderer.initialized = True
-            self.renderer.render(self)
-
-    def store_data(self):
-        '''
-        将数据复制，返回复制后的数据
-
-        注：仅复制自身数据，不复制子物件的数据
-        '''
-        return self.Data._store(self)
-
-    def ref_data(self):
-        '''
-        返回数据的引用，不进行复制
-        '''
-        return self.Data._ref(self)
+    def not_changed(self, other: Self) -> bool:
+        if self.get_children() != other.get_children():
+            return False
+        for key, cmpt in self.components.items():
+            if not cmpt.not_changed(other.components[key]):
+                return False
+        return True
 
-    def restore_data(self, data: Data[Self]) -> Self:
-        self.ref_data()._restore(data)
-        return self
+    def current(self, *, as_time: float | None = None, skip_dynamic=False) -> Self:
+        return self.timeline.item_current(self, as_time=as_time, skip_dynamic=skip_dynamic)
 
-    def copy(self) -> Self:
+    def copy(self, *, root_only=False) -> Self:
         '''
         复制物件
         '''
         copy_item = copy.copy(self)
 
         copy_item.reset_refresh()
 
         copy_item.parents = []
-        copy_item.parents_changed()
-
         copy_item.children = []
-        copy_item.add(*[item.copy() for item in self.children])
+        if root_only:
+            copy_item.stored = True
+            copy_item.stored_parents = self.get_parents().copy()
+            copy_item.stored_children = self.get_children().copy()
+        else:
+            copy_item.add(*[item.copy() for item in self.children])
+            copy_item.parents_changed()
 
         new_cmpts = {}
         for key, cmpt in self.components.items():
             if isinstance(cmpt, _CmptGroup):
                 # 因为现在的 Python 版本中，dict 取键值保留原序
                 # 所以 new_cmpts 肯定有 _CmptGroup 所需要的
                 cmpt_copy = cmpt.copy(new_cmpts=new_cmpts)
             else:
                 cmpt_copy = cmpt.copy()
 
-            cmpt_copy.init_bind(Component.BindInfo(cmpt.bind.decl_cls,
-                                                   copy_item,
-                                                   key))
+            if cmpt.bind is not None:
+                cmpt_copy.init_bind(Component.BindInfo(cmpt.bind.decl_cls,
+                                                       copy_item,
+                                                       key))
 
             new_cmpts[key] = cmpt_copy
             setattr(copy_item, key, cmpt_copy)
 
         copy_item.components = new_cmpts
         copy_item._astype_mock_cmpt = {}
 
-        copy_item.register_to_timeline(raise_exc=False)
         return copy_item
 
+    # TODO: optimize
+    def _current_family(self, *, up: bool) -> list[Item]:   # use DFS
+        lst = self.stored_parents if up else self.stored_children
+        res = []
+
+        for sub_obj in lst:
+            current = sub_obj.current()
+            if current not in res:
+                res.append(current)
+            res.extend(filter(
+                lambda obj: obj not in res,
+                current._current_family(up=up)
+                if current.stored
+                else (current.ancestors() if up else current.descendants())
+            ))
+
+        return res
+
     def become(self, other: Item) -> Self:
         '''
         将该物件的数据设置为与传入的物件相同（以复制的方式，不是引用）
         '''
         # self.parents 不变
 
         children = self.children.copy()
@@ -564,28 +459,122 @@
         from janim.anims.timeline import Timeline
         timeline = Timeline.get_context(raise_exc=False)
         if timeline is not None and timeline.is_displaying(self):
             timeline.show(self)
 
         return self
 
+    def store(self) -> Self:
+        return self.copy(root_only=True)
+
+    def restore(self, other: Item) -> Self:
+        self.parents = other.parents.copy()
+        self.parents_changed()
+        self.children = other.children.copy()
+        self.children_changed()
+
+        for key in self.components.keys() & other.components.keys():
+            self.components[key].become(other.components[key])
+
+        return self
+
+    @classmethod
+    def align_for_interpolate(
+        cls,
+        item1: Item,
+        item2: Item
+    ) -> AlignedData[Self]:
+        '''
+        进行数据对齐，以便插值
+        '''
+        aligned = AlignedData(item1.store(),
+                              item1.store(),
+                              item2.store())
+
+        # align components
+        for key, cmpt1 in item1.components.items():
+            cmpt2 = item2.components.get(key, None)
+
+            if isinstance(cmpt1, _CmptGroup) and isinstance(cmpt2, _CmptGroup):
+                cmpt_aligned = cmpt1.align(cmpt1, cmpt2, aligned)
+
+            elif cmpt2 is None or not isinstance(cmpt1, SupportsInterpolate):
+                cmpt_aligned = AlignedData(cmpt1, cmpt1, cmpt1)
+            else:
+                cmpt_aligned = cmpt1.align_for_interpolate(cmpt1, cmpt2)
+
+            aligned.data1.set_component(key, cmpt_aligned.data1)
+            aligned.data2.set_component(key, cmpt_aligned.data2)
+            aligned.union.set_component(key, cmpt_aligned.union)
+
+        # align children
+        max_len = max(len(item1.get_children()), len(item2.get_children()))
+        aligned.data1.stored_children = resize_preserving_order(item1.get_children(), max_len)
+        aligned.data2.stored_children = resize_preserving_order(item2.get_children(), max_len)
+
+        return aligned
+
+    def interpolate(
+        self,
+        item1: Item,
+        item2: Item,
+        alpha: float,
+        *,
+        path_func: PathFunc = straight_path,
+    ) -> None:
+        '''
+        进行插值（仅对该物件进行，不包含后代物件）
+        '''
+        for key, cmpt in self.components.items():
+            cmpt1 = item1.components[key]
+            cmpt2 = item2.components[key]
+
+            if not isinstance(cmpt, SupportsInterpolate):
+                continue
+
+            cmpt.interpolate(cmpt1, cmpt2, alpha, path_func=path_func)
+
+    def apart_alpha(self, n: int) -> None:
+        for cmpt in self.components.values():
+            if isinstance(cmpt, SupportsApartAlpha):
+                cmpt.apart_alpha(n)
+
+    @classmethod
+    def get_global_renderer(cls) -> None:
+        if cls.global_renderer is None:
+            cls.global_renderer = cls.renderer_cls()
+        return cls.global_renderer
+
+    def create_renderer(self) -> None:
+        if self.is_temporary:
+            self.renderer = self.get_global_renderer()
+        else:
+            self.renderer = self.renderer_cls()
+
+    def render(self) -> None:
+        if self.renderer is None:
+            self.create_renderer()
+
+        if not self.renderer.initialized:
+            self.renderer.init()
+            self.renderer.initialized = True
+        self.renderer.render(self)
+
     # endregion
 
     # region timeline
 
     def show(self, **kwargs) -> Self:
         '''
         显示物件
         '''
-        from janim.anims.timeline import Timeline
-        Timeline.get_context().show(self, **kwargs)
+        self.timeline.show(self, **kwargs)
         return self
 
     def hide(self, **kwargs) -> Self:
         '''
         隐藏物件
         '''
-        from janim.anims.timeline import Timeline
-        Timeline.get_context().hide(self, **kwargs)
+        self.timeline.hide(self, **kwargs)
         return self
 
     # endregion
```

### Comparing `janim-0.5.2/janim/items/points.py` & `janim-1.0.0/janim/items/points.py`

 * *Files 8% similar despite different names*

```diff
@@ -74,40 +74,39 @@
     def set_style(
         self,
         color: JAnimColor | ColorArray | None = None,
         alpha: float | Iterable[float] | None = None,
         radius: float | Iterable[float] | None = None,
         **kwargs
     ) -> Self:
-        self.color.set(color, alpha)
+        self.color.set(color, alpha, root_only=True)
         if radius is not None:
-            self.radius.set(radius)
+            self.radius.set(radius, root_only=True)
 
         return super().set_style(**kwargs)
 
-    class Data(Item.Data['DotCloud']):
-        @classmethod
-        def align_for_interpolate(
-            cls,
-            data1: DotCloud.Data,
-            data2: DotCloud.Data,
-        ) -> AlignedData[DotCloud.Data]:
-            len1 = len(data1.cmpt.points.get())
-            len2 = len(data2.cmpt.points.get())
-
-            aligned = super().align_for_interpolate(data1, data2)
-
-            for data in (aligned.data1, aligned.data2):
-                points_count = data.cmpt.points.count()
-                data.cmpt.color.resize(points_count)
-                data.cmpt.radius.resize(points_count)
-
-            if len1 != len2:
-                indice_groups = resize_preserving_order_indice_groups(min(len1, len2), max(len1, len2))
-
-                cmpt_to_fade = aligned.data1.cmpt.color if len1 < len2 else aligned.data2.cmpt.color
-                rgbas = cmpt_to_fade.get()
-                for group in indice_groups:
-                    rgbas[group, 3] = apart_alpha(rgbas[group[0], 3], len(group))
-                cmpt_to_fade.set_rgbas(rgbas)
+    @classmethod
+    def align_for_interpolate(
+        cls,
+        item1: DotCloud,
+        item2: DotCloud,
+    ) -> AlignedData[DotCloud]:
+        len1 = len(item1.points.get())
+        len2 = len(item2.points.get())
+
+        aligned = super().align_for_interpolate(item1, item2)
+
+        for data in (aligned.data1, aligned.data2):
+            points_count = data.points.count()
+            data.color.resize(points_count)
+            data.radius.resize(points_count)
+
+        if len1 != len2:
+            indice_groups = resize_preserving_order_indice_groups(min(len1, len2), max(len1, len2))
+
+            cmpt_to_fade = aligned.data1.color if len1 < len2 else aligned.data2.color
+            rgbas = cmpt_to_fade.get().copy()
+            for group in indice_groups:
+                rgbas[group, 3] = apart_alpha(rgbas[group[0], 3], len(group))
+            cmpt_to_fade.set_rgbas(rgbas)
 
-            return aligned
+        return aligned
```

### Comparing `janim-0.5.2/janim/items/relation.py` & `janim-1.0.0/janim/items/relation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import random
 from typing import Callable, Generator, Self
 
 import janim.utils.refresh as refresh
 from janim.utils.signal import Signal
 
 
 class Relation[GRelT: 'Relation'](refresh.Refreshable):
@@ -27,15 +28,15 @@
 
         self.parents: list[GRelT] = []
         self.children: list[GRelT] = []
 
     def mark_refresh(self, func: Callable | str, *, recurse_up=False, recurse_down=False) -> Self:
         super().mark_refresh(func)
 
-        name = func.__name__ if isinstance(func, Callable) else func
+        name = func.__name__ if callable(func) else func
 
         if recurse_up:
             for obj in self.ancestors():
                 if hasattr(obj, name):
                     obj.mark_refresh(name)
 
         if recurse_down:
@@ -94,29 +95,35 @@
                 obj.parents.remove(self)
             except ValueError: ...
             obj.parents_changed()
 
         self.children_changed()
         return self
 
+    def shuffle(self) -> Self:
+        random.shuffle(self.children)
+        self.children_changed()
+        return self
+
     def clear_parents(self) -> Self:
         for parent in self.parents:
             parent.remove(self)
         return self
 
     def clear_children(self) -> Self:
         self.remove(*self.children)
         return self
 
     def _family(self, *, up: bool) -> list[GRelT]:  # use DFS
         lst = self.parents if up else self.children
         res = []
 
         for sub_obj in lst:
-            res.append(sub_obj)
+            if sub_obj not in res:
+                res.append(sub_obj)
             res.extend(filter(
                 lambda obj: obj not in res,
                 sub_obj._family(up=up)
             ))
 
         return res
 
@@ -135,15 +142,16 @@
         获得后代对象列表
         '''
         return self._family(up=False)
 
     @staticmethod
     def _walk_lst[RelT](base_cls: type[RelT] | None, lst: list[GRelT]) -> Generator[RelT, None, None]:
         if base_cls is None:
-            base_cls = Relation
+            yield from lst
+            return
 
         for obj in lst:
             if isinstance(obj, base_cls):
                 yield obj
 
     def _walk_nearest_family[RelT](
         self: Relation,
@@ -173,27 +181,29 @@
 
     def walk_descendants[RelT](self, base_cls: type[RelT] = None) -> Generator[RelT, None, None]:
         '''
         遍历后代节点中以 ``base_cls`` （缺省则遍历全部）为基类的对象
         '''
         yield from self._walk_lst(base_cls, self.descendants())
 
-    def walk_self_and_ancestors(self) -> Generator[GRelT, None, None]:
+    def walk_self_and_ancestors(self, root_only=False) -> Generator[GRelT, None, None]:
         '''
         遍历自己以及祖先节点
         '''
         yield self
-        yield from self.ancestors()
+        if not root_only:
+            yield from self.ancestors()
 
-    def walk_self_and_descendants(self) -> Generator[GRelT, None, None]:
+    def walk_self_and_descendants(self, root_only=False) -> Generator[GRelT, None, None]:
         '''
         遍历自己以及后代节点
         '''
         yield self
-        yield from self.descendants()
+        if not root_only:
+            yield from self.descendants()
 
     def walk_nearest_ancestors[RelT](self, base_cls: type[RelT]) -> Generator[RelT, None, None]:
         '''
         遍历祖先节点中以 ``base_cls`` 为基类的对象，但是排除已经满足条件的对象的祖先对象
         '''
         yield from self._walk_nearest_family(base_cls, lambda rel: rel.ancestors())
```

### Comparing `janim-0.5.2/janim/items/svg/brace.py` & `janim-1.0.0/janim/items/svg/brace.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 
 import math
 import os
 from typing import Self
 
 import numpy as np
 
-from janim.anims.timeline import Timeline
 from janim.components.component import CmptInfo
 from janim.components.vpoints import Cmpt_VPoints
 from janim.constants import DEFAULT_ITEM_TO_ITEM_BUFF, DOWN, PI, SMALL_BUFF
-from janim.items.item import Item
 from janim.items.points import Points
 from janim.items.svg.svg_item import SVGItem
 from janim.items.svg.typst import Typst
 from janim.items.text.text import Text
 from janim.items.vitem import VItem
 from janim.typing import Vect
 from janim.utils.file_ops import get_janim_dir
@@ -23,83 +21,81 @@
 class Cmpt_VPoints_BraceImpl[ItemT](Cmpt_VPoints[ItemT], impl=True):
     '''
     在 :class:`Brace` 中对 :class:`Cmpt_VPoints` 的进一步实现
     '''
     # 复制时，``brace_length`` 随 ``copy.copy(self)`` 而复制，因此不用重写 ``copy`` 方法
     def match(
         self,
-        item_or_data: Points | Item.Data[Points] | None,
+        item: Points | None,
         direction: Vect | None = None,
-        buff: float = SMALL_BUFF
+        buff: float = SMALL_BUFF,
+        root_only: bool = False
     ) -> Self:
         '''
-        将花括号进行伸缩，使得与 ``item_or_data`` 在 ``direction`` 方向的宽度匹配
+        将花括号进行伸缩，使得与 ``item`` 在 ``direction`` 方向的宽度匹配
         '''
         if direction is None:
             direction = self.direction if self.has() else DOWN
 
         self.set(get_brace_orig_points())
 
         angle = math.atan2(direction[1], direction[0]) + PI / 2
         rot = np.array(rotation_about_z(-angle))
 
-        if item_or_data is None:
+        if item is None:
             self.brace_length = self.box.width
         else:
-            if isinstance(item_or_data, Points):
-                cmpt = item_or_data.points
-            else:
-                cmpt = item_or_data.cmpt.points
+            cmpt = item.points
 
-            rot_points = np.dot(cmpt.get(), rot.T)   # dot(points, rot.T) == dot(rot, points.T).T
+            rot_points = np.dot(
+                cmpt.get() if root_only else cmpt.get_all(),
+                rot.T
+            )   # dot(points, rot.T) == dot(rot, points.T).T
 
             box = self.BoundingBox(rot_points)
             self.brace_length = box.width
 
             self.set_width(box.width, stretch=box.width > self.box.width)
             self.move_to(box.bottom + DOWN * (buff + self.box.height / 2))
 
         self.apply_matrix(rot.T)     # rot.T == rot.I
 
         return self
 
     @property
     def tip_point(self) -> np.ndarray:
         '''得到花括号中间凸出处的坐标'''
-        return self._points._data[get_brace_tip_point_index()].copy()
+        return self._points.data[get_brace_tip_point_index()]
 
     @property
     def brace_left(self) -> np.ndarray:
         '''得到括号指向方向左边的尖端处的坐标'''
-        return self._points._data[get_brace_left_index()].copy()
+        return self._points.data[get_brace_left_index()]
 
     @property
     def brace_right(self) -> np.ndarray:
         '''得到括号指向方向右边的尖端处的坐标'''
-        return self._points._data[get_brace_right_index()].copy()
+        return self._points.data[get_brace_right_index()]
 
     @property
     def direction(self) -> np.ndarray:
         '''得到括号指向的方向'''
         return normalize(self.tip_point - self.box.center)
 
     def put_at_tip(
         self,
-        item_or_data: Points | Item.Data[Points],
+        item: Points,
         use_next_to: bool = True,
         buff: float = DEFAULT_ITEM_TO_ITEM_BUFF,
         **kwargs
     ) -> Self:
         '''
         将物件放置在花括号中间的凸出处
         '''
-        if isinstance(item_or_data, Points):
-            cmpt = item_or_data.points
-        else:
-            cmpt = item_or_data.cmpt.points
+        cmpt = item.points
 
         if use_next_to:
             cmpt.next_to(
                 self.tip_point,
                 np.round(self.direction),
                 buff=buff,
                 **kwargs
@@ -150,20 +146,19 @@
 
 
 def get_brace_orig_points() -> np.ndarray:
     global brace_orig_points
     if brace_orig_points is not None:
         return brace_orig_points
 
-    with Timeline.CtxBlocker():
-        svg = SVGItem(os.path.join(get_janim_dir(), 'items', 'svg', 'brace.svg'))
+    svg = SVGItem(os.path.join(get_janim_dir(), 'items', 'svg', 'brace.svg'))
     points = svg[0].points.get()
-    points -= (points.min(axis=0) + points.max(axis=0)) * 0.5
-    brace_orig_points = points
+    center = (points.min(axis=0) + points.max(axis=0)) * 0.5
 
+    brace_orig_points = points - center
     return brace_orig_points
 
 
 def get_brace_tip_point_index() -> int:
     global brace_tip_point_index
     if brace_tip_point_index is not None:
         return brace_tip_point_index
```

### Comparing `janim-0.5.2/janim/items/svg/brace.svg` & `janim-1.0.0/janim/items/svg/brace.svg`

 * *Files identical despite different names*

### Comparing `janim-0.5.2/janim/items/svg/svg_item.py` & `janim-1.0.0/janim/items/svg/svg_item.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,240 +16,259 @@
 000000f0: 7465 6d0d 0a66 726f 6d20 6a61 6e69 6d2e  tem..from janim.
 00000100: 6c6f 6767 6572 2069 6d70 6f72 7420 6c6f  logger import lo
 00000110: 670d 0a66 726f 6d20 6a61 6e69 6d2e 7574  g..from janim.ut
 00000120: 696c 732e 6265 7a69 6572 2069 6d70 6f72  ils.bezier impor
 00000130: 7420 5061 7468 4275 696c 6465 720d 0a66  t PathBuilder..f
 00000140: 726f 6d20 6a61 6e69 6d2e 7574 696c 732e  rom janim.utils.
 00000150: 636f 6e66 6967 2069 6d70 6f72 7420 436f  config import Co
-00000160: 6e66 6967 0d0a 0d0a 2320 e8bf 99e9 878c  nfig....# ......
-00000170: e79a 8420 332e 3237 3220 e698 afe6 898b  ... 3.272 ......
-00000180: e58a a8e8 af95 e587 bae6 9da5 e79a 840d  ................
-00000190: 0a44 4546 4155 4c54 5f53 5647 4954 454d  .DEFAULT_SVGITEM
-000001a0: 5f53 4341 4c45 5f46 4143 544f 5220 3d20  _SCALE_FACTOR = 
-000001b0: 332e 3237 320d 0a53 5452 4f4b 455f 5749  3.272..STROKE_WI
-000001c0: 4454 485f 434f 4e56 4552 5349 4f4e 203d  DTH_CONVERSION =
-000001d0: 2030 2e30 310d 0a0d 0a74 7970 6520 5649   0.01....type VI
-000001e0: 7465 6d42 7569 6c64 6572 203d 2043 616c  temBuilder = Cal
-000001f0: 6c61 626c 655b 5b5d 2c20 5649 7465 6d5d  lable[[], VItem]
-00000200: 0d0a 0d0a 0d0a 6465 6620 5f63 6f6e 7665  ......def _conve
-00000210: 7274 5f70 6f69 6e74 5f74 6f5f 3364 2878  rt_point_to_3d(x
-00000220: 3a20 666c 6f61 742c 2079 3a20 666c 6f61  : float, y: floa
-00000230: 7429 202d 3e20 6e70 2e6e 6461 7272 6179  t) -> np.ndarray
-00000240: 3a0d 0a20 2020 2072 6574 7572 6e20 6e70  :..    return np
-00000250: 2e61 7272 6179 285b 782c 2079 2c20 305d  .array([x, y, 0]
-00000260: 290d 0a0d 0a0d 0a64 6566 205f 636f 6e76  )......def _conv
-00000270: 6572 745f 616c 7068 615f 746f 5f66 6c6f  ert_alpha_to_flo
-00000280: 6174 2878 3a20 696e 7420 7c20 4e6f 6e65  at(x: int | None
-00000290: 2920 2d3e 2066 6c6f 6174 3a0d 0a20 2020  ) -> float:..   
-000002a0: 2072 6574 7572 6e20 4e6f 6e65 2069 6620   return None if 
-000002b0: 7820 6973 204e 6f6e 6520 656c 7365 2078  x is None else x
-000002c0: 202f 2032 3535 0d0a 0d0a 0d0a 636c 6173   / 255......clas
-000002d0: 7320 5356 4749 7465 6d28 4772 6f75 705b  s SVGItem(Group[
-000002e0: 5649 7465 6d5d 293a 0d0a 2020 2020 2727  VItem]):..    ''
-000002f0: 270d 0a20 2020 20e4 bca0 e585 a520 5356  '..    ...... SV
-00000300: 4720 e696 87e4 bbb6 e8b7 afe5 be84 efbc  G ..............
-00000310: 8ce8 a7a3 e69e 90e4 b8ba e789 a9e4 bbb6  ................
-00000320: 0d0a 2020 2020 2727 270d 0a20 2020 2073  ..    '''..    s
-00000330: 7667 5f70 6172 745f 6465 6661 756c 745f  vg_part_default_
-00000340: 6b77 6172 6773 203d 2064 6963 7428 0d0a  kwargs = dict(..
-00000350: 2020 2020 2020 2020 7374 726f 6b65 5f72          stroke_r
-00000360: 6164 6975 733d 312e 3020 2a20 5354 524f  adius=1.0 * STRO
-00000370: 4b45 5f57 4944 5448 5f43 4f4e 5645 5253  KE_WIDTH_CONVERS
-00000380: 494f 4e20 2f20 322c 0d0a 2020 2020 2020  ION / 2,..      
-00000390: 2020 7374 726f 6b65 5f63 6f6c 6f72 3d4e    stroke_color=N
-000003a0: 6f6e 652c 0d0a 2020 2020 2020 2020 7374  one,..        st
-000003b0: 726f 6b65 5f61 6c70 6861 3d30 2c0d 0a20  roke_alpha=0,.. 
-000003c0: 2020 2020 2020 2066 696c 6c5f 636f 6c6f         fill_colo
-000003d0: 723d 4e6f 6e65 2c0d 0a20 2020 2020 2020  r=None,..       
-000003e0: 2066 696c 6c5f 616c 7068 613d 300d 0a20   fill_alpha=0.. 
-000003f0: 2020 2029 0d0a 2020 2020 7669 7465 6d5f     )..    vitem_
-00000400: 6275 696c 6465 7273 5f6d 6170 3a20 6469  builders_map: di
-00000410: 6374 5b74 7570 6c65 2c20 6c69 7374 5b56  ct[tuple, list[V
-00000420: 4974 656d 4275 696c 6465 725d 5d20 3d20  ItemBuilder]] = 
-00000430: 7b7d 0d0a 0d0a 2020 2020 6465 6620 5f5f  {}....    def __
-00000440: 696e 6974 5f5f 2873 656c 662c 2066 696c  init__(self, fil
-00000450: 655f 7061 7468 3a20 7374 722c 202a 2a6b  e_path: str, **k
-00000460: 7761 7267 7329 3a0d 0a20 2020 2020 2020  wargs):..       
-00000470: 2069 7465 6d73 203d 2073 656c 662e 6765   items = self.ge
-00000480: 745f 6974 656d 735f 6672 6f6d 5f66 696c  t_items_from_fil
-00000490: 6528 6669 6c65 5f70 6174 6829 0d0a 0d0a  e(file_path)....
-000004a0: 2020 2020 2020 2020 7375 7065 7228 292e          super().
-000004b0: 5f5f 696e 6974 5f5f 282a 6974 656d 732c  __init__(*items,
-000004c0: 202a 2a6b 7761 7267 7329 0d0a 0d0a 2020   **kwargs)....  
-000004d0: 2020 2020 2020 7365 6c66 2856 4974 656d        self(VItem
-000004e0: 292e 706f 696e 7473 2e73 6361 6c65 280d  ).points.scale(.
-000004f0: 0a20 2020 2020 2020 2020 2020 2043 6f6e  .            Con
-00000500: 6669 672e 6765 742e 7069 7865 6c5f 746f  fig.get.pixel_to
-00000510: 5f66 7261 6d65 5f72 6174 696f 202a 2044  _frame_ratio * D
-00000520: 4546 4155 4c54 5f53 5647 4954 454d 5f53  EFAULT_SVGITEM_S
-00000530: 4341 4c45 5f46 4143 544f 522c 0d0a 2020  CALE_FACTOR,..  
-00000540: 2020 2020 2020 2020 2020 6162 6f75 745f            about_
-00000550: 706f 696e 743d 4f52 4947 494e 0d0a 2020  point=ORIGIN..  
-00000560: 2020 2020 2020 292e 666c 6970 2852 4947        ).flip(RIG
-00000570: 4854 290d 0a0d 0a20 2020 2020 2020 2073  HT)....        s
-00000580: 656c 662e 6d6f 7665 5f69 6e74 6f5f 706f  elf.move_into_po
-00000590: 7369 7469 6f6e 2829 0d0a 0d0a 2020 2020  sition()....    
-000005a0: 6465 6620 6d6f 7665 5f69 6e74 6f5f 706f  def move_into_po
-000005b0: 7369 7469 6f6e 2873 656c 6629 202d 3e20  sition(self) -> 
-000005c0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2070  None:..        p
-000005d0: 6173 730d 0a0d 0a20 2020 2040 7374 6174  ass....    @stat
-000005e0: 6963 6d65 7468 6f64 0d0a 2020 2020 6465  icmethod..    de
-000005f0: 6620 6765 745f 6974 656d 735f 6672 6f6d  f get_items_from
-00000600: 5f66 696c 6528 6669 6c65 5f70 6174 683a  _file(file_path:
-00000610: 2073 7472 2920 2d3e 206c 6973 745b 4974   str) -> list[It
-00000620: 656d 5d3a 0d0a 2020 2020 2020 2020 2727  em]:..        ''
-00000630: 270d 0a20 2020 2020 2020 20e8 a7a3 e69e  '..        .....
-00000640: 90e6 9687 e4bb b6e5 b9b6 e5be 97e5 88b0  ................
-00000650: e789 a9e4 bbb6 e588 97e8 a1a8 0d0a 2020  ..............  
-00000660: 2020 2020 2020 2727 270d 0a20 2020 2020        '''..     
-00000670: 2020 206d 7469 6d65 203d 206f 732e 7061     mtime = os.pa
-00000680: 7468 2e67 6574 6d74 696d 6528 6669 6c65  th.getmtime(file
-00000690: 5f70 6174 6829 0d0a 2020 2020 2020 2020  _path)..        
-000006a0: 6e61 6d65 203d 206f 732e 7061 7468 2e73  name = os.path.s
-000006b0: 706c 6974 6578 7428 6f73 2e70 6174 682e  plitext(os.path.
-000006c0: 6261 7365 6e61 6d65 2866 696c 655f 7061  basename(file_pa
-000006d0: 7468 2929 5b30 5d0d 0a20 2020 2020 2020  th))[0]..       
-000006e0: 206b 6579 203d 2028 6e61 6d65 2c20 6d74   key = (name, mt
-000006f0: 696d 6529 0d0a 0d0a 2020 2020 2020 2020  ime)....        
-00000700: 6361 6368 6564 203d 2053 5647 4974 656d  cached = SVGItem
-00000710: 2e76 6974 656d 5f62 7569 6c64 6572 735f  .vitem_builders_
-00000720: 6d61 702e 6765 7428 6b65 792c 204e 6f6e  map.get(key, Non
-00000730: 6529 0d0a 2020 2020 2020 2020 6966 2063  e)..        if c
-00000740: 6163 6865 6420 6973 206e 6f74 204e 6f6e  ached is not Non
-00000750: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00000760: 7265 7475 726e 205b 6275 696c 6465 7228  return [builder(
-00000770: 2920 666f 7220 6275 696c 6465 7220 696e  ) for builder in
-00000780: 2063 6163 6865 645d 0d0a 0d0a 2020 2020   cached]....    
-00000790: 2020 2020 7376 673a 2073 652e 5356 4720      svg: se.SVG 
-000007a0: 3d20 7365 2e53 5647 2e70 6172 7365 2866  = se.SVG.parse(f
-000007b0: 696c 655f 7061 7468 290d 0a0d 0a20 2020  ile_path)....   
-000007c0: 2020 2020 206f 6666 7365 7420 3d20 6e70       offset = np
-000007d0: 2e61 7272 6179 285b 7376 672e 7769 6474  .array([svg.widt
-000007e0: 6820 2f20 2d32 2c20 7376 672e 6865 6967  h / -2, svg.heig
-000007f0: 6874 202f 202d 325d 290d 0a0d 0a20 2020  ht / -2])....   
-00000800: 2020 2020 2062 7569 6c64 6572 733a 206c       builders: l
-00000810: 6973 745b 5649 7465 6d42 7569 6c64 6572  ist[VItemBuilder
-00000820: 5d20 3d20 5b5d 0d0a 2020 2020 2020 2020  ] = []..        
-00000830: 666f 7220 7368 6170 6520 696e 2073 7667  for shape in svg
-00000840: 2e65 6c65 6d65 6e74 7328 293a 0d0a 2020  .elements():..  
-00000850: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
-00000860: 6e73 7461 6e63 6528 7368 6170 652c 2028  nstance(shape, (
-00000870: 7365 2e47 726f 7570 2c20 7365 2e55 7365  se.Group, se.Use
-00000880: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
-00000890: 2020 2020 2063 6f6e 7469 6e75 650d 0a20       continue.. 
-000008a0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-000008b0: 6973 696e 7374 616e 6365 2873 6861 7065  isinstance(shape
-000008c0: 2c20 7365 2e50 6174 6829 3a0d 0a20 2020  , se.Path):..   
-000008d0: 2020 2020 2020 2020 2020 2020 2062 7569               bui
-000008e0: 6c64 6572 732e 6170 7065 6e64 2853 5647  lders.append(SVG
-000008f0: 4974 656d 2e63 6f6e 7665 7274 5f70 6174  Item.convert_pat
-00000900: 6828 7368 6170 652c 206f 6666 7365 7429  h(shape, offset)
-00000910: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
-00000920: 6c69 6620 7479 7065 2873 6861 7065 2920  lif type(shape) 
-00000930: 6973 2073 652e 5356 4745 6c65 6d65 6e74  is se.SVGElement
-00000940: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00000950: 2020 2063 6f6e 7469 6e75 650d 0a20 2020     continue..   
-00000960: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
-00000970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000980: 6c6f 672e 7761 726e 696e 6728 6627 556e  log.warning(f'Un
-00000990: 7375 7070 6f72 7465 6420 656c 656d 656e  supported elemen
-000009a0: 7420 7479 7065 3a20 7b74 7970 6528 7368  t type: {type(sh
-000009b0: 6170 6529 7d27 290d 0a0d 0a20 2020 2020  ape)}')....     
-000009c0: 2020 2053 5647 4974 656d 2e76 6974 656d     SVGItem.vitem
-000009d0: 5f62 7569 6c64 6572 735f 6d61 705b 6b65  _builders_map[ke
-000009e0: 795d 203d 2062 7569 6c64 6572 730d 0a20  y] = builders.. 
-000009f0: 2020 2020 2020 2072 6574 7572 6e20 5b62         return [b
-00000a00: 7569 6c64 6572 2829 2066 6f72 2062 7569  uilder() for bui
-00000a10: 6c64 6572 2069 6e20 6275 696c 6465 7273  lder in builders
-00000a20: 5d0d 0a0d 0a20 2020 2040 7374 6174 6963  ]....    @static
-00000a30: 6d65 7468 6f64 0d0a 2020 2020 6465 6620  method..    def 
-00000a40: 636f 6e76 6572 745f 7061 7468 2870 6174  convert_path(pat
-00000a50: 683a 2073 652e 5061 7468 2c20 6f66 6673  h: se.Path, offs
-00000a60: 6574 3a20 6e70 2e6e 6461 7272 6179 2920  et: np.ndarray) 
-00000a70: 2d3e 2056 4974 656d 4275 696c 6465 723a  -> VItemBuilder:
-00000a80: 0d0a 2020 2020 2020 2020 6275 696c 6465  ..        builde
-00000a90: 7220 3d20 5061 7468 4275 696c 6465 7228  r = PathBuilder(
-00000aa0: 290d 0a20 2020 2020 2020 2073 6567 6d65  )..        segme
-00000ab0: 6e74 5f63 6c61 7373 5f74 6f5f 6675 6e63  nt_class_to_func
-00000ac0: 5f6d 6170 203d 207b 0d0a 2020 2020 2020  _map = {..      
-00000ad0: 2020 2020 2020 7365 2e4d 6f76 653a 2028        se.Move: (
-00000ae0: 6275 696c 6465 722e 6d6f 7665 5f74 6f2c  builder.move_to,
-00000af0: 2028 2765 6e64 272c 2929 2c0d 0a20 2020   ('end',)),..   
-00000b00: 2020 2020 2020 2020 2073 652e 436c 6f73           se.Clos
-00000b10: 653a 2028 6275 696c 6465 722e 636c 6f73  e: (builder.clos
-00000b20: 655f 7061 7468 2c20 2829 292c 0d0a 2020  e_path, ()),..  
-00000b30: 2020 2020 2020 2020 2020 7365 2e4c 696e            se.Lin
-00000b40: 653a 2028 6275 696c 6465 722e 6c69 6e65  e: (builder.line
-00000b50: 5f74 6f2c 2028 2765 6e64 272c 2929 2c0d  _to, ('end',)),.
-00000b60: 0a20 2020 2020 2020 2020 2020 2073 652e  .            se.
-00000b70: 5175 6164 7261 7469 6342 657a 6965 723a  QuadraticBezier:
-00000b80: 2028 6275 696c 6465 722e 636f 6e69 635f   (builder.conic_
-00000b90: 746f 2c20 2827 636f 6e74 726f 6c27 2c20  to, ('control', 
-00000ba0: 2765 6e64 2729 292c 0d0a 2020 2020 2020  'end')),..      
-00000bb0: 2020 2020 2020 7365 2e43 7562 6963 4265        se.CubicBe
-00000bc0: 7a69 6572 3a20 2862 7569 6c64 6572 2e63  zier: (builder.c
-00000bd0: 7562 6963 5f74 6f2c 2028 2763 6f6e 7472  ubic_to, ('contr
-00000be0: 6f6c 3127 2c20 2763 6f6e 7472 6f6c 3227  ol1', 'control2'
-00000bf0: 2c20 2765 6e64 2729 290d 0a20 2020 2020  , 'end'))..     
-00000c00: 2020 207d 0d0a 0d0a 2020 2020 2020 2020     }....        
-00000c10: 666f 7220 7365 676d 656e 7420 696e 2070  for segment in p
-00000c20: 6174 683a 0d0a 2020 2020 2020 2020 2020  ath:..          
-00000c30: 2020 7365 676d 656e 745f 636c 6173 7320    segment_class 
-00000c40: 3d20 7365 676d 656e 742e 5f5f 636c 6173  = segment.__clas
-00000c50: 735f 5f0d 0a20 2020 2020 2020 2020 2020  s__..           
-00000c60: 2066 756e 632c 2061 7474 725f 6e61 6d65   func, attr_name
-00000c70: 7320 3d20 7365 676d 656e 745f 636c 6173  s = segment_clas
-00000c80: 735f 746f 5f66 756e 635f 6d61 705b 7365  s_to_func_map[se
-00000c90: 676d 656e 745f 636c 6173 735d 0d0a 2020  gment_class]..  
-00000ca0: 2020 2020 2020 2020 2020 706f 696e 7473            points
-00000cb0: 203d 205b 0d0a 2020 2020 2020 2020 2020   = [..          
-00000cc0: 2020 2020 2020 5f63 6f6e 7665 7274 5f70        _convert_p
-00000cd0: 6f69 6e74 5f74 6f5f 3364 282a 6765 7461  oint_to_3d(*geta
-00000ce0: 7474 7228 7365 676d 656e 742c 2061 7474  ttr(segment, att
-00000cf0: 725f 6e61 6d65 2929 0d0a 2020 2020 2020  r_name))..      
-00000d00: 2020 2020 2020 2020 2020 666f 7220 6174            for at
-00000d10: 7472 5f6e 616d 6520 696e 2061 7474 725f  tr_name in attr_
-00000d20: 6e61 6d65 730d 0a20 2020 2020 2020 2020  names..         
-00000d30: 2020 205d 0d0a 2020 2020 2020 2020 2020     ]..          
-00000d40: 2020 6675 6e63 282a 706f 696e 7473 290d    func(*points).
-00000d50: 0a0d 0a20 2020 2020 2020 2076 6974 656d  ...        vitem
-00000d60: 5f73 7479 6c65 7320 3d20 6469 6374 280d  _styles = dict(.
-00000d70: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
-00000d80: 6f6b 655f 7261 6469 7573 3d70 6174 682e  oke_radius=path.
-00000d90: 7374 726f 6b65 5f77 6964 7468 202a 2053  stroke_width * S
-00000da0: 5452 4f4b 455f 5749 4454 485f 434f 4e56  TROKE_WIDTH_CONV
-00000db0: 4552 5349 4f4e 202f 2032 2c0d 0a20 2020  ERSION / 2,..   
-00000dc0: 2020 2020 2020 2020 2073 7472 6f6b 655f           stroke_
-00000dd0: 636f 6c6f 723d 7061 7468 2e73 7472 6f6b  color=path.strok
-00000de0: 652e 6865 782c 0d0a 2020 2020 2020 2020  e.hex,..        
-00000df0: 2020 2020 7374 726f 6b65 5f61 6c70 6861      stroke_alpha
-00000e00: 3d5f 636f 6e76 6572 745f 616c 7068 615f  =_convert_alpha_
-00000e10: 746f 5f66 6c6f 6174 2870 6174 682e 7374  to_float(path.st
-00000e20: 726f 6b65 2e61 6c70 6861 292c 0d0a 2020  roke.alpha),..  
-00000e30: 2020 2020 2020 2020 2020 6669 6c6c 5f63            fill_c
-00000e40: 6f6c 6f72 3d70 6174 682e 6669 6c6c 2e68  olor=path.fill.h
-00000e50: 6578 2c0d 0a20 2020 2020 2020 2020 2020  ex,..           
-00000e60: 2066 696c 6c5f 616c 7068 613d 5f63 6f6e   fill_alpha=_con
-00000e70: 7665 7274 5f61 6c70 6861 5f74 6f5f 666c  vert_alpha_to_fl
-00000e80: 6f61 7428 7061 7468 2e66 696c 6c2e 616c  oat(path.fill.al
-00000e90: 7068 6129 0d0a 2020 2020 2020 2020 290d  pha)..        ).
-00000ea0: 0a20 2020 2020 2020 2076 6974 656d 5f70  .        vitem_p
-00000eb0: 6f69 6e74 7320 3d20 6275 696c 6465 722e  oints = builder.
-00000ec0: 6765 7428 290d 0a20 2020 2020 2020 2076  get()..        v
-00000ed0: 6974 656d 5f70 6f69 6e74 735b 3a2c 203a  item_points[:, :
-00000ee0: 325d 202b 3d20 6f66 6673 6574 0d0a 0d0a  2] += offset....
-00000ef0: 2020 2020 2020 2020 6465 6620 7669 7465          def vite
-00000f00: 6d5f 6275 696c 6465 7228 2920 2d3e 2056  m_builder() -> V
-00000f10: 4974 656d 3a0d 0a20 2020 2020 2020 2020  Item:..         
-00000f20: 2020 2076 6974 656d 203d 2056 4974 656d     vitem = VItem
-00000f30: 282a 2a53 5647 4974 656d 2e73 7667 5f70  (**SVGItem.svg_p
-00000f40: 6172 745f 6465 6661 756c 745f 6b77 6172  art_default_kwar
-00000f50: 6773 290d 0a20 2020 2020 2020 2020 2020  gs)..           
-00000f60: 2076 6974 656d 2e73 6574 5f73 7479 6c65   vitem.set_style
-00000f70: 282a 2a76 6974 656d 5f73 7479 6c65 7329  (**vitem_styles)
-00000f80: 0d0a 2020 2020 2020 2020 2020 2020 7669  ..            vi
-00000f90: 7465 6d2e 706f 696e 7473 2e73 6574 2876  tem.points.set(v
-00000fa0: 6974 656d 5f70 6f69 6e74 7329 0d0a 2020  item_points)..  
-00000fb0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00000fc0: 2076 6974 656d 0d0a 0d0a 2020 2020 2020   vitem....      
-00000fd0: 2020 7265 7475 726e 2076 6974 656d 5f62    return vitem_b
-00000fe0: 7569 6c64 6572 0d0a                      uilder..
+00000160: 6e66 6967 0d0a 6672 6f6d 206a 616e 696d  nfig..from janim
+00000170: 2e75 7469 6c73 2e66 696c 655f 6f70 7320  .utils.file_ops 
+00000180: 696d 706f 7274 2066 696e 645f 6669 6c65  import find_file
+00000190: 0d0a 0d0a 2320 e8bf 99e9 878c e79a 8420  ....# ......... 
+000001a0: 332e 3237 3220 e698 afe6 898b e58a a8e8  3.272 ..........
+000001b0: af95 e587 bae6 9da5 e79a 840d 0a44 4546  .............DEF
+000001c0: 4155 4c54 5f53 5647 4954 454d 5f53 4341  AULT_SVGITEM_SCA
+000001d0: 4c45 5f46 4143 544f 5220 3d20 332e 3237  LE_FACTOR = 3.27
+000001e0: 320d 0a53 5452 4f4b 455f 5749 4454 485f  2..STROKE_WIDTH_
+000001f0: 434f 4e56 4552 5349 4f4e 203d 2030 2e30  CONVERSION = 0.0
+00000200: 310d 0a0d 0a74 7970 6520 5649 7465 6d42  1....type VItemB
+00000210: 7569 6c64 6572 203d 2043 616c 6c61 626c  uilder = Callabl
+00000220: 655b 5b5d 2c20 5649 7465 6d5d 0d0a 0d0a  e[[], VItem]....
+00000230: 0d0a 6465 6620 5f63 6f6e 7665 7274 5f70  ..def _convert_p
+00000240: 6f69 6e74 5f74 6f5f 3364 2878 3a20 666c  oint_to_3d(x: fl
+00000250: 6f61 742c 2079 3a20 666c 6f61 7429 202d  oat, y: float) -
+00000260: 3e20 6e70 2e6e 6461 7272 6179 3a0d 0a20  > np.ndarray:.. 
+00000270: 2020 2072 6574 7572 6e20 6e70 2e61 7272     return np.arr
+00000280: 6179 285b 782c 2079 2c20 305d 290d 0a0d  ay([x, y, 0])...
+00000290: 0a0d 0a64 6566 205f 636f 6e76 6572 745f  ...def _convert_
+000002a0: 616c 7068 615f 746f 5f66 6c6f 6174 2878  alpha_to_float(x
+000002b0: 3a20 696e 7420 7c20 4e6f 6e65 2920 2d3e  : int | None) ->
+000002c0: 2066 6c6f 6174 3a0d 0a20 2020 2072 6574   float:..    ret
+000002d0: 7572 6e20 4e6f 6e65 2069 6620 7820 6973  urn None if x is
+000002e0: 204e 6f6e 6520 656c 7365 2078 202f 2032   None else x / 2
+000002f0: 3535 0d0a 0d0a 0d0a 636c 6173 7320 5356  55......class SV
+00000300: 4749 7465 6d28 4772 6f75 705b 5649 7465  GItem(Group[VIte
+00000310: 6d5d 293a 0d0a 2020 2020 2727 270d 0a20  m]):..    '''.. 
+00000320: 2020 20e4 bca0 e585 a520 5356 4720 e696     ...... SVG ..
+00000330: 87e4 bbb6 e8b7 afe5 be84 efbc 8ce8 a7a3  ................
+00000340: e69e 90e4 b8ba e789 a9e4 bbb6 0d0a 2020  ..............  
+00000350: 2020 2727 270d 0a20 2020 2073 7667 5f70    '''..    svg_p
+00000360: 6172 745f 6465 6661 756c 745f 6b77 6172  art_default_kwar
+00000370: 6773 203d 2064 6963 7428 0d0a 2020 2020  gs = dict(..    
+00000380: 2020 2020 7374 726f 6b65 5f72 6164 6975      stroke_radiu
+00000390: 733d 312e 3020 2a20 5354 524f 4b45 5f57  s=1.0 * STROKE_W
+000003a0: 4944 5448 5f43 4f4e 5645 5253 494f 4e20  IDTH_CONVERSION 
+000003b0: 2f20 322c 0d0a 2020 2020 2020 2020 7374  / 2,..        st
+000003c0: 726f 6b65 5f63 6f6c 6f72 3d4e 6f6e 652c  roke_color=None,
+000003d0: 0d0a 2020 2020 2020 2020 7374 726f 6b65  ..        stroke
+000003e0: 5f61 6c70 6861 3d30 2c0d 0a20 2020 2020  _alpha=0,..     
+000003f0: 2020 2066 696c 6c5f 636f 6c6f 723d 4e6f     fill_color=No
+00000400: 6e65 2c0d 0a20 2020 2020 2020 2066 696c  ne,..        fil
+00000410: 6c5f 616c 7068 613d 300d 0a20 2020 2029  l_alpha=0..    )
+00000420: 0d0a 2020 2020 7669 7465 6d5f 6275 696c  ..    vitem_buil
+00000430: 6465 7273 5f6d 6170 3a20 6469 6374 5b74  ders_map: dict[t
+00000440: 7570 6c65 2c20 6c69 7374 5b56 4974 656d  uple, list[VItem
+00000450: 4275 696c 6465 725d 5d20 3d20 7b7d 0d0a  Builder]] = {}..
+00000460: 0d0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
+00000470: 5f5f 2873 656c 662c 2066 696c 655f 7061  __(self, file_pa
+00000480: 7468 3a20 7374 722c 202a 2a6b 7761 7267  th: str, **kwarg
+00000490: 7329 3a0d 0a20 2020 2020 2020 2069 7465  s):..        ite
+000004a0: 6d73 203d 2073 656c 662e 6765 745f 6974  ms = self.get_it
+000004b0: 656d 735f 6672 6f6d 5f66 696c 6528 6669  ems_from_file(fi
+000004c0: 6c65 5f70 6174 6829 0d0a 0d0a 2020 2020  le_path)....    
+000004d0: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
+000004e0: 6974 5f5f 282a 6974 656d 732c 202a 2a6b  it__(*items, **k
+000004f0: 7761 7267 7329 0d0a 0d0a 2020 2020 2020  wargs)....      
+00000500: 2020 7365 6c66 2856 4974 656d 292e 706f    self(VItem).po
+00000510: 696e 7473 2e73 6361 6c65 280d 0a20 2020  ints.scale(..   
+00000520: 2020 2020 2020 2020 2043 6f6e 6669 672e           Config.
+00000530: 6765 742e 7069 7865 6c5f 746f 5f66 7261  get.pixel_to_fra
+00000540: 6d65 5f72 6174 696f 202a 2044 4546 4155  me_ratio * DEFAU
+00000550: 4c54 5f53 5647 4954 454d 5f53 4341 4c45  LT_SVGITEM_SCALE
+00000560: 5f46 4143 544f 522c 0d0a 2020 2020 2020  _FACTOR,..      
+00000570: 2020 2020 2020 6162 6f75 745f 706f 696e        about_poin
+00000580: 743d 4f52 4947 494e 0d0a 2020 2020 2020  t=ORIGIN..      
+00000590: 2020 292e 666c 6970 2852 4947 4854 290d    ).flip(RIGHT).
+000005a0: 0a0d 0a20 2020 2020 2020 2073 656c 662e  ...        self.
+000005b0: 6d6f 7665 5f69 6e74 6f5f 706f 7369 7469  move_into_positi
+000005c0: 6f6e 2829 0d0a 0d0a 2020 2020 6465 6620  on()....    def 
+000005d0: 6d6f 7665 5f69 6e74 6f5f 706f 7369 7469  move_into_positi
+000005e0: 6f6e 2873 656c 6629 202d 3e20 4e6f 6e65  on(self) -> None
+000005f0: 3a0d 0a20 2020 2020 2020 2070 6173 730d  :..        pass.
+00000600: 0a0d 0a20 2020 2040 7374 6174 6963 6d65  ...    @staticme
+00000610: 7468 6f64 0d0a 2020 2020 6465 6620 6765  thod..    def ge
+00000620: 745f 6974 656d 735f 6672 6f6d 5f66 696c  t_items_from_fil
+00000630: 6528 6669 6c65 5f70 6174 683a 2073 7472  e(file_path: str
+00000640: 2920 2d3e 206c 6973 745b 4974 656d 5d3a  ) -> list[Item]:
+00000650: 0d0a 2020 2020 2020 2020 2727 270d 0a20  ..        '''.. 
+00000660: 2020 2020 2020 20e8 a7a3 e69e 90e6 9687         .........
+00000670: e4bb b6e5 b9b6 e5be 97e5 88b0 e789 a9e4  ................
+00000680: bbb6 e588 97e8 a1a8 0d0a 2020 2020 2020  ..........      
+00000690: 2020 2727 270d 0a20 2020 2020 2020 2066    '''..        f
+000006a0: 696c 655f 7061 7468 203d 2066 696e 645f  ile_path = find_
+000006b0: 6669 6c65 2866 696c 655f 7061 7468 290d  file(file_path).
+000006c0: 0a20 2020 2020 2020 206d 7469 6d65 203d  .        mtime =
+000006d0: 206f 732e 7061 7468 2e67 6574 6d74 696d   os.path.getmtim
+000006e0: 6528 6669 6c65 5f70 6174 6829 0d0a 2020  e(file_path)..  
+000006f0: 2020 2020 2020 6e61 6d65 203d 206f 732e        name = os.
+00000700: 7061 7468 2e73 706c 6974 6578 7428 6f73  path.splitext(os
+00000710: 2e70 6174 682e 6261 7365 6e61 6d65 2866  .path.basename(f
+00000720: 696c 655f 7061 7468 2929 5b30 5d0d 0a20  ile_path))[0].. 
+00000730: 2020 2020 2020 206b 6579 203d 2028 6e61         key = (na
+00000740: 6d65 2c20 6d74 696d 6529 0d0a 0d0a 2020  me, mtime)....  
+00000750: 2020 2020 2020 6361 6368 6564 203d 2053        cached = S
+00000760: 5647 4974 656d 2e76 6974 656d 5f62 7569  VGItem.vitem_bui
+00000770: 6c64 6572 735f 6d61 702e 6765 7428 6b65  lders_map.get(ke
+00000780: 792c 204e 6f6e 6529 0d0a 2020 2020 2020  y, None)..      
+00000790: 2020 6966 2063 6163 6865 6420 6973 206e    if cached is n
+000007a0: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+000007b0: 2020 2020 2020 7265 7475 726e 205b 6275        return [bu
+000007c0: 696c 6465 7228 2920 666f 7220 6275 696c  ilder() for buil
+000007d0: 6465 7220 696e 2063 6163 6865 645d 0d0a  der in cached]..
+000007e0: 0d0a 2020 2020 2020 2020 7376 673a 2073  ..        svg: s
+000007f0: 652e 5356 4720 3d20 7365 2e53 5647 2e70  e.SVG = se.SVG.p
+00000800: 6172 7365 2866 696c 655f 7061 7468 290d  arse(file_path).
+00000810: 0a0d 0a20 2020 2020 2020 206f 6666 7365  ...        offse
+00000820: 7420 3d20 6e70 2e61 7272 6179 285b 7376  t = np.array([sv
+00000830: 672e 7769 6474 6820 2f20 2d32 2c20 7376  g.width / -2, sv
+00000840: 672e 6865 6967 6874 202f 202d 325d 290d  g.height / -2]).
+00000850: 0a0d 0a20 2020 2020 2020 2062 7569 6c64  ...        build
+00000860: 6572 733a 206c 6973 745b 5649 7465 6d42  ers: list[VItemB
+00000870: 7569 6c64 6572 5d20 3d20 5b5d 0d0a 2020  uilder] = []..  
+00000880: 2020 2020 2020 666f 7220 7368 6170 6520        for shape 
+00000890: 696e 2073 7667 2e65 6c65 6d65 6e74 7328  in svg.elements(
+000008a0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+000008b0: 6966 2069 7369 6e73 7461 6e63 6528 7368  if isinstance(sh
+000008c0: 6170 652c 2028 7365 2e47 726f 7570 2c20  ape, (se.Group, 
+000008d0: 7365 2e55 7365 2929 3a0d 0a20 2020 2020  se.Use)):..     
+000008e0: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
+000008f0: 6e75 650d 0a20 2020 2020 2020 2020 2020  nue..           
+00000900: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
+00000910: 2873 6861 7065 2c20 7365 2e50 6174 6829  (shape, se.Path)
+00000920: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00000930: 2020 2062 7569 6c64 6572 732e 6170 7065     builders.appe
+00000940: 6e64 2853 5647 4974 656d 2e63 6f6e 7665  nd(SVGItem.conve
+00000950: 7274 5f70 6174 6828 7368 6170 652c 206f  rt_path(shape, o
+00000960: 6666 7365 7429 290d 0a20 2020 2020 2020  ffset))..       
+00000970: 2020 2020 2065 6c69 6620 7479 7065 2873       elif type(s
+00000980: 6861 7065 2920 6973 2073 652e 5356 4745  hape) is se.SVGE
+00000990: 6c65 6d65 6e74 3a0d 0a20 2020 2020 2020  lement:..       
+000009a0: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
+000009b0: 650d 0a20 2020 2020 2020 2020 2020 2065  e..            e
+000009c0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+000009d0: 2020 2020 2020 6c6f 672e 7761 726e 696e        log.warnin
+000009e0: 6728 6627 556e 7375 7070 6f72 7465 6420  g(f'Unsupported 
+000009f0: 656c 656d 656e 7420 7479 7065 3a20 7b74  element type: {t
+00000a00: 7970 6528 7368 6170 6529 7d27 290d 0a0d  ype(shape)}')...
+00000a10: 0a20 2020 2020 2020 2053 5647 4974 656d  .        SVGItem
+00000a20: 2e76 6974 656d 5f62 7569 6c64 6572 735f  .vitem_builders_
+00000a30: 6d61 705b 6b65 795d 203d 2062 7569 6c64  map[key] = build
+00000a40: 6572 730d 0a20 2020 2020 2020 2072 6574  ers..        ret
+00000a50: 7572 6e20 5b62 7569 6c64 6572 2829 2066  urn [builder() f
+00000a60: 6f72 2062 7569 6c64 6572 2069 6e20 6275  or builder in bu
+00000a70: 696c 6465 7273 5d0d 0a0d 0a20 2020 2040  ilders]....    @
+00000a80: 7374 6174 6963 6d65 7468 6f64 0d0a 2020  staticmethod..  
+00000a90: 2020 6465 6620 636f 6e76 6572 745f 7061    def convert_pa
+00000aa0: 7468 2870 6174 683a 2073 652e 5061 7468  th(path: se.Path
+00000ab0: 2c20 6f66 6673 6574 3a20 6e70 2e6e 6461  , offset: np.nda
+00000ac0: 7272 6179 2920 2d3e 2056 4974 656d 4275  rray) -> VItemBu
+00000ad0: 696c 6465 723a 0d0a 2020 2020 2020 2020  ilder:..        
+00000ae0: 6275 696c 6465 7220 3d20 5061 7468 4275  builder = PathBu
+00000af0: 696c 6465 7228 290d 0a20 2020 2020 2020  ilder()..       
+00000b00: 2073 6567 6d65 6e74 5f63 6c61 7373 5f74   segment_class_t
+00000b10: 6f5f 6675 6e63 5f6d 6170 203d 207b 0d0a  o_func_map = {..
+00000b20: 2020 2020 2020 2020 2020 2020 7365 2e4d              se.M
+00000b30: 6f76 653a 2028 6275 696c 6465 722e 6d6f  ove: (builder.mo
+00000b40: 7665 5f74 6f2c 2028 2765 6e64 272c 2929  ve_to, ('end',))
+00000b50: 2c0d 0a20 2020 2020 2020 2020 2020 2073  ,..            s
+00000b60: 652e 436c 6f73 653a 2028 6275 696c 6465  e.Close: (builde
+00000b70: 722e 636c 6f73 655f 7061 7468 2c20 2829  r.close_path, ()
+00000b80: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+00000b90: 7365 2e4c 696e 653a 2028 6275 696c 6465  se.Line: (builde
+00000ba0: 722e 6c69 6e65 5f74 6f2c 2028 2765 6e64  r.line_to, ('end
+00000bb0: 272c 2929 2c0d 0a20 2020 2020 2020 2020  ',)),..         
+00000bc0: 2020 2073 652e 5175 6164 7261 7469 6342     se.QuadraticB
+00000bd0: 657a 6965 723a 2028 6275 696c 6465 722e  ezier: (builder.
+00000be0: 636f 6e69 635f 746f 2c20 2827 636f 6e74  conic_to, ('cont
+00000bf0: 726f 6c27 2c20 2765 6e64 2729 292c 0d0a  rol', 'end')),..
+00000c00: 2020 2020 2020 2020 2020 2020 7365 2e43              se.C
+00000c10: 7562 6963 4265 7a69 6572 3a20 2862 7569  ubicBezier: (bui
+00000c20: 6c64 6572 2e63 7562 6963 5f74 6f2c 2028  lder.cubic_to, (
+00000c30: 2763 6f6e 7472 6f6c 3127 2c20 2763 6f6e  'control1', 'con
+00000c40: 7472 6f6c 3227 2c20 2765 6e64 2729 292c  trol2', 'end')),
+00000c50: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00000c60: 2e41 7263 3a20 286c 616d 6264 6120 7365  .Arc: (lambda se
+00000c70: 676d 656e 743a 2062 7569 6c64 6572 2e61  gment: builder.a
+00000c80: 7263 5f74 6f28 5f63 6f6e 7665 7274 5f70  rc_to(_convert_p
+00000c90: 6f69 6e74 5f74 6f5f 3364 282a 7365 676d  oint_to_3d(*segm
+00000ca0: 656e 742e 656e 6429 2c20 7365 676d 656e  ent.end), segmen
+00000cb0: 742e 7377 6565 7029 2c20 4e6f 6e65 292c  t.sweep), None),
+00000cc0: 0d0a 2020 2020 2020 2020 7d0d 0a0d 0a20  ..        }.... 
+00000cd0: 2020 2020 2020 2066 6f72 2073 6567 6d65         for segme
+00000ce0: 6e74 2069 6e20 7061 7468 3a0d 0a20 2020  nt in path:..   
+00000cf0: 2020 2020 2020 2020 2073 6567 6d65 6e74           segment
+00000d00: 5f63 6c61 7373 203d 2073 6567 6d65 6e74  _class = segment
+00000d10: 2e5f 5f63 6c61 7373 5f5f 0d0a 2020 2020  .__class__..    
+00000d20: 2020 2020 2020 2020 6675 6e63 2c20 6174          func, at
+00000d30: 7472 5f6e 616d 6573 203d 2073 6567 6d65  tr_names = segme
+00000d40: 6e74 5f63 6c61 7373 5f74 6f5f 6675 6e63  nt_class_to_func
+00000d50: 5f6d 6170 5b73 6567 6d65 6e74 5f63 6c61  _map[segment_cla
+00000d60: 7373 5d0d 0a20 2020 2020 2020 2020 2020  ss]..           
+00000d70: 2069 6620 6174 7472 5f6e 616d 6573 2069   if attr_names i
+00000d80: 7320 4e6f 6e65 3a0d 0a20 2020 2020 2020  s None:..       
+00000d90: 2020 2020 2020 2020 2066 756e 6328 7365           func(se
+00000da0: 676d 656e 7429 0d0a 2020 2020 2020 2020  gment)..        
+00000db0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00000dc0: 2020 2020 2020 2020 2020 2070 6f69 6e74             point
+00000dd0: 7320 3d20 5b0d 0a20 2020 2020 2020 2020  s = [..         
+00000de0: 2020 2020 2020 2020 2020 205f 636f 6e76             _conv
+00000df0: 6572 745f 706f 696e 745f 746f 5f33 6428  ert_point_to_3d(
+00000e00: 2a67 6574 6174 7472 2873 6567 6d65 6e74  *getattr(segment
+00000e10: 2c20 6174 7472 5f6e 616d 6529 290d 0a20  , attr_name)).. 
+00000e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e30: 2020 2066 6f72 2061 7474 725f 6e61 6d65     for attr_name
+00000e40: 2069 6e20 6174 7472 5f6e 616d 6573 0d0a   in attr_names..
+00000e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e60: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00000e70: 2020 2066 756e 6328 2a70 6f69 6e74 7329     func(*points)
+00000e80: 0d0a 0d0a 2020 2020 2020 2020 7669 7465  ....        vite
+00000e90: 6d5f 7374 796c 6573 203d 2064 6963 7428  m_styles = dict(
+00000ea0: 0d0a 2020 2020 2020 2020 2020 2020 7374  ..            st
+00000eb0: 726f 6b65 5f72 6164 6975 733d 7061 7468  roke_radius=path
+00000ec0: 2e73 7472 6f6b 655f 7769 6474 6820 2a20  .stroke_width * 
+00000ed0: 5354 524f 4b45 5f57 4944 5448 5f43 4f4e  STROKE_WIDTH_CON
+00000ee0: 5645 5253 494f 4e20 2f20 322c 0d0a 2020  VERSION / 2,..  
+00000ef0: 2020 2020 2020 2020 2020 7374 726f 6b65            stroke
+00000f00: 5f63 6f6c 6f72 3d70 6174 682e 7374 726f  _color=path.stro
+00000f10: 6b65 2e68 6578 2c0d 0a20 2020 2020 2020  ke.hex,..       
+00000f20: 2020 2020 2073 7472 6f6b 655f 616c 7068       stroke_alph
+00000f30: 613d 5f63 6f6e 7665 7274 5f61 6c70 6861  a=_convert_alpha
+00000f40: 5f74 6f5f 666c 6f61 7428 7061 7468 2e73  _to_float(path.s
+00000f50: 7472 6f6b 652e 616c 7068 6129 2c0d 0a20  troke.alpha),.. 
+00000f60: 2020 2020 2020 2020 2020 2066 696c 6c5f             fill_
+00000f70: 636f 6c6f 723d 7061 7468 2e66 696c 6c2e  color=path.fill.
+00000f80: 6865 782c 0d0a 2020 2020 2020 2020 2020  hex,..          
+00000f90: 2020 6669 6c6c 5f61 6c70 6861 3d5f 636f    fill_alpha=_co
+00000fa0: 6e76 6572 745f 616c 7068 615f 746f 5f66  nvert_alpha_to_f
+00000fb0: 6c6f 6174 2870 6174 682e 6669 6c6c 2e61  loat(path.fill.a
+00000fc0: 6c70 6861 290d 0a20 2020 2020 2020 2029  lpha)..        )
+00000fd0: 0d0a 2020 2020 2020 2020 7669 7465 6d5f  ..        vitem_
+00000fe0: 706f 696e 7473 203d 2062 7569 6c64 6572  points = builder
+00000ff0: 2e67 6574 2829 0d0a 2020 2020 2020 2020  .get()..        
+00001000: 7669 7465 6d5f 706f 696e 7473 5b3a 2c20  vitem_points[:, 
+00001010: 3a32 5d20 2b3d 206f 6666 7365 740d 0a0d  :2] += offset...
+00001020: 0a20 2020 2020 2020 2064 6566 2076 6974  .        def vit
+00001030: 656d 5f62 7569 6c64 6572 2829 202d 3e20  em_builder() -> 
+00001040: 5649 7465 6d3a 0d0a 2020 2020 2020 2020  VItem:..        
+00001050: 2020 2020 7669 7465 6d20 3d20 5649 7465      vitem = VIte
+00001060: 6d28 2a2a 5356 4749 7465 6d2e 7376 675f  m(**SVGItem.svg_
+00001070: 7061 7274 5f64 6566 6175 6c74 5f6b 7761  part_default_kwa
+00001080: 7267 7329 0d0a 2020 2020 2020 2020 2020  rgs)..          
+00001090: 2020 7669 7465 6d2e 7365 745f 7374 796c    vitem.set_styl
+000010a0: 6528 2a2a 7669 7465 6d5f 7374 796c 6573  e(**vitem_styles
+000010b0: 290d 0a20 2020 2020 2020 2020 2020 2076  )..            v
+000010c0: 6974 656d 2e70 6f69 6e74 732e 7365 7428  item.points.set(
+000010d0: 7669 7465 6d5f 706f 696e 7473 290d 0a20  vitem_points).. 
+000010e0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000010f0: 6e20 7669 7465 6d0d 0a0d 0a20 2020 2020  n vitem....     
+00001100: 2020 2072 6574 7572 6e20 7669 7465 6d5f     return vitem_
+00001110: 6275 696c 6465 720d 0a                   builder..
```

### Comparing `janim-0.5.2/janim/items/svg/typst.py` & `janim-1.0.0/janim/items/svg/typst.py`

 * *Files identical despite different names*

### Comparing `janim-0.5.2/janim/items/text/text.py` & `janim-1.0.0/janim/items/text/text.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from janim.utils.simple_functions import decode_utf8
 from janim.utils.space_ops import get_norm, normalize
 
 DEFAULT_FONT_SIZE = 24
 ORIG_FONT_SIZE = 48
 
 
-def get_color_value(key: str) -> JAnimColor:
+def _get_color_value(key: str) -> JAnimColor:
     '''
     根据 ``key`` 从 ``janim.constants.colors`` 得到颜色
 
     如果 ``key`` 以 ``#`` 开头，则直接返回原值
     '''
     if key.startswith('#'):
         return key
@@ -53,68 +53,75 @@
 type ActAt = int
 type ActStart = tuple[ActName, ActParams]
 type ActEnd = str
 
 available_act_map: dict[ActName, list[Act]] = defaultdict(list)
 
 
-def register_acts(names: list[ActName], *acts: Act) -> None:
+def _register_acts(names: list[ActName], *acts: Act) -> None:
     '''
     用于声明可用的富文本格式
     '''
     for name in names:
         available_act_map[name].extend(acts)
 
 
-register_acts(
+_register_acts(
     ['color', 'c'],
-    ((get_color_value,),            lambda char, color: char.color.set(color)),
+    ((_get_color_value,),           lambda char, color: char.color.set(color)),
     ((float, float, float),         lambda char, r, g, b: char.color.set([r, g, b])),
     ((float, float, float, float),  lambda char, r, g, b, a: char.color.set_rgbas([[r, g, b, a]]))
 )
-register_acts(
+_register_acts(
     ['stroke_color', 'sc'],
-    ((get_color_value,),            lambda char, color: char.stroke.set(color)),
+    ((_get_color_value,),           lambda char, color: char.stroke.set(color)),
     ((float, float, float),         lambda char, r, g, b: char.stroke.set([r, g, b])),
     ((float, float, float, float),  lambda char, r, g, b, a: char.stroke.set_rgbas([[r, g, b, a]]))
 )
-register_acts(
+_register_acts(
     ['fill_color', 'fc'],
-    ((get_color_value,),            lambda char, color: char.fill.set(color)),
+    ((_get_color_value,),           lambda char, color: char.fill.set(color)),
     ((float, float, float),         lambda char, r, g, b: char.fill.set([r, g, b])),
     ((float, float, float, float),  lambda char, r, g, b, a: char.fill.set_rgbas([[r, g, b, a]]))
 )
-register_acts(
+_register_acts(
     ['alpha', 'a'],
     ((float,), lambda char, a: char.color.set(alpha=a))
 )
-register_acts(
+_register_acts(
     ['stroke_alpha', 'sa'],
     ((float,), lambda char, a: char.stroke.set(alpha=a))
 )
-register_acts(
+_register_acts(
     ['fill_alpha', 'fa'],
     ((float,), lambda char, a: char.fill.set(alpha=a))
 )
-register_acts(
+_register_acts(
     ['stroke', 's'],
-    ((float,), lambda char, radius: char.stroke.set(radius))
+    ((float,), lambda char, radius: char.radius.set(radius))
 )
-register_acts(
+_register_acts(
     ['font_scale', 'fs'],
     ((float,), lambda char, factor: char.points.scale(factor, about_point=ORIGIN))
 )
 
 
 class TextChar(VItem):
     '''
     字符物件，作为 :class:`TextLine` 的子物件，在创建 :class:`TextLine` 时产生
     '''
-    def __init__(self, char: str, fonts: list[Font], font_size: float, **kwargs):
-        super().__init__(**kwargs)
+    def __init__(
+        self,
+        char: str,
+        fonts: list[Font],
+        font_size: float,
+        fill_alpha=None,
+        **kwargs
+    ):
+        super().__init__(fill_alpha=fill_alpha, **kwargs)
         self.char = char
 
         unicode = decode_utf8(char)
         font_render = self.get_font_for_render(unicode, fonts)
 
         outline, advance = font_render.get_glyph_data(unicode)
 
@@ -127,15 +134,17 @@
         # 标记位置
         self.mark = Points(
             ORIGIN, RIGHT * font_scale_factor, UP * font_scale_factor,
             [advance[0] * scale_factor, advance[1] * scale_factor, 0]
         )
         Cmpt_Points.apply_points_fn.connect(
             self.points,
-            lambda func, about_point: self.mark.points.apply_points_fn(func, about_point=about_point)
+            lambda func, about_point: self.mark.points.apply_points_fn(func,
+                                                                       about_point=about_point,
+                                                                       about_edge=None)
         )
 
     @staticmethod
     def get_font_for_render(unicode: str, fonts: list[Font]) -> Font:
         '''
         从字体列表中找到支持显示 ``unicode`` 的字体，如果找不到只好选用第一个
         '''
@@ -144,24 +153,24 @@
             idx = font.face.get_char_index(unicode)
             if idx != 0:
                 font_render = font
                 break
         return font_render
 
     def get_mark_orig(self) -> np.ndarray:
-        return self.mark.points._points._data[0].copy()
+        return self.mark.points._points.data[0]
 
     def get_mark_right(self) -> np.ndarray:
-        return self.mark.points._points._data[1].copy()
+        return self.mark.points._points.data[1]
 
     def get_mark_up(self) -> np.ndarray:
-        return self.mark.points._points._data[2].copy()
+        return self.mark.points._points.data[2]
 
     def get_mark_advance(self) -> np.ndarray:
-        return self.mark.points._points._data[3].copy()
+        return self.mark.points._points.data[3]
 
     def get_advance_length(self) -> float:
         return get_norm(self.get_mark_advance() - self.get_mark_orig())
 
     def apply_act_list(self, act_params_map: dict[str, ActParamsStack]) -> None:
         '''
         应用富文本样式，由 :meth:`Text.apply_rich_text` 调用
@@ -190,62 +199,70 @@
                 log.warning(f'应用 "{name}" 时，{params} 与 {txt} 没有匹配项')
 
 
 class TextLine(VItem, Group[TextChar]):
     '''
     单行文字物件，作为 :class:`Text` 的子物件，在创建 :class:`Text` 时产生s
     '''
-    def __init__(self, text: str, fonts: list[Font], font_size: float, char_kwargs={}, **kwargs):
+    def __init__(
+        self,
+        text: str,
+        fonts: list[Font],
+        font_size: float,
+        char_kwargs={},
+        fill_alpha=None,
+        **kwargs
+    ):
         self.text = text
 
         super().__init__(
             *[
                 TextChar(char, fonts, font_size, **char_kwargs)
                 for char in text
             ],
+            fill_alpha=fill_alpha,
             **kwargs
         )
 
         # 标记位置
         self.mark = Points(ORIGIN, RIGHT, UP)
         self.mark.points.scale(font_size / ORIG_FONT_SIZE, about_point=ORIGIN)
         Cmpt_Points.apply_points_fn.connect(
             self.points,
-            lambda func, about_point: self.mark.points.apply_points_fn(func, about_point=about_point)
+            lambda func, about_point: self.mark.points.apply_points_fn(func,
+                                                                       about_point=about_point,
+                                                                       about_edge=None)
         )
 
     def get_mark_orig(self) -> np.ndarray:
-        return self.mark.points._points._data[0].copy()
+        return self.mark.points._points.data[0]
 
     def get_mark_right(self) -> np.ndarray:
-        return self.mark.points._points._data[1].copy()
+        return self.mark.points._points.data[1]
 
     def get_mark_up(self) -> np.ndarray:
-        return self.mark.points._points._data[2].copy()
+        return self.mark.points._points.data[2]
 
     def arrange_in_line(self, buff: float = 0) -> Self:
         '''
         根据 ``advance`` 的标记信息排列该行
         '''
         if len(self.children) == 0:
             return
 
-        pos: np.ndarray = None
+        pos = None
+
+        for i, char in enumerate(self):
+            if i != 0:
+                char.points.shift(pos - char.get_mark_orig())
 
-        def update(char: TextChar) -> None:
-            nonlocal pos
             orig = char.get_mark_orig()
             advance = char.get_mark_advance()
             pos = advance if buff == 0 else advance + buff * normalize(advance - orig)
 
-        update(self[0])
-        for char in self[1:]:
-            char.points.shift(pos - char.get_mark_orig())
-            update(char)
-
         return self
 
 
 class Text(VItem, Group[TextLine]):
     '''
     文字物件
     '''
@@ -375,14 +392,16 @@
                 target - line.get_mark_orig()
             )
             pos = line.get_mark_orig()
 
         return self
 
     # TODO: word_wrap
+    # 使用 TypstDoc 可以轻松做到
+    # 我感觉可以不用给 Text 实现这功能了
 
     def apply_rich_text(self) -> None:
         '''
         应用富文本效果
         '''
         text_at = 0
         act_idx = 0
```

### Comparing `janim-0.5.2/janim/items/value_tracker.py` & `janim-1.0.0/janim/items/value_tracker.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 import copy
 from typing import Self
 
 from janim.components.component import CmptInfo
-from janim.components.data import Cmpt_Data, CopyFn, EqFn, InterpolateFn
+from janim.components.data import Cmpt_Data, CopyFn, MaybeSameFn, InterpolateFn
 from janim.items.item import Item
 from janim.utils.bezier import interpolate
 
 
 class ValueTracker[T](Item):
     '''
     记录一个数值数据（传入的数据作为初始值），可以进行动画插值
@@ -28,14 +28,14 @@
 
     data = CmptInfo(Cmpt_Data[Self, T])
 
     def __init__(
         self,
         value: T,
         copy_func: CopyFn[T] = copy.copy,
-        eq_func: EqFn[T] = lambda a, b: a == b,
+        maybe_same_func: MaybeSameFn[T] = lambda a, b: a == b,
         interpolate_func: InterpolateFn[T] = interpolate,
         **kwargs
     ):
         super().__init__(**kwargs)
-        self.data.set_func(copy_func, eq_func, interpolate_func)
+        self.data.set_func(copy_func, maybe_same_func, interpolate_func)
         self.data.set(value)
```

### Comparing `janim-0.5.2/janim/items/vitem.py` & `janim-1.0.0/janim/items/vitem.py`

 * *Files 16% similar despite different names*

```diff
@@ -61,17 +61,17 @@
 
         if fill_color is None:
             fill_color = color
         if fill_alpha is None:
             fill_alpha = alpha
 
         if stroke_radius is not None:
-            self.radius.set(stroke_radius)
-        self.stroke.set(stroke_color, stroke_alpha)
-        self.fill.set(fill_color, fill_alpha)
+            self.radius.set(stroke_radius, root_only=True)
+        self.stroke.set(stroke_color, stroke_alpha, root_only=True)
+        self.fill.set(fill_color, fill_alpha, root_only=True)
 
         return super().set_style(**kwargs)
 
     def add_tip(
         self,
         alpha: float = 1.0,
         reverse: bool = False,
@@ -113,42 +113,41 @@
         from janim.items.geometry.arrow import ArrowTip
         tip = ArrowTip(angle=angle, fill_color=fill_color, stroke_color=stroke_color, **tip_kwargs)
         tip.move_anchor_to(pos)
         self.add(tip)
 
         return tip
 
-    class Data(Points.Data['VItem']):
-        @classmethod
-        def align_for_interpolate(cls, data1: VItem.Data, data2: VItem.Data) -> AlignedData[Self]:
-            subpaths1_count = len(data1.cmpt.points.get_subpath_end_indices())
-            subpaths2_count = len(data2.cmpt.points.get_subpath_end_indices())
+    @classmethod
+    def align_for_interpolate(cls, item1: VItem, item2: VItem) -> AlignedData[Self]:
+        subpaths1_count = len(item1.points.get_subpath_end_indices())
+        subpaths2_count = len(item2.points.get_subpath_end_indices())
 
-            aligned = super().align_for_interpolate(data1, data2)
+        aligned = super().align_for_interpolate(item1, item2)
 
-            for data in (aligned.data1, aligned.data2):
-                count = (data.cmpt.points.count() + 1) // 2
-                data.cmpt.color.resize(count)
-                data.cmpt.radius.resize(count)
+        for item in (aligned.data1, aligned.data2):
+            count = (item.points.count() + 1) // 2
+            item.color.resize(count)
+            item.radius.resize(count)
 
-            if subpaths1_count != subpaths2_count:
-                diff = abs(subpaths1_count - subpaths2_count)
-                data = aligned.data1 if subpaths1_count < subpaths2_count else aligned.data2
-                indices = data.cmpt.points.get_subpath_end_indices()
+        if subpaths1_count != subpaths2_count:
+            diff = abs(subpaths1_count - subpaths2_count)
+            item = aligned.data1 if subpaths1_count < subpaths2_count else aligned.data2
+            indices = item.points.get_subpath_end_indices()
 
-                left_end = indices[0] // 2
-                right_start = indices[-1 - diff] // 2 + 1
+            left_end = indices[0] // 2
+            right_start = indices[-1 - diff] // 2 + 1
 
-                rgbas = data.cmpt.stroke.get()
+            rgbas = item.stroke.get().copy()
 
-                left = rgbas[:left_end + 1]
-                right = rgbas[right_start:]
+            left = rgbas[:left_end + 1]
+            right = rgbas[right_start:]
 
-                alphas = np.array([apart_alpha(alpha, diff + 1) for alpha in left[:, 3]])
-                left[:, 3] = alphas
+            alphas = np.array([apart_alpha(alpha, diff + 1) for alpha in left[:, 3]])
+            left[:, 3] = alphas
 
-                alphas = np.array([apart_alpha(alpha, diff + 1) for alpha in right[:, 3]])
-                right[:, 3] = alphas
+            alphas = np.array([apart_alpha(alpha, diff + 1) for alpha in right[:, 3]])
+            right[:, 3] = alphas
 
-                data.cmpt.stroke.set(rgbas)
+            item.stroke.set(rgbas)
 
-            return aligned
+        return aligned
```

### Comparing `janim-0.5.2/janim/render/base.py` & `janim-1.0.0/janim/render/base.py`

 * *Files identical despite different names*

### Comparing `janim-0.5.2/janim/render/impl.py` & `janim-1.0.0/janim/render/impl.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,18 +29,18 @@
             (self.vbo_radius, '1f', 'in_radius')
         ])
 
         self.prev_points = np.array([])
         self.prev_color = np.array([])
         self.prev_radius = np.array([])
 
-    def render(self, data: 'DotCloud.Data') -> None:
-        new_color = data.cmpt.color._rgbas._data
-        new_radius = data.cmpt.radius._radii._data
-        new_points = data.cmpt.points._points._data
+    def render(self, item: 'DotCloud') -> None:
+        new_color = item.color._rgbas.data
+        new_radius = item.radius._radii.data
+        new_points = item.points._points.data
 
         if id(new_color) != id(self.prev_color) or len(new_points) != len(self.prev_points):
             color = resize_with_interpolation(new_color, len(new_points))
             bytes = color.astype('f4').tobytes()
 
             if len(bytes) != self.vbo_color.size:
                 self.vbo_color.orphan(len(bytes))
@@ -86,30 +86,30 @@
         self.prev_camera_info = None
 
         self.prev_points = np.array([])
         self.prev_radius = np.array([])
         self.prev_stroke = np.array([])
         self.prev_fill = np.array([])
 
-    def render(self, data: 'VItem.Data') -> None:
-        if data.cmpt.points.curves_count() == 0:
+    def render(self, item: 'VItem') -> None:
+        if item.points.curves_count() == 0:
             return
         render_data = self.data_ctx.get()
 
         new_camera_info = render_data.camera_info
 
-        new_points = data.cmpt.points._points._data
-        new_radius = data.cmpt.radius._radii._data
-        new_stroke = data.cmpt.stroke._rgbas._data
-        new_fill = data.cmpt.fill._rgbas._data
+        new_points = item.points._points.data
+        new_radius = item.radius._radii.data
+        new_stroke = item.stroke._rgbas.data
+        new_fill = item.fill._rgbas.data
 
         is_camera_changed = id(new_camera_info) != id(self.prev_camera_info)
 
         if id(new_radius) != id(self.prev_radius) or id(new_points) != id(self.prev_points) or is_camera_changed:
-            clip_box = render_data.camera_info.map_points(data.cmpt.points.box.get_corners())
+            clip_box = render_data.camera_info.map_points(item.points.self_box.get_corners())
             clip_box *= render_data.camera_info.frame_radius
 
             buff = new_radius.max() + render_data.anti_alias_radius
             clip_min = np.min(clip_box, axis=0) - buff
             clip_max = np.max(clip_box, axis=0) + buff
             clip_box = np.array([
                 clip_min,
@@ -155,15 +155,15 @@
 
         if id(new_points) != id(self.prev_points) or is_camera_changed:
             mapped = render_data.camera_info.map_points(new_points)
             mapped *= render_data.camera_info.frame_radius
 
             bytes = np.hstack([
                 mapped,
-                data.cmpt.points.get_closepath_flags()[:, np.newaxis],
+                item.points.get_closepath_flags()[:, np.newaxis],
                 np.zeros((len(mapped), 1))
             ]).astype('f4').tobytes()
 
             if len(bytes) != self.vbo_mapped_points.size:
                 self.vbo_mapped_points.orphan(len(bytes))
 
             self.vbo_mapped_points.write(bytes)
@@ -199,17 +199,17 @@
             (self.vbo_texcoords, '2f', 'in_texcoord')
         ])
 
         self.prev_points = np.array([])
         self.prev_color = np.array([])
         self.prev_img = None
 
-    def render(self, data: 'ImageItem.Data') -> None:
-        new_color = data.cmpt.color._rgbas._data
-        new_points = data.cmpt.points._points._data
+    def render(self, item: 'ImageItem') -> None:
+        new_color = item.color._rgbas.data
+        new_points = item.points._points.data
 
         if id(new_color) != id(self.prev_color):
             color = resize_with_interpolation(new_color, 4)
             bytes = color.astype('f4').tobytes()
 
             assert len(bytes) == self.vbo_color.size
 
@@ -220,16 +220,16 @@
             bytes = new_points.astype('f4').tobytes()
 
             assert len(bytes) == self.vbo_points.size
 
             self.vbo_points.write(bytes)
             self.prev_points = new_points
 
-        if self.prev_img is None or data.cmpt.image != self.prev_img:
-            self.texture = get_texture_from_img(data.cmpt.image.get())
+        if self.prev_img is None or item.image != self.prev_img:
+            self.texture = get_texture_from_img(item.image.get())
             self.texture.build_mipmaps()
-            self.prev_img = data.cmpt.image
+            self.prev_img = item.image
 
         self.prog['image'] = 0
-        self.texture.filter = data.cmpt.image.get_filter()
+        self.texture.filter = item.image.get_filter()
         self.texture.use(0)
         self.vao.render(mgl.TRIANGLE_STRIP)
```

### Comparing `janim-0.5.2/janim/render/shaders/dotcloud.geom.glsl` & `janim-1.0.0/janim/render/shaders/dotcloud.geom.glsl`

 * *Files identical despite different names*

### Comparing `janim-0.5.2/janim/render/shaders/vitem.frag.glsl` & `janim-1.0.0/janim/render/shaders/vitem.frag.glsl`

 * *Files identical despite different names*

### Comparing `janim-0.5.2/janim/render/texture.py` & `janim-1.0.0/janim/render/texture.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,28 @@
+import os
+
 import moderngl as mgl
 from PIL import Image
 
 from janim.render.base import Renderer
+from janim.utils.file_ops import find_file
 
 filepath_to_img_map: dict[str, Image.Image] = {}
 
 
 def get_img_from_file(file_path: str) -> Image.Image:
-    img = filepath_to_img_map.get(file_path, None)
+    file_path = find_file(file_path)
+    mtime = os.path.getmtime(file_path)
+    key = (file_path, mtime)
+
+    img = filepath_to_img_map.get(key, None)
     if img is not None:
         return img
     img = Image.open(file_path).convert('RGBA')
-    filepath_to_img_map[file_path] = img
+    filepath_to_img_map[key] = img
     return img
 
 
 img_to_texture_map: dict[int, mgl.Texture] = {}
 
 
 def get_texture_from_img(img: Image.Image) -> mgl.Texture:
```

### Comparing `janim-0.5.2/janim/render/writer.py` & `janim-1.0.0/janim/render/writer.py`

 * *Files identical despite different names*

### Comparing `janim-0.5.2/janim/typing.py` & `janim-1.0.0/janim/typing.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,13 +21,13 @@
 
 
 @runtime_checkable
 class SupportsInterpolate[T](Protocol):
     @classmethod
     def align_for_interpolate(cls, obj1: object, obj2: object) -> AlignedData[T]: ...
 
-    def interpolate(self, obj1: object, obj2: object, *, path_func): ...
+    def interpolate(self, obj1: object, obj2: object, alpha: float, *, path_func): ...
 
 
 @runtime_checkable
 class SupportsApartAlpha(Protocol):
     def apart_alpha(self, n: int) -> None: ...
```

### Comparing `janim-0.5.2/janim/utils/bezier.py` & `janim-1.0.0/janim/utils/bezier.py`

 * *Files identical despite different names*

### Comparing `janim-0.5.2/janim/utils/dict_ops.py` & `janim-1.0.0/janim/utils/dict_ops.py`

 * *Files identical despite different names*

### Comparing `janim-0.5.2/janim/utils/font.py` & `janim-1.0.0/janim/utils/font.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+from dataclasses import dataclass
 from typing import Callable
 from functools import lru_cache
 
 import freetype as FT
 import numpy as np
 from fontTools.ttLib import TTCollection, TTFont
 
@@ -50,18 +51,29 @@
         Font.filepath_to_font_map[filepath] = font
         return font
 
     def __init__(self, filepath: str) -> None:
         self.face = FT.Face(filepath)
         self.face.select_charmap(FT.FT_ENCODING_UNICODE)
         self.face.set_char_size(48 << 6)
+        self.cached_glyph: dict[int, Font.GlyphData] = {}
+
+    @dataclass
+    class GlyphData:
+        array: np.ndarray
+        advance: tuple[int, int]
 
     def get_glyph_data(self, char: str) -> tuple[np.ndarray, tuple[int, int]]:
+        value = ord(char)
+        cached = self.cached_glyph.get(value, None)
+        if cached is not None:
+            return cached.array, cached.advance
+
         # 读取字符
-        self.face.load_char(char, FT.FT_LOAD_DEFAULT | FT.FT_LOAD_NO_BITMAP)
+        self.face.load_char(value, FT.FT_LOAD_DEFAULT | FT.FT_LOAD_NO_BITMAP)
         glyph: FT.Glyph = self.face.glyph
         outline: FT.Outline = glyph.outline
 
         builder: PathBuilder = PathBuilder()
 
         def wrap_points(func: Callable) -> Callable:
             def wrapper(*args) -> None:
@@ -73,8 +85,12 @@
             outline,
             wrap_points(builder.move_to),
             wrap_points(builder.line_to),
             wrap_points(builder.conic_to),
             wrap_points(builder.cubic_to)
         )
 
-        return builder.get(), (glyph.advance.x, glyph.advance.y)
+        data = Font.GlyphData(builder.get(), (glyph.advance.x, glyph.advance.y))
+        data.array.setflags(write=False)
+        self.cached_glyph[value] = data
+
+        return data.array, data.advance
```

### Comparing `janim-0.5.2/janim/utils/font_manager.py` & `janim-1.0.0/janim/utils/font_manager.py`

 * *Files identical despite different names*

### Comparing `janim-0.5.2/janim/utils/iterables.py` & `janim-1.0.0/janim/utils/iterables.py`

 * *Files identical despite different names*

### Comparing `janim-0.5.2/janim/utils/paths.py` & `janim-1.0.0/janim/utils/paths.py`

 * *Files identical despite different names*

### Comparing `janim-0.5.2/janim/utils/rate_functions.py` & `janim-1.0.0/janim/utils/rate_functions.py`

 * *Files identical despite different names*

### Comparing `janim-0.5.2/janim/utils/refresh.py` & `janim-1.0.0/janim/utils/refresh.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,57 @@
-from functools import wraps
-from typing import Any, Self, Callable, ParamSpec, TypeVar
 from collections import defaultdict
+from functools import partial, wraps
+from typing import Any, Callable, Self, overload
 
-# 使 sphinx 可用
-P = ParamSpec('P')
-R = TypeVar('R')
 
+@overload
+def register[T](func=None, /, *, fallback_check: Callable[[Any], bool]) -> Callable[[T], T]: ...
+@overload
+def register[T](func: T) -> T: ...
 
-def register(func: Callable[P, R]) -> Callable[P, R]:
+
+def register(func=None, /, *, fallback_check=None):
     '''
     用于在需要时才进行值的重新计算，提升性能
 
     当一个方法 self.func 被修饰后，会记忆 self.func 被调用后的返回值，
     并在之后的调用中直接返回该值，而不对 self.func 进行真正的调用；
     需要 ``self.mark_refresh_required(self.func)`` 才会对 self.func 重新调用以更新返回值
 
     例如，``Item`` 的 ``get_family`` 方法不会每次都进行计算
     只有在 ``add`` 或 ``remove`` 执行后，才会将 ``get_family`` 标记为需要更新
     使得在下次调用 ``get_family`` 才重新计算结果并返回
 
+    如果指定了 ``fallback_check`` 函数，则每次都会调用该函数，
+    如果返回值为 True，则忽略缓存，并且得到的结果不记录到缓存中
+
     另见：
 
     - ``test.utils.test_refresh.RefreshTest``.
     '''
+    if func is None:
+        # Called with @register()
+        return partial(_register, fallback_check=fallback_check)
+
+    # Called with @register
+    return _register(func)
+
+
+def _register[T](
+    func: T,
+    *,
+    fallback_check: Callable[[Any], bool] | None = None
+) -> T:
     name = func.__name__
 
     @wraps(func)
     def wrapper(self: Refreshable, *args, **kwargs):
+        if fallback_check is not None and fallback_check(self):
+            return func(self, *args, **kwargs)
+
         data = self.refresh_data[name]
 
         if data.is_required:
             data.stored = func(self, *args, **kwargs)
             data.is_required = False
 
         return data.stored
@@ -44,16 +65,16 @@
 
         self.refresh_data: defaultdict[str, RefreshData] = defaultdict(RefreshData)
 
     def mark_refresh(self, func: Callable | str) -> Self:
         '''
         标记指定的 ``func`` 需要进行更新
         '''
-        name = func.__name__ if isinstance(func, Callable) else func
-        data: RefreshData = self.refresh_data.setdefault(name, RefreshData())
+        name = func.__name__ if callable(func) else func
+        data: RefreshData = self.refresh_data[name]
         data.is_required = True
 
         return self
 
     def reset_refresh(self) -> Self:
         self.refresh_data = defaultdict(RefreshData)
```

### Comparing `janim-0.5.2/janim/utils/signal.py` & `janim-1.0.0/janim/utils/signal.py`

 * *Files 2% similar despite different names*

```diff
@@ -239,26 +239,14 @@
         for cls in sender.__class__.mro():
             full_qualname = self._get_cls_full_qualname(cls)
             if full_qualname not in all_slots.self_slots_dict:
                 continue
 
             slots = all_slots.self_slots_dict[full_qualname]
 
-            # pre-check
-            if slots.self_refresh_slots_with_recurse:
-                from janim.components.component import Component
-                from janim.items.relation import Relation
-
-                if not isinstance(sender, Relation) and not isinstance(sender, Component):
-                    # TODO: i18n
-                    raise TypeError(
-                        f'self_refresh_with_recurse() 无法在类 {sender.__class__} 中使用，'
-                        '只能在 Relation 和 Component 及子类中使用'
-                    )
-
             # self_normal_slots
             for func in slots.self_normal_slots:
                 func(sender, *args, **kwargs)
 
             # self_refresh_slots
             for func in slots.self_refresh_slots:
                 sender.mark_refresh(func)
```

### Comparing `janim-0.5.2/janim/utils/simple_functions.py` & `janim-1.0.0/janim/utils/simple_functions.py`

 * *Files identical despite different names*

### Comparing `janim-0.5.2/janim/utils/space_ops.py` & `janim-1.0.0/janim/utils/space_ops.py`

 * *Files identical despite different names*

### Comparing `janim-0.5.2/logo.png` & `janim-1.0.0/logo.png`

 * *Files identical despite different names*

### Comparing `janim-0.5.2/pyproject.toml` & `janim-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `janim-0.5.2/PKG-INFO` & `janim-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: janim
-Version: 0.5.2
+Version: 1.0.0
 Summary: a library for simple animation effects
 Author: jkjkil4
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python
 Requires-Dist: numpy
 Requires-Dist: scipy
```

