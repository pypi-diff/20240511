# Comparing `tmp/petram_rf-1.5.5.tar.gz` & `tmp/petram_rf-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petram_rf-1.5.5.tar", last modified: Thu Apr 25 14:22:40 2024, max compression
+gzip compressed data, was "petram_rf-1.5.7.tar", last modified: Sat May 11 04:56:29 2024, max compression
```

## Comparing `petram_rf-1.5.5.tar` & `petram_rf-1.5.7.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:40.069489 petram_rf-1.5.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-25 14:22:32.000000 petram_rf-1.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-04-25 14:22:40.069489 petram_rf-1.5.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:40.069489 petram_rf-1.5.5/PetraM_RF.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-04-25 14:22:40.000000 petram_rf-1.5.5/PetraM_RF.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-25 14:22:40.000000 petram_rf-1.5.5/PetraM_RF.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 14:22:40.000000 petram_rf-1.5.5/PetraM_RF.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 14:22:40.000000 petram_rf-1.5.5/PetraM_RF.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-25 14:22:32.000000 petram_rf-1.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:40.057489 petram_rf-1.5.5/petram/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:40.057489 petram_rf-1.5.5/petram/phys/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:40.057489 petram_rf-1.5.5/petram/phys/common/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/common/numba_zfunc.py
--rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/common/rf_dispersion_coldplasma.py
--rw-r--r--   0 runner    (1001) docker     (127)     6641 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/common/rf_dispersion_coldplasma_numba.py
--rw-r--r--   0 runner    (1001) docker     (127)     7449 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/common/rf_port_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/common/rf_stix_terms_panel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:40.061489 petram_rf-1.5.5/petram/phys/em1d/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em1d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10565 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em1d/em1d_anisotropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em1d/em1d_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10011 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em1d/em1d_coldplasma.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em1d/em1d_const.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em1d/em1d_cont.py
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em1d/em1d_e.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em1d/em1d_extj.py
--rw-r--r--   0 runner    (1001) docker     (127)    10996 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em1d/em1d_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em1d/em1d_pec.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em1d/em1d_pmc.py
--rw-r--r--   0 runner    (1001) docker     (127)    12219 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em1d/em1d_port.py
--rw-r--r--   0 runner    (1001) docker     (127)    10220 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em1d/em1d_vac.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em1d/eval_deriv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:40.061489 petram_rf-1.5.5/petram/phys/em2d/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em2d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em2d/em2d_anisotropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em2d/em2d_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8826 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em2d/em2d_coldplasma.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em2d/em2d_cont.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em2d/em2d_e.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em2d/em2d_extj.py
--rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em2d/em2d_floquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em2d/em2d_h.py
--rw-r--r--   0 runner    (1001) docker     (127)    11849 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em2d/em2d_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em2d/em2d_pec.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em2d/em2d_pmc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em2d/em2d_pml.py
--rw-r--r--   0 runner    (1001) docker     (127)    11214 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em2d/em2d_vac.py
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em2d/em2d_z.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:40.065489 petram_rf-1.5.5/petram/phys/em2da/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em2da/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14600 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em2da/em2da_anisotropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em2da/em2da_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11695 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em2da/em2da_coldplasma.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em2da/em2da_const.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em2da/em2da_cont.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em2da/em2da_e.py
--rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em2da/em2da_extj.py
--rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em2da/em2da_floquet.py
--rw-r--r--   0 runner    (1001) docker     (127)    12651 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em2da/em2da_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em2da/em2da_pec.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em2da/em2da_pmc.py
--rw-r--r--   0 runner    (1001) docker     (127)    17666 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em2da/em2da_port.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em2da/em2da_surfj.py
--rw-r--r--   0 runner    (1001) docker     (127)    12715 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em2da/em2da_vac.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em2da/eval_deriv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:40.069489 petram_rf-1.5.5/petram/phys/em3d/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em3d/em3d_anisotropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em3d/em3d_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8291 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em3d/em3d_coldplasma.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em3d/em3d_const.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em3d/em3d_cont.py
--rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em3d/em3d_div.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em3d/em3d_e.py
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em3d/em3d_extj.py
--rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em3d/em3d_floquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em3d/em3d_h.py
--rw-r--r--   0 runner    (1001) docker     (127)    15240 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em3d/em3d_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em3d/em3d_pec.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em3d/em3d_pmc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9731 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em3d/em3d_pml.py
--rw-r--r--   0 runner    (1001) docker     (127)    16697 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em3d/em3d_port.py
--rw-r--r--   0 runner    (1001) docker     (127)    20220 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em3d/em3d_portarray.py
--rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em3d/em3d_portload.py
--rw-r--r--   0 runner    (1001) docker     (127)     7590 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em3d/em3d_portmode.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em3d/em3d_surfj.py
--rw-r--r--   0 runner    (1001) docker     (127)     5471 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em3d/em3d_vac.py
--rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em3d/em3d_z.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em3d/eval_deriv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:40.069489 petram_rf-1.5.5/petram/phys/em3d/helper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em3d/helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15533 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em3d/helper/export_nodalvalues.py
--rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-04-25 14:22:32.000000 petram_rf-1.5.5/petram/phys/em3d/helper/write_cdf.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 14:22:40.069489 petram_rf-1.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-25 14:22:32.000000 petram_rf-1.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:56:29.064386 petram_rf-1.5.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-11 04:56:19.000000 petram_rf-1.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-11 04:56:29.064386 petram_rf-1.5.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:56:29.064386 petram_rf-1.5.7/PetraM_RF.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-11 04:56:29.000000 petram_rf-1.5.7/PetraM_RF.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-11 04:56:29.000000 petram_rf-1.5.7/PetraM_RF.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 04:56:29.000000 petram_rf-1.5.7/PetraM_RF.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-11 04:56:29.000000 petram_rf-1.5.7/PetraM_RF.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-05-11 04:56:19.000000 petram_rf-1.5.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:56:29.052386 petram_rf-1.5.7/petram/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:56:29.052386 petram_rf-1.5.7/petram/phys/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:56:29.052386 petram_rf-1.5.7/petram/phys/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/common/numba_zfunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/common/rf_dispersion_coldplasma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6409 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/common/rf_dispersion_coldplasma_numba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7449 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/common/rf_port_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/common/rf_stix_terms_panel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:56:29.052386 petram_rf-1.5.7/petram/phys/em1d/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em1d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10565 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em1d/em1d_anisotropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em1d/em1d_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10045 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em1d/em1d_coldplasma.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em1d/em1d_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em1d/em1d_cont.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em1d/em1d_e.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em1d/em1d_extj.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10996 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em1d/em1d_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em1d/em1d_pec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em1d/em1d_pmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12219 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em1d/em1d_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10220 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em1d/em1d_vac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em1d/eval_deriv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:56:29.056386 petram_rf-1.5.7/petram/phys/em2d/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em2d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em2d/em2d_anisotropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em2d/em2d_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8860 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em2d/em2d_coldplasma.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em2d/em2d_cont.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em2d/em2d_e.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em2d/em2d_extj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em2d/em2d_floquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em2d/em2d_h.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11849 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em2d/em2d_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em2d/em2d_pec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em2d/em2d_pmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em2d/em2d_pml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11214 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em2d/em2d_vac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em2d/em2d_z.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:56:29.060386 petram_rf-1.5.7/petram/phys/em2da/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em2da/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14600 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em2da/em2da_anisotropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em2da/em2da_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11729 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em2da/em2da_coldplasma.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em2da/em2da_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em2da/em2da_cont.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em2da/em2da_e.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em2da/em2da_extj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em2da/em2da_floquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12651 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em2da/em2da_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em2da/em2da_pec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em2da/em2da_pmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17666 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em2da/em2da_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em2da/em2da_surfj.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12715 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em2da/em2da_vac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em2da/eval_deriv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:56:29.064386 petram_rf-1.5.7/petram/phys/em3d/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em3d/em3d_anisotropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em3d/em3d_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8326 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em3d/em3d_coldplasma.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em3d/em3d_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em3d/em3d_cont.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em3d/em3d_div.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em3d/em3d_e.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em3d/em3d_extj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em3d/em3d_floquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em3d/em3d_h.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15240 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em3d/em3d_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em3d/em3d_pec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em3d/em3d_pmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9731 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em3d/em3d_pml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16697 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em3d/em3d_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20220 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em3d/em3d_portarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em3d/em3d_portload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7590 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em3d/em3d_portmode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em3d/em3d_surfj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5471 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em3d/em3d_vac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em3d/em3d_z.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em3d/eval_deriv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:56:29.064386 petram_rf-1.5.7/petram/phys/em3d/helper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em3d/helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15533 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em3d/helper/export_nodalvalues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-05-11 04:56:19.000000 petram_rf-1.5.7/petram/phys/em3d/helper/write_cdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 04:56:29.064386 petram_rf-1.5.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-11 04:56:19.000000 petram_rf-1.5.7/setup.py
```

### Comparing `petram_rf-1.5.5/LICENSE` & `petram_rf-1.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/PKG-INFO` & `petram_rf-1.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PetraM_RF
-Version: 1.5.5
+Version: 1.5.7
 Summary: PetraM RF package
 Home-page: https://github.com/piScope/PetraM
 Author: S. Shiraiwa
 Author-email: shiraiwa@princeton.edu
 License: GNUv3
 Keywords: MFEM physics
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `petram_rf-1.5.5/PetraM_RF.egg-info/PKG-INFO` & `petram_rf-1.5.7/PetraM_RF.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PetraM_RF
-Version: 1.5.5
+Version: 1.5.7
 Summary: PetraM RF package
 Home-page: https://github.com/piScope/PetraM
 Author: S. Shiraiwa
 Author-email: shiraiwa@princeton.edu
 License: GNUv3
 Keywords: MFEM physics
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `petram_rf-1.5.5/PetraM_RF.egg-info/SOURCES.txt` & `petram_rf-1.5.7/PetraM_RF.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/README.md` & `petram_rf-1.5.7/README.md`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/common/numba_zfunc.py` & `petram_rf-1.5.7/petram/phys/common/numba_zfunc.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/common/rf_dispersion_coldplasma.py` & `petram_rf-1.5.7/petram/phys/common/rf_dispersion_coldplasma.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     import mfem.par as mfem
     from mpi4py import MPI
     myid = MPI.COMM_WORLD.rank
 else:
     import mfem.ser as mfem
     myid = 0
 
-vtable_data = [('B', VtableElement('bext', type='array',
+vtable_data0= [('B', VtableElement('bext', type='array',
                                    guilabel='magnetic field',
                                    default="=[0,0,0]",
                                    tip="external magnetic field")),
                ('dens_e', VtableElement('dens_e', type='float',
                                         guilabel='electron density(m-3)',
                                         default="1e19",
                                         tip="electron density")),
```

