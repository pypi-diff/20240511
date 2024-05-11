# Comparing `tmp/OWSLib-0.9.1.tar.gz` & `tmp/OWSLib-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/OWSLib-0.9.1.tar", last modified: Thu Sep  3 23:38:01 2015, max compression
+gzip compressed data, was "dist/OWSLib-0.9.2.tar", last modified: Thu Sep 24 00:07:14 2015, max compression
```

## Comparing `OWSLib-0.9.1.tar` & `OWSLib-0.9.2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 tkralidi  (1000) tkralidi  (1000)        0 2015-09-03 23:38:01.000000 OWSLib-0.9.1/
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)       22 2014-11-24 01:41:10.000000 OWSLib-0.9.1/DEPENDENCIES.txt
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)       52 2014-11-24 01:41:10.000000 OWSLib-0.9.1/INSTALL.txt
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)     1447 2014-11-24 01:41:10.000000 OWSLib-0.9.1/CHANGES.txt
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)     1732 2015-06-09 23:47:36.000000 OWSLib-0.9.1/setup.py
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)      522 2014-11-24 01:41:10.000000 OWSLib-0.9.1/CREDITS.txt
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)        6 2015-09-03 23:33:58.000000 OWSLib-0.9.1/VERSION.txt
-drwxr-xr-x   0 tkralidi  (1000) tkralidi  (1000)        0 2015-09-03 23:38:01.000000 OWSLib-0.9.1/owslib/
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)      980 2015-01-16 19:08:09.000000 OWSLib-0.9.1/owslib/sos.py
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)     2213 2015-07-28 11:56:38.000000 OWSLib-0.9.1/owslib/etree.py
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    24196 2015-07-03 15:39:33.000000 OWSLib-0.9.1/owslib/wms.py
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)     1742 2015-01-16 19:08:09.000000 OWSLib-0.9.1/owslib/wfs.py
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    16894 2015-06-09 23:47:36.000000 OWSLib-0.9.1/owslib/fes.py
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)     6723 2015-01-16 19:08:09.000000 OWSLib-0.9.1/owslib/wmc.py
-drwxr-xr-x   0 tkralidi  (1000) tkralidi  (1000)        0 2015-09-03 23:38:01.000000 OWSLib-0.9.1/owslib/waterml/
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)     1156 2015-06-09 23:47:36.000000 OWSLib-0.9.1/owslib/waterml/wml11.py
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)     1156 2015-06-09 23:47:36.000000 OWSLib-0.9.1/owslib/waterml/wml10.py
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)       68 2015-01-16 19:08:09.000000 OWSLib-0.9.1/owslib/waterml/__init__.py
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    32978 2015-01-16 19:08:09.000000 OWSLib-0.9.1/owslib/waterml/wml.py
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    22127 2015-07-02 00:29:20.000000 OWSLib-0.9.1/owslib/crs.py
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)     5587 2015-04-16 11:00:56.000000 OWSLib-0.9.1/owslib/namespaces.py
-drwxr-xr-x   0 tkralidi  (1000) tkralidi  (1000)        0 2015-09-03 23:38:01.000000 OWSLib-0.9.1/owslib/feature/
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    14558 2015-06-09 23:47:36.000000 OWSLib-0.9.1/owslib/feature/wfs110.py
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    18756 2015-08-07 14:58:39.000000 OWSLib-0.9.1/owslib/feature/wfs200.py
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    15760 2015-07-06 17:58:57.000000 OWSLib-0.9.1/owslib/feature/wfs100.py
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)     5792 2015-06-09 23:47:36.000000 OWSLib-0.9.1/owslib/feature/__init__.py
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    35403 2015-06-12 20:52:46.000000 OWSLib-0.9.1/owslib/csw.py
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    11849 2015-06-09 23:47:36.000000 OWSLib-0.9.1/owslib/tms.py
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    66408 2015-09-03 23:04:10.000000 OWSLib-0.9.1/owslib/wps.py
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    16918 2015-07-06 17:58:57.000000 OWSLib-0.9.1/owslib/util.py
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    10447 2015-01-16 19:08:09.000000 OWSLib-0.9.1/owslib/fgdc.py
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)     1550 2015-06-09 23:47:36.000000 OWSLib-0.9.1/owslib/wcs.py
-drwxr-xr-x   0 tkralidi  (1000) tkralidi  (1000)        0 2015-09-03 23:38:01.000000 OWSLib-0.9.1/owslib/swe/
-drwxr-xr-x   0 tkralidi  (1000) tkralidi  (1000)        0 2015-09-03 23:38:01.000000 OWSLib-0.9.1/owslib/swe/sensor/
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)       68 2015-01-16 19:08:09.000000 OWSLib-0.9.1/owslib/swe/sensor/__init__.py
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    14826 2015-06-09 23:47:36.000000 OWSLib-0.9.1/owslib/swe/sensor/sml.py
-drwxr-xr-x   0 tkralidi  (1000) tkralidi  (1000)        0 2015-09-03 23:38:01.000000 OWSLib-0.9.1/owslib/swe/observation/
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    12855 2015-06-09 23:47:36.000000 OWSLib-0.9.1/owslib/swe/observation/sos200.py
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    12996 2015-04-16 11:03:04.000000 OWSLib-0.9.1/owslib/swe/observation/sos100.py
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)       68 2015-01-16 19:08:09.000000 OWSLib-0.9.1/owslib/swe/observation/__init__.py
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    17823 2015-06-09 23:47:36.000000 OWSLib-0.9.1/owslib/swe/common.py
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)       68 2015-01-16 19:08:09.000000 OWSLib-0.9.1/owslib/swe/__init__.py
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    29164 2015-06-09 23:47:36.000000 OWSLib-0.9.1/owslib/wmts.py
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)     6066 2015-09-03 23:04:10.000000 OWSLib-0.9.1/owslib/interfaces.py
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)       90 2015-09-03 23:34:06.000000 OWSLib-0.9.1/owslib/__init__.py
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    19593 2015-01-16 19:08:09.000000 OWSLib-0.9.1/owslib/dif.py
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    38112 2015-09-03 23:04:10.000000 OWSLib-0.9.1/owslib/iso.py
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    10735 2015-06-10 12:13:52.000000 OWSLib-0.9.1/owslib/ows.py
-drwxr-xr-x   0 tkralidi  (1000) tkralidi  (1000)        0 2015-09-03 23:38:01.000000 OWSLib-0.9.1/owslib/coverage/
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)     6443 2015-06-09 23:47:36.000000 OWSLib-0.9.1/owslib/coverage/wcsBase.py
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    18950 2015-06-09 23:47:36.000000 OWSLib-0.9.1/owslib/coverage/wcs100.py
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)      881 2015-06-09 23:47:36.000000 OWSLib-0.9.1/owslib/coverage/wcs111.py
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    18251 2015-06-09 23:47:36.000000 OWSLib-0.9.1/owslib/coverage/wcs110.py
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)       68 2015-01-16 19:08:09.000000 OWSLib-0.9.1/owslib/coverage/__init__.py
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)     3909 2015-01-16 19:08:09.000000 OWSLib-0.9.1/owslib/coverage/wcsdecoder.py
-drwxr-xr-x   0 tkralidi  (1000) tkralidi  (1000)        0 2015-09-03 23:38:01.000000 OWSLib-0.9.1/OWSLib.egg-info/
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)     1202 2015-09-03 23:38:01.000000 OWSLib-0.9.1/OWSLib.egg-info/SOURCES.txt
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)     5387 2015-09-03 23:38:00.000000 OWSLib-0.9.1/OWSLib.egg-info/PKG-INFO
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)        1 2015-09-03 23:38:00.000000 OWSLib-0.9.1/OWSLib.egg-info/dependency_links.txt
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)        7 2015-09-03 23:38:00.000000 OWSLib-0.9.1/OWSLib.egg-info/top_level.txt
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)       47 2015-09-03 23:38:00.000000 OWSLib-0.9.1/OWSLib.egg-info/requires.txt
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)     5387 2015-09-03 23:38:01.000000 OWSLib-0.9.1/PKG-INFO
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)       34 2014-11-24 01:41:10.000000 OWSLib-0.9.1/requirements-dev.txt
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)      669 2014-11-24 01:41:10.000000 OWSLib-0.9.1/HISTORY.txt
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)       47 2015-07-28 11:56:38.000000 OWSLib-0.9.1/requirements.txt
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)       13 2014-11-24 01:41:10.000000 OWSLib-0.9.1/MANIFEST.in
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)     1549 2014-11-24 01:41:10.000000 OWSLib-0.9.1/LICENSE.txt
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)     3864 2014-11-24 01:41:10.000000 OWSLib-0.9.1/README.txt
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)       59 2015-09-03 23:38:01.000000 OWSLib-0.9.1/setup.cfg
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)        0 2014-11-24 01:41:10.000000 OWSLib-0.9.1/FAQ.txt
--rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)       17 2014-11-24 01:41:10.000000 OWSLib-0.9.1/requirements-2.6.txt
+drwxr-xr-x   0 tkralidi  (1000) tkralidi  (1000)        0 2015-09-24 00:07:14.000000 OWSLib-0.9.2/
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)       22 2015-09-24 00:06:17.000000 OWSLib-0.9.2/DEPENDENCIES.txt
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)       52 2015-09-24 00:06:17.000000 OWSLib-0.9.2/INSTALL.txt
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)     1447 2015-09-24 00:06:17.000000 OWSLib-0.9.2/CHANGES.txt
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)     1732 2015-09-24 00:06:17.000000 OWSLib-0.9.2/setup.py
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)      522 2015-09-24 00:06:17.000000 OWSLib-0.9.2/CREDITS.txt
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)        6 2015-09-24 00:06:17.000000 OWSLib-0.9.2/VERSION.txt
+drwxr-xr-x   0 tkralidi  (1000) tkralidi  (1000)        0 2015-09-24 00:07:14.000000 OWSLib-0.9.2/owslib/
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)      980 2015-09-24 00:06:17.000000 OWSLib-0.9.2/owslib/sos.py
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)     2213 2015-09-24 00:06:17.000000 OWSLib-0.9.2/owslib/etree.py
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    27171 2015-09-24 00:06:17.000000 OWSLib-0.9.2/owslib/wms.py
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)     1742 2015-09-24 00:06:17.000000 OWSLib-0.9.2/owslib/wfs.py
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    16894 2015-09-24 00:06:17.000000 OWSLib-0.9.2/owslib/fes.py
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)     6723 2015-09-24 00:06:17.000000 OWSLib-0.9.2/owslib/wmc.py
+drwxr-xr-x   0 tkralidi  (1000) tkralidi  (1000)        0 2015-09-24 00:07:14.000000 OWSLib-0.9.2/owslib/waterml/
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)     1156 2015-09-24 00:06:17.000000 OWSLib-0.9.2/owslib/waterml/wml11.py
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)     1156 2015-09-24 00:06:17.000000 OWSLib-0.9.2/owslib/waterml/wml10.py
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)       68 2015-09-24 00:06:17.000000 OWSLib-0.9.2/owslib/waterml/__init__.py
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    32978 2015-09-24 00:06:17.000000 OWSLib-0.9.2/owslib/waterml/wml.py
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    22127 2015-09-24 00:06:17.000000 OWSLib-0.9.2/owslib/crs.py
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)     5587 2015-09-24 00:06:17.000000 OWSLib-0.9.2/owslib/namespaces.py
+drwxr-xr-x   0 tkralidi  (1000) tkralidi  (1000)        0 2015-09-24 00:07:14.000000 OWSLib-0.9.2/owslib/feature/
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    14558 2015-09-24 00:06:17.000000 OWSLib-0.9.2/owslib/feature/wfs110.py
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    18756 2015-09-24 00:06:17.000000 OWSLib-0.9.2/owslib/feature/wfs200.py
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    15760 2015-09-24 00:06:17.000000 OWSLib-0.9.2/owslib/feature/wfs100.py
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)     5792 2015-09-24 00:06:17.000000 OWSLib-0.9.2/owslib/feature/__init__.py
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    35403 2015-09-24 00:06:17.000000 OWSLib-0.9.2/owslib/csw.py
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    11849 2015-09-24 00:06:17.000000 OWSLib-0.9.2/owslib/tms.py
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    66408 2015-09-24 00:06:17.000000 OWSLib-0.9.2/owslib/wps.py
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    17341 2015-09-24 00:06:17.000000 OWSLib-0.9.2/owslib/util.py
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    10447 2015-09-24 00:06:17.000000 OWSLib-0.9.2/owslib/fgdc.py
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)     1550 2015-09-24 00:06:17.000000 OWSLib-0.9.2/owslib/wcs.py
+drwxr-xr-x   0 tkralidi  (1000) tkralidi  (1000)        0 2015-09-24 00:07:14.000000 OWSLib-0.9.2/owslib/swe/
+drwxr-xr-x   0 tkralidi  (1000) tkralidi  (1000)        0 2015-09-24 00:07:14.000000 OWSLib-0.9.2/owslib/swe/sensor/
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)       68 2015-09-24 00:06:17.000000 OWSLib-0.9.2/owslib/swe/sensor/__init__.py
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    14826 2015-09-24 00:06:17.000000 OWSLib-0.9.2/owslib/swe/sensor/sml.py
+drwxr-xr-x   0 tkralidi  (1000) tkralidi  (1000)        0 2015-09-24 00:07:14.000000 OWSLib-0.9.2/owslib/swe/observation/
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    12855 2015-09-24 00:06:17.000000 OWSLib-0.9.2/owslib/swe/observation/sos200.py
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    12996 2015-09-24 00:06:17.000000 OWSLib-0.9.2/owslib/swe/observation/sos100.py
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)       68 2015-09-24 00:06:17.000000 OWSLib-0.9.2/owslib/swe/observation/__init__.py
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    17823 2015-09-24 00:06:17.000000 OWSLib-0.9.2/owslib/swe/common.py
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)       68 2015-09-24 00:06:17.000000 OWSLib-0.9.2/owslib/swe/__init__.py
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    31462 2015-09-24 00:06:17.000000 OWSLib-0.9.2/owslib/wmts.py
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)     6066 2015-09-24 00:06:17.000000 OWSLib-0.9.2/owslib/interfaces.py
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)       90 2015-09-24 00:06:17.000000 OWSLib-0.9.2/owslib/__init__.py
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    19593 2015-09-24 00:06:17.000000 OWSLib-0.9.2/owslib/dif.py
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    38112 2015-09-24 00:06:17.000000 OWSLib-0.9.2/owslib/iso.py
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    10735 2015-09-24 00:06:17.000000 OWSLib-0.9.2/owslib/ows.py
+drwxr-xr-x   0 tkralidi  (1000) tkralidi  (1000)        0 2015-09-24 00:07:14.000000 OWSLib-0.9.2/owslib/coverage/
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)     6443 2015-09-24 00:06:17.000000 OWSLib-0.9.2/owslib/coverage/wcsBase.py
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    18950 2015-09-24 00:06:17.000000 OWSLib-0.9.2/owslib/coverage/wcs100.py
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)      881 2015-09-24 00:06:17.000000 OWSLib-0.9.2/owslib/coverage/wcs111.py
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)    18251 2015-09-24 00:06:17.000000 OWSLib-0.9.2/owslib/coverage/wcs110.py
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)       68 2015-09-24 00:06:17.000000 OWSLib-0.9.2/owslib/coverage/__init__.py
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)     3909 2015-09-24 00:06:17.000000 OWSLib-0.9.2/owslib/coverage/wcsdecoder.py
+drwxr-xr-x   0 tkralidi  (1000) tkralidi  (1000)        0 2015-09-24 00:07:14.000000 OWSLib-0.9.2/OWSLib.egg-info/
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)     1202 2015-09-24 00:07:14.000000 OWSLib-0.9.2/OWSLib.egg-info/SOURCES.txt
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)     5387 2015-09-24 00:07:12.000000 OWSLib-0.9.2/OWSLib.egg-info/PKG-INFO
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)        1 2015-09-24 00:07:12.000000 OWSLib-0.9.2/OWSLib.egg-info/dependency_links.txt
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)        7 2015-09-24 00:07:12.000000 OWSLib-0.9.2/OWSLib.egg-info/top_level.txt
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)       47 2015-09-24 00:07:12.000000 OWSLib-0.9.2/OWSLib.egg-info/requires.txt
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)     5387 2015-09-24 00:07:14.000000 OWSLib-0.9.2/PKG-INFO
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)       34 2015-09-24 00:06:17.000000 OWSLib-0.9.2/requirements-dev.txt
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)      669 2015-09-24 00:06:17.000000 OWSLib-0.9.2/HISTORY.txt
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)       47 2015-09-24 00:06:17.000000 OWSLib-0.9.2/requirements.txt
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)       13 2015-09-24 00:06:17.000000 OWSLib-0.9.2/MANIFEST.in
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)     1549 2015-09-24 00:06:17.000000 OWSLib-0.9.2/LICENSE.txt
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)     3864 2015-09-24 00:06:17.000000 OWSLib-0.9.2/README.txt
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)       59 2015-09-24 00:07:14.000000 OWSLib-0.9.2/setup.cfg
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)        0 2015-09-24 00:06:17.000000 OWSLib-0.9.2/FAQ.txt
+-rw-r--r--   0 tkralidi  (1000) tkralidi  (1000)       17 2015-09-24 00:06:17.000000 OWSLib-0.9.2/requirements-2.6.txt
```

### Comparing `OWSLib-0.9.1/CHANGES.txt` & `OWSLib-0.9.2/CHANGES.txt`

 * *Files identical despite different names*

### Comparing `OWSLib-0.9.1/setup.py` & `OWSLib-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `OWSLib-0.9.1/CREDITS.txt` & `OWSLib-0.9.2/CREDITS.txt`

 * *Files identical despite different names*

