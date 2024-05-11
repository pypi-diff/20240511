# Comparing `tmp/plom-0.9.3.tar.gz` & `tmp/plom-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plom-0.9.3.tar", last modified: Tue Jul 19 00:26:20 2022, max compression
+gzip compressed data, was "plom-0.9.4.tar", last modified: Fri Aug  5 05:51:22 2022, max compression
```

## Comparing `plom-0.9.3.tar` & `plom-0.9.4.tar`

### file list

```diff
@@ -1,346 +1,346 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 00:26:20.922581 plom-0.9.3/
--rw-rw-rw-   0 root         (0) root         (0)    32007 2022-07-19 00:26:14.000000 plom-0.9.3/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)     1021 2022-07-19 00:26:14.000000 plom-0.9.3/CONTRIBUTORS
--rw-rw-rw-   0 root         (0) root         (0)     1547 2022-07-19 00:26:14.000000 plom-0.9.3/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)    34283 2022-07-19 00:26:14.000000 plom-0.9.3/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)     1137 2022-07-19 00:26:14.000000 plom-0.9.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2366 2022-07-19 00:26:20.922581 plom-0.9.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1835 2022-07-19 00:26:14.000000 plom-0.9.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 00:26:20.825570 plom-0.9.3/contrib/
--rw-rw-rw-   0 root         (0) root         (0)      252 2022-07-19 00:26:14.000000 plom-0.9.3/contrib/README.txt
--rwxrwxrwx   0 root         (0) root         (0)    11813 2022-07-19 00:26:14.000000 plom-0.9.3/contrib/plom-push-to-canvas.py
--rwxrwxrwx   0 root         (0) root         (0)     2162 2022-07-19 00:26:14.000000 plom-0.9.3/contrib/plom-return_codes_to_canvas_csv.py
--rwxrwxrwx   0 root         (0) root         (0)     2138 2022-07-19 00:26:14.000000 plom-0.9.3/contrib/plom-write_grades_to_canvas_csv.py
--rwxrwxrwx   0 root         (0) root         (0)     7058 2022-07-19 00:26:14.000000 plom-0.9.3/contrib/upload_hw_from_zip_of_jpegs.py
--rw-rw-rw-   0 root         (0) root         (0)      583 2022-07-19 00:26:14.000000 plom-0.9.3/org.plomgrading.PlomClient.desktop
--rw-rw-rw-   0 root         (0) root         (0)     4895 2022-07-19 00:26:14.000000 plom-0.9.3/org.plomgrading.PlomClient.metainfo.xml
--rw-rw-rw-   0 root         (0) root         (0)     7237 2022-07-19 00:26:14.000000 plom-0.9.3/org.plomgrading.PlomClient.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 00:26:20.836571 plom-0.9.3/plom/
--rw-rw-rw-   0 root         (0) root         (0)     1379 2022-07-19 00:26:14.000000 plom-0.9.3/plom/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7404 2022-07-19 00:26:14.000000 plom-0.9.3/plom/aliceBob.py
--rw-rw-rw-   0 root         (0) root         (0)    39534 2022-07-19 00:26:14.000000 plom-0.9.3/plom/baseMessenger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 00:26:20.839572 plom-0.9.3/plom/canvas/
--rw-rw-rw-   0 root         (0) root         (0)      629 2022-07-19 00:26:14.000000 plom-0.9.3/plom/canvas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12833 2022-07-19 00:26:14.000000 plom-0.9.3/plom/canvas/canvas_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5856 2022-07-19 00:26:14.000000 plom-0.9.3/plom/canvas/canvasapi_extensions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 00:26:20.848573 plom-0.9.3/plom/client/
--rw-rw-rw-   0 root         (0) root         (0)      722 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5580 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)    75770 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/annotator.py
--rw-rw-rw-   0 root         (0) root         (0)      850 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/backGrid.py
--rw-rw-rw-   0 root         (0) root         (0)     3632 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/backGrid1.svg
--rw-rw-rw-   0 root         (0) root         (0)    46182 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/backGrid2.png
--rw-rw-rw-   0 root         (0) root         (0)     4282 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/background_downloader.py
--rw-rw-rw-   0 root         (0) root         (0)    19204 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/chooser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 00:26:20.853573 plom-0.9.3/plom/client/cursors/
--rw-rw-rw-   0 root         (0) root         (0)      236 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/cursors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1234 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/cursors/arrow.png
--rw-rw-rw-   0 root         (0) root         (0)     1177 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/cursors/box.png
--rw-rw-rw-   0 root         (0) root         (0)     1049 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/cursors/crop.png
--rw-rw-rw-   0 root         (0) root         (0)     1049 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/cursors/cross.png
--rw-rw-rw-   0 root         (0) root         (0)     1465 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/cursors/delete.png
--rw-rw-rw-   0 root         (0) root         (0)     1297 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/cursors/double_arrow.png
--rw-rw-rw-   0 root         (0) root         (0)     1252 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/cursors/ellipse.png
--rw-rw-rw-   0 root         (0) root         (0)     1116 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/cursors/highlighter.png
--rw-rw-rw-   0 root         (0) root         (0)     1159 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/cursors/line.png
--rw-rw-rw-   0 root         (0) root         (0)      890 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/cursors/pen.png
--rw-rw-rw-   0 root         (0) root         (0)     1116 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/cursors/question_mark.png
--rw-rw-rw-   0 root         (0) root         (0)     1037 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/cursors/text-comment.png
--rw-rw-rw-   0 root         (0) root         (0)      933 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/cursors/text-delta.png
--rw-rw-rw-   0 root         (0) root         (0)      655 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/cursors/text.png
--rw-rw-rw-   0 root         (0) root         (0)      978 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/cursors/tick.png
--rw-rw-rw-   0 root         (0) root         (0)    11967 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/elastics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 00:26:20.862574 plom-0.9.3/plom/client/icons/
--rw-rw-rw-   0 root         (0) root         (0)       85 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/icons/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3242 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/icons/comment.svg
--rw-rw-rw-   0 root         (0) root         (0)     3072 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/icons/comment_down.svg
--rw-rw-rw-   0 root         (0) root         (0)     3117 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/icons/comment_up.svg
--rw-rw-rw-   0 root         (0) root         (0)     2777 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/icons/cross.svg
--rw-rw-rw-   0 root         (0) root         (0)    11993 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/icons/delete.svg
--rw-rw-rw-   0 root         (0) root         (0)     2558 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/icons/delta.svg
--rw-rw-rw-   0 root         (0) root         (0)     3971 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/icons/line.svg
--rw-rw-rw-   0 root         (0) root         (0)     5497 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/icons/manager_collide.svg
--rw-rw-rw-   0 root         (0) root         (0)     4911 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/icons/manager_discard.svg
--rw-rw-rw-   0 root         (0) root         (0)     4891 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/icons/manager_extra.svg
--rw-rw-rw-   0 root         (0) root         (0)     7021 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/icons/manager_hw.svg
--rw-rw-rw-   0 root         (0) root         (0)     4965 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/icons/manager_move.svg
--rw-rw-rw-   0 root         (0) root         (0)     4362 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/icons/manager_none.svg
--rw-rw-rw-   0 root         (0) root         (0)     4469 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/icons/manager_test.svg
--rw-rw-rw-   0 root         (0) root         (0)     5434 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/icons/manager_unknown.svg
--rw-rw-rw-   0 root         (0) root         (0)    13239 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/icons/move.svg
--rw-rw-rw-   0 root         (0) root         (0)    14761 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/icons/pan.svg
--rw-rw-rw-   0 root         (0) root         (0)     3261 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/icons/pen.svg
--rw-rw-rw-   0 root         (0) root         (0)     4726 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/icons/rectangle.svg
--rw-rw-rw-   0 root         (0) root         (0)     5031 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/icons/rectangle_highlight.svg
--rw-rw-rw-   0 root         (0) root         (0)    10387 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/icons/redo.svg
--rw-rw-rw-   0 root         (0) root         (0)     3303 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/icons/text.svg
--rw-rw-rw-   0 root         (0) root         (0)     2570 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/icons/tick.svg
--rw-rw-rw-   0 root         (0) root         (0)    11036 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/icons/undo.svg
--rw-rw-rw-   0 root         (0) root         (0)    11769 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/icons/zoom.svg
--rw-rw-rw-   0 root         (0) root         (0)    13599 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/icons/zoom_in.svg
--rw-rw-rw-   0 root         (0) root         (0)    13229 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/icons/zoom_out.svg
--rw-rw-rw-   0 root         (0) root         (0)    30999 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/identifier.py
--rw-rw-rw-   0 root         (0) root         (0)    15267 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/image_view_widget.py
--rw-rw-rw-   0 root         (0) root         (0)     6837 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/key_help.py
--rw-rw-rw-   0 root         (0) root         (0)     7612 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/key_wrangler.py
--rw-rw-rw-   0 root         (0) root         (0)    83202 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/marker.py
--rw-rw-rw-   0 root         (0) root         (0)     2194 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/pagecache.py
--rw-rw-rw-   0 root         (0) root         (0)    28631 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/pagerearranger.py
--rw-rw-rw-   0 root         (0) root         (0)    99179 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/pagescene.py
--rw-rw-rw-   0 root         (0) root         (0)    10280 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/pageview.py
--rwxrwxrwx   0 root         (0) root         (0)     1499 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/randoIDer.py
--rwxrwxrwx   0 root         (0) root         (0)     1730 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/randoMarker.py
--rw-rw-rw-   0 root         (0) root         (0)     3343 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/random_identifying_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    11554 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/random_marking_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    56247 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/rubric_list.py
--rw-rw-rw-   0 root         (0) root         (0)    16603 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/rubric_wrangler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 00:26:20.867575 plom-0.9.3/plom/client/tools/
--rw-rw-rw-   0 root         (0) root         (0)     1282 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5199 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/tools/arrow.py
--rw-rw-rw-   0 root         (0) root         (0)     2552 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/tools/box.py
--rw-rw-rw-   0 root         (0) root         (0)      582 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/tools/crop.py
--rw-rw-rw-   0 root         (0) root         (0)     2516 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/tools/cross.py
--rw-rw-rw-   0 root         (0) root         (0)     1838 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/tools/delete.py
--rw-rw-rw-   0 root         (0) root         (0)     3753 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/tools/delta.py
--rw-rw-rw-   0 root         (0) root         (0)     2568 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/tools/ellipse.py
--rw-rw-rw-   0 root         (0) root         (0)     1852 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/tools/highlight.py
--rw-rw-rw-   0 root         (0) root         (0)     8225 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/tools/image.py
--rw-rw-rw-   0 root         (0) root         (0)     2582 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/tools/line.py
--rw-rw-rw-   0 root         (0) root         (0)     1867 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/tools/move.py
--rw-rw-rw-   0 root         (0) root         (0)     3616 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/tools/pen.py
--rw-rw-rw-   0 root         (0) root         (0)     3959 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/tools/penArrow.py
--rw-rw-rw-   0 root         (0) root         (0)     2704 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/tools/questionMark.py
--rw-rw-rw-   0 root         (0) root         (0)     9149 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/tools/rubric.py
--rw-rw-rw-   0 root         (0) root         (0)    13217 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/tools/text.py
--rw-rw-rw-   0 root         (0) root         (0)     2446 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/tools/tick.py
--rw-rw-rw-   0 root         (0) root         (0)     2425 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/tools/tool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 00:26:20.869575 plom-0.9.3/plom/client/uiFiles/
--rw-rw-rw-   0 root         (0) root         (0)       14 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/uiFiles/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    24089 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/uiFiles/ui_annotator.py
--rw-rw-rw-   0 root         (0) root         (0)    12332 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/uiFiles/ui_chooser.py
--rw-rw-rw-   0 root         (0) root         (0)    10772 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/uiFiles/ui_identify.py
--rw-rw-rw-   0 root         (0) root         (0)    31396 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/uiFiles/ui_iic.py
--rw-rw-rw-   0 root         (0) root         (0)    11490 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/uiFiles/ui_marker.py
--rw-rw-rw-   0 root         (0) root         (0)     7511 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/uiFiles/ui_totaler.py
--rw-rw-rw-   0 root         (0) root         (0)    16621 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/useful_classes.py
--rw-rw-rw-   0 root         (0) root         (0)    14386 2022-07-19 00:26:14.000000 plom-0.9.3/plom/client/viewers.py
--rw-rw-rw-   0 root         (0) root         (0)      743 2022-07-19 00:26:14.000000 plom-0.9.3/plom/comment_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 00:26:20.876576 plom-0.9.3/plom/create/
--rw-rw-rw-   0 root         (0) root         (0)     1847 2022-07-19 00:26:14.000000 plom-0.9.3/plom/create/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    27224 2022-07-19 00:26:14.000000 plom-0.9.3/plom/create/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     2304 2022-07-19 00:26:14.000000 plom-0.9.3/plom/create/_digitHunter.py
--rw-rw-rw-   0 root         (0) root         (0)     9253 2022-07-19 00:26:14.000000 plom-0.9.3/plom/create/buildClasslist.py
--rw-rw-rw-   0 root         (0) root         (0)     6457 2022-07-19 00:26:14.000000 plom-0.9.3/plom/create/buildDatabaseAndPapers.py
--rw-rw-rw-   0 root         (0) root         (0)     7272 2022-07-19 00:26:14.000000 plom-0.9.3/plom/create/buildNamedPDF.py
--rw-rw-rw-   0 root         (0) root         (0)    14722 2022-07-19 00:26:14.000000 plom-0.9.3/plom/create/classlistValidator.py
--rw-rw-rw-   0 root         (0) root         (0)     3603 2022-07-19 00:26:14.000000 plom-0.9.3/plom/create/demotools.py
--rw-rw-rw-   0 root         (0) root         (0)    74624 2022-07-19 00:26:14.000000 plom-0.9.3/plom/create/digits.json
--rw-rw-rw-   0 root         (0) root         (0)     1379 2022-07-19 00:26:14.000000 plom-0.9.3/plom/create/exam_scribbler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 00:26:20.877576 plom-0.9.3/plom/create/fonts/
--rw-rw-rw-   0 root         (0) root         (0)      134 2022-07-19 00:26:14.000000 plom-0.9.3/plom/create/fonts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    30820 2022-07-19 00:26:14.000000 plom-0.9.3/plom/create/fonts/ejx_handwriting.ttf
--rw-rw-rw-   0 root         (0) root         (0)     1344 2022-07-19 00:26:14.000000 plom-0.9.3/plom/create/homework_scribbler.py
--rw-rw-rw-   0 root         (0) root         (0)    15341 2022-07-19 00:26:14.000000 plom-0.9.3/plom/create/mergeAndCodePages.py
--rw-rw-rw-   0 root         (0) root         (0)     5682 2022-07-19 00:26:14.000000 plom-0.9.3/plom/create/push_pull_rubrics.py
--rw-rw-rw-   0 root         (0) root         (0)     4664 2022-07-19 00:26:14.000000 plom-0.9.3/plom/create/scribble_hw_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    13789 2022-07-19 00:26:14.000000 plom-0.9.3/plom/create/scribble_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2354 2022-07-19 00:26:14.000000 plom-0.9.3/plom/create/start_messenger.py
--rw-rw-rw-   0 root         (0) root         (0)     5093 2022-07-19 00:26:14.000000 plom-0.9.3/plom/create/status.py
--rw-rw-rw-   0 root         (0) root         (0)      868 2022-07-19 00:26:14.000000 plom-0.9.3/plom/create/test_build_source_exams.py
--rw-rw-rw-   0 root         (0) root         (0)    14097 2022-07-19 00:26:14.000000 plom-0.9.3/plom/create/test_classlists.py
--rw-rw-rw-   0 root         (0) root         (0)     3582 2022-07-19 00:26:14.000000 plom-0.9.3/plom/create/test_stamps.py
--rw-rw-rw-   0 root         (0) root         (0)      773 2022-07-19 00:26:14.000000 plom-0.9.3/plom/create/test_upload_classlist.py
--rw-rw-rw-   0 root         (0) root         (0)     2472 2022-07-19 00:26:14.000000 plom-0.9.3/plom/create/upload_classlist.py
--rw-rw-rw-   0 root         (0) root         (0)     5739 2022-07-19 00:26:14.000000 plom-0.9.3/plom/create/version_map_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 00:26:20.881576 plom-0.9.3/plom/db/
--rw-rw-rw-   0 root         (0) root         (0)      436 2022-07-19 00:26:14.000000 plom-0.9.3/plom/db/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3687 2022-07-19 00:26:14.000000 plom-0.9.3/plom/db/buildPlomDB.py
--rw-rw-rw-   0 root         (0) root         (0)    18184 2022-07-19 00:26:14.000000 plom-0.9.3/plom/db/db_create.py
--rw-rw-rw-   0 root         (0) root         (0)    16391 2022-07-19 00:26:14.000000 plom-0.9.3/plom/db/db_identify.py
--rw-rw-rw-   0 root         (0) root         (0)    23177 2022-07-19 00:26:14.000000 plom-0.9.3/plom/db/db_manage.py
--rw-rw-rw-   0 root         (0) root         (0)    28534 2022-07-19 00:26:14.000000 plom-0.9.3/plom/db/db_mark.py
--rw-rw-rw-   0 root         (0) root         (0)    27253 2022-07-19 00:26:14.000000 plom-0.9.3/plom/db/db_report.py
--rw-rw-rw-   0 root         (0) root         (0)     9877 2022-07-19 00:26:14.000000 plom-0.9.3/plom/db/db_rubric.py
--rw-rw-rw-   0 root         (0) root         (0)    40935 2022-07-19 00:26:14.000000 plom-0.9.3/plom/db/db_upload.py
--rw-rw-rw-   0 root         (0) root         (0)     5199 2022-07-19 00:26:14.000000 plom-0.9.3/plom/db/db_user.py
--rw-rw-rw-   0 root         (0) root         (0)     6143 2022-07-19 00:26:14.000000 plom-0.9.3/plom/db/examDB.py
--rw-rw-rw-   0 root         (0) root         (0)     7912 2022-07-19 00:26:14.000000 plom-0.9.3/plom/db/tables.py
--rw-rw-rw-   0 root         (0) root         (0)    27045 2022-07-19 00:26:14.000000 plom-0.9.3/plom/demoClassList.csv
--rw-rw-rw-   0 root         (0) root         (0)     1622 2022-07-19 00:26:14.000000 plom-0.9.3/plom/demo_rubrics.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 00:26:20.886577 plom-0.9.3/plom/finish/
--rw-rw-rw-   0 root         (0) root         (0)     1457 2022-07-19 00:26:14.000000 plom-0.9.3/plom/finish/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9129 2022-07-19 00:26:14.000000 plom-0.9.3/plom/finish/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     5955 2022-07-19 00:26:14.000000 plom-0.9.3/plom/finish/assemble_solutions.py
--rw-rw-rw-   0 root         (0) root         (0)      620 2022-07-19 00:26:14.000000 plom-0.9.3/plom/finish/audit.py
--rw-rw-rw-   0 root         (0) root         (0)     6582 2022-07-19 00:26:14.000000 plom-0.9.3/plom/finish/check_completed.py
--rw-rw-rw-   0 root         (0) root         (0)      721 2022-07-19 00:26:14.000000 plom-0.9.3/plom/finish/clear_manager_login.py
--rwxrwxrwx   0 root         (0) root         (0)     5463 2022-07-19 00:26:14.000000 plom-0.9.3/plom/finish/coded_return.py
--rw-rw-rw-   0 root         (0) root         (0)     2919 2022-07-19 00:26:14.000000 plom-0.9.3/plom/finish/coverPageBuilder.py
--rw-rw-rw-   0 root         (0) root         (0)     4966 2022-07-19 00:26:14.000000 plom-0.9.3/plom/finish/examReassembler.py
--rw-rw-rw-   0 root         (0) root         (0)     4997 2022-07-19 00:26:14.000000 plom-0.9.3/plom/finish/html_view_test_template.py
--rw-rw-rw-   0 root         (0) root         (0)     3026 2022-07-19 00:26:14.000000 plom-0.9.3/plom/finish/reassemble_ID_only.py
--rw-rw-rw-   0 root         (0) root         (0)     8980 2022-07-19 00:26:14.000000 plom-0.9.3/plom/finish/reassemble_completed.py
--rw-rw-rw-   0 root         (0) root         (0)    12834 2022-07-19 00:26:14.000000 plom-0.9.3/plom/finish/return_tools.py
--rw-rw-rw-   0 root         (0) root         (0)      952 2022-07-19 00:26:14.000000 plom-0.9.3/plom/finish/rubric_downloads.py
--rw-rw-rw-   0 root         (0) root         (0)     3227 2022-07-19 00:26:14.000000 plom-0.9.3/plom/finish/solutionAssembler.py
--rw-rw-rw-   0 root         (0) root         (0)     4635 2022-07-19 00:26:14.000000 plom-0.9.3/plom/finish/spreadsheet.py
--rw-rw-rw-   0 root         (0) root         (0)     1850 2022-07-19 00:26:14.000000 plom-0.9.3/plom/finish/start_messenger.py
--rw-rw-rw-   0 root         (0) root         (0)     1284 2022-07-19 00:26:14.000000 plom-0.9.3/plom/finish/test_hash.py
--rw-rw-rw-   0 root         (0) root         (0)     4523 2022-07-19 00:26:14.000000 plom-0.9.3/plom/finish/test_return_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     2894 2022-07-19 00:26:14.000000 plom-0.9.3/plom/finish/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3612 2022-07-19 00:26:14.000000 plom-0.9.3/plom/finishMessenger.py
--rw-rw-rw-   0 root         (0) root         (0)     9457 2022-07-19 00:26:14.000000 plom-0.9.3/plom/idBox2.pdf
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 00:26:20.888577 plom-0.9.3/plom/idreader/
--rw-rw-rw-   0 root         (0) root         (0)      746 2022-07-19 00:26:14.000000 plom-0.9.3/plom/idreader/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3157 2022-07-19 00:26:14.000000 plom-0.9.3/plom/idreader/assign_prob.py
--rw-rw-rw-   0 root         (0) root         (0)     3217 2022-07-19 00:26:14.000000 plom-0.9.3/plom/idreader/model_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    10292 2022-07-19 00:26:14.000000 plom-0.9.3/plom/idreader/predictStudentID.py
--rw-rw-rw-   0 root         (0) root         (0)     4683 2022-07-19 00:26:14.000000 plom-0.9.3/plom/idreader/test_IDreader.py
--rw-rw-rw-   0 root         (0) root         (0)     1768 2022-07-19 00:26:14.000000 plom-0.9.3/plom/idreader/trainRandomForestModel.py
--rw-rw-rw-   0 root         (0) root         (0)     7476 2022-07-19 00:26:14.000000 plom-0.9.3/plom/latexTemplate.tex
--rw-rw-rw-   0 root         (0) root         (0)     7475 2022-07-19 00:26:14.000000 plom-0.9.3/plom/latexTemplatev2.tex
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 00:26:20.891577 plom-0.9.3/plom/manager/
--rw-rw-rw-   0 root         (0) root         (0)      425 2022-07-19 00:26:14.000000 plom-0.9.3/plom/manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2017 2022-07-19 00:26:14.000000 plom-0.9.3/plom/manager/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     4809 2022-07-19 00:26:14.000000 plom-0.9.3/plom/manager/collideview.py
--rw-rw-rw-   0 root         (0) root         (0)     1274 2022-07-19 00:26:14.000000 plom-0.9.3/plom/manager/discardview.py
--rwxrwxrwx   0 root         (0) root         (0)   106072 2022-07-19 00:26:14.000000 plom-0.9.3/plom/manager/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     3512 2022-07-19 00:26:14.000000 plom-0.9.3/plom/manager/reviewview.py
--rw-rw-rw-   0 root         (0) root         (0)     8065 2022-07-19 00:26:14.000000 plom-0.9.3/plom/manager/selectrectangle.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 00:26:20.892578 plom-0.9.3/plom/manager/uiFiles/
--rw-rw-rw-   0 root         (0) root         (0)       14 2022-07-19 00:26:14.000000 plom-0.9.3/plom/manager/uiFiles/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    77263 2022-07-19 00:26:14.000000 plom-0.9.3/plom/manager/uiFiles/ui_manager.py
--rw-rw-rw-   0 root         (0) root         (0)    10612 2022-07-19 00:26:14.000000 plom-0.9.3/plom/manager/unknownpageview.py
--rw-rw-rw-   0 root         (0) root         (0)    63380 2022-07-19 00:26:14.000000 plom-0.9.3/plom/managerMessenger.py
--rw-rw-rw-   0 root         (0) root         (0)    20270 2022-07-19 00:26:14.000000 plom-0.9.3/plom/messenger.py
--rw-rw-rw-   0 root         (0) root         (0)     5718 2022-07-19 00:26:14.000000 plom-0.9.3/plom/misc_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3115 2022-07-19 00:26:14.000000 plom-0.9.3/plom/plom_exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2940 2022-07-19 00:26:14.000000 plom-0.9.3/plom/rules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 00:26:20.898578 plom-0.9.3/plom/scan/
--rw-rw-rw-   0 root         (0) root         (0)     1094 2022-07-19 00:26:14.000000 plom-0.9.3/plom/scan/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8432 2022-07-19 00:26:14.000000 plom-0.9.3/plom/scan/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     3905 2022-07-19 00:26:14.000000 plom-0.9.3/plom/scan/bundle_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4079 2022-07-19 00:26:14.000000 plom-0.9.3/plom/scan/checkScanStatus.py
--rw-rw-rw-   0 root         (0) root         (0)      600 2022-07-19 00:26:14.000000 plom-0.9.3/plom/scan/clearScannerLogin.py
--rw-rw-rw-   0 root         (0) root         (0)     4297 2022-07-19 00:26:14.000000 plom-0.9.3/plom/scan/fasterQRExtract.py
--rw-rw-rw-   0 root         (0) root         (0)    11901 2022-07-19 00:26:14.000000 plom-0.9.3/plom/scan/frontend_hwscan.py
--rw-rw-rw-   0 root         (0) root         (0)     9982 2022-07-19 00:26:14.000000 plom-0.9.3/plom/scan/frontend_scan.py
--rw-rw-rw-   0 root         (0) root         (0)     4157 2022-07-19 00:26:14.000000 plom-0.9.3/plom/scan/hwSubmissionsCheck.py
--rw-rw-rw-   0 root         (0) root         (0)     1049 2022-07-19 00:26:14.000000 plom-0.9.3/plom/scan/listBundles.py
--rw-rw-rw-   0 root         (0) root         (0)    10196 2022-07-19 00:26:14.000000 plom-0.9.3/plom/scan/readQRCodes.py
--rw-rw-rw-   0 root         (0) root         (0)     2175 2022-07-19 00:26:14.000000 plom-0.9.3/plom/scan/rotate.py
--rw-rw-rw-   0 root         (0) root         (0)    14545 2022-07-19 00:26:14.000000 plom-0.9.3/plom/scan/scansToImages.py
--rw-rw-rw-   0 root         (0) root         (0)     5011 2022-07-19 00:26:14.000000 plom-0.9.3/plom/scan/sendCollisionsToServer.py
--rw-rw-rw-   0 root         (0) root         (0)    10040 2022-07-19 00:26:14.000000 plom-0.9.3/plom/scan/sendPagesToServer.py
--rw-rw-rw-   0 root         (0) root         (0)     4327 2022-07-19 00:26:14.000000 plom-0.9.3/plom/scan/sendUnknownsToServer.py
--rw-rw-rw-   0 root         (0) root         (0)     1776 2022-07-19 00:26:14.000000 plom-0.9.3/plom/scan/start_messenger.py
--rw-rw-rw-   0 root         (0) root         (0)     2662 2022-07-19 00:26:14.000000 plom-0.9.3/plom/scan/test_pdf_img_extraction.py
--rw-rw-rw-   0 root         (0) root         (0)     2610 2022-07-19 00:26:14.000000 plom-0.9.3/plom/scan/test_qr_reads.py
--rw-rw-rw-   0 root         (0) root         (0)     2636 2022-07-19 00:26:14.000000 plom-0.9.3/plom/scan/test_question_map_parse.py
--rw-rw-rw-   0 root         (0) root         (0)    84508 2022-07-19 00:26:14.000000 plom-0.9.3/plom/scan/test_zbar_fails.png
--rw-rw-rw-   0 root         (0) root         (0)    17361 2022-07-19 00:26:14.000000 plom-0.9.3/plom/scanMessenger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 00:26:20.901579 plom-0.9.3/plom/scripts/
--rw-rw-rw-   0 root         (0) root         (0)      315 2022-07-19 00:26:14.000000 plom-0.9.3/plom/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      785 2022-07-19 00:26:14.000000 plom-0.9.3/plom/scripts/build_stub.py
--rw-rw-rw-   0 root         (0) root         (0)     6843 2022-07-19 00:26:14.000000 plom-0.9.3/plom/scripts/demo.py
--rw-rw-rw-   0 root         (0) root         (0)     7019 2022-07-19 00:26:14.000000 plom-0.9.3/plom/scripts/hwdemo.py
--rw-rw-rw-   0 root         (0) root         (0)     8384 2022-07-19 00:26:14.000000 plom-0.9.3/plom/scripts/hwscan.py
--rw-rw-rw-   0 root         (0) root         (0)      869 2022-07-19 00:26:14.000000 plom-0.9.3/plom/scripts/plominit.py
--rw-rw-rw-   0 root         (0) root         (0)     1003 2022-07-19 00:26:14.000000 plom-0.9.3/plom/scripts/test_script_help_ver.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 00:26:20.907579 plom-0.9.3/plom/server/
--rw-rw-rw-   0 root         (0) root         (0)     1019 2022-07-19 00:26:14.000000 plom-0.9.3/plom/server/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9964 2022-07-19 00:26:14.000000 plom-0.9.3/plom/server/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     6493 2022-07-19 00:26:14.000000 plom-0.9.3/plom/server/authenticate.py
--rw-rw-rw-   0 root         (0) root         (0)    11839 2022-07-19 00:26:14.000000 plom-0.9.3/plom/server/background.py
--rw-rw-rw-   0 root         (0) root         (0)     1598 2022-07-19 00:26:14.000000 plom-0.9.3/plom/server/cert_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     7604 2022-07-19 00:26:14.000000 plom-0.9.3/plom/server/demo.py
--rw-rw-rw-   0 root         (0) root         (0)     7818 2022-07-19 00:26:14.000000 plom-0.9.3/plom/server/manageUserFiles.py
--rw-rw-rw-   0 root         (0) root         (0)     3187 2022-07-19 00:26:14.000000 plom-0.9.3/plom/server/misc.py
--rwxrwxrwx   0 root         (0) root         (0)    10204 2022-07-19 00:26:14.000000 plom-0.9.3/plom/server/pageNotSubmitted.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 00:26:20.912580 plom-0.9.3/plom/server/plomServer/
--rw-rw-rw-   0 root         (0) root         (0)     1001 2022-07-19 00:26:14.000000 plom-0.9.3/plom/server/plomServer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    26935 2022-07-19 00:26:14.000000 plom-0.9.3/plom/server/plomServer/routesID.py
--rw-rw-rw-   0 root         (0) root         (0)    34265 2022-07-19 00:26:14.000000 plom-0.9.3/plom/server/plomServer/routesMark.py
--rw-rw-rw-   0 root         (0) root         (0)    21505 2022-07-19 00:26:14.000000 plom-0.9.3/plom/server/plomServer/routesReport.py
--rw-rw-rw-   0 root         (0) root         (0)    14096 2022-07-19 00:26:14.000000 plom-0.9.3/plom/server/plomServer/routesRubric.py
--rw-rw-rw-   0 root         (0) root         (0)     3587 2022-07-19 00:26:14.000000 plom-0.9.3/plom/server/plomServer/routesSolution.py
--rw-rw-rw-   0 root         (0) root         (0)    42249 2022-07-19 00:26:14.000000 plom-0.9.3/plom/server/plomServer/routesUpload.py
--rw-rw-rw-   0 root         (0) root         (0)     8716 2022-07-19 00:26:14.000000 plom-0.9.3/plom/server/plomServer/routesUserInit.py
--rw-rw-rw-   0 root         (0) root         (0)     7186 2022-07-19 00:26:14.000000 plom-0.9.3/plom/server/plomServer/routeutils.py
--rw-rw-rw-   0 root         (0) root         (0)    18745 2022-07-19 00:26:14.000000 plom-0.9.3/plom/server/plomServer/serverID.py
--rw-rw-rw-   0 root         (0) root         (0)     9964 2022-07-19 00:26:14.000000 plom-0.9.3/plom/server/plomServer/serverMark.py
--rw-rw-rw-   0 root         (0) root         (0)     1828 2022-07-19 00:26:14.000000 plom-0.9.3/plom/server/plomServer/serverReport.py
--rw-rw-rw-   0 root         (0) root         (0)     2073 2022-07-19 00:26:14.000000 plom-0.9.3/plom/server/plomServer/serverRubric.py
--rw-rw-rw-   0 root         (0) root         (0)     1947 2022-07-19 00:26:14.000000 plom-0.9.3/plom/server/plomServer/serverSolution.py
--rw-rw-rw-   0 root         (0) root         (0)    16293 2022-07-19 00:26:14.000000 plom-0.9.3/plom/server/plomServer/serverUpload.py
--rw-rw-rw-   0 root         (0) root         (0)     5634 2022-07-19 00:26:14.000000 plom-0.9.3/plom/server/plomServer/serverUserInit.py
--rw-rw-rw-   0 root         (0) root         (0)     6069 2022-07-19 00:26:14.000000 plom-0.9.3/plom/server/prepare.py
--rw-rw-rw-   0 root         (0) root         (0)     1630 2022-07-19 00:26:14.000000 plom-0.9.3/plom/server/run_the_predictor.py
--rw-rw-rw-   0 root         (0) root         (0)     1334 2022-07-19 00:26:14.000000 plom-0.9.3/plom/server/target_Q_latex_plom.png
--rw-rw-rw-   0 root         (0) root         (0)      420 2022-07-19 00:26:14.000000 plom-0.9.3/plom/server/test_background.py
--rw-rw-rw-   0 root         (0) root         (0)     1197 2022-07-19 00:26:14.000000 plom-0.9.3/plom/server/test_background_multiprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)     1046 2022-07-19 00:26:14.000000 plom-0.9.3/plom/server/test_background_subprocess.py
--rw-rw-rw-   0 root         (0) root         (0)      984 2022-07-19 00:26:14.000000 plom-0.9.3/plom/server/test_configs.py
--rw-rw-rw-   0 root         (0) root         (0)     8085 2022-07-19 00:26:14.000000 plom-0.9.3/plom/server/test_demo.py
--rw-rw-rw-   0 root         (0) root         (0)      691 2022-07-19 00:26:14.000000 plom-0.9.3/plom/server/test_dirs.py
--rw-rw-rw-   0 root         (0) root         (0)      539 2022-07-19 00:26:14.000000 plom-0.9.3/plom/server/test_ssl_selfsigned.py
--rw-rw-rw-   0 root         (0) root         (0)    11520 2022-07-19 00:26:14.000000 plom-0.9.3/plom/server/theServer.py
--rw-rw-rw-   0 root         (0) root         (0)      595 2022-07-19 00:26:14.000000 plom-0.9.3/plom/serverDetails.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 00:26:20.915580 plom-0.9.3/plom/solutions/
--rw-rw-rw-   0 root         (0) root         (0)     1120 2022-07-19 00:26:14.000000 plom-0.9.3/plom/solutions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9228 2022-07-19 00:26:14.000000 plom-0.9.3/plom/solutions/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)      598 2022-07-19 00:26:14.000000 plom-0.9.3/plom/solutions/checkSolutionStatus.py
--rw-rw-rw-   0 root         (0) root         (0)     1021 2022-07-19 00:26:14.000000 plom-0.9.3/plom/solutions/deleteSolutionImage.py
--rw-rw-rw-   0 root         (0) root         (0)     5317 2022-07-19 00:26:14.000000 plom-0.9.3/plom/solutions/extractSolutions.py
--rw-rw-rw-   0 root         (0) root         (0)     1006 2022-07-19 00:26:14.000000 plom-0.9.3/plom/solutions/getSolutionImage.py
--rw-rw-rw-   0 root         (0) root         (0)      328 2022-07-19 00:26:14.000000 plom-0.9.3/plom/solutions/msgr_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2348 2022-07-19 00:26:14.000000 plom-0.9.3/plom/solutions/putSolutionImage.py
--rw-rw-rw-   0 root         (0) root         (0)    27974 2022-07-19 00:26:14.000000 plom-0.9.3/plom/specVerifier.py
--rw-rw-rw-   0 root         (0) root         (0)      661 2022-07-19 00:26:14.000000 plom-0.9.3/plom/templateSolutionSpec.toml
--rw-rw-rw-   0 root         (0) root         (0)     1712 2022-07-19 00:26:14.000000 plom-0.9.3/plom/templateTestSpec.toml
--rw-rw-rw-   0 root         (0) root         (0)      115 2022-07-19 00:26:14.000000 plom-0.9.3/plom/templateUserList.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 00:26:20.922581 plom-0.9.3/plom/testTemplates/
--rw-rw-rw-   0 root         (0) root         (0)     2131 2022-07-19 00:26:14.000000 plom-0.9.3/plom/testTemplates/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1383 2022-07-19 00:26:14.000000 plom-0.9.3/plom/testTemplates/dummy_left_staple.png
--rw-rw-rw-   0 root         (0) root         (0)    12633 2022-07-19 00:26:14.000000 plom-0.9.3/plom/testTemplates/dummy_left_staple_red.png
--rw-rw-rw-   0 root         (0) root         (0)      652 2022-07-19 00:26:14.000000 plom-0.9.3/plom/testTemplates/dummy_qr_code.png
--rw-rw-rw-   0 root         (0) root         (0)    17894 2022-07-19 00:26:14.000000 plom-0.9.3/plom/testTemplates/dummy_qr_code_red.png
--rw-rw-rw-   0 root         (0) root         (0)     2307 2022-07-19 00:26:14.000000 plom-0.9.3/plom/testTemplates/dummy_right_staple.png
--rw-rw-rw-   0 root         (0) root         (0)    13933 2022-07-19 00:26:14.000000 plom-0.9.3/plom/testTemplates/dummy_right_staple_red.png
--rw-rw-rw-   0 root         (0) root         (0)     2460 2022-07-19 00:26:14.000000 plom-0.9.3/plom/testTemplates/extraSheets.tex
--rw-rw-rw-   0 root         (0) root         (0)     2378 2022-07-19 00:26:14.000000 plom-0.9.3/plom/testTemplates/extraSheets_noname.tex
--rw-rw-rw-   0 root         (0) root         (0)      997 2022-07-19 00:26:14.000000 plom-0.9.3/plom/testTemplates/idBox-source.tex
--rw-rw-rw-   0 root         (0) root         (0)    43340 2022-07-19 00:26:14.000000 plom-0.9.3/plom/testTemplates/idBox.eps
--rw-rw-rw-   0 root         (0) root         (0)    13872 2022-07-19 00:26:14.000000 plom-0.9.3/plom/testTemplates/idBox.pdf
--rw-rw-rw-   0 root         (0) root         (0)    35624 2022-07-19 00:26:14.000000 plom-0.9.3/plom/testTemplates/idBox.svg
--rw-rw-rw-   0 root         (0) root         (0)      941 2022-07-19 00:26:14.000000 plom-0.9.3/plom/testTemplates/idBox2-source.tex
--rw-rw-rw-   0 root         (0) root         (0)    29216 2022-07-19 00:26:14.000000 plom-0.9.3/plom/testTemplates/idBox2.eps
--rw-rw-rw-   0 root         (0) root         (0)     9457 2022-07-19 00:26:14.000000 plom-0.9.3/plom/testTemplates/idBox2.pdf
--rw-rw-rw-   0 root         (0) root         (0)    29857 2022-07-19 00:26:14.000000 plom-0.9.3/plom/testTemplates/idBox2.svg
--rw-rw-rw-   0 root         (0) root         (0)     7537 2022-07-19 00:26:14.000000 plom-0.9.3/plom/testTemplates/latexTemplate.tex
--rw-rw-rw-   0 root         (0) root         (0)     7536 2022-07-19 00:26:14.000000 plom-0.9.3/plom/testTemplates/latexTemplatev2.tex
--rw-rw-rw-   0 root         (0) root         (0)     2411 2022-07-19 00:26:14.000000 plom-0.9.3/plom/testTemplates/mockplom.sty
--rw-rw-rw-   0 root         (0) root         (0)      805 2022-07-19 00:26:14.000000 plom-0.9.3/plom/test_exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)      955 2022-07-19 00:26:14.000000 plom-0.9.3/plom/test_latex.py
--rw-rw-rw-   0 root         (0) root         (0)     2659 2022-07-19 00:26:14.000000 plom-0.9.3/plom/test_latexfrag.py
--rw-rw-rw-   0 root         (0) root         (0)      338 2022-07-19 00:26:14.000000 plom-0.9.3/plom/test_messengers.py
--rw-rw-rw-   0 root         (0) root         (0)     1093 2022-07-19 00:26:14.000000 plom-0.9.3/plom/test_misc_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     7636 2022-07-19 00:26:14.000000 plom-0.9.3/plom/test_spec.py
--rw-rw-rw-   0 root         (0) root         (0)      124 2022-07-19 00:26:14.000000 plom-0.9.3/plom/test_version.py
--rw-rw-rw-   0 root         (0) root         (0)     2935 2022-07-19 00:26:14.000000 plom-0.9.3/plom/test_version_maps.py
--rw-rw-rw-   0 root         (0) root         (0)     5419 2022-07-19 00:26:14.000000 plom-0.9.3/plom/textools.py
--rw-rw-rw-   0 root         (0) root         (0)     3683 2022-07-19 00:26:14.000000 plom-0.9.3/plom/tpv_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      197 2022-07-19 00:26:14.000000 plom-0.9.3/plom/version.py
--rw-rw-rw-   0 root         (0) root         (0)     5153 2022-07-19 00:26:14.000000 plom-0.9.3/plom/version_maps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 00:26:20.838571 plom-0.9.3/plom.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2366 2022-07-19 00:26:20.000000 plom-0.9.3/plom.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9293 2022-07-19 00:26:20.000000 plom-0.9.3/plom.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-19 00:26:20.000000 plom-0.9.3/plom.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      496 2022-07-19 00:26:20.000000 plom-0.9.3/plom.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      316 2022-07-19 00:26:20.000000 plom-0.9.3/plom.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2022-07-19 00:26:20.000000 plom-0.9.3/plom.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      870 2022-07-19 00:26:14.000000 plom-0.9.3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      887 2022-07-19 00:26:14.000000 plom-0.9.3/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      644 2022-07-19 00:26:14.000000 plom-0.9.3/requirements.txt.client
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-19 00:26:20.922581 plom-0.9.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     4823 2022-07-19 00:26:14.000000 plom-0.9.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-05 05:51:22.037250 plom-0.9.4/
+-rw-rw-rw-   0 root         (0) root         (0)    32223 2022-08-05 05:51:14.000000 plom-0.9.4/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)     1021 2022-08-05 05:51:14.000000 plom-0.9.4/CONTRIBUTORS
+-rw-rw-rw-   0 root         (0) root         (0)     1547 2022-08-05 05:51:14.000000 plom-0.9.4/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)    34283 2022-08-05 05:51:14.000000 plom-0.9.4/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)     1137 2022-08-05 05:51:14.000000 plom-0.9.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2366 2022-08-05 05:51:22.036250 plom-0.9.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1835 2022-08-05 05:51:14.000000 plom-0.9.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-05 05:51:21.932239 plom-0.9.4/contrib/
+-rw-rw-rw-   0 root         (0) root         (0)      252 2022-08-05 05:51:14.000000 plom-0.9.4/contrib/README.txt
+-rwxrwxrwx   0 root         (0) root         (0)    11813 2022-08-05 05:51:14.000000 plom-0.9.4/contrib/plom-push-to-canvas.py
+-rwxrwxrwx   0 root         (0) root         (0)     2162 2022-08-05 05:51:14.000000 plom-0.9.4/contrib/plom-return_codes_to_canvas_csv.py
+-rwxrwxrwx   0 root         (0) root         (0)     2138 2022-08-05 05:51:14.000000 plom-0.9.4/contrib/plom-write_grades_to_canvas_csv.py
+-rwxrwxrwx   0 root         (0) root         (0)     7058 2022-08-05 05:51:14.000000 plom-0.9.4/contrib/upload_hw_from_zip_of_jpegs.py
+-rw-rw-rw-   0 root         (0) root         (0)      583 2022-08-05 05:51:14.000000 plom-0.9.4/org.plomgrading.PlomClient.desktop
+-rw-rw-rw-   0 root         (0) root         (0)     4944 2022-08-05 05:51:14.000000 plom-0.9.4/org.plomgrading.PlomClient.metainfo.xml
+-rw-rw-rw-   0 root         (0) root         (0)     7237 2022-08-05 05:51:14.000000 plom-0.9.4/org.plomgrading.PlomClient.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-05 05:51:21.943240 plom-0.9.4/plom/
+-rw-rw-rw-   0 root         (0) root         (0)     1379 2022-08-05 05:51:14.000000 plom-0.9.4/plom/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7404 2022-08-05 05:51:14.000000 plom-0.9.4/plom/aliceBob.py
+-rw-rw-rw-   0 root         (0) root         (0)    39534 2022-08-05 05:51:14.000000 plom-0.9.4/plom/baseMessenger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-05 05:51:21.946241 plom-0.9.4/plom/canvas/
+-rw-rw-rw-   0 root         (0) root         (0)      629 2022-08-05 05:51:14.000000 plom-0.9.4/plom/canvas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12833 2022-08-05 05:51:14.000000 plom-0.9.4/plom/canvas/canvas_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5856 2022-08-05 05:51:14.000000 plom-0.9.4/plom/canvas/canvasapi_extensions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-05 05:51:21.954241 plom-0.9.4/plom/client/
+-rw-rw-rw-   0 root         (0) root         (0)      722 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5580 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)    75770 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/annotator.py
+-rw-rw-rw-   0 root         (0) root         (0)      850 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/backGrid.py
+-rw-rw-rw-   0 root         (0) root         (0)     3632 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/backGrid1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    46182 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/backGrid2.png
+-rw-rw-rw-   0 root         (0) root         (0)     4282 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/background_downloader.py
+-rw-rw-rw-   0 root         (0) root         (0)    19204 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/chooser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-05 05:51:21.959242 plom-0.9.4/plom/client/cursors/
+-rw-rw-rw-   0 root         (0) root         (0)      236 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/cursors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1234 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/cursors/arrow.png
+-rw-rw-rw-   0 root         (0) root         (0)     1177 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/cursors/box.png
+-rw-rw-rw-   0 root         (0) root         (0)     1049 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/cursors/crop.png
+-rw-rw-rw-   0 root         (0) root         (0)     1049 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/cursors/cross.png
+-rw-rw-rw-   0 root         (0) root         (0)     1465 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/cursors/delete.png
+-rw-rw-rw-   0 root         (0) root         (0)     1297 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/cursors/double_arrow.png
+-rw-rw-rw-   0 root         (0) root         (0)     1252 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/cursors/ellipse.png
+-rw-rw-rw-   0 root         (0) root         (0)     1116 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/cursors/highlighter.png
+-rw-rw-rw-   0 root         (0) root         (0)     1159 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/cursors/line.png
+-rw-rw-rw-   0 root         (0) root         (0)      890 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/cursors/pen.png
+-rw-rw-rw-   0 root         (0) root         (0)     1116 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/cursors/question_mark.png
+-rw-rw-rw-   0 root         (0) root         (0)     1037 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/cursors/text-comment.png
+-rw-rw-rw-   0 root         (0) root         (0)      933 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/cursors/text-delta.png
+-rw-rw-rw-   0 root         (0) root         (0)      655 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/cursors/text.png
+-rw-rw-rw-   0 root         (0) root         (0)      978 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/cursors/tick.png
+-rw-rw-rw-   0 root         (0) root         (0)    11967 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/elastics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-05 05:51:21.969243 plom-0.9.4/plom/client/icons/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/icons/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3242 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/icons/comment.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3072 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/icons/comment_down.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3117 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/icons/comment_up.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2777 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/icons/cross.svg
+-rw-rw-rw-   0 root         (0) root         (0)    11993 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/icons/delete.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2558 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/icons/delta.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3971 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/icons/line.svg
+-rw-rw-rw-   0 root         (0) root         (0)     5497 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/icons/manager_collide.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4911 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/icons/manager_discard.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4891 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/icons/manager_extra.svg
+-rw-rw-rw-   0 root         (0) root         (0)     7021 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/icons/manager_hw.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4965 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/icons/manager_move.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4362 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/icons/manager_none.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4469 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/icons/manager_test.svg
+-rw-rw-rw-   0 root         (0) root         (0)     5434 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/icons/manager_unknown.svg
+-rw-rw-rw-   0 root         (0) root         (0)    13239 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/icons/move.svg
+-rw-rw-rw-   0 root         (0) root         (0)    14761 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/icons/pan.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3261 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/icons/pen.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4726 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/icons/rectangle.svg
+-rw-rw-rw-   0 root         (0) root         (0)     5031 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/icons/rectangle_highlight.svg
+-rw-rw-rw-   0 root         (0) root         (0)    10387 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/icons/redo.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3303 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/icons/text.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2570 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/icons/tick.svg
+-rw-rw-rw-   0 root         (0) root         (0)    11036 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/icons/undo.svg
+-rw-rw-rw-   0 root         (0) root         (0)    11769 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/icons/zoom.svg
+-rw-rw-rw-   0 root         (0) root         (0)    13599 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/icons/zoom_in.svg
+-rw-rw-rw-   0 root         (0) root         (0)    13229 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/icons/zoom_out.svg
+-rw-rw-rw-   0 root         (0) root         (0)    30999 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/identifier.py
+-rw-rw-rw-   0 root         (0) root         (0)    15267 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/image_view_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     6837 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/key_help.py
+-rw-rw-rw-   0 root         (0) root         (0)     7612 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/key_wrangler.py
+-rw-rw-rw-   0 root         (0) root         (0)    83202 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/marker.py
+-rw-rw-rw-   0 root         (0) root         (0)     2194 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/pagecache.py
+-rw-rw-rw-   0 root         (0) root         (0)    28631 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/pagerearranger.py
+-rw-rw-rw-   0 root         (0) root         (0)    99179 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/pagescene.py
+-rw-rw-rw-   0 root         (0) root         (0)    10280 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/pageview.py
+-rwxrwxrwx   0 root         (0) root         (0)     1499 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/randoIDer.py
+-rwxrwxrwx   0 root         (0) root         (0)     1730 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/randoMarker.py
+-rw-rw-rw-   0 root         (0) root         (0)     3343 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/random_identifying_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    11554 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/random_marking_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    56247 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/rubric_list.py
+-rw-rw-rw-   0 root         (0) root         (0)    16603 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/rubric_wrangler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-05 05:51:21.975243 plom-0.9.4/plom/client/tools/
+-rw-rw-rw-   0 root         (0) root         (0)     1282 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5199 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/tools/arrow.py
+-rw-rw-rw-   0 root         (0) root         (0)     2552 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/tools/box.py
+-rw-rw-rw-   0 root         (0) root         (0)      582 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/tools/crop.py
+-rw-rw-rw-   0 root         (0) root         (0)     2516 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/tools/cross.py
+-rw-rw-rw-   0 root         (0) root         (0)     1838 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/tools/delete.py
+-rw-rw-rw-   0 root         (0) root         (0)     3753 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/tools/delta.py
+-rw-rw-rw-   0 root         (0) root         (0)     2568 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/tools/ellipse.py
+-rw-rw-rw-   0 root         (0) root         (0)     1852 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/tools/highlight.py
+-rw-rw-rw-   0 root         (0) root         (0)     8225 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/tools/image.py
+-rw-rw-rw-   0 root         (0) root         (0)     2582 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/tools/line.py
+-rw-rw-rw-   0 root         (0) root         (0)     1867 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/tools/move.py
+-rw-rw-rw-   0 root         (0) root         (0)     3616 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/tools/pen.py
+-rw-rw-rw-   0 root         (0) root         (0)     3959 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/tools/penArrow.py
+-rw-rw-rw-   0 root         (0) root         (0)     2704 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/tools/questionMark.py
+-rw-rw-rw-   0 root         (0) root         (0)     9149 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/tools/rubric.py
+-rw-rw-rw-   0 root         (0) root         (0)    13217 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/tools/text.py
+-rw-rw-rw-   0 root         (0) root         (0)     2446 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/tools/tick.py
+-rw-rw-rw-   0 root         (0) root         (0)     2425 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/tools/tool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-05 05:51:21.977244 plom-0.9.4/plom/client/uiFiles/
+-rw-rw-rw-   0 root         (0) root         (0)       14 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/uiFiles/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    24089 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/uiFiles/ui_annotator.py
+-rw-rw-rw-   0 root         (0) root         (0)    12332 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/uiFiles/ui_chooser.py
+-rw-rw-rw-   0 root         (0) root         (0)    10772 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/uiFiles/ui_identify.py
+-rw-rw-rw-   0 root         (0) root         (0)    31396 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/uiFiles/ui_iic.py
+-rw-rw-rw-   0 root         (0) root         (0)    11490 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/uiFiles/ui_marker.py
+-rw-rw-rw-   0 root         (0) root         (0)     7511 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/uiFiles/ui_totaler.py
+-rw-rw-rw-   0 root         (0) root         (0)    16621 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/useful_classes.py
+-rw-rw-rw-   0 root         (0) root         (0)    14386 2022-08-05 05:51:14.000000 plom-0.9.4/plom/client/viewers.py
+-rw-rw-rw-   0 root         (0) root         (0)      743 2022-08-05 05:51:14.000000 plom-0.9.4/plom/comment_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-05 05:51:21.985245 plom-0.9.4/plom/create/
+-rw-rw-rw-   0 root         (0) root         (0)     1847 2022-08-05 05:51:14.000000 plom-0.9.4/plom/create/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    27224 2022-08-05 05:51:14.000000 plom-0.9.4/plom/create/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2304 2022-08-05 05:51:14.000000 plom-0.9.4/plom/create/_digitHunter.py
+-rw-rw-rw-   0 root         (0) root         (0)     9253 2022-08-05 05:51:14.000000 plom-0.9.4/plom/create/buildClasslist.py
+-rw-rw-rw-   0 root         (0) root         (0)     6530 2022-08-05 05:51:14.000000 plom-0.9.4/plom/create/buildDatabaseAndPapers.py
+-rw-rw-rw-   0 root         (0) root         (0)     7272 2022-08-05 05:51:14.000000 plom-0.9.4/plom/create/buildNamedPDF.py
+-rw-rw-rw-   0 root         (0) root         (0)    14722 2022-08-05 05:51:14.000000 plom-0.9.4/plom/create/classlistValidator.py
+-rw-rw-rw-   0 root         (0) root         (0)     3603 2022-08-05 05:51:14.000000 plom-0.9.4/plom/create/demotools.py
+-rw-rw-rw-   0 root         (0) root         (0)    74624 2022-08-05 05:51:14.000000 plom-0.9.4/plom/create/digits.json
+-rw-rw-rw-   0 root         (0) root         (0)     1379 2022-08-05 05:51:14.000000 plom-0.9.4/plom/create/exam_scribbler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-05 05:51:21.985245 plom-0.9.4/plom/create/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)      134 2022-08-05 05:51:14.000000 plom-0.9.4/plom/create/fonts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    30820 2022-08-05 05:51:14.000000 plom-0.9.4/plom/create/fonts/ejx_handwriting.ttf
+-rw-rw-rw-   0 root         (0) root         (0)     1344 2022-08-05 05:51:14.000000 plom-0.9.4/plom/create/homework_scribbler.py
+-rw-rw-rw-   0 root         (0) root         (0)    15341 2022-08-05 05:51:14.000000 plom-0.9.4/plom/create/mergeAndCodePages.py
+-rw-rw-rw-   0 root         (0) root         (0)     5682 2022-08-05 05:51:14.000000 plom-0.9.4/plom/create/push_pull_rubrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     4664 2022-08-05 05:51:14.000000 plom-0.9.4/plom/create/scribble_hw_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    13789 2022-08-05 05:51:14.000000 plom-0.9.4/plom/create/scribble_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2354 2022-08-05 05:51:14.000000 plom-0.9.4/plom/create/start_messenger.py
+-rw-rw-rw-   0 root         (0) root         (0)     5093 2022-08-05 05:51:14.000000 plom-0.9.4/plom/create/status.py
+-rw-rw-rw-   0 root         (0) root         (0)      868 2022-08-05 05:51:14.000000 plom-0.9.4/plom/create/test_build_source_exams.py
+-rw-rw-rw-   0 root         (0) root         (0)    14097 2022-08-05 05:51:14.000000 plom-0.9.4/plom/create/test_classlists.py
+-rw-rw-rw-   0 root         (0) root         (0)     3582 2022-08-05 05:51:14.000000 plom-0.9.4/plom/create/test_stamps.py
+-rw-rw-rw-   0 root         (0) root         (0)      773 2022-08-05 05:51:14.000000 plom-0.9.4/plom/create/test_upload_classlist.py
+-rw-rw-rw-   0 root         (0) root         (0)     2472 2022-08-05 05:51:14.000000 plom-0.9.4/plom/create/upload_classlist.py
+-rw-rw-rw-   0 root         (0) root         (0)     5739 2022-08-05 05:51:14.000000 plom-0.9.4/plom/create/version_map_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-05 05:51:21.990245 plom-0.9.4/plom/db/
+-rw-rw-rw-   0 root         (0) root         (0)      436 2022-08-05 05:51:14.000000 plom-0.9.4/plom/db/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3687 2022-08-05 05:51:14.000000 plom-0.9.4/plom/db/buildPlomDB.py
+-rw-rw-rw-   0 root         (0) root         (0)    18184 2022-08-05 05:51:14.000000 plom-0.9.4/plom/db/db_create.py
+-rw-rw-rw-   0 root         (0) root         (0)    16391 2022-08-05 05:51:14.000000 plom-0.9.4/plom/db/db_identify.py
+-rw-rw-rw-   0 root         (0) root         (0)    23177 2022-08-05 05:51:14.000000 plom-0.9.4/plom/db/db_manage.py
+-rw-rw-rw-   0 root         (0) root         (0)    28534 2022-08-05 05:51:14.000000 plom-0.9.4/plom/db/db_mark.py
+-rw-rw-rw-   0 root         (0) root         (0)    27253 2022-08-05 05:51:14.000000 plom-0.9.4/plom/db/db_report.py
+-rw-rw-rw-   0 root         (0) root         (0)     9877 2022-08-05 05:51:14.000000 plom-0.9.4/plom/db/db_rubric.py
+-rw-rw-rw-   0 root         (0) root         (0)    40935 2022-08-05 05:51:14.000000 plom-0.9.4/plom/db/db_upload.py
+-rw-rw-rw-   0 root         (0) root         (0)     5199 2022-08-05 05:51:14.000000 plom-0.9.4/plom/db/db_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     6143 2022-08-05 05:51:14.000000 plom-0.9.4/plom/db/examDB.py
+-rw-rw-rw-   0 root         (0) root         (0)     7912 2022-08-05 05:51:14.000000 plom-0.9.4/plom/db/tables.py
+-rw-rw-rw-   0 root         (0) root         (0)    27045 2022-08-05 05:51:14.000000 plom-0.9.4/plom/demoClassList.csv
+-rw-rw-rw-   0 root         (0) root         (0)     1622 2022-08-05 05:51:14.000000 plom-0.9.4/plom/demo_rubrics.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-05 05:51:21.996246 plom-0.9.4/plom/finish/
+-rw-rw-rw-   0 root         (0) root         (0)     1457 2022-08-05 05:51:14.000000 plom-0.9.4/plom/finish/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9129 2022-08-05 05:51:14.000000 plom-0.9.4/plom/finish/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5955 2022-08-05 05:51:14.000000 plom-0.9.4/plom/finish/assemble_solutions.py
+-rw-rw-rw-   0 root         (0) root         (0)      620 2022-08-05 05:51:14.000000 plom-0.9.4/plom/finish/audit.py
+-rw-rw-rw-   0 root         (0) root         (0)     6582 2022-08-05 05:51:14.000000 plom-0.9.4/plom/finish/check_completed.py
+-rw-rw-rw-   0 root         (0) root         (0)      721 2022-08-05 05:51:14.000000 plom-0.9.4/plom/finish/clear_manager_login.py
+-rwxrwxrwx   0 root         (0) root         (0)     5463 2022-08-05 05:51:14.000000 plom-0.9.4/plom/finish/coded_return.py
+-rw-rw-rw-   0 root         (0) root         (0)     2991 2022-08-05 05:51:14.000000 plom-0.9.4/plom/finish/coverPageBuilder.py
+-rw-rw-rw-   0 root         (0) root         (0)     4966 2022-08-05 05:51:14.000000 plom-0.9.4/plom/finish/examReassembler.py
+-rw-rw-rw-   0 root         (0) root         (0)     4997 2022-08-05 05:51:14.000000 plom-0.9.4/plom/finish/html_view_test_template.py
+-rw-rw-rw-   0 root         (0) root         (0)     3026 2022-08-05 05:51:14.000000 plom-0.9.4/plom/finish/reassemble_ID_only.py
+-rw-rw-rw-   0 root         (0) root         (0)     8980 2022-08-05 05:51:14.000000 plom-0.9.4/plom/finish/reassemble_completed.py
+-rw-rw-rw-   0 root         (0) root         (0)    12834 2022-08-05 05:51:14.000000 plom-0.9.4/plom/finish/return_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)      952 2022-08-05 05:51:14.000000 plom-0.9.4/plom/finish/rubric_downloads.py
+-rw-rw-rw-   0 root         (0) root         (0)     3227 2022-08-05 05:51:14.000000 plom-0.9.4/plom/finish/solutionAssembler.py
+-rw-rw-rw-   0 root         (0) root         (0)     4635 2022-08-05 05:51:14.000000 plom-0.9.4/plom/finish/spreadsheet.py
+-rw-rw-rw-   0 root         (0) root         (0)     1850 2022-08-05 05:51:14.000000 plom-0.9.4/plom/finish/start_messenger.py
+-rw-rw-rw-   0 root         (0) root         (0)     1284 2022-08-05 05:51:14.000000 plom-0.9.4/plom/finish/test_hash.py
+-rw-rw-rw-   0 root         (0) root         (0)     4523 2022-08-05 05:51:14.000000 plom-0.9.4/plom/finish/test_return_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     2894 2022-08-05 05:51:14.000000 plom-0.9.4/plom/finish/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3612 2022-08-05 05:51:14.000000 plom-0.9.4/plom/finishMessenger.py
+-rw-rw-rw-   0 root         (0) root         (0)     9457 2022-08-05 05:51:14.000000 plom-0.9.4/plom/idBox2.pdf
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-05 05:51:21.998246 plom-0.9.4/plom/idreader/
+-rw-rw-rw-   0 root         (0) root         (0)      746 2022-08-05 05:51:14.000000 plom-0.9.4/plom/idreader/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3157 2022-08-05 05:51:14.000000 plom-0.9.4/plom/idreader/assign_prob.py
+-rw-rw-rw-   0 root         (0) root         (0)     3217 2022-08-05 05:51:14.000000 plom-0.9.4/plom/idreader/model_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    10292 2022-08-05 05:51:14.000000 plom-0.9.4/plom/idreader/predictStudentID.py
+-rw-rw-rw-   0 root         (0) root         (0)     4683 2022-08-05 05:51:14.000000 plom-0.9.4/plom/idreader/test_IDreader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1768 2022-08-05 05:51:14.000000 plom-0.9.4/plom/idreader/trainRandomForestModel.py
+-rw-rw-rw-   0 root         (0) root         (0)     7476 2022-08-05 05:51:14.000000 plom-0.9.4/plom/latexTemplate.tex
+-rw-rw-rw-   0 root         (0) root         (0)     7475 2022-08-05 05:51:14.000000 plom-0.9.4/plom/latexTemplatev2.tex
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-05 05:51:22.004246 plom-0.9.4/plom/manager/
+-rw-rw-rw-   0 root         (0) root         (0)      425 2022-08-05 05:51:14.000000 plom-0.9.4/plom/manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2017 2022-08-05 05:51:14.000000 plom-0.9.4/plom/manager/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4809 2022-08-05 05:51:14.000000 plom-0.9.4/plom/manager/collideview.py
+-rw-rw-rw-   0 root         (0) root         (0)     1274 2022-08-05 05:51:14.000000 plom-0.9.4/plom/manager/discardview.py
+-rwxrwxrwx   0 root         (0) root         (0)   106236 2022-08-05 05:51:14.000000 plom-0.9.4/plom/manager/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     3512 2022-08-05 05:51:14.000000 plom-0.9.4/plom/manager/reviewview.py
+-rw-rw-rw-   0 root         (0) root         (0)     8065 2022-08-05 05:51:14.000000 plom-0.9.4/plom/manager/selectrectangle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-05 05:51:22.004246 plom-0.9.4/plom/manager/uiFiles/
+-rw-rw-rw-   0 root         (0) root         (0)       14 2022-08-05 05:51:14.000000 plom-0.9.4/plom/manager/uiFiles/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    77263 2022-08-05 05:51:14.000000 plom-0.9.4/plom/manager/uiFiles/ui_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)    10612 2022-08-05 05:51:14.000000 plom-0.9.4/plom/manager/unknownpageview.py
+-rw-rw-rw-   0 root         (0) root         (0)    63380 2022-08-05 05:51:14.000000 plom-0.9.4/plom/managerMessenger.py
+-rw-rw-rw-   0 root         (0) root         (0)    20270 2022-08-05 05:51:14.000000 plom-0.9.4/plom/messenger.py
+-rw-rw-rw-   0 root         (0) root         (0)     5718 2022-08-05 05:51:14.000000 plom-0.9.4/plom/misc_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3115 2022-08-05 05:51:14.000000 plom-0.9.4/plom/plom_exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2940 2022-08-05 05:51:14.000000 plom-0.9.4/plom/rules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-05 05:51:22.011247 plom-0.9.4/plom/scan/
+-rw-rw-rw-   0 root         (0) root         (0)     1094 2022-08-05 05:51:14.000000 plom-0.9.4/plom/scan/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8432 2022-08-05 05:51:14.000000 plom-0.9.4/plom/scan/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3905 2022-08-05 05:51:14.000000 plom-0.9.4/plom/scan/bundle_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4079 2022-08-05 05:51:14.000000 plom-0.9.4/plom/scan/checkScanStatus.py
+-rw-rw-rw-   0 root         (0) root         (0)      600 2022-08-05 05:51:14.000000 plom-0.9.4/plom/scan/clearScannerLogin.py
+-rw-rw-rw-   0 root         (0) root         (0)     4297 2022-08-05 05:51:14.000000 plom-0.9.4/plom/scan/fasterQRExtract.py
+-rw-rw-rw-   0 root         (0) root         (0)    11901 2022-08-05 05:51:14.000000 plom-0.9.4/plom/scan/frontend_hwscan.py
+-rw-rw-rw-   0 root         (0) root         (0)     9982 2022-08-05 05:51:14.000000 plom-0.9.4/plom/scan/frontend_scan.py
+-rw-rw-rw-   0 root         (0) root         (0)     4157 2022-08-05 05:51:14.000000 plom-0.9.4/plom/scan/hwSubmissionsCheck.py
+-rw-rw-rw-   0 root         (0) root         (0)     1049 2022-08-05 05:51:14.000000 plom-0.9.4/plom/scan/listBundles.py
+-rw-rw-rw-   0 root         (0) root         (0)    10196 2022-08-05 05:51:14.000000 plom-0.9.4/plom/scan/readQRCodes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2175 2022-08-05 05:51:14.000000 plom-0.9.4/plom/scan/rotate.py
+-rw-rw-rw-   0 root         (0) root         (0)    14545 2022-08-05 05:51:14.000000 plom-0.9.4/plom/scan/scansToImages.py
+-rw-rw-rw-   0 root         (0) root         (0)     5011 2022-08-05 05:51:14.000000 plom-0.9.4/plom/scan/sendCollisionsToServer.py
+-rw-rw-rw-   0 root         (0) root         (0)    10040 2022-08-05 05:51:14.000000 plom-0.9.4/plom/scan/sendPagesToServer.py
+-rw-rw-rw-   0 root         (0) root         (0)     4327 2022-08-05 05:51:14.000000 plom-0.9.4/plom/scan/sendUnknownsToServer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1776 2022-08-05 05:51:14.000000 plom-0.9.4/plom/scan/start_messenger.py
+-rw-rw-rw-   0 root         (0) root         (0)     2662 2022-08-05 05:51:14.000000 plom-0.9.4/plom/scan/test_pdf_img_extraction.py
+-rw-rw-rw-   0 root         (0) root         (0)     2610 2022-08-05 05:51:14.000000 plom-0.9.4/plom/scan/test_qr_reads.py
+-rw-rw-rw-   0 root         (0) root         (0)     2636 2022-08-05 05:51:14.000000 plom-0.9.4/plom/scan/test_question_map_parse.py
+-rw-rw-rw-   0 root         (0) root         (0)    84508 2022-08-05 05:51:14.000000 plom-0.9.4/plom/scan/test_zbar_fails.png
+-rw-rw-rw-   0 root         (0) root         (0)    17361 2022-08-05 05:51:14.000000 plom-0.9.4/plom/scanMessenger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-05 05:51:22.014248 plom-0.9.4/plom/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)      315 2022-08-05 05:51:14.000000 plom-0.9.4/plom/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      785 2022-08-05 05:51:14.000000 plom-0.9.4/plom/scripts/build_stub.py
+-rw-rw-rw-   0 root         (0) root         (0)     6843 2022-08-05 05:51:14.000000 plom-0.9.4/plom/scripts/demo.py
+-rw-rw-rw-   0 root         (0) root         (0)     7019 2022-08-05 05:51:14.000000 plom-0.9.4/plom/scripts/hwdemo.py
+-rw-rw-rw-   0 root         (0) root         (0)     8384 2022-08-05 05:51:14.000000 plom-0.9.4/plom/scripts/hwscan.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2022-08-05 05:51:14.000000 plom-0.9.4/plom/scripts/plominit.py
+-rw-rw-rw-   0 root         (0) root         (0)     1003 2022-08-05 05:51:14.000000 plom-0.9.4/plom/scripts/test_script_help_ver.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-05 05:51:22.020248 plom-0.9.4/plom/server/
+-rw-rw-rw-   0 root         (0) root         (0)     1019 2022-08-05 05:51:14.000000 plom-0.9.4/plom/server/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9964 2022-08-05 05:51:14.000000 plom-0.9.4/plom/server/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6493 2022-08-05 05:51:14.000000 plom-0.9.4/plom/server/authenticate.py
+-rw-rw-rw-   0 root         (0) root         (0)    11839 2022-08-05 05:51:14.000000 plom-0.9.4/plom/server/background.py
+-rw-rw-rw-   0 root         (0) root         (0)     1598 2022-08-05 05:51:14.000000 plom-0.9.4/plom/server/cert_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     7604 2022-08-05 05:51:14.000000 plom-0.9.4/plom/server/demo.py
+-rw-rw-rw-   0 root         (0) root         (0)     7818 2022-08-05 05:51:14.000000 plom-0.9.4/plom/server/manageUserFiles.py
+-rw-rw-rw-   0 root         (0) root         (0)     3187 2022-08-05 05:51:14.000000 plom-0.9.4/plom/server/misc.py
+-rwxrwxrwx   0 root         (0) root         (0)    10204 2022-08-05 05:51:14.000000 plom-0.9.4/plom/server/pageNotSubmitted.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-05 05:51:22.026249 plom-0.9.4/plom/server/plomServer/
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2022-08-05 05:51:14.000000 plom-0.9.4/plom/server/plomServer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    26935 2022-08-05 05:51:14.000000 plom-0.9.4/plom/server/plomServer/routesID.py
+-rw-rw-rw-   0 root         (0) root         (0)    34265 2022-08-05 05:51:14.000000 plom-0.9.4/plom/server/plomServer/routesMark.py
+-rw-rw-rw-   0 root         (0) root         (0)    21505 2022-08-05 05:51:14.000000 plom-0.9.4/plom/server/plomServer/routesReport.py
+-rw-rw-rw-   0 root         (0) root         (0)    14096 2022-08-05 05:51:14.000000 plom-0.9.4/plom/server/plomServer/routesRubric.py
+-rw-rw-rw-   0 root         (0) root         (0)     3587 2022-08-05 05:51:14.000000 plom-0.9.4/plom/server/plomServer/routesSolution.py
+-rw-rw-rw-   0 root         (0) root         (0)    42249 2022-08-05 05:51:14.000000 plom-0.9.4/plom/server/plomServer/routesUpload.py
+-rw-rw-rw-   0 root         (0) root         (0)     8716 2022-08-05 05:51:14.000000 plom-0.9.4/plom/server/plomServer/routesUserInit.py
+-rw-rw-rw-   0 root         (0) root         (0)     7186 2022-08-05 05:51:14.000000 plom-0.9.4/plom/server/plomServer/routeutils.py
+-rw-rw-rw-   0 root         (0) root         (0)    18745 2022-08-05 05:51:14.000000 plom-0.9.4/plom/server/plomServer/serverID.py
+-rw-rw-rw-   0 root         (0) root         (0)     9964 2022-08-05 05:51:14.000000 plom-0.9.4/plom/server/plomServer/serverMark.py
+-rw-rw-rw-   0 root         (0) root         (0)     1828 2022-08-05 05:51:14.000000 plom-0.9.4/plom/server/plomServer/serverReport.py
+-rw-rw-rw-   0 root         (0) root         (0)     2073 2022-08-05 05:51:14.000000 plom-0.9.4/plom/server/plomServer/serverRubric.py
+-rw-rw-rw-   0 root         (0) root         (0)     1947 2022-08-05 05:51:14.000000 plom-0.9.4/plom/server/plomServer/serverSolution.py
+-rw-rw-rw-   0 root         (0) root         (0)    16293 2022-08-05 05:51:14.000000 plom-0.9.4/plom/server/plomServer/serverUpload.py
+-rw-rw-rw-   0 root         (0) root         (0)     5634 2022-08-05 05:51:14.000000 plom-0.9.4/plom/server/plomServer/serverUserInit.py
+-rw-rw-rw-   0 root         (0) root         (0)     6069 2022-08-05 05:51:14.000000 plom-0.9.4/plom/server/prepare.py
+-rw-rw-rw-   0 root         (0) root         (0)     1630 2022-08-05 05:51:14.000000 plom-0.9.4/plom/server/run_the_predictor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1334 2022-08-05 05:51:14.000000 plom-0.9.4/plom/server/target_Q_latex_plom.png
+-rw-rw-rw-   0 root         (0) root         (0)      420 2022-08-05 05:51:14.000000 plom-0.9.4/plom/server/test_background.py
+-rw-rw-rw-   0 root         (0) root         (0)     1197 2022-08-05 05:51:14.000000 plom-0.9.4/plom/server/test_background_multiprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1046 2022-08-05 05:51:14.000000 plom-0.9.4/plom/server/test_background_subprocess.py
+-rw-rw-rw-   0 root         (0) root         (0)      984 2022-08-05 05:51:14.000000 plom-0.9.4/plom/server/test_configs.py
+-rw-rw-rw-   0 root         (0) root         (0)     8085 2022-08-05 05:51:14.000000 plom-0.9.4/plom/server/test_demo.py
+-rw-rw-rw-   0 root         (0) root         (0)      691 2022-08-05 05:51:14.000000 plom-0.9.4/plom/server/test_dirs.py
+-rw-rw-rw-   0 root         (0) root         (0)      539 2022-08-05 05:51:14.000000 plom-0.9.4/plom/server/test_ssl_selfsigned.py
+-rw-rw-rw-   0 root         (0) root         (0)    11520 2022-08-05 05:51:14.000000 plom-0.9.4/plom/server/theServer.py
+-rw-rw-rw-   0 root         (0) root         (0)      595 2022-08-05 05:51:14.000000 plom-0.9.4/plom/serverDetails.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-05 05:51:22.029249 plom-0.9.4/plom/solutions/
+-rw-rw-rw-   0 root         (0) root         (0)     1120 2022-08-05 05:51:14.000000 plom-0.9.4/plom/solutions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9228 2022-08-05 05:51:14.000000 plom-0.9.4/plom/solutions/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      598 2022-08-05 05:51:14.000000 plom-0.9.4/plom/solutions/checkSolutionStatus.py
+-rw-rw-rw-   0 root         (0) root         (0)     1021 2022-08-05 05:51:14.000000 plom-0.9.4/plom/solutions/deleteSolutionImage.py
+-rw-rw-rw-   0 root         (0) root         (0)     5317 2022-08-05 05:51:14.000000 plom-0.9.4/plom/solutions/extractSolutions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1006 2022-08-05 05:51:14.000000 plom-0.9.4/plom/solutions/getSolutionImage.py
+-rw-rw-rw-   0 root         (0) root         (0)      328 2022-08-05 05:51:14.000000 plom-0.9.4/plom/solutions/msgr_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2348 2022-08-05 05:51:14.000000 plom-0.9.4/plom/solutions/putSolutionImage.py
+-rw-rw-rw-   0 root         (0) root         (0)    27974 2022-08-05 05:51:14.000000 plom-0.9.4/plom/specVerifier.py
+-rw-rw-rw-   0 root         (0) root         (0)      661 2022-08-05 05:51:14.000000 plom-0.9.4/plom/templateSolutionSpec.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1712 2022-08-05 05:51:14.000000 plom-0.9.4/plom/templateTestSpec.toml
+-rw-rw-rw-   0 root         (0) root         (0)      115 2022-08-05 05:51:14.000000 plom-0.9.4/plom/templateUserList.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-05 05:51:22.036250 plom-0.9.4/plom/testTemplates/
+-rw-rw-rw-   0 root         (0) root         (0)     2131 2022-08-05 05:51:14.000000 plom-0.9.4/plom/testTemplates/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1383 2022-08-05 05:51:14.000000 plom-0.9.4/plom/testTemplates/dummy_left_staple.png
+-rw-rw-rw-   0 root         (0) root         (0)    12633 2022-08-05 05:51:14.000000 plom-0.9.4/plom/testTemplates/dummy_left_staple_red.png
+-rw-rw-rw-   0 root         (0) root         (0)      652 2022-08-05 05:51:14.000000 plom-0.9.4/plom/testTemplates/dummy_qr_code.png
+-rw-rw-rw-   0 root         (0) root         (0)    17894 2022-08-05 05:51:14.000000 plom-0.9.4/plom/testTemplates/dummy_qr_code_red.png
+-rw-rw-rw-   0 root         (0) root         (0)     2307 2022-08-05 05:51:14.000000 plom-0.9.4/plom/testTemplates/dummy_right_staple.png
+-rw-rw-rw-   0 root         (0) root         (0)    13933 2022-08-05 05:51:14.000000 plom-0.9.4/plom/testTemplates/dummy_right_staple_red.png
+-rw-rw-rw-   0 root         (0) root         (0)     2460 2022-08-05 05:51:14.000000 plom-0.9.4/plom/testTemplates/extraSheets.tex
+-rw-rw-rw-   0 root         (0) root         (0)     2378 2022-08-05 05:51:14.000000 plom-0.9.4/plom/testTemplates/extraSheets_noname.tex
+-rw-rw-rw-   0 root         (0) root         (0)      997 2022-08-05 05:51:14.000000 plom-0.9.4/plom/testTemplates/idBox-source.tex
+-rw-rw-rw-   0 root         (0) root         (0)    43340 2022-08-05 05:51:14.000000 plom-0.9.4/plom/testTemplates/idBox.eps
+-rw-rw-rw-   0 root         (0) root         (0)    13872 2022-08-05 05:51:14.000000 plom-0.9.4/plom/testTemplates/idBox.pdf
+-rw-rw-rw-   0 root         (0) root         (0)    35624 2022-08-05 05:51:14.000000 plom-0.9.4/plom/testTemplates/idBox.svg
+-rw-rw-rw-   0 root         (0) root         (0)      941 2022-08-05 05:51:14.000000 plom-0.9.4/plom/testTemplates/idBox2-source.tex
+-rw-rw-rw-   0 root         (0) root         (0)    29216 2022-08-05 05:51:14.000000 plom-0.9.4/plom/testTemplates/idBox2.eps
+-rw-rw-rw-   0 root         (0) root         (0)     9457 2022-08-05 05:51:14.000000 plom-0.9.4/plom/testTemplates/idBox2.pdf
+-rw-rw-rw-   0 root         (0) root         (0)    29857 2022-08-05 05:51:14.000000 plom-0.9.4/plom/testTemplates/idBox2.svg
+-rw-rw-rw-   0 root         (0) root         (0)     7537 2022-08-05 05:51:14.000000 plom-0.9.4/plom/testTemplates/latexTemplate.tex
+-rw-rw-rw-   0 root         (0) root         (0)     7536 2022-08-05 05:51:14.000000 plom-0.9.4/plom/testTemplates/latexTemplatev2.tex
+-rw-rw-rw-   0 root         (0) root         (0)     2411 2022-08-05 05:51:14.000000 plom-0.9.4/plom/testTemplates/mockplom.sty
+-rw-rw-rw-   0 root         (0) root         (0)      805 2022-08-05 05:51:14.000000 plom-0.9.4/plom/test_exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)      955 2022-08-05 05:51:14.000000 plom-0.9.4/plom/test_latex.py
+-rw-rw-rw-   0 root         (0) root         (0)     2659 2022-08-05 05:51:14.000000 plom-0.9.4/plom/test_latexfrag.py
+-rw-rw-rw-   0 root         (0) root         (0)      338 2022-08-05 05:51:14.000000 plom-0.9.4/plom/test_messengers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1093 2022-08-05 05:51:14.000000 plom-0.9.4/plom/test_misc_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     7636 2022-08-05 05:51:14.000000 plom-0.9.4/plom/test_spec.py
+-rw-rw-rw-   0 root         (0) root         (0)      124 2022-08-05 05:51:14.000000 plom-0.9.4/plom/test_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2935 2022-08-05 05:51:14.000000 plom-0.9.4/plom/test_version_maps.py
+-rw-rw-rw-   0 root         (0) root         (0)     5419 2022-08-05 05:51:14.000000 plom-0.9.4/plom/textools.py
+-rw-rw-rw-   0 root         (0) root         (0)     3683 2022-08-05 05:51:14.000000 plom-0.9.4/plom/tpv_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      197 2022-08-05 05:51:14.000000 plom-0.9.4/plom/version.py
+-rw-rw-rw-   0 root         (0) root         (0)     5153 2022-08-05 05:51:14.000000 plom-0.9.4/plom/version_maps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-05 05:51:21.945241 plom-0.9.4/plom.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2366 2022-08-05 05:51:21.000000 plom-0.9.4/plom.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9293 2022-08-05 05:51:21.000000 plom-0.9.4/plom.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-05 05:51:21.000000 plom-0.9.4/plom.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      496 2022-08-05 05:51:21.000000 plom-0.9.4/plom.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      316 2022-08-05 05:51:21.000000 plom-0.9.4/plom.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2022-08-05 05:51:21.000000 plom-0.9.4/plom.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      870 2022-08-05 05:51:14.000000 plom-0.9.4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      887 2022-08-05 05:51:14.000000 plom-0.9.4/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      656 2022-08-05 05:51:14.000000 plom-0.9.4/requirements.txt.client
+-rw-r--r--   0 root         (0) root         (0)       38 2022-08-05 05:51:22.037250 plom-0.9.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4823 2022-08-05 05:51:14.000000 plom-0.9.4/setup.py
```

### Comparing `plom-0.9.3/CHANGELOG.md` & `plom-0.9.4/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,21 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 
+## [0.9.4] - 2022-08-04
+
+### Fixed
+* Fix various Manager UI paper creation functions when using precompiled binaries.
+* Fix several Manager UI crashes.
+
+
 ## [0.9.3] - 2022-07-18
 
 ### Added
 * `plom-create` can manipulate tags.
 * Can tag while peeking at previously marked papers.
 
 ### Fixed
