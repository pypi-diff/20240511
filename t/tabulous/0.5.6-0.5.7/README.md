# Comparing `tmp/tabulous-0.5.6.tar.gz` & `tmp/tabulous-0.5.7.tar.gz`

## Comparing `tabulous-0.5.6.tar` & `tabulous-0.5.7.tar`

### file list

```diff
@@ -1,217 +1,217 @@
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/__init__.py
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/__main__.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_async_importer.py
--rw-r--r--   0        0        0     5310 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_colormap.py
--rw-r--r--   0        0        0    11502 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_dtype.py
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_fetch_and_install.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_io.py
--rw-r--r--   0        0        0     6407 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_ipython.py
--rw-r--r--   0        0        0     8796 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_map_model.py
--rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_pd_index.py
--rw-r--r--   0        0        0    11539 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_range.py
--rw-r--r--   0        0        0    13505 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_selection_model.py
--rw-r--r--   0        0        0    15630 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_selection_op.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_slice_op.py
--rw-r--r--   0        0        0    18522 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_sort_filter_proxy.py
--rw-r--r--   0        0        0    15100 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_text_formatter.py
--rw-r--r--   0        0        0    10351 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_utils.py
--rw-r--r--   0        0        0    13695 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/color.py
--rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/core.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/exceptions.py
--rw-r--r--   0        0        0     6494 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/post_init.py
--rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/threading.py
--rw-r--r--   0        0        0     5260 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/types.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_keymap/__init__.py
--rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_keymap/_callback.py
--rw-r--r--   0        0        0    22386 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_keymap/_keymap_objects.py
--rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_keymap/_keymapview.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_magicgui/__init__.py
--rw-r--r--   0        0        0     5175 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_magicgui/_color_edit.py
--rw-r--r--   0        0        0     5034 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_magicgui/_dialog.py
--rw-r--r--   0        0        0     8402 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_magicgui/_register.py
--rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_magicgui/_selection.py
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_magicgui/_table.py
--rw-r--r--   0        0        0     7798 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_magicgui/_timedelta.py
--rw-r--r--   0        0        0    10017 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_magicgui/_toggle_switch.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_psygnal/__init__.py
--rw-r--r--   0        0        0    13624 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_psygnal/_array.py
--rw-r--r--   0        0        0    33079 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_psygnal/_psygnal_compat.py
--rw-r--r--   0        0        0    23939 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_psygnal/_slots.py
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_psygnal/_special_objects.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/__init__.py
--rw-r--r--   0        0        0     4510 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_action_registry.py
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_app.py
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_clickable_label.py
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_dockwidget.py
--rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_filetree.py
--rw-r--r--   0        0        0     4692 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_history.py
--rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_jump.py
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_multitips.py
--rw-r--r--   0        0        0     5836 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_progress.py
--rw-r--r--   0        0        0    13892 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_proxy_button.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_qt_const.py
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_svg.py
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_titlebar.py
--rw-r--r--   0        0        0    11639 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_traceback.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_tree_header.py
--rw-r--r--   0        0        0     4717 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_undo.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_console/__init__.py
--rw-r--r--   0        0        0    11936 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_console/_widget.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/barplot.svg
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/boxenplot.svg
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/boxplot.svg
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/column_filter.svg
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/copy.svg
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/copy_as_spreadsheet.svg
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/copy_as_table.svg
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/cut.svg
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/eval.svg
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/filter.svg
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/find_item.svg
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/groupby.svg
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/hist.svg
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/melt.svg
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/more.svg
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/new_figure.svg
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/new_spreadsheet.svg
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/open_sample.svg
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/open_spreadsheet.svg
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/open_table.svg
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/optimize.svg
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/palette.svg
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/paste.svg
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/pivot.svg
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/plot.svg
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/preferences.svg
--rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/random.svg
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/redo.svg
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/restore_columns.svg
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/round.svg
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/save_table.svg
--rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/scatter.svg
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/settings.svg
--rw-r--r--   0        0        0     3472 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/sklearn_analysis.svg
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/sort_table.svg
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/stats_test.svg
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/summarize_table.svg
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/swarmplot.svg
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/switch_header.svg
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/switch_layout.svg
--rw-r--r--   0        0        0    67646 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/tabulous.ico
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/tile.svg
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/toggle_console.svg
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/trash_bin.svg
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/trash_bin_opened.svg
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/undo.svg
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/untile.svg
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/view_dual_h.svg
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/view_dual_v.svg
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/view_popup.svg
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/view_reset.svg
--rw-r--r--   0        0        0    12285 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_icons/window_icon.png
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_mainwindow/__init__.py
--rw-r--r--   0        0        0     9224 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_mainwindow/_base.py
--rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_mainwindow/_command_palette.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_mainwindow/_keycombo.py
--rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_mainwindow/_mainwidgets.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_mainwindow/_namespace.py
--rw-r--r--   0        0        0     5024 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_mainwindow/_titlebar.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_plot/__init__.py
--rw-r--r--   0        0        0    15100 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_plot/_artist_editors.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_plot/_artist_types.py
--rw-r--r--   0        0        0    10164 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_plot/_mpl_canvas.py
--rw-r--r--   0        0        0     7596 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_plot/_widget.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_preference/__init__.py
--rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_preference/_general.py
--rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_preference/_main.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_preference/_shared.py
--rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_preference/_table_config.py
--rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_preference/_theme.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_table/__init__.py
--rw-r--r--   0        0        0     7552 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_table/_animation.py
--rw-r--r--   0        0        0     8721 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_table/_display.py
--rw-r--r--   0        0        0     6917 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_table/_groupby.py
--rw-r--r--   0        0        0    38833 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_table/_spreadsheet.py
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_table/_table.py
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_table/_base/__init__.py
--rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_table/_base/_delegate.py
--rw-r--r--   0        0        0    27304 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_table/_base/_enhanced_table.py
--rw-r--r--   0        0        0    11370 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_table/_base/_header_view.py
--rw-r--r--   0        0        0    15319 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_table/_base/_item_model.py
--rw-r--r--   0        0        0     4761 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_table/_base/_keycombo.py
--rw-r--r--   0        0        0    28672 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_table/_base/_line_edit.py
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_table/_base/_object_holder.py
--rw-r--r--   0        0        0     4141 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_table/_base/_overlay.py
--rw-r--r--   0        0        0     4275 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_table/_base/_side_area.py
--rw-r--r--   0        0        0    62073 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_table/_base/_table_base.py
--rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_table/_base/_table_group.py
--rw-r--r--   0        0        0     3762 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_table/_base/_table_wrappers.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_table_stack/__init__.py
--rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_table_stack/_column_filter_widget.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_table_stack/_eval.py
--rw-r--r--   0        0        0    14746 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_table_stack/_finder.py
--rw-r--r--   0        0        0     9943 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_table_stack/_overlay.py
--rw-r--r--   0        0        0     3450 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_table_stack/_start.py
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_table_stack/_tabbar.py
--rw-r--r--   0        0        0    26670 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_table_stack/_tabwidget.py
--rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_table_stack/_utils.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_toolbar/__init__.py
--rw-r--r--   0        0        0     6599 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_toolbar/_corner.py
--rw-r--r--   0        0        0    12384 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_toolbar/_toolbar_widget.py
--rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/_qt/_toolbar/_toolbutton.py
--rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/commands/__init__.py
--rw-r--r--   0        0        0     6297 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/commands/_arange.py
--rw-r--r--   0        0        0    11818 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/commands/_dialogs.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/commands/_optimizer.py
--rw-r--r--   0        0        0    15417 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/commands/_plot_models.py
--rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/commands/_random_data.py
--rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/commands/_regression.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/commands/_storage.py
--rw-r--r--   0        0        0     3670 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/commands/_utils.py
--rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/commands/analysis.py
--rw-r--r--   0        0        0     5246 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/commands/column.py
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/commands/file.py
--rw-r--r--   0        0        0     5650 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/commands/plot.py
--rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/commands/selection.py
--rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/commands/tab.py
--rw-r--r--   0        0        0    10989 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/commands/table.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/commands/view.py
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/commands/window.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/commands/_sklearn/__init__.py
--rw-r--r--   0        0        0    14540 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/commands/_sklearn/_models.py
--rw-r--r--   0        0        0    10865 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/commands/_sklearn/_widget.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/commands/_stats/__init__.py
--rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/commands/_stats/_distribution.py
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/commands/_stats/_latex.py
--rw-r--r--   0        0        0    10460 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/commands/_stats/_statstest.py
--rw-r--r--   0        0        0     6236 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/commands/_stats/_widgets.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/style/__init__.py
--rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/style/_style.py
--rw-r--r--   0        0        0    12444 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/style/_style.qss
--rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/style/defaults.json
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/widgets/__init__.py
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/widgets/_doc.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/widgets/_keymap_abc.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/widgets/_magicgui.py
--rw-r--r--   0        0        0    24541 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/widgets/_mainwindow.py
--rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/widgets/_registry.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/widgets/_sample.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/widgets/_source.py
--rw-r--r--   0        0        0    34833 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/widgets/_table.py
--rw-r--r--   0        0        0     7459 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/widgets/_tablelist.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/widgets/_component/__init__.py
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/widgets/_component/_base.py
--rw-r--r--   0        0        0    10338 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/widgets/_component/_cell.py
--rw-r--r--   0        0        0    13602 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/widgets/_component/_column_setting.py
--rw-r--r--   0        0        0    11119 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/widgets/_component/_header.py
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/widgets/_component/_keymap.py
--rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/widgets/_component/_plot.py
--rw-r--r--   0        0        0    10386 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/widgets/_component/_proxy.py
--rw-r--r--   0        0        0     5286 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/widgets/_component/_ranges.py
--rw-r--r--   0        0        0    11531 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/widgets/_component/_table_subset.py
--rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 tabulous-0.5.6/tabulous/widgets/_component/_viewer.py
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 tabulous-0.5.6/.gitignore
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 tabulous-0.5.6/LICENSE
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 tabulous-0.5.6/README.md
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 tabulous-0.5.6/pyproject.toml
--rw-r--r--   0        0        0     4841 2020-02-02 00:00:00.000000 tabulous-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/__init__.py
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/__main__.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_async_importer.py
+-rw-r--r--   0        0        0     5310 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_colormap.py
+-rw-r--r--   0        0        0    11502 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_dtype.py
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_fetch_and_install.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_io.py
+-rw-r--r--   0        0        0     6407 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_ipython.py
+-rw-r--r--   0        0        0     8796 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_map_model.py
+-rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_pd_index.py
+-rw-r--r--   0        0        0    11539 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_range.py
+-rw-r--r--   0        0        0    13505 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_selection_model.py
+-rw-r--r--   0        0        0    15630 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_selection_op.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_slice_op.py
+-rw-r--r--   0        0        0    18522 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_sort_filter_proxy.py
+-rw-r--r--   0        0        0    15100 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_text_formatter.py
+-rw-r--r--   0        0        0    10351 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_utils.py
+-rw-r--r--   0        0        0    13695 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/color.py
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/core.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/exceptions.py
+-rw-r--r--   0        0        0     6494 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/post_init.py
+-rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/threading.py
+-rw-r--r--   0        0        0     5260 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/types.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_keymap/__init__.py
+-rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_keymap/_callback.py
+-rw-r--r--   0        0        0    22386 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_keymap/_keymap_objects.py
+-rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_keymap/_keymapview.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_magicgui/__init__.py
+-rw-r--r--   0        0        0     5175 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_magicgui/_color_edit.py
+-rw-r--r--   0        0        0     5034 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_magicgui/_dialog.py
+-rw-r--r--   0        0        0     8402 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_magicgui/_register.py
+-rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_magicgui/_selection.py
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_magicgui/_table.py
+-rw-r--r--   0        0        0     7798 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_magicgui/_timedelta.py
+-rw-r--r--   0        0        0    10017 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_magicgui/_toggle_switch.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_psygnal/__init__.py
+-rw-r--r--   0        0        0    13624 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_psygnal/_array.py
+-rw-r--r--   0        0        0    33079 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_psygnal/_psygnal_compat.py
+-rw-r--r--   0        0        0    23939 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_psygnal/_slots.py
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_psygnal/_special_objects.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/__init__.py
+-rw-r--r--   0        0        0     4510 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_action_registry.py
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_app.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_clickable_label.py
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_dockwidget.py
+-rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_filetree.py
+-rw-r--r--   0        0        0     4692 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_history.py
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_jump.py
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_multitips.py
+-rw-r--r--   0        0        0     5836 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_progress.py
+-rw-r--r--   0        0        0    13892 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_proxy_button.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_qt_const.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_svg.py
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_titlebar.py
+-rw-r--r--   0        0        0    11639 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_traceback.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_tree_header.py
+-rw-r--r--   0        0        0     4717 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_undo.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_console/__init__.py
+-rw-r--r--   0        0        0    11936 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_console/_widget.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/barplot.svg
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/boxenplot.svg
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/boxplot.svg
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/column_filter.svg
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/copy.svg
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/copy_as_spreadsheet.svg
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/copy_as_table.svg
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/cut.svg
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/eval.svg
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/filter.svg
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/find_item.svg
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/groupby.svg
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/hist.svg
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/melt.svg
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/more.svg
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/new_figure.svg
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/new_spreadsheet.svg
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/open_sample.svg
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/open_spreadsheet.svg
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/open_table.svg
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/optimize.svg
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/palette.svg
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/paste.svg
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/pivot.svg
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/plot.svg
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/preferences.svg
+-rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/random.svg
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/redo.svg
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/restore_columns.svg
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/round.svg
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/save_table.svg
+-rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/scatter.svg
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/settings.svg
+-rw-r--r--   0        0        0     3472 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/sklearn_analysis.svg
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/sort_table.svg
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/stats_test.svg
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/summarize_table.svg
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/swarmplot.svg
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/switch_header.svg
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/switch_layout.svg
+-rw-r--r--   0        0        0    67646 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/tabulous.ico
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/tile.svg
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/toggle_console.svg
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/trash_bin.svg
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/trash_bin_opened.svg
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/undo.svg
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/untile.svg
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/view_dual_h.svg
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/view_dual_v.svg
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/view_popup.svg
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/view_reset.svg
+-rw-r--r--   0        0        0    12285 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_icons/window_icon.png
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_mainwindow/__init__.py
+-rw-r--r--   0        0        0     9224 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_mainwindow/_base.py
+-rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_mainwindow/_command_palette.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_mainwindow/_keycombo.py
+-rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_mainwindow/_mainwidgets.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_mainwindow/_namespace.py
+-rw-r--r--   0        0        0     5024 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_mainwindow/_titlebar.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_plot/__init__.py
+-rw-r--r--   0        0        0    15100 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_plot/_artist_editors.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_plot/_artist_types.py
+-rw-r--r--   0        0        0    10164 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_plot/_mpl_canvas.py
+-rw-r--r--   0        0        0     7596 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_plot/_widget.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_preference/__init__.py
+-rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_preference/_general.py
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_preference/_main.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_preference/_shared.py
+-rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_preference/_table_config.py
+-rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_preference/_theme.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_table/__init__.py
+-rw-r--r--   0        0        0     7590 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_table/_animation.py
+-rw-r--r--   0        0        0     8721 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_table/_display.py
+-rw-r--r--   0        0        0     6917 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_table/_groupby.py
+-rw-r--r--   0        0        0    39019 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_table/_spreadsheet.py
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_table/_table.py
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_table/_base/__init__.py
+-rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_table/_base/_delegate.py
+-rw-r--r--   0        0        0    27381 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_table/_base/_enhanced_table.py
+-rw-r--r--   0        0        0    11370 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_table/_base/_header_view.py
+-rw-r--r--   0        0        0    15466 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_table/_base/_item_model.py
+-rw-r--r--   0        0        0     4761 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_table/_base/_keycombo.py
+-rw-r--r--   0        0        0    28672 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_table/_base/_line_edit.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_table/_base/_object_holder.py
+-rw-r--r--   0        0        0     4141 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_table/_base/_overlay.py
+-rw-r--r--   0        0        0     4275 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_table/_base/_side_area.py
+-rw-r--r--   0        0        0    62073 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_table/_base/_table_base.py
+-rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_table/_base/_table_group.py
+-rw-r--r--   0        0        0     3762 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_table/_base/_table_wrappers.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_table_stack/__init__.py
+-rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_table_stack/_column_filter_widget.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_table_stack/_eval.py
+-rw-r--r--   0        0        0    14746 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_table_stack/_finder.py
+-rw-r--r--   0        0        0     9943 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_table_stack/_overlay.py
+-rw-r--r--   0        0        0     3450 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_table_stack/_start.py
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_table_stack/_tabbar.py
+-rw-r--r--   0        0        0    26670 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_table_stack/_tabwidget.py
+-rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_table_stack/_utils.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_toolbar/__init__.py
+-rw-r--r--   0        0        0     6599 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_toolbar/_corner.py
+-rw-r--r--   0        0        0    12384 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_toolbar/_toolbar_widget.py
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/_qt/_toolbar/_toolbutton.py
+-rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/commands/__init__.py
+-rw-r--r--   0        0        0     6297 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/commands/_arange.py
+-rw-r--r--   0        0        0    11818 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/commands/_dialogs.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/commands/_optimizer.py
+-rw-r--r--   0        0        0    15417 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/commands/_plot_models.py
+-rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/commands/_random_data.py
+-rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/commands/_regression.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/commands/_storage.py
+-rw-r--r--   0        0        0     3670 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/commands/_utils.py
+-rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/commands/analysis.py
+-rw-r--r--   0        0        0     5246 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/commands/column.py
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/commands/file.py
+-rw-r--r--   0        0        0     5650 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/commands/plot.py
+-rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/commands/selection.py
+-rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/commands/tab.py
+-rw-r--r--   0        0        0    10989 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/commands/table.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/commands/view.py
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/commands/window.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/commands/_sklearn/__init__.py
+-rw-r--r--   0        0        0    14540 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/commands/_sklearn/_models.py
+-rw-r--r--   0        0        0    10865 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/commands/_sklearn/_widget.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/commands/_stats/__init__.py
+-rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/commands/_stats/_distribution.py
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/commands/_stats/_latex.py
+-rw-r--r--   0        0        0    10460 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/commands/_stats/_statstest.py
+-rw-r--r--   0        0        0     6236 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/commands/_stats/_widgets.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/style/__init__.py
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/style/_style.py
+-rw-r--r--   0        0        0    12444 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/style/_style.qss
+-rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/style/defaults.json
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/widgets/__init__.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/widgets/_doc.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/widgets/_keymap_abc.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/widgets/_magicgui.py
+-rw-r--r--   0        0        0    24541 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/widgets/_mainwindow.py
+-rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/widgets/_registry.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/widgets/_sample.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/widgets/_source.py
+-rw-r--r--   0        0        0    34833 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/widgets/_table.py
+-rw-r--r--   0        0        0     7459 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/widgets/_tablelist.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/widgets/_component/__init__.py
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/widgets/_component/_base.py
+-rw-r--r--   0        0        0    10339 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/widgets/_component/_cell.py
+-rw-r--r--   0        0        0    13602 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/widgets/_component/_column_setting.py
+-rw-r--r--   0        0        0    11119 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/widgets/_component/_header.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/widgets/_component/_keymap.py
+-rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/widgets/_component/_plot.py
+-rw-r--r--   0        0        0    10386 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/widgets/_component/_proxy.py
+-rw-r--r--   0        0        0     5286 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/widgets/_component/_ranges.py
+-rw-r--r--   0        0        0    11531 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/widgets/_component/_table_subset.py
+-rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 tabulous-0.5.7/tabulous/widgets/_component/_viewer.py
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 tabulous-0.5.7/.gitignore
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 tabulous-0.5.7/LICENSE
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 tabulous-0.5.7/README.md
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 tabulous-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0     4841 2020-02-02 00:00:00.000000 tabulous-0.5.7/PKG-INFO
```

