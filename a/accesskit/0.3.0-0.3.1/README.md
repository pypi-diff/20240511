# Comparing `tmp/accesskit-0.3.0.tar.gz` & `tmp/accesskit-0.3.1.tar.gz`

## Comparing `accesskit-0.3.0.tar` & `accesskit-0.3.1.tar`

### file list

```diff
@@ -1,95 +1,95 @@
--rw-r--r--   0     1001      127     1294 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/unix/Cargo.toml
--rw-r--r--   0     1001      127    11392 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/unix/CHANGELOG.md
--rw-r--r--   0     1001      127      487 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/unix/README.md
--rw-r--r--   0     1001      127     6935 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/unix/src/adapter.rs
--rw-r--r--   0     1001      127    13572 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/unix/src/atspi/bus.rs
--rw-r--r--   0     1001      127     6053 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/unix/src/atspi/interfaces/accessible.rs
--rw-r--r--   0     1001      127     1473 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/unix/src/atspi/interfaces/action.rs
--rw-r--r--   0     1001      127     1096 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/unix/src/atspi/interfaces/application.rs
--rw-r--r--   0     1001      127     2195 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/unix/src/atspi/interfaces/component.rs
--rw-r--r--   0     1001      127      945 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/unix/src/atspi/interfaces/mod.rs
--rw-r--r--   0     1001      127     1459 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/unix/src/atspi/interfaces/value.rs
--rw-r--r--   0     1001      127      404 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/unix/src/atspi/mod.rs
--rw-r--r--   0     1001      127     1224 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/unix/src/atspi/object_address.rs
--rw-r--r--   0     1001      127     2185 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/unix/src/atspi/object_id.rs
--rw-r--r--   0     1001      127     8048 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/unix/src/context.rs
--rw-r--r--   0     1001      127     4885 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/unix/src/executor.rs
--rw-r--r--   0     1001      127     1005 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/unix/src/lib.rs
--rw-r--r--   0     1001      127     1389 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/unix/src/util.rs
--rw-r--r--   0     1001      127      956 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/windows/Cargo.toml
--rw-r--r--   0     1001      127    25318 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/windows/CHANGELOG.md
--rw-r--r--   0     1001      127      172 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/windows/README.md
--rw-r--r--   0     1001      127    11651 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/windows/examples/hello_world.rs
--rw-r--r--   0     1001      127    16519 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/windows/src/adapter.rs
--rw-r--r--   0     1001      127     1696 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/windows/src/context.rs
--rw-r--r--   0     1001      127      403 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/windows/src/filters.rs
--rw-r--r--   0     1001      127      482 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/windows/src/lib.rs
--rw-r--r--   0     1001      127    37537 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/windows/src/node.rs
--rw-r--r--   0     1001      127     6179 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/windows/src/subclass.rs
--rw-r--r--   0     1001      127    11438 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/windows/src/tests/mod.rs
--rw-r--r--   0     1001      127     6937 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/windows/src/tests/simple.rs
--rw-r--r--   0     1001      127     3536 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/windows/src/tests/subclassed.rs
--rw-r--r--   0     1001      127    19705 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/windows/src/text.rs
--rw-r--r--   0     1001      127     6500 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/windows/src/util.rs
--rw-r--r--   0     1001      127      705 2024-04-30 13:52:12.000000 accesskit-0.3.0/common/Cargo.toml
--rw-r--r--   0     1001      127    15163 2024-04-30 13:52:12.000000 accesskit-0.3.0/common/CHANGELOG.md
--rw-r--r--   0     1001      127      740 2024-04-30 13:52:12.000000 accesskit-0.3.0/common/README.md
--rw-r--r--   0     1001      127    22792 2024-04-30 13:52:12.000000 accesskit-0.3.0/common/src/geometry.rs
--rw-r--r--   0     1001      127    78839 2024-04-30 13:52:12.000000 accesskit-0.3.0/common/src/lib.rs
--rw-r--r--   0     1001      127      670 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/atspi-common/Cargo.toml
--rw-r--r--   0     1001      127     3246 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/atspi-common/CHANGELOG.md
--rw-r--r--   0     1001      127      317 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/atspi-common/README.md
--rw-r--r--   0     1001      127      432 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/atspi-common/src/action.rs
--rw-r--r--   0     1001      127    12747 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/atspi-common/src/adapter.rs
--rw-r--r--   0     1001      127      583 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/atspi-common/src/callback.rs
--rw-r--r--   0     1001      127     3414 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/atspi-common/src/context.rs
--rw-r--r--   0     1001      127      541 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/atspi-common/src/error.rs
--rw-r--r--   0     1001      127     1036 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/atspi-common/src/events.rs
--rw-r--r--   0     1001      127      334 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/atspi-common/src/filters.rs
--rw-r--r--   0     1001      127      753 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/atspi-common/src/lib.rs
--rw-r--r--   0     1001      127    39282 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/atspi-common/src/node.rs
--rw-r--r--   0     1001      127      898 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/atspi-common/src/rect.rs
--rw-r--r--   0     1001      127    13107 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/atspi-common/src/simplified.rs
--rw-r--r--   0     1001      127     1157 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/atspi-common/src/util.rs
--rw-r--r--   0     1001      127      942 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/macos/Cargo.toml
--rw-r--r--   0     1001      127    15387 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/macos/CHANGELOG.md
--rw-r--r--   0     1001      127      183 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/macos/README.md
--rw-r--r--   0     1001      127     9554 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/macos/src/adapter.rs
--rw-r--r--   0     1001      127     2731 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/macos/src/context.rs
--rw-r--r--   0     1001      127     9063 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/macos/src/event.rs
--rw-r--r--   0     1001      127      334 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/macos/src/filters.rs
--rw-r--r--   0     1001      127      557 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/macos/src/lib.rs
--rw-r--r--   0     1001      127    33624 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/macos/src/node.rs
--rw-r--r--   0     1001      127     3146 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/macos/src/patch.rs
--rw-r--r--   0     1001      127     9523 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/macos/src/subclass.rs
--rw-r--r--   0     1001      127     2819 2024-04-30 13:52:12.000000 accesskit-0.3.0/platforms/macos/src/util.rs
--rw-r--r--   0     1001      127      406 2024-04-30 13:52:12.000000 accesskit-0.3.0/consumer/Cargo.toml
--rw-r--r--   0     1001      127    17755 2024-04-30 13:52:12.000000 accesskit-0.3.0/consumer/CHANGELOG.md
--rw-r--r--   0     1001      127      207 2024-04-30 13:52:12.000000 accesskit-0.3.0/consumer/README.md
--rw-r--r--   0     1001      127     1262 2024-04-30 13:52:12.000000 accesskit-0.3.0/consumer/src/filters.rs
--rw-r--r--   0     1001      127    24021 2024-04-30 13:52:12.000000 accesskit-0.3.0/consumer/src/iterators.rs
--rw-r--r--   0     1001      127     6115 2024-04-30 13:52:12.000000 accesskit-0.3.0/consumer/src/lib.rs
--rw-r--r--   0     1001      127    33886 2024-04-30 13:52:12.000000 accesskit-0.3.0/consumer/src/node.rs
--rw-r--r--   0     1001      127    64423 2024-04-30 13:52:12.000000 accesskit-0.3.0/consumer/src/text.rs
--rw-r--r--   0     1001      127    26521 2024-04-30 13:52:12.000000 accesskit-0.3.0/consumer/src/tree.rs
--rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 accesskit-0.3.0/bindings/python/Cargo.toml
--rw-r--r--   0     1001      127      224 2024-04-30 13:52:12.000000 accesskit-0.3.0/bindings/python/.cargo/config.toml
--rw-r--r--   0     1001      127     4763 2024-04-30 13:52:12.000000 accesskit-0.3.0/bindings/python/CHANGELOG.md
--rw-r--r--   0     1001      127      981 2024-04-30 13:52:12.000000 accesskit-0.3.0/bindings/python/README.md
--rw-r--r--   0     1001      127     3078 2024-04-30 13:52:12.000000 accesskit-0.3.0/bindings/python/examples/pygame/.gitignore
--rw-r--r--   0     1001      127      367 2024-04-30 13:52:12.000000 accesskit-0.3.0/bindings/python/examples/pygame/README.md
--rw-r--r--   0     1001      127     6979 2024-04-30 13:52:12.000000 accesskit-0.3.0/bindings/python/examples/pygame/hello_world.py
--rw-r--r--   0     1001      127       24 2024-04-30 13:52:12.000000 accesskit-0.3.0/bindings/python/examples/pygame/requirements.txt
--rw-r--r--   0     1001      127    24054 2024-04-30 13:52:12.000000 accesskit-0.3.0/bindings/python/src/common.rs
--rw-r--r--   0     1001      127     4784 2024-04-30 13:52:12.000000 accesskit-0.3.0/bindings/python/src/geometry.rs
--rw-r--r--   0     1001      127     2818 2024-04-30 13:52:12.000000 accesskit-0.3.0/bindings/python/src/lib.rs
--rw-r--r--   0     1001      127     7316 2024-04-30 13:52:12.000000 accesskit-0.3.0/bindings/python/src/macos.rs
--rw-r--r--   0     1001      127     1506 2024-04-30 13:52:12.000000 accesskit-0.3.0/bindings/python/src/unix.rs
--rw-r--r--   0     1001      127     4126 2024-04-30 13:52:12.000000 accesskit-0.3.0/bindings/python/src/windows.rs
--rw-r--r--   0     1001      127    73406 2024-04-30 13:52:12.000000 accesskit-0.3.0/Cargo.lock
--rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 accesskit-0.3.0/Cargo.toml
--rw-r--r--   0     1001      127     1043 2024-04-30 13:52:12.000000 accesskit-0.3.0/pyproject.toml
--rw-r--r--   0     1001      127     9723 2024-04-30 13:52:12.000000 accesskit-0.3.0/LICENSE-APACHE
--rw-r--r--   0     1001      127     1023 2024-04-30 13:52:12.000000 accesskit-0.3.0/LICENSE-MIT
--rw-r--r--   0     1001      127     1559 2024-04-30 13:52:12.000000 accesskit-0.3.0/LICENSE.chromium
--rw-r--r--   0        0        0     1958 1970-01-01 00:00:00.000000 accesskit-0.3.0/PKG-INFO
+-rw-r--r--   0     1001      127     1294 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/unix/Cargo.toml
+-rw-r--r--   0     1001      127    11518 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/unix/CHANGELOG.md
+-rw-r--r--   0     1001      127      487 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/unix/README.md
+-rw-r--r--   0     1001      127     6935 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/unix/src/adapter.rs
+-rw-r--r--   0     1001      127    13572 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/unix/src/atspi/bus.rs
+-rw-r--r--   0     1001      127     6053 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/unix/src/atspi/interfaces/accessible.rs
+-rw-r--r--   0     1001      127     1473 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/unix/src/atspi/interfaces/action.rs
+-rw-r--r--   0     1001      127     1096 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/unix/src/atspi/interfaces/application.rs
+-rw-r--r--   0     1001      127     2195 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/unix/src/atspi/interfaces/component.rs
+-rw-r--r--   0     1001      127      945 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/unix/src/atspi/interfaces/mod.rs
+-rw-r--r--   0     1001      127     1459 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/unix/src/atspi/interfaces/value.rs
+-rw-r--r--   0     1001      127      404 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/unix/src/atspi/mod.rs
+-rw-r--r--   0     1001      127     1224 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/unix/src/atspi/object_address.rs
+-rw-r--r--   0     1001      127     2185 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/unix/src/atspi/object_id.rs
+-rw-r--r--   0     1001      127     8048 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/unix/src/context.rs
+-rw-r--r--   0     1001      127     4885 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/unix/src/executor.rs
+-rw-r--r--   0     1001      127     1005 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/unix/src/lib.rs
+-rw-r--r--   0     1001      127     1389 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/unix/src/util.rs
+-rw-r--r--   0     1001      127      670 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/atspi-common/Cargo.toml
+-rw-r--r--   0     1001      127     3370 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/atspi-common/CHANGELOG.md
+-rw-r--r--   0     1001      127      317 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/atspi-common/README.md
+-rw-r--r--   0     1001      127      432 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/atspi-common/src/action.rs
+-rw-r--r--   0     1001      127    12747 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/atspi-common/src/adapter.rs
+-rw-r--r--   0     1001      127      583 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/atspi-common/src/callback.rs
+-rw-r--r--   0     1001      127     3414 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/atspi-common/src/context.rs
+-rw-r--r--   0     1001      127      541 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/atspi-common/src/error.rs
+-rw-r--r--   0     1001      127     1036 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/atspi-common/src/events.rs
+-rw-r--r--   0     1001      127      334 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/atspi-common/src/filters.rs
+-rw-r--r--   0     1001      127      753 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/atspi-common/src/lib.rs
+-rw-r--r--   0     1001      127    39324 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/atspi-common/src/node.rs
+-rw-r--r--   0     1001      127      898 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/atspi-common/src/rect.rs
+-rw-r--r--   0     1001      127    13107 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/atspi-common/src/simplified.rs
+-rw-r--r--   0     1001      127     1157 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/atspi-common/src/util.rs
+-rw-r--r--   0     1001      127      705 2024-05-11 16:09:37.000000 accesskit-0.3.1/common/Cargo.toml
+-rw-r--r--   0     1001      127    15163 2024-05-11 16:09:37.000000 accesskit-0.3.1/common/CHANGELOG.md
+-rw-r--r--   0     1001      127      740 2024-05-11 16:09:37.000000 accesskit-0.3.1/common/README.md
+-rw-r--r--   0     1001      127    22792 2024-05-11 16:09:37.000000 accesskit-0.3.1/common/src/geometry.rs
+-rw-r--r--   0     1001      127    78839 2024-05-11 16:09:37.000000 accesskit-0.3.1/common/src/lib.rs
+-rw-r--r--   0     1001      127      942 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/macos/Cargo.toml
+-rw-r--r--   0     1001      127    15511 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/macos/CHANGELOG.md
+-rw-r--r--   0     1001      127      183 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/macos/README.md
+-rw-r--r--   0     1001      127     9554 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/macos/src/adapter.rs
+-rw-r--r--   0     1001      127     2731 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/macos/src/context.rs
+-rw-r--r--   0     1001      127     9063 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/macos/src/event.rs
+-rw-r--r--   0     1001      127      334 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/macos/src/filters.rs
+-rw-r--r--   0     1001      127      557 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/macos/src/lib.rs
+-rw-r--r--   0     1001      127    33624 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/macos/src/node.rs
+-rw-r--r--   0     1001      127     3146 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/macos/src/patch.rs
+-rw-r--r--   0     1001      127     9523 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/macos/src/subclass.rs
+-rw-r--r--   0     1001      127     2819 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/macos/src/util.rs
+-rw-r--r--   0     1001      127      956 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/windows/Cargo.toml
+-rw-r--r--   0     1001      127    25830 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/windows/CHANGELOG.md
+-rw-r--r--   0     1001      127      172 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/windows/README.md
+-rw-r--r--   0     1001      127    11651 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/windows/examples/hello_world.rs
+-rw-r--r--   0     1001      127    15926 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/windows/src/adapter.rs
+-rw-r--r--   0     1001      127     1850 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/windows/src/context.rs
+-rw-r--r--   0     1001      127      403 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/windows/src/filters.rs
+-rw-r--r--   0     1001      127      482 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/windows/src/lib.rs
+-rw-r--r--   0     1001      127    38489 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/windows/src/node.rs
+-rw-r--r--   0     1001      127     6179 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/windows/src/subclass.rs
+-rw-r--r--   0     1001      127    11438 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/windows/src/tests/mod.rs
+-rw-r--r--   0     1001      127     6937 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/windows/src/tests/simple.rs
+-rw-r--r--   0     1001      127     3536 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/windows/src/tests/subclassed.rs
+-rw-r--r--   0     1001      127    19711 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/windows/src/text.rs
+-rw-r--r--   0     1001      127     6500 2024-05-11 16:09:37.000000 accesskit-0.3.1/platforms/windows/src/util.rs
+-rw-r--r--   0     1001      127      406 2024-05-11 16:09:37.000000 accesskit-0.3.1/consumer/Cargo.toml
+-rw-r--r--   0     1001      127    18087 2024-05-11 16:09:37.000000 accesskit-0.3.1/consumer/CHANGELOG.md
+-rw-r--r--   0     1001      127      207 2024-05-11 16:09:37.000000 accesskit-0.3.1/consumer/README.md
+-rw-r--r--   0     1001      127     1262 2024-05-11 16:09:37.000000 accesskit-0.3.1/consumer/src/filters.rs
+-rw-r--r--   0     1001      127    24021 2024-05-11 16:09:37.000000 accesskit-0.3.1/consumer/src/iterators.rs
+-rw-r--r--   0     1001      127     6115 2024-05-11 16:09:37.000000 accesskit-0.3.1/consumer/src/lib.rs
+-rw-r--r--   0     1001      127    33886 2024-05-11 16:09:37.000000 accesskit-0.3.1/consumer/src/node.rs
+-rw-r--r--   0     1001      127    64423 2024-05-11 16:09:37.000000 accesskit-0.3.1/consumer/src/text.rs
+-rw-r--r--   0     1001      127    27978 2024-05-11 16:09:37.000000 accesskit-0.3.1/consumer/src/tree.rs
+-rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 accesskit-0.3.1/bindings/python/Cargo.toml
+-rw-r--r--   0     1001      127      224 2024-05-11 16:09:37.000000 accesskit-0.3.1/bindings/python/.cargo/config.toml
+-rw-r--r--   0     1001      127     5346 2024-05-11 16:09:37.000000 accesskit-0.3.1/bindings/python/CHANGELOG.md
+-rw-r--r--   0     1001      127      981 2024-05-11 16:09:37.000000 accesskit-0.3.1/bindings/python/README.md
+-rw-r--r--   0     1001      127     3078 2024-05-11 16:09:37.000000 accesskit-0.3.1/bindings/python/examples/pygame/.gitignore
+-rw-r--r--   0     1001      127      367 2024-05-11 16:09:37.000000 accesskit-0.3.1/bindings/python/examples/pygame/README.md
+-rw-r--r--   0     1001      127     6979 2024-05-11 16:09:37.000000 accesskit-0.3.1/bindings/python/examples/pygame/hello_world.py
+-rw-r--r--   0     1001      127       24 2024-05-11 16:09:37.000000 accesskit-0.3.1/bindings/python/examples/pygame/requirements.txt
+-rw-r--r--   0     1001      127    24191 2024-05-11 16:09:37.000000 accesskit-0.3.1/bindings/python/src/common.rs
+-rw-r--r--   0     1001      127     4784 2024-05-11 16:09:37.000000 accesskit-0.3.1/bindings/python/src/geometry.rs
+-rw-r--r--   0     1001      127     2818 2024-05-11 16:09:37.000000 accesskit-0.3.1/bindings/python/src/lib.rs
+-rw-r--r--   0     1001      127     7316 2024-05-11 16:09:37.000000 accesskit-0.3.1/bindings/python/src/macos.rs
+-rw-r--r--   0     1001      127     1506 2024-05-11 16:09:37.000000 accesskit-0.3.1/bindings/python/src/unix.rs
+-rw-r--r--   0     1001      127     4126 2024-05-11 16:09:37.000000 accesskit-0.3.1/bindings/python/src/windows.rs
+-rw-r--r--   0     1001      127    73407 2024-05-11 16:09:37.000000 accesskit-0.3.1/Cargo.lock
+-rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 accesskit-0.3.1/Cargo.toml
+-rw-r--r--   0     1001      127     1043 2024-05-11 16:09:37.000000 accesskit-0.3.1/pyproject.toml
+-rw-r--r--   0     1001      127     9723 2024-05-11 16:09:37.000000 accesskit-0.3.1/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1023 2024-05-11 16:09:37.000000 accesskit-0.3.1/LICENSE-MIT
+-rw-r--r--   0     1001      127     1559 2024-05-11 16:09:37.000000 accesskit-0.3.1/LICENSE.chromium
+-rw-r--r--   0        0        0     1958 1970-01-01 00:00:00.000000 accesskit-0.3.1/PKG-INFO
```