### Comparing `petram_rf-1.5.5/petram/phys/common/rf_dispersion_coldplasma_numba.py` & `petram_rf-1.5.7/petram/phys/common/rf_dispersion_coldplasma_numba.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from numba import njit, void, int32, int64, float64, complex128, types
 from numpy import (pi, sin, cos, exp, sqrt, log, arctan2,
                    max, array, linspace, conj, transpose,
-                   sum, zeros, dot, array)
+                   sum, zeros, dot, array, ascontiguousarray)
 import numpy as np
 
 # vacuum permittivity
 e0 = 8.8541878176e-12
 q_base = 1.60217662e-19
 qe = -q_base
 me = 9.10938356e-31
@@ -152,20 +152,22 @@
             M += M2
 
         kion = kion + 1
 
     return M
 
 
-@njit(complex128[:, :](float64, float64[:], float64[:], darray_ro, iarray_ro, float64, float64))
-def epsilonr_pl_cold(w, B, denses, masses, charges, Te, ne):
-    '''
-    standard SPD stix
-    '''
-    M = epsilonr_pl_cold_std(w, B, denses, masses, charges, Te, ne)
+@njit(complex128[:, :](float64[:], complex128[:, :]))
+def rotate_dielectric(B, M):
+    #
+    #  B : magnetic field.
+    #  M : dielectric matrix.
+    #
+    B = ascontiguousarray(B)
+    M = ascontiguousarray(M)
 
     def R1(ph):
         return array([[cos(ph), 0.,  sin(ph)],
                       [0,       1.,   0],
                       [-sin(ph), 0,  cos(ph)]], dtype=complex128)
 
     def R2(th):