### Comparing `tabulous-0.5.6/tabulous/__main__.py` & `tabulous-0.5.7/tabulous/__main__.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_async_importer.py` & `tabulous-0.5.7/tabulous/_async_importer.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_colormap.py` & `tabulous-0.5.7/tabulous/_colormap.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_dtype.py` & `tabulous-0.5.7/tabulous/_dtype.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_fetch_and_install.py` & `tabulous-0.5.7/tabulous/_fetch_and_install.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_io.py` & `tabulous-0.5.7/tabulous/_io.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_ipython.py` & `tabulous-0.5.7/tabulous/_ipython.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_map_model.py` & `tabulous-0.5.7/tabulous/_map_model.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_pd_index.py` & `tabulous-0.5.7/tabulous/_pd_index.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_range.py` & `tabulous-0.5.7/tabulous/_range.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_selection_model.py` & `tabulous-0.5.7/tabulous/_selection_model.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_selection_op.py` & `tabulous-0.5.7/tabulous/_selection_op.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_slice_op.py` & `tabulous-0.5.7/tabulous/_slice_op.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_sort_filter_proxy.py` & `tabulous-0.5.7/tabulous/_sort_filter_proxy.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_text_formatter.py` & `tabulous-0.5.7/tabulous/_text_formatter.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_utils.py` & `tabulous-0.5.7/tabulous/_utils.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/color.py` & `tabulous-0.5.7/tabulous/color.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/core.py` & `tabulous-0.5.7/tabulous/core.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/exceptions.py` & `tabulous-0.5.7/tabulous/exceptions.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/post_init.py` & `tabulous-0.5.7/tabulous/post_init.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/threading.py` & `tabulous-0.5.7/tabulous/threading.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/types.py` & `tabulous-0.5.7/tabulous/types.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_keymap/_callback.py` & `tabulous-0.5.7/tabulous/_keymap/_callback.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_keymap/_keymap_objects.py` & `tabulous-0.5.7/tabulous/_keymap/_keymap_objects.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_keymap/_keymapview.py` & `tabulous-0.5.7/tabulous/_keymap/_keymapview.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_magicgui/__init__.py` & `tabulous-0.5.7/tabulous/_magicgui/__init__.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_magicgui/_color_edit.py` & `tabulous-0.5.7/tabulous/_magicgui/_color_edit.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_magicgui/_dialog.py` & `tabulous-0.5.7/tabulous/_magicgui/_dialog.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_magicgui/_register.py` & `tabulous-0.5.7/tabulous/_magicgui/_register.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_magicgui/_selection.py` & `tabulous-0.5.7/tabulous/_magicgui/_selection.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_magicgui/_table.py` & `tabulous-0.5.7/tabulous/_magicgui/_table.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_magicgui/_timedelta.py` & `tabulous-0.5.7/tabulous/_magicgui/_timedelta.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_magicgui/_toggle_switch.py` & `tabulous-0.5.7/tabulous/_magicgui/_toggle_switch.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_psygnal/_array.py` & `tabulous-0.5.7/tabulous/_psygnal/_array.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_psygnal/_psygnal_compat.py` & `tabulous-0.5.7/tabulous/_psygnal/_psygnal_compat.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_psygnal/_slots.py` & `tabulous-0.5.7/tabulous/_psygnal/_slots.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_psygnal/_special_objects.py` & `tabulous-0.5.7/tabulous/_psygnal/_special_objects.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_action_registry.py` & `tabulous-0.5.7/tabulous/_qt/_action_registry.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_app.py` & `tabulous-0.5.7/tabulous/_qt/_app.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_clickable_label.py` & `tabulous-0.5.7/tabulous/_qt/_clickable_label.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_dockwidget.py` & `tabulous-0.5.7/tabulous/_qt/_dockwidget.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_filetree.py` & `tabulous-0.5.7/tabulous/_qt/_filetree.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_history.py` & `tabulous-0.5.7/tabulous/_qt/_history.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_jump.py` & `tabulous-0.5.7/tabulous/_qt/_jump.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_multitips.py` & `tabulous-0.5.7/tabulous/_qt/_multitips.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_progress.py` & `tabulous-0.5.7/tabulous/_qt/_progress.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_proxy_button.py` & `tabulous-0.5.7/tabulous/_qt/_proxy_button.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_svg.py` & `tabulous-0.5.7/tabulous/_qt/_svg.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_titlebar.py` & `tabulous-0.5.7/tabulous/_qt/_titlebar.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_traceback.py` & `tabulous-0.5.7/tabulous/_qt/_traceback.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_tree_header.py` & `tabulous-0.5.7/tabulous/_qt/_tree_header.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_undo.py` & `tabulous-0.5.7/tabulous/_qt/_undo.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_console/__init__.py` & `tabulous-0.5.7/tabulous/_qt/_console/__init__.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_console/_widget.py` & `tabulous-0.5.7/tabulous/_qt/_console/_widget.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/barplot.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/barplot.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/boxenplot.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/boxenplot.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/boxplot.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/boxplot.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/column_filter.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/column_filter.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/copy.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/copy.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/copy_as_spreadsheet.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/copy_as_spreadsheet.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/copy_as_table.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/copy_as_table.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/cut.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/cut.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/eval.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/eval.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/filter.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/filter.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/find_item.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/find_item.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/groupby.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/groupby.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/hist.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/hist.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/melt.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/melt.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/more.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/more.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/new_figure.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/new_figure.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/new_spreadsheet.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/new_spreadsheet.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/open_sample.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/open_sample.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/open_spreadsheet.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/open_spreadsheet.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/open_table.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/open_table.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/optimize.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/optimize.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/palette.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/palette.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/paste.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/paste.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/pivot.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/pivot.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/plot.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/plot.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/preferences.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/preferences.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/random.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/random.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/redo.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/redo.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/restore_columns.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/restore_columns.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/round.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/round.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/save_table.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/save_table.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/scatter.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/scatter.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/settings.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/settings.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/sklearn_analysis.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/sklearn_analysis.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/sort_table.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/sort_table.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/stats_test.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/stats_test.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/summarize_table.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/summarize_table.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/swarmplot.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/swarmplot.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/switch_header.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/switch_header.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/switch_layout.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/switch_layout.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/tabulous.ico` & `tabulous-0.5.7/tabulous/_qt/_icons/tabulous.ico`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/tile.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/tile.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/toggle_console.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/toggle_console.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/trash_bin.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/trash_bin.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/trash_bin_opened.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/trash_bin_opened.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/undo.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/undo.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/untile.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/untile.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/view_dual_h.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/view_dual_h.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/view_dual_v.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/view_dual_v.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/view_popup.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/view_popup.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/view_reset.svg` & `tabulous-0.5.7/tabulous/_qt/_icons/view_reset.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_icons/window_icon.png` & `tabulous-0.5.7/tabulous/_qt/_icons/window_icon.png`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_mainwindow/_base.py` & `tabulous-0.5.7/tabulous/_qt/_mainwindow/_base.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_mainwindow/_command_palette.py` & `tabulous-0.5.7/tabulous/_qt/_mainwindow/_command_palette.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_mainwindow/_keycombo.py` & `tabulous-0.5.7/tabulous/_qt/_mainwindow/_keycombo.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_mainwindow/_mainwidgets.py` & `tabulous-0.5.7/tabulous/_qt/_mainwindow/_mainwidgets.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_mainwindow/_namespace.py` & `tabulous-0.5.7/tabulous/_qt/_mainwindow/_namespace.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_mainwindow/_titlebar.py` & `tabulous-0.5.7/tabulous/_qt/_mainwindow/_titlebar.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_plot/_artist_editors.py` & `tabulous-0.5.7/tabulous/_qt/_plot/_artist_editors.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_plot/_artist_types.py` & `tabulous-0.5.7/tabulous/_qt/_plot/_artist_types.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_plot/_mpl_canvas.py` & `tabulous-0.5.7/tabulous/_qt/_plot/_mpl_canvas.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_plot/_widget.py` & `tabulous-0.5.7/tabulous/_qt/_plot/_widget.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_preference/_general.py` & `tabulous-0.5.7/tabulous/_qt/_preference/_general.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_preference/_main.py` & `tabulous-0.5.7/tabulous/_qt/_preference/_main.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_preference/_table_config.py` & `tabulous-0.5.7/tabulous/_qt/_preference/_table_config.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_preference/_theme.py` & `tabulous-0.5.7/tabulous/_qt/_preference/_theme.py`

 * *Files 26% similar despite different names*

