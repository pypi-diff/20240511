# Comparing `tmp/pyyeti-1.4.1.1.tar.gz` & `tmp/pyyeti-1.4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyyeti-1.4.1.1.tar", last modified: Sat Apr 27 19:48:41 2024, max compression
+gzip compressed data, was "pyyeti-1.4.1.2.tar", last modified: Sat May 11 18:16:52 2024, max compression
```

## Comparing `pyyeti-1.4.1.1.tar` & `pyyeti-1.4.1.2.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-04-27 19:48:41.229643 pyyeti-1.4.1.1/
--rw-rw-r--   0 macro     (1000) macro     (1000)     1545 2024-03-30 16:48:11.000000 pyyeti-1.4.1.1/LICENSE.txt
--rw-rw-r--   0 macro     (1000) macro     (1000)      333 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/MANIFEST.in
--rw-r--r--   0 macro     (1000) macro     (1000)     4071 2024-04-27 19:48:41.229643 pyyeti-1.4.1.1/PKG-INFO
--rw-rw-r--   0 macro     (1000) macro     (1000)     3189 2024-03-30 16:48:01.000000 pyyeti-1.4.1.1/README.md
--rw-rw-r--   0 macro     (1000) macro     (1000)       89 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyproject.toml
-drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-04-27 19:48:41.209642 pyyeti-1.4.1.1/pyyeti/
--rw-rw-r--   0 macro     (1000) macro     (1000)     1035 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/__init__.py
--rw-rw-r--   0 macro     (1000) macro     (1000)   106855 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/cb.py
-drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-04-27 19:48:41.213642 pyyeti-1.4.1.1/pyyeti/cla/
--rw-rw-r--   0 macro     (1000) macro     (1000)      478 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/cla/__init__.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    15306 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/cla/_magpct.py
--rw-rw-r--   0 macro     (1000) macro     (1000)     4520 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/cla/_rptext1.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    36575 2024-04-27 19:48:26.000000 pyyeti-1.4.1.1/pyyeti/cla/_rptpct1.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    10341 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/cla/_rpttab1.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    21512 2024-03-30 16:35:32.000000 pyyeti-1.4.1.1/pyyeti/cla/_utilities.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    50944 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/cla/dr_def.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    27609 2024-01-28 18:47:10.000000 pyyeti-1.4.1.1/pyyeti/cla/dr_event.py
--rw-rw-r--   0 macro     (1000) macro     (1000)   111343 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/cla/dr_results.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    22910 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/cla/dr_results_plots.py
--rw-rw-r--   0 macro     (1000) macro     (1000)     7083 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/cla/rel_disp_dtm.py
--rw-rw-r--   0 macro     (1000) macro     (1000)     3912 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/column_plotter.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    24375 2024-03-30 16:14:58.000000 pyyeti-1.4.1.1/pyyeti/cyclecount.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    28432 2024-02-03 17:54:03.000000 pyyeti-1.4.1.1/pyyeti/datacursor.py
--rw-rw-r--   0 macro     (1000) macro     (1000)   127401 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/dsp.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    71114 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/era.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    42924 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/expmint.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    29847 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/fdepsd.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    48733 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/frclim.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    16400 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/guitools.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    16361 2024-01-28 18:47:10.000000 pyyeti-1.4.1.1/pyyeti/locate.py
-drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-04-27 19:48:41.217642 pyyeti-1.4.1.1/pyyeti/nastran/
--rw-rw-r--   0 macro     (1000) macro     (1000)      138 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/nastran/__init__.py
--rw-rw-r--   0 macro     (1000) macro     (1000)   189330 2024-03-30 16:12:46.000000 pyyeti-1.4.1.1/pyyeti/nastran/bulk.py
--rw-rw-r--   0 macro     (1000) macro     (1000)   136739 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/nastran/n2p.py
--rw-rw-r--   0 macro     (1000) macro     (1000)   177827 2024-02-25 16:48:06.000000 pyyeti-1.4.1.1/pyyeti/nastran/op2.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    91364 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/nastran/op4.py
-drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-04-27 19:48:41.217642 pyyeti-1.4.1.1/pyyeti/ode/
--rw-rw-r--   0 macro     (1000) macro     (1000)      869 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/ode/__init__.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    18978 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/ode/_base_ode_class.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    39142 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/ode/_utilities.py
--rw-rw-r--   0 macro     (1000) macro     (1000)     9992 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/ode/freqdirect.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    17472 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/ode/frf_mode_participation.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    10065 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/ode/solvecdf.py
--rw-rw-r--   0 macro     (1000) macro     (1000)     5653 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/ode/solveexp1.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    28080 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/ode/solveexp2.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    27510 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/ode/solvenewmark.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    71837 2024-02-25 16:48:06.000000 pyyeti-1.4.1.1/pyyeti/ode/solveunc.py
--rw-rw-r--   0 macro     (1000) macro     (1000)     9390 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/pp.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    43921 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/psd.py
-drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-04-27 19:48:41.217642 pyyeti-1.4.1.1/pyyeti/rainflow/
--rw-rw-r--   0 macro     (1000) macro     (1000)      195 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/rainflow/__init__.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    13898 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/rainflow/c_rain.c
--rw-rw-r--   0 macro     (1000) macro     (1000)     6540 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/rainflow/py_rain.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    75180 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/srs.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    11892 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/ssmodel.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    14070 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/stats.py
-drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-04-27 19:48:41.205642 pyyeti-1.4.1.1/pyyeti/tests/
-drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-04-27 19:48:41.221643 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_csuper/
--rw-rw-r--   0 macro     (1000) macro     (1000)     1622 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_csuper/inboard.asm
--rw-rw-r--   0 macro     (1000) macro     (1000)    25840 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_csuper/inboard.op4
--rw-rw-r--   0 macro     (1000) macro     (1000)     4727 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_csuper/inboard.pch
--rw-rw-r--   0 macro     (1000) macro     (1000)    15736 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_csuper/nas2cam.op2
--rw-rw-r--   0 macro     (1000) macro     (1000)   147552 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_csuper/nas2cam.op4
-drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-04-27 19:48:41.225643 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/
--rw-rw-r--   0 macro     (1000) macro     (1000)     2432 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/assemble.dat
--rw-rw-r--   0 macro     (1000) macro     (1000)   133180 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/assemble.op2
--rw-rw-r--   0 macro     (1000) macro     (1000)   162313 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/assemble.out
--rw-rw-r--   0 macro     (1000) macro     (1000)     1622 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/inboard.asm
--rw-rw-r--   0 macro     (1000) macro     (1000)     5827 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/inboard.blk
--rw-rw-r--   0 macro     (1000) macro     (1000)     6894 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/inboard.dat
--rw-rw-r--   0 macro     (1000) macro     (1000)    24052 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/inboard.op2
--rw-rw-r--   0 macro     (1000) macro     (1000)    36504 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/inboard.op4
--rw-rw-r--   0 macro     (1000) macro     (1000)   134889 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/inboard.out
--rw-rw-r--   0 macro     (1000) macro     (1000)     8939 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/inboard.pch
--rw-rw-r--   0 macro     (1000) macro     (1000)     2012 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/outboard.asm
--rw-rw-r--   0 macro     (1000) macro     (1000)     4946 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/outboard.blk
--rw-rw-r--   0 macro     (1000) macro     (1000)      767 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/outboard.dat
--rw-rw-r--   0 macro     (1000) macro     (1000)    38384 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/outboard.op4
--rw-rw-r--   0 macro     (1000) macro     (1000)    74780 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/outboard.out
--rw-rw-r--   0 macro     (1000) macro     (1000)     5944 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/outboard.pch
-drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-04-27 19:48:41.225643 pyyeti-1.4.1.1/pyyeti/tests/nastran_drm12/
--rw-rw-r--   0 macro     (1000) macro     (1000)    13464 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nastran_drm12/drm12.op2
--rw-rw-r--   0 macro     (1000) macro     (1000)    77852 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nastran_drm12/drm12.op4
--rw-rw-r--   0 macro     (1000) macro     (1000)    17160 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nastran_drm12/inboard_nas2cam.op2
--rw-rw-r--   0 macro     (1000) macro     (1000)    51624 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/tests/nastran_drm12/inboard_nas2cam.op4
--rw-rw-r--   0 macro     (1000) macro     (1000)    12371 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/writer.py
--rw-rw-r--   0 macro     (1000) macro     (1000)    61169 2024-01-24 22:45:59.000000 pyyeti-1.4.1.1/pyyeti/ytools.py
-drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-04-27 19:48:41.209642 pyyeti-1.4.1.1/pyyeti.egg-info/
--rw-r--r--   0 macro     (1000) macro     (1000)     4071 2024-04-27 19:48:41.000000 pyyeti-1.4.1.1/pyyeti.egg-info/PKG-INFO
--rw-rw-r--   0 macro     (1000) macro     (1000)     2311 2024-04-27 19:48:41.000000 pyyeti-1.4.1.1/pyyeti.egg-info/SOURCES.txt
--rw-rw-r--   0 macro     (1000) macro     (1000)        1 2024-04-27 19:48:41.000000 pyyeti-1.4.1.1/pyyeti.egg-info/dependency_links.txt
--rw-rw-r--   0 macro     (1000) macro     (1000)        7 2024-04-27 19:48:41.000000 pyyeti-1.4.1.1/pyyeti.egg-info/top_level.txt
-drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-04-27 19:48:41.225643 pyyeti-1.4.1.1/scripts/
--rwxrwxr-x   0 macro     (1000) macro     (1000)      861 2024-02-25 16:48:06.000000 pyyeti-1.4.1.1/scripts/lsop2
--rwxrwxr-x   0 macro     (1000) macro     (1000)      561 2024-02-25 16:48:06.000000 pyyeti-1.4.1.1/scripts/lsop4
--rw-rw-r--   0 macro     (1000) macro     (1000)      198 2024-04-27 19:48:41.229643 pyyeti-1.4.1.1/setup.cfg
--rw-rw-r--   0 macro     (1000) macro     (1000)     5161 2024-04-27 19:48:26.000000 pyyeti-1.4.1.1/setup.py
+drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-05-11 18:16:52.587719 pyyeti-1.4.1.2/
+-rw-rw-r--   0 macro     (1000) macro     (1000)     1545 2024-03-30 16:48:11.000000 pyyeti-1.4.1.2/LICENSE.txt
+-rw-rw-r--   0 macro     (1000) macro     (1000)      333 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/MANIFEST.in
+-rw-r--r--   0 macro     (1000) macro     (1000)     4071 2024-05-11 18:16:52.587719 pyyeti-1.4.1.2/PKG-INFO
+-rw-rw-r--   0 macro     (1000) macro     (1000)     3189 2024-03-30 16:48:01.000000 pyyeti-1.4.1.2/README.md
+-rw-rw-r--   0 macro     (1000) macro     (1000)       89 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyproject.toml
+drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-05-11 18:16:52.579718 pyyeti-1.4.1.2/pyyeti/
+-rw-rw-r--   0 macro     (1000) macro     (1000)     1035 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/__init__.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)   106855 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/cb.py
+drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-05-11 18:16:52.579718 pyyeti-1.4.1.2/pyyeti/cla/
+-rw-rw-r--   0 macro     (1000) macro     (1000)      478 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/cla/__init__.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    15306 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/cla/_magpct.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)     4520 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/cla/_rptext1.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    36575 2024-04-27 19:48:26.000000 pyyeti-1.4.1.2/pyyeti/cla/_rptpct1.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    10341 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/cla/_rpttab1.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    21512 2024-03-30 16:35:32.000000 pyyeti-1.4.1.2/pyyeti/cla/_utilities.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    50944 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/cla/dr_def.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    27609 2024-01-28 18:47:10.000000 pyyeti-1.4.1.2/pyyeti/cla/dr_event.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)   111343 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/cla/dr_results.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    22910 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/cla/dr_results_plots.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)     7083 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/cla/rel_disp_dtm.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)     3912 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/column_plotter.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    24375 2024-03-30 16:14:58.000000 pyyeti-1.4.1.2/pyyeti/cyclecount.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    28432 2024-02-03 17:54:03.000000 pyyeti-1.4.1.2/pyyeti/datacursor.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)   127401 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/dsp.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    71114 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/era.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    42924 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/expmint.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    29847 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/fdepsd.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    48733 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/frclim.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    16400 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/guitools.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    16361 2024-01-28 18:47:10.000000 pyyeti-1.4.1.2/pyyeti/locate.py
+drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-05-11 18:16:52.579718 pyyeti-1.4.1.2/pyyeti/nastran/
+-rw-rw-r--   0 macro     (1000) macro     (1000)      138 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/nastran/__init__.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)   189330 2024-03-30 16:12:46.000000 pyyeti-1.4.1.2/pyyeti/nastran/bulk.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)   136739 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/nastran/n2p.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)   178090 2024-05-11 18:08:19.000000 pyyeti-1.4.1.2/pyyeti/nastran/op2.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    91364 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/nastran/op4.py
+drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-05-11 18:16:52.583718 pyyeti-1.4.1.2/pyyeti/ode/
+-rw-rw-r--   0 macro     (1000) macro     (1000)      869 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/ode/__init__.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    18978 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/ode/_base_ode_class.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    39142 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/ode/_utilities.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)     9992 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/ode/freqdirect.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    17472 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/ode/frf_mode_participation.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    10065 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/ode/solvecdf.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)     5653 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/ode/solveexp1.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    28080 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/ode/solveexp2.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    27510 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/ode/solvenewmark.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    71837 2024-02-25 16:48:06.000000 pyyeti-1.4.1.2/pyyeti/ode/solveunc.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)     9390 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/pp.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    43921 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/psd.py
+drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-05-11 18:16:52.583718 pyyeti-1.4.1.2/pyyeti/rainflow/
+-rw-rw-r--   0 macro     (1000) macro     (1000)      195 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/rainflow/__init__.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    13898 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/rainflow/c_rain.c
+-rw-rw-r--   0 macro     (1000) macro     (1000)     6540 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/rainflow/py_rain.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    75180 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/srs.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    11892 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/ssmodel.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    14070 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/stats.py
+drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-05-11 18:16:52.575718 pyyeti-1.4.1.2/pyyeti/tests/
+drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-05-11 18:16:52.583718 pyyeti-1.4.1.2/pyyeti/tests/nas2cam_csuper/
+-rw-rw-r--   0 macro     (1000) macro     (1000)     1622 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/tests/nas2cam_csuper/inboard.asm
+-rw-rw-r--   0 macro     (1000) macro     (1000)    25840 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/tests/nas2cam_csuper/inboard.op4
+-rw-rw-r--   0 macro     (1000) macro     (1000)     4727 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/tests/nas2cam_csuper/inboard.pch
+-rw-rw-r--   0 macro     (1000) macro     (1000)    15736 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/tests/nas2cam_csuper/nas2cam.op2
+-rw-rw-r--   0 macro     (1000) macro     (1000)   147552 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/tests/nas2cam_csuper/nas2cam.op4
+drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-05-11 18:16:52.587719 pyyeti-1.4.1.2/pyyeti/tests/nas2cam_extseout/
+-rw-rw-r--   0 macro     (1000) macro     (1000)     2432 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/tests/nas2cam_extseout/assemble.dat
+-rw-rw-r--   0 macro     (1000) macro     (1000)   133180 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/tests/nas2cam_extseout/assemble.op2
+-rw-rw-r--   0 macro     (1000) macro     (1000)   162313 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/tests/nas2cam_extseout/assemble.out
+-rw-rw-r--   0 macro     (1000) macro     (1000)     1622 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/tests/nas2cam_extseout/inboard.asm
+-rw-rw-r--   0 macro     (1000) macro     (1000)     5827 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/tests/nas2cam_extseout/inboard.blk
+-rw-rw-r--   0 macro     (1000) macro     (1000)     6894 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/tests/nas2cam_extseout/inboard.dat
+-rw-rw-r--   0 macro     (1000) macro     (1000)    24052 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/tests/nas2cam_extseout/inboard.op2
+-rw-rw-r--   0 macro     (1000) macro     (1000)    36504 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/tests/nas2cam_extseout/inboard.op4
+-rw-rw-r--   0 macro     (1000) macro     (1000)   134889 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/tests/nas2cam_extseout/inboard.out
+-rw-rw-r--   0 macro     (1000) macro     (1000)     8939 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/tests/nas2cam_extseout/inboard.pch
+-rw-rw-r--   0 macro     (1000) macro     (1000)     2012 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/tests/nas2cam_extseout/outboard.asm
+-rw-rw-r--   0 macro     (1000) macro     (1000)     4946 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/tests/nas2cam_extseout/outboard.blk
+-rw-rw-r--   0 macro     (1000) macro     (1000)      767 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/tests/nas2cam_extseout/outboard.dat
+-rw-rw-r--   0 macro     (1000) macro     (1000)    38384 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/tests/nas2cam_extseout/outboard.op4
+-rw-rw-r--   0 macro     (1000) macro     (1000)    74780 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/tests/nas2cam_extseout/outboard.out
+-rw-rw-r--   0 macro     (1000) macro     (1000)     5944 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/tests/nas2cam_extseout/outboard.pch
+drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-05-11 18:16:52.587719 pyyeti-1.4.1.2/pyyeti/tests/nastran_drm12/
+-rw-rw-r--   0 macro     (1000) macro     (1000)    13464 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/tests/nastran_drm12/drm12.op2
+-rw-rw-r--   0 macro     (1000) macro     (1000)    77852 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/tests/nastran_drm12/drm12.op4
+-rw-rw-r--   0 macro     (1000) macro     (1000)    17160 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/tests/nastran_drm12/inboard_nas2cam.op2
+-rw-rw-r--   0 macro     (1000) macro     (1000)    51624 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/tests/nastran_drm12/inboard_nas2cam.op4
+-rw-rw-r--   0 macro     (1000) macro     (1000)    12371 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/writer.py
+-rw-rw-r--   0 macro     (1000) macro     (1000)    61169 2024-01-24 22:45:59.000000 pyyeti-1.4.1.2/pyyeti/ytools.py
+drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-05-11 18:16:52.579718 pyyeti-1.4.1.2/pyyeti.egg-info/
+-rw-r--r--   0 macro     (1000) macro     (1000)     4071 2024-05-11 18:16:52.000000 pyyeti-1.4.1.2/pyyeti.egg-info/PKG-INFO
+-rw-rw-r--   0 macro     (1000) macro     (1000)     2311 2024-05-11 18:16:52.000000 pyyeti-1.4.1.2/pyyeti.egg-info/SOURCES.txt
+-rw-rw-r--   0 macro     (1000) macro     (1000)        1 2024-05-11 18:16:52.000000 pyyeti-1.4.1.2/pyyeti.egg-info/dependency_links.txt
+-rw-rw-r--   0 macro     (1000) macro     (1000)        7 2024-05-11 18:16:52.000000 pyyeti-1.4.1.2/pyyeti.egg-info/top_level.txt
+drwxrwxr-x   0 macro     (1000) macro     (1000)        0 2024-05-11 18:16:52.587719 pyyeti-1.4.1.2/scripts/
+-rwxrwxr-x   0 macro     (1000) macro     (1000)      861 2024-02-25 16:48:06.000000 pyyeti-1.4.1.2/scripts/lsop2
+-rwxrwxr-x   0 macro     (1000) macro     (1000)      561 2024-02-25 16:48:06.000000 pyyeti-1.4.1.2/scripts/lsop4
+-rw-rw-r--   0 macro     (1000) macro     (1000)      198 2024-05-11 18:16:52.587719 pyyeti-1.4.1.2/setup.cfg
+-rw-rw-r--   0 macro     (1000) macro     (1000)     5161 2024-05-11 18:08:19.000000 pyyeti-1.4.1.2/setup.py
```

### Comparing `pyyeti-1.4.1.1/LICENSE.txt` & `pyyeti-1.4.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/PKG-INFO` & `pyyeti-1.4.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyyeti
-Version: 1.4.1.1
+Version: 1.4.1.2
 Summary: Tools mostly related to structural dynamics
 Home-page: http://github.com/twmacro/pyyeti/
 Author: Tim Widrick
 Author-email: twmacro@gmail.com
 License: BSD
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyyeti Version: 1.4.1.1 Summary: Tools mostly
+Metadata-Version: 2.1 Name: pyyeti Version: 1.4.1.2 Summary: Tools mostly
 related to structural dynamics Home-page: http://github.com/twmacro/pyyeti/
 Author: Tim Widrick Author-email: twmacro@gmail.com License: BSD Platform: any
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 C Classifier: Programming Language :: Python Classifier: Programming Language
 :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
 Language :: Python :: Implementation :: CPython Classifier: Natural Language ::