### Comparing `OWSLib-0.9.1/owslib/sos.py` & `OWSLib-0.9.2/owslib/sos.py`

 * *Files identical despite different names*

### Comparing `OWSLib-0.9.1/owslib/etree.py` & `OWSLib-0.9.2/owslib/etree.py`

 * *Files identical despite different names*

### Comparing `OWSLib-0.9.1/owslib/wms.py` & `OWSLib-0.9.2/owslib/wms.py`

 * *Files 8% similar despite different names*

```diff
@@ -119,21 +119,24 @@
         #layer as a metadata organizer, nothing more.
         self.contents = OrderedDict()
         caps = self._capabilities.find('Capability')
         
         #recursively gather content metadata for all layer elements.
         #To the WebMapService.contents store only metadata of named layers.
         def gather_layers(parent_elem, parent_metadata):
+            layers = []
             for index, elem in enumerate(parent_elem.findall('Layer')):
                 cm = ContentMetadata(elem, parent=parent_metadata, index=index+1, parse_remote_metadata=parse_remote_metadata)
                 if cm.id:
                     if cm.id in self.contents:
                         warnings.warn('Content metadata for layer "%s" already exists. Using child layer' % cm.id)
+                    layers.append(cm)
                     self.contents[cm.id] = cm
-                gather_layers(elem, cm)
+                cm.children = gather_layers(elem, cm)
+            return layers
         gather_layers(caps, None)
         
         #exceptions
         self.exceptions = [f.text for f \
                 in self._capabilities.findall('Capability/Exception/Format')]
             
     def items(self):
@@ -156,14 +159,49 @@
         if u.info()['Content-Type'] == 'application/vnd.ogc.se_xml':
             se_xml = u.read()
             se_tree = etree.fromstring(se_xml)
             err_message = str(se_tree.find('ServiceException').text).strip()
             raise ServiceException(err_message, se_xml)
         return u
 
+    def __build_getmap_request(self, layers=None, styles=None, srs=None, bbox=None,
+               format=None, size=None, time=None, transparent=False,
+               bgcolor=None, exceptions=None, **kwargs):
+
+        request = {'version': self.version, 'request': 'GetMap'}
+
+        # check layers and styles
+        assert len(layers) > 0
+        request['layers'] = ','.join(layers)
+        if styles:
+            assert len(styles) == len(layers)
+            request['styles'] = ','.join(styles)
+        else:
+            request['styles'] = ''
+
+        # size
+        request['width'] = str(size[0])
+        request['height'] = str(size[1])
+
+        request['srs'] = str(srs)
+        request['bbox'] = ','.join([repr(x) for x in bbox])
+        request['format'] = str(format)
+        request['transparent'] = str(transparent).upper()
+        request['bgcolor'] = '0x' + bgcolor[1:7]
+        request['exceptions'] = str(exceptions)
+
+        if time is not None:
+            request['time'] = str(time)
+
+        if kwargs:
+            for kw in kwargs:
+                request[kw]=kwargs[kw]
+
+        return request
+
     def getmap(self, layers=None, styles=None, srs=None, bbox=None,
                format=None, size=None, time=None, transparent=False,
                bgcolor='#FFFFFF',
                exceptions='application/vnd.ogc.se_xml',
                method='Get',
                timeout=None,
                **kwargs
@@ -209,64 +247,83 @@
             >>> out.close()
 
         """        
         try:
             base_url = next((m.get('url') for m in self.getOperationByName('GetMap').methods if m.get('type').lower() == method.lower()))
         except StopIteration:
             base_url = self.url
-        request = {'version': self.version, 'request': 'GetMap'}
-        
-        # check layers and styles
-        assert len(layers) > 0
-        request['layers'] = ','.join(layers)
-        if styles:
-            assert len(styles) == len(layers)
-            request['styles'] = ','.join(styles)
-        else:
-            request['styles'] = ''
 
-        # size
-        request['width'] = str(size[0])
-        request['height'] = str(size[1])
-        
-        request['srs'] = str(srs)
-        request['bbox'] = ','.join([repr(x) for x in bbox])
-        request['format'] = str(format)
-        request['transparent'] = str(transparent).upper()
-        request['bgcolor'] = '0x' + bgcolor[1:7]
-        request['exceptions'] = str(exceptions)
+        request = self.__build_getmap_request(layers=layers, styles=styles, srs=srs, bbox=bbox,
+               format=format, size=size, time=time, transparent=transparent,
+               bgcolor=bgcolor, exceptions=exceptions, kwargs=kwargs)
         
-        if time is not None:
-            request['time'] = str(time)
+        data = urlencode(request)
         
-        if kwargs:
-            for kw in kwargs:
-                request[kw]=kwargs[kw]
+        u = openURL(base_url, data, method, username=self.username, password=self.password, timeout=timeout or self.timeout)
+
+        # check for service exceptions, and return
+        if u.info()['Content-Type'] == 'application/vnd.ogc.se_xml':
+            se_xml = u.read()
+            se_tree = etree.fromstring(se_xml)
+            err_message = six.text_type(se_tree.find('ServiceException').text).strip()
+            raise ServiceException(err_message, se_xml)
+        return u
+
+
+    def getfeatureinfo(self, layers=None, styles=None, srs=None, bbox=None,
+               format=None, size=None, time=None, transparent=False,
+               bgcolor='#FFFFFF',
+               exceptions='application/vnd.ogc.se_xml',
+               query_layers = None, xy=None, info_format=None, feature_count=20,
+               method='Get',
+               timeout=None,
+               **kwargs
+               ):
+        try:
+            base_url = next((m.get('url') for m in self.getOperationByName('GetFeatureInfo').methods if m.get('type').lower() == method.lower()))
+        except StopIteration:
+            base_url = self.url
+
+        # GetMap-Request
+        request = self.__build_getmap_request(layers=layers, styles=styles, srs=srs, bbox=bbox,
+               format=format, size=size, time=time, transparent=transparent,
+               bgcolor=bgcolor, exceptions=exceptions, kwargs=kwargs)
+
+        # extend to GetFeatureInfo-Request
+        request['request'] = 'GetFeatureInfo'
+
+        if not query_layers:
+            __str_query_layers = ','.join(layers)
+        else:
+            __str_query_layers = ','.join(query_layers)
+
+        request['query_layers'] = __str_query_layers
+        request['x'] = str(xy[0])
+        request['y'] = str(xy[1])
+        request['info_format'] = info_format
+        request['feature_count'] = str(feature_count)
 
         data = urlencode(request)
-        
+
         u = openURL(base_url, data, method, username=self.username, password=self.password, timeout=timeout or self.timeout)
 
         # check for service exceptions, and return
         if u.info()['Content-Type'] == 'application/vnd.ogc.se_xml':
             se_xml = u.read()
             se_tree = etree.fromstring(se_xml)
             err_message = six.text_type(se_tree.find('ServiceException').text).strip()
             raise ServiceException(err_message, se_xml)
         return u
-        
+
     def getServiceXML(self):
         xml = None
         if self._capabilities is not None:
             xml = etree.tostring(self._capabilities)
         return xml
 
-    def getfeatureinfo(self):
-        raise NotImplementedError
-
     def getOperationByName(self, name): 
         """Return a named content item."""
         for item in self.operations:
             if item.name == name:
                 return item
         raise KeyError("No operation named %s" % name)
     
@@ -318,23 +375,25 @@
         
 class ContentMetadata:
     """
     Abstraction for WMS layer metadata.
 
     Implements IContentMetadata.
     """
-    def __init__(self, elem, parent=None, index=0, parse_remote_metadata=False, timeout=30):
+    def __init__(self, elem, parent=None, children=None, index=0, parse_remote_metadata=False, timeout=30):
         if elem.tag != 'Layer':
             raise ValueError('%s should be a Layer' % (elem,))
         
         self.parent = parent
         if parent:
             self.index = "%s.%d" % (parent.index, index)
         else:
             self.index = str(index)
+
+        self._children = children
         
         self.id = self.name = testXMLValue(elem.find('Name'))
 
         # layer attributes
         self.queryable = int(elem.attrib.get('queryable', 0))
         self.cascaded = int(elem.attrib.get('cascaded', 0))
         self.opaque = int(elem.attrib.get('opaque', 0))
@@ -506,14 +565,32 @@
             }
             self.dataUrls.append(dataUrl)
                 
         self.layers = []
         for child in elem.findall('Layer'):
             self.layers.append(ContentMetadata(child, self))
 
+    @property
+    def children(self):
+        return self._children
+
+    @children.setter
+    def children(self, value):
+        if self._children is None:
+            self._children = value
+        else:
+            self._children.extend(value)
+        # If layer is a group and one of its children is queryable, the layer must be queryable.
+        if self._children and self.queryable == 0:
+            for child in self._children:
+                if child.queryable:
+                    self.queryable = child.queryable
+                    break
+
+
     def __str__(self):
         return 'Layer Name: %s Title: %s' % (self.name, self.title)
 
 
 class OperationMetadata:
     """Abstraction for WMS OperationMetadata.
```