### Comparing `accesskit-0.3.0/platforms/unix/Cargo.toml` & `accesskit-0.3.1/platforms/unix/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "accesskit_unix"
-version = "0.9.0"
+version = "0.9.1"
 authors.workspace = true
 license.workspace = true
 description = "AccessKit UI accessibility infrastructure: Linux adapter"
 categories.workspace = true
 keywords = ["gui", "ui", "accessibility"]
 repository.workspace = true
 readme = "README.md"
@@ -14,15 +14,15 @@
 [features]
 default = ["async-io"]
 async-io = ["dep:async-channel", "dep:async-executor", "dep:async-task", "dep:futures-util", "atspi/async-std", "zbus/async-io"]
 tokio = ["dep:tokio", "dep:tokio-stream", "atspi/tokio", "zbus/tokio"]
 
 [dependencies]
 accesskit = { version = "0.14.0", path = "../../common" }
-accesskit_atspi_common = { version = "0.4.0", path = "../atspi-common" }
+accesskit_atspi_common = { version = "0.4.1", path = "../atspi-common" }
 atspi = { version = "0.19", default-features = false }
 futures-lite = "1.13"
 serde = "1.0"
 zbus = { version = "3.14", default-features = false }
 
 # async-io support
 async-channel = { version = "2.1.1", optional = true }