```diff
@@ -67,28 +67,32 @@
     def sizeHint(self) -> QtCore.QSize:
         return QtCore.QSize(30, 30)
 
     def paintEvent(self, a0: QtGui.QPaintEvent) -> None:
         painter = QtGui.QPainter(self)
         geo = self.rect()
 
-        grad = QtGui.QLinearGradient(geo.topLeft(), geo.bottomRight())
+        grad = QtGui.QLinearGradient(
+            QtCore.QPointF(geo.topLeft()), QtCore.QPointF(geo.bottomRight())
+        )
         grad.setColorAt(0, QtGui.QColor(self._style_theme.background0))
         grad.setColorAt(1, QtGui.QColor(self._style_theme.background1))
-        path = QtGui.QPainterPath(geo.topLeft())
-        path.lineTo(geo.topRight())
-        path.lineTo(geo.bottomLeft())
+        path = QtGui.QPainterPath(QtCore.QPointF(geo.topLeft()))
+        path.lineTo(QtCore.QPointF(geo.topRight()))
+        path.lineTo(QtCore.QPointF(geo.bottomLeft()))
         painter.fillPath(path, grad)
 
-        grad = QtGui.QLinearGradient(geo.topLeft(), geo.bottomRight())
+        grad = QtGui.QLinearGradient(
+            QtCore.QPointF(geo.topLeft()), QtCore.QPointF(geo.bottomRight())
+        )
         grad.setColorAt(0, QtGui.QColor(self._style_theme.highlight0))
         grad.setColorAt(1, QtGui.QColor(self._style_theme.highlight1))
-        path = QtGui.QPainterPath(geo.topRight())
-        path.lineTo(geo.bottomLeft())
-        path.lineTo(geo.bottomRight())
+        path = QtGui.QPainterPath(QtCore.QPointF(geo.topRight()))
+        path.lineTo(QtCore.QPointF(geo.bottomLeft()))
+        path.lineTo(QtCore.QPointF(geo.bottomRight()))
         painter.fillPath(path, grad)
 
         if self._checked:
             painter.setPen(QtGui.QPen(QtGui.QColor(255, 20, 20), 3))
             painter.drawRect(geo)
 
         painter.setPen(QtGui.QPen(QtGui.QColor(self._style_theme.foreground), 3))
```

