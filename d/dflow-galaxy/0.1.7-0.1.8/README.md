# Comparing `tmp/dflow_galaxy-0.1.7.tar.gz` & `tmp/dflow_galaxy-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dflow_galaxy-0.1.7.tar", max compression
+gzip compressed data, was "dflow_galaxy-0.1.8.tar", max compression
```

## Comparing `dflow_galaxy-0.1.7.tar` & `dflow_galaxy-0.1.8.tar`

### file list

```diff
@@ -1,80 +1,83 @@
--rw-r--r--   0        0        0    34523 2024-02-19 03:12:58.574253 dflow_galaxy-0.1.7/LICENSE
--rw-r--r--   0        0        0     2010 2024-04-12 09:29:48.592387 dflow_galaxy-0.1.7/README.md
--rw-r--r--   0        0        0        0 2024-01-30 01:22:58.649023 dflow_galaxy-0.1.7/dflow_galaxy/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.7/dflow_galaxy/app/__init__.py
--rw-r--r--   0        0        0     2498 2024-04-19 08:40:55.003134 dflow_galaxy-0.1.7/dflow_galaxy/app/common.py
--rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.7/dflow_galaxy/app/cp2k_lightning/__init__.py
--rw-r--r--   0        0        0     2167 2024-04-10 12:51:32.469597 dflow_galaxy-0.1.7/dflow_galaxy/app/cp2k_lightning/dflow.py
--rw-r--r--   0        0        0     7139 2024-04-19 09:47:38.573186 dflow_galaxy-0.1.7/dflow_galaxy/app/cp2k_lightning/main.py
--rw-r--r--   0        0        0        0 2024-04-07 12:32:16.436174 dflow_galaxy-0.1.7/dflow_galaxy/app/dynacat_md/__init__.py
--rw-r--r--   0        0        0     2006 2024-04-10 13:00:43.009583 dflow_galaxy-0.1.7/dflow_galaxy/app/dynacat_md/dflow.py
--rw-r--r--   0        0        0     4874 2024-04-19 08:41:31.523135 dflow_galaxy-0.1.7/dflow_galaxy/app/dynacat_md/main.py
--rw-r--r--   0        0        0     2525 2024-04-11 09:39:14.159344 dflow_galaxy-0.1.7/dflow_galaxy/app/dynacat_md/report.py
--rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.7/dflow_galaxy/app/dynacat_tesla/__init__.py
--rw-r--r--   0        0        0    16373 2024-04-19 09:26:16.823169 dflow_galaxy-0.1.7/dflow_galaxy/app/dynacat_tesla/main.py
--rw-r--r--   0        0        0     5892 2024-04-11 08:26:42.349456 dflow_galaxy-0.1.7/dflow_galaxy/app/dynacat_tesla/report.py
--rw-r--r--   0        0        0        0 2024-02-06 03:07:45.063120 dflow_galaxy-0.1.7/dflow_galaxy/core/__init__.py
--rw-r--r--   0        0        0    28431 2024-04-09 03:02:40.485846 dflow_galaxy-0.1.7/dflow_galaxy/core/dflow.py
--rw-r--r--   0        0        0     4687 2024-04-10 06:26:03.273692 dflow_galaxy-0.1.7/dflow_galaxy/core/dispatcher.py
--rw-r--r--   0        0        0      163 2024-02-06 03:07:45.063120 dflow_galaxy-0.1.7/dflow_galaxy/core/log.py
--rw-r--r--   0        0        0       97 2024-04-01 07:14:05.895738 dflow_galaxy-0.1.7/dflow_galaxy/core/pydantic.py
--rw-r--r--   0        0        0      541 2024-04-03 16:22:36.889294 dflow_galaxy-0.1.7/dflow_galaxy/core/types.py
--rw-r--r--   0        0        0     6065 2024-04-11 08:26:42.349456 dflow_galaxy-0.1.7/dflow_galaxy/core/util.py
--rw-r--r--   0        0        0      335 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.7/dflow_galaxy/main.py
--rw-r--r--   0        0        0      146 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.7/dflow_galaxy/res/__init__.py
--rw-r--r--   0        0        0   189331 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/ALL_BASIS_SETS
--rw-r--r--   0        0        0     2717 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/ALL_POTENTIALS
--rw-r--r--   0        0        0    15836 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/AcPP1_POTENTIALS
--rw-r--r--   0        0        0    57524 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_ADMM
--rw-r--r--   0        0        0   189911 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_ADMM_MOLOPT
--rw-r--r--   0        0        0   133011 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_ADMM_UZH
--rw-r--r--   0        0        0    66934 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_ADMM_ae
--rw-r--r--   0        0        0    17509 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_LRIGPW_AUXMOLOPT
--rw-r--r--   0        0        0   244853 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_MINBAS
--rw-r--r--   0        0        0    49588 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_MINIX
--rw-r--r--   0        0        0   127679 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT
--rw-r--r--   0        0        0    55644 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_AcPP1
--rw-r--r--   0        0        0    23527 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP1
--rw-r--r--   0        0        0    65485 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP2
--rw-r--r--   0        0        0   179850 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UCL
--rw-r--r--   0        0        0  1574370 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UZH
--rw-r--r--   0        0        0     6644 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_PERIODIC_GW
--rw-r--r--   0        0        0    37261 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_RI_cc-TZ
--rw-r--r--   0        0        0   195109 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_SET
--rw-r--r--   0        0        0     5526 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_ZIJLSTRA
--rw-r--r--   0        0        0   324291 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_ccGRB_UZH
--rw-r--r--   0        0        0   258169 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_def2_QZVP_RI_ALL
--rw-r--r--   0        0        0   191314 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_pob
--rw-r--r--   0        0        0   223481 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS
--rw-r--r--   0        0        0    23668 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS_pob-TZVP-rev2
--rw-r--r--   0        0        0  1713484 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/EMSL_BASIS_SETS
--rw-r--r--   0        0        0   119403 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/GTH_BASIS_SETS
--rw-r--r--   0        0        0   167483 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/GTH_POTENTIALS
--rw-r--r--   0        0        0   253677 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/GTH_SOC_POTENTIALS
--rw-r--r--   0        0        0    17275 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/HFX_BASIS
--rw-r--r--   0        0        0     2106 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/HF_POTENTIALS
--rw-r--r--   0        0        0     5486 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/LnPP1_POTENTIALS
--rw-r--r--   0        0        0     7829 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/LnPP2_POTENTIALS
--rw-r--r--   0        0        0      447 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/MM_POTENTIAL
--rw-r--r--   0        0        0     5498 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/NLCC_POTENTIALS
--rw-r--r--   0        0        0   177804 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/POTENTIAL
--rw-r--r--   0        0        0   385325 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/POTENTIAL_UZH
--rw-r--r--   0        0        0      125 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/README.md
--rw-r--r--   0        0        0    91811 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/nm12_parameters.xml
--rw-r--r--   0        0        0    32194 2024-04-02 03:42:50.640085 dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/xTB_parameters
--rw-r--r--   0        0        0     1128 2024-04-19 08:58:50.173149 dflow_galaxy-0.1.7/dflow_galaxy/res/dynacat/deepmd.json
--rw-r--r--   0        0        0     1171 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.7/dflow_galaxy/res/dynacat/tesla_template.yml
--rw-r--r--   0        0        0      906 2024-04-18 09:39:30.561274 dflow_galaxy-0.1.7/dflow_galaxy/util.py
--rw-r--r--   0        0        0        0 2024-02-07 08:30:41.445577 dflow_galaxy-0.1.7/dflow_galaxy/workflow/__init__.py
--rw-r--r--   0        0        0        0 2024-02-07 08:30:41.445577 dflow_galaxy-0.1.7/dflow_galaxy/workflow/tesla/__init__.py
--rw-r--r--   0        0        0     1702 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.7/dflow_galaxy/workflow/tesla/config.py
--rw-r--r--   0        0        0        0 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.7/dflow_galaxy/workflow/tesla/domain/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.7/dflow_galaxy/workflow/tesla/domain/abacus.py
--rw-r--r--   0        0        0     6339 2024-04-10 05:02:53.113820 dflow_galaxy-0.1.7/dflow_galaxy/workflow/tesla/domain/cp2k.py
--rw-r--r--   0        0        0     9692 2024-04-11 08:26:42.349456 dflow_galaxy-0.1.7/dflow_galaxy/workflow/tesla/domain/deepmd.py
--rw-r--r--   0        0        0     8057 2024-04-11 02:42:29.459986 dflow_galaxy-0.1.7/dflow_galaxy/workflow/tesla/domain/lammps.py
--rw-r--r--   0        0        0     1261 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.7/dflow_galaxy/workflow/tesla/domain/lib.py
--rw-r--r--   0        0        0     6334 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.7/dflow_galaxy/workflow/tesla/domain/model_devi.py
--rw-r--r--   0        0        0     8185 2024-04-11 01:41:14.700081 dflow_galaxy-0.1.7/dflow_galaxy/workflow/tesla/main.py
--rw-r--r--   0        0        0      560 2024-04-19 09:48:39.823185 dflow_galaxy-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2695 1970-01-01 00:00:00.000000 dflow_galaxy-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-02-19 03:12:58.574253 dflow_galaxy-0.1.8/LICENSE
+-rw-r--r--   0        0        0     2009 2024-04-22 00:50:41.993871 dflow_galaxy-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2024-01-30 01:22:58.649023 dflow_galaxy-0.1.8/dflow_galaxy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.8/dflow_galaxy/app/__init__.py
+-rw-r--r--   0        0        0     2498 2024-04-19 08:40:55.003134 dflow_galaxy-0.1.8/dflow_galaxy/app/common.py
+-rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.8/dflow_galaxy/app/cp2k_lightning/__init__.py
+-rw-r--r--   0        0        0     2211 2024-05-11 02:28:32.269795 dflow_galaxy-0.1.8/dflow_galaxy/app/cp2k_lightning/dflow.py
+-rw-r--r--   0        0        0     7096 2024-05-11 02:28:32.269795 dflow_galaxy-0.1.8/dflow_galaxy/app/cp2k_lightning/main.py
+-rw-r--r--   0        0        0        0 2024-04-07 12:32:16.436174 dflow_galaxy-0.1.8/dflow_galaxy/app/dynacat_md/__init__.py
+-rw-r--r--   0        0        0     2050 2024-05-11 02:28:32.269795 dflow_galaxy-0.1.8/dflow_galaxy/app/dynacat_md/dflow.py
+-rw-r--r--   0        0        0     4874 2024-04-19 08:41:31.523135 dflow_galaxy-0.1.8/dflow_galaxy/app/dynacat_md/main.py
+-rw-r--r--   0        0        0     2525 2024-04-11 09:39:14.159344 dflow_galaxy-0.1.8/dflow_galaxy/app/dynacat_md/report.py
+-rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.8/dflow_galaxy/app/dynacat_tesla/__init__.py
+-rw-r--r--   0        0        0    16373 2024-04-19 11:59:38.140345 dflow_galaxy-0.1.8/dflow_galaxy/app/dynacat_tesla/main.py
+-rw-r--r--   0        0        0     5892 2024-04-11 08:26:42.349456 dflow_galaxy-0.1.8/dflow_galaxy/app/dynacat_tesla/report.py
+-rw-r--r--   0        0        0        0 2024-02-06 03:07:45.063120 dflow_galaxy-0.1.8/dflow_galaxy/core/__init__.py
+-rw-r--r--   0        0        0    29475 2024-05-11 02:28:32.269795 dflow_galaxy-0.1.8/dflow_galaxy/core/dflow_builder.py
+-rw-r--r--   0        0        0     4687 2024-04-10 06:26:03.273692 dflow_galaxy-0.1.8/dflow_galaxy/core/dispatcher.py
+-rw-r--r--   0        0        0      163 2024-02-06 03:07:45.063120 dflow_galaxy-0.1.8/dflow_galaxy/core/log.py
+-rw-r--r--   0        0        0       97 2024-04-01 07:14:05.895738 dflow_galaxy-0.1.8/dflow_galaxy/core/pydantic.py
+-rw-r--r--   0        0        0      541 2024-05-09 06:36:33.177848 dflow_galaxy-0.1.8/dflow_galaxy/core/types.py
+-rw-r--r--   0        0        0     6065 2024-04-11 08:26:42.349456 dflow_galaxy-0.1.8/dflow_galaxy/core/util.py
+-rw-r--r--   0        0        0      335 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.8/dflow_galaxy/main.py
+-rw-r--r--   0        0        0      146 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.8/dflow_galaxy/res/__init__.py
+-rw-r--r--   0        0        0   189331 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/ALL_BASIS_SETS
+-rw-r--r--   0        0        0     2717 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/ALL_POTENTIALS
+-rw-r--r--   0        0        0    15836 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/AcPP1_POTENTIALS
+-rw-r--r--   0        0        0    57524 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_ADMM
+-rw-r--r--   0        0        0   189911 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_ADMM_MOLOPT
+-rw-r--r--   0        0        0   133011 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_ADMM_UZH
+-rw-r--r--   0        0        0    66934 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_ADMM_ae
+-rw-r--r--   0        0        0    17509 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_LRIGPW_AUXMOLOPT
+-rw-r--r--   0        0        0   244853 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_MINBAS
+-rw-r--r--   0        0        0    49588 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_MINIX
+-rw-r--r--   0        0        0   127679 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT
+-rw-r--r--   0        0        0    55644 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_AcPP1
+-rw-r--r--   0        0        0    23527 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP1
+-rw-r--r--   0        0        0    65485 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP2
+-rw-r--r--   0        0        0   179850 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UCL
+-rw-r--r--   0        0        0  1574370 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UZH
+-rw-r--r--   0        0        0     6644 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_PERIODIC_GW
+-rw-r--r--   0        0        0    37261 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_RI_cc-TZ
+-rw-r--r--   0        0        0   195109 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_SET
+-rw-r--r--   0        0        0     5526 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_ZIJLSTRA
+-rw-r--r--   0        0        0   324291 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_ccGRB_UZH
+-rw-r--r--   0        0        0   258169 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_def2_QZVP_RI_ALL
+-rw-r--r--   0        0        0   191314 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_pob
+-rw-r--r--   0        0        0   223481 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS
+-rw-r--r--   0        0        0    23668 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS_pob-TZVP-rev2
+-rw-r--r--   0        0        0  1713484 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/EMSL_BASIS_SETS
+-rw-r--r--   0        0        0   119403 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/GTH_BASIS_SETS
+-rw-r--r--   0        0        0   167483 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/GTH_POTENTIALS
+-rw-r--r--   0        0        0   253677 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/GTH_SOC_POTENTIALS
+-rw-r--r--   0        0        0    17275 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/HFX_BASIS
+-rw-r--r--   0        0        0     2106 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/HF_POTENTIALS
+-rw-r--r--   0        0        0     5486 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/LnPP1_POTENTIALS
+-rw-r--r--   0        0        0     7829 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/LnPP2_POTENTIALS
+-rw-r--r--   0        0        0      447 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/MM_POTENTIAL
+-rw-r--r--   0        0        0     5498 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/NLCC_POTENTIALS
+-rw-r--r--   0        0        0   177804 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/POTENTIAL
+-rw-r--r--   0        0        0   385325 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/POTENTIAL_UZH
+-rw-r--r--   0        0        0      125 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/README.md
+-rw-r--r--   0        0        0    91811 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/nm12_parameters.xml
+-rw-r--r--   0        0        0    32194 2024-04-02 03:42:50.640085 dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/xTB_parameters
+-rw-r--r--   0        0        0     1128 2024-04-19 08:58:50.173149 dflow_galaxy-0.1.8/dflow_galaxy/res/dynacat/deepmd.json
+-rw-r--r--   0        0        0     1171 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.8/dflow_galaxy/res/dynacat/tesla_template.yml
+-rw-r--r--   0        0        0      906 2024-04-18 09:39:30.561274 dflow_galaxy-0.1.8/dflow_galaxy/util.py
+-rw-r--r--   0        0        0        0 2024-02-07 08:30:41.445577 dflow_galaxy-0.1.8/dflow_galaxy/workflow/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-11 02:28:32.269795 dflow_galaxy-0.1.8/dflow_galaxy/workflow/reweighting/__init__.py
+-rw-r--r--   0        0        0     1172 2024-05-11 02:28:32.269795 dflow_galaxy-0.1.8/dflow_galaxy/workflow/reweighting/domain.py
+-rw-r--r--   0        0        0     1255 2024-05-11 02:28:32.269795 dflow_galaxy-0.1.8/dflow_galaxy/workflow/reweighting/main.py
+-rw-r--r--   0        0        0        0 2024-02-07 08:30:41.445577 dflow_galaxy-0.1.8/dflow_galaxy/workflow/tesla/__init__.py
+-rw-r--r--   0        0        0     1702 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.8/dflow_galaxy/workflow/tesla/config.py
+-rw-r--r--   0        0        0        0 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.8/dflow_galaxy/workflow/tesla/domain/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.8/dflow_galaxy/workflow/tesla/domain/abacus.py
+-rw-r--r--   0        0        0     6347 2024-05-11 02:28:32.269795 dflow_galaxy-0.1.8/dflow_galaxy/workflow/tesla/domain/cp2k.py
+-rw-r--r--   0        0        0     9700 2024-05-11 02:28:32.269795 dflow_galaxy-0.1.8/dflow_galaxy/workflow/tesla/domain/deepmd.py
+-rw-r--r--   0        0        0     8065 2024-05-11 02:28:32.269795 dflow_galaxy-0.1.8/dflow_galaxy/workflow/tesla/domain/lammps.py
+-rw-r--r--   0        0        0     1261 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.8/dflow_galaxy/workflow/tesla/domain/lib.py
+-rw-r--r--   0        0        0     6342 2024-05-11 02:28:32.269795 dflow_galaxy-0.1.8/dflow_galaxy/workflow/tesla/domain/model_devi.py
+-rw-r--r--   0        0        0     8193 2024-05-11 02:28:32.269795 dflow_galaxy-0.1.8/dflow_galaxy/workflow/tesla/main.py
+-rw-r--r--   0        0        0      740 2024-05-11 02:30:33.739764 dflow_galaxy-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2694 1970-01-01 00:00:00.000000 dflow_galaxy-0.1.8/PKG-INFO
```

### Comparing `dflow_galaxy-0.1.7/LICENSE` & `dflow_galaxy-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/README.md` & `dflow_galaxy-0.1.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 ## Features
 
 ### Tools
 * DFlowBuilder: A type friendly wrapper for `DFlow` to build workflows in a more intuitive way.
 
 ### Workflow