```

### Comparing `accesskit-0.3.0/platforms/unix/CHANGELOG.md` & `accesskit-0.3.1/platforms/unix/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,18 @@
     * accesskit bumped from 0.12.2 to 0.12.3
     * accesskit_atspi_common bumped from 0.1.1 to 0.1.2
 
 * The following workspace dependencies were updated
   * dependencies
     * accesskit_atspi_common bumped from 0.1.2 to 0.2.0
 
+* The following workspace dependencies were updated
+  * dependencies
+    * accesskit_atspi_common bumped from 0.4.0 to 0.4.1
+
 ## [0.9.0](https://github.com/AccessKit/accesskit/compare/accesskit_unix-v0.8.0...accesskit_unix-v0.9.0) (2024-04-30)
 
 
 ### ⚠ BREAKING CHANGES
 
 * Force a semver-breaking release ([#398](https://github.com/AccessKit/accesskit/issues/398))
```

### Comparing `accesskit-0.3.0/platforms/unix/src/adapter.rs` & `accesskit-0.3.1/platforms/unix/src/adapter.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/platforms/unix/src/atspi/bus.rs` & `accesskit-0.3.1/platforms/unix/src/atspi/bus.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/platforms/unix/src/atspi/interfaces/accessible.rs` & `accesskit-0.3.1/platforms/unix/src/atspi/interfaces/accessible.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/platforms/unix/src/atspi/interfaces/action.rs` & `accesskit-0.3.1/platforms/unix/src/atspi/interfaces/action.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/platforms/unix/src/atspi/interfaces/application.rs` & `accesskit-0.3.1/platforms/unix/src/atspi/interfaces/application.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/platforms/unix/src/atspi/interfaces/component.rs` & `accesskit-0.3.1/platforms/unix/src/atspi/interfaces/component.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/platforms/unix/src/atspi/interfaces/mod.rs` & `accesskit-0.3.1/platforms/unix/src/atspi/interfaces/mod.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/platforms/unix/src/atspi/interfaces/value.rs` & `accesskit-0.3.1/platforms/unix/src/atspi/interfaces/value.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/platforms/unix/src/atspi/object_address.rs` & `accesskit-0.3.1/platforms/unix/src/atspi/object_address.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/platforms/unix/src/atspi/object_id.rs` & `accesskit-0.3.1/platforms/unix/src/atspi/object_id.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/platforms/unix/src/context.rs` & `accesskit-0.3.1/platforms/unix/src/context.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/platforms/unix/src/executor.rs` & `accesskit-0.3.1/platforms/unix/src/executor.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/platforms/unix/src/lib.rs` & `accesskit-0.3.1/platforms/unix/src/lib.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/platforms/unix/src/util.rs` & `accesskit-0.3.1/platforms/unix/src/util.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/platforms/windows/Cargo.toml` & `accesskit-0.3.1/platforms/windows/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [package]
 name = "accesskit_windows"
-version = "0.18.0"
+version = "0.18.1"
 authors.workspace = true
 license.workspace = true
 description = "AccessKit UI accessibility infrastructure: Windows adapter"
 categories.workspace = true
 keywords = ["gui", "ui", "accessibility"]
 repository.workspace = true
 readme = "README.md"
 edition.workspace = true
 rust-version.workspace = true
 
 [dependencies]
 accesskit = { version = "0.14.0", path = "../../common" }
-accesskit_consumer = { version = "0.19.0", path = "../../consumer" }
+accesskit_consumer = { version = "0.19.1", path = "../../consumer" }
 paste = "1.0"
 static_assertions = "1.1.0"
 
 [dependencies.windows]
 version = "0.54"
 features = [
     "implement",
```

### Comparing `accesskit-0.3.0/platforms/windows/CHANGELOG.md` & `accesskit-0.3.1/platforms/windows/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,28 @@
     * accesskit_consumer bumped from 0.15.1 to 0.15.2
 
 * The following workspace dependencies were updated
   * dependencies
     * accesskit bumped from 0.12.2 to 0.12.3
     * accesskit_consumer bumped from 0.17.0 to 0.17.1
 
+## [0.18.1](https://github.com/AccessKit/accesskit/compare/accesskit_windows-v0.18.0...accesskit_windows-v0.18.1) (2024-05-11)
+
+
+### Bug Fixes
+
+* Make the transition from placeholder to real tree more robust ([#405](https://github.com/AccessKit/accesskit/issues/405)) ([928e11d](https://github.com/AccessKit/accesskit/commit/928e11d00e7c60b3cafcc0ac623f6377b36f7ea7))
+
+
+### Dependencies
+
+* The following workspace dependencies were updated
+  * dependencies
+    * accesskit_consumer bumped from 0.19.0 to 0.19.1
+
 ## [0.18.0](https://github.com/AccessKit/accesskit/compare/accesskit_windows-v0.17.0...accesskit_windows-v0.18.0) (2024-04-30)
 
 
 ### ⚠ BREAKING CHANGES
 
 * Update winit to 0.30 ([#397](https://github.com/AccessKit/accesskit/issues/397))
 * Clean up table roles and properties ([#393](https://github.com/AccessKit/accesskit/issues/393))
```

### Comparing `accesskit-0.3.0/platforms/windows/examples/hello_world.rs` & `accesskit-0.3.1/platforms/windows/examples/hello_world.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/platforms/windows/src/adapter.rs` & `accesskit-0.3.1/platforms/windows/src/adapter.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 // Copyright 2022 The AccessKit Authors. All rights reserved.
 // Licensed under the Apache License, Version 2.0 (found in
 // the LICENSE-APACHE file) or the MIT license (found in
 // the LICENSE-MIT file), at your option.
 
 use accesskit::{
-    ActionHandler, ActionRequest, ActivationHandler, Live, NodeBuilder, NodeId, Role,
-    Tree as TreeData, TreeUpdate,
+    ActionHandler, ActivationHandler, Live, NodeBuilder, NodeId, Role, Tree as TreeData, TreeUpdate,
 };
 use accesskit_consumer::{DetachedNode, FilterResult, Node, Tree, TreeChangeHandler, TreeState};
-use std::{collections::HashSet, sync::Arc};
+use std::{
+    collections::HashSet,
+    sync::{atomic::Ordering, Arc},
+};
 use windows::Win32::{
     Foundation::*,
     UI::{Accessibility::*, WindowsAndMessaging::*},
 };
 
 use crate::{
     context::{ActionHandlerNoMut, ActionHandlerWrapper, Context},
@@ -158,28 +160,18 @@
 
 enum State {
     Inactive {
         hwnd: HWND,
         is_window_focused: bool,
         action_handler: Arc<dyn ActionHandlerNoMut + Send + Sync>,
     },
-    Placeholder {
-        placeholder_context: Arc<Context>,
-        is_window_focused: bool,
-        action_handler: Arc<dyn ActionHandlerNoMut + Send + Sync>,
-    },
+    Placeholder(Arc<Context>),
     Active(Arc<Context>),
 }
 
-struct PlaceholderActionHandler;
-
-impl ActionHandler for PlaceholderActionHandler {
-    fn do_action(&mut self, _request: ActionRequest) {}
-}
-
 pub struct Adapter {
     state: State,
 }
 
 impl Adapter {
     /// Creates a new Windows platform adapter.
     ///
@@ -235,28 +227,25 @@
     /// it should be called.
     pub fn update_if_active(
         &mut self,
         update_factory: impl FnOnce() -> TreeUpdate,
     ) -> Option<QueuedEvents> {
         match &self.state {
             State::Inactive { .. } => None,
-            State::Placeholder {
-                placeholder_context,
-                is_window_focused,
-                action_handler,
-            } => {
-                let tree = Tree::new(update_factory(), *is_window_focused);
-                let context =
-                    Context::new(placeholder_context.hwnd, tree, Arc::clone(action_handler));
+            State::Placeholder(context) => {
+                let is_window_focused = context.read_tree().state().is_host_focused();
+                let tree = Tree::new(update_factory(), is_window_focused);
+                *context.tree.write().unwrap() = tree;
+                context.is_placeholder.store(false, Ordering::SeqCst);
                 let result = context
                     .read_tree()
                     .state()
                     .focus_id()
-                    .map(|id| QueuedEvents(vec![focus_event(&context, id)]));
-                self.state = State::Active(context);
+                    .map(|id| QueuedEvents(vec![focus_event(context, id)]));
+                self.state = State::Active(Arc::clone(context));
                 result
             }
             State::Active(context) => {
                 let mut handler = AdapterChangeHandler::new(context);
                 let mut tree = context.tree.write().unwrap();
                 tree.update_and_process_changes(update_factory(), &mut handler);
                 Some(QueuedEvents(handler.queue))
@@ -276,19 +265,19 @@
         match &mut self.state {
             State::Inactive {
                 is_window_focused, ..
             } => {
                 *is_window_focused = is_focused;
                 None
             }
-            State::Placeholder {
-                is_window_focused, ..
-            } => {
-                *is_window_focused = is_focused;
-                None
+            State::Placeholder(context) => {
+                let mut handler = AdapterChangeHandler::new(context);
+                let mut tree = context.tree.write().unwrap();
+                tree.update_host_focus_state_and_process_changes(is_focused, &mut handler);
+                Some(QueuedEvents(handler.queue))
             }
             State::Active(context) => {
                 let mut handler = AdapterChangeHandler::new(context);
                 let mut tree = context.tree.write().unwrap();
                 tree.update_host_focus_state_and_process_changes(is_focused, &mut handler);
                 Some(QueuedEvents(handler.queue))
             }
@@ -326,50 +315,36 @@
                 hwnd,
                 is_window_focused,
                 action_handler,
             } => match activation_handler.request_initial_tree() {
                 Some(initial_state) => {
                     let hwnd = *hwnd;
                     let tree = Tree::new(initial_state, *is_window_focused);
-                    let context = Context::new(hwnd, tree, Arc::clone(action_handler));
+                    let context = Context::new(hwnd, tree, Arc::clone(action_handler), false);
                     let node_id = context.read_tree().state().root_id();
                     let platform_node = PlatformNode::new(&context, node_id);
                     self.state = State::Active(context);
                     (hwnd, platform_node)
                 }
                 None => {
                     let hwnd = *hwnd;
                     let placeholder_update = TreeUpdate {
                         nodes: vec![(PLACEHOLDER_ROOT_ID, NodeBuilder::new(Role::Window).build())],
                         tree: Some(TreeData::new(PLACEHOLDER_ROOT_ID)),
                         focus: PLACEHOLDER_ROOT_ID,
                     };
-                    let placeholder_tree = Tree::new(placeholder_update, false);
-                    let placeholder_context = Context::new(
-                        hwnd,
-                        placeholder_tree,
-                        Arc::new(ActionHandlerWrapper::new(PlaceholderActionHandler {})),
-                    );
-                    let platform_node =
-                        PlatformNode::new(&placeholder_context, PLACEHOLDER_ROOT_ID);
-                    self.state = State::Placeholder {
-                        placeholder_context,
-                        is_window_focused: *is_window_focused,
-                        action_handler: Arc::clone(action_handler),
-                    };
+                    let placeholder_tree = Tree::new(placeholder_update, *is_window_focused);
+                    let context =
+                        Context::new(hwnd, placeholder_tree, Arc::clone(action_handler), true);
+                    let platform_node = PlatformNode::unspecified_root(&context);
+                    self.state = State::Placeholder(context);
                     (hwnd, platform_node)
                 }
             },
-            State::Placeholder {
-                placeholder_context,
-                ..
-            } => (
-                placeholder_context.hwnd,
-                PlatformNode::new(placeholder_context, PLACEHOLDER_ROOT_ID),
-            ),
+            State::Placeholder(context) => (context.hwnd, PlatformNode::unspecified_root(context)),
             State::Active(context) => {
                 let node_id = context.read_tree().state().root_id();
                 (context.hwnd, PlatformNode::new(context, node_id))
             }
         };
         let el: IRawElementProviderSimple = platform_node.into();
         Some(WmGetObjectResult {
```

### Comparing `accesskit-0.3.0/platforms/windows/src/context.rs` & `accesskit-0.3.1/platforms/windows/src/context.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 // Copyright 2023 The AccessKit Authors. All rights reserved.
 // Licensed under the Apache License, Version 2.0 (found in
 // the LICENSE-APACHE file) or the MIT license (found in
 // the LICENSE-MIT file), at your option.
 
 use accesskit::{ActionHandler, ActionRequest, Point};
 use accesskit_consumer::Tree;
-use std::sync::{Arc, Mutex, RwLock, RwLockReadGuard};
+use std::sync::{atomic::AtomicBool, Arc, Mutex, RwLock, RwLockReadGuard};
 use windows::Win32::Foundation::*;
 
 use crate::util::*;
 
 pub(crate) trait ActionHandlerNoMut {
     fn do_action(&self, request: ActionRequest);
 }
@@ -28,26 +28,29 @@
     }
 }
 
 pub(crate) struct Context {
     pub(crate) hwnd: HWND,
     pub(crate) tree: RwLock<Tree>,
     pub(crate) action_handler: Arc<dyn ActionHandlerNoMut + Send + Sync>,
+    pub(crate) is_placeholder: AtomicBool,
 }
 
 impl Context {
     pub(crate) fn new(
         hwnd: HWND,
         tree: Tree,
         action_handler: Arc<dyn ActionHandlerNoMut + Send + Sync>,
+        is_placeholder: bool,
     ) -> Arc<Self> {
         Arc::new(Self {
             hwnd,
             tree: RwLock::new(tree),
             action_handler,
+            is_placeholder: AtomicBool::new(is_placeholder),
         })
     }
 
     pub(crate) fn read_tree(&self) -> RwLockReadGuard<'_, Tree> {
         self.tree.read().unwrap()
     }
```

### Comparing `accesskit-0.3.0/platforms/windows/src/node.rs` & `accesskit-0.3.1/platforms/windows/src/node.rs`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #![allow(non_upper_case_globals)]
 
 use accesskit::{
     Action, ActionData, ActionRequest, Live, NodeId, NodeIdContent, Point, Role, Toggled,
 };
 use accesskit_consumer::{DetachedNode, FilterResult, Node, NodeState, TreeState};
 use paste::paste;
-use std::sync::{Arc, Weak};
+use std::sync::{atomic::Ordering, Arc, Weak};
 use windows::{
     core::*,
     Win32::{Foundation::*, System::Com::*, UI::Accessibility::*},
 };
 
 use crate::{
     context::Context,
@@ -488,22 +488,29 @@
     IValueProvider,
     IRangeValueProvider,
     ISelectionItemProvider,
     ITextProvider
 )]
 pub(crate) struct PlatformNode {
     pub(crate) context: Weak<Context>,
-    pub(crate) node_id: NodeId,
+    pub(crate) node_id: Option<NodeId>,
 }
 
 impl PlatformNode {
     pub(crate) fn new(context: &Arc<Context>, node_id: NodeId) -> Self {
         Self {
             context: Arc::downgrade(context),
-            node_id,
+            node_id: Some(node_id),
+        }
+    }
+
+    pub(crate) fn unspecified_root(context: &Arc<Context>) -> Self {
+        Self {
+            context: Arc::downgrade(context),
+            node_id: None,
         }
     }
 
     fn upgrade_context(&self) -> Result<Arc<Context>> {
         upgrade(&self.context)
     }
 
@@ -519,37 +526,43 @@
     fn with_tree_state<F, T>(&self, f: F) -> Result<T>
     where
         F: FnOnce(&TreeState) -> Result<T>,
     {
         self.with_tree_state_and_context(|state, _| f(state))
     }
 
+    fn node<'a>(&self, state: &'a TreeState) -> Result<Node<'a>> {
+        if let Some(id) = self.node_id {
+            if let Some(node) = state.node_by_id(id) {
+                Ok(node)
+            } else {
+                Err(element_not_available())
+            }
+        } else {
+            Ok(state.root())
+        }
+    }
+
     fn resolve_with_context<F, T>(&self, f: F) -> Result<T>
     where
         for<'a> F: FnOnce(Node<'a>, &Context) -> Result<T>,
     {
         self.with_tree_state_and_context(|state, context| {
-            if let Some(node) = state.node_by_id(self.node_id) {
-                f(node, context)
-            } else {
-                Err(element_not_available())
-            }
+            let node = self.node(state)?;
+            f(node, context)
         })
     }
 
     fn resolve_with_tree_state_and_context<F, T>(&self, f: F) -> Result<T>
     where
         for<'a> F: FnOnce(Node<'a>, &TreeState, &Context) -> Result<T>,
     {
         self.with_tree_state_and_context(|state, context| {
-            if let Some(node) = state.node_by_id(self.node_id) {
-                f(node, state, context)
-            } else {
-                Err(element_not_available())
-            }
+            let node = self.node(state)?;
+            f(node, state, context)
         })
     }
 
     fn resolve<F, T>(&self, f: F) -> Result<T>
     where
         for<'a> F: FnOnce(Node<'a>) -> Result<T>,
     {
@@ -557,18 +570,16 @@
     }
 
     fn resolve_with_context_for_text_pattern<F, T>(&self, f: F) -> Result<T>
     where
         for<'a> F: FnOnce(Node<'a>, &Context) -> Result<T>,
     {
         self.with_tree_state_and_context(|state, context| {
-            if let Some(node) = state
-                .node_by_id(self.node_id)
-                .filter(Node::supports_text_ranges)
-            {
+            let node = self.node(state)?;
+            if node.supports_text_ranges() {
                 f(node, context)
             } else {
                 Err(element_not_available())
             }
         })
     }
 
@@ -577,42 +588,54 @@
         for<'a> F: FnOnce(Node<'a>) -> Result<T>,
     {
         self.resolve_with_context_for_text_pattern(|node, _| f(node))
     }
 
     fn do_action<F>(&self, f: F) -> Result<()>
     where
-        F: FnOnce() -> ActionRequest,
+        F: FnOnce() -> (Action, Option<ActionData>),
     {
         let context = self.upgrade_context()?;
+        if context.is_placeholder.load(Ordering::SeqCst) {
+            return Ok(());
+        }
         let tree = context.read_tree();
-        if tree.state().has_node(self.node_id) {
-            drop(tree);
-            let request = f();
-            context.do_action(request);
-            Ok(())
+        let node_id = if let Some(id) = self.node_id {
+            if !tree.state().has_node(id) {
+                return Err(element_not_available());
+            }
+            id
         } else {
-            Err(element_not_available())
-        }
+            tree.state().root_id()
+        };
+        drop(tree);
+        let (action, data) = f();
+        let request = ActionRequest {
+            target: node_id,
+            action,
+            data,
+        };
+        context.do_action(request);
+        Ok(())
     }
 
     fn do_default_action(&self) -> Result<()> {
-        self.do_action(|| ActionRequest {
-            action: Action::Default,
-            target: self.node_id,
-            data: None,
-        })
+        self.do_action(|| (Action::Default, None))
     }
 
     fn relative(&self, node_id: NodeId) -> Self {
         Self {
             context: self.context.clone(),
-            node_id,
+            node_id: Some(node_id),
         }
     }
+
+    fn is_root(&self, state: &TreeState) -> bool {
+        self.node_id.map_or(false, |id| id == state.root_id())
+    }
 }
 
 #[allow(non_snake_case)]
 impl IRawElementProviderSimple_Impl for PlatformNode {
     fn ProviderOptions(&self) -> Result<ProviderOptions> {
         Ok(ProviderOptions_ServerSideProvider)
     }
@@ -647,15 +670,15 @@
             }
             Ok(result.into())
         })
     }
 
     fn HostRawElementProvider(&self) -> Result<IRawElementProviderSimple> {
         self.with_tree_state_and_context(|state, context| {
-            if self.node_id == state.root_id() {
+            if self.is_root(state) {
                 unsafe { UiaHostProviderFromHwnd(context.hwnd) }
             } else {
                 Err(Error::empty())
             }
         })
     }
 }
@@ -678,15 +701,25 @@
                 Some(result) => Ok(self.relative(result.id()).into()),
                 None => Err(Error::empty()),
             }
         })
     }
 
     fn GetRuntimeId(&self) -> Result<*mut SAFEARRAY> {
-        let runtime_id = runtime_id_from_node_id(self.node_id);
+        let node_id = if let Some(id) = self.node_id {
+            id
+        } else {
+            // Since this `PlatformNode` isn't associated with a specific
+            // node ID, but always uses whatever node is currently the root,
+            // we shouldn't return a UIA runtime ID calculated from an
+            // AccessKit node ID, as we normally do. Fortunately,
+            // UIA doesn't seem to actually call `GetRuntimeId` on the root.
+            return Err(not_implemented());
+        };
+        let runtime_id = runtime_id_from_node_id(node_id);
         Ok(safe_array_from_i32_slice(&runtime_id))
     }
 
     fn BoundingRectangle(&self) -> Result<UiaRect> {
         self.resolve_with_context(|node, context| {
             let rect = node.bounding_box().map_or(UiaRect::default(), |rect| {
                 let client_top_left = context.client_top_left();
@@ -702,28 +735,24 @@
     }
 
     fn GetEmbeddedFragmentRoots(&self) -> Result<*mut SAFEARRAY> {
         Ok(std::ptr::null_mut())
     }
 
     fn SetFocus(&self) -> Result<()> {
-        self.do_action(|| ActionRequest {
-            action: Action::Focus,
-            target: self.node_id,
-            data: None,
-        })
+        self.do_action(|| (Action::Focus, None))
     }
 
     fn FragmentRoot(&self) -> Result<IRawElementProviderFragmentRoot> {
         self.with_tree_state(|state| {
-            let root_id = state.root_id();
-            if root_id == self.node_id {
+            if self.is_root(state) {
                 // SAFETY: We know &self is inside a full COM implementation.
                 unsafe { self.cast() }
             } else {
+                let root_id = state.root_id();
                 Ok(self.relative(root_id).into())
             }
         })
     }
 }
 
 #[allow(non_snake_case)]
@@ -739,15 +768,20 @@
             )
         })
     }
 
     fn GetFocus(&self) -> Result<IRawElementProviderFragment> {
         self.with_tree_state(|state| {
             if let Some(id) = state.focus_id() {
-                if id != self.node_id {
+                let self_id = if let Some(id) = self.node_id {
+                    id
+                } else {
+                    state.root_id()
+                };
+                if id != self_id {
                     return Ok(self.relative(id).into());
                 }
             }
             Err(Error::empty())
         })
     }
 }
@@ -881,37 +915,29 @@
     (Value, is_value_pattern_supported, (
         (Value, value, BSTR),
         (IsReadOnly, is_read_only, BOOL)
     ), (
         fn SetValue(&self, value: &PCWSTR) -> Result<()> {
             self.do_action(|| {
                 let value = unsafe { value.to_string() }.unwrap();
-                ActionRequest {
-                    action: Action::SetValue,
-                    target: self.node_id,
-                    data: Some(ActionData::Value(value.into())),
-                }
+                (Action::SetValue, Some(ActionData::Value(value.into())))
             })
         }
     )),
     (RangeValue, is_range_value_pattern_supported, (
         (Value, numeric_value, f64),
         (IsReadOnly, is_read_only, BOOL),
         (Minimum, min_numeric_value, f64),
         (Maximum, max_numeric_value, f64),
         (SmallChange, numeric_value_step, f64),
         (LargeChange, numeric_value_jump, f64)
     ), (
         fn SetValue(&self, value: f64) -> Result<()> {
             self.do_action(|| {
-                ActionRequest {
-                    action: Action::SetValue,
-                    target: self.node_id,
-                    data: Some(ActionData::NumericValue(value)),
-                }
+                (Action::SetValue, Some(ActionData::NumericValue(value)))
             })
         }
     )),
     (SelectionItem, is_selection_item_pattern_supported, (
         (IsSelected, is_selected, BOOL)
     ), (
         fn Select(&self) -> Result<()> {
```

### Comparing `accesskit-0.3.0/platforms/windows/src/subclass.rs` & `accesskit-0.3.1/platforms/windows/src/subclass.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/platforms/windows/src/tests/mod.rs` & `accesskit-0.3.1/platforms/windows/src/tests/mod.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/platforms/windows/src/tests/simple.rs` & `accesskit-0.3.1/platforms/windows/src/tests/simple.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/platforms/windows/src/tests/subclassed.rs` & `accesskit-0.3.1/platforms/windows/src/tests/subclassed.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/platforms/windows/src/text.rs` & `accesskit-0.3.1/platforms/windows/src/text.rs`

 * *Files 0% similar despite different names*

```diff
@@ -470,15 +470,15 @@
     }
 
     fn GetEnclosingElement(&self) -> Result<IRawElementProviderSimple> {
         self.with_node(|node| {
             // Revisit this if we eventually support embedded objects.
             Ok(PlatformNode {
                 context: self.context.clone(),
-                node_id: node.id(),
+                node_id: Some(node.id()),
             }
             .into())
         })
     }
 
     fn GetText(&self, _max_length: i32) -> Result<BSTR> {
         // The Microsoft docs imply that the provider isn't _required_
```

### Comparing `accesskit-0.3.0/platforms/windows/src/util.rs` & `accesskit-0.3.1/platforms/windows/src/util.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/common/Cargo.toml` & `accesskit-0.3.1/common/Cargo.toml`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/common/CHANGELOG.md` & `accesskit-0.3.1/common/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/common/README.md` & `accesskit-0.3.1/common/README.md`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/common/src/geometry.rs` & `accesskit-0.3.1/common/src/geometry.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/common/src/lib.rs` & `accesskit-0.3.1/common/src/lib.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/platforms/atspi-common/Cargo.toml` & `accesskit-0.3.1/platforms/atspi-common/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [package]
 name = "accesskit_atspi_common"
-version = "0.4.0"
+version = "0.4.1"
 authors.workspace = true
 license.workspace = true
 description = "AccessKit UI accessibility infrastructure: core AT-SPI translation layer"
 categories.workspace = true
 keywords = ["gui", "ui", "accessibility"]
 repository.workspace = true
 readme = "README.md"
 edition.workspace = true
 rust-version.workspace = true
 
 [dependencies]
 accesskit = { version = "0.14.0", path = "../../common" }
-accesskit_consumer = { version = "0.19.0", path = "../../consumer" }
+accesskit_consumer = { version = "0.19.1", path = "../../consumer" }
 atspi-common = { version = "0.3.0", default-features = false }
 serde = "1.0"
 thiserror = "1.0.39"
 zvariant = { version = "3", default-features = false }
```

### Comparing `accesskit-0.3.0/platforms/atspi-common/CHANGELOG.md` & `accesskit-0.3.1/platforms/atspi-common/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # Changelog
 
 * The following workspace dependencies were updated
   * dependencies
     * accesskit bumped from 0.12.2 to 0.12.3
     * accesskit_consumer bumped from 0.17.0 to 0.17.1
 
+* The following workspace dependencies were updated
+  * dependencies
+    * accesskit_consumer bumped from 0.19.0 to 0.19.1
+
 ## [0.4.0](https://github.com/AccessKit/accesskit/compare/accesskit_atspi_common-v0.3.0...accesskit_atspi_common-v0.4.0) (2024-04-30)
 
 
 ### ⚠ BREAKING CHANGES
 
 * Clean up table roles and properties ([#393](https://github.com/AccessKit/accesskit/issues/393))
 * Rename `Checked` to `Toggled`; drop `ToggleButton` role ([#388](https://github.com/AccessKit/accesskit/issues/388))
```

### Comparing `accesskit-0.3.0/platforms/atspi-common/src/adapter.rs` & `accesskit-0.3.1/platforms/atspi-common/src/adapter.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/platforms/atspi-common/src/callback.rs` & `accesskit-0.3.1/platforms/atspi-common/src/callback.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/platforms/atspi-common/src/context.rs` & `accesskit-0.3.1/platforms/atspi-common/src/context.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/platforms/atspi-common/src/error.rs` & `accesskit-0.3.1/platforms/atspi-common/src/error.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/platforms/atspi-common/src/events.rs` & `accesskit-0.3.1/platforms/atspi-common/src/events.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/platforms/atspi-common/src/lib.rs` & `accesskit-0.3.1/platforms/atspi-common/src/lib.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/platforms/atspi-common/src/node.rs` & `accesskit-0.3.1/platforms/atspi-common/src/node.rs`

 * *Files 2% similar despite different names*

```diff
@@ -40,33 +40,33 @@
     fn node_state(&self) -> &NodeState {
         match self {
             Self::Node(node) => node.state(),
             Self::DetachedNode(node) => node.state(),
         }
     }
 
-    pub fn name(&self) -> Option<String> {
+    pub(crate) fn name(&self) -> Option<String> {
         match self {
             Self::Node(node) => node.name(),
             Self::DetachedNode(node) => node.name(),
         }
     }
 
     pub(crate) fn description(&self) -> Option<String> {
         match self {
             Self::Node(node) => node.description(),
             Self::DetachedNode(node) => node.description(),
         }
     }
 
-    pub fn parent_id(&self) -> Option<NodeId> {
+    pub(crate) fn parent_id(&self) -> Option<NodeId> {
         self.node_state().parent_id()
     }
 
-    pub fn id(&self) -> NodeId {
+    pub(crate) fn id(&self) -> NodeId {
         self.node_state().id()
     }
 
     fn child_ids(
         &self,
     ) -> impl DoubleEndedIterator<Item = NodeId>
            + ExactSizeIterator<Item = NodeId>
@@ -80,15 +80,15 @@
     ) -> impl DoubleEndedIterator<Item = NodeId> + FusedIterator<Item = NodeId> + '_ {
         match self {
             Self::Node(node) => node.filtered_children(&filter).map(|child| child.id()),
             _ => unreachable!(),
         }
     }
 
-    pub fn role(&self) -> AtspiRole {
+    pub(crate) fn role(&self) -> AtspiRole {
         if self.node_state().has_role_description() {
             return AtspiRole::Extended;
         }
 
         match self.node_state().role() {
             Role::Alert => AtspiRole::Notification,
             Role::AlertDialog => AtspiRole::Alert,
@@ -303,15 +303,15 @@
     fn is_focused(&self) -> bool {
         match self {
             Self::Node(node) => node.is_focused(),
             Self::DetachedNode(node) => node.is_focused(),
         }
     }
 
-    pub fn state(&self, is_window_focused: bool) -> StateSet {
+    pub(crate) fn state(&self, is_window_focused: bool) -> StateSet {
         let state = self.node_state();
         let atspi_role = self.role();
         let mut atspi_state = StateSet::empty();
         if state.parent_id().is_none() && state.role() == Role::Window && is_window_focused {
             atspi_state.insert(State::Active);
         }
         // TODO: Focus and selection.
@@ -387,15 +387,15 @@
         self.node_state().raw_bounds().is_some() || self.is_root()
     }
 
     fn supports_value(&self) -> bool {
         self.current_value().is_some()
     }
 
-    pub fn interfaces(&self) -> InterfaceSet {
+    pub(crate) fn interfaces(&self) -> InterfaceSet {
         let mut interfaces = InterfaceSet::new(Interface::Accessible);
         if self.supports_action() {
             interfaces.insert(Interface::Action);
         }
         if self.supports_component() {
             interfaces.insert(Interface::Component);
         }
```

### Comparing `accesskit-0.3.0/platforms/atspi-common/src/rect.rs` & `accesskit-0.3.1/platforms/atspi-common/src/rect.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/platforms/atspi-common/src/simplified.rs` & `accesskit-0.3.1/platforms/atspi-common/src/simplified.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/platforms/atspi-common/src/util.rs` & `accesskit-0.3.1/platforms/atspi-common/src/util.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/platforms/macos/Cargo.toml` & `accesskit-0.3.1/platforms/macos/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "accesskit_macos"
-version = "0.13.0"
+version = "0.13.1"
 authors.workspace = true
 license.workspace = true
 description = "AccessKit UI accessibility infrastructure: macOS adapter"
 categories.workspace = true
 keywords = ["gui", "ui", "accessibility"]
 repository.workspace = true
 readme = "README.md"
@@ -12,15 +12,15 @@
 rust-version.workspace = true
 
 [package.metadata.docs.rs]
 default-target = "x86_64-apple-darwin"
 
 [dependencies]
 accesskit = { version = "0.14.0", path = "../../common" }
-accesskit_consumer = { version = "0.19.0", path = "../../consumer" }
+accesskit_consumer = { version = "0.19.1", path = "../../consumer" }
 once_cell = "1.13.0"
 objc2 = "0.5.1"
 objc2-foundation = { version = "0.2.0", features = [
     "NSArray",
     "NSDictionary",
     "NSValue",
     "NSThread",
```

### Comparing `accesskit-0.3.0/platforms/macos/CHANGELOG.md` & `accesskit-0.3.1/platforms/macos/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,18 @@
     * accesskit_consumer bumped from 0.16.0 to 0.16.1
 
 * The following workspace dependencies were updated
   * dependencies
     * accesskit bumped from 0.12.2 to 0.12.3
     * accesskit_consumer bumped from 0.17.0 to 0.17.1
 
+* The following workspace dependencies were updated
+  * dependencies
+    * accesskit_consumer bumped from 0.19.0 to 0.19.1
+
 ## [0.13.0](https://github.com/AccessKit/accesskit/compare/accesskit_macos-v0.12.0...accesskit_macos-v0.13.0) (2024-04-30)
 
 
 ### ⚠ BREAKING CHANGES
 
 * Clean up table roles and properties ([#393](https://github.com/AccessKit/accesskit/issues/393))
 * Drop `NodeClassSet` ([#389](https://github.com/AccessKit/accesskit/issues/389))
```

### Comparing `accesskit-0.3.0/platforms/macos/src/adapter.rs` & `accesskit-0.3.1/platforms/macos/src/adapter.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/platforms/macos/src/context.rs` & `accesskit-0.3.1/platforms/macos/src/context.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/platforms/macos/src/event.rs` & `accesskit-0.3.1/platforms/macos/src/event.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/platforms/macos/src/lib.rs` & `accesskit-0.3.1/platforms/macos/src/lib.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/platforms/macos/src/node.rs` & `accesskit-0.3.1/platforms/macos/src/node.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/platforms/macos/src/patch.rs` & `accesskit-0.3.1/platforms/macos/src/patch.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/platforms/macos/src/subclass.rs` & `accesskit-0.3.1/platforms/macos/src/subclass.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/platforms/macos/src/util.rs` & `accesskit-0.3.1/platforms/macos/src/util.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/consumer/CHANGELOG.md` & `accesskit-0.3.1/consumer/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,21 @@
   * dependencies
     * accesskit bumped from 0.11.1 to 0.11.2
 
 * The following workspace dependencies were updated
   * dependencies
     * accesskit bumped from 0.12.2 to 0.12.3
 
+## [0.19.1](https://github.com/AccessKit/accesskit/compare/accesskit_consumer-v0.19.0...accesskit_consumer-v0.19.1) (2024-05-11)
+
+
+### Bug Fixes
+
+* Improve panic messages ([#401](https://github.com/AccessKit/accesskit/issues/401)) ([e6ce021](https://github.com/AccessKit/accesskit/commit/e6ce021b3b172f5ea7ee31496c9afaf66b1871f2))
+
 ## [0.19.0](https://github.com/AccessKit/accesskit/compare/accesskit_consumer-v0.18.0...accesskit_consumer-v0.19.0) (2024-04-30)
 
 
 ### ⚠ BREAKING CHANGES
 
 * Drop `NodeClassSet` ([#389](https://github.com/AccessKit/accesskit/issues/389))
 * Rename `Checked` to `Toggled`; drop `ToggleButton` role ([#388](https://github.com/AccessKit/accesskit/issues/388))
```

### Comparing `accesskit-0.3.0/consumer/src/filters.rs` & `accesskit-0.3.1/consumer/src/filters.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/consumer/src/iterators.rs` & `accesskit-0.3.1/consumer/src/iterators.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/consumer/src/lib.rs` & `accesskit-0.3.1/consumer/src/lib.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/consumer/src/node.rs` & `accesskit-0.3.1/consumer/src/node.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/consumer/src/text.rs` & `accesskit-0.3.1/consumer/src/text.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/consumer/src/tree.rs` & `accesskit-0.3.1/consumer/src/tree.rs`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,20 @@
     updated_nodes: HashMap<NodeId, DetachedNode>,
     focus_change: Option<InternalFocusChange>,
     removed_nodes: HashMap<NodeId, DetachedNode>,
 }
 
 impl State {
     fn validate_global(&self) {
-        assert!(self.nodes.contains_key(&self.data.root));
-        assert!(self.nodes.contains_key(&self.focus));
+        if !self.nodes.contains_key(&self.data.root) {
+            panic!("Root id #{} is not in the node list", self.data.root.0);
+        }
+        if !self.nodes.contains_key(&self.focus) {
+            panic!("Focused id #{} is not in the node list", self.focus.0);
+        }
     }
 
     fn update(
         &mut self,
         update: TreeUpdate,
         is_host_focused: bool,
         mut changes: Option<&mut InternalChanges>,
@@ -89,15 +93,20 @@
         }
 
         for (node_id, node_data) in update.nodes {
             orphans.remove(&node_id);
 
             let mut seen_child_ids = HashSet::new();
             for (child_index, child_id) in node_data.children().iter().enumerate() {
-                assert!(!seen_child_ids.contains(child_id));
+                if seen_child_ids.contains(child_id) {
+                    panic!(
+                        "Node #{} of TreeUpdate includes duplicate child #{};",
+                        node_id.0, child_id.0
+                    );
+                }
                 orphans.remove(child_id);
                 let parent_and_index = ParentAndIndex(node_id, child_index);
                 if let Some(child_state) = self.nodes.get_mut(child_id) {
                     if child_state.parent_and_index != Some(parent_and_index) {
                         child_state.parent_and_index = Some(parent_and_index);
                     }
                 } else if let Some(child_data) = pending_nodes.remove(child_id) {
@@ -135,16 +144,20 @@
             } else if node_id == root {
                 add_node(&mut self.nodes, &mut changes, None, node_id, node_data);
             } else {
                 pending_nodes.insert(node_id, node_data);
             }
         }
 
-        assert_eq!(pending_nodes.len(), 0);
-        assert_eq!(pending_children.len(), 0);
+        if !pending_nodes.is_empty() {
+            panic!("TreeUpdate includes {} nodes which are neither in the current tree nor a child of another node from the update: {}", pending_nodes.len(), short_node_list(pending_nodes.keys()));
+        }
+        if !pending_children.is_empty() {
+            panic!("TreeUpdate's nodes include {} children ids which are neither in the current tree nor the id of another node from the update: {}", pending_children.len(), short_node_list(pending_children.keys()));
+        }
 
         if update.focus != self.focus || is_host_focused != self.is_host_focused {
             let old_focus = old_focus_id.map(|id| self.node_by_id(id).unwrap().detached());
             let new_focus = is_host_focused.then_some(update.focus);
             if let Some(changes) = &mut changes {
                 changes.focus_change = Some(InternalFocusChange {
                     old_focus,
@@ -301,17 +314,20 @@
 
 pub struct Tree {
     state: State,
 }
 
 impl Tree {
     pub fn new(mut initial_state: TreeUpdate, is_host_focused: bool) -> Self {
+        let Some(tree) = initial_state.tree.take() else {
+            panic!("Tried to initialize the accessibility tree without a root tree. TreeUpdate::tree must be Some.");
+        };
         let mut state = State {
             nodes: HashMap::new(),
-            data: initial_state.tree.take().unwrap(),
+            data: tree,
             focus: initial_state.focus,
             is_host_focused,
         };
         state.update(initial_state, is_host_focused, None);
         Self { state }
     }
 
@@ -387,14 +403,35 @@
     }
 
     pub fn state(&self) -> &State {
         &self.state
     }
 }
 
+fn short_node_list<'a>(nodes: impl ExactSizeIterator<Item = &'a NodeId>) -> String {
+    if nodes.len() > 10 {
+        format!(
+            "[{} ...]",
+            nodes
+                .take(10)
+                .map(|id| format!("#{}", id.0))
+                .collect::<Vec<_>>()
+                .join(", "),
+        )
+    } else {
+        format!(
+            "[{}]",
+            nodes
+                .map(|id| format!("#{}", id.0))
+                .collect::<Vec<_>>()
+                .join(", "),
+        )
+    }
+}
+
 #[cfg(test)]
 mod tests {
     use accesskit::{NodeBuilder, NodeId, Role, Tree, TreeUpdate};
 
     #[test]
     fn init_tree_with_root_node() {
         let update = TreeUpdate {
```

### Comparing `accesskit-0.3.0/bindings/python/Cargo.toml` & `accesskit-0.3.1/bindings/python/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "accesskit_python"
-version = "0.3.0"
+version = "0.3.1"
 authors.workspace = true
 license.workspace = true
 description = "Python bindings to the AccessKit library"
 readme = "README.md"
 publish = false
 edition.workspace = true
 
@@ -17,14 +17,14 @@
 extension-module = ["pyo3/extension-module"]
 
 [dependencies]
 accesskit = { version = "0.14.0", path = "../../common", features = ["pyo3"] }
 pyo3 = { version = "0.20", features = ["abi3-py38", "multiple-pymethods"] }
 
 [target.'cfg(target_os = "windows")'.dependencies]
-accesskit_windows = { version = "0.18.0", path = "../../platforms/windows" }
+accesskit_windows = { version = "0.18.1", path = "../../platforms/windows" }
 
 [target.'cfg(target_os = "macos")'.dependencies]
-accesskit_macos = { version = "0.13.0", path = "../../platforms/macos" }
+accesskit_macos = { version = "0.13.1", path = "../../platforms/macos" }
 
 [target.'cfg(any(target_os = "linux", target_os = "dragonfly", target_os = "freebsd", target_os = "openbsd", target_os = "netbsd"))'.dependencies]
-accesskit_unix = { version = "0.9.0", path = "../../platforms/unix" }
+accesskit_unix = { version = "0.9.1", path = "../../platforms/unix" }
```

### Comparing `accesskit-0.3.0/bindings/python/CHANGELOG.md` & `accesskit-0.3.1/bindings/python/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,30 @@
   * dependencies
     * accesskit_unix bumped from 0.7.4 to 0.7.5
 
 * The following workspace dependencies were updated
   * dependencies
     * accesskit_windows bumped from 0.16.3 to 0.16.4
 
+## [0.3.1](https://github.com/AccessKit/accesskit/compare/accesskit_python-v0.3.0...accesskit_python-v0.3.1) (2024-05-11)
+
+
+### Bug Fixes
+
+* Fix dead code warning on Unix platforms ([#403](https://github.com/AccessKit/accesskit/issues/403)) ([09d9157](https://github.com/AccessKit/accesskit/commit/09d91577dd88743e379a1fdea34b25a94726d0fb))
+
+
+### Dependencies
+
+* The following workspace dependencies were updated
+  * dependencies
+    * accesskit_windows bumped from 0.18.0 to 0.18.1
+    * accesskit_macos bumped from 0.13.0 to 0.13.1
+    * accesskit_unix bumped from 0.9.0 to 0.9.1
+
 ## [0.3.0](https://github.com/AccessKit/accesskit/compare/accesskit_python-v0.2.0...accesskit_python-v0.3.0) (2024-04-30)
 
 
 ### ⚠ BREAKING CHANGES
 
 * Clean up table roles and properties ([#393](https://github.com/AccessKit/accesskit/issues/393))
 * Rename `hierarchical_level` to `level` ([#390](https://github.com/AccessKit/accesskit/issues/390))
```

### Comparing `accesskit-0.3.0/bindings/python/README.md` & `accesskit-0.3.1/bindings/python/README.md`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/bindings/python/examples/pygame/.gitignore` & `accesskit-0.3.1/bindings/python/examples/pygame/.gitignore`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/bindings/python/examples/pygame/hello_world.py` & `accesskit-0.3.1/bindings/python/examples/pygame/hello_world.py`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/bindings/python/src/common.rs` & `accesskit-0.3.1/bindings/python/src/common.rs`

 * *Files 0% similar despite different names*

```diff
@@ -711,14 +711,17 @@
                     TextSelection::from(&selection).into_py(py),
                 ),
             }),
         })
     }
 }
 
+// The following exception is needed because this struct is only used
+// in the bindings for some platform adapters.
+#[allow(dead_code)]
 pub(crate) struct LocalPythonActivationHandler<'a> {
     pub(crate) py: Python<'a>,
     pub(crate) handler: Py<PyAny>,
 }
 
 impl accesskit::ActivationHandler for LocalPythonActivationHandler<'_> {
     fn request_initial_tree(&mut self) -> Option<accesskit::TreeUpdate> {
```

### Comparing `accesskit-0.3.0/bindings/python/src/geometry.rs` & `accesskit-0.3.1/bindings/python/src/geometry.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/bindings/python/src/lib.rs` & `accesskit-0.3.1/bindings/python/src/lib.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/bindings/python/src/macos.rs` & `accesskit-0.3.1/bindings/python/src/macos.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/bindings/python/src/unix.rs` & `accesskit-0.3.1/bindings/python/src/unix.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/bindings/python/src/windows.rs` & `accesskit-0.3.1/bindings/python/src/windows.rs`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/Cargo.lock` & `accesskit-0.3.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -26,68 +26,68 @@
  "pyo3",
  "schemars",
  "serde",
 ]
 
 [[package]]
 name = "accesskit_atspi_common"
-version = "0.4.0"
+version = "0.4.1"
 dependencies = [
  "accesskit",
  "accesskit_consumer",
  "atspi-common",
  "serde",
  "thiserror",
  "zvariant",
 ]
 
 [[package]]
 name = "accesskit_c"
-version = "0.9.0"
+version = "0.10.0"
 dependencies = [
  "accesskit",
  "accesskit_macos",
  "accesskit_unix",
  "accesskit_windows",
  "paste",
 ]
 
 [[package]]
 name = "accesskit_consumer"
-version = "0.19.0"
+version = "0.19.1"
 dependencies = [
  "accesskit",
 ]
 
 [[package]]
 name = "accesskit_macos"
-version = "0.13.0"
+version = "0.13.1"
 dependencies = [
  "accesskit",
  "accesskit_consumer",
  "objc2",
  "objc2-app-kit",
  "objc2-foundation",
  "once_cell",
 ]
 
 [[package]]
 name = "accesskit_python"
-version = "0.3.0"
+version = "0.3.1"
 dependencies = [
  "accesskit",
  "accesskit_macos",
  "accesskit_unix",
  "accesskit_windows",
  "pyo3",
 ]
 
 [[package]]
 name = "accesskit_unix"
-version = "0.9.0"
+version = "0.9.1"
 dependencies = [
  "accesskit",
  "accesskit_atspi_common",
  "async-channel 2.1.1",
  "async-executor",
  "async-task",
  "atspi",
@@ -97,29 +97,29 @@
  "tokio",
  "tokio-stream",
  "zbus",
 ]
 
 [[package]]
 name = "accesskit_windows"
-version = "0.18.0"
+version = "0.18.1"
 dependencies = [
  "accesskit",
  "accesskit_consumer",
  "once_cell",
  "paste",
  "scopeguard",
  "static_assertions",
  "windows",
  "winit",
 ]
 
 [[package]]
 name = "accesskit_winit"
-version = "0.20.0"
+version = "0.20.1"
 dependencies = [
  "accesskit",
  "accesskit_macos",
  "accesskit_unix",
  "accesskit_windows",
  "raw-window-handle 0.5.2",
  "raw-window-handle 0.6.0",
```

### Comparing `accesskit-0.3.0/pyproject.toml` & `accesskit-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/LICENSE-APACHE` & `accesskit-0.3.1/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/LICENSE-MIT` & `accesskit-0.3.1/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/LICENSE.chromium` & `accesskit-0.3.1/LICENSE.chromium`

 * *Files identical despite different names*

### Comparing `accesskit-0.3.0/PKG-INFO` & `accesskit-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: accesskit
-Version: 0.3.0
+Version: 0.3.1
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