### Comparing `tabulous-0.5.6/tabulous/_qt/_table/_animation.py` & `tabulous-0.5.7/tabulous/_qt/_table/_animation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Callable, Generic, SupportsIndex, TypeVar
 from abc import ABC, abstractmethod
 from contextlib import contextmanager
 from tabulous._utils import get_config
 from tabulous._range import MultiRectRange, RectRange
+from tabulous._qt._qt_const import background_color_role
 
 from qtpy import QtCore, QtWidgets as QtW, QtGui
 
 if TYPE_CHECKING:
     from ._base import QBaseTable
     from ._base._item_model import AbstractDataFrameModel
 
@@ -119,15 +120,15 @@
         return (index.row(), index.column()) in rng
 
     def get_brush(self, size: QtCore.QSize, time: float, bg) -> QtGui.QBrush:
         """Return the brush for the given size and time, with cache support."""
         qtable = self._parent.parent()
         is_qvariant = not isinstance(bg, QtGui.QColor)
         if is_qvariant:
-            bg = qtable.palette().color(QtGui.QPalette.ColorRole.Background)
+            bg = background_color_role(qtable.palette())
         col = qtable._qtable_view.selectionColor
         length = max(size.width(), size.height())
         dh = 4 / length
         col.setAlpha(96)
         grad = QtGui.QLinearGradient(0, 0, length, length)
         grad.setColorAt(0.0, bg)
         grad.setColorAt(max(time - dh, 0.0), bg)
