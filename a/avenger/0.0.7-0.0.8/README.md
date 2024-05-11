# Comparing `tmp/avenger-0.0.7.tar.gz` & `tmp/avenger-0.0.8.tar.gz`

## Comparing `avenger-0.0.7.tar` & `avenger-0.0.8.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0      501       20     1510 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-wgpu/Cargo.toml
--rw-r--r--   0      501       20       78 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-wgpu/README.md
--rw-r--r--   0      501       20    28421 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-wgpu/src/canvas.rs
--rw-r--r--   0      501       20     1800 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-wgpu/src/error.rs
--rw-r--r--   0      501       20     6818 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-wgpu/src/html_canvas.rs
--rw-r--r--   0      501       20      273 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-wgpu/src/lib.rs
--rw-r--r--   0      501       20    11018 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-wgpu/src/marks/cosmic.rs
--rw-r--r--   0      501       20     6491 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-wgpu/src/marks/gradient.rs
--rw-r--r--   0      501       20     4996 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-wgpu/src/marks/image.rs
--rw-r--r--   0      501       20    12845 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-wgpu/src/marks/instanced_mark.rs
--rw-r--r--   0      501       20      151 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-wgpu/src/marks/mod.rs
--rw-r--r--   0      501       20    83346 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-wgpu/src/marks/multi.rs
--rw-r--r--   0      501       20     8946 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-wgpu/src/marks/multi.wgsl
--rw-r--r--   0      501       20     8759 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-wgpu/src/marks/symbol.rs
--rw-r--r--   0      501       20     3130 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-wgpu/src/marks/symbol.wgsl
--rw-r--r--   0      501       20    15441 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-wgpu/src/marks/text.rs
--rw-r--r--   0      501       20     1329 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-wgpu/src/util.rs
--rw-r--r--   0      501       20    10704 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-wgpu/tests/test_image_baselines.rs
--rw-r--r--   0      501       20      533 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger/Cargo.toml
--rw-r--r--   0      501       20      129 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger/README.md
--rw-r--r--   0      501       20      735 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger/src/error.rs
--rw-r--r--   0      501       20       51 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger/src/lib.rs
--rw-r--r--   0      501       20     3689 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger/src/marks/arc.rs
--rw-r--r--   0      501       20     2414 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger/src/marks/area.rs
--rw-r--r--   0      501       20     4672 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger/src/marks/group.rs
--rw-r--r--   0      501       20     3031 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger/src/marks/image.rs
--rw-r--r--   0      501       20     1634 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger/src/marks/line.rs
--rw-r--r--   0      501       20     1329 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger/src/marks/mark.rs
--rw-r--r--   0      501       20      187 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger/src/marks/mod.rs
--rw-r--r--   0      501       20     2882 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger/src/marks/path.rs
--rw-r--r--   0      501       20     3831 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger/src/marks/rect.rs
--rw-r--r--   0      501       20     2873 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger/src/marks/rule.rs
--rw-r--r--   0      501       20    10808 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger/src/marks/symbol.rs
--rw-r--r--   0      501       20     5005 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger/src/marks/text.rs
--rw-r--r--   0      501       20     1551 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger/src/marks/trail.rs
--rw-r--r--   0      501       20     3215 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger/src/marks/value.rs
--rw-r--r--   0      501       20      249 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger/src/scene_graph.rs
--rw-r--r--   0      501       20       89 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger/tests/test_scene_graph.rs
--rw-r--r--   0      501       20     1101 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/Cargo.toml
--rw-r--r--   0      501       20      109 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/README.md
--rw-r--r--   0      501       20     1490 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/error.rs
--rw-r--r--   0      501       20      757 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/image/mod.rs
--rw-r--r--   0      501       20     1504 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/image/reqwest_fetcher.rs
--rw-r--r--   0      501       20     1724 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/image/svg.rs
--rw-r--r--   0      501       20      131 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/lib.rs
--rw-r--r--   0      501       20     5495 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/marks/arc.rs
--rw-r--r--   0      501       20     4361 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/marks/area.rs
--rw-r--r--   0      501       20     6737 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/marks/group.rs
--rw-r--r--   0      501       20     3759 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/marks/image.rs
--rw-r--r--   0      501       20     3215 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/marks/line.rs
--rw-r--r--   0      501       20     1522 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/marks/mark.rs
--rw-r--r--   0      501       20      203 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/marks/mod.rs
--rw-r--r--   0      501       20     5626 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/marks/path.rs
--rw-r--r--   0      501       20     4307 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/marks/rect.rs
--rw-r--r--   0      501       20     4382 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/marks/rule.rs
--rw-r--r--   0      501       20     5019 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/marks/shape.rs
--rw-r--r--   0      501       20     8093 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/marks/symbol.rs
--rw-r--r--   0      501       20     6400 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/marks/text.rs
--rw-r--r--   0      501       20     2795 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/marks/trail.rs
--rw-r--r--   0      501       20     6163 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/marks/values.rs
--rw-r--r--   0      501       20      749 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/src/scene_graph.rs
--rw-r--r--   0      501       20      757 2024-05-03 19:02:43.000000 avenger-0.0.7/avenger-vega/tests/test_parsing.rs
--rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 avenger-0.0.7/avenger-python/Cargo.toml
--rw-r--r--   0      501       20     1453 2024-05-03 19:02:42.000000 avenger-0.0.7/avenger-python/LICENSE
--rw-r--r--   0      501       20     2375 2024-05-03 19:02:42.000000 avenger-0.0.7/avenger-python/README.md
--rw-r--r--   0      501       20      172 2024-05-03 19:02:42.000000 avenger-0.0.7/avenger-python/avenger/__init__.py
--rw-r--r--   0      501       20     3643 2024-05-03 19:02:42.000000 avenger-0.0.7/avenger-python/avenger/altair_utils.py
--rw-r--r--   0      501       20     2547 2024-05-03 19:02:42.000000 avenger-0.0.7/avenger-python/src/lib.rs
--rw-r--r--   0      501       20   195804 2024-05-03 19:02:42.000000 avenger-0.0.7/Cargo.lock
--rw-r--r--   0        0        0      432 1970-01-01 00:00:00.000000 avenger-0.0.7/Cargo.toml
--rw-r--r--   0        0        0      496 1970-01-01 00:00:00.000000 avenger-0.0.7/pyproject.toml
--rw-r--r--   0      501       20      172 2024-05-03 19:02:42.000000 avenger-0.0.7/avenger/__init__.py
--rw-r--r--   0      501       20     3643 2024-05-03 19:02:42.000000 avenger-0.0.7/avenger/altair_utils.py
--rw-r--r--   0      501       20     2375 2024-05-03 19:02:42.000000 avenger-0.0.7/README.md
--rw-r--r--   0      501       20     1453 2024-05-03 19:02:42.000000 avenger-0.0.7/LICENSE
--rw-r--r--   0        0        0     2585 1970-01-01 00:00:00.000000 avenger-0.0.7/PKG-INFO
+-rw-r--r--   0      501       20     1562 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-wgpu/Cargo.toml
+-rw-r--r--   0      501       20       78 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-wgpu/README.md
+-rw-r--r--   0      501       20    28421 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-wgpu/src/canvas.rs
+-rw-r--r--   0      501       20     1800 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-wgpu/src/error.rs
+-rw-r--r--   0      501       20     6906 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-wgpu/src/html_canvas.rs
+-rw-r--r--   0      501       20      273 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-wgpu/src/lib.rs
+-rw-r--r--   0      501       20    11018 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-wgpu/src/marks/cosmic.rs
+-rw-r--r--   0      501       20     6491 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-wgpu/src/marks/gradient.rs
+-rw-r--r--   0      501       20     4996 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-wgpu/src/marks/image.rs
+-rw-r--r--   0      501       20    12959 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-wgpu/src/marks/instanced_mark.rs
+-rw-r--r--   0      501       20      151 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-wgpu/src/marks/mod.rs
+-rw-r--r--   0      501       20    83574 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-wgpu/src/marks/multi.rs
+-rw-r--r--   0      501       20     8946 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-wgpu/src/marks/multi.wgsl
+-rw-r--r--   0      501       20     8759 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-wgpu/src/marks/symbol.rs
+-rw-r--r--   0      501       20     3130 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-wgpu/src/marks/symbol.wgsl
+-rw-r--r--   0      501       20    15441 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-wgpu/src/marks/text.rs
+-rw-r--r--   0      501       20     1329 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-wgpu/src/util.rs
+-rw-r--r--   0      501       20    10704 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-wgpu/tests/test_image_baselines.rs
+-rw-r--r--   0      501       20     1101 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-vega/Cargo.toml
+-rw-r--r--   0      501       20      109 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-vega/README.md
+-rw-r--r--   0      501       20     1490 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-vega/src/error.rs
+-rw-r--r--   0      501       20      757 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-vega/src/image/mod.rs
+-rw-r--r--   0      501       20     1504 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-vega/src/image/reqwest_fetcher.rs
+-rw-r--r--   0      501       20     1724 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-vega/src/image/svg.rs
+-rw-r--r--   0      501       20      131 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-vega/src/lib.rs
+-rw-r--r--   0      501       20     5495 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-vega/src/marks/arc.rs
+-rw-r--r--   0      501       20     4361 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-vega/src/marks/area.rs
+-rw-r--r--   0      501       20     6737 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-vega/src/marks/group.rs
+-rw-r--r--   0      501       20     3759 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-vega/src/marks/image.rs
+-rw-r--r--   0      501       20     3215 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-vega/src/marks/line.rs
+-rw-r--r--   0      501       20     1522 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-vega/src/marks/mark.rs
+-rw-r--r--   0      501       20      203 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-vega/src/marks/mod.rs
+-rw-r--r--   0      501       20     5626 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-vega/src/marks/path.rs
+-rw-r--r--   0      501       20     4307 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-vega/src/marks/rect.rs
+-rw-r--r--   0      501       20     4382 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-vega/src/marks/rule.rs
+-rw-r--r--   0      501       20     5019 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-vega/src/marks/shape.rs
+-rw-r--r--   0      501       20     8093 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-vega/src/marks/symbol.rs
+-rw-r--r--   0      501       20     6400 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-vega/src/marks/text.rs
+-rw-r--r--   0      501       20     2795 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-vega/src/marks/trail.rs
+-rw-r--r--   0      501       20     6163 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-vega/src/marks/values.rs
+-rw-r--r--   0      501       20      749 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-vega/src/scene_graph.rs
+-rw-r--r--   0      501       20      757 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-vega/tests/test_parsing.rs
+-rw-r--r--   0      501       20      533 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger/Cargo.toml
+-rw-r--r--   0      501       20      129 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger/README.md
+-rw-r--r--   0      501       20      735 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger/src/error.rs
+-rw-r--r--   0      501       20       51 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger/src/lib.rs
+-rw-r--r--   0      501       20     3689 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger/src/marks/arc.rs
+-rw-r--r--   0      501       20     2414 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger/src/marks/area.rs
+-rw-r--r--   0      501       20     4672 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger/src/marks/group.rs
+-rw-r--r--   0      501       20     3031 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger/src/marks/image.rs
+-rw-r--r--   0      501       20     1634 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger/src/marks/line.rs
+-rw-r--r--   0      501       20     1329 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger/src/marks/mark.rs
+-rw-r--r--   0      501       20      187 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger/src/marks/mod.rs
+-rw-r--r--   0      501       20     2882 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger/src/marks/path.rs
+-rw-r--r--   0      501       20     3831 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger/src/marks/rect.rs
+-rw-r--r--   0      501       20     2873 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger/src/marks/rule.rs
+-rw-r--r--   0      501       20    10808 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger/src/marks/symbol.rs
+-rw-r--r--   0      501       20     5005 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger/src/marks/text.rs
+-rw-r--r--   0      501       20     1551 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger/src/marks/trail.rs
+-rw-r--r--   0      501       20     3215 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger/src/marks/value.rs
+-rw-r--r--   0      501       20      249 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger/src/scene_graph.rs
+-rw-r--r--   0      501       20       89 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger/tests/test_scene_graph.rs
+-rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 avenger-0.0.8/avenger-python/Cargo.toml
+-rw-r--r--   0      501       20     1453 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-python/LICENSE
+-rw-r--r--   0      501       20     2375 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-python/README.md
+-rw-r--r--   0      501       20      172 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-python/avenger/__init__.py
+-rw-r--r--   0      501       20     3643 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-python/avenger/altair_utils.py
+-rw-r--r--   0      501       20     2547 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger-python/src/lib.rs
+-rw-r--r--   0      501       20   196037 2024-05-11 20:50:15.000000 avenger-0.0.8/Cargo.lock
+-rw-r--r--   0        0        0      432 1970-01-01 00:00:00.000000 avenger-0.0.8/Cargo.toml
+-rw-r--r--   0        0        0      496 1970-01-01 00:00:00.000000 avenger-0.0.8/pyproject.toml
+-rw-r--r--   0      501       20      172 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger/__init__.py
+-rw-r--r--   0      501       20     3643 2024-05-11 20:50:15.000000 avenger-0.0.8/avenger/altair_utils.py
+-rw-r--r--   0      501       20     2375 2024-05-11 20:50:15.000000 avenger-0.0.8/README.md
+-rw-r--r--   0      501       20     1453 2024-05-11 20:50:15.000000 avenger-0.0.8/LICENSE
+-rw-r--r--   0        0        0     2585 1970-01-01 00:00:00.000000 avenger-0.0.8/PKG-INFO
```

### Comparing `avenger-0.0.7/avenger-wgpu/Cargo.toml` & `avenger-0.0.8/avenger-wgpu/Cargo.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 [package]
 name = "avenger-wgpu"