@@ -790,14 +797,15 @@
 
 
 ## 0.1.0 - 2019-06-26
 
 This is the first release of Plom, PaperLess Open Marking.
 
 
+[0.9.4]: https://gitlab.com/plom/plom/compare/v0.9.3...v0.9.4
 [0.9.3]: https://gitlab.com/plom/plom/compare/v0.9.2...v0.9.3
 [0.9.2]: https://gitlab.com/plom/plom/compare/v0.9.0...v0.9.2
 [0.9.0]: https://gitlab.com/plom/plom/compare/v0.8.11...v0.9.0
 [0.8.11]: https://gitlab.com/plom/plom/compare/v0.8.10...v0.8.11
 [0.8.10]: https://gitlab.com/plom/plom/compare/v0.8.8...v0.8.10
 [0.8.8]: https://gitlab.com/plom/plom/compare/v0.8.7...v0.8.8
 [0.8.7]: https://gitlab.com/plom/plom/compare/v0.8.6...v0.8.7
```

### Comparing `plom-0.9.3/CONTRIBUTORS` & `plom-0.9.4/CONTRIBUTORS`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/Dockerfile` & `plom-0.9.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/LICENSE.md` & `plom-0.9.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/MANIFEST.in` & `plom-0.9.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/PKG-INFO` & `plom-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plom
-Version: 0.9.3
+Version: 0.9.4
 Summary: Plom is Paperless Open Marking
 Home-page: https://plomgrading.org
 Author: Andrew Rechnitzer
 License: AGPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `plom-0.9.3/README.md` & `plom-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/contrib/plom-push-to-canvas.py` & `plom-0.9.4/contrib/plom-push-to-canvas.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/contrib/plom-return_codes_to_canvas_csv.py` & `plom-0.9.4/contrib/plom-return_codes_to_canvas_csv.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/contrib/plom-write_grades_to_canvas_csv.py` & `plom-0.9.4/contrib/plom-write_grades_to_canvas_csv.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/contrib/upload_hw_from_zip_of_jpegs.py` & `plom-0.9.4/contrib/upload_hw_from_zip_of_jpegs.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/org.plomgrading.PlomClient.desktop` & `plom-0.9.4/org.plomgrading.PlomClient.desktop`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/org.plomgrading.PlomClient.metainfo.xml` & `plom-0.9.4/org.plomgrading.PlomClient.metainfo.xml`

 * *Files 0% similar despite different names*