```

### Comparing `tabulous-0.5.6/tabulous/_qt/_table/_display.py` & `tabulous-0.5.7/tabulous/_qt/_table/_display.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_table/_groupby.py` & `tabulous-0.5.7/tabulous/_qt/_table/_groupby.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_table/_spreadsheet.py` & `tabulous-0.5.7/tabulous/_qt/_table/_spreadsheet.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,18 +145,21 @@
             if slot := qtable._qtable_view._table_map.get_by_dest((r, c), None):
                 ref = f"\nExpr: {slot.as_literal(dest=True)}"
                 if slot._current_error is not None:
                     ref += "\n" + slot.format_error()
             else:
                 ref = ""
             dtype = self._columns_dtype.get(name, None)
+            val_repr = repr(val)
+            if len(val_repr) > 64:
+                val_repr = val_repr[:60] + "..." + val_repr[-4:]
             if dtype is None:
-                return f"{val!r} (dtype: infer){ref}"
+                return f"{val_repr} (dtype: infer){ref}"
             else:
-                return f"{val!r} (dtype: {dtype}){ref}"
+                return f"{val_repr} (dtype: {dtype}){ref}"
         return QtCore.QVariant()
 
     def rename_column(self, old_name: str, new_name: str):
         super().rename_column(old_name, new_name)
         if dtype := self._columns_dtype.pop(old_name, None):
             self._columns_dtype[new_name] = dtype
         return None
