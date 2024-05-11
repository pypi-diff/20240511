# Comparing `tmp/sarcharts-0.1.7.tar.gz` & `tmp/sarcharts-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarcharts-0.1.7.tar", last modified: Wed May  8 15:15:37 2024, max compression
+gzip compressed data, was "sarcharts-0.1.8.tar", last modified: Sat May 11 15:51:06 2024, max compression
```

## Comparing `sarcharts-0.1.7.tar` & `sarcharts-0.1.8.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:15:37.412011 sarcharts-0.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:15:37.404010 sarcharts-0.1.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:15:37.404010 sarcharts-0.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-08 15:15:31.000000 sarcharts-0.1.7/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-08 15:15:31.000000 sarcharts-0.1.7/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-08 15:15:37.000000 sarcharts-0.1.7/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-08 15:15:37.000000 sarcharts-0.1.7/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-08 15:15:31.000000 sarcharts-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-08 15:15:37.412011 sarcharts-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-08 15:15:31.000000 sarcharts-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:15:37.408010 sarcharts-0.1.7/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-08 15:15:31.000000 sarcharts-0.1.7/doc/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   137178 2024-05-08 15:15:31.000000 sarcharts-0.1.7/doc/sarcharts.png
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-08 15:15:31.000000 sarcharts-0.1.7/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:15:37.408010 sarcharts-0.1.7/sarcharts/
--rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-05-08 15:15:31.000000 sarcharts-0.1.7/sarcharts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:15:37.408010 sarcharts-0.1.7/sarcharts/bin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:15:31.000000 sarcharts-0.1.7/sarcharts/bin/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      204 2024-05-08 15:15:31.000000 sarcharts-0.1.7/sarcharts/bin/sarcharts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:15:37.404010 sarcharts-0.1.7/sarcharts/html/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:15:37.408010 sarcharts-0.1.7/sarcharts/html/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-08 15:15:31.000000 sarcharts-0.1.7/sarcharts/html/css/sarcharts.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:15:37.408010 sarcharts-0.1.7/sarcharts/html/js/
--rw-r--r--   0 runner    (1001) docker     (127)   205214 2024-05-08 15:15:31.000000 sarcharts-0.1.7/sarcharts/html/js/chart.umd.js
--rw-r--r--   0 runner    (1001) docker     (127)    12854 2024-05-08 15:15:31.000000 sarcharts-0.1.7/sarcharts/html/js/chartjs-plugin-zoom.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    20765 2024-05-08 15:15:31.000000 sarcharts-0.1.7/sarcharts/html/js/hammer.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   271751 2024-05-08 15:15:31.000000 sarcharts-0.1.7/sarcharts/html/js/jquery.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:15:37.412011 sarcharts-0.1.7/sarcharts/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-08 15:15:31.000000 sarcharts-0.1.7/sarcharts/lib/chartjs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6808 2024-05-08 15:15:31.000000 sarcharts-0.1.7/sarcharts/lib/chartsconf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-08 15:15:31.000000 sarcharts-0.1.7/sarcharts/lib/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-05-08 15:15:31.000000 sarcharts-0.1.7/sarcharts/lib/sadf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-08 15:15:31.000000 sarcharts-0.1.7/sarcharts/lib/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:15:37.412011 sarcharts-0.1.7/sarcharts/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-08 15:15:31.000000 sarcharts-0.1.7/sarcharts/templates/chart.html
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-08 15:15:31.000000 sarcharts-0.1.7/sarcharts/templates/header.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:15:37.412011 sarcharts-0.1.7/sarcharts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-08 15:15:37.000000 sarcharts-0.1.7/sarcharts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-08 15:15:37.000000 sarcharts-0.1.7/sarcharts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:15:37.000000 sarcharts-0.1.7/sarcharts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-08 15:15:37.000000 sarcharts-0.1.7/sarcharts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:15:37.000000 sarcharts-0.1.7/sarcharts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-08 15:15:37.000000 sarcharts-0.1.7/sarcharts.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-08 15:15:37.000000 sarcharts-0.1.7/sarcharts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 15:15:37.000000 sarcharts-0.1.7/sarcharts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-08 15:15:37.412011 sarcharts-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-08 15:15:31.000000 sarcharts-0.1.7/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-08 15:15:31.000000 sarcharts-0.1.7/test-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-08 15:15:31.000000 sarcharts-0.1.7/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:51:06.257505 sarcharts-0.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:51:06.249505 sarcharts-0.1.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:51:06.253505 sarcharts-0.1.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-11 15:51:00.000000 sarcharts-0.1.8/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-11 15:51:00.000000 sarcharts-0.1.8/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-11 15:51:06.000000 sarcharts-0.1.8/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-11 15:51:06.000000 sarcharts-0.1.8/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-11 15:51:00.000000 sarcharts-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-11 15:51:06.257505 sarcharts-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-11 15:51:00.000000 sarcharts-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:51:06.253505 sarcharts-0.1.8/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-11 15:51:00.000000 sarcharts-0.1.8/doc/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   137178 2024-05-11 15:51:00.000000 sarcharts-0.1.8/doc/sarcharts.png
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-11 15:51:00.000000 sarcharts-0.1.8/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:51:06.253505 sarcharts-0.1.8/sarcharts/
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-11 15:51:00.000000 sarcharts-0.1.8/sarcharts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:51:06.257505 sarcharts-0.1.8/sarcharts/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 15:51:00.000000 sarcharts-0.1.8/sarcharts/bin/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      204 2024-05-11 15:51:00.000000 sarcharts-0.1.8/sarcharts/bin/sarcharts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:51:06.249505 sarcharts-0.1.8/sarcharts/html/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:51:06.257505 sarcharts-0.1.8/sarcharts/html/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-11 15:51:00.000000 sarcharts-0.1.8/sarcharts/html/css/sarcharts.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:51:06.257505 sarcharts-0.1.8/sarcharts/html/js/
+-rw-r--r--   0 runner    (1001) docker     (127)   205214 2024-05-11 15:51:00.000000 sarcharts-0.1.8/sarcharts/html/js/chart.umd.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12854 2024-05-11 15:51:00.000000 sarcharts-0.1.8/sarcharts/html/js/chartjs-plugin-zoom.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20765 2024-05-11 15:51:00.000000 sarcharts-0.1.8/sarcharts/html/js/hammer.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   271751 2024-05-11 15:51:00.000000 sarcharts-0.1.8/sarcharts/html/js/jquery.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:51:06.257505 sarcharts-0.1.8/sarcharts/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-11 15:51:00.000000 sarcharts-0.1.8/sarcharts/lib/chartjs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6808 2024-05-11 15:51:00.000000 sarcharts-0.1.8/sarcharts/lib/chartsconf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-11 15:51:00.000000 sarcharts-0.1.8/sarcharts/lib/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-05-11 15:51:00.000000 sarcharts-0.1.8/sarcharts/lib/sadf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-11 15:51:00.000000 sarcharts-0.1.8/sarcharts/lib/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:51:06.257505 sarcharts-0.1.8/sarcharts/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-11 15:51:00.000000 sarcharts-0.1.8/sarcharts/templates/chart.html
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-11 15:51:00.000000 sarcharts-0.1.8/sarcharts/templates/header.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:51:06.257505 sarcharts-0.1.8/sarcharts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-11 15:51:06.000000 sarcharts-0.1.8/sarcharts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-11 15:51:06.000000 sarcharts-0.1.8/sarcharts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 15:51:06.000000 sarcharts-0.1.8/sarcharts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-11 15:51:06.000000 sarcharts-0.1.8/sarcharts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 15:51:06.000000 sarcharts-0.1.8/sarcharts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-11 15:51:06.000000 sarcharts-0.1.8/sarcharts.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-11 15:51:06.000000 sarcharts-0.1.8/sarcharts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-11 15:51:06.000000 sarcharts-0.1.8/sarcharts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-11 15:51:06.261505 sarcharts-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-11 15:51:00.000000 sarcharts-0.1.8/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-11 15:51:00.000000 sarcharts-0.1.8/test-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-11 15:51:00.000000 sarcharts-0.1.8/tox.ini
```

### Comparing `sarcharts-0.1.7/.github/workflows/python-publish.yml` & `sarcharts-0.1.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.7/.pylintrc` & `sarcharts-0.1.8/.pylintrc`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.7/LICENSE` & `sarcharts-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.7/PKG-INFO` & `sarcharts-0.1.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarcharts
-Version: 0.1.7
+Version: 0.1.8
 Summary: SarCharts gets sysstat files from provided sarfilespaths and generates dynamic HTML Charts
 Home-page: https://github.com/pafernanr/sarcharts
 Author: Pablo Fernández Rodríguez
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
@@ -22,14 +22,17 @@
 
 ### SarCharts
 SarCharts gets [sysstat](https://sysstat.github.io/) files from provided `sarfilespaths` and generates dynamic HTML Charts.
 
 ### Requirements
 `sadf` command is needed to read sar files. Hence [sysstat](https://sysstat.github.io/) package is required.
 
+### Installation
+`pip install sarcharts`
+
 ### Usage
 ~~~
 usage: sarcharts.py [-h] [-d {D,I,W,E}] [-f FROMDATE] [-o OUTPUTPATH] [-t TODATE] [sarfilespaths ...]
 
 SarCharts gets "sysstat" files from provided `sarfilespaths` and generates dynamic HTML Charts.
 
 positional arguments:
```

