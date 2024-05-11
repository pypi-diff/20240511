# Comparing `tmp/pyxllib-0.3.95.tar.gz` & `tmp/pyxllib-0.3.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxllib-0.3.95.tar", last modified: Thu Feb 22 06:22:49 2024, max compression
+gzip compressed data, was "pyxllib-0.3.96.tar", last modified: Wed Mar  6 02:59:49 2024, max compression
```

## Comparing `pyxllib-0.3.95.tar` & `pyxllib-0.3.96.tar`

### file list

```diff
@@ -1,393 +1,393 @@
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.419696 pyxllib-0.3.95/
--rw-rw-rw-   0        0        0    10443 2024-01-08 13:05:59.000000 pyxllib-0.3.95/LICENSE
--rw-rw-rw-   0        0        0       80 2024-01-08 13:05:59.000000 pyxllib-0.3.95/MANIFEST.in
--rw-rw-rw-   0        0        0     1057 2024-02-22 06:22:49.419696 pyxllib-0.3.95/PKG-INFO
--rw-rw-rw-   0        0        0      441 2024-01-08 13:05:59.000000 pyxllib-0.3.95/README.md
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.241112 pyxllib-0.3.95/pyxllib/
--rw-rw-rw-   0        0        0      529 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.249112 pyxllib-0.3.95/pyxllib/algo/
--rw-rw-rw-   0        0        0      161 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/algo/__init__.py
--rw-rw-rw-   0        0        0     1450 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/algo/disjoint.py
--rw-rw-rw-   0        0        0    18190 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/algo/geo.py
--rw-rw-rw-   0        0        0    36718 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/algo/intervals.py
--rw-rw-rw-   0        0        0    12600 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/algo/matcher.py
--rw-rw-rw-   0        0        0     4168 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/algo/newbie.py
--rw-rw-rw-   0        0        0    17029 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/algo/pupil.py
--rw-rw-rw-   0        0        0     2393 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/algo/shapelylib.py
--rw-rw-rw-   0        0        0     8584 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/algo/specialist.py
--rw-rw-rw-   0        0        0    16792 2024-01-24 11:47:10.000000 pyxllib-0.3.95/pyxllib/algo/stat.py
--rw-rw-rw-   0        0        0     5094 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/algo/treelib.py
--rw-rw-rw-   0        0        0     1953 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/algo/unitlib.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.257112 pyxllib-0.3.95/pyxllib/cv/
--rw-rw-rw-   0        0        0      132 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/cv/__init__.py
--rw-rw-rw-   0        0        0    11378 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/cv/expert.py
--rw-rw-rw-   0        0        0     6757 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/cv/imfile.py
--rw-rw-rw-   0        0        0      977 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/cv/imhash.py
--rw-rw-rw-   0        0        0      339 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/cv/pupil.py
--rw-rw-rw-   0        0        0    38270 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/cv/rgbfmt.py
--rw-rw-rw-   0        0        0     9259 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/cv/trackbartools.py
--rw-rw-rw-   0        0        0    40787 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/cv/xlcvlib.py
--rw-rw-rw-   0        0        0    15454 2024-01-11 16:11:21.000000 pyxllib-0.3.95/pyxllib/cv/xlpillib.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.260112 pyxllib-0.3.95/pyxllib/data/
--rw-rw-rw-   0        0        0        0 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/data/__init__.py
--rw-rw-rw-   0        0        0     3876 2024-01-14 08:47:19.000000 pyxllib-0.3.95/pyxllib/data/echarts.py
--rw-rw-rw-   0        0        0     2477 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/data/oss.py
--rw-rw-rw-   0        0        0    28830 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/data/pglib.py
--rw-rw-rw-   0        0        0    12791 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/data/sqlite.py
--rw-rw-rw-   0        0        0    11955 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/data/sqllib.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.266116 pyxllib-0.3.95/pyxllib/ext/
--rw-rw-rw-   0        0        0    19419 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/ext/JLineViewer.py
--rw-rw-rw-   0        0        0      134 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/ext/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.268112 pyxllib-0.3.95/pyxllib/ext/autogui/
--rw-rw-rw-   0        0        0      223 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/ext/autogui/__init__.py
--rw-rw-rw-   0        0        0    29612 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/ext/autogui/autogui.py
--rw-rw-rw-   0        0        0     3654 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/ext/autogui/virtualkey.py
--rw-rw-rw-   0        0        0     8552 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/ext/demolib.py
--rw-rw-rw-   0        0        0    70865 2024-02-22 01:39:47.000000 pyxllib-0.3.95/pyxllib/ext/kq5034lib.py
--rw-rw-rw-   0        0        0    27407 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/ext/old.py
--rw-rw-rw-   0        0        0    16090 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/ext/qt.py
--rw-rw-rw-   0        0        0     2771 2024-01-24 09:13:45.000000 pyxllib-0.3.95/pyxllib/ext/seleniumlib.py
--rw-rw-rw-   0        0        0     5004 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/ext/tk.py
--rw-rw-rw-   0        0        0    34607 2024-01-29 05:10:36.000000 pyxllib-0.3.95/pyxllib/ext/unixlib.py
--rw-rw-rw-   0        0        0    13663 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/ext/utools.py
--rw-rw-rw-   0        0        0     2922 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/ext/webhook.py
--rw-rw-rw-   0        0        0     1237 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/ext/win32lib.py
--rw-rw-rw-   0        0        0     5857 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/ext/yuquelib.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.272112 pyxllib-0.3.95/pyxllib/file/
--rw-rw-rw-   0        0        0      452 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/file/__init__.py
--rw-rw-rw-   0        0        0    29778 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/file/docxlib.py
--rw-rw-rw-   0        0        0    11620 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/file/gitlib.py
--rw-rw-rw-   0        0        0     5880 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/file/movielib.py
--rw-rw-rw-   0        0        0      218 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/file/newbie.py
--rw-rw-rw-   0        0        0    55027 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/file/onenotelib.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.273114 pyxllib-0.3.95/pyxllib/file/packlib/
--rw-rw-rw-   0        0        0    11464 2024-01-10 13:03:47.000000 pyxllib-0.3.95/pyxllib/file/packlib/__init__.py
--rw-rw-rw-   0        0        0    90165 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/file/packlib/zipfile.py
--rw-rw-rw-   0        0        0    17010 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/file/pdflib.py
--rw-rw-rw-   0        0        0     5997 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/file/pupil.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.277115 pyxllib-0.3.95/pyxllib/file/specialist/
--rw-rw-rw-   0        0        0    28260 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/file/specialist/__init__.py
--rw-rw-rw-   0        0        0    32411 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/file/specialist/dirlib.py
--rw-rw-rw-   0        0        0     6763 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/file/specialist/download.py
--rw-rw-rw-   0        0        0   101158 2024-01-12 08:19:59.000000 pyxllib-0.3.95/pyxllib/file/specialist/filelib.py
--rw-rw-rw-   0        0        0   125766 2024-01-26 09:42:16.000000 pyxllib-0.3.95/pyxllib/file/xlsxlib.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.280114 pyxllib-0.3.95/pyxllib/prog/
--rw-rw-rw-   0        0        0      132 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/prog/__init__.py
--rw-rw-rw-   0        0        0     8499 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/prog/deprecatedlib.py
--rw-rw-rw-   0        0        0     9229 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/prog/ipyexec.py
--rw-rw-rw-   0        0        0    15005 2024-01-13 15:01:52.000000 pyxllib-0.3.95/pyxllib/prog/newbie.py
--rw-rw-rw-   0        0        0    43196 2024-01-23 12:35:18.000000 pyxllib-0.3.95/pyxllib/prog/pupil.py
--rw-rw-rw-   0        0        0      996 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/prog/sitepackages.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.284113 pyxllib-0.3.95/pyxllib/prog/specialist/
--rw-rw-rw-   0        0        0     7901 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/prog/specialist/__init__.py
--rw-rw-rw-   0        0        0     9657 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/prog/specialist/bc.py
--rw-rw-rw-   0        0        0    19868 2024-02-19 15:29:00.000000 pyxllib-0.3.95/pyxllib/prog/specialist/browser.py
--rw-rw-rw-   0        0        0    13309 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/prog/specialist/common.py
--rw-rw-rw-   0        0        0     4525 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/prog/specialist/datetime.py
--rw-rw-rw-   0        0        0     8206 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/prog/specialist/tictoc.py
--rw-rw-rw-   0        0        0     8298 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/prog/specialist/xllog.py
--rw-rw-rw-   0        0        0     3669 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/prog/xlosenv.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.284113 pyxllib-0.3.95/pyxllib/stdlib/
--rw-rw-rw-   0        0        0      581 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/stdlib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.286115 pyxllib-0.3.95/pyxllib/stdlib/tablepyxl/
--rw-rw-rw-   0        0        0      193 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/stdlib/tablepyxl/__init__.py
--rw-rw-rw-   0        0        0    10924 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/stdlib/tablepyxl/style.py
--rw-rw-rw-   0        0        0     4531 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/stdlib/tablepyxl/tablepyxl.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.292214 pyxllib-0.3.95/pyxllib/text/
--rw-rw-rw-   0        0        0      170 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/text/__init__.py
--rw-rw-rw-   0        0        0     1259 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/text/ahocorasick.py
--rw-rw-rw-   0        0        0    37115 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/text/charclasslib.py
--rw-rw-rw-   0        0        0     8830 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/text/jiebalib.py
--rw-rw-rw-   0        0        0    33455 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/text/jscode.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.293216 pyxllib-0.3.95/pyxllib/text/latex/
--rw-rw-rw-   0        0        0     6416 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/text/latex/__init__.py
--rw-rw-rw-   0        0        0    12259 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/text/levenshtein.py
--rw-rw-rw-   0        0        0    51690 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/text/nestenv.py
--rw-rw-rw-   0        0        0     7335 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/text/newbie.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.294215 pyxllib-0.3.95/pyxllib/text/pupil/
--rw-rw-rw-   0        0        0      217 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/text/pupil/__init__.py
--rw-rw-rw-   0        0        0    37217 2024-02-22 06:22:06.000000 pyxllib-0.3.95/pyxllib/text/pupil/common.py
--rw-rw-rw-   0        0        0    11126 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/text/pupil/xlalign.py
--rw-rw-rw-   0        0        0     1585 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/text/pycode.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.295219 pyxllib-0.3.95/pyxllib/text/specialist/
--rw-rw-rw-   0        0        0      224 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/text/specialist/__init__.py
--rw-rw-rw-   0        0        0     3935 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/text/specialist/common.py
--rw-rw-rw-   0        0        0     6686 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/text/specialist/ptag.py
--rw-rw-rw-   0        0        0     7706 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/text/spellchecker.py
--rw-rw-rw-   0        0        0      514 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/text/vbacode.py
--rw-rw-rw-   0        0        0    26727 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/text/xmllib.py
--rw-rw-rw-   0        0        0     1012 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/xl.py
--rw-rw-rw-   0        0        0      652 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxllib/xlcv.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.243112 pyxllib-0.3.95/pyxllib.egg-info/
--rw-rw-rw-   0        0        0     1057 2024-02-22 06:22:48.000000 pyxllib-0.3.95/pyxllib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    11628 2024-02-22 06:22:49.000000 pyxllib-0.3.95/pyxllib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-22 06:22:48.000000 pyxllib-0.3.95/pyxllib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      334 2024-02-22 06:22:48.000000 pyxllib-0.3.95/pyxllib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-02-22 06:22:48.000000 pyxllib-0.3.95/pyxllib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.297216 pyxllib-0.3.95/pyxlpr/
--rw-rw-rw-   0        0        0      126 2024-01-08 13:05:58.000000 pyxllib-0.3.95/pyxlpr/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.300218 pyxllib-0.3.95/pyxlpr/ai/
--rw-rw-rw-   0        0        0      132 2024-01-08 13:05:58.000000 pyxllib-0.3.95/pyxlpr/ai/__init__.py
--rw-rw-rw-   0        0        0    57362 2024-01-08 13:05:58.000000 pyxllib-0.3.95/pyxlpr/ai/clientlib.py
--rw-rw-rw-   0        0        0     9682 2024-01-08 13:05:58.000000 pyxllib-0.3.95/pyxlpr/ai/specialist.py
--rw-rw-rw-   0        0        0     6591 2024-01-08 13:05:58.000000 pyxllib-0.3.95/pyxlpr/ai/torch_app.py
--rw-rw-rw-   0        0        0    25241 2024-01-08 13:05:58.000000 pyxllib-0.3.95/pyxlpr/ai/xlpaddle.py
--rw-rw-rw-   0        0        0    29450 2024-01-08 13:05:58.000000 pyxllib-0.3.95/pyxlpr/ai/xltorch.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.305216 pyxllib-0.3.95/pyxlpr/data/
--rw-rw-rw-   0        0        0      281 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/data/__init__.py
--rw-rw-rw-   0        0        0    57159 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/data/coco.py
--rw-rw-rw-   0        0        0    14619 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/data/datacls.py
--rw-rw-rw-   0        0        0     8252 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/data/datasets.py
--rw-rw-rw-   0        0        0    53627 2024-01-20 08:31:51.000000 pyxllib-0.3.95/pyxlpr/data/gptlib.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.308214 pyxllib-0.3.95/pyxlpr/data/icdar/
--rw-rw-rw-   0        0        0     4603 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/data/icdar/__init__.py
--rw-rw-rw-   0        0        0    18077 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/data/icdar/deteval.py
--rw-rw-rw-   0        0        0    16306 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/data/icdar/icdar2013.py
--rw-rw-rw-   0        0        0    13859 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/data/icdar/iou.py
--rw-rw-rw-   0        0        0    20202 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/data/icdar/rrc_evaluation_funcs_1_1.py
--rw-rw-rw-   0        0        0    19054 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/data/imtextline.py
--rw-rw-rw-   0        0        0    35626 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/data/labelme.py
--rw-rw-rw-   0        0        0     6499 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/data/removeline.py
--rw-rw-rw-   0        0        0     2066 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/data/specialist.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.308214 pyxllib-0.3.95/pyxlpr/eval/
--rw-rw-rw-   0        0        0     2980 2024-01-08 13:05:58.000000 pyxllib-0.3.95/pyxlpr/eval/__init__.py
--rw-rw-rw-   0        0        0    32303 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/paddleocr.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.309214 pyxllib-0.3.95/pyxlpr/ppocr/
--rw-rw-rw-   0        0        0      651 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.234112 pyxllib-0.3.95/pyxlpr/ppocr/configs/
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.234112 pyxllib-0.3.95/pyxlpr/ppocr/configs/rec/
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.309214 pyxllib-0.3.95/pyxlpr/ppocr/configs/rec/multi_language/
--rw-rw-rw-   0        0        0     8633 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/configs/rec/multi_language/generate_multi_language_configs.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.311215 pyxllib-0.3.95/pyxlpr/ppocr/data/
--rw-rw-rw-   0        0        0     5565 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.320214 pyxllib-0.3.95/pyxlpr/ppocr/data/imaug/
--rw-rw-rw-   0        0        0     1053 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/data/imaug/ColorJitter.py
--rw-rw-rw-   0        0        0     2395 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/data/imaug/__init__.py
--rw-rw-rw-   0        0        0     6655 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/data/imaug/copy_paste.py
--rw-rw-rw-   0        0        0    17757 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/data/imaug/east_process.py
--rw-rw-rw-   0        0        0     9565 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/data/imaug/gen_table_mask.py
--rw-rw-rw-   0        0        0     3791 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/data/imaug/iaa_augment.py
--rw-rw-rw-   0        0        0    28912 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/data/imaug/label_ops.py
--rw-rw-rw-   0        0        0     7144 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/data/imaug/make_border_map.py
--rw-rw-rw-   0        0        0     4008 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/data/imaug/make_pse_gt.py
--rw-rw-rw-   0        0        0     4898 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/data/imaug/make_shrink_map.py
--rw-rw-rw-   0        0        0    15625 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/data/imaug/operators.py
--rw-rw-rw-   0        0        0    36408 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/data/imaug/pg_process.py
--rw-rw-rw-   0        0        0     5591 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/data/imaug/randaugment.py
--rw-rw-rw-   0        0        0     8442 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/data/imaug/random_crop_data.py
--rw-rw-rw-   0        0        0    17398 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/data/imaug/rec_img_aug.py
--rw-rw-rw-   0        0        0    30175 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/data/imaug/sast_process.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.321215 pyxllib-0.3.95/pyxlpr/ppocr/data/imaug/text_image_aug/
--rw-rw-rw-   0        0        0      750 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/data/imaug/text_image_aug/__init__.py
--rw-rw-rw-   0        0        0     3557 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/data/imaug/text_image_aug/augment.py
--rw-rw-rw-   0        0        0     6619 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/data/imaug/text_image_aug/warp_mls.py
--rw-rw-rw-   0        0        0     4485 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/data/lmdb_dataset.py
--rw-rw-rw-   0        0        0     4235 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/data/pgnet_dataset.py
--rw-rw-rw-   0        0        0     4410 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/data/pubtab_dataset.py
--rw-rw-rw-   0        0        0    15429 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/data/simple_dataset.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.331215 pyxllib-0.3.95/pyxlpr/ppocr/losses/
--rw-rw-rw-   0        0        0     1925 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/losses/__init__.py
--rw-rw-rw-   0        0        0     1811 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/losses/ace_loss.py
--rw-rw-rw-   0        0        0     4431 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/losses/basic_loss.py
--rw-rw-rw-   0        0        0     3581 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/losses/center_loss.py
--rw-rw-rw-   0        0        0     1106 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/losses/cls_loss.py
--rw-rw-rw-   0        0        0     2497 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/losses/combined_loss.py
--rw-rw-rw-   0        0        0     7682 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/losses/det_basic_loss.py
--rw-rw-rw-   0        0        0     3245 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/losses/det_db_loss.py
--rw-rw-rw-   0        0        0     2338 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/losses/det_east_loss.py
--rw-rw-rw-   0        0        0     5872 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/losses/det_pse_loss.py
--rw-rw-rw-   0        0        0     5197 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/losses/det_sast_loss.py
--rw-rw-rw-   0        0        0     9741 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/losses/distillation_loss.py
--rw-rw-rw-   0        0        0     6716 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/losses/e2e_pg_loss.py
--rw-rw-rw-   0        0        0     4779 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/losses/kie_sdmgr_loss.py
--rw-rw-rw-   0        0        0     3860 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/losses/rec_aster_loss.py
--rw-rw-rw-   0        0        0     1568 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/losses/rec_att_loss.py
--rw-rw-rw-   0        0        0     1761 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/losses/rec_ctc_loss.py
--rw-rw-rw-   0        0        0     2570 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/losses/rec_enhanced_ctc_loss.py
--rw-rw-rw-   0        0        0     1120 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/losses/rec_nrtr_loss.py
--rw-rw-rw-   0        0        0     1110 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/losses/rec_sar_loss.py
--rw-rw-rw-   0        0        0     1864 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/losses/rec_srn_loss.py
--rw-rw-rw-   0        0        0     4735 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/losses/table_att_loss.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.336214 pyxllib-0.3.95/pyxlpr/ppocr/metrics/
--rw-rw-rw-   0        0        0     1526 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/metrics/__init__.py
--rw-rw-rw-   0        0        0     1497 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/metrics/cls_metric.py
--rw-rw-rw-   0        0        0     3256 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/metrics/det_metric.py
--rw-rw-rw-   0        0        0     2460 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/metrics/distillation_metric.py
--rw-rw-rw-   0        0        0     3278 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/metrics/e2e_metric.py
--rw-rw-rw-   0        0        0    10453 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/metrics/eval_det_iou.py
--rw-rw-rw-   0        0        0     2445 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/metrics/kie_metric.py
--rw-rw-rw-   0        0        0     2637 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/metrics/rec_metric.py
--rw-rw-rw-   0        0        0     1784 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/metrics/table_metric.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.235112 pyxllib-0.3.95/pyxlpr/ppocr/modeling/
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.337222 pyxllib-0.3.95/pyxlpr/ppocr/modeling/architectures/
--rw-rw-rw-   0        0        0     1058 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/architectures/__init__.py
--rw-rw-rw-   0        0        0     3373 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/architectures/base_model.py
--rw-rw-rw-   0        0        0     2406 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/architectures/distillation_model.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.343215 pyxllib-0.3.95/pyxlpr/ppocr/modeling/backbones/
--rw-rw-rw-   0        0        0     2296 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/backbones/__init__.py
--rw-rw-rw-   0        0        0     9218 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/backbones/det_mobilenet_v3.py
--rw-rw-rw-   0        0        0     8164 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/backbones/det_resnet_vd.py
--rw-rw-rw-   0        0        0     9816 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/backbones/det_resnet_vd_sast.py
--rw-rw-rw-   0        0        0     9163 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/backbones/e2e_resnet_vd_pg.py
--rw-rw-rw-   0        0        0     6270 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/backbones/kie_unet_sdmgr.py
--rw-rw-rw-   0        0        0     5677 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/backbones/rec_mobilenet_v3.py
--rw-rw-rw-   0        0        0     8192 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/backbones/rec_mv1_enhance.py
--rw-rw-rw-   0        0        0     1883 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/backbones/rec_nrtr_mtb.py
--rw-rw-rw-   0        0        0     7365 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/backbones/rec_resnet_31.py
--rw-rw-rw-   0        0        0     4714 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/backbones/rec_resnet_aster.py
--rw-rw-rw-   0        0        0    11084 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/backbones/rec_resnet_fpn.py
--rw-rw-rw-   0        0        0     9715 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/backbones/rec_resnet_vd.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.352214 pyxllib-0.3.95/pyxlpr/ppocr/modeling/heads/
--rw-rw-rw-   0        0        0     1799 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/heads/__init__.py
--rw-rw-rw-   0        0        0     1694 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/heads/cls_head.py
--rw-rw-rw-   0        0        0     4333 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/heads/det_db_head.py
--rw-rw-rw-   0        0        0     3836 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/heads/det_east_head.py
--rw-rw-rw-   0        0        0     1374 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/heads/det_pse_head.py
--rw-rw-rw-   0        0        0     4880 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/heads/det_sast_head.py
--rw-rw-rw-   0        0        0     8013 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/heads/e2e_pg_head.py
--rw-rw-rw-   0        0        0     8314 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/heads/kie_sdmgr_head.py
--rw-rw-rw-   0        0        0     6646 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/heads/multiheadAttention.py
--rw-rw-rw-   0        0        0    16232 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/heads/rec_aster_head.py
--rw-rw-rw-   0        0        0     8171 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/heads/rec_att_head.py
--rw-rw-rw-   0        0        0     3014 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/heads/rec_ctc_head.py
--rw-rw-rw-   0        0        0    33928 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/heads/rec_nrtr_head.py
--rw-rw-rw-   0        0        0    14454 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/heads/rec_sar_head.py
--rw-rw-rw-   0        0        0    11171 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/heads/rec_srn_head.py
--rw-rw-rw-   0        0        0    15211 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/heads/self_attention.py
--rw-rw-rw-   0        0        0    10680 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/heads/table_att_head.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.356214 pyxllib-0.3.95/pyxlpr/ppocr/modeling/necks/
--rw-rw-rw-   0        0        0     1230 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/necks/__init__.py
--rw-rw-rw-   0        0        0     4130 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/necks/db_fpn.py
--rw-rw-rw-   0        0        0     6050 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/necks/east_fpn.py
--rw-rw-rw-   0        0        0     5113 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/necks/fpn.py
--rw-rw-rw-   0        0        0    10185 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/necks/pg_fpn.py
--rw-rw-rw-   0        0        0     3149 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/necks/rnn.py
--rw-rw-rw-   0        0        0    11150 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/necks/sast_fpn.py
--rw-rw-rw-   0        0        0     4306 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/necks/table_fpn.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.357219 pyxllib-0.3.95/pyxlpr/ppocr/modeling/transforms/
--rw-rw-rw-   0        0        0     1009 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/transforms/__init__.py
--rw-rw-rw-   0        0        0     5251 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/transforms/stn.py
--rw-rw-rw-   0        0        0    11696 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/transforms/tps.py
--rw-rw-rw-   0        0        0     6923 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/modeling/transforms/tps_spatial_transformer.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.360214 pyxllib-0.3.95/pyxlpr/ppocr/optimizer/
--rw-rw-rw-   0        0        0     2280 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/optimizer/__init__.py
--rw-rw-rw-   0        0        0     8587 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/optimizer/learning_rate.py
--rw-rw-rw-   0        0        0     2036 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/optimizer/lr_scheduler.py
--rw-rw-rw-   0        0        0     5476 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/optimizer/optimizer.py
--rw-rw-rw-   0        0        0     1665 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/optimizer/regularizer.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.364215 pyxllib-0.3.95/pyxlpr/ppocr/postprocess/
--rw-rw-rw-   0        0        0     2201 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/postprocess/__init__.py
--rw-rw-rw-   0        0        0     1323 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/postprocess/cls_postprocess.py
--rw-rw-rw-   0        0        0     8752 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/postprocess/db_postprocess.py
--rw-rw-rw-   0        0        0     5238 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/postprocess/east_postprocess.py
--rw-rw-rw-   0        0        0     5233 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/postprocess/locality_aware_nms.py
--rw-rw-rw-   0        0        0     1872 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/postprocess/pg_postprocess.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.365215 pyxllib-0.3.95/pyxlpr/ppocr/postprocess/pse_postprocess/
--rw-rw-rw-   0        0        0      668 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/postprocess/pse_postprocess/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.366214 pyxllib-0.3.95/pyxlpr/ppocr/postprocess/pse_postprocess/pse/
--rw-rw-rw-   0        0        0     1174 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/postprocess/pse_postprocess/pse/__init__.py
--rw-rw-rw-   0        0        0      340 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/postprocess/pse_postprocess/pse/setup.py
--rw-rw-rw-   0        0        0     4172 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/postprocess/pse_postprocess/pse_postprocess.py
--rw-rw-rw-   0        0        0    25827 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/postprocess/rec_postprocess.py
--rw-rw-rw-   0        0        0    14016 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/postprocess/sast_postprocess.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.372220 pyxllib-0.3.95/pyxlpr/ppocr/tools/
--rw-rw-rw-   0        0        0      708 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/tools/__init__.py
--rw-rw-rw-   0        0        0     3132 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/tools/eval.py
--rw-rw-rw-   0        0        0     2777 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/tools/export_center.py
--rw-rw-rw-   0        0        0     5319 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/tools/export_model.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.375229 pyxllib-0.3.95/pyxlpr/ppocr/tools/infer/
--rw-rw-rw-   0        0        0     5927 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/tools/infer/predict_cls.py
--rw-rw-rw-   0        0        0    11911 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/tools/infer/predict_det.py
--rw-rw-rw-   0        0        0     6501 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/tools/infer/predict_e2e.py
--rw-rw-rw-   0        0        0    17592 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/tools/infer/predict_rec.py
--rw-rw-rw-   0        0        0     7531 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/tools/infer/predict_system.py
--rw-rw-rw-   0        0        0    25355 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/tools/infer/utility.py
--rw-rw-rw-   0        0        0     2747 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/tools/infer_cls.py
--rw-rw-rw-   0        0        0     5009 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/tools/infer_det.py
--rw-rw-rw-   0        0        0     4472 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/tools/infer_e2e.py
--rw-rw-rw-   0        0        0     5558 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/tools/infer_kie.py
--rw-rw-rw-   0        0        0     5865 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/tools/infer_rec.py
--rw-rw-rw-   0        0        0     3842 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/tools/infer_table.py
--rw-rw-rw-   0        0        0    24550 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/tools/program.py
--rw-rw-rw-   0        0        0     4200 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/tools/test_hubserving.py
--rw-rw-rw-   0        0        0     6109 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/tools/train.py
--rw-rw-rw-   0        0        0    33700 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/tools/xlprog.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.383224 pyxllib-0.3.95/pyxlpr/ppocr/utils/
--rw-rw-rw-   0        0        0      280 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/EN_symbol_dict.txt
--rw-rw-rw-   0        0        0      881 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.406696 pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/
--rw-rw-rw-   0        0        0      390 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/ar_dict.txt
--rw-rw-rw-   0        0        0      569 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/arabic_dict.txt
--rw-rw-rw-   0        0        0      502 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/be_dict.txt
--rw-rw-rw-   0        0        0      481 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/bg_dict.txt
--rw-rw-rw-   0        0        0    41864 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/chinese_cht_dict.txt
--rw-rw-rw-   0        0        0      573 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/cyrillic_dict.txt
--rw-rw-rw-   0        0        0      675 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/devanagari_dict.txt
--rw-rw-rw-   0        0        0      189 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/en_dict.txt
--rw-rw-rw-   0        0        0      466 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/fa_dict.txt
--rw-rw-rw-   0        0        0      460 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/french_dict.txt
--rw-rw-rw-   0        0        0      489 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/german_dict.txt
--rw-rw-rw-   0        0        0      650 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/hi_dict.txt
--rw-rw-rw-   0        0        0      384 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/it_dict.txt
--rw-rw-rw-   0        0        0    21731 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/japan_dict.txt
--rw-rw-rw-   0        0        0      606 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/ka_dict.txt
--rw-rw-rw-   0        0        0    18168 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/korean_dict.txt
--rw-rw-rw-   0        0        0      653 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/latin_dict.txt
--rw-rw-rw-   0        0        0      605 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/mr_dict.txt
--rw-rw-rw-   0        0        0      605 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/ne_dict.txt
--rw-rw-rw-   0        0        0      306 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/oc_dict.txt
--rw-rw-rw-   0        0        0      435 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/pu_dict.txt
--rw-rw-rw-   0        0        0      285 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/rs_dict.txt
--rw-rw-rw-   0        0        0      458 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/rsc_dict.txt
--rw-rw-rw-   0        0        0      438 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/ru_dict.txt
--rw-rw-rw-   0        0        0      481 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/ta_dict.txt
--rw-rw-rw-   0        0        0     1171 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/table_dict.txt
--rw-rw-rw-   0        0        0    21350 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/table_structure_dict.txt
--rw-rw-rw-   0        0        0      580 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/te_dict.txt
--rw-rw-rw-   0        0        0      377 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/ug_dict.txt
--rw-rw-rw-   0        0        0      490 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/uk_dict.txt
--rw-rw-rw-   0        0        0      469 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/ur_dict.txt
--rw-rw-rw-   0        0        0      360 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/xi_dict.txt
--rw-rw-rw-   0        0        0      268 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/dict90.txt
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.407696 pyxllib-0.3.95/pyxlpr/ppocr/utils/e2e_metric/
--rw-rw-rw-   0        0        0    26617 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/e2e_metric/Deteval.py
--rw-rw-rw-   0        0        0     2925 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/e2e_metric/polygon_fast.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.410700 pyxllib-0.3.95/pyxlpr/ppocr/utils/e2e_utils/
--rw-rw-rw-   0        0        0     3373 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/e2e_utils/extract_batchsize.py
--rw-rw-rw-   0        0        0    17760 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/e2e_utils/extract_textpoint_fast.py
--rw-rw-rw-   0        0        0    22815 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/e2e_utils/extract_textpoint_slow.py
--rw-rw-rw-   0        0        0     6513 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/e2e_utils/pgnet_pp_utils.py
--rw-rw-rw-   0        0        0     5420 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/e2e_utils/visual.py
--rw-rw-rw-   0        0        0      285 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/en_dict.txt
--rw-rw-rw-   0        0        0     3054 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/gen_label.py
--rw-rw-rw-   0        0        0      106 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/ic15_dict.txt
--rw-rw-rw-   0        0        0     1754 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/iou.py
--rw-rw-rw-   0        0        0     2724 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/logging.py
--rw-rw-rw-   0        0        0     3253 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/network.py
--rw-rw-rw-   0        0        0    32871 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/ppocr_keys_v1.txt
--rw-rw-rw-   0        0        0     4503 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/profiler.py
--rw-rw-rw-   0        0        0     5637 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/save_load.py
--rw-rw-rw-   0        0        0     2304 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/stats.py
--rw-rw-rw-   0        0        0     3160 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/ppocr/utils/utility.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.412696 pyxllib-0.3.95/pyxlpr/ppstructure/
--rw-rw-rw-   0        0        0      621 2024-01-08 13:05:58.000000 pyxllib-0.3.95/pyxlpr/ppstructure/__init__.py
--rw-rw-rw-   0        0        0     7797 2024-01-08 13:05:58.000000 pyxllib-0.3.95/pyxlpr/ppstructure/predict_system.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.415696 pyxllib-0.3.95/pyxlpr/ppstructure/table/
--rw-rw-rw-   0        0        0      621 2024-01-08 13:05:58.000000 pyxllib-0.3.95/pyxlpr/ppstructure/table/__init__.py
--rw-rw-rw-   0        0        0     2377 2024-01-08 13:05:58.000000 pyxllib-0.3.95/pyxlpr/ppstructure/table/eval_table.py
--rw-rw-rw-   0        0        0     7168 2024-01-08 13:05:58.000000 pyxllib-0.3.95/pyxlpr/ppstructure/table/matcher.py
--rw-rw-rw-   0        0        0     4663 2024-01-08 13:05:58.000000 pyxllib-0.3.95/pyxlpr/ppstructure/table/predict_structure.py
--rw-rw-rw-   0        0        0     8851 2024-01-08 13:05:58.000000 pyxllib-0.3.95/pyxlpr/ppstructure/table/predict_table.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.417696 pyxllib-0.3.95/pyxlpr/ppstructure/table/table_metric/
--rw-rw-rw-   0        0        0      673 2024-01-08 13:05:58.000000 pyxllib-0.3.95/pyxlpr/ppstructure/table/table_metric/__init__.py
--rw-rw-rw-   0        0        0     2198 2024-01-08 13:05:58.000000 pyxllib-0.3.95/pyxlpr/ppstructure/table/table_metric/parallel.py
--rw-rw-rw-   0        0        0     9532 2024-01-08 13:05:58.000000 pyxllib-0.3.95/pyxlpr/ppstructure/table/table_metric/table_metric.py
-drwxrwxrwx   0        0        0        0 2024-02-22 06:22:49.418696 pyxllib-0.3.95/pyxlpr/ppstructure/table/tablepyxl/
--rw-rw-rw-   0        0        0      619 2024-01-08 13:05:58.000000 pyxllib-0.3.95/pyxlpr/ppstructure/table/tablepyxl/__init__.py
--rw-rw-rw-   0        0        0    10415 2024-01-08 13:05:58.000000 pyxllib-0.3.95/pyxlpr/ppstructure/table/tablepyxl/style.py
--rw-rw-rw-   0        0        0     4217 2024-01-08 13:05:58.000000 pyxllib-0.3.95/pyxlpr/ppstructure/table/tablepyxl/tablepyxl.py
--rw-rw-rw-   0        0        0     2538 2024-01-08 13:05:58.000000 pyxllib-0.3.95/pyxlpr/ppstructure/utility.py
--rw-rw-rw-   0        0        0      260 2024-01-08 13:05:59.000000 pyxllib-0.3.95/pyxlpr/xlai.py
--rw-rw-rw-   0        0        0      223 2024-01-08 13:05:59.000000 pyxllib-0.3.95/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-02-22 06:22:49.419696 pyxllib-0.3.95/setup.cfg
--rw-rw-rw-   0        0        0     2478 2024-02-22 06:22:48.000000 pyxllib-0.3.95/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.984533 pyxllib-0.3.96/
+-rw-rw-rw-   0        0        0    10443 2024-01-08 12:52:36.000000 pyxllib-0.3.96/LICENSE
+-rw-rw-rw-   0        0        0       80 2024-01-08 12:52:36.000000 pyxllib-0.3.96/MANIFEST.in
+-rw-rw-rw-   0        0        0      612 2024-03-06 02:59:49.983533 pyxllib-0.3.96/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2024-02-27 07:18:24.000000 pyxllib-0.3.96/README.md
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.835274 pyxllib-0.3.96/pyxllib/
+-rw-rw-rw-   0        0        0      529 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.844274 pyxllib-0.3.96/pyxllib/algo/
+-rw-rw-rw-   0        0        0      161 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/algo/__init__.py
+-rw-rw-rw-   0        0        0     1450 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/algo/disjoint.py
+-rw-rw-rw-   0        0        0    18190 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/algo/geo.py
+-rw-rw-rw-   0        0        0    36718 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/algo/intervals.py
+-rw-rw-rw-   0        0        0    12600 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/algo/matcher.py
+-rw-rw-rw-   0        0        0     4168 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/algo/newbie.py
+-rw-rw-rw-   0        0        0    17029 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/algo/pupil.py
+-rw-rw-rw-   0        0        0     2393 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/algo/shapelylib.py
+-rw-rw-rw-   0        0        0     8584 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/algo/specialist.py
+-rw-rw-rw-   0        0        0    18383 2024-02-26 16:00:04.000000 pyxllib-0.3.96/pyxllib/algo/stat.py
+-rw-rw-rw-   0        0        0     5094 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/algo/treelib.py
+-rw-rw-rw-   0        0        0     1953 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/algo/unitlib.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.848274 pyxllib-0.3.96/pyxllib/cv/
+-rw-rw-rw-   0        0        0      132 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/cv/__init__.py
+-rw-rw-rw-   0        0        0    11378 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/cv/expert.py
+-rw-rw-rw-   0        0        0     6757 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/cv/imfile.py
+-rw-rw-rw-   0        0        0      977 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/cv/imhash.py
+-rw-rw-rw-   0        0        0      339 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/cv/pupil.py
+-rw-rw-rw-   0        0        0    38270 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/cv/rgbfmt.py
+-rw-rw-rw-   0        0        0     9259 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/cv/trackbartools.py
+-rw-rw-rw-   0        0        0    40787 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/cv/xlcvlib.py
+-rw-rw-rw-   0        0        0    15454 2024-01-11 16:11:21.000000 pyxllib-0.3.96/pyxllib/cv/xlpillib.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.851325 pyxllib-0.3.96/pyxllib/data/
+-rw-rw-rw-   0        0        0        0 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/data/__init__.py
+-rw-rw-rw-   0        0        0     3933 2024-03-06 02:38:28.000000 pyxllib-0.3.96/pyxllib/data/echarts.py
+-rw-rw-rw-   0        0        0     2477 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/data/oss.py
+-rw-rw-rw-   0        0        0    28830 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/data/pglib.py
+-rw-rw-rw-   0        0        0    12791 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/data/sqlite.py
+-rw-rw-rw-   0        0        0    11955 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/data/sqllib.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.857845 pyxllib-0.3.96/pyxllib/ext/
+-rw-rw-rw-   0        0        0    19419 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/ext/JLineViewer.py
+-rw-rw-rw-   0        0        0      134 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/ext/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.858841 pyxllib-0.3.96/pyxllib/ext/autogui/
+-rw-rw-rw-   0        0        0      223 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/ext/autogui/__init__.py
+-rw-rw-rw-   0        0        0    29612 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/ext/autogui/autogui.py
+-rw-rw-rw-   0        0        0     3654 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/ext/autogui/virtualkey.py
+-rw-rw-rw-   0        0        0     8552 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/ext/demolib.py
+-rw-rw-rw-   0        0        0    72416 2024-02-26 10:49:54.000000 pyxllib-0.3.96/pyxllib/ext/kq5034lib.py
+-rw-rw-rw-   0        0        0    27407 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/ext/old.py
+-rw-rw-rw-   0        0        0    16090 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/ext/qt.py
+-rw-rw-rw-   0        0        0     2771 2024-01-24 09:13:45.000000 pyxllib-0.3.96/pyxllib/ext/seleniumlib.py
+-rw-rw-rw-   0        0        0     5004 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/ext/tk.py
+-rw-rw-rw-   0        0        0    34850 2024-03-06 02:38:05.000000 pyxllib-0.3.96/pyxllib/ext/unixlib.py
+-rw-rw-rw-   0        0        0    13663 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/ext/utools.py
+-rw-rw-rw-   0        0        0     3458 2024-02-26 14:12:56.000000 pyxllib-0.3.96/pyxllib/ext/webhook.py
+-rw-rw-rw-   0        0        0     1237 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/ext/win32lib.py
+-rw-rw-rw-   0        0        0     5857 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/ext/yuquelib.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.863840 pyxllib-0.3.96/pyxllib/file/
+-rw-rw-rw-   0        0        0      452 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/file/__init__.py
+-rw-rw-rw-   0        0        0    29778 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/file/docxlib.py
+-rw-rw-rw-   0        0        0    11620 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/file/gitlib.py
+-rw-rw-rw-   0        0        0     5880 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/file/movielib.py
+-rw-rw-rw-   0        0        0      218 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/file/newbie.py
+-rw-rw-rw-   0        0        0    55027 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/file/onenotelib.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.864840 pyxllib-0.3.96/pyxllib/file/packlib/
+-rw-rw-rw-   0        0        0    11464 2024-01-10 13:03:47.000000 pyxllib-0.3.96/pyxllib/file/packlib/__init__.py
+-rw-rw-rw-   0        0        0    90165 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/file/packlib/zipfile.py
+-rw-rw-rw-   0        0        0    17010 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/file/pdflib.py
+-rw-rw-rw-   0        0        0     5997 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/file/pupil.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.867840 pyxllib-0.3.96/pyxllib/file/specialist/
+-rw-rw-rw-   0        0        0    28260 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/file/specialist/__init__.py
+-rw-rw-rw-   0        0        0    32411 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/file/specialist/dirlib.py
+-rw-rw-rw-   0        0        0     6763 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/file/specialist/download.py
+-rw-rw-rw-   0        0        0   101158 2024-01-12 08:19:59.000000 pyxllib-0.3.96/pyxllib/file/specialist/filelib.py
+-rw-rw-rw-   0        0        0   125754 2024-02-29 09:14:19.000000 pyxllib-0.3.96/pyxllib/file/xlsxlib.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.871841 pyxllib-0.3.96/pyxllib/prog/
+-rw-rw-rw-   0        0        0      132 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/prog/__init__.py
+-rw-rw-rw-   0        0        0     8499 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/prog/deprecatedlib.py
+-rw-rw-rw-   0        0        0     9229 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/prog/ipyexec.py
+-rw-rw-rw-   0        0        0    15005 2024-01-13 15:01:52.000000 pyxllib-0.3.96/pyxllib/prog/newbie.py
+-rw-rw-rw-   0        0        0    43196 2024-01-23 12:35:18.000000 pyxllib-0.3.96/pyxllib/prog/pupil.py
+-rw-rw-rw-   0        0        0      996 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/prog/sitepackages.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.874841 pyxllib-0.3.96/pyxllib/prog/specialist/
+-rw-rw-rw-   0        0        0     7913 2024-02-26 15:27:55.000000 pyxllib-0.3.96/pyxllib/prog/specialist/__init__.py
+-rw-rw-rw-   0        0        0     9657 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/prog/specialist/bc.py
+-rw-rw-rw-   0        0        0    19868 2024-02-19 15:29:00.000000 pyxllib-0.3.96/pyxllib/prog/specialist/browser.py
+-rw-rw-rw-   0        0        0    13309 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/prog/specialist/common.py
+-rw-rw-rw-   0        0        0     4525 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/prog/specialist/datetime.py
+-rw-rw-rw-   0        0        0     8206 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/prog/specialist/tictoc.py
+-rw-rw-rw-   0        0        0     8298 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/prog/specialist/xllog.py
+-rw-rw-rw-   0        0        0     3669 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/prog/xlosenv.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.875840 pyxllib-0.3.96/pyxllib/stdlib/
+-rw-rw-rw-   0        0        0      581 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/stdlib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.876840 pyxllib-0.3.96/pyxllib/stdlib/tablepyxl/
+-rw-rw-rw-   0        0        0      193 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/stdlib/tablepyxl/__init__.py
+-rw-rw-rw-   0        0        0    10924 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/stdlib/tablepyxl/style.py
+-rw-rw-rw-   0        0        0     4531 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/stdlib/tablepyxl/tablepyxl.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.882841 pyxllib-0.3.96/pyxllib/text/
+-rw-rw-rw-   0        0        0      170 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/text/__init__.py
+-rw-rw-rw-   0        0        0     1259 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/text/ahocorasick.py
+-rw-rw-rw-   0        0        0    37115 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/text/charclasslib.py
+-rw-rw-rw-   0        0        0     8830 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/text/jiebalib.py
+-rw-rw-rw-   0        0        0    33455 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/text/jscode.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.883841 pyxllib-0.3.96/pyxllib/text/latex/
+-rw-rw-rw-   0        0        0     6416 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/text/latex/__init__.py
+-rw-rw-rw-   0        0        0    12259 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/text/levenshtein.py
+-rw-rw-rw-   0        0        0    51690 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/text/nestenv.py
+-rw-rw-rw-   0        0        0     7335 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/text/newbie.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.884840 pyxllib-0.3.96/pyxllib/text/pupil/
+-rw-rw-rw-   0        0        0      217 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/text/pupil/__init__.py
+-rw-rw-rw-   0        0        0    37217 2024-02-22 15:39:37.000000 pyxllib-0.3.96/pyxllib/text/pupil/common.py
+-rw-rw-rw-   0        0        0    11126 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/text/pupil/xlalign.py
+-rw-rw-rw-   0        0        0     1585 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/text/pycode.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.885841 pyxllib-0.3.96/pyxllib/text/specialist/
+-rw-rw-rw-   0        0        0      224 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/text/specialist/__init__.py
+-rw-rw-rw-   0        0        0     3935 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/text/specialist/common.py
+-rw-rw-rw-   0        0        0     6686 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/text/specialist/ptag.py
+-rw-rw-rw-   0        0        0     7706 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/text/spellchecker.py
+-rw-rw-rw-   0        0        0      514 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/text/vbacode.py
+-rw-rw-rw-   0        0        0    26727 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/text/xmllib.py
+-rw-rw-rw-   0        0        0     1012 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/xl.py
+-rw-rw-rw-   0        0        0      652 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxllib/xlcv.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.838274 pyxllib-0.3.96/pyxllib.egg-info/
+-rw-rw-rw-   0        0        0      612 2024-03-06 02:59:49.000000 pyxllib-0.3.96/pyxllib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    11628 2024-03-06 02:59:49.000000 pyxllib-0.3.96/pyxllib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-06 02:59:49.000000 pyxllib-0.3.96/pyxllib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      334 2024-03-06 02:59:49.000000 pyxllib-0.3.96/pyxllib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-03-06 02:59:49.000000 pyxllib-0.3.96/pyxllib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.886845 pyxllib-0.3.96/pyxlpr/
+-rw-rw-rw-   0        0        0      126 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.889840 pyxllib-0.3.96/pyxlpr/ai/
+-rw-rw-rw-   0        0        0      132 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ai/__init__.py
+-rw-rw-rw-   0        0        0    57362 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ai/clientlib.py
+-rw-rw-rw-   0        0        0     9682 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ai/specialist.py
+-rw-rw-rw-   0        0        0     6591 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ai/torch_app.py
+-rw-rw-rw-   0        0        0    25241 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ai/xlpaddle.py
+-rw-rw-rw-   0        0        0    29450 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ai/xltorch.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.894840 pyxllib-0.3.96/pyxlpr/data/
+-rw-rw-rw-   0        0        0      281 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/data/__init__.py
+-rw-rw-rw-   0        0        0    57159 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/data/coco.py
+-rw-rw-rw-   0        0        0    14619 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/data/datacls.py
+-rw-rw-rw-   0        0        0     8252 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/data/datasets.py
+-rw-rw-rw-   0        0        0    53627 2024-01-20 08:31:51.000000 pyxllib-0.3.96/pyxlpr/data/gptlib.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.896840 pyxllib-0.3.96/pyxlpr/data/icdar/
+-rw-rw-rw-   0        0        0     4603 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/data/icdar/__init__.py
+-rw-rw-rw-   0        0        0    18077 2024-01-08 13:01:03.000000 pyxllib-0.3.96/pyxlpr/data/icdar/deteval.py
+-rw-rw-rw-   0        0        0    16306 2024-01-08 13:01:03.000000 pyxllib-0.3.96/pyxlpr/data/icdar/icdar2013.py
+-rw-rw-rw-   0        0        0    13859 2024-01-08 13:01:03.000000 pyxllib-0.3.96/pyxlpr/data/icdar/iou.py
+-rw-rw-rw-   0        0        0    20202 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/data/icdar/rrc_evaluation_funcs_1_1.py
+-rw-rw-rw-   0        0        0    19054 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/data/imtextline.py
+-rw-rw-rw-   0        0        0    35626 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/data/labelme.py
+-rw-rw-rw-   0        0        0     6499 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/data/removeline.py
+-rw-rw-rw-   0        0        0     2066 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/data/specialist.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.896840 pyxllib-0.3.96/pyxlpr/eval/
+-rw-rw-rw-   0        0        0     2980 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/eval/__init__.py
+-rw-rw-rw-   0        0        0    32303 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/paddleocr.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.897840 pyxllib-0.3.96/pyxlpr/ppocr/
+-rw-rw-rw-   0        0        0      651 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.830274 pyxllib-0.3.96/pyxlpr/ppocr/configs/
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.830274 pyxllib-0.3.96/pyxlpr/ppocr/configs/rec/
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.897840 pyxllib-0.3.96/pyxlpr/ppocr/configs/rec/multi_language/
+-rw-rw-rw-   0        0        0     8633 2021-11-11 08:55:03.000000 pyxllib-0.3.96/pyxlpr/ppocr/configs/rec/multi_language/generate_multi_language_configs.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.900840 pyxllib-0.3.96/pyxlpr/ppocr/data/
+-rw-rw-rw-   0        0        0     5565 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.907877 pyxllib-0.3.96/pyxlpr/ppocr/data/imaug/
+-rw-rw-rw-   0        0        0     1053 2022-01-14 02:17:07.000000 pyxllib-0.3.96/pyxlpr/ppocr/data/imaug/ColorJitter.py
+-rw-rw-rw-   0        0        0     2395 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/data/imaug/__init__.py
+-rw-rw-rw-   0        0        0     6655 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/data/imaug/copy_paste.py
+-rw-rw-rw-   0        0        0    17757 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/data/imaug/east_process.py
+-rw-rw-rw-   0        0        0     9565 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/data/imaug/gen_table_mask.py
+-rw-rw-rw-   0        0        0     3791 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/data/imaug/iaa_augment.py
+-rw-rw-rw-   0        0        0    28912 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/data/imaug/label_ops.py
+-rw-rw-rw-   0        0        0     7144 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/data/imaug/make_border_map.py
+-rw-rw-rw-   0        0        0     4008 2022-01-14 02:17:07.000000 pyxllib-0.3.96/pyxlpr/ppocr/data/imaug/make_pse_gt.py
+-rw-rw-rw-   0        0        0     4898 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/data/imaug/make_shrink_map.py
+-rw-rw-rw-   0        0        0    15625 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/data/imaug/operators.py
+-rw-rw-rw-   0        0        0    36408 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/data/imaug/pg_process.py
+-rw-rw-rw-   0        0        0     5591 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/data/imaug/randaugment.py
+-rw-rw-rw-   0        0        0     8442 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/data/imaug/random_crop_data.py
+-rw-rw-rw-   0        0        0    17398 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/data/imaug/rec_img_aug.py
+-rw-rw-rw-   0        0        0    30175 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/data/imaug/sast_process.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.909840 pyxllib-0.3.96/pyxlpr/ppocr/data/imaug/text_image_aug/
+-rw-rw-rw-   0        0        0      750 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/data/imaug/text_image_aug/__init__.py
+-rw-rw-rw-   0        0        0     3557 2022-01-14 02:17:07.000000 pyxllib-0.3.96/pyxlpr/ppocr/data/imaug/text_image_aug/augment.py
+-rw-rw-rw-   0        0        0     6619 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/data/imaug/text_image_aug/warp_mls.py
+-rw-rw-rw-   0        0        0     4485 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/data/lmdb_dataset.py
+-rw-rw-rw-   0        0        0     4235 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/data/pgnet_dataset.py
+-rw-rw-rw-   0        0        0     4410 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/data/pubtab_dataset.py
+-rw-rw-rw-   0        0        0    15429 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/data/simple_dataset.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.919842 pyxllib-0.3.96/pyxlpr/ppocr/losses/
+-rw-rw-rw-   0        0        0     1925 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/losses/__init__.py
+-rw-rw-rw-   0        0        0     1811 2022-01-14 02:17:07.000000 pyxllib-0.3.96/pyxlpr/ppocr/losses/ace_loss.py
+-rw-rw-rw-   0        0        0     4431 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/losses/basic_loss.py
+-rw-rw-rw-   0        0        0     3581 2022-01-14 02:17:07.000000 pyxllib-0.3.96/pyxlpr/ppocr/losses/center_loss.py
+-rw-rw-rw-   0        0        0     1106 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/losses/cls_loss.py
+-rw-rw-rw-   0        0        0     2497 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/losses/combined_loss.py
+-rw-rw-rw-   0        0        0     7682 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/losses/det_basic_loss.py
+-rw-rw-rw-   0        0        0     3245 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/losses/det_db_loss.py
+-rw-rw-rw-   0        0        0     2338 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/losses/det_east_loss.py
+-rw-rw-rw-   0        0        0     5872 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/losses/det_pse_loss.py
+-rw-rw-rw-   0        0        0     5197 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/losses/det_sast_loss.py
+-rw-rw-rw-   0        0        0     9741 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/losses/distillation_loss.py
+-rw-rw-rw-   0        0        0     6716 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/losses/e2e_pg_loss.py
+-rw-rw-rw-   0        0        0     4779 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/losses/kie_sdmgr_loss.py
+-rw-rw-rw-   0        0        0     3860 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/losses/rec_aster_loss.py
+-rw-rw-rw-   0        0        0     1568 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/losses/rec_att_loss.py
+-rw-rw-rw-   0        0        0     1761 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/losses/rec_ctc_loss.py
+-rw-rw-rw-   0        0        0     2570 2022-01-14 02:17:07.000000 pyxllib-0.3.96/pyxlpr/ppocr/losses/rec_enhanced_ctc_loss.py
+-rw-rw-rw-   0        0        0     1120 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/losses/rec_nrtr_loss.py
+-rw-rw-rw-   0        0        0     1110 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/losses/rec_sar_loss.py
+-rw-rw-rw-   0        0        0     1864 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/losses/rec_srn_loss.py
+-rw-rw-rw-   0        0        0     4735 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/losses/table_att_loss.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.923842 pyxllib-0.3.96/pyxlpr/ppocr/metrics/
+-rw-rw-rw-   0        0        0     1526 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/metrics/__init__.py
+-rw-rw-rw-   0        0        0     1497 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/metrics/cls_metric.py
+-rw-rw-rw-   0        0        0     3256 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/metrics/det_metric.py
+-rw-rw-rw-   0        0        0     2460 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/metrics/distillation_metric.py
+-rw-rw-rw-   0        0        0     3278 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/metrics/e2e_metric.py
+-rw-rw-rw-   0        0        0    10453 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/metrics/eval_det_iou.py
+-rw-rw-rw-   0        0        0     2445 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/metrics/kie_metric.py
+-rw-rw-rw-   0        0        0     2637 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/metrics/rec_metric.py
+-rw-rw-rw-   0        0        0     1784 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/metrics/table_metric.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.831274 pyxllib-0.3.96/pyxlpr/ppocr/modeling/
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.925842 pyxllib-0.3.96/pyxlpr/ppocr/modeling/architectures/
+-rw-rw-rw-   0        0        0     1058 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/architectures/__init__.py
+-rw-rw-rw-   0        0        0     3373 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/architectures/base_model.py
+-rw-rw-rw-   0        0        0     2406 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/architectures/distillation_model.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.931356 pyxllib-0.3.96/pyxlpr/ppocr/modeling/backbones/
+-rw-rw-rw-   0        0        0     2296 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/backbones/__init__.py
+-rw-rw-rw-   0        0        0     9218 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/backbones/det_mobilenet_v3.py
+-rw-rw-rw-   0        0        0     8164 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/backbones/det_resnet_vd.py
+-rw-rw-rw-   0        0        0     9816 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/backbones/det_resnet_vd_sast.py
+-rw-rw-rw-   0        0        0     9163 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/backbones/e2e_resnet_vd_pg.py
+-rw-rw-rw-   0        0        0     6270 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/backbones/kie_unet_sdmgr.py
+-rw-rw-rw-   0        0        0     5677 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/backbones/rec_mobilenet_v3.py
+-rw-rw-rw-   0        0        0     8192 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/backbones/rec_mv1_enhance.py
+-rw-rw-rw-   0        0        0     1883 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/backbones/rec_nrtr_mtb.py
+-rw-rw-rw-   0        0        0     7365 2022-01-14 02:17:07.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/backbones/rec_resnet_31.py
+-rw-rw-rw-   0        0        0     4714 2022-01-14 02:17:07.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/backbones/rec_resnet_aster.py
+-rw-rw-rw-   0        0        0    11084 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/backbones/rec_resnet_fpn.py
+-rw-rw-rw-   0        0        0     9715 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/backbones/rec_resnet_vd.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.937533 pyxllib-0.3.96/pyxlpr/ppocr/modeling/heads/
+-rw-rw-rw-   0        0        0     1799 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/heads/__init__.py
+-rw-rw-rw-   0        0        0     1694 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/heads/cls_head.py
+-rw-rw-rw-   0        0        0     4333 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/heads/det_db_head.py
+-rw-rw-rw-   0        0        0     3836 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/heads/det_east_head.py
+-rw-rw-rw-   0        0        0     1374 2022-01-14 02:17:07.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/heads/det_pse_head.py
+-rw-rw-rw-   0        0        0     4880 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/heads/det_sast_head.py
+-rw-rw-rw-   0        0        0     8013 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/heads/e2e_pg_head.py
+-rw-rw-rw-   0        0        0     8314 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/heads/kie_sdmgr_head.py
+-rw-rw-rw-   0        0        0     6646 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/heads/multiheadAttention.py
+-rw-rw-rw-   0        0        0    16232 2022-01-14 02:17:07.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/heads/rec_aster_head.py
+-rw-rw-rw-   0        0        0     8171 2022-01-14 02:17:07.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/heads/rec_att_head.py
+-rw-rw-rw-   0        0        0     3014 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/heads/rec_ctc_head.py
+-rw-rw-rw-   0        0        0    33928 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/heads/rec_nrtr_head.py
+-rw-rw-rw-   0        0        0    14454 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/heads/rec_sar_head.py
+-rw-rw-rw-   0        0        0    11171 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/heads/rec_srn_head.py
+-rw-rw-rw-   0        0        0    15211 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/heads/self_attention.py
+-rw-rw-rw-   0        0        0    10680 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/heads/table_att_head.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.941552 pyxllib-0.3.96/pyxlpr/ppocr/modeling/necks/
+-rw-rw-rw-   0        0        0     1230 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/necks/__init__.py
+-rw-rw-rw-   0        0        0     4130 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/necks/db_fpn.py
+-rw-rw-rw-   0        0        0     6050 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/necks/east_fpn.py
+-rw-rw-rw-   0        0        0     5113 2022-01-14 02:17:07.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/necks/fpn.py
+-rw-rw-rw-   0        0        0    10185 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/necks/pg_fpn.py
+-rw-rw-rw-   0        0        0     3149 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/necks/rnn.py
+-rw-rw-rw-   0        0        0    11150 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/necks/sast_fpn.py
+-rw-rw-rw-   0        0        0     4306 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/necks/table_fpn.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.942533 pyxllib-0.3.96/pyxlpr/ppocr/modeling/transforms/
+-rw-rw-rw-   0        0        0     1009 2022-01-14 02:17:07.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/transforms/__init__.py
+-rw-rw-rw-   0        0        0     5251 2022-01-14 02:17:07.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/transforms/stn.py
+-rw-rw-rw-   0        0        0    11696 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/transforms/tps.py
+-rw-rw-rw-   0        0        0     6923 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/modeling/transforms/tps_spatial_transformer.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.944536 pyxllib-0.3.96/pyxlpr/ppocr/optimizer/
+-rw-rw-rw-   0        0        0     2280 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/optimizer/__init__.py
+-rw-rw-rw-   0        0        0     8587 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/optimizer/learning_rate.py
+-rw-rw-rw-   0        0        0     2036 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/optimizer/lr_scheduler.py
+-rw-rw-rw-   0        0        0     5476 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/optimizer/optimizer.py
+-rw-rw-rw-   0        0        0     1665 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/optimizer/regularizer.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.948534 pyxllib-0.3.96/pyxlpr/ppocr/postprocess/
+-rw-rw-rw-   0        0        0     2201 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/postprocess/__init__.py
+-rw-rw-rw-   0        0        0     1323 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/postprocess/cls_postprocess.py
+-rw-rw-rw-   0        0        0     8752 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/postprocess/db_postprocess.py
+-rw-rw-rw-   0        0        0     5238 2022-01-14 02:17:07.000000 pyxllib-0.3.96/pyxlpr/ppocr/postprocess/east_postprocess.py
+-rw-rw-rw-   0        0        0     5233 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/postprocess/locality_aware_nms.py
+-rw-rw-rw-   0        0        0     1872 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/postprocess/pg_postprocess.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.948534 pyxllib-0.3.96/pyxlpr/ppocr/postprocess/pse_postprocess/
+-rw-rw-rw-   0        0        0      668 2022-01-14 02:17:07.000000 pyxllib-0.3.96/pyxlpr/ppocr/postprocess/pse_postprocess/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.949533 pyxllib-0.3.96/pyxlpr/ppocr/postprocess/pse_postprocess/pse/
+-rw-rw-rw-   0        0        0     1174 2022-01-14 02:17:07.000000 pyxllib-0.3.96/pyxlpr/ppocr/postprocess/pse_postprocess/pse/__init__.py
+-rw-rw-rw-   0        0        0      340 2022-01-14 02:17:07.000000 pyxllib-0.3.96/pyxlpr/ppocr/postprocess/pse_postprocess/pse/setup.py
+-rw-rw-rw-   0        0        0     4172 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/postprocess/pse_postprocess/pse_postprocess.py
+-rw-rw-rw-   0        0        0    25827 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/postprocess/rec_postprocess.py
+-rw-rw-rw-   0        0        0    14016 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/postprocess/sast_postprocess.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.955533 pyxllib-0.3.96/pyxlpr/ppocr/tools/
+-rw-rw-rw-   0        0        0      708 2022-01-14 02:17:07.000000 pyxllib-0.3.96/pyxlpr/ppocr/tools/__init__.py
+-rw-rw-rw-   0        0        0     3132 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/tools/eval.py
+-rw-rw-rw-   0        0        0     2777 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/tools/export_center.py
+-rw-rw-rw-   0        0        0     5319 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/tools/export_model.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.957534 pyxllib-0.3.96/pyxlpr/ppocr/tools/infer/
+-rw-rw-rw-   0        0        0     5927 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/tools/infer/predict_cls.py
+-rw-rw-rw-   0        0        0    11911 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/tools/infer/predict_det.py
+-rw-rw-rw-   0        0        0     6501 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/tools/infer/predict_e2e.py
+-rw-rw-rw-   0        0        0    17592 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/tools/infer/predict_rec.py
+-rw-rw-rw-   0        0        0     7531 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/tools/infer/predict_system.py
+-rw-rw-rw-   0        0        0    25355 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/tools/infer/utility.py
+-rw-rw-rw-   0        0        0     2747 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/tools/infer_cls.py
+-rw-rw-rw-   0        0        0     5009 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/tools/infer_det.py
+-rw-rw-rw-   0        0        0     4472 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/tools/infer_e2e.py
+-rw-rw-rw-   0        0        0     5558 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/tools/infer_kie.py
+-rw-rw-rw-   0        0        0     5865 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/tools/infer_rec.py
+-rw-rw-rw-   0        0        0     3842 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/tools/infer_table.py
+-rw-rw-rw-   0        0        0    24550 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/tools/program.py
+-rw-rw-rw-   0        0        0     4200 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/tools/test_hubserving.py
+-rw-rw-rw-   0        0        0     6109 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/tools/train.py
+-rw-rw-rw-   0        0        0    33700 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/tools/xlprog.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.962533 pyxllib-0.3.96/pyxlpr/ppocr/utils/
+-rw-rw-rw-   0        0        0      280 2022-01-14 02:17:07.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/EN_symbol_dict.txt
+-rw-rw-rw-   0        0        0      881 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.975533 pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/
+-rw-rw-rw-   0        0        0      390 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/ar_dict.txt
+-rw-rw-rw-   0        0        0      569 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/arabic_dict.txt
+-rw-rw-rw-   0        0        0      502 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/be_dict.txt
+-rw-rw-rw-   0        0        0      481 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/bg_dict.txt
+-rw-rw-rw-   0        0        0    41864 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/chinese_cht_dict.txt
+-rw-rw-rw-   0        0        0      573 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/cyrillic_dict.txt
+-rw-rw-rw-   0        0        0      675 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/devanagari_dict.txt
+-rw-rw-rw-   0        0        0      189 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/en_dict.txt
+-rw-rw-rw-   0        0        0      466 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/fa_dict.txt
+-rw-rw-rw-   0        0        0      460 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/french_dict.txt
+-rw-rw-rw-   0        0        0      489 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/german_dict.txt
+-rw-rw-rw-   0        0        0      650 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/hi_dict.txt
+-rw-rw-rw-   0        0        0      384 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/it_dict.txt
+-rw-rw-rw-   0        0        0    21731 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/japan_dict.txt
+-rw-rw-rw-   0        0        0      606 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/ka_dict.txt
+-rw-rw-rw-   0        0        0    18168 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/korean_dict.txt
+-rw-rw-rw-   0        0        0      653 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/latin_dict.txt
+-rw-rw-rw-   0        0        0      605 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/mr_dict.txt
+-rw-rw-rw-   0        0        0      605 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/ne_dict.txt
+-rw-rw-rw-   0        0        0      306 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/oc_dict.txt
+-rw-rw-rw-   0        0        0      435 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/pu_dict.txt
+-rw-rw-rw-   0        0        0      285 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/rs_dict.txt
+-rw-rw-rw-   0        0        0      458 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/rsc_dict.txt
+-rw-rw-rw-   0        0        0      438 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/ru_dict.txt
+-rw-rw-rw-   0        0        0      481 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/ta_dict.txt
+-rw-rw-rw-   0        0        0     1171 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/table_dict.txt
+-rw-rw-rw-   0        0        0    21350 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/table_structure_dict.txt
+-rw-rw-rw-   0        0        0      580 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/te_dict.txt
+-rw-rw-rw-   0        0        0      377 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/ug_dict.txt
+-rw-rw-rw-   0        0        0      490 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/uk_dict.txt
+-rw-rw-rw-   0        0        0      469 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/ur_dict.txt
+-rw-rw-rw-   0        0        0      360 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/xi_dict.txt
+-rw-rw-rw-   0        0        0      268 2022-01-14 02:17:07.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/dict90.txt
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.976534 pyxllib-0.3.96/pyxlpr/ppocr/utils/e2e_metric/
+-rw-rw-rw-   0        0        0    26617 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/e2e_metric/Deteval.py
+-rw-rw-rw-   0        0        0     2925 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/e2e_metric/polygon_fast.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.977533 pyxllib-0.3.96/pyxlpr/ppocr/utils/e2e_utils/
+-rw-rw-rw-   0        0        0     3373 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/e2e_utils/extract_batchsize.py
+-rw-rw-rw-   0        0        0    17760 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/e2e_utils/extract_textpoint_fast.py
+-rw-rw-rw-   0        0        0    22815 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/e2e_utils/extract_textpoint_slow.py
+-rw-rw-rw-   0        0        0     6513 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/e2e_utils/pgnet_pp_utils.py
+-rw-rw-rw-   0        0        0     5420 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/e2e_utils/visual.py
+-rw-rw-rw-   0        0        0      285 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/en_dict.txt
+-rw-rw-rw-   0        0        0     3054 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/gen_label.py
+-rw-rw-rw-   0        0        0      106 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/ic15_dict.txt
+-rw-rw-rw-   0        0        0     1754 2022-01-14 02:17:07.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/iou.py
+-rw-rw-rw-   0        0        0     2724 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/logging.py
+-rw-rw-rw-   0        0        0     3253 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/network.py
+-rw-rw-rw-   0        0        0    32871 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/ppocr_keys_v1.txt
+-rw-rw-rw-   0        0        0     4503 2022-01-14 02:17:07.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/profiler.py
+-rw-rw-rw-   0        0        0     5637 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/save_load.py
+-rw-rw-rw-   0        0        0     2304 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/stats.py
+-rw-rw-rw-   0        0        0     3160 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppocr/utils/utility.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.979533 pyxllib-0.3.96/pyxlpr/ppstructure/
+-rw-rw-rw-   0        0        0      621 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppstructure/__init__.py
+-rw-rw-rw-   0        0        0     7797 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppstructure/predict_system.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.981533 pyxllib-0.3.96/pyxlpr/ppstructure/table/
+-rw-rw-rw-   0        0        0      621 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppstructure/table/__init__.py
+-rw-rw-rw-   0        0        0     2377 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppstructure/table/eval_table.py
+-rw-rw-rw-   0        0        0     7168 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppstructure/table/matcher.py
+-rw-rw-rw-   0        0        0     4663 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppstructure/table/predict_structure.py
+-rw-rw-rw-   0        0        0     8851 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppstructure/table/predict_table.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.982533 pyxllib-0.3.96/pyxlpr/ppstructure/table/table_metric/
+-rw-rw-rw-   0        0        0      673 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppstructure/table/table_metric/__init__.py
+-rw-rw-rw-   0        0        0     2198 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppstructure/table/table_metric/parallel.py
+-rw-rw-rw-   0        0        0     9532 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppstructure/table/table_metric/table_metric.py
+drwxrwxrwx   0        0        0        0 2024-03-06 02:59:49.983533 pyxllib-0.3.96/pyxlpr/ppstructure/table/tablepyxl/
+-rw-rw-rw-   0        0        0      619 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppstructure/table/tablepyxl/__init__.py
+-rw-rw-rw-   0        0        0    10415 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppstructure/table/tablepyxl/style.py
+-rw-rw-rw-   0        0        0     4217 2021-11-11 08:55:05.000000 pyxllib-0.3.96/pyxlpr/ppstructure/table/tablepyxl/tablepyxl.py
+-rw-rw-rw-   0        0        0     2538 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/ppstructure/utility.py
+-rw-rw-rw-   0        0        0      260 2024-01-08 12:52:36.000000 pyxllib-0.3.96/pyxlpr/xlai.py
+-rw-rw-rw-   0        0        0      223 2024-01-08 12:52:36.000000 pyxllib-0.3.96/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-03-06 02:59:49.984533 pyxllib-0.3.96/setup.cfg
+-rw-rw-rw-   0        0        0     2478 2024-03-06 02:59:48.000000 pyxllib-0.3.96/setup.py
```

### Comparing `pyxllib-0.3.95/LICENSE` & `pyxllib-0.3.96/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/__init__.py` & `pyxllib-0.3.96/pyxllib/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/algo/disjoint.py` & `pyxllib-0.3.96/pyxllib/algo/disjoint.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/algo/geo.py` & `pyxllib-0.3.96/pyxllib/algo/geo.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/algo/intervals.py` & `pyxllib-0.3.96/pyxllib/algo/intervals.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/algo/matcher.py` & `pyxllib-0.3.96/pyxllib/algo/matcher.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/algo/newbie.py` & `pyxllib-0.3.96/pyxllib/algo/newbie.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/algo/pupil.py` & `pyxllib-0.3.96/pyxllib/algo/pupil.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/algo/shapelylib.py` & `pyxllib-0.3.96/pyxllib/algo/shapelylib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/algo/specialist.py` & `pyxllib-0.3.96/pyxllib/algo/specialist.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/algo/stat.py` & `pyxllib-0.3.96/pyxllib/algo/stat.py`

 * *Files 7% similar despite different names*

```diff
@@ -426,7 +426,33 @@
     with pd.option_context('display.max_rows', None,
                            'display.max_columns', None,
                            'display.width', 1000,
                            'display.max_colwidth', None):
         print(df)
 
     pd.options('display.max_rows', 60)
