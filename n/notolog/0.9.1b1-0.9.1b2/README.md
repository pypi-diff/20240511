# Comparing `tmp/notolog-0.9.1b1.tar.gz` & `tmp/notolog-0.9.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notolog-0.9.1b1.tar", last modified: Mon May  6 20:29:08 2024, max compression
+gzip compressed data, was "notolog-0.9.1b2.tar", last modified: Sat May 11 12:36:17 2024, max compression
```

## Comparing `notolog-0.9.1b1.tar` & `notolog-0.9.1b2.tar`

### file list

```diff
@@ -1,430 +1,350 @@
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.382591 notolog-0.9.1b1/
--rw-r--r--   0 vadikus    (501) staff       (20)     5008 2024-05-06 20:09:20.000000 notolog-0.9.1b1/CHANGELOG.md
--rw-r--r--   0 vadikus    (501) staff       (20)     1073 2024-05-04 21:27:31.000000 notolog-0.9.1b1/LICENSE
--rw-r--r--   0 vadikus    (501) staff       (20)      191 2024-05-05 14:33:15.000000 notolog-0.9.1b1/MANIFEST.in
--rw-r--r--   0 vadikus    (501) staff       (20)    17029 2024-05-06 20:29:08.380968 notolog-0.9.1b1/PKG-INFO
--rw-r--r--   0 vadikus    (501) staff       (20)    14998 2024-05-06 20:20:54.000000 notolog-0.9.1b1/README.md
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:07.809018 notolog-0.9.1b1/app/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4777 2024-05-06 20:09:20.000000 notolog-0.9.1b1/app/app_config.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:07.815389 notolog-0.9.1b1/app/assets/
--rw-r--r--   0 vadikus    (501) staff       (20)     4202 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/notolog-example-image.png
--rw-r--r--   0 vadikus    (501) staff       (20)    88211 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/notolog-logo.png
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:07.752985 notolog-0.9.1b1/app/assets/themes/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:07.832963 notolog-0.9.1b1/app/assets/themes/calligraphy/
--rw-r--r--   0 vadikus    (501) staff       (20)      777 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/calligraphy/about_popup.css
--rw-r--r--   0 vadikus    (501) staff       (20)      365 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/calligraphy/ai_assistant.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2767 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/calligraphy/default.ini
--rw-r--r--   0 vadikus    (501) staff       (20)       56 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/calligraphy/editor.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2187 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/calligraphy/md.ini
--rw-r--r--   0 vadikus    (501) staff       (20)      903 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/calligraphy/settings_dialog.css
--rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/calligraphy/statusbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)     6330 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/calligraphy/styles.css
--rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/calligraphy/toolbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)      743 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/calligraphy/tree_view.css
--rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/calligraphy/viewer.css
--rw-r--r--   0 vadikus    (501) staff       (20)       80 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/calligraphy/viewer.ini
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:07.876101 notolog-0.9.1b1/app/assets/themes/default/
--rw-r--r--   0 vadikus    (501) staff       (20)      798 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/about_popup.css
--rw-r--r--   0 vadikus    (501) staff       (20)      253 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/ai_assistant.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2775 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/default.ini
--rw-r--r--   0 vadikus    (501) staff       (20)      174 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/editor.css
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:07.999339 notolog-0.9.1b1/app/assets/themes/default/icons/
--rw-r--r--   0 vadikus    (501) staff       (20)     1093 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/LICENSE
--rw-r--r--   0 vadikus    (501) staff       (20)      349 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/arrow-clockwise.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      567 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/arrow-repeat.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      736 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/balloon-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      797 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/balloon.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      812 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/bandaid-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      959 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/bandaid.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      528 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/box-arrow-up-right.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      538 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/box-arrow-up.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      265 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/caret-down-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      265 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/caret-up-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      455 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/code-slash.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      694 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/cursor-text.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      459 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/eyedropper.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      403 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/eyeglasses.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      479 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/file-earmark-lock2.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      394 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/file-earmark-plus-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      481 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/file-earmark-x.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      294 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/file-earmark.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      547 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/filetype-html.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      705 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/filetype-md.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      524 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/filetype-txt.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      401 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/floppy2-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      606 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/floppy2.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      428 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/folder-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      708 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/folder-symlink.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      527 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/folder.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      708 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/github.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      518 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/link-45deg.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      666 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/linkedin.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      575 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/pencil-square.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      261 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/power.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      582 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/quote.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      996 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/robot.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      316 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/share-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      653 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/shield-lock-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)     1057 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/shield-lock.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      399 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/star-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      623 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/star.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      272 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/three-dots.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      577 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/trash3-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      656 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/trash3.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      301 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/twitter-x.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      465 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/type-bold.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      351 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/type-italic.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      574 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/type-strikethrough.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      319 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/type-underline.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      351 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/x-circle-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      397 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/x-square-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      491 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/icons/x-square.svg
--rw-r--r--   0 vadikus    (501) staff       (20)     2250 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/md.ini
--rw-r--r--   0 vadikus    (501) staff       (20)      739 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/settings_dialog.css
--rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/statusbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)     7980 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/styles.css
--rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/toolbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)      744 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/tree_view.css
--rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/viewer.css
--rw-r--r--   0 vadikus    (501) staff       (20)       82 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/default/viewer.ini
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.021476 notolog-0.9.1b1/app/assets/themes/noir_dark/
--rw-r--r--   0 vadikus    (501) staff       (20)      777 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/noir_dark/about_popup.css
--rw-r--r--   0 vadikus    (501) staff       (20)      347 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/noir_dark/ai_assistant.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2745 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/noir_dark/default.ini
--rw-r--r--   0 vadikus    (501) staff       (20)       56 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/noir_dark/editor.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2357 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/noir_dark/md.ini
--rw-r--r--   0 vadikus    (501) staff       (20)     1435 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/noir_dark/settings_dialog.css
--rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/noir_dark/statusbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)     6433 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/noir_dark/styles.css
--rw-r--r--   0 vadikus    (501) staff       (20)      280 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/noir_dark/toolbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)      711 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/noir_dark/tree_view.css
--rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/assets/themes/noir_dark/viewer.css
--rw-r--r--   0 vadikus    (501) staff       (20)       76 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/noir_dark/viewer.ini
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.034576 notolog-0.9.1b1/app/assets/themes/strawberry/
--rw-r--r--   0 vadikus    (501) staff       (20)      790 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/strawberry/about_popup.css
--rw-r--r--   0 vadikus    (501) staff       (20)      317 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/strawberry/ai_assistant.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2775 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/strawberry/default.ini
--rw-r--r--   0 vadikus    (501) staff       (20)       50 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/strawberry/editor.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2268 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/strawberry/md.ini
--rw-r--r--   0 vadikus    (501) staff       (20)      771 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/strawberry/settings_dialog.css
--rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/strawberry/statusbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)     7963 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/strawberry/styles.css
--rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/strawberry/toolbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)      764 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/strawberry/tree_view.css
--rw-r--r--   0 vadikus    (501) staff       (20)       60 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/strawberry/viewer.css
--rw-r--r--   0 vadikus    (501) staff       (20)       84 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/assets/themes/strawberry/viewer.ini
--rw-r--r--   0 vadikus    (501) staff       (20)     7823 2024-05-04 21:27:27.000000 notolog-0.9.1b1/app/edit_widget.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4196 2024-05-04 21:27:27.000000 notolog-0.9.1b1/app/editor_state.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.041930 notolog-0.9.1b1/app/encrypt/
--rw-r--r--   0 vadikus    (501) staff       (20)      152 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/encrypt/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4337 2024-05-06 20:24:02.000000 notolog-0.9.1b1/app/encrypt/enc_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6076 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/encrypt/enc_new_password_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)      626 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/encrypt/enc_password.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4172 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/encrypt/enc_password_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3211 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/encrypt/enc_password_reset_dialog.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.051858 notolog-0.9.1b1/app/enums/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/enums/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1876 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/enums/ai_model_names.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6158 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/enums/colors.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1487 2024-05-06 20:09:20.000000 notolog-0.9.1b1/app/enums/languages.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1386 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/enums/themes.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3236 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/etree_extension.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.053109 notolog-0.9.1b1/app/exceptions/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/exceptions/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)       52 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/exceptions/file_header_empty_exception.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7559 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/file_header.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2856 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/file_system_watcher.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.058743 notolog-0.9.1b1/app/helpers/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/helpers/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)      187 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/helpers/clipboard_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4227 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/helpers/file_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5511 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/helpers/theme_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1036 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/helpers/tooltip_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7411 2024-05-04 21:27:31.000000 notolog-0.9.1b1/app/helpers/update_helper.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.063403 notolog-0.9.1b1/app/highlight/
--rw-r--r--   0 vadikus    (501) staff       (20)      126 2024-05-04 21:27:27.000000 notolog-0.9.1b1/app/highlight/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9027 2024-05-04 21:27:27.000000 notolog-0.9.1b1/app/highlight/main_highlighter.py
--rw-r--r--   0 vadikus    (501) staff       (20)    48888 2024-05-04 21:27:27.000000 notolog-0.9.1b1/app/highlight/md_highlighter.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8475 2024-05-04 21:27:27.000000 notolog-0.9.1b1/app/highlight/view_highlighter.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9600 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/image_downloader.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.065333 notolog-0.9.1b1/app/lexemes/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/__init__.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.067687 notolog-0.9.1b1/app/lexemes/__pycache__/
--rw-r--r--   0 vadikus    (501) staff       (20)      160 2024-05-04 21:42:24.000000 notolog-0.9.1b1/app/lexemes/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     3224 2024-05-06 20:15:44.000000 notolog-0.9.1b1/app/lexemes/__pycache__/lexemes.cpython-39.pyc
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.079033 notolog-0.9.1b1/app/lexemes/de/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.090534 notolog-0.9.1b1/app/lexemes/de/__pycache__/
--rw-r--r--   0 vadikus    (501) staff       (20)      898 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/de/__pycache__/ai_assistant.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     6854 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/de/__pycache__/color_picker_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     5899 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/de/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2183 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/de/__pycache__/main_menu.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2914 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/de/__pycache__/settings_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1272 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/de/__pycache__/statusbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2730 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/de/__pycache__/toolbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)      830 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/de/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7202 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/de/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6579 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/de/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2267 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/de/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3788 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/de/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1225 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/de/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2757 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/de/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.099809 notolog-0.9.1b1/app/lexemes/en/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.107424 notolog-0.9.1b1/app/lexemes/en/__pycache__/
--rw-r--r--   0 vadikus    (501) staff       (20)      886 2024-05-04 21:55:13.000000 notolog-0.9.1b1/app/lexemes/en/__pycache__/ai_assistant.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     6663 2024-05-04 21:55:13.000000 notolog-0.9.1b1/app/lexemes/en/__pycache__/color_picker_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     5462 2024-05-04 21:55:13.000000 notolog-0.9.1b1/app/lexemes/en/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2086 2024-05-04 21:55:13.000000 notolog-0.9.1b1/app/lexemes/en/__pycache__/main_menu.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     3470 2024-05-04 21:55:13.000000 notolog-0.9.1b1/app/lexemes/en/__pycache__/settings_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1243 2024-05-04 21:55:13.000000 notolog-0.9.1b1/app/lexemes/en/__pycache__/statusbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2495 2024-05-04 21:55:13.000000 notolog-0.9.1b1/app/lexemes/en/__pycache__/toolbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)      827 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/en/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7096 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/en/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6044 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/en/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2181 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/en/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3586 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/en/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1201 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/en/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2573 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/en/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.113391 notolog-0.9.1b1/app/lexemes/es/
--rw-r--r--   0 vadikus    (501) staff       (20)      882 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/es/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7309 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/es/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6549 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/es/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2316 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/es/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3890 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/es/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1222 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/es/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2793 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/es/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.119517 notolog-0.9.1b1/app/lexemes/fi/
--rw-r--r--   0 vadikus    (501) staff       (20)      856 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/lexemes/fi/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7559 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/lexemes/fi/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6284 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/lexemes/fi/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2261 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/lexemes/fi/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3759 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/lexemes/fi/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1334 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/lexemes/fi/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2662 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/lexemes/fi/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.130970 notolog-0.9.1b1/app/lexemes/fr/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.141109 notolog-0.9.1b1/app/lexemes/fr/__pycache__/
--rw-r--r--   0 vadikus    (501) staff       (20)      977 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/fr/__pycache__/ai_assistant.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     6899 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/fr/__pycache__/color_picker_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     6212 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/fr/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2256 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/fr/__pycache__/main_menu.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     3928 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/fr/__pycache__/settings_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1274 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/fr/__pycache__/statusbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2794 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/fr/__pycache__/toolbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)      886 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/fr/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7247 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/fr/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6709 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/fr/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2344 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/fr/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3978 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/fr/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1236 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/fr/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2824 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/fr/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.148603 notolog-0.9.1b1/app/lexemes/ge/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.155476 notolog-0.9.1b1/app/lexemes/ge/__pycache__/
--rw-r--r--   0 vadikus    (501) staff       (20)     1355 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/ge/__pycache__/ai_assistant.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)    10384 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ge/__pycache__/color_picker_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     9053 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ge/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     3389 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ge/__pycache__/main_menu.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     5710 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ge/__pycache__/settings_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1642 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/ge/__pycache__/statusbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     4138 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ge/__pycache__/toolbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1323 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ge/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)    10627 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ge/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9721 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/ge/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3459 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ge/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5742 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/ge/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1583 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ge/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4107 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/ge/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.162290 notolog-0.9.1b1/app/lexemes/gr/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.170560 notolog-0.9.1b1/app/lexemes/gr/__pycache__/
--rw-r--r--   0 vadikus    (501) staff       (20)     1172 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/gr/__pycache__/ai_assistant.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     8982 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/gr/__pycache__/color_picker_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     8175 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/gr/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2804 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/gr/__pycache__/main_menu.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     5014 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/gr/__pycache__/settings_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1528 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/gr/__pycache__/statusbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     3735 2024-05-04 21:27:27.000000 notolog-0.9.1b1/app/lexemes/gr/__pycache__/toolbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1100 2024-05-04 21:27:27.000000 notolog-0.9.1b1/app/lexemes/gr/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8990 2024-05-04 21:27:27.000000 notolog-0.9.1b1/app/lexemes/gr/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8654 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/gr/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2907 2024-05-04 21:27:27.000000 notolog-0.9.1b1/app/lexemes/gr/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5016 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/gr/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1561 2024-05-04 21:27:27.000000 notolog-0.9.1b1/app/lexemes/gr/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3679 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/gr/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.187388 notolog-0.9.1b1/app/lexemes/in/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.195193 notolog-0.9.1b1/app/lexemes/in/__pycache__/
--rw-r--r--   0 vadikus    (501) staff       (20)     1328 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/in/__pycache__/ai_assistant.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     9403 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/in/__pycache__/color_picker_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     9416 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/in/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     3029 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/in/__pycache__/main_menu.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     5585 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/in/__pycache__/settings_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1618 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/in/__pycache__/statusbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     3828 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/in/__pycache__/toolbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1208 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/in/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9434 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/in/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)    10062 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/in/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3124 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/in/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5546 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/in/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1549 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/in/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3828 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/in/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.202894 notolog-0.9.1b1/app/lexemes/it/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.210712 notolog-0.9.1b1/app/lexemes/it/__pycache__/
--rw-r--r--   0 vadikus    (501) staff       (20)      930 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/it/__pycache__/ai_assistant.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     6824 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/it/__pycache__/color_picker_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     5639 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/it/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2188 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/it/__pycache__/main_menu.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2925 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/it/__pycache__/settings_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1290 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/it/__pycache__/statusbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2700 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/it/__pycache__/toolbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)      864 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/it/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7263 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/it/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6359 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/it/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2302 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/it/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3825 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/it/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1238 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/it/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2780 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/it/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.217774 notolog-0.9.1b1/app/lexemes/ja/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.229700 notolog-0.9.1b1/app/lexemes/ja/__pycache__/
--rw-r--r--   0 vadikus    (501) staff       (20)     1023 2024-05-06 20:16:27.000000 notolog-0.9.1b1/app/lexemes/ja/__pycache__/ai_assistant.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     8455 2024-05-06 20:16:27.000000 notolog-0.9.1b1/app/lexemes/ja/__pycache__/color_picker_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     6840 2024-05-06 20:16:27.000000 notolog-0.9.1b1/app/lexemes/ja/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2414 2024-05-06 20:16:27.000000 notolog-0.9.1b1/app/lexemes/ja/__pycache__/main_menu.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     4049 2024-05-06 20:16:27.000000 notolog-0.9.1b1/app/lexemes/ja/__pycache__/settings_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1304 2024-05-06 20:16:27.000000 notolog-0.9.1b1/app/lexemes/ja/__pycache__/statusbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     3050 2024-05-06 20:16:27.000000 notolog-0.9.1b1/app/lexemes/ja/__pycache__/toolbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)      931 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ja/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8464 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ja/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7241 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ja/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2443 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ja/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4014 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ja/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1242 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ja/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3000 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ja/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.241178 notolog-0.9.1b1/app/lexemes/ko/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.250342 notolog-0.9.1b1/app/lexemes/ko/__pycache__/
--rw-r--r--   0 vadikus    (501) staff       (20)      954 2024-05-04 21:28:24.000000 notolog-0.9.1b1/app/lexemes/ko/__pycache__/ai_assistant.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     7562 2024-05-04 21:28:24.000000 notolog-0.9.1b1/app/lexemes/ko/__pycache__/color_picker_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     6404 2024-05-04 21:28:24.000000 notolog-0.9.1b1/app/lexemes/ko/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2277 2024-05-04 21:28:24.000000 notolog-0.9.1b1/app/lexemes/ko/__pycache__/main_menu.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     3723 2024-05-04 21:28:24.000000 notolog-0.9.1b1/app/lexemes/ko/__pycache__/settings_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1285 2024-05-04 21:28:24.000000 notolog-0.9.1b1/app/lexemes/ko/__pycache__/statusbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2735 2024-05-04 21:28:24.000000 notolog-0.9.1b1/app/lexemes/ko/__pycache__/toolbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)      848 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/ko/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7597 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/ko/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6765 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/ko/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2268 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/ko/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3697 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/ko/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1221 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/ko/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2666 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/ko/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.257817 notolog-0.9.1b1/app/lexemes/la/
--rw-r--r--   0 vadikus    (501) staff       (20)      842 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/la/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7538 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/la/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6236 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/la/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2297 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/la/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3753 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/la/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1257 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/la/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2736 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/la/toolbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3739 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/lexemes/lexemes.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.264114 notolog-0.9.1b1/app/lexemes/nl/
--rw-r--r--   0 vadikus    (501) staff       (20)      840 2024-05-06 20:09:20.000000 notolog-0.9.1b1/app/lexemes/nl/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7094 2024-05-06 20:09:20.000000 notolog-0.9.1b1/app/lexemes/nl/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6468 2024-05-06 20:09:20.000000 notolog-0.9.1b1/app/lexemes/nl/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2229 2024-05-06 20:09:20.000000 notolog-0.9.1b1/app/lexemes/nl/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3673 2024-05-06 20:09:20.000000 notolog-0.9.1b1/app/lexemes/nl/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1220 2024-05-06 20:09:20.000000 notolog-0.9.1b1/app/lexemes/nl/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2647 2024-05-06 20:09:20.000000 notolog-0.9.1b1/app/lexemes/nl/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.270007 notolog-0.9.1b1/app/lexemes/pt/
--rw-r--r--   0 vadikus    (501) staff       (20)      898 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/pt/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7304 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/pt/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6347 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/pt/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2326 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/pt/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3830 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/pt/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1223 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/pt/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2830 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/pt/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.278185 notolog-0.9.1b1/app/lexemes/ru/
--rw-r--r--   0 vadikus    (501) staff       (20)      997 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ru/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9135 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ru/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7931 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ru/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2883 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ru/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4896 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ru/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1428 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ru/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3453 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/ru/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.291170 notolog-0.9.1b1/app/lexemes/se/
--rw-r--r--   0 vadikus    (501) staff       (20)      835 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/lexemes/se/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7048 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/lexemes/se/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6246 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/lexemes/se/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2216 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/lexemes/se/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3627 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/lexemes/se/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1220 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/lexemes/se/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2611 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/lexemes/se/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.308613 notolog-0.9.1b1/app/lexemes/tr/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.322106 notolog-0.9.1b1/app/lexemes/tr/__pycache__/
--rw-r--r--   0 vadikus    (501) staff       (20)      912 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/tr/__pycache__/ai_assistant.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     7114 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/tr/__pycache__/color_picker_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     5741 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/tr/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2272 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/tr/__pycache__/main_menu.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     3751 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/tr/__pycache__/settings_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1297 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/tr/__pycache__/statusbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2767 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/tr/__pycache__/toolbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)      809 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/tr/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7401 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/tr/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6147 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/tr/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2276 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/tr/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3733 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/tr/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1240 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/tr/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2735 2024-05-04 21:27:29.000000 notolog-0.9.1b1/app/lexemes/tr/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.331958 notolog-0.9.1b1/app/lexemes/zh/
--rw-r--r--   0 vadikus    (501) staff       (20)      792 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/zh/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7074 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/zh/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5770 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/zh/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2175 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/zh/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3476 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/zh/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1202 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/zh/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2559 2024-05-04 21:27:28.000000 notolog-0.9.1b1/app/lexemes/zh/toolbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)   175569 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/notolog_editor.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6260 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/settings.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3481 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/text_block_data.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6022 2024-05-04 21:27:27.000000 notolog-0.9.1b1/app/theme.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.355075 notolog-0.9.1b1/app/ui/
--rw-r--r--   0 vadikus    (501) staff       (20)      152 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/ui/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8224 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/ui/about_popup.py
--rw-r--r--   0 vadikus    (501) staff       (20)    16816 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/ui/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2099 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/ui/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3509 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/ui/common_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1306 2024-05-04 21:27:27.000000 notolog-0.9.1b1/app/ui/enum_combo_box.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5615 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/ui/file_system_model.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6999 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/ui/line_numbers.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2610 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/ui/rename_file_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1229 2024-05-04 21:27:27.000000 notolog-0.9.1b1/app/ui/rotating_label.py
--rw-r--r--   0 vadikus    (501) staff       (20)    37283 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/ui/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3197 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/ui/sort_filter_proxy_model.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6840 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/ui/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)    12655 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app/ui/toolbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)      455 2024-05-04 21:27:26.000000 notolog-0.9.1b1/app/ui/vertical_line_spacer.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8191 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/view_decorator.py
--rw-r--r--   0 vadikus    (501) staff       (20)    16132 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/view_processor.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2446 2024-05-04 21:27:30.000000 notolog-0.9.1b1/app/view_widget.py
--rw-r--r--   0 vadikus    (501) staff       (20)       87 2024-05-05 14:33:15.000000 notolog-0.9.1b1/app_config.toml
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.356988 notolog-0.9.1b1/docs/
--rw-r--r--   0 vadikus    (501) staff       (20)     7749 2024-05-06 20:22:54.000000 notolog-0.9.1b1/docs/Examples.md
--rw-r--r--   0 vadikus    (501) staff       (20)   247033 2024-05-04 21:27:32.000000 notolog-0.9.1b1/docs/notolog-ui-settings.png
--rw-r--r--   0 vadikus    (501) staff       (20)     2770 2024-05-05 14:33:15.000000 notolog-0.9.1b1/main.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.378317 notolog-0.9.1b1/notolog.egg-info/
--rw-r--r--   0 vadikus    (501) staff       (20)    17029 2024-05-06 20:29:07.000000 notolog-0.9.1b1/notolog.egg-info/PKG-INFO
--rw-r--r--   0 vadikus    (501) staff       (20)    14093 2024-05-06 20:29:07.000000 notolog-0.9.1b1/notolog.egg-info/SOURCES.txt
--rw-r--r--   0 vadikus    (501) staff       (20)        1 2024-05-06 20:29:07.000000 notolog-0.9.1b1/notolog.egg-info/dependency_links.txt
--rw-r--r--   0 vadikus    (501) staff       (20)       38 2024-05-06 20:29:07.000000 notolog-0.9.1b1/notolog.egg-info/entry_points.txt
--rw-r--r--   0 vadikus    (501) staff       (20)      297 2024-05-06 20:29:07.000000 notolog-0.9.1b1/notolog.egg-info/requires.txt
--rw-r--r--   0 vadikus    (501) staff       (20)       15 2024-05-06 20:29:07.000000 notolog-0.9.1b1/notolog.egg-info/top_level.txt
--rw-r--r--   0 vadikus    (501) staff       (20)      297 2024-05-06 20:09:20.000000 notolog-0.9.1b1/requirements.txt
--rw-r--r--   0 vadikus    (501) staff       (20)       38 2024-05-06 20:29:08.383136 notolog-0.9.1b1/setup.cfg
--rw-r--r--   0 vadikus    (501) staff       (20)     2166 2024-05-06 20:09:20.000000 notolog-0.9.1b1/setup.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-06 20:29:08.376505 notolog-0.9.1b1/tests/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:31.000000 notolog-0.9.1b1/tests/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5975 2024-05-04 21:27:31.000000 notolog-0.9.1b1/tests/test_enc_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2305 2024-05-04 21:27:32.000000 notolog-0.9.1b1/tests/test_enc_password.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9880 2024-05-05 14:33:15.000000 notolog-0.9.1b1/tests/test_file_header.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3962 2024-05-04 21:27:31.000000 notolog-0.9.1b1/tests/test_html_view.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5810 2024-05-04 21:27:31.000000 notolog-0.9.1b1/tests/test_lexemes.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5823 2024-05-04 21:27:31.000000 notolog-0.9.1b1/tests/test_notolog_editor.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1154 2024-05-04 21:27:32.000000 notolog-0.9.1b1/tests/test_settings.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4971 2024-05-04 21:27:32.000000 notolog-0.9.1b1/tests/test_text_block_data.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4464 2024-05-04 21:27:32.000000 notolog-0.9.1b1/tests/test_theme_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6222 2024-05-04 21:27:32.000000 notolog-0.9.1b1/tests/test_themes.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:36:17.770034 notolog-0.9.1b2/
+-rw-r--r--   0 vadikus    (501) staff       (20)     6814 2024-05-11 12:17:28.000000 notolog-0.9.1b2/CHANGELOG.md
+-rw-r--r--   0 vadikus    (501) staff       (20)     3490 2024-05-11 12:17:28.000000 notolog-0.9.1b2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 vadikus    (501) staff       (20)     1073 2024-05-04 21:27:31.000000 notolog-0.9.1b2/LICENSE
+-rw-r--r--   0 vadikus    (501) staff       (20)      433 2024-05-11 12:17:28.000000 notolog-0.9.1b2/MANIFEST.in
+-rw-r--r--   0 vadikus    (501) staff       (20)    17100 2024-05-11 12:36:17.769200 notolog-0.9.1b2/PKG-INFO
+-rw-r--r--   0 vadikus    (501) staff       (20)    15048 2024-05-11 12:17:28.000000 notolog-0.9.1b2/README.md
+-rw-r--r--   0 vadikus    (501) staff       (20)       87 2024-05-05 14:33:15.000000 notolog-0.9.1b2/app_config.toml
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:36:17.328769 notolog-0.9.1b2/docs/
+-rw-r--r--   0 vadikus    (501) staff       (20)     8631 2024-05-11 12:17:28.000000 notolog-0.9.1b2/docs/Examples.md
+-rw-r--r--   0 vadikus    (501) staff       (20)   247033 2024-05-04 21:27:32.000000 notolog-0.9.1b2/docs/notolog-ui-settings.png
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:36:17.356038 notolog-0.9.1b2/notolog/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4777 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/app_config.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:36:17.373646 notolog-0.9.1b2/notolog/assets/
+-rw-r--r--   0 vadikus    (501) staff       (20)     4202 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/notolog-example-image.png
+-rw-r--r--   0 vadikus    (501) staff       (20)    88211 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/notolog-logo.png
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:36:17.308695 notolog-0.9.1b2/notolog/assets/themes/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:36:17.390794 notolog-0.9.1b2/notolog/assets/themes/calligraphy/
+-rw-r--r--   0 vadikus    (501) staff       (20)      777 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/calligraphy/about_popup.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      365 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/calligraphy/ai_assistant.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2767 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/calligraphy/default.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)       56 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/calligraphy/editor.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2311 2024-05-11 12:17:28.000000 notolog-0.9.1b2/notolog/assets/themes/calligraphy/md.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)      885 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/calligraphy/settings_dialog.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/calligraphy/statusbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     6818 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/calligraphy/styles.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/calligraphy/toolbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      743 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/calligraphy/tree_view.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/calligraphy/viewer.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       80 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/calligraphy/viewer.ini
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:36:17.408769 notolog-0.9.1b2/notolog/assets/themes/default/
+-rw-r--r--   0 vadikus    (501) staff       (20)      798 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/about_popup.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      253 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/ai_assistant.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2775 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/default.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)      174 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/editor.css
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:36:17.481989 notolog-0.9.1b2/notolog/assets/themes/default/icons/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1093 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/LICENSE
+-rw-r--r--   0 vadikus    (501) staff       (20)      349 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/arrow-clockwise.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      567 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/arrow-repeat.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      736 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/balloon-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      797 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/balloon.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      812 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/bandaid-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      959 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/bandaid.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      528 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/box-arrow-up-right.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      538 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/box-arrow-up.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      265 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/caret-down-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      265 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/caret-up-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      455 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/code-slash.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      694 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/cursor-text.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      459 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/eyedropper.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      403 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/eyeglasses.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      479 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/file-earmark-lock2.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      394 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/file-earmark-plus-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      481 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/file-earmark-x.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      294 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/file-earmark.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      547 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/filetype-html.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      705 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/filetype-md.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      524 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/filetype-txt.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      401 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/floppy2-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      606 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/floppy2.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      428 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/folder-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      708 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/folder-symlink.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      527 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/folder.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      708 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/github.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      518 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/link-45deg.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      666 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/linkedin.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      575 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/pencil-square.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      261 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/power.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      582 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/quote.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      996 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/robot.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      316 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/share-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      653 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/shield-lock-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)     1057 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/shield-lock.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      399 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/star-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      623 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/star.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      272 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/three-dots.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      577 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/trash3-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      656 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/trash3.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      301 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/twitter-x.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      465 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/type-bold.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      351 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/type-italic.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      574 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/type-strikethrough.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      319 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/type-underline.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      351 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/x-circle-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      397 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/x-square-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      491 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/icons/x-square.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)     2363 2024-05-11 12:17:28.000000 notolog-0.9.1b2/notolog/assets/themes/default/md.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)      721 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/settings_dialog.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/statusbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     8472 2024-05-11 12:17:28.000000 notolog-0.9.1b2/notolog/assets/themes/default/styles.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/toolbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      744 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/tree_view.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/viewer.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       82 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/default/viewer.ini
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:36:17.513010 notolog-0.9.1b2/notolog/assets/themes/noir_dark/
+-rw-r--r--   0 vadikus    (501) staff       (20)      777 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/noir_dark/about_popup.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      347 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/noir_dark/ai_assistant.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2745 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/noir_dark/default.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)       56 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/noir_dark/editor.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2480 2024-05-11 12:17:28.000000 notolog-0.9.1b2/notolog/assets/themes/noir_dark/md.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)     1435 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/noir_dark/settings_dialog.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/noir_dark/statusbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     6935 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/noir_dark/styles.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      280 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/noir_dark/toolbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      711 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/noir_dark/tree_view.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/noir_dark/viewer.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       76 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/noir_dark/viewer.ini
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:36:17.523398 notolog-0.9.1b2/notolog/assets/themes/strawberry/
+-rw-r--r--   0 vadikus    (501) staff       (20)      790 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/strawberry/about_popup.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      317 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/strawberry/ai_assistant.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2775 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/strawberry/default.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)       50 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/strawberry/editor.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2408 2024-05-11 12:17:28.000000 notolog-0.9.1b2/notolog/assets/themes/strawberry/md.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)      753 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/strawberry/settings_dialog.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/strawberry/statusbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     8451 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/strawberry/styles.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/strawberry/toolbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      764 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/strawberry/tree_view.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       60 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/strawberry/viewer.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       84 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/assets/themes/strawberry/viewer.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)     7823 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/edit_widget.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4196 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/editor_state.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:36:17.539188 notolog-0.9.1b2/notolog/encrypt/
+-rw-r--r--   0 vadikus    (501) staff       (20)      152 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/encrypt/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4341 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/encrypt/enc_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6076 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/encrypt/enc_new_password_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      626 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/encrypt/enc_password.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4172 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/encrypt/enc_password_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3211 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/encrypt/enc_password_reset_dialog.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:36:17.548566 notolog-0.9.1b2/notolog/enums/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/enums/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1433 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/enums/ai_model_names.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5624 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/enums/colors.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1125 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/enums/enum_base.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1367 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/enums/languages.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      451 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/enums/themes.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4516 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/etree_extension.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:36:17.550237 notolog-0.9.1b2/notolog/exceptions/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/exceptions/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)       52 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/exceptions/file_header_empty_exception.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7559 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/file_header.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2856 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/file_system_watcher.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:36:17.558615 notolog-0.9.1b2/notolog/helpers/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/helpers/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      187 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/helpers/clipboard_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4227 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/helpers/file_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5511 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/helpers/theme_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1036 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/helpers/tooltip_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7411 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/helpers/update_helper.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:36:17.564013 notolog-0.9.1b2/notolog/highlight/
+-rw-r--r--   0 vadikus    (501) staff       (20)      126 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/highlight/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9213 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/highlight/main_highlighter.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    51699 2024-05-11 12:17:28.000000 notolog-0.9.1b2/notolog/highlight/md_highlighter.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8475 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/highlight/view_highlighter.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9909 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/image_downloader.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:36:17.566847 notolog-0.9.1b2/notolog/lexemes/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/__init__.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:36:17.574517 notolog-0.9.1b2/notolog/lexemes/de/
+-rw-r--r--   0 vadikus    (501) staff       (20)      830 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/de/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7202 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/de/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6586 2024-05-11 12:17:28.000000 notolog-0.9.1b2/notolog/lexemes/de/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2267 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/de/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3788 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/de/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1225 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/de/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2757 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/de/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:36:17.593010 notolog-0.9.1b2/notolog/lexemes/en/
+-rw-r--r--   0 vadikus    (501) staff       (20)      827 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/en/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7096 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/en/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6051 2024-05-11 12:17:28.000000 notolog-0.9.1b2/notolog/lexemes/en/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2181 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/en/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3586 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/en/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1201 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/en/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2573 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/en/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:36:17.602148 notolog-0.9.1b2/notolog/lexemes/es/
+-rw-r--r--   0 vadikus    (501) staff       (20)      882 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/es/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7309 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/es/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6560 2024-05-11 12:17:28.000000 notolog-0.9.1b2/notolog/lexemes/es/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2316 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/es/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3890 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/es/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1222 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/es/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2793 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/es/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:36:17.610151 notolog-0.9.1b2/notolog/lexemes/fi/
+-rw-r--r--   0 vadikus    (501) staff       (20)      856 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/fi/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7559 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/fi/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6292 2024-05-11 12:17:28.000000 notolog-0.9.1b2/notolog/lexemes/fi/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2261 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/fi/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3759 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/fi/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1334 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/fi/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2662 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/fi/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:36:17.619033 notolog-0.9.1b2/notolog/lexemes/fr/
+-rw-r--r--   0 vadikus    (501) staff       (20)      886 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/fr/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7247 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/fr/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6716 2024-05-11 12:17:28.000000 notolog-0.9.1b2/notolog/lexemes/fr/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2344 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/fr/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3978 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/fr/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1236 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/fr/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2824 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/fr/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:36:17.626454 notolog-0.9.1b2/notolog/lexemes/ge/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1323 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/ge/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    10627 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/ge/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9735 2024-05-11 12:17:28.000000 notolog-0.9.1b2/notolog/lexemes/ge/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3459 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/ge/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5742 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/ge/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1583 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/ge/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4107 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/ge/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:36:17.642596 notolog-0.9.1b2/notolog/lexemes/gr/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1100 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/gr/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8990 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/gr/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8668 2024-05-11 12:17:28.000000 notolog-0.9.1b2/notolog/lexemes/gr/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2907 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/gr/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5016 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/gr/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1561 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/gr/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3679 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/gr/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:36:17.650267 notolog-0.9.1b2/notolog/lexemes/in/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1208 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/in/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9434 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/in/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    10078 2024-05-11 12:17:28.000000 notolog-0.9.1b2/notolog/lexemes/in/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3124 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/in/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5546 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/in/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1549 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/in/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3828 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/in/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:36:17.658962 notolog-0.9.1b2/notolog/lexemes/it/
+-rw-r--r--   0 vadikus    (501) staff       (20)      864 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/it/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7263 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/it/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6366 2024-05-11 12:17:28.000000 notolog-0.9.1b2/notolog/lexemes/it/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2302 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/it/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3825 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/it/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1238 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/it/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2780 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/it/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:36:17.666519 notolog-0.9.1b2/notolog/lexemes/ja/
+-rw-r--r--   0 vadikus    (501) staff       (20)      931 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/ja/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8464 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/ja/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7248 2024-05-11 12:17:28.000000 notolog-0.9.1b2/notolog/lexemes/ja/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2443 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/ja/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4014 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/ja/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1242 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/ja/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3000 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/ja/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:36:17.673514 notolog-0.9.1b2/notolog/lexemes/ko/
+-rw-r--r--   0 vadikus    (501) staff       (20)      848 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/ko/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7597 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/ko/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6775 2024-05-11 12:17:28.000000 notolog-0.9.1b2/notolog/lexemes/ko/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2268 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/ko/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3697 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/ko/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1221 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/ko/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2666 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/ko/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:36:17.685415 notolog-0.9.1b2/notolog/lexemes/la/
+-rw-r--r--   0 vadikus    (501) staff       (20)      842 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/la/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7538 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/la/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6245 2024-05-11 12:17:28.000000 notolog-0.9.1b2/notolog/lexemes/la/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2297 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/la/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3753 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/la/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1257 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/la/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2736 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/la/toolbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3739 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/lexemes.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:36:17.699152 notolog-0.9.1b2/notolog/lexemes/nl/
+-rw-r--r--   0 vadikus    (501) staff       (20)      840 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/nl/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7094 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/nl/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6475 2024-05-11 12:17:28.000000 notolog-0.9.1b2/notolog/lexemes/nl/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2229 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/nl/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3673 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/nl/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1220 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/nl/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2647 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/nl/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:36:17.707205 notolog-0.9.1b2/notolog/lexemes/pt/
+-rw-r--r--   0 vadikus    (501) staff       (20)      898 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/pt/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7304 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/pt/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6357 2024-05-11 12:17:28.000000 notolog-0.9.1b2/notolog/lexemes/pt/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2326 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/pt/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3830 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/pt/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1223 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/pt/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2830 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/pt/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:36:17.715193 notolog-0.9.1b2/notolog/lexemes/ru/
+-rw-r--r--   0 vadikus    (501) staff       (20)      997 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/ru/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9135 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/ru/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7938 2024-05-11 12:17:28.000000 notolog-0.9.1b2/notolog/lexemes/ru/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2883 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/ru/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4896 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/ru/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1428 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/ru/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3453 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/ru/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:36:17.721644 notolog-0.9.1b2/notolog/lexemes/se/
+-rw-r--r--   0 vadikus    (501) staff       (20)      835 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/se/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7048 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/se/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6253 2024-05-11 12:17:28.000000 notolog-0.9.1b2/notolog/lexemes/se/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2216 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/se/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3627 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/se/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1220 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/se/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2611 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/se/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:36:17.729999 notolog-0.9.1b2/notolog/lexemes/tr/
+-rw-r--r--   0 vadikus    (501) staff       (20)      809 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/tr/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7401 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/tr/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6154 2024-05-11 12:17:28.000000 notolog-0.9.1b2/notolog/lexemes/tr/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2276 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/tr/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3733 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/tr/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1240 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/tr/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2735 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/tr/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:36:17.741221 notolog-0.9.1b2/notolog/lexemes/zh/
+-rw-r--r--   0 vadikus    (501) staff       (20)      792 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/zh/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7074 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/zh/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5777 2024-05-11 12:17:28.000000 notolog-0.9.1b2/notolog/lexemes/zh/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2175 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/zh/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3476 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/zh/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1202 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/zh/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2559 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/lexemes/zh/toolbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2860 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/main.py
+-rw-r--r--   0 vadikus    (501) staff       (20)   177588 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/notolog_editor.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6260 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/settings.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3481 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/text_block_data.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6022 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/theme.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:36:17.755694 notolog-0.9.1b2/notolog/ui/
+-rw-r--r--   0 vadikus    (501) staff       (20)      152 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/ui/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8224 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/ui/about_popup.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    16816 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/ui/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2099 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/ui/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3509 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/ui/common_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1306 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/ui/enum_combo_box.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5615 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/ui/file_system_model.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6999 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/ui/line_numbers.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2610 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/ui/rename_file_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1229 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/ui/rotating_label.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    37284 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/ui/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3197 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/ui/sort_filter_proxy_model.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6840 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/ui/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    12804 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/ui/toolbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      455 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/ui/vertical_line_spacer.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8191 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/view_decorator.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    16132 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/view_processor.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2446 2024-05-11 09:19:41.000000 notolog-0.9.1b2/notolog/view_widget.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:36:17.768388 notolog-0.9.1b2/notolog.egg-info/
+-rw-r--r--   0 vadikus    (501) staff       (20)    17100 2024-05-11 12:36:17.000000 notolog-0.9.1b2/notolog.egg-info/PKG-INFO
+-rw-r--r--   0 vadikus    (501) staff       (20)    11426 2024-05-11 12:36:17.000000 notolog-0.9.1b2/notolog.egg-info/SOURCES.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)        1 2024-05-11 12:36:17.000000 notolog-0.9.1b2/notolog.egg-info/dependency_links.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)       46 2024-05-11 12:36:17.000000 notolog-0.9.1b2/notolog.egg-info/entry_points.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)      297 2024-05-11 12:36:17.000000 notolog-0.9.1b2/notolog.egg-info/requires.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)       14 2024-05-11 12:36:17.000000 notolog-0.9.1b2/notolog.egg-info/top_level.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)      297 2024-05-06 20:09:20.000000 notolog-0.9.1b2/requirements.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)       38 2024-05-11 12:36:17.770209 notolog-0.9.1b2/setup.cfg
+-rw-r--r--   0 vadikus    (501) staff       (20)     2377 2024-05-11 12:17:28.000000 notolog-0.9.1b2/setup.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-11 12:36:17.767634 notolog-0.9.1b2/tests/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:31.000000 notolog-0.9.1b2/tests/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5983 2024-05-11 09:19:41.000000 notolog-0.9.1b2/tests/test_enc_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2309 2024-05-11 09:19:41.000000 notolog-0.9.1b2/tests/test_enc_password.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9888 2024-05-11 09:19:41.000000 notolog-0.9.1b2/tests/test_file_header.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3974 2024-05-11 09:19:41.000000 notolog-0.9.1b2/tests/test_html_view.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5814 2024-05-11 09:19:41.000000 notolog-0.9.1b2/tests/test_lexemes.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5839 2024-05-11 09:19:41.000000 notolog-0.9.1b2/tests/test_notolog_editor.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1943 2024-05-11 09:19:41.000000 notolog-0.9.1b2/tests/test_pkg_integration.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1178 2024-05-11 09:19:41.000000 notolog-0.9.1b2/tests/test_settings.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4975 2024-05-11 09:19:41.000000 notolog-0.9.1b2/tests/test_text_block_data.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4484 2024-05-11 09:19:41.000000 notolog-0.9.1b2/tests/test_theme_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6226 2024-05-11 09:19:41.000000 notolog-0.9.1b2/tests/test_themes.py
```

### Comparing `notolog-0.9.1b1/CHANGELOG.md` & `notolog-0.9.1b2/CHANGELOG.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,60 @@
 # Changelog
 All notologable changes to this project will be documented in this file.
 
+## [0.9.1b2] - 2024-05-11
+
+### Added
+- Introduced the [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) file to promote a respectful and positive environment for all contributors and participants. This document outlines our commitment to providing a harassment-free experience for everyone and offers guidelines for respectful communication practices.
+- Support for highlighting tables in markdown edit mode, enhancing the editing experience.
+- A new EnumBase class to incorporate common methods across enums, improving code reusability.
+- Additional tests to increase coverage and ensure the stability of new features.
+
+### Changed
+- Renamed the main package directory from app to notolog and moved main.py into the notolog directory to better reflect the project structure.
+- Refined the handling of external and local links, as well as local files, now routing them through a unified links router for improved security and consistency.
+- Updated the table styles in view mode across all themes for more consistent visual presentation.
+- Eliminated the need for a preliminary empty line to highlight lists in markdown edit mode, enhancing the user experience by simplifying text formatting.
+
+### Updated
+- Enhanced the language selection mechanism to prefer the system language by default, with a fallback to a predefined language if the system language is not available.
+- Optimized the checking of image downloader statuses and the updating of signal processing for increased performance and reliability.
+
+### Fixed
+- Corrected the processing for confirming external links to eliminate unintended navigational behaviors and enhance user security.
+- Various minor fixes to address small issues in the codebase, enhancing stability and performance without significantly changing functionality.
+
 ## [0.9.1b1] - 2024-05-06
+
 ### Added
 - New interface language: Dutch
 
 ### Updated
 - Upgraded `cryptography` to version 42.0.7 to align with the latest standards and enhance security.
 
 ### Changed
 - Updated requirements.txt to match the actual package list.
 
 ## [0.9.1b0] - 2024-05-05
+
 ### Added
 - New interface languages: Finnish and Swedish, expanding accessibility for users in these regions.
 - Additional entries to the `.gitignore` and `.gitattributes` files to improve version control practices.
 - A dedicated `app_config.toml` file with initial configuration parameters, simplifying initial setup and customization.
 
 ### Updated
-- Updated the `Libraries and Licenses` section within the README.md file to provide comprehensive information about third-party dependencies and their licenses.
+- Updated the `Libraries and Licenses` section within the [README.md](README.md) file to provide comprehensive information about third-party dependencies and their licenses.
 - Updated `cryptography` to version 42.0.6 and `Pygments` to version 2.18.0 to ensure compatibility with the latest standards and to incorporate the newest features and security enhancements.
 
 ### Changed
 - Modified file handling: The file header can now be the only content of the file, streamlining setups where minimal data is required.
 - Updated encryption description to clarify that Fernet uses AES-128 for encryption, derived from a 256-bit key, accurately reflecting the cryptographic standards employed.
 
 ## [0.9.0b11] - 2024-05-04
+
 ### Added
 - Support for embedding external images within documents, with caching.
 - Option to auto-save downloaded image resources on local disk and reuse them in subsequent document sessions.
 - New interface languages: Greek, Hindi, Turkish.
 - Expanded example content and resources.
 - Added `CHANGELOG.md` to document all notable changes to the project, enhancing transparency and trackability for developers and users alike.
 
@@ -42,21 +67,23 @@
 - Minor logo adjustment.
 
 ### Fixed
 - Resolved sudden crashes when switching between edit and view modes.
 - Addressed UI style issues for improved text visibility under various color schemes.
 
 ## [0.9.0b10] - 2024-04-29
+
 ### Changed
 - Updated pip installer related packages and file structure.
 
 ### Fixed
 - Corrected startup failures following pip installation.
 
 ## [0.9.0b0] - 2024-04-29
+
 ### Added
 - Initial release features, open sourced under the MIT license for full transparency and collaboration.
 - Markdown syntax highlighting:
     - Editor mode offers smooth highlighting tailored specifically for Notolog by our development team, including line numbers and extended syntax highlighting.
     - View mode utilizes the Python Markdown library for seamless rendering of Markdown syntax.
     - Supports multi-line block open-close tokens for enhanced readability and structure.
 - Multi-platform support: Compatible with all major platforms where Python is installed, ensuring accessibility across operating systems.
```

### Comparing `notolog-0.9.1b1/LICENSE` & `notolog-0.9.1b2/LICENSE`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/PKG-INFO` & `notolog-0.9.1b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: notolog
-Version: 0.9.1b1
-Summary: Notolog Markdown Editor
+Version: 0.9.1b2
+Summary: Notolog - Python Markdown Editor
 Home-page: https://github.com/notolog/notolog-editor
 Author: Vadim Bakhrenkov
 License: MIT
 Project-URL: Bug Reports, https://github.com/notolog/notolog-editor/issues
 Project-URL: Source, https://github.com/notolog/notolog-editor/
-Keywords: notolog,ai,markdown,editor
+Keywords: notolog,python,markdown,editor,ai,text
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
@@ -47,18 +47,18 @@
 Requires-Dist: PySide6_Essentials==6.7.0
 Requires-Dist: pytest==8.2.0
 Requires-Dist: pytest-mock==3.14.0
 Requires-Dist: qasync==0.27.1
 Requires-Dist: shiboken6==6.7.0
 Requires-Dist: tomli==2.0.1
 
-<!-- {"notolog.app": {"created": "2023-12-25 18:59:43.806614", "updated": "2024-05-06 21:20:54.001715"}} -->
+<!-- {"notolog.app": {"created": "2023-12-25 18:59:43.806614", "updated": "2024-05-11 11:15:29.656338"}} -->
 # Notolog
 
-![Notolog](https://raw.githubusercontent.com/notolog/notolog-editor/main/app/assets/notolog-example-image.png)&nbsp;&nbsp;&nbsp;![PyPI - Version](https://img.shields.io/pypi/v/notolog) ![PyPI - License](https://img.shields.io/pypi/l/notolog) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/notolog)
+![Notolog](https://raw.githubusercontent.com/notolog/notolog-editor/main/notolog/assets/notolog-example-image.png)&nbsp;&nbsp;&nbsp;![PyPI - Version](https://img.shields.io/pypi/v/notolog) ![PyPI - License](https://img.shields.io/pypi/l/notolog) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/notolog)
 
 ## Overview
 
 Notolog is a versatile open-source markdown editor developed with Python and Qt, ideal for anyone looking for an efficient and straightforward way to handle markdown files. Born from a personal endeavor to address daily programming challenges and deepen Python proficiency, Notolog stands as a proof-of-concept that seamlessly integrates simplicity with functionality, offering an intuitive user experience across various platforms.
 
 ---
 ![Notolog settings UI example](https://raw.githubusercontent.com/notolog/notolog-editor/main/docs/notolog-ui-settings.png)
@@ -77,20 +77,20 @@
 	* Font size adjustment for better readability.
 * Background and cross-action save changes experience:
 	* Automatically saves changes in the background to ensure data integrity and minimize user intervention.
 	* Seamlessly handles unsaved changes when performing cross-actions, providing a smooth user experience.
 * Search functionality:
 	* Allows users to search within the opened file.
 	* Quick search by file name within the tree, enabling efficient navigation and content retrieval.
-* File meta-headers in the form of HTML comments to avoid excess visibility.
 * Password-based File Encryption and Decryption:
 	* Utilizes Fernet for encryption, providing a secure and user-friendly method for symmetric (also known as "secret key") encryption.
 	* Fernet employs AES-128 in CBC mode. Plans to introduce AES-256 in future updates are aimed at further enhancing security.
 * File Meta-Headers:
-	* Notolog implements file meta-headers to store encryption parameters, ensuring a seamless decryption process.
+	* Notolog employs file meta-headers to store encryption/decryption parameters and other essential file information.
+	* To minimize visibility, these meta-headers are formatted as HTML comments.
 * Translations-friendly file structure:
 	* Supports several languages out of the box, with provisions for adding and supporting additional languages.
 * Color themes support:
 	* Comes with a few predefined color themes to customize the editor's appearance, for both light and dark modes.
 * Hotkeys support:
 	* It currently supports hotkeys like Ctrl+S for saving and Ctrl+F for searching, with plans for further expansion.
 * In-line context menus:
@@ -110,15 +110,15 @@
 
 If you haven't already, download and install Python from the official website [python.org](python.org).
 
 Check the version of Python available with this command `python3 -V`.
 
 **pip (Python package installer) should be available.**
 
-You can check if pip is installed by running `pip3 --version` in your terminal/command prompt.
+You can check if pip is installed by running `pip --version` in your terminal/command prompt.
 
 **Virtual Environment**
 
 It is highly recommended to use as it helps avoid version conflicts and interference from other packages. Below is a description of how to set up a virtual environment on your machine.
 
 
 ## Installation
@@ -142,18 +142,18 @@
 1. Clone project's GitHub repository to get a latest version.
 	* `git clone https://github.com/notolog/notolog-editor.git`
 2. Navigate to the just cloned project's directory using the **cd** command.
 3. Make sure the virtual environment is activated as it's a common practice to isolate project code (activation described below).
 4. Simply run this command to set up project dependencies:
 
 ```sh
-pip3 install -r requirements.txt
+pip install -r requirements.txt
 ```
 
-That's it! Starting the app is as simple as `python3 main.py`
+That's it! Starting the app is as simple as `python -m notolog.main` form the project's root directory.
 
 <details>
 <summary>Run tests</summary>
 
 To run all available tests:
 ```sh
 pytest
```

### Comparing `notolog-0.9.1b1/README.md` & `notolog-0.9.1b2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-<!-- {"notolog.app": {"created": "2023-12-25 18:59:43.806614", "updated": "2024-05-06 21:20:54.001715"}} -->
+<!-- {"notolog.app": {"created": "2023-12-25 18:59:43.806614", "updated": "2024-05-11 11:15:29.656338"}} -->
 # Notolog
 
-![Notolog](https://raw.githubusercontent.com/notolog/notolog-editor/main/app/assets/notolog-example-image.png)&nbsp;&nbsp;&nbsp;![PyPI - Version](https://img.shields.io/pypi/v/notolog) ![PyPI - License](https://img.shields.io/pypi/l/notolog) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/notolog)
+![Notolog](https://raw.githubusercontent.com/notolog/notolog-editor/main/notolog/assets/notolog-example-image.png)&nbsp;&nbsp;&nbsp;![PyPI - Version](https://img.shields.io/pypi/v/notolog) ![PyPI - License](https://img.shields.io/pypi/l/notolog) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/notolog)
 
 ## Overview
 
 Notolog is a versatile open-source markdown editor developed with Python and Qt, ideal for anyone looking for an efficient and straightforward way to handle markdown files. Born from a personal endeavor to address daily programming challenges and deepen Python proficiency, Notolog stands as a proof-of-concept that seamlessly integrates simplicity with functionality, offering an intuitive user experience across various platforms.
 
 ---
 ![Notolog settings UI example](https://raw.githubusercontent.com/notolog/notolog-editor/main/docs/notolog-ui-settings.png)
@@ -24,20 +24,20 @@
 	* Font size adjustment for better readability.
 * Background and cross-action save changes experience:
 	* Automatically saves changes in the background to ensure data integrity and minimize user intervention.
 	* Seamlessly handles unsaved changes when performing cross-actions, providing a smooth user experience.
 * Search functionality:
 	* Allows users to search within the opened file.
 	* Quick search by file name within the tree, enabling efficient navigation and content retrieval.
-* File meta-headers in the form of HTML comments to avoid excess visibility.
 * Password-based File Encryption and Decryption:
 	* Utilizes Fernet for encryption, providing a secure and user-friendly method for symmetric (also known as "secret key") encryption.
 	* Fernet employs AES-128 in CBC mode. Plans to introduce AES-256 in future updates are aimed at further enhancing security.
 * File Meta-Headers:
-	* Notolog implements file meta-headers to store encryption parameters, ensuring a seamless decryption process.
+	* Notolog employs file meta-headers to store encryption/decryption parameters and other essential file information.
+	* To minimize visibility, these meta-headers are formatted as HTML comments.
 * Translations-friendly file structure:
 	* Supports several languages out of the box, with provisions for adding and supporting additional languages.
 * Color themes support:
 	* Comes with a few predefined color themes to customize the editor's appearance, for both light and dark modes.
 * Hotkeys support:
 	* It currently supports hotkeys like Ctrl+S for saving and Ctrl+F for searching, with plans for further expansion.
 * In-line context menus:
@@ -57,15 +57,15 @@
 
 If you haven't already, download and install Python from the official website [python.org](python.org).
 
 Check the version of Python available with this command `python3 -V`.
 
 **pip (Python package installer) should be available.**
 
-You can check if pip is installed by running `pip3 --version` in your terminal/command prompt.
+You can check if pip is installed by running `pip --version` in your terminal/command prompt.
 
 **Virtual Environment**
 
 It is highly recommended to use as it helps avoid version conflicts and interference from other packages. Below is a description of how to set up a virtual environment on your machine.
 
 
 ## Installation
@@ -89,18 +89,18 @@
 1. Clone project's GitHub repository to get a latest version.
 	* `git clone https://github.com/notolog/notolog-editor.git`
 2. Navigate to the just cloned project's directory using the **cd** command.
 3. Make sure the virtual environment is activated as it's a common practice to isolate project code (activation described below).
 4. Simply run this command to set up project dependencies:
 
 ```sh
-pip3 install -r requirements.txt
+pip install -r requirements.txt
 ```
 
-That's it! Starting the app is as simple as `python3 main.py`
+That's it! Starting the app is as simple as `python -m notolog.main` form the project's root directory.
 
 <details>
 <summary>Run tests</summary>
 
 To run all available tests:
 ```sh
 pytest
```

### Comparing `notolog-0.9.1b1/app/app_config.py` & `notolog-0.9.1b2/notolog/app_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import tomli
 
 toml_base_app_config = """
 [app]
 name = "Notolog"
-version = "0.9.1b1"
+version = "0.9.1b2"
 license = "MIT"
 date = "2024"
 website = "https://notolog.app"
 repository = "https://github.com/notolog/notolog-editor"
 pypi = "https://pypi.org/project/notolog"
 author = "Vadim Bakhrenkov"
```

### Comparing `notolog-0.9.1b1/app/assets/notolog-example-image.png` & `notolog-0.9.1b2/notolog/assets/notolog-example-image.png`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/assets/notolog-logo.png` & `notolog-0.9.1b2/notolog/assets/notolog-logo.png`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/assets/themes/calligraphy/about_popup.css` & `notolog-0.9.1b2/notolog/assets/themes/calligraphy/about_popup.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/assets/themes/calligraphy/default.ini` & `notolog-0.9.1b2/notolog/assets/themes/calligraphy/default.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/assets/themes/calligraphy/md.ini` & `notolog-0.9.1b2/notolog/assets/themes/calligraphy/md.ini`

 * *Files 10% similar despite different names*

```diff
@@ -43,14 +43,18 @@
 md_background_color_code_indent=black
 md_color_code_content=black
 md_background_color_code_content=whitesmoke
 md_color_wrong_indent=
 md_background_color_wrong_indent=black
 md_color_comment=grey
 md_background_color_comment=white
+md_color_table_h=whitesmoke
+md_background_color_table_h=black
+md_color_table_d=black
+md_background_color_table_d=whitesmoke
 md_color_img=black
 md_color_ref=white
 md_background_color_ref=black
 md_color_abbr=white
 md_background_color_abbr=black
 md_color_abbr_text=white
 md_background_color_abbr_text=black
```

### Comparing `notolog-0.9.1b1/app/assets/themes/calligraphy/settings_dialog.css` & `notolog-0.9.1b2/notolog/assets/themes/calligraphy/settings_dialog.css`

 * *Files 3% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 QTabBar::tab:selected {
     color: red;
 }
 QComboBox {}
 QLabel {
     color: black;
 }
-QLineEdit {
-    color: gray;
-}
+QLineEdit {}
 /* Group titles, todo somehow distinguish them without id */
 QLabel#settings_dialog_general_app_config_label,
 QLabel#settings_dialog_general_app_main_menu_label,
 QLabel#settings_dialog_general_statusbar_label,
 QLabel#settings_dialog_general_app_font_size_label,
 QLabel#settings_dialog_editor_config_label,
 QLabel#settings_dialog_viewer_config_label,
```

### Comparing `notolog-0.9.1b1/app/assets/themes/calligraphy/styles.css` & `notolog-0.9.1b2/notolog/assets/themes/calligraphy/styles.css`

 * *Files 9% similar despite different names*

```diff
@@ -20,14 +20,36 @@
 h1 { font-size: xx-large; }
 h2 { font-size: x-large; }
 h3 { font-size: large; }
 h4 { font-size: medium; }
 h5 { font-size: small; }
 h6 { font-size: 8pt; font-weight: bold; }
 
+/* Markdown table */
+table._nl_tbl {
+    margin-top: 10px;
+    border-collapse: collapse;
+    border: 1px solid black;
+}
+table._nl_tbl td {
+    border: 1px solid black;
+    padding: 5px;
+}
+table._nl_tbl th {
+    border: 1px solid black;
+    background: whitesmoke;
+    color: black;
+    font-weight: bold;
+    padding: 5px;
+}
+/* Style substitution for tree-processor */
+._nl_tbl .left { text-align: left; }
+._nl_tbl .center { text-align: center; }
+._nl_tbl .right { text-align: right; }
+
 /* Expandable block, which replaces the <details><summary>...</summary>...</details> with:
 <p class="_ds_expand">
 <a href="expandable:{}" data-group="{}" data-level="{}">▼{}</a>
 </p>
 */
 /* Expanded block (collapsible), which appears after expandable block click:
 <table class="_n_details">
```

#### html2text {}

```diff
@@ -2,15 +2,21 @@
 family: 'Arial', 'Liberation Sans', sans-serif; line-height: 23px; } a
 { display: inline-block; } /* Fix new line issue within the p block */ p
 { white-space: pre-line; } pre { /*display: block; white-space: pre; max-width:
 100%; text-indent: 20px; margin: 10px;*/ } img { max-width: 100%; } a { color:
 red; } /* Somehow h5 and h6 are not balanced. Hence h6 adjusted in pt */ h1
 { font-size: xx-large; } h2 { font-size: x-large; } h3 { font-size: large; } h4
 { font-size: medium; } h5 { font-size: small; } h6 { font-size: 8pt; font-
-weight: bold; } /* Expandable block, which replaces the ...... with:
+weight: bold; } /* Markdown table */ table._nl_tbl { margin-top: 10px; border-
+collapse: collapse; border: 1px solid black; } table._nl_tbl td { border: 1px
+solid black; padding: 5px; } table._nl_tbl th { border: 1px solid black;
+background: whitesmoke; color: black; font-weight: bold; padding: 5px; } /
+* Style substitution for tree-processor */ ._nl_tbl .left { text-align: left; }
+._nl_tbl .center { text-align: center; } ._nl_tbl .right { text-align: right; }
+/* Expandable block, which replaces the ...... with:
 _â__¼_{_}
 */ /* Expanded block (collapsible), which appears after expandable block click:
 {}
 {}
 */ /* anchor details-summary common */ ._ds_expand { border: 1px solid grey
 !important; background: transparent; } /* anchor details-summary expandable */
 ._ds_expand > a { color: black; text-decoration: none; font-weight: bold; }
```

### Comparing `notolog-0.9.1b1/app/assets/themes/calligraphy/tree_view.css` & `notolog-0.9.1b2/notolog/assets/themes/calligraphy/tree_view.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/assets/themes/default/about_popup.css` & `notolog-0.9.1b2/notolog/assets/themes/default/about_popup.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/assets/themes/default/default.ini` & `notolog-0.9.1b2/notolog/assets/themes/default/default.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/assets/themes/default/icons/LICENSE` & `notolog-0.9.1b2/notolog/assets/themes/default/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/assets/themes/default/icons/arrow-repeat.svg` & `notolog-0.9.1b2/notolog/assets/themes/default/icons/arrow-repeat.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/assets/themes/default/icons/balloon-fill.svg` & `notolog-0.9.1b2/notolog/assets/themes/default/icons/balloon-fill.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/assets/themes/default/icons/balloon.svg` & `notolog-0.9.1b2/notolog/assets/themes/default/icons/balloon.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/assets/themes/default/icons/bandaid-fill.svg` & `notolog-0.9.1b2/notolog/assets/themes/default/icons/bandaid-fill.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/assets/themes/default/icons/bandaid.svg` & `notolog-0.9.1b2/notolog/assets/themes/default/icons/bandaid.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/assets/themes/default/icons/box-arrow-up-right.svg` & `notolog-0.9.1b2/notolog/assets/themes/default/icons/box-arrow-up-right.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/assets/themes/default/icons/box-arrow-up.svg` & `notolog-0.9.1b2/notolog/assets/themes/default/icons/box-arrow-up.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/assets/themes/default/icons/cursor-text.svg` & `notolog-0.9.1b2/notolog/assets/themes/default/icons/cursor-text.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/assets/themes/default/icons/filetype-html.svg` & `notolog-0.9.1b2/notolog/assets/themes/default/icons/filetype-html.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/assets/themes/default/icons/filetype-md.svg` & `notolog-0.9.1b2/notolog/assets/themes/default/icons/filetype-md.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/assets/themes/default/icons/filetype-txt.svg` & `notolog-0.9.1b2/notolog/assets/themes/default/icons/filetype-txt.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/assets/themes/default/icons/floppy2.svg` & `notolog-0.9.1b2/notolog/assets/themes/default/icons/floppy2.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/assets/themes/default/icons/folder-symlink.svg` & `notolog-0.9.1b2/notolog/assets/themes/default/icons/folder-symlink.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/assets/themes/default/icons/folder.svg` & `notolog-0.9.1b2/notolog/assets/themes/default/icons/folder.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/assets/themes/default/icons/github.svg` & `notolog-0.9.1b2/notolog/assets/themes/default/icons/github.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/assets/themes/default/icons/link-45deg.svg` & `notolog-0.9.1b2/notolog/assets/themes/default/icons/link-45deg.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/assets/themes/default/icons/linkedin.svg` & `notolog-0.9.1b2/notolog/assets/themes/default/icons/linkedin.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/assets/themes/default/icons/pencil-square.svg` & `notolog-0.9.1b2/notolog/assets/themes/default/icons/pencil-square.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/assets/themes/default/icons/quote.svg` & `notolog-0.9.1b2/notolog/assets/themes/default/icons/quote.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/assets/themes/default/icons/robot.svg` & `notolog-0.9.1b2/notolog/assets/themes/default/icons/robot.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/assets/themes/default/icons/shield-lock-fill.svg` & `notolog-0.9.1b2/notolog/assets/themes/default/icons/shield-lock-fill.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/assets/themes/default/icons/shield-lock.svg` & `notolog-0.9.1b2/notolog/assets/themes/default/icons/shield-lock.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/assets/themes/default/icons/star.svg` & `notolog-0.9.1b2/notolog/assets/themes/default/icons/star.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/assets/themes/default/icons/trash3-fill.svg` & `notolog-0.9.1b2/notolog/assets/themes/default/icons/trash3-fill.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/assets/themes/default/icons/trash3.svg` & `notolog-0.9.1b2/notolog/assets/themes/default/icons/trash3.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/assets/themes/default/icons/type-strikethrough.svg` & `notolog-0.9.1b2/notolog/assets/themes/default/icons/type-strikethrough.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/assets/themes/default/md.ini` & `notolog-0.9.1b2/notolog/assets/themes/default/md.ini`

 * *Files 6% similar despite different names*

```diff
@@ -42,14 +42,18 @@
 md_color_code_indent=
 md_background_color_code_indent=pink
 md_color_code_content=brown
 md_color_wrong_indent=
 md_background_color_wrong_indent=red
 md_color_comment=grey
 md_background_color_comment=lightGrey
+md_color_table_h=
+md_background_color_table_h=lightGrey
+md_color_table_d=
+md_background_color_table_d=whiteSmoke
 md_color_img=green
 md_color_ref=white
 md_background_color_ref=green
 md_color_abbr=white
 md_background_color_abbr=dodgerBlue
 md_color_abbr_text=white
 md_background_color_abbr_text=dodgerBlue
```

### Comparing `notolog-0.9.1b1/app/assets/themes/default/settings_dialog.css` & `notolog-0.9.1b2/notolog/assets/themes/default/settings_dialog.css`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 /* Tabs */
 QTabBar::tab {}
 /* Active tab */
 QTabBar::tab:selected {}
 QComboBox {}
 QLabel {}
-QLineEdit {
-    color: gray;
-}
+QLineEdit {}
 /* Group titles */
 QLabel#settings_dialog_general_app_config_label,
 QLabel#settings_dialog_general_app_main_menu_label,
 QLabel#settings_dialog_general_statusbar_label,
 QLabel#settings_dialog_general_app_font_size_label,
 QLabel#settings_dialog_editor_config_label,
 QLabel#settings_dialog_viewer_config_label,
```

### Comparing `notolog-0.9.1b1/app/assets/themes/default/styles.css` & `notolog-0.9.1b2/notolog/assets/themes/default/styles.css`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,36 @@
 h1 { font-size: xx-large; }
 h2 { font-size: x-large; }
 h3 { font-size: large; }
 h4 { font-size: medium; }
 h5 { font-size: small; }
 h6 { font-size: 8pt; font-weight: bold; }
 
+/* Markdown table */
+table._nl_tbl {
+    margin-top: 10px;
+    border-collapse: collapse;
+    border: 1px solid grey;
+}
+table._nl_tbl td {
+    border: 1px solid grey;
+    padding: 5px;
+}
+table._nl_tbl th {
+    border: 1px solid grey;
+    background: lightgrey;
+    color: darkSlateGrey;
+    font-weight: bold;
+    padding: 5px;
+}
+/* Style substitution for tree-processor */
+._nl_tbl .left { text-align: left; }
+._nl_tbl .center { text-align: center; }
+._nl_tbl .right { text-align: right; }
+
 /* Expandable block, which replaces the <details><summary>...</summary>...</details> with:
 <p class="_ds_expand">
 <a href="expandable:{}" data-group="{}" data-level="{}">▼{}</a>
 </p>
 */
 /* Expanded block (collapsible), which appears after expandable block click:
 <table class="_n_details">
```

#### html2text {}

```diff
@@ -2,15 +2,21 @@
 family: 'Arial', 'Liberation Sans', sans-serif; line-height: 23px; } a
 { display: inline-block; } /* Fix new line issue within the p block */ p
 { white-space: pre-line; } pre { /*display: block; white-space: pre; max-width:
 100%; text-indent: 20px; margin: 10px;*/ } img { max-width: 100%; } a { color:
 royalblue; } /* Somehow h5 and h6 are not balanced. Hence h6 adjusted in pt */
 h1 { font-size: xx-large; } h2 { font-size: x-large; } h3 { font-size: large; }
 h4 { font-size: medium; } h5 { font-size: small; } h6 { font-size: 8pt; font-
-weight: bold; } /* Expandable block, which replaces the ...... with:
+weight: bold; } /* Markdown table */ table._nl_tbl { margin-top: 10px; border-
+collapse: collapse; border: 1px solid grey; } table._nl_tbl td { border: 1px
+solid grey; padding: 5px; } table._nl_tbl th { border: 1px solid grey;
+background: lightgrey; color: darkSlateGrey; font-weight: bold; padding: 5px; }
+/* Style substitution for tree-processor */ ._nl_tbl .left { text-align: left;
+} ._nl_tbl .center { text-align: center; } ._nl_tbl .right { text-align: right;
+} /* Expandable block, which replaces the ...... with:
 _â__¼_{_}
 */ /* Expanded block (collapsible), which appears after expandable block click:
 {}
 {}
 */ /* anchor details-summary common */ ._ds_expand { border: 1px solid grey
 !important; background: transparent; } /* anchor details-summary expandable */
 ._ds_expand > a { color: black; text-decoration: none; font-weight: bold; }
```

### Comparing `notolog-0.9.1b1/app/assets/themes/default/tree_view.css` & `notolog-0.9.1b2/notolog/assets/themes/default/tree_view.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/assets/themes/noir_dark/about_popup.css` & `notolog-0.9.1b2/notolog/assets/themes/noir_dark/about_popup.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/assets/themes/noir_dark/default.ini` & `notolog-0.9.1b2/notolog/assets/themes/noir_dark/default.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/assets/themes/noir_dark/md.ini` & `notolog-0.9.1b2/notolog/assets/themes/noir_dark/md.ini`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,18 @@
 md_color_code_indent=
 md_background_color_code_indent=whitesmoke
 md_color_code_content=whitesmoke
 md_color_wrong_indent=
 md_background_color_wrong_indent=whitesmoke
 md_color_comment=grey
 md_background_color_comment=black
+md_color_table_h=whiteSmoke
+md_background_color_table_h=grey
+md_color_table_d=whiteSmoke
+md_background_color_table_d=black
 md_color_img=whitesmoke
 md_color_ref=black
 md_background_color_ref=whitesmoke
 md_color_abbr=black
 md_background_color_abbr=whitesmoke
 md_color_abbr_text=black
 md_background_color_abbr_text=whitesmoke
```

### Comparing `notolog-0.9.1b1/app/assets/themes/noir_dark/settings_dialog.css` & `notolog-0.9.1b2/notolog/assets/themes/noir_dark/settings_dialog.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/assets/themes/noir_dark/styles.css` & `notolog-0.9.1b2/notolog/assets/themes/noir_dark/styles.css`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,36 @@
 h1 { font-size: xx-large; }
 h2 { font-size: x-large; }
 h3 { font-size: large; }
 h4 { font-size: medium; }
 h5 { font-size: small; }
 h6 { font-size: 8pt; font-weight: bold; }
 
+/* Markdown table */
+table._nl_tbl {
+    margin-top: 10px;
+    border-collapse: collapse;
+    border: 1px solid whitesmoke;
+}
+table._nl_tbl td {
+    border: 1px solid whitesmoke;
+    padding: 5px;
+}
+table._nl_tbl th {
+    border: 1px solid whitesmoke;
+    background: grey;
+    color: whitesmoke;
+    font-weight: bold;
+    padding: 5px;
+}
+/* Style substitution for tree-processor */
+._nl_tbl .left { text-align: left; }
+._nl_tbl .center { text-align: center; }
+._nl_tbl .right { text-align: right; }
+
 /* Expandable block, which replaces the <details><summary>...</summary>...</details> with:
 <p class="_ds_expand">
 <a href="expandable:{}" data-group="{}" data-level="{}">▼{}</a>
 </p>
 */
 /* Expanded block (collapsible), which appears after expandable block click:
 <table class="_n_details">
```

#### html2text {}

```diff
@@ -2,15 +2,21 @@
 family: 'Arial', 'Liberation Sans', sans-serif; line-height: 23px; } a
 { display: inline-block; } /* Fix new line issue within the p block */ p
 { white-space: pre-line; } pre { /*display: block; white-space: pre; max-width:
 100%; text-indent: 20px; margin: 10px;*/ } img { max-width: 100%; } a { color:
 red; } /* Somehow h5 and h6 are not balanced. Hence h6 adjusted in pt */ h1
 { font-size: xx-large; } h2 { font-size: x-large; } h3 { font-size: large; } h4
 { font-size: medium; } h5 { font-size: small; } h6 { font-size: 8pt; font-
-weight: bold; } /* Expandable block, which replaces the ...... with:
+weight: bold; } /* Markdown table */ table._nl_tbl { margin-top: 10px; border-
+collapse: collapse; border: 1px solid whitesmoke; } table._nl_tbl td { border:
+1px solid whitesmoke; padding: 5px; } table._nl_tbl th { border: 1px solid
+whitesmoke; background: grey; color: whitesmoke; font-weight: bold; padding:
+5px; } /* Style substitution for tree-processor */ ._nl_tbl .left { text-align:
+left; } ._nl_tbl .center { text-align: center; } ._nl_tbl .right { text-align:
+right; } /* Expandable block, which replaces the ...... with:
 _â__¼_{_}
 */ /* Expanded block (collapsible), which appears after expandable block click:
 {}
 {}
 */ /* anchor details-summary common */ ._ds_expand { border: 1px solid grey
 !important; background: transparent; } /* anchor details-summary expandable */
 ._ds_expand > a { color: whitesmoke; text-decoration: none; font-weight: bold;
```

### Comparing `notolog-0.9.1b1/app/assets/themes/noir_dark/tree_view.css` & `notolog-0.9.1b2/notolog/assets/themes/noir_dark/tree_view.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/assets/themes/strawberry/about_popup.css` & `notolog-0.9.1b2/notolog/assets/themes/strawberry/about_popup.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/assets/themes/strawberry/default.ini` & `notolog-0.9.1b2/notolog/assets/themes/strawberry/default.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/assets/themes/strawberry/md.ini` & `notolog-0.9.1b2/notolog/assets/themes/strawberry/md.ini`

 * *Files 8% similar despite different names*

```diff
@@ -42,14 +42,18 @@
 md_color_code_indent=
 md_background_color_code_indent=pink
 md_color_code_content=brown
 md_color_wrong_indent=
 md_background_color_wrong_indent=red
 md_color_comment=grey
 md_background_color_comment=lightGrey
+md_color_table_h=lightPink
+md_background_color_table_h=mediumVioletRed
+md_color_table_d=mediumVioletRed
+md_background_color_table_d=#fff7f7
 md_color_img=green
 md_color_ref=white
 md_background_color_ref=green
 md_color_abbr=white
 md_background_color_abbr=hotPink
 md_color_abbr_text=white
 md_background_color_abbr_text=hotPink
```

### Comparing `notolog-0.9.1b1/app/assets/themes/strawberry/settings_dialog.css` & `notolog-0.9.1b2/notolog/assets/themes/strawberry/settings_dialog.css`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 /* Tabs */
 QTabBar::tab {}
 /* Active tab */
 QTabBar::tab:selected {}
 QComboBox {}
 QLabel {}
-QLineEdit {
-    color: gray;
-}
+QLineEdit {}
 /* Group titles */
 QLabel#settings_dialog_general_app_config_label,
 QLabel#settings_dialog_general_app_main_menu_label,
 QLabel#settings_dialog_general_statusbar_label,
 QLabel#settings_dialog_general_app_font_size_label,
 QLabel#settings_dialog_editor_config_label,
 QLabel#settings_dialog_viewer_config_label,
```

### Comparing `notolog-0.9.1b1/app/assets/themes/strawberry/styles.css` & `notolog-0.9.1b2/notolog/assets/themes/strawberry/styles.css`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,35 @@
 h1 { font-size: xx-large; }
 h2 { font-size: x-large; }
 h3 { font-size: large; }
 h4 { font-size: medium; }
 h5 { font-size: small; }
 h6 { font-size: 8pt; font-weight: bold; }
 
+/* Markdown table */
+table._nl_tbl {
+    margin-top: 10px;
+    border-collapse: collapse;
+}
+table._nl_tbl td {
+    border: 1px solid mediumvioletred;
+    padding: 5px;
+}
+table._nl_tbl th {
+    border: 1px solid mediumvioletred;
+    background: lightpink;
+    color: mediumvioletred;
+    font-weight: bold;
+    padding: 5px;
+}
+/* Style substitution for tree-processor */
+._nl_tbl .left { text-align: left; }
+._nl_tbl .center { text-align: center; }
+._nl_tbl .right { text-align: right; }
+
 /* Expandable block, which replaces the <details><summary>...</summary>...</details> with:
 <p class="_ds_expand">
 <a href="expandable:{}" data-group="{}" data-level="{}">▼{}</a>
 </p>
 */
 /* Expanded block (collapsible), which appears after expandable block click:
 <table class="_n_details">
```

#### html2text {}

```diff
@@ -2,15 +2,21 @@
 family: 'Arial', 'Liberation Sans', sans-serif; line-height: 23px; } a
 { display: inline-block; } /* Fix new line issue within the p block */ p
 { white-space: pre-line; } pre { /*display: block; white-space: pre; max-width:
 100%; text-indent: 20px; margin: 10px;*/ } img { max-width: 100%; } a { color:
 deeppink; } /* Somehow h5 and h6 are not balanced. Hence h6 adjusted in pt */
 h1 { font-size: xx-large; } h2 { font-size: x-large; } h3 { font-size: large; }
 h4 { font-size: medium; } h5 { font-size: small; } h6 { font-size: 8pt; font-
-weight: bold; } /* Expandable block, which replaces the ...... with:
+weight: bold; } /* Markdown table */ table._nl_tbl { margin-top: 10px; border-
+collapse: collapse; } table._nl_tbl td { border: 1px solid mediumvioletred;
+padding: 5px; } table._nl_tbl th { border: 1px solid mediumvioletred;
+background: lightpink; color: mediumvioletred; font-weight: bold; padding: 5px;
+} /* Style substitution for tree-processor */ ._nl_tbl .left { text-align:
+left; } ._nl_tbl .center { text-align: center; } ._nl_tbl .right { text-align:
+right; } /* Expandable block, which replaces the ...... with:
 _â__¼_{_}
 */ /* Expanded block (collapsible), which appears after expandable block click:
 {}
 {}
 */ /* anchor details-summary common */ ._ds_expand { border: 1px solid grey
 !important; background: transparent; } /* anchor details-summary expandable */
 ._ds_expand > a { color: black; text-decoration: none; font-weight: bold; }
```

### Comparing `notolog-0.9.1b1/app/assets/themes/strawberry/tree_view.css` & `notolog-0.9.1b2/notolog/assets/themes/strawberry/tree_view.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/edit_widget.py` & `notolog-0.9.1b2/notolog/edit_widget.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/editor_state.py` & `notolog-0.9.1b2/notolog/editor_state.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/encrypt/enc_helper.py` & `notolog-0.9.1b2/notolog/encrypt/enc_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             if self.logging:
                 self.logger.warning('No iterations provided! Default value fallback')
             self.iterations = self.__class__.get_default_iterations()
 
         # Derive key from password
         key = self.generate_key_from_password()
         encoded_key = base64.urlsafe_b64encode(key)
-        # Fernet uses only the first 128 bits (16 bytes) of the key for AES encryption.
+        # Fernet uses only the first 128 bits (16 bytes) of the decoded key for AES encryption.
         self.cipher_suite = Fernet(encoded_key)
 
         self.key = None
 
     def generate_key_from_password(self) -> bytes:
         """
         Generate a key from the password
@@ -76,15 +76,15 @@
         Password-Based Key Derivation Function 2 (PBKDF2) implementation.
         The param length=32 is the length of the derived key.
         """
         kdf = PBKDF2HMAC(
             algorithm=hashes.SHA256(),
             iterations=self.iterations,
             salt=self.salt,
-            length=32  # 32 bytes = 256 bits key
+            length=32  # 32 bytes = 256 bits
         )
 
         self.key = kdf.derive(self.password)
 
         return self.key
 
     @staticmethod
```

### Comparing `notolog-0.9.1b1/app/encrypt/enc_new_password_dialog.py` & `notolog-0.9.1b2/notolog/encrypt/enc_new_password_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/encrypt/enc_password.py` & `notolog-0.9.1b2/notolog/encrypt/enc_password.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/encrypt/enc_password_dialog.py` & `notolog-0.9.1b2/notolog/encrypt/enc_password_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/encrypt/enc_password_reset_dialog.py` & `notolog-0.9.1b2/notolog/encrypt/enc_password_reset_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/enums/ai_model_names.py` & `notolog-0.9.1b2/notolog/enums/enum_base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,21 @@
 from enum import Enum
 
 
-class AiModelNames(Enum):
+class EnumBase(Enum):
 
     @staticmethod
     def _generate_next_value_(name, start, count, last_values):
         """
         Override _generate_next_value_ to allow for custom attributes on enum members (mostly for default).
 
         'name' is the name of the Enum's member, which will be 'A', 'B', 'C', etc.
-        This method returns the name itself, a 'default' marker (False), and a 'legacy' marker (False)
+        This method returns the name itself and a 'default' marker (False)
         """
-        return name, False, False
-
-    GPT_3_5 = ("gpt-3.5-turbo", True)  # The second item in the tuple marks this as the default
-    GPT_3_5_LEGACY = ("gpt-3.5-turbo-instruct", False, True)  # Third param is a legacy flag (e.g. legacy completions)
-
-    def __init__(self, value, is_default=False, legacy=False):
-        # If the value is a tuple, unpack it.
-        if isinstance(value, tuple):
-            self._value_, self.is_default, self.legacy = value
-        else:
-            self._value_ = value
-            self.is_default = is_default
-            self.legacy = legacy
+        return name, False
 
     def __str__(self):
         return self.name.lower()
 
     @classmethod
     def __getitem__(cls, key):
         if isinstance(key, str):
@@ -40,18 +28,10 @@
         Returns the default value of the Enum.
         Usage:
             self.default()
         @return: Any
         """
         # Find and return the default enum member
         for member in cls:
-            if member.is_default:
+            if hasattr(member, 'is_default') and member.is_default:
                 return member
         return None  # If no default is marked, return None or consider raising an error
-
-    @classmethod
-    def legacy_members(cls):
-        return [member for member in cls if member.legacy]
-
-    @classmethod
-    def legacy(cls, member):
-        return member in cls.legacy_members()
```

### Comparing `notolog-0.9.1b1/app/enums/themes.py` & `notolog-0.9.1b2/notolog/enums/languages.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,52 @@
-from enum import Enum
+from PySide6.QtCore import QLocale
 
+from .enum_base import EnumBase
 
-class Themes(Enum):
+assert hasattr(EnumBase, 'default'), "Check default() method is implemented in the base class"
 
-    @staticmethod
-    def _generate_next_value_(name, start, count, last_values):
-        """
-        Override _generate_next_value_ to allow for custom attributes on enum members (mostly for default).
 
-        'name' is the name of the Enum's member, which will be 'A', 'B', 'C', etc.
-        This method returns the name itself and a 'default' marker (False)
-        """
-        return name, False
+class Languages(EnumBase):
 
-    DEFAULT = ("Default", True)  # The second item in the tuple marks this as the default
-    CALLIGRAPHY = "Calligraphy"
-    NOIR_DARK = "Noir Dark"
-    STRAWBERRY = "Strawberry"
+    DE = "German"
+    EN = ("English", True)  # Fallback default option
+    ES = "Spanish"
+    FI = "Finnish"
+    FR = "French"
+    GE = "Georgian"
+    GR = "Greek"
+    IN = "Hindi"
+    IT = "Italian"
+    JA = "Japanese"
+    KO = "Korean"
+    LA = "Latin"
+    NL = "Dutch"
+    PT = "Portuguese"
+    RU = "Russian"
+    SE = "Swedish"
+    TR = "Turkish"
+    ZH = "Chinese"
 
     def __init__(self, value, is_default=False):
         self._value_ = value
         self.is_default = is_default
 
-    def __str__(self):
-        return self.name.lower()
-
-    @classmethod
-    def __getitem__(cls, key):
-        if isinstance(key, str):
-            key = key.upper()  # Normalize the key to uppercase
-        return cls._member_map_[key]
-
     @classmethod
     def default(cls):
         """
         Returns the default value of the Enum.
         Usage:
             self.default()
         @return: Any
         """
-        # Find and return the default enum member
+
+        locale = QLocale.system()  # Get the system's locale
+        iso_language_code = locale.name().split('_')[0]  # Extract the language part and ignore the country part
+
+        # Find and return the default enum member based on the system locale
         for member in cls:
-            if member.is_default:
+            # System locale as a default locale
+            if iso_language_code and member.name.lower() == iso_language_code:
                 return member
-        return None  # If no default is marked, return None or consider raising an error
+
+        # Fallback to the parent's logic
+        return super().default()
```

### Comparing `notolog-0.9.1b1/app/etree_extension.py` & `notolog-0.9.1b2/notolog/etree_extension.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,83 +2,125 @@
 
 from markdown import Markdown
 from markdown.extensions import Extension
 from markdown.treeprocessors import Treeprocessor
 
 from .app_config import AppConfig
 
+import re
 import logging
 
 
 class ElementTreeExtension(Extension):
     """
-    Custom markdown extension
+    Custom markdown extension.
     """
 
     logger = logging.getLogger('tree_extension')
 
     logging = AppConfig.get_logging()
     debug = AppConfig.get_debug()
 
     def extendMarkdown(self, md: Markdown) -> None:
         if self.debug:
-            self.logger.info('%s extension engaged' % self . __class__ . __qualname__)
-
+            self.logger.info('%s extension engaged' % self.__class__.__qualname__)
+        # Registering extension
         md.registerExtension(self)
         # noinspection SpellCheckingInspection
         md.treeprocessors.register(ElementTreeProcessor(md), 'notolog_extension', 1)
 
 
 class ElementTreeProcessor(Treeprocessor):
     """
-    Custom markdown extension processor
+    Custom markdown extension tree processor.
     """
 
     logger = logging.getLogger('tree_processor')
 
     logging = AppConfig.get_logging()
     debug = AppConfig.get_debug()
 
     def run(self, root):
         # Customize elements tree here
         for idx, elem in enumerate(root.iter()):
             if self.debug:
-                self.logger.debug('%s > %d: %s' % (self . __class__ . __qualname__, idx, elem.tag))
+                self.logger.debug('Process elements > %d: %s' % (idx, elem.tag))
+            # Process <table> elements
+            if elem.tag == 'table':
+                self.process_table(elem)
+            if elem.tag in ['th', 'td']:
+                self.process_table_td(elem)
+            # Process <img> elements
+            if elem.tag == 'img':
+                self.process_image(elem)
+            # Process <p> elements
+            if elem.tag == 'p':
+                self.process_paragraph(elem)
             # noinspection SpellCheckingInspection
             """
             Works when `codehilite` is switched off:
             if elem.tag == 'pre':
                 for id_xy, c_elem in enumerate(elem):
                     if c_elem.tag == 'code':
                         c_elem.set('style', 'background-color: #373737; color: #f5f5f5; padding: 10px;')
             """
-            # if elem.tag == 'img':
-            #    elem.set('title', '...')
-            #    elem.set('onerror', "this.onerror=null;this.src='app/assets/themes/default/icons/...';")
-            if elem.tag == 'p' and len(elem) > 0:
-                for id_xy, c_elem in enumerate(elem):
-                    if self.debug:
-                        self.logger.debug('%s > Inner element > %d: %s'
-                                          % (self . __class__ . __qualname__, id_xy, c_elem.tag))
-                    # Example of how to update elements tree
-                    if c_elem.tag == 'a' and False:
-                        # Skip element that was already re-inserted
-                        if c_elem.get('class') == '_re-inserted':
-                            continue
-                        # Add break space before the element
-                        br_str = "<br/>"
-                        br_elem = ElementTree.fromstring(br_str)
-                        # Remove `a` element
-                        elem.remove(c_elem)
-                        # Insert `br` element
-                        elem.insert(id_xy, br_elem)
-                        # Setup class as a flag to determine re-inserted `a` element
-                        c_elem.set('class', '_re-inserted')
-                        # Re-insert the `a` element with a new class
-                        elem.insert(id_xy + 1, c_elem)
 
     def get_index(self, root, element):
         for idx, child in enumerate(root):
             if element == child:
                 return idx
         else:
             raise ValueError("No inner '%s' tag found in '%s'" % (element.tag, root.tag))
+
+    def process_table(self, elem):
+        if not elem.get('class'):
+            if self.debug:
+                self.logger.debug(f'Table without class found {elem}')
+            elem.set('class', '_nl_tbl')
+            elem.set('cellpadding', '0')
+            elem.set('cellspacing', '0')
+
+    def process_table_td(self, elem):
+        # Replace 'style' with 'class' as css doesn't work otherwise
+        if elem.get('style') and elem.get('style').startswith('text-align'):
+            """
+            re = QRegularExpression(r'^text-align:\s?(.*?);$')
+            match = re.match(elem.get('style'))
+            if match.capturedTexts() and match.captured(1):
+                ...
+            """
+            pattern = re.compile(r'^text-align:\s?(.*?);$')
+            match = pattern.search(elem.get('style'))
+            if match:
+                del elem.attrib['style']
+                elem.set('class', match.group(1))
+
+    def process_image(self, elem):
+        if self.debug:
+            self.logger.debug(f'Image element {elem}')
+        # elem.set('title', '...')
+        # elem.set('onerror', "this.onerror=null;this.src='...';")
+
+    def process_paragraph(self, elem):
+        # Check inner elements
+        if not (len(elem) > 0):
+            return
+        # Process inner elements
+        for id_xy, c_elem in enumerate(elem):
+            if self.debug:
+                self.logger.debug('Inner element > %d: %s' % (id_xy, c_elem.tag))
+            # Example of how to update elements tree
+            if c_elem.tag == 'a' and False:
+                # Skip element that was already re-inserted
+                if c_elem.get('class') == '_re-inserted':
+                    continue
+                # Add break space before the element
+                br_str = "<br/>"
+                br_elem = ElementTree.fromstring(br_str)
+                # Remove `a` element
+                elem.remove(c_elem)
+                # Insert `br` element
+                elem.insert(id_xy, br_elem)
+                # Setup class as a flag to determine re-inserted `a` element
+                c_elem.set('class', '_re-inserted')
+                # Re-insert the `a` element with a new class
+                elem.insert(id_xy + 1, c_elem)
```

### Comparing `notolog-0.9.1b1/app/file_header.py` & `notolog-0.9.1b2/notolog/file_header.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/file_system_watcher.py` & `notolog-0.9.1b2/notolog/file_system_watcher.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/helpers/file_helper.py` & `notolog-0.9.1b2/notolog/helpers/file_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/helpers/theme_helper.py` & `notolog-0.9.1b2/notolog/helpers/theme_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/helpers/tooltip_helper.py` & `notolog-0.9.1b2/notolog/helpers/tooltip_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/helpers/update_helper.py` & `notolog-0.9.1b2/notolog/helpers/update_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/highlight/main_highlighter.py` & `notolog-0.9.1b2/notolog/highlight/main_highlighter.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
     def __init__(self, document: QTextDocument = None):
         super().__init__(document)
 
         self.logger = logging.getLogger('highlighter')
 
         self.logging = AppConfig.get_logging()
-        self.debug = AppConfig.get_debug()
+        self.debug = False  # AppConfig.get_debug()
 
         # Get app's global font size
         self.font_size = AppConfig.get_font_size()
 
         # Walk rules to create QRegExp for each pattern
         self.rules = [(self.get_regex(pattern), nth, tag, group, duple, fmt, reckon)
                       for (pattern, nth, tag, group, duple, fmt, reckon) in self.re_rules]
@@ -83,14 +83,19 @@
         self.user_data = None  # type: Union[TextBlockData, QTextBlockUserData, None]
         self.prev_user_data = None  # type: Union[TextBlockData, QTextBlockUserData, None]
 
         self.theme_helper = ThemeHelper()
 
         self.override_colors()
 
+    def __init_subclass__(cls):
+        # Check the required methods are implemented
+        if not hasattr(cls, 'highlightBlock'):
+            raise NotImplementedError(f'Method highlightBlock() have to be implemented in subclass {cls.__name__}.')
+
     def override_colors(self):
         for item in self.theme:
             """
             Proof of concept method of how to override the colors set to highlighter's syntax.
             Consider to override the whole map with styles like background pattern.
             """
             # Get color values from the theme helper
@@ -140,16 +145,15 @@
         if not (color or style or bg or font_size_ratio):
             return
 
         cformat = QTextCharFormat()
 
         # Foreground
         if color:
-            color_obj = QColor()
-            color_obj.setNamedColor(color)
+            color_obj = QColor(color)
             cformat.setForeground(color_obj)
 
         # Background
         if bg:
             bg_color = None  # type: Union[str, None]
             """
             Qt::BrushStyle https://doc.qt.io/qt-6/qt.html#BrushStyle-enum
@@ -160,16 +164,15 @@
             elif type(bg) is dict:
                 if 'color' in bg:
                     bg_color = bg['color']
                 if 'pattern' in bg and bg['pattern'] in Qt.BrushStyle:
                     bg_pattern = bg['pattern']
             # Color required
             if bg_color is not None:
-                bg_color_obj = QColor()
-                bg_color_obj.setNamedColor(bg_color)
+                bg_color_obj = QColor(bg_color)
                 """
                 https://doc.qt.io/qt-6/qbrush.html
                 """
                 cformat.setBackground(QBrush(bg_color_obj, bg_pattern))
 
         # Font size
         if font_size_ratio and self.font_size:
@@ -184,17 +187,17 @@
             cformat.setFontItalic(True)
         if 'underline' in style:
             cformat.setFontUnderline(True)
         if 'strikethrough' in style:
             cformat.setFontStrikeOut(True)
         if 'monospace' in style:
             monospace_font = QFont(
-                "font-family: 'Consolas', 'Menlo', 'Monaco', 'Lucida Console', 'Liberation Mono', 'DejaVu Sans Mono', "
+                "font-family: 'Menlo', 'Monaco', 'Consolas', 'Lucida Console', 'Liberation Mono', 'DejaVu Sans Mono', "
                 "'Courier New', monospace;")
-            monospace_font.setStyleHint(QFont.Monospace)
+            monospace_font.setStyleHint(QFont.StyleHint.Monospace)
             # 100% means normal spacing, no extra spacing
             monospace_font.setLetterSpacing(QFont.SpacingType.PercentageSpacing, 100)
             cformat.setFont(monospace_font)
 
         return cformat
 
     def rehighlightBlock(self, block):
```

### Comparing `notolog-0.9.1b1/app/highlight/md_highlighter.py` & `notolog-0.9.1b2/notolog/highlight/md_highlighter.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,21 @@
 # - PyPI: https://pypi.org/project/notolog
 # - WebSite: https://notolog.app
 # - Author: Vadim Bakhrenkov
 # - Copyright 2024 Vadim Bakhrenkov
 # - License: MIT License
 
 from PySide6.QtCore import Qt
+from PySide6.QtGui import QTextBlockUserData
 
 from .main_highlighter import MainHighlighter
 from . import TextBlockData
 
+from typing import Union
+
 import re
 
 
 class MdHighlighter(MainHighlighter):
     """
     Syntax highlighter class for the Markdown language
     """
@@ -69,14 +72,16 @@
         'codelf': {'color': 'white', 'style': 'monospace', 'bg': {'color': 'magenta', 'pattern': Qt.BrushStyle.Dense2Pattern}},
         'code_lang': {'color': 'magenta', 'style': 'bold'},
         'code_indent': {'bg': {'color': 'pink', 'pattern': Qt.BrushStyle.Dense6Pattern}},
         'code_content': {'color': 'brown'},
         # Debug: 'bg': {'color': 'darkGrey', 'pattern': Qt.BrushStyle.Dense2Pattern}
         'wrong_indent': {'bg': {'color': 'red', 'pattern': Qt.BrushStyle.DiagCrossPattern}},
         'comment': {'color': 'grey', 'bg': {'color': 'lightGrey', 'pattern': Qt.BrushStyle.Dense6Pattern}},
+        'table_h': {'style': ['bold', 'monospace'], 'bg': {'color': 'lightGrey'}},
+        'table_d': {'style': 'monospace', 'bg': {'color': 'whiteSmoke'}},
         'img': {'color': 'green'},
         'ref': {'color': 'white', 'bg': {'color': 'green', 'pattern': Qt.BrushStyle.Dense3Pattern}},
         # 'ref_data': {'color': 'green', 'bg': {'color': 'yellow', 'pattern': Qt.BrushStyle.Dense6Pattern}},
         'abbr': {'color': 'white', 'bg': {'color': 'dodgerBlue', 'pattern': Qt.BrushStyle.SolidPattern}},
         'abbr_text': {'color': 'white', 'style': 'bold', 'bg': {'color': 'dodgerBlue', 'pattern': Qt.BrushStyle.SolidPattern}},
         'link': {'color': 'white', 'style': 'italic', 'bg': 'blue'},
         'list': {'color': 'white', 'bg': 'darkMagenta'},
@@ -181,14 +186,17 @@
         (r'^((?:[\s\t]*?)[#]{3}\s*?)(.*)$', 2, 'h3_text', 'h', False, theme['h3_text'], None),
         (r'^((?:[\s\t]*?)[#]{4})\s*?.*?', 1, 'h4', 'h', False, theme['h4'], None),
         (r'^((?:[\s\t]*?)[#]{4}\s*?)(.*)$', 2, 'h4_text', 'h', False, theme['h4_text'], None),
         (r'^((?:[\s\t]*?)[#]{5})\s*?.*?', 1, 'h5', 'h', False, theme['h5'], None),
         (r'^((?:[\s\t]*?)[#]{5}\s*?)(.*)$', 2, 'h5_text', 'h', False, theme['h5_text'], None),
         (r'^((?:[\s\t]*?)[#]{6})\s*?.*?', 1, 'h6', 'h', False, theme['h6'], None),
         (r'^((?:[\s\t]*?)[#]{6}\s*?)(.*)$', 2, 'h6_text', 'h', False, theme['h6_text'], None),
+        # Table
+        (r'^(\|[\s\|\:\-]+?\|)$', 1, 'table_h', 'table', False, theme['table_h'], None),
+        (r'^(\|(?=.*?[a-zA-Z0-9]).*?\|)$', 1, 'table_d', 'table', False, theme['table_d'], None),
         # Image
         (r'(!\[[^\]]*?\]\([^\)]*?\))', 1, 'img', 'img', False, theme['img'], None),
         (r'(!\[[^\]]*?\]\[[^\]]*?\])', 1, 'img', 'img', False, theme['img'], None),
         # reference either image or link, footnotes also
         (r'((?<!\*)\[[^\]]*?\]:)', 1, 'ref', 'ref', False, theme['ref'], None),
         # (r'(\[[^\]]*?\]:)(\S*?)$', 2, 'ref_data', 'ref', False, theme['ref_data'], None),
         # abbreviations
@@ -290,18 +298,18 @@
         """
         Apply a syntax highlighting to each line of the text.
         * https://doc.qt.io/qt-6/qsyntaxhighlighter.html#highlightBlock
         """
 
         # Get the current block and associated user data
         self.current_block = self.currentBlock()
-        self.user_data = self.current_block.userData()
+        self.user_data = self.current_block.userData()  # type: Union[TextBlockData, QTextBlockUserData]
 
         self.prev_block = self.current_block.previous()
-        self.prev_user_data = self.prev_block.userData()
+        self.prev_user_data = self.prev_block.userData()  # type: Union[TextBlockData, QTextBlockUserData]
 
         self.line_number = self.currentBlock().blockNumber()
         # Line number as it appears in the editor
         self.line_number_log = self.line_number + 1
 
         if self.user_data is None or not isinstance(self.user_data, TextBlockData):
             if self.debug:
@@ -514,16 +522,16 @@
 
                 if ((tag in {'codec', 'list'}
                      # Code block :::: has to start with empty line or at very beginning of the document.
                      and (self.line_number == 0
                           # Check prev line is an empty line
                           or (self.line_number - 1 in self.line_tokens
                               and 'rn' in self.line_tokens[self.line_number - 1])))
-                        # Blockquote may start without preliminary empty line
-                        or (tag not in {'codec', 'list'}
+                        # Blockquote and list may start without preliminary empty line
+                        or (tag not in {'codec'}
                             and not self.tokens[tag]['o'])):
                     # Mind the indents
                     self.tokens[tag]['cnt'] += 1
                     self.tokens[tag]['o'] = True
                     if self.debug:
                         self.logger.debug(
                             '{%r} >>> Open "%s" at [%d*]'
@@ -602,14 +610,22 @@
             if reckon is not None and not reckon(self):
                 """
                 To check some additional conditions for the token, say:
                 if not self.is_in_code() and group in {'comment'}: ...
                 """
                 continue
 
+            if self.rehighlight_block:
+                if tag in self.tokens:
+                    """
+                    Opened tokens continue to apply for the following inline parts
+                    Logic slightly differ apart with open-close tokens approach.
+                    """
+                    self.tokens[tag]['o'] = self.user_data.get_param(tag, 'within')
+
             """
             Regular Python regular expression operations instead of QRegularExpression, QRegularExpressionMatchIterator
             and QRegularExpressionMatch as sometimes it doesn't work properly.
             * https://docs.python.org/3/library/re.html
             * https://doc.qt.io/qt-6/qregularexpression.html
             """
             matches = re.finditer(pattern, text_str)
@@ -667,14 +683,42 @@
                     if not 'o' in self.tokens[tag]:
                         self.tokens[tag]['o'] = True
                     elif self.tokens[tag]['o']:
                         self.tokens[tag]['o'] = False
                     else:
                         self.tokens[tag]['o'] = True
 
+                # Table
+                if (tag == 'table_h'
+                    and (self.line_number - 1 in self.line_tokens
+                         # Previous token is a table header
+                         and (self.line_number - 1 in self.line_tokens
+                              and 'table_d' in self.line_tokens[self.line_number - 1])
+                         # The token before the table header either a new line or file's first line
+                         and ((self.line_number - 2 in self.line_tokens
+                              and 'rn' in self.line_tokens[self.line_number - 2])
+                              # line number "1" as table header token earliest line is next to "0"
+                              or self.line_number == 1))):
+                    self.tokens['table_d']['o'] = True
+                    # It will be highlighted after the next re-highlight
+                    if self.prev_user_data:
+                        self.prev_user_data.put(tag='table_d', opened=True, within=True, closed=False)
+                elif 'table_d' in self.tokens and self.tokens['table_d']['o'] and tag != 'table_d':
+                    self.tokens['table_d']['o'] = False
+                    if self.prev_user_data:
+                        self.prev_user_data.put(tag='table_d', opened=False, within=True, closed=True)
+                elif tag == 'table_d' and self.tokens['table_d']['o']:
+                    self.user_data.put(tag=tag, opened=False, within=True, closed=False)
+                if (group == 'table'
+                        # Skip if not in table context yet
+                        and not (self.user_data.get_param('table_d', 'within')
+                                 or ('table_d' in self.tokens and self.tokens['table_d']['o']))):
+                    continue
+                # No save to block's data as it will be self stored for next block re-highlight iteration
+
                 # Prevent passing reference of the dict
                 cfc = cf_data.copy()
 
                 # Within the code block
                 if self.is_in_code():
                     # Search whether line within code block or not
                     # or True in [True if x['in_code'] else False for x in self.line_tokens[self.line_number][tag]]):
```

### Comparing `notolog-0.9.1b1/app/highlight/view_highlighter.py` & `notolog-0.9.1b2/notolog/highlight/view_highlighter.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/image_downloader.py` & `notolog-0.9.1b2/notolog/image_downloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 class ImageDownloader(QObject):  # QObject to allow signal emitting
 
     # Signal to emit upon single resource was downloaded
     downloaded = Signal(dict)
 
     # Signal to emit upon all downloading tasks in queue have been finished
-    finished = Signal()
+    finished = Signal(int)
 
     RESOURCE_DIR = 'images'
 
     def __init__(self, base_folder: str = None):
 
         super().__init__()
 
@@ -42,14 +42,17 @@
         self.lexemes = Lexemes()
 
         # Async event loop
         self.event_loop = asyncio.get_event_loop()
         # async download tasks queue
         self.resource_tasks = []
 
+        # Downloaded counter till finished emitted
+        self.downloaded_cnt = 0
+
         # Validate folder and make it QDir
         self.folder = self.get_resource_folder(base_folder)
 
         if self.debug:
             self.logger.debug(f'Folder to save downloaded resources: {self.folder.path()}')
 
         os.makedirs(self.folder.path(), exist_ok=True)
@@ -113,23 +116,24 @@
                 self.logger.debug(result_message)
 
             # Check if the resource is an image
             mime_type = reply.header(QNetworkRequest.KnownHeaders.ContentTypeHeader)
             if 'image' in mime_type:
                 url = reply.url().toString()
                 data = reply.readAll()  # type: QByteArray
-                #if self.debug:
-                self.logger.debug(f"Resource data downloaded {url} [{size_f(len(data))}]")
+                if self.debug:
+                    self.logger.debug(f"Resource data downloaded {url} [{size_f(len(data))}]")
 
                 # Store the image within the app's cache first
                 pixmap = QPixmap()
                 pixmap.loadFromData(data)
                 QPixmapCache.insert(url, pixmap)
 
                 self.downloaded.emit({'resource_name': url})
+                self.downloaded_cnt += 1
 
                 if self.settings.viewer_save_resources:
                     # Saving downloaded files
                     self.save_image(url, data)
 
                 """
                 base_name = self.url_to_filename(url)
@@ -180,24 +184,27 @@
             # timeout = 1.5  # to return after the timeout, some task could be pending
         )
 
         if self.debug:
             self.logger.debug(f'Downloading resource tasks progress. Done {len(done)}, pending {len(pending)}')
 
         if len(self.resource_tasks) <= 1:
-            # All tasks in queue have finished
-            self.finished.emit()
+            # Hold this method a particular amount of time to allow completed tasks to settle as this step is
+            # typically ahead.
+            await asyncio.sleep(0.25, self.event_loop)
+            if self.downloaded_cnt > 0:
+                # All tasks in queue have finished
+                self.finished.emit(self.downloaded_cnt)
+                self.downloaded_cnt = 0
 
     async def resource_download_async(self, image_url) -> None:
         """
         Downloading resource which is will be processed by resource_downloaded_handler() then.
         """
         self.download_image(image_url)
-        # Keep this method particular amount of time to avoid overwhelming
-        await asyncio.sleep(0.1, self.event_loop)
 
     @staticmethod
     def is_external_url(url, base_domain='example.com'):
         """
         Determine if the given URL is an external URL.
         """
         parsed_url = urlparse(url)
```

### Comparing `notolog-0.9.1b1/app/lexemes/de/__pycache__/main_menu.cpython-39.pyc` & `notolog-0.9.1b2/notolog/lexemes/pt/main_menu.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,137 +1,146 @@
-00000000: 610d 0d0a 0000 0000 b254 2c66 db08 0000  a........T,f....
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0029 0000 0040 0000 0073 5a00 0000 6400  .)...@...sZ...d.
-00000030: 6401 6402 6403 6404 6404 6405 6406 6407  d.d.d.d.d.d.d.d.
-00000040: 6408 6409 640a 640b 640c 6401 640d 640e  d.d.d.d.d.d.d.d.
-00000050: 640f 6410 6411 6412 6413 6414 6415 6416  d.d.d.d.d.d.d.d.
-00000060: 6417 6418 6419 641a 641b 641c 641d 641e  d.d.d.d.d.d.d.d.
-00000070: 641e 641f 641f 6420 6421 6422 6422 6423  d.d.d.d d!d"d"d#
-00000080: 9c28 5a00 6424 5300 2925 5a05 4461 7465  .(Z.d$S.)%Z.Date
-00000090: 695a 0a42 6561 7262 6569 7465 6e5a 0957  iZ.BearbeitenZ.W
-000000a0: 6572 6b7a 6575 6765 5a05 4869 6c66 657a  erkzeugeZ.Hilfez
-000000b0: 0e4e 6575 6573 2044 6f6b 756d 656e 7475  .Neues Dokumentu
-000000c0: 0700 0000 c396 6666 6e65 6e75 1000 0000  ......ffnenu....
-000000d0: 446f 6b75 6d65 6e74 20c3 b666 666e 656e  Dokument ..ffnen
-000000e0: 5a09 5370 6569 6368 6572 6e7a 1244 6f6b  Z.Speichernz.Dok
-000000f0: 756d 656e 7420 7370 6569 6368 6572 6e7a  ument speichernz
-00000100: 0f53 7065 6963 6865 726e 2075 6e74 6572  .Speichern unter
-00000110: 7a1d 4b6f 7069 6520 6465 7320 446f 6b75  z.Kopie des Doku
-00000120: 6d65 6e74 7320 7370 6569 6368 6572 6e5a  ments speichernZ
-00000130: 0742 6565 6e64 656e 7a0b 4170 7020 6265  .Beendenz.App be
-00000140: 656e 6465 6e7a 1044 6174 6569 2062 6561  endenz.Datei bea
-00000150: 7262 6569 7465 6e5a 0651 7565 6c6c 655a  rbeitenZ.QuelleZ
-00000160: 0951 7565 6c6c 636f 6465 5a04 4665 7474  .QuellcodeZ.Fett
-00000170: 7a12 4665 7474 7363 6872 6966 7420 466f  z.Fettschrift Fo
-00000180: 726d 6174 5a06 4b75 7273 6976 7a14 4b75  rmatZ.Kursivz.Ku
-00000190: 7273 6976 7363 6872 6966 7420 466f 726d  rsivschrift Form
-000001a0: 6174 5a0e 556e 7465 7273 7472 6569 6368  atZ.Unterstreich
-000001b0: 656e 7a18 556e 7465 7273 7472 6963 6865  enz.Unterstriche
-000001c0: 6e20 5465 7874 666f 726d 6174 5a0f 4475  n TextformatZ.Du
-000001d0: 7263 6867 6573 7472 6963 6865 6e7a 1c44  rchgestrichenz.D
-000001e0: 7572 6368 6765 7374 7269 6368 656e 6573  urchgestrichenes
-000001f0: 2054 6578 7466 6f72 6d61 745a 0a42 6c6f   TextformatZ.Blo
-00000200: 636b 7a69 7461 747a 1542 6c6f 636b 7a69  ckzitatz.Blockzi
-00000210: 7461 7420 5465 7874 666f 726d 6174 7a0c  tat Textformatz.
-00000220: 4b49 2d41 7373 6973 7465 6e74 7a14 4b49  KI-Assistentz.KI
-00000230: 2d41 7373 6973 7465 6e74 2073 7461 7274  -Assistent start
-00000240: 656e 750b 0000 0046 6172 6277 c3a4 686c  enu....Farbw..hl
-00000250: 6572 7514 0000 0054 6578 7466 6172 6265  eru....Textfarbe
-00000260: 2061 7573 77c3 a468 6c65 6e7a 0f4d 6172   ausw..hlenz.Mar
-00000270: 6b64 6f77 6e2d 5379 6e74 6178 7513 0000  kdown-Syntaxu...
-00000280: 0041 7566 2055 7064 6174 6573 2070 72c3  .Auf Updates pr.
-00000290: bc66 656e 5a0d 4665 686c 6572 6265 7269  .fenZ.Fehlerberi
-000002a0: 6368 747a 1446 6568 6c65 7262 6572 6963  chtz.Fehlerberic
-000002b0: 6874 2073 656e 6465 6e75 0500 0000 c39c  ht sendenu......
-000002c0: 6265 7229 28da 1067 726f 7570 5f66 696c  ber)(..group_fil
-000002d0: 655f 6c61 6265 6cda 1067 726f 7570 5f65  e_label..group_e
-000002e0: 6469 745f 6c61 6265 6cda 1167 726f 7570  dit_label..group
-000002f0: 5f74 6f6f 6c73 5f6c 6162 656c da10 6772  _tools_label..gr
-00000300: 6f75 705f 6865 6c70 5f6c 6162 656c da1f  oup_help_label..
-00000310: 6163 7469 6f6e 735f 6669 6c65 5f6c 6162  actions_file_lab
-00000320: 656c 5f6e 6577 5f64 6f63 756d 656e 74da  el_new_document.
-00000330: 2961 6374 696f 6e73 5f66 696c 655f 6163  )actions_file_ac
-00000340: 6365 7373 6962 6c65 5f6e 616d 655f 6e65  cessible_name_ne
-00000350: 775f 646f 6375 6d65 6e74 da17 6163 7469  w_document..acti
-00000360: 6f6e 735f 6669 6c65 5f6c 6162 656c 5f6f  ons_file_label_o
-00000370: 7065 6eda 2161 6374 696f 6e73 5f66 696c  pen.!actions_fil
-00000380: 655f 6163 6365 7373 6962 6c65 5f6e 616d  e_accessible_nam
-00000390: 655f 6f70 656e da17 6163 7469 6f6e 735f  e_open..actions_
-000003a0: 6669 6c65 5f6c 6162 656c 5f73 6176 65da  file_label_save.
-000003b0: 2161 6374 696f 6e73 5f66 696c 655f 6163  !actions_file_ac
-000003c0: 6365 7373 6962 6c65 5f6e 616d 655f 7361  cessible_name_sa
-000003d0: 7665 da1a 6163 7469 6f6e 735f 6669 6c65  ve..actions_file
-000003e0: 5f6c 6162 656c 5f73 6176 655f 6173 da24  _label_save_as.$
-000003f0: 6163 7469 6f6e 735f 6669 6c65 5f61 6363  actions_file_acc
-00000400: 6573 7369 626c 655f 6e61 6d65 5f73 6176  essible_name_sav
-00000410: 655f 6173 da17 6163 7469 6f6e 735f 6669  e_as..actions_fi
-00000420: 6c65 5f6c 6162 656c 5f65 7869 74da 2161  le_label_exit.!a
-00000430: 6374 696f 6e73 5f66 696c 655f 6163 6365  ctions_file_acce
-00000440: 7373 6962 6c65 5f6e 616d 655f 6578 6974  ssible_name_exit
-00000450: da16 6564 6974 5f61 6374 696f 6e73 5f65  ..edit_actions_e
-00000460: 6469 745f 6d6f 6465 da26 6564 6974 5f61  dit_mode.&edit_a
-00000470: 6374 696f 6e73 5f61 6363 6573 7369 626c  ctions_accessibl
-00000480: 655f 6e61 6d65 5f65 6469 745f 6d6f 6465  e_name_edit_mode
-00000490: da18 6564 6974 5f61 6374 696f 6e73 5f73  ..edit_actions_s
-000004a0: 6f75 7263 655f 6d6f 6465 da28 6564 6974  ource_mode.(edit
-000004b0: 5f61 6374 696f 6e73 5f61 6363 6573 7369  _actions_accessi
-000004c0: 626c 655f 6e61 6d65 5f73 6f75 7263 655f  ble_name_source_
-000004d0: 6d6f 6465 da11 6564 6974 5f61 6374 696f  mode..edit_actio
-000004e0: 6e73 5f62 6f6c 64da 2165 6469 745f 6163  ns_bold.!edit_ac
-000004f0: 7469 6f6e 735f 6163 6365 7373 6962 6c65  tions_accessible
-00000500: 5f6e 616d 655f 626f 6c64 da13 6564 6974  _name_bold..edit
-00000510: 5f61 6374 696f 6e73 5f69 7461 6c69 63da  _actions_italic.
-00000520: 2365 6469 745f 6163 7469 6f6e 735f 6163  #edit_actions_ac
-00000530: 6365 7373 6962 6c65 5f6e 616d 655f 6974  cessible_name_it
-00000540: 616c 6963 da16 6564 6974 5f61 6374 696f  alic..edit_actio
-00000550: 6e73 5f75 6e64 6572 6c69 6e65 da26 6564  ns_underline.&ed
-00000560: 6974 5f61 6374 696f 6e73 5f61 6363 6573  it_actions_acces
-00000570: 7369 626c 655f 6e61 6d65 5f75 6e64 6572  sible_name_under
-00000580: 6c69 6e65 da1a 6564 6974 5f61 6374 696f  line..edit_actio
-00000590: 6e73 5f73 7472 696b 6574 6872 6f75 6768  ns_strikethrough
-000005a0: da2a 6564 6974 5f61 6374 696f 6e73 5f61  .*edit_actions_a
-000005b0: 6363 6573 7369 626c 655f 6e61 6d65 5f73  ccessible_name_s
-000005c0: 7472 696b 6574 6872 6f75 6768 da17 6564  trikethrough..ed
-000005d0: 6974 5f61 6374 696f 6e73 5f62 6c6f 636b  it_actions_block
-000005e0: 7175 6f74 65da 2765 6469 745f 6163 7469  quote.'edit_acti
-000005f0: 6f6e 735f 6163 6365 7373 6962 6c65 5f6e  ons_accessible_n
-00000600: 616d 655f 626c 6f63 6b71 756f 7465 da1a  ame_blockquote..
-00000610: 746f 6f6c 735f 6163 7469 6f6e 735f 6169  tools_actions_ai
-00000620: 5f61 7373 6973 7461 6e74 da2a 746f 6f6c  _assistant.*tool
-00000630: 735f 6163 7469 6f6e 735f 6163 6365 7373  s_actions_access
-00000640: 6962 6c65 5f6e 616d 655f 6169 5f61 7373  ible_name_ai_ass
-00000650: 6973 7461 6e74 da1a 746f 6f6c 735f 6163  istant..tools_ac
-00000660: 7469 6f6e 735f 636f 6c6f 725f 7069 636b  tions_color_pick
-00000670: 6572 da2a 746f 6f6c 735f 6163 7469 6f6e  er.*tools_action
-00000680: 735f 6163 6365 7373 6962 6c65 5f6e 616d  s_accessible_nam
-00000690: 655f 636f 6c6f 725f 7069 636b 6572 da1c  e_color_picker..
-000006a0: 6163 7469 6f6e 735f 6865 6c70 5f6c 6162  actions_help_lab
-000006b0: 656c 5f6d 645f 7379 6e74 6178 da26 6163  el_md_syntax.&ac
-000006c0: 7469 6f6e 735f 6865 6c70 5f61 6363 6573  tions_help_acces
-000006d0: 7369 626c 655f 6e61 6d65 5f6d 645f 7379  sible_name_md_sy
-000006e0: 6e74 6178 da24 6163 7469 6f6e 735f 6865  ntax.$actions_he
-000006f0: 6c70 5f6c 6162 656c 5f63 6865 636b 5f66  lp_label_check_f
-00000700: 6f72 5f75 7064 6174 6573 da2e 6163 7469  or_updates..acti
-00000710: 6f6e 735f 6865 6c70 5f61 6363 6573 7369  ons_help_accessi
-00000720: 626c 655f 6e61 6d65 5f63 6865 636b 5f66  ble_name_check_f
-00000730: 6f72 5f75 7064 6174 6573 da1d 6163 7469  or_updates..acti
-00000740: 6f6e 735f 6865 6c70 5f6c 6162 656c 5f62  ons_help_label_b
-00000750: 7567 5f72 6570 6f72 74da 2761 6374 696f  ug_report.'actio
-00000760: 6e73 5f68 656c 705f 6163 6365 7373 6962  ns_help_accessib
-00000770: 6c65 5f6e 616d 655f 6275 675f 7265 706f  le_name_bug_repo
-00000780: 7274 da18 6163 7469 6f6e 735f 6865 6c70  rt..actions_help
-00000790: 5f6c 6162 656c 5f61 626f 7574 da22 6163  _label_about."ac
-000007a0: 7469 6f6e 735f 6865 6c70 5f61 6363 6573  tions_help_acces
-000007b0: 7369 626c 655f 6e61 6d65 5f61 626f 7574  sible_name_about
-000007c0: 4e29 01da 076c 6578 656d 6573 a900 722a  N)...lexemes..r*
-000007d0: 0000 0072 2a00 0000 fa4a 2f55 7365 7273  ...r*....J/Users
-000007e0: 2f76 6164 696b 7573 2f50 7963 6861 726d  /vadikus/Pycharm
-000007f0: 5072 6f6a 6563 7473 2f6e 6f74 6f6c 6f67  Projects/notolog
-00000800: 2d64 6576 2f6e 6f74 6f6c 6f67 2f6c 6578  -dev/notolog/lex
-00000810: 656d 6573 2f64 652f 6d61 696e 5f6d 656e  emes/de/main_men
-00000820: 752e 7079 da08 3c6d 6f64 756c 653e 0300  u.py..<module>..
-00000830: 0000 7350 0000 0002 0102 0102 0102 0202  ..sP............
-00000840: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-00000850: 0102 0202 0102 0102 0102 0102 0102 0102  ................
-00000860: 0102 0102 0102 0102 0102 0102 0102 0202  ................
-00000870: 0102 0102 0102 0202 0102 0102 0102 0102  ................
-00000880: 0102 0102 0102 d4                        .......
+00000000: 2320 506f 7274 7567 7565 7365 206c 6578  # Portuguese lex
+00000010: 656d 6573 206d 6169 6e5f 6d65 6e75 2e70  emes main_menu.p
+00000020: 790a 6c65 7865 6d65 7320 3d20 7b0a 2020  y.lexemes = {.  
+00000030: 2020 2267 726f 7570 5f66 696c 655f 6c61    "group_file_la
+00000040: 6265 6c22 3a20 2241 7271 7569 766f 222c  bel": "Arquivo",
+00000050: 0a20 2020 2022 6772 6f75 705f 6564 6974  .    "group_edit
+00000060: 5f6c 6162 656c 223a 2022 4564 6974 6172  _label": "Editar
+00000070: 222c 0a20 2020 2022 6772 6f75 705f 746f  ",.    "group_to
+00000080: 6f6c 735f 6c61 6265 6c22 3a20 2246 6572  ols_label": "Fer
+00000090: 7261 6d65 6e74 6173 222c 0a20 2020 2022  ramentas",.    "
+000000a0: 6772 6f75 705f 6865 6c70 5f6c 6162 656c  group_help_label
+000000b0: 223a 2022 416a 7564 6122 2c0a 0a20 2020  ": "Ajuda",..   
+000000c0: 2022 6163 7469 6f6e 735f 6669 6c65 5f6c   "actions_file_l
+000000d0: 6162 656c 5f6e 6577 5f64 6f63 756d 656e  abel_new_documen
+000000e0: 7422 3a20 224e 6f76 6f20 646f 6375 6d65  t": "Novo docume
+000000f0: 6e74 6f22 2c0a 2020 2020 2261 6374 696f  nto",.    "actio
+00000100: 6e73 5f66 696c 655f 6163 6365 7373 6962  ns_file_accessib
+00000110: 6c65 5f6e 616d 655f 6e65 775f 646f 6375  le_name_new_docu
+00000120: 6d65 6e74 223a 2022 4e6f 766f 2064 6f63  ment": "Novo doc
+00000130: 756d 656e 746f 222c 0a20 2020 2022 6163  umento",.    "ac
+00000140: 7469 6f6e 735f 6669 6c65 5f6c 6162 656c  tions_file_label
+00000150: 5f6f 7065 6e22 3a20 2241 6272 6972 222c  _open": "Abrir",
+00000160: 0a20 2020 2022 6163 7469 6f6e 735f 6669  .    "actions_fi
+00000170: 6c65 5f61 6363 6573 7369 626c 655f 6e61  le_accessible_na
+00000180: 6d65 5f6f 7065 6e22 3a20 2241 6272 6972  me_open": "Abrir
+00000190: 2064 6f63 756d 656e 746f 222c 0a20 2020   documento",.   
+000001a0: 2022 6163 7469 6f6e 735f 6669 6c65 5f6c   "actions_file_l
+000001b0: 6162 656c 5f73 6176 6522 3a20 2253 616c  abel_save": "Sal
+000001c0: 7661 7222 2c0a 2020 2020 2261 6374 696f  var",.    "actio
+000001d0: 6e73 5f66 696c 655f 6163 6365 7373 6962  ns_file_accessib
+000001e0: 6c65 5f6e 616d 655f 7361 7665 223a 2022  le_name_save": "
+000001f0: 5361 6c76 6172 2064 6f63 756d 656e 746f  Salvar documento
+00000200: 222c 0a20 2020 2022 6163 7469 6f6e 735f  ",.    "actions_
+00000210: 6669 6c65 5f6c 6162 656c 5f73 6176 655f  file_label_save_
+00000220: 6173 223a 2022 5361 6c76 6172 2063 6f6d  as": "Salvar com
+00000230: 6f22 2c0a 2020 2020 2261 6374 696f 6e73  o",.    "actions
+00000240: 5f66 696c 655f 6163 6365 7373 6962 6c65  _file_accessible
+00000250: 5f6e 616d 655f 7361 7665 5f61 7322 3a20  _name_save_as": 
+00000260: 2253 616c 7661 7220 636f 6d6f 2063 c3b3  "Salvar como c..
+00000270: 7069 6120 646f 2064 6f63 756d 656e 746f  pia do documento
+00000280: 222c 0a20 2020 2022 6163 7469 6f6e 735f  ",.    "actions_
+00000290: 6669 6c65 5f6c 6162 656c 5f65 7869 7422  file_label_exit"
+000002a0: 3a20 2253 6169 7220 646f 2061 706c 6963  : "Sair do aplic
+000002b0: 6174 6976 6f22 2c0a 2020 2020 2261 6374  ativo",.    "act
+000002c0: 696f 6e73 5f66 696c 655f 6163 6365 7373  ions_file_access
+000002d0: 6962 6c65 5f6e 616d 655f 6578 6974 223a  ible_name_exit":
+000002e0: 2022 5361 6972 2064 6f20 6170 6c69 6361   "Sair do aplica
+000002f0: 7469 766f 222c 0a0a 2020 2020 2265 6469  tivo",..    "edi
+00000300: 745f 6163 7469 6f6e 735f 6564 6974 5f6d  t_actions_edit_m
+00000310: 6f64 6522 3a20 2245 6469 7461 7222 2c0a  ode": "Editar",.
+00000320: 2020 2020 2265 6469 745f 6163 7469 6f6e      "edit_action
+00000330: 735f 6163 6365 7373 6962 6c65 5f6e 616d  s_accessible_nam
+00000340: 655f 6564 6974 5f6d 6f64 6522 3a20 2245  e_edit_mode": "E
+00000350: 6469 7461 7220 6172 7175 6976 6f22 2c0a  ditar arquivo",.
+00000360: 2020 2020 2265 6469 745f 6163 7469 6f6e      "edit_action
+00000370: 735f 736f 7572 6365 5f6d 6f64 6522 3a20  s_source_mode": 
+00000380: 2246 6f6e 7465 222c 0a20 2020 2022 6564  "Fonte",.    "ed
+00000390: 6974 5f61 6374 696f 6e73 5f61 6363 6573  it_actions_acces
+000003a0: 7369 626c 655f 6e61 6d65 5f73 6f75 7263  sible_name_sourc
+000003b0: 655f 6d6f 6465 223a 2022 43c3 b364 6967  e_mode": "C..dig
+000003c0: 6f2d 666f 6e74 6522 2c0a 2020 2020 2265  o-fonte",.    "e
+000003d0: 6469 745f 6163 7469 6f6e 735f 626f 6c64  dit_actions_bold
+000003e0: 223a 2022 4e65 6772 6974 6f22 2c0a 2020  ": "Negrito",.  
+000003f0: 2020 2265 6469 745f 6163 7469 6f6e 735f    "edit_actions_
+00000400: 6163 6365 7373 6962 6c65 5f6e 616d 655f  accessible_name_
+00000410: 626f 6c64 223a 2022 466f 726d 6174 6f20  bold": "Formato 
+00000420: 6465 2074 6578 746f 2065 6d20 6e65 6772  de texto em negr
+00000430: 6974 6f22 2c0a 2020 2020 2265 6469 745f  ito",.    "edit_
+00000440: 6163 7469 6f6e 735f 6974 616c 6963 223a  actions_italic":
+00000450: 2022 4974 c3a1 6c69 636f 222c 0a20 2020   "It..lico",.   
+00000460: 2022 6564 6974 5f61 6374 696f 6e73 5f61   "edit_actions_a
+00000470: 6363 6573 7369 626c 655f 6e61 6d65 5f69  ccessible_name_i
+00000480: 7461 6c69 6322 3a20 2246 6f72 6d61 746f  talic": "Formato
+00000490: 2064 6520 7465 7874 6f20 656d 2069 74c3   de texto em it.
+000004a0: a16c 6963 6f22 2c0a 2020 2020 2265 6469  .lico",.    "edi
+000004b0: 745f 6163 7469 6f6e 735f 756e 6465 726c  t_actions_underl
+000004c0: 696e 6522 3a20 2253 7562 6c69 6e68 6164  ine": "Sublinhad
+000004d0: 6f22 2c0a 2020 2020 2265 6469 745f 6163  o",.    "edit_ac
+000004e0: 7469 6f6e 735f 6163 6365 7373 6962 6c65  tions_accessible
+000004f0: 5f6e 616d 655f 756e 6465 726c 696e 6522  _name_underline"
+00000500: 3a20 2246 6f72 6d61 746f 2064 6520 7465  : "Formato de te
+00000510: 7874 6f20 7375 626c 696e 6861 646f 222c  xto sublinhado",
+00000520: 0a20 2020 2022 6564 6974 5f61 6374 696f  .    "edit_actio
+00000530: 6e73 5f73 7472 696b 6574 6872 6f75 6768  ns_strikethrough
+00000540: 223a 2022 5269 7363 6164 6f22 2c0a 2020  ": "Riscado",.  
+00000550: 2020 2265 6469 745f 6163 7469 6f6e 735f    "edit_actions_
+00000560: 6163 6365 7373 6962 6c65 5f6e 616d 655f  accessible_name_
+00000570: 7374 7269 6b65 7468 726f 7567 6822 3a20  strikethrough": 
+00000580: 2246 6f72 6d61 746f 2064 6520 7465 7874  "Formato de text
+00000590: 6f20 7269 7363 6164 6f22 2c0a 2020 2020  o riscado",.    
+000005a0: 2265 6469 745f 6163 7469 6f6e 735f 626c  "edit_actions_bl
+000005b0: 6f63 6b71 756f 7465 223a 2022 4369 7461  ockquote": "Cita
+000005c0: c3a7 c3a3 6f22 2c0a 2020 2020 2265 6469  ....o",.    "edi
+000005d0: 745f 6163 7469 6f6e 735f 6163 6365 7373  t_actions_access
+000005e0: 6962 6c65 5f6e 616d 655f 626c 6f63 6b71  ible_name_blockq
+000005f0: 756f 7465 223a 2022 466f 726d 6174 6f20  uote": "Formato 
+00000600: 6465 2074 6578 746f 2064 6520 6369 7461  de texto de cita
+00000610: c3a7 c3a3 6f22 2c0a 0a20 2020 2022 746f  ....o",..    "to
+00000620: 6f6c 735f 6163 7469 6f6e 735f 6169 5f61  ols_actions_ai_a
+00000630: 7373 6973 7461 6e74 223a 2022 4173 7369  ssistant": "Assi
+00000640: 7374 656e 7465 2064 6520 4941 222c 0a20  stente de IA",. 
+00000650: 2020 2022 746f 6f6c 735f 6163 7469 6f6e     "tools_action
+00000660: 735f 6163 6365 7373 6962 6c65 5f6e 616d  s_accessible_nam
+00000670: 655f 6169 5f61 7373 6973 7461 6e74 223a  e_ai_assistant":
+00000680: 2022 4c61 6ec3 a761 7220 4173 7369 7374   "Lan..ar Assist
+00000690: 656e 7465 2064 6520 4941 222c 0a20 2020  ente de IA",.   
+000006a0: 2022 746f 6f6c 735f 6163 7469 6f6e 735f   "tools_actions_
+000006b0: 636f 6c6f 725f 7069 636b 6572 223a 2022  color_picker": "
+000006c0: 5365 6c65 746f 7220 6465 2043 6f72 222c  Seletor de Cor",
+000006d0: 0a20 2020 2022 746f 6f6c 735f 6163 7469  .    "tools_acti
+000006e0: 6f6e 735f 6163 6365 7373 6962 6c65 5f6e  ons_accessible_n
+000006f0: 616d 655f 636f 6c6f 725f 7069 636b 6572  ame_color_picker
+00000700: 223a 2022 4573 636f 6c68 6572 2075 6d61  ": "Escolher uma
+00000710: 2063 6f72 2070 6172 6120 6f20 7465 7874   cor para o text
+00000720: 6f22 2c0a 0a20 2020 2022 6163 7469 6f6e  o",..    "action
+00000730: 735f 6865 6c70 5f6c 6162 656c 5f6d 645f  s_help_label_md_
+00000740: 7379 6e74 6178 223a 2022 5369 6e74 6178  syntax": "Sintax
+00000750: 6520 4d61 726b 646f 776e 222c 0a20 2020  e Markdown",.   
+00000760: 2022 6163 7469 6f6e 735f 6865 6c70 5f61   "actions_help_a
+00000770: 6363 6573 7369 626c 655f 6e61 6d65 5f6d  ccessible_name_m
+00000780: 645f 7379 6e74 6178 223a 2022 5369 6e74  d_syntax": "Sint
+00000790: 6178 6520 4d61 726b 646f 776e 222c 0a20  axe Markdown",. 
+000007a0: 2020 2022 6163 7469 6f6e 735f 6865 6c70     "actions_help
+000007b0: 5f6c 6162 656c 5f63 6865 636b 5f66 6f72  _label_check_for
+000007c0: 5f75 7064 6174 6573 223a 2022 5665 7269  _updates": "Veri
+000007d0: 6669 6361 7220 6174 7561 6c69 7a61 c3a7  ficar atualiza..
+000007e0: c3b5 6573 222c 0a20 2020 2022 6163 7469  ..es",.    "acti
+000007f0: 6f6e 735f 6865 6c70 5f61 6363 6573 7369  ons_help_accessi
+00000800: 626c 655f 6e61 6d65 5f63 6865 636b 5f66  ble_name_check_f
+00000810: 6f72 5f75 7064 6174 6573 223a 2022 5665  or_updates": "Ve
+00000820: 7269 6669 6361 7220 6174 7561 6c69 7a61  rificar atualiza
+00000830: c3a7 c3b5 6573 222c 0a20 2020 2022 6163  ....es",.    "ac
+00000840: 7469 6f6e 735f 6865 6c70 5f6c 6162 656c  tions_help_label
+00000850: 5f62 7567 5f72 6570 6f72 7422 3a20 2252  _bug_report": "R
+00000860: 656c 6174 6172 2062 7567 222c 0a20 2020  elatar bug",.   
+00000870: 2022 6163 7469 6f6e 735f 6865 6c70 5f61   "actions_help_a
+00000880: 6363 6573 7369 626c 655f 6e61 6d65 5f62  ccessible_name_b
+00000890: 7567 5f72 6570 6f72 7422 3a20 2245 6e76  ug_report": "Env
+000008a0: 6961 7220 7265 6c61 74c3 b372 696f 2064  iar relat..rio d
+000008b0: 6520 6275 6722 2c0a 2020 2020 2261 6374  e bug",.    "act
+000008c0: 696f 6e73 5f68 656c 705f 6c61 6265 6c5f  ions_help_label_
+000008d0: 6162 6f75 7422 3a20 2253 6f62 7265 222c  about": "Sobre",
+000008e0: 0a20 2020 2022 6163 7469 6f6e 735f 6865  .    "actions_he
+000008f0: 6c70 5f61 6363 6573 7369 626c 655f 6e61  lp_accessible_na
+00000900: 6d65 5f61 626f 7574 223a 2022 536f 6272  me_about": "Sobr
+00000910: 6522 2c0a 7d0a                           e",.}.
```

### Comparing `notolog-0.9.1b1/app/lexemes/de/__pycache__/statusbar.cpython-39.pyc` & `notolog-0.9.1b2/notolog/lexemes/en/statusbar.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,80 +1,76 @@
-00000000: 610d 0d0a 0000 0000 b254 2c66 c904 0000  a........T,f....
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0012 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
-00000030: 6401 6402 6403 6404 6405 6406 6407 6408  d.d.d.d.d.d.d.d.
-00000040: 6409 640a 640b 640c 640d 640e 640f 6410  d.d.d.d.d.d.d.d.
-00000050: 6411 9c11 5a00 6412 5300 2913 5a0a 5061  d...Z.d.S.).Z.Pa
-00000060: 7069 6572 6b6f 7262 7a1f 496e 6861 6c74  pierkorbz.Inhalt
-00000070: 2064 6573 2050 6170 6965 726b 6f72 6273   des Papierkorbs
-00000080: 2061 6e7a 6569 6765 6e73 0400 0000 f09f   anzeigens......
-00000090: 92be 7304 0000 00f0 9f94 9273 0400 0000  ..s........s....
-000000a0: f09f 9493 5a0d 416e 7369 6368 7473 6d6f  ....Z.Ansichtsmo
-000000b0: 6475 735a 1142 6561 7262 6569 7475 6e67  dusZ.Bearbeitung
-000000c0: 736d 6f64 7573 5a0a 5175 656c 6c6d 6f64  smodusZ.Quellmod
-000000d0: 7573 da08 4d61 726b 646f 776e da04 4854  us..Markdown..HT
-000000e0: 4d4c 7a13 7b65 6e63 7279 7074 696f 6e7d  MLz.{encryption}
-000000f0: 207b 6963 6f6e 7d5a 044b 6c61 7275 0e00   {icon}Z.Klaru..
-00000100: 0000 5665 7273 6368 6cc3 bc73 7365 6c74  ..Verschl..sselt
-00000110: 751e 0000 005a 6569 6c65 3a20 7b6c 696e  u....Zeile: {lin
-00000120: 657d 20e2 8692 2053 703a 207b 636f 6c75  e} ... Sp: {colu
-00000130: 6d6e 7d75 3300 0000 5a65 696c 653a 207b  mn}u3...Zeile: {
-00000140: 6c69 6e65 7d20 e286 9220 5370 3a20 7b63  line} ... Sp: {c
-00000150: 6f6c 756d 6e7d 20e2 8692 2041 7573 773a  olumn} ... Ausw:
-00000160: 207b 7365 6c65 6374 6564 7d75 3200 0000   {selected}u2...
-00000170: 5a65 696c 653a 207b 6c69 6e65 7d20 e286  Zeile: {line} ..
-00000180: 9220 5370 3a20 7b63 6f6c 756d 6e7d 20e2  . Sp: {column} .
-00000190: 8692 2050 6f73 3a20 7b70 6f73 6974 696f  .. Pos: {positio
-000001a0: 6e7d 7547 0000 005a 6569 6c65 3a20 7b6c  n}uG...Zeile: {l
-000001b0: 696e 657d 20e2 8692 2053 703a 207b 636f  ine} ... Sp: {co
-000001c0: 6c75 6d6e 7d20 e286 9220 506f 733a 207b  lumn} ... Pos: {
-000001d0: 706f 7369 7469 6f6e 7d20 e286 9220 4175  position} ... Au
-000001e0: 7377 3a20 7b73 656c 6563 7465 647d 2911  sw: {selected}).
-000001f0: da1a 7374 6174 7573 6261 725f 6c69 7474  ..statusbar_litt
-00000200: 6572 5f62 696e 5f6c 6162 656c da24 7374  er_bin_label.$st
-00000210: 6174 7573 6261 725f 6c69 7474 6572 5f62  atusbar_litter_b
-00000220: 696e 5f61 6363 6573 7369 626c 655f 6e61  in_accessible_na
-00000230: 6d65 da1d 7374 6174 7573 6261 725f 7361  me..statusbar_sa
-00000240: 7665 5f70 726f 6772 6573 735f 6c61 6265  ve_progress_labe
-00000250: 6cda 2b73 7461 7475 7362 6172 5f65 6e63  l.+statusbar_enc
-00000260: 7279 7074 696f 6e5f 7379 6d62 6f6c 5f65  ryption_symbol_e
-00000270: 6e63 7279 7074 6564 5f6c 6162 656c da2d  ncrypted_label.-
+00000000: 2320 456e 676c 6973 6820 6c65 7865 6d65  # English lexeme
+00000010: 7320 7374 6174 7573 6261 722e 7079 0a6c  s statusbar.py.l
+00000020: 6578 656d 6573 203d 207b 0a20 2020 2022  exemes = {.    "
+00000030: 7374 6174 7573 6261 725f 6c69 7474 6572  statusbar_litter
+00000040: 5f62 696e 5f6c 6162 656c 223a 2022 4c69  _bin_label": "Li
+00000050: 7474 6572 2062 696e 222c 0a20 2020 2022  tter bin",.    "
+00000060: 7374 6174 7573 6261 725f 6c69 7474 6572  statusbar_litter
+00000070: 5f62 696e 5f61 6363 6573 7369 626c 655f  _bin_accessible_
+00000080: 6e61 6d65 223a 2022 5368 6f77 206c 6974  name": "Show lit
+00000090: 7465 7220 6269 6e20 636f 6e74 656e 7422  ter bin content"
+000000a0: 2c0a 0a20 2020 2022 7374 6174 7573 6261  ,..    "statusba
+000000b0: 725f 7361 7665 5f70 726f 6772 6573 735f  r_save_progress_
+000000c0: 6c61 6265 6c22 3a20 6227 5c78 6630 5c78  label": b'\xf0\x
+000000d0: 3966 5c78 3932 5c78 6265 272c 0a20 2020  9f\x92\xbe',.   
+000000e0: 2022 7374 6174 7573 6261 725f 656e 6372   "statusbar_encr
+000000f0: 7970 7469 6f6e 5f73 796d 626f 6c5f 656e  yption_symbol_en
+00000100: 6372 7970 7465 645f 6c61 6265 6c22 3a20  crypted_label": 
+00000110: 6227 5c78 6630 5c78 3966 5c78 3934 5c78  b'\xf0\x9f\x94\x
+00000120: 3932 272c 0a20 2020 2022 7374 6174 7573  92',.    "status
+00000130: 6261 725f 656e 6372 7970 7469 6f6e 5f73  bar_encryption_s
+00000140: 796d 626f 6c5f 756e 656e 6372 7970 7465  ymbol_unencrypte
+00000150: 645f 6c61 6265 6c22 3a20 6227 5c78 6630  d_label": b'\xf0
+00000160: 5c78 3966 5c78 3934 5c78 3933 272c 0a0a  \x9f\x94\x93',..
+00000170: 2020 2020 2273 7461 7475 7362 6172 5f6d      "statusbar_m
+00000180: 6f64 655f 6c61 6265 6c5f 6d6f 6465 5f76  ode_label_mode_v
+00000190: 6965 7722 3a20 2256 6965 7720 6d6f 6465  iew": "View mode
+000001a0: 222c 0a20 2020 2022 7374 6174 7573 6261  ",.    "statusba
+000001b0: 725f 6d6f 6465 5f6c 6162 656c 5f6d 6f64  r_mode_label_mod
+000001c0: 655f 6564 6974 223a 2022 4564 6974 206d  e_edit": "Edit m
+000001d0: 6f64 6522 2c0a 2020 2020 2273 7461 7475  ode",.    "statu
+000001e0: 7362 6172 5f6d 6f64 655f 6c61 6265 6c5f  sbar_mode_label_
+000001f0: 6d6f 6465 5f73 6f75 7263 6522 3a20 2253  mode_source": "S
+00000200: 6f75 7263 6520 6d6f 6465 222c 0a0a 2020  ource mode",..  
+00000210: 2020 2273 7461 7475 7362 6172 5f73 6f75    "statusbar_sou
+00000220: 7263 655f 6c61 6265 6c5f 736f 7572 6365  rce_label_source
+00000230: 5f6d 6172 6b64 6f77 6e22 3a20 224d 6172  _markdown": "Mar
+00000240: 6b64 6f77 6e22 2c0a 2020 2020 2273 7461  kdown",.    "sta
+00000250: 7475 7362 6172 5f73 6f75 7263 655f 6c61  tusbar_source_la
+00000260: 6265 6c5f 736f 7572 6365 5f68 746d 6c22  bel_source_html"
+00000270: 3a20 2248 544d 4c22 2c0a 0a20 2020 2022  : "HTML",..    "
 00000280: 7374 6174 7573 6261 725f 656e 6372 7970  statusbar_encryp
-00000290: 7469 6f6e 5f73 796d 626f 6c5f 756e 656e  tion_symbol_unen
-000002a0: 6372 7970 7465 645f 6c61 6265 6cda 1e73  crypted_label..s
-000002b0: 7461 7475 7362 6172 5f6d 6f64 655f 6c61  tatusbar_mode_la
-000002c0: 6265 6c5f 6d6f 6465 5f76 6965 77da 1e73  bel_mode_view..s
-000002d0: 7461 7475 7362 6172 5f6d 6f64 655f 6c61  tatusbar_mode_la
-000002e0: 6265 6c5f 6d6f 6465 5f65 6469 74da 2073  bel_mode_edit. s
-000002f0: 7461 7475 7362 6172 5f6d 6f64 655f 6c61  tatusbar_mode_la
-00000300: 6265 6c5f 6d6f 6465 5f73 6f75 7263 65da  bel_mode_source.
-00000310: 2673 7461 7475 7362 6172 5f73 6f75 7263  &statusbar_sourc
-00000320: 655f 6c61 6265 6c5f 736f 7572 6365 5f6d  e_label_source_m
-00000330: 6172 6b64 6f77 6eda 2273 7461 7475 7362  arkdown."statusb
-00000340: 6172 5f73 6f75 7263 655f 6c61 6265 6c5f  ar_source_label_
-00000350: 736f 7572 6365 5f68 746d 6cda 1a73 7461  source_html..sta
-00000360: 7475 7362 6172 5f65 6e63 7279 7074 696f  tusbar_encryptio
-00000370: 6e5f 6c61 6265 6cda 2b73 7461 7475 7362  n_label.+statusb
-00000380: 6172 5f65 6e63 7279 7074 696f 6e5f 6c61  ar_encryption_la
-00000390: 6265 6c5f 656e 6372 7970 7469 6f6e 5f70  bel_encryption_p
-000003a0: 6c61 696e da2f 7374 6174 7573 6261 725f  lain./statusbar_
-000003b0: 656e 6372 7970 7469 6f6e 5f6c 6162 656c  encryption_label
-000003c0: 5f65 6e63 7279 7074 696f 6e5f 656e 6372  _encryption_encr
-000003d0: 7970 7465 64da 1673 7461 7475 7362 6172  ypted..statusbar
-000003e0: 5f63 7572 736f 725f 6c61 6265 6cda 1f73  _cursor_label..s
-000003f0: 7461 7475 7362 6172 5f63 7572 736f 725f  tatusbar_cursor_
-00000400: 6c61 6265 6c5f 7365 6c65 6374 6564 da22  label_selected."
-00000410: 7374 6174 7573 6261 725f 6375 7273 6f72  statusbar_cursor
-00000420: 5f6c 6162 656c 5f77 6974 685f 676c 6f62  _label_with_glob
-00000430: 616c da2b 7374 6174 7573 6261 725f 6375  al.+statusbar_cu
-00000440: 7273 6f72 5f6c 6162 656c 5f73 656c 6563  rsor_label_selec
-00000450: 7465 645f 7769 7468 5f67 6c6f 6261 6c4e  ted_with_globalN
-00000460: 2901 da07 6c65 7865 6d65 73a9 0072 1500  )...lexemes..r..
-00000470: 0000 7215 0000 00fa 4a2f 5573 6572 732f  ..r.....J/Users/
-00000480: 7661 6469 6b75 732f 5079 6368 6172 6d50  vadikus/PycharmP
-00000490: 726f 6a65 6374 732f 6e6f 746f 6c6f 672d  rojects/notolog-
-000004a0: 6465 762f 6e6f 746f 6c6f 672f 6c65 7865  dev/notolog/lexe
-000004b0: 6d65 732f 6465 2f73 7461 7475 7362 6172  mes/de/statusbar
-000004c0: 2e70 79da 083c 6d6f 6475 6c65 3e03 0000  .py..<module>...
-000004d0: 0073 2200 0000 0201 0202 0201 0201 0202  .s".............
-000004e0: 0201 0201 0202 0201 0202 0201 0201 0202  ................
-000004f0: 0201 0201 0201 02ea                      ........
+00000290: 7469 6f6e 5f6c 6162 656c 223a 2022 7b65  tion_label": "{e
+000002a0: 6e63 7279 7074 696f 6e7d 207b 6963 6f6e  ncryption} {icon
+000002b0: 7d22 2c0a 2020 2020 2273 7461 7475 7362  }",.    "statusb
+000002c0: 6172 5f65 6e63 7279 7074 696f 6e5f 6c61  ar_encryption_la
+000002d0: 6265 6c5f 656e 6372 7970 7469 6f6e 5f70  bel_encryption_p
+000002e0: 6c61 696e 223a 2022 506c 6169 6e22 2c0a  lain": "Plain",.
+000002f0: 2020 2020 2273 7461 7475 7362 6172 5f65      "statusbar_e
+00000300: 6e63 7279 7074 696f 6e5f 6c61 6265 6c5f  ncryption_label_
+00000310: 656e 6372 7970 7469 6f6e 5f65 6e63 7279  encryption_encry
+00000320: 7074 6564 223a 2022 456e 6372 7970 7465  pted": "Encrypte
+00000330: 6422 2c0a 0a20 2020 2022 7374 6174 7573  d",..    "status
+00000340: 6261 725f 6375 7273 6f72 5f6c 6162 656c  bar_cursor_label
+00000350: 223a 2022 6c69 6e65 3a20 7b6c 696e 657d  ": "line: {line}
+00000360: 20e2 8692 2063 6f6c 3a20 7b63 6f6c 756d   ... col: {colum
+00000370: 6e7d 222c 0a20 2020 2022 7374 6174 7573  n}",.    "status
+00000380: 6261 725f 6375 7273 6f72 5f6c 6162 656c  bar_cursor_label
+00000390: 5f73 656c 6563 7465 6422 3a20 226c 696e  _selected": "lin
+000003a0: 653a 207b 6c69 6e65 7d20 e286 9220 636f  e: {line} ... co
+000003b0: 6c3a 207b 636f 6c75 6d6e 7d20 e286 9220  l: {column} ... 
+000003c0: 7365 6c3a 207b 7365 6c65 6374 6564 7d22  sel: {selected}"
+000003d0: 2c0a 2020 2020 2273 7461 7475 7362 6172  ,.    "statusbar
+000003e0: 5f63 7572 736f 725f 6c61 6265 6c5f 7769  _cursor_label_wi
+000003f0: 7468 5f67 6c6f 6261 6c22 3a20 226c 696e  th_global": "lin
+00000400: 653a 207b 6c69 6e65 7d20 e286 9220 636f  e: {line} ... co
+00000410: 6c3a 207b 636f 6c75 6d6e 7d20 e286 9220  l: {column} ... 
+00000420: 706f 733a 207b 706f 7369 7469 6f6e 7d22  pos: {position}"
+00000430: 2c0a 2020 2020 2273 7461 7475 7362 6172  ,.    "statusbar
+00000440: 5f63 7572 736f 725f 6c61 6265 6c5f 7365  _cursor_label_se
+00000450: 6c65 6374 6564 5f77 6974 685f 676c 6f62  lected_with_glob
+00000460: 616c 223a 2022 6c69 6e65 3a20 7b6c 696e  al": "line: {lin
+00000470: 657d 20e2 8692 2063 6f6c 3a20 7b63 6f6c  e} ... col: {col
+00000480: 756d 6e7d 20e2 8692 2070 6f73 3a20 7b70  umn} ... pos: {p
+00000490: 6f73 6974 696f 6e7d 20e2 8692 2073 656c  osition} ... sel
+000004a0: 3a20 7b73 656c 6563 7465 647d 222c 0a7d  : {selected}",.}
+000004b0: 0a                                       .
```

### Comparing `notolog-0.9.1b1/app/lexemes/de/ai_assistant.py` & `notolog-0.9.1b2/notolog/lexemes/de/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/de/color_picker_dialog.py` & `notolog-0.9.1b2/notolog/lexemes/de/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/de/common.py` & `notolog-0.9.1b2/notolog/lexemes/de/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     "save_active_file_error_occurred": "Datei kann nicht gespeichert werden, ein Fehler ist aufgetreten",
 
     "expandable_block_default_title": "Weitere Informationen...",
 
     "dialog_color_picker_color_copied_to_the_clipboard": "Formatierter Text wurde in die Zwischenablage kopiert",
 
     "popup_about_title": "Anwendungsinfo",
-    "popup_about_app_name_description": "Markdown Editor",
+    "popup_about_app_name_description": "Python Markdown-Editor",
 
     "popup_about_version": "Version",
     "popup_about_license": "Lizenz",
     "popup_about_website": "Webseite",
     "popup_about_repository": "GitHub",
     "popup_about_pypi": "PyPi",
     "popup_about_date": "Datum",
```

### Comparing `notolog-0.9.1b1/app/lexemes/de/main_menu.py` & `notolog-0.9.1b2/notolog/lexemes/de/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/de/settings_dialog.py` & `notolog-0.9.1b2/notolog/lexemes/de/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/de/statusbar.py` & `notolog-0.9.1b2/notolog/lexemes/de/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/de/toolbar.py` & `notolog-0.9.1b2/notolog/lexemes/de/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/en/ai_assistant.py` & `notolog-0.9.1b2/notolog/lexemes/en/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/en/color_picker_dialog.py` & `notolog-0.9.1b2/notolog/lexemes/en/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/en/common.py` & `notolog-0.9.1b2/notolog/lexemes/en/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     "save_active_file_error_occurred": "Cannot save file, error occurred",
 
     "expandable_block_default_title": "More info...",
 
     "dialog_color_picker_color_copied_to_the_clipboard": "Formatted text has been copied to the clipboard",
 
     "popup_about_title": "Application Info",
-    "popup_about_app_name_description": "Markdown Editor",
+    "popup_about_app_name_description": "Python Markdown Editor",
 
     "popup_about_version": "Version",
     "popup_about_license": "License",
     "popup_about_website": "Website",
     "popup_about_repository": "GitHub",
     "popup_about_pypi": "PyPi",
     "popup_about_date": "Date",
```

### Comparing `notolog-0.9.1b1/app/lexemes/en/main_menu.py` & `notolog-0.9.1b2/notolog/lexemes/en/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/en/settings_dialog.py` & `notolog-0.9.1b2/notolog/lexemes/en/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/en/statusbar.py` & `notolog-0.9.1b2/notolog/lexemes/it/statusbar.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# English lexemes statusbar.py
+# Italian lexemes statusbar.py
 lexemes = {
-    "statusbar_litter_bin_label": "Litter bin",
-    "statusbar_litter_bin_accessible_name": "Show litter bin content",
+    "statusbar_litter_bin_label": "Cestino",
+    "statusbar_litter_bin_accessible_name": "Mostra il contenuto del cestino",
 
     "statusbar_save_progress_label": b'\xf0\x9f\x92\xbe',
     "statusbar_encryption_symbol_encrypted_label": b'\xf0\x9f\x94\x92',
     "statusbar_encryption_symbol_unencrypted_label": b'\xf0\x9f\x94\x93',
 
-    "statusbar_mode_label_mode_view": "View mode",
-    "statusbar_mode_label_mode_edit": "Edit mode",
-    "statusbar_mode_label_mode_source": "Source mode",
+    "statusbar_mode_label_mode_view": "Modalità Visualizza",
+    "statusbar_mode_label_mode_edit": "Modalità Modifica",
+    "statusbar_mode_label_mode_source": "Modalità Sorgente",
 
     "statusbar_source_label_source_markdown": "Markdown",
     "statusbar_source_label_source_html": "HTML",
 
     "statusbar_encryption_label": "{encryption} {icon}",
-    "statusbar_encryption_label_encryption_plain": "Plain",
-    "statusbar_encryption_label_encryption_encrypted": "Encrypted",
+    "statusbar_encryption_label_encryption_plain": "Normale",
+    "statusbar_encryption_label_encryption_encrypted": "Criptato",
 
-    "statusbar_cursor_label": "line: {line} → col: {column}",
-    "statusbar_cursor_label_selected": "line: {line} → col: {column} → sel: {selected}",
-    "statusbar_cursor_label_with_global": "line: {line} → col: {column} → pos: {position}",
-    "statusbar_cursor_label_selected_with_global": "line: {line} → col: {column} → pos: {position} → sel: {selected}",
+    "statusbar_cursor_label": "linea: {line} → col: {column}",
+    "statusbar_cursor_label_selected": "linea: {line} → col: {column} → sel: {selected}",
+    "statusbar_cursor_label_with_global": "linea: {line} → col: {column} → pos: {position}",
+    "statusbar_cursor_label_selected_with_global": "linea: {line} → col: {column} → pos: {position} → sel: {selected}",
 }
```

### Comparing `notolog-0.9.1b1/app/lexemes/en/toolbar.py` & `notolog-0.9.1b2/notolog/lexemes/en/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/es/ai_assistant.py` & `notolog-0.9.1b2/notolog/lexemes/es/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/es/color_picker_dialog.py` & `notolog-0.9.1b2/notolog/lexemes/es/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/es/common.py` & `notolog-0.9.1b2/notolog/lexemes/es/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     "save_active_file_error_occurred": "No se puede guardar el archivo, ocurrió un error",
 
     "expandable_block_default_title": "Más información...",
 
     "dialog_color_picker_color_copied_to_the_clipboard": "El texto formateado ha sido copiado al portapapeles",
 
     "popup_about_title": "Información de la Aplicación",
-    "popup_about_app_name_description": "Editor Markdown",
+    "popup_about_app_name_description": "Editor Markdown de Python",
 
     "popup_about_version": "Versión",
     "popup_about_license": "Licencia",
     "popup_about_website": "Sitio Web",
     "popup_about_repository": "GitHub",
     "popup_about_pypi": "PyPi",
     "popup_about_date": "Fecha",
@@ -107,8 +107,8 @@
         "Host no encontrado. Puede haber un problema con la conexión a internet o DNS.",
     "network_connection_error_connection_refused":
         "Conexión rechazada. El servidor podría estar caído o puede haber problemas de red.",
     "network_connection_error_connection_timed_out": "Tiempo de conexión agotado. Puede haber problemas de red.",
     "network_connection_error_connection_404_error":
         "Error de conexión 404. La página o recurso solicitado no se encuentra.",
     "network_connection_error_generic_with_status_code": "La solicitud falló con el código de estado: {status_code}",
-}
+}
```

### Comparing `notolog-0.9.1b1/app/lexemes/es/main_menu.py` & `notolog-0.9.1b2/notolog/lexemes/es/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/es/settings_dialog.py` & `notolog-0.9.1b2/notolog/lexemes/es/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/es/statusbar.py` & `notolog-0.9.1b2/notolog/lexemes/es/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/es/toolbar.py` & `notolog-0.9.1b2/notolog/lexemes/es/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/fi/ai_assistant.py` & `notolog-0.9.1b2/notolog/lexemes/fi/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/fi/color_picker_dialog.py` & `notolog-0.9.1b2/notolog/lexemes/fi/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/fi/common.py` & `notolog-0.9.1b2/notolog/lexemes/fi/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     "save_active_file_error_occurred": "Tiedostoa ei voi tallentaa, tapahtui virhe",
 
     "expandable_block_default_title": "Lisätietoja...",
 
     "dialog_color_picker_color_copied_to_the_clipboard": "Muotoiltu teksti on kopioitu leikepöydälle",
 
     "popup_about_title": "Sovelluksen tiedot",
-    "popup_about_app_name_description": "Markdown Editori",
+    "popup_about_app_name_description": "Python Markdown -editori",
 
     "popup_about_version": "Versio",
     "popup_about_license": "Lisenssi",
     "popup_about_website": "Verkkosivusto",
     "popup_about_repository": "GitHub",
     "popup_about_pypi": "PyPi",
     "popup_about_date": "Päivämäärä",
```

### Comparing `notolog-0.9.1b1/app/lexemes/fi/main_menu.py` & `notolog-0.9.1b2/notolog/lexemes/fi/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/fi/settings_dialog.py` & `notolog-0.9.1b2/notolog/lexemes/fi/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/fi/statusbar.py` & `notolog-0.9.1b2/notolog/lexemes/fi/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/fi/toolbar.py` & `notolog-0.9.1b2/notolog/lexemes/fi/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/fr/__pycache__/statusbar.cpython-39.pyc` & `notolog-0.9.1b2/notolog/lexemes/fr/statusbar.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,80 +1,78 @@
-00000000: 610d 0d0a 0000 0000 020f 3066 d404 0000  a.........0f....
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0012 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
-00000030: 6401 6402 6403 6404 6405 6406 6407 6408  d.d.d.d.d.d.d.d.
-00000040: 6409 640a 640b 640c 640d 640e 640f 6410  d.d.d.d.d.d.d.d.
-00000050: 6411 9c11 5a00 6412 5300 2913 5a09 436f  d...Z.d.S.).Z.Co
-00000060: 7262 6569 6c6c 657a 2341 6666 6963 6865  rbeillez#Affiche
-00000070: 7220 6c65 2063 6f6e 7465 6e75 2064 6520  r le contenu de 
-00000080: 6c61 2063 6f72 6265 696c 6c65 7304 0000  la corbeilles...
-00000090: 00f0 9f92 be73 0400 0000 f09f 9492 7304  .....s........s.
-000000a0: 0000 00f0 9f94 937a 084d 6f64 6520 5675  .......z.Mode Vu
-000000b0: 6575 0d00 0000 4d6f 6465 20c3 8964 6974  eu....Mode ..dit
-000000c0: 696f 6e7a 0b4d 6f64 6520 536f 7572 6365  ionz.Mode Source
-000000d0: da08 4d61 726b 646f 776e da04 4854 4d4c  ..Markdown..HTML
-000000e0: 7a13 7b65 6e63 7279 7074 696f 6e7d 207b  z.{encryption} {
-000000f0: 6963 6f6e 7d5a 0543 6c61 6972 7507 0000  icon}Z.Clairu...
-00000100: 0043 7279 7074 c3a9 7521 0000 006c 6967  .Crypt..u!...lig
-00000110: 6e65 203a 207b 6c69 6e65 7d20 e286 9220  ne : {line} ... 
-00000120: 636f 6c20 3a20 7b63 6f6c 756d 6e7d 7536  col : {column}u6
-00000130: 0000 006c 6967 6e65 203a 207b 6c69 6e65  ...ligne : {line
-00000140: 7d20 e286 9220 636f 6c20 3a20 7b63 6f6c  } ... col : {col
-00000150: 756d 6e7d 20e2 8692 2073 656c 203a 207b  umn} ... sel : {
-00000160: 7365 6c65 6374 6564 7d75 3600 0000 6c69  selected}u6...li
-00000170: 676e 6520 3a20 7b6c 696e 657d 20e2 8692  gne : {line} ...
-00000180: 2063 6f6c 203a 207b 636f 6c75 6d6e 7d20   col : {column} 
-00000190: e286 9220 706f 7320 3a20 7b70 6f73 6974  ... pos : {posit
-000001a0: 696f 6e7d 754b 0000 006c 6967 6e65 203a  ion}uK...ligne :
-000001b0: 207b 6c69 6e65 7d20 e286 9220 636f 6c20   {line} ... col 
-000001c0: 3a20 7b63 6f6c 756d 6e7d 20e2 8692 2070  : {column} ... p
-000001d0: 6f73 203a 207b 706f 7369 7469 6f6e 7d20  os : {position} 
-000001e0: e286 9220 7365 6c20 3a20 7b73 656c 6563  ... sel : {selec
-000001f0: 7465 647d 2911 da1a 7374 6174 7573 6261  ted})...statusba
-00000200: 725f 6c69 7474 6572 5f62 696e 5f6c 6162  r_litter_bin_lab
-00000210: 656c da24 7374 6174 7573 6261 725f 6c69  el.$statusbar_li
-00000220: 7474 6572 5f62 696e 5f61 6363 6573 7369  tter_bin_accessi
-00000230: 626c 655f 6e61 6d65 da1d 7374 6174 7573  ble_name..status
-00000240: 6261 725f 7361 7665 5f70 726f 6772 6573  bar_save_progres
-00000250: 735f 6c61 6265 6cda 2b73 7461 7475 7362  s_label.+statusb
-00000260: 6172 5f65 6e63 7279 7074 696f 6e5f 7379  ar_encryption_sy
-00000270: 6d62 6f6c 5f65 6e63 7279 7074 6564 5f6c  mbol_encrypted_l
-00000280: 6162 656c da2d 7374 6174 7573 6261 725f  abel.-statusbar_
-00000290: 656e 6372 7970 7469 6f6e 5f73 796d 626f  encryption_symbo
-000002a0: 6c5f 756e 656e 6372 7970 7465 645f 6c61  l_unencrypted_la
-000002b0: 6265 6cda 1e73 7461 7475 7362 6172 5f6d  bel..statusbar_m
-000002c0: 6f64 655f 6c61 6265 6c5f 6d6f 6465 5f76  ode_label_mode_v
-000002d0: 6965 77da 1e73 7461 7475 7362 6172 5f6d  iew..statusbar_m
-000002e0: 6f64 655f 6c61 6265 6c5f 6d6f 6465 5f65  ode_label_mode_e
-000002f0: 6469 74da 2073 7461 7475 7362 6172 5f6d  dit. statusbar_m
-00000300: 6f64 655f 6c61 6265 6c5f 6d6f 6465 5f73  ode_label_mode_s
-00000310: 6f75 7263 65da 2673 7461 7475 7362 6172  ource.&statusbar
-00000320: 5f73 6f75 7263 655f 6c61 6265 6c5f 736f  _source_label_so
-00000330: 7572 6365 5f6d 6172 6b64 6f77 6eda 2273  urce_markdown."s
-00000340: 7461 7475 7362 6172 5f73 6f75 7263 655f  tatusbar_source_
-00000350: 6c61 6265 6c5f 736f 7572 6365 5f68 746d  label_source_htm
-00000360: 6cda 1a73 7461 7475 7362 6172 5f65 6e63  l..statusbar_enc
-00000370: 7279 7074 696f 6e5f 6c61 6265 6cda 2b73  ryption_label.+s
-00000380: 7461 7475 7362 6172 5f65 6e63 7279 7074  tatusbar_encrypt
-00000390: 696f 6e5f 6c61 6265 6c5f 656e 6372 7970  ion_label_encryp
-000003a0: 7469 6f6e 5f70 6c61 696e da2f 7374 6174  tion_plain./stat
-000003b0: 7573 6261 725f 656e 6372 7970 7469 6f6e  usbar_encryption
-000003c0: 5f6c 6162 656c 5f65 6e63 7279 7074 696f  _label_encryptio
-000003d0: 6e5f 656e 6372 7970 7465 64da 1673 7461  n_encrypted..sta
-000003e0: 7475 7362 6172 5f63 7572 736f 725f 6c61  tusbar_cursor_la
-000003f0: 6265 6cda 1f73 7461 7475 7362 6172 5f63  bel..statusbar_c
-00000400: 7572 736f 725f 6c61 6265 6c5f 7365 6c65  ursor_label_sele
-00000410: 6374 6564 da22 7374 6174 7573 6261 725f  cted."statusbar_
-00000420: 6375 7273 6f72 5f6c 6162 656c 5f77 6974  cursor_label_wit
-00000430: 685f 676c 6f62 616c da2b 7374 6174 7573  h_global.+status
-00000440: 6261 725f 6375 7273 6f72 5f6c 6162 656c  bar_cursor_label
-00000450: 5f73 656c 6563 7465 645f 7769 7468 5f67  _selected_with_g
-00000460: 6c6f 6261 6c4e 2901 da07 6c65 7865 6d65  lobalN)...lexeme
-00000470: 73a9 0072 1500 0000 7215 0000 00fa 462f  s..r....r.....F/
-00000480: 5573 6572 732f 7661 6469 6b75 732f 5079  Users/vadikus/Py
-00000490: 6368 6172 6d50 726f 6a65 6374 732f 6e6f  charmProjects/no
-000004a0: 746f 6c6f 672d 6465 762f 6170 702f 6c65  tolog-dev/app/le
-000004b0: 7865 6d65 732f 6672 2f73 7461 7475 7362  xemes/fr/statusb
-000004c0: 6172 2e70 79da 083c 6d6f 6475 6c65 3e03  ar.py..<module>.
-000004d0: 0000 0073 2200 0000 0201 0202 0201 0201  ...s"...........
-000004e0: 0202 0201 0201 0202 0201 0202 0201 0201  ................
-000004f0: 0202 0201 0201 0202 02e9                 ..........
+00000000: 2320 4672 656e 6368 206c 6578 656d 6573  # French lexemes
+00000010: 2073 7461 7475 7362 6172 2e70 790a 6c65   statusbar.py.le
+00000020: 7865 6d65 7320 3d20 7b0a 2020 2020 2273  xemes = {.    "s
+00000030: 7461 7475 7362 6172 5f6c 6974 7465 725f  tatusbar_litter_
+00000040: 6269 6e5f 6c61 6265 6c22 3a20 2243 6f72  bin_label": "Cor
+00000050: 6265 696c 6c65 222c 0a20 2020 2022 7374  beille",.    "st
+00000060: 6174 7573 6261 725f 6c69 7474 6572 5f62  atusbar_litter_b
+00000070: 696e 5f61 6363 6573 7369 626c 655f 6e61  in_accessible_na
+00000080: 6d65 223a 2022 4166 6669 6368 6572 206c  me": "Afficher l
+00000090: 6520 636f 6e74 656e 7520 6465 206c 6120  e contenu de la 
+000000a0: 636f 7262 6569 6c6c 6522 2c0a 0a20 2020  corbeille",..   
+000000b0: 2022 7374 6174 7573 6261 725f 7361 7665   "statusbar_save
+000000c0: 5f70 726f 6772 6573 735f 6c61 6265 6c22  _progress_label"
+000000d0: 3a20 6227 5c78 6630 5c78 3966 5c78 3932  : b'\xf0\x9f\x92
+000000e0: 5c78 6265 272c 0a20 2020 2022 7374 6174  \xbe',.    "stat
+000000f0: 7573 6261 725f 656e 6372 7970 7469 6f6e  usbar_encryption
+00000100: 5f73 796d 626f 6c5f 656e 6372 7970 7465  _symbol_encrypte
+00000110: 645f 6c61 6265 6c22 3a20 6227 5c78 6630  d_label": b'\xf0
+00000120: 5c78 3966 5c78 3934 5c78 3932 272c 0a20  \x9f\x94\x92',. 
+00000130: 2020 2022 7374 6174 7573 6261 725f 656e     "statusbar_en
+00000140: 6372 7970 7469 6f6e 5f73 796d 626f 6c5f  cryption_symbol_
+00000150: 756e 656e 6372 7970 7465 645f 6c61 6265  unencrypted_labe
+00000160: 6c22 3a20 6227 5c78 6630 5c78 3966 5c78  l": b'\xf0\x9f\x
+00000170: 3934 5c78 3933 272c 0a0a 2020 2020 2273  94\x93',..    "s
+00000180: 7461 7475 7362 6172 5f6d 6f64 655f 6c61  tatusbar_mode_la
+00000190: 6265 6c5f 6d6f 6465 5f76 6965 7722 3a20  bel_mode_view": 
+000001a0: 224d 6f64 6520 5675 6522 2c0a 2020 2020  "Mode Vue",.    
+000001b0: 2273 7461 7475 7362 6172 5f6d 6f64 655f  "statusbar_mode_
+000001c0: 6c61 6265 6c5f 6d6f 6465 5f65 6469 7422  label_mode_edit"
+000001d0: 3a20 224d 6f64 6520 c389 6469 7469 6f6e  : "Mode ..dition
+000001e0: 222c 0a20 2020 2022 7374 6174 7573 6261  ",.    "statusba
+000001f0: 725f 6d6f 6465 5f6c 6162 656c 5f6d 6f64  r_mode_label_mod
+00000200: 655f 736f 7572 6365 223a 2022 4d6f 6465  e_source": "Mode
+00000210: 2053 6f75 7263 6522 2c0a 0a20 2020 2022   Source",..    "
+00000220: 7374 6174 7573 6261 725f 736f 7572 6365  statusbar_source
+00000230: 5f6c 6162 656c 5f73 6f75 7263 655f 6d61  _label_source_ma
+00000240: 726b 646f 776e 223a 2022 4d61 726b 646f  rkdown": "Markdo
+00000250: 776e 222c 0a20 2020 2022 7374 6174 7573  wn",.    "status
+00000260: 6261 725f 736f 7572 6365 5f6c 6162 656c  bar_source_label
+00000270: 5f73 6f75 7263 655f 6874 6d6c 223a 2022  _source_html": "
+00000280: 4854 4d4c 222c 0a0a 2020 2020 2273 7461  HTML",..    "sta
+00000290: 7475 7362 6172 5f65 6e63 7279 7074 696f  tusbar_encryptio
+000002a0: 6e5f 6c61 6265 6c22 3a20 227b 656e 6372  n_label": "{encr
+000002b0: 7970 7469 6f6e 7d20 7b69 636f 6e7d 222c  yption} {icon}",
+000002c0: 0a20 2020 2022 7374 6174 7573 6261 725f  .    "statusbar_
+000002d0: 656e 6372 7970 7469 6f6e 5f6c 6162 656c  encryption_label
+000002e0: 5f65 6e63 7279 7074 696f 6e5f 706c 6169  _encryption_plai
+000002f0: 6e22 3a20 2243 6c61 6972 222c 0a20 2020  n": "Clair",.   
+00000300: 2022 7374 6174 7573 6261 725f 656e 6372   "statusbar_encr
+00000310: 7970 7469 6f6e 5f6c 6162 656c 5f65 6e63  yption_label_enc
+00000320: 7279 7074 696f 6e5f 656e 6372 7970 7465  ryption_encrypte
+00000330: 6422 3a20 2243 7279 7074 c3a9 222c 0a0a  d": "Crypt..",..
+00000340: 2020 2020 2273 7461 7475 7362 6172 5f63      "statusbar_c
+00000350: 7572 736f 725f 6c61 6265 6c22 3a20 226c  ursor_label": "l
+00000360: 6967 6e65 203a 207b 6c69 6e65 7d20 e286  igne : {line} ..
+00000370: 9220 636f 6c20 3a20 7b63 6f6c 756d 6e7d  . col : {column}
+00000380: 222c 0a20 2020 2022 7374 6174 7573 6261  ",.    "statusba
+00000390: 725f 6375 7273 6f72 5f6c 6162 656c 5f73  r_cursor_label_s
+000003a0: 656c 6563 7465 6422 3a20 226c 6967 6e65  elected": "ligne
+000003b0: 203a 207b 6c69 6e65 7d20 e286 9220 636f   : {line} ... co
+000003c0: 6c20 3a20 7b63 6f6c 756d 6e7d 20e2 8692  l : {column} ...
+000003d0: 2073 656c 203a 207b 7365 6c65 6374 6564   sel : {selected
+000003e0: 7d22 2c0a 2020 2020 2273 7461 7475 7362  }",.    "statusb
+000003f0: 6172 5f63 7572 736f 725f 6c61 6265 6c5f  ar_cursor_label_
+00000400: 7769 7468 5f67 6c6f 6261 6c22 3a20 226c  with_global": "l
+00000410: 6967 6e65 203a 207b 6c69 6e65 7d20 e286  igne : {line} ..
+00000420: 9220 636f 6c20 3a20 7b63 6f6c 756d 6e7d  . col : {column}
+00000430: 20e2 8692 2070 6f73 203a 207b 706f 7369   ... pos : {posi
+00000440: 7469 6f6e 7d22 2c0a 2020 2020 2273 7461  tion}",.    "sta
+00000450: 7475 7362 6172 5f63 7572 736f 725f 6c61  tusbar_cursor_la
+00000460: 6265 6c5f 7365 6c65 6374 6564 5f77 6974  bel_selected_wit
+00000470: 685f 676c 6f62 616c 223a 0a20 2020 2020  h_global":.     
+00000480: 2020 2022 6c69 676e 6520 3a20 7b6c 696e     "ligne : {lin
+00000490: 657d 20e2 8692 2063 6f6c 203a 207b 636f  e} ... col : {co
+000004a0: 6c75 6d6e 7d20 e286 9220 706f 7320 3a20  lumn} ... pos : 
+000004b0: 7b70 6f73 6974 696f 6e7d 20e2 8692 2073  {position} ... s
+000004c0: 656c 203a 207b 7365 6c65 6374 6564 7d22  el : {selected}"
+000004d0: 2c0a 7d0a                                ,.}.
```

### Comparing `notolog-0.9.1b1/app/lexemes/fr/ai_assistant.py` & `notolog-0.9.1b2/notolog/lexemes/fr/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/fr/color_picker_dialog.py` & `notolog-0.9.1b2/notolog/lexemes/fr/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/fr/common.py` & `notolog-0.9.1b2/notolog/lexemes/fr/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     "save_active_file_error_occurred": "Impossible d'enregistrer le fichier, une erreur s'est produite",
 
     "expandable_block_default_title": "Plus d'infos...",
 
     "dialog_color_picker_color_copied_to_the_clipboard": "Le texte formaté a été copié dans le presse-papiers",
 
     "popup_about_title": "Infos de l'Application",
-    "popup_about_app_name_description": "Éditeur Markdown",
+    "popup_about_app_name_description": "Éditeur Markdown Python",
 
     "popup_about_version": "Version",
     "popup_about_license": "Licence",
     "popup_about_website": "Site Web",
     "popup_about_repository": "GitHub",
     "popup_about_pypi": "PyPi",
     "popup_about_date": "Date",
```

### Comparing `notolog-0.9.1b1/app/lexemes/fr/main_menu.py` & `notolog-0.9.1b2/notolog/lexemes/fr/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/fr/settings_dialog.py` & `notolog-0.9.1b2/notolog/lexemes/fr/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/fr/statusbar.py` & `notolog-0.9.1b2/notolog/lexemes/ja/statusbar.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-# French lexemes statusbar.py
+# Japanese lexemes statusbar.py
 lexemes = {
-    "statusbar_litter_bin_label": "Corbeille",
-    "statusbar_litter_bin_accessible_name": "Afficher le contenu de la corbeille",
+    "statusbar_litter_bin_label": "ごみ箱",
+    "statusbar_litter_bin_accessible_name": "ごみ箱の内容を表示",
 
     "statusbar_save_progress_label": b'\xf0\x9f\x92\xbe',
     "statusbar_encryption_symbol_encrypted_label": b'\xf0\x9f\x94\x92',
     "statusbar_encryption_symbol_unencrypted_label": b'\xf0\x9f\x94\x93',
 
-    "statusbar_mode_label_mode_view": "Mode Vue",
-    "statusbar_mode_label_mode_edit": "Mode Édition",
-    "statusbar_mode_label_mode_source": "Mode Source",
+    "statusbar_mode_label_mode_view": "ビューモード",
+    "statusbar_mode_label_mode_edit": "編集モード",
+    "statusbar_mode_label_mode_source": "ソースモード",
 
     "statusbar_source_label_source_markdown": "Markdown",
     "statusbar_source_label_source_html": "HTML",
 
     "statusbar_encryption_label": "{encryption} {icon}",
-    "statusbar_encryption_label_encryption_plain": "Clair",
-    "statusbar_encryption_label_encryption_encrypted": "Crypté",
+    "statusbar_encryption_label_encryption_plain": "プレーン",
+    "statusbar_encryption_label_encryption_encrypted": "暗号化",
 
-    "statusbar_cursor_label": "ligne : {line} → col : {column}",
-    "statusbar_cursor_label_selected": "ligne : {line} → col : {column} → sel : {selected}",
-    "statusbar_cursor_label_with_global": "ligne : {line} → col : {column} → pos : {position}",
-    "statusbar_cursor_label_selected_with_global":
-        "ligne : {line} → col : {column} → pos : {position} → sel : {selected}",
+    "statusbar_cursor_label": "行: {line} → 列: {column}",
+    "statusbar_cursor_label_selected": "行: {line} → 列: {column} → 選択: {selected}",
+    "statusbar_cursor_label_with_global": "行: {line} → 列: {column} → 位置: {position}",
+    "statusbar_cursor_label_selected_with_global": "行: {line} → 列: {column} → 位置: {position} → 選択: {selected}",
 }
```

### Comparing `notolog-0.9.1b1/app/lexemes/fr/toolbar.py` & `notolog-0.9.1b2/notolog/lexemes/fr/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/ge/__pycache__/settings_dialog.cpython-39.pyc` & `notolog-0.9.1b2/notolog/lexemes/ge/settings_dialog.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,357 +1,359 @@
-00000000: 610d 0d0a 0000 0000 42a9 3566 6e16 0000  a.......B.5fn...
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0030 0000 0040 0000 0073 6800 0000 6400  .0...@...sh...d.
-00000030: 6401 6402 6403 6404 6405 6406 6407 6408  d.d.d.d.d.d.d.d.
-00000040: 6409 640a 640b 640c 640d 640e 640f 6410  d.d.d.d.d.d.d.d.
-00000050: 6411 6412 6413 6414 6415 6416 6417 6418  d.d.d.d.d.d.d.d.
-00000060: 6419 641a 641b 641c 641d 641e 641f 6420  d.d.d.d.d.d.d.d 
-00000070: 6421 6422 6423 6424 6425 6426 6427 6428  d!d"d#d$d%d&d'd(
-00000080: 6429 642a 642b 642c 642d 642e 642f 9c2f  d)d*d+d,d-d.d/./
-00000090: 5a00 6430 5300 2931 7521 0000 00e1 839e  Z.d0S.)1u!......
-000000a0: e183 90e1 83a0 e183 90e1 839b e183 94e1  ................
-000000b0: 83a2 e183 a0e1 8394 e183 91e1 8398 7515  ..............u.
-000000c0: 0000 00e1 8393 e183 90e1 83ae e183 a3e1  ................
-000000d0: 83a0 e183 95e1 8390 7518 0000 00e1 83ab  ........u.......
-000000e0: e183 98e1 83a0 e183 98e1 8397 e183 90e1  ................
-000000f0: 8393 e183 9875 1b00 0000 e183 a0e1 8394  .....u..........
-00000100: e183 93e1 8390 e183 a5e1 83a2 e183 9de1  ................
-00000110: 83a0 e183 9875 1b00 0000 e183 93e1 8390  .....u..........
-00000120: e183 9be1 8399 e183 95e1 83a0 e183 94e1  ................
-00000130: 839a e183 9875 2700 0000 4149 20e1 8399  .....u'...AI ...
-00000140: e183 9de1 839c e183 a4e1 8398 e183 92e1  ................
-00000150: 83a3 e183 a0e1 8390 e183 aae1 8398 e183  ................
-00000160: 9075 4300 0000 e183 90e1 839e e183 9ae1  .uC.............
-00000170: 8398 e183 99e1 8390 e183 aae1 8398 e183  ................
-00000180: 98e1 83a1 20e1 8399 e183 9de1 839c e183  .... ...........
-00000190: a4e1 8398 e183 92e1 83a3 e183 a0e1 8390  ................
-000001a0: e183 aae1 8398 e183 9075 0900 0000 e183  .........u......
-000001b0: 94e1 839c e183 9075 1f00 0000 e183 90e1  .......u........
-000001c0: 8398 e183 a0e1 83a9 e183 98e1 8394 e183  ................
-000001d0: 9720 e183 94e1 839c e183 9075 4a00 0000  . .........uJ...
-000001e0: e183 90e1 839e e183 9ae1 8398 e183 99e1  ................
-000001f0: 8390 e183 aae1 8398 e183 98e1 83a1 20e1  .............. .
-00000200: 8398 e183 9ce1 83a2 e183 94e1 83a0 e183  ................
-00000210: a4e1 8394 e183 98e1 83a1 e183 98e1 83a1  ................
-00000220: 20e1 8394 e183 9ce1 8390 750c 0000 00e1   .........u.....
-00000230: 8397 e183 94e1 839b e183 9075 2200 0000  ...........u"...
-00000240: e183 90e1 8398 e183 a0e1 83a9 e183 98e1  ................
-00000250: 8394 e183 9720 e183 97e1 8394 e183 9be1  ..... ..........
-00000260: 8390 754d 0000 00e1 8390 e183 9ee1 839a  ..uM............
-00000270: e183 98e1 8399 e183 90e1 83aa e183 98e1  ................
-00000280: 8398 e183 a120 e183 98e1 839c e183 a2e1  ..... ..........
-00000290: 8394 e183 a0e1 83a4 e183 94e1 8398 e183  ................
-000002a0: a1e1 8398 e183 a120 e183 97e1 8394 e183  ....... ........
-000002b0: 9be1 8390 7525 0000 00e1 839b e183 97e1  ....u%..........
-000002c0: 8390 e183 95e1 8390 e183 a0e1 8398 20e1  .............. .
-000002d0: 839b e183 94e1 839c e183 98e1 83a3 753e  ..............u>
-000002e0: 0000 00e1 839b e183 97e1 8390 e183 95e1  ................
-000002f0: 8390 e183 a0e1 8398 20e1 839b e183 94e1  ........ .......
-00000300: 839c e183 98e1 83a3 e183 a120 e183 a9e1  ........... ....
-00000310: 8395 e183 94e1 839c e183 94e1 8391 e183  ................
-00000320: 9075 7600 0000 e183 90e1 83a9 e183 95e1  .uv.............
-00000330: 8394 e183 9ce1 8394 e183 9720 e183 90e1  ........... ....
-00000340: 839e e183 9ae1 8398 e183 99e1 8390 e183  ................
-00000350: aae1 8398 e183 98e1 83a1 20e1 839b e183  .......... .....
-00000360: 97e1 8390 e183 95e1 8390 e183 a0e1 8398  ................
-00000370: 20e1 83a9 e183 90e1 839b e183 9de1 83a8   ...............
-00000380: e183 9ae1 8398 e183 9ae1 8398 20e1 839b  ............ ...
-00000390: e183 94e1 839c e183 98e1 83a3 752c 0000  ............u,..
-000003a0: 00e1 83a8 e183 a0e1 8398 e183 a4e1 83a2  ................
-000003b0: e183 98e1 83a1 20e1 8396 e183 9de1 839b  ...... .........
-000003c0: e183 903a 207b 7369 7a65 7d70 7475 6000  ...: {size}ptu`.
-000003d0: 0000 e183 a8e1 83a0 e183 98e1 83a4 e183  ................
-000003e0: a2e1 8398 e183 a120 e183 92e1 839a e183  ....... ........
-000003f0: 9de1 8391 e183 90e1 839a e183 a3e1 83a0  ................
-00000400: e183 9820 e183 96e1 839d e183 9be1 8398  ... ............
-00000410: e183 a120 e183 a0e1 8394 e183 92e1 83a3  ... ............
-00000420: e183 9ae1 8398 e183 a0e1 8394 e183 91e1  ................
-00000430: 8390 7525 0000 00e1 83a1 e183 a2e1 8390  ..u%............
-00000440: e183 a2e1 83a3 e183 a1e1 8398 e183 a120  ............... 
-00000450: e183 96e1 839d e183 9ae1 8398 755d 0000  ............u]..
-00000460: 00e1 839b e183 a1e1 839d e183 a4e1 839a  ................
-00000470: e183 98e1 839d 20e1 8399 e183 a3e1 83a0  ...... .........
-00000480: e183 a1e1 839d e183 a0e1 8398 e183 a120  ............... 
-00000490: e183 9ee1 839d e183 96e1 8398 e183 aae1  ................
-000004a0: 8398 e183 98e1 83a1 20e1 83a9 e183 95e1  ........ .......
-000004b0: 8394 e183 9ce1 8394 e183 91e1 8390 7583  ..............u.
-000004c0: 0000 00e1 8390 e183 a9e1 8395 e183 94e1  ................
-000004d0: 839c e183 94e1 8397 20e1 8399 e183 a3e1  ........ .......
-000004e0: 83a0 e183 a1e1 839d e183 a0e1 8398 e183  ................
-000004f0: a120 e183 9be1 83a1 e183 9de1 83a4 e183  . ..............
-00000500: 9ae1 8398 e183 9d20 e183 9ee1 839d e183  ....... ........
-00000510: 96e1 8398 e183 aae1 8398 e183 9020 e183  ............. ..
-00000520: a1e1 83a2 e183 90e1 83a2 e183 a3e1 83a1  ................
-00000530: e183 98e1 83a1 20e1 8396 e183 9de1 839a  ...... .........
-00000540: e183 a8e1 8398 7543 0000 00e1 83a0 e183  ......uC........
-00000550: 94e1 8393 e183 90e1 83a5 e183 a2e1 839d  ................
-00000560: e183 a0e1 8398 e183 a120 e183 99e1 839d  ......... ......
-00000570: e183 9ce1 83a4 e183 98e1 8392 e183 a3e1  ................
-00000580: 83a0 e183 90e1 83aa e183 98e1 8390 7544  ..............uD
-00000590: 0000 00e1 83ae e183 90e1 8396 e183 94e1  ................
-000005a0: 8391 e183 98e1 83a1 20e1 839c e183 9de1  ........ .......
-000005b0: 839b e183 a0e1 8394 e183 91e1 8398 e183  ................
-000005c0: a120 e183 a9e1 8395 e183 94e1 839c e183  . ..............
-000005d0: 94e1 8391 e183 9075 6300 0000 e183 aee1  .......uc.......
-000005e0: 8390 e183 96e1 8394 e183 91e1 8398 e183  ................
-000005f0: a120 e183 9ce1 839d e183 9be1 83a0 e183  . ..............
-00000600: 94e1 8391 e183 98e1 83a1 20e1 83a9 e183  .......... .....
-00000610: 95e1 8394 e183 9ce1 8394 e183 91e1 8390  ................
-00000620: 20e1 83a0 e183 94e1 8393 e183 90e1 83a5   ...............
-00000630: e183 a2e1 839d e183 a0e1 83a8 e183 9875  ...............u
-00000640: 4300 0000 e183 93e1 8390 e183 9be1 8399  C...............
-00000650: e183 95e1 83a0 e183 94e1 839a e183 98e1  ................
-00000660: 83a1 20e1 8399 e183 9de1 839c e183 a4e1  .. .............
-00000670: 8398 e183 92e1 83a3 e183 a0e1 8390 e183  ................
-00000680: aae1 8398 e183 9075 6600 0000 e183 a2e1  .......uf.......
-00000690: 8394 e183 a5e1 83a1 e183 a2e1 83a3 e183  ................
-000006a0: a0e1 8398 20e1 8394 e183 9be1 839d e183  .... ...........
-000006b0: afe1 8398 e183 a120 e183 92e1 83a0 e183  ....... ........
-000006c0: 90e1 83a4 e183 98e1 8399 e183 a3e1 839a  ................
-000006d0: e183 90e1 8393 20e1 8392 e183 90e1 83a0  ...... .........
-000006e0: e183 93e1 8390 e183 a5e1 839b e183 9ce1  ................
-000006f0: 8390 7569 0000 00e1 83a2 e183 94e1 83a5  ..ui............
-00000700: e183 a1e1 83a2 e183 a3e1 83a0 e183 9820  ............... 
-00000710: e183 94e1 839b e183 9de1 83af e183 94e1  ................
-00000720: 8391 e183 98e1 83a1 20e1 8392 e183 a0e1  ........ .......
-00000730: 8390 e183 a4e1 8398 e183 99e1 83a3 e183  ................
-00000740: 9ae1 8398 20e1 83ac e183 90e1 83a0 e183  .... ...........
-00000750: 9be1 839d e183 a9e1 8394 e183 9ce1 8390  ................
-00000760: 752a 0000 0054 4f44 4f2d e183 94e1 8391  u*...TODO-......
-00000770: e183 98e1 83a1 20e1 8392 e183 90e1 839b  ...... .........
-00000780: e183 9de1 83a7 e183 9de1 83a4 e183 9075  ...............u
-00000790: 4900 0000 544f 444f 20e1 83a2 e183 94e1  I...TODO .......
-000007a0: 8392 e183 94e1 8391 e183 98e1 83a1 20e1  .............. .
-000007b0: 8392 e183 90e1 839b e183 9de1 83a7 e183  ................
-000007c0: 9de1 83a4 e183 9020 e183 a2e1 8394 e183  ....... ........
-000007d0: a5e1 83a1 e183 a2e1 83a8 e183 9875 4400  .............uD.
-000007e0: 0000 e183 91e1 839b e183 a3e1 839a e183  ................
-000007f0: 94e1 8391 e183 98e1 83a1 20e1 8392 e183  .......... .....
-00000800: 90e1 83ae e183 a1e1 839c e183 98e1 83a1  ................
-00000810: 20e1 8393 e183 90e1 83a1 e183 a2e1 83a3   ...............
-00000820: e183 a0e1 8398 7566 0000 00e1 8391 e183  ......uf........
-00000830: 9be1 83a3 e183 9ae1 8394 e183 91e1 8398  ................
-00000840: e183 a120 e183 92e1 8390 e183 aee1 83a1  ... ............
-00000850: e183 9ce1 8398 e183 a1e1 8390 e183 a120  ............... 
-00000860: e183 93e1 8390 e183 a1e1 83a2 e183 a3e1  ................
-00000870: 83a0 e183 98e1 83a1 20e1 839b e183 9de1  ........ .......
-00000880: 8397 e183 aee1 839d e183 95e1 839c e183  ................
-00000890: 9075 7000 0000 e183 92e1 8390 e183 a0e1  .up.............
-000008a0: 8394 20e1 83a1 e183 a3e1 83a0 e183 90e1  .. .............
-000008b0: 8397 e183 94e1 8391 e183 98e1 83a1 20e1  .............. .
-000008c0: 8390 e183 95e1 83a2 e183 9de1 839b e183  ................
-000008d0: 90e1 83a2 e183 a3e1 83a0 e183 9820 e183  ............. ..
-000008e0: a8e1 8394 e183 9ce1 8390 e183 aee1 8395  ................
-000008f0: e183 9020 e183 93e1 8398 e183 a1e1 8399  ... ............
-00000900: e183 96e1 8394 75bf 0000 00e1 8392 e183  ......u.........
-00000910: 90e1 83a0 e183 9420 e183 a1e1 83a3 e183  ....... ........
-00000920: a0e1 8390 e183 97e1 8394 e183 91e1 8398  ................
-00000930: e183 a120 e183 90e1 83a1 e183 9ae1 8394  ... ............
-00000940: e183 91e1 8398 e183 a120 e183 90e1 8395  ......... ......
-00000950: e183 a2e1 839d e183 9be1 8390 e183 a2e1  ................
-00000960: 83a3 e183 a0e1 8390 e183 9320 e183 a8e1  ........... ....
-00000970: 8394 e183 9ce1 8390 e183 aee1 8395 e183  ................
-00000980: 9020 e183 93e1 8398 e183 a1e1 8399 e183  . ..............
-00000990: 96e1 8394 20e1 839d e183 a4e1 839a e183  .... ...........
-000009a0: 90e1 8398 e183 9c20 e183 ace1 8395 e183  ....... ........
-000009b0: 93e1 839d e183 9be1 8398 e183 a1e1 8397  ................
-000009c0: e183 95e1 8398 e183 a12e 7a0a 4f70 656e  ..........z.Open
-000009d0: 4149 2041 5049 7a07 4150 4920 5552 4c7a  AI APIz.API URLz
-000009e0: 0e4f 7065 6e41 4920 4150 4920 5552 4c75  .OpenAI API URLu
-000009f0: 1c00 0000 4150 4920 e183 92e1 8390 e183  ....API ........
-00000a00: a1e1 8390 e183 a6e1 8394 e183 91e1 8398  ................
-00000a10: 7523 0000 004f 7065 6e41 4920 4150 4920  u#...OpenAI API 
-00000a20: e183 92e1 8390 e183 a1e1 8390 e183 a6e1  ................
-00000a30: 8394 e183 91e1 8398 753d 0000 00e1 839b  ........u=......
-00000a40: e183 aee1 8390 e183 a0e1 8393 e183 90e1  ................
-00000a50: 83ad e183 94e1 83a0 e183 98e1 839a e183  ................
-00000a60: 9820 e183 9be1 839d e183 93e1 8394 e183  . ..............
-00000a70: 9ae1 8394 e183 91e1 8398 7528 0000 00e1  ..........u(....
-00000a80: 839b e183 9de1 8393 e183 94e1 839a e183  ................
-00000a90: 98e1 83a1 20e1 8390 e183 a0e1 83a9 e183  .... ...........
-00000aa0: 94e1 8395 e183 9075 5300 0000 e183 9be1  .......uS.......
-00000ab0: 83ae e183 90e1 83a0 e183 93e1 8390 e183  ................
-00000ac0: ade1 8394 e183 a0e1 8398 e183 9ae1 8398  ................
-00000ad0: 20e1 839b e183 9de1 8393 e183 94e1 839a   ...............
-00000ae0: e183 94e1 8391 e183 98e1 83a1 20e1 8390  ............ ...
-00000af0: e183 a0e1 83a9 e183 94e1 8395 e183 9075  ...............u
-00000b00: 3400 0000 e183 a1e1 8390 e183 91e1 8390  4...............
-00000b10: e183 96e1 839d 20e1 839e e183 90e1 83a0  ...... .........
-00000b20: e183 90e1 839b e183 94e1 83a2 e183 a0e1  ................
-00000b30: 8394 e183 91e1 8398 7531 0000 00e1 83a1  ........u1......
-00000b40: e183 98e1 83a1 e183 a2e1 8394 e183 9be1  ................
-00000b50: 83a3 e183 a0e1 8398 20e1 839e e183 a0e1  ........ .......
-00000b60: 839d e183 9be1 839e e183 a2e1 8398 75b0  ..............u.
-00000b70: 0000 00e1 83a1 e183 90e1 8391 e183 90e1  ................
-00000b80: 8396 e183 9d20 e183 a1e1 8398 e183 a1e1  ..... ..........
-00000b90: 83a2 e183 94e1 839b e183 a3e1 83a0 e183  ................
-00000ba0: 9820 e183 9ee1 83a0 e183 9de1 839b e183  . ..............
-00000bb0: 9ee1 83a2 e183 982c 20e1 83a0 e183 9de1  ......., .......
-00000bc0: 839b e183 94e1 839a e183 98e1 83aa 20e1  .............. .
-00000bd0: 83a7 e183 9de1 8395 e183 94e1 839a 20e1  .............. .
-00000be0: 839b e183 9de1 8397 e183 aee1 839d e183  ................
-00000bf0: 95e1 839c e183 90e1 83a1 20e1 83ac e183  .......... .....
-00000c00: 98e1 839c e183 90e1 83a1 e183 ace1 8390  ................
-00000c10: e183 a020 e183 9be1 8398 e183 93e1 8398  ... ............
-00000c20: e183 a175 cf00 0000 e183 a1e1 8390 e183  ...u............
-00000c30: 91e1 8390 e183 96e1 839d 20e1 83a1 e183  .......... .....
-00000c40: 98e1 83a1 e183 a2e1 8394 e183 9be1 83a3  ................
-00000c50: e183 a0e1 8398 20e1 839e e183 a0e1 839d  ...... .........
-00000c60: e183 9be1 839e e183 a2e1 8398 2c20 e183  ............, ..
-00000c70: a0e1 839d e183 9be1 8394 e183 9ae1 8398  ................
-00000c80: e183 aa20 e183 a7e1 839d e183 95e1 8394  ... ............
-00000c90: e183 9a20 e183 9be1 839d e183 97e1 83ae  ... ............
-00000ca0: e183 9de1 8395 e183 9ce1 8390 e183 a120  ............... 
-00000cb0: e183 ace1 8398 e183 9ce1 8390 e183 a1e1  ................
-00000cc0: 83ac e183 90e1 83a0 20e1 839b e183 98e1  ........ .......
-00000cd0: 8393 e183 98e1 83a1 2e20 e183 94e1 83a1  ......... ......
-00000ce0: 20e1 83a2 e183 94e1 83a5 e183 a1e1 83a2   ...............
-00000cf0: e183 98e1 8390 2e75 5000 0000 e183 9ee1  .......uP.......
-00000d00: 8390 e183 a1e1 83a3 e183 aee1 8398 e183  ................
-00000d10: a120 e183 9be1 8390 e183 a5e1 83a1 e183  . ..............
-00000d20: 98e1 839b e183 90e1 839a e183 a3e1 83a0  ................
-00000d30: e183 9820 e183 a2e1 839d e183 99e1 8394  ... ............
-00000d40: e183 9ce1 8394 e183 91e1 8398 7588 0000  ............u...
-00000d50: 00e1 839e e183 90e1 83a1 e183 a3e1 83ae  ................
-00000d60: e183 a8e1 8398 20e1 839b e183 98e1 83a1  ...... .........
-00000d70: e183 90e1 83a6 e183 94e1 8391 e183 9820  ............... 
-00000d80: e183 a2e1 839d e183 99e1 8394 e183 9ce1  ................
-00000d90: 8394 e183 91e1 8398 e183 a120 e183 9be1  ........... ....
-00000da0: 8390 e183 a5e1 83a1 e183 98e1 839b e183  ................
-00000db0: 90e1 839a e183 a3e1 83a0 e183 9820 e183  ............. ..
-00000dc0: a0e1 8390 e183 9de1 8393 e183 94e1 839c  ................
-00000dd0: e183 9de1 8391 e183 9029 2fda 0c77 696e  .........)/..win
-00000de0: 646f 775f 7469 746c 65da 0c62 7574 746f  dow_title..butto
-00000df0: 6e5f 636c 6f73 65da 0b74 6162 5f67 656e  n_close..tab_gen
-00000e00: 6572 616c da11 7461 625f 6564 6974 6f72  eral..tab_editor
-00000e10: 5f63 6f6e 6669 67da 1174 6162 5f76 6965  _config..tab_vie
-00000e20: 7765 725f 636f 6e66 6967 da0d 7461 625f  wer_config..tab_
-00000e30: 6169 5f63 6f6e 6669 67da 1867 656e 6572  ai_config..gener
-00000e40: 616c 5f61 7070 5f63 6f6e 6669 675f 6c61  al_app_config_la
-00000e50: 6265 6cda 1a67 656e 6572 616c 5f61 7070  bel..general_app
-00000e60: 5f6c 616e 6775 6167 655f 6c61 6265 6cda  _language_label.
-00000e70: 2b67 656e 6572 616c 5f61 7070 5f6c 616e  +general_app_lan
-00000e80: 6775 6167 655f 636f 6d62 6f5f 706c 6163  guage_combo_plac
-00000e90: 6568 6f6c 6465 725f 7465 7874 da31 6765  eholder_text.1ge
-00000ea0: 6e65 7261 6c5f 6170 705f 6c61 6e67 7561  neral_app_langua
-00000eb0: 6765 5f63 6f6d 626f 5f61 6363 6573 7369  ge_combo_accessi
-00000ec0: 626c 655f 6465 7363 7269 7074 696f 6eda  ble_description.
-00000ed0: 1767 656e 6572 616c 5f61 7070 5f74 6865  .general_app_the
-00000ee0: 6d65 5f6c 6162 656c da28 6765 6e65 7261  me_label.(genera
-00000ef0: 6c5f 6170 705f 7468 656d 655f 636f 6d62  l_app_theme_comb
-00000f00: 6f5f 706c 6163 6568 6f6c 6465 725f 7465  o_placeholder_te
-00000f10: 7874 da2e 6765 6e65 7261 6c5f 6170 705f  xt..general_app_
-00000f20: 7468 656d 655f 636f 6d62 6f5f 6163 6365  theme_combo_acce
-00000f30: 7373 6962 6c65 5f64 6573 6372 6970 7469  ssible_descripti
-00000f40: 6f6e da1b 6765 6e65 7261 6c5f 6170 705f  on..general_app_
-00000f50: 6d61 696e 5f6d 656e 755f 6c61 6265 6cda  main_menu_label.
-00000f60: 1e67 656e 6572 616c 5f61 7070 5f6d 6169  .general_app_mai
-00000f70: 6e5f 6d65 6e75 5f63 6865 636b 626f 78da  n_menu_checkbox.
-00000f80: 3567 656e 6572 616c 5f61 7070 5f6d 6169  5general_app_mai
-00000f90: 6e5f 6d65 6e75 5f63 6865 636b 626f 785f  n_menu_checkbox_
-00000fa0: 6163 6365 7373 6962 6c65 5f64 6573 6372  accessible_descr
-00000fb0: 6970 7469 6f6e da1b 6765 6e65 7261 6c5f  iption..general_
-00000fc0: 6170 705f 666f 6e74 5f73 697a 655f 6c61  app_font_size_la
-00000fd0: 6265 6cda 3367 656e 6572 616c 5f61 7070  bel.3general_app
-00000fe0: 5f66 6f6e 745f 7369 7a65 5f73 6c69 6465  _font_size_slide
-00000ff0: 725f 6163 6365 7373 6962 6c65 5f64 6573  r_accessible_des
-00001000: 6372 6970 7469 6f6e da17 6765 6e65 7261  cription..genera
-00001010: 6c5f 7374 6174 7573 6261 725f 6c61 6265  l_statusbar_labe
-00001020: 6cda 3667 656e 6572 616c 5f73 7461 7475  l.6general_statu
-00001030: 7362 6172 5f73 686f 775f 676c 6f62 616c  sbar_show_global
-00001040: 5f63 7572 736f 725f 706f 7369 7469 6f6e  _cursor_position
-00001050: 5f63 6865 636b 626f 78da 4d67 656e 6572  _checkbox.Mgener
-00001060: 616c 5f73 7461 7475 7362 6172 5f73 686f  al_statusbar_sho
-00001070: 775f 676c 6f62 616c 5f63 7572 736f 725f  w_global_cursor_
-00001080: 706f 7369 7469 6f6e 5f63 6865 636b 626f  position_checkbo
-00001090: 785f 6163 6365 7373 6962 6c65 5f64 6573  x_accessible_des
-000010a0: 6372 6970 7469 6f6e da13 6564 6974 6f72  cription..editor
-000010b0: 5f63 6f6e 6669 675f 6c61 6265 6cda 2865  _config_label.(e
-000010c0: 6469 746f 725f 636f 6e66 6967 5f73 686f  ditor_config_sho
-000010d0: 775f 6c69 6e65 5f6e 756d 6265 7273 5f63  w_line_numbers_c
-000010e0: 6865 636b 626f 78da 3f65 6469 746f 725f  heckbox.?editor_
-000010f0: 636f 6e66 6967 5f73 686f 775f 6c69 6e65  config_show_line
-00001100: 5f6e 756d 6265 7273 5f63 6865 636b 626f  _numbers_checkbo
-00001110: 785f 6163 6365 7373 6962 6c65 5f64 6573  x_accessible_des
-00001120: 6372 6970 7469 6f6e da13 7669 6577 6572  cription..viewer
-00001130: 5f63 6f6e 6669 675f 6c61 6265 6cda 2576  _config_label.%v
-00001140: 6965 7765 725f 636f 6e66 6967 5f70 726f  iewer_config_pro
-00001150: 6365 7373 5f65 6d6f 6a69 735f 6368 6563  cess_emojis_chec
-00001160: 6b62 6f78 da3c 7669 6577 6572 5f63 6f6e  kbox.<viewer_con
-00001170: 6669 675f 7072 6f63 6573 735f 656d 6f6a  fig_process_emoj
-00001180: 6973 5f63 6865 636b 626f 785f 6163 6365  is_checkbox_acce
-00001190: 7373 6962 6c65 5f64 6573 6372 6970 7469  ssible_descripti
-000011a0: 6f6e da26 7669 6577 6572 5f63 6f6e 6669  on.&viewer_confi
-000011b0: 675f 6869 6768 6c69 6768 745f 746f 646f  g_highlight_todo
-000011c0: 735f 6368 6563 6b62 6f78 da3d 7669 6577  s_checkbox.=view
-000011d0: 6572 5f63 6f6e 6669 675f 6869 6768 6c69  er_config_highli
-000011e0: 6768 745f 746f 646f 735f 6368 6563 6b62  ght_todos_checkb
-000011f0: 6f78 5f61 6363 6573 7369 626c 655f 6465  ox_accessible_de
-00001200: 7363 7269 7074 696f 6eda 2d76 6965 7765  scription.-viewe
-00001210: 725f 636f 6e66 6967 5f6f 7065 6e5f 6c69  r_config_open_li
-00001220: 6e6b 5f63 6f6e 6669 726d 6174 696f 6e5f  nk_confirmation_
-00001230: 6368 6563 6b62 6f78 da44 7669 6577 6572  checkbox.Dviewer
-00001240: 5f63 6f6e 6669 675f 6f70 656e 5f6c 696e  _config_open_lin
-00001250: 6b5f 636f 6e66 6972 6d61 7469 6f6e 5f63  k_confirmation_c
-00001260: 6865 636b 626f 785f 6163 6365 7373 6962  heckbox_accessib
-00001270: 6c65 5f64 6573 6372 6970 7469 6f6e da25  le_description.%
-00001280: 7669 6577 6572 5f63 6f6e 6669 675f 7361  viewer_config_sa
-00001290: 7665 5f72 6573 6f75 7263 6573 5f63 6865  ve_resources_che
-000012a0: 636b 626f 78da 3c76 6965 7765 725f 636f  ckbox.<viewer_co
-000012b0: 6e66 6967 5f73 6176 655f 7265 736f 7572  nfig_save_resour
-000012c0: 6365 735f 6368 6563 6b62 6f78 5f61 6363  ces_checkbox_acc
-000012d0: 6573 7369 626c 655f 6465 7363 7269 7074  essible_descript
-000012e0: 696f 6eda 1a61 695f 636f 6e66 6967 5f6f  ion..ai_config_o
-000012f0: 7065 6e61 695f 6170 695f 6c61 6265 6cda  penai_api_label.
-00001300: 2f61 695f 636f 6e66 6967 5f6f 7065 6e61  /ai_config_opena
-00001310: 695f 6170 695f 7572 6c5f 696e 7075 745f  i_api_url_input_
-00001320: 706c 6163 6568 6f6c 6465 725f 7465 7874  placeholder_text
-00001330: da35 6169 5f63 6f6e 6669 675f 6f70 656e  .5ai_config_open
-00001340: 6169 5f61 7069 5f75 726c 5f69 6e70 7574  ai_api_url_input
-00001350: 5f61 6363 6573 7369 626c 655f 6465 7363  _accessible_desc
-00001360: 7269 7074 696f 6eda 2f61 695f 636f 6e66  ription./ai_conf
-00001370: 6967 5f6f 7065 6e61 695f 6170 695f 6b65  ig_openai_api_ke
-00001380: 795f 696e 7075 745f 706c 6163 6568 6f6c  y_input_placehol
-00001390: 6465 725f 7465 7874 da35 6169 5f63 6f6e  der_text.5ai_con
-000013a0: 6669 675f 6f70 656e 6169 5f61 7069 5f6b  fig_openai_api_k
-000013b0: 6579 5f69 6e70 7574 5f61 6363 6573 7369  ey_input_accessi
-000013c0: 626c 655f 6465 7363 7269 7074 696f 6eda  ble_description.
-000013d0: 2b61 695f 636f 6e66 6967 5f6f 7065 6e61  +ai_config_opena
-000013e0: 695f 6170 695f 7375 7070 6f72 7465 645f  i_api_supported_
-000013f0: 6d6f 6465 6c73 5f6c 6162 656c da2f 6169  models_label./ai
-00001400: 5f63 6f6e 6669 675f 6169 5f6d 6f64 656c  _config_ai_model
-00001410: 5f6e 616d 6573 5f63 6f6d 626f 5f70 6c61  _names_combo_pla
-00001420: 6365 686f 6c64 6572 5f74 6578 74da 3561  ceholder_text.5a
-00001430: 695f 636f 6e66 6967 5f61 695f 6d6f 6465  i_config_ai_mode
-00001440: 6c5f 6e61 6d65 735f 636f 6d62 6f5f 6163  l_names_combo_ac
-00001450: 6365 7373 6962 6c65 5f64 6573 6372 6970  cessible_descrip
-00001460: 7469 6f6e da14 6169 5f63 6f6e 6669 675f  tion..ai_config_
-00001470: 6261 7365 5f6c 6162 656c da22 6169 5f63  base_label."ai_c
-00001480: 6f6e 6669 675f 6261 7365 5f73 7973 7465  onfig_base_syste
-00001490: 6d5f 7072 6f6d 7074 5f6c 6162 656c da32  m_prompt_label.2
-000014a0: 6169 5f63 6f6e 6669 675f 6261 7365 5f73  ai_config_base_s
-000014b0: 7973 7465 6d5f 7072 6f6d 7074 5f65 6469  ystem_prompt_edi
-000014c0: 745f 706c 6163 6568 6f6c 6465 725f 7465  t_placeholder_te
-000014d0: 7874 da38 6169 5f63 6f6e 6669 675f 6261  xt.8ai_config_ba
-000014e0: 7365 5f73 7973 7465 6d5f 7072 6f6d 7074  se_system_prompt
-000014f0: 5f65 6469 745f 6163 6365 7373 6962 6c65  _edit_accessible
-00001500: 5f64 6573 6372 6970 7469 6f6e da28 6169  _description.(ai
-00001510: 5f63 6f6e 6669 675f 6261 7365 5f72 6573  _config_base_res
-00001520: 706f 6e73 655f 6d61 785f 746f 6b65 6e73  ponse_max_tokens
-00001530: 5f6c 6162 656c da3f 6169 5f63 6f6e 6669  _label.?ai_confi
-00001540: 675f 6261 7365 5f72 6573 706f 6e73 655f  g_base_response_
-00001550: 6d61 785f 746f 6b65 6e73 5f69 6e70 7574  max_tokens_input
-00001560: 5f61 6363 6573 7369 626c 655f 6465 7363  _accessible_desc
-00001570: 7269 7074 696f 6e4e 2901 da07 6c65 7865  riptionN)...lexe
-00001580: 6d65 73a9 0072 3100 0000 7231 0000 00fa  mes..r1...r1....
-00001590: 4c2f 5573 6572 732f 7661 6469 6b75 732f  L/Users/vadikus/
-000015a0: 5079 6368 6172 6d50 726f 6a65 6374 732f  PycharmProjects/
-000015b0: 6e6f 746f 6c6f 672d 6465 762f 6170 702f  notolog-dev/app/
-000015c0: 6c65 7865 6d65 732f 6765 2f73 6574 7469  lexemes/ge/setti
-000015d0: 6e67 735f 6469 616c 6f67 2e70 79da 083c  ngs_dialog.py..<
-000015e0: 6d6f 6475 6c65 3e04 0000 0073 5e00 0000  module>....s^...
-000015f0: 0202 0202 0201 0201 0201 0202 0201 0201  ................
-00001600: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00001610: 0201 0202 0201 0202 0202 0201 0201 0202  ................
-00001620: 0201 0201 0201 0201 0201 0202 0201 0202  ................
-00001630: 0202 0201 0201 0201 0201 0201 0201 0201  ................
-00001640: 0202 0201 0201 0202 0201 0201 02c4       ..............
+00000000: 2320 4765 6f72 6769 616e 206c 6578 656d  # Georgian lexem
+00000010: 6573 2073 6574 7469 6e67 735f 6469 616c  es settings_dial
+00000020: 6f67 2e70 790a 6c65 7865 6d65 7320 3d20  og.py.lexemes = 
+00000030: 7b0a 2020 2020 2320 e183 9ee1 8390 e183  {.    # ........
+00000040: a0e1 8390 e183 9be1 8394 e183 a2e1 83a0  ................
+00000050: e183 94e1 8391 e183 98e1 83a1 20e1 8393  ............ ...
+00000060: e183 98e1 8390 e183 9ae1 839d e183 92e1  ................
+00000070: 8398 0a20 2020 2022 7769 6e64 6f77 5f74  ...    "window_t
+00000080: 6974 6c65 223a 2022 e183 9ee1 8390 e183  itle": "........
+00000090: a0e1 8390 e183 9be1 8394 e183 a2e1 83a0  ................
+000000a0: e183 94e1 8391 e183 9822 2c0a 0a20 2020  .........",..   
+000000b0: 2022 6275 7474 6f6e 5f63 6c6f 7365 223a   "button_close":
+000000c0: 2022 e183 93e1 8390 e183 aee1 83a3 e183   "..............
+000000d0: a0e1 8395 e183 9022 2c0a 0a20 2020 2022  .......",..    "
+000000e0: 7461 625f 6765 6e65 7261 6c22 3a20 22e1  tab_general": ".
+000000f0: 83ab e183 98e1 83a0 e183 98e1 8397 e183  ................
+00000100: 90e1 8393 e183 9822 2c0a 2020 2020 2274  .......",.    "t
+00000110: 6162 5f65 6469 746f 725f 636f 6e66 6967  ab_editor_config
+00000120: 223a 2022 e183 a0e1 8394 e183 93e1 8390  ": "............
+00000130: e183 a5e1 83a2 e183 9de1 83a0 e183 9822  ..............."
+00000140: 2c0a 2020 2020 2274 6162 5f76 6965 7765  ,.    "tab_viewe
+00000150: 725f 636f 6e66 6967 223a 2022 e183 93e1  r_config": "....
+00000160: 8390 e183 9be1 8399 e183 95e1 83a0 e183  ................
+00000170: 94e1 839a e183 9822 2c0a 2020 2020 2274  .......",.    "t
+00000180: 6162 5f61 695f 636f 6e66 6967 223a 2022  ab_ai_config": "
+00000190: 4149 20e1 8399 e183 9de1 839c e183 a4e1  AI .............
+000001a0: 8398 e183 92e1 83a3 e183 a0e1 8390 e183  ................
+000001b0: aae1 8398 e183 9022 2c0a 0a20 2020 2022  .......",..    "
+000001c0: 6765 6e65 7261 6c5f 6170 705f 636f 6e66  general_app_conf
+000001d0: 6967 5f6c 6162 656c 223a 2022 e183 90e1  ig_label": "....
+000001e0: 839e e183 9ae1 8398 e183 99e1 8390 e183  ................
+000001f0: aae1 8398 e183 98e1 83a1 20e1 8399 e183  .......... .....
+00000200: 9de1 839c e183 a4e1 8398 e183 92e1 83a3  ................
+00000210: e183 a0e1 8390 e183 aae1 8398 e183 9022  ..............."
+00000220: 2c0a 2020 2020 2267 656e 6572 616c 5f61  ,.    "general_a
+00000230: 7070 5f6c 616e 6775 6167 655f 6c61 6265  pp_language_labe
+00000240: 6c22 3a20 22e1 8394 e183 9ce1 8390 222c  l": ".........",
+00000250: 0a20 2020 2022 6765 6e65 7261 6c5f 6170  .    "general_ap
+00000260: 705f 6c61 6e67 7561 6765 5f63 6f6d 626f  p_language_combo
+00000270: 5f70 6c61 6365 686f 6c64 6572 5f74 6578  _placeholder_tex
+00000280: 7422 3a20 22e1 8390 e183 98e1 83a0 e183  t": "...........
+00000290: a9e1 8398 e183 94e1 8397 20e1 8394 e183  .......... .....
+000002a0: 9ce1 8390 222c 0a20 2020 2022 6765 6e65  ....",.    "gene
+000002b0: 7261 6c5f 6170 705f 6c61 6e67 7561 6765  ral_app_language
+000002c0: 5f63 6f6d 626f 5f61 6363 6573 7369 626c  _combo_accessibl
+000002d0: 655f 6465 7363 7269 7074 696f 6e22 3a20  e_description": 
+000002e0: 22e1 8390 e183 9ee1 839a e183 98e1 8399  "...............
+000002f0: e183 90e1 83aa e183 98e1 8398 e183 a120  ............... 
+00000300: e183 98e1 839c e183 a2e1 8394 e183 a0e1  ................
+00000310: 83a4 e183 94e1 8398 e183 a1e1 8398 e183  ................
+00000320: a120 e183 94e1 839c e183 9022 2c0a 2020  . .........",.  
+00000330: 2020 2267 656e 6572 616c 5f61 7070 5f74    "general_app_t
+00000340: 6865 6d65 5f6c 6162 656c 223a 2022 e183  heme_label": "..
+00000350: 97e1 8394 e183 9be1 8390 222c 0a20 2020  ..........",.   
+00000360: 2022 6765 6e65 7261 6c5f 6170 705f 7468   "general_app_th
+00000370: 656d 655f 636f 6d62 6f5f 706c 6163 6568  eme_combo_placeh
+00000380: 6f6c 6465 725f 7465 7874 223a 2022 e183  older_text": "..
+00000390: 90e1 8398 e183 a0e1 83a9 e183 98e1 8394  ................
+000003a0: e183 9720 e183 97e1 8394 e183 9be1 8390  ... ............
+000003b0: 222c 0a20 2020 2022 6765 6e65 7261 6c5f  ",.    "general_
+000003c0: 6170 705f 7468 656d 655f 636f 6d62 6f5f  app_theme_combo_
+000003d0: 6163 6365 7373 6962 6c65 5f64 6573 6372  accessible_descr
+000003e0: 6970 7469 6f6e 223a 2022 e183 90e1 839e  iption": "......
+000003f0: e183 9ae1 8398 e183 99e1 8390 e183 aae1  ................
+00000400: 8398 e183 98e1 83a1 20e1 8398 e183 9ce1  ........ .......
+00000410: 83a2 e183 94e1 83a0 e183 a4e1 8394 e183  ................
+00000420: 98e1 83a1 e183 98e1 83a1 20e1 8397 e183  .......... .....
+00000430: 94e1 839b e183 9022 2c0a 2020 2020 2267  .......",.    "g
+00000440: 656e 6572 616c 5f61 7070 5f6d 6169 6e5f  eneral_app_main_
+00000450: 6d65 6e75 5f6c 6162 656c 223a 2022 e183  menu_label": "..
+00000460: 9be1 8397 e183 90e1 8395 e183 90e1 83a0  ................
+00000470: e183 9820 e183 9be1 8394 e183 9ce1 8398  ... ............
+00000480: e183 a322 2c0a 2020 2020 2267 656e 6572  ...",.    "gener
+00000490: 616c 5f61 7070 5f6d 6169 6e5f 6d65 6e75  al_app_main_menu
+000004a0: 5f63 6865 636b 626f 7822 3a20 22e1 839b  _checkbox": "...
+000004b0: e183 97e1 8390 e183 95e1 8390 e183 a0e1  ................
+000004c0: 8398 20e1 839b e183 94e1 839c e183 98e1  .. .............
+000004d0: 83a3 e183 a120 e183 a9e1 8395 e183 94e1  ..... ..........
+000004e0: 839c e183 94e1 8391 e183 9022 2c0a 2020  ...........",.  
+000004f0: 2020 2267 656e 6572 616c 5f61 7070 5f6d    "general_app_m
+00000500: 6169 6e5f 6d65 6e75 5f63 6865 636b 626f  ain_menu_checkbo
+00000510: 785f 6163 6365 7373 6962 6c65 5f64 6573  x_accessible_des
+00000520: 6372 6970 7469 6f6e 223a 2022 e183 90e1  cription": "....
+00000530: 83a9 e183 95e1 8394 e183 9ce1 8394 e183  ................
+00000540: 9720 e183 90e1 839e e183 9ae1 8398 e183  . ..............
+00000550: 99e1 8390 e183 aae1 8398 e183 98e1 83a1  ................
+00000560: 20e1 839b e183 97e1 8390 e183 95e1 8390   ...............
+00000570: e183 a0e1 8398 20e1 83a9 e183 90e1 839b  ...... .........
+00000580: e183 9de1 83a8 e183 9ae1 8398 e183 9ae1  ................
+00000590: 8398 20e1 839b e183 94e1 839c e183 98e1  .. .............
+000005a0: 83a3 222c 0a20 2020 2022 6765 6e65 7261  ..",.    "genera
+000005b0: 6c5f 6170 705f 666f 6e74 5f73 697a 655f  l_app_font_size_
+000005c0: 6c61 6265 6c22 3a20 22e1 83a8 e183 a0e1  label": ".......
+000005d0: 8398 e183 a4e1 83a2 e183 98e1 83a1 20e1  .............. .
+000005e0: 8396 e183 9de1 839b e183 903a 207b 7369  ...........: {si
+000005f0: 7a65 7d70 7422 2c0a 2020 2020 2267 656e  ze}pt",.    "gen
+00000600: 6572 616c 5f61 7070 5f66 6f6e 745f 7369  eral_app_font_si
+00000610: 7a65 5f73 6c69 6465 725f 6163 6365 7373  ze_slider_access
+00000620: 6962 6c65 5f64 6573 6372 6970 7469 6f6e  ible_description
+00000630: 223a 2022 e183 a8e1 83a0 e183 98e1 83a4  ": "............
+00000640: e183 a2e1 8398 e183 a120 e183 92e1 839a  ......... ......
+00000650: e183 9de1 8391 e183 90e1 839a e183 a3e1  ................
+00000660: 83a0 e183 9820 e183 96e1 839d e183 9be1  ..... ..........
+00000670: 8398 e183 a120 e183 a0e1 8394 e183 92e1  ..... ..........
+00000680: 83a3 e183 9ae1 8398 e183 a0e1 8394 e183  ................
+00000690: 91e1 8390 222c 0a0a 2020 2020 2267 656e  ....",..    "gen
+000006a0: 6572 616c 5f73 7461 7475 7362 6172 5f6c  eral_statusbar_l
+000006b0: 6162 656c 223a 2022 e183 a1e1 83a2 e183  abel": "........
+000006c0: 90e1 83a2 e183 a3e1 83a1 e183 98e1 83a1  ................
+000006d0: 20e1 8396 e183 9de1 839a e183 9822 2c0a   ............",.
+000006e0: 2020 2020 2267 656e 6572 616c 5f73 7461      "general_sta
+000006f0: 7475 7362 6172 5f73 686f 775f 676c 6f62  tusbar_show_glob
+00000700: 616c 5f63 7572 736f 725f 706f 7369 7469  al_cursor_positi
+00000710: 6f6e 5f63 6865 636b 626f 7822 3a20 22e1  on_checkbox": ".
+00000720: 839b e183 a1e1 839d e183 a4e1 839a e183  ................
+00000730: 98e1 839d 20e1 8399 e183 a3e1 83a0 e183  .... ...........
+00000740: a1e1 839d e183 a0e1 8398 e183 a120 e183  ............. ..
+00000750: 9ee1 839d e183 96e1 8398 e183 aae1 8398  ................
+00000760: e183 98e1 83a1 20e1 83a9 e183 95e1 8394  ...... .........
+00000770: e183 9ce1 8394 e183 91e1 8390 222c 0a20  ............",. 
+00000780: 2020 2022 6765 6e65 7261 6c5f 7374 6174     "general_stat
+00000790: 7573 6261 725f 7368 6f77 5f67 6c6f 6261  usbar_show_globa
+000007a0: 6c5f 6375 7273 6f72 5f70 6f73 6974 696f  l_cursor_positio
+000007b0: 6e5f 6368 6563 6b62 6f78 5f61 6363 6573  n_checkbox_acces
+000007c0: 7369 626c 655f 6465 7363 7269 7074 696f  sible_descriptio
+000007d0: 6e22 3a0a 2020 2020 2020 2020 22e1 8390  n":.        "...
+000007e0: e183 a9e1 8395 e183 94e1 839c e183 94e1  ................
+000007f0: 8397 20e1 8399 e183 a3e1 83a0 e183 a1e1  .. .............
+00000800: 839d e183 a0e1 8398 e183 a120 e183 9be1  ........... ....
+00000810: 83a1 e183 9de1 83a4 e183 9ae1 8398 e183  ................
+00000820: 9d20 e183 9ee1 839d e183 96e1 8398 e183  . ..............
+00000830: aae1 8398 e183 9020 e183 a1e1 83a2 e183  ....... ........
+00000840: 90e1 83a2 e183 a3e1 83a1 e183 98e1 83a1  ................
+00000850: 20e1 8396 e183 9de1 839a e183 a8e1 8398   ...............
+00000860: 222c 0a0a 2020 2020 2265 6469 746f 725f  ",..    "editor_
+00000870: 636f 6e66 6967 5f6c 6162 656c 223a 2022  config_label": "
+00000880: e183 a0e1 8394 e183 93e1 8390 e183 a5e1  ................
+00000890: 83a2 e183 9de1 83a0 e183 98e1 83a1 20e1  .............. .
+000008a0: 8399 e183 9de1 839c e183 a4e1 8398 e183  ................
+000008b0: 92e1 83a3 e183 a0e1 8390 e183 aae1 8398  ................
+000008c0: e183 9022 2c0a 2020 2020 2265 6469 746f  ...",.    "edito
+000008d0: 725f 636f 6e66 6967 5f73 686f 775f 6c69  r_config_show_li
+000008e0: 6e65 5f6e 756d 6265 7273 5f63 6865 636b  ne_numbers_check
+000008f0: 626f 7822 3a20 22e1 83ae e183 90e1 8396  box": ".........
+00000900: e183 94e1 8391 e183 98e1 83a1 20e1 839c  ............ ...
+00000910: e183 9de1 839b e183 a0e1 8394 e183 91e1  ................
+00000920: 8398 e183 a120 e183 a9e1 8395 e183 94e1  ..... ..........
+00000930: 839c e183 94e1 8391 e183 9022 2c0a 2020  ...........",.  
+00000940: 2020 2265 6469 746f 725f 636f 6e66 6967    "editor_config
+00000950: 5f73 686f 775f 6c69 6e65 5f6e 756d 6265  _show_line_numbe
+00000960: 7273 5f63 6865 636b 626f 785f 6163 6365  rs_checkbox_acce
+00000970: 7373 6962 6c65 5f64 6573 6372 6970 7469  ssible_descripti
+00000980: 6f6e 223a 2022 e183 aee1 8390 e183 96e1  on": "..........
+00000990: 8394 e183 91e1 8398 e183 a120 e183 9ce1  ........... ....
+000009a0: 839d e183 9be1 83a0 e183 94e1 8391 e183  ................
+000009b0: 98e1 83a1 20e1 83a9 e183 95e1 8394 e183  .... ...........
+000009c0: 9ce1 8394 e183 91e1 8390 20e1 83a0 e183  .......... .....
+000009d0: 94e1 8393 e183 90e1 83a5 e183 a2e1 839d  ................
+000009e0: e183 a0e1 83a8 e183 9822 2c0a 0a20 2020  .........",..   
+000009f0: 2022 7669 6577 6572 5f63 6f6e 6669 675f   "viewer_config_
+00000a00: 6c61 6265 6c22 3a20 22e1 8393 e183 90e1  label": ".......
+00000a10: 839b e183 99e1 8395 e183 a0e1 8394 e183  ................
+00000a20: 9ae1 8398 e183 a120 e183 99e1 839d e183  ....... ........
+00000a30: 9ce1 83a4 e183 98e1 8392 e183 a3e1 83a0  ................
+00000a40: e183 90e1 83aa e183 98e1 8390 222c 0a20  ............",. 
+00000a50: 2020 2022 7669 6577 6572 5f63 6f6e 6669     "viewer_confi
+00000a60: 675f 7072 6f63 6573 735f 656d 6f6a 6973  g_process_emojis
+00000a70: 5f63 6865 636b 626f 7822 3a20 22e1 83a2  _checkbox": "...
+00000a80: e183 94e1 83a5 e183 a1e1 83a2 e183 a3e1  ................
+00000a90: 83a0 e183 9820 e183 94e1 839b e183 9de1  ..... ..........
+00000aa0: 83af e183 98e1 83a1 20e1 8392 e183 a0e1  ........ .......
+00000ab0: 8390 e183 a4e1 8398 e183 99e1 83a3 e183  ................
+00000ac0: 9ae1 8390 e183 9320 e183 92e1 8390 e183  ....... ........
+00000ad0: a0e1 8393 e183 90e1 83a5 e183 9be1 839c  ................
+00000ae0: e183 9022 2c0a 2020 2020 2276 6965 7765  ...",.    "viewe
+00000af0: 725f 636f 6e66 6967 5f70 726f 6365 7373  r_config_process
+00000b00: 5f65 6d6f 6a69 735f 6368 6563 6b62 6f78  _emojis_checkbox
+00000b10: 5f61 6363 6573 7369 626c 655f 6465 7363  _accessible_desc
+00000b20: 7269 7074 696f 6e22 3a20 22e1 83a2 e183  ription": ".....
+00000b30: 94e1 83a5 e183 a1e1 83a2 e183 a3e1 83a0  ................
+00000b40: e183 9820 e183 94e1 839b e183 9de1 83af  ... ............
+00000b50: e183 94e1 8391 e183 98e1 83a1 20e1 8392  ............ ...
+00000b60: e183 a0e1 8390 e183 a4e1 8398 e183 99e1  ................
+00000b70: 83a3 e183 9ae1 8398 20e1 83ac e183 90e1  ........ .......
+00000b80: 83a0 e183 9be1 839d e183 a9e1 8394 e183  ................
+00000b90: 9ce1 8390 222c 0a20 2020 2022 7669 6577  ....",.    "view
+00000ba0: 6572 5f63 6f6e 6669 675f 6869 6768 6c69  er_config_highli
+00000bb0: 6768 745f 746f 646f 735f 6368 6563 6b62  ght_todos_checkb
+00000bc0: 6f78 223a 2022 544f 444f 2de1 8394 e183  ox": "TODO-.....
+00000bd0: 91e1 8398 e183 a120 e183 92e1 8390 e183  ....... ........
+00000be0: 9be1 839d e183 a7e1 839d e183 a4e1 8390  ................
+00000bf0: 222c 0a20 2020 2022 7669 6577 6572 5f63  ",.    "viewer_c
+00000c00: 6f6e 6669 675f 6869 6768 6c69 6768 745f  onfig_highlight_
+00000c10: 746f 646f 735f 6368 6563 6b62 6f78 5f61  todos_checkbox_a
+00000c20: 6363 6573 7369 626c 655f 6465 7363 7269  ccessible_descri
+00000c30: 7074 696f 6e22 3a20 2254 4f44 4f20 e183  ption": "TODO ..
+00000c40: a2e1 8394 e183 92e1 8394 e183 91e1 8398  ................
+00000c50: e183 a120 e183 92e1 8390 e183 9be1 839d  ... ............
+00000c60: e183 a7e1 839d e183 a4e1 8390 20e1 83a2  ............ ...
+00000c70: e183 94e1 83a5 e183 a1e1 83a2 e183 a8e1  ................
+00000c80: 8398 222c 0a20 2020 2022 7669 6577 6572  ..",.    "viewer
+00000c90: 5f63 6f6e 6669 675f 6f70 656e 5f6c 696e  _config_open_lin
+00000ca0: 6b5f 636f 6e66 6972 6d61 7469 6f6e 5f63  k_confirmation_c
+00000cb0: 6865 636b 626f 7822 3a20 22e1 8391 e183  heckbox": ".....
+00000cc0: 9be1 83a3 e183 9ae1 8394 e183 91e1 8398  ................
+00000cd0: e183 a120 e183 92e1 8390 e183 aee1 83a1  ... ............
+00000ce0: e183 9ce1 8398 e183 a120 e183 93e1 8390  ......... ......
+00000cf0: e183 a1e1 83a2 e183 a3e1 83a0 e183 9822  ..............."
+00000d00: 2c0a 2020 2020 2276 6965 7765 725f 636f  ,.    "viewer_co
+00000d10: 6e66 6967 5f6f 7065 6e5f 6c69 6e6b 5f63  nfig_open_link_c
+00000d20: 6f6e 6669 726d 6174 696f 6e5f 6368 6563  onfirmation_chec
+00000d30: 6b62 6f78 5f61 6363 6573 7369 626c 655f  kbox_accessible_
+00000d40: 6465 7363 7269 7074 696f 6e22 3a0a 2020  description":.  
+00000d50: 2020 2020 2020 22e1 8391 e183 9be1 83a3        ".........
+00000d60: e183 9ae1 8394 e183 91e1 8398 e183 a120  ............... 
+00000d70: e183 92e1 8390 e183 aee1 83a1 e183 9ce1  ................
+00000d80: 8398 e183 a1e1 8390 e183 a120 e183 93e1  ........... ....
+00000d90: 8390 e183 a1e1 83a2 e183 a3e1 83a0 e183  ................
+00000da0: 98e1 83a1 20e1 839b e183 9de1 8397 e183  .... ...........
+00000db0: aee1 839d e183 95e1 839c e183 9022 2c0a  .............",.
+00000dc0: 2020 2020 2276 6965 7765 725f 636f 6e66      "viewer_conf
+00000dd0: 6967 5f73 6176 655f 7265 736f 7572 6365  ig_save_resource
+00000de0: 735f 6368 6563 6b62 6f78 223a 2022 e183  s_checkbox": "..
+00000df0: 92e1 8390 e183 a0e1 8394 20e1 83a1 e183  .......... .....
+00000e00: a3e1 83a0 e183 90e1 8397 e183 94e1 8391  ................
+00000e10: e183 98e1 83a1 20e1 8390 e183 95e1 83a2  ...... .........
+00000e20: e183 9de1 839b e183 90e1 83a2 e183 a3e1  ................
+00000e30: 83a0 e183 9820 e183 a8e1 8394 e183 9ce1  ..... ..........
+00000e40: 8390 e183 aee1 8395 e183 9020 e183 93e1  ........... ....
+00000e50: 8398 e183 a1e1 8399 e183 96e1 8394 222c  ..............",
+00000e60: 0a20 2020 2022 7669 6577 6572 5f63 6f6e  .    "viewer_con
+00000e70: 6669 675f 7361 7665 5f72 6573 6f75 7263  fig_save_resourc
+00000e80: 6573 5f63 6865 636b 626f 785f 6163 6365  es_checkbox_acce
+00000e90: 7373 6962 6c65 5f64 6573 6372 6970 7469  ssible_descripti
+00000ea0: 6f6e 223a 0a20 2020 2020 2020 2022 e183  on":.        "..
+00000eb0: 92e1 8390 e183 a0e1 8394 20e1 83a1 e183  .......... .....
+00000ec0: a3e1 83a0 e183 90e1 8397 e183 94e1 8391  ................
+00000ed0: e183 98e1 83a1 20e1 8390 e183 a1e1 839a  ...... .........
+00000ee0: e183 94e1 8391 e183 98e1 83a1 20e1 8390  ............ ...
+00000ef0: e183 95e1 83a2 e183 9de1 839b e183 90e1  ................
+00000f00: 83a2 e183 a3e1 83a0 e183 90e1 8393 20e1  .............. .
+00000f10: 83a8 e183 94e1 839c e183 90e1 83ae e183  ................
+00000f20: 95e1 8390 20e1 8393 e183 98e1 83a1 e183  .... ...........
+00000f30: 99e1 8396 e183 9420 e183 9de1 83a4 e183  ....... ........
+00000f40: 9ae1 8390 e183 98e1 839c 20e1 83ac e183  .......... .....
+00000f50: 95e1 8393 e183 9de1 839b e183 98e1 83a1  ................
+00000f60: e183 97e1 8395 e183 98e1 83a1 2e22 2c0a  .............",.
+00000f70: 0a20 2020 2022 6169 5f63 6f6e 6669 675f  .    "ai_config_
+00000f80: 6f70 656e 6169 5f61 7069 5f6c 6162 656c  openai_api_label
+00000f90: 223a 2022 4f70 656e 4149 2041 5049 222c  ": "OpenAI API",
+00000fa0: 0a20 2020 2022 6169 5f63 6f6e 6669 675f  .    "ai_config_
+00000fb0: 6f70 656e 6169 5f61 7069 5f75 726c 5f69  openai_api_url_i
+00000fc0: 6e70 7574 5f70 6c61 6365 686f 6c64 6572  nput_placeholder
+00000fd0: 5f74 6578 7422 3a20 2241 5049 2055 524c  _text": "API URL
+00000fe0: 222c 0a20 2020 2022 6169 5f63 6f6e 6669  ",.    "ai_confi
+00000ff0: 675f 6f70 656e 6169 5f61 7069 5f75 726c  g_openai_api_url
+00001000: 5f69 6e70 7574 5f61 6363 6573 7369 626c  _input_accessibl
+00001010: 655f 6465 7363 7269 7074 696f 6e22 3a20  e_description": 
+00001020: 224f 7065 6e41 4920 4150 4920 5552 4c22  "OpenAI API URL"
+00001030: 2c0a 2020 2020 2261 695f 636f 6e66 6967  ,.    "ai_config
+00001040: 5f6f 7065 6e61 695f 6170 695f 6b65 795f  _openai_api_key_
+00001050: 696e 7075 745f 706c 6163 6568 6f6c 6465  input_placeholde
+00001060: 725f 7465 7874 223a 2022 4150 4920 e183  r_text": "API ..
+00001070: 92e1 8390 e183 a1e1 8390 e183 a6e1 8394  ................
+00001080: e183 91e1 8398 222c 0a20 2020 2022 6169  ......",.    "ai
+00001090: 5f63 6f6e 6669 675f 6f70 656e 6169 5f61  _config_openai_a
+000010a0: 7069 5f6b 6579 5f69 6e70 7574 5f61 6363  pi_key_input_acc
+000010b0: 6573 7369 626c 655f 6465 7363 7269 7074  essible_descript
+000010c0: 696f 6e22 3a20 224f 7065 6e41 4920 4150  ion": "OpenAI AP
+000010d0: 4920 e183 92e1 8390 e183 a1e1 8390 e183  I ..............
+000010e0: a6e1 8394 e183 91e1 8398 222c 0a20 2020  ..........",.   
+000010f0: 2022 6169 5f63 6f6e 6669 675f 6f70 656e   "ai_config_open
+00001100: 6169 5f61 7069 5f73 7570 706f 7274 6564  ai_api_supported
+00001110: 5f6d 6f64 656c 735f 6c61 6265 6c22 3a20  _models_label": 
+00001120: 22e1 839b e183 aee1 8390 e183 a0e1 8393  "...............
+00001130: e183 90e1 83ad e183 94e1 83a0 e183 98e1  ................
+00001140: 839a e183 9820 e183 9be1 839d e183 93e1  ..... ..........
+00001150: 8394 e183 9ae1 8394 e183 91e1 8398 222c  ..............",
+00001160: 0a20 2020 2022 6169 5f63 6f6e 6669 675f  .    "ai_config_
+00001170: 6169 5f6d 6f64 656c 5f6e 616d 6573 5f63  ai_model_names_c
+00001180: 6f6d 626f 5f70 6c61 6365 686f 6c64 6572  ombo_placeholder
+00001190: 5f74 6578 7422 3a20 22e1 839b e183 9de1  _text": ".......
+000011a0: 8393 e183 94e1 839a e183 98e1 83a1 20e1  .............. .
+000011b0: 8390 e183 a0e1 83a9 e183 94e1 8395 e183  ................
+000011c0: 9022 2c0a 2020 2020 2261 695f 636f 6e66  .",.    "ai_conf
+000011d0: 6967 5f61 695f 6d6f 6465 6c5f 6e61 6d65  ig_ai_model_name
+000011e0: 735f 636f 6d62 6f5f 6163 6365 7373 6962  s_combo_accessib
+000011f0: 6c65 5f64 6573 6372 6970 7469 6f6e 223a  le_description":
+00001200: 2022 e183 9be1 83ae e183 90e1 83a0 e183   "..............
+00001210: 93e1 8390 e183 ade1 8394 e183 a0e1 8398  ................
+00001220: e183 9ae1 8398 20e1 839b e183 9de1 8393  ...... .........
+00001230: e183 94e1 839a e183 94e1 8391 e183 98e1  ................
+00001240: 83a1 20e1 8390 e183 a0e1 83a9 e183 94e1  .. .............
+00001250: 8395 e183 9022 2c0a 0a20 2020 2022 6169  .....",..    "ai
+00001260: 5f63 6f6e 6669 675f 6261 7365 5f6c 6162  _config_base_lab
+00001270: 656c 223a 2022 e183 a1e1 8390 e183 91e1  el": "..........
+00001280: 8390 e183 96e1 839d 20e1 839e e183 90e1  ........ .......
+00001290: 83a0 e183 90e1 839b e183 94e1 83a2 e183  ................
+000012a0: a0e1 8394 e183 91e1 8398 222c 0a20 2020  ..........",.   
+000012b0: 2022 6169 5f63 6f6e 6669 675f 6261 7365   "ai_config_base
+000012c0: 5f73 7973 7465 6d5f 7072 6f6d 7074 5f6c  _system_prompt_l
+000012d0: 6162 656c 223a 2022 e183 a1e1 8398 e183  abel": "........
+000012e0: a1e1 83a2 e183 94e1 839b e183 a3e1 83a0  ................
+000012f0: e183 9820 e183 9ee1 83a0 e183 9de1 839b  ... ............
+00001300: e183 9ee1 83a2 e183 9822 2c0a 2020 2020  .........",.    
+00001310: 2261 695f 636f 6e66 6967 5f62 6173 655f  "ai_config_base_
+00001320: 7379 7374 656d 5f70 726f 6d70 745f 6564  system_prompt_ed
+00001330: 6974 5f70 6c61 6365 686f 6c64 6572 5f74  it_placeholder_t
+00001340: 6578 7422 3a20 22e1 83a1 e183 90e1 8391  ext": ".........
+00001350: e183 90e1 8396 e183 9d20 e183 a1e1 8398  ......... ......
+00001360: e183 a1e1 83a2 e183 94e1 839b e183 a3e1  ................
+00001370: 83a0 e183 9820 e183 9ee1 83a0 e183 9de1  ..... ..........
+00001380: 839b e183 9ee1 83a2 e183 982c 20e1 83a0  ..........., ...
+00001390: e183 9de1 839b e183 94e1 839a e183 98e1  ................
+000013a0: 83aa 20e1 83a7 e183 9de1 8395 e183 94e1  .. .............
+000013b0: 839a 20e1 839b e183 9de1 8397 e183 aee1  .. .............
+000013c0: 839d e183 95e1 839c e183 90e1 83a1 20e1  .............. .
+000013d0: 83ac e183 98e1 839c e183 90e1 83a1 e183  ................
+000013e0: ace1 8390 e183 a020 e183 9be1 8398 e183  ....... ........
+000013f0: 93e1 8398 e183 a122 2c0a 2020 2020 2261  .......",.    "a
+00001400: 695f 636f 6e66 6967 5f62 6173 655f 7379  i_config_base_sy
+00001410: 7374 656d 5f70 726f 6d70 745f 6564 6974  stem_prompt_edit
+00001420: 5f61 6363 6573 7369 626c 655f 6465 7363  _accessible_desc
+00001430: 7269 7074 696f 6e22 3a0a 2020 2020 2020  ription":.      
+00001440: 2020 22e1 83a1 e183 90e1 8391 e183 90e1    ".............
+00001450: 8396 e183 9d20 e183 a1e1 8398 e183 a1e1  ..... ..........
+00001460: 83a2 e183 94e1 839b e183 a3e1 83a0 e183  ................
+00001470: 9820 e183 9ee1 83a0 e183 9de1 839b e183  . ..............
+00001480: 9ee1 83a2 e183 982c 20e1 83a0 e183 9de1  ......., .......
+00001490: 839b e183 94e1 839a e183 98e1 83aa 20e1  .............. .
+000014a0: 83a7 e183 9de1 8395 e183 94e1 839a 20e1  .............. .
+000014b0: 839b e183 9de1 8397 e183 aee1 839d e183  ................
+000014c0: 95e1 839c e183 90e1 83a1 20e1 83ac e183  .......... .....
+000014d0: 98e1 839c e183 90e1 83a1 e183 ace1 8390  ................
+000014e0: e183 a020 e183 9be1 8398 e183 93e1 8398  ... ............
+000014f0: e183 a12e 20e1 8394 e183 a120 e183 a2e1  .... ...... ....
+00001500: 8394 e183 a5e1 83a1 e183 a2e1 8398 e183  ................
+00001510: 902e 222c 0a20 2020 2022 6169 5f63 6f6e  ..",.    "ai_con
+00001520: 6669 675f 6261 7365 5f72 6573 706f 6e73  fig_base_respons
+00001530: 655f 6d61 785f 746f 6b65 6e73 5f6c 6162  e_max_tokens_lab
+00001540: 656c 223a 2022 e183 9ee1 8390 e183 a1e1  el": "..........
+00001550: 83a3 e183 aee1 8398 e183 a120 e183 9be1  ........... ....
+00001560: 8390 e183 a5e1 83a1 e183 98e1 839b e183  ................
+00001570: 90e1 839a e183 a3e1 83a0 e183 9820 e183  ............. ..
+00001580: a2e1 839d e183 99e1 8394 e183 9ce1 8394  ................
+00001590: e183 91e1 8398 222c 0a20 2020 2022 6169  ......",.    "ai
+000015a0: 5f63 6f6e 6669 675f 6261 7365 5f72 6573  _config_base_res
+000015b0: 706f 6e73 655f 6d61 785f 746f 6b65 6e73  ponse_max_tokens
+000015c0: 5f69 6e70 7574 5f61 6363 6573 7369 626c  _input_accessibl
+000015d0: 655f 6465 7363 7269 7074 696f 6e22 3a20  e_description": 
+000015e0: 22e1 839e e183 90e1 83a1 e183 a3e1 83ae  "...............
+000015f0: e183 a8e1 8398 20e1 839b e183 98e1 83a1  ...... .........
+00001600: e183 90e1 83a6 e183 94e1 8391 e183 9820  ............... 
+00001610: e183 a2e1 839d e183 99e1 8394 e183 9ce1  ................
+00001620: 8394 e183 91e1 8398 e183 a120 e183 9be1  ........... ....
+00001630: 8390 e183 a5e1 83a1 e183 98e1 839b e183  ................
+00001640: 90e1 839a e183 a3e1 83a0 e183 9820 e183  ............. ..
+00001650: a0e1 8390 e183 9de1 8393 e183 94e1 839c  ................
+00001660: e183 9de1 8391 e183 9022 2c0a 7d0a       .........",.}.
```

### Comparing `notolog-0.9.1b1/app/lexemes/ge/ai_assistant.py` & `notolog-0.9.1b2/notolog/lexemes/ge/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/ge/color_picker_dialog.py` & `notolog-0.9.1b2/notolog/lexemes/ge/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/ge/common.py` & `notolog-0.9.1b2/notolog/lexemes/ge/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     "save_active_file_error_occurred": "ფაილის შენახვა ვერ ხერხდება, წარმოიშვა შეცდომა",
 
     "expandable_block_default_title": "მეტი ინფორმაცია...",
 
     "dialog_color_picker_color_copied_to_the_clipboard": "ფორმატირებული ტექსტი ბუფერში ასლი გადაიტანეს",
 
     "popup_about_title": "აპლიკაციის ინფორმაცია",
-    "popup_about_app_name_description": "Markdown რედაქტორი",
+    "popup_about_app_name_description": "Python-ის Markdown რედაქტორი",
 
     "popup_about_version": "ვერსია",
     "popup_about_license": "ლიცენზია",
     "popup_about_website": "ვებგვერდი",
     "popup_about_repository": "GitHub",
     "popup_about_pypi": "PyPi",
     "popup_about_date": "თარიღი",
```

### Comparing `notolog-0.9.1b1/app/lexemes/ge/main_menu.py` & `notolog-0.9.1b2/notolog/lexemes/ge/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/ge/statusbar.py` & `notolog-0.9.1b2/notolog/lexemes/ge/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/ge/toolbar.py` & `notolog-0.9.1b2/notolog/lexemes/ge/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/gr/__pycache__/main_menu.cpython-39.pyc` & `notolog-0.9.1b2/notolog/lexemes/gr/main_menu.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,176 +1,182 @@
-00000000: 610d 0d0a 0000 0000 42a9 3566 5b0b 0000  a.......B.5f[...
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0029 0000 0040 0000 0073 5a00 0000 6400  .)...@...sZ...d.
-00000030: 6401 6402 6403 6404 6404 6405 6406 6407  d.d.d.d.d.d.d.d.
-00000040: 6408 6409 640a 640b 640c 6401 640d 640e  d.d.d.d.d.d.d.d.
-00000050: 640e 640f 6410 6411 6412 6413 6414 6415  d.d.d.d.d.d.d.d.
-00000060: 6416 6417 6418 6419 641a 641b 641c 641d  d.d.d.d.d.d.d.d.
-00000070: 641d 641e 641e 641f 6420 6421 6421 6422  d.d.d.d.d d!d!d"
-00000080: 9c28 5a00 6423 5300 2924 750c 0000 00ce  .(Z.d#S.)$u.....
-00000090: 91cf 81cf 87ce b5ce afce bf75 1600 0000  ...........u....
-000000a0: ce95 cf80 ceb5 cebe ceb5 cf81 ceb3 ceb1  ................
-000000b0: cf83 ceaf ceb1 7510 0000 00ce 95cf 81ce  ......u.........
-000000c0: b3ce b1ce bbce b5ce afce b175 0e00 0000  ...........u....
-000000d0: ce92 cebf ceae ceb8 ceb5 ceb9 ceb1 7515  ..............u.
-000000e0: 0000 00ce 9dce adce bf20 cead ceb3 ceb3  ......... ......
-000000f0: cf81 ceb1 cf86 cebf 750e 0000 00ce 86ce  ........u.......
-00000100: bdce bfce b9ce b3ce bcce b175 1f00 0000  ...........u....
-00000110: ce86 cebd cebf ceb9 ceb3 cebc ceb1 20ce  .............. .
-00000120: b5ce b3ce b3cf 81ce accf 86ce bfcf 8575  ...............u
-00000130: 1400 0000 ce91 cf80 cebf ceb8 ceae ceba  ................
-00000140: ceb5 cf85 cf83 ceb7 7525 0000 00ce 91cf  ........u%......
-00000150: 80ce bfce b8ce aece bace b5cf 85cf 83ce  ................
-00000160: b720 ceb5 ceb3 ceb3 cf81 ceac cf86 cebf  . ..............
-00000170: cf85 7519 0000 00ce 91cf 80ce bfce b8ce  ..u.............
-00000180: aece bace b5cf 85cf 83ce b720 cf89 cf82  ........... ....
-00000190: 753d 0000 00ce 91cf 80ce bfce b8ce aece  u=..............
-000001a0: bace b5cf 85cf 83ce b720 cf89 cf82 20ce  ......... .... .
-000001b0: b1ce bdcf 84ce afce b3cf 81ce b1cf 86ce  ................
-000001c0: bf20 ceb5 ceb3 ceb3 cf81 ceac cf86 cebf  . ..............
-000001d0: cf85 750c 0000 00ce 88ce bece bfce b4ce  ..u.............
-000001e0: bfcf 8275 2b00 0000 ce88 cebe cebf ceb4  ...u+...........
-000001f0: cebf cf82 20ce b1cf 80cf 8c20 cf84 ceb7  .... ...... ....
-00000200: cebd 20ce b5cf 86ce b1cf 81ce bcce bfce  .. .............
-00000210: b3ce ae75 2500 0000 ce95 cf80 ceb5 cebe  ...u%...........
-00000220: ceb5 cf81 ceb3 ceb1 cf83 ceaf ceb1 20ce  .............. .
-00000230: b1cf 81cf 87ce b5ce afce bfcf 8575 1d00  .............u..
-00000240: 0000 cea0 ceb7 ceb3 ceb1 ceaf cebf cf82  ................
-00000250: 20ce bacf 8ece b4ce b9ce bace b1cf 8275   ..............u
-00000260: 0c00 0000 ce88 cebd cf84 cebf cebd ceb1  ................
-00000270: 752a 0000 00ce 9cce bfcf 81cf 86ce ae20  u*............. 
-00000280: cead cebd cf84 cebf cebd cebf cf85 20ce  .............. .
-00000290: bace b5ce b9ce bcce adce bdce bfcf 8575  ...............u
-000002a0: 0c00 0000 cea0 cebb ceac ceb3 ceb9 ceb1  ................
-000002b0: 752a 0000 00ce 9cce bfcf 81cf 86ce ae20  u*............. 
-000002c0: cf80 cebb ceac ceb3 ceb9 cebf cf85 20ce  .............. .
-000002d0: bace b5ce b9ce bcce adce bdce bfcf 8575  ...............u
-000002e0: 1600 0000 cea5 cf80 cebf ceb3 cf81 ceac  ................
-000002f0: cebc cebc ceb9 cf83 ceb7 7538 0000 00ce  ..........u8....
-00000300: 9cce bfcf 81cf 86ce ae20 cf85 cf80 cebf  ......... ......
-00000310: ceb3 ceb5 ceb3 cf81 ceb1 cebc cebc cead  ................
-00000320: cebd cebf cf85 20ce bace b5ce b9ce bcce  ...... .........
-00000330: adce bdce bfcf 8575 1a00 0000 ce94 ceb9  .......u........
-00000340: ceb1 ceb3 cf81 ceb1 cebc cebc ceaf cf83  ................
-00000350: ceb5 ceb9 cf82 753a 0000 00ce 9cce bfcf  ......u:........
-00000360: 81cf 86ce ae20 ceb4 ceb9 ceb1 ceb3 cf81  ..... ..........
-00000370: ceb1 cebc cebc ceb9 cf83 cebc cead cebd  ................
-00000380: cebf cf85 20ce bace b5ce b9ce bcce adce  .... ...........
-00000390: bdce bfcf 8575 1000 0000 cea0 ceb1 cf81  .....u..........
-000003a0: ceac ceb8 ceb5 cf83 ceb7 752e 0000 00ce  ..........u.....
-000003b0: 9cce bfcf 81cf 86ce ae20 ceba ceb5 ceb9  ......... ......
-000003c0: cebc cead cebd cebf cf85 20cf 80ce b1cf  .......... .....
-000003d0: 81ce acce b8ce b5cf 83ce b7cf 8275 0f00  .............u..
-000003e0: 0000 ce92 cebf ceb7 ceb8 cf8c cf82 2041  .............. A
-000003f0: 4975 2000 0000 ce95 ceba ceba ceaf cebd  Iu .............
-00000400: ceb7 cf83 ceb7 20ce 92ce bfce b7ce b8ce  ...... .........
-00000410: bfcf 8d20 4149 7523 0000 00ce 95cf 80ce  ... AIu#........
-00000420: b9ce bbce bfce b3ce adce b1cf 8220 cf87  ............. ..
-00000430: cf81 cf8e cebc ceb1 cf84 cebf cf82 752c  ..............u,
-00000440: 0000 00ce 95cf 80ce b9ce bbce adce becf  ................
-00000450: 84ce b520 cf87 cf81 cf8e cebc ceb1 20ce  ... .......... .
-00000460: bace b5ce b9ce bcce adce bdce bfcf 8575  ...............u
-00000470: 1700 0000 cea3 cf8d cebd cf84 ceb1 cebe  ................
-00000480: ceb7 204d 6172 6b64 6f77 6e75 2c00 0000  .. Markdownu,...
-00000490: ce88 cebb ceb5 ceb3 cf87 cebf cf82 20ce  .............. .
-000004a0: b3ce b9ce b120 ceb5 cebd ceb7 cebc ceb5  ..... ..........
-000004b0: cf81 cf8e cf83 ceb5 ceb9 cf82 7521 0000  ............u!..
-000004c0: 00ce 91ce bdce b1cf 86ce bfcf 81ce ac20  ............... 
-000004d0: cf83 cf86 ceb1 cebb cebc ceac cf84 cf89  ................
-000004e0: cebd 7532 0000 00ce a5cf 80ce bfce b2ce  ..u2............
-000004f0: bfce bbce ae20 ceb1 cebd ceb1 cf86 cebf  ..... ..........
-00000500: cf81 ceac cf82 20cf 83cf 86ce acce bbce  ...... .........
-00000510: bcce b1cf 84ce bfcf 8275 1600 0000 cea0  .........u......
-00000520: cebb ceb7 cf81 cebf cf86 cebf cf81 ceaf  ................
-00000530: ceb5 cf82 2928 da10 6772 6f75 705f 6669  ....)(..group_fi
-00000540: 6c65 5f6c 6162 656c da10 6772 6f75 705f  le_label..group_
-00000550: 6564 6974 5f6c 6162 656c da11 6772 6f75  edit_label..grou
-00000560: 705f 746f 6f6c 735f 6c61 6265 6cda 1067  p_tools_label..g
-00000570: 726f 7570 5f68 656c 705f 6c61 6265 6cda  roup_help_label.
-00000580: 1f61 6374 696f 6e73 5f66 696c 655f 6c61  .actions_file_la
-00000590: 6265 6c5f 6e65 775f 646f 6375 6d65 6e74  bel_new_document
-000005a0: da29 6163 7469 6f6e 735f 6669 6c65 5f61  .)actions_file_a
-000005b0: 6363 6573 7369 626c 655f 6e61 6d65 5f6e  ccessible_name_n
-000005c0: 6577 5f64 6f63 756d 656e 74da 1761 6374  ew_document..act
-000005d0: 696f 6e73 5f66 696c 655f 6c61 6265 6c5f  ions_file_label_
-000005e0: 6f70 656e da21 6163 7469 6f6e 735f 6669  open.!actions_fi
-000005f0: 6c65 5f61 6363 6573 7369 626c 655f 6e61  le_accessible_na
-00000600: 6d65 5f6f 7065 6eda 1761 6374 696f 6e73  me_open..actions
-00000610: 5f66 696c 655f 6c61 6265 6c5f 7361 7665  _file_label_save
-00000620: da21 6163 7469 6f6e 735f 6669 6c65 5f61  .!actions_file_a
-00000630: 6363 6573 7369 626c 655f 6e61 6d65 5f73  ccessible_name_s
-00000640: 6176 65da 1a61 6374 696f 6e73 5f66 696c  ave..actions_fil
-00000650: 655f 6c61 6265 6c5f 7361 7665 5f61 73da  e_label_save_as.
-00000660: 2461 6374 696f 6e73 5f66 696c 655f 6163  $actions_file_ac
-00000670: 6365 7373 6962 6c65 5f6e 616d 655f 7361  cessible_name_sa
-00000680: 7665 5f61 73da 1761 6374 696f 6e73 5f66  ve_as..actions_f
-00000690: 696c 655f 6c61 6265 6c5f 6578 6974 da21  ile_label_exit.!
-000006a0: 6163 7469 6f6e 735f 6669 6c65 5f61 6363  actions_file_acc
-000006b0: 6573 7369 626c 655f 6e61 6d65 5f65 7869  essible_name_exi
-000006c0: 74da 1665 6469 745f 6163 7469 6f6e 735f  t..edit_actions_
-000006d0: 6564 6974 5f6d 6f64 65da 2665 6469 745f  edit_mode.&edit_
-000006e0: 6163 7469 6f6e 735f 6163 6365 7373 6962  actions_accessib
-000006f0: 6c65 5f6e 616d 655f 6564 6974 5f6d 6f64  le_name_edit_mod
-00000700: 65da 1865 6469 745f 6163 7469 6f6e 735f  e..edit_actions_
-00000710: 736f 7572 6365 5f6d 6f64 65da 2865 6469  source_mode.(edi
-00000720: 745f 6163 7469 6f6e 735f 6163 6365 7373  t_actions_access
-00000730: 6962 6c65 5f6e 616d 655f 736f 7572 6365  ible_name_source
-00000740: 5f6d 6f64 65da 1165 6469 745f 6163 7469  _mode..edit_acti
-00000750: 6f6e 735f 626f 6c64 da21 6564 6974 5f61  ons_bold.!edit_a
-00000760: 6374 696f 6e73 5f61 6363 6573 7369 626c  ctions_accessibl
-00000770: 655f 6e61 6d65 5f62 6f6c 64da 1365 6469  e_name_bold..edi
-00000780: 745f 6163 7469 6f6e 735f 6974 616c 6963  t_actions_italic
-00000790: da23 6564 6974 5f61 6374 696f 6e73 5f61  .#edit_actions_a
-000007a0: 6363 6573 7369 626c 655f 6e61 6d65 5f69  ccessible_name_i
-000007b0: 7461 6c69 63da 1665 6469 745f 6163 7469  talic..edit_acti
-000007c0: 6f6e 735f 756e 6465 726c 696e 65da 2665  ons_underline.&e
-000007d0: 6469 745f 6163 7469 6f6e 735f 6163 6365  dit_actions_acce
-000007e0: 7373 6962 6c65 5f6e 616d 655f 756e 6465  ssible_name_unde
-000007f0: 726c 696e 65da 1a65 6469 745f 6163 7469  rline..edit_acti
-00000800: 6f6e 735f 7374 7269 6b65 7468 726f 7567  ons_strikethroug
-00000810: 68da 2a65 6469 745f 6163 7469 6f6e 735f  h.*edit_actions_
-00000820: 6163 6365 7373 6962 6c65 5f6e 616d 655f  accessible_name_
-00000830: 7374 7269 6b65 7468 726f 7567 68da 1765  strikethrough..e
-00000840: 6469 745f 6163 7469 6f6e 735f 626c 6f63  dit_actions_bloc
-00000850: 6b71 756f 7465 da27 6564 6974 5f61 6374  kquote.'edit_act
-00000860: 696f 6e73 5f61 6363 6573 7369 626c 655f  ions_accessible_
-00000870: 6e61 6d65 5f62 6c6f 636b 7175 6f74 65da  name_blockquote.
-00000880: 1a74 6f6f 6c73 5f61 6374 696f 6e73 5f61  .tools_actions_a
-00000890: 695f 6173 7369 7374 616e 74da 2a74 6f6f  i_assistant.*too
-000008a0: 6c73 5f61 6374 696f 6e73 5f61 6363 6573  ls_actions_acces
-000008b0: 7369 626c 655f 6e61 6d65 5f61 695f 6173  sible_name_ai_as
-000008c0: 7369 7374 616e 74da 1a74 6f6f 6c73 5f61  sistant..tools_a
-000008d0: 6374 696f 6e73 5f63 6f6c 6f72 5f70 6963  ctions_color_pic
-000008e0: 6b65 72da 2a74 6f6f 6c73 5f61 6374 696f  ker.*tools_actio
-000008f0: 6e73 5f61 6363 6573 7369 626c 655f 6e61  ns_accessible_na
-00000900: 6d65 5f63 6f6c 6f72 5f70 6963 6b65 72da  me_color_picker.
-00000910: 1c61 6374 696f 6e73 5f68 656c 705f 6c61  .actions_help_la
-00000920: 6265 6c5f 6d64 5f73 796e 7461 78da 2661  bel_md_syntax.&a
-00000930: 6374 696f 6e73 5f68 656c 705f 6163 6365  ctions_help_acce
-00000940: 7373 6962 6c65 5f6e 616d 655f 6d64 5f73  ssible_name_md_s
-00000950: 796e 7461 78da 2461 6374 696f 6e73 5f68  yntax.$actions_h
-00000960: 656c 705f 6c61 6265 6c5f 6368 6563 6b5f  elp_label_check_
-00000970: 666f 725f 7570 6461 7465 73da 2e61 6374  for_updates..act
-00000980: 696f 6e73 5f68 656c 705f 6163 6365 7373  ions_help_access
-00000990: 6962 6c65 5f6e 616d 655f 6368 6563 6b5f  ible_name_check_
-000009a0: 666f 725f 7570 6461 7465 73da 1d61 6374  for_updates..act
-000009b0: 696f 6e73 5f68 656c 705f 6c61 6265 6c5f  ions_help_label_
-000009c0: 6275 675f 7265 706f 7274 da27 6163 7469  bug_report.'acti
-000009d0: 6f6e 735f 6865 6c70 5f61 6363 6573 7369  ons_help_accessi
-000009e0: 626c 655f 6e61 6d65 5f62 7567 5f72 6570  ble_name_bug_rep
-000009f0: 6f72 74da 1861 6374 696f 6e73 5f68 656c  ort..actions_hel
-00000a00: 705f 6c61 6265 6c5f 6162 6f75 74da 2261  p_label_about."a
-00000a10: 6374 696f 6e73 5f68 656c 705f 6163 6365  ctions_help_acce
-00000a20: 7373 6962 6c65 5f6e 616d 655f 6162 6f75  ssible_name_abou
-00000a30: 744e 2901 da07 6c65 7865 6d65 73a9 0072  tN)...lexemes..r
-00000a40: 2a00 0000 722a 0000 00fa 462f 5573 6572  *...r*....F/User
-00000a50: 732f 7661 6469 6b75 732f 5079 6368 6172  s/vadikus/Pychar
-00000a60: 6d50 726f 6a65 6374 732f 6e6f 746f 6c6f  mProjects/notolo
-00000a70: 672d 6465 762f 6170 702f 6c65 7865 6d65  g-dev/app/lexeme
-00000a80: 732f 6772 2f6d 6169 6e5f 6d65 6e75 2e70  s/gr/main_menu.p
-00000a90: 79da 083c 6d6f 6475 6c65 3e03 0000 0073  y..<module>....s
-00000aa0: 5000 0000 0201 0201 0201 0202 0201 0201  P...............
-00000ab0: 0201 0201 0201 0201 0201 0201 0201 0202  ................
-00000ac0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00000ad0: 0201 0201 0201 0201 0201 0202 0201 0201  ................
-00000ae0: 0201 0202 0201 0201 0201 0201 0201 0201  ................
-00000af0: 0201 02d4                                ....
+00000000: 2320 4772 6565 6b20 6c65 7865 6d65 7320  # Greek lexemes 
+00000010: 6d61 696e 5f6d 656e 752e 7079 0a6c 6578  main_menu.py.lex
+00000020: 656d 6573 203d 207b 0a20 2020 2022 6772  emes = {.    "gr
+00000030: 6f75 705f 6669 6c65 5f6c 6162 656c 223a  oup_file_label":
+00000040: 2022 ce91 cf81 cf87 ceb5 ceaf cebf 222c   "............",
+00000050: 0a20 2020 2022 6772 6f75 705f 6564 6974  .    "group_edit
+00000060: 5f6c 6162 656c 223a 2022 ce95 cf80 ceb5  _label": "......
+00000070: cebe ceb5 cf81 ceb3 ceb1 cf83 ceaf ceb1  ................
+00000080: 222c 0a20 2020 2022 6772 6f75 705f 746f  ",.    "group_to
+00000090: 6f6c 735f 6c61 6265 6c22 3a20 22ce 95cf  ols_label": "...
+000000a0: 81ce b3ce b1ce bbce b5ce afce b122 2c0a  .............",.
+000000b0: 2020 2020 2267 726f 7570 5f68 656c 705f      "group_help_
+000000c0: 6c61 6265 6c22 3a20 22ce 92ce bfce aece  label": ".......
+000000d0: b8ce b5ce b9ce b122 2c0a 0a20 2020 2022  .......",..    "
+000000e0: 6163 7469 6f6e 735f 6669 6c65 5f6c 6162  actions_file_lab
+000000f0: 656c 5f6e 6577 5f64 6f63 756d 656e 7422  el_new_document"
+00000100: 3a20 22ce 9dce adce bf20 cead ceb3 ceb3  : "...... ......
+00000110: cf81 ceb1 cf86 cebf 222c 0a20 2020 2022  ........",.    "
+00000120: 6163 7469 6f6e 735f 6669 6c65 5f61 6363  actions_file_acc
+00000130: 6573 7369 626c 655f 6e61 6d65 5f6e 6577  essible_name_new
+00000140: 5f64 6f63 756d 656e 7422 3a20 22ce 9dce  _document": "...
+00000150: adce bf20 cead ceb3 ceb3 cf81 ceb1 cf86  ... ............
+00000160: cebf 222c 0a20 2020 2022 6163 7469 6f6e  ..",.    "action
+00000170: 735f 6669 6c65 5f6c 6162 656c 5f6f 7065  s_file_label_ope
+00000180: 6e22 3a20 22ce 86ce bdce bfce b9ce b3ce  n": "...........
+00000190: bcce b122 2c0a 2020 2020 2261 6374 696f  ...",.    "actio
+000001a0: 6e73 5f66 696c 655f 6163 6365 7373 6962  ns_file_accessib
+000001b0: 6c65 5f6e 616d 655f 6f70 656e 223a 2022  le_name_open": "
+000001c0: ce86 cebd cebf ceb9 ceb3 cebc ceb1 20ce  .............. .
+000001d0: b5ce b3ce b3cf 81ce accf 86ce bfcf 8522  ..............."
+000001e0: 2c0a 2020 2020 2261 6374 696f 6e73 5f66  ,.    "actions_f
+000001f0: 696c 655f 6c61 6265 6c5f 7361 7665 223a  ile_label_save":
+00000200: 2022 ce91 cf80 cebf ceb8 ceae ceba ceb5   "..............
+00000210: cf85 cf83 ceb7 222c 0a20 2020 2022 6163  ......",.    "ac
+00000220: 7469 6f6e 735f 6669 6c65 5f61 6363 6573  tions_file_acces
+00000230: 7369 626c 655f 6e61 6d65 5f73 6176 6522  sible_name_save"
+00000240: 3a20 22ce 91cf 80ce bfce b8ce aece bace  : ".............
+00000250: b5cf 85cf 83ce b720 ceb5 ceb3 ceb3 cf81  ....... ........
+00000260: ceac cf86 cebf cf85 222c 0a20 2020 2022  ........",.    "
+00000270: 6163 7469 6f6e 735f 6669 6c65 5f6c 6162  actions_file_lab
+00000280: 656c 5f73 6176 655f 6173 223a 2022 ce91  el_save_as": "..
+00000290: cf80 cebf ceb8 ceae ceba ceb5 cf85 cf83  ................
+000002a0: ceb7 20cf 89cf 8222 2c0a 2020 2020 2261  .. ....",.    "a
+000002b0: 6374 696f 6e73 5f66 696c 655f 6163 6365  ctions_file_acce
+000002c0: 7373 6962 6c65 5f6e 616d 655f 7361 7665  ssible_name_save
+000002d0: 5f61 7322 3a20 22ce 91cf 80ce bfce b8ce  _as": ".........
+000002e0: aece bace b5cf 85cf 83ce b720 cf89 cf82  ........... ....
+000002f0: 20ce b1ce bdcf 84ce afce b3cf 81ce b1cf   ...............
+00000300: 86ce bf20 ceb5 ceb3 ceb3 cf81 ceac cf86  ... ............
+00000310: cebf cf85 222c 0a20 2020 2022 6163 7469  ....",.    "acti
+00000320: 6f6e 735f 6669 6c65 5f6c 6162 656c 5f65  ons_file_label_e
+00000330: 7869 7422 3a20 22ce 88ce bece bfce b4ce  xit": ".........
+00000340: bfcf 8222 2c0a 2020 2020 2261 6374 696f  ...",.    "actio
+00000350: 6e73 5f66 696c 655f 6163 6365 7373 6962  ns_file_accessib
+00000360: 6c65 5f6e 616d 655f 6578 6974 223a 2022  le_name_exit": "
+00000370: ce88 cebe cebf ceb4 cebf cf82 20ce b1cf  ............ ...
+00000380: 80cf 8c20 cf84 ceb7 cebd 20ce b5cf 86ce  ... ...... .....
+00000390: b1cf 81ce bcce bfce b3ce ae22 2c0a 0a20  ...........",.. 
+000003a0: 2020 2022 6564 6974 5f61 6374 696f 6e73     "edit_actions
+000003b0: 5f65 6469 745f 6d6f 6465 223a 2022 ce95  _edit_mode": "..
+000003c0: cf80 ceb5 cebe ceb5 cf81 ceb3 ceb1 cf83  ................
+000003d0: ceaf ceb1 222c 0a20 2020 2022 6564 6974  ....",.    "edit
+000003e0: 5f61 6374 696f 6e73 5f61 6363 6573 7369  _actions_accessi
+000003f0: 626c 655f 6e61 6d65 5f65 6469 745f 6d6f  ble_name_edit_mo
+00000400: 6465 223a 2022 ce95 cf80 ceb5 cebe ceb5  de": "..........
+00000410: cf81 ceb3 ceb1 cf83 ceaf ceb1 20ce b1cf  ............ ...
+00000420: 81cf 87ce b5ce afce bfcf 8522 2c0a 2020  ...........",.  
+00000430: 2020 2265 6469 745f 6163 7469 6f6e 735f    "edit_actions_
+00000440: 736f 7572 6365 5f6d 6f64 6522 3a20 22ce  source_mode": ".
+00000450: a0ce b7ce b3ce b1ce afce bfcf 8220 ceba  ............. ..
+00000460: cf8e ceb4 ceb9 ceba ceb1 cf82 222c 0a20  ............",. 
+00000470: 2020 2022 6564 6974 5f61 6374 696f 6e73     "edit_actions
+00000480: 5f61 6363 6573 7369 626c 655f 6e61 6d65  _accessible_name
+00000490: 5f73 6f75 7263 655f 6d6f 6465 223a 2022  _source_mode": "
+000004a0: cea0 ceb7 ceb3 ceb1 ceaf cebf cf82 20ce  .............. .
+000004b0: bacf 8ece b4ce b9ce bace b1cf 8222 2c0a  .............",.
+000004c0: 2020 2020 2265 6469 745f 6163 7469 6f6e      "edit_action
+000004d0: 735f 626f 6c64 223a 2022 ce88 cebd cf84  s_bold": "......
+000004e0: cebf cebd ceb1 222c 0a20 2020 2022 6564  ......",.    "ed
+000004f0: 6974 5f61 6374 696f 6e73 5f61 6363 6573  it_actions_acces
+00000500: 7369 626c 655f 6e61 6d65 5f62 6f6c 6422  sible_name_bold"
+00000510: 3a20 22ce 9cce bfcf 81cf 86ce ae20 cead  : ".......... ..
+00000520: cebd cf84 cebf cebd cebf cf85 20ce bace  ............ ...
+00000530: b5ce b9ce bcce adce bdce bfcf 8522 2c0a  .............",.
+00000540: 2020 2020 2265 6469 745f 6163 7469 6f6e      "edit_action
+00000550: 735f 6974 616c 6963 223a 2022 cea0 cebb  s_italic": "....
+00000560: ceac ceb3 ceb9 ceb1 222c 0a20 2020 2022  ........",.    "
+00000570: 6564 6974 5f61 6374 696f 6e73 5f61 6363  edit_actions_acc
+00000580: 6573 7369 626c 655f 6e61 6d65 5f69 7461  essible_name_ita
+00000590: 6c69 6322 3a20 22ce 9cce bfcf 81cf 86ce  lic": ".........
+000005a0: ae20 cf80 cebb ceac ceb3 ceb9 cebf cf85  . ..............
+000005b0: 20ce bace b5ce b9ce bcce adce bdce bfcf   ...............
+000005c0: 8522 2c0a 2020 2020 2265 6469 745f 6163  .",.    "edit_ac
+000005d0: 7469 6f6e 735f 756e 6465 726c 696e 6522  tions_underline"
+000005e0: 3a20 22ce a5cf 80ce bfce b3cf 81ce acce  : ".............
+000005f0: bcce bcce b9cf 83ce b722 2c0a 2020 2020  .........",.    
+00000600: 2265 6469 745f 6163 7469 6f6e 735f 6163  "edit_actions_ac
+00000610: 6365 7373 6962 6c65 5f6e 616d 655f 756e  cessible_name_un
+00000620: 6465 726c 696e 6522 3a20 22ce 9cce bfcf  derline": ".....
+00000630: 81cf 86ce ae20 cf85 cf80 cebf ceb3 ceb5  ..... ..........
+00000640: ceb3 cf81 ceb1 cebc cebc cead cebd cebf  ................
+00000650: cf85 20ce bace b5ce b9ce bcce adce bdce  .. .............
+00000660: bfcf 8522 2c0a 2020 2020 2265 6469 745f  ...",.    "edit_
+00000670: 6163 7469 6f6e 735f 7374 7269 6b65 7468  actions_striketh
+00000680: 726f 7567 6822 3a20 22ce 94ce b9ce b1ce  rough": ".......
+00000690: b3cf 81ce b1ce bcce bcce afcf 83ce b5ce  ................
+000006a0: b9cf 8222 2c0a 2020 2020 2265 6469 745f  ...",.    "edit_
+000006b0: 6163 7469 6f6e 735f 6163 6365 7373 6962  actions_accessib
+000006c0: 6c65 5f6e 616d 655f 7374 7269 6b65 7468  le_name_striketh
+000006d0: 726f 7567 6822 3a20 22ce 9cce bfcf 81cf  rough": ".......
+000006e0: 86ce ae20 ceb4 ceb9 ceb1 ceb3 cf81 ceb1  ... ............
+000006f0: cebc cebc ceb9 cf83 cebc cead cebd cebf  ................
+00000700: cf85 20ce bace b5ce b9ce bcce adce bdce  .. .............
+00000710: bfcf 8522 2c0a 2020 2020 2265 6469 745f  ...",.    "edit_
+00000720: 6163 7469 6f6e 735f 626c 6f63 6b71 756f  actions_blockquo
+00000730: 7465 223a 2022 cea0 ceb1 cf81 ceac ceb8  te": "..........
+00000740: ceb5 cf83 ceb7 222c 0a20 2020 2022 6564  ......",.    "ed
+00000750: 6974 5f61 6374 696f 6e73 5f61 6363 6573  it_actions_acces
+00000760: 7369 626c 655f 6e61 6d65 5f62 6c6f 636b  sible_name_block
+00000770: 7175 6f74 6522 3a20 22ce 9cce bfcf 81cf  quote": ".......
+00000780: 86ce ae20 ceba ceb5 ceb9 cebc cead cebd  ... ............
+00000790: cebf cf85 20cf 80ce b1cf 81ce acce b8ce  .... ...........
+000007a0: b5cf 83ce b7cf 8222 2c0a 0a20 2020 2022  .......",..    "
+000007b0: 746f 6f6c 735f 6163 7469 6f6e 735f 6169  tools_actions_ai
+000007c0: 5f61 7373 6973 7461 6e74 223a 2022 ce92  _assistant": "..
+000007d0: cebf ceb7 ceb8 cf8c cf82 2041 4922 2c0a  .......... AI",.
+000007e0: 2020 2020 2274 6f6f 6c73 5f61 6374 696f      "tools_actio
+000007f0: 6e73 5f61 6363 6573 7369 626c 655f 6e61  ns_accessible_na
+00000800: 6d65 5f61 695f 6173 7369 7374 616e 7422  me_ai_assistant"
+00000810: 3a20 22ce 95ce bace bace afce bdce b7cf  : ".............
+00000820: 83ce b720 ce92 cebf ceb7 ceb8 cebf cf8d  ... ............
+00000830: 2041 4922 2c0a 2020 2020 2274 6f6f 6c73   AI",.    "tools
+00000840: 5f61 6374 696f 6e73 5f63 6f6c 6f72 5f70  _actions_color_p
+00000850: 6963 6b65 7222 3a20 22ce 95cf 80ce b9ce  icker": ".......
+00000860: bbce bfce b3ce adce b1cf 8220 cf87 cf81  ........... ....
+00000870: cf8e cebc ceb1 cf84 cebf cf82 222c 0a20  ............",. 
+00000880: 2020 2022 746f 6f6c 735f 6163 7469 6f6e     "tools_action
+00000890: 735f 6163 6365 7373 6962 6c65 5f6e 616d  s_accessible_nam
+000008a0: 655f 636f 6c6f 725f 7069 636b 6572 223a  e_color_picker":
+000008b0: 2022 ce95 cf80 ceb9 cebb cead cebe cf84   "..............
+000008c0: ceb5 20cf 87cf 81cf 8ece bcce b120 ceba  .. .......... ..
+000008d0: ceb5 ceb9 cebc cead cebd cebf cf85 222c  ..............",
+000008e0: 0a0a 2020 2020 2261 6374 696f 6e73 5f68  ..    "actions_h
+000008f0: 656c 705f 6c61 6265 6c5f 6d64 5f73 796e  elp_label_md_syn
+00000900: 7461 7822 3a20 22ce a3cf 8dce bdcf 84ce  tax": ".........
+00000910: b1ce bece b720 4d61 726b 646f 776e 222c  ..... Markdown",
+00000920: 0a20 2020 2022 6163 7469 6f6e 735f 6865  .    "actions_he
+00000930: 6c70 5f61 6363 6573 7369 626c 655f 6e61  lp_accessible_na
+00000940: 6d65 5f6d 645f 7379 6e74 6178 223a 2022  me_md_syntax": "
+00000950: cea3 cf8d cebd cf84 ceb1 cebe ceb7 204d  .............. M
+00000960: 6172 6b64 6f77 6e22 2c0a 2020 2020 2261  arkdown",.    "a
+00000970: 6374 696f 6e73 5f68 656c 705f 6c61 6265  ctions_help_labe
+00000980: 6c5f 6368 6563 6b5f 666f 725f 7570 6461  l_check_for_upda
+00000990: 7465 7322 3a20 22ce 88ce bbce b5ce b3cf  tes": ".........
+000009a0: 87ce bfcf 8220 ceb3 ceb9 ceb1 20ce b5ce  ..... ...... ...
+000009b0: bdce b7ce bcce b5cf 81cf 8ecf 83ce b5ce  ................
+000009c0: b9cf 8222 2c0a 2020 2020 2261 6374 696f  ...",.    "actio
+000009d0: 6e73 5f68 656c 705f 6163 6365 7373 6962  ns_help_accessib
+000009e0: 6c65 5f6e 616d 655f 6368 6563 6b5f 666f  le_name_check_fo
+000009f0: 725f 7570 6461 7465 7322 3a20 22ce 88ce  r_updates": "...
+00000a00: bbce b5ce b3cf 87ce bfcf 8220 ceb3 ceb9  ........... ....
+00000a10: ceb1 20ce b5ce bdce b7ce bcce b5cf 81cf  .. .............
+00000a20: 8ecf 83ce b5ce b9cf 8222 2c0a 2020 2020  .........",.    
+00000a30: 2261 6374 696f 6e73 5f68 656c 705f 6c61  "actions_help_la
+00000a40: 6265 6c5f 6275 675f 7265 706f 7274 223a  bel_bug_report":
+00000a50: 2022 ce91 cebd ceb1 cf86 cebf cf81 ceac   "..............
+00000a60: 20cf 83cf 86ce b1ce bbce bcce accf 84cf   ...............
+00000a70: 89ce bd22 2c0a 2020 2020 2261 6374 696f  ...",.    "actio
+00000a80: 6e73 5f68 656c 705f 6163 6365 7373 6962  ns_help_accessib
+00000a90: 6c65 5f6e 616d 655f 6275 675f 7265 706f  le_name_bug_repo
+00000aa0: 7274 223a 2022 cea5 cf80 cebf ceb2 cebf  rt": "..........
+00000ab0: cebb ceae 20ce b1ce bdce b1cf 86ce bfcf  .... ...........
+00000ac0: 81ce accf 8220 cf83 cf86 ceac cebb cebc  ..... ..........
+00000ad0: ceb1 cf84 cebf cf82 222c 0a20 2020 2022  ........",.    "
+00000ae0: 6163 7469 6f6e 735f 6865 6c70 5f6c 6162  actions_help_lab
+00000af0: 656c 5f61 626f 7574 223a 2022 cea0 cebb  el_about": "....
+00000b00: ceb7 cf81 cebf cf86 cebf cf81 ceaf ceb5  ................
+00000b10: cf82 222c 0a20 2020 2022 6163 7469 6f6e  ..",.    "action
+00000b20: 735f 6865 6c70 5f61 6363 6573 7369 626c  s_help_accessibl
+00000b30: 655f 6e61 6d65 5f61 626f 7574 223a 2022  e_name_about": "
+00000b40: cea0 cebb ceb7 cf81 cebf cf86 cebf cf81  ................
+00000b50: ceaf ceb5 cf82 222c 0a7d 0a              ......",.}.
```

### Comparing `notolog-0.9.1b1/app/lexemes/gr/ai_assistant.py` & `notolog-0.9.1b2/notolog/lexemes/gr/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/gr/color_picker_dialog.py` & `notolog-0.9.1b2/notolog/lexemes/gr/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/gr/common.py` & `notolog-0.9.1b2/notolog/lexemes/gr/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     "save_active_file_error_occurred": "Αδυναμία αποθήκευσης αρχείου, συνέβη σφάλμα",
 
     "expandable_block_default_title": "Περισσότερες πληροφορίες...",
 
     "dialog_color_picker_color_copied_to_the_clipboard": "Το μορφοποιημένο κείμενο έχει αντιγραφεί στο πρόχειρο",
 
     "popup_about_title": "Πληροφορίες Εφαρμογής",
-    "popup_about_app_name_description": "Επεξεργαστής Markdown",
+    "popup_about_app_name_description": "Επεξεργαστής Markdown της Python",
 
     "popup_about_version": "Έκδοση",
     "popup_about_license": "Άδεια",
     "popup_about_website": "Ιστοσελίδα",
     "popup_about_repository": "GitHub",
     "popup_about_pypi": "PyPi",
     "popup_about_date": "Ημερομηνία",
```

### Comparing `notolog-0.9.1b1/app/lexemes/gr/main_menu.py` & `notolog-0.9.1b2/notolog/lexemes/ko/main_menu.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-# Greek lexemes main_menu.py
+# Korean lexemes main_menu.py
 lexemes = {
-    "group_file_label": "Αρχείο",
-    "group_edit_label": "Επεξεργασία",
-    "group_tools_label": "Εργαλεία",
-    "group_help_label": "Βοήθεια",
+    "group_file_label": "파일",
+    "group_edit_label": "편집",
+    "group_tools_label": "도구",
+    "group_help_label": "도움말",
 
-    "actions_file_label_new_document": "Νέο έγγραφο",
-    "actions_file_accessible_name_new_document": "Νέο έγγραφο",
-    "actions_file_label_open": "Άνοιγμα",
-    "actions_file_accessible_name_open": "Άνοιγμα εγγράφου",
-    "actions_file_label_save": "Αποθήκευση",
-    "actions_file_accessible_name_save": "Αποθήκευση εγγράφου",
-    "actions_file_label_save_as": "Αποθήκευση ως",
-    "actions_file_accessible_name_save_as": "Αποθήκευση ως αντίγραφο εγγράφου",
-    "actions_file_label_exit": "Έξοδος",
-    "actions_file_accessible_name_exit": "Έξοδος από την εφαρμογή",
+    "actions_file_label_new_document": "새 문서",
+    "actions_file_accessible_name_new_document": "새 문서",
+    "actions_file_label_open": "열기",
+    "actions_file_accessible_name_open": "문서 열기",
+    "actions_file_label_save": "저장",
+    "actions_file_accessible_name_save": "문서 저장",
+    "actions_file_label_save_as": "다른 이름으로 저장",
+    "actions_file_accessible_name_save_as": "문서 복사본 저장",
+    "actions_file_label_exit": "종료",
+    "actions_file_accessible_name_exit": "앱 종료",
 
-    "edit_actions_edit_mode": "Επεξεργασία",
-    "edit_actions_accessible_name_edit_mode": "Επεξεργασία αρχείου",
-    "edit_actions_source_mode": "Πηγαίος κώδικας",
-    "edit_actions_accessible_name_source_mode": "Πηγαίος κώδικας",
-    "edit_actions_bold": "Έντονα",
-    "edit_actions_accessible_name_bold": "Μορφή έντονου κειμένου",
-    "edit_actions_italic": "Πλάγια",
-    "edit_actions_accessible_name_italic": "Μορφή πλάγιου κειμένου",
-    "edit_actions_underline": "Υπογράμμιση",
-    "edit_actions_accessible_name_underline": "Μορφή υπογεγραμμένου κειμένου",
-    "edit_actions_strikethrough": "Διαγραμμίσεις",
-    "edit_actions_accessible_name_strikethrough": "Μορφή διαγραμμισμένου κειμένου",
-    "edit_actions_blockquote": "Παράθεση",
-    "edit_actions_accessible_name_blockquote": "Μορφή κειμένου παράθεσης",
+    "edit_actions_edit_mode": "편집",
+    "edit_actions_accessible_name_edit_mode": "파일 편집",
+    "edit_actions_source_mode": "소스",
+    "edit_actions_accessible_name_source_mode": "소스 코드",
+    "edit_actions_bold": "굵게",
+    "edit_actions_accessible_name_bold": "굵은 텍스트 형식",
+    "edit_actions_italic": "기울임꼴",
+    "edit_actions_accessible_name_italic": "기울임꼴 텍스트 형식",
+    "edit_actions_underline": "밑줄",
+    "edit_actions_accessible_name_underline": "밑줄 텍스트 형식",
+    "edit_actions_strikethrough": "취소선",
+    "edit_actions_accessible_name_strikethrough": "취소선 텍스트 형식",
+    "edit_actions_blockquote": "블록 인용",
+    "edit_actions_accessible_name_blockquote": "블록 인용 텍스트 형식",
 
-    "tools_actions_ai_assistant": "Βοηθός AI",
-    "tools_actions_accessible_name_ai_assistant": "Εκκίνηση Βοηθού AI",
-    "tools_actions_color_picker": "Επιλογέας χρώματος",
-    "tools_actions_accessible_name_color_picker": "Επιλέξτε χρώμα κειμένου",
+    "tools_actions_ai_assistant": "AI 보조",
+    "tools_actions_accessible_name_ai_assistant": "AI 보조 시작",
+    "tools_actions_color_picker": "색상 선택기",
+    "tools_actions_accessible_name_color_picker": "텍스트 색상 선택",
 
-    "actions_help_label_md_syntax": "Σύνταξη Markdown",
-    "actions_help_accessible_name_md_syntax": "Σύνταξη Markdown",
-    "actions_help_label_check_for_updates": "Έλεγχος για ενημερώσεις",
-    "actions_help_accessible_name_check_for_updates": "Έλεγχος για ενημερώσεις",
-    "actions_help_label_bug_report": "Αναφορά σφαλμάτων",
-    "actions_help_accessible_name_bug_report": "Υποβολή αναφοράς σφάλματος",
-    "actions_help_label_about": "Πληροφορίες",
-    "actions_help_accessible_name_about": "Πληροφορίες",
+    "actions_help_label_md_syntax": "Markdown 문법",
+    "actions_help_accessible_name_md_syntax": "Markdown 문법",
+    "actions_help_label_check_for_updates": "업데이트 확인",
+    "actions_help_accessible_name_check_for_updates": "업데이트 확인",
+    "actions_help_label_bug_report": "버그 보고",
+    "actions_help_accessible_name_bug_report": "버그 보고서 제출",
+    "actions_help_label_about": "정보",
+    "actions_help_accessible_name_about": "정보",
 }
```

### Comparing `notolog-0.9.1b1/app/lexemes/gr/settings_dialog.py` & `notolog-0.9.1b2/notolog/lexemes/gr/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/gr/statusbar.py` & `notolog-0.9.1b2/notolog/lexemes/gr/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/gr/toolbar.py` & `notolog-0.9.1b2/notolog/lexemes/gr/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/in/__pycache__/common.cpython-39.pyc` & `notolog-0.9.1b2/notolog/lexemes/in/common.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,589 +1,630 @@
-00000000: 610d 0d0a 0000 0000 42a9 3566 4e27 0000  a.......B.5fN'..
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0055 0000 0040 0000 0073 b200 0000 6400  .U...@...s....d.
-00000030: 6401 6402 6403 6404 6405 6406 6407 6408  d.d.d.d.d.d.d.d.
-00000040: 6403 6409 640a 640b 640c 640d 640e 640f  d.d.d.d.d.d.d.d.
-00000050: 6410 6411 6412 6413 6414 6415 6416 6417  d.d.d.d.d.d.d.d.
-00000060: 6418 6419 641a 641b 641c 641d 641e 641f  d.d.d.d.d.d.d.d.
-00000070: 6420 6421 6422 641e 641f 6423 6424 6425  d d!d"d.d.d#d$d%
-00000080: 6426 6427 6428 6429 642a 642b 642c 642b  d&d'd(d)d*d+d,d+
-00000090: 642d 642e 6424 642e 6426 6429 642a 642f  d-d.d$d.d&d)d*d/
-000000a0: 6430 642a 6431 6432 6433 6434 6435 6436  d0d*d1d2d3d4d5d6
-000000b0: 6437 6438 6439 643a 643b 643c 643d 643e  d7d8d9d:d;d<d=d>
-000000c0: 643f 6440 6441 6442 6443 6444 6445 6446  d?d@dAdBdCdDdEdF
-000000d0: 6447 6448 6449 644a 9c54 5a00 644b 5300  dGdHdIdJ.TZ.dKS.
-000000e0: 294c 7525 0000 00e0 a4a8 e0a5 8be0 a49f  )Lu%............
-000000f0: e0a5 8be0 a4b2 e0a5 89e0 a497 20e0 a48f  ............ ...
-00000100: e0a4 a1e0 a4bf e0a4 9fe0 a4b0 7a19 7b61  ............z.{a
-00000110: 7070 5f74 6974 6c65 7d20 2d20 7b73 7562  pp_title} - {sub
-00000120: 5f74 6974 6c65 7d75 3800 0000 e0a4 abe0  _title}u8.......
-00000130: a4bc e0a4 bee0 a487 e0a4 b220 e0a4 abe0  ........... ....
-00000140: a4bc e0a4 bfe0 a4b2 e0a5 8de0 a49f e0a4  ................
-00000150: b020 e0a4 abe0 a4bc e0a5 80e0 a4b2 e0a5  . ..............
-00000160: 8de0 a4a1 7519 0000 00e0 a4a8 e0a4 bee0  ....u...........
-00000170: a4ae 20e0 a4ac e0a4 a6e0 a4b2 e0a5 87e0  .. .............
-00000180: a482 750f 0000 00e0 a4b9 e0a4 9fe0 a4be  ..u.............
-00000190: e0a4 8fe0 a482 752d 0000 00e0 a4aa e0a5  ......u-........
-000001a0: 82e0 a4b0 e0a5 8020 e0a4 a4e0 a4b0 e0a4  ....... ........
-000001b0: b920 e0a4 b8e0 a587 20e0 a4b9 e0a4 9fe0  . ...... .......
-000001c0: a4be e0a4 8fe0 a482 7531 0000 00e0 a4aa  ........u1......
-000001d0: e0a5 81e0 a4a8 e0a4 b0e0 a58d e0a4 b8e0  ................
-000001e0: a58d e0a4 a5e0 a4be e0a4 aae0 a4bf e0a4  ................
-000001f0: a420 e0a4 95e0 a4b0 e0a5 87e0 a482 7530  . ............u0
-00000200: 0000 00e0 a4ab e0a4 bce0 a4be e0a4 87e0  ................
-00000210: a4b2 20e0 a495 e0a4 be20 e0a4 a8e0 a4be  .. ...... ......
-00000220: e0a4 ae20 e0a4 ace0 a4a6 e0a4 b2e0 a587  ... ............
-00000230: e0a4 8275 3d00 0000 e0a4 a8e0 a4af e0a4  ...u=...........
-00000240: be20 e0a4 abe0 a4bc e0a4 bee0 a487 e0a4  . ..............
-00000250: b220 e0a4 a8e0 a4be e0a4 ae20 e0a4 a6e0  . ......... ....
-00000260: a4b0 e0a5 8de0 a49c 20e0 a495 e0a4 b0e0  ........ .......
-00000270: a587 e0a4 8275 5500 0000 e0a4 87e0 a4b8  .....uU.........
-00000280: e0a5 8020 e0a4 a8e0 a4be e0a4 ae20 e0a4  ... ......... ..
-00000290: 95e0 a580 20e0 a4ab e0a4 bce0 a4be e0a4  .... ...........
-000002a0: 87e0 a4b2 20e0 a4aa e0a4 b9e0 a4b2 e0a5  .... ...........
-000002b0: 8720 e0a4 b8e0 a587 20e0 a4ae e0a5 8ce0  . ...... .......
-000002c0: a49c e0a5 82e0 a4a6 20e0 a4b9 e0a5 8875  ........ ......u
-000002d0: 1f00 0000 e0a4 abe0 a4bc e0a4 bee0 a487  ................
-000002e0: e0a4 b220 e0a4 b9e0 a49f e0a4 bee0 a48f  ... ............
-000002f0: e0a4 8275 7000 0000 e0a4 95e0 a58d e0a4  ...up...........
-00000300: afe0 a4be 20e0 a486 e0a4 aa20 e0a4 b5e0  .... ...... ....
-00000310: a4be e0a4 95e0 a488 20e0 a4ab e0a4 bce0  ........ .......
-00000320: a4be e0a4 87e0 a4b2 2022 7b66 696c 655f  ........ "{file_
-00000330: 6e61 6d65 7d22 20e0 a495 e0a5 8b20 e0a4  name}" ...... ..
-00000340: b9e0 a49f e0a4 bee0 a4a8 e0a4 be20 e0a4  ............. ..
-00000350: 9ae0 a4be e0a4 b9e0 a4a4 e0a5 8720 e0a4  ............. ..
-00000360: b9e0 a588 e0a4 823f 7544 0000 00e0 a4ab  .......?uD......
-00000370: e0a4 bce0 a4be e0a4 87e0 a4b2 20e0 a495  ............ ...
-00000380: e0a5 8b20 e0a4 aae0 a582 e0a4 b0e0 a580  ... ............
-00000390: 20e0 a4a4 e0a4 b0e0 a4b9 20e0 a4b8 e0a5   ......... .....
-000003a0: 8720 e0a4 b9e0 a49f e0a4 bee0 a48f e0a4  . ..............
-000003b0: 8275 8e00 0000 e0a4 95e0 a58d e0a4 afe0  .u..............
-000003c0: a4be 20e0 a486 e0a4 aa20 e0a4 b5e0 a4be  .. ...... ......
-000003d0: e0a4 95e0 a488 20e0 a4ab e0a4 bce0 a4be  ...... .........
-000003e0: e0a4 87e0 a4b2 2022 7b66 696c 655f 6e61  ...... "{file_na
-000003f0: 6d65 7d22 20e0 a495 e0a5 8b20 e0a4 aae0  me}" ...... ....
-00000400: a582 e0a4 b0e0 a580 20e0 a4a4 e0a4 b0e0  ........ .......
-00000410: a4b9 20e0 a4b8 e0a5 8720 e0a4 b9e0 a49f  .. ...... ......
-00000420: e0a4 bee0 a4a8 e0a4 be20 e0a4 9ae0 a4be  ......... ......
-00000430: e0a4 b9e0 a4a4 e0a5 8720 e0a4 b9e0 a588  ......... ......
-00000440: e0a4 823f 7561 0000 00e0 a4ab e0a4 bce0  ...?ua..........
-00000450: a4be e0a4 87e0 a4b2 20e0 a4b9 e0a4 9fe0  ........ .......
-00000460: a4be e0a4 a8e0 a587 20e0 a4ae e0a5 87e0  ........ .......
-00000470: a482 20e0 a485 e0a4 b8e0 a4ae e0a4 b0e0  .. .............
-00000480: a58d e0a4 a52c 20e0 a4a4 e0a5 8de0 a4b0  ....., .........
-00000490: e0a5 81e0 a49f e0a4 bf20 e0a4 b9e0 a581  ......... ......
-000004a0: e0a4 8820 e0a4 b9e0 a588 7529 0000 00e0  ... ......u)....
-000004b0: a4ab e0a4 bce0 a4be e0a4 87e0 a4b2 20e0  .............. .
-000004c0: a4a8 e0a4 b9e0 a580 e0a4 8220 e0a4 aee0  ........... ....
-000004d0: a4bf e0a4 b2e0 a580 7541 0000 00e0 a4ab  ........uA......
-000004e0: e0a4 bce0 a4be e0a4 87e0 a4b2 20e0 a4aa  ............ ...
-000004f0: e0a5 81e0 a4a8 e0a4 b0e0 a58d e0a4 b8e0  ................
-00000500: a58d e0a4 a5e0 a4be e0a4 aae0 a4bf e0a4  ................
-00000510: a420 e0a4 95e0 a4b0 e0a5 87e0 a482 7592  . ............u.
-00000520: 0000 00e0 a495 e0a5 8de0 a4af e0a4 be20  ............... 
-00000530: e0a4 86e0 a4aa 20e0 a4b5 e0a4 bee0 a495  ...... .........
-00000540: e0a4 8820 e0a4 abe0 a4bc e0a4 bee0 a487  ... ............
-00000550: e0a4 b220 227b 6669 6c65 5f6e 616d 657d  ... "{file_name}
-00000560: 2220 e0a4 95e0 a58b 20e0 a4aa e0a5 81e0  " ...... .......
-00000570: a4a8 e0a4 b0e0 a58d e0a4 b8e0 a58d e0a4  ................
-00000580: a5e0 a4be e0a4 aae0 a4bf e0a4 a420 e0a4  ............. ..
-00000590: 95e0 a4b0 e0a4 a8e0 a4be 20e0 a49a e0a4  .......... .....
-000005a0: bee0 a4b9 e0a4 a4e0 a587 20e0 a4b9 e0a5  .......... .....
-000005b0: 88e0 a482 3f75 8a00 0000 e0a4 abe0 a4bc  ....?u..........
-000005c0: e0a4 bee0 a487 e0a4 b220 e0a4 95e0 a58b  ......... ......
-000005d0: 20e0 a4aa e0a5 81e0 a4a8 e0a4 b0e0 a58d   ...............
-000005e0: e0a4 b8e0 a58d e0a4 a5e0 a4be e0a4 aae0  ................
-000005f0: a4bf e0a4 a420 e0a4 95e0 a4b0 e0a4 a8e0  ..... ..........
-00000600: a587 20e0 a4ae e0a5 87e0 a482 20e0 a485  .. ......... ...
-00000610: e0a4 b8e0 a4ae e0a4 b0e0 a58d e0a4 a52c  ...............,
-00000620: 20e0 a4a4 e0a5 8de0 a4b0 e0a5 81e0 a49f   ...............
-00000630: e0a4 bf20 e0a4 b9e0 a581 e0a4 8820 e0a4  ... ......... ..
-00000640: b9e0 a588 7552 0000 00e0 a487 e0a4 b820  ....uR......... 
-00000650: e0a4 a8e0 a4be e0a4 ae20 e0a4 95e0 a580  ......... ......
-00000660: 20e0 a4ab e0a4 bce0 a4be e0a4 87e0 a4b2   ...............
-00000670: 20e0 a4aa e0a4 b9e0 a4b2 e0a5 8720 e0a4   ............ ..
-00000680: b8e0 a587 20e0 a4ae e0a5 8ce0 a49c e0a5  .... ...........
-00000690: 82e0 a4a6 20e0 a4b9 e0a5 8875 0f00 0000  .... ......u....
-000006a0: e0a4 b8e0 a482 e0a4 a6e0 a587 e0a4 b675  ...............u
-000006b0: 1600 0000 e0a4 ace0 a482 e0a4 a620 e0a4  ............. ..
-000006c0: 95e0 a4b0 e0a5 87e0 a482 7525 0000 00e0  ..........u%....
-000006d0: a4a8 e0a4 afe0 a4be 20e0 a4a6 e0a4 b8e0  ........ .......
-000006e0: a58d e0a4 a4e0 a4be e0a4 b5e0 a587 e0a4  ................
-000006f0: 9ce0 a4bc 751f 0000 00e0 a4ab e0a4 bce0  ....u...........
-00000700: a4be e0a4 87e0 a4b2 20e0 a496 e0a5 8be0  ........ .......
-00000710: a4b2 e0a5 87e0 a482 7522 0000 00e0 a4ab  ........u"......
-00000720: e0a4 bce0 a4be e0a4 87e0 a4b2 20e0 a4b8  ............ ...
-00000730: e0a4 b9e0 a587 e0a4 9ce0 a587 e0a4 8275  ...............u
-00000740: 2f00 0000 e0a4 96e0 a4be e0a4 b2e0 a580  /...............
-00000750: 20e0 a4ab e0a4 bce0 a4be e0a4 87e0 a4b2   ...............
-00000760: 20e0 a4b8 e0a4 b9e0 a587 e0a4 9ce0 a587   ...............
-00000770: e0a4 8275 8f00 0000 e0a4 95e0 a58d e0a4  ...u............
-00000780: afe0 a4be 20e0 a496 e0a4 bee0 a4b2 e0a5  .... ...........
-00000790: 8020 e0a4 b8e0 a4be e0a4 aee0 a497 e0a5  . ..............
-000007a0: 8de0 a4b0 e0a5 8020 e0a4 95e0 a587 20e0  ....... ...... .
-000007b0: a4b8 e0a4 bee0 a4a5 20e0 a4ab e0a4 bce0  ........ .......
-000007c0: a4be e0a4 87e0 a4b2 20e0 a495 e0a5 8b20  ........ ...... 
-000007d0: e0a4 b8e0 a4b9 e0a5 87e0 a49c e0a4 a8e0  ................
-000007e0: a587 20e0 a495 e0a5 8020 e0a4 85e0 a4a8  .. ...... ......
-000007f0: e0a5 81e0 a4ae e0a4 a4e0 a4bf 20e0 a4a6  ............ ...
-00000800: e0a5 87e0 a482 3f75 3b00 0000 e0a4 abe0  ......?u;.......
-00000810: a4bc e0a4 bee0 a487 e0a4 b220 e0a4 8fe0  ........... ....
-00000820: a4a8 e0a5 8de0 a495 e0a5 8de0 a4b0 e0a4  ................
-00000830: bfe0 a4aa e0a5 8de0 a49f 20e0 a495 e0a4  .......... .....
-00000840: b0e0 a587 e0a4 8275 8c00 0000 e0a4 95e0  .......u........
-00000850: a58d e0a4 afe0 a4be 20e0 a486 e0a4 aa20  ........ ...... 
-00000860: e0a4 b5e0 a4be e0a4 95e0 a488 20e0 a4ab  ............ ...
-00000870: e0a4 bce0 a4be e0a4 87e0 a4b2 2022 7b66  ............ "{f
-00000880: 696c 655f 6e61 6d65 7d22 20e0 a495 e0a5  ile_name}" .....
-00000890: 8b20 e0a4 8fe0 a4a8 e0a5 8de0 a495 e0a5  . ..............
-000008a0: 8de0 a4b0 e0a4 bfe0 a4aa e0a5 8de0 a49f  ................
-000008b0: 20e0 a495 e0a4 b0e0 a4a8 e0a4 be20 e0a4   ............ ..
-000008c0: 9ae0 a4be e0a4 b9e0 a4a4 e0a5 8720 e0a4  ............. ..
-000008d0: b9e0 a588 e0a4 823f 7557 0000 00e0 a4ab  .......?uW......
-000008e0: e0a4 bce0 a4be e0a4 87e0 a4b2 20e0 a4aa  ............ ...
-000008f0: e0a4 b9e0 a4b2 e0a5 8720 e0a4 b8e0 a587  ......... ......
-00000900: 20e0 a4b9 e0a5 8020 e0a4 8fe0 a4a8 e0a5   ...... ........
-00000910: 8de0 a495 e0a5 8de0 a4b0 e0a4 bfe0 a4aa  ................
-00000920: e0a5 8de0 a49f e0a5 87e0 a4a1 20e0 a4b9  ............ ...
-00000930: e0a5 8821 7546 0000 00e0 a4ae e0a5 8ce0  ...!uF..........
-00000940: a49c e0a5 82e0 a4a6 e0a4 be20 e0a4 abe0  ........... ....
-00000950: a4bc e0a4 bee0 a487 e0a4 b220 e0a4 95e0  ........... ....
-00000960: a58b 20e0 a4aa e0a5 81e0 a4a8 e0a4 8320  .. ............ 
-00000970: e0a4 b2e0 a4bf e0a4 96e0 a587 e0a4 8275  ...............u
-00000980: 9000 0000 e0a4 95e0 a58d e0a4 afe0 a4be  ................
-00000990: 20e0 a486 e0a4 aa20 e0a4 b5e0 a4be e0a4   ...... ........
-000009a0: 95e0 a488 20e0 a4ae e0a5 8ce0 a49c e0a5  .... ...........
-000009b0: 82e0 a4a6 e0a4 be20 e0a4 abe0 a4bc e0a4  ....... ........
-000009c0: bee0 a487 e0a4 b220 227b 6669 6c65 5f70  ....... "{file_p
-000009d0: 6174 687d 2220 e0a4 95e0 a58b 20e0 a4aa  ath}" ...... ...
-000009e0: e0a5 81e0 a4a8 e0a4 8320 e0a4 b2e0 a4bf  ......... ......
-000009f0: e0a4 96e0 a4a8 e0a4 be20 e0a4 9ae0 a4be  ......... ......
-00000a00: e0a4 b9e0 a4a4 e0a5 8720 e0a4 b9e0 a588  ......... ......
-00000a10: e0a4 823f 7538 0000 00e0 a4ab e0a4 bce0  ...?u8..........
-00000a20: a4be e0a4 87e0 a4b2 20e0 a4a1 e0a4 bfe0  ........ .......
-00000a30: a495 e0a5 8de0 a4b0 e0a4 bfe0 a4aa e0a5  ................
-00000a40: 8de0 a49f 20e0 a495 e0a4 b0e0 a587 e0a4  .... ...........
-00000a50: 8275 8900 0000 e0a4 95e0 a58d e0a4 afe0  .u..............
-00000a60: a4be 20e0 a486 e0a4 aa20 e0a4 b5e0 a4be  .. ...... ......
-00000a70: e0a4 95e0 a488 20e0 a4ab e0a4 bce0 a4be  ...... .........
-00000a80: e0a4 87e0 a4b2 2022 7b66 696c 655f 6e61  ...... "{file_na
-00000a90: 6d65 7d22 20e0 a495 e0a5 8b20 e0a4 a1e0  me}" ...... ....
-00000aa0: a4bf e0a4 95e0 a58d e0a4 b0e0 a4bf e0a4  ................
-00000ab0: aae0 a58d e0a4 9f20 e0a4 95e0 a4b0 e0a4  ....... ........
-00000ac0: a8e0 a4be 20e0 a49a e0a4 bee0 a4b9 e0a4  .... ...........
-00000ad0: a4e0 a587 20e0 a4b9 e0a5 88e0 a482 3f75  .... .........?u
-00000ae0: 4900 0000 e0a4 abe0 a4bc e0a4 bee0 a487  I...............
-00000af0: e0a4 b220 e0a4 8fe0 a4a8 e0a5 8de0 a495  ... ............
-00000b00: e0a5 8de0 a4b0 e0a4 bfe0 a4aa e0a5 8de0  ................
-00000b10: a49f e0a5 87e0 a4a1 20e0 a4a8 e0a4 b9e0  ........ .......
-00000b20: a580 e0a4 8220 e0a4 b9e0 a588 2175 1f00  ..... ......!u..
-00000b30: 0000 e0a4 a8e0 a4af e0a4 be20 e0a4 aae0  ........... ....
-00000b40: a4be e0a4 b8e0 a4b5 e0a4 b0e0 a58d e0a4  ................
-00000b50: a175 1600 0000 e0a4 aae0 a4be e0a4 b8e0  .u..............
-00000b60: a4b5 e0a4 b0e0 a58d e0a4 a13a 7539 0000  ...........:u9..
-00000b70: 00e0 a4a8 e0a4 afe0 a4be 20e0 a4aa e0a4  .......... .....
-00000b80: bee0 a4b8 e0a4 b5e0 a4b0 e0a5 8de0 a4a1  ................
-00000b90: 20e0 a4a6 e0a4 b0e0 a58d e0a4 9c20 e0a4   ............ ..
-00000ba0: 95e0 a4b0 e0a5 87e0 a482 7510 0000 00e0  ..........u.....
-00000bb0: a4b8 e0a4 82e0 a495 e0a5 87e0 a4a4 3a75  ..............:u
-00000bc0: 3402 0000 e0a4 b8e0 a482 e0a4 95e0 a587  4...............
-00000bd0: e0a4 a420 e0a4 8fe0 a4a8 e0a5 8de0 a495  ... ............
-00000be0: e0a5 8de0 a4b0 e0a4 bfe0 a4aa e0a5 8de0  ................
-00000bf0: a49f e0a5 87e0 a4a1 20e0 a4a8 e0a4 b9e0  ........ .......
-00000c00: a580 e0a4 8220 e0a4 b9e0 a58b e0a4 a4e0  ..... ..........
-00000c10: a4be 20e0 a4b9 e0a5 8820 e0a4 94e0 a4b0  .. ...... ......
-00000c20: 20e0 a4ab e0a4 bce0 a4be e0a4 87e0 a4b2   ...............
-00000c30: 20e0 a4b8 e0a5 8720 e0a4 aae0 a4a2 e0a4   ...... ........
-00000c40: bce0 a4be 20e0 a49c e0a4 be20 e0a4 b8e0  .... ...... ....
-00000c50: a495 e0a4 a4e0 a4be 20e0 a4b9 e0a5 8821  ........ ......!
-00000c60: 0ae0 a49c e0a4 a8e0 a58d e0a4 ae20 e0a4  ............. ..
-00000c70: a4e0 a4bf e0a4 a5e0 a4bf e0a4 afe0 a58b  ................
-00000c80: e0a4 8220 e0a4 9ce0 a588 e0a4 b8e0 a587  ... ............
-00000c90: 20e0 a486 e0a4 b8e0 a4be e0a4 a8e0 a580   ...............
-00000ca0: 20e0 a4b8 e0a5 8720 e0a4 85e0 a4a8 e0a5   ...... ........
-00000cb0: 81e0 a4ae e0a4 bee0 a4a8 20e0 a4b2 e0a4  .......... .....
-00000cc0: 97e0 a4be e0a4 8f20 e0a4 9ce0 a4be 20e0  ....... ...... .
-00000cd0: a4b8 e0a4 95e0 a4a8 e0a5 8720 e0a4 b5e0  ........... ....
-00000ce0: a4be e0a4 b2e0 a587 20e0 a4b8 e0a5 8de0  ........ .......
-00000cf0: a4aa e0a4 b7e0 a58d e0a4 9f20 e0a4 b8e0  ........... ....
-00000d00: a482 e0a4 95e0 a587 e0a4 a4e0 a58b e0a4  ................
-00000d10: 8220 e0a4 b8e0 a587 20e0 a4ac e0a4 9ae0  . ...... .......
-00000d20: a587 e0a4 82e0 a5a4 0ae0 a486 e0a4 aae0  ................
-00000d30: a495 e0a5 8720 e0a4 b8e0 a4be e0a4 a520  ..... ......... 
-00000d40: e0a4 86e0 a4b8 e0a4 bee0 a4a8 e0a5 8020  ............... 
-00000d50: e0a4 b8e0 a587 20e0 a49c e0a5 81e0 a4a1  ...... .........
-00000d60: e0a4 bce0 a587 20e0 a4a8 e0a4 b9e0 a580  ...... .........
-00000d70: e0a4 8220 e0a4 9ce0 a4be 20e0 a4b8 e0a4  ... ...... .....
-00000d80: 95e0 a4a8 e0a5 8720 e0a4 b5e0 a4be e0a4  ....... ........
-00000d90: b2e0 a587 20e0 a4b8 e0a4 82e0 a4a6 e0a4  .... ...........
-00000da0: b0e0 a58d e0a4 ad20 e0a4 95e0 a4be 20e0  ....... ...... .
-00000db0: a4aa e0a5 8de0 a4b0 e0a4 afe0 a58b e0a4  ................
-00000dc0: 9720 e0a4 95e0 a4b0 e0a4 a8e0 a587 20e0  . ............ .
-00000dd0: a495 e0a4 be20 e0a4 aae0 a58d e0a4 b0e0  ..... ..........
-00000de0: a4af e0a4 bee0 a4b8 20e0 a495 e0a4 b0e0  ........ .......
-00000df0: a587 e0a4 82e0 a5a4 7544 0000 00e0 a4b8  ........uD......
-00000e00: e0a4 82e0 a495 e0a5 87e0 a4a4 20e0 a4a6  ............ ...
-00000e10: e0a4 b0e0 a58d e0a4 9c20 e0a4 95e0 a4b0  ......... ......
-00000e20: e0a5 87e0 a482 2028 e0a4 b5e0 a588 e0a4  ...... (........
-00000e30: 95e0 a4b2 e0a5 8de0 a4aa e0a4 bfe0 a495  ................
-00000e40: 2975 1000 0000 e0a4 a0e0 a580 e0a4 9520  )u............. 
-00000e50: e0a4 b9e0 a588 7519 0000 00e0 a4b0 e0a4  ......u.........
-00000e60: a6e0 a58d e0a4 a620 e0a4 95e0 a4b0 e0a5  ....... ........
-00000e70: 87e0 a482 7515 0000 00e0 a49a e0a5 87e0  ....u...........
-00000e80: a4a4 e0a4 bee0 a4b5 e0a4 a8e0 a580 7557  ..............uW
-00000e90: 0000 00e0 a4aa e0a4 bee0 a4b8 e0a4 b5e0  ................
-00000ea0: a4b0 e0a5 8de0 a4a1 20e0 a4ab e0a4 bce0  ........ .......
-00000eb0: a580 e0a4 b2e0 a58d e0a4 a120 e0a4 96e0  ........... ....
-00000ec0: a4be e0a4 b2e0 a580 20e0 a4a8 e0a4 b9e0  ........ .......
-00000ed0: a580 e0a4 8220 e0a4 b9e0 a58b 20e0 a4b8  ..... ...... ...
-00000ee0: e0a4 95e0 a4a4 e0a5 8021 7572 0000 00e0  .........!ur....
-00000ef0: a4b8 e0a4 82e0 a495 e0a5 87e0 a4a4 20e0  .............. .
-00000f00: a4ab e0a4 bce0 a580 e0a4 b2e0 a58d e0a4  ................
-00000f10: a120 e0a4 ace0 a4b9 e0a5 81e0 a4a4 20e0  . ............ .
-00000f20: a4b2 e0a4 82e0 a4ac e0a5 8020 e0a4 b9e0  ........... ....
-00000f30: a588 2c20 e0a4 85e0 a4a7 e0a4 bfe0 a495  .., ............
-00000f40: e0a4 a4e0 a4ae 207b 7379 6d62 6f6c 737d  ...... {symbols}
-00000f50: 20e0 a485 e0a4 95e0 a58d e0a4 b7e0 a4b0   ...............
-00000f60: 2175 2f00 0000 e0a4 aae0 a4be e0a4 b8e0  !u/.............
-00000f70: a4b5 e0a4 b0e0 a58d e0a4 a120 e0a4 a6e0  ........... ....
-00000f80: a4b0 e0a5 8de0 a49c 20e0 a495 e0a4 b0e0  ........ .......
-00000f90: a587 e0a4 8275 5400 0000 e0a4 8fe0 a4a8  .....uT.........
-00000fa0: e0a5 8de0 a495 e0a5 8de0 a4b0 e0a4 bfe0  ................
-00000fb0: a4aa e0a5 8de0 a4b6 e0a4 a820 e0a4 aae0  ........... ....
-00000fc0: a4be e0a4 b8e0 a4b5 e0a4 b0e0 a58d e0a4  ................
-00000fd0: a120 e0a4 b0e0 a580 e0a4 b8e0 a587 e0a4  . ..............
-00000fe0: 9f20 e0a4 95e0 a4b0 e0a5 87e0 a482 75aa  . ............u.
-00000ff0: 0000 00e0 a495 e0a5 8de0 a4af e0a4 be20  ............... 
-00001000: e0a4 86e0 a4aa 20e0 a4b5 e0a4 bee0 a495  ...... .........
-00001010: e0a4 8820 e0a4 aee0 a58c e0a4 9ce0 a582  ... ............
-00001020: e0a4 a6e0 a4be 20e0 a48f e0a4 a8e0 a58d  ...... .........
-00001030: e0a4 95e0 a58d e0a4 b0e0 a4bf e0a4 aae0  ................
-00001040: a58d e0a4 b6e0 a4a8 20e0 a4aa e0a4 bee0  ........ .......
-00001050: a4b8 e0a4 b5e0 a4b0 e0a5 8de0 a4a1 20e0  .............. .
-00001060: a495 e0a5 8b20 e0a4 b0e0 a580 e0a4 b8e0  ..... ..........
-00001070: a587 e0a4 9f20 e0a4 95e0 a4b0 e0a4 a8e0  ..... ..........
-00001080: a4be 20e0 a49a e0a4 bee0 a4b9 e0a4 a4e0  .. .............
-00001090: a587 20e0 a4b9 e0a5 88e0 a482 3f75 0900  .. .........?u..
-000010a0: 0000 e0a4 b9e0 a4be e0a4 8175 0c00 0000  ...........u....
-000010b0: e0a4 b2e0 a4bf e0a4 82e0 a495 754f 0000  ............uO..
-000010c0: 00e0 a4b2 e0a4 bfe0 a482 e0a4 9520 227b  ............. "{
-000010d0: 7572 6c7d 2220 e0a4 95e0 a58b 20e0 a4ac  url}" ...... ...
-000010e0: e0a5 8de0 a4b0 e0a4 bee0 a489 e0a4 9ce0  ................
-000010f0: a4bc e0a4 b020 e0a4 aee0 a587 e0a4 8220  ..... ......... 
-00001100: e0a4 96e0 a58b e0a4 b2e0 a587 e0a4 823f  ...............?
-00001110: 755c 0000 00e0 a48f e0a4 a8e0 a58d e0a4  u\..............
-00001120: 95e0 a58d e0a4 b0e0 a4bf e0a4 aae0 a58d  ................
-00001130: e0a4 b6e0 a4a8 20e0 a4aa e0a4 bee0 a4b8  ...... .........
-00001140: e0a4 b5e0 a4b0 e0a5 8de0 a4a1 20e0 a4ae  ............ ...
-00001150: e0a5 87e0 a4b2 20e0 a4a8 e0a4 b9e0 a580  ...... .........
-00001160: e0a4 8220 e0a4 96e0 a4be e0a4 a4e0 a4be  ... ............
-00001170: 2175 4900 0000 e0a4 8fe0 a4a8 e0a5 8de0  !uI.............
-00001180: a495 e0a5 8de0 a4b0 e0a4 bfe0 a4aa e0a5  ................
-00001190: 8de0 a4b6 e0a4 a820 e0a4 aae0 a4be e0a4  ....... ........
-000011a0: b8e0 a4b5 e0a4 b0e0 a58d e0a4 a120 e0a4  ............. ..
-000011b0: 97e0 a4b2 e0a4 a420 e0a4 b9e0 a588 2175  ....... ......!u
-000011c0: 4400 0000 e0a4 abe0 a4bc e0a4 bee0 a487  D...............
-000011d0: e0a4 b220 e0a4 b2e0 a58b e0a4 a120 e0a4  ... ......... ..
-000011e0: a8e0 a4b9 e0a5 80e0 a482 20e0 a495 e0a5  .......... .....
-000011f0: 8020 e0a4 9ce0 a4be 20e0 a4b8 e0a4 95e0  . ...... .......
-00001200: a4a4 e0a5 80e0 a5a4 7564 0000 00e0 a4ab  ........ud......
-00001210: e0a4 bce0 a4be e0a4 87e0 a4b2 20e0 a4b8  ............ ...
-00001220: e0a4 b9e0 a587 e0a4 9ce0 a4a8 e0a5 8720  ............... 
-00001230: e0a4 aee0 a587 e0a4 8220 e0a4 85e0 a4b8  ......... ......
-00001240: e0a4 aee0 a4b0 e0a5 8de0 a4a5 2c20 e0a4  ............, ..
-00001250: a4e0 a58d e0a4 b0e0 a581 e0a4 9fe0 a4bf  ................
-00001260: 20e0 a4b9 e0a5 81e0 a488 20e0 a4b9 e0a5   ......... .....
-00001270: 8875 2500 0000 e0a4 85e0 a4a7 e0a4 bfe0  .u%.............
-00001280: a495 20e0 a49c e0a4 bee0 a4a8 e0a4 95e0  .. .............
-00001290: a4be e0a4 b0e0 a580 2e2e 2e75 7600 0000  ...........uv...
-000012a0: e0a4 b8e0 a58d e0a4 b5e0 a4b0 e0a5 82e0  ................
-000012b0: a4aa e0a4 bfe0 a4a4 20e0 a4aa e0a4 bee0  ........ .......
-000012c0: a4a0 20e0 a495 e0a5 8de0 a4b2 e0a4 bfe0  .. .............
-000012d0: a4aa e0a4 ace0 a58b e0a4 b0e0 a58d e0a4  ................
-000012e0: a120 e0a4 aee0 a587 e0a4 8220 e0a4 95e0  . ......... ....
-000012f0: a589 e0a4 aae0 a580 20e0 a495 e0a4 bfe0  ........ .......
-00001300: a4af e0a4 be20 e0a4 97e0 a4af e0a4 be20  ..... ......... 
-00001310: e0a4 b9e0 a588 7538 0000 00e0 a48f e0a4  ......u8........
-00001320: aae0 a58d e0a4 b2e0 a4bf e0a4 95e0 a587  ................
-00001330: e0a4 b6e0 a4a8 20e0 a495 e0a5 8020 e0a4  ...... ...... ..
-00001340: 9ce0 a4be e0a4 a8e0 a495 e0a4 bee0 a4b0  ................
-00001350: e0a5 8075 2b00 0000 e0a4 aee0 a4be e0a4  ...u+...........
-00001360: b0e0 a58d e0a4 95e0 a4a1 e0a4 bee0 a489  ................
-00001370: e0a4 a820 e0a4 8fe0 a4a1 e0a4 bfe0 a49f  ... ............
-00001380: e0a4 b075 1500 0000 e0a4 b8e0 a482 e0a4  ...u............
-00001390: b8e0 a58d e0a4 95e0 a4b0 e0a4 a375 1500  .............u..
-000013a0: 0000 e0a4 b2e0 a4be e0a4 87e0 a4b8 e0a5  ................
-000013b0: 87e0 a482 e0a4 b875 1500 0000 e0a4 b5e0  .......u........
-000013c0: a587 e0a4 ace0 a4b8 e0a4 bee0 a487 e0a4  ................
-000013d0: 9f75 0f00 0000 e0a4 97e0 a4bf e0a4 9fe0  .u..............
-000013e0: a4b9 e0a4 ac75 0f00 0000 e0a4 aae0 a4be  .....u..........
-000013f0: e0a4 87e0 a4aa e0a5 8075 0f00 0000 e0a4  .........u......
-00001400: a4e0 a4be e0a4 b0e0 a580 e0a4 9675 5a00  .............uZ.
-00001410: 0000 e0a4 90e0 a4aa 20e0 a495 e0a4 be20  ........ ...... 
-00001420: e0a4 a8e0 a4af e0a4 be20 e0a4 b8e0 a482  ......... ......
-00001430: e0a4 b8e0 a58d e0a4 95e0 a4b0 e0a4 a320  ............... 
-00001440: 277b 6c61 7465 7374 5f76 6572 7369 6f6e  '{latest_version
-00001450: 7d27 20e0 a489 e0a4 aae0 a4b2 e0a4 ace0  }' .............
-00001460: a58d e0a4 a720 e0a4 b9e0 a588 7553 0000  ..... ......uS..
-00001470: 00e0 a490 e0a4 aa20 e0a4 95e0 a4be 20e0  ....... ...... .
-00001480: a4a8 e0a4 b5e0 a580 e0a4 a8e0 a4a4 e0a4  ................
-00001490: ae20 e0a4 b8e0 a482 e0a4 b8e0 a58d e0a4  . ..............
-000014a0: 95e0 a4b0 e0a4 a320 e0a4 b8e0 a58d e0a4  ....... ........
-000014b0: a5e0 a4be e0a4 aae0 a4bf e0a4 a420 e0a4  ............. ..
-000014c0: b9e0 a588 7577 0000 00e0 a4aa e0a5 8de0  ....uw..........
-000014d0: a4b0 e0a4 a4e0 a4bf e0a4 95e0 a58d e0a4  ................
-000014e0: b0e0 a4bf e0a4 afe0 a4be 20e0 a49c e0a4  .......... .....
-000014f0: bee0 a4a8 e0a4 95e0 a4be e0a4 b0e0 a580  ................
-00001500: 20e0 a4aa e0a5 8de0 a4b0 e0a4 bee0 a4aa   ...............
-00001510: e0a5 8de0 a4a4 20e0 a495 e0a4 b0e0 a4a8  ...... .........
-00001520: e0a5 8720 e0a4 aee0 a587 e0a4 8220 e0a4  ... ......... ..
-00001530: 85e0 a4b8 e0a4 aee0 a4b0 e0a5 8de0 a4a5  ................
-00001540: 759e 0000 00e0 a4b9 e0a5 8be0 a4b8 e0a5  u...............
-00001550: 8de0 a49f 20e0 a4a8 e0a4 b9e0 a580 e0a4  .... ...........
-00001560: 8220 e0a4 aee0 a4bf e0a4 b2e0 a4be e0a5  . ..............
-00001570: a420 e0a4 87e0 a482 e0a4 9fe0 a4b0 e0a4  . ..............
-00001580: a8e0 a587 e0a4 9f20 e0a4 95e0 a4a8 e0a5  ....... ........
-00001590: 87e0 a495 e0a5 8de0 a4b6 e0a4 a820 e0a4  ............. ..
-000015a0: afe0 a4be 2044 4e53 20e0 a4ae e0a5 87e0  .... DNS .......
-000015b0: a482 20e0 a4b8 e0a4 aee0 a4b8 e0a5 8de0  .. .............
-000015c0: a4af e0a4 be20 e0a4 b9e0 a58b 20e0 a4b8  ..... ...... ...
-000015d0: e0a4 95e0 a4a4 e0a5 8020 e0a4 b9e0 a588  ......... ......
-000015e0: e0a5 a475 d600 0000 e0a4 95e0 a4a8 e0a5  ...u............
-000015f0: 87e0 a495 e0a5 8de0 a4b6 e0a4 a820 e0a4  ............. ..
-00001600: 85e0 a4b8 e0a5 8de0 a4b5 e0a5 80e0 a495  ................
-00001610: e0a5 83e0 a4a4 20e0 a495 e0a4 bfe0 a4af  ...... .........
-00001620: e0a4 be20 e0a4 97e0 a4af e0a4 bee0 a5a4  ... ............
-00001630: 20e0 a4b8 e0a4 b0e0 a58d e0a4 b5e0 a4b0   ...............
-00001640: 20e0 a4ac e0a4 82e0 a4a6 20e0 a4b9 e0a5   ......... .....
-00001650: 8b20 e0a4 b8e0 a495 e0a4 a4e0 a4be 20e0  . ............ .
-00001660: a4b9 e0a5 882c 20e0 a4af e0a4 be20 e0a4  ....., ...... ..
-00001670: a8e0 a587 e0a4 9fe0 a4b5 e0a4 b0e0 a58d  ................
-00001680: e0a4 9520 e0a4 aee0 a587 e0a4 8220 e0a4  ... ......... ..
-00001690: b8e0 a4ae e0a4 b8e0 a58d e0a4 afe0 a4be  ................
-000016a0: 20e0 a4b9 e0a5 8b20 e0a4 b8e0 a495 e0a4   ...... ........
-000016b0: a4e0 a580 20e0 a4b9 e0a5 88e0 a5a4 759e  .... .........u.
-000016c0: 0000 00e0 a495 e0a4 a8e0 a587 e0a4 95e0  ................
-000016d0: a58d e0a4 b6e0 a4a8 20e0 a495 e0a4 be20  ........ ...... 
-000016e0: e0a4 b8e0 a4ae e0a4 af20 e0a4 b8e0 a4ae  ......... ......
-000016f0: e0a4 bee0 a4aa e0a5 8de0 a4a4 20e0 a4b9  ............ ...
-00001700: e0a5 8b20 e0a4 97e0 a4af e0a4 bee0 a5a4  ... ............
-00001710: 20e0 a4a8 e0a5 87e0 a49f e0a4 b5e0 a4b0   ...............
-00001720: e0a5 8de0 a495 20e0 a4ae e0a5 87e0 a482  ...... .........
-00001730: 20e0 a4b8 e0a4 aee0 a4b8 e0a5 8de0 a4af   ...............
-00001740: e0a4 be20 e0a4 b9e0 a58b 20e0 a4b8 e0a4  ... ...... .....
-00001750: 95e0 a4a4 e0a5 8020 e0a4 b9e0 a588 e0a5  ....... ........
-00001760: a475 8f00 0000 e0a4 95e0 a4a8 e0a5 87e0  .u..............
-00001770: a495 e0a5 8de0 a4b6 e0a4 a820 3430 3420  ........... 404 
-00001780: e0a4 a4e0 a58d e0a4 b0e0 a581 e0a4 9fe0  ................
-00001790: a4bf e0a5 a420 e0a4 85e0 a4a8 e0a5 81e0  ..... ..........
-000017a0: a4b0 e0a5 8be0 a4a7 e0a4 bfe0 a4a4 20e0  .............. .
-000017b0: a4aa e0a5 83e0 a4b7 e0a5 8de0 a4a0 20e0  .............. .
-000017c0: a4af e0a4 be20 e0a4 b8e0 a482 e0a4 b8e0  ..... ..........
-000017d0: a4be e0a4 a7e0 a4a8 20e0 a4a8 e0a4 b9e0  ........ .......
-000017e0: a580 e0a4 8220 e0a4 aee0 a4bf e0a4 b2e0  ..... ..........
-000017f0: a4be e0a5 a475 5c00 0000 e0a4 b8e0 a58d  .....u\.........
-00001800: e0a4 a5e0 a4bf e0a4 a4e0 a4bf 20e0 a495  ............ ...
-00001810: e0a5 8be0 a4a1 20e0 a495 e0a5 8720 e0a4  ...... ...... ..
-00001820: b8e0 a4be e0a4 a520 e0a4 85e0 a4a8 e0a5  ....... ........
-00001830: 81e0 a4b0 e0a5 8be0 a4a7 20e0 a4b5 e0a4  .......... .....
-00001840: bfe0 a4ab e0a4 b23a 207b 7374 6174 7573  .......: {status
-00001850: 5f63 6f64 657d 2954 da09 6170 705f 7469  _code})T..app_ti
-00001860: 746c 65da 1261 7070 5f74 6974 6c65 5f77  tle..app_title_w
-00001870: 6974 685f 7375 62da 1b74 7265 655f 6669  ith_sub..tree_fi
-00001880: 6c74 6572 5f61 6363 6573 7369 626c 655f  lter_accessible_
-00001890: 6465 7363 da12 6d65 6e75 5f61 6374 696f  desc..menu_actio
-000018a0: 6e5f 7265 6e61 6d65 da12 6d65 6e75 5f61  n_rename..menu_a
-000018b0: 6374 696f 6e5f 6465 6c65 7465 da1d 6d65  ction_delete..me
-000018c0: 6e75 5f61 6374 696f 6e5f 6465 6c65 7465  nu_action_delete
-000018d0: 5f63 6f6d 706c 6574 656c 79da 136d 656e  _completely..men
-000018e0: 755f 6163 7469 6f6e 5f72 6573 746f 7265  u_action_restore
-000018f0: da18 6469 616c 6f67 5f66 696c 655f 7265  ..dialog_file_re
-00001900: 6e61 6d65 5f74 6974 6c65 da1e 6469 616c  name_title..dial
-00001910: 6f67 5f66 696c 655f 7265 6e61 6d65 5f66  og_file_rename_f
-00001920: 6965 6c64 5f6c 6162 656c da1c 6469 616c  ield_label..dial
-00001930: 6f67 5f66 696c 655f 7265 6e61 6d65 5f62  og_file_rename_b
-00001940: 7574 746f 6e5f 6f6b da21 6469 616c 6f67  utton_ok.!dialog
-00001950: 5f66 696c 655f 7265 6e61 6d65 5f77 6172  _file_rename_war
-00001960: 6e69 6e67 5f65 7869 7374 73da 1864 6961  ning_exists..dia
-00001970: 6c6f 675f 6669 6c65 5f64 656c 6574 655f  log_file_delete_
-00001980: 7469 746c 65da 1764 6961 6c6f 675f 6669  title..dialog_fi
-00001990: 6c65 5f64 656c 6574 655f 7465 7874 da23  le_delete_text.#
-000019a0: 6469 616c 6f67 5f66 696c 655f 6465 6c65  dialog_file_dele
-000019b0: 7465 5f63 6f6d 706c 6574 656c 795f 7469  te_completely_ti
-000019c0: 746c 65da 2264 6961 6c6f 675f 6669 6c65  tle."dialog_file
-000019d0: 5f64 656c 6574 655f 636f 6d70 6c65 7465  _delete_complete
-000019e0: 6c79 5f74 6578 74da 1864 6961 6c6f 675f  ly_text..dialog_
-000019f0: 6669 6c65 5f64 656c 6574 655f 6572 726f  file_delete_erro
-00001a00: 72da 2264 6961 6c6f 675f 6669 6c65 5f64  r."dialog_file_d
-00001a10: 656c 6574 655f 6572 726f 725f 6e6f 745f  elete_error_not_
-00001a20: 666f 756e 64da 1964 6961 6c6f 675f 6669  found..dialog_fi
-00001a30: 6c65 5f72 6573 746f 7265 5f74 6974 6c65  le_restore_title
-00001a40: da18 6469 616c 6f67 5f66 696c 655f 7265  ..dialog_file_re
-00001a50: 7374 6f72 655f 7465 7874 da19 6469 616c  store_text..dial
-00001a60: 6f67 5f66 696c 655f 7265 7374 6f72 655f  og_file_restore_
-00001a70: 6572 726f 72da 2264 6961 6c6f 675f 6669  error."dialog_fi
-00001a80: 6c65 5f72 6573 746f 7265 5f77 6172 6e69  le_restore_warni
-00001a90: 6e67 5f65 7869 7374 73da 1864 6961 6c6f  ng_exists..dialo
-00001aa0: 675f 6d65 7373 6167 655f 626f 785f 7469  g_message_box_ti
-00001ab0: 746c 65da 1c64 6961 6c6f 675f 6d65 7373  tle..dialog_mess
-00001ac0: 6167 655f 626f 785f 6275 7474 6f6e 5f6f  age_box_button_o
-00001ad0: 6bda 2861 6374 696f 6e5f 6e65 775f 6669  k.(action_new_fi
-00001ae0: 6c65 5f66 6972 7374 5f6c 696e 655f 7465  le_first_line_te
-00001af0: 6d70 6c61 7465 5f74 6578 74da 1f61 6374  mplate_text..act
-00001b00: 696f 6e5f 6f70 656e 5f66 696c 655f 6469  ion_open_file_di
-00001b10: 616c 6f67 5f63 6170 7469 6f6e da22 6163  alog_caption."ac
-00001b20: 7469 6f6e 5f73 6176 655f 6173 5f66 696c  tion_save_as_fil
-00001b30: 655f 6469 616c 6f67 5f63 6170 7469 6f6e  e_dialog_caption
-00001b40: da1c 6469 616c 6f67 5f73 6176 655f 656d  ..dialog_save_em
-00001b50: 7074 795f 6669 6c65 5f74 6974 6c65 da1b  pty_file_title..
-00001b60: 6469 616c 6f67 5f73 6176 655f 656d 7074  dialog_save_empt
-00001b70: 795f 6669 6c65 5f74 6578 74da 1964 6961  y_file_text..dia
-00001b80: 6c6f 675f 656e 6372 7970 745f 6669 6c65  log_encrypt_file
-00001b90: 5f74 6974 6c65 da18 6469 616c 6f67 5f65  _title..dialog_e
-00001ba0: 6e63 7279 7074 5f66 696c 655f 7465 7874  ncrypt_file_text
-00001bb0: da2e 656e 6372 7970 745f 6669 6c65 5f77  ..encrypt_file_w
-00001bc0: 6172 6e69 6e67 5f66 696c 655f 6973 5f61  arning_file_is_a
-00001bd0: 6c72 6561 6479 5f65 6e63 7279 7074 6564  lready_encrypted
-00001be0: da2a 6469 616c 6f67 5f65 6e63 7279 7074  .*dialog_encrypt
-00001bf0: 5f66 696c 655f 7265 7772 6974 655f 6578  _file_rewrite_ex
-00001c00: 6973 7469 6e67 5f74 6974 6c65 da29 6469  isting_title.)di
-00001c10: 616c 6f67 5f65 6e63 7279 7074 5f66 696c  alog_encrypt_fil
-00001c20: 655f 7265 7772 6974 655f 6578 6973 7469  e_rewrite_existi
-00001c30: 6e67 5f74 6578 74da 1964 6961 6c6f 675f  ng_text..dialog_
-00001c40: 6465 6372 7970 745f 6669 6c65 5f74 6974  decrypt_file_tit
-00001c50: 6c65 da18 6469 616c 6f67 5f64 6563 7279  le..dialog_decry
-00001c60: 7074 5f66 696c 655f 7465 7874 da2a 6465  pt_file_text.*de
-00001c70: 6372 7970 745f 6669 6c65 5f77 6172 6e69  crypt_file_warni
-00001c80: 6e67 5f66 696c 655f 6973 5f6e 6f74 5f65  ng_file_is_not_e
-00001c90: 6e63 7279 7074 6564 da2a 6469 616c 6f67  ncrypted.*dialog
-00001ca0: 5f64 6563 7279 7074 5f66 696c 655f 7265  _decrypt_file_re
-00001cb0: 7772 6974 655f 6578 6973 7469 6e67 5f74  write_existing_t
-00001cc0: 6974 6c65 da29 6469 616c 6f67 5f64 6563  itle.)dialog_dec
-00001cd0: 7279 7074 5f66 696c 655f 7265 7772 6974  rypt_file_rewrit
-00001ce0: 655f 6578 6973 7469 6e67 5f74 6578 74da  e_existing_text.
-00001cf0: 2164 6961 6c6f 675f 656e 6372 7970 745f  !dialog_encrypt_
-00001d00: 6e65 775f 7061 7373 776f 7264 5f74 6974  new_password_tit
-00001d10: 6c65 da21 6469 616c 6f67 5f65 6e63 7279  le.!dialog_encry
-00001d20: 7074 5f6e 6577 5f70 6173 7377 6f72 645f  pt_new_password_
-00001d30: 6c61 6265 6cda 3264 6961 6c6f 675f 656e  label.2dialog_en
-00001d40: 6372 7970 745f 6e65 775f 7061 7373 776f  crypt_new_passwo
-00001d50: 7264 5f69 6e70 7574 5f70 6c61 6365 686f  rd_input_placeho
-00001d60: 6c64 6572 5f74 6578 74da 2664 6961 6c6f  lder_text.&dialo
-00001d70: 675f 656e 6372 7970 745f 6e65 775f 7061  g_encrypt_new_pa
-00001d80: 7373 776f 7264 5f68 696e 745f 6c61 6265  ssword_hint_labe
-00001d90: 6cda 3264 6961 6c6f 675f 656e 6372 7970  l.2dialog_encryp
-00001da0: 745f 6e65 775f 7061 7373 776f 7264 5f68  t_new_password_h
-00001db0: 696e 745f 6c61 6265 6c5f 6465 7363 7269  int_label_descri
-00001dc0: 7074 696f 6eda 3764 6961 6c6f 675f 656e  ption.7dialog_en
-00001dd0: 6372 7970 745f 6e65 775f 7061 7373 776f  crypt_new_passwo
-00001de0: 7264 5f68 696e 745f 696e 7075 745f 706c  rd_hint_input_pl
-00001df0: 6163 6568 6f6c 6465 725f 7465 7874 da25  aceholder_text.%
-00001e00: 6469 616c 6f67 5f65 6e63 7279 7074 5f6e  dialog_encrypt_n
-00001e10: 6577 5f70 6173 7377 6f72 645f 6275 7474  ew_password_butt
-00001e20: 6f6e 5f6f 6bda 2964 6961 6c6f 675f 656e  on_ok.)dialog_en
-00001e30: 6372 7970 745f 6e65 775f 7061 7373 776f  crypt_new_passwo
-00001e40: 7264 5f62 7574 746f 6e5f 6361 6e63 656c  rd_button_cancel
-00001e50: da2f 6469 616c 6f67 5f65 6e63 7279 7074  ./dialog_encrypt
-00001e60: 5f6e 6577 5f70 6173 7377 6f72 645f 7761  _new_password_wa
-00001e70: 726e 696e 675f 656d 7074 795f 7469 746c  rning_empty_titl
-00001e80: 65da 2e64 6961 6c6f 675f 656e 6372 7970  e..dialog_encryp
-00001e90: 745f 6e65 775f 7061 7373 776f 7264 5f77  t_new_password_w
-00001ea0: 6172 6e69 6e67 5f65 6d70 7479 5f74 6578  arning_empty_tex
-00001eb0: 74da 3264 6961 6c6f 675f 656e 6372 7970  t.2dialog_encryp
-00001ec0: 745f 6e65 775f 7061 7373 776f 7264 5f77  t_new_password_w
-00001ed0: 6172 6e69 6e67 5f74 6f6f 5f6c 6f6e 675f  arning_too_long_
-00001ee0: 7469 746c 65da 3164 6961 6c6f 675f 656e  title.1dialog_en
-00001ef0: 6372 7970 745f 6e65 775f 7061 7373 776f  crypt_new_passwo
-00001f00: 7264 5f77 6172 6e69 6e67 5f74 6f6f 5f6c  rd_warning_too_l
-00001f10: 6f6e 675f 7465 7874 da1d 6469 616c 6f67  ong_text..dialog
-00001f20: 5f65 6e63 7279 7074 5f70 6173 7377 6f72  _encrypt_passwor
-00001f30: 645f 7469 746c 65da 1d64 6961 6c6f 675f  d_title..dialog_
-00001f40: 656e 6372 7970 745f 7061 7373 776f 7264  encrypt_password
-00001f50: 5f6c 6162 656c da2e 6469 616c 6f67 5f65  _label..dialog_e
-00001f60: 6e63 7279 7074 5f70 6173 7377 6f72 645f  ncrypt_password_
-00001f70: 696e 7075 745f 706c 6163 6568 6f6c 6465  input_placeholde
-00001f80: 725f 7465 7874 da22 6469 616c 6f67 5f65  r_text."dialog_e
-00001f90: 6e63 7279 7074 5f70 6173 7377 6f72 645f  ncrypt_password_
-00001fa0: 6869 6e74 5f6c 6162 656c da21 6469 616c  hint_label.!dial
-00001fb0: 6f67 5f65 6e63 7279 7074 5f70 6173 7377  og_encrypt_passw
-00001fc0: 6f72 645f 6275 7474 6f6e 5f6f 6bda 2564  ord_button_ok.%d
-00001fd0: 6961 6c6f 675f 656e 6372 7970 745f 7061  ialog_encrypt_pa
-00001fe0: 7373 776f 7264 5f62 7574 746f 6e5f 6361  ssword_button_ca
-00001ff0: 6e63 656c da23 6469 616c 6f67 5f65 6e63  ncel.#dialog_enc
-00002000: 7279 7074 5f70 6173 7377 6f72 645f 7265  rypt_password_re
-00002010: 7365 745f 7469 746c 65da 2264 6961 6c6f  set_title."dialo
-00002020: 675f 656e 6372 7970 745f 7061 7373 776f  g_encrypt_passwo
-00002030: 7264 5f72 6573 6574 5f74 6578 74da 2b64  rd_reset_text.+d
-00002040: 6961 6c6f 675f 656e 6372 7970 745f 7061  ialog_encrypt_pa
-00002050: 7373 776f 7264 5f72 6573 6574 5f62 7574  ssword_reset_but
-00002060: 746f 6e5f 6361 6e63 656c da28 6469 616c  ton_cancel.(dial
-00002070: 6f67 5f65 6e63 7279 7074 5f70 6173 7377  og_encrypt_passw
-00002080: 6f72 645f 7265 7365 745f 6275 7474 6f6e  ord_reset_button
-00002090: 5f79 6573 da16 6469 616c 6f67 5f6f 7065  _yes..dialog_ope
-000020a0: 6e5f 6c69 6e6b 5f74 6974 6c65 da15 6469  n_link_title..di
-000020b0: 616c 6f67 5f6f 7065 6e5f 6c69 6e6b 5f74  alog_open_link_t
-000020c0: 6578 74da 266c 6f61 645f 6669 6c65 5f65  ext.&load_file_e
-000020d0: 6e63 7279 7074 696f 6e5f 7061 7373 776f  ncryption_passwo
-000020e0: 7264 5f6d 6973 6d61 7463 68da 276c 6f61  rd_mismatch.'loa
-000020f0: 645f 6669 6c65 5f65 6e63 7279 7074 696f  d_file_encryptio
-00002100: 6e5f 7061 7373 776f 7264 5f69 6e63 6f72  n_password_incor
-00002110: 7265 6374 da1c 6c6f 6164 5f66 696c 655f  rect..load_file_
-00002120: 6e6f 6e65 5f63 6f6e 7465 6e74 5f65 7272  none_content_err
-00002130: 6f72 da1f 7361 7665 5f61 6374 6976 655f  or..save_active_
-00002140: 6669 6c65 5f65 7272 6f72 5f6f 6363 7572  file_error_occur
-00002150: 7265 64da 1e65 7870 616e 6461 626c 655f  red..expandable_
-00002160: 626c 6f63 6b5f 6465 6661 756c 745f 7469  block_default_ti
-00002170: 746c 65da 3164 6961 6c6f 675f 636f 6c6f  tle.1dialog_colo
-00002180: 725f 7069 636b 6572 5f63 6f6c 6f72 5f63  r_picker_color_c
-00002190: 6f70 6965 645f 746f 5f74 6865 5f63 6c69  opied_to_the_cli
-000021a0: 7062 6f61 7264 da11 706f 7075 705f 6162  pboard..popup_ab
-000021b0: 6f75 745f 7469 746c 65da 2070 6f70 7570  out_title. popup
-000021c0: 5f61 626f 7574 5f61 7070 5f6e 616d 655f  _about_app_name_
-000021d0: 6465 7363 7269 7074 696f 6eda 1370 6f70  description..pop
-000021e0: 7570 5f61 626f 7574 5f76 6572 7369 6f6e  up_about_version
-000021f0: da13 706f 7075 705f 6162 6f75 745f 6c69  ..popup_about_li
-00002200: 6365 6e73 65da 1370 6f70 7570 5f61 626f  cense..popup_abo
-00002210: 7574 5f77 6562 7369 7465 da16 706f 7075  ut_website..popu
-00002220: 705f 6162 6f75 745f 7265 706f 7369 746f  p_about_reposito
-00002230: 7279 da10 706f 7075 705f 6162 6f75 745f  ry..popup_about_
-00002240: 7079 7069 da10 706f 7075 705f 6162 6f75  pypi..popup_abou
-00002250: 745f 6461 7465 da26 7570 6461 7465 5f68  t_date.&update_h
-00002260: 656c 7065 725f 6e65 775f 7665 7273 696f  elper_new_versio
-00002270: 6e5f 6973 5f61 7661 696c 6162 6c65 da26  n_is_available.&
-00002280: 7570 6461 7465 5f68 656c 7065 725f 6c61  update_helper_la
-00002290: 7465 7374 5f76 6572 7369 6f6e 5f69 6e73  test_version_ins
-000022a0: 7461 6c6c 6564 da1e 6e65 7477 6f72 6b5f  talled..network_
-000022b0: 636f 6e6e 6563 7469 6f6e 5f65 7272 6f72  connection_error
-000022c0: 5f65 6d70 7479 da2a 6e65 7477 6f72 6b5f  _empty.*network_
-000022d0: 636f 6e6e 6563 7469 6f6e 5f65 7272 6f72  connection_error
-000022e0: 5f63 6f6e 6e65 6374 696f 6e5f 6f72 5f64  _connection_or_d
-000022f0: 6e73 da2b 6e65 7477 6f72 6b5f 636f 6e6e  ns.+network_conn
-00002300: 6563 7469 6f6e 5f65 7272 6f72 5f63 6f6e  ection_error_con
-00002310: 6e65 6374 696f 6e5f 7265 6675 7365 64da  nection_refused.
-00002320: 2d6e 6574 776f 726b 5f63 6f6e 6e65 6374  -network_connect
-00002330: 696f 6e5f 6572 726f 725f 636f 6e6e 6563  ion_error_connec
-00002340: 7469 6f6e 5f74 696d 6564 5f6f 7574 da2d  tion_timed_out.-
-00002350: 6e65 7477 6f72 6b5f 636f 6e6e 6563 7469  network_connecti
-00002360: 6f6e 5f65 7272 6f72 5f63 6f6e 6e65 6374  on_error_connect
-00002370: 696f 6e5f 3430 345f 6572 726f 72da 316e  ion_404_error.1n
-00002380: 6574 776f 726b 5f63 6f6e 6e65 6374 696f  etwork_connectio
-00002390: 6e5f 6572 726f 725f 6765 6e65 7269 635f  n_error_generic_
-000023a0: 7769 7468 5f73 7461 7475 735f 636f 6465  with_status_code
-000023b0: 4e29 01da 076c 6578 656d 6573 a900 7256  N)...lexemes..rV
-000023c0: 0000 0072 5600 0000 fa43 2f55 7365 7273  ...rV....C/Users
-000023d0: 2f76 6164 696b 7573 2f50 7963 6861 726d  /vadikus/Pycharm
-000023e0: 5072 6f6a 6563 7473 2f6e 6f74 6f6c 6f67  Projects/notolog
-000023f0: 2d64 6576 2f61 7070 2f6c 6578 656d 6573  -dev/app/lexemes
-00002400: 2f69 6e2f 636f 6d6d 6f6e 2e70 79da 083c  /in/common.py..<
-00002410: 6d6f 6475 6c65 3e03 0000 0073 a800 0000  module>....s....
-00002420: 0201 0202 0202 0201 0201 0201 0202 0201  ................
-00002430: 0201 0201 0202 0201 0201 0201 0201 0201  ................
-00002440: 0202 0201 0201 0201 0202 0201 0202 0201  ................
-00002450: 0201 0202 0201 0202 0201 0201 0201 0201  ................
-00002460: 0202 0201 0201 0201 0201 0202 0201 0201  ................
-00002470: 0201 0201 0204 0201 0201 0201 0201 0201  ................
-00002480: 0201 0202 0201 0201 0201 0201 0201 0202  ................
-00002490: 0201 0201 0201 0202 0201 0202 0201 0201  ................
-000024a0: 0202 0202 0202 0202 0201 0202 0201 0201  ................
-000024b0: 0201 0201 0201 0202 0201 0202 0201 0202  ................
-000024c0: 0201 0201 0201 0292                      ........
+00000000: 2320 4869 6e64 6920 6c65 7865 6d65 7320  # Hindi lexemes 
+00000010: 636f 6d6d 6f6e 2e70 790a 6c65 7865 6d65  common.py.lexeme
+00000020: 7320 3d20 7b0a 2020 2020 2261 7070 5f74  s = {.    "app_t
+00000030: 6974 6c65 223a 2022 e0a4 a8e0 a58b e0a4  itle": "........
+00000040: 9fe0 a58b e0a4 b2e0 a589 e0a4 9720 e0a4  ............. ..
+00000050: 8fe0 a4a1 e0a4 bfe0 a49f e0a4 b022 2c0a  .............",.
+00000060: 2020 2020 2261 7070 5f74 6974 6c65 5f77      "app_title_w
+00000070: 6974 685f 7375 6222 3a20 227b 6170 705f  ith_sub": "{app_
+00000080: 7469 746c 657d 202d 207b 7375 625f 7469  title} - {sub_ti
+00000090: 746c 657d 222c 0a0a 2020 2020 2274 7265  tle}",..    "tre
+000000a0: 655f 6669 6c74 6572 5f61 6363 6573 7369  e_filter_accessi
+000000b0: 626c 655f 6465 7363 223a 2022 e0a4 abe0  ble_desc": "....
+000000c0: a4bc e0a4 bee0 a487 e0a4 b220 e0a4 abe0  ........... ....
+000000d0: a4bc e0a4 bfe0 a4b2 e0a5 8de0 a49f e0a4  ................
+000000e0: b020 e0a4 abe0 a4bc e0a5 80e0 a4b2 e0a5  . ..............
+000000f0: 8de0 a4a1 222c 0a0a 2020 2020 226d 656e  ....",..    "men
+00000100: 755f 6163 7469 6f6e 5f72 656e 616d 6522  u_action_rename"
+00000110: 3a20 22e0 a4a8 e0a4 bee0 a4ae 20e0 a4ac  : "......... ...
+00000120: e0a4 a6e0 a4b2 e0a5 87e0 a482 222c 0a20  ............",. 
+00000130: 2020 2022 6d65 6e75 5f61 6374 696f 6e5f     "menu_action_
+00000140: 6465 6c65 7465 223a 2022 e0a4 b9e0 a49f  delete": "......
+00000150: e0a4 bee0 a48f e0a4 8222 2c0a 2020 2020  .........",.    
+00000160: 226d 656e 755f 6163 7469 6f6e 5f64 656c  "menu_action_del
+00000170: 6574 655f 636f 6d70 6c65 7465 6c79 223a  ete_completely":
+00000180: 2022 e0a4 aae0 a582 e0a4 b0e0 a580 20e0   "............ .
+00000190: a4a4 e0a4 b0e0 a4b9 20e0 a4b8 e0a5 8720  ........ ...... 
+000001a0: e0a4 b9e0 a49f e0a4 bee0 a48f e0a4 8222  ..............."
+000001b0: 2c0a 2020 2020 226d 656e 755f 6163 7469  ,.    "menu_acti
+000001c0: 6f6e 5f72 6573 746f 7265 223a 2022 e0a4  on_restore": "..
+000001d0: aae0 a581 e0a4 a8e0 a4b0 e0a5 8de0 a4b8  ................
+000001e0: e0a5 8de0 a4a5 e0a4 bee0 a4aa e0a4 bfe0  ................
+000001f0: a4a4 20e0 a495 e0a4 b0e0 a587 e0a4 8222  .. ............"
+00000200: 2c0a 0a20 2020 2022 6469 616c 6f67 5f66  ,..    "dialog_f
+00000210: 696c 655f 7265 6e61 6d65 5f74 6974 6c65  ile_rename_title
+00000220: 223a 2022 e0a4 abe0 a4bc e0a4 bee0 a487  ": "............
+00000230: e0a4 b220 e0a4 95e0 a4be 20e0 a4a8 e0a4  ... ...... .....
+00000240: bee0 a4ae 20e0 a4ac e0a4 a6e0 a4b2 e0a5  .... ...........
+00000250: 87e0 a482 222c 0a20 2020 2022 6469 616c  ....",.    "dial
+00000260: 6f67 5f66 696c 655f 7265 6e61 6d65 5f66  og_file_rename_f
+00000270: 6965 6c64 5f6c 6162 656c 223a 2022 e0a4  ield_label": "..
+00000280: a8e0 a4af e0a4 be20 e0a4 abe0 a4bc e0a4  ....... ........
+00000290: bee0 a487 e0a4 b220 e0a4 a8e0 a4be e0a4  ....... ........
+000002a0: ae20 e0a4 a6e0 a4b0 e0a5 8de0 a49c 20e0  . ............ .
+000002b0: a495 e0a4 b0e0 a587 e0a4 8222 2c0a 2020  ...........",.  
+000002c0: 2020 2264 6961 6c6f 675f 6669 6c65 5f72    "dialog_file_r
+000002d0: 656e 616d 655f 6275 7474 6f6e 5f6f 6b22  ename_button_ok"
+000002e0: 3a20 22e0 a4a8 e0a4 bee0 a4ae 20e0 a4ac  : "......... ...
+000002f0: e0a4 a6e0 a4b2 e0a5 87e0 a482 222c 0a20  ............",. 
+00000300: 2020 2022 6469 616c 6f67 5f66 696c 655f     "dialog_file_
+00000310: 7265 6e61 6d65 5f77 6172 6e69 6e67 5f65  rename_warning_e
+00000320: 7869 7374 7322 3a20 22e0 a487 e0a4 b8e0  xists": ".......
+00000330: a580 20e0 a4a8 e0a4 bee0 a4ae 20e0 a495  .. ......... ...
+00000340: e0a5 8020 e0a4 abe0 a4bc e0a4 bee0 a487  ... ............
+00000350: e0a4 b220 e0a4 aae0 a4b9 e0a4 b2e0 a587  ... ............
+00000360: 20e0 a4b8 e0a5 8720 e0a4 aee0 a58c e0a4   ...... ........
+00000370: 9ce0 a582 e0a4 a620 e0a4 b9e0 a588 222c  ....... ......",
+00000380: 0a0a 2020 2020 2264 6961 6c6f 675f 6669  ..    "dialog_fi
+00000390: 6c65 5f64 656c 6574 655f 7469 746c 6522  le_delete_title"
+000003a0: 3a20 22e0 a4ab e0a4 bce0 a4be e0a4 87e0  : ".............
+000003b0: a4b2 20e0 a4b9 e0a4 9fe0 a4be e0a4 8fe0  .. .............
+000003c0: a482 222c 0a20 2020 2022 6469 616c 6f67  ..",.    "dialog
+000003d0: 5f66 696c 655f 6465 6c65 7465 5f74 6578  _file_delete_tex
+000003e0: 7422 3a20 22e0 a495 e0a5 8de0 a4af e0a4  t": "...........
+000003f0: be20 e0a4 86e0 a4aa 20e0 a4b5 e0a4 bee0  . ...... .......
+00000400: a495 e0a4 8820 e0a4 abe0 a4bc e0a4 bee0  ..... ..........
+00000410: a487 e0a4 b220 5c22 7b66 696c 655f 6e61  ..... \"{file_na
+00000420: 6d65 7d5c 2220 e0a4 95e0 a58b 20e0 a4b9  me}\" ...... ...
+00000430: e0a4 9fe0 a4be e0a4 a8e0 a4be 20e0 a49a  ............ ...
+00000440: e0a4 bee0 a4b9 e0a4 a4e0 a587 20e0 a4b9  ............ ...
+00000450: e0a5 88e0 a482 3f22 2c0a 2020 2020 2264  ......?",.    "d
+00000460: 6961 6c6f 675f 6669 6c65 5f64 656c 6574  ialog_file_delet
+00000470: 655f 636f 6d70 6c65 7465 6c79 5f74 6974  e_completely_tit
+00000480: 6c65 223a 2022 e0a4 abe0 a4bc e0a4 bee0  le": "..........
+00000490: a487 e0a4 b220 e0a4 95e0 a58b 20e0 a4aa  ..... ...... ...
+000004a0: e0a5 82e0 a4b0 e0a5 8020 e0a4 a4e0 a4b0  ......... ......
+000004b0: e0a4 b920 e0a4 b8e0 a587 20e0 a4b9 e0a4  ... ...... .....
+000004c0: 9fe0 a4be e0a4 8fe0 a482 222c 0a20 2020  ..........",.   
+000004d0: 2022 6469 616c 6f67 5f66 696c 655f 6465   "dialog_file_de
+000004e0: 6c65 7465 5f63 6f6d 706c 6574 656c 795f  lete_completely_
+000004f0: 7465 7874 223a 2022 e0a4 95e0 a58d e0a4  text": "........
+00000500: afe0 a4be 20e0 a486 e0a4 aa20 e0a4 b5e0  .... ...... ....
+00000510: a4be e0a4 95e0 a488 20e0 a4ab e0a4 bce0  ........ .......
+00000520: a4be e0a4 87e0 a4b2 205c 227b 6669 6c65  ........ \"{file
+00000530: 5f6e 616d 657d 5c22 20e0 a495 e0a5 8b20  _name}\" ...... 
+00000540: e0a4 aae0 a582 e0a4 b0e0 a580 20e0 a4a4  ............ ...
+00000550: e0a4 b0e0 a4b9 20e0 a4b8 e0a5 8720 e0a4  ...... ...... ..
+00000560: b9e0 a49f e0a4 bee0 a4a8 e0a4 be20 e0a4  ............. ..
+00000570: 9ae0 a4be e0a4 b9e0 a4a4 e0a5 8720 e0a4  ............. ..
+00000580: b9e0 a588 e0a4 823f 222c 0a20 2020 2022  .......?",.    "
+00000590: 6469 616c 6f67 5f66 696c 655f 6465 6c65  dialog_file_dele
+000005a0: 7465 5f65 7272 6f72 223a 2022 e0a4 abe0  te_error": "....
+000005b0: a4bc e0a4 bee0 a487 e0a4 b220 e0a4 b9e0  ........... ....
+000005c0: a49f e0a4 bee0 a4a8 e0a5 8720 e0a4 aee0  ........... ....
+000005d0: a587 e0a4 8220 e0a4 85e0 a4b8 e0a4 aee0  ..... ..........
+000005e0: a4b0 e0a5 8de0 a4a5 2c20 e0a4 a4e0 a58d  ........, ......
+000005f0: e0a4 b0e0 a581 e0a4 9fe0 a4bf 20e0 a4b9  ............ ...
+00000600: e0a5 81e0 a488 20e0 a4b9 e0a5 8822 2c0a  ...... ......",.
+00000610: 2020 2020 2264 6961 6c6f 675f 6669 6c65      "dialog_file
+00000620: 5f64 656c 6574 655f 6572 726f 725f 6e6f  _delete_error_no
+00000630: 745f 666f 756e 6422 3a20 22e0 a4ab e0a4  t_found": ".....
+00000640: bce0 a4be e0a4 87e0 a4b2 20e0 a4a8 e0a4  .......... .....
+00000650: b9e0 a580 e0a4 8220 e0a4 aee0 a4bf e0a4  ....... ........
+00000660: b2e0 a580 222c 0a0a 2020 2020 2264 6961  ....",..    "dia
+00000670: 6c6f 675f 6669 6c65 5f72 6573 746f 7265  log_file_restore
+00000680: 5f74 6974 6c65 223a 2022 e0a4 abe0 a4bc  _title": "......
+00000690: e0a4 bee0 a487 e0a4 b220 e0a4 aae0 a581  ......... ......
+000006a0: e0a4 a8e0 a4b0 e0a5 8de0 a4b8 e0a5 8de0  ................
+000006b0: a4a5 e0a4 bee0 a4aa e0a4 bfe0 a4a4 20e0  .............. .
+000006c0: a495 e0a4 b0e0 a587 e0a4 8222 2c0a 2020  ...........",.  
+000006d0: 2020 2264 6961 6c6f 675f 6669 6c65 5f72    "dialog_file_r
+000006e0: 6573 746f 7265 5f74 6578 7422 3a20 22e0  estore_text": ".
+000006f0: a495 e0a5 8de0 a4af e0a4 be20 e0a4 86e0  ........... ....
+00000700: a4aa 20e0 a4b5 e0a4 bee0 a495 e0a4 8820  .. ............ 
+00000710: e0a4 abe0 a4bc e0a4 bee0 a487 e0a4 b220  ............... 
+00000720: 5c22 7b66 696c 655f 6e61 6d65 7d5c 2220  \"{file_name}\" 
+00000730: e0a4 95e0 a58b 20e0 a4aa e0a5 81e0 a4a8  ...... .........
+00000740: e0a4 b0e0 a58d e0a4 b8e0 a58d e0a4 a5e0  ................
+00000750: a4be e0a4 aae0 a4bf e0a4 a420 e0a4 95e0  ........... ....
+00000760: a4b0 e0a4 a8e0 a4be 20e0 a49a e0a4 bee0  ........ .......
+00000770: a4b9 e0a4 a4e0 a587 20e0 a4b9 e0a5 88e0  ........ .......
+00000780: a482 3f22 2c0a 2020 2020 2264 6961 6c6f  ..?",.    "dialo
+00000790: 675f 6669 6c65 5f72 6573 746f 7265 5f65  g_file_restore_e
+000007a0: 7272 6f72 223a 2022 e0a4 abe0 a4bc e0a4  rror": "........
+000007b0: bee0 a487 e0a4 b220 e0a4 95e0 a58b 20e0  ....... ...... .
+000007c0: a4aa e0a5 81e0 a4a8 e0a4 b0e0 a58d e0a4  ................
+000007d0: b8e0 a58d e0a4 a5e0 a4be e0a4 aae0 a4bf  ................
+000007e0: e0a4 a420 e0a4 95e0 a4b0 e0a4 a8e0 a587  ... ............
+000007f0: 20e0 a4ae e0a5 87e0 a482 20e0 a485 e0a4   ......... .....
+00000800: b8e0 a4ae e0a4 b0e0 a58d e0a4 a52c 20e0  ............., .
+00000810: a4a4 e0a5 8de0 a4b0 e0a5 81e0 a49f e0a4  ................
+00000820: bf20 e0a4 b9e0 a581 e0a4 8820 e0a4 b9e0  . ......... ....
+00000830: a588 222c 0a20 2020 2022 6469 616c 6f67  ..",.    "dialog
+00000840: 5f66 696c 655f 7265 7374 6f72 655f 7761  _file_restore_wa
+00000850: 726e 696e 675f 6578 6973 7473 223a 2022  rning_exists": "
+00000860: e0a4 87e0 a4b8 20e0 a4a8 e0a4 bee0 a4ae  ...... .........
+00000870: 20e0 a495 e0a5 8020 e0a4 abe0 a4bc e0a4   ...... ........
+00000880: bee0 a487 e0a4 b220 e0a4 aae0 a4b9 e0a4  ....... ........
+00000890: b2e0 a587 20e0 a4b8 e0a5 8720 e0a4 aee0  .... ...... ....
+000008a0: a58c e0a4 9ce0 a582 e0a4 a620 e0a4 b9e0  ........... ....
+000008b0: a588 222c 0a0a 2020 2020 2264 6961 6c6f  ..",..    "dialo
+000008c0: 675f 6d65 7373 6167 655f 626f 785f 7469  g_message_box_ti
+000008d0: 746c 6522 3a20 22e0 a4b8 e0a4 82e0 a4a6  tle": ".........
+000008e0: e0a5 87e0 a4b6 222c 0a20 2020 2022 6469  ......",.    "di
+000008f0: 616c 6f67 5f6d 6573 7361 6765 5f62 6f78  alog_message_box
+00000900: 5f62 7574 746f 6e5f 6f6b 223a 2022 e0a4  _button_ok": "..
+00000910: ace0 a482 e0a4 a620 e0a4 95e0 a4b0 e0a5  ....... ........
+00000920: 87e0 a482 222c 0a0a 2020 2020 2261 6374  ....",..    "act
+00000930: 696f 6e5f 6e65 775f 6669 6c65 5f66 6972  ion_new_file_fir
+00000940: 7374 5f6c 696e 655f 7465 6d70 6c61 7465  st_line_template
+00000950: 5f74 6578 7422 3a20 22e0 a4a8 e0a4 afe0  _text": ".......
+00000960: a4be 20e0 a4a6 e0a4 b8e0 a58d e0a4 a4e0  .. .............
+00000970: a4be e0a4 b5e0 a587 e0a4 9ce0 a4bc 222c  ..............",
+00000980: 0a20 2020 2022 6163 7469 6f6e 5f6f 7065  .    "action_ope
+00000990: 6e5f 6669 6c65 5f64 6961 6c6f 675f 6361  n_file_dialog_ca
+000009a0: 7074 696f 6e22 3a20 22e0 a4ab e0a4 bce0  ption": ".......
+000009b0: a4be e0a4 87e0 a4b2 20e0 a496 e0a5 8be0  ........ .......
+000009c0: a4b2 e0a5 87e0 a482 222c 0a20 2020 2022  ........",.    "
+000009d0: 6163 7469 6f6e 5f73 6176 655f 6173 5f66  action_save_as_f
+000009e0: 696c 655f 6469 616c 6f67 5f63 6170 7469  ile_dialog_capti
+000009f0: 6f6e 223a 2022 e0a4 abe0 a4bc e0a4 bee0  on": "..........
+00000a00: a487 e0a4 b220 e0a4 b8e0 a4b9 e0a5 87e0  ..... ..........
+00000a10: a49c e0a5 87e0 a482 222c 0a0a 2020 2020  ........",..    
+00000a20: 2264 6961 6c6f 675f 7361 7665 5f65 6d70  "dialog_save_emp
+00000a30: 7479 5f66 696c 655f 7469 746c 6522 3a20  ty_file_title": 
+00000a40: 22e0 a496 e0a4 bee0 a4b2 e0a5 8020 e0a4  "............ ..
+00000a50: abe0 a4bc e0a4 bee0 a487 e0a4 b220 e0a4  ............. ..
+00000a60: b8e0 a4b9 e0a5 87e0 a49c e0a5 87e0 a482  ................
+00000a70: 222c 0a20 2020 2022 6469 616c 6f67 5f73  ",.    "dialog_s
+00000a80: 6176 655f 656d 7074 795f 6669 6c65 5f74  ave_empty_file_t
+00000a90: 6578 7422 3a20 22e0 a495 e0a5 8de0 a4af  ext": ".........
+00000aa0: e0a4 be20 e0a4 96e0 a4be e0a4 b2e0 a580  ... ............
+00000ab0: 20e0 a4b8 e0a4 bee0 a4ae e0a4 97e0 a58d   ...............
+00000ac0: e0a4 b0e0 a580 20e0 a495 e0a5 8720 e0a4  ...... ...... ..
+00000ad0: b8e0 a4be e0a4 a520 e0a4 abe0 a4bc e0a4  ....... ........
+00000ae0: bee0 a487 e0a4 b220 e0a4 95e0 a58b 20e0  ....... ...... .
+00000af0: a4b8 e0a4 b9e0 a587 e0a4 9ce0 a4a8 e0a5  ................
+00000b00: 8720 e0a4 95e0 a580 20e0 a485 e0a4 a8e0  . ...... .......
+00000b10: a581 e0a4 aee0 a4a4 e0a4 bf20 e0a4 a6e0  ........... ....
+00000b20: a587 e0a4 823f 222c 0a0a 2020 2020 2264  .....?",..    "d
+00000b30: 6961 6c6f 675f 656e 6372 7970 745f 6669  ialog_encrypt_fi
+00000b40: 6c65 5f74 6974 6c65 223a 2022 e0a4 abe0  le_title": "....
+00000b50: a4bc e0a4 bee0 a487 e0a4 b220 e0a4 8fe0  ........... ....
+00000b60: a4a8 e0a5 8de0 a495 e0a5 8de0 a4b0 e0a4  ................
+00000b70: bfe0 a4aa e0a5 8de0 a49f 20e0 a495 e0a4  .......... .....
+00000b80: b0e0 a587 e0a4 8222 2c0a 2020 2020 2264  .......",.    "d
+00000b90: 6961 6c6f 675f 656e 6372 7970 745f 6669  ialog_encrypt_fi
+00000ba0: 6c65 5f74 6578 7422 3a20 22e0 a495 e0a5  le_text": ".....
+00000bb0: 8de0 a4af e0a4 be20 e0a4 86e0 a4aa 20e0  ....... ...... .
+00000bc0: a4b5 e0a4 bee0 a495 e0a4 8820 e0a4 abe0  ........... ....
+00000bd0: a4bc e0a4 bee0 a487 e0a4 b220 5c22 7b66  ........... \"{f
+00000be0: 696c 655f 6e61 6d65 7d5c 2220 e0a4 95e0  ile_name}\" ....
+00000bf0: a58b 20e0 a48f e0a4 a8e0 a58d e0a4 95e0  .. .............
+00000c00: a58d e0a4 b0e0 a4bf e0a4 aae0 a58d e0a4  ................
+00000c10: 9f20 e0a4 95e0 a4b0 e0a4 a8e0 a4be 20e0  . ............ .
+00000c20: a49a e0a4 bee0 a4b9 e0a4 a4e0 a587 20e0  .............. .
+00000c30: a4b9 e0a5 88e0 a482 3f22 2c0a 2020 2020  ........?",.    
+00000c40: 2265 6e63 7279 7074 5f66 696c 655f 7761  "encrypt_file_wa
+00000c50: 726e 696e 675f 6669 6c65 5f69 735f 616c  rning_file_is_al
+00000c60: 7265 6164 795f 656e 6372 7970 7465 6422  ready_encrypted"
+00000c70: 3a20 22e0 a4ab e0a4 bce0 a4be e0a4 87e0  : ".............
+00000c80: a4b2 20e0 a4aa e0a4 b9e0 a4b2 e0a5 8720  .. ............ 
+00000c90: e0a4 b8e0 a587 20e0 a4b9 e0a5 8020 e0a4  ...... ...... ..
+00000ca0: 8fe0 a4a8 e0a5 8de0 a495 e0a5 8de0 a4b0  ................
+00000cb0: e0a4 bfe0 a4aa e0a5 8de0 a49f e0a5 87e0  ................
+00000cc0: a4a1 20e0 a4b9 e0a5 8821 222c 0a20 2020  .. ......!",.   
+00000cd0: 2022 6469 616c 6f67 5f65 6e63 7279 7074   "dialog_encrypt
+00000ce0: 5f66 696c 655f 7265 7772 6974 655f 6578  _file_rewrite_ex
+00000cf0: 6973 7469 6e67 5f74 6974 6c65 223a 2022  isting_title": "
+00000d00: e0a4 aee0 a58c e0a4 9ce0 a582 e0a4 a6e0  ................
+00000d10: a4be 20e0 a4ab e0a4 bce0 a4be e0a4 87e0  .. .............
+00000d20: a4b2 20e0 a495 e0a5 8b20 e0a4 aae0 a581  .. ...... ......
+00000d30: e0a4 a8e0 a483 20e0 a4b2 e0a4 bfe0 a496  ...... .........
+00000d40: e0a5 87e0 a482 222c 0a20 2020 2022 6469  ......",.    "di
+00000d50: 616c 6f67 5f65 6e63 7279 7074 5f66 696c  alog_encrypt_fil
+00000d60: 655f 7265 7772 6974 655f 6578 6973 7469  e_rewrite_existi
+00000d70: 6e67 5f74 6578 7422 3a20 22e0 a495 e0a5  ng_text": ".....
+00000d80: 8de0 a4af e0a4 be20 e0a4 86e0 a4aa 20e0  ....... ...... .
+00000d90: a4b5 e0a4 bee0 a495 e0a4 8820 e0a4 aee0  ........... ....
+00000da0: a58c e0a4 9ce0 a582 e0a4 a6e0 a4be 20e0  .............. .
+00000db0: a4ab e0a4 bce0 a4be e0a4 87e0 a4b2 205c  .............. \
+00000dc0: 227b 6669 6c65 5f70 6174 687d 5c22 20e0  "{file_path}\" .
+00000dd0: a495 e0a5 8b20 e0a4 aae0 a581 e0a4 a8e0  ..... ..........
+00000de0: a483 20e0 a4b2 e0a4 bfe0 a496 e0a4 a8e0  .. .............
+00000df0: a4be 20e0 a49a e0a4 bee0 a4b9 e0a4 a4e0  .. .............
+00000e00: a587 20e0 a4b9 e0a5 88e0 a482 3f22 2c0a  .. .........?",.
+00000e10: 0a20 2020 2022 6469 616c 6f67 5f64 6563  .    "dialog_dec
+00000e20: 7279 7074 5f66 696c 655f 7469 746c 6522  rypt_file_title"
+00000e30: 3a20 22e0 a4ab e0a4 bce0 a4be e0a4 87e0  : ".............
+00000e40: a4b2 20e0 a4a1 e0a4 bfe0 a495 e0a5 8de0  .. .............
+00000e50: a4b0 e0a4 bfe0 a4aa e0a5 8de0 a49f 20e0  .............. .
+00000e60: a495 e0a4 b0e0 a587 e0a4 8222 2c0a 2020  ...........",.  
+00000e70: 2020 2264 6961 6c6f 675f 6465 6372 7970    "dialog_decryp
+00000e80: 745f 6669 6c65 5f74 6578 7422 3a20 22e0  t_file_text": ".
+00000e90: a495 e0a5 8de0 a4af e0a4 be20 e0a4 86e0  ........... ....
+00000ea0: a4aa 20e0 a4b5 e0a4 bee0 a495 e0a4 8820  .. ............ 
+00000eb0: e0a4 abe0 a4bc e0a4 bee0 a487 e0a4 b220  ............... 
+00000ec0: 5c22 7b66 696c 655f 6e61 6d65 7d5c 2220  \"{file_name}\" 
+00000ed0: e0a4 95e0 a58b 20e0 a4a1 e0a4 bfe0 a495  ...... .........
+00000ee0: e0a5 8de0 a4b0 e0a4 bfe0 a4aa e0a5 8de0  ................
+00000ef0: a49f 20e0 a495 e0a4 b0e0 a4a8 e0a4 be20  .. ............ 
+00000f00: e0a4 9ae0 a4be e0a4 b9e0 a4a4 e0a5 8720  ............... 
+00000f10: e0a4 b9e0 a588 e0a4 823f 222c 0a20 2020  .........?",.   
+00000f20: 2022 6465 6372 7970 745f 6669 6c65 5f77   "decrypt_file_w
+00000f30: 6172 6e69 6e67 5f66 696c 655f 6973 5f6e  arning_file_is_n
+00000f40: 6f74 5f65 6e63 7279 7074 6564 223a 2022  ot_encrypted": "
+00000f50: e0a4 abe0 a4bc e0a4 bee0 a487 e0a4 b220  ............... 
+00000f60: e0a4 8fe0 a4a8 e0a5 8de0 a495 e0a5 8de0  ................
+00000f70: a4b0 e0a4 bfe0 a4aa e0a5 8de0 a49f e0a5  ................
+00000f80: 87e0 a4a1 20e0 a4a8 e0a4 b9e0 a580 e0a4  .... ...........
+00000f90: 8220 e0a4 b9e0 a588 2122 2c0a 2020 2020  . ......!",.    
+00000fa0: 2264 6961 6c6f 675f 6465 6372 7970 745f  "dialog_decrypt_
+00000fb0: 6669 6c65 5f72 6577 7269 7465 5f65 7869  file_rewrite_exi
+00000fc0: 7374 696e 675f 7469 746c 6522 3a20 22e0  sting_title": ".
+00000fd0: a4ae e0a5 8ce0 a49c e0a5 82e0 a4a6 e0a4  ................
+00000fe0: be20 e0a4 abe0 a4bc e0a4 bee0 a487 e0a4  . ..............
+00000ff0: b220 e0a4 95e0 a58b 20e0 a4aa e0a5 81e0  . ...... .......
+00001000: a4a8 e0a4 8320 e0a4 b2e0 a4bf e0a4 96e0  ..... ..........
+00001010: a587 e0a4 8222 2c0a 2020 2020 2264 6961  .....",.    "dia
+00001020: 6c6f 675f 6465 6372 7970 745f 6669 6c65  log_decrypt_file
+00001030: 5f72 6577 7269 7465 5f65 7869 7374 696e  _rewrite_existin
+00001040: 675f 7465 7874 223a 2022 e0a4 95e0 a58d  g_text": "......
+00001050: e0a4 afe0 a4be 20e0 a486 e0a4 aa20 e0a4  ...... ...... ..
+00001060: b5e0 a4be e0a4 95e0 a488 20e0 a4ae e0a5  .......... .....
+00001070: 8ce0 a49c e0a5 82e0 a4a6 e0a4 be20 e0a4  ............. ..
+00001080: abe0 a4bc e0a4 bee0 a487 e0a4 b220 5c22  ............. \"
+00001090: 7b66 696c 655f 7061 7468 7d5c 2220 e0a4  {file_path}\" ..
+000010a0: 95e0 a58b 20e0 a4aa e0a5 81e0 a4a8 e0a4  .... ...........
+000010b0: 8320 e0a4 b2e0 a4bf e0a4 96e0 a4a8 e0a4  . ..............
+000010c0: be20 e0a4 9ae0 a4be e0a4 b9e0 a4a4 e0a5  . ..............
+000010d0: 8720 e0a4 b9e0 a588 e0a4 823f 222c 0a0a  . .........?",..
+000010e0: 2020 2020 2264 6961 6c6f 675f 656e 6372      "dialog_encr
+000010f0: 7970 745f 6e65 775f 7061 7373 776f 7264  ypt_new_password
+00001100: 5f74 6974 6c65 223a 2022 e0a4 a8e0 a4af  _title": "......
+00001110: e0a4 be20 e0a4 aae0 a4be e0a4 b8e0 a4b5  ... ............
+00001120: e0a4 b0e0 a58d e0a4 a122 2c0a 2020 2020  .........",.    
+00001130: 2264 6961 6c6f 675f 656e 6372 7970 745f  "dialog_encrypt_
+00001140: 6e65 775f 7061 7373 776f 7264 5f6c 6162  new_password_lab
+00001150: 656c 223a 2022 e0a4 aae0 a4be e0a4 b8e0  el": "..........
+00001160: a4b5 e0a4 b0e0 a58d e0a4 a13a 222c 0a20  ...........:",. 
+00001170: 2020 2022 6469 616c 6f67 5f65 6e63 7279     "dialog_encry
+00001180: 7074 5f6e 6577 5f70 6173 7377 6f72 645f  pt_new_password_
+00001190: 696e 7075 745f 706c 6163 6568 6f6c 6465  input_placeholde
+000011a0: 725f 7465 7874 223a 2022 e0a4 a8e0 a4af  r_text": "......
+000011b0: e0a4 be20 e0a4 aae0 a4be e0a4 b8e0 a4b5  ... ............
+000011c0: e0a4 b0e0 a58d e0a4 a120 e0a4 a6e0 a4b0  ......... ......
+000011d0: e0a5 8de0 a49c 20e0 a495 e0a4 b0e0 a587  ...... .........
+000011e0: e0a4 8222 2c0a 2020 2020 2264 6961 6c6f  ...",.    "dialo
+000011f0: 675f 656e 6372 7970 745f 6e65 775f 7061  g_encrypt_new_pa
+00001200: 7373 776f 7264 5f68 696e 745f 6c61 6265  ssword_hint_labe
+00001210: 6c22 3a20 22e0 a4b8 e0a4 82e0 a495 e0a5  l": "...........
+00001220: 87e0 a4a4 3a22 2c0a 2020 2020 2264 6961  ....:",.    "dia
+00001230: 6c6f 675f 656e 6372 7970 745f 6e65 775f  log_encrypt_new_
+00001240: 7061 7373 776f 7264 5f68 696e 745f 6c61  password_hint_la
+00001250: 6265 6c5f 6465 7363 7269 7074 696f 6e22  bel_description"
+00001260: 3a20 22e0 a4b8 e0a4 82e0 a495 e0a5 87e0  : ".............
+00001270: a4a4 20e0 a48f e0a4 a8e0 a58d e0a4 95e0  .. .............
+00001280: a58d e0a4 b0e0 a4bf e0a4 aae0 a58d e0a4  ................
+00001290: 9fe0 a587 e0a4 a120 e0a4 a8e0 a4b9 e0a5  ....... ........
+000012a0: 80e0 a482 20e0 a4b9 e0a5 8be0 a4a4 e0a4  .... ...........
+000012b0: be20 e0a4 b9e0 a588 20e0 a494 e0a4 b020  . ...... ...... 
+000012c0: e0a4 abe0 a4bc e0a4 bee0 a487 e0a4 b220  ............... 
+000012d0: e0a4 b8e0 a587 20e0 a4aa e0a4 a2e0 a4bc  ...... .........
+000012e0: e0a4 be20 e0a4 9ce0 a4be 20e0 a4b8 e0a4  ... ...... .....
+000012f0: 95e0 a4a4 e0a4 be20 e0a4 b9e0 a588 2122  ....... ......!"
+00001300: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001330: 2020 2020 2020 2020 2020 2022 5c6e e0a4             "\n..
+00001340: 9ce0 a4a8 e0a5 8de0 a4ae 20e0 a4a4 e0a4  .......... .....
+00001350: bfe0 a4a5 e0a4 bfe0 a4af e0a5 8be0 a482  ................
+00001360: 20e0 a49c e0a5 88e0 a4b8 e0a5 8720 e0a4   ............ ..
+00001370: 86e0 a4b8 e0a4 bee0 a4a8 e0a5 8020 e0a4  ............. ..
+00001380: b8e0 a587 20e0 a485 e0a4 a8e0 a581 e0a4  .... ...........
+00001390: aee0 a4be e0a4 a820 e0a4 b2e0 a497 e0a4  ....... ........
+000013a0: bee0 a48f 20e0 a49c e0a4 be20 e0a4 b8e0  .... ...... ....
+000013b0: a495 e0a4 a8e0 a587 20e0 a4b5 e0a4 bee0  ........ .......
+000013c0: a4b2 e0a5 8720 220a 2020 2020 2020 2020  ..... ".        
+000013d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001400: 2020 22e0 a4b8 e0a5 8de0 a4aa e0a4 b7e0    ".............
+00001410: a58d e0a4 9f20 e0a4 b8e0 a482 e0a4 95e0  ..... ..........
+00001420: a587 e0a4 a4e0 a58b e0a4 8220 e0a4 b8e0  ........... ....
+00001430: a587 20e0 a4ac e0a4 9ae0 a587 e0a4 82e0  .. .............
+00001440: a5a4 5c6e e0a4 86e0 a4aa e0a4 95e0 a587  ..\n............
+00001450: 20e0 a4b8 e0a4 bee0 a4a5 20e0 a486 e0a4   ......... .....
+00001460: b8e0 a4be e0a4 a8e0 a580 20e0 a4b8 e0a5  .......... .....
+00001470: 8720 e0a4 9ce0 a581 e0a4 a1e0 a4bc e0a5  . ..............
+00001480: 8720 e0a4 a8e0 a4b9 e0a5 80e0 a482 20e0  . ............ .
+00001490: a49c e0a4 be20 220a 2020 2020 2020 2020  ..... ".        
+000014a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014d0: 2020 22e0 a4b8 e0a4 95e0 a4a8 e0a5 8720    "............ 
+000014e0: e0a4 b5e0 a4be e0a4 b2e0 a587 20e0 a4b8  ............ ...
+000014f0: e0a4 82e0 a4a6 e0a4 b0e0 a58d e0a4 ad20  ............... 
+00001500: e0a4 95e0 a4be 20e0 a4aa e0a5 8de0 a4b0  ...... .........
+00001510: e0a4 afe0 a58b e0a4 9720 e0a4 95e0 a4b0  ......... ......
+00001520: e0a4 a8e0 a587 20e0 a495 e0a4 be20 e0a4  ...... ...... ..
+00001530: aae0 a58d e0a4 b0e0 a4af e0a4 bee0 a4b8  ................
+00001540: 20e0 a495 e0a4 b0e0 a587 e0a4 82e0 a5a4   ...............
+00001550: 222c 0a20 2020 2022 6469 616c 6f67 5f65  ",.    "dialog_e
+00001560: 6e63 7279 7074 5f6e 6577 5f70 6173 7377  ncrypt_new_passw
+00001570: 6f72 645f 6869 6e74 5f69 6e70 7574 5f70  ord_hint_input_p
+00001580: 6c61 6365 686f 6c64 6572 5f74 6578 7422  laceholder_text"
+00001590: 3a20 22e0 a4b8 e0a4 82e0 a495 e0a5 87e0  : ".............
+000015a0: a4a4 20e0 a4a6 e0a4 b0e0 a58d e0a4 9c20  .. ............ 
+000015b0: e0a4 95e0 a4b0 e0a5 87e0 a482 2028 e0a4  ............ (..
+000015c0: b5e0 a588 e0a4 95e0 a4b2 e0a5 8de0 a4aa  ................
+000015d0: e0a4 bfe0 a495 2922 2c0a 2020 2020 2264  ......)",.    "d
+000015e0: 6961 6c6f 675f 656e 6372 7970 745f 6e65  ialog_encrypt_ne
+000015f0: 775f 7061 7373 776f 7264 5f62 7574 746f  w_password_butto
+00001600: 6e5f 6f6b 223a 2022 e0a4 a0e0 a580 e0a4  n_ok": "........
+00001610: 9520 e0a4 b9e0 a588 222c 0a20 2020 2022  . ......",.    "
+00001620: 6469 616c 6f67 5f65 6e63 7279 7074 5f6e  dialog_encrypt_n
+00001630: 6577 5f70 6173 7377 6f72 645f 6275 7474  ew_password_butt
+00001640: 6f6e 5f63 616e 6365 6c22 3a20 22e0 a4b0  on_cancel": "...
+00001650: e0a4 a6e0 a58d e0a4 a620 e0a4 95e0 a4b0  ......... ......
+00001660: e0a5 87e0 a482 222c 0a20 2020 2022 6469  ......",.    "di
+00001670: 616c 6f67 5f65 6e63 7279 7074 5f6e 6577  alog_encrypt_new
+00001680: 5f70 6173 7377 6f72 645f 7761 726e 696e  _password_warnin
+00001690: 675f 656d 7074 795f 7469 746c 6522 3a20  g_empty_title": 
+000016a0: 22e0 a49a e0a5 87e0 a4a4 e0a4 bee0 a4b5  "...............
+000016b0: e0a4 a8e0 a580 222c 0a20 2020 2022 6469  ......",.    "di
+000016c0: 616c 6f67 5f65 6e63 7279 7074 5f6e 6577  alog_encrypt_new
+000016d0: 5f70 6173 7377 6f72 645f 7761 726e 696e  _password_warnin
+000016e0: 675f 656d 7074 795f 7465 7874 223a 2022  g_empty_text": "
+000016f0: e0a4 aae0 a4be e0a4 b8e0 a4b5 e0a4 b0e0  ................
+00001700: a58d e0a4 a120 e0a4 abe0 a4bc e0a5 80e0  ..... ..........
+00001710: a4b2 e0a5 8de0 a4a1 20e0 a496 e0a4 bee0  ........ .......
+00001720: a4b2 e0a5 8020 e0a4 a8e0 a4b9 e0a5 80e0  ..... ..........
+00001730: a482 20e0 a4b9 e0a5 8b20 e0a4 b8e0 a495  .. ...... ......
+00001740: e0a4 a4e0 a580 2122 2c0a 2020 2020 2264  ......!",.    "d
+00001750: 6961 6c6f 675f 656e 6372 7970 745f 6e65  ialog_encrypt_ne
+00001760: 775f 7061 7373 776f 7264 5f77 6172 6e69  w_password_warni
+00001770: 6e67 5f74 6f6f 5f6c 6f6e 675f 7469 746c  ng_too_long_titl
+00001780: 6522 3a20 22e0 a49a e0a5 87e0 a4a4 e0a4  e": "...........
+00001790: bee0 a4b5 e0a4 a8e0 a580 222c 0a20 2020  ..........",.   
+000017a0: 2022 6469 616c 6f67 5f65 6e63 7279 7074   "dialog_encrypt
+000017b0: 5f6e 6577 5f70 6173 7377 6f72 645f 7761  _new_password_wa
+000017c0: 726e 696e 675f 746f 6f5f 6c6f 6e67 5f74  rning_too_long_t
+000017d0: 6578 7422 3a20 22e0 a4b8 e0a4 82e0 a495  ext": ".........
+000017e0: e0a5 87e0 a4a4 20e0 a4ab e0a4 bce0 a580  ...... .........
+000017f0: e0a4 b2e0 a58d e0a4 a120 e0a4 ace0 a4b9  ......... ......
+00001800: e0a5 81e0 a4a4 20e0 a4b2 e0a4 82e0 a4ac  ...... .........
+00001810: e0a5 8020 e0a4 b9e0 a588 2c20 e0a4 85e0  ... ......, ....
+00001820: a4a7 e0a4 bfe0 a495 e0a4 a4e0 a4ae 207b  .............. {
+00001830: 7379 6d62 6f6c 737d 20e0 a485 e0a4 95e0  symbols} .......
+00001840: a58d e0a4 b7e0 a4b0 2122 2c0a 0a20 2020  ........!",..   
+00001850: 2022 6469 616c 6f67 5f65 6e63 7279 7074   "dialog_encrypt
+00001860: 5f70 6173 7377 6f72 645f 7469 746c 6522  _password_title"
+00001870: 3a20 22e0 a4aa e0a4 bee0 a4b8 e0a4 b5e0  : ".............
+00001880: a4b0 e0a5 8de0 a4a1 20e0 a4a6 e0a4 b0e0  ........ .......
+00001890: a58d e0a4 9c20 e0a4 95e0 a4b0 e0a5 87e0  ..... ..........
+000018a0: a482 222c 0a20 2020 2022 6469 616c 6f67  ..",.    "dialog
+000018b0: 5f65 6e63 7279 7074 5f70 6173 7377 6f72  _encrypt_passwor
+000018c0: 645f 6c61 6265 6c22 3a20 22e0 a4aa e0a4  d_label": ".....
+000018d0: bee0 a4b8 e0a4 b5e0 a4b0 e0a5 8de0 a4a1  ................
+000018e0: 3a22 2c0a 2020 2020 2264 6961 6c6f 675f  :",.    "dialog_
+000018f0: 656e 6372 7970 745f 7061 7373 776f 7264  encrypt_password
+00001900: 5f69 6e70 7574 5f70 6c61 6365 686f 6c64  _input_placehold
+00001910: 6572 5f74 6578 7422 3a20 22e0 a4aa e0a4  er_text": ".....
+00001920: bee0 a4b8 e0a4 b5e0 a4b0 e0a5 8de0 a4a1  ................
+00001930: 20e0 a4a6 e0a4 b0e0 a58d e0a4 9c20 e0a4   ............ ..
+00001940: 95e0 a4b0 e0a5 87e0 a482 222c 0a20 2020  ..........",.   
+00001950: 2022 6469 616c 6f67 5f65 6e63 7279 7074   "dialog_encrypt
+00001960: 5f70 6173 7377 6f72 645f 6869 6e74 5f6c  _password_hint_l
+00001970: 6162 656c 223a 2022 e0a4 b8e0 a482 e0a4  abel": "........
+00001980: 95e0 a587 e0a4 a43a 222c 0a20 2020 2022  .......:",.    "
+00001990: 6469 616c 6f67 5f65 6e63 7279 7074 5f70  dialog_encrypt_p
+000019a0: 6173 7377 6f72 645f 6275 7474 6f6e 5f6f  assword_button_o
+000019b0: 6b22 3a20 22e0 a4a0 e0a5 80e0 a495 20e0  k": "......... .
+000019c0: a4b9 e0a5 8822 2c0a 2020 2020 2264 6961  .....",.    "dia
+000019d0: 6c6f 675f 656e 6372 7970 745f 7061 7373  log_encrypt_pass
+000019e0: 776f 7264 5f62 7574 746f 6e5f 6361 6e63  word_button_canc
+000019f0: 656c 223a 2022 e0a4 b0e0 a4a6 e0a5 8de0  el": "..........
+00001a00: a4a6 20e0 a495 e0a4 b0e0 a587 e0a4 8222  .. ............"
+00001a10: 2c0a 0a20 2020 2022 6469 616c 6f67 5f65  ,..    "dialog_e
+00001a20: 6e63 7279 7074 5f70 6173 7377 6f72 645f  ncrypt_password_
+00001a30: 7265 7365 745f 7469 746c 6522 3a20 22e0  reset_title": ".
+00001a40: a48f e0a4 a8e0 a58d e0a4 95e0 a58d e0a4  ................
+00001a50: b0e0 a4bf e0a4 aae0 a58d e0a4 b6e0 a4a8  ................
+00001a60: 20e0 a4aa e0a4 bee0 a4b8 e0a4 b5e0 a4b0   ...............
+00001a70: e0a5 8de0 a4a1 20e0 a4b0 e0a5 80e0 a4b8  ...... .........
+00001a80: e0a5 87e0 a49f 20e0 a495 e0a4 b0e0 a587  ...... .........
+00001a90: e0a4 8222 2c0a 2020 2020 2264 6961 6c6f  ...",.    "dialo
+00001aa0: 675f 656e 6372 7970 745f 7061 7373 776f  g_encrypt_passwo
+00001ab0: 7264 5f72 6573 6574 5f74 6578 7422 3a20  rd_reset_text": 
+00001ac0: 22e0 a495 e0a5 8de0 a4af e0a4 be20 e0a4  "............ ..
+00001ad0: 86e0 a4aa 20e0 a4b5 e0a4 bee0 a495 e0a4  .... ...........
+00001ae0: 8820 e0a4 aee0 a58c e0a4 9ce0 a582 e0a4  . ..............
+00001af0: a6e0 a4be 20e0 a48f e0a4 a8e0 a58d e0a4  .... ...........
+00001b00: 95e0 a58d e0a4 b0e0 a4bf e0a4 aae0 a58d  ................
+00001b10: e0a4 b6e0 a4a8 20e0 a4aa e0a4 bee0 a4b8  ...... .........
+00001b20: e0a4 b5e0 a4b0 e0a5 8de0 a4a1 20e0 a495  ............ ...
+00001b30: e0a5 8b20 e0a4 b0e0 a580 e0a4 b8e0 a587  ... ............
+00001b40: e0a4 9f20 e0a4 95e0 a4b0 e0a4 a8e0 a4be  ... ............
+00001b50: 20e0 a49a e0a4 bee0 a4b9 e0a4 a4e0 a587   ...............
+00001b60: 20e0 a4b9 e0a5 88e0 a482 3f22 2c0a 2020   .........?",.  
+00001b70: 2020 2264 6961 6c6f 675f 656e 6372 7970    "dialog_encryp
+00001b80: 745f 7061 7373 776f 7264 5f72 6573 6574  t_password_reset
+00001b90: 5f62 7574 746f 6e5f 6361 6e63 656c 223a  _button_cancel":
+00001ba0: 2022 e0a4 b0e0 a4a6 e0a5 8de0 a4a6 20e0   "............ .
+00001bb0: a495 e0a4 b0e0 a587 e0a4 8222 2c0a 2020  ...........",.  
+00001bc0: 2020 2264 6961 6c6f 675f 656e 6372 7970    "dialog_encryp
+00001bd0: 745f 7061 7373 776f 7264 5f72 6573 6574  t_password_reset
+00001be0: 5f62 7574 746f 6e5f 7965 7322 3a20 22e0  _button_yes": ".
+00001bf0: a4b9 e0a4 bee0 a481 222c 0a0a 2020 2020  ........",..    
+00001c00: 2264 6961 6c6f 675f 6f70 656e 5f6c 696e  "dialog_open_lin
+00001c10: 6b5f 7469 746c 6522 3a20 22e0 a4b2 e0a4  k_title": ".....
+00001c20: bfe0 a482 e0a4 9522 2c0a 2020 2020 2264  .......",.    "d
+00001c30: 6961 6c6f 675f 6f70 656e 5f6c 696e 6b5f  ialog_open_link_
+00001c40: 7465 7874 223a 2022 e0a4 b2e0 a4bf e0a4  text": "........
+00001c50: 82e0 a495 205c 227b 7572 6c7d 5c22 20e0  .... \"{url}\" .
+00001c60: a495 e0a5 8b20 e0a4 ace0 a58d e0a4 b0e0  ..... ..........
+00001c70: a4be e0a4 89e0 a49c e0a4 bce0 a4b0 20e0  .............. .
+00001c80: a4ae e0a5 87e0 a482 20e0 a496 e0a5 8be0  ........ .......
+00001c90: a4b2 e0a5 87e0 a482 3f22 2c0a 0a20 2020  ........?",..   
+00001ca0: 2022 6c6f 6164 5f66 696c 655f 656e 6372   "load_file_encr
+00001cb0: 7970 7469 6f6e 5f70 6173 7377 6f72 645f  yption_password_
+00001cc0: 6d69 736d 6174 6368 223a 2022 e0a4 8fe0  mismatch": "....
+00001cd0: a4a8 e0a5 8de0 a495 e0a5 8de0 a4b0 e0a4  ................
+00001ce0: bfe0 a4aa e0a5 8de0 a4b6 e0a4 a820 e0a4  ............. ..
+00001cf0: aae0 a4be e0a4 b8e0 a4b5 e0a4 b0e0 a58d  ................
+00001d00: e0a4 a120 e0a4 aee0 a587 e0a4 b220 e0a4  ... ......... ..
+00001d10: a8e0 a4b9 e0a5 80e0 a482 20e0 a496 e0a4  .......... .....
+00001d20: bee0 a4a4 e0a4 be21 222c 0a20 2020 2022  .......!",.    "
+00001d30: 6c6f 6164 5f66 696c 655f 656e 6372 7970  load_file_encryp
+00001d40: 7469 6f6e 5f70 6173 7377 6f72 645f 696e  tion_password_in
+00001d50: 636f 7272 6563 7422 3a20 22e0 a48f e0a4  correct": ".....
+00001d60: a8e0 a58d e0a4 95e0 a58d e0a4 b0e0 a4bf  ................
+00001d70: e0a4 aae0 a58d e0a4 b6e0 a4a8 20e0 a4aa  ............ ...
+00001d80: e0a4 bee0 a4b8 e0a4 b5e0 a4b0 e0a5 8de0  ................
+00001d90: a4a1 20e0 a497 e0a4 b2e0 a4a4 20e0 a4b9  .. ......... ...
+00001da0: e0a5 8821 222c 0a20 2020 2022 6c6f 6164  ...!",.    "load
+00001db0: 5f66 696c 655f 6e6f 6e65 5f63 6f6e 7465  _file_none_conte
+00001dc0: 6e74 5f65 7272 6f72 223a 2022 e0a4 abe0  nt_error": "....
+00001dd0: a4bc e0a4 bee0 a487 e0a4 b220 e0a4 b2e0  ........... ....
+00001de0: a58b e0a4 a120 e0a4 a8e0 a4b9 e0a5 80e0  ..... ..........
+00001df0: a482 20e0 a495 e0a5 8020 e0a4 9ce0 a4be  .. ...... ......
+00001e00: 20e0 a4b8 e0a4 95e0 a4a4 e0a5 80e0 a5a4   ...............
+00001e10: 222c 0a0a 2020 2020 2273 6176 655f 6163  ",..    "save_ac
+00001e20: 7469 7665 5f66 696c 655f 6572 726f 725f  tive_file_error_
+00001e30: 6f63 6375 7272 6564 223a 2022 e0a4 abe0  occurred": "....
+00001e40: a4bc e0a4 bee0 a487 e0a4 b220 e0a4 b8e0  ........... ....
+00001e50: a4b9 e0a5 87e0 a49c e0a4 a8e0 a587 20e0  .............. .
+00001e60: a4ae e0a5 87e0 a482 20e0 a485 e0a4 b8e0  ........ .......
+00001e70: a4ae e0a4 b0e0 a58d e0a4 a52c 20e0 a4a4  ..........., ...
+00001e80: e0a5 8de0 a4b0 e0a5 81e0 a49f e0a4 bf20  ............... 
+00001e90: e0a4 b9e0 a581 e0a4 8820 e0a4 b9e0 a588  ......... ......
+00001ea0: 222c 0a0a 2020 2020 2265 7870 616e 6461  ",..    "expanda
+00001eb0: 626c 655f 626c 6f63 6b5f 6465 6661 756c  ble_block_defaul
+00001ec0: 745f 7469 746c 6522 3a20 22e0 a485 e0a4  t_title": ".....
+00001ed0: a7e0 a4bf e0a4 9520 e0a4 9ce0 a4be e0a4  ....... ........
+00001ee0: a8e0 a495 e0a4 bee0 a4b0 e0a5 802e 2e2e  ................
+00001ef0: 222c 0a0a 2020 2020 2264 6961 6c6f 675f  ",..    "dialog_
+00001f00: 636f 6c6f 725f 7069 636b 6572 5f63 6f6c  color_picker_col
+00001f10: 6f72 5f63 6f70 6965 645f 746f 5f74 6865  or_copied_to_the
+00001f20: 5f63 6c69 7062 6f61 7264 223a 2022 e0a4  _clipboard": "..
+00001f30: b8e0 a58d e0a4 b5e0 a4b0 e0a5 82e0 a4aa  ................
+00001f40: e0a4 bfe0 a4a4 20e0 a4aa e0a4 bee0 a4a0  ...... .........
+00001f50: 20e0 a495 e0a5 8de0 a4b2 e0a4 bfe0 a4aa   ...............
+00001f60: e0a4 ace0 a58b e0a4 b0e0 a58d e0a4 a120  ............... 
+00001f70: e0a4 aee0 a587 e0a4 8220 e0a4 95e0 a589  ......... ......
+00001f80: e0a4 aae0 a580 20e0 a495 e0a4 bfe0 a4af  ...... .........
+00001f90: e0a4 be20 e0a4 97e0 a4af e0a4 be20 e0a4  ... ......... ..
+00001fa0: b9e0 a588 222c 0a0a 2020 2020 2270 6f70  ....",..    "pop
+00001fb0: 7570 5f61 626f 7574 5f74 6974 6c65 223a  up_about_title":
+00001fc0: 2022 e0a4 8fe0 a4aa e0a5 8de0 a4b2 e0a4   "..............
+00001fd0: bfe0 a495 e0a5 87e0 a4b6 e0a4 a820 e0a4  ............. ..
+00001fe0: 95e0 a580 20e0 a49c e0a4 bee0 a4a8 e0a4  .... ...........
+00001ff0: 95e0 a4be e0a4 b0e0 a580 222c 0a20 2020  ..........",.   
+00002000: 2022 706f 7075 705f 6162 6f75 745f 6170   "popup_about_ap
+00002010: 705f 6e61 6d65 5f64 6573 6372 6970 7469  p_name_descripti
+00002020: 6f6e 223a 2022 e0a4 aae0 a4be e0a4 afe0  on": "..........
+00002030: a4a5 e0a4 a820 e0a4 aee0 a4be e0a4 b0e0  ..... ..........
+00002040: a58d e0a4 95e0 a4a1 e0a4 bee0 a489 e0a4  ................
+00002050: a820 e0a4 8fe0 a4a1 e0a4 bfe0 a49f e0a4  . ..............
+00002060: b022 2c0a 0a20 2020 2022 706f 7075 705f  .",..    "popup_
+00002070: 6162 6f75 745f 7665 7273 696f 6e22 3a20  about_version": 
+00002080: 22e0 a4b8 e0a4 82e0 a4b8 e0a5 8de0 a495  "...............
+00002090: e0a4 b0e0 a4a3 222c 0a20 2020 2022 706f  ......",.    "po
+000020a0: 7075 705f 6162 6f75 745f 6c69 6365 6e73  pup_about_licens
+000020b0: 6522 3a20 22e0 a4b2 e0a4 bee0 a487 e0a4  e": "...........
+000020c0: b8e0 a587 e0a4 82e0 a4b8 222c 0a20 2020  ..........",.   
+000020d0: 2022 706f 7075 705f 6162 6f75 745f 7765   "popup_about_we
+000020e0: 6273 6974 6522 3a20 22e0 a4b5 e0a5 87e0  bsite": ".......
+000020f0: a4ac e0a4 b8e0 a4be e0a4 87e0 a49f 222c  ..............",
+00002100: 0a20 2020 2022 706f 7075 705f 6162 6f75  .    "popup_abou
+00002110: 745f 7265 706f 7369 746f 7279 223a 2022  t_repository": "
+00002120: e0a4 97e0 a4bf e0a4 9fe0 a4b9 e0a4 ac22  ..............."
+00002130: 2c0a 2020 2020 2270 6f70 7570 5f61 626f  ,.    "popup_abo
+00002140: 7574 5f70 7970 6922 3a20 22e0 a4aa e0a4  ut_pypi": ".....
+00002150: bee0 a487 e0a4 aae0 a580 222c 0a20 2020  ..........",.   
+00002160: 2022 706f 7075 705f 6162 6f75 745f 6461   "popup_about_da
+00002170: 7465 223a 2022 e0a4 a4e0 a4be e0a4 b0e0  te": "..........
+00002180: a580 e0a4 9622 2c0a 0a20 2020 2022 7570  .....",..    "up
+00002190: 6461 7465 5f68 656c 7065 725f 6e65 775f  date_helper_new_
+000021a0: 7665 7273 696f 6e5f 6973 5f61 7661 696c  version_is_avail
+000021b0: 6162 6c65 223a 2022 e0a4 90e0 a4aa 20e0  able": "...... .
+000021c0: a495 e0a4 be20 e0a4 a8e0 a4af e0a4 be20  ..... ......... 
+000021d0: e0a4 b8e0 a482 e0a4 b8e0 a58d e0a4 95e0  ................
+000021e0: a4b0 e0a4 a320 277b 6c61 7465 7374 5f76  ..... '{latest_v
+000021f0: 6572 7369 6f6e 7d27 20e0 a489 e0a4 aae0  ersion}' .......
+00002200: a4b2 e0a4 ace0 a58d e0a4 a720 e0a4 b9e0  ........... ....
+00002210: a588 222c 0a20 2020 2022 7570 6461 7465  ..",.    "update
+00002220: 5f68 656c 7065 725f 6c61 7465 7374 5f76  _helper_latest_v
+00002230: 6572 7369 6f6e 5f69 6e73 7461 6c6c 6564  ersion_installed
+00002240: 223a 2022 e0a4 90e0 a4aa 20e0 a495 e0a4  ": "...... .....
+00002250: be20 e0a4 a8e0 a4b5 e0a5 80e0 a4a8 e0a4  . ..............
+00002260: a4e0 a4ae 20e0 a4b8 e0a4 82e0 a4b8 e0a5  .... ...........
+00002270: 8de0 a495 e0a4 b0e0 a4a3 20e0 a4b8 e0a5  .......... .....
+00002280: 8de0 a4a5 e0a4 bee0 a4aa e0a4 bfe0 a4a4  ................
+00002290: 20e0 a4b9 e0a5 8822 2c0a 0a20 2020 2022   ......",..    "
+000022a0: 6e65 7477 6f72 6b5f 636f 6e6e 6563 7469  network_connecti
+000022b0: 6f6e 5f65 7272 6f72 5f65 6d70 7479 223a  on_error_empty":
+000022c0: 2022 e0a4 aae0 a58d e0a4 b0e0 a4a4 e0a4   "..............
+000022d0: bfe0 a495 e0a5 8de0 a4b0 e0a4 bfe0 a4af  ................
+000022e0: e0a4 be20 e0a4 9ce0 a4be e0a4 a8e0 a495  ... ............
+000022f0: e0a4 bee0 a4b0 e0a5 8020 e0a4 aae0 a58d  ......... ......
+00002300: e0a4 b0e0 a4be e0a4 aae0 a58d e0a4 a420  ............... 
+00002310: e0a4 95e0 a4b0 e0a4 a8e0 a587 20e0 a4ae  ............ ...
+00002320: e0a5 87e0 a482 20e0 a485 e0a4 b8e0 a4ae  ...... .........
+00002330: e0a4 b0e0 a58d e0a4 a522 2c0a 2020 2020  .........",.    
+00002340: 226e 6574 776f 726b 5f63 6f6e 6e65 6374  "network_connect
+00002350: 696f 6e5f 6572 726f 725f 636f 6e6e 6563  ion_error_connec
+00002360: 7469 6f6e 5f6f 725f 646e 7322 3a20 22e0  tion_or_dns": ".
+00002370: a4b9 e0a5 8be0 a4b8 e0a5 8de0 a49f 20e0  .............. .
+00002380: a4a8 e0a4 b9e0 a580 e0a4 8220 e0a4 aee0  ........... ....
+00002390: a4bf e0a4 b2e0 a4be e0a5 a420 e0a4 87e0  ........... ....
+000023a0: a482 e0a4 9fe0 a4b0 e0a4 a8e0 a587 e0a4  ................
+000023b0: 9f20 e0a4 95e0 a4a8 e0a5 87e0 a495 e0a5  . ..............
+000023c0: 8de0 a4b6 e0a4 a820 e0a4 afe0 a4be 2044  ....... ...... D
+000023d0: 4e53 20e0 a4ae e0a5 87e0 a482 20e0 a4b8  NS ......... ...
+000023e0: e0a4 aee0 a4b8 e0a5 8de0 a4af e0a4 be20  ............... 
+000023f0: e0a4 b9e0 a58b 20e0 a4b8 e0a4 95e0 a4a4  ...... .........
+00002400: e0a5 8020 e0a4 b9e0 a588 e0a5 a422 2c0a  ... .........",.
+00002410: 2020 2020 226e 6574 776f 726b 5f63 6f6e      "network_con
+00002420: 6e65 6374 696f 6e5f 6572 726f 725f 636f  nection_error_co
+00002430: 6e6e 6563 7469 6f6e 5f72 6566 7573 6564  nnection_refused
+00002440: 223a 0a20 2020 2020 2020 2022 e0a4 95e0  ":.        "....
+00002450: a4a8 e0a5 87e0 a495 e0a5 8de0 a4b6 e0a4  ................
+00002460: a820 e0a4 85e0 a4b8 e0a5 8de0 a4b5 e0a5  . ..............
+00002470: 80e0 a495 e0a5 83e0 a4a4 20e0 a495 e0a4  .......... .....
+00002480: bfe0 a4af e0a4 be20 e0a4 97e0 a4af e0a4  ....... ........
+00002490: bee0 a5a4 20e0 a4b8 e0a4 b0e0 a58d e0a4  .... ...........
+000024a0: b5e0 a4b0 20e0 a4ac e0a4 82e0 a4a6 20e0  .... ......... .
+000024b0: a4b9 e0a5 8b20 e0a4 b8e0 a495 e0a4 a4e0  ..... ..........
+000024c0: a4be 20e0 a4b9 e0a5 882c 20e0 a4af e0a4  .. ......, .....
+000024d0: be20 e0a4 a8e0 a587 e0a4 9fe0 a4b5 e0a4  . ..............
+000024e0: b0e0 a58d e0a4 9520 e0a4 aee0 a587 e0a4  ....... ........
+000024f0: 8220 e0a4 b8e0 a4ae e0a4 b8e0 a58d e0a4  . ..............
+00002500: afe0 a4be 20e0 a4b9 e0a5 8b20 e0a4 b8e0  .... ...... ....
+00002510: a495 e0a4 a4e0 a580 20e0 a4b9 e0a5 88e0  ........ .......
+00002520: a5a4 222c 0a20 2020 2022 6e65 7477 6f72  ..",.    "networ
+00002530: 6b5f 636f 6e6e 6563 7469 6f6e 5f65 7272  k_connection_err
+00002540: 6f72 5f63 6f6e 6e65 6374 696f 6e5f 7469  or_connection_ti
+00002550: 6d65 645f 6f75 7422 3a20 22e0 a495 e0a4  med_out": ".....
+00002560: a8e0 a587 e0a4 95e0 a58d e0a4 b6e0 a4a8  ................
+00002570: 20e0 a495 e0a4 be20 e0a4 b8e0 a4ae e0a4   ...... ........
+00002580: af20 e0a4 b8e0 a4ae e0a4 bee0 a4aa e0a5  . ..............
+00002590: 8de0 a4a4 20e0 a4b9 e0a5 8b20 e0a4 97e0  .... ...... ....
+000025a0: a4af e0a4 bee0 a5a4 20e0 a4a8 e0a5 87e0  ........ .......
+000025b0: a49f e0a4 b5e0 a4b0 e0a5 8de0 a495 20e0  .............. .
+000025c0: a4ae e0a5 87e0 a482 20e0 a4b8 e0a4 aee0  ........ .......
+000025d0: a4b8 e0a5 8de0 a4af e0a4 be20 e0a4 b9e0  ........... ....
+000025e0: a58b 20e0 a4b8 e0a4 95e0 a4a4 e0a5 8020  .. ............ 
+000025f0: e0a4 b9e0 a588 e0a5 a422 2c0a 2020 2020  .........",.    
+00002600: 226e 6574 776f 726b 5f63 6f6e 6e65 6374  "network_connect
+00002610: 696f 6e5f 6572 726f 725f 636f 6e6e 6563  ion_error_connec
+00002620: 7469 6f6e 5f34 3034 5f65 7272 6f72 223a  tion_404_error":
+00002630: 2022 e0a4 95e0 a4a8 e0a5 87e0 a495 e0a5   "..............
+00002640: 8de0 a4b6 e0a4 a820 3430 3420 e0a4 a4e0  ....... 404 ....
+00002650: a58d e0a4 b0e0 a581 e0a4 9fe0 a4bf e0a5  ................
+00002660: a420 e0a4 85e0 a4a8 e0a5 81e0 a4b0 e0a5  . ..............
+00002670: 8be0 a4a7 e0a4 bfe0 a4a4 20e0 a4aa e0a5  .......... .....
+00002680: 83e0 a4b7 e0a5 8de0 a4a0 20e0 a4af e0a4  .......... .....
+00002690: be20 e0a4 b8e0 a482 e0a4 b8e0 a4be e0a4  . ..............
+000026a0: a7e0 a4a8 20e0 a4a8 e0a4 b9e0 a580 e0a4  .... ...........
+000026b0: 8220 e0a4 aee0 a4bf e0a4 b2e0 a4be e0a5  . ..............
+000026c0: a422 2c0a 2020 2020 226e 6574 776f 726b  .",.    "network
+000026d0: 5f63 6f6e 6e65 6374 696f 6e5f 6572 726f  _connection_erro
+000026e0: 725f 6765 6e65 7269 635f 7769 7468 5f73  r_generic_with_s
+000026f0: 7461 7475 735f 636f 6465 223a 2022 e0a4  tatus_code": "..
+00002700: b8e0 a58d e0a4 a5e0 a4bf e0a4 a4e0 a4bf  ................
+00002710: 20e0 a495 e0a5 8be0 a4a1 20e0 a495 e0a5   ......... .....
+00002720: 8720 e0a4 b8e0 a4be e0a4 a520 e0a4 85e0  . ......... ....
+00002730: a4a8 e0a5 81e0 a4b0 e0a5 8be0 a4a7 20e0  .............. .
+00002740: a4b5 e0a4 bfe0 a4ab e0a4 b23a 207b 7374  ...........: {st
+00002750: 6174 7573 5f63 6f64 657d 220a 7d0a       atus_code}".}.
```

### Comparing `notolog-0.9.1b1/app/lexemes/in/__pycache__/settings_dialog.cpython-39.pyc` & `notolog-0.9.1b2/notolog/lexemes/in/settings_dialog.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,350 +1,347 @@
-00000000: 610d 0d0a 0000 0000 42a9 3566 aa15 0000  a.......B.5f....
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0030 0000 0040 0000 0073 6800 0000 6400  .0...@...sh...d.
-00000030: 6401 6402 6403 6404 6405 6406 6407 6408  d.d.d.d.d.d.d.d.
-00000040: 6409 640a 640b 640c 640d 640e 640f 6410  d.d.d.d.d.d.d.d.
-00000050: 6411 6412 6413 6414 6415 6416 6417 6418  d.d.d.d.d.d.d.d.
-00000060: 6419 641a 641b 641c 641d 641e 641f 6420  d.d.d.d.d.d.d.d 
-00000070: 6421 6422 6423 6424 6425 6426 6427 6428  d!d"d#d$d%d&d'd(
-00000080: 6429 642a 642b 642c 642d 642e 642f 9c2f  d)d*d+d,d-d.d/./
-00000090: 5a00 6430 5300 2931 7518 0000 00e0 a4b8  Z.d0S.)1u.......
-000000a0: e0a5 87e0 a49f e0a4 bfe0 a482 e0a4 97e0  ................
-000000b0: a58d e0a4 b875 1600 0000 e0a4 ace0 a482  .....u..........
-000000c0: e0a4 a620 e0a4 95e0 a4b0 e0a5 87e0 a482  ... ............
-000000d0: 7515 0000 00e0 a4b8 e0a4 bee0 a4ae e0a4  u...............
-000000e0: bee0 a4a8 e0a5 8de0 a4af 7512 0000 00e0  ..........u.....
-000000f0: a4b8 e0a4 82e0 a4aa e0a4 bee0 a4a6 e0a4  ................
-00000100: 9575 0f00 0000 e0a4 a6e0 a4b0 e0a5 8de0  .u..............
-00000110: a4b6 e0a4 9575 2200 0000 e0a4 8fe0 a486  .....u".........
-00000120: e0a4 8820 e0a4 95e0 a589 e0a4 a8e0 a58d  ... ............
-00000130: e0a4 abe0 a4bc e0a4 bfe0 a497 7534 0000  ............u4..
-00000140: 00e0 a48f e0a4 aae0 a58d e0a4 b2e0 a4bf  ................
-00000150: e0a4 95e0 a587 e0a4 b6e0 a4a8 20e0 a495  ............ ...
-00000160: e0a5 89e0 a4a8 e0a5 8de0 a4ab e0a4 bce0  ................
-00000170: a4bf e0a4 9775 0c00 0000 e0a4 ade0 a4be  .....u..........
-00000180: e0a4 b7e0 a4be 7523 0000 00e0 a48f e0a4  ......u#........
-00000190: 9520 e0a4 ade0 a4be e0a4 b7e0 a4be 20e0  . ............ .
-000001a0: a49a e0a5 81e0 a4a8 e0a5 87e0 a482 7548  ..............uH
-000001b0: 0000 00e0 a48f e0a4 aae0 a58d e0a4 b2e0  ................
-000001c0: a4bf e0a4 95e0 a587 e0a4 b6e0 a4a8 20e0  .............. .
-000001d0: a495 e0a5 8020 e0a4 87e0 a482 e0a4 9fe0  ..... ..........
-000001e0: a4b0 e0a4 abe0 a4bc e0a5 87e0 a4b8 20e0  .............. .
-000001f0: a4ad e0a4 bee0 a4b7 e0a4 be75 0900 0000  ...........u....
-00000200: e0a4 a5e0 a580 e0a4 ae75 2000 0000 e0a4  .........u .....
-00000210: 8fe0 a495 20e0 a4a5 e0a5 80e0 a4ae 20e0  .... ......... .
-00000220: a49a e0a5 81e0 a4a8 e0a5 87e0 a482 7545  ..............uE
-00000230: 0000 00e0 a48f e0a4 aae0 a58d e0a4 b2e0  ................
-00000240: a4bf e0a4 95e0 a587 e0a4 b6e0 a4a8 20e0  .............. .
-00000250: a495 e0a5 8020 e0a4 87e0 a482 e0a4 9fe0  ..... ..........
-00000260: a4b0 e0a4 abe0 a4bc e0a5 87e0 a4b8 20e0  .............. .
-00000270: a4a5 e0a5 80e0 a4ae 751c 0000 00e0 a4ae  ........u.......
-00000280: e0a5 81e0 a496 e0a5 8de0 a4af 20e0 a4ae  ............ ...
-00000290: e0a5 87e0 a4a8 e0a5 8275 2f00 0000 e0a4  .........u/.....
-000002a0: aee0 a581 e0a4 96e0 a58d e0a4 af20 e0a4  ............. ..
-000002b0: aee0 a587 e0a4 a8e0 a582 20e0 a4a6 e0a4  .......... .....
-000002c0: bfe0 a496 e0a4 bee0 a48f e0a4 8275 5900  .............uY.
-000002d0: 0000 e0a4 90e0 a4aa 20e0 a495 e0a4 be20  ........ ...... 
-000002e0: e0a4 aee0 a581 e0a4 96e0 a58d e0a4 af20  ............... 
-000002f0: e0a4 a1e0 a58d e0a4 b0e0 a589 e0a4 aae0  ................
-00000300: a4a1 e0a4 bee0 a489 e0a4 a820 e0a4 aee0  ........... ....
-00000310: a587 e0a4 a8e0 a582 20e0 a4a6 e0a4 bfe0  ........ .......
-00000320: a496 e0a4 bee0 a48f e0a4 8275 3400 0000  ...........u4...
-00000330: e0a4 abe0 a4bc e0a5 89e0 a4a8 e0a5 8de0  ................
-00000340: a49f 20e0 a486 e0a4 95e0 a4be e0a4 b03a  .. ............:
-00000350: 207b 7369 7a65 7d20 e0a4 aae0 a580 e0a4   {size} ........
-00000360: 9fe0 a580 7569 0000 00e0 a490 e0a4 aa20  ....ui......... 
-00000370: e0a4 95e0 a4be 20e0 a4b5 e0a5 88e0 a4b6  ...... .........
-00000380: e0a5 8de0 a4b5 e0a4 bfe0 a495 20e0 a4ab  ............ ...
-00000390: e0a4 bce0 a589 e0a4 a8e0 a58d e0a4 9f20  ............... 
-000003a0: e0a4 86e0 a495 e0a4 bee0 a4b0 20e0 a4b8  ............ ...
-000003b0: e0a4 aee0 a4be e0a4 afe0 a58b e0a4 9ce0  ................
-000003c0: a4bf e0a4 a420 e0a4 95e0 a4b0 e0a5 87e0  ..... ..........
-000003d0: a482 7522 0000 00e0 a4b8 e0a5 8de0 a4a5  ..u"............
-000003e0: e0a4 bfe0 a4a4 e0a4 bf20 e0a4 aae0 a49f  ......... ......
-000003f0: e0a5 8de0 a49f e0a5 8075 4800 0000 e0a4  .........uH.....
-00000400: 97e0 a58d e0a4 b2e0 a58b e0a4 ace0 a4b2  ................
-00000410: 20e0 a495 e0a4 b0e0 a58d e0a4 b8e0 a4b0   ...............
-00000420: 20e0 a4b8 e0a5 8de0 a4a5 e0a4 bfe0 a4a4   ...............
-00000430: e0a4 bf20 e0a4 a6e0 a4bf e0a4 96e0 a4be  ... ............
-00000440: e0a4 8fe0 a482 7575 0000 00e0 a4b8 e0a5  ......uu........
-00000450: 8de0 a4a5 e0a4 bfe0 a4a4 e0a4 bf20 e0a4  ............. ..
-00000460: aae0 a49f e0a5 8de0 a49f e0a5 8020 e0a4  ............. ..
-00000470: aee0 a587 e0a4 8220 e0a4 97e0 a58d e0a4  ....... ........
-00000480: b2e0 a58b e0a4 ace0 a4b2 20e0 a495 e0a4  .......... .....
-00000490: b0e0 a58d e0a4 b8e0 a4b0 20e0 a4b8 e0a5  .......... .....
-000004a0: 8de0 a4a5 e0a4 bfe0 a4a4 e0a4 bf20 e0a4  ............. ..
-000004b0: a6e0 a4bf e0a4 96e0 a4be e0a4 8fe0 a482  ................
-000004c0: 7537 0000 00e0 a4b8 e0a4 82e0 a4aa e0a4  u7..............
-000004d0: bee0 a4a6 e0a4 9520 e0a4 95e0 a589 e0a4  ....... ........
-000004e0: a8e0 a58d e0a4 abe0 a4bc e0a4 bfe0 a497  ................
-000004f0: e0a4 b0e0 a587 e0a4 b6e0 a4a8 7538 0000  ............u8..
-00000500: 00e0 a4b2 e0a4 bee0 a487 e0a4 a820 e0a4  ............. ..
-00000510: b8e0 a482 e0a4 96e0 a58d e0a4 afe0 a4be  ................
-00000520: e0a4 8fe0 a481 20e0 a4a6 e0a4 bfe0 a496  ...... .........
-00000530: e0a4 bee0 a48f e0a4 8275 5500 0000 e0a4  .........uU.....
-00000540: b8e0 a482 e0a4 aae0 a4be e0a4 a6e0 a495  ................
-00000550: 20e0 a4ae e0a5 87e0 a482 20e0 a4b2 e0a4   ......... .....
-00000560: bee0 a487 e0a4 a820 e0a4 b8e0 a482 e0a4  ....... ........
-00000570: 96e0 a58d e0a4 afe0 a4be e0a4 8fe0 a481  ................
-00000580: 20e0 a4a6 e0a4 bfe0 a496 e0a4 bee0 a48f   ...............
-00000590: e0a4 8275 3400 0000 e0a4 a6e0 a4b0 e0a5  ...u4...........
-000005a0: 8de0 a4b6 e0a4 9520 e0a4 95e0 a589 e0a4  ....... ........
-000005b0: a8e0 a58d e0a4 abe0 a4bc e0a4 bfe0 a497  ................
-000005c0: e0a4 b0e0 a587 e0a4 b6e0 a4a8 7569 0000  ............ui..
-000005d0: 00e0 a4aa e0a4 bee0 a4a0 20e0 a487 e0a4  .......... .....
-000005e0: aee0 a58b e0a4 9ce0 a580 20e0 a495 e0a5  .......... .....
-000005f0: 8b20 e0a4 97e0 a58d e0a4 b0e0 a4be e0a4  . ..............
-00000600: abe0 a4bf e0a4 9520 e0a4 aee0 a587 e0a4  ....... ........
-00000610: 8220 e0a4 aae0 a4b0 e0a4 bfe0 a4b5 e0a4  . ..............
-00000620: b0e0 a58d e0a4 a4e0 a4bf e0a4 a420 e0a4  ............. ..
-00000630: 95e0 a4b0 e0a5 87e0 a482 7585 0000 00e0  ..........u.....
-00000640: a4aa e0a4 bee0 a4a0 20e0 a487 e0a4 aee0  ........ .......
-00000650: a58b e0a4 9ce0 a580 20e0 a495 e0a5 8b20  ........ ...... 
-00000660: e0a4 9ae0 a4bf e0a4 a4e0 a58d e0a4 b0e0  ................
-00000670: a4bf e0a4 a420 e0a4 aae0 a58d e0a4 b0e0  ..... ..........
-00000680: a4a4 e0a4 bfe0 a4a8 e0a4 bfe0 a4a7 e0a4  ................
-00000690: bf20 e0a4 aee0 a587 e0a4 8220 e0a4 aae0  . ......... ....
-000006a0: a4b0 e0a4 bfe0 a4b5 e0a4 b0e0 a58d e0a4  ................
-000006b0: a4e0 a4bf e0a4 a420 e0a4 95e0 a4b0 e0a5  ....... ........
-000006c0: 87e0 a482 752e 0000 0054 4f44 4f20 e0a4  ....u....TODO ..
-000006d0: 95e0 a58b 20e0 a4b9 e0a4 bee0 a487 e0a4  .... ...........
-000006e0: b2e0 a4be e0a4 87e0 a49f 20e0 a495 e0a4  .......... .....
-000006f0: b0e0 a587 e0a4 8275 5800 0000 e0a4 aae0  .......uX.......
-00000700: a4be e0a4 a020 e0a4 aee0 a587 e0a4 8220  ..... ......... 
-00000710: 544f 444f 20e0 a49f e0a5 88e0 a497 20e0  TODO ......... .
-00000720: a495 e0a5 8b20 e0a4 aee0 a4b9 e0a4 a4e0  ..... ..........
-00000730: a58d e0a4 b5e0 a4aa e0a5 82e0 a4b0 e0a5  ................
-00000740: 8de0 a4a3 20e0 a4ac e0a4 a8e0 a4be e0a4  .... ...........
-00000750: 8fe0 a482 7560 0000 00e0 a4b2 e0a4 bfe0  ....u`..........
-00000760: a482 e0a4 9520 e0a4 96e0 a58b e0a4 b2e0  ..... ..........
-00000770: a4a8 e0a5 8720 e0a4 95e0 a587 20e0 a4b2  ..... ...... ...
-00000780: e0a4 bfe0 a48f 20e0 a4aa e0a5 81e0 a4b7  ...... .........
-00000790: e0a5 8de0 a49f e0a4 bf20 e0a4 95e0 a580  ......... ......
-000007a0: 20e0 a486 e0a4 b5e0 a4b6 e0a5 8de0 a4af   ...............
-000007b0: e0a4 95e0 a4a4 e0a4 be75 6a00 0000 e0a4  .........uj.....
-000007c0: b2e0 a4bf e0a4 82e0 a495 20e0 a496 e0a5  .......... .....
-000007d0: 8be0 a4b2 e0a4 a8e0 a587 20e0 a4b8 e0a5  .......... .....
-000007e0: 8720 e0a4 aae0 a4b9 e0a4 b2e0 a587 20e0  . ............ .
-000007f0: a4aa e0a5 81e0 a4b7 e0a5 8de0 a49f e0a4  ................
-00000800: bf20 e0a4 95e0 a580 20e0 a486 e0a4 b5e0  . ...... .......
-00000810: a4b6 e0a5 8de0 a4af e0a4 95e0 a4a4 e0a4  ................
-00000820: be20 e0a4 b9e0 a588 7580 0000 00e0 a4ac  . ......u.......
-00000830: e0a4 bee0 a4b9 e0a4 b0e0 a580 20e0 a49b  ............ ...
-00000840: e0a4 b5e0 a4bf e0a4 afe0 a58b e0a4 8220  ............... 
-00000850: e0a4 95e0 a58b 20e0 a4a1 e0a4 bfe0 a4b8  ...... .........
-00000860: e0a5 8de0 a495 20e0 a4ae e0a5 87e0 a482  ...... .........
-00000870: 20e0 a4b8 e0a5 8de0 a4b5 e0a4 9ae0 a4be   ...............
-00000880: e0a4 b2e0 a4bf e0a4 a420 e0a4 b0e0 a582  ......... ......
-00000890: e0a4 aa20 e0a4 b8e0 a587 20e0 a4b8 e0a4  ... ...... .....
-000008a0: b9e0 a587 e0a4 9ce0 a587 e0a4 8275 ce00  .............u..
-000008b0: 0000 e0a4 91e0 a4ab e0a4 bce0 a4b2 e0a4  ................
-000008c0: bee0 a487 e0a4 a820 e0a4 aae0 a4b9 e0a5  ....... ........
-000008d0: 81e0 a482 e0a4 9a20 e0a4 95e0 a587 20e0  ....... ...... .
-000008e0: a4b2 e0a4 bfe0 a48f 20e0 a4ac e0a4 bee0  ........ .......
-000008f0: a4b9 e0a4 b0e0 a580 20e0 a49b e0a4 b5e0  ........ .......
-00000900: a4bf e0a4 afe0 a58b e0a4 8220 e0a4 95e0  ........... ....
-00000910: a580 20e0 a4b8 e0a5 8de0 a4b5 e0a4 9ae0  .. .............
-00000920: a4be e0a4 b2e0 a4bf e0a4 a420 e0a4 aae0  ........... ....
-00000930: a58d e0a4 b0e0 a4a4 e0a4 bfe0 a4b2 e0a4  ................
-00000940: bfe0 a4aa e0a4 bfe0 a4af e0a4 bee0 a481  ................
-00000950: 20e0 a4a1 e0a4 bfe0 a4b8 e0a5 8de0 a495   ...............
-00000960: 20e0 a4ae e0a5 87e0 a482 20e0 a4b8 e0a4   ......... .....
-00000970: b9e0 a587 e0a4 9ce0 a587 e0a4 82e0 a5a4  ................
-00000980: 7522 0000 00e0 a493 e0a4 aae0 a4a8 e0a4  u"..............
-00000990: 8fe0 a486 e0a4 8820 e0a4 8fe0 a4aa e0a5  ....... ........
-000009a0: 80e0 a486 e0a4 8875 2200 0000 e0a4 8fe0  .......u".......
-000009b0: a4aa e0a5 80e0 a486 e0a4 8820 e0a4 afe0  ........... ....
-000009c0: a582 e0a4 86e0 a4b0 e0a4 8fe0 a4b2 7535  ..............u5
-000009d0: 0000 00e0 a493 e0a4 aae0 a4a8 e0a4 8fe0  ................
-000009e0: a486 e0a4 8820 e0a4 8fe0 a4aa e0a5 80e0  ..... ..........
-000009f0: a486 e0a4 8820 e0a4 afe0 a582 e0a4 86e0  ..... ..........
-00000a00: a4b0 e0a4 8fe0 a4b2 751f 0000 00e0 a48f  ........u.......
-00000a10: e0a4 aae0 a580 e0a4 86e0 a488 20e0 a495  ............ ...
-00000a20: e0a5 81e0 a482 e0a4 9ce0 a580 7532 0000  ............u2..
-00000a30: 00e0 a493 e0a4 aae0 a4a8 e0a4 8fe0 a486  ................
-00000a40: e0a4 8820 e0a4 8fe0 a4aa e0a5 80e0 a486  ... ............
-00000a50: e0a4 8820 e0a4 95e0 a581 e0a4 82e0 a49c  ... ............
-00000a60: e0a5 8075 2800 0000 e0a4 b8e0 a4ae e0a4  ...u(...........
-00000a70: b0e0 a58d e0a4 a5e0 a4bf e0a4 a420 e0a4  ............. ..
-00000a80: aee0 a589 e0a4 a1e0 a4b2 e0a5 8de0 a4b8  ................
-00000a90: 751c 0000 00e0 a4ae e0a5 89e0 a4a1 e0a4  u...............
-00000aa0: b220 e0a4 9ae0 a581 e0a4 a8e0 a587 e0a4  . ..............
-00000ab0: 8275 4900 0000 e0a4 9ae0 a581 e0a4 a8e0  .uI.............
-00000ac0: a4a8 e0a5 8720 e0a4 95e0 a587 20e0 a4b2  ..... ...... ...
-00000ad0: e0a4 bfe0 a48f 20e0 a4b8 e0a4 aee0 a4b0  ...... .........
-00000ae0: e0a5 8de0 a4a5 e0a4 bfe0 a4a4 20e0 a4ae  ............ ...
-00000af0: e0a5 89e0 a4a1 e0a4 b2e0 a58d e0a4 b875  ...............u
-00000b00: 2200 0000 e0a4 aee0 a582 e0a4 b220 e0a4  "............ ..
-00000b10: aae0 a588 e0a4 b0e0 a4be e0a4 aee0 a580  ................
-00000b20: e0a4 9fe0 a4b0 752e 0000 00e0 a4b8 e0a4  ......u.........
-00000b30: bfe0 a4b8 e0a5 8de0 a49f e0a4 ae20 e0a4  ............. ..
-00000b40: aae0 a58d e0a4 b0e0 a589 e0a4 aee0 a58d  ................
-00000b50: e0a4 aae0 a58d e0a4 9f75 7800 0000 e0a4  .........ux.....
-00000b60: aae0 a58d e0a4 b0e0 a4a4 e0a5 8de0 a4af  ................
-00000b70: e0a5 87e0 a495 20e0 a485 e0a4 a8e0 a581  ...... .........
-00000b80: e0a4 b0e0 a58b e0a4 a720 e0a4 b8e0 a587  ......... ......
-00000b90: 20e0 a4aa e0a4 b9e0 a4b2 e0a5 8720 e0a4   ............ ..
-00000ba0: aee0 a582 e0a4 b220 e0a4 b8e0 a4bf e0a4  ....... ........
-00000bb0: b8e0 a58d e0a4 9fe0 a4ae 20e0 a4aa e0a5  .......... .....
-00000bc0: 8de0 a4b0 e0a5 89e0 a4ae e0a5 8de0 a4aa  ................
-00000bd0: e0a5 8de0 a49f 75a3 0000 00e0 a4aa e0a5  ......u.........
-00000be0: 8de0 a4b0 e0a4 a4e0 a58d e0a4 afe0 a587  ................
-00000bf0: e0a4 9520 e0a4 85e0 a4a8 e0a5 81e0 a4b0  ... ............
-00000c00: e0a5 8be0 a4a7 20e0 a4b8 e0a5 8720 e0a4  ...... ...... ..
-00000c10: aae0 a4b9 e0a4 b2e0 a587 20e0 a4ae e0a5  .......... .....
-00000c20: 82e0 a4b2 20e0 a4b8 e0a4 bfe0 a4b8 e0a5  .... ...........
-00000c30: 8de0 a49f e0a4 ae20 e0a4 aae0 a58d e0a4  ....... ........
-00000c40: b0e0 a589 e0a4 aee0 a58d e0a4 aae0 a58d  ................
-00000c50: e0a4 9fe0 a5a4 20e0 a4af e0a4 b920 e0a4  ...... ...... ..
-00000c60: b8e0 a4be e0a4 a6e0 a4be 20e0 a4aa e0a4  .......... .....
-00000c70: bee0 a4a0 20e0 a4b9 e0a5 88e0 a5a4 753e  .... .........u>
-00000c80: 0000 00e0 a485 e0a4 a7e0 a4bf e0a4 95e0  ................
-00000c90: a4a4 e0a4 ae20 e0a4 aae0 a58d e0a4 b0e0  ..... ..........
-00000ca0: a4a4 e0a4 bfe0 a4b8 e0a4 bee0 a4a6 20e0  .............. .
-00000cb0: a49f e0a5 8be0 a495 e0a4 a8e0 a58d e0a4  ................
-00000cc0: b875 9600 0000 e0a4 aae0 a58d e0a4 b0e0  .u..............
-00000cd0: a4a4 e0a4 bfe0 a4b8 e0a4 bee0 a4a6 20e0  .............. .
-00000ce0: a4ae e0a5 87e0 a482 20e0 a4aa e0a5 8de0  ........ .......
-00000cf0: a4b0 e0a4 bee0 a4aa e0a5 8de0 a4a4 20e0  .............. .
-00000d00: a495 e0a4 b0e0 a4a8 e0a5 8720 e0a4 95e0  ........... ....
-00000d10: a587 20e0 a4b2 e0a4 bfe0 a48f 20e0 a485  .. ......... ...
-00000d20: e0a4 a7e0 a4bf e0a4 95e0 a4a4 e0a4 ae20  ............... 
-00000d30: e0a4 9fe0 a58b e0a4 95e0 a4a8 e0a5 8de0  ................
-00000d40: a4b8 20e0 a495 e0a5 8020 e0a4 b8e0 a482  .. ...... ......
-00000d50: e0a4 96e0 a58d e0a4 afe0 a4be 292f da0c  ............)/..
-00000d60: 7769 6e64 6f77 5f74 6974 6c65 da0c 6275  window_title..bu
-00000d70: 7474 6f6e 5f63 6c6f 7365 da0b 7461 625f  tton_close..tab_
-00000d80: 6765 6e65 7261 6cda 1174 6162 5f65 6469  general..tab_edi
-00000d90: 746f 725f 636f 6e66 6967 da11 7461 625f  tor_config..tab_
-00000da0: 7669 6577 6572 5f63 6f6e 6669 67da 0d74  viewer_config..t
-00000db0: 6162 5f61 695f 636f 6e66 6967 da18 6765  ab_ai_config..ge
-00000dc0: 6e65 7261 6c5f 6170 705f 636f 6e66 6967  neral_app_config
-00000dd0: 5f6c 6162 656c da1a 6765 6e65 7261 6c5f  _label..general_
-00000de0: 6170 705f 6c61 6e67 7561 6765 5f6c 6162  app_language_lab
-00000df0: 656c da2b 6765 6e65 7261 6c5f 6170 705f  el.+general_app_
-00000e00: 6c61 6e67 7561 6765 5f63 6f6d 626f 5f70  language_combo_p
-00000e10: 6c61 6365 686f 6c64 6572 5f74 6578 74da  laceholder_text.
-00000e20: 3167 656e 6572 616c 5f61 7070 5f6c 616e  1general_app_lan
-00000e30: 6775 6167 655f 636f 6d62 6f5f 6163 6365  guage_combo_acce
-00000e40: 7373 6962 6c65 5f64 6573 6372 6970 7469  ssible_descripti
-00000e50: 6f6e da17 6765 6e65 7261 6c5f 6170 705f  on..general_app_
-00000e60: 7468 656d 655f 6c61 6265 6cda 2867 656e  theme_label.(gen
-00000e70: 6572 616c 5f61 7070 5f74 6865 6d65 5f63  eral_app_theme_c
-00000e80: 6f6d 626f 5f70 6c61 6365 686f 6c64 6572  ombo_placeholder
-00000e90: 5f74 6578 74da 2e67 656e 6572 616c 5f61  _text..general_a
-00000ea0: 7070 5f74 6865 6d65 5f63 6f6d 626f 5f61  pp_theme_combo_a
-00000eb0: 6363 6573 7369 626c 655f 6465 7363 7269  ccessible_descri
-00000ec0: 7074 696f 6eda 1b67 656e 6572 616c 5f61  ption..general_a
-00000ed0: 7070 5f6d 6169 6e5f 6d65 6e75 5f6c 6162  pp_main_menu_lab
-00000ee0: 656c da1e 6765 6e65 7261 6c5f 6170 705f  el..general_app_
-00000ef0: 6d61 696e 5f6d 656e 755f 6368 6563 6b62  main_menu_checkb
-00000f00: 6f78 da35 6765 6e65 7261 6c5f 6170 705f  ox.5general_app_
-00000f10: 6d61 696e 5f6d 656e 755f 6368 6563 6b62  main_menu_checkb
-00000f20: 6f78 5f61 6363 6573 7369 626c 655f 6465  ox_accessible_de
-00000f30: 7363 7269 7074 696f 6eda 1b67 656e 6572  scription..gener
-00000f40: 616c 5f61 7070 5f66 6f6e 745f 7369 7a65  al_app_font_size
-00000f50: 5f6c 6162 656c da33 6765 6e65 7261 6c5f  _label.3general_
-00000f60: 6170 705f 666f 6e74 5f73 697a 655f 736c  app_font_size_sl
-00000f70: 6964 6572 5f61 6363 6573 7369 626c 655f  ider_accessible_
-00000f80: 6465 7363 7269 7074 696f 6eda 1767 656e  description..gen
-00000f90: 6572 616c 5f73 7461 7475 7362 6172 5f6c  eral_statusbar_l
-00000fa0: 6162 656c da36 6765 6e65 7261 6c5f 7374  abel.6general_st
-00000fb0: 6174 7573 6261 725f 7368 6f77 5f67 6c6f  atusbar_show_glo
-00000fc0: 6261 6c5f 6375 7273 6f72 5f70 6f73 6974  bal_cursor_posit
-00000fd0: 696f 6e5f 6368 6563 6b62 6f78 da4d 6765  ion_checkbox.Mge
-00000fe0: 6e65 7261 6c5f 7374 6174 7573 6261 725f  neral_statusbar_
-00000ff0: 7368 6f77 5f67 6c6f 6261 6c5f 6375 7273  show_global_curs
-00001000: 6f72 5f70 6f73 6974 696f 6e5f 6368 6563  or_position_chec
-00001010: 6b62 6f78 5f61 6363 6573 7369 626c 655f  kbox_accessible_
-00001020: 6465 7363 7269 7074 696f 6eda 1365 6469  description..edi
-00001030: 746f 725f 636f 6e66 6967 5f6c 6162 656c  tor_config_label
-00001040: da28 6564 6974 6f72 5f63 6f6e 6669 675f  .(editor_config_
-00001050: 7368 6f77 5f6c 696e 655f 6e75 6d62 6572  show_line_number
-00001060: 735f 6368 6563 6b62 6f78 da3f 6564 6974  s_checkbox.?edit
-00001070: 6f72 5f63 6f6e 6669 675f 7368 6f77 5f6c  or_config_show_l
-00001080: 696e 655f 6e75 6d62 6572 735f 6368 6563  ine_numbers_chec
-00001090: 6b62 6f78 5f61 6363 6573 7369 626c 655f  kbox_accessible_
-000010a0: 6465 7363 7269 7074 696f 6eda 1376 6965  description..vie
-000010b0: 7765 725f 636f 6e66 6967 5f6c 6162 656c  wer_config_label
-000010c0: da25 7669 6577 6572 5f63 6f6e 6669 675f  .%viewer_config_
-000010d0: 7072 6f63 6573 735f 656d 6f6a 6973 5f63  process_emojis_c
-000010e0: 6865 636b 626f 78da 3c76 6965 7765 725f  heckbox.<viewer_
-000010f0: 636f 6e66 6967 5f70 726f 6365 7373 5f65  config_process_e
-00001100: 6d6f 6a69 735f 6368 6563 6b62 6f78 5f61  mojis_checkbox_a
-00001110: 6363 6573 7369 626c 655f 6465 7363 7269  ccessible_descri
-00001120: 7074 696f 6eda 2676 6965 7765 725f 636f  ption.&viewer_co
-00001130: 6e66 6967 5f68 6967 686c 6967 6874 5f74  nfig_highlight_t
-00001140: 6f64 6f73 5f63 6865 636b 626f 78da 3d76  odos_checkbox.=v
-00001150: 6965 7765 725f 636f 6e66 6967 5f68 6967  iewer_config_hig
-00001160: 686c 6967 6874 5f74 6f64 6f73 5f63 6865  hlight_todos_che
-00001170: 636b 626f 785f 6163 6365 7373 6962 6c65  ckbox_accessible
-00001180: 5f64 6573 6372 6970 7469 6f6e da2d 7669  _description.-vi
-00001190: 6577 6572 5f63 6f6e 6669 675f 6f70 656e  ewer_config_open
-000011a0: 5f6c 696e 6b5f 636f 6e66 6972 6d61 7469  _link_confirmati
-000011b0: 6f6e 5f63 6865 636b 626f 78da 4476 6965  on_checkbox.Dvie
-000011c0: 7765 725f 636f 6e66 6967 5f6f 7065 6e5f  wer_config_open_
-000011d0: 6c69 6e6b 5f63 6f6e 6669 726d 6174 696f  link_confirmatio
-000011e0: 6e5f 6368 6563 6b62 6f78 5f61 6363 6573  n_checkbox_acces
-000011f0: 7369 626c 655f 6465 7363 7269 7074 696f  sible_descriptio
-00001200: 6eda 2576 6965 7765 725f 636f 6e66 6967  n.%viewer_config
-00001210: 5f73 6176 655f 7265 736f 7572 6365 735f  _save_resources_
-00001220: 6368 6563 6b62 6f78 da3c 7669 6577 6572  checkbox.<viewer
-00001230: 5f63 6f6e 6669 675f 7361 7665 5f72 6573  _config_save_res
-00001240: 6f75 7263 6573 5f63 6865 636b 626f 785f  ources_checkbox_
-00001250: 6163 6365 7373 6962 6c65 5f64 6573 6372  accessible_descr
-00001260: 6970 7469 6f6e da1a 6169 5f63 6f6e 6669  iption..ai_confi
-00001270: 675f 6f70 656e 6169 5f61 7069 5f6c 6162  g_openai_api_lab
-00001280: 656c da2f 6169 5f63 6f6e 6669 675f 6f70  el./ai_config_op
-00001290: 656e 6169 5f61 7069 5f75 726c 5f69 6e70  enai_api_url_inp
-000012a0: 7574 5f70 6c61 6365 686f 6c64 6572 5f74  ut_placeholder_t
-000012b0: 6578 74da 3561 695f 636f 6e66 6967 5f6f  ext.5ai_config_o
-000012c0: 7065 6e61 695f 6170 695f 7572 6c5f 696e  penai_api_url_in
-000012d0: 7075 745f 6163 6365 7373 6962 6c65 5f64  put_accessible_d
-000012e0: 6573 6372 6970 7469 6f6e da2f 6169 5f63  escription./ai_c
-000012f0: 6f6e 6669 675f 6f70 656e 6169 5f61 7069  onfig_openai_api
-00001300: 5f6b 6579 5f69 6e70 7574 5f70 6c61 6365  _key_input_place
-00001310: 686f 6c64 6572 5f74 6578 74da 3561 695f  holder_text.5ai_
-00001320: 636f 6e66 6967 5f6f 7065 6e61 695f 6170  config_openai_ap
-00001330: 695f 6b65 795f 696e 7075 745f 6163 6365  i_key_input_acce
-00001340: 7373 6962 6c65 5f64 6573 6372 6970 7469  ssible_descripti
-00001350: 6f6e da2b 6169 5f63 6f6e 6669 675f 6f70  on.+ai_config_op
-00001360: 656e 6169 5f61 7069 5f73 7570 706f 7274  enai_api_support
-00001370: 6564 5f6d 6f64 656c 735f 6c61 6265 6cda  ed_models_label.
-00001380: 2f61 695f 636f 6e66 6967 5f61 695f 6d6f  /ai_config_ai_mo
-00001390: 6465 6c5f 6e61 6d65 735f 636f 6d62 6f5f  del_names_combo_
-000013a0: 706c 6163 6568 6f6c 6465 725f 7465 7874  placeholder_text
-000013b0: da35 6169 5f63 6f6e 6669 675f 6169 5f6d  .5ai_config_ai_m
-000013c0: 6f64 656c 5f6e 616d 6573 5f63 6f6d 626f  odel_names_combo
-000013d0: 5f61 6363 6573 7369 626c 655f 6465 7363  _accessible_desc
-000013e0: 7269 7074 696f 6eda 1461 695f 636f 6e66  ription..ai_conf
-000013f0: 6967 5f62 6173 655f 6c61 6265 6cda 2261  ig_base_label."a
-00001400: 695f 636f 6e66 6967 5f62 6173 655f 7379  i_config_base_sy
-00001410: 7374 656d 5f70 726f 6d70 745f 6c61 6265  stem_prompt_labe
-00001420: 6cda 3261 695f 636f 6e66 6967 5f62 6173  l.2ai_config_bas
-00001430: 655f 7379 7374 656d 5f70 726f 6d70 745f  e_system_prompt_
-00001440: 6564 6974 5f70 6c61 6365 686f 6c64 6572  edit_placeholder
-00001450: 5f74 6578 74da 3861 695f 636f 6e66 6967  _text.8ai_config
-00001460: 5f62 6173 655f 7379 7374 656d 5f70 726f  _base_system_pro
-00001470: 6d70 745f 6564 6974 5f61 6363 6573 7369  mpt_edit_accessi
-00001480: 626c 655f 6465 7363 7269 7074 696f 6eda  ble_description.
-00001490: 2861 695f 636f 6e66 6967 5f62 6173 655f  (ai_config_base_
-000014a0: 7265 7370 6f6e 7365 5f6d 6178 5f74 6f6b  response_max_tok
-000014b0: 656e 735f 6c61 6265 6cda 3f61 695f 636f  ens_label.?ai_co
-000014c0: 6e66 6967 5f62 6173 655f 7265 7370 6f6e  nfig_base_respon
-000014d0: 7365 5f6d 6178 5f74 6f6b 656e 735f 696e  se_max_tokens_in
-000014e0: 7075 745f 6163 6365 7373 6962 6c65 5f64  put_accessible_d
-000014f0: 6573 6372 6970 7469 6f6e 4e29 01da 076c  escriptionN)...l
-00001500: 6578 656d 6573 a900 7231 0000 0072 3100  exemes..r1...r1.
-00001510: 0000 fa4c 2f55 7365 7273 2f76 6164 696b  ...L/Users/vadik
-00001520: 7573 2f50 7963 6861 726d 5072 6f6a 6563  us/PycharmProjec
-00001530: 7473 2f6e 6f74 6f6c 6f67 2d64 6576 2f61  ts/notolog-dev/a
-00001540: 7070 2f6c 6578 656d 6573 2f69 6e2f 7365  pp/lexemes/in/se
-00001550: 7474 696e 6773 5f64 6961 6c6f 672e 7079  ttings_dialog.py
-00001560: da08 3c6d 6f64 756c 653e 0300 0000 735e  ..<module>....s^
-00001570: 0000 0002 0202 0202 0102 0102 0102 0202  ................
-00001580: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-00001590: 0102 0102 0102 0202 0102 0202 0202 0102  ................
-000015a0: 0102 0202 0102 0102 0102 0102 0102 0202  ................
-000015b0: 0102 0202 0202 0102 0102 0102 0102 0102  ................
-000015c0: 0102 0102 0202 0102 0102 0202 0102 0202  ................
-000015d0: c4                                       .
+00000000: 2320 4869 6e64 6920 6c65 7865 6d65 7320  # Hindi lexemes 
+00000010: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
+00000020: 7079 0a6c 6578 656d 6573 203d 207b 0a20  py.lexemes = {. 
+00000030: 2020 2022 7769 6e64 6f77 5f74 6974 6c65     "window_title
+00000040: 223a 2022 e0a4 b8e0 a587 e0a4 9fe0 a4bf  ": "............
+00000050: e0a4 82e0 a497 e0a5 8de0 a4b8 222c 0a0a  ............",..
+00000060: 2020 2020 2262 7574 746f 6e5f 636c 6f73      "button_clos
+00000070: 6522 3a20 22e0 a4ac e0a4 82e0 a4a6 20e0  e": "......... .
+00000080: a495 e0a4 b0e0 a587 e0a4 8222 2c0a 0a20  ...........",.. 
+00000090: 2020 2022 7461 625f 6765 6e65 7261 6c22     "tab_general"
+000000a0: 3a20 22e0 a4b8 e0a4 bee0 a4ae e0a4 bee0  : ".............
+000000b0: a4a8 e0a5 8de0 a4af 222c 0a20 2020 2022  ........",.    "
+000000c0: 7461 625f 6564 6974 6f72 5f63 6f6e 6669  tab_editor_confi
+000000d0: 6722 3a20 22e0 a4b8 e0a4 82e0 a4aa e0a4  g": "...........
+000000e0: bee0 a4a6 e0a4 9522 2c0a 2020 2020 2274  .......",.    "t
+000000f0: 6162 5f76 6965 7765 725f 636f 6e66 6967  ab_viewer_config
+00000100: 223a 2022 e0a4 a6e0 a4b0 e0a5 8de0 a4b6  ": "............
+00000110: e0a4 9522 2c0a 2020 2020 2274 6162 5f61  ...",.    "tab_a
+00000120: 695f 636f 6e66 6967 223a 2022 e0a4 8fe0  i_config": "....
+00000130: a486 e0a4 8820 e0a4 95e0 a589 e0a4 a8e0  ..... ..........
+00000140: a58d e0a4 abe0 a4bc e0a4 bfe0 a497 222c  ..............",
+00000150: 0a0a 2020 2020 2267 656e 6572 616c 5f61  ..    "general_a
+00000160: 7070 5f63 6f6e 6669 675f 6c61 6265 6c22  pp_config_label"
+00000170: 3a20 22e0 a48f e0a4 aae0 a58d e0a4 b2e0  : ".............
+00000180: a4bf e0a4 95e0 a587 e0a4 b6e0 a4a8 20e0  .............. .
+00000190: a495 e0a5 89e0 a4a8 e0a5 8de0 a4ab e0a4  ................
+000001a0: bce0 a4bf e0a4 9722 2c0a 2020 2020 2267  .......",.    "g
+000001b0: 656e 6572 616c 5f61 7070 5f6c 616e 6775  eneral_app_langu
+000001c0: 6167 655f 6c61 6265 6c22 3a20 22e0 a4ad  age_label": "...
+000001d0: e0a4 bee0 a4b7 e0a4 be22 2c0a 2020 2020  .........",.    
+000001e0: 2267 656e 6572 616c 5f61 7070 5f6c 616e  "general_app_lan
+000001f0: 6775 6167 655f 636f 6d62 6f5f 706c 6163  guage_combo_plac
+00000200: 6568 6f6c 6465 725f 7465 7874 223a 2022  eholder_text": "
+00000210: e0a4 8fe0 a495 20e0 a4ad e0a4 bee0 a4b7  ...... .........
+00000220: e0a4 be20 e0a4 9ae0 a581 e0a4 a8e0 a587  ... ............
+00000230: e0a4 8222 2c0a 2020 2020 2267 656e 6572  ...",.    "gener
+00000240: 616c 5f61 7070 5f6c 616e 6775 6167 655f  al_app_language_
+00000250: 636f 6d62 6f5f 6163 6365 7373 6962 6c65  combo_accessible
+00000260: 5f64 6573 6372 6970 7469 6f6e 223a 2022  _description": "
+00000270: e0a4 8fe0 a4aa e0a5 8de0 a4b2 e0a4 bfe0  ................
+00000280: a495 e0a5 87e0 a4b6 e0a4 a820 e0a4 95e0  ........... ....
+00000290: a580 20e0 a487 e0a4 82e0 a49f e0a4 b0e0  .. .............
+000002a0: a4ab e0a4 bce0 a587 e0a4 b820 e0a4 ade0  ........... ....
+000002b0: a4be e0a4 b7e0 a4be 222c 0a20 2020 2022  ........",.    "
+000002c0: 6765 6e65 7261 6c5f 6170 705f 7468 656d  general_app_them
+000002d0: 655f 6c61 6265 6c22 3a20 22e0 a4a5 e0a5  e_label": ".....
+000002e0: 80e0 a4ae 222c 0a20 2020 2022 6765 6e65  ....",.    "gene
+000002f0: 7261 6c5f 6170 705f 7468 656d 655f 636f  ral_app_theme_co
+00000300: 6d62 6f5f 706c 6163 6568 6f6c 6465 725f  mbo_placeholder_
+00000310: 7465 7874 223a 2022 e0a4 8fe0 a495 20e0  text": "...... .
+00000320: a4a5 e0a5 80e0 a4ae 20e0 a49a e0a5 81e0  ........ .......
+00000330: a4a8 e0a5 87e0 a482 222c 0a20 2020 2022  ........",.    "
+00000340: 6765 6e65 7261 6c5f 6170 705f 7468 656d  general_app_them
+00000350: 655f 636f 6d62 6f5f 6163 6365 7373 6962  e_combo_accessib
+00000360: 6c65 5f64 6573 6372 6970 7469 6f6e 223a  le_description":
+00000370: 2022 e0a4 8fe0 a4aa e0a5 8de0 a4b2 e0a4   "..............
+00000380: bfe0 a495 e0a5 87e0 a4b6 e0a4 a820 e0a4  ............. ..
+00000390: 95e0 a580 20e0 a487 e0a4 82e0 a49f e0a4  .... ...........
+000003a0: b0e0 a4ab e0a4 bce0 a587 e0a4 b820 e0a4  ............. ..
+000003b0: a5e0 a580 e0a4 ae22 2c0a 2020 2020 2267  .......",.    "g
+000003c0: 656e 6572 616c 5f61 7070 5f6d 6169 6e5f  eneral_app_main_
+000003d0: 6d65 6e75 5f6c 6162 656c 223a 2022 e0a4  menu_label": "..
+000003e0: aee0 a581 e0a4 96e0 a58d e0a4 af20 e0a4  ............. ..
+000003f0: aee0 a587 e0a4 a8e0 a582 222c 0a20 2020  ..........",.   
+00000400: 2022 6765 6e65 7261 6c5f 6170 705f 6d61   "general_app_ma
+00000410: 696e 5f6d 656e 755f 6368 6563 6b62 6f78  in_menu_checkbox
+00000420: 223a 2022 e0a4 aee0 a581 e0a4 96e0 a58d  ": "............
+00000430: e0a4 af20 e0a4 aee0 a587 e0a4 a8e0 a582  ... ............
+00000440: 20e0 a4a6 e0a4 bfe0 a496 e0a4 bee0 a48f   ...............
+00000450: e0a4 8222 2c0a 2020 2020 2267 656e 6572  ...",.    "gener
+00000460: 616c 5f61 7070 5f6d 6169 6e5f 6d65 6e75  al_app_main_menu
+00000470: 5f63 6865 636b 626f 785f 6163 6365 7373  _checkbox_access
+00000480: 6962 6c65 5f64 6573 6372 6970 7469 6f6e  ible_description
+00000490: 223a 2022 e0a4 90e0 a4aa 20e0 a495 e0a4  ": "...... .....
+000004a0: be20 e0a4 aee0 a581 e0a4 96e0 a58d e0a4  . ..............
+000004b0: af20 e0a4 a1e0 a58d e0a4 b0e0 a589 e0a4  . ..............
+000004c0: aae0 a4a1 e0a4 bee0 a489 e0a4 a820 e0a4  ............. ..
+000004d0: aee0 a587 e0a4 a8e0 a582 20e0 a4a6 e0a4  .......... .....
+000004e0: bfe0 a496 e0a4 bee0 a48f e0a4 8222 2c0a  .............",.
+000004f0: 2020 2020 2267 656e 6572 616c 5f61 7070      "general_app
+00000500: 5f66 6f6e 745f 7369 7a65 5f6c 6162 656c  _font_size_label
+00000510: 223a 2022 e0a4 abe0 a4bc e0a5 89e0 a4a8  ": "............
+00000520: e0a5 8de0 a49f 20e0 a486 e0a4 95e0 a4be  ...... .........
+00000530: e0a4 b03a 207b 7369 7a65 7d20 e0a4 aae0  ...: {size} ....
+00000540: a580 e0a4 9fe0 a580 222c 0a20 2020 2022  ........",.    "
+00000550: 6765 6e65 7261 6c5f 6170 705f 666f 6e74  general_app_font
+00000560: 5f73 697a 655f 736c 6964 6572 5f61 6363  _size_slider_acc
+00000570: 6573 7369 626c 655f 6465 7363 7269 7074  essible_descript
+00000580: 696f 6e22 3a20 22e0 a490 e0a4 aa20 e0a4  ion": "...... ..
+00000590: 95e0 a4be 20e0 a4b5 e0a5 88e0 a4b6 e0a5  .... ...........
+000005a0: 8de0 a4b5 e0a4 bfe0 a495 20e0 a4ab e0a4  .......... .....
+000005b0: bce0 a589 e0a4 a8e0 a58d e0a4 9f20 e0a4  ............. ..
+000005c0: 86e0 a495 e0a4 bee0 a4b0 20e0 a4b8 e0a4  .......... .....
+000005d0: aee0 a4be e0a4 afe0 a58b e0a4 9ce0 a4bf  ................
+000005e0: e0a4 a420 e0a4 95e0 a4b0 e0a5 87e0 a482  ... ............
+000005f0: 222c 0a0a 2020 2020 2267 656e 6572 616c  ",..    "general
+00000600: 5f73 7461 7475 7362 6172 5f6c 6162 656c  _statusbar_label
+00000610: 223a 2022 e0a4 b8e0 a58d e0a4 a5e0 a4bf  ": "............
+00000620: e0a4 a4e0 a4bf 20e0 a4aa e0a4 9fe0 a58d  ...... .........
+00000630: e0a4 9fe0 a580 222c 0a20 2020 2022 6765  ......",.    "ge
+00000640: 6e65 7261 6c5f 7374 6174 7573 6261 725f  neral_statusbar_
+00000650: 7368 6f77 5f67 6c6f 6261 6c5f 6375 7273  show_global_curs
+00000660: 6f72 5f70 6f73 6974 696f 6e5f 6368 6563  or_position_chec
+00000670: 6b62 6f78 223a 2022 e0a4 97e0 a58d e0a4  kbox": "........
+00000680: b2e0 a58b e0a4 ace0 a4b2 20e0 a495 e0a4  .......... .....
+00000690: b0e0 a58d e0a4 b8e0 a4b0 20e0 a4b8 e0a5  .......... .....
+000006a0: 8de0 a4a5 e0a4 bfe0 a4a4 e0a4 bf20 e0a4  ............. ..
+000006b0: a6e0 a4bf e0a4 96e0 a4be e0a4 8fe0 a482  ................
+000006c0: 222c 0a20 2020 2022 6765 6e65 7261 6c5f  ",.    "general_
+000006d0: 7374 6174 7573 6261 725f 7368 6f77 5f67  statusbar_show_g
+000006e0: 6c6f 6261 6c5f 6375 7273 6f72 5f70 6f73  lobal_cursor_pos
+000006f0: 6974 696f 6e5f 6368 6563 6b62 6f78 5f61  ition_checkbox_a
+00000700: 6363 6573 7369 626c 655f 6465 7363 7269  ccessible_descri
+00000710: 7074 696f 6e22 3a0a 2020 2020 2020 2020  ption":.        
+00000720: 22e0 a4b8 e0a5 8de0 a4a5 e0a4 bfe0 a4a4  "...............
+00000730: e0a4 bf20 e0a4 aae0 a49f e0a5 8de0 a49f  ... ............
+00000740: e0a5 8020 e0a4 aee0 a587 e0a4 8220 e0a4  ... ......... ..
+00000750: 97e0 a58d e0a4 b2e0 a58b e0a4 ace0 a4b2  ................
+00000760: 20e0 a495 e0a4 b0e0 a58d e0a4 b8e0 a4b0   ...............
+00000770: 20e0 a4b8 e0a5 8de0 a4a5 e0a4 bfe0 a4a4   ...............
+00000780: e0a4 bf20 e0a4 a6e0 a4bf e0a4 96e0 a4be  ... ............
+00000790: e0a4 8fe0 a482 222c 0a0a 2020 2020 2265  ......",..    "e
+000007a0: 6469 746f 725f 636f 6e66 6967 5f6c 6162  ditor_config_lab
+000007b0: 656c 223a 2022 e0a4 b8e0 a482 e0a4 aae0  el": "..........
+000007c0: a4be e0a4 a6e0 a495 20e0 a495 e0a5 89e0  ........ .......
+000007d0: a4a8 e0a5 8de0 a4ab e0a4 bce0 a4bf e0a4  ................
+000007e0: 97e0 a4b0 e0a5 87e0 a4b6 e0a4 a822 2c0a  .............",.
+000007f0: 2020 2020 2265 6469 746f 725f 636f 6e66      "editor_conf
+00000800: 6967 5f73 686f 775f 6c69 6e65 5f6e 756d  ig_show_line_num
+00000810: 6265 7273 5f63 6865 636b 626f 7822 3a20  bers_checkbox": 
+00000820: 22e0 a4b2 e0a4 bee0 a487 e0a4 a820 e0a4  "............ ..
+00000830: b8e0 a482 e0a4 96e0 a58d e0a4 afe0 a4be  ................
+00000840: e0a4 8fe0 a481 20e0 a4a6 e0a4 bfe0 a496  ...... .........
+00000850: e0a4 bee0 a48f e0a4 8222 2c0a 2020 2020  .........",.    
+00000860: 2265 6469 746f 725f 636f 6e66 6967 5f73  "editor_config_s
+00000870: 686f 775f 6c69 6e65 5f6e 756d 6265 7273  how_line_numbers
+00000880: 5f63 6865 636b 626f 785f 6163 6365 7373  _checkbox_access
+00000890: 6962 6c65 5f64 6573 6372 6970 7469 6f6e  ible_description
+000008a0: 223a 2022 e0a4 b8e0 a482 e0a4 aae0 a4be  ": "............
+000008b0: e0a4 a6e0 a495 20e0 a4ae e0a5 87e0 a482  ...... .........
+000008c0: 20e0 a4b2 e0a4 bee0 a487 e0a4 a820 e0a4   ............ ..
+000008d0: b8e0 a482 e0a4 96e0 a58d e0a4 afe0 a4be  ................
+000008e0: e0a4 8fe0 a481 20e0 a4a6 e0a4 bfe0 a496  ...... .........
+000008f0: e0a4 bee0 a48f e0a4 8222 2c0a 0a20 2020  .........",..   
+00000900: 2022 7669 6577 6572 5f63 6f6e 6669 675f   "viewer_config_
+00000910: 6c61 6265 6c22 3a20 22e0 a4a6 e0a4 b0e0  label": ".......
+00000920: a58d e0a4 b6e0 a495 20e0 a495 e0a5 89e0  ........ .......
+00000930: a4a8 e0a5 8de0 a4ab e0a4 bce0 a4bf e0a4  ................
+00000940: 97e0 a4b0 e0a5 87e0 a4b6 e0a4 a822 2c0a  .............",.
+00000950: 2020 2020 2276 6965 7765 725f 636f 6e66      "viewer_conf
+00000960: 6967 5f70 726f 6365 7373 5f65 6d6f 6a69  ig_process_emoji
+00000970: 735f 6368 6563 6b62 6f78 223a 2022 e0a4  s_checkbox": "..
+00000980: aae0 a4be e0a4 a020 e0a4 87e0 a4ae e0a5  ....... ........
+00000990: 8be0 a49c e0a5 8020 e0a4 95e0 a58b 20e0  ....... ...... .
+000009a0: a497 e0a5 8de0 a4b0 e0a4 bee0 a4ab e0a4  ................
+000009b0: bfe0 a495 20e0 a4ae e0a5 87e0 a482 20e0  .... ......... .
+000009c0: a4aa e0a4 b0e0 a4bf e0a4 b5e0 a4b0 e0a5  ................
+000009d0: 8de0 a4a4 e0a4 bfe0 a4a4 20e0 a495 e0a4  .......... .....
+000009e0: b0e0 a587 e0a4 8222 2c0a 2020 2020 2276  .......",.    "v
+000009f0: 6965 7765 725f 636f 6e66 6967 5f70 726f  iewer_config_pro
+00000a00: 6365 7373 5f65 6d6f 6a69 735f 6368 6563  cess_emojis_chec
+00000a10: 6b62 6f78 5f61 6363 6573 7369 626c 655f  kbox_accessible_
+00000a20: 6465 7363 7269 7074 696f 6e22 3a20 22e0  description": ".
+00000a30: a4aa e0a4 bee0 a4a0 20e0 a487 e0a4 aee0  ........ .......
+00000a40: a58b e0a4 9ce0 a580 20e0 a495 e0a5 8b20  ........ ...... 
+00000a50: e0a4 9ae0 a4bf e0a4 a4e0 a58d e0a4 b0e0  ................
+00000a60: a4bf e0a4 a420 e0a4 aae0 a58d e0a4 b0e0  ..... ..........
+00000a70: a4a4 e0a4 bfe0 a4a8 e0a4 bfe0 a4a7 e0a4  ................
+00000a80: bf20 e0a4 aee0 a587 e0a4 8220 e0a4 aae0  . ......... ....
+00000a90: a4b0 e0a4 bfe0 a4b5 e0a4 b0e0 a58d e0a4  ................
+00000aa0: a4e0 a4bf e0a4 a420 e0a4 95e0 a4b0 e0a5  ....... ........
+00000ab0: 87e0 a482 222c 0a20 2020 2022 7669 6577  ....",.    "view
+00000ac0: 6572 5f63 6f6e 6669 675f 6869 6768 6c69  er_config_highli
+00000ad0: 6768 745f 746f 646f 735f 6368 6563 6b62  ght_todos_checkb
+00000ae0: 6f78 223a 2022 544f 444f 20e0 a495 e0a5  ox": "TODO .....
+00000af0: 8b20 e0a4 b9e0 a4be e0a4 87e0 a4b2 e0a4  . ..............
+00000b00: bee0 a487 e0a4 9f20 e0a4 95e0 a4b0 e0a5  ....... ........
+00000b10: 87e0 a482 222c 0a20 2020 2022 7669 6577  ....",.    "view
+00000b20: 6572 5f63 6f6e 6669 675f 6869 6768 6c69  er_config_highli
+00000b30: 6768 745f 746f 646f 735f 6368 6563 6b62  ght_todos_checkb
+00000b40: 6f78 5f61 6363 6573 7369 626c 655f 6465  ox_accessible_de
+00000b50: 7363 7269 7074 696f 6e22 3a20 22e0 a4aa  scription": "...
+00000b60: e0a4 bee0 a4a0 20e0 a4ae e0a5 87e0 a482  ...... .........
+00000b70: 2054 4f44 4f20 e0a4 9fe0 a588 e0a4 9720   TODO ......... 
+00000b80: e0a4 95e0 a58b 20e0 a4ae e0a4 b9e0 a4a4  ...... .........
+00000b90: e0a5 8de0 a4b5 e0a4 aae0 a582 e0a4 b0e0  ................
+00000ba0: a58d e0a4 a320 e0a4 ace0 a4a8 e0a4 bee0  ..... ..........
+00000bb0: a48f e0a4 8222 2c0a 2020 2020 2276 6965  .....",.    "vie
+00000bc0: 7765 725f 636f 6e66 6967 5f6f 7065 6e5f  wer_config_open_
+00000bd0: 6c69 6e6b 5f63 6f6e 6669 726d 6174 696f  link_confirmatio
+00000be0: 6e5f 6368 6563 6b62 6f78 223a 2022 e0a4  n_checkbox": "..
+00000bf0: b2e0 a4bf e0a4 82e0 a495 20e0 a496 e0a5  .......... .....
+00000c00: 8be0 a4b2 e0a4 a8e0 a587 20e0 a495 e0a5  .......... .....
+00000c10: 8720 e0a4 b2e0 a4bf e0a4 8f20 e0a4 aae0  . ......... ....
+00000c20: a581 e0a4 b7e0 a58d e0a4 9fe0 a4bf 20e0  .............. .
+00000c30: a495 e0a5 8020 e0a4 86e0 a4b5 e0a4 b6e0  ..... ..........
+00000c40: a58d e0a4 afe0 a495 e0a4 a4e0 a4be 222c  ..............",
+00000c50: 0a20 2020 2022 7669 6577 6572 5f63 6f6e  .    "viewer_con
+00000c60: 6669 675f 6f70 656e 5f6c 696e 6b5f 636f  fig_open_link_co
+00000c70: 6e66 6972 6d61 7469 6f6e 5f63 6865 636b  nfirmation_check
+00000c80: 626f 785f 6163 6365 7373 6962 6c65 5f64  box_accessible_d
+00000c90: 6573 6372 6970 7469 6f6e 223a 0a20 2020  escription":.   
+00000ca0: 2020 2020 2022 e0a4 b2e0 a4bf e0a4 82e0       "..........
+00000cb0: a495 20e0 a496 e0a5 8be0 a4b2 e0a4 a8e0  .. .............
+00000cc0: a587 20e0 a4b8 e0a5 8720 e0a4 aae0 a4b9  .. ...... ......
+00000cd0: e0a4 b2e0 a587 20e0 a4aa e0a5 81e0 a4b7  ...... .........
+00000ce0: e0a5 8de0 a49f e0a4 bf20 e0a4 95e0 a580  ......... ......
+00000cf0: 20e0 a486 e0a4 b5e0 a4b6 e0a5 8de0 a4af   ...............
+00000d00: e0a4 95e0 a4a4 e0a4 be20 e0a4 b9e0 a588  ......... ......
+00000d10: 222c 0a20 2020 2022 7669 6577 6572 5f63  ",.    "viewer_c
+00000d20: 6f6e 6669 675f 7361 7665 5f72 6573 6f75  onfig_save_resou
+00000d30: 7263 6573 5f63 6865 636b 626f 7822 3a20  rces_checkbox": 
+00000d40: 22e0 a4ac e0a4 bee0 a4b9 e0a4 b0e0 a580  "...............
+00000d50: 20e0 a49b e0a4 b5e0 a4bf e0a4 afe0 a58b   ...............
+00000d60: e0a4 8220 e0a4 95e0 a58b 20e0 a4a1 e0a4  ... ...... .....
+00000d70: bfe0 a4b8 e0a5 8de0 a495 20e0 a4ae e0a5  .......... .....
+00000d80: 87e0 a482 20e0 a4b8 e0a5 8de0 a4b5 e0a4  .... ...........
+00000d90: 9ae0 a4be e0a4 b2e0 a4bf e0a4 a420 e0a4  ............. ..
+00000da0: b0e0 a582 e0a4 aa20 e0a4 b8e0 a587 20e0  ....... ...... .
+00000db0: a4b8 e0a4 b9e0 a587 e0a4 9ce0 a587 e0a4  ................
+00000dc0: 8222 2c0a 2020 2020 2276 6965 7765 725f  .",.    "viewer_
+00000dd0: 636f 6e66 6967 5f73 6176 655f 7265 736f  config_save_reso
+00000de0: 7572 6365 735f 6368 6563 6b62 6f78 5f61  urces_checkbox_a
+00000df0: 6363 6573 7369 626c 655f 6465 7363 7269  ccessible_descri
+00000e00: 7074 696f 6e22 3a0a 2020 2020 2020 2020  ption":.        
+00000e10: 22e0 a491 e0a4 abe0 a4bc e0a4 b2e0 a4be  "...............
+00000e20: e0a4 87e0 a4a8 20e0 a4aa e0a4 b9e0 a581  ...... .........
+00000e30: e0a4 82e0 a49a 20e0 a495 e0a5 8720 e0a4  ...... ...... ..
+00000e40: b2e0 a4bf e0a4 8f20 e0a4 ace0 a4be e0a4  ....... ........
+00000e50: b9e0 a4b0 e0a5 8020 e0a4 9be0 a4b5 e0a4  ....... ........
+00000e60: bfe0 a4af e0a5 8be0 a482 20e0 a495 e0a5  .......... .....
+00000e70: 8020 e0a4 b8e0 a58d e0a4 b5e0 a49a e0a4  . ..............
+00000e80: bee0 a4b2 e0a4 bfe0 a4a4 20e0 a4aa e0a5  .......... .....
+00000e90: 8de0 a4b0 e0a4 a4e0 a4bf e0a4 b2e0 a4bf  ................
+00000ea0: e0a4 aae0 a4bf e0a4 afe0 a4be e0a4 8120  ............... 
+00000eb0: e0a4 a1e0 a4bf e0a4 b8e0 a58d e0a4 9520  ............... 
+00000ec0: e0a4 aee0 a587 e0a4 8220 e0a4 b8e0 a4b9  ......... ......
+00000ed0: e0a5 87e0 a49c e0a5 87e0 a482 e0a5 a422  ..............."
+00000ee0: 2c0a 0a20 2020 2022 6169 5f63 6f6e 6669  ,..    "ai_confi
+00000ef0: 675f 6f70 656e 6169 5f61 7069 5f6c 6162  g_openai_api_lab
+00000f00: 656c 223a 2022 e0a4 93e0 a4aa e0a4 a8e0  el": "..........
+00000f10: a48f e0a4 86e0 a488 20e0 a48f e0a4 aae0  ........ .......
+00000f20: a580 e0a4 86e0 a488 222c 0a20 2020 2022  ........",.    "
+00000f30: 6169 5f63 6f6e 6669 675f 6f70 656e 6169  ai_config_openai
+00000f40: 5f61 7069 5f75 726c 5f69 6e70 7574 5f70  _api_url_input_p
+00000f50: 6c61 6365 686f 6c64 6572 5f74 6578 7422  laceholder_text"
+00000f60: 3a20 22e0 a48f e0a4 aae0 a580 e0a4 86e0  : ".............
+00000f70: a488 20e0 a4af e0a5 82e0 a486 e0a4 b0e0  .. .............
+00000f80: a48f e0a4 b222 2c0a 2020 2020 2261 695f  .....",.    "ai_
+00000f90: 636f 6e66 6967 5f6f 7065 6e61 695f 6170  config_openai_ap
+00000fa0: 695f 7572 6c5f 696e 7075 745f 6163 6365  i_url_input_acce
+00000fb0: 7373 6962 6c65 5f64 6573 6372 6970 7469  ssible_descripti
+00000fc0: 6f6e 223a 2022 e0a4 93e0 a4aa e0a4 a8e0  on": "..........
+00000fd0: a48f e0a4 86e0 a488 20e0 a48f e0a4 aae0  ........ .......
+00000fe0: a580 e0a4 86e0 a488 20e0 a4af e0a5 82e0  ........ .......
+00000ff0: a486 e0a4 b0e0 a48f e0a4 b222 2c0a 2020  ...........",.  
+00001000: 2020 2261 695f 636f 6e66 6967 5f6f 7065    "ai_config_ope
+00001010: 6e61 695f 6170 695f 6b65 795f 696e 7075  nai_api_key_inpu
+00001020: 745f 706c 6163 6568 6f6c 6465 725f 7465  t_placeholder_te
+00001030: 7874 223a 2022 e0a4 8fe0 a4aa e0a5 80e0  xt": "..........
+00001040: a486 e0a4 8820 e0a4 95e0 a581 e0a4 82e0  ..... ..........
+00001050: a49c e0a5 8022 2c0a 2020 2020 2261 695f  .....",.    "ai_
+00001060: 636f 6e66 6967 5f6f 7065 6e61 695f 6170  config_openai_ap
+00001070: 695f 6b65 795f 696e 7075 745f 6163 6365  i_key_input_acce
+00001080: 7373 6962 6c65 5f64 6573 6372 6970 7469  ssible_descripti
+00001090: 6f6e 223a 2022 e0a4 93e0 a4aa e0a4 a8e0  on": "..........
+000010a0: a48f e0a4 86e0 a488 20e0 a48f e0a4 aae0  ........ .......
+000010b0: a580 e0a4 86e0 a488 20e0 a495 e0a5 81e0  ........ .......
+000010c0: a482 e0a4 9ce0 a580 222c 0a20 2020 2022  ........",.    "
+000010d0: 6169 5f63 6f6e 6669 675f 6f70 656e 6169  ai_config_openai
+000010e0: 5f61 7069 5f73 7570 706f 7274 6564 5f6d  _api_supported_m
+000010f0: 6f64 656c 735f 6c61 6265 6c22 3a20 22e0  odels_label": ".
+00001100: a4b8 e0a4 aee0 a4b0 e0a5 8de0 a4a5 e0a4  ................
+00001110: bfe0 a4a4 20e0 a4ae e0a5 89e0 a4a1 e0a4  .... ...........
+00001120: b2e0 a58d e0a4 b822 2c0a 2020 2020 2261  .......",.    "a
+00001130: 695f 636f 6e66 6967 5f61 695f 6d6f 6465  i_config_ai_mode
+00001140: 6c5f 6e61 6d65 735f 636f 6d62 6f5f 706c  l_names_combo_pl
+00001150: 6163 6568 6f6c 6465 725f 7465 7874 223a  aceholder_text":
+00001160: 2022 e0a4 aee0 a589 e0a4 a1e0 a4b2 20e0   "............ .
+00001170: a49a e0a5 81e0 a4a8 e0a5 87e0 a482 222c  ..............",
+00001180: 0a20 2020 2022 6169 5f63 6f6e 6669 675f  .    "ai_config_
+00001190: 6169 5f6d 6f64 656c 5f6e 616d 6573 5f63  ai_model_names_c
+000011a0: 6f6d 626f 5f61 6363 6573 7369 626c 655f  ombo_accessible_
+000011b0: 6465 7363 7269 7074 696f 6e22 3a20 22e0  description": ".
+000011c0: a49a e0a5 81e0 a4a8 e0a4 a8e0 a587 20e0  .............. .
+000011d0: a495 e0a5 8720 e0a4 b2e0 a4bf e0a4 8f20  ..... ......... 
+000011e0: e0a4 b8e0 a4ae e0a4 b0e0 a58d e0a4 a5e0  ................
+000011f0: a4bf e0a4 a420 e0a4 aee0 a589 e0a4 a1e0  ..... ..........
+00001200: a4b2 e0a5 8de0 a4b8 222c 0a0a 2020 2020  ........",..    
+00001210: 2261 695f 636f 6e66 6967 5f62 6173 655f  "ai_config_base_
+00001220: 6c61 6265 6c22 3a20 22e0 a4ae e0a5 82e0  label": ".......
+00001230: a4b2 20e0 a4aa e0a5 88e0 a4b0 e0a4 bee0  .. .............
+00001240: a4ae e0a5 80e0 a49f e0a4 b022 2c0a 2020  ...........",.  
+00001250: 2020 2261 695f 636f 6e66 6967 5f62 6173    "ai_config_bas
+00001260: 655f 7379 7374 656d 5f70 726f 6d70 745f  e_system_prompt_
+00001270: 6c61 6265 6c22 3a20 22e0 a4b8 e0a4 bfe0  label": ".......
+00001280: a4b8 e0a5 8de0 a49f e0a4 ae20 e0a4 aae0  ........... ....
+00001290: a58d e0a4 b0e0 a589 e0a4 aee0 a58d e0a4  ................
+000012a0: aae0 a58d e0a4 9f22 2c0a 2020 2020 2261  .......",.    "a
+000012b0: 695f 636f 6e66 6967 5f62 6173 655f 7379  i_config_base_sy
+000012c0: 7374 656d 5f70 726f 6d70 745f 6564 6974  stem_prompt_edit
+000012d0: 5f70 6c61 6365 686f 6c64 6572 5f74 6578  _placeholder_tex
+000012e0: 7422 3a20 22e0 a4aa e0a5 8de0 a4b0 e0a4  t": "...........
+000012f0: a4e0 a58d e0a4 afe0 a587 e0a4 9520 e0a4  ............. ..
+00001300: 85e0 a4a8 e0a5 81e0 a4b0 e0a5 8be0 a4a7  ................
+00001310: 20e0 a4b8 e0a5 8720 e0a4 aae0 a4b9 e0a4   ...... ........
+00001320: b2e0 a587 20e0 a4ae e0a5 82e0 a4b2 20e0  .... ......... .
+00001330: a4b8 e0a4 bfe0 a4b8 e0a5 8de0 a49f e0a4  ................
+00001340: ae20 e0a4 aae0 a58d e0a4 b0e0 a589 e0a4  . ..............
+00001350: aee0 a58d e0a4 aae0 a58d e0a4 9f22 2c0a  .............",.
+00001360: 2020 2020 2261 695f 636f 6e66 6967 5f62      "ai_config_b
+00001370: 6173 655f 7379 7374 656d 5f70 726f 6d70  ase_system_promp
+00001380: 745f 6564 6974 5f61 6363 6573 7369 626c  t_edit_accessibl
+00001390: 655f 6465 7363 7269 7074 696f 6e22 3a0a  e_description":.
+000013a0: 2020 2020 2020 2020 22e0 a4aa e0a5 8de0          ".......
+000013b0: a4b0 e0a4 a4e0 a58d e0a4 afe0 a587 e0a4  ................
+000013c0: 9520 e0a4 85e0 a4a8 e0a5 81e0 a4b0 e0a5  . ..............
+000013d0: 8be0 a4a7 20e0 a4b8 e0a5 8720 e0a4 aae0  .... ...... ....
+000013e0: a4b9 e0a4 b2e0 a587 20e0 a4ae e0a5 82e0  ........ .......
+000013f0: a4b2 20e0 a4b8 e0a4 bfe0 a4b8 e0a5 8de0  .. .............
+00001400: a49f e0a4 ae20 e0a4 aae0 a58d e0a4 b0e0  ..... ..........
+00001410: a589 e0a4 aee0 a58d e0a4 aae0 a58d e0a4  ................
+00001420: 9fe0 a5a4 20e0 a4af e0a4 b920 e0a4 b8e0  .... ...... ....
+00001430: a4be e0a4 a6e0 a4be 20e0 a4aa e0a4 bee0  ........ .......
+00001440: a4a0 20e0 a4b9 e0a5 88e0 a5a4 222c 0a20  .. .........",. 
+00001450: 2020 2022 6169 5f63 6f6e 6669 675f 6261     "ai_config_ba
+00001460: 7365 5f72 6573 706f 6e73 655f 6d61 785f  se_response_max_
+00001470: 746f 6b65 6e73 5f6c 6162 656c 223a 2022  tokens_label": "
+00001480: e0a4 85e0 a4a7 e0a4 bfe0 a495 e0a4 a4e0  ................
+00001490: a4ae 20e0 a4aa e0a5 8de0 a4b0 e0a4 a4e0  .. .............
+000014a0: a4bf e0a4 b8e0 a4be e0a4 a620 e0a4 9fe0  ........... ....
+000014b0: a58b e0a4 95e0 a4a8 e0a5 8de0 a4b8 222c  ..............",
+000014c0: 0a20 2020 2022 6169 5f63 6f6e 6669 675f  .    "ai_config_
+000014d0: 6261 7365 5f72 6573 706f 6e73 655f 6d61  base_response_ma
+000014e0: 785f 746f 6b65 6e73 5f69 6e70 7574 5f61  x_tokens_input_a
+000014f0: 6363 6573 7369 626c 655f 6465 7363 7269  ccessible_descri
+00001500: 7074 696f 6e22 3a0a 2020 2020 2020 2020  ption":.        
+00001510: 22e0 a4aa e0a5 8de0 a4b0 e0a4 a4e0 a4bf  "...............
+00001520: e0a4 b8e0 a4be e0a4 a620 e0a4 aee0 a587  ......... ......
+00001530: e0a4 8220 e0a4 aae0 a58d e0a4 b0e0 a4be  ... ............
+00001540: e0a4 aae0 a58d e0a4 a420 e0a4 95e0 a4b0  ......... ......
+00001550: e0a4 a8e0 a587 20e0 a495 e0a5 8720 e0a4  ...... ...... ..
+00001560: b2e0 a4bf e0a4 8f20 e0a4 85e0 a4a7 e0a4  ....... ........
+00001570: bfe0 a495 e0a4 a4e0 a4ae 20e0 a49f e0a5  .......... .....
+00001580: 8be0 a495 e0a4 a8e0 a58d e0a4 b820 e0a4  ............. ..
+00001590: 95e0 a580 20e0 a4b8 e0a4 82e0 a496 e0a5  .... ...........
+000015a0: 8de0 a4af e0a4 be22 0a7d                 .......".}
```

### Comparing `notolog-0.9.1b1/app/lexemes/in/ai_assistant.py` & `notolog-0.9.1b2/notolog/lexemes/in/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/in/color_picker_dialog.py` & `notolog-0.9.1b2/notolog/lexemes/in/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/in/main_menu.py` & `notolog-0.9.1b2/notolog/lexemes/in/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/in/statusbar.py` & `notolog-0.9.1b2/notolog/lexemes/in/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/in/toolbar.py` & `notolog-0.9.1b2/notolog/lexemes/in/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/it/ai_assistant.py` & `notolog-0.9.1b2/notolog/lexemes/it/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/it/color_picker_dialog.py` & `notolog-0.9.1b2/notolog/lexemes/it/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/it/common.py` & `notolog-0.9.1b2/notolog/lexemes/it/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     "save_active_file_error_occurred": "Impossibile salvare il file, si è verificato un errore",
 
     "expandable_block_default_title": "Ulteriori informazioni...",
 
     "dialog_color_picker_color_copied_to_the_clipboard": "Il testo formattato è stato copiato negli appunti",
 
     "popup_about_title": "Informazioni sull'Applicazione",
-    "popup_about_app_name_description": "Editor Markdown",
+    "popup_about_app_name_description": "Editor Markdown Python",
 
     "popup_about_version": "Versione",
     "popup_about_license": "Licenza",
     "popup_about_website": "Sito Web",
     "popup_about_repository": "GitHub",
     "popup_about_pypi": "PyPi",
     "popup_about_date": "Data",
```

### Comparing `notolog-0.9.1b1/app/lexemes/it/main_menu.py` & `notolog-0.9.1b2/notolog/lexemes/it/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/it/settings_dialog.py` & `notolog-0.9.1b2/notolog/lexemes/it/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/it/statusbar.py` & `notolog-0.9.1b2/notolog/lexemes/zh/statusbar.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# Italian lexemes statusbar.py
+# Chinese lexemes statusbar.py
 lexemes = {
-    "statusbar_litter_bin_label": "Cestino",
-    "statusbar_litter_bin_accessible_name": "Mostra il contenuto del cestino",
+    "statusbar_litter_bin_label": "垃圾箱",
+    "statusbar_litter_bin_accessible_name": "显示垃圾箱内容",
 
     "statusbar_save_progress_label": b'\xf0\x9f\x92\xbe',
     "statusbar_encryption_symbol_encrypted_label": b'\xf0\x9f\x94\x92',
     "statusbar_encryption_symbol_unencrypted_label": b'\xf0\x9f\x94\x93',
 
-    "statusbar_mode_label_mode_view": "Modalità Visualizza",
-    "statusbar_mode_label_mode_edit": "Modalità Modifica",
-    "statusbar_mode_label_mode_source": "Modalità Sorgente",
+    "statusbar_mode_label_mode_view": "查看模式",
+    "statusbar_mode_label_mode_edit": "编辑模式",
+    "statusbar_mode_label_mode_source": "源代码模式",
 
     "statusbar_source_label_source_markdown": "Markdown",
     "statusbar_source_label_source_html": "HTML",
 
     "statusbar_encryption_label": "{encryption} {icon}",
-    "statusbar_encryption_label_encryption_plain": "Normale",
-    "statusbar_encryption_label_encryption_encrypted": "Criptato",
+    "statusbar_encryption_label_encryption_plain": "明文",
+    "statusbar_encryption_label_encryption_encrypted": "加密",
 
-    "statusbar_cursor_label": "linea: {line} → col: {column}",
-    "statusbar_cursor_label_selected": "linea: {line} → col: {column} → sel: {selected}",
-    "statusbar_cursor_label_with_global": "linea: {line} → col: {column} → pos: {position}",
-    "statusbar_cursor_label_selected_with_global": "linea: {line} → col: {column} → pos: {position} → sel: {selected}",
+    "statusbar_cursor_label": "行: {line} → 列: {column}",
+    "statusbar_cursor_label_selected": "行: {line} → 列: {column} → 选: {selected}",
+    "statusbar_cursor_label_with_global": "行: {line} → 列: {column} → 位: {position}",
+    "statusbar_cursor_label_selected_with_global": "行: {line} → 列: {column} → 位: {position} → 选: {selected}",
 }
```

### Comparing `notolog-0.9.1b1/app/lexemes/it/toolbar.py` & `notolog-0.9.1b2/notolog/lexemes/it/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/ja/__pycache__/main_menu.cpython-39.pyc` & `notolog-0.9.1b2/notolog/lexemes/ja/main_menu.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,151 +1,153 @@
-00000000: 610d 0d0a 0000 0000 40a8 3666 8b09 0000  a.......@.6f....
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0029 0000 0040 0000 0073 5a00 0000 6400  .)...@...sZ...d.
-00000030: 6401 6402 6403 6404 6404 6405 6406 6407  d.d.d.d.d.d.d.d.
-00000040: 6408 6409 640a 640b 640b 6401 640c 640d  d.d.d.d.d.d.d.d.
-00000050: 640e 640f 6410 6411 6412 6413 6414 6415  d.d.d.d.d.d.d.d.
-00000060: 6416 6417 6418 6419 641a 641b 641c 641d  d.d.d.d.d.d.d.d.
-00000070: 641d 641e 641e 641f 6420 6421 6421 6422  d.d.d.d.d d!d!d"
-00000080: 9c28 5a00 6423 5300 2924 750c 0000 00e3  .(Z.d#S.)$u.....
-00000090: 8395 e382 a1e3 82a4 e383 ab75 0600 0000  ...........u....
-000000a0: e7b7 a8e9 9b86 7509 0000 00e3 8384 e383  ......u.........
-000000b0: bce3 83ab 7509 0000 00e3 8398 e383 abe3  ....u...........
-000000c0: 8397 751b 0000 00e6 96b0 e381 97e3 8184  ..u.............
-000000d0: e383 89e3 82ad e383 a5e3 83a1 e383 b3e3  ................
-000000e0: 8388 7506 0000 00e9 968b e381 8f75 1b00  ..u..........u..
-000000f0: 0000 e383 89e3 82ad e383 a5e3 83a1 e383  ................
-00000100: b3e3 8388 e382 92e9 968b e381 8f75 0600  .............u..
-00000110: 0000 e4bf 9de5 ad98 751b 0000 00e3 8389  ........u.......
-00000120: e382 ade3 83a5 e383 a1e3 83b3 e383 88e3  ................
-00000130: 8292 e4bf 9de5 ad98 7518 0000 00e5 908d  ........u.......
-00000140: e589 8de3 8292 e4bb 98e3 8191 e381 a6e4  ................
-00000150: bf9d e5ad 9875 2700 0000 e383 89e3 82ad  .....u'.........
-00000160: e383 a5e3 83a1 e383 b3e3 8388 e381 aee3  ................
-00000170: 82b3 e383 94e3 83bc e382 92e4 bf9d e5ad  ................
-00000180: 9875 1200 0000 e382 a2e3 8397 e383 aae3  .u..............
-00000190: 8292 e7b5 82e4 ba86 7515 0000 00e3 8395  ........u.......
-000001a0: e382 a1e3 82a4 e383 abe3 8292 e7b7 a8e9  ................
-000001b0: 9b86 7509 0000 00e3 82bd e383 bce3 82b9  ..u.............
-000001c0: 7512 0000 00e3 82bd e383 bce3 82b9 e382  u...............
-000001d0: b3e3 83bc e383 8975 0600 0000 e5a4 aae5  .......u........
-000001e0: ad97 7518 0000 00e5 a4aa e5ad 97e3 8386  ..u.............
-000001f0: e382 ade3 82b9 e383 88e5 bda2 e5bc 8f75  ...............u
-00000200: 0f00 0000 e382 a4e3 82bf e383 aae3 8383  ................
-00000210: e382 af75 2100 0000 e382 a4e3 82bf e383  ...u!...........
-00000220: aae3 8383 e382 afe3 8386 e382 ade3 82b9  ................
-00000230: e383 88e5 bda2 e5bc 8f75 0600 0000 e4b8  .........u......
-00000240: 8be7 b79a 7518 0000 00e4 b88b e7b7 9ae3  ....u...........
-00000250: 8386 e382 ade3 82b9 e383 88e5 bda2 e5bc  ................
-00000260: 8f75 0f00 0000 e58f 96e3 828a e6b6 88e3  .u..............
-00000270: 8197 e7b7 9a75 2100 0000 e58f 96e3 828a  .....u!.........
-00000280: e6b6 88e3 8197 e7b7 9ae3 8386 e382 ade3  ................
-00000290: 82b9 e383 88e5 bda2 e5bc 8f75 1200 0000  ...........u....
-000002a0: e383 96e3 83ad e383 83e3 82af e5bc 95e7  ................
-000002b0: 94a8 7524 0000 00e3 8396 e383 ade3 8383  ..u$............
-000002c0: e382 afe5 bc95 e794 a8e3 8386 e382 ade3  ................
-000002d0: 82b9 e383 88e5 bda2 e5bc 8f75 1400 0000  ...........u....
-000002e0: 4149 e382 a2e3 82b7 e382 b9e3 82bf e383  AI..............
-000002f0: b3e3 8388 751d 0000 0041 49e3 82a2 e382  ....u....AI.....
-00000300: b7e3 82b9 e382 bfe3 83b3 e383 88e3 8292  ................
-00000310: e8b5 b7e5 8b95 7515 0000 00e3 82ab e383  ......u.........
-00000320: a9e3 83bc e383 94e3 8383 e382 abe3 83bc  ................
-00000330: 7518 0000 00e3 8386 e382 ade3 82b9 e383  u...............
-00000340: 88e8 89b2 e382 92e9 81b8 e68a 9e75 0f00  .............u..
-00000350: 0000 4d61 726b 646f 776e 20e6 a78b e696  ..Markdown .....
-00000360: 8775 0f00 0000 e69b b4e6 96b0 e382 92e7  .u..............
-00000370: a2ba e8aa 8d75 0c00 0000 e383 90e3 82b0  .....u..........
-00000380: e5a0 b1e5 918a 7515 0000 00e3 8390 e382  ......u.........
-00000390: b0e5 a0b1 e591 8ae3 8292 e980 81e4 bfa1  ................
-000003a0: 7506 0000 00e6 8385 e5a0 b129 28da 1067  u..........)(..g
-000003b0: 726f 7570 5f66 696c 655f 6c61 6265 6cda  roup_file_label.
-000003c0: 1067 726f 7570 5f65 6469 745f 6c61 6265  .group_edit_labe
-000003d0: 6cda 1167 726f 7570 5f74 6f6f 6c73 5f6c  l..group_tools_l
-000003e0: 6162 656c da10 6772 6f75 705f 6865 6c70  abel..group_help
-000003f0: 5f6c 6162 656c da1f 6163 7469 6f6e 735f  _label..actions_
-00000400: 6669 6c65 5f6c 6162 656c 5f6e 6577 5f64  file_label_new_d
-00000410: 6f63 756d 656e 74da 2961 6374 696f 6e73  ocument.)actions
-00000420: 5f66 696c 655f 6163 6365 7373 6962 6c65  _file_accessible
-00000430: 5f6e 616d 655f 6e65 775f 646f 6375 6d65  _name_new_docume
-00000440: 6e74 da17 6163 7469 6f6e 735f 6669 6c65  nt..actions_file
-00000450: 5f6c 6162 656c 5f6f 7065 6eda 2161 6374  _label_open.!act
-00000460: 696f 6e73 5f66 696c 655f 6163 6365 7373  ions_file_access
-00000470: 6962 6c65 5f6e 616d 655f 6f70 656e da17  ible_name_open..
-00000480: 6163 7469 6f6e 735f 6669 6c65 5f6c 6162  actions_file_lab
-00000490: 656c 5f73 6176 65da 2161 6374 696f 6e73  el_save.!actions
-000004a0: 5f66 696c 655f 6163 6365 7373 6962 6c65  _file_accessible
-000004b0: 5f6e 616d 655f 7361 7665 da1a 6163 7469  _name_save..acti
-000004c0: 6f6e 735f 6669 6c65 5f6c 6162 656c 5f73  ons_file_label_s
-000004d0: 6176 655f 6173 da24 6163 7469 6f6e 735f  ave_as.$actions_
-000004e0: 6669 6c65 5f61 6363 6573 7369 626c 655f  file_accessible_
-000004f0: 6e61 6d65 5f73 6176 655f 6173 da17 6163  name_save_as..ac
-00000500: 7469 6f6e 735f 6669 6c65 5f6c 6162 656c  tions_file_label
-00000510: 5f65 7869 74da 2161 6374 696f 6e73 5f66  _exit.!actions_f
-00000520: 696c 655f 6163 6365 7373 6962 6c65 5f6e  ile_accessible_n
-00000530: 616d 655f 6578 6974 da16 6564 6974 5f61  ame_exit..edit_a
-00000540: 6374 696f 6e73 5f65 6469 745f 6d6f 6465  ctions_edit_mode
-00000550: da26 6564 6974 5f61 6374 696f 6e73 5f61  .&edit_actions_a
-00000560: 6363 6573 7369 626c 655f 6e61 6d65 5f65  ccessible_name_e
-00000570: 6469 745f 6d6f 6465 da18 6564 6974 5f61  dit_mode..edit_a
-00000580: 6374 696f 6e73 5f73 6f75 7263 655f 6d6f  ctions_source_mo
-00000590: 6465 da28 6564 6974 5f61 6374 696f 6e73  de.(edit_actions
-000005a0: 5f61 6363 6573 7369 626c 655f 6e61 6d65  _accessible_name
-000005b0: 5f73 6f75 7263 655f 6d6f 6465 da11 6564  _source_mode..ed
-000005c0: 6974 5f61 6374 696f 6e73 5f62 6f6c 64da  it_actions_bold.
-000005d0: 2165 6469 745f 6163 7469 6f6e 735f 6163  !edit_actions_ac
-000005e0: 6365 7373 6962 6c65 5f6e 616d 655f 626f  cessible_name_bo
-000005f0: 6c64 da13 6564 6974 5f61 6374 696f 6e73  ld..edit_actions
-00000600: 5f69 7461 6c69 63da 2365 6469 745f 6163  _italic.#edit_ac
-00000610: 7469 6f6e 735f 6163 6365 7373 6962 6c65  tions_accessible
-00000620: 5f6e 616d 655f 6974 616c 6963 da16 6564  _name_italic..ed
-00000630: 6974 5f61 6374 696f 6e73 5f75 6e64 6572  it_actions_under
-00000640: 6c69 6e65 da26 6564 6974 5f61 6374 696f  line.&edit_actio
-00000650: 6e73 5f61 6363 6573 7369 626c 655f 6e61  ns_accessible_na
-00000660: 6d65 5f75 6e64 6572 6c69 6e65 da1a 6564  me_underline..ed
-00000670: 6974 5f61 6374 696f 6e73 5f73 7472 696b  it_actions_strik
-00000680: 6574 6872 6f75 6768 da2a 6564 6974 5f61  ethrough.*edit_a
-00000690: 6374 696f 6e73 5f61 6363 6573 7369 626c  ctions_accessibl
-000006a0: 655f 6e61 6d65 5f73 7472 696b 6574 6872  e_name_strikethr
-000006b0: 6f75 6768 da17 6564 6974 5f61 6374 696f  ough..edit_actio
-000006c0: 6e73 5f62 6c6f 636b 7175 6f74 65da 2765  ns_blockquote.'e
-000006d0: 6469 745f 6163 7469 6f6e 735f 6163 6365  dit_actions_acce
-000006e0: 7373 6962 6c65 5f6e 616d 655f 626c 6f63  ssible_name_bloc
-000006f0: 6b71 756f 7465 da1a 746f 6f6c 735f 6163  kquote..tools_ac
-00000700: 7469 6f6e 735f 6169 5f61 7373 6973 7461  tions_ai_assista
-00000710: 6e74 da2a 746f 6f6c 735f 6163 7469 6f6e  nt.*tools_action
-00000720: 735f 6163 6365 7373 6962 6c65 5f6e 616d  s_accessible_nam
-00000730: 655f 6169 5f61 7373 6973 7461 6e74 da1a  e_ai_assistant..
-00000740: 746f 6f6c 735f 6163 7469 6f6e 735f 636f  tools_actions_co
-00000750: 6c6f 725f 7069 636b 6572 da2a 746f 6f6c  lor_picker.*tool
-00000760: 735f 6163 7469 6f6e 735f 6163 6365 7373  s_actions_access
-00000770: 6962 6c65 5f6e 616d 655f 636f 6c6f 725f  ible_name_color_
-00000780: 7069 636b 6572 5a1c 6163 7469 6f6e 735f  pickerZ.actions_
-00000790: 6865 6c70 5f6c 6162 656c 5f6d 645f 7379  help_label_md_sy
-000007a0: 6e74 6178 5a26 6163 7469 6f6e 735f 6865  ntaxZ&actions_he
-000007b0: 6c70 5f61 6363 6573 7369 626c 655f 6e61  lp_accessible_na
-000007c0: 6d65 5f6d 645f 7379 6e74 6178 da24 6163  me_md_syntax.$ac
-000007d0: 7469 6f6e 735f 6865 6c70 5f6c 6162 656c  tions_help_label
-000007e0: 5f63 6865 636b 5f66 6f72 5f75 7064 6174  _check_for_updat
-000007f0: 6573 da2e 6163 7469 6f6e 735f 6865 6c70  es..actions_help
-00000800: 5f61 6363 6573 7369 626c 655f 6e61 6d65  _accessible_name
-00000810: 5f63 6865 636b 5f66 6f72 5f75 7064 6174  _check_for_updat
-00000820: 6573 da1d 6163 7469 6f6e 735f 6865 6c70  es..actions_help
-00000830: 5f6c 6162 656c 5f62 7567 5f72 6570 6f72  _label_bug_repor
-00000840: 74da 2761 6374 696f 6e73 5f68 656c 705f  t.'actions_help_
-00000850: 6163 6365 7373 6962 6c65 5f6e 616d 655f  accessible_name_
-00000860: 6275 675f 7265 706f 7274 da18 6163 7469  bug_report..acti
-00000870: 6f6e 735f 6865 6c70 5f6c 6162 656c 5f61  ons_help_label_a
-00000880: 626f 7574 da22 6163 7469 6f6e 735f 6865  bout."actions_he
-00000890: 6c70 5f61 6363 6573 7369 626c 655f 6e61  lp_accessible_na
-000008a0: 6d65 5f61 626f 7574 4e29 01da 076c 6578  me_aboutN)...lex
-000008b0: 656d 6573 a900 7228 0000 0072 2800 0000  emes..r(...r(...
-000008c0: fa49 2f55 7365 7273 2f76 6164 696b 7573  .I/Users/vadikus
-000008d0: 2f50 7963 6861 726d 5072 6f6a 6563 7473  /PycharmProjects
-000008e0: 2f6e 6f74 6f6c 6f67 2d65 6469 746f 722f  /notolog-editor/
-000008f0: 6170 702f 6c65 7865 6d65 732f 6a61 2f6d  app/lexemes/ja/m
-00000900: 6169 6e5f 6d65 6e75 2e70 79da 083c 6d6f  ain_menu.py..<mo
-00000910: 6475 6c65 3e03 0000 0073 5000 0000 0201  dule>....sP.....
-00000920: 0201 0201 0202 0201 0201 0201 0201 0201  ................
-00000930: 0201 0201 0201 0201 0202 0201 0201 0201  ................
-00000940: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00000950: 0201 0201 0202 0201 0201 0201 0202 0201  ................
-00000960: 0201 0201 0201 0201 0201 0201 02d4       ..............
+00000000: 2320 4a61 7061 6e65 7365 206c 6578 656d  # Japanese lexem
+00000010: 6573 206d 6169 6e5f 6d65 6e75 2e70 790a  es main_menu.py.
+00000020: 6c65 7865 6d65 7320 3d20 7b0a 2020 2020  lexemes = {.    
+00000030: 2267 726f 7570 5f66 696c 655f 6c61 6265  "group_file_labe
+00000040: 6c22 3a20 22e3 8395 e382 a1e3 82a4 e383  l": "...........
+00000050: ab22 2c0a 2020 2020 2267 726f 7570 5f65  .",.    "group_e
+00000060: 6469 745f 6c61 6265 6c22 3a20 22e7 b7a8  dit_label": "...
+00000070: e99b 8622 2c0a 2020 2020 2267 726f 7570  ...",.    "group
+00000080: 5f74 6f6f 6c73 5f6c 6162 656c 223a 2022  _tools_label": "
+00000090: e383 84e3 83bc e383 ab22 2c0a 2020 2020  .........",.    
+000000a0: 2267 726f 7570 5f68 656c 705f 6c61 6265  "group_help_labe
+000000b0: 6c22 3a20 22e3 8398 e383 abe3 8397 222c  l": ".........",
+000000c0: 0a0a 2020 2020 2261 6374 696f 6e73 5f66  ..    "actions_f
+000000d0: 696c 655f 6c61 6265 6c5f 6e65 775f 646f  ile_label_new_do
+000000e0: 6375 6d65 6e74 223a 2022 e696 b0e3 8197  cument": "......
+000000f0: e381 84e3 8389 e382 ade3 83a5 e383 a1e3  ................
+00000100: 83b3 e383 8822 2c0a 2020 2020 2261 6374  .....",.    "act
+00000110: 696f 6e73 5f66 696c 655f 6163 6365 7373  ions_file_access
+00000120: 6962 6c65 5f6e 616d 655f 6e65 775f 646f  ible_name_new_do
+00000130: 6375 6d65 6e74 223a 2022 e696 b0e3 8197  cument": "......
+00000140: e381 84e3 8389 e382 ade3 83a5 e383 a1e3  ................
+00000150: 83b3 e383 8822 2c0a 2020 2020 2261 6374  .....",.    "act
+00000160: 696f 6e73 5f66 696c 655f 6c61 6265 6c5f  ions_file_label_
+00000170: 6f70 656e 223a 2022 e996 8be3 818f 222c  open": "......",
+00000180: 0a20 2020 2022 6163 7469 6f6e 735f 6669  .    "actions_fi
+00000190: 6c65 5f61 6363 6573 7369 626c 655f 6e61  le_accessible_na
+000001a0: 6d65 5f6f 7065 6e22 3a20 22e3 8389 e382  me_open": ".....
+000001b0: ade3 83a5 e383 a1e3 83b3 e383 88e3 8292  ................
+000001c0: e996 8be3 818f 222c 0a20 2020 2022 6163  ......",.    "ac
+000001d0: 7469 6f6e 735f 6669 6c65 5f6c 6162 656c  tions_file_label
+000001e0: 5f73 6176 6522 3a20 22e4 bf9d e5ad 9822  _save": "......"
+000001f0: 2c0a 2020 2020 2261 6374 696f 6e73 5f66  ,.    "actions_f
+00000200: 696c 655f 6163 6365 7373 6962 6c65 5f6e  ile_accessible_n
+00000210: 616d 655f 7361 7665 223a 2022 e383 89e3  ame_save": "....
+00000220: 82ad e383 a5e3 83a1 e383 b3e3 8388 e382  ................
+00000230: 92e4 bf9d e5ad 9822 2c0a 2020 2020 2261  .......",.    "a
+00000240: 6374 696f 6e73 5f66 696c 655f 6c61 6265  ctions_file_labe
+00000250: 6c5f 7361 7665 5f61 7322 3a20 22e5 908d  l_save_as": "...
+00000260: e589 8de3 8292 e4bb 98e3 8191 e381 a6e4  ................
+00000270: bf9d e5ad 9822 2c0a 2020 2020 2261 6374  .....",.    "act
+00000280: 696f 6e73 5f66 696c 655f 6163 6365 7373  ions_file_access
+00000290: 6962 6c65 5f6e 616d 655f 7361 7665 5f61  ible_name_save_a
+000002a0: 7322 3a20 22e3 8389 e382 ade3 83a5 e383  s": "...........
+000002b0: a1e3 83b3 e383 88e3 81ae e382 b3e3 8394  ................
+000002c0: e383 bce3 8292 e4bf 9de5 ad98 222c 0a20  ............",. 
+000002d0: 2020 2022 6163 7469 6f6e 735f 6669 6c65     "actions_file
+000002e0: 5f6c 6162 656c 5f65 7869 7422 3a20 22e3  _label_exit": ".
+000002f0: 82a2 e383 97e3 83aa e382 92e7 b582 e4ba  ................
+00000300: 8622 2c0a 2020 2020 2261 6374 696f 6e73  .",.    "actions
+00000310: 5f66 696c 655f 6163 6365 7373 6962 6c65  _file_accessible
+00000320: 5f6e 616d 655f 6578 6974 223a 2022 e382  _name_exit": "..
+00000330: a2e3 8397 e383 aae3 8292 e7b5 82e4 ba86  ................
+00000340: 222c 0a0a 2020 2020 2265 6469 745f 6163  ",..    "edit_ac
+00000350: 7469 6f6e 735f 6564 6974 5f6d 6f64 6522  tions_edit_mode"
+00000360: 3a20 22e7 b7a8 e99b 8622 2c0a 2020 2020  : "......",.    
+00000370: 2265 6469 745f 6163 7469 6f6e 735f 6163  "edit_actions_ac
+00000380: 6365 7373 6962 6c65 5f6e 616d 655f 6564  cessible_name_ed
+00000390: 6974 5f6d 6f64 6522 3a20 22e3 8395 e382  it_mode": ".....
+000003a0: a1e3 82a4 e383 abe3 8292 e7b7 a8e9 9b86  ................
+000003b0: 222c 0a20 2020 2022 6564 6974 5f61 6374  ",.    "edit_act
+000003c0: 696f 6e73 5f73 6f75 7263 655f 6d6f 6465  ions_source_mode
+000003d0: 223a 2022 e382 bde3 83bc e382 b922 2c0a  ": ".........",.
+000003e0: 2020 2020 2265 6469 745f 6163 7469 6f6e      "edit_action
+000003f0: 735f 6163 6365 7373 6962 6c65 5f6e 616d  s_accessible_nam
+00000400: 655f 736f 7572 6365 5f6d 6f64 6522 3a20  e_source_mode": 
+00000410: 22e3 82bd e383 bce3 82b9 e382 b3e3 83bc  "...............
+00000420: e383 8922 2c0a 2020 2020 2265 6469 745f  ...",.    "edit_
+00000430: 6163 7469 6f6e 735f 626f 6c64 223a 2022  actions_bold": "
+00000440: e5a4 aae5 ad97 222c 0a20 2020 2022 6564  ......",.    "ed
+00000450: 6974 5f61 6374 696f 6e73 5f61 6363 6573  it_actions_acces
+00000460: 7369 626c 655f 6e61 6d65 5f62 6f6c 6422  sible_name_bold"
+00000470: 3a20 22e5 a4aa e5ad 97e3 8386 e382 ade3  : ".............
+00000480: 82b9 e383 88e5 bda2 e5bc 8f22 2c0a 2020  ...........",.  
+00000490: 2020 2265 6469 745f 6163 7469 6f6e 735f    "edit_actions_
+000004a0: 6974 616c 6963 223a 2022 e382 a4e3 82bf  italic": "......
+000004b0: e383 aae3 8383 e382 af22 2c0a 2020 2020  .........",.    
+000004c0: 2265 6469 745f 6163 7469 6f6e 735f 6163  "edit_actions_ac
+000004d0: 6365 7373 6962 6c65 5f6e 616d 655f 6974  cessible_name_it
+000004e0: 616c 6963 223a 2022 e382 a4e3 82bf e383  alic": "........
+000004f0: aae3 8383 e382 afe3 8386 e382 ade3 82b9  ................
+00000500: e383 88e5 bda2 e5bc 8f22 2c0a 2020 2020  .........",.    
+00000510: 2265 6469 745f 6163 7469 6f6e 735f 756e  "edit_actions_un
+00000520: 6465 726c 696e 6522 3a20 22e4 b88b e7b7  derline": ".....
+00000530: 9a22 2c0a 2020 2020 2265 6469 745f 6163  .",.    "edit_ac
+00000540: 7469 6f6e 735f 6163 6365 7373 6962 6c65  tions_accessible
+00000550: 5f6e 616d 655f 756e 6465 726c 696e 6522  _name_underline"
+00000560: 3a20 22e4 b88b e7b7 9ae3 8386 e382 ade3  : ".............
+00000570: 82b9 e383 88e5 bda2 e5bc 8f22 2c0a 2020  ...........",.  
+00000580: 2020 2265 6469 745f 6163 7469 6f6e 735f    "edit_actions_
+00000590: 7374 7269 6b65 7468 726f 7567 6822 3a20  strikethrough": 
+000005a0: 22e5 8f96 e382 8ae6 b688 e381 97e7 b79a  "...............
+000005b0: 222c 0a20 2020 2022 6564 6974 5f61 6374  ",.    "edit_act
+000005c0: 696f 6e73 5f61 6363 6573 7369 626c 655f  ions_accessible_
+000005d0: 6e61 6d65 5f73 7472 696b 6574 6872 6f75  name_strikethrou
+000005e0: 6768 223a 2022 e58f 96e3 828a e6b6 88e3  gh": "..........
+000005f0: 8197 e7b7 9ae3 8386 e382 ade3 82b9 e383  ................
+00000600: 88e5 bda2 e5bc 8f22 2c0a 2020 2020 2265  .......",.    "e
+00000610: 6469 745f 6163 7469 6f6e 735f 626c 6f63  dit_actions_bloc
+00000620: 6b71 756f 7465 223a 2022 e383 96e3 83ad  kquote": "......
+00000630: e383 83e3 82af e5bc 95e7 94a8 222c 0a20  ............",. 
+00000640: 2020 2022 6564 6974 5f61 6374 696f 6e73     "edit_actions
+00000650: 5f61 6363 6573 7369 626c 655f 6e61 6d65  _accessible_name
+00000660: 5f62 6c6f 636b 7175 6f74 6522 3a20 22e3  _blockquote": ".
+00000670: 8396 e383 ade3 8383 e382 afe5 bc95 e794  ................
+00000680: a8e3 8386 e382 ade3 82b9 e383 88e5 bda2  ................
+00000690: e5bc 8f22 2c0a 0a20 2020 2022 746f 6f6c  ...",..    "tool
+000006a0: 735f 6163 7469 6f6e 735f 6169 5f61 7373  s_actions_ai_ass
+000006b0: 6973 7461 6e74 223a 2022 4149 e382 a2e3  istant": "AI....
+000006c0: 82b7 e382 b9e3 82bf e383 b3e3 8388 222c  ..............",
+000006d0: 0a20 2020 2022 746f 6f6c 735f 6163 7469  .    "tools_acti
+000006e0: 6f6e 735f 6163 6365 7373 6962 6c65 5f6e  ons_accessible_n
+000006f0: 616d 655f 6169 5f61 7373 6973 7461 6e74  ame_ai_assistant
+00000700: 223a 2022 4149 e382 a2e3 82b7 e382 b9e3  ": "AI..........
+00000710: 82bf e383 b3e3 8388 e382 92e8 b5b7 e58b  ................
+00000720: 9522 2c0a 2020 2020 2274 6f6f 6c73 5f61  .",.    "tools_a
+00000730: 6374 696f 6e73 5f63 6f6c 6f72 5f70 6963  ctions_color_pic
+00000740: 6b65 7222 3a20 22e3 82ab e383 a9e3 83bc  ker": ".........
+00000750: e383 94e3 8383 e382 abe3 83bc 222c 0a20  ............",. 
+00000760: 2020 2022 746f 6f6c 735f 6163 7469 6f6e     "tools_action
+00000770: 735f 6163 6365 7373 6962 6c65 5f6e 616d  s_accessible_nam
+00000780: 655f 636f 6c6f 725f 7069 636b 6572 223a  e_color_picker":
+00000790: 2022 e383 86e3 82ad e382 b9e3 8388 e889   "..............
+000007a0: b2e3 8292 e981 b8e6 8a9e 222c 0a0a 2020  ..........",..  
+000007b0: 2020 2261 6374 696f 6e73 5f68 656c 705f    "actions_help_
+000007c0: 6c61 6265 6c5f 6d64 5f73 796e 7461 7822  label_md_syntax"
+000007d0: 3a20 224d 6172 6b64 6f77 6e20 e6a7 8be6  : "Markdown ....
+000007e0: 9687 222c 0a20 2020 2022 6163 7469 6f6e  ..",.    "action
+000007f0: 735f 6865 6c70 5f61 6363 6573 7369 626c  s_help_accessibl
+00000800: 655f 6e61 6d65 5f6d 645f 7379 6e74 6178  e_name_md_syntax
+00000810: 223a 2022 4d61 726b 646f 776e 20e6 a78b  ": "Markdown ...
+00000820: e696 8722 2c0a 2020 2020 2261 6374 696f  ...",.    "actio
+00000830: 6e73 5f68 656c 705f 6c61 6265 6c5f 6368  ns_help_label_ch
+00000840: 6563 6b5f 666f 725f 7570 6461 7465 7322  eck_for_updates"
+00000850: 3a20 22e6 9bb4 e696 b0e3 8292 e7a2 bae8  : ".............
+00000860: aa8d 222c 0a20 2020 2022 6163 7469 6f6e  ..",.    "action
+00000870: 735f 6865 6c70 5f61 6363 6573 7369 626c  s_help_accessibl
+00000880: 655f 6e61 6d65 5f63 6865 636b 5f66 6f72  e_name_check_for
+00000890: 5f75 7064 6174 6573 223a 2022 e69b b4e6  _updates": "....
+000008a0: 96b0 e382 92e7 a2ba e8aa 8d22 2c0a 2020  ...........",.  
+000008b0: 2020 2261 6374 696f 6e73 5f68 656c 705f    "actions_help_
+000008c0: 6c61 6265 6c5f 6275 675f 7265 706f 7274  label_bug_report
+000008d0: 223a 2022 e383 90e3 82b0 e5a0 b1e5 918a  ": "............
+000008e0: 222c 0a20 2020 2022 6163 7469 6f6e 735f  ",.    "actions_
+000008f0: 6865 6c70 5f61 6363 6573 7369 626c 655f  help_accessible_
+00000900: 6e61 6d65 5f62 7567 5f72 6570 6f72 7422  name_bug_report"
+00000910: 3a20 22e3 8390 e382 b0e5 a0b1 e591 8ae3  : ".............
+00000920: 8292 e980 81e4 bfa1 222c 0a20 2020 2022  ........",.    "
+00000930: 6163 7469 6f6e 735f 6865 6c70 5f6c 6162  actions_help_lab
+00000940: 656c 5f61 626f 7574 223a 2022 e683 85e5  el_about": "....
+00000950: a0b1 222c 0a20 2020 2022 6163 7469 6f6e  ..",.    "action
+00000960: 735f 6865 6c70 5f61 6363 6573 7369 626c  s_help_accessibl
+00000970: 655f 6e61 6d65 5f61 626f 7574 223a 2022  e_name_about": "
+00000980: e683 85e5 a0b1 222c 0a7d 0a              ......",.}.
```

### Comparing `notolog-0.9.1b1/app/lexemes/ja/ai_assistant.py` & `notolog-0.9.1b2/notolog/lexemes/ja/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/ja/color_picker_dialog.py` & `notolog-0.9.1b2/notolog/lexemes/ja/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/ja/common.py` & `notolog-0.9.1b2/notolog/lexemes/ja/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     "save_active_file_error_occurred": "ファイルを保存できませんでした。エラーが発生しました",
 
     "expandable_block_default_title": "詳細情報...",
 
     "dialog_color_picker_color_copied_to_the_clipboard": "フォーマットされたテキストがクリップボードにコピーされました",
 
     "popup_about_title": "アプリ情報",
-    "popup_about_app_name_description": "Markdown エディタ",
+    "popup_about_app_name_description": "Python Markdown エディタ",
 
     "popup_about_version": "バージョン",
     "popup_about_license": "ライセンス",
     "popup_about_website": "ウェブサイト",
     "popup_about_repository": "GitHub",
     "popup_about_pypi": "PyPi",
     "popup_about_date": "日付",
```

### Comparing `notolog-0.9.1b1/app/lexemes/ja/settings_dialog.py` & `notolog-0.9.1b2/notolog/lexemes/ja/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/ja/statusbar.py` & `notolog-0.9.1b2/notolog/lexemes/la/statusbar.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-# Japanese lexemes statusbar.py
+# Latin lexemes statusbar.py
 lexemes = {
-    "statusbar_litter_bin_label": "ごみ箱",
-    "statusbar_litter_bin_accessible_name": "ごみ箱の内容を表示",
+    "statusbar_litter_bin_label": "Fiscina",
+    "statusbar_litter_bin_accessible_name": "Ostendere contentum fiscinae",
 
     "statusbar_save_progress_label": b'\xf0\x9f\x92\xbe',
     "statusbar_encryption_symbol_encrypted_label": b'\xf0\x9f\x94\x92',
     "statusbar_encryption_symbol_unencrypted_label": b'\xf0\x9f\x94\x93',
 
-    "statusbar_mode_label_mode_view": "ビューモード",
-    "statusbar_mode_label_mode_edit": "編集モード",
-    "statusbar_mode_label_mode_source": "ソースモード",
+    "statusbar_mode_label_mode_view": "Modus Visum",
+    "statusbar_mode_label_mode_edit": "Modus Editio",
+    "statusbar_mode_label_mode_source": "Modus Fons",
 
     "statusbar_source_label_source_markdown": "Markdown",
     "statusbar_source_label_source_html": "HTML",
 
     "statusbar_encryption_label": "{encryption} {icon}",
-    "statusbar_encryption_label_encryption_plain": "プレーン",
-    "statusbar_encryption_label_encryption_encrypted": "暗号化",
+    "statusbar_encryption_label_encryption_plain": "Simplicitas",
+    "statusbar_encryption_label_encryption_encrypted": "Cryptatus",
 
-    "statusbar_cursor_label": "行: {line} → 列: {column}",
-    "statusbar_cursor_label_selected": "行: {line} → 列: {column} → 選択: {selected}",
-    "statusbar_cursor_label_with_global": "行: {line} → 列: {column} → 位置: {position}",
-    "statusbar_cursor_label_selected_with_global": "行: {line} → 列: {column} → 位置: {position} → 選択: {selected}",
+    "statusbar_cursor_label": "linea: {line} → columna: {column}",
+    "statusbar_cursor_label_selected": "linea: {line} → columna: {column} → selectus: {selected}",
+    "statusbar_cursor_label_with_global": "linea: {line} → columna: {column} → positio: {position}",
+    "statusbar_cursor_label_selected_with_global":
+        "linea: {line} → columna: {column} → positio: {position} → selectus: {selected}",
 }
```

### Comparing `notolog-0.9.1b1/app/lexemes/ja/toolbar.py` & `notolog-0.9.1b2/notolog/lexemes/ja/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/ko/ai_assistant.py` & `notolog-0.9.1b2/notolog/lexemes/ko/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/ko/color_picker_dialog.py` & `notolog-0.9.1b2/notolog/lexemes/ko/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/ko/common.py` & `notolog-0.9.1b2/notolog/lexemes/ko/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     "save_active_file_error_occurred": "파일을 저장할 수 없습니다. 오류가 발생했습니다",
 
     "expandable_block_default_title": "추가 정보...",
 
     "dialog_color_picker_color_copied_to_the_clipboard": "서식이 지정된 텍스트가 클립보드에 복사되었습니다",
 
     "popup_about_title": "애플리케이션 정보",
-    "popup_about_app_name_description": "마크다운 에디터",
+    "popup_about_app_name_description": "파이썬 마크다운 에디터",
 
     "popup_about_version": "버전",
     "popup_about_license": "라이선스",
     "popup_about_website": "웹사이트",
     "popup_about_repository": "GitHub",
     "popup_about_pypi": "PyPi",
     "popup_about_date": "날짜",
```

### Comparing `notolog-0.9.1b1/app/lexemes/ko/main_menu.py` & `notolog-0.9.1b2/notolog/lexemes/se/main_menu.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-# Korean lexemes main_menu.py
+# Swedish lexemes main_menu.py
 lexemes = {
-    "group_file_label": "파일",
-    "group_edit_label": "편집",
-    "group_tools_label": "도구",
-    "group_help_label": "도움말",
+    "group_file_label": "Fil",
+    "group_edit_label": "Redigera",
+    "group_tools_label": "Verktyg",
+    "group_help_label": "Hjälp",
 
-    "actions_file_label_new_document": "새 문서",
-    "actions_file_accessible_name_new_document": "새 문서",
-    "actions_file_label_open": "열기",
-    "actions_file_accessible_name_open": "문서 열기",
-    "actions_file_label_save": "저장",
-    "actions_file_accessible_name_save": "문서 저장",
-    "actions_file_label_save_as": "다른 이름으로 저장",
-    "actions_file_accessible_name_save_as": "문서 복사본 저장",
-    "actions_file_label_exit": "종료",
-    "actions_file_accessible_name_exit": "앱 종료",
+    "actions_file_label_new_document": "Nytt dokument",
+    "actions_file_accessible_name_new_document": "Nytt dokument",
+    "actions_file_label_open": "Öppna",
+    "actions_file_accessible_name_open": "Öppna dokument",
+    "actions_file_label_save": "Spara",
+    "actions_file_accessible_name_save": "Spara dokument",
+    "actions_file_label_save_as": "Spara som",
+    "actions_file_accessible_name_save_as": "Spara dokumentkopior",
+    "actions_file_label_exit": "Avsluta",
+    "actions_file_accessible_name_exit": "Avsluta programmet",
 
-    "edit_actions_edit_mode": "편집",
-    "edit_actions_accessible_name_edit_mode": "파일 편집",
-    "edit_actions_source_mode": "소스",
-    "edit_actions_accessible_name_source_mode": "소스 코드",
-    "edit_actions_bold": "굵게",
-    "edit_actions_accessible_name_bold": "굵은 텍스트 형식",
-    "edit_actions_italic": "기울임꼴",
-    "edit_actions_accessible_name_italic": "기울임꼴 텍스트 형식",
-    "edit_actions_underline": "밑줄",
-    "edit_actions_accessible_name_underline": "밑줄 텍스트 형식",
-    "edit_actions_strikethrough": "취소선",
-    "edit_actions_accessible_name_strikethrough": "취소선 텍스트 형식",
-    "edit_actions_blockquote": "블록 인용",
-    "edit_actions_accessible_name_blockquote": "블록 인용 텍스트 형식",
+    "edit_actions_edit_mode": "Redigera",
+    "edit_actions_accessible_name_edit_mode": "Redigera fil",
+    "edit_actions_source_mode": "Källkod",
+    "edit_actions_accessible_name_source_mode": "Källkod",
+    "edit_actions_bold": "Fet",
+    "edit_actions_accessible_name_bold": "Fet textformat",
+    "edit_actions_italic": "Kursiv",
+    "edit_actions_accessible_name_italic": "Kursiv textformat",
+    "edit_actions_underline": "Understrykning",
+    "edit_actions_accessible_name_underline": "Understruken textformat",
+    "edit_actions_strikethrough": "Genomstrykning",
+    "edit_actions_accessible_name_strikethrough": "Genomstruken textformat",
+    "edit_actions_blockquote": "Blockcitat",
+    "edit_actions_accessible_name_blockquote": "Blockcitat textformat",
 
-    "tools_actions_ai_assistant": "AI 보조",
-    "tools_actions_accessible_name_ai_assistant": "AI 보조 시작",
-    "tools_actions_color_picker": "색상 선택기",
-    "tools_actions_accessible_name_color_picker": "텍스트 색상 선택",
+    "tools_actions_ai_assistant": "AI-assistent",
+    "tools_actions_accessible_name_ai_assistant": "Starta AI-assistent",
+    "tools_actions_color_picker": "Färgväljare",
+    "tools_actions_accessible_name_color_picker": "Välj textfärg",
 
-    "actions_help_label_md_syntax": "Markdown 문법",
-    "actions_help_accessible_name_md_syntax": "Markdown 문법",
-    "actions_help_label_check_for_updates": "업데이트 확인",
-    "actions_help_accessible_name_check_for_updates": "업데이트 확인",
-    "actions_help_label_bug_report": "버그 보고",
-    "actions_help_accessible_name_bug_report": "버그 보고서 제출",
-    "actions_help_label_about": "정보",
-    "actions_help_accessible_name_about": "정보",
+    "actions_help_label_md_syntax": "Markdown-syntax",
+    "actions_help_accessible_name_md_syntax": "Markdown-syntax",
+    "actions_help_label_check_for_updates": "Sök efter uppdateringar",
+    "actions_help_accessible_name_check_for_updates": "Sök efter uppdateringar",
+    "actions_help_label_bug_report": "Felrapport",
+    "actions_help_accessible_name_bug_report": "Skicka felrapport",
+    "actions_help_label_about": "Om",
+    "actions_help_accessible_name_about": "Om"
 }
```

### Comparing `notolog-0.9.1b1/app/lexemes/ko/settings_dialog.py` & `notolog-0.9.1b2/notolog/lexemes/ko/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/ko/statusbar.py` & `notolog-0.9.1b2/notolog/lexemes/ko/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/ko/toolbar.py` & `notolog-0.9.1b2/notolog/lexemes/ko/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/la/ai_assistant.py` & `notolog-0.9.1b2/notolog/lexemes/la/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/la/color_picker_dialog.py` & `notolog-0.9.1b2/notolog/lexemes/la/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/la/common.py` & `notolog-0.9.1b2/notolog/lexemes/la/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     "save_active_file_error_occurred": "Fasciculum servare non potest, error accidit",
 
     "expandable_block_default_title": "Amplius info...",
 
     "dialog_color_picker_color_copied_to_the_clipboard": "Textus formatus in tabulam appensionis est copiatus",
 
     "popup_about_title": "De Applicatione",
-    "popup_about_app_name_description": "Editor Markdown",
+    "popup_about_app_name_description": "Editor Markdown Pythonis",
 
     "popup_about_version": "Versio",
     "popup_about_license": "Licentia",
     "popup_about_website": "Situs",
     "popup_about_repository": "GitHub",
     "popup_about_pypi": "PyPi",
     "popup_about_date": "Dies",
```

### Comparing `notolog-0.9.1b1/app/lexemes/la/main_menu.py` & `notolog-0.9.1b2/notolog/lexemes/la/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/la/settings_dialog.py` & `notolog-0.9.1b2/notolog/lexemes/la/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/la/statusbar.py` & `notolog-0.9.1b2/notolog/lexemes/ru/statusbar.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-# Latin lexemes statusbar.py
+# Russian lexemes statusbar.py
 lexemes = {
-    "statusbar_litter_bin_label": "Fiscina",
-    "statusbar_litter_bin_accessible_name": "Ostendere contentum fiscinae",
+    "statusbar_litter_bin_label": "Корзина",
+    "statusbar_litter_bin_accessible_name": "Показать содержимое корзины",
 
     "statusbar_save_progress_label": b'\xf0\x9f\x92\xbe',
     "statusbar_encryption_symbol_encrypted_label": b'\xf0\x9f\x94\x92',
     "statusbar_encryption_symbol_unencrypted_label": b'\xf0\x9f\x94\x93',
 
-    "statusbar_mode_label_mode_view": "Modus Visum",
-    "statusbar_mode_label_mode_edit": "Modus Editio",
-    "statusbar_mode_label_mode_source": "Modus Fons",
+    "statusbar_mode_label_mode_view": "Режим просмотра",
+    "statusbar_mode_label_mode_edit": "Режим редактирования",
+    "statusbar_mode_label_mode_source": "Режим источника",
 
     "statusbar_source_label_source_markdown": "Markdown",
     "statusbar_source_label_source_html": "HTML",
 
     "statusbar_encryption_label": "{encryption} {icon}",
-    "statusbar_encryption_label_encryption_plain": "Simplicitas",
-    "statusbar_encryption_label_encryption_encrypted": "Cryptatus",
+    "statusbar_encryption_label_encryption_plain": "Обычный",
+    "statusbar_encryption_label_encryption_encrypted": "Зашифрованный",
 
-    "statusbar_cursor_label": "linea: {line} → columna: {column}",
-    "statusbar_cursor_label_selected": "linea: {line} → columna: {column} → selectus: {selected}",
-    "statusbar_cursor_label_with_global": "linea: {line} → columna: {column} → positio: {position}",
+    "statusbar_cursor_label": "строка: {line} → столбец: {column}",
+    "statusbar_cursor_label_selected": "строка: {line} → столбец: {column} → выбр: {selected}",
+    "statusbar_cursor_label_with_global": "строка: {line} → столбец: {column} → поз: {position}",
     "statusbar_cursor_label_selected_with_global":
-        "linea: {line} → columna: {column} → positio: {position} → selectus: {selected}",
+        "строка: {line} → столбец: {column} → поз: {position} → выбр: {selected}",
 }
```

### Comparing `notolog-0.9.1b1/app/lexemes/la/toolbar.py` & `notolog-0.9.1b2/notolog/lexemes/la/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/lexemes.py` & `notolog-0.9.1b2/notolog/lexemes/lexemes.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/nl/ai_assistant.py` & `notolog-0.9.1b2/notolog/lexemes/nl/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/nl/color_picker_dialog.py` & `notolog-0.9.1b2/notolog/lexemes/nl/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/nl/common.py` & `notolog-0.9.1b2/notolog/lexemes/nl/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     "save_active_file_error_occurred": "Kan bestand niet opslaan, er is een fout opgetreden",
 
     "expandable_block_default_title": "Meer info...",
 
     "dialog_color_picker_color_copied_to_the_clipboard": "Geformatteerde tekst is naar het klembord gekopieerd",
 
     "popup_about_title": "Applicatie-info",
-    "popup_about_app_name_description": "Markdown Editor",
+    "popup_about_app_name_description": "Python Markdown Editor",
 
     "popup_about_version": "Versie",
     "popup_about_license": "Licentie",
     "popup_about_website": "Website",
     "popup_about_repository": "GitHub",
     "popup_about_pypi": "PyPi",
     "popup_about_date": "Datum",
```

### Comparing `notolog-0.9.1b1/app/lexemes/nl/main_menu.py` & `notolog-0.9.1b2/notolog/lexemes/nl/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/nl/settings_dialog.py` & `notolog-0.9.1b2/notolog/lexemes/nl/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/nl/statusbar.py` & `notolog-0.9.1b2/notolog/lexemes/nl/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/nl/toolbar.py` & `notolog-0.9.1b2/notolog/lexemes/nl/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/pt/ai_assistant.py` & `notolog-0.9.1b2/notolog/lexemes/pt/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/pt/color_picker_dialog.py` & `notolog-0.9.1b2/notolog/lexemes/pt/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/pt/common.py` & `notolog-0.9.1b2/notolog/lexemes/pt/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     "save_active_file_error_occurred": "Não foi possível salvar o arquivo, ocorreu um erro",
 
     "expandable_block_default_title": "Mais informações...",
 
     "dialog_color_picker_color_copied_to_the_clipboard": "O texto formatado foi copiado para a área de transferência",
 
     "popup_about_title": "Informações do Aplicativo",
-    "popup_about_app_name_description": "Editor Markdown",
+    "popup_about_app_name_description": "Editor de Markdown Python",
 
     "popup_about_version": "Versão",
     "popup_about_license": "Licença",
     "popup_about_website": "Site",
     "popup_about_repository": "GitHub",
     "popup_about_pypi": "PyPi",
     "popup_about_date": "Data",
```

### Comparing `notolog-0.9.1b1/app/lexemes/pt/main_menu.py` & `notolog-0.9.1b2/notolog/lexemes/tr/main_menu.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-# Portuguese lexemes main_menu.py
+# Turkish lexemes main_menu.py
 lexemes = {
-    "group_file_label": "Arquivo",
-    "group_edit_label": "Editar",
-    "group_tools_label": "Ferramentas",
-    "group_help_label": "Ajuda",
+    "group_file_label": "Dosya",
+    "group_edit_label": "Düzenle",
+    "group_tools_label": "Araçlar",
+    "group_help_label": "Yardım",
 
-    "actions_file_label_new_document": "Novo documento",
-    "actions_file_accessible_name_new_document": "Novo documento",
-    "actions_file_label_open": "Abrir",
-    "actions_file_accessible_name_open": "Abrir documento",
-    "actions_file_label_save": "Salvar",
-    "actions_file_accessible_name_save": "Salvar documento",
-    "actions_file_label_save_as": "Salvar como",
-    "actions_file_accessible_name_save_as": "Salvar como cópia do documento",
-    "actions_file_label_exit": "Sair do aplicativo",
-    "actions_file_accessible_name_exit": "Sair do aplicativo",
+    "actions_file_label_new_document": "Yeni belge",
+    "actions_file_accessible_name_new_document": "Yeni belge",
+    "actions_file_label_open": "Aç",
+    "actions_file_accessible_name_open": "Belgeyi aç",
+    "actions_file_label_save": "Kaydet",
+    "actions_file_accessible_name_save": "Belgeyi kaydet",
+    "actions_file_label_save_as": "Farklı Kaydet",
+    "actions_file_accessible_name_save_as": "Belgeyi kopya olarak kaydet",
+    "actions_file_label_exit": "Çıkış",
+    "actions_file_accessible_name_exit": "Uygulamadan çık",
 
-    "edit_actions_edit_mode": "Editar",
-    "edit_actions_accessible_name_edit_mode": "Editar arquivo",
-    "edit_actions_source_mode": "Fonte",
-    "edit_actions_accessible_name_source_mode": "Código-fonte",
-    "edit_actions_bold": "Negrito",
-    "edit_actions_accessible_name_bold": "Formato de texto em negrito",
-    "edit_actions_italic": "Itálico",
-    "edit_actions_accessible_name_italic": "Formato de texto em itálico",
-    "edit_actions_underline": "Sublinhado",
-    "edit_actions_accessible_name_underline": "Formato de texto sublinhado",
-    "edit_actions_strikethrough": "Riscado",
-    "edit_actions_accessible_name_strikethrough": "Formato de texto riscado",
-    "edit_actions_blockquote": "Citação",
-    "edit_actions_accessible_name_blockquote": "Formato de texto de citação",
+    "edit_actions_edit_mode": "Düzenle",
+    "edit_actions_accessible_name_edit_mode": "Dosyayı düzenle",
+    "edit_actions_source_mode": "Kaynak",
+    "edit_actions_accessible_name_source_mode": "Kaynak kodu",
+    "edit_actions_bold": "Kalın",
+    "edit_actions_accessible_name_bold": "Kalın metin biçimi",
+    "edit_actions_italic": "İtalik",
+    "edit_actions_accessible_name_italic": "İtalik metin biçimi",
+    "edit_actions_underline": "Altı çizili",
+    "edit_actions_accessible_name_underline": "Altı çizili metin biçimi",
+    "edit_actions_strikethrough": "Üstü çizili",
+    "edit_actions_accessible_name_strikethrough": "Üstü çizili metin biçimi",
+    "edit_actions_blockquote": "Alıntı",
+    "edit_actions_accessible_name_blockquote": "Alıntı metin biçimi",
 
-    "tools_actions_ai_assistant": "Assistente de IA",
-    "tools_actions_accessible_name_ai_assistant": "Lançar Assistente de IA",
-    "tools_actions_color_picker": "Seletor de Cor",
-    "tools_actions_accessible_name_color_picker": "Escolher uma cor para o texto",
+    "tools_actions_ai_assistant": "AI Asistanı",
+    "tools_actions_accessible_name_ai_assistant": "AI Asistanını Başlat",
+    "tools_actions_color_picker": "Renk Seçici",
+    "tools_actions_accessible_name_color_picker": "Metin rengi seç",
 
-    "actions_help_label_md_syntax": "Sintaxe Markdown",
-    "actions_help_accessible_name_md_syntax": "Sintaxe Markdown",
-    "actions_help_label_check_for_updates": "Verificar atualizações",
-    "actions_help_accessible_name_check_for_updates": "Verificar atualizações",
-    "actions_help_label_bug_report": "Relatar bug",
-    "actions_help_accessible_name_bug_report": "Enviar relatório de bug",
-    "actions_help_label_about": "Sobre",
-    "actions_help_accessible_name_about": "Sobre",
+    "actions_help_label_md_syntax": "Markdown Sözdizimi",
+    "actions_help_accessible_name_md_syntax": "Markdown Sözdizimi",
+    "actions_help_label_check_for_updates": "Güncellemeleri Denetle",
+    "actions_help_accessible_name_check_for_updates": "Güncellemeleri denetle",
+    "actions_help_label_bug_report": "Hata Raporu",
+    "actions_help_accessible_name_bug_report": "Hata raporu gönder",
+    "actions_help_label_about": "Hakkında",
+    "actions_help_accessible_name_about": "Hakkında",
 }
```

### Comparing `notolog-0.9.1b1/app/lexemes/pt/settings_dialog.py` & `notolog-0.9.1b2/notolog/lexemes/pt/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/pt/statusbar.py` & `notolog-0.9.1b2/notolog/lexemes/pt/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/pt/toolbar.py` & `notolog-0.9.1b2/notolog/lexemes/pt/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/ru/ai_assistant.py` & `notolog-0.9.1b2/notolog/lexemes/ru/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/ru/color_picker_dialog.py` & `notolog-0.9.1b2/notolog/lexemes/ru/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/ru/common.py` & `notolog-0.9.1b2/notolog/lexemes/ru/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     "save_active_file_error_occurred": "Невозможно сохранить файл, произошла ошибка",
 
     "expandable_block_default_title": "Больше информации...",
 
     "dialog_color_picker_color_copied_to_the_clipboard": "Форматированный текст был скопирован в буфер обмена",
 
     "popup_about_title": "Информация о приложении",
-    "popup_about_app_name_description": "Редактор Markdown",
+    "popup_about_app_name_description": "Python Markdown Редактор",
 
     "popup_about_version": "Версия",
     "popup_about_license": "Лицензия",
     "popup_about_website": "Веб-сайт",
     "popup_about_repository": "GitHub",
     "popup_about_pypi": "PyPi",
     "popup_about_date": "Дата",
```

### Comparing `notolog-0.9.1b1/app/lexemes/ru/main_menu.py` & `notolog-0.9.1b2/notolog/lexemes/ru/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/ru/settings_dialog.py` & `notolog-0.9.1b2/notolog/lexemes/ru/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/ru/toolbar.py` & `notolog-0.9.1b2/notolog/lexemes/ru/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/se/ai_assistant.py` & `notolog-0.9.1b2/notolog/lexemes/se/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/se/color_picker_dialog.py` & `notolog-0.9.1b2/notolog/lexemes/se/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/se/common.py` & `notolog-0.9.1b2/notolog/lexemes/se/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     "save_active_file_error_occurred": "Kan inte spara filen, ett fel inträffade",
 
     "expandable_block_default_title": "Mer information...",
 
     "dialog_color_picker_color_copied_to_the_clipboard": "Formaterad text har kopierats till urklipp",
 
     "popup_about_title": "Om programmet",
-    "popup_about_app_name_description": "Markdown-redigerare",
+    "popup_about_app_name_description": "Python Markdown-redigerare",
 
     "popup_about_version": "Version",
     "popup_about_license": "Licens",
     "popup_about_website": "Webbplats",
     "popup_about_repository": "GitHub",
     "popup_about_pypi": "PyPi",
     "popup_about_date": "Datum",
```

### Comparing `notolog-0.9.1b1/app/lexemes/se/main_menu.py` & `notolog-0.9.1b2/notolog/lexemes/zh/main_menu.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-# Swedish lexemes main_menu.py
+# Chinese lexemes main_menu.py
 lexemes = {
-    "group_file_label": "Fil",
-    "group_edit_label": "Redigera",
-    "group_tools_label": "Verktyg",
-    "group_help_label": "Hjälp",
+    "group_file_label": "文件",
+    "group_edit_label": "编辑",
+    "group_tools_label": "工具",
+    "group_help_label": "帮助",
 
-    "actions_file_label_new_document": "Nytt dokument",
-    "actions_file_accessible_name_new_document": "Nytt dokument",
-    "actions_file_label_open": "Öppna",
-    "actions_file_accessible_name_open": "Öppna dokument",
-    "actions_file_label_save": "Spara",
-    "actions_file_accessible_name_save": "Spara dokument",
-    "actions_file_label_save_as": "Spara som",
-    "actions_file_accessible_name_save_as": "Spara dokumentkopior",
-    "actions_file_label_exit": "Avsluta",
-    "actions_file_accessible_name_exit": "Avsluta programmet",
+    "actions_file_label_new_document": "新建文档",
+    "actions_file_accessible_name_new_document": "新文档",
+    "actions_file_label_open": "打开",
+    "actions_file_accessible_name_open": "打开文档",
+    "actions_file_label_save": "保存",
+    "actions_file_accessible_name_save": "保存文件",
+    "actions_file_label_save_as": "另存为",
+    "actions_file_accessible_name_save_as": "另存文档副本",
+    "actions_file_label_exit": "退出",
+    "actions_file_accessible_name_exit": "退出应用程序",
 
-    "edit_actions_edit_mode": "Redigera",
-    "edit_actions_accessible_name_edit_mode": "Redigera fil",
-    "edit_actions_source_mode": "Källkod",
-    "edit_actions_accessible_name_source_mode": "Källkod",
-    "edit_actions_bold": "Fet",
-    "edit_actions_accessible_name_bold": "Fet textformat",
-    "edit_actions_italic": "Kursiv",
-    "edit_actions_accessible_name_italic": "Kursiv textformat",
-    "edit_actions_underline": "Understrykning",
-    "edit_actions_accessible_name_underline": "Understruken textformat",
-    "edit_actions_strikethrough": "Genomstrykning",
-    "edit_actions_accessible_name_strikethrough": "Genomstruken textformat",
-    "edit_actions_blockquote": "Blockcitat",
-    "edit_actions_accessible_name_blockquote": "Blockcitat textformat",
+    "edit_actions_edit_mode": "编辑",
+    "edit_actions_accessible_name_edit_mode": "编辑文件",
+    "edit_actions_source_mode": "源码",
+    "edit_actions_accessible_name_source_mode": "源代码",
+    "edit_actions_bold": "加粗",
+    "edit_actions_accessible_name_bold": "加粗文字格式",
+    "edit_actions_italic": "斜体",
+    "edit_actions_accessible_name_italic": "斜体文字格式",
+    "edit_actions_underline": "下划线",
+    "edit_actions_accessible_name_underline": "下划线文字格式",
+    "edit_actions_strikethrough": "删除线",
+    "edit_actions_accessible_name_strikethrough": "删除线文字格式",
+    "edit_actions_blockquote": "引用",
+    "edit_actions_accessible_name_blockquote": "引用文字格式",
 
-    "tools_actions_ai_assistant": "AI-assistent",
-    "tools_actions_accessible_name_ai_assistant": "Starta AI-assistent",
-    "tools_actions_color_picker": "Färgväljare",
-    "tools_actions_accessible_name_color_picker": "Välj textfärg",
+    "tools_actions_ai_assistant": "AI 助手",
+    "tools_actions_accessible_name_ai_assistant": "启动 AI 助手",
+    "tools_actions_color_picker": "颜色选择器",
+    "tools_actions_accessible_name_color_picker": "选择文字颜色",
 
-    "actions_help_label_md_syntax": "Markdown-syntax",
-    "actions_help_accessible_name_md_syntax": "Markdown-syntax",
-    "actions_help_label_check_for_updates": "Sök efter uppdateringar",
-    "actions_help_accessible_name_check_for_updates": "Sök efter uppdateringar",
-    "actions_help_label_bug_report": "Felrapport",
-    "actions_help_accessible_name_bug_report": "Skicka felrapport",
-    "actions_help_label_about": "Om",
-    "actions_help_accessible_name_about": "Om"
+    "actions_help_label_md_syntax": "Markdown 语法",
+    "actions_help_accessible_name_md_syntax": "Markdown 语法",
+    "actions_help_label_check_for_updates": "检查更新",
+    "actions_help_accessible_name_check_for_updates": "检查更新",
+    "actions_help_label_bug_report": "错误报告",
+    "actions_help_accessible_name_bug_report": "提交错误报告",
+    "actions_help_label_about": "关于",
+    "actions_help_accessible_name_about": "关于",
 }
```

### Comparing `notolog-0.9.1b1/app/lexemes/se/settings_dialog.py` & `notolog-0.9.1b2/notolog/lexemes/se/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/se/statusbar.py` & `notolog-0.9.1b2/notolog/lexemes/se/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/se/toolbar.py` & `notolog-0.9.1b2/notolog/lexemes/se/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/tr/ai_assistant.py` & `notolog-0.9.1b2/notolog/lexemes/tr/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/tr/color_picker_dialog.py` & `notolog-0.9.1b2/notolog/lexemes/tr/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/tr/common.py` & `notolog-0.9.1b2/notolog/lexemes/tr/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     "save_active_file_error_occurred": "Dosya kaydedilemedi, hata oluştu",
 
     "expandable_block_default_title": "Daha fazla bilgi...",
 
     "dialog_color_picker_color_copied_to_the_clipboard": "Biçimlendirilmiş metin panoya kopyalandı",
 
     "popup_about_title": "Uygulama Bilgisi",
-    "popup_about_app_name_description": "Markdown Editörü",
+    "popup_about_app_name_description": "Python Markdown Editörü",
 
     "popup_about_version": "Versiyon",
     "popup_about_license": "Lisans",
     "popup_about_website": "Web Sitesi",
     "popup_about_repository": "GitHub",
     "popup_about_pypi": "PyPi",
     "popup_about_date": "Tarih",
```

### Comparing `notolog-0.9.1b1/app/lexemes/tr/settings_dialog.py` & `notolog-0.9.1b2/notolog/lexemes/tr/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/tr/statusbar.py` & `notolog-0.9.1b2/notolog/lexemes/tr/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/tr/toolbar.py` & `notolog-0.9.1b2/notolog/lexemes/tr/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/zh/ai_assistant.py` & `notolog-0.9.1b2/notolog/lexemes/zh/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/zh/color_picker_dialog.py` & `notolog-0.9.1b2/notolog/lexemes/zh/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/zh/common.py` & `notolog-0.9.1b2/notolog/lexemes/zh/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     "save_active_file_error_occurred": "无法保存文件，发生错误",
 
     "expandable_block_default_title": "更多信息...",
 
     "dialog_color_picker_color_copied_to_the_clipboard": "格式化文本已复制到剪贴板",
 
     "popup_about_title": "应用信息",
-    "popup_about_app_name_description": "Markdown 编辑器",
+    "popup_about_app_name_description": "Python Markdown 编辑器",
 
     "popup_about_version": "版本",
     "popup_about_license": "许可证",
     "popup_about_website": "网站",
     "popup_about_repository": "GitHub",
     "popup_about_pypi": "PyPi",
     "popup_about_date": "日期",
```

### Comparing `notolog-0.9.1b1/app/lexemes/zh/settings_dialog.py` & `notolog-0.9.1b2/notolog/lexemes/zh/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/lexemes/zh/toolbar.py` & `notolog-0.9.1b2/notolog/lexemes/zh/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/notolog_editor.py` & `notolog-0.9.1b2/notolog/notolog_editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -353,15 +353,15 @@
         if 'show_line_numbers' in data and hasattr(self, 'line_numbers'):
             # Show / hide line numbers area
             self.line_numbers.update_numbers()
 
         if 'app_font_size' in data and hasattr(self, 'theme_helper'):
             # Set up global font params
             self.init_font()
-            # Set up font to the view's document
+            # View document
             view_doc = self.get_view_doc()  # type: QTextDocument
             # Apply font from the main window to the widget
             view_doc.setDefaultFont(self.font())
             """
             # Or via view widget, also works
             view_widget = self.get_view_widget()  # type: Union[ViewWidget, QTextBrowser]
             view_widget.document().setDefaultFont(self.font())
@@ -979,14 +979,22 @@
         root_index = self.file_model.index(dir_path)
         """
         More info about this mapping https://doc.qt.io/qt-6/qsortfilterproxymodel.html#mapFromSource
         """
         proxy_index = self.tree_proxy_model.mapFromSource(root_index)
         self.tree_view.setRootIndex(proxy_index)
 
+        # View document
+        view_doc = self.get_view_doc()  # type: QTextDocument
+        # Set up document's base resource path
+        """
+        If a resource file not found QTextBrowser will try to search either this script or package root path (IDE run).
+        """
+        view_doc.setBaseUrl(QUrl.fromLocalFile(dir_path + '/'))
+
     def get_current_file_path(self, is_base: bool = False) -> str:
         """
         Get current file path.
         """
         return os.path.dirname(self.file_path) if is_base else self.file_path
 
     def get_active_dir(self):
@@ -1542,15 +1550,15 @@
                                         # Restore cursor and asure text widget has a focus
                                         (self.restore_doc_cursor_pos(self.get_mode(), edit_widget),
                                          edit_widget.setFocus()))
         if self.debug:
             self.logger.debug('Edit widget geometry %d x %d' %
                               (edit_widget.frameGeometry().width(), edit_widget.frameGeometry().height()))
 
-        # Could be synced with self.debug constant
+        # Set up markdown highlighter
         self.md_highlighter = MdHighlighter(document=edit_widget.document())
 
         # Restore widget's signals
         edit_widget.blockSignals(was_blocked)
         if self.debug:
             self.logger.debug(f'View widget created, signals was un-blocked "{was_blocked}"')
 
@@ -1562,30 +1570,63 @@
     def create_line_numbers(self, widget: Union[EditWidget, QPlainTextEdit]) -> None:
         """
         Init with a text edit.
         """
         self.line_numbers = LineNumbers(editor=widget)
 
     def open_link_dialog_proxy(self):
+        # Open confirmation set for external link
         if self.settings.viewer_open_link_confirmation:
             # Open a link after confirmation dialog only
             return lambda url: (
-                # Check if the clicked anchor is an internal doc link starts with '#'
-                self.get_view_widget().setSource(url) if url.toString().startswith('#') else self.common_dialog(
+                # Check if the clicked anchor is a local link
+                self.check_local_link(url, True) if self.check_local_link(url) else self.common_dialog(
                     self.lexemes.get('dialog_open_link_title'),
                     self.lexemes.get(name='dialog_open_link_text',
                                      url=url.toString()),
                     # Open url with system browser
                     callback=lambda dialog_callback:
                     # Open link in a system browser and run dialog's callback
                     (QDesktopServices.openUrl(url), dialog_callback())))
         # Just open a link without a confirmation dialog
-        return lambda url:(
-            # Check if the clicked anchor is an internal doc link starts with '#'
-            self.get_view_widget().setSource(url) if url.toString().startswith('#') else QDesktopServices.openUrl(url))
+        return lambda url: self.check_local_link(url, True)
+
+    def check_local_link(self, url: QUrl, execute: bool = False) -> Any:
+        # Anchor
+        if url.toString().startswith('#'):
+            # Anchor is an internal doc link starts with '#'
+            if execute:
+                self.get_view_widget().setSource(url)
+            return True
+
+        # Try external link
+        if not (url.isRelative() or url.isLocalFile()):
+            # Open in a system browser
+            if execute:
+                QDesktopServices.openUrl(url)
+            return False
+
+        # Try to find local file
+        try:
+            is_file = os.path.isfile(url.toString())
+        except PermissionError:
+            if self.logging:
+                self.logger.warning(f"Permission denied when accessing the file: {url.toString()}")
+            is_file = False
+        except OSError as e:
+            if self.logging:
+                self.logger.warning(f"Error when checking the file: {e}")
+            is_file = False
+        if is_file:
+            # Load local file
+            if execute:
+                self.load_file(url.toString())
+            return True
+
+        return None
 
     def get_view_doc(self) -> QTextDocument:
         if not hasattr(self, 'view_doc') or not self.view_doc:
             self.view_doc = QTextDocument(self)
             # Apply font from the main window to the widget
             self.view_doc.setDefaultFont(self.font())
             # Set default styles
@@ -2144,15 +2185,16 @@
              'action': self.action_save_file, 'var_name': 'toolbar_save_button', 'switched_off_check': lambda: True},
             {'type': 'delimiter'},
             {'type': 'action', 'weight': 4, 'name': 'toolbar_actions_label_edit',
              'system_icon': 'accessories-text-editor', 'theme_icon': 'pencil-square.svg',
              'color': self.theme_helper.get_color('toolbar_icon_color_edit'),
              'label': self.lexemes.get('actions_label_edit', scope='toolbar'),
              'accessible_name': self.lexemes.get('actions_accessible_name_edit', scope='toolbar'),
-             'action': self.action_edit_file, 'active_state_check': lambda: self.get_mode() != Mode.EDIT},
+             'action': self.action_edit_file, 'var_name': 'toolbar_edit_button',
+             'active_state_check': lambda: self.get_mode() != Mode.EDIT},
             # Active Edit Mode icon
             {'type': 'action', 'weight': 4, 'name': 'toolbar_actions_label_edit_act',
              'system_icon': 'accessories-text-editor', 'theme_icon': 'pencil-square.svg',
              'color': self.theme_helper.get_color('toolbar_icon_color_edit_act'),
              'label': self.lexemes.get('actions_label_edit', scope='toolbar'),
              'accessible_name': self.lexemes.get('actions_accessible_name_edit', scope='toolbar'),
              'action': self.action_edit_file, 'active_state_check': lambda: self.get_mode() == Mode.EDIT},
@@ -2995,14 +3037,17 @@
         self.setCursor(Qt.CursorShape.ArrowCursor)
 
     def load_file(self, file_path: str) -> bool:
         """
         Helper: Load content of the file.
         """
 
+        if not os.path.isabs(file_path):
+            file_path = os.path.abspath(file_path)  # Make sure it's an absolute path
+
         # Current file path and a new one can be the same but the MODE can differ
         current_file_path = self.get_current_file_path()
         # Update the tree and related indexes
         self.set_current_path(file_path)
 
         if current_file_path is not None and file_path != current_file_path:
             # Highlight the file to switch from
@@ -3252,14 +3297,19 @@
         # The dialog about empty content was shown at least once
         if allow_save_empty_content is not None:
             self.estate.allow_save_empty = allow_save_empty_content
 
         if self.debug:
             self.logger.debug(f"Save active file '{current_file_path}' (clear field after: '{clear_after}')")
 
+        if not os.path.exists(current_file_path):
+            if self.logging:
+                self.logger.warning(f"Cannot save active file '{current_file_path}', check if it was moved or deleted")
+            return
+
         with open(current_file_path, 'r', encoding='utf-8') as file:
             # Edit widget
             edit_widget = self.get_edit_widget()  # type: Union[EditWidget, QPlainTextEdit]
             file_content = edit_widget.toPlainText()
 
             # If new content is empty ask confirmation to be sure
             if (not file_content
@@ -3480,17 +3530,17 @@
         There is also possible to update QTextEdit with html:
         view_widget.setHtml(self.HTML_TPL % (title, css_data, view_doc.toPlainText()))
         Or update and set up document itself:
         view_widget.setDocument(updated_doc)
         """
         view_doc.setHtml(self.HTML_TPL % (title, css_data, view_doc.toPlainText()))
 
-        # TODO do not process twice
-        # Extract string image resources from the document, download and append
+        # Extract string image resources from the document, download and append.
         self.process_document_images(view_doc)
+
         """
         # Load resource from the document
         res = view_doc.loadResource(QTextDocument.ResourceType.ImageResource, image_url)
         """
 
         """
         View decorator to modify result text.
@@ -3549,16 +3599,17 @@
         elif os.path.exists(file_path):
             # Load from disk and cache
             pixmap.load(file_path)
             QPixmapCache.insert(image_url, pixmap)
             if self.debug:
                 self.logger.debug(f"Loaded from disk and cached: {image_url}")
         else:
-            if self.logging:
-                self.logger.warning(f"Resource's '{image_url}' file doesn't exist '{file_path}'")
+            if (self.resource_downloader.is_external_url(image_url)
+                    and self.debug):
+                self.logger.debug(f"Resource's '{image_url}' file doesn't exist '{file_path}' yet")
         return pixmap
 
     @Slot()
     def resource_downloaded_handler(self, data) -> None:
         if 'resource_name' not in data:
             if self.logging:
                 self.logger.warning(f'Wrong data for added resource: {data}')
@@ -3570,21 +3621,23 @@
             # Attach resource
             self.attach_resource(image_url, pixmap)
         else:
             if self.logging:
                 self.logger.warning(f"Resource '{image_url}' data not found")
 
     @Slot()
-    def resource_downloader_finished_handler(self):
+    def resource_downloader_finished_handler(self, downloaded_cnt):
         if self.debug:
-            self.logger.debug(f"All resource downloader tasks have been completed")
-        # View widget
-        view_widget = self.get_view_widget()  # type: Union[ViewWidget, QTextBrowser]
-        # Re-set up view's (or document's) content to get the added resources shown
-        view_widget.setHtml(view_widget.toHtml())
+            self.logger.debug(f"All resource downloader tasks ({downloaded_cnt}) have been completed")
+        # Run update only if anything was downloaded
+        if downloaded_cnt > 0:
+            # View widget
+            view_widget = self.get_view_widget()  # type: Union[ViewWidget, QTextBrowser]
+            # Re-set up view's (or document's) content to get the added resources shown
+            view_widget.setHtml(view_widget.toHtml())
 
     def process_document_images(self, text_document):
         """
         Extract image urls from the given document
         """
 
         # Init image downloader instance
@@ -3608,15 +3661,17 @@
                             self.logger.debug(f"Found image resource url: {image_url}")
                         # Check if the resource has been already added
                         if not self.is_resource_attached(image_url):
                             # Try to get cached resource data
                             pixmap = self.get_cached_resource_pixmap(image_url)
                             # Download if not found
                             if pixmap.isNull():
-                                self.resource_downloader.download_resource_in_queue(image_url)
+                                # Download external resources only
+                                if self.resource_downloader.is_external_url(image_url):
+                                    self.resource_downloader.download_resource_in_queue(image_url)
                             else:
                                 # Attach resource
                                 self.attach_resource(image_url, pixmap)
                         else:
                             if self.debug:
                                 self.logger.debug(f"Resource is already attached: {image_url}")
                 it += 1
```

### Comparing `notolog-0.9.1b1/app/settings.py` & `notolog-0.9.1b2/notolog/settings.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/text_block_data.py` & `notolog-0.9.1b2/notolog/text_block_data.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/theme.py` & `notolog-0.9.1b2/notolog/theme.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/ui/about_popup.py` & `notolog-0.9.1b2/notolog/ui/about_popup.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/ui/ai_assistant.py` & `notolog-0.9.1b2/notolog/ui/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/ui/color_picker_dialog.py` & `notolog-0.9.1b2/notolog/ui/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/ui/common_dialog.py` & `notolog-0.9.1b2/notolog/ui/common_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/ui/enum_combo_box.py` & `notolog-0.9.1b2/notolog/ui/enum_combo_box.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/ui/file_system_model.py` & `notolog-0.9.1b2/notolog/ui/file_system_model.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/ui/line_numbers.py` & `notolog-0.9.1b2/notolog/ui/line_numbers.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/ui/rename_file_dialog.py` & `notolog-0.9.1b2/notolog/ui/rename_file_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/ui/rotating_label.py` & `notolog-0.9.1b2/notolog/ui/rotating_label.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/ui/settings_dialog.py` & `notolog-0.9.1b2/notolog/ui/settings_dialog.py`

 * *Files 0% similar despite different names*

```diff
@@ -571,27 +571,27 @@
                     # self.findChildren() contains only the elements related to this dialog
                     found_objects = self.findChildren(QObject, regex, Qt.FindChildOption.FindChildrenRecursively)
                     if not found_objects:
                         # Try to find it in the parent dialog
                         found_objects = self.parent.findChildren(QObject, regex,
                                                                  Qt.FindChildOption.FindChildrenRecursively)
                         if self.debug and found_objects:
-                            self.logger.debug(f"Found object to update (?={scope}_)?{lexeme_key}.*?: {found_objects}")
+                            self.logger.debug(f"Found object to update ({scope}){lexeme_key}: {found_objects}")
 
                     # Search by full object name
                     # object_name = self.lexemes.get_full_key(lexeme_key)
                     # found_objects = self.findChildren(QObject, object_name, Qt.FindChildrenRecursively)
 
                     for obj in found_objects:
-                        if self.debug:
-                            self.logger.debug(
-                                f'Object for lexeme update: {obj.objectName()} with id: {id(obj)}, lexeme "{lexeme}"')
                         if ((isinstance(obj, (QLabel, QCheckBox, QComboBox, QPushButton)))
                                 and hasattr(obj, 'setText')
                                 and callable(getattr(obj, 'setText'))):
+                            if self.debug:
+                                self.logger.debug(
+                                    f'Object lexeme update: {obj.objectName()} with id: {id(obj)}, lexeme "{lexeme}"')
                             obj.setText(lexeme)
                         if isinstance(obj, QWidget):
                             # Add iterable map of the tabs to change the search by QWidget to explicitly set tab text.
                             self.set_tab_text(obj.objectName(), lexeme)
                         # Exclusions
                         if obj.objectName() == "settings_dialog_general_app_font_size_label":
                             obj.setText(
```

### Comparing `notolog-0.9.1b1/app/ui/sort_filter_proxy_model.py` & `notolog-0.9.1b2/notolog/ui/sort_filter_proxy_model.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/ui/statusbar.py` & `notolog-0.9.1b2/notolog/ui/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/ui/toolbar.py` & `notolog-0.9.1b2/notolog/ui/toolbar.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,17 @@
         self.search_match_case = None  # type: Union[QCheckBox, None]
         self.search_input = None  # type: Union[QLineEdit, None]
         self.btn_search_clear = None  # type: Union[QPushButton, None]
         self.btn_search_prev = None  # type: Union[QPushButton, None]
         self.btn_search_next = None  # type: Union[QPushButton, None]
         self.search_match_case = None  # type: Union[QCheckBox, None]
 
+        self.toolbar_save_button = None  # type: Union[QToolButton, None]
+        self.toolbar_edit_button = None  # type: Union[QToolButton, None]
+
         self.setMovable(False)
 
         self.init_ui()
 
     def init_ui(self):
         prev_type = None
         for icon in self.actions:
```

### Comparing `notolog-0.9.1b1/app/view_decorator.py` & `notolog-0.9.1b2/notolog/view_decorator.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/view_processor.py` & `notolog-0.9.1b2/notolog/view_processor.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/app/view_widget.py` & `notolog-0.9.1b2/notolog/view_widget.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/docs/Examples.md` & `notolog-0.9.1b2/docs/Examples.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!-- {"notolog.app": {"created": "2024-03-26 00:19:36.466439", "updated": "2024-05-06 21:22:54.003826"}} -->
+<!-- {"notolog.app": {"created": "2024-03-26 00:19:36.466439", "updated": "2024-05-11 12:23:43.657587"}} -->
 # Markdown syntax
 
 ## Headings
 
 Keep space between the `#` sign and the heading itself.
 
 # Header 1
@@ -10,22 +10,43 @@
 ### Header 3
 #### Header 4
 ##### Header 5
 ###### Header 6
 
 *No alternate syntax supported for the headings at the moment.*
 
+## Tables
+
+Markdown table syntax is supported, complete with column alignment options to enhance readability and presentation.
+
+A Markdown table is composed of rows of data, divided by pipes (`|`). The first row is typically the header, followed by a separator line, and then the data rows.
+
+| Item                  | In Stock | Price |
+| :-------------------- | :------: | ----: |
+| Unicorn Bubble Tea    | Yes      | 7.99  |
+| Dragon's Breath Chili | No       | 23.99 |
+| Fairy Dust Tiramisu   | Yes      | 17.99 |
+| Wizard's Cloak Hoodie | No       | 42.99 |
+
+### Alignment Operands
+
+To align the content within your table cells, you can use colons (`:`) in the separator line:
+
+* Left-aligned: Use `:--` or `:---` (colon on the left side)
+* Center-aligned: Use `:--:` or `:---:` (colons on both sides)
+* Right-aligned: Use `--:` or `---:` (colon on the right side)
+
 
 ## Images
 
 ### Image with path
 
-![Notolog](app/assets/notolog-example-image.png)
+![Notolog](../notolog/assets/notolog-example-image.png)
 
-Code looks like: `![Alt text](app/assets/notolog-example-image.png)`
+Code looks like: `![Alt text](notolog/assets/notolog-example-image.png)`.
 
 ### Image with base64 data
 
 ![Notolog inline logo](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAQAAADZc7J/AAABImlDQ1BJQ0MgcHJvZmlsZQAAKJGdkLFKw1AUhr/UokV0UhTEIYNrRwOCg1UhCBVirGB1SpMUi0kMSUrxDXwTfZgOguAzOCs4+9/o4GAWbzj8H4dz/v/eQMtOwrRsH0CaVYXr94aXwyt76Y02m/r26ARhmfc8r0/j+XzFMvrSNV7Nc3+exSguQ+lclYV5UYG1L3ZmVW5YxfrtwD8SP4jtKM0i8ZN4J0ojw2bXT5Np+ONpbrMSZxfnpq/axuWEUzxsRkyZkFDRlWbqHOOwK3UpCLinJJQmxOrNNFNxIyrl5HIoGoh0m4a8rTrPU8pIHhN5mYQ7UnmaPMz//V77OKs3rY15HhRB3VpQtcZjeH+E1SGsPcPydUNW5/fbGmaceuafb/wCNn9Qi6s+bdsAAAACYktHRADENoQlmwAABZlJREFUSMdtlWtsXMUVx38z9+57vY4fG+zFjhM7tkOc1ElKCXWbSrQQVBAIqrQqNEhAyBeKYrVFjdpIobRWPkSRSGhUakiLgqBVU7lIhJhSIZqKGEofOCWY2ImJ467ttZP1Y73Pu/femX7w2rHbzpHm05zfnPOfc+aIaQY44cnsCD3ka7PcbQNVp4LvbbBr+X/raVRj8rvyDq/h71v1/LqhxzSI07xdduFw9tEf+G/hJLXUF3yv8vTNqdv+x/0AFz439we7MSj8eAgkbtodfrcLw/YMPOfu3e7tU3GFrMVnZre4dcm32p3/BnR7rr10fbsSAgMTWeZ2BH9zV96ov2f0UEbn/ywHP3Y+DQ/gSq9UbXn3vXMdeiWgv7z/uaxPYOLHj5eZSOrcty+biUcdp+3XhUYrXn2xECmrPl//Uftm76r9U/966o3jKxDpYMbj4lBkliI+5qSKgml1tJ2MTsevZ3c3NHzdrCOvLxhvYARDx/PDTw78YhnAEg5gk8emiIc8NiAJbTySMe0DG1vqfTNG3mgxvy+6aWS4buiX0xV/WgZw0Gg0FgUKpMiRBczAxKQe2Sd9l6kgzRwXuYnbuZswf+kYPPT8vp32DQC4uEgkFgqFRmP64qtr3/FaCPxEaKKZecZoZR1Snt2T+vib3afUIsLFQSEQaECw3gTpfymzfoFWJM8wffRxjT6SFGj3THVN3X5fyV2hAI2Lu4ASlR6QFT2xflC4OGSYJckoPUyS4AOmWVeZ6LZiXQAUcbFxUSgUDpKIRyN7lN/VGGgciuSYYZoIm0nSygAu5W3jx6+GFkVciNVYiEZICXI/42Elokg0Di42RWZp4imSRPgbRTF//8CB3eaCBhqNnyCVGCjtapDj3rMHlS8G6CWhXA5jsYt2Khhk3hj+XvwbDwtRCr4Ol9WYgEQjCxsTXzMII5BQeul5ApwgSz3f4j7KSfmHj05thnJChKnCIYaBIYQ4iSxsap0wXYNmPl8CBHRjup8cf+cic6zlQXZCbfxluyYPbCHNLXgpUoMse/FhaeO5bqs8ecbQKMBbaP+hmfsrI8AME6SoYgvBrddeqPRsJI2gmX8SI6qzruoymjIVsc++IAwPcSLk0Yjil/a4Vu4rSTmGQDFNlixKzMUMaVLHKj5kjC1k1ezrvntl6Mqtv0JdZh7NDBpw9Oli+ZHK36HTnOd9LvEhCVzKqcHPRd5khPX4mHRq7XzBPEVntqg91DDJYs1O80DhTKfTcPXLmgIFYKSkuQYMmqhjjPAH/97me1tqXrOaMbibJ/Audd7jRKfX7qm+4kHgI0IQA4GBjxjt1DKJNRq9lNvZcFhYtMRahycDNj/hKt1cwZPx1sxk4R6srxZ72lf9kQQRgvgI4EVhk6I5V/gssX7D7prXJewJT4gGxvgxsI9deEsl1UvLWe/+aPEYe6kiwVUGucAnDDHOPwIjm9u9FeVJaWoMI06IJgb5EXUUsPGUEnlBPfByb+tY5+PGXoYYIU2Aenr5PYZoYVbKrTMBqbFxOM8cqwkzwTU0oNAoNL321mfef+sRfZQUrWynkcsUuJcYKQbR17lTagwEFqNMkENB6cNY6P08VZn6J92BV+jmI5IYbGIH46S5RBbTLEZMjXI1oFk5CHRpf5Zn4vYT1unz0U+pwUueOSwcNCEtNskkOTpiMlfqIo1Ge9MNoRzL7TGx45GywvIzaLRXbZv9Yqd02ZCrzi6/e421UyhumMvPdeVv1x4z3ZWDpijmc209EqYyVb1iaYQIIu9kC3ophYX0XnWaf9pwRq4YNP5i9KAal5o7nLpnqz9ZQEhiVxp+dqtzw3lxhbM1e9ee8TiL11Tmbuu6+ZWjWowC3yG0Jt6p7hL4z605VjZ0aElEEEuSHuFSYH7X3ENTjWE72l99oq7voAv/AaLcmaVSeOLtAAAAAElFTkSuQmCC)
 
 To get base64 image code from the real image use this example in Python (*Learn more about code blocks below*):
```

### Comparing `notolog-0.9.1b1/docs/notolog-ui-settings.png` & `notolog-0.9.1b2/docs/notolog-ui-settings.png`

 * *Files identical despite different names*

### Comparing `notolog-0.9.1b1/main.py` & `notolog-0.9.1b2/notolog/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,21 +24,25 @@
 # - Copyright 2024 Vadim Bakhrenkov
 # - License: MIT License
 
 
 from PySide6.QtWidgets import QStyleFactory
 from qasync import QEventLoop, QApplication
 
-from app.app_config import AppConfig
-from app.notolog_editor import NotologEditor
+# from notolog.app_config import AppConfig
+from notolog.notolog_editor import NotologEditor
 
 import platform
 import logging
 import asyncio
 import sys
+import os
+
+# Force Qt style override
+os.environ["QT_STYLE_OVERRIDE"] = "Fusion"
 
 
 def main():
     """
     Possible params:
     filename='notolog.log'
     format='%(asctime)s:%(levelname)s:%(name)s:%(message)s'
```

### Comparing `notolog-0.9.1b1/notolog.egg-info/PKG-INFO` & `notolog-0.9.1b2/notolog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: notolog
-Version: 0.9.1b1
-Summary: Notolog Markdown Editor
+Version: 0.9.1b2
+Summary: Notolog - Python Markdown Editor
 Home-page: https://github.com/notolog/notolog-editor
 Author: Vadim Bakhrenkov
 License: MIT
 Project-URL: Bug Reports, https://github.com/notolog/notolog-editor/issues
 Project-URL: Source, https://github.com/notolog/notolog-editor/
-Keywords: notolog,ai,markdown,editor
+Keywords: notolog,python,markdown,editor,ai,text
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
@@ -47,18 +47,18 @@
 Requires-Dist: PySide6_Essentials==6.7.0
 Requires-Dist: pytest==8.2.0
 Requires-Dist: pytest-mock==3.14.0
 Requires-Dist: qasync==0.27.1
 Requires-Dist: shiboken6==6.7.0
 Requires-Dist: tomli==2.0.1
 
-<!-- {"notolog.app": {"created": "2023-12-25 18:59:43.806614", "updated": "2024-05-06 21:20:54.001715"}} -->
+<!-- {"notolog.app": {"created": "2023-12-25 18:59:43.806614", "updated": "2024-05-11 11:15:29.656338"}} -->
 # Notolog
 
-![Notolog](https://raw.githubusercontent.com/notolog/notolog-editor/main/app/assets/notolog-example-image.png)&nbsp;&nbsp;&nbsp;![PyPI - Version](https://img.shields.io/pypi/v/notolog) ![PyPI - License](https://img.shields.io/pypi/l/notolog) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/notolog)
+![Notolog](https://raw.githubusercontent.com/notolog/notolog-editor/main/notolog/assets/notolog-example-image.png)&nbsp;&nbsp;&nbsp;![PyPI - Version](https://img.shields.io/pypi/v/notolog) ![PyPI - License](https://img.shields.io/pypi/l/notolog) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/notolog)
 
 ## Overview
 
 Notolog is a versatile open-source markdown editor developed with Python and Qt, ideal for anyone looking for an efficient and straightforward way to handle markdown files. Born from a personal endeavor to address daily programming challenges and deepen Python proficiency, Notolog stands as a proof-of-concept that seamlessly integrates simplicity with functionality, offering an intuitive user experience across various platforms.
 
 ---
 ![Notolog settings UI example](https://raw.githubusercontent.com/notolog/notolog-editor/main/docs/notolog-ui-settings.png)
@@ -77,20 +77,20 @@
 	* Font size adjustment for better readability.
 * Background and cross-action save changes experience:
 	* Automatically saves changes in the background to ensure data integrity and minimize user intervention.
 	* Seamlessly handles unsaved changes when performing cross-actions, providing a smooth user experience.
 * Search functionality:
 	* Allows users to search within the opened file.
 	* Quick search by file name within the tree, enabling efficient navigation and content retrieval.
-* File meta-headers in the form of HTML comments to avoid excess visibility.
 * Password-based File Encryption and Decryption:
 	* Utilizes Fernet for encryption, providing a secure and user-friendly method for symmetric (also known as "secret key") encryption.
 	* Fernet employs AES-128 in CBC mode. Plans to introduce AES-256 in future updates are aimed at further enhancing security.
 * File Meta-Headers:
-	* Notolog implements file meta-headers to store encryption parameters, ensuring a seamless decryption process.
+	* Notolog employs file meta-headers to store encryption/decryption parameters and other essential file information.
+	* To minimize visibility, these meta-headers are formatted as HTML comments.
 * Translations-friendly file structure:
 	* Supports several languages out of the box, with provisions for adding and supporting additional languages.
 * Color themes support:
 	* Comes with a few predefined color themes to customize the editor's appearance, for both light and dark modes.
 * Hotkeys support:
 	* It currently supports hotkeys like Ctrl+S for saving and Ctrl+F for searching, with plans for further expansion.
 * In-line context menus:
@@ -110,15 +110,15 @@
 
 If you haven't already, download and install Python from the official website [python.org](python.org).
 
 Check the version of Python available with this command `python3 -V`.
 
 **pip (Python package installer) should be available.**
 
-You can check if pip is installed by running `pip3 --version` in your terminal/command prompt.
+You can check if pip is installed by running `pip --version` in your terminal/command prompt.
 
 **Virtual Environment**
 
 It is highly recommended to use as it helps avoid version conflicts and interference from other packages. Below is a description of how to set up a virtual environment on your machine.
 
 
 ## Installation
@@ -142,18 +142,18 @@
 1. Clone project's GitHub repository to get a latest version.
 	* `git clone https://github.com/notolog/notolog-editor.git`
 2. Navigate to the just cloned project's directory using the **cd** command.
 3. Make sure the virtual environment is activated as it's a common practice to isolate project code (activation described below).
 4. Simply run this command to set up project dependencies:
 
 ```sh
-pip3 install -r requirements.txt
+pip install -r requirements.txt
 ```
 
-That's it! Starting the app is as simple as `python3 main.py`
+That's it! Starting the app is as simple as `python -m notolog.main` form the project's root directory.
 
 <details>
 <summary>Run tests</summary>
 
 To run all available tests:
 ```sh
 pytest
```

### Comparing `notolog-0.9.1b1/setup.py` & `notolog-0.9.1b2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 
 # Read the contents of README file
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='notolog',
-    version='0.9.1b1',
-    description='Notolog Markdown Editor',
+    version='0.9.1b2',
+    description='Notolog - Python Markdown Editor',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/notolog/notolog-editor',
     author='Vadim Bakhrenkov',
     license='MIT',
-    py_modules=['main'],
+    # py_modules=['main'],  # This refers to the standalone 'main.py' at the top-level directory
     entry_points={
         'console_scripts': [
-            'notolog=main:main',
+            # 'notolog=main:main',  # main.py at the top-level directory
+            'notolog=notolog.main:main',  # main.py within the main package
         ],
     },
     classifiers=[
         # More info https://pypi.org/classifiers/
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
@@ -48,9 +49,9 @@
     include_package_data=True,  # Include data files specified in MANIFEST.in
     python_requires='>=3.9, <4',
     install_requires=[line.strip() for line in open("requirements.txt", "r")],
     project_urls={
         'Bug Reports': 'https://github.com/notolog/notolog-editor/issues',
         'Source': 'https://github.com/notolog/notolog-editor/',
     },
-    keywords='notolog, ai, markdown, editor',
+    keywords='notolog, python, markdown, editor, ai, text',
 )
```

### Comparing `notolog-0.9.1b1/tests/test_enc_helper.py` & `notolog-0.9.1b2/tests/test_enc_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # tests/test_enc_helper.py
-from app.encrypt.enc_helper import EncHelper
-from app.encrypt.enc_password import EncPassword
+from notolog.encrypt.enc_helper import EncHelper
+from notolog.encrypt.enc_password import EncPassword
 
 from cryptography.fernet import Fernet
 
 from logging import Logger
 
 import pytest
```

### Comparing `notolog-0.9.1b1/tests/test_enc_password.py` & `notolog-0.9.1b2/tests/test_enc_password.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # tests/test_enc_password.py
-from app.encrypt.enc_password import EncPassword
+from notolog.encrypt.enc_password import EncPassword
 
 import pytest
 
 
 class TestEncPassword:
 
     @pytest.fixture(scope="function", autouse=True)
```

### Comparing `notolog-0.9.1b1/tests/test_file_header.py` & `notolog-0.9.1b2/tests/test_file_header.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # tests/test_file_header.py
 
-from app.file_header import FileHeader
+from notolog.file_header import FileHeader
 
-from app.exceptions.file_header_empty_exception import FileHeaderEmptyException
+from notolog.exceptions.file_header_empty_exception import FileHeaderEmptyException
 
 from logging import Logger
 
 import pytest
 
 
 class TestFileHeader:
```

### Comparing `notolog-0.9.1b1/tests/test_html_view.py` & `notolog-0.9.1b2/tests/test_html_view.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # tests/test_html_view.py
 from PySide6.QtGui import QTextDocument, QFont
 
-from app.highlight.view_highlighter import ViewHighlighter
-from app.view_processor import ViewProcessor
-from app.view_decorator import ViewDecorator
+from notolog.highlight.view_highlighter import ViewHighlighter
+from notolog.view_processor import ViewProcessor
+from notolog.view_decorator import ViewDecorator
 
 import pytest
 
 
 class TestHtmlView:
 
     @pytest.fixture(scope="function", autouse=True)
```

### Comparing `notolog-0.9.1b1/tests/test_lexemes.py` & `notolog-0.9.1b2/tests/test_lexemes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # tests/test_lexemes.py
 
-from app.lexemes.lexemes import Lexemes
+from notolog.lexemes.lexemes import Lexemes
 
 from logging import Logger
 
 import pytest
 import os
```

### Comparing `notolog-0.9.1b1/tests/test_notolog_editor.py` & `notolog-0.9.1b2/tests/test_notolog_editor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # tests/test_notolog_editor.py
 
-from app.notolog_editor import NotologEditor
-from app.settings import Settings
-from app.editor_state import Mode
-from app.lexemes.lexemes import Lexemes
+from notolog.notolog_editor import NotologEditor
+from notolog.settings import Settings
+from notolog.editor_state import Mode
+from notolog.lexemes.lexemes import Lexemes
 
 import pytest
 
 import os
 
 
 class TestNotologEditor:
```

### Comparing `notolog-0.9.1b1/tests/test_settings.py` & `notolog-0.9.1b2/tests/test_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # tests/test_settings.py
-from app.settings import Settings
+from notolog.settings import Settings
 
 import pytest
 
 class TestSettings():
 
     def test_settings_defaults(self):
         obj = Settings()
+        obj.clear()
         assert obj.ui_width == 0
         assert obj.ui_height == 0
         assert obj.ui_pos_x == 0
         assert obj.ui_pos_y == 0
         assert obj.file_path is ''
         assert obj.toolbar_icons is 0
```

### Comparing `notolog-0.9.1b1/tests/test_text_block_data.py` & `notolog-0.9.1b2/tests/test_text_block_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # tests/test_text_block_data.py
-from app.text_block_data import TextBlockData
+from notolog.text_block_data import TextBlockData
 
 import pytest
 
 
 class TestTextBlockData:
 
     @pytest.fixture(scope="class", autouse=True)
```

### Comparing `notolog-0.9.1b1/tests/test_theme_helper.py` & `notolog-0.9.1b2/tests/test_theme_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # tests/test_themes.py
 
-from app.helpers.theme_helper import ThemeHelper
-from app.enums.themes import Themes
-from app.theme import Theme
-from app.settings import Settings
-from app.app_config import AppConfig
+from notolog.helpers.theme_helper import ThemeHelper
+from notolog.enums.themes import Themes
+from notolog.theme import Theme
+from notolog.settings import Settings
+from notolog.app_config import AppConfig
 
 from logging import Logger
 
 import os
 import pytest
```

### Comparing `notolog-0.9.1b1/tests/test_themes.py` & `notolog-0.9.1b2/tests/test_themes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # tests/test_themes.py
 
-from app.theme import Theme
+from notolog.theme import Theme
 
 from logging import Logger
 
 import pytest
 import os
```