### Comparing `OWSLib-0.9.1/owslib/wfs.py` & `OWSLib-0.9.2/owslib/wfs.py`

 * *Files identical despite different names*

### Comparing `OWSLib-0.9.1/owslib/fes.py` & `OWSLib-0.9.2/owslib/fes.py`

 * *Files identical despite different names*

### Comparing `OWSLib-0.9.1/owslib/wmc.py` & `OWSLib-0.9.2/owslib/wmc.py`

 * *Files identical despite different names*

### Comparing `OWSLib-0.9.1/owslib/waterml/wml11.py` & `OWSLib-0.9.2/owslib/waterml/wml11.py`

 * *Files identical despite different names*

### Comparing `OWSLib-0.9.1/owslib/waterml/wml10.py` & `OWSLib-0.9.2/owslib/waterml/wml10.py`

 * *Files identical despite different names*

### Comparing `OWSLib-0.9.1/owslib/waterml/wml.py` & `OWSLib-0.9.2/owslib/waterml/wml.py`

 * *Files identical despite different names*

### Comparing `OWSLib-0.9.1/owslib/crs.py` & `OWSLib-0.9.2/owslib/crs.py`

 * *Files identical despite different names*

### Comparing `OWSLib-0.9.1/owslib/namespaces.py` & `OWSLib-0.9.2/owslib/namespaces.py`

 * *Files identical despite different names*