@@ -181,38 +183,30 @@
     #  By = sin(phi) sin(th)
     #  Bz = cos(phi)
 
     # B = [Bx, By, Bz]
     th = arctan2(B[1], B[0])
     ph = arctan2(B[0]*cos(th)+B[1]*sin(th), B[2])
     A = dot(R1(ph), dot(M, R1(-ph)))
-
     ans = dot(R2(th), dot(A, R2(-th)))
-    # print_mat(ans, 3, 3)
+
     return ans
 
 
+@njit(complex128[:, :](float64, float64[:], float64[:], darray_ro, iarray_ro, float64, float64))
+def epsilonr_pl_cold(w, B, denses, masses, charges, Te, ne):
+    '''
+    standard SPD stix
+    '''
+    M = epsilonr_pl_cold_std(w, B, denses, masses, charges, Te, ne)
+    return rotate_dielectric(B, M)
+
+
 @njit(complex128[:, :](float64, float64[:], float64[:], darray_ro, iarray_ro, float64, float64, iarray_ro))
 def epsilonr_pl_cold_generic(w, B, denses, masses, charges, Te, ne, terms):
     '''
     standard SPD stix
     '''
     M = epsilonr_pl_cold_g(w, B, denses, masses,
                            charges, Te, ne, terms)
 