-version = "0.0.7"
+version = "0.0.8"
 edition = "2021"
 description = "WGPU rendering engine for the Avenger visualization framework"
 license = "BSD-3-Clause"
+repository = "https://github.com/jonmmease/avenger"
 
 [lib]
 crate-type = [ "cdylib", "rlib",]
 
 [features]
 default = [ "cosmic-text", "rayon",]
 cosmic-text = [ "dep:cosmic-text", "lazy_static",]
 deno = []
 
 [dependencies]
 cfg-if = "1"
 winit = "0.29.9"
 env_logger = "0.10"
 log = "0.4"
-wgpu = "0.19.3"
+wgpu = "0.20.0"
 pollster = "0.3"
 cgmath = "0.18.0"
 itertools = "0.12.0"
 image = "0.24.7"
 futures-intrusive = "^0.5"
 etagere = "0.2.10"
 colorgrad = "0.6.2"
 
 [dev-dependencies]
 dssim = "3.2.4"
 rstest = "0.18.2"
 
 [dependencies.avenger]
 path = "../avenger"
-version = "0.0.7"
+version = "0.0.8"
 
 [dependencies.rayon]
 workspace = true
 optional = true
 
 [dependencies.tracing]
 workspace = true
@@ -63,19 +64,19 @@
 
 [dependencies.lyon]
 workspace = true
 
 [dev-dependencies.avenger-vega]
 path = "../avenger-vega"
 features = [ "image-request", "svg",]