### Comparing `OWSLib-0.9.1/owslib/feature/wfs110.py` & `OWSLib-0.9.2/owslib/feature/wfs110.py`

 * *Files identical despite different names*

### Comparing `OWSLib-0.9.1/owslib/feature/wfs200.py` & `OWSLib-0.9.2/owslib/feature/wfs200.py`

 * *Files identical despite different names*

### Comparing `OWSLib-0.9.1/owslib/feature/wfs100.py` & `OWSLib-0.9.2/owslib/feature/wfs100.py`

 * *Files identical despite different names*

### Comparing `OWSLib-0.9.1/owslib/feature/__init__.py` & `OWSLib-0.9.2/owslib/feature/__init__.py`

 * *Files identical despite different names*

### Comparing `OWSLib-0.9.1/owslib/csw.py` & `OWSLib-0.9.2/owslib/csw.py`

 * *Files identical despite different names*

### Comparing `OWSLib-0.9.1/owslib/tms.py` & `OWSLib-0.9.2/owslib/tms.py`

 * *Files identical despite different names*

### Comparing `OWSLib-0.9.1/owslib/wps.py` & `OWSLib-0.9.2/owslib/wps.py`

 * *Files identical despite different names*

### Comparing `OWSLib-0.9.1/owslib/util.py` & `OWSLib-0.9.2/owslib/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -143,15 +143,15 @@
 def openURL(url_base, data=None, method='Get', cookies=None, username=None, password=None, timeout=30):
     """
     Function to open URLs.
 
     Uses requests library but with additional checks for OGC service exceptions and url formatting.
     Also handles cookies and simple user password authentication.
     """