```

### Comparing `pyyeti-1.4.1.1/README.md` & `pyyeti-1.4.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/__init__.py` & `pyyeti-1.4.1.2/pyyeti/__init__.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/cb.py` & `pyyeti-1.4.1.2/pyyeti/cb.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/cla/_magpct.py` & `pyyeti-1.4.1.2/pyyeti/cla/_magpct.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/cla/_rptext1.py` & `pyyeti-1.4.1.2/pyyeti/cla/_rptext1.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/cla/_rptpct1.py` & `pyyeti-1.4.1.2/pyyeti/cla/_rptpct1.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/cla/_rpttab1.py` & `pyyeti-1.4.1.2/pyyeti/cla/_rpttab1.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/cla/_utilities.py` & `pyyeti-1.4.1.2/pyyeti/cla/_utilities.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/cla/dr_def.py` & `pyyeti-1.4.1.2/pyyeti/cla/dr_def.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/cla/dr_event.py` & `pyyeti-1.4.1.2/pyyeti/cla/dr_event.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/cla/dr_results.py` & `pyyeti-1.4.1.2/pyyeti/cla/dr_results.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/cla/dr_results_plots.py` & `pyyeti-1.4.1.2/pyyeti/cla/dr_results_plots.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/cla/rel_disp_dtm.py` & `pyyeti-1.4.1.2/pyyeti/cla/rel_disp_dtm.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/column_plotter.py` & `pyyeti-1.4.1.2/pyyeti/column_plotter.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/cyclecount.py` & `pyyeti-1.4.1.2/pyyeti/cyclecount.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/datacursor.py` & `pyyeti-1.4.1.2/pyyeti/datacursor.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/dsp.py` & `pyyeti-1.4.1.2/pyyeti/dsp.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/era.py` & `pyyeti-1.4.1.2/pyyeti/era.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/expmint.py` & `pyyeti-1.4.1.2/pyyeti/expmint.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/fdepsd.py` & `pyyeti-1.4.1.2/pyyeti/fdepsd.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/frclim.py` & `pyyeti-1.4.1.2/pyyeti/frclim.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/guitools.py` & `pyyeti-1.4.1.2/pyyeti/guitools.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/locate.py` & `pyyeti-1.4.1.2/pyyeti/locate.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/nastran/bulk.py` & `pyyeti-1.4.1.2/pyyeti/nastran/bulk.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/nastran/n2p.py` & `pyyeti-1.4.1.2/pyyeti/nastran/n2p.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/nastran/op2.py` & `pyyeti-1.4.1.2/pyyeti/nastran/op2.py`

 * *Files 2% similar despite different names*

```diff
@@ -2301,20 +2301,28 @@
         return None, None
 
     def _rd_dr_table(self, name, pos, verbose):
         self.set_position(pos)
         self.rdop2nt()
         self.rdop2record()
         rec2 = self.rdop2record("bytes")