-version = "0.0.7"
+version = "0.0.8"
 
 [dev-dependencies.serde_json]
 version = "1.0.111"
 
 [target."cfg(target_arch = \"wasm32\")".dependencies.wgpu]
-version = "0.19.3"
+version = "0.20.0"
 default-features = false
 
 [target."cfg(target_arch = \"wasm32\")".dependencies.web-sys]
 version = "0.3.67"
 features = [ "Document", "Window", "Element", "HtmlCanvasElement",]
```

### Comparing `avenger-0.0.7/avenger-wgpu/src/canvas.rs` & `avenger-0.0.8/avenger-wgpu/src/canvas.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger-wgpu/src/error.rs` & `avenger-0.0.8/avenger-wgpu/src/error.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger-wgpu/src/html_canvas.rs` & `avenger-0.0.8/avenger-wgpu/src/html_canvas.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 use crate::canvas::{
     create_multisampled_framebuffer, get_supported_sample_count, make_background_command,
-    make_wgpu_adapter, make_wgpu_instance, request_wgpu_device, Canvas, CanvasConfig,
-    CanvasDimensions, MarkRenderer,
+    make_wgpu_adapter, request_wgpu_device, Canvas, CanvasConfig, CanvasDimensions, MarkRenderer,
 };
 use crate::error::AvengerWgpuError;
 use crate::marks::multi::MultiMarkRenderer;
 use web_sys::HtmlCanvasElement;
 use wgpu::{
     Device, Queue, Surface, SurfaceConfiguration, SurfaceTarget, TextureFormat, TextureUsages,
     TextureView, TextureViewDescriptor,
@@ -31,15 +30,18 @@
     pub async fn new(
         canvas: HtmlCanvasElement,
         dimensions: CanvasDimensions,
         config: CanvasConfig,
     ) -> Result<Self, AvengerWgpuError> {
         canvas.set_width(dimensions.to_physical_width());
         canvas.set_height(dimensions.to_physical_height());
-        let instance = make_wgpu_instance();
+        let instance = wgpu::Instance::new(wgpu::InstanceDescriptor {
+            backends: wgpu::Backends::GL,
+            ..Default::default()
+        });
         let surface = instance.create_surface(SurfaceTarget::Canvas(canvas))?;
         let adapter = make_wgpu_adapter(&instance, Some(&surface)).await?;
         let (device, queue) = request_wgpu_device(&adapter).await?;
 
         let surface_caps = surface.get_capabilities(&adapter);
 
         // Select first non-srgb texture format
```

### Comparing `avenger-0.0.7/avenger-wgpu/src/marks/cosmic.rs` & `avenger-0.0.8/avenger-wgpu/src/marks/cosmic.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger-wgpu/src/marks/gradient.rs` & `avenger-0.0.8/avenger-wgpu/src/marks/gradient.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger-wgpu/src/marks/image.rs` & `avenger-0.0.8/avenger-wgpu/src/marks/image.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger-wgpu/src/marks/instanced_mark.rs` & `avenger-0.0.8/avenger-wgpu/src/marks/instanced_mark.rs`

 * *Files 1% similar despite different names*

```diff
@@ -177,19 +177,21 @@
 
         let render_pipeline = device.create_render_pipeline(&wgpu::RenderPipelineDescriptor {
             label: Some("Render Pipeline"),
             layout: Some(&render_pipeline_layout),
             vertex: wgpu::VertexState {
                 module: &shader,
                 entry_point: mark_shader.vertex_entry_point(),
+                compilation_options: Default::default(),
                 buffers: &[mark_shader.vertex_desc(), mark_shader.instance_desc()],
             },
             fragment: Some(wgpu::FragmentState {
                 module: &shader,
                 entry_point: mark_shader.fragment_entry_point(),
+                compilation_options: Default::default(),
                 targets: &[Some(wgpu::ColorTargetState {
                     format: texture_format,
                     blend: Some(wgpu::BlendState::ALPHA_BLENDING),
                     write_mask: wgpu::ColorWrites::ALL,
                 })],
             }),
             primitive: wgpu::PrimitiveState {
```

### Comparing `avenger-0.0.7/avenger-wgpu/src/marks/multi.rs` & `avenger-0.0.8/avenger-wgpu/src/marks/multi.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1619,19 +1619,21 @@
 
         let render_pipeline = device.create_render_pipeline(&wgpu::RenderPipelineDescriptor {
             label: Some("Render Pipeline"),
             layout: Some(&render_pipeline_layout),
             vertex: wgpu::VertexState {
                 module: &shader,
                 entry_point: "vs_main",
+                compilation_options: Default::default(),
                 buffers: &[MultiVertex::desc()],
             },
             fragment: Some(wgpu::FragmentState {
                 module: &shader,
                 entry_point: "fs_main",
+                compilation_options: Default::default(),
                 targets: &[Some(wgpu::ColorTargetState {
                     format: texture_format,
                     blend: Some(wgpu::BlendState::ALPHA_BLENDING),
                     write_mask: wgpu::ColorWrites::ALL,
                 })],
             }),
             primitive: wgpu::PrimitiveState {
@@ -1669,19 +1671,21 @@
 
         let stencil_pipeline = device.create_render_pipeline(&wgpu::RenderPipelineDescriptor {
             label: None,
             layout: Some(&render_pipeline_layout),
             vertex: wgpu::VertexState {
                 module: &shader,
                 entry_point: "vs_main",
+                compilation_options: Default::default(),
                 buffers: &[MultiVertex::desc()],
             },
             fragment: Some(wgpu::FragmentState {
                 module: &shader,
                 entry_point: "fs_main",
+                compilation_options: Default::default(),
                 targets: &[Some(wgpu::ColorTargetState {
                     format: texture_format,
                     blend: None,
                     write_mask: wgpu::ColorWrites::empty(),
                 })],
             }),
             primitive: Default::default(),
```

### Comparing `avenger-0.0.7/avenger-wgpu/src/marks/multi.wgsl` & `avenger-0.0.8/avenger-wgpu/src/marks/multi.wgsl`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger-wgpu/src/marks/symbol.rs` & `avenger-0.0.8/avenger-wgpu/src/marks/symbol.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger-wgpu/src/marks/symbol.wgsl` & `avenger-0.0.8/avenger-wgpu/src/marks/symbol.wgsl`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger-wgpu/src/marks/text.rs` & `avenger-0.0.8/avenger-wgpu/src/marks/text.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger-wgpu/src/util.rs` & `avenger-0.0.8/avenger-wgpu/src/util.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger-wgpu/tests/test_image_baselines.rs` & `avenger-0.0.8/avenger-wgpu/tests/test_image_baselines.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger/Cargo.toml` & `avenger-0.0.8/avenger/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "avenger"
-version = "0.0.7"
+version = "0.0.8"
 edition = "2021"
 description = "A visualization engine and renderer"
 license = "BSD-3-Clause"
 
 [dependencies.thiserror]
 workspace = true
```

### Comparing `avenger-0.0.7/avenger/src/error.rs` & `avenger-0.0.8/avenger/src/error.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger/src/marks/arc.rs` & `avenger-0.0.8/avenger/src/marks/arc.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger/src/marks/area.rs` & `avenger-0.0.8/avenger/src/marks/area.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger/src/marks/group.rs` & `avenger-0.0.8/avenger/src/marks/group.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger/src/marks/image.rs` & `avenger-0.0.8/avenger/src/marks/image.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger/src/marks/line.rs` & `avenger-0.0.8/avenger/src/marks/line.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger/src/marks/mark.rs` & `avenger-0.0.8/avenger/src/marks/mark.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger/src/marks/path.rs` & `avenger-0.0.8/avenger/src/marks/path.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger/src/marks/rect.rs` & `avenger-0.0.8/avenger/src/marks/rect.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger/src/marks/rule.rs` & `avenger-0.0.8/avenger/src/marks/rule.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger/src/marks/symbol.rs` & `avenger-0.0.8/avenger/src/marks/symbol.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger/src/marks/text.rs` & `avenger-0.0.8/avenger/src/marks/text.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger/src/marks/trail.rs` & `avenger-0.0.8/avenger/src/marks/trail.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger/src/marks/value.rs` & `avenger-0.0.8/avenger/src/marks/value.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger-vega/Cargo.toml` & `avenger-0.0.8/avenger-vega/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "avenger-vega"
-version = "0.0.7"
+version = "0.0.8"
 edition = "2021"
 description = "Utilities for importing Vega scenegraphs into Avenger"
 license = "BSD-3-Clause"
 
 [features]
 image-request = [ "reqwest",]
 svg = [ "resvg", "usvg", "tiny-skia",]
@@ -29,15 +29,15 @@
 workspace = true
 
 [dependencies.tracing]
 workspace = true
 
 [dependencies.avenger]
 path = "../avenger"
-version = "0.0.7"
+version = "0.0.8"
 
 [dependencies.thiserror]
 workspace = true
 
 [dependencies.serde]
 workspace = true
```

### Comparing `avenger-0.0.7/avenger-vega/src/error.rs` & `avenger-0.0.8/avenger-vega/src/error.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger-vega/src/image/mod.rs` & `avenger-0.0.8/avenger-vega/src/image/mod.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger-vega/src/image/reqwest_fetcher.rs` & `avenger-0.0.8/avenger-vega/src/image/reqwest_fetcher.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger-vega/src/image/svg.rs` & `avenger-0.0.8/avenger-vega/src/image/svg.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger-vega/src/marks/arc.rs` & `avenger-0.0.8/avenger-vega/src/marks/arc.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger-vega/src/marks/area.rs` & `avenger-0.0.8/avenger-vega/src/marks/area.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger-vega/src/marks/group.rs` & `avenger-0.0.8/avenger-vega/src/marks/group.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger-vega/src/marks/image.rs` & `avenger-0.0.8/avenger-vega/src/marks/image.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger-vega/src/marks/line.rs` & `avenger-0.0.8/avenger-vega/src/marks/line.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger-vega/src/marks/mark.rs` & `avenger-0.0.8/avenger-vega/src/marks/mark.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger-vega/src/marks/path.rs` & `avenger-0.0.8/avenger-vega/src/marks/path.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger-vega/src/marks/rect.rs` & `avenger-0.0.8/avenger-vega/src/marks/rect.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger-vega/src/marks/rule.rs` & `avenger-0.0.8/avenger-vega/src/marks/rule.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger-vega/src/marks/shape.rs` & `avenger-0.0.8/avenger-vega/src/marks/shape.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger-vega/src/marks/symbol.rs` & `avenger-0.0.8/avenger-vega/src/marks/symbol.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger-vega/src/marks/text.rs` & `avenger-0.0.8/avenger-vega/src/marks/text.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger-vega/src/marks/trail.rs` & `avenger-0.0.8/avenger-vega/src/marks/trail.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger-vega/src/marks/values.rs` & `avenger-0.0.8/avenger-vega/src/marks/values.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger-vega/src/scene_graph.rs` & `avenger-0.0.8/avenger-vega/src/scene_graph.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger-vega/tests/test_parsing.rs` & `avenger-0.0.8/avenger-vega/tests/test_parsing.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger-python/Cargo.toml` & `avenger-0.0.8/avenger-python/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "avenger-python"
-version = "0.0.7"
+version = "0.0.8"
 edition = "2021"
 license = "BSD-3-Clause"
 description = "Python API to Avenger visualization framework"
 publish = false
 
 [lib]
 name = "avenger"
@@ -13,25 +13,25 @@
 [dependencies]
 pythonize = "0.20.0"
 pollster = "0.3"
 
 [dependencies.avenger]
 path = "../avenger"
 features = [ "pyo3",]
-version = "0.0.7"
+version = "0.0.8"
 
 [dependencies.avenger-vega]
 path = "../avenger-vega"
 features = [ "pyo3",]
-version = "0.0.7"
+version = "0.0.8"
 
 [dependencies.avenger-wgpu]
 path = "../avenger-wgpu"
 features = [ "pyo3",]
-version = "0.0.7"
+version = "0.0.8"
 
 [dependencies.pyo3]
 workspace = true
 features = [ "extension-module", "abi3-py38",]
 
 [dependencies.serde]
 workspace = true
```

### Comparing `avenger-0.0.7/avenger-python/LICENSE` & `avenger-0.0.8/avenger-python/LICENSE`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger-python/README.md` & `avenger-0.0.8/avenger-python/README.md`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger-python/avenger/altair_utils.py` & `avenger-0.0.8/avenger-python/avenger/altair_utils.py`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/avenger-python/src/lib.rs` & `avenger-0.0.8/avenger-python/src/lib.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/Cargo.lock` & `avenger-0.0.8/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
 [[package]]
 name = "android-activity"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ee91c0c2905bae44f84bfa4e044536541df26b7703fd0888deeb9060fcc44289"
 dependencies = [
  "android-properties",
- "bitflags 2.4.1",
+ "bitflags 2.5.0",
  "cc",
  "cesu8",
  "jni",
  "jni-sys",
  "libc",
  "log",
  "ndk",
@@ -321,29 +321,29 @@
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "avenger"
-version = "0.0.7"
+version = "0.0.8"
 dependencies = [
  "image",
  "lyon_extra",
  "lyon_path",
  "pyo3",
  "rayon",
  "serde",
  "thiserror",
  "tracing",
 ]
 
 [[package]]
 name = "avenger-python"
-version = "0.0.7"
+version = "0.0.8"
 dependencies = [
  "avenger",
  "avenger-vega",
  "avenger-wgpu",
  "image",
  "lazy_static",
  "pollster",
@@ -352,15 +352,15 @@
  "serde",
  "tracing",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "avenger-vega"
-version = "0.0.7"
+version = "0.0.8"
 dependencies = [
  "avenger",
  "cfg-if",
  "csscolorparser",
  "image",
  "lazy_static",
  "lyon_extra",
@@ -374,15 +374,15 @@
  "tiny-skia",
  "tracing",
  "usvg 0.38.0",
 ]
 
 [[package]]
 name = "avenger-vega-renderer"
-version = "0.0.7"
+version = "0.0.8"
 dependencies = [
  "avenger",
  "avenger-vega",
  "avenger-wgpu",
  "console_error_panic_hook",
  "csscolorparser",
  "gloo-utils",
@@ -398,24 +398,24 @@
  "wasm-bindgen-futures",
  "web-sys",
  "wgpu",
 ]
 
 [[package]]
 name = "avenger-vega-test-data"
-version = "0.0.7"
+version = "0.0.8"
 dependencies = [
  "pollster",
  "serde_json",
  "vl-convert-rs",
 ]
 
 [[package]]
 name = "avenger-wgpu"
-version = "0.0.7"
+version = "0.0.8"
 dependencies = [
  "avenger",
  "avenger-vega",
  "bytemuck",
  "cfg-if",
  "cgmath",
  "colorgrad",
@@ -524,17 +524,17 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
-version = "2.4.1"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "327762f6e5a765692301e5bb513e0d9fef63be86bbc14528052b1cd3e6f03e07"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "block"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0d8c1fef690941d3e7788d328517591fecc684c084084702d6ff1641e993699a"
 
@@ -642,15 +642,15 @@
 
 [[package]]
 name = "calloop"
 version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fba7adb4dd5aa98e5553510223000e7148f621165ec5f9acd7113f6ca4995298"
 dependencies = [
- "bitflags 2.4.1",
+ "bitflags 2.5.0",
  "log",
  "polling",
  "rustix",
  "slab",
  "thiserror",
 ]
 
@@ -882,15 +882,15 @@
 
 [[package]]
 name = "cosmic-text"
 version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c578f2b9abb4d5f3fbb12aba4008084d435dc6a8425c195cfe0b3594bfea0c25"
 dependencies = [
- "bitflags 2.4.1",
+ "bitflags 2.5.0",
  "fontdb 0.16.0",
  "libm",
  "log",
  "rangemap",
  "rustc-hash",
  "rustybuzz 0.12.1",
  "self_cell",
@@ -1055,20 +1055,20 @@
  "proc-macro2",
  "quote",
  "syn 2.0.47",
 ]
 
 [[package]]
 name = "d3d12"
-version = "0.19.0"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3e3d747f100290a1ca24b752186f61f6637e1deffe3bf6320de6fcb29510a307"
+checksum = "b28bfe653d79bd16c77f659305b195b82bb5ce0c0eb2a4846b82ddbd77586813"
 dependencies = [
- "bitflags 2.4.1",
- "libloading 0.8.1",
+ "bitflags 2.5.0",
+ "libloading 0.7.4",
  "winapi",
 ]
 
 [[package]]
 name = "dashmap"
 version = "5.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1917,14 +1917,23 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.47",
 ]
 
 [[package]]
+name = "document-features"
+version = "0.2.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ef5282ad69563b5fc40319526ba27e0e7363d552a896f0297d54f767717f9b95"
+dependencies = [
+ "litrs",
+]
+
+[[package]]
 name = "downcast-rs"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ea835d29036a4087793836fa931b08837ad5e957da9e23886b29586fb9b6650"
 
 [[package]]
 name = "dprint-swc-ext"
@@ -2696,25 +2705,25 @@
 
 [[package]]
 name = "gpu-alloc"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fbcd2dba93594b227a1f57ee09b8b9da8892c34d55aa332e034a228d0fe6a171"
 dependencies = [
- "bitflags 2.4.1",
+ "bitflags 2.5.0",
  "gpu-alloc-types",
 ]
 
 [[package]]
 name = "gpu-alloc-types"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "98ff03b468aa837d70984d55f5d3f846f6ec31fe34bbb97c4f85219caeee1ca4"
 dependencies = [
- "bitflags 2.4.1",
+ "bitflags 2.5.0",
 ]
 
 [[package]]
 name = "gpu-allocator"
 version = "0.25.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6f56f6318968d03c18e1bcf4857ff88c61157e9da8e47c5f29055d60e1228884"
@@ -2724,30 +2733,30 @@
  "thiserror",
  "winapi",
  "windows",
 ]
 
 [[package]]
 name = "gpu-descriptor"
-version = "0.2.4"
+version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cc11df1ace8e7e564511f53af41f3e42ddc95b56fd07b3f4445d2a6048bc682c"
+checksum = "9c08c1f623a8d0b722b8b99f821eb0ba672a1618f0d3b16ddbee1cedd2dd8557"
 dependencies = [
- "bitflags 2.4.1",
+ "bitflags 2.5.0",
  "gpu-descriptor-types",
  "hashbrown 0.14.3",
 ]
 
 [[package]]
 name = "gpu-descriptor-types"
-version = "0.1.2"
+version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6bf0b36e6f090b7e1d8a4b49c0cb81c1f8376f72198c65dd3ad9ff3556b8b78c"
+checksum = "fdf242682df893b86f33a73828fb09ca4b2d3bb6cc95249707fc684d27484b91"
 dependencies = [
- "bitflags 2.4.1",
+ "bitflags 2.5.0",
 ]
 
 [[package]]
 name = "group"
 version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f0f9ef7462f7c099f518d754361858f86d8a07af53ba9af0fe635bbccb151a63"
@@ -2821,15 +2830,15 @@
 
 [[package]]
 name = "hassle-rs"
 version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "af2a7e73e1f34c48da31fb668a907f250794837e08faa144fd24f0b8b741e890"
 dependencies = [
- "bitflags 2.4.1",
+ "bitflags 2.5.0",
  "com",
  "libc",
  "libloading 0.8.1",
  "thiserror",
  "widestring",
  "winapi",
 ]
@@ -3477,15 +3486,15 @@
 
 [[package]]
 name = "libredox"
 version = "0.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3af92c55d7d839293953fcd0fda5ecfe93297cfde6ffbdec13b41d99c0ba6607"
 dependencies = [
- "bitflags 2.4.1",
+ "bitflags 2.5.0",
  "libc",
  "redox_syscall 0.4.1",
 ]
 
 [[package]]
 name = "libsqlite3-sys"
 version = "0.26.0"
@@ -3517,14 +3526,20 @@
 [[package]]
 name = "linux-raw-sys"
 version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c4cd1a83af159aa67994778be9070f0ae1bd732942279cabb14f86f986a21456"
 
 [[package]]
+name = "litrs"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b4ce301924b7887e9d637144fdade93f9dfff9b60981d4ac161db09720d39aa5"
+
+[[package]]
 name = "load_image"
 version = "3.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "20c73d7e075d05bdcc5ff4cf16b35b50b2be696b93c1be1b32201fb32c35a814"
 dependencies = [
  "bytemuck",
  "imgref",
@@ -3747,19 +3762,19 @@
 checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "metal"
-version = "0.27.0"
+version = "0.28.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c43f73953f8cbe511f021b58f18c3ce1c3d1ae13fe953293e13345bf83217f25"
+checksum = "5637e166ea14be6063a3f8ba5ccb9a4159df7d8f6d61c02fc3d480b1f90dcfcb"
 dependencies = [
- "bitflags 2.4.1",
+ "bitflags 2.5.0",
  "block",
  "core-graphics-types",
  "foreign-types 0.5.0",
  "log",
  "objc",
  "paste",
 ]
@@ -3808,20 +3823,21 @@
 name = "multimap"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5ce46fe64a9d73be07dcbe690a38ce1b293be448fd8ce1e6c1b8062c9f72c6a"
 
 [[package]]
 name = "naga"
-version = "0.19.2"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "50e3524642f53d9af419ab5e8dd29d3ba155708267667c2f3f06c88c9e130843"
+checksum = "e536ae46fcab0876853bd4a632ede5df4b1c2527a58f6c5a4150fe86be858231"
 dependencies = [
+ "arrayvec",
  "bit-set",
- "bitflags 2.4.1",
+ "bitflags 2.5.0",
  "codespan-reporting",
  "hexf-parse",
  "indexmap 2.2.5",
  "log",
  "num-traits",
  "rustc-hash",
  "spirv",
@@ -3850,15 +3866,15 @@
 
 [[package]]
 name = "ndk"
 version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2076a31b7010b17a38c01907c45b945e8f11495ee4dd588309718901b1f7a5b7"
 dependencies = [
- "bitflags 2.4.1",
+ "bitflags 2.5.0",
  "jni-sys",
  "log",
  "ndk-sys",
  "num_enum",
  "raw-window-handle",
  "thiserror",
 ]
@@ -4096,15 +4112,14 @@
 [[package]]
 name = "objc"
 version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "915b1b472bc21c53464d6c8461c9d3af805ba1ef837e1cac254428f4a77177b1"
 dependencies = [
  "malloc_buf",
- "objc_exception",
 ]
 
 [[package]]
 name = "objc-sys"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c7c71324e4180d0899963fc83d9d241ac39e699609fc1025a850aadac8257459"
@@ -4122,23 +4137,14 @@
 [[package]]
 name = "objc2-encode"
 version = "3.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d079845b37af429bfe5dfa76e6d087d788031045b25cfc6fd898486fd9847666"
 
 [[package]]
-name = "objc_exception"
-version = "0.1.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ad970fb455818ad6cba4c122ad012fae53ae8b4795f86378bce65e4f6bab2ca4"
-dependencies = [
- "cc",
-]
-
-[[package]]
 name = "object"
 version = "0.32.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9cf5f9dd3933bd50a9e1f149ec995f39ae2c496d31fd772c1fd45ebc27e902b0"
 dependencies = [
  "memchr",
 ]
@@ -4166,15 +4172,15 @@
 
 [[package]]
 name = "openssl"
 version = "0.10.62"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8cde4d2d9200ad5909f8dac647e29482e07c3a35de8a13fce7c9c7747ad9f671"
 dependencies = [
- "bitflags 2.4.1",
+ "bitflags 2.5.0",
  "cfg-if",
  "foreign-types 0.3.2",
  "libc",
  "once_cell",
  "openssl-macros",
  "openssl-sys",
 ]
@@ -5022,17 +5028,17 @@
 name = "relative-path"
 version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c707298afce11da2efef2f600116fa93ffa7a032b5d7b628aa17711ec81383ca"
 
 [[package]]
 name = "renderdoc-sys"
-version = "1.0.0"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "216080ab382b992234dda86873c18d4c48358f5cfcb70fd693d7f6f2131b628b"
+checksum = "19b30a45b0cd0bcca8037f3d0dc3421eaf95327a17cad11964fb8179b4fc4832"
 
 [[package]]
 name = "reqwest"
 version = "0.11.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "37b1ae8d9ac08420c66222fb9096fc5de435c3c48542bc5336c51892cffafb41"
 dependencies = [
@@ -5238,15 +5244,15 @@
 
 [[package]]
 name = "rusqlite"
 version = "0.29.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "549b9d036d571d42e6e85d1c1425e2ac83491075078ca9a15be021c56b1641f2"
 dependencies = [
- "bitflags 2.4.1",
+ "bitflags 2.5.0",
  "fallible-iterator",
  "fallible-streaming-iterator",
  "hashlink",
  "libsqlite3-sys",
  "smallvec",
 ]
 
@@ -5291,15 +5297,15 @@
 
 [[package]]
 name = "rustix"
 version = "0.38.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72e572a5e8ca657d7366229cdde4bd14c4eb5499a9573d4d366fe1b599daa316"
 dependencies = [
- "bitflags 2.4.1",
+ "bitflags 2.5.0",
  "errno 0.3.8",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
@@ -5380,15 +5386,15 @@
 
 [[package]]
 name = "rustybuzz"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f0ae5692c5beaad6a9e22830deeed7874eae8a4e3ba4076fb48e12c56856222c"
 dependencies = [
- "bitflags 2.4.1",
+ "bitflags 2.5.0",
  "bytemuck",
  "libm",
  "smallvec",
  "ttf-parser 0.20.0",
  "unicode-bidi-mirroring",
  "unicode-ccc",
  "unicode-properties",
@@ -5775,15 +5781,15 @@
 
 [[package]]
 name = "smithay-client-toolkit"
 version = "0.18.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "922fd3eeab3bd820d76537ce8f582b1cf951eceb5475c28500c7457d9d17f53a"
 dependencies = [
- "bitflags 2.4.1",
+ "bitflags 2.5.0",
  "calloop",
  "calloop-wayland-source",
  "cursor-icon",
  "libc",
  "log",
  "memmap2 0.9.4",
  "rustix",
@@ -5866,15 +5872,15 @@
 
 [[package]]
 name = "spirv"
 version = "0.3.0+sdk-1.3.268.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eda41003dc44290527a59b13432d4a0379379fa074b70174882adfbdfd917844"
 dependencies = [
- "bitflags 2.4.1",
+ "bitflags 2.5.0",
 ]
 
 [[package]]
 name = "spki"
 version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d91ed6c858b01f942cd56b37a94b3e0a1798290327d1236e4d9cf4eaca44d29d"
@@ -6103,15 +6109,15 @@
 
 [[package]]
 name = "swc_ecma_ast"
 version = "0.110.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2c3d416121da2d56bcbd1b1623725a68890af4552fef0c6d1e4bfa92776ccd6a"
 dependencies = [
- "bitflags 2.4.1",
+ "bitflags 2.5.0",
  "is-macro",
  "num-bigint",
  "phf",
  "scoped-tls",
  "serde",
  "string_enum",
  "swc_atoms",
@@ -6189,15 +6195,15 @@
 [[package]]
 name = "swc_ecma_transforms_base"
 version = "0.134.42"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d74ca42a400257d8563624122813c1849c3d87e7abe3b9b2ed7514c76f64ad2f"
 dependencies = [
  "better_scoped_tls",
- "bitflags 2.4.1",
+ "bitflags 2.5.0",
  "indexmap 1.9.3",
  "once_cell",
  "phf",
  "rustc-hash",
  "serde",
  "smallvec",
  "swc_atoms",
@@ -6525,26 +6531,26 @@
 checksum = "7fd5828de7deaa782e1dd713006ae96b3bee32d3279b79eb67ecf8072c059bcf"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.58"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
+checksum = "579e9083ca58dd9dcf91a9923bb9054071b9ebbd800b342194c9feb0ee89fc18"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.58"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
+checksum = "e2470041c06ec3ac1ab38d0356a6119054dedaea53e12fbefc0de730a1c08524"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.47",
 ]
 
 [[package]]
@@ -7446,27 +7452,27 @@
 
 [[package]]
 name = "wayland-client"
 version = "0.31.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "82fb96ee935c2cea6668ccb470fb7771f6215d1691746c2d896b447a00ad3f1f"
 dependencies = [
- "bitflags 2.4.1",
+ "bitflags 2.5.0",
  "rustix",
  "wayland-backend",
  "wayland-scanner",
 ]
 
 [[package]]
 name = "wayland-csd-frame"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "625c5029dbd43d25e6aa9615e88b829a5cad13b2819c4ae129fdbb7c31ab4c7e"
 dependencies = [
- "bitflags 2.4.1",
+ "bitflags 2.5.0",
  "cursor-icon",
  "wayland-backend",
 ]
 
 [[package]]
 name = "wayland-cursor"
 version = "0.31.1"
@@ -7480,40 +7486,40 @@
 
 [[package]]
 name = "wayland-protocols"
 version = "0.31.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f81f365b8b4a97f422ac0e8737c438024b5951734506b0e1d775c73030561f4"
 dependencies = [
- "bitflags 2.4.1",
+ "bitflags 2.5.0",
  "wayland-backend",
  "wayland-client",
  "wayland-scanner",
 ]
 
 [[package]]
 name = "wayland-protocols-plasma"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "23803551115ff9ea9bce586860c5c5a971e360825a0309264102a9495a5ff479"
 dependencies = [
- "bitflags 2.4.1",
+ "bitflags 2.5.0",
  "wayland-backend",
  "wayland-client",
  "wayland-protocols",
  "wayland-scanner",
 ]
 
 [[package]]
 name = "wayland-protocols-wlr"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ad1f61b76b6c2d8742e10f9ba5c3737f6530b4c243132c2a2ccc8aa96fe25cd6"
 dependencies = [
- "bitflags 2.4.1",
+ "bitflags 2.5.0",
  "wayland-backend",
  "wayland-client",
  "wayland-protocols",
  "wayland-scanner",
 ]
 
 [[package]]
@@ -7569,21 +7575,22 @@
 name = "weezl"
 version = "0.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9193164d4de03a926d909d3bc7c30543cecb35400c02114792c2cae20d5e2dbb"
 
 [[package]]
 name = "wgpu"
-version = "0.19.3"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a4b1213b52478a7631d6e387543ed8f642bc02c578ef4e3b49aca2a29a7df0cb"
+checksum = "32ff1bfee408e1028e2e3acbf6d32d98b08a5a059ccbf5f33305534453ba5d3e"
 dependencies = [
  "arrayvec",
  "cfg-if",
  "cfg_aliases",
+ "document-features",
  "js-sys",
  "log",
  "naga",
  "parking_lot 0.12.1",
  "profiling",
  "raw-window-handle",
  "smallvec",
@@ -7594,23 +7601,24 @@
  "wgpu-core",
  "wgpu-hal",
  "wgpu-types",
 ]
 
 [[package]]
 name = "wgpu-core"
-version = "0.19.3"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9f6b033c2f00ae0bc8ea872c5989777c60bc241aac4e58b24774faa8b391f78"
+checksum = "ac6a86eaa5e763e59c73cf9e97d55fffd4dfda69fd8bda19589fcf851ddfef1f"
 dependencies = [
  "arrayvec",
  "bit-vec",
- "bitflags 2.4.1",
+ "bitflags 2.5.0",
  "cfg_aliases",
  "codespan-reporting",
+ "document-features",
  "indexmap 2.2.5",
  "log",
  "naga",
  "once_cell",
  "parking_lot 0.12.1",
  "profiling",
  "raw-window-handle",
@@ -7620,23 +7628,23 @@
  "web-sys",
  "wgpu-hal",
  "wgpu-types",
 ]
 
 [[package]]
 name = "wgpu-hal"
-version = "0.19.3"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "49f972c280505ab52ffe17e94a7413d9d54b58af0114ab226b9fc4999a47082e"
+checksum = "4d71c8ae05170583049b65ee562fd839fdc0b3e9ddb84f4e40c9d5f8ea0d4c8c"
 dependencies = [
  "android_system_properties",
  "arrayvec",
  "ash",
  "bit-set",
- "bitflags 2.4.1",
+ "bitflags 2.5.0",
  "block",
  "cfg_aliases",
  "core-graphics-types",
  "d3d12",
  "glow",
  "glutin_wgl_sys",
  "gpu-alloc",
@@ -7665,19 +7673,19 @@
  "web-sys",
  "wgpu-types",
  "winapi",
 ]
 
 [[package]]
 name = "wgpu-types"
-version = "0.19.2"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b671ff9fb03f78b46ff176494ee1ebe7d603393f42664be55b64dc8d53969805"
+checksum = "1353d9a46bff7f955a680577f34c69122628cc2076e1d6f3a9be6ef00ae793ef"
 dependencies = [
- "bitflags 2.4.1",
+ "bitflags 2.5.0",
  "js-sys",
  "web-sys",
 ]
 
 [[package]]
 name = "which"
 version = "4.4.2"
@@ -7959,15 +7967,15 @@
 version = "0.29.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0d59ad965a635657faf09c8f062badd885748428933dad8e8bdd64064d92e5ca"
 dependencies = [
  "ahash",
  "android-activity",
  "atomic-waker",
- "bitflags 2.4.1",
+ "bitflags 2.5.0",
  "bytemuck",
  "calloop",
  "cfg_aliases",
  "core-foundation",
  "core-graphics",
  "cursor-icon",
  "icrate",
@@ -8099,15 +8107,15 @@
 
 [[package]]
 name = "xkbcommon-dl"
 version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d039de8032a9a8856a6be89cea3e5d12fdd82306ab7c94d74e6deab2460651c5"
 dependencies = [
- "bitflags 2.4.1",
+ "bitflags 2.5.0",
  "dlib",
  "log",
  "once_cell",
  "xkeysym",
 ]
 
 [[package]]
```

### Comparing `avenger-0.0.7/avenger/altair_utils.py` & `avenger-0.0.8/avenger/altair_utils.py`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/README.md` & `avenger-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/LICENSE` & `avenger-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `avenger-0.0.7/PKG-INFO` & `avenger-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: avenger
-Version: 0.0.7
+Version: 0.0.8
 License-File: LICENSE
 Summary: A Visualization Engine and Renderer
 License: BSD-3-Clause
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # Avenger: A visualization engine and renderer
 Avenger is an early stage prototype of a new foundational rendering library for information visualization (InfoVis) systems. Avenger defines a 2D scenegraph representation tailored to the needs of InfoVis systems. To start with, the initial application of Avenger is to serve as an alternative, GPU accelerated, rendering backend for Vega visualizations.
```