-    def R1(ph):
-        return array([[cos(ph), 0.,  sin(ph)],
-                      [0,       1.,   0],
-                      [-sin(ph), 0,  cos(ph)]], dtype=complex128)
-
-    def R2(th):
-        return array([[cos(th), -sin(th), 0],
-                      [sin(th), cos(th), 0],
-                      [0, 0,  1.]], dtype=complex128)
-
-    th = arctan2(B[1], B[0])
-    ph = arctan2(B[0]*cos(th)+B[1]*sin(th), B[2])
-    A = dot(R1(ph), dot(M, R1(-ph)))
-
-    ans = dot(R2(th), dot(A, R2(-th)))
-
-    return ans
+    return rotate_dielectric(B, M)
```

### Comparing `petram_rf-1.5.5/petram/phys/common/rf_port_scanner.py` & `petram_rf-1.5.7/petram/phys/common/rf_port_scanner.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/common/rf_stix_terms_panel.py` & `petram_rf-1.5.7/petram/phys/common/rf_stix_terms_panel.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em1d/em1d_anisotropic.py` & `petram_rf-1.5.7/petram/phys/em1d/em1d_anisotropic.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em1d/em1d_base.py` & `petram_rf-1.5.7/petram/phys/em1d/em1d_base.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em1d/em1d_coldplasma.py` & `petram_rf-1.5.7/petram/phys/em1d/em1d_coldplasma.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
    cold plasma.
 '''
 from petram.phys.common.rf_dispersion_coldplasma import (stix_options,
                                                          default_stix_option,
-                                                         vtable_data)
+                                                         vtable_data0)
 import numpy as np
 
 from petram.mfem_config import use_parallel, get_numba_debug
 
 from petram.phys.vtable import VtableElement, Vtable
 from petram.phys.phys_const import mu0, epsilon0
 from petram.phys.numba_coefficient import NumbaCoefficient
@@ -23,15 +23,15 @@
     import mfem.par as mfem
     from mpi4py import MPI
     myid = MPI.COMM_WORLD.rank
 else:
     import mfem.ser as mfem
     myid = 0
 
-
+vtable_data = vtable_data0.copy()
 vtable_data.extend(
     [('ky', VtableElement('ky', type='float',
                           guilabel='ky',
                           default=0.,
                           no_func=True,
                           tip="wave number in the y direction")),
      ('kz', VtableElement('kz', type='float',
```

### Comparing `petram_rf-1.5.5/petram/phys/em1d/em1d_e.py` & `petram_rf-1.5.7/petram/phys/em1d/em1d_e.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em1d/em1d_extj.py` & `petram_rf-1.5.7/petram/phys/em1d/em1d_extj.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em1d/em1d_model.py` & `petram_rf-1.5.7/petram/phys/em1d/em1d_model.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em1d/em1d_pec.py` & `petram_rf-1.5.7/petram/phys/em1d/em1d_pec.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em1d/em1d_pmc.py` & `petram_rf-1.5.7/petram/phys/em1d/em1d_pmc.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em1d/em1d_port.py` & `petram_rf-1.5.7/petram/phys/em1d/em1d_port.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em1d/em1d_vac.py` & `petram_rf-1.5.7/petram/phys/em1d/em1d_vac.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em1d/eval_deriv.py` & `petram_rf-1.5.7/petram/phys/em1d/eval_deriv.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em2d/em2d_anisotropic.py` & `petram_rf-1.5.7/petram/phys/em2d/em2d_anisotropic.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em2d/em2d_base.py` & `petram_rf-1.5.7/petram/phys/em2d/em2d_base.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em2d/em2d_coldplasma.py` & `petram_rf-1.5.7/petram/phys/em2d/em2d_coldplasma.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
   Exy = Ex e_x + Ey e_y
   Ez =  Ez e_z
 
 '''
 from petram.phys.common.rf_dispersion_coldplasma import (stix_options,
                                                          default_stix_option,
-                                                         vtable_data,)
+                                                         vtable_data0,)
 
 from petram.phys.em2d.em2d_base import EM2D_Bdry, EM2D_Domain, EM2D_Domain_helper
 from petram.phys.phys_const import mu0, epsilon0
 from petram.phys.vtable import VtableElement, Vtable
 from petram.mfem_config import use_parallel
 import numpy as np
 