#### Comparing `plom-0.9.3/org.plomgrading.PlomClient.metainfo.xml` & `plom-0.9.4/org.plomgrading.PlomClient.metainfo.xml`

```diff
@@ -52,14 +52,15 @@
     <kudo>ModernToolkit</kudo>
   </kudos>
   <url type="homepage">https://plomgrading.org</url>
   <update_contact>devs@plomgrading.org</update_contact>
   <developer_name>Andrew Rechnitzer, Colin B. Macdonald, and others</developer_name>
   <content_rating type="oars-1.0"/>
   <releases>
+    <release date="2022-08-04" version="0.9.4"/>
     <release date="2022-07-18" version="0.9.3"/>
     <release date="2022-06-14" version="0.9.2"/>
     <release date="2022-05-25" version="0.9.0"/>
     <release date="2022-04-12" version="0.8.11"/>
     <release date="2022-03-27" version="0.8.10"/>
     <release date="2022-03-14" version="0.8.8"/>
     <release date="2022-03-02" version="0.8.7"/>
```

### Comparing `plom-0.9.3/org.plomgrading.PlomClient.png` & `plom-0.9.4/org.plomgrading.PlomClient.png`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/__init__.py` & `plom-0.9.4/plom/__init__.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/aliceBob.py` & `plom-0.9.4/plom/aliceBob.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/baseMessenger.py` & `plom-0.9.4/plom/baseMessenger.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/canvas/__init__.py` & `plom-0.9.4/plom/canvas/__init__.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/canvas/canvas_utils.py` & `plom-0.9.4/plom/canvas/canvas_utils.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/canvas/canvasapi_extensions.py` & `plom-0.9.4/plom/canvas/canvasapi_extensions.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/__init__.py` & `plom-0.9.4/plom/client/__init__.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/__main__.py` & `plom-0.9.4/plom/client/__main__.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/annotator.py` & `plom-0.9.4/plom/client/annotator.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/backGrid.py` & `plom-0.9.4/plom/client/backGrid.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/backGrid1.svg` & `plom-0.9.4/plom/client/backGrid1.svg`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/backGrid2.png` & `plom-0.9.4/plom/client/backGrid2.png`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/background_downloader.py` & `plom-0.9.4/plom/client/background_downloader.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/chooser.py` & `plom-0.9.4/plom/client/chooser.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/cursors/arrow.png` & `plom-0.9.4/plom/client/cursors/arrow.png`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/cursors/box.png` & `plom-0.9.4/plom/client/cursors/box.png`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/cursors/crop.png` & `plom-0.9.4/plom/client/cursors/crop.png`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/cursors/cross.png` & `plom-0.9.4/plom/client/cursors/cross.png`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/cursors/delete.png` & `plom-0.9.4/plom/client/cursors/delete.png`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/cursors/double_arrow.png` & `plom-0.9.4/plom/client/cursors/double_arrow.png`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/cursors/ellipse.png` & `plom-0.9.4/plom/client/cursors/ellipse.png`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/cursors/highlighter.png` & `plom-0.9.4/plom/client/cursors/highlighter.png`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/cursors/line.png` & `plom-0.9.4/plom/client/cursors/line.png`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/cursors/pen.png` & `plom-0.9.4/plom/client/cursors/pen.png`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/cursors/question_mark.png` & `plom-0.9.4/plom/client/cursors/question_mark.png`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/cursors/text-comment.png` & `plom-0.9.4/plom/client/cursors/text-comment.png`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/cursors/text-delta.png` & `plom-0.9.4/plom/client/cursors/text-delta.png`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/cursors/text.png` & `plom-0.9.4/plom/client/cursors/text.png`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/cursors/tick.png` & `plom-0.9.4/plom/client/cursors/tick.png`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/elastics.py` & `plom-0.9.4/plom/client/elastics.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/icons/comment.svg` & `plom-0.9.4/plom/client/icons/comment.svg`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/icons/comment_down.svg` & `plom-0.9.4/plom/client/icons/comment_down.svg`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/icons/comment_up.svg` & `plom-0.9.4/plom/client/icons/comment_up.svg`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/icons/cross.svg` & `plom-0.9.4/plom/client/icons/cross.svg`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/icons/delete.svg` & `plom-0.9.4/plom/client/icons/delete.svg`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/icons/delta.svg` & `plom-0.9.4/plom/client/icons/delta.svg`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/icons/line.svg` & `plom-0.9.4/plom/client/icons/line.svg`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/icons/manager_collide.svg` & `plom-0.9.4/plom/client/icons/manager_collide.svg`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/icons/manager_discard.svg` & `plom-0.9.4/plom/client/icons/manager_discard.svg`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/icons/manager_extra.svg` & `plom-0.9.4/plom/client/icons/manager_extra.svg`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/icons/manager_hw.svg` & `plom-0.9.4/plom/client/icons/manager_hw.svg`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/icons/manager_move.svg` & `plom-0.9.4/plom/client/icons/manager_move.svg`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/icons/manager_none.svg` & `plom-0.9.4/plom/client/icons/manager_none.svg`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/icons/manager_test.svg` & `plom-0.9.4/plom/client/icons/manager_test.svg`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/icons/manager_unknown.svg` & `plom-0.9.4/plom/client/icons/manager_unknown.svg`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/icons/move.svg` & `plom-0.9.4/plom/client/icons/move.svg`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/icons/pan.svg` & `plom-0.9.4/plom/client/icons/pan.svg`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/icons/pen.svg` & `plom-0.9.4/plom/client/icons/pen.svg`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/icons/rectangle.svg` & `plom-0.9.4/plom/client/icons/rectangle.svg`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/icons/rectangle_highlight.svg` & `plom-0.9.4/plom/client/icons/rectangle_highlight.svg`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/icons/redo.svg` & `plom-0.9.4/plom/client/icons/redo.svg`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/icons/text.svg` & `plom-0.9.4/plom/client/icons/text.svg`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/icons/tick.svg` & `plom-0.9.4/plom/client/icons/tick.svg`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/icons/undo.svg` & `plom-0.9.4/plom/client/icons/undo.svg`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/icons/zoom.svg` & `plom-0.9.4/plom/client/icons/zoom.svg`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/icons/zoom_in.svg` & `plom-0.9.4/plom/client/icons/zoom_in.svg`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/icons/zoom_out.svg` & `plom-0.9.4/plom/client/icons/zoom_out.svg`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/identifier.py` & `plom-0.9.4/plom/client/identifier.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/image_view_widget.py` & `plom-0.9.4/plom/client/image_view_widget.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/key_help.py` & `plom-0.9.4/plom/client/key_help.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/key_wrangler.py` & `plom-0.9.4/plom/client/key_wrangler.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/marker.py` & `plom-0.9.4/plom/client/marker.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/pagecache.py` & `plom-0.9.4/plom/client/pagecache.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/pagerearranger.py` & `plom-0.9.4/plom/client/pagerearranger.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/pagescene.py` & `plom-0.9.4/plom/client/pagescene.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/pageview.py` & `plom-0.9.4/plom/client/pageview.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/randoIDer.py` & `plom-0.9.4/plom/client/randoIDer.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/randoMarker.py` & `plom-0.9.4/plom/client/randoMarker.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/random_identifying_utils.py` & `plom-0.9.4/plom/client/random_identifying_utils.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/random_marking_utils.py` & `plom-0.9.4/plom/client/random_marking_utils.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/rubric_list.py` & `plom-0.9.4/plom/client/rubric_list.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/rubric_wrangler.py` & `plom-0.9.4/plom/client/rubric_wrangler.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/tools/__init__.py` & `plom-0.9.4/plom/client/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/tools/arrow.py` & `plom-0.9.4/plom/client/tools/arrow.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/tools/box.py` & `plom-0.9.4/plom/client/tools/box.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/tools/crop.py` & `plom-0.9.4/plom/client/tools/crop.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/tools/cross.py` & `plom-0.9.4/plom/client/tools/cross.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/tools/delete.py` & `plom-0.9.4/plom/client/tools/delete.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/tools/delta.py` & `plom-0.9.4/plom/client/tools/delta.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/tools/ellipse.py` & `plom-0.9.4/plom/client/tools/ellipse.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/tools/highlight.py` & `plom-0.9.4/plom/client/tools/highlight.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/tools/image.py` & `plom-0.9.4/plom/client/tools/image.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/tools/line.py` & `plom-0.9.4/plom/client/tools/line.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/tools/move.py` & `plom-0.9.4/plom/client/tools/move.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/tools/pen.py` & `plom-0.9.4/plom/client/tools/pen.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/tools/penArrow.py` & `plom-0.9.4/plom/client/tools/penArrow.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/tools/questionMark.py` & `plom-0.9.4/plom/client/tools/questionMark.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/tools/rubric.py` & `plom-0.9.4/plom/client/tools/rubric.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/tools/text.py` & `plom-0.9.4/plom/client/tools/text.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/tools/tick.py` & `plom-0.9.4/plom/client/tools/tick.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/tools/tool.py` & `plom-0.9.4/plom/client/tools/tool.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/uiFiles/ui_annotator.py` & `plom-0.9.4/plom/client/uiFiles/ui_annotator.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/uiFiles/ui_chooser.py` & `plom-0.9.4/plom/client/uiFiles/ui_chooser.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/uiFiles/ui_identify.py` & `plom-0.9.4/plom/client/uiFiles/ui_identify.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/uiFiles/ui_iic.py` & `plom-0.9.4/plom/client/uiFiles/ui_iic.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/uiFiles/ui_marker.py` & `plom-0.9.4/plom/client/uiFiles/ui_marker.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/uiFiles/ui_totaler.py` & `plom-0.9.4/plom/client/uiFiles/ui_totaler.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/useful_classes.py` & `plom-0.9.4/plom/client/useful_classes.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/client/viewers.py` & `plom-0.9.4/plom/client/viewers.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/comment_utils.py` & `plom-0.9.4/plom/comment_utils.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/create/__init__.py` & `plom-0.9.4/plom/create/__init__.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/create/__main__.py` & `plom-0.9.4/plom/create/__main__.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/create/_digitHunter.py` & `plom-0.9.4/plom/create/_digitHunter.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/create/buildClasslist.py` & `plom-0.9.4/plom/create/buildClasslist.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/create/buildDatabaseAndPapers.py` & `plom-0.9.4/plom/create/buildDatabaseAndPapers.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
             box for prenamed papers.  None for a default value.
 
     Raises:
         PlomConflict: server does not yet have a version map database, say
             b/c build_database has not yet been called.
         ValueError: not enough papers for prenamed, indexToMake out of range,
             maybe other cases.