-    headers = {}
+    headers = None
     rkwargs = {}
 
     rkwargs['timeout'] = timeout
 
     auth = None
     if username and password:
         auth = (username, password)
@@ -161,30 +161,32 @@
     # FIXUP for WFS in particular, remove xml style namespace
     # @TODO does this belong here?
     method = method.split("}")[-1]
 
     if method.lower() == 'post':
         try:
             xml = etree.fromstring(data)
-            headers['Content-Type'] = "text/xml"
+            headers = {'Content-Type': 'text/xml'}
         except (ParseError, UnicodeEncodeError):
             pass
 
         rkwargs['data'] = data
 
     elif method.lower() == 'get':
         rkwargs['params'] = data
+        
     else:
         raise ValueError("Unknown method ('%s'), expected 'get' or 'post'" % method)
 
     if cookies is not None:
         rkwargs['cookies'] = cookies
 
     req = requests.request(method.upper(),
                            url_base,
+                           headers=headers,
                            **rkwargs)
 
     if req.status_code in [400, 401]:
         raise ServiceException(req.text)
 
     if req.status_code in [404]:    # add more if needed
         req.raise_for_status()
@@ -577,7 +579,20 @@
 # OrderedDict
 try:  # 2.7
     from collections import OrderedDict
 except:  # 2.6
     from ordereddict import OrderedDict
 
 