### Comparing `sarcharts-0.1.7/README.md` & `sarcharts-0.1.8/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 ### SarCharts
 SarCharts gets [sysstat](https://sysstat.github.io/) files from provided `sarfilespaths` and generates dynamic HTML Charts.
 
 ### Requirements
 `sadf` command is needed to read sar files. Hence [sysstat](https://sysstat.github.io/) package is required.
 
+### Installation
+`pip install sarcharts`
+
 ### Usage
 ~~~
 usage: sarcharts.py [-h] [-d {D,I,W,E}] [-f FROMDATE] [-o OUTPUTPATH] [-t TODATE] [sarfilespaths ...]
 
 SarCharts gets "sysstat" files from provided `sarfilespaths` and generates dynamic HTML Charts.
 
 positional arguments:
```

### Comparing `sarcharts-0.1.7/doc/README.md` & `sarcharts-0.1.8/doc/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 ### SarCharts
 SarCharts gets [sysstat](https://sysstat.github.io/) files from provided `sarfilespaths` and generates dynamic HTML Charts.
 
 ### Requirements
 `sadf` command is needed to read sar files. Hence [sysstat](https://sysstat.github.io/) package is required.
 
+### Installation
+`pip install sarcharts`
+
 ### Usage
 ~~~
 usage: sarcharts.py [-h] [-d {D,I,W,E}] [-f FROMDATE] [-o OUTPUTPATH] [-t TODATE] [sarfilespaths ...]
 
 SarCharts gets "sysstat" files from provided `sarfilespaths` and generates dynamic HTML Charts.
 
 positional arguments:
```

### Comparing `sarcharts-0.1.7/doc/sarcharts.png` & `sarcharts-0.1.8/doc/sarcharts.png`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.7/sarcharts/__init__.py` & `sarcharts-0.1.8/sarcharts/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,19 +13,29 @@
 
 
 class SarCharts:
     args = ()
     cwd = os.getcwd()
     C = ChartsConf()
 
-    def valid_date(self, date):
-        try:
-            return datetime.datetime.strptime(date, "%Y-%m-%d %H:%M:%S")
-        except ValueError:
-            raise argparse.ArgumentTypeError(f"not a valid date: {date!r}")
+    def valid_date(self, d):
+        valid = ["%Y-%m-%d %H:%M:%S",
+                 "%Y-%m-%d %H",
+                 "%Y-%m-%d %H:%M",
+                 "%Y-%m-%d"
+                 ]
+        format = "%Y-%m-%d %H:%M:%S"
+        for v in valid:
+            try:
+                o = datetime.datetime.strptime(d, v)
+                return datetime.datetime.strptime(str(o), format)
+            except ValueError:
+                pass
+        raise argparse.ArgumentTypeError(
+            f"not a valid date: {d!r}. Valid formats: {str(valid)}")
 
     def valid_path(self, path):
         if os.path.exists(path):
             return path
         else:
             raise argparse.ArgumentTypeError(f"not a valid path: {path!r}")
```

### Comparing `sarcharts-0.1.7/sarcharts/html/css/sarcharts.css` & `sarcharts-0.1.8/sarcharts/html/css/sarcharts.css`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.7/sarcharts/html/js/chart.umd.js` & `sarcharts-0.1.8/sarcharts/html/js/chart.umd.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.7/sarcharts/html/js/chartjs-plugin-zoom.min.js` & `sarcharts-0.1.8/sarcharts/html/js/chartjs-plugin-zoom.min.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.7/sarcharts/html/js/hammer.min.js` & `sarcharts-0.1.8/sarcharts/html/js/hammer.min.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.7/sarcharts/html/js/jquery.js` & `sarcharts-0.1.8/sarcharts/html/js/jquery.js`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.7/sarcharts/lib/chartjs.py` & `sarcharts-0.1.8/sarcharts/lib/chartjs.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.7/sarcharts/lib/chartsconf.py` & `sarcharts-0.1.8/sarcharts/lib/chartsconf.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.7/sarcharts/lib/progressbar.py` & `sarcharts-0.1.8/sarcharts/lib/progressbar.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.7/sarcharts/lib/sadf.py` & `sarcharts-0.1.8/sarcharts/lib/sadf.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,37 +5,37 @@
 from sarcharts.lib.progressbar import ProgressBar
 from sarcharts.lib import util
 
 
 class Sadf:
 
     def sar_to_csv(self, inputfile, arg, debuglevel):
-        command = f"sadf -d {inputfile} -- {arg}"
+        command = f"sadf -td {inputfile} -- {arg}"
         [stdout, stderr] = util.exec_command(debuglevel, command)
         if stderr:
             if "Try to convert it to current format" in stderr:
                 # tf = tempfile.NamedTemporaryFile(prefix="sarcharts")
                 command = f"sadf -c {inputfile} > /tmp/sarcharts.tmp"
                 [stdout, stderr] = util.exec_command(debuglevel, command)
-                return self.sar_to_csv(
-                    "/tmp/sarcharts.tmp", arg, debuglevel
-                    )
+                return self.sar_to_csv("/tmp/sarcharts.tmp", arg, debuglevel)
             elif "Requested activities not available" in stderr:
                 util.debug(debuglevel, 'I', stderr.strip())
             else:
                 util.debug(debuglevel, 'W', command)
                 util.debug(debuglevel, 'W', stderr.strip())
         else:
             out = []
             for line in stdout.split("\n"):
                 if line != "":
-                    out.append(line.split(";"))
+                    tmp = line.split(";")
+                    out.append(tmp)
             return out
 
-    def merge_sarfiles(self, debuglevel, sarfiles, outputpath, charts, dfrom, dto):
+    def merge_sarfiles(
+            self, debuglevel, sarfiles, outputpath, charts, dfrom, dto):
         pb = ProgressBar()
         pb.all_entries = len(charts) * len(sarfiles)
         pb.start_time = datetime.datetime.now()
         pbi = 0
         for k, v in charts.items():
             content = []
             csvfile = f"{outputpath}/{k}.csv"
@@ -52,16 +52,18 @@
                                f"Merge {inputfile} to {csvfile}")
                     content = content + out
             if out:
                 with open(csvfile, "w") as f:
                     f.write(';'.join(headers) + "\n")
                     content.sort(key=lambda x: x[2])
                     for line in content:
-                        if (line[2] != "timestamp" and util.in_date_range(
-                                debuglevel, dfrom, dto, line[2])):
+                        if ("LINUX-RESTART" not in line[3]
+                                and line[2] != "timestamp"
+                                and util.in_date_range(
+                                    debuglevel, dfrom, dto, line[2])):
                             f.write(';'.join(line) + "\n")
         pb.finish("  Get data.")
 
     def sar_to_chartjs(
             self, debuglevel, sarfiles, outputpath, charts, dfrom, dto):
         self.merge_sarfiles(
             debuglevel, sarfiles, outputpath, charts, dfrom, dto)
@@ -92,16 +94,14 @@
                     pos = f.tell()
                     line = f.readline().split(";")
                     chartinfo['hostname'] = line[0]
                     chartinfo['firstdate'] = line[2]
                     # seek file to first stats line
                     f.seek(pos)
                     for line in f:
-                        if "LINUX-RESTART" in line or re.match(r"^#", line):
-                            continue
                         fields = line.strip().split(";")
                         # set fake item on non multiple charts
                         item = fields[3] if charts[k]['multiple'] else ""
                         # add date field to Chart labels
                         if fields[2] not in charts[k]['labels']:
                             charts[k]['labels'].append(fields[2])
                         if item not in charts[k]['datasets'].keys():
```

### Comparing `sarcharts-0.1.7/sarcharts/lib/util.py` & `sarcharts-0.1.8/sarcharts/lib/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import datetime
 import os
-import re
 import sys
 
 import fnmatch
 from pathlib import Path
 import subprocess
 
 
@@ -64,30 +63,24 @@
         mtime = os.path.getmtime(f)
         details[mtime] = f
     # 'sorted' returns a 'set' hence no duplicates
     # but it should be converted to a list
     return list(dict(sorted(details.items())).values())
 
 
-def valid_date(s: str) -> datetime.datetime:
-    try:
-        return datetime.datetime.strptime(s, "%Y-%m-%d %H:%M:%S")
-    except ValueError:
-        return False
+def valid_date(debuglevel, d):
+    formats = ["%Y-%m-%d %H:%M:%S %Z", "%Y-%m-%d %H:%M:%S"]
+    for format in formats:
+        try:
+            return datetime.datetime.strptime(d, format)
+        except ValueError:
+            pass
+    debug(debuglevel, 'E',
+          f"ERROR: date '{d}' doesn't match {str(formats)}.")
 
 
-def is_valid_date(debuglevel, d):
-    if re.match(r'\d{4}-\d{2}-\d{2} \d{2}:\d{2}:\d{2} UTC', d):
+def in_date_range(debuglevel, dfrom, dto, d):
+    d = valid_date(debuglevel, d)
+    if d >= dfrom and d <= dto:
         return True
     else:
-        debug(debuglevel, 'E', "ERROR: date '" + d
-              + "' doesn't match %Y-%m-%d %H:%M:%S UTC")
-
-
-def in_date_range(debuglevel, dfrom, dto, d):
-    if is_valid_date(debuglevel, d):
-        d = datetime.datetime.strptime(d, '%Y-%m-%d %H:%M:%S UTC')
-        if dfrom and dto:
-            if d >= dfrom and d <= dto:
-                return True
-        else:
-            return True
+        return False
```

### Comparing `sarcharts-0.1.7/sarcharts/templates/chart.html` & `sarcharts-0.1.8/sarcharts/templates/chart.html`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.7/sarcharts.egg-info/PKG-INFO` & `sarcharts-0.1.8/sarcharts.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarcharts
-Version: 0.1.7
+Version: 0.1.8
 Summary: SarCharts gets sysstat files from provided sarfilespaths and generates dynamic HTML Charts
 Home-page: https://github.com/pafernanr/sarcharts
 Author: Pablo Fernández Rodríguez
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
@@ -22,14 +22,17 @@
 
 ### SarCharts
 SarCharts gets [sysstat](https://sysstat.github.io/) files from provided `sarfilespaths` and generates dynamic HTML Charts.
 
 ### Requirements
 `sadf` command is needed to read sar files. Hence [sysstat](https://sysstat.github.io/) package is required.
 
+### Installation
+`pip install sarcharts`
+
 ### Usage
 ~~~
 usage: sarcharts.py [-h] [-d {D,I,W,E}] [-f FROMDATE] [-o OUTPUTPATH] [-t TODATE] [sarfilespaths ...]
 
 SarCharts gets "sysstat" files from provided `sarfilespaths` and generates dynamic HTML Charts.
 
 positional arguments:
```

### Comparing `sarcharts-0.1.7/sarcharts.egg-info/SOURCES.txt` & `sarcharts-0.1.8/sarcharts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.7/setup.cfg` & `sarcharts-0.1.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.7/setup.py` & `sarcharts-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `sarcharts-0.1.7/tox.ini` & `sarcharts-0.1.8/tox.ini`

 * *Files identical despite different names*