@@ -292,15 +295,15 @@
         self._anim_row.set_animate(cfg.window.animate)
         self._anim_col.set_animate(cfg.window.animate)
         return super().load_config(cfg)
 
     @QMutableSimpleTable._mgr.interface
     def setDataFrame(self, data: pd.DataFrame) -> None:
         """Set data frame as a string table."""
-        self._data_raw = data.astype(_STRING_DTYPE)
+        self._data_raw = data.astype(_STRING_DTYPE).fillna("")
 
         # SpreadSheet columns should be str if possible. Convert it.
         if isinstance(self._data_raw.columns, pd.RangeIndex):
             self._data_raw.columns = _pd_index.char_arange(self._data_raw.columns.size)
         elif self._data_raw.columns.dtype.kind in "iuf":
             self._data_raw.columns = self._data_raw.columns.astype(str)
 
@@ -382,15 +385,15 @@
     def assignColumns(self, serieses: dict[str, pd.Series]):
         to_delete = set()
         to_assign: dict[str, pd.Series] = {}
         for k, v in serieses.items():
             if v is self.__delete:
                 to_delete.add(k)
             else:
-                to_assign[k] = v.astype(_STRING_DTYPE)
+                to_assign[k] = v.astype(_STRING_DTYPE).fillna("")
         old_value = self._data_raw
         self._data_raw: pd.DataFrame = self._data_raw.assign(**to_assign).drop(
             to_delete, axis=1, inplace=False
         )
 
         self.model().df = self._data_raw
         self.setProxy(None)
@@ -480,15 +483,15 @@
                 model = self._qtable_view.model()
                 index = model.index(r, c, QtCore.QModelIndex())
                 text = model.data(index, Qt.ItemDataRole.DisplayRole)
                 if text == value:
                     return
 
         elif isinstance(value, pd.DataFrame) and any(value.dtypes != "string"):
-            value = value.astype(_STRING_DTYPE)
+            value = value.astype(_STRING_DTYPE).fillna("")
 
         with self._mgr.merging(formatter=lambda _: self._set_value_fmt(r, c, value)):
             if need_expand:
                 self.expandDataFrame(max(rmax - nr + 1, 0), max(cmax - nc + 1, 0))
             super().setDataFrameValue(r, c, value)
             self._set_proxy(self._proxy)
 
@@ -497,15 +500,15 @@
     def setLabeledData(self, r: slice, c: slice, value: pd.Series):
         nr, nc = self._data_raw.shape
         rmax = _get_limit(r)
         cmax = _get_limit(c)
         need_expand = nr <= rmax or nc <= cmax
 
         if value.dtype != "string":