+def which_etree():
+    """decipher which etree library is being used by OWSLib"""
+
+    which_etree = None
+
+    if 'lxml' in etree.__file__:
+        which_etree = 'lxml.etree'
+    elif 'xml/etree' in etree.__file__:
+        which_etree = 'xml.etree'
+    elif 'elementree' in etree.__file__:
+        which_etree = 'elementtree.ElementTree'
+    
+    return which_etree
```

### Comparing `OWSLib-0.9.1/owslib/fgdc.py` & `OWSLib-0.9.2/owslib/fgdc.py`

 * *Files identical despite different names*

### Comparing `OWSLib-0.9.1/owslib/wcs.py` & `OWSLib-0.9.2/owslib/wcs.py`

 * *Files identical despite different names*

### Comparing `OWSLib-0.9.1/owslib/swe/sensor/sml.py` & `OWSLib-0.9.2/owslib/swe/sensor/sml.py`

 * *Files identical despite different names*

### Comparing `OWSLib-0.9.1/owslib/swe/observation/sos200.py` & `OWSLib-0.9.2/owslib/swe/observation/sos200.py`

 * *Files identical despite different names*

### Comparing `OWSLib-0.9.1/owslib/swe/observation/sos100.py` & `OWSLib-0.9.2/owslib/swe/observation/sos100.py`

 * *Files identical despite different names*

### Comparing `OWSLib-0.9.1/owslib/swe/common.py` & `OWSLib-0.9.2/owslib/swe/common.py`

 * *Files identical despite different names*

### Comparing `OWSLib-0.9.1/owslib/wmts.py` & `OWSLib-0.9.2/owslib/wmts.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 More extensive testing is needed and feedback (to bradh@frogmouth.net)
 would be appreciated.
 
 """
 
 from __future__ import (absolute_import, division, print_function)
 
+from random import randint
 import warnings
 import six
 from six.moves import filter
 try:                    # Python 3
     from urllib.parse import (urlencode, urlparse, urlunparse, parse_qs,
                               ParseResult)
 except ImportError:      # Python 2
@@ -195,16 +196,19 @@
 
         # serviceProvider metadata
         serviceprov = self._capabilities.find(_SERVICE_PROVIDER_TAG)
         self.provider = ServiceProvider(serviceprov)
 
         # serviceOperations metadata
         self.operations = []
-        for elem in self._capabilities.find(_OPERATIONS_METADATA_TAG)[:]:
-            self.operations.append(OperationsMetadata(elem))
+        serviceop = self._capabilities.find(_OPERATIONS_METADATA_TAG)
+        #  REST only WMTS does not have any Operations
+        if serviceop is not None:
+            for elem in serviceop[:]:
+                self.operations.append(OperationsMetadata(elem))
 
         # serviceContents metadata: our assumption is that services use
         # a top-level layer as a metadata organizer, nothing more.
         self.contents = {}
         caps = self._capabilities.find(_CONTENTS_TAG)
 
         def gather_layers(parent_elem, parent_metadata):
@@ -289,15 +293,14 @@
             ...                       tilematrix='6',
             ...                       row=4, column=4)
             'SERVICE=WMTS&REQUEST=GetTile&VERSION=1.0.0&\
 LAYER=VIIRS_CityLights_2012&STYLE=default&TILEMATRIXSET=EPSG4326_500m&\
 TILEMATRIX=6&TILEROW=4&TILECOL=4&FORMAT=image%2Fjpeg'
 
         """