-* TESLA: a **T**raining-**E**xploration-**S**creening-**L**abeling workflow developed by **AI4EC**. Get inspired by [DPGEN](https://github.com/deepmodeling/dpgen), [DPGEN2](https://github.com/deepmodeling/dpgen2), ported from [ai2-kit](https://github.com/chenggroup/ai2-kit).
+* TESLA: a **T**raining-**E**xploration-**S**creening-**L**abeling workflow developed by **AI4EC**. Get inspired by [DPGEN](https://github.com/deepmodeling/dpgen), [DPGEN2](https://github.com/deepmodeling/dpgen2), powered by [ai2-kit](https://github.com/chenggroup/ai2-kit).
 
 ### [Bohrium Apps](https://bohrium.dp.tech/apps)
 Bohrium Apps are cloud native apps that can be run on Bohrium Platform. 
 
 * CP2K Lightning: Run CP2K without building input files from scratch.
 * DynaCat TESLA: An automated workflow to generated DeepMD potential for DynaCat.
 * DynaCat MD: Run MD simulations with DeepMD potential for DynaCat.
```

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/app/common.py` & `dflow_galaxy-0.1.8/dflow_galaxy/app/common.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/app/cp2k_lightning/dflow.py` & `dflow_galaxy-0.1.8/dflow_galaxy/app/cp2k_lightning/dflow.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from dataclasses import dataclass
-from dflow_galaxy.core import dflow, types, dispatcher
+from dflow_galaxy.core import types, dispatcher
+from dflow_galaxy.core.dflow_builder import DFlowBuilder
 import shutil
 import os
 
 
 @dataclass(frozen=True)
 class RunCp2kArgs:
     input_dir : types.InputArtifact
@@ -36,15 +37,15 @@
                       cp2k_script: str):
 
     # bohrium dispatcher will be configured in bohrium.config
     # so here we just leave it empty
     bohrium_config = dispatcher.BohriumConfig()
 
     # start to build workflow
-    dflow_builder = dflow.DFlowBuilder('cp2k', s3_prefix='cp2k')
+    dflow_builder = DFlowBuilder('cp2k', s3_prefix='cp2k')
 
     # setup and add cp2k step to workflow
     cp2k_res = dispatcher.Resource(
         bohrium=dispatcher.BohriumInputData(
             image_name=cp2k_image,
             scass_type=cp2k_device_model,
             disk_size=100,
```

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/app/cp2k_lightning/main.py` & `dflow_galaxy-0.1.8/dflow_galaxy/app/cp2k_lightning/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from dp.launching.typing import BaseModel, Field, OutputDirectory, InputFilePath, Optional
 from dp.launching.typing import Int, String, Enum, Float, Boolean, Set
-from dp.launching.cli import to_runner, default_minimal_exception_handler
+from dp.launching.cli import to_runner
 
 from dflow_galaxy.app.common import DFlowOptionsMixin, setup_dflow_context
 from dflow_galaxy.res import get_cp2k_data_dir
 from dflow_galaxy.core.log import get_logger
 from ai2_kit.feat import catalysis as ai2cat
-from ai2_kit.tool.ase import AseHelper
-from ai2_kit.tool.dpdata import DpdataHelper
+from ai2_kit.tool.ase import AseTool
+from ai2_kit.tool.dpdata import DpdataTool
 
 from pathlib import Path
 import shutil
 import sys
 import os
 
 from .dflow import run_cp2k_workflow
@@ -187,21 +187,21 @@
         cp2k_device_model=str(args.cp2k_device_model),
         cp2k_image=str(args.cp2k_image),
         cp2k_script=str(args.cp2k_script),
     )
 
     # stage 3: post-process cp2k output
     # convert cp2k output to xyz file and dpdata set
-    AseHelper().read(
+    AseTool().read(
         os.path.join(cp2k_output_dir, '*-pos-1.xyz')
     ).set_by_ref(
         system_file
     ).write(str(out_dir / 'aimd.xyz' ))
 
-    DpdataHelper().read(
+    DpdataTool().read(
         cp2k_output_dir, fmt='cp2kdata/md', cp2k_output_name='output'
     ).write(str(out_dir / 'dp-dataset'))
 
     return 0
 
 def main():
     to_runner(
```

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/app/dynacat_md/dflow.py` & `dflow_galaxy-0.1.8/dflow_galaxy/app/dynacat_md/dflow.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from dataclasses import dataclass
-from dflow_galaxy.core import dflow, types, dispatcher
+from dflow_galaxy.core import types, dispatcher
+from dflow_galaxy.core.dflow_builder import DFlowBuilder
 import shutil
 import os
 
 
 @dataclass(frozen=True)
 class RunLammpsArgs:
     input_dir : types.InputArtifact
@@ -31,15 +32,15 @@
                         lammps_script: str):
 
     # bohrium dispatcher will be configured in bohrium.config
     # so here we just leave it empty
     bohrium_config = dispatcher.BohriumConfig()
 
     # start to build workflow
-    dflow_builder = dflow.DFlowBuilder('lammps', s3_prefix='lammps')
+    dflow_builder = DFlowBuilder('lammps', s3_prefix='lammps')
 
     # setup and add lammps step to workflow
     lammps_res = dispatcher.Resource(
         bohrium=dispatcher.BohriumInputData(
             image_name=lammps_image,
             scass_type=lammps_device_model,
             disk_size=100,
```

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/app/dynacat_md/main.py` & `dflow_galaxy-0.1.8/dflow_galaxy/app/dynacat_md/main.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/app/dynacat_md/report.py` & `dflow_galaxy-0.1.8/dflow_galaxy/app/dynacat_md/report.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/app/dynacat_tesla/main.py` & `dflow_galaxy-0.1.8/dflow_galaxy/app/dynacat_tesla/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 BH_CP2K_DEFAULT = {
     'image_name': 'registry.dp.tech/dptech/cp2k:11',
     'scass_type': 'c32_m64_cpu',
 }
 
 BH_PYTHON_DEFAULT = {
-    'image_name': 'registry.dp.tech/dptech/prod-13325/dflow-galaxy:0.1.4-main-8bb98c7',
+    'image_name': 'registry.dp.tech/dptech/prod-13325/dflow-galaxy:0.1.7-main-07745fb',
     'scass_type': 'c2_m4_cpu',
 }
 
 
 class KvItem(BaseModel):
     key: String = Field(
         description="Key of the item")
```

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/app/dynacat_tesla/report.py` & `dflow_galaxy-0.1.8/dflow_galaxy/app/dynacat_tesla/report.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/core/dflow.py` & `dflow_galaxy-0.1.8/dflow_galaxy/core/dflow_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from dflow.op_template import ScriptOPTemplate
 from dflow.plugins.dispatcher import DispatcherExecutor
 import dflow
 
-from typing import Final, Callable, TypeVar, Optional, Union, Annotated, Generic, Dict, Any, Iterable
+from typing import Final, Callable, TypeVar, Optional, Union, Generic, Dict, Any, Iterable, get_args, get_origin
+
 from dataclasses import fields, is_dataclass
 from urllib.parse import urlparse
 from collections import namedtuple
 from pathlib import Path
 from uuid import uuid4
 import cloudpickle as cp
 import tempfile
@@ -56,41 +57,70 @@
     def __getattr__(self, name):
         for obj in self.objs:
             if name in obj:
                 return obj[name]
         raise AttributeError(f'{name} not found in {self.objs}')
 
 
+def parse_dflow_field(field):
+    name = field.name
+    _type = field.type
+
+    args = get_args(_type)
+    origin = get_origin(_type)
+    optional = False
+
+    if origin is Union:
+        if type(None) not in args or len(args) != 2:
+            raise ValueError(f'Invalid Union type `{_type}` for field `{name}`, you may want to use Optional[T]?')
+        _type = args[0]
+        origin = get_origin(_type)
+        args = get_args(_type)
+        optional = True
+
+    error_msg = f'Invalid type `{_type}` for field `{name}`, must be one of InputParam, InputArtifact, OutputParam, OutputArtifact, Annotated[str, dflow.InputArtifact(...)], Annotated[str, dflow.OutputArtifact(...)]'
+    metadata = getattr(_type, '__metadata__', None)
+    if metadata is None or len(metadata) != 1:
+        raise ValueError(error_msg)
+
+    if metadata[0] not in (
+        types.Symbol.INPUT_PARAMETER,
+        types.Symbol.INPUT_ARTIFACT,
+        types.Symbol.OUTPUT_ARTIFACT,
+    ) and not isinstance(metadata[0], dflow.InputArtifact) and not isinstance(metadata[0], dflow.OutputArtifact):
+        raise ValueError(error_msg)
+
+    return _type, optional
+
+
 def pickle_converts(obj, pickle_module='cp', bz2_module='bz2', base64_module='base64'):
     """
     convert an object to its pickle string form
     """
     obj_pkl = cp.dumps(obj, protocol=cp.DEFAULT_PROTOCOL)
     compress_level = 5 if len(obj_pkl) > 4096 else 1
     compressed = bz2.compress(obj_pkl, compress_level)
     obj_b64 = base64.b64encode(compressed).decode('ascii')
     return f'{pickle_module}.loads({bz2_module}.decompress({base64_module}.b64decode({repr(obj_b64)})))'
 
 
+_ParsedField = namedtuple('_ParseField', ['name', 'type', 'optional', 'value'])
+
 def iter_python_step_args(obj):
     """
     Iterate over the input fields of a python step.
     A python step input should be:
     1. A frozen dataclass.
     2. All fields are annotated with InputParam, InputArtifact or OutputArtifact.
     """
     assert is_dataclass(obj), f'{obj} is not a dataclass'
-    assert obj.__dataclass_params__.frozen, f'{obj} is not frozen'
     for f in fields(obj):
-        msg = f'{f.name} is not annotated with InputParam, InputArtifact or OutputArtifact'
-        assert hasattr(f.type, '__metadata__'), msg
-        assert f.type.__metadata__[0] in (
-            types.Symbol.INPUT_PARAMETER, types.Symbol.INPUT_ARTIFACT,
-            types.Symbol.OUTPUT_ARTIFACT), msg
-        yield f, getattr(obj, f.name, None)
+        _type, optional = parse_dflow_field(f)
+        yield _ParsedField(name=f.name, type=_type,
+                           optional=optional, value=getattr(obj, f.name, None))
 
 
 def iter_python_step_return(obj):
     """
     Iterate over the output fields of a python step.
     A python step output should be:
     1. A dataclass.
@@ -142,15 +172,15 @@
         setup_script,
         ''
         f'mkdir -p {shlex.quote(output_artifacts_dir)}',
         '',
         '# Setup Variables',
     ]
 
-    for f, v in iter_python_step_args(args_type):
+    for f in iter_python_step_args(args_type):
         meta = f.type.__metadata__[0]
         if meta == types.Symbol.INPUT_PARAMETER:
             # input parameter can be a multiline string
             bash_name = f'_DF_INPUT_PARAMETER_{f.name}_'
             source.extend([
                 f"{bash_name}=$(cat << {eof}",
                 f"{{{{inputs.parameters.{f.name}}}}}",
@@ -162,25 +192,25 @@
 
         elif meta == types.Symbol.INPUT_ARTIFACT or isinstance(meta, dflow.InputArtifact):
             bash_name = f'_DF_INPUT_ARTIFACT_{f.name}_'
             path = os.path.join(input_artifacts_dir, f.name)
             source.append(f'{bash_name}={shlex.quote(path)}')
             artifact = meta
             if not isinstance(artifact, dflow.InputArtifact):
-                artifact = dflow.InputArtifact(path=path, archive=default_archive)  # type: ignore
+                artifact = dflow.InputArtifact(path=path, archive=default_archive, optional=f.optional)  # type: ignore
             dflow_input_artifacts[f.name] = artifact
             args_dict[f.name] = f'${bash_name}'
 
         elif meta == types.Symbol.OUTPUT_ARTIFACT or isinstance(meta, dflow.OutputArtifact):
             bash_name = f'_DF_OUTPUT_ARTIFACT_{f.name}_'
             path = os.path.join(output_artifacts_dir, f.name)
             source.append(f'{bash_name}={shlex.quote(path)}')
             artifact = meta
             if not isinstance(artifact, dflow.OutputArtifact):
-                artifact = dflow.OutputArtifact(path=path, archive=default_archive)  # type: ignore
+                artifact = dflow.OutputArtifact(path=path, archive=default_archive, optional=f.optional)  # type: ignore
             dflow_output_artifacts[f.name] = artifact
 
             args_dict[f.name] = f'${bash_name}'
         else:
             raise ValueError(f'unsupported type {f.type}')
 
     bash_script = py_fn(ObjProxy(args_dict))
@@ -256,15 +286,15 @@
         'os.makedirs(fn_dir, exist_ok=True)',
         'os.makedirs(pkg_dir, exist_ok=True)',
         'os.makedirs(output_parameters_dir, exist_ok=True)',
         'os.makedirs(output_artifacts_dir, exist_ok=True)',
         'args = dict()',
     ]
 
-    for f, v in iter_python_step_args(args_type):
+    for f in iter_python_step_args(args_type):
         meta = f.type.__metadata__[0]
         if meta == types.Symbol.INPUT_PARAMETER:
             # FIXME: may have error in some corner cases
             if _is_str_type(f.type.__origin__):
                 val = f'"""{{{{inputs.parameters.{f.name}}}}}"""'
             else:
                 val = f'json.loads("""{{{{inputs.parameters.{f.name}}}}}""")'
@@ -642,22 +672,22 @@
                     with_param: Any=None,
                     executor: Optional[DispatcherExecutor] = None):
         if executor is None:
             executor = self._default_executor
 
         parameters = {}
         artifacts = {}
-        for f, v in iter_python_step_args(args):
+        for f in iter_python_step_args(args):
             meta = f.type.__metadata__[0]
             if meta == types.Symbol.INPUT_PARAMETER:
-                parameters[f.name] = v
+                parameters[f.name] = f.value
             elif meta == types.Symbol.INPUT_ARTIFACT or isinstance(meta, dflow.InputArtifact):
-                artifacts[f.name] = self._ensure_artifact(v)  # type: ignore
+                artifacts[f.name] = self._ensure_artifact(f.value)  # type: ignore
             elif meta == types.Symbol.OUTPUT_ARTIFACT or isinstance(meta, dflow.OutputArtifact):
-                template.outputs.artifacts[f.name].save = [self._ensure_artifact(v)]  # type: ignore
+                template.outputs.artifacts[f.name].save = [self._ensure_artifact(f.value)]  # type: ignore
             else:
                 raise ValueError(f'unsupported type {f.type}')
 
         step = dflow.Step(
             name=name,
             template=template,
             with_param=with_param,
```

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/core/dispatcher.py` & `dflow_galaxy-0.1.8/dflow_galaxy/core/dispatcher.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/core/types.py` & `dflow_galaxy-0.1.8/dflow_galaxy/core/types.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/core/util.py` & `dflow_galaxy-0.1.8/dflow_galaxy/core/util.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/ALL_BASIS_SETS` & `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/ALL_BASIS_SETS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/ALL_POTENTIALS` & `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/ALL_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/AcPP1_POTENTIALS` & `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/AcPP1_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_ADMM` & `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_ADMM`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_ADMM_MOLOPT` & `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_ADMM_MOLOPT`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_ADMM_UZH` & `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_ADMM_UZH`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_ADMM_ae` & `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_ADMM_ae`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_LRIGPW_AUXMOLOPT` & `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_LRIGPW_AUXMOLOPT`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_MINBAS` & `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_MINBAS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_MINIX` & `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_MINIX`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT` & `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_AcPP1` & `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_AcPP1`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP1` & `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP1`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP2` & `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP2`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UCL` & `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UCL`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UZH` & `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UZH`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_PERIODIC_GW` & `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_PERIODIC_GW`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_RI_cc-TZ` & `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_RI_cc-TZ`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_SET` & `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_SET`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_ZIJLSTRA` & `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_ZIJLSTRA`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_ccGRB_UZH` & `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_ccGRB_UZH`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_def2_QZVP_RI_ALL` & `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_def2_QZVP_RI_ALL`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/BASIS_pob` & `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/BASIS_pob`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS` & `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS_pob-TZVP-rev2` & `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS_pob-TZVP-rev2`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/EMSL_BASIS_SETS` & `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/EMSL_BASIS_SETS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/GTH_BASIS_SETS` & `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/GTH_BASIS_SETS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/GTH_POTENTIALS` & `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/GTH_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/GTH_SOC_POTENTIALS` & `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/GTH_SOC_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/HFX_BASIS` & `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/HFX_BASIS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/HF_POTENTIALS` & `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/HF_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/LnPP1_POTENTIALS` & `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/LnPP1_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/LnPP2_POTENTIALS` & `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/LnPP2_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/NLCC_POTENTIALS` & `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/NLCC_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/POTENTIAL` & `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/POTENTIAL`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/POTENTIAL_UZH` & `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/POTENTIAL_UZH`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/nm12_parameters.xml` & `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/nm12_parameters.xml`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/res/cp2k_data/xTB_parameters` & `dflow_galaxy-0.1.8/dflow_galaxy/res/cp2k_data/xTB_parameters`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/res/dynacat/deepmd.json` & `dflow_galaxy-0.1.8/dflow_galaxy/res/dynacat/deepmd.json`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/res/dynacat/tesla_template.yml` & `dflow_galaxy-0.1.8/dflow_galaxy/res/dynacat/tesla_template.yml`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/util.py` & `dflow_galaxy-0.1.8/dflow_galaxy/util.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/workflow/tesla/config.py` & `dflow_galaxy-0.1.8/dflow_galaxy/workflow/tesla/config.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/workflow/tesla/domain/cp2k.py` & `dflow_galaxy-0.1.8/dflow_galaxy/workflow/tesla/domain/cp2k.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from copy import deepcopy
 from pathlib import Path
 import glob
 import os
 
 from dflow_galaxy.core.pydantic import BaseModel
 from dflow_galaxy.core.dispatcher import BaseApp, PythonApp, create_dispatcher, ExecutorConfig
-from dflow_galaxy.core.dflow import DFlowBuilder
+from dflow_galaxy.core.dflow_builder import DFlowBuilder
 from dflow_galaxy.core.util import bash_iter_ls_slice, safe_ln, bash_ln_cmd, bash_inspect_dir, inspect_dir
 from dflow_galaxy.core import types
 
 from ai2_kit.domain.cp2k import make_cp2k_task_dirs
 from ai2_kit.core.artifact import Artifact, ArtifactDict
 from ai2_kit.core.util import cmd_with_checkpoint as cmd_cp, list_sample, load_text, dump_text, ensure_dir
```

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/workflow/tesla/domain/deepmd.py` & `dflow_galaxy-0.1.8/dflow_galaxy/workflow/tesla/domain/deepmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from ai2_kit.domain.deepmd import make_deepmd_task_dirs
 from ai2_kit.core.util import cmd_with_checkpoint as cmd_cp, load_text
 from ai2_kit.domain.constant import DP_INPUT_FILE, DP_ORIGINAL_MODEL, DP_FROZEN_MODEL
 
 from dflow_galaxy.core.pydantic import BaseModel
 from dflow_galaxy.core.dispatcher import BaseApp, PythonApp, create_dispatcher, ExecutorConfig
-from dflow_galaxy.core.dflow import DFlowBuilder
+from dflow_galaxy.core.dflow_builder import DFlowBuilder
 from dflow_galaxy.core.util import bash_iter_ls_slice, safe_ln, bash_ln_cmd, bash_inspect_dir, inspect_dir
 from dflow_galaxy.core.log import get_logger
 from dflow_galaxy.core import types
 
 from dflow import argo_range
 import dpdata
```

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/workflow/tesla/domain/lammps.py` & `dflow_galaxy-0.1.8/dflow_galaxy/workflow/tesla/domain/lammps.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from dataclasses import dataclass
 from copy import deepcopy
 import glob
 import os
 
 from dflow_galaxy.core.pydantic import BaseModel
 from dflow_galaxy.core.dispatcher import BaseApp, PythonApp, create_dispatcher, ExecutorConfig
-from dflow_galaxy.core.dflow import DFlowBuilder
+from dflow_galaxy.core.dflow_builder import DFlowBuilder
 from dflow_galaxy.core.util import bash_iter_ls_slice, safe_ln, bash_ln_cmd, inspect_dir, bash_inspect_dir
 from dflow_galaxy.core import types
 
 from ai2_kit.domain.lammps import make_lammps_task_dirs, FepOptions
 from ai2_kit.domain.constant import DP_FROZEN_MODEL
 from ai2_kit.core.artifact import Artifact, ArtifactDict
 from ai2_kit.core.util import cmd_with_checkpoint as cmd_cp, dump_text
```

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/workflow/tesla/domain/lib.py` & `dflow_galaxy-0.1.8/dflow_galaxy/workflow/tesla/domain/lib.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/workflow/tesla/domain/model_devi.py` & `dflow_galaxy-0.1.8/dflow_galaxy/workflow/tesla/domain/model_devi.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from tabulate import tabulate
 import pandas as pd
 import ase.io
 
 from dflow_galaxy.core.pydantic import BaseModel
 
 from dflow_galaxy.core.dispatcher import PythonApp, create_dispatcher, ExecutorConfig
-from dflow_galaxy.core.dflow import DFlowBuilder
+from dflow_galaxy.core.dflow_builder import DFlowBuilder
 from dflow_galaxy.core import types
 from dflow_galaxy.core.util import inspect_dir
 
 from ai2_kit.core.util import load_text, dump_text
 
 from .lib import ExploreApp
```

### Comparing `dflow_galaxy-0.1.7/dflow_galaxy/workflow/tesla/main.py` & `dflow_galaxy-0.1.8/dflow_galaxy/workflow/tesla/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional
 from copy import deepcopy
 
 from ai2_kit.core.util import load_yaml_files, merge_dict
 from ai2_kit.core.cmd import CmdGroup
 
-from dflow_galaxy.core.dflow import DFlowBuilder
+from dflow_galaxy.core.dflow_builder import DFlowBuilder
 from dflow_galaxy.core.util import not_none
 from dflow_galaxy.core.log import get_logger
 
 from .config import TeslaConfig, WorkflowConfig
 from .domain import deepmd, lammps, model_devi, cp2k
 from .domain.lib import StepSwitch, LabelApp, ExploreApp
```

### Comparing `dflow_galaxy-0.1.7/pyproject.toml` & `dflow_galaxy-0.1.8/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,37 @@
 [tool.poetry]
 name = "dflow-galaxy"
-version = "0.1.7"
+version = "0.1.8"
 description = ""
 authors = ["weihong.xu <xuweihong.cn@gmail.com>"]
 readme = "README.md"
 include = ["dflow_galaxy/res/*"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pydflow = "1.8.60"
 dpdispatcher = "^0.6.4"
-ai2-kit= "0.16.0"
+ai2-kit= "0.18.1"
 dp-launching-sdk = "^0.12.0"
 lbg = "^1.2.24"
 cp2kdata = "^0.6.6"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.0"
 sphinx = "^7.2.6"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-dgcli = "dflow_galaxy.main:main"
+dgcli = "dflow_galaxy.main:main"
+
+[tool.ruff]
+preview = true
+line-length = 120
+
+[tool.ruff.lint]
+explicit-preview-rules = true
+ignore = ["E741", "F541", "F841", "F401", "E731", "E722"]
+extend-select = ["PLR1704"]
```

### Comparing `dflow_galaxy-0.1.7/PKG-INFO` & `dflow_galaxy-0.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: dflow-galaxy
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Author: weihong.xu
 Author-email: xuweihong.cn@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: ai2-kit (==0.16.0)
+Requires-Dist: ai2-kit (==0.18.1)
 Requires-Dist: cp2kdata (>=0.6.6,<0.7.0)
 Requires-Dist: dp-launching-sdk (>=0.12.0,<0.13.0)
 Requires-Dist: dpdispatcher (>=0.6.4,<0.7.0)
 Requires-Dist: lbg (>=1.2.24,<2.0.0)
 Requires-Dist: pydflow (==1.8.60)
 Description-Content-Type: text/markdown
 
@@ -29,15 +29,15 @@
 
 ## Features
 
 ### Tools
 * DFlowBuilder: A type friendly wrapper for `DFlow` to build workflows in a more intuitive way.
 
 ### Workflow
-* TESLA: a **T**raining-**E**xploration-**S**creening-**L**abeling workflow developed by **AI4EC**. Get inspired by [DPGEN](https://github.com/deepmodeling/dpgen), [DPGEN2](https://github.com/deepmodeling/dpgen2), ported from [ai2-kit](https://github.com/chenggroup/ai2-kit).
+* TESLA: a **T**raining-**E**xploration-**S**creening-**L**abeling workflow developed by **AI4EC**. Get inspired by [DPGEN](https://github.com/deepmodeling/dpgen), [DPGEN2](https://github.com/deepmodeling/dpgen2), powered by [ai2-kit](https://github.com/chenggroup/ai2-kit).
 
 ### [Bohrium Apps](https://bohrium.dp.tech/apps)
 Bohrium Apps are cloud native apps that can be run on Bohrium Platform. 
 
 * CP2K Lightning: Run CP2K without building input files from scratch.
 * DynaCat TESLA: An automated workflow to generated DeepMD potential for DynaCat.
 * DynaCat MD: Run MD simulations with DeepMD potential for DynaCat.
```