@@ -29,15 +29,15 @@
 dprint1, dprint2, dprint3 = debug.init_dprints('EM2D_ColdPlasma')
 
 if use_parallel:
     import mfem.par as mfem
 else:
     import mfem.ser as mfem
 
-
+vtable_data = vtable_data0.copy()
 vtable_data.extend([('kz', VtableElement('kz', type='float',
                                          guilabel='kz',
                                          default=0.0,
                                          no_func=True,
                                          tip="out-of-plane wave number")), ])
```

### Comparing `petram_rf-1.5.5/petram/phys/em2d/em2d_e.py` & `petram_rf-1.5.7/petram/phys/em2d/em2d_e.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em2d/em2d_extj.py` & `petram_rf-1.5.7/petram/phys/em2d/em2d_extj.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em2d/em2d_floquet.py` & `petram_rf-1.5.7/petram/phys/em2d/em2d_floquet.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em2d/em2d_h.py` & `petram_rf-1.5.7/petram/phys/em2d/em2d_h.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em2d/em2d_model.py` & `petram_rf-1.5.7/petram/phys/em2d/em2d_model.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em2d/em2d_pec.py` & `petram_rf-1.5.7/petram/phys/em2d/em2d_pec.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em2d/em2d_pmc.py` & `petram_rf-1.5.7/petram/phys/em2d/em2d_pmc.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em2d/em2d_pml.py` & `petram_rf-1.5.7/petram/phys/em2d/em2d_pml.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em2d/em2d_vac.py` & `petram_rf-1.5.7/petram/phys/em2d/em2d_vac.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em2d/em2d_z.py` & `petram_rf-1.5.7/petram/phys/em2d/em2d_z.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em2da/em2da_anisotropic.py` & `petram_rf-1.5.7/petram/phys/em2da/em2da_anisotropic.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em2da/em2da_base.py` & `petram_rf-1.5.7/petram/phys/em2da/em2da_base.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em2da/em2da_coldplasma.py` & `petram_rf-1.5.7/petram/phys/em2da/em2da_coldplasma.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
    Cold plasma:
 '''
 from petram.phys.common.rf_dispersion_coldplasma import (stix_options,
                                                          default_stix_option,
-                                                         vtable_data)
+                                                         vtable_data0)
 
 from petram.phys.phys_const import mu0, epsilon0
 from petram.phys.numba_coefficient import (func_to_numba_coeff_scalar,
                                            func_to_numba_coeff_vector,
                                            func_to_numba_coeff_matrix)
 from petram.phys.vtable import VtableElement, Vtable
 from petram.mfem_config import use_parallel
@@ -21,15 +21,15 @@
 dprint1, dprint2, dprint3 = debug.init_dprints('EM2Da_ColdPlasma')
 
 if use_parallel:
     import mfem.par as mfem
 else:
     import mfem.ser as mfem
 
-
+vtable_data = vtable_data0.copy()
 vtable_data.extend([
     ('t_mode', VtableElement('t_mode', type="float",
                              guilabel='m',
                              default=0.0,
                              tip="mode number")), ])
```

### Comparing `petram_rf-1.5.5/petram/phys/em2da/em2da_e.py` & `petram_rf-1.5.7/petram/phys/em2da/em2da_e.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em2da/em2da_extj.py` & `petram_rf-1.5.7/petram/phys/em2da/em2da_extj.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em2da/em2da_floquet.py` & `petram_rf-1.5.7/petram/phys/em2da/em2da_floquet.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em2da/em2da_model.py` & `petram_rf-1.5.7/petram/phys/em2da/em2da_model.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em2da/em2da_pec.py` & `petram_rf-1.5.7/petram/phys/em2da/em2da_pec.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em2da/em2da_pmc.py` & `petram_rf-1.5.7/petram/phys/em2da/em2da_pmc.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em2da/em2da_port.py` & `petram_rf-1.5.7/petram/phys/em2da/em2da_port.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em2da/em2da_surfj.py` & `petram_rf-1.5.7/petram/phys/em2da/em2da_surfj.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em2da/em2da_vac.py` & `petram_rf-1.5.7/petram/phys/em2da/em2da_vac.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em2da/eval_deriv.py` & `petram_rf-1.5.7/petram/phys/em2da/eval_deriv.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em3d/em3d_anisotropic.py` & `petram_rf-1.5.7/petram/phys/em3d/em3d_anisotropic.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em3d/em3d_base.py` & `petram_rf-1.5.7/petram/phys/em3d/em3d_base.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em3d/em3d_coldplasma.py` & `petram_rf-1.5.7/petram/phys/em3d/em3d_coldplasma.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
    cold plasma.
 '''
 from petram.phys.common.rf_dispersion_coldplasma import (stix_options,
                                                          default_stix_option,
-                                                         vtable_data)
+                                                         vtable_data0)
 
 import numpy as np
 
 from petram.mfem_config import use_parallel, get_numba_debug
 
 from petram.phys.vtable import VtableElement, Vtable
 from petram.phys.em3d.em3d_const import mu0, epsilon0