-        request = {'version': self.version, 'request': 'GetTile'}
 
         if (layer is None):
             raise ValueError("layer is mandatory (cannot be None)")
         if style is None:
             style = list(self[layer].styles.keys())[0]
         if format is None:
             format = self[layer].formats[0]
@@ -325,14 +328,66 @@
 
         for key, value in six.iteritems(kwargs):
             request.append((key, value))
 
         data = urlencode(request, True)
         return data
 
+    def buildTileResource(self, layer=None, style=None, format=None,
+                          tilematrixset=None, tilematrix=None, row=None,
+                          column=None, **kwargs):
+
+        tileresourceurls = []
+        for resourceURL in self[layer].resourceURLs:
+            if resourceURL['resourceType'] == 'tile':
+                tileresourceurls.append(resourceURL)
+        numres = len(tileresourceurls)
+        if numres > 0:
+            # choose random ResourceURL if more than one available
+            resindex = randint(0, numres - 1)
+            resurl = tileresourceurls[resindex]['template']
+            if tilematrixset:
+                resurl = resurl.replace('{TileMatrixSet}', tilematrixset)
+            resurl = resurl.replace('{TileMatrix}', tilematrix)
+            resurl = resurl.replace('{TileRow}', row)
+            resurl = resurl.replace('{TileCol}', column)
+            if style:
+                resurl = resurl.replace('{Style}', style)
+            return resurl
+
+        return None
+
+    @property
+    def restonly(self):
+
+        # if OperationsMetadata is missing completely --> use REST
+        if len(self.operations) == 0:
+            return True
+
+        # check if KVP or RESTful are available
+        restenc = False
+        kvpenc = False
+        for operation in self.operations:
+            if operation.name == 'GetTile':
+                for method in operation.methods:
+                    if 'kvp' in str(method['constraints']).lower():
+                        kvpenc = True
+                    if 'rest' in str(method['constraints']).lower():
+                        restenc = True
+
+        # if KVP is available --> use KVP
+        if kvpenc:
+            return False
+
+        # if the operation has no constraint --> use KVP
+        if not kvpenc and not restenc:
+            return False
+
+        return restenc
+
     def gettile(self, base_url=None, layer=None, style=None, format=None,
                 tilematrixset=None, tilematrix=None, row=None, column=None,
                 **kwargs):
         """Return a tile from the WMTS.
 
         Returns the tile image as a file-like object.
 
@@ -375,14 +430,24 @@
             >>> out = open('tile.jpg', 'wb')
             >>> bytes_written = out.write(img.read())
             >>> out.close()
 
         """
         vendor_kwargs = self.vendor_kwargs or {}
         vendor_kwargs.update(kwargs)