-            value = value.astype(_STRING_DTYPE)
+            value = value.astype(_STRING_DTYPE).fillna("")
 
         with self._mgr.merging(formatter=lambda cmds: cmds[-2].format()):
             if need_expand:
                 self.expandDataFrame(max(rmax - nr + 1, 0), max(cmax - nc + 1, 0))
             super().setLabeledData(r, c, value)
             self._set_proxy(self._proxy)
```

### Comparing `tabulous-0.5.6/tabulous/_qt/_table/_table.py` & `tabulous-0.5.7/tabulous/_qt/_table/_table.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_table/_base/_delegate.py` & `tabulous-0.5.7/tabulous/_qt/_table/_base/_delegate.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_table/_base/_enhanced_table.py` & `tabulous-0.5.7/tabulous/_qt/_table/_base/_enhanced_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,14 +356,16 @@
             self._mouse_track.last_button = "right"
             return
         _selection_model.set_shift(True)
         return super().mousePressEvent(e)
 
     def mouseMoveEvent(self, e: QtGui.QMouseEvent) -> None:
         """Scroll table plane when mouse is moved with right click."""
+        if e.buttons() == Qt.MouseButton.NoButton:
+            return None
         if self._mouse_track.last_button == "right":
             pos = e.pos()
             dy = pos.y() - self._mouse_track.last_rightclick_pos.y()
             dx = pos.x() - self._mouse_track.last_rightclick_pos.x()
             self.verticalScrollBar().setValue(self.verticalScrollBar().value() - dy)
             self.horizontalScrollBar().setValue(self.horizontalScrollBar().value() - dx)
             self._mouse_track.last_rightclick_pos = pos
```

### Comparing `tabulous-0.5.6/tabulous/_qt/_table/_base/_header_view.py` & `tabulous-0.5.7/tabulous/_qt/_table/_base/_header_view.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_table/_base/_item_model.py` & `tabulous-0.5.7/tabulous/_qt/_table/_base/_item_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,17 +35,17 @@
         self._background_colormap: dict[Hashable, Callable[[Any], ColorType]] = {}
         self._text_formatter: dict[Hashable, Callable[[Any], str]] = {}
         self._validator: dict[Hashable, Callable[[Any], None]] = {}
 
         self._data_role_map = {
             Qt.ItemDataRole.DisplayRole: self._data_display,
             Qt.ItemDataRole.EditRole: self._data_edit,
-            Qt.ItemDataRole.TextColorRole: self._data_text_color,
+            Qt.ItemDataRole.ForegroundRole: self._data_text_color,
             Qt.ItemDataRole.ToolTipRole: self._data_tooltip,
-            Qt.ItemDataRole.BackgroundColorRole: self._data_background_color_rendered,
+            Qt.ItemDataRole.BackgroundRole: self._data_background_color_rendered,
             Qt.ItemDataRole.DecorationRole: self._data_decoration,
             Qt.ItemDataRole.SizeHintRole: self._data_size_hint,
         }
 
         self._decorations: TableMapping[tuple[QtGui.QPixmap, str]] = TableMapping()
         self._background_color_anim = CellColorAnimation(self)
 
@@ -142,15 +142,18 @@
             if ref_expr := self.parent()._get_ref_expr_by_dest(r, c):
                 ref = f"\nExpr: {ref_expr}"
             else:
                 ref = ""
             if dtype != object:
                 return f"{val!r} (dtype: {dtype}){ref}"
             else:
-                return f"{val!r} (dtype: {dtype}; type: {type(val).__name__}){ref}"
+                val_repr = repr(val)
+                if len(val_repr) > 64:
+                    val_repr = val_repr[:60] + "..." + val_repr[-4:]
+                return f"{val_repr} (dtype: {dtype}; type: {type(val).__name__}){ref}"
         return QtCore.QVariant()
 
     def _data_background_color(self, index: QtCore.QModelIndex):
         if not self._background_colormap:
             return QtCore.QVariant()
         r, c = index.row(), index.column()
         df = self.df