-        if rec2[:40] == b"TYPE  IDCOMP ROW    TYPE  IDCOMP ROW    ":
+        if (rec2[:40] == b"TYPE  IDCOMP ROW    TYPE  IDCOMP ROW    ") or (
+            rec2[:40] == b"TYPE      ID    COMP     ROW            "
+        ):
             if verbose:
                 print(f"Reading table {name} at position {pos}...")
-            type_id_ndof = np.frombuffer(rec2[40:], self._endian + "i4").reshape(-1, 5)[
-                :, :3
-            ]
+            if rec2[:8] == b"TYPE  ID":
+                offset = 40
+                iform = "i4"
+            else:
+                offset = 80
+                iform = "i8"
+            type_id_ndof = np.frombuffer(rec2[offset:], self._endian + iform).reshape(
+                -1, 5
+            )[:, :3]
             mat = np.array(
                 [
                     [i, dof, etype]
                     for etype, i, ndof in type_id_ndof
                     for dof in range(1, ndof + 1)
                 ]
             )
```

### Comparing `pyyeti-1.4.1.1/pyyeti/nastran/op4.py` & `pyyeti-1.4.1.2/pyyeti/nastran/op4.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/ode/__init__.py` & `pyyeti-1.4.1.2/pyyeti/ode/__init__.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/ode/_base_ode_class.py` & `pyyeti-1.4.1.2/pyyeti/ode/_base_ode_class.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/ode/_utilities.py` & `pyyeti-1.4.1.2/pyyeti/ode/_utilities.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/ode/freqdirect.py` & `pyyeti-1.4.1.2/pyyeti/ode/freqdirect.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/ode/frf_mode_participation.py` & `pyyeti-1.4.1.2/pyyeti/ode/frf_mode_participation.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/ode/solvecdf.py` & `pyyeti-1.4.1.2/pyyeti/ode/solvecdf.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/ode/solveexp1.py` & `pyyeti-1.4.1.2/pyyeti/ode/solveexp1.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/ode/solveexp2.py` & `pyyeti-1.4.1.2/pyyeti/ode/solveexp2.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/ode/solvenewmark.py` & `pyyeti-1.4.1.2/pyyeti/ode/solvenewmark.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/ode/solveunc.py` & `pyyeti-1.4.1.2/pyyeti/ode/solveunc.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/pp.py` & `pyyeti-1.4.1.2/pyyeti/pp.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/psd.py` & `pyyeti-1.4.1.2/pyyeti/psd.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/rainflow/c_rain.c` & `pyyeti-1.4.1.2/pyyeti/rainflow/c_rain.c`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/rainflow/py_rain.py` & `pyyeti-1.4.1.2/pyyeti/rainflow/py_rain.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/srs.py` & `pyyeti-1.4.1.2/pyyeti/srs.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/ssmodel.py` & `pyyeti-1.4.1.2/pyyeti/ssmodel.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/stats.py` & `pyyeti-1.4.1.2/pyyeti/stats.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_csuper/inboard.asm` & `pyyeti-1.4.1.2/pyyeti/tests/nas2cam_csuper/inboard.asm`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_csuper/inboard.op4` & `pyyeti-1.4.1.2/pyyeti/tests/nas2cam_csuper/inboard.op4`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_csuper/inboard.pch` & `pyyeti-1.4.1.2/pyyeti/tests/nas2cam_csuper/inboard.pch`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_csuper/nas2cam.op2` & `pyyeti-1.4.1.2/pyyeti/tests/nas2cam_csuper/nas2cam.op2`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_csuper/nas2cam.op4` & `pyyeti-1.4.1.2/pyyeti/tests/nas2cam_csuper/nas2cam.op4`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/assemble.dat` & `pyyeti-1.4.1.2/pyyeti/tests/nas2cam_extseout/assemble.dat`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/assemble.op2` & `pyyeti-1.4.1.2/pyyeti/tests/nas2cam_extseout/assemble.op2`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/assemble.out` & `pyyeti-1.4.1.2/pyyeti/tests/nas2cam_extseout/assemble.out`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/inboard.asm` & `pyyeti-1.4.1.2/pyyeti/tests/nas2cam_extseout/inboard.asm`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/inboard.blk` & `pyyeti-1.4.1.2/pyyeti/tests/nas2cam_extseout/inboard.blk`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/inboard.dat` & `pyyeti-1.4.1.2/pyyeti/tests/nas2cam_extseout/inboard.dat`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/inboard.op2` & `pyyeti-1.4.1.2/pyyeti/tests/nas2cam_extseout/inboard.op2`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/inboard.op4` & `pyyeti-1.4.1.2/pyyeti/tests/nas2cam_extseout/inboard.op4`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/inboard.out` & `pyyeti-1.4.1.2/pyyeti/tests/nas2cam_extseout/inboard.out`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/inboard.pch` & `pyyeti-1.4.1.2/pyyeti/tests/nas2cam_extseout/inboard.pch`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/outboard.asm` & `pyyeti-1.4.1.2/pyyeti/tests/nas2cam_extseout/outboard.asm`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/outboard.blk` & `pyyeti-1.4.1.2/pyyeti/tests/nas2cam_extseout/outboard.blk`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/outboard.dat` & `pyyeti-1.4.1.2/pyyeti/tests/nas2cam_extseout/outboard.dat`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/outboard.op4` & `pyyeti-1.4.1.2/pyyeti/tests/nas2cam_extseout/outboard.op4`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/outboard.out` & `pyyeti-1.4.1.2/pyyeti/tests/nas2cam_extseout/outboard.out`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/tests/nas2cam_extseout/outboard.pch` & `pyyeti-1.4.1.2/pyyeti/tests/nas2cam_extseout/outboard.pch`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/tests/nastran_drm12/drm12.op2` & `pyyeti-1.4.1.2/pyyeti/tests/nastran_drm12/drm12.op2`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/tests/nastran_drm12/drm12.op4` & `pyyeti-1.4.1.2/pyyeti/tests/nastran_drm12/drm12.op4`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/tests/nastran_drm12/inboard_nas2cam.op2` & `pyyeti-1.4.1.2/pyyeti/tests/nastran_drm12/inboard_nas2cam.op2`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/tests/nastran_drm12/inboard_nas2cam.op4` & `pyyeti-1.4.1.2/pyyeti/tests/nastran_drm12/inboard_nas2cam.op4`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/writer.py` & `pyyeti-1.4.1.2/pyyeti/writer.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti/ytools.py` & `pyyeti-1.4.1.2/pyyeti/ytools.py`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/pyyeti.egg-info/PKG-INFO` & `pyyeti-1.4.1.2/pyyeti.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyyeti
-Version: 1.4.1.1
+Version: 1.4.1.2
 Summary: Tools mostly related to structural dynamics
 Home-page: http://github.com/twmacro/pyyeti/
 Author: Tim Widrick
 Author-email: twmacro@gmail.com
 License: BSD
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyyeti Version: 1.4.1.1 Summary: Tools mostly
+Metadata-Version: 2.1 Name: pyyeti Version: 1.4.1.2 Summary: Tools mostly
 related to structural dynamics Home-page: http://github.com/twmacro/pyyeti/
 Author: Tim Widrick Author-email: twmacro@gmail.com License: BSD Platform: any
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 C Classifier: Programming Language :: Python Classifier: Programming Language
 :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
 Language :: Python :: Implementation :: CPython Classifier: Natural Language ::
```

### Comparing `pyyeti-1.4.1.1/pyyeti.egg-info/SOURCES.txt` & `pyyeti-1.4.1.2/pyyeti.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/scripts/lsop2` & `pyyeti-1.4.1.2/scripts/lsop2`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/scripts/lsop4` & `pyyeti-1.4.1.2/scripts/lsop4`

 * *Files identical despite different names*

### Comparing `pyyeti-1.4.1.1/setup.py` & `pyyeti-1.4.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         )
     else:
         kw = {}
 
     install_requires = check_dependencies()
     setup(
         name="pyyeti",
-        version="1.4.1.1",
+        version="1.4.1.2",
         url="http://github.com/twmacro/pyyeti/",
         license="BSD",
         author="Tim Widrick",
         install_requires=install_requires,
         author_email="twmacro@gmail.com",
         description=("Tools mostly related to structural dynamics"),
         long_description=long_description,
```