+
+        # REST only WMTS
+        if self.restonly:
+            resurl = self.buildTileResource(
+                layer, style, format, tilematrixset, tilematrix,
+                row, column, **vendor_kwargs)
+            u = openURL(resurl, username=self.username, password=self.password)
+            return u
+
+        # KVP implemetation
         data = self.buildTileRequest(layer, style, format, tilematrixset,
                                      tilematrix, row, column, **vendor_kwargs)
 
         if base_url is None:
             base_url = self.url
             try:
                 methods = self.getOperationByName('GetTile').methods
```

### Comparing `OWSLib-0.9.1/owslib/interfaces.py` & `OWSLib-0.9.2/owslib/interfaces.py`

 * *Files identical despite different names*

### Comparing `OWSLib-0.9.1/owslib/dif.py` & `OWSLib-0.9.2/owslib/dif.py`

 * *Files identical despite different names*

### Comparing `OWSLib-0.9.1/owslib/iso.py` & `OWSLib-0.9.2/owslib/iso.py`

 * *Files identical despite different names*

### Comparing `OWSLib-0.9.1/owslib/ows.py` & `OWSLib-0.9.2/owslib/ows.py`

 * *Files identical despite different names*

### Comparing `OWSLib-0.9.1/owslib/coverage/wcsBase.py` & `OWSLib-0.9.2/owslib/coverage/wcsBase.py`

 * *Files identical despite different names*

### Comparing `OWSLib-0.9.1/owslib/coverage/wcs100.py` & `OWSLib-0.9.2/owslib/coverage/wcs100.py`

 * *Files identical despite different names*

### Comparing `OWSLib-0.9.1/owslib/coverage/wcs111.py` & `OWSLib-0.9.2/owslib/coverage/wcs111.py`

 * *Files identical despite different names*

### Comparing `OWSLib-0.9.1/owslib/coverage/wcs110.py` & `OWSLib-0.9.2/owslib/coverage/wcs110.py`

 * *Files identical despite different names*

### Comparing `OWSLib-0.9.1/owslib/coverage/wcsdecoder.py` & `OWSLib-0.9.2/owslib/coverage/wcsdecoder.py`

 * *Files identical despite different names*

### Comparing `OWSLib-0.9.1/OWSLib.egg-info/SOURCES.txt` & `OWSLib-0.9.2/OWSLib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OWSLib-0.9.1/OWSLib.egg-info/PKG-INFO` & `OWSLib-0.9.2/OWSLib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: OWSLib
-Version: 0.9.1
+Version: 0.9.2
 Summary: OGC Web Service utility library
 Home-page: http://geopython.github.io/OWSLib
 Author: Tom Kralidis
 Author-email: tomkralidis@gmail.com
 License: BSD
 Description: OWSLib
         ======
```

### Comparing `OWSLib-0.9.1/PKG-INFO` & `OWSLib-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: OWSLib
-Version: 0.9.1
+Version: 0.9.2
 Summary: OGC Web Service utility library
 Home-page: http://geopython.github.io/OWSLib
 Author: Tom Kralidis
 Author-email: tomkralidis@gmail.com
 License: BSD
 Description: OWSLib
         ======
```

### Comparing `OWSLib-0.9.1/HISTORY.txt` & `OWSLib-0.9.2/HISTORY.txt`

 * *Files identical despite different names*

### Comparing `OWSLib-0.9.1/LICENSE.txt` & `OWSLib-0.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `OWSLib-0.9.1/README.txt` & `OWSLib-0.9.2/README.txt`

 * *Files identical despite different names*