```

### Comparing `tabulous-0.5.6/tabulous/_qt/_table/_base/_keycombo.py` & `tabulous-0.5.7/tabulous/_qt/_table/_base/_keycombo.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_table/_base/_line_edit.py` & `tabulous-0.5.7/tabulous/_qt/_table/_base/_line_edit.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_table/_base/_object_holder.py` & `tabulous-0.5.7/tabulous/_qt/_table/_base/_object_holder.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_table/_base/_overlay.py` & `tabulous-0.5.7/tabulous/_qt/_table/_base/_overlay.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_table/_base/_side_area.py` & `tabulous-0.5.7/tabulous/_qt/_table/_base/_side_area.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_table/_base/_table_base.py` & `tabulous-0.5.7/tabulous/_qt/_table/_base/_table_base.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_table/_base/_table_group.py` & `tabulous-0.5.7/tabulous/_qt/_table/_base/_table_group.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_table/_base/_table_wrappers.py` & `tabulous-0.5.7/tabulous/_qt/_table/_base/_table_wrappers.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_table_stack/_column_filter_widget.py` & `tabulous-0.5.7/tabulous/_qt/_table_stack/_column_filter_widget.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_table_stack/_eval.py` & `tabulous-0.5.7/tabulous/_qt/_table_stack/_eval.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_table_stack/_finder.py` & `tabulous-0.5.7/tabulous/_qt/_table_stack/_finder.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_table_stack/_overlay.py` & `tabulous-0.5.7/tabulous/_qt/_table_stack/_overlay.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_table_stack/_start.py` & `tabulous-0.5.7/tabulous/_qt/_table_stack/_start.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_table_stack/_tabbar.py` & `tabulous-0.5.7/tabulous/_qt/_table_stack/_tabbar.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_table_stack/_tabwidget.py` & `tabulous-0.5.7/tabulous/_qt/_table_stack/_tabwidget.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_table_stack/_utils.py` & `tabulous-0.5.7/tabulous/_qt/_table_stack/_utils.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_toolbar/_corner.py` & `tabulous-0.5.7/tabulous/_qt/_toolbar/_corner.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_toolbar/_toolbar_widget.py` & `tabulous-0.5.7/tabulous/_qt/_toolbar/_toolbar_widget.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/_qt/_toolbar/_toolbutton.py` & `tabulous-0.5.7/tabulous/_qt/_toolbar/_toolbutton.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/commands/__init__.py` & `tabulous-0.5.7/tabulous/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/commands/_arange.py` & `tabulous-0.5.7/tabulous/commands/_arange.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/commands/_dialogs.py` & `tabulous-0.5.7/tabulous/commands/_dialogs.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/commands/_optimizer.py` & `tabulous-0.5.7/tabulous/commands/_optimizer.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/commands/_plot_models.py` & `tabulous-0.5.7/tabulous/commands/_plot_models.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/commands/_random_data.py` & `tabulous-0.5.7/tabulous/commands/_random_data.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/commands/_regression.py` & `tabulous-0.5.7/tabulous/commands/_regression.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/commands/_utils.py` & `tabulous-0.5.7/tabulous/commands/_utils.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/commands/analysis.py` & `tabulous-0.5.7/tabulous/commands/analysis.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/commands/column.py` & `tabulous-0.5.7/tabulous/commands/column.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/commands/file.py` & `tabulous-0.5.7/tabulous/commands/file.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/commands/plot.py` & `tabulous-0.5.7/tabulous/commands/plot.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/commands/selection.py` & `tabulous-0.5.7/tabulous/commands/selection.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/commands/tab.py` & `tabulous-0.5.7/tabulous/commands/tab.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/commands/table.py` & `tabulous-0.5.7/tabulous/commands/table.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/commands/view.py` & `tabulous-0.5.7/tabulous/commands/view.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/commands/window.py` & `tabulous-0.5.7/tabulous/commands/window.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/commands/_sklearn/_models.py` & `tabulous-0.5.7/tabulous/commands/_sklearn/_models.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/commands/_sklearn/_widget.py` & `tabulous-0.5.7/tabulous/commands/_sklearn/_widget.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/commands/_stats/_distribution.py` & `tabulous-0.5.7/tabulous/commands/_stats/_distribution.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/commands/_stats/_latex.py` & `tabulous-0.5.7/tabulous/commands/_stats/_latex.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/commands/_stats/_statstest.py` & `tabulous-0.5.7/tabulous/commands/_stats/_statstest.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/commands/_stats/_widgets.py` & `tabulous-0.5.7/tabulous/commands/_stats/_widgets.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/style/_style.py` & `tabulous-0.5.7/tabulous/style/_style.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/style/_style.qss` & `tabulous-0.5.7/tabulous/style/_style.qss`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/style/defaults.json` & `tabulous-0.5.7/tabulous/style/defaults.json`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/widgets/_doc.py` & `tabulous-0.5.7/tabulous/widgets/_doc.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/widgets/_magicgui.py` & `tabulous-0.5.7/tabulous/widgets/_magicgui.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/widgets/_mainwindow.py` & `tabulous-0.5.7/tabulous/widgets/_mainwindow.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/widgets/_registry.py` & `tabulous-0.5.7/tabulous/widgets/_registry.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/widgets/_sample.py` & `tabulous-0.5.7/tabulous/widgets/_sample.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/widgets/_source.py` & `tabulous-0.5.7/tabulous/widgets/_source.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/widgets/_table.py` & `tabulous-0.5.7/tabulous/widgets/_table.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/widgets/_tablelist.py` & `tabulous-0.5.7/tabulous/widgets/_tablelist.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/widgets/_component/__init__.py` & `tabulous-0.5.7/tabulous/widgets/_component/__init__.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/widgets/_component/_base.py` & `tabulous-0.5.7/tabulous/widgets/_component/_base.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/widgets/_component/_cell.py` & `tabulous-0.5.7/tabulous/widgets/_component/_cell.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
 class CellForegroundColorInterface(_Sequence2D):
     def __getitem__(self, key: tuple[int, int]) -> ColorTuple | None:
         """Get the text color of a cell."""
         self._assert_integers(key)
         model = self.parent.native.model()
         idx = model.index(*key)
-        qcolor = model.data(idx, role=Qt.ItemDataRole.TextColorRole)
+        qcolor = model.data(idx, role=Qt.ItemDataRole.ForegroundRole)
         if isinstance(qcolor, QtGui.QColor):
             return ColorTuple(*qcolor.getRgb())
         return None
 
 
 class CellDisplayedTextInterface(_Sequence2D):
     def __getitem__(self, key: tuple[int, int]) -> str:
```

### Comparing `tabulous-0.5.6/tabulous/widgets/_component/_column_setting.py` & `tabulous-0.5.7/tabulous/widgets/_component/_column_setting.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/widgets/_component/_header.py` & `tabulous-0.5.7/tabulous/widgets/_component/_header.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/widgets/_component/_keymap.py` & `tabulous-0.5.7/tabulous/widgets/_component/_keymap.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/widgets/_component/_plot.py` & `tabulous-0.5.7/tabulous/widgets/_component/_plot.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/widgets/_component/_proxy.py` & `tabulous-0.5.7/tabulous/widgets/_component/_proxy.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/widgets/_component/_ranges.py` & `tabulous-0.5.7/tabulous/widgets/_component/_ranges.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/widgets/_component/_table_subset.py` & `tabulous-0.5.7/tabulous/widgets/_component/_table_subset.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/tabulous/widgets/_component/_viewer.py` & `tabulous-0.5.7/tabulous/widgets/_component/_viewer.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/.gitignore` & `tabulous-0.5.7/.gitignore`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/LICENSE` & `tabulous-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/README.md` & `tabulous-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/pyproject.toml` & `tabulous-0.5.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.6/PKG-INFO` & `tabulous-0.5.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: tabulous
-Version: 0.5.6
+Version: 0.5.7
 Summary: A table data viewer for Python
 Project-URL: Download, https://github.com/hanjinliu/tabulous
 Author-email: Hanjin Liu <liuhanjin-sc@g.ecc.u-tokyo.ac.jp>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Hanjin Liu
         All rights reserved.
```