@@ -24,14 +24,15 @@
     import mfem.par as mfem
     from mpi4py import MPI
     myid = MPI.COMM_WORLD.rank
 else:
     import mfem.ser as mfem
     myid = 0
 
+vtable_data = vtable_data0.copy()
 
 def domain_constraints():
     return [EM3D_ColdPlasma]
 
 
 class EM3D_ColdPlasma(EM3D_Domain):
     allow_custom_intorder = True
```

### Comparing `petram_rf-1.5.5/petram/phys/em3d/em3d_div.py` & `petram_rf-1.5.7/petram/phys/em3d/em3d_div.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em3d/em3d_e.py` & `petram_rf-1.5.7/petram/phys/em3d/em3d_e.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em3d/em3d_extj.py` & `petram_rf-1.5.7/petram/phys/em3d/em3d_extj.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em3d/em3d_floquet.py` & `petram_rf-1.5.7/petram/phys/em3d/em3d_floquet.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em3d/em3d_h.py` & `petram_rf-1.5.7/petram/phys/em3d/em3d_h.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em3d/em3d_model.py` & `petram_rf-1.5.7/petram/phys/em3d/em3d_model.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em3d/em3d_pec.py` & `petram_rf-1.5.7/petram/phys/em3d/em3d_pec.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em3d/em3d_pmc.py` & `petram_rf-1.5.7/petram/phys/em3d/em3d_pmc.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em3d/em3d_pml.py` & `petram_rf-1.5.7/petram/phys/em3d/em3d_pml.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em3d/em3d_port.py` & `petram_rf-1.5.7/petram/phys/em3d/em3d_port.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em3d/em3d_portarray.py` & `petram_rf-1.5.7/petram/phys/em3d/em3d_portarray.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em3d/em3d_portload.py` & `petram_rf-1.5.7/petram/phys/em3d/em3d_portload.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em3d/em3d_portmode.py` & `petram_rf-1.5.7/petram/phys/em3d/em3d_portmode.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em3d/em3d_surfj.py` & `petram_rf-1.5.7/petram/phys/em3d/em3d_surfj.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em3d/em3d_vac.py` & `petram_rf-1.5.7/petram/phys/em3d/em3d_vac.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em3d/em3d_z.py` & `petram_rf-1.5.7/petram/phys/em3d/em3d_z.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em3d/eval_deriv.py` & `petram_rf-1.5.7/petram/phys/em3d/eval_deriv.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em3d/helper/export_nodalvalues.py` & `petram_rf-1.5.7/petram/phys/em3d/helper/export_nodalvalues.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/petram/phys/em3d/helper/write_cdf.py` & `petram_rf-1.5.7/petram/phys/em3d/helper/write_cdf.py`

 * *Files identical despite different names*

### Comparing `petram_rf-1.5.5/setup.py` & `petram_rf-1.5.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, 'README.md')) as f:
     long_description = f.read()
 
 setup(
     name='PetraM_RF',
-    version='1.5.5',
+    version='1.5.7',
 
     description='PetraM RF package',
     long_description=long_description,
     long_description_content_type = 'text/markdown', 
     url='https://github.com/piScope/PetraM',
     author='S. Shiraiwa',
     author_email='shiraiwa@princeton.edu',
```