+        fitz.FileNotFoundError/RuntimeError: source PDF files not found.
 
     We try to get a classlist from the server to prename any papers
     where the `paper_number` is specified.  If the server does not yet
     have a classlist, we create no prenamed papers.
     """
     basedir = Path(basedir)
     paperdir = basedir / paperdir_name
```

### Comparing `plom-0.9.3/plom/create/buildNamedPDF.py` & `plom-0.9.4/plom/create/buildNamedPDF.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/create/classlistValidator.py` & `plom-0.9.4/plom/create/classlistValidator.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/create/demotools.py` & `plom-0.9.4/plom/create/demotools.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/create/digits.json` & `plom-0.9.4/plom/create/digits.json`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/create/exam_scribbler.py` & `plom-0.9.4/plom/create/exam_scribbler.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/create/fonts/ejx_handwriting.ttf` & `plom-0.9.4/plom/create/fonts/ejx_handwriting.ttf`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/create/homework_scribbler.py` & `plom-0.9.4/plom/create/homework_scribbler.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/create/mergeAndCodePages.py` & `plom-0.9.4/plom/create/mergeAndCodePages.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/create/push_pull_rubrics.py` & `plom-0.9.4/plom/create/push_pull_rubrics.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/create/scribble_hw_utils.py` & `plom-0.9.4/plom/create/scribble_hw_utils.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/create/scribble_utils.py` & `plom-0.9.4/plom/create/scribble_utils.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/create/start_messenger.py` & `plom-0.9.4/plom/create/start_messenger.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/create/status.py` & `plom-0.9.4/plom/create/status.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/create/test_build_source_exams.py` & `plom-0.9.4/plom/create/test_build_source_exams.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/create/test_classlists.py` & `plom-0.9.4/plom/create/test_classlists.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/create/test_stamps.py` & `plom-0.9.4/plom/create/test_stamps.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/create/test_upload_classlist.py` & `plom-0.9.4/plom/create/test_upload_classlist.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/create/upload_classlist.py` & `plom-0.9.4/plom/create/upload_classlist.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/create/version_map_utils.py` & `plom-0.9.4/plom/create/version_map_utils.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/db/buildPlomDB.py` & `plom-0.9.4/plom/db/buildPlomDB.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/db/db_create.py` & `plom-0.9.4/plom/db/db_create.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/db/db_identify.py` & `plom-0.9.4/plom/db/db_identify.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/db/db_manage.py` & `plom-0.9.4/plom/db/db_manage.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/db/db_mark.py` & `plom-0.9.4/plom/db/db_mark.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/db/db_report.py` & `plom-0.9.4/plom/db/db_report.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/db/db_rubric.py` & `plom-0.9.4/plom/db/db_rubric.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/db/db_upload.py` & `plom-0.9.4/plom/db/db_upload.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/db/db_user.py` & `plom-0.9.4/plom/db/db_user.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/db/examDB.py` & `plom-0.9.4/plom/db/examDB.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/db/tables.py` & `plom-0.9.4/plom/db/tables.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/demoClassList.csv` & `plom-0.9.4/plom/demoClassList.csv`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/demo_rubrics.toml` & `plom-0.9.4/plom/demo_rubrics.toml`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/finish/__init__.py` & `plom-0.9.4/plom/finish/__init__.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/finish/__main__.py` & `plom-0.9.4/plom/finish/__main__.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/finish/assemble_solutions.py` & `plom-0.9.4/plom/finish/assemble_solutions.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/finish/audit.py` & `plom-0.9.4/plom/finish/audit.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/finish/check_completed.py` & `plom-0.9.4/plom/finish/check_completed.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/finish/clear_manager_login.py` & `plom-0.9.4/plom/finish/clear_manager_login.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/finish/coded_return.py` & `plom-0.9.4/plom/finish/coded_return.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/finish/coverPageBuilder.py` & `plom-0.9.4/plom/finish/coverPageBuilder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,48 +1,50 @@
 # SPDX-License-Identifier: AGPL-3.0-or-later
 # Copyright (C) 2018-2022 Andrew Rechnitzer
 # Copyright (C) 2018 Elvis Cai
-# Copyright (C) 2019-2020 Colin B. Macdonald
+# Copyright (C) 2019-2020, 2022 Colin B. Macdonald
 # Copyright (C) 2020 Dryden Wiebe
 # Copyright (C) 2021 Liam Yih
 
-from weasyprint import HTML, CSS
 from plom.misc_utils import local_now_to_simple_string
 
-# A simple CSS header to style the cover page nicely.
-css = CSS(
-    string="""
+
+def makeCover(test_num, sname, sid, tab, pdfname, solution=False):
+    """Create html page of name ID etc and table of marks.
+
+    Args:
+        test_num (int): the test number for the test we are making the cover for.
+        sname (str): student name.
+        sid (str): student id.
+        tab (list): information about the test that should be put on the coverpage.
+        pdfname (pathlib.Path): filename to save the pdf into
+        solution (bool): whether or not this is a cover page for solutions
+    """
+    # hide imports until needed Issue #2231.
+    from weasyprint import HTML, CSS
+
+    # A simple CSS header to style the cover page nicely.
+    css = CSS(
+        string="""
 @page {
   size: Letter; /* Change from the default size of A4 */
   margin: 2.5cm; /* Set margin on each page */
 }
 body {
     font-family: sans serif;
 }
 table, th, td {
     border: 1px solid black;
     border-collapse: collapse;
     padding: 5px;
     text-align: center;
 }
 """
-)
+    )
 