+
+
+def custom_fillna(df, default_fill_value='', numeric_fill_value=None, specific_fill=None):
+    """ 使用更多灵活性填充DataFrame中的NaN值。
+
+    :param pandas.DataFrame df: 需要处理的DataFrame。
+    :param str default_fill_value: 非数值列中NaN的默认填充值。
+    :param numeric_fill_value: 数值列中NaN的填充值，如果不指定，则默认为None。
+    :param dict specific_fill: 指定列名及其NaN的填充值，如果不指定，则默认为None。
+    :return: 已根据指定标准填充NaN值的pandas.DataFrame。
+
+    >>> df = pd.DataFrame({'A': [1, 2, None], 'B': [None, 'x', 'y'], 'C': [None, None, None]})
+    >>> custom_fillna(df, 'filled', 0, {'C': 'special'})
+    """
+    for column in df.columns:
+        # 检查列是否在specific_fill中指定；如果是，则使用指定的值填充。
+        if specific_fill and column in specific_fill:
+            df[column] = df[column].fillna(specific_fill[column])
+        # 如果列是数值型且指定了numeric_fill_value，则使用numeric_fill_value填充。
+        elif numeric_fill_value is not None and pd.api.types.is_numeric_dtype(df[column]):
+            df[column] = df[column].fillna(numeric_fill_value)
+        # 否则，对非数值列使用default_fill_value进行填充。
+        elif pd.api.types.is_object_dtype(df[column]) or pd.api.types.is_string_dtype(df[column]):
+            df[column] = df[column].fillna(default_fill_value)
+        # 可以在这里添加更多条件，以处理其他数据类型，如datetime。
+    return df
```

### Comparing `pyxllib-0.3.95/pyxllib/algo/treelib.py` & `pyxllib-0.3.96/pyxllib/algo/treelib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/algo/unitlib.py` & `pyxllib-0.3.96/pyxllib/algo/unitlib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/cv/expert.py` & `pyxllib-0.3.96/pyxllib/cv/expert.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/cv/imfile.py` & `pyxllib-0.3.96/pyxllib/cv/imfile.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/cv/imhash.py` & `pyxllib-0.3.96/pyxllib/cv/imhash.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/cv/rgbfmt.py` & `pyxllib-0.3.96/pyxllib/cv/rgbfmt.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/cv/trackbartools.py` & `pyxllib-0.3.96/pyxllib/cv/trackbartools.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/cv/xlcvlib.py` & `pyxllib-0.3.96/pyxllib/cv/xlcvlib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/cv/xlpillib.py` & `pyxllib-0.3.96/pyxllib/cv/xlpillib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/data/echarts.py` & `pyxllib-0.3.96/pyxllib/data/echarts.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
                 kwargs['label'].opts['formatter'] = fmt
             else:
                 kwargs['label']['show'] = True
                 kwargs['label']['formatter'] = fmt
 
         self._append_color(color)
         self._append_legend(name)