-
-def makeCover(test_num, sname, sid, tab, pdfname, solution=False):
-    """Create html page of name ID etc and table of marks.
-
-    Args:
-        test_num (int): the test number for the test we are making the cover for.
-        sname (str): student name.
-        sid (str): student id.
-        tab (list): information about the test that should be put on the coverpage.
-        pdfname (pathlib.Path): filename to save the pdf into
-        solution (bool): whether or not this is a cover page for solutions
-    """
     htmlText = "<html><body>\n"
     if solution:
         htmlText += "<h3>Solutions</h3>\n"
     else:
         htmlText += "<h3>Results</h3>\n"
     htmlText += """
 <ul>
```

### Comparing `plom-0.9.3/plom/finish/examReassembler.py` & `plom-0.9.4/plom/finish/examReassembler.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/finish/html_view_test_template.py` & `plom-0.9.4/plom/finish/html_view_test_template.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/finish/reassemble_ID_only.py` & `plom-0.9.4/plom/finish/reassemble_ID_only.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/finish/reassemble_completed.py` & `plom-0.9.4/plom/finish/reassemble_completed.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/finish/return_tools.py` & `plom-0.9.4/plom/finish/return_tools.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/finish/rubric_downloads.py` & `plom-0.9.4/plom/finish/rubric_downloads.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/finish/solutionAssembler.py` & `plom-0.9.4/plom/finish/solutionAssembler.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/finish/spreadsheet.py` & `plom-0.9.4/plom/finish/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/finish/start_messenger.py` & `plom-0.9.4/plom/finish/start_messenger.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/finish/test_hash.py` & `plom-0.9.4/plom/finish/test_hash.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/finish/test_return_tools.py` & `plom-0.9.4/plom/finish/test_return_tools.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/finish/utils.py` & `plom-0.9.4/plom/finish/utils.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/finishMessenger.py` & `plom-0.9.4/plom/finishMessenger.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/idBox2.pdf` & `plom-0.9.4/plom/idBox2.pdf`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/idreader/__init__.py` & `plom-0.9.4/plom/idreader/__init__.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/idreader/assign_prob.py` & `plom-0.9.4/plom/idreader/assign_prob.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/idreader/model_utils.py` & `plom-0.9.4/plom/idreader/model_utils.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/idreader/predictStudentID.py` & `plom-0.9.4/plom/idreader/predictStudentID.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/idreader/test_IDreader.py` & `plom-0.9.4/plom/idreader/test_IDreader.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/idreader/trainRandomForestModel.py` & `plom-0.9.4/plom/idreader/trainRandomForestModel.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/latexTemplate.tex` & `plom-0.9.4/plom/latexTemplate.tex`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/latexTemplatev2.tex` & `plom-0.9.4/plom/latexTemplatev2.tex`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/manager/__main__.py` & `plom-0.9.4/plom/manager/__main__.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/manager/collideview.py` & `plom-0.9.4/plom/manager/collideview.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/manager/discardview.py` & `plom-0.9.4/plom/manager/discardview.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/manager/manager.py` & `plom-0.9.4/plom/manager/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -751,15 +751,22 @@
                 fakepdf=False,
                 no_qr=False,
                 indexToMake=which,
                 xcoord=xpos,
                 ycoord=ypos,
                 msgr=self.msgr,
             )
-        except (PlomServerNotReady, PlomConflict, OSError) as e:
+        except (
+            PlomServerNotReady,
+            PlomConflict,
+            OSError,
+            RuntimeError,
+            ValueError,
+        ) as e:
+            # fitz.FileNotFoundError is a subclass of RuntimeError
             self.Qapp.restoreOverrideCursor()
             WarnMsg(self, "Could not build papers.", info=e).exec()
         self.Qapp.restoreOverrideCursor()
         self.setEnabled(True)
 
     ################
     # scan tab stuff
```

### Comparing `plom-0.9.3/plom/manager/reviewview.py` & `plom-0.9.4/plom/manager/reviewview.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/manager/selectrectangle.py` & `plom-0.9.4/plom/manager/selectrectangle.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/manager/uiFiles/ui_manager.py` & `plom-0.9.4/plom/manager/uiFiles/ui_manager.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/manager/unknownpageview.py` & `plom-0.9.4/plom/manager/unknownpageview.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/managerMessenger.py` & `plom-0.9.4/plom/managerMessenger.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/messenger.py` & `plom-0.9.4/plom/messenger.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/misc_utils.py` & `plom-0.9.4/plom/misc_utils.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/plom_exceptions.py` & `plom-0.9.4/plom/plom_exceptions.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/rules.py` & `plom-0.9.4/plom/rules.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/scan/__init__.py` & `plom-0.9.4/plom/scan/__init__.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/scan/__main__.py` & `plom-0.9.4/plom/scan/__main__.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/scan/bundle_utils.py` & `plom-0.9.4/plom/scan/bundle_utils.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/scan/checkScanStatus.py` & `plom-0.9.4/plom/scan/checkScanStatus.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/scan/clearScannerLogin.py` & `plom-0.9.4/plom/scan/clearScannerLogin.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/scan/fasterQRExtract.py` & `plom-0.9.4/plom/scan/fasterQRExtract.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/scan/frontend_hwscan.py` & `plom-0.9.4/plom/scan/frontend_hwscan.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/scan/frontend_scan.py` & `plom-0.9.4/plom/scan/frontend_scan.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/scan/hwSubmissionsCheck.py` & `plom-0.9.4/plom/scan/hwSubmissionsCheck.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/scan/listBundles.py` & `plom-0.9.4/plom/scan/listBundles.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/scan/readQRCodes.py` & `plom-0.9.4/plom/scan/readQRCodes.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/scan/rotate.py` & `plom-0.9.4/plom/scan/rotate.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/scan/scansToImages.py` & `plom-0.9.4/plom/scan/scansToImages.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/scan/sendCollisionsToServer.py` & `plom-0.9.4/plom/scan/sendCollisionsToServer.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/scan/sendPagesToServer.py` & `plom-0.9.4/plom/scan/sendPagesToServer.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/scan/sendUnknownsToServer.py` & `plom-0.9.4/plom/scan/sendUnknownsToServer.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/scan/start_messenger.py` & `plom-0.9.4/plom/scan/start_messenger.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/scan/test_pdf_img_extraction.py` & `plom-0.9.4/plom/scan/test_pdf_img_extraction.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/scan/test_qr_reads.py` & `plom-0.9.4/plom/scan/test_qr_reads.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/scan/test_question_map_parse.py` & `plom-0.9.4/plom/scan/test_question_map_parse.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/scan/test_zbar_fails.png` & `plom-0.9.4/plom/scan/test_zbar_fails.png`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/scanMessenger.py` & `plom-0.9.4/plom/scanMessenger.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/scripts/build_stub.py` & `plom-0.9.4/plom/scripts/build_stub.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/scripts/demo.py` & `plom-0.9.4/plom/scripts/demo.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/scripts/hwdemo.py` & `plom-0.9.4/plom/scripts/hwdemo.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/scripts/hwscan.py` & `plom-0.9.4/plom/scripts/hwscan.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/scripts/plominit.py` & `plom-0.9.4/plom/scripts/plominit.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/scripts/test_script_help_ver.py` & `plom-0.9.4/plom/scripts/test_script_help_ver.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/server/__init__.py` & `plom-0.9.4/plom/server/__init__.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/server/__main__.py` & `plom-0.9.4/plom/server/__main__.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/server/authenticate.py` & `plom-0.9.4/plom/server/authenticate.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/server/background.py` & `plom-0.9.4/plom/server/background.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/server/cert_utils.py` & `plom-0.9.4/plom/server/cert_utils.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/server/demo.py` & `plom-0.9.4/plom/server/demo.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/server/manageUserFiles.py` & `plom-0.9.4/plom/server/manageUserFiles.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/server/misc.py` & `plom-0.9.4/plom/server/misc.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/server/pageNotSubmitted.py` & `plom-0.9.4/plom/server/pageNotSubmitted.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/server/plomServer/__init__.py` & `plom-0.9.4/plom/server/plomServer/__init__.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/server/plomServer/routesID.py` & `plom-0.9.4/plom/server/plomServer/routesID.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/server/plomServer/routesMark.py` & `plom-0.9.4/plom/server/plomServer/routesMark.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/server/plomServer/routesReport.py` & `plom-0.9.4/plom/server/plomServer/routesReport.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/server/plomServer/routesRubric.py` & `plom-0.9.4/plom/server/plomServer/routesRubric.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/server/plomServer/routesSolution.py` & `plom-0.9.4/plom/server/plomServer/routesSolution.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/server/plomServer/routesUpload.py` & `plom-0.9.4/plom/server/plomServer/routesUpload.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/server/plomServer/routesUserInit.py` & `plom-0.9.4/plom/server/plomServer/routesUserInit.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/server/plomServer/routeutils.py` & `plom-0.9.4/plom/server/plomServer/routeutils.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/server/plomServer/serverID.py` & `plom-0.9.4/plom/server/plomServer/serverID.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/server/plomServer/serverMark.py` & `plom-0.9.4/plom/server/plomServer/serverMark.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/server/plomServer/serverReport.py` & `plom-0.9.4/plom/server/plomServer/serverReport.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/server/plomServer/serverRubric.py` & `plom-0.9.4/plom/server/plomServer/serverRubric.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/server/plomServer/serverSolution.py` & `plom-0.9.4/plom/server/plomServer/serverSolution.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/server/plomServer/serverUpload.py` & `plom-0.9.4/plom/server/plomServer/serverUpload.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/server/plomServer/serverUserInit.py` & `plom-0.9.4/plom/server/plomServer/serverUserInit.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/server/prepare.py` & `plom-0.9.4/plom/server/prepare.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/server/run_the_predictor.py` & `plom-0.9.4/plom/server/run_the_predictor.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/server/target_Q_latex_plom.png` & `plom-0.9.4/plom/server/target_Q_latex_plom.png`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/server/test_background_multiprocessing.py` & `plom-0.9.4/plom/server/test_background_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/server/test_background_subprocess.py` & `plom-0.9.4/plom/server/test_background_subprocess.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/server/test_configs.py` & `plom-0.9.4/plom/server/test_configs.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/server/test_demo.py` & `plom-0.9.4/plom/server/test_demo.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/server/test_dirs.py` & `plom-0.9.4/plom/server/test_dirs.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/server/test_ssl_selfsigned.py` & `plom-0.9.4/plom/server/test_ssl_selfsigned.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/server/theServer.py` & `plom-0.9.4/plom/server/theServer.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/serverDetails.toml` & `plom-0.9.4/plom/serverDetails.toml`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/solutions/__init__.py` & `plom-0.9.4/plom/solutions/__init__.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/solutions/__main__.py` & `plom-0.9.4/plom/solutions/__main__.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/solutions/checkSolutionStatus.py` & `plom-0.9.4/plom/solutions/checkSolutionStatus.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/solutions/deleteSolutionImage.py` & `plom-0.9.4/plom/solutions/deleteSolutionImage.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/solutions/extractSolutions.py` & `plom-0.9.4/plom/solutions/extractSolutions.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/solutions/getSolutionImage.py` & `plom-0.9.4/plom/solutions/getSolutionImage.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/solutions/putSolutionImage.py` & `plom-0.9.4/plom/solutions/putSolutionImage.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/specVerifier.py` & `plom-0.9.4/plom/specVerifier.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/templateSolutionSpec.toml` & `plom-0.9.4/plom/templateSolutionSpec.toml`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/templateTestSpec.toml` & `plom-0.9.4/plom/templateTestSpec.toml`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/testTemplates/README.md` & `plom-0.9.4/plom/testTemplates/README.md`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/testTemplates/dummy_left_staple.png` & `plom-0.9.4/plom/testTemplates/dummy_left_staple.png`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/testTemplates/dummy_left_staple_red.png` & `plom-0.9.4/plom/testTemplates/dummy_left_staple_red.png`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/testTemplates/dummy_qr_code.png` & `plom-0.9.4/plom/testTemplates/dummy_qr_code.png`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/testTemplates/dummy_qr_code_red.png` & `plom-0.9.4/plom/testTemplates/dummy_qr_code_red.png`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/testTemplates/dummy_right_staple.png` & `plom-0.9.4/plom/testTemplates/dummy_right_staple.png`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/testTemplates/dummy_right_staple_red.png` & `plom-0.9.4/plom/testTemplates/dummy_right_staple_red.png`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/testTemplates/extraSheets.tex` & `plom-0.9.4/plom/testTemplates/extraSheets.tex`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/testTemplates/extraSheets_noname.tex` & `plom-0.9.4/plom/testTemplates/extraSheets_noname.tex`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/testTemplates/idBox-source.tex` & `plom-0.9.4/plom/testTemplates/idBox-source.tex`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/testTemplates/idBox.eps` & `plom-0.9.4/plom/testTemplates/idBox.eps`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/testTemplates/idBox.pdf` & `plom-0.9.4/plom/testTemplates/idBox.pdf`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/testTemplates/idBox.svg` & `plom-0.9.4/plom/testTemplates/idBox.svg`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/testTemplates/idBox2-source.tex` & `plom-0.9.4/plom/testTemplates/idBox2-source.tex`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/testTemplates/idBox2.eps` & `plom-0.9.4/plom/testTemplates/idBox2.eps`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/testTemplates/idBox2.pdf` & `plom-0.9.4/plom/testTemplates/idBox2.pdf`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/testTemplates/idBox2.svg` & `plom-0.9.4/plom/testTemplates/idBox2.svg`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/testTemplates/latexTemplate.tex` & `plom-0.9.4/plom/testTemplates/latexTemplate.tex`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/testTemplates/latexTemplatev2.tex` & `plom-0.9.4/plom/testTemplates/latexTemplatev2.tex`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/testTemplates/mockplom.sty` & `plom-0.9.4/plom/testTemplates/mockplom.sty`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/test_exceptions.py` & `plom-0.9.4/plom/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/test_latex.py` & `plom-0.9.4/plom/test_latex.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/test_latexfrag.py` & `plom-0.9.4/plom/test_latexfrag.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/test_misc_utils.py` & `plom-0.9.4/plom/test_misc_utils.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/test_spec.py` & `plom-0.9.4/plom/test_spec.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/test_version_maps.py` & `plom-0.9.4/plom/test_version_maps.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/textools.py` & `plom-0.9.4/plom/textools.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/tpv_utils.py` & `plom-0.9.4/plom/tpv_utils.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom/version_maps.py` & `plom-0.9.4/plom/version_maps.py`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/plom.egg-info/PKG-INFO` & `plom-0.9.4/plom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plom
-Version: 0.9.3
+Version: 0.9.4
 Summary: Plom is Paperless Open Marking
 Home-page: https://plomgrading.org
 Author: Andrew Rechnitzer
 License: AGPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `plom-0.9.3/plom.egg-info/SOURCES.txt` & `plom-0.9.4/plom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/pyproject.toml` & `plom-0.9.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plom-0.9.3/requirements.txt` & `plom-0.9.4/requirements.txt`

 * *Files 11% similar despite different names*

```diff
@@ -33,9 +33,9 @@
 requests==2.28.1
 requests-toolbelt==0.9.1
 scikit-learn==1.1.1
 segno==1.5.2
 stdiomask==0.0.6
 toml==0.10.2
 tqdm==4.64.0
-urllib3==1.26.10
-weasyprint==56.0
+urllib3==1.26.11
+weasyprint==56.1
```

### Comparing `plom-0.9.3/requirements.txt.client` & `plom-0.9.4/requirements.txt.client`

 * *Files 15% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 # without any warranty.
 
 # These should be kept lock-step with `requirements.txt`
 PyQt5==5.15.7
 PyQt5-sip==12.11.0
 appdirs==1.4.4
 arrow==1.2.2
+exif==1.3.5
 packaging==21.3
 passlib==1.7.4
 Pillow==9.2.0
 pymupdf==1.20.1
 requests==2.28.1
 requests-toolbelt==0.9.1
 segno==1.5.2
 stdiomask==0.0.6
 toml==0.10.2
 tqdm==4.64.0
-urllib3==1.26.10
+urllib3==1.26.11
```

### Comparing `plom-0.9.3/setup.py` & `plom-0.9.4/setup.py`

 * *Files identical despite different names*