+        # self._append_legend(name, is_selected=True)
 
         self.options.get('series').append(
             {
                 'type': type,
                 'name': name,
                 'data': data,
                 **kwargs,
@@ -113,15 +114,15 @@
 def draw_pareto_chart(data, accuracy=0.1, *, title='帕累托累积权重', value_unit_type='K'):
     from pyxllib.algo.stat import pareto_accumulate
     pts, labels = pareto_accumulate(data, accuracy=accuracy, value_unit_type=value_unit_type)
     x = Line()
     x.add_series(title, pts, labels=labels, label={'position': 'right'})
     x.set_global_opts(
         # x轴末尾要故意撑大一些，不然有部分内容会显示不全
-        xaxis_opts=opts.AxisOpts(name='条目数', max_=int(float(f'{pts[-1][0]*1.2:.2g}'))),
+        xaxis_opts=opts.AxisOpts(name='条目数', max_=int(float(f'{pts[-1][0] * 1.2:.2g}'))),
         yaxis_opts=opts.AxisOpts(name='累积和')
     )
     return x
 
 
 if __name__ == '__main__':
     with TicToc(__name__):
```

### Comparing `pyxllib-0.3.95/pyxllib/data/oss.py` & `pyxllib-0.3.96/pyxllib/data/oss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/data/pglib.py` & `pyxllib-0.3.96/pyxllib/data/pglib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/data/sqlite.py` & `pyxllib-0.3.96/pyxllib/data/sqlite.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/data/sqllib.py` & `pyxllib-0.3.96/pyxllib/data/sqllib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/ext/JLineViewer.py` & `pyxllib-0.3.96/pyxllib/ext/JLineViewer.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/ext/autogui/autogui.py` & `pyxllib-0.3.96/pyxllib/ext/autogui/autogui.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/ext/autogui/virtualkey.py` & `pyxllib-0.3.96/pyxllib/ext/autogui/virtualkey.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/ext/demolib.py` & `pyxllib-0.3.96/pyxllib/ext/demolib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/ext/kq5034lib.py` & `pyxllib-0.3.96/pyxllib/ext/kq5034lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     def __init__(self):
         self.app_id = ''
         self.client_id = ''
         self.secret_key = ''
         self.token = ''
 
     def login(self, app_id, client_id, secret_key):
-        """ 登录
+        """ 登录，获取token
         """
         self.app_id = app_id
         self.client_id = client_id
         self.secret_key = secret_key
 
         # 启用缓存
         requests_cache.install_cache('access_token_cache', expire_after=600)  # 设置缓存过期时间xx（单位：秒）
@@ -74,14 +74,16 @@
                 self.token = result['data']['access_token']
             else:
                 raise Exception("Error getting access token: {}".format(result['msg']))
         else:
             raise Exception("HTTP request failed with status code {}".format(response.status_code))
 
     def get_alive_user_list(self, resource_id, page_size=100):
+        """ 获取直播间用户
+        """
         # 1 获取总页数
         url = "https://api.xiaoe-tech.com/xe.alive.user.list/1.0.0"  # 接口地址【路径：API列表 -> 直播管理 -> 获取直播间用户列表】
         data_1 = {
             "access_token": self.token,
             "resource_id": resource_id,
             "page": 1,
             "page_size": page_size
@@ -102,14 +104,45 @@
             response = requests.post(url, data=data)
             result = response.json()
             data_1 = result['data']['list']
             lst += data_1
             # lst.extend(data_1)
         return lst
 
+    def get_elock_actor(self, activity_id, page_size=100):
+        """ 获取打卡参与用户
+        """
+        # 获取总页数
+        url = "https://api.xiaoe-tech.com/xe.elock.actor/1.0.0"     # 接口地址【路径：API列表 -> 打卡管理 -> 获取打卡参与用户】
+        data_1 = {
+            "access_token": self.token,
+            "activity_id": activity_id,
+            "page_index": 1,
+            "page_size": page_size
+        }
+        response_1 = requests.post(url, data=data_1)
+        result_1 = response_1.json()
+        page = math.ceil(result_1['data']['count'] / page_size)  # 页数
+        # 获取打卡用户数据
+        lst = result_1['data']['list']
+        for i in range(1, page):    # 为什么从1开始，因为第一页的数据上面已经获取到了，这里没必要从新获取一次
+            data = {
+                "access_token": self.token,
+                "activity_id": activity_id,
+                "page_index": i + 1,
+                "page_size": page_size
+            }
+            response = requests.post(url, data=data)
+            result = response.json()
+            data_1 = result['data']['list']
+            lst += data_1
+            # lst.extend(data_1)
+        return lst
+
+
 
 class 网课考勤:
     def __init__(self, today=None):
         self.返款标题 = ''
         self.表格路径 = r'考勤.xlsx'
         self.在线表格 = 'https://docs.qq.com/sheet/DUlF1UnRackJ2Vm5U'  # 生成日报用
         self.开课日期 = '2022-01-08'
@@ -647,14 +680,20 @@
             pass
 
         if df is None:
             try:
                 df = pd.read_csv(files[-1])  # 221005周三09:19，小鹅通又双叒更新了
             except UnicodeDecodeError:
                 pass
+            
+        if df is None:
+            try:
+                df = pd.read_csv(files[-1], encoding="ANSI")  # 240226周一11:21，
+            except UnicodeDecodeError:
+                pass
 
         if df is None:
             raise ValueError
 
         df = df.applymap(lambda x: x.strip() if isinstance(x, str) else x)
         df.columns = df.columns.map(lambda x: x.strip() if isinstance(x, str) else x)
```

### Comparing `pyxllib-0.3.95/pyxllib/ext/old.py` & `pyxllib-0.3.96/pyxllib/ext/old.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/ext/qt.py` & `pyxllib-0.3.96/pyxllib/ext/qt.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/ext/seleniumlib.py` & `pyxllib-0.3.96/pyxllib/ext/seleniumlib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/ext/tk.py` & `pyxllib-0.3.96/pyxllib/ext/tk.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/ext/unixlib.py` & `pyxllib-0.3.96/pyxllib/ext/unixlib.py`

 * *Files 1% similar despite different names*

```diff
@@ -564,14 +564,19 @@
 
         self.exec(f'useradd -d /home/{name} -s /bin/bash -m {name}')
         self.set_user_passwd(name, passwd)
         if sudo:
             self.exec(f'usermod -aG sudo {name}')
 
     def check_cpu_usage(self, *, print_mode=False):
+        """
+
+        下面代码的cmds拼接出来是这样的：
+        sudo ps --no-headers -eo "pcpu,pmem,user"|awk 'BEGIN{FS=OFS=" "}{a0[$3]+=$1; a1[$3]+=$2}END {for (i in a0) print i,a0[i],a1[i]}'|sort -rn -k1,2 -k2,3
+        """
         # 1 获取原始信息
         cmds = ['ps --no-headers -eo "pcpu,pmem,user"',  # 列出所有程序情况
                 # 使用awk，按用户分组统计cpu（百分比）、内存总使用量（绝对量）
                 """awk 'BEGIN{FS=OFS=" "}{a0[$3]+=$1; a1[$3]+=$2}END {for (i in a0) print i,a0[i],a1[i]}'""",
                 'sort -rn -k1,2 -k2,3'  # 按cpu、内存使用量从大到小排序，不是必须的
                 ]
         lines = self.exec('|'.join(cmds)).splitlines()
```

### Comparing `pyxllib-0.3.95/pyxllib/ext/utools.py` & `pyxllib-0.3.96/pyxllib/ext/utools.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/ext/webhook.py` & `pyxllib-0.3.96/pyxllib/ext/webhook.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,59 +34,68 @@
 class DingtalkRobot:
     """ 钉钉 自定义webhook机器人
 
     https://ding-doc.dingtalk.com/doc#/serverapi2/qf2nxq
     """
 
     def __init__(self, url, secret):
-        self.url = url
-        self.url += self.add_secret(secret)
+        self.base_url = url  # 原始url，不包含时间戳和签名
+        self.secret = secret
         self.headers = {"Content-Type": "application/json"}
+        self.last_timestamp = 0  # 初始化上次时间戳
+        self.update_url()  # 初始化时更新URL
+
+    def update_url(self):
+        """更新URL中的时间戳和签名"""
+        self.url = self.base_url + self.add_secret(self.secret)
+        self.last_timestamp = round(time.time())  # 更新上次时间戳
 
     @classmethod
     def add_secret(cls, secret):
         """ 钉钉机器人需要加签，确保安全性 """
         timestamp = str(round(time.time() * 1000))
         secret_enc = secret.encode('utf-8')
         string_to_sign = '{}\n{}'.format(timestamp, secret)
         string_to_sign_enc = string_to_sign.encode('utf-8')
         hmac_code = hmac.new(secret_enc, string_to_sign_enc, digestmod=hashlib.sha256).digest()
         sign = urllib.parse.quote_plus(base64.b64encode(hmac_code))
-
         return f'&timestamp={timestamp}&sign={sign}'
 
-    def push_data(self, data):
+    def send_data(self, data):
+        # 检查当前时间是否超过30分钟
+        if round(time.time()) - self.last_timestamp > 1800:  # 30 * 60
+            self.update_url()  # 更新URL
         try:
             requests.post(url=self.url, headers=self.headers, json=data)
-        except requests.exceptions.ConnectionError:  # 没网发送失败的时候也不报错
-            pass
+        except requests.exceptions.ConnectionError as e:  # 没网发送失败的时候也不报错
+            raise e
 
-    def push_text(self, content):
+    def send_text(self, content):
         msgtype = 'text'
         d = {}
         if content: d['content'] = content
         data = {"msgtype": msgtype, msgtype: d}
-        self.push_data(data)
+        self.send_data(data)
 
-    def push_link(self, text='', title='', pic_url='', message_url=''):
+    def send_link(self, text='', title='', pic_url='', message_url=''):
         msgtype = 'link'
         d = {}
         if text: d['text'] = text
         if title: d['title'] = title
         if pic_url: d['picUrl'] = pic_url
         if message_url: d['messageUrl'] = message_url
         data = {"msgtype": msgtype, msgtype: d}
-        self.push_data(data)
+        self.send_data(data)
 
-    def push_markdown(self, text='', title=''):
+    def send_markdown(self, text='', title=''):
         msgtype = 'link'
         d = {}
         if text: d['text'] = text
         if title: d['title'] = title
         data = {"msgtype": msgtype, msgtype: d}
-        self.push_data(data)
+        self.send_data(data)
 
-    def push_actioncard(self, text='', title='', siggle_url='', siggle_title='', btn_orientation='0'):
+    def send_actioncard(self, text='', title='', siggle_url='', siggle_title='', btn_orientation='0'):
         raise NotImplementedError
 
-    def push_feedcard(self):
+    def send_feedcard(self):
         raise NotImplementedError
```

### Comparing `pyxllib-0.3.95/pyxllib/ext/win32lib.py` & `pyxllib-0.3.96/pyxllib/ext/win32lib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/ext/yuquelib.py` & `pyxllib-0.3.96/pyxllib/ext/yuquelib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/file/docxlib.py` & `pyxllib-0.3.96/pyxllib/file/docxlib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/file/gitlib.py` & `pyxllib-0.3.96/pyxllib/file/gitlib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/file/movielib.py` & `pyxllib-0.3.96/pyxllib/file/movielib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/file/onenotelib.py` & `pyxllib-0.3.96/pyxllib/file/onenotelib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/file/packlib/__init__.py` & `pyxllib-0.3.96/pyxllib/file/packlib/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/file/packlib/zipfile.py` & `pyxllib-0.3.96/pyxllib/file/packlib/zipfile.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/file/pdflib.py` & `pyxllib-0.3.96/pyxllib/file/pdflib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/file/pupil.py` & `pyxllib-0.3.96/pyxllib/file/pupil.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/file/specialist/__init__.py` & `pyxllib-0.3.96/pyxllib/file/specialist/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/file/specialist/dirlib.py` & `pyxllib-0.3.96/pyxllib/file/specialist/dirlib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/file/specialist/download.py` & `pyxllib-0.3.96/pyxllib/file/specialist/download.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/file/specialist/filelib.py` & `pyxllib-0.3.96/pyxllib/file/specialist/filelib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/file/xlsxlib.py` & `pyxllib-0.3.96/pyxllib/file/xlsxlib.py`

 * *Files 0% similar despite different names*

```diff
@@ -548,15 +548,15 @@
 
         注意，如果self是合并单元格，分两种清空
             母格（左上角），会撤销合并到和母格数值、格式
             衍生格，只会撤销合并单元格，但不会清除母格的数值、格式
 
         :return: 涉及到合并单元格的情况，新单元格和原单元格已经不一样了，需要重新获取对象
         """
-        ct, mid_result = self.celltype(return_mid_result=True)
+        ct, mid_result = self.celltype(return_mode=True)
         x = self
         if ct:  # 如果是合并单元格，取消该区域的合并单元格
             rng = mid_result['rng'] if ('rng' in mid_result) else self.in_range()
             self.parent.unmerge_cells(rng.coord)
             x = self.parent[self.coordinate]
         x.value = None
         x.style = 'Normal'
@@ -586,15 +586,15 @@
         """ 单元格全格式、包括值的整体复制
 
         注意合并单元格比较复杂，比如要把 'A1:C3' 复制到 'A2:D4'，是会出现问题的
             在预先清空A2:D4数据的时候，会把
             一般这种清空，推荐先将数据库复制到一个临时sheet，再复制回原sheet更安全
         """
         from itertools import product
-        ct, mid_result = self.celltype(return_mid_result=True)
+        ct, mid_result = self.celltype(return_mode=True)
 
         if ct == 0:  # 普通单元格，只复制值和格式
             dst_cell = dst_cell.clear()
             dst_cell.value = self.value
             self.copy_cell_format(dst_cell)
         elif ct == 2:  # 合并单元格，除了值和格式，要考虑单元格整体性的复制替换
             dst_cell = dst_cell.clear()
```

### Comparing `pyxllib-0.3.95/pyxllib/prog/deprecatedlib.py` & `pyxllib-0.3.96/pyxllib/prog/deprecatedlib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/prog/ipyexec.py` & `pyxllib-0.3.96/pyxllib/prog/ipyexec.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/prog/newbie.py` & `pyxllib-0.3.96/pyxllib/prog/newbie.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/prog/pupil.py` & `pyxllib-0.3.96/pyxllib/prog/pupil.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/prog/sitepackages.py` & `pyxllib-0.3.96/pyxllib/prog/sitepackages.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/prog/specialist/__init__.py` & `pyxllib-0.3.96/pyxllib/prog/specialist/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     # 2 改版本号
     if version:
         f = XlPath(root) / version_file
         s = re.sub(r"(version\s*=\s*)(['\"])(.+?)(\2)", fr'\1\g<2>{version}\4', f.read_text())
         f.write_text(s)
 
     # 3 打包
-    subprocess.run('python setup.py sdist')
+    subprocess.run('python setup.py sdist bdist_wheel')
 
     # 4 上传
     if upload:
         # 上传
         cmd = 'twine upload dist/*'
         if repository:
             cmd += f' -r {repository}'
```

### Comparing `pyxllib-0.3.95/pyxllib/prog/specialist/bc.py` & `pyxllib-0.3.96/pyxllib/prog/specialist/bc.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/prog/specialist/browser.py` & `pyxllib-0.3.96/pyxllib/prog/specialist/browser.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/prog/specialist/common.py` & `pyxllib-0.3.96/pyxllib/prog/specialist/common.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/prog/specialist/datetime.py` & `pyxllib-0.3.96/pyxllib/prog/specialist/datetime.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/prog/specialist/tictoc.py` & `pyxllib-0.3.96/pyxllib/prog/specialist/tictoc.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/prog/specialist/xllog.py` & `pyxllib-0.3.96/pyxllib/prog/specialist/xllog.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/prog/xlosenv.py` & `pyxllib-0.3.96/pyxllib/prog/xlosenv.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/stdlib/__init__.py` & `pyxllib-0.3.96/pyxllib/stdlib/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/stdlib/tablepyxl/style.py` & `pyxllib-0.3.96/pyxllib/stdlib/tablepyxl/style.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/stdlib/tablepyxl/tablepyxl.py` & `pyxllib-0.3.96/pyxllib/stdlib/tablepyxl/tablepyxl.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/text/ahocorasick.py` & `pyxllib-0.3.96/pyxllib/text/ahocorasick.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/text/charclasslib.py` & `pyxllib-0.3.96/pyxllib/text/charclasslib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/text/jiebalib.py` & `pyxllib-0.3.96/pyxllib/text/jiebalib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/text/jscode.py` & `pyxllib-0.3.96/pyxllib/text/jscode.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/text/latex/__init__.py` & `pyxllib-0.3.96/pyxllib/text/latex/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/text/levenshtein.py` & `pyxllib-0.3.96/pyxllib/text/levenshtein.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/text/nestenv.py` & `pyxllib-0.3.96/pyxllib/text/nestenv.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/text/newbie.py` & `pyxllib-0.3.96/pyxllib/text/newbie.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/text/pupil/common.py` & `pyxllib-0.3.96/pyxllib/text/pupil/common.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/text/pupil/xlalign.py` & `pyxllib-0.3.96/pyxllib/text/pupil/xlalign.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/text/pycode.py` & `pyxllib-0.3.96/pyxllib/text/pycode.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/text/specialist/common.py` & `pyxllib-0.3.96/pyxllib/text/specialist/common.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/text/specialist/ptag.py` & `pyxllib-0.3.96/pyxllib/text/specialist/ptag.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/text/spellchecker.py` & `pyxllib-0.3.96/pyxllib/text/spellchecker.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/text/vbacode.py` & `pyxllib-0.3.96/pyxllib/text/vbacode.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/text/xmllib.py` & `pyxllib-0.3.96/pyxllib/text/xmllib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/xl.py` & `pyxllib-0.3.96/pyxllib/xl.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib/xlcv.py` & `pyxllib-0.3.96/pyxllib/xlcv.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxllib.egg-info/SOURCES.txt` & `pyxllib-0.3.96/pyxllib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ai/clientlib.py` & `pyxllib-0.3.96/pyxlpr/ai/clientlib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ai/specialist.py` & `pyxllib-0.3.96/pyxlpr/ai/specialist.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ai/torch_app.py` & `pyxllib-0.3.96/pyxlpr/ai/torch_app.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ai/xlpaddle.py` & `pyxllib-0.3.96/pyxlpr/ai/xlpaddle.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ai/xltorch.py` & `pyxllib-0.3.96/pyxlpr/ai/xltorch.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/data/coco.py` & `pyxllib-0.3.96/pyxlpr/data/coco.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/data/datacls.py` & `pyxllib-0.3.96/pyxlpr/data/datacls.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/data/datasets.py` & `pyxllib-0.3.96/pyxlpr/data/datasets.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/data/gptlib.py` & `pyxllib-0.3.96/pyxlpr/data/gptlib.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/data/icdar/__init__.py` & `pyxllib-0.3.96/pyxlpr/data/icdar/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/data/icdar/deteval.py` & `pyxllib-0.3.96/pyxlpr/data/icdar/deteval.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/data/icdar/icdar2013.py` & `pyxllib-0.3.96/pyxlpr/data/icdar/icdar2013.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/data/icdar/iou.py` & `pyxllib-0.3.96/pyxlpr/data/icdar/iou.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/data/icdar/rrc_evaluation_funcs_1_1.py` & `pyxllib-0.3.96/pyxlpr/data/icdar/rrc_evaluation_funcs_1_1.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/data/imtextline.py` & `pyxllib-0.3.96/pyxlpr/data/imtextline.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/data/labelme.py` & `pyxllib-0.3.96/pyxlpr/data/labelme.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/data/removeline.py` & `pyxllib-0.3.96/pyxlpr/data/removeline.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/data/specialist.py` & `pyxllib-0.3.96/pyxlpr/data/specialist.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/eval/__init__.py` & `pyxllib-0.3.96/pyxlpr/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/paddleocr.py` & `pyxllib-0.3.96/pyxlpr/paddleocr.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/__init__.py` & `pyxllib-0.3.96/pyxlpr/ppocr/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/configs/rec/multi_language/generate_multi_language_configs.py` & `pyxllib-0.3.96/pyxlpr/ppocr/configs/rec/multi_language/generate_multi_language_configs.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/data/__init__.py` & `pyxllib-0.3.96/pyxlpr/ppocr/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/data/imaug/ColorJitter.py` & `pyxllib-0.3.96/pyxlpr/ppocr/data/imaug/ColorJitter.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/data/imaug/__init__.py` & `pyxllib-0.3.96/pyxlpr/ppocr/data/imaug/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/data/imaug/copy_paste.py` & `pyxllib-0.3.96/pyxlpr/ppocr/data/imaug/copy_paste.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/data/imaug/east_process.py` & `pyxllib-0.3.96/pyxlpr/ppocr/data/imaug/east_process.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/data/imaug/gen_table_mask.py` & `pyxllib-0.3.96/pyxlpr/ppocr/data/imaug/gen_table_mask.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/data/imaug/iaa_augment.py` & `pyxllib-0.3.96/pyxlpr/ppocr/data/imaug/iaa_augment.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/data/imaug/label_ops.py` & `pyxllib-0.3.96/pyxlpr/ppocr/data/imaug/label_ops.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/data/imaug/make_border_map.py` & `pyxllib-0.3.96/pyxlpr/ppocr/data/imaug/make_border_map.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/data/imaug/make_pse_gt.py` & `pyxllib-0.3.96/pyxlpr/ppocr/data/imaug/make_pse_gt.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/data/imaug/make_shrink_map.py` & `pyxllib-0.3.96/pyxlpr/ppocr/data/imaug/make_shrink_map.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/data/imaug/operators.py` & `pyxllib-0.3.96/pyxlpr/ppocr/data/imaug/operators.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/data/imaug/pg_process.py` & `pyxllib-0.3.96/pyxlpr/ppocr/data/imaug/pg_process.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/data/imaug/randaugment.py` & `pyxllib-0.3.96/pyxlpr/ppocr/data/imaug/randaugment.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/data/imaug/random_crop_data.py` & `pyxllib-0.3.96/pyxlpr/ppocr/data/imaug/random_crop_data.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/data/imaug/rec_img_aug.py` & `pyxllib-0.3.96/pyxlpr/ppocr/data/imaug/rec_img_aug.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/data/imaug/sast_process.py` & `pyxllib-0.3.96/pyxlpr/ppocr/data/imaug/sast_process.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/data/imaug/text_image_aug/__init__.py` & `pyxllib-0.3.96/pyxlpr/ppocr/data/imaug/text_image_aug/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/data/imaug/text_image_aug/augment.py` & `pyxllib-0.3.96/pyxlpr/ppocr/data/imaug/text_image_aug/augment.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/data/imaug/text_image_aug/warp_mls.py` & `pyxllib-0.3.96/pyxlpr/ppocr/data/imaug/text_image_aug/warp_mls.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/data/lmdb_dataset.py` & `pyxllib-0.3.96/pyxlpr/ppocr/data/lmdb_dataset.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/data/pgnet_dataset.py` & `pyxllib-0.3.96/pyxlpr/ppocr/data/pgnet_dataset.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/data/pubtab_dataset.py` & `pyxllib-0.3.96/pyxlpr/ppocr/data/pubtab_dataset.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/data/simple_dataset.py` & `pyxllib-0.3.96/pyxlpr/ppocr/data/simple_dataset.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/losses/__init__.py` & `pyxllib-0.3.96/pyxlpr/ppocr/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/losses/ace_loss.py` & `pyxllib-0.3.96/pyxlpr/ppocr/losses/ace_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/losses/basic_loss.py` & `pyxllib-0.3.96/pyxlpr/ppocr/losses/basic_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/losses/center_loss.py` & `pyxllib-0.3.96/pyxlpr/ppocr/losses/center_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/losses/cls_loss.py` & `pyxllib-0.3.96/pyxlpr/ppocr/losses/cls_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/losses/combined_loss.py` & `pyxllib-0.3.96/pyxlpr/ppocr/losses/combined_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/losses/det_basic_loss.py` & `pyxllib-0.3.96/pyxlpr/ppocr/losses/det_basic_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/losses/det_db_loss.py` & `pyxllib-0.3.96/pyxlpr/ppocr/losses/det_db_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/losses/det_east_loss.py` & `pyxllib-0.3.96/pyxlpr/ppocr/losses/det_east_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/losses/det_pse_loss.py` & `pyxllib-0.3.96/pyxlpr/ppocr/losses/det_pse_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/losses/det_sast_loss.py` & `pyxllib-0.3.96/pyxlpr/ppocr/losses/det_sast_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/losses/distillation_loss.py` & `pyxllib-0.3.96/pyxlpr/ppocr/losses/distillation_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/losses/e2e_pg_loss.py` & `pyxllib-0.3.96/pyxlpr/ppocr/losses/e2e_pg_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/losses/kie_sdmgr_loss.py` & `pyxllib-0.3.96/pyxlpr/ppocr/losses/kie_sdmgr_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/losses/rec_aster_loss.py` & `pyxllib-0.3.96/pyxlpr/ppocr/losses/rec_aster_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/losses/rec_att_loss.py` & `pyxllib-0.3.96/pyxlpr/ppocr/losses/rec_att_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/losses/rec_ctc_loss.py` & `pyxllib-0.3.96/pyxlpr/ppocr/losses/rec_ctc_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/losses/rec_enhanced_ctc_loss.py` & `pyxllib-0.3.96/pyxlpr/ppocr/losses/rec_enhanced_ctc_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/losses/rec_nrtr_loss.py` & `pyxllib-0.3.96/pyxlpr/ppocr/losses/rec_nrtr_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/losses/rec_sar_loss.py` & `pyxllib-0.3.96/pyxlpr/ppocr/losses/rec_sar_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/losses/rec_srn_loss.py` & `pyxllib-0.3.96/pyxlpr/ppocr/losses/rec_srn_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/losses/table_att_loss.py` & `pyxllib-0.3.96/pyxlpr/ppocr/losses/table_att_loss.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/metrics/__init__.py` & `pyxllib-0.3.96/pyxlpr/ppocr/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/metrics/cls_metric.py` & `pyxllib-0.3.96/pyxlpr/ppocr/metrics/cls_metric.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/metrics/det_metric.py` & `pyxllib-0.3.96/pyxlpr/ppocr/metrics/det_metric.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/metrics/distillation_metric.py` & `pyxllib-0.3.96/pyxlpr/ppocr/metrics/distillation_metric.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/metrics/e2e_metric.py` & `pyxllib-0.3.96/pyxlpr/ppocr/metrics/e2e_metric.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/metrics/eval_det_iou.py` & `pyxllib-0.3.96/pyxlpr/ppocr/metrics/eval_det_iou.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/metrics/kie_metric.py` & `pyxllib-0.3.96/pyxlpr/ppocr/metrics/kie_metric.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/metrics/rec_metric.py` & `pyxllib-0.3.96/pyxlpr/ppocr/metrics/rec_metric.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/metrics/table_metric.py` & `pyxllib-0.3.96/pyxlpr/ppocr/metrics/table_metric.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/architectures/__init__.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/architectures/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/architectures/base_model.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/architectures/base_model.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/architectures/distillation_model.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/architectures/distillation_model.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/backbones/__init__.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/backbones/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/backbones/det_mobilenet_v3.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/backbones/det_mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/backbones/det_resnet_vd.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/backbones/det_resnet_vd.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/backbones/det_resnet_vd_sast.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/backbones/det_resnet_vd_sast.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/backbones/e2e_resnet_vd_pg.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/backbones/e2e_resnet_vd_pg.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/backbones/kie_unet_sdmgr.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/backbones/kie_unet_sdmgr.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/backbones/rec_mobilenet_v3.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/backbones/rec_mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/backbones/rec_mv1_enhance.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/backbones/rec_mv1_enhance.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/backbones/rec_nrtr_mtb.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/backbones/rec_nrtr_mtb.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/backbones/rec_resnet_31.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/backbones/rec_resnet_31.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/backbones/rec_resnet_aster.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/backbones/rec_resnet_aster.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/backbones/rec_resnet_fpn.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/backbones/rec_resnet_fpn.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/backbones/rec_resnet_vd.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/backbones/rec_resnet_vd.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/heads/__init__.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/heads/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/heads/cls_head.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/heads/cls_head.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/heads/det_db_head.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/heads/det_db_head.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/heads/det_east_head.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/heads/det_east_head.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/heads/det_pse_head.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/heads/det_pse_head.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/heads/det_sast_head.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/heads/det_sast_head.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/heads/e2e_pg_head.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/heads/e2e_pg_head.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/heads/kie_sdmgr_head.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/heads/kie_sdmgr_head.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/heads/multiheadAttention.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/heads/multiheadAttention.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/heads/rec_aster_head.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/heads/rec_aster_head.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/heads/rec_att_head.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/heads/rec_att_head.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/heads/rec_ctc_head.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/heads/rec_ctc_head.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/heads/rec_nrtr_head.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/heads/rec_nrtr_head.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/heads/rec_sar_head.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/heads/rec_sar_head.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/heads/rec_srn_head.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/heads/rec_srn_head.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/heads/self_attention.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/heads/self_attention.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/heads/table_att_head.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/heads/table_att_head.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/necks/__init__.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/necks/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/necks/db_fpn.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/necks/db_fpn.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/necks/east_fpn.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/necks/east_fpn.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/necks/fpn.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/necks/fpn.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/necks/pg_fpn.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/necks/pg_fpn.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/necks/rnn.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/necks/rnn.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/necks/sast_fpn.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/necks/sast_fpn.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/necks/table_fpn.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/necks/table_fpn.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/transforms/__init__.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/transforms/stn.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/transforms/stn.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/transforms/tps.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/transforms/tps.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/modeling/transforms/tps_spatial_transformer.py` & `pyxllib-0.3.96/pyxlpr/ppocr/modeling/transforms/tps_spatial_transformer.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/optimizer/__init__.py` & `pyxllib-0.3.96/pyxlpr/ppocr/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/optimizer/learning_rate.py` & `pyxllib-0.3.96/pyxlpr/ppocr/optimizer/learning_rate.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/optimizer/lr_scheduler.py` & `pyxllib-0.3.96/pyxlpr/ppocr/optimizer/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/optimizer/optimizer.py` & `pyxllib-0.3.96/pyxlpr/ppocr/optimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/optimizer/regularizer.py` & `pyxllib-0.3.96/pyxlpr/ppocr/optimizer/regularizer.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/postprocess/__init__.py` & `pyxllib-0.3.96/pyxlpr/ppocr/postprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/postprocess/cls_postprocess.py` & `pyxllib-0.3.96/pyxlpr/ppocr/postprocess/cls_postprocess.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/postprocess/db_postprocess.py` & `pyxllib-0.3.96/pyxlpr/ppocr/postprocess/db_postprocess.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/postprocess/east_postprocess.py` & `pyxllib-0.3.96/pyxlpr/ppocr/postprocess/east_postprocess.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/postprocess/locality_aware_nms.py` & `pyxllib-0.3.96/pyxlpr/ppocr/postprocess/locality_aware_nms.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/postprocess/pg_postprocess.py` & `pyxllib-0.3.96/pyxlpr/ppocr/postprocess/pg_postprocess.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/postprocess/pse_postprocess/__init__.py` & `pyxllib-0.3.96/pyxlpr/ppocr/postprocess/pse_postprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/postprocess/pse_postprocess/pse/__init__.py` & `pyxllib-0.3.96/pyxlpr/ppocr/postprocess/pse_postprocess/pse/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/postprocess/pse_postprocess/pse_postprocess.py` & `pyxllib-0.3.96/pyxlpr/ppocr/postprocess/pse_postprocess/pse_postprocess.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/postprocess/rec_postprocess.py` & `pyxllib-0.3.96/pyxlpr/ppocr/postprocess/rec_postprocess.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/postprocess/sast_postprocess.py` & `pyxllib-0.3.96/pyxlpr/ppocr/postprocess/sast_postprocess.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/tools/__init__.py` & `pyxllib-0.3.96/pyxlpr/ppocr/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/tools/eval.py` & `pyxllib-0.3.96/pyxlpr/ppocr/tools/eval.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/tools/export_center.py` & `pyxllib-0.3.96/pyxlpr/ppocr/tools/export_center.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/tools/export_model.py` & `pyxllib-0.3.96/pyxlpr/ppocr/tools/export_model.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/tools/infer/predict_cls.py` & `pyxllib-0.3.96/pyxlpr/ppocr/tools/infer/predict_cls.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/tools/infer/predict_det.py` & `pyxllib-0.3.96/pyxlpr/ppocr/tools/infer/predict_det.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/tools/infer/predict_e2e.py` & `pyxllib-0.3.96/pyxlpr/ppocr/tools/infer/predict_e2e.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/tools/infer/predict_rec.py` & `pyxllib-0.3.96/pyxlpr/ppocr/tools/infer/predict_rec.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/tools/infer/predict_system.py` & `pyxllib-0.3.96/pyxlpr/ppocr/tools/infer/predict_system.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/tools/infer/utility.py` & `pyxllib-0.3.96/pyxlpr/ppocr/tools/infer/utility.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/tools/infer_cls.py` & `pyxllib-0.3.96/pyxlpr/ppocr/tools/infer_cls.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/tools/infer_det.py` & `pyxllib-0.3.96/pyxlpr/ppocr/tools/infer_det.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/tools/infer_e2e.py` & `pyxllib-0.3.96/pyxlpr/ppocr/tools/infer_e2e.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/tools/infer_kie.py` & `pyxllib-0.3.96/pyxlpr/ppocr/tools/infer_kie.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/tools/infer_rec.py` & `pyxllib-0.3.96/pyxlpr/ppocr/tools/infer_rec.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/tools/infer_table.py` & `pyxllib-0.3.96/pyxlpr/ppocr/tools/infer_table.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/tools/program.py` & `pyxllib-0.3.96/pyxlpr/ppocr/tools/program.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/tools/test_hubserving.py` & `pyxllib-0.3.96/pyxlpr/ppocr/tools/test_hubserving.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/tools/train.py` & `pyxllib-0.3.96/pyxlpr/ppocr/tools/train.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/tools/xlprog.py` & `pyxllib-0.3.96/pyxlpr/ppocr/tools/xlprog.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/utils/__init__.py` & `pyxllib-0.3.96/pyxlpr/ppocr/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/arabic_dict.txt` & `pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/arabic_dict.txt`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/chinese_cht_dict.txt` & `pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/chinese_cht_dict.txt`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/cyrillic_dict.txt` & `pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/cyrillic_dict.txt`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/devanagari_dict.txt` & `pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/devanagari_dict.txt`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/hi_dict.txt` & `pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/hi_dict.txt`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/japan_dict.txt` & `pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/japan_dict.txt`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/ka_dict.txt` & `pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/ka_dict.txt`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/korean_dict.txt` & `pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/korean_dict.txt`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/latin_dict.txt` & `pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/latin_dict.txt`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/mr_dict.txt` & `pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/mr_dict.txt`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/ne_dict.txt` & `pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/ne_dict.txt`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/table_dict.txt` & `pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/table_dict.txt`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/table_structure_dict.txt` & `pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/table_structure_dict.txt`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/utils/dict/te_dict.txt` & `pyxllib-0.3.96/pyxlpr/ppocr/utils/dict/te_dict.txt`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/utils/e2e_metric/Deteval.py` & `pyxllib-0.3.96/pyxlpr/ppocr/utils/e2e_metric/Deteval.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/utils/e2e_metric/polygon_fast.py` & `pyxllib-0.3.96/pyxlpr/ppocr/utils/e2e_metric/polygon_fast.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/utils/e2e_utils/extract_batchsize.py` & `pyxllib-0.3.96/pyxlpr/ppocr/utils/e2e_utils/extract_batchsize.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/utils/e2e_utils/extract_textpoint_fast.py` & `pyxllib-0.3.96/pyxlpr/ppocr/utils/e2e_utils/extract_textpoint_fast.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/utils/e2e_utils/extract_textpoint_slow.py` & `pyxllib-0.3.96/pyxlpr/ppocr/utils/e2e_utils/extract_textpoint_slow.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/utils/e2e_utils/pgnet_pp_utils.py` & `pyxllib-0.3.96/pyxlpr/ppocr/utils/e2e_utils/pgnet_pp_utils.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/utils/e2e_utils/visual.py` & `pyxllib-0.3.96/pyxlpr/ppocr/utils/e2e_utils/visual.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/utils/gen_label.py` & `pyxllib-0.3.96/pyxlpr/ppocr/utils/gen_label.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/utils/iou.py` & `pyxllib-0.3.96/pyxlpr/ppocr/utils/iou.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/utils/logging.py` & `pyxllib-0.3.96/pyxlpr/ppocr/utils/logging.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/utils/network.py` & `pyxllib-0.3.96/pyxlpr/ppocr/utils/network.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/utils/ppocr_keys_v1.txt` & `pyxllib-0.3.96/pyxlpr/ppocr/utils/ppocr_keys_v1.txt`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/utils/profiler.py` & `pyxllib-0.3.96/pyxlpr/ppocr/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/utils/save_load.py` & `pyxllib-0.3.96/pyxlpr/ppocr/utils/save_load.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/utils/stats.py` & `pyxllib-0.3.96/pyxlpr/ppocr/utils/stats.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppocr/utils/utility.py` & `pyxllib-0.3.96/pyxlpr/ppocr/utils/utility.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppstructure/__init__.py` & `pyxllib-0.3.96/pyxlpr/ppstructure/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppstructure/predict_system.py` & `pyxllib-0.3.96/pyxlpr/ppstructure/predict_system.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppstructure/table/__init__.py` & `pyxllib-0.3.96/pyxlpr/ppstructure/table/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppstructure/table/eval_table.py` & `pyxllib-0.3.96/pyxlpr/ppstructure/table/eval_table.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppstructure/table/matcher.py` & `pyxllib-0.3.96/pyxlpr/ppstructure/table/matcher.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppstructure/table/predict_structure.py` & `pyxllib-0.3.96/pyxlpr/ppstructure/table/predict_structure.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppstructure/table/predict_table.py` & `pyxllib-0.3.96/pyxlpr/ppstructure/table/predict_table.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppstructure/table/table_metric/__init__.py` & `pyxllib-0.3.96/pyxlpr/ppstructure/table/table_metric/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppstructure/table/table_metric/parallel.py` & `pyxllib-0.3.96/pyxlpr/ppstructure/table/table_metric/parallel.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppstructure/table/table_metric/table_metric.py` & `pyxllib-0.3.96/pyxlpr/ppstructure/table/table_metric/table_metric.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppstructure/table/tablepyxl/__init__.py` & `pyxllib-0.3.96/pyxlpr/ppstructure/table/tablepyxl/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppstructure/table/tablepyxl/style.py` & `pyxllib-0.3.96/pyxlpr/ppstructure/table/tablepyxl/style.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppstructure/table/tablepyxl/tablepyxl.py` & `pyxllib-0.3.96/pyxlpr/ppstructure/table/tablepyxl/tablepyxl.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/pyxlpr/ppstructure/utility.py` & `pyxllib-0.3.96/pyxlpr/ppstructure/utility.py`

 * *Files identical despite different names*

### Comparing `pyxllib-0.3.95/setup.py` & `pyxllib-0.3.96/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 """
 # fvcore
 
 _dir = Path(__file__).parent
 
 setup(
     name='pyxllib',  # pip 安装时用的名字
-    version='0.3.95',  # 当前版本，每次更新上传到pypi都需要修改; 第4位版本号一般是修紧急bug
+    version='0.3.96',  # 当前版本，每次更新上传到pypi都需要修改; 第4位版本号一般是修紧急bug
     author='code4101',
     author_email='877362867@qq.com',
     url='https://github.com/XLPRUtils/pyxllib',
     keywords=['pyxllib',  # 通用工具
               'pyxlpr',  # 模式识别相关功能
               ],
     description='厦门理工模式识别团队通用python代码工具库',
```

