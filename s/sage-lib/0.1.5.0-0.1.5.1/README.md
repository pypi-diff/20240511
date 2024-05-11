# Comparing `tmp/sage_lib-0.1.5.0.tar.gz` & `tmp/sage_lib-0.1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sage_lib-0.1.5.0.tar", last modified: Thu May  9 09:43:00 2024, max compression
+gzip compressed data, was "sage_lib-0.1.5.1.tar", last modified: Sat May 11 07:21:27 2024, max compression
```

## Comparing `sage_lib-0.1.5.0.tar` & `sage_lib-0.1.5.1.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-09 09:43:00.910612 sage_lib-0.1.5.0/
--rw-r--r--   0 dimitry    (501) staff       (20)      122 2024-05-09 09:43:00.910410 sage_lib-0.1.5.0/PKG-INFO
--rw-rw-r--   0 dimitry    (501) staff       (20)        7 2023-11-24 15:31:44.000000 sage_lib-0.1.5.0/README.md
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-09 09:43:00.889206 sage_lib-0.1.5.0/sage_lib/
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-09 09:43:00.892930 sage_lib-0.1.5.0/sage_lib/IO/
--rw-rw-r--   0 dimitry    (501) staff       (20)     5213 2023-11-26 10:15:10.000000 sage_lib-0.1.5.0/sage_lib/IO/BashScriptManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     4088 2023-11-26 10:15:54.000000 sage_lib-0.1.5.0/sage_lib/IO/BinaryDataHandler.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     3145 2023-11-26 10:15:38.000000 sage_lib-0.1.5.0/sage_lib/IO/ChargeFileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     6402 2023-11-30 08:47:00.000000 sage_lib-0.1.5.0/sage_lib/IO/DOSManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     9400 2023-11-30 16:58:50.000000 sage_lib-0.1.5.0/sage_lib/IO/EigenvalueFileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)      559 2023-11-26 11:22:04.000000 sage_lib-0.1.5.0/sage_lib/IO/ForceFieldManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     8862 2023-11-30 09:14:10.000000 sage_lib-0.1.5.0/sage_lib/IO/KPointsManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    15441 2024-05-09 06:44:19.000000 sage_lib-0.1.5.0/sage_lib/IO/OutFileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     5292 2023-11-26 10:15:38.000000 sage_lib-0.1.5.0/sage_lib/IO/PROFileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     8151 2023-11-26 10:16:36.000000 sage_lib-0.1.5.0/sage_lib/IO/PotentialManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     2756 2023-11-26 10:15:40.000000 sage_lib-0.1.5.0/sage_lib/IO/WaveFileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.0/sage_lib/IO/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-09 09:43:00.894307 sage_lib-0.1.5.0/sage_lib/IO/input_handling_tools/
--rw-rw-r--   0 dimitry    (501) staff       (20)      609 2024-01-17 11:45:45.000000 sage_lib-0.1.5.0/sage_lib/IO/input_handling_tools/InputClassic.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    24368 2024-01-17 11:45:39.000000 sage_lib-0.1.5.0/sage_lib/IO/input_handling_tools/InputDFT.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     1168 2024-01-17 11:45:21.000000 sage_lib-0.1.5.0/sage_lib/IO/input_handling_tools/InputFile.py
--rw-rw-r--   0 dimitry    (501) staff       (20)      873 2023-11-26 10:17:02.000000 sage_lib-0.1.5.0/sage_lib/IO/input_handling_tools/InputFileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.0/sage_lib/IO/input_handling_tools/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-09 09:43:00.896957 sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/
--rw-rw-r--   0 dimitry    (501) staff       (20)     2622 2024-01-17 11:44:29.000000 sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/AtomPosition.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     4991 2024-01-17 15:22:15.000000 sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/AtomPositionLoader.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     5924 2023-12-29 02:33:08.000000 sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/AtomPositionMaker.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    21571 2024-04-29 15:23:19.000000 sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/AtomPositionManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    47828 2024-04-29 15:23:19.000000 sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/AtomPositionOperator.py
--rw-rw-r--   0 dimitry    (501) staff       (20)      666 2024-01-30 15:22:44.000000 sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/NonPeriodicSystem.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    31224 2024-05-02 06:40:23.000000 sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/PeriodicSystem.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/__init__.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    10187 2024-01-25 08:34:17.000000 sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/plot.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-09 09:43:00.899271 sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/structural_file_readers/
--rw-rw-r--   0 dimitry    (501) staff       (20)     5733 2023-12-12 15:25:04.000000 sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/structural_file_readers/AIMS.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     4702 2023-12-18 08:26:38.000000 sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/structural_file_readers/ASE.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     3458 2023-11-28 08:43:18.000000 sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/structural_file_readers/CIF.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     6036 2024-01-17 16:13:47.000000 sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/structural_file_readers/GEN.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     7960 2024-04-03 12:15:20.000000 sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/structural_file_readers/PDB.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     4892 2024-04-29 15:21:19.000000 sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/structural_file_readers/POSCAR.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     2583 2023-11-28 07:46:02.000000 sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/structural_file_readers/SI.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    12012 2024-04-29 15:28:10.000000 sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/structural_file_readers/XYZ.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/structural_file_readers/__init__.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     5409 2024-01-17 14:07:15.000000 sage_lib-0.1.5.0/sage_lib/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-09 09:43:00.900907 sage_lib-0.1.5.0/sage_lib/descriptor/
--rw-rw-r--   0 dimitry    (501) staff       (20)    22605 2024-01-30 14:35:03.000000 sage_lib-0.1.5.0/sage_lib/descriptor/MBTR.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    12332 2024-01-26 13:40:44.000000 sage_lib-0.1.5.0/sage_lib/descriptor/MDTR_rev.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.0/sage_lib/descriptor/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-09 09:43:00.901687 sage_lib-0.1.5.0/sage_lib/ensemble/
--rw-rw-r--   0 dimitry    (501) staff       (20)      723 2023-11-30 08:05:18.000000 sage_lib-0.1.5.0/sage_lib/ensemble/DFTEnsemble.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     1943 2023-11-30 08:04:04.000000 sage_lib-0.1.5.0/sage_lib/ensemble/FFEnsembleManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.0/sage_lib/ensemble/__init__.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    60962 2024-05-02 06:53:44.000000 sage_lib-0.1.5.0/sage_lib/main.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-09 09:43:00.902971 sage_lib-0.1.5.0/sage_lib/master/
--rw-rw-r--   0 dimitry    (501) staff       (20)    56677 2024-04-03 13:00:04.000000 sage_lib-0.1.5.0/sage_lib/master/AtomicProperties.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    12789 2024-01-17 14:49:37.000000 sage_lib-0.1.5.0/sage_lib/master/FileManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.0/sage_lib/master/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-09 09:43:00.903800 sage_lib-0.1.5.0/sage_lib/miscellaneous/
--rw-rw-r--   0 dimitry    (501) staff       (20)     7176 2024-01-17 14:09:09.000000 sage_lib-0.1.5.0/sage_lib/miscellaneous/BandPathGenerator.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    24192 2024-03-27 14:48:16.000000 sage_lib-0.1.5.0/sage_lib/miscellaneous/MD_tools.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.0/sage_lib/miscellaneous/__init__.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    22279 2024-01-31 09:07:23.000000 sage_lib-0.1.5.0/sage_lib/miscellaneous/periodic_kdtree.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-09 09:43:00.904559 sage_lib-0.1.5.0/sage_lib/partition/
--rw-rw-r--   0 dimitry    (501) staff       (20)    18091 2024-03-31 12:51:40.000000 sage_lib-0.1.5.0/sage_lib/partition/Partition.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    25994 2024-04-29 15:00:22.000000 sage_lib-0.1.5.0/sage_lib/partition/PartitionManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.0/sage_lib/partition/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-09 09:43:00.908903 sage_lib-0.1.5.0/sage_lib/partition/partition_builder/
--rw-rw-r--   0 dimitry    (501) staff       (20)     7189 2024-02-23 12:29:06.000000 sage_lib-0.1.5.0/sage_lib/partition/partition_builder/AbInitioThermodynamics_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     2503 2023-11-26 11:03:08.000000 sage_lib-0.1.5.0/sage_lib/partition/partition_builder/BandStructure_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    24419 2024-04-30 06:33:56.000000 sage_lib-0.1.5.0/sage_lib/partition/partition_builder/Blender_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    11799 2024-04-15 15:59:15.000000 sage_lib-0.1.5.0/sage_lib/partition/partition_builder/Config_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    11764 2024-01-30 14:29:29.000000 sage_lib-0.1.5.0/sage_lib/partition/partition_builder/CrystalDefect_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)      614 2023-11-26 10:15:36.000000 sage_lib-0.1.5.0/sage_lib/partition/partition_builder/Crystal_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     2714 2024-02-28 10:50:31.000000 sage_lib-0.1.5.0/sage_lib/partition/partition_builder/Dataset_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    14023 2024-02-28 09:01:31.000000 sage_lib-0.1.5.0/sage_lib/partition/partition_builder/Filter_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    35233 2024-05-02 11:31:03.000000 sage_lib-0.1.5.0/sage_lib/partition/partition_builder/MolecularDynamic_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    13519 2024-03-15 18:00:18.000000 sage_lib-0.1.5.0/sage_lib/partition/partition_builder/MoleculeCluster_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     3669 2024-01-17 14:10:13.000000 sage_lib-0.1.5.0/sage_lib/partition/partition_builder/Molecule_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     4199 2024-04-02 14:56:25.000000 sage_lib-0.1.5.0/sage_lib/partition/partition_builder/PositionEditor_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    11331 2024-01-17 14:16:35.000000 sage_lib-0.1.5.0/sage_lib/partition/partition_builder/SupercellEmbedding_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     5375 2023-11-26 12:34:42.000000 sage_lib-0.1.5.0/sage_lib/partition/partition_builder/SurfaceStates_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     6358 2024-02-23 08:00:39.000000 sage_lib-0.1.5.0/sage_lib/partition/partition_builder/VacuumStates_builder.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.0/sage_lib/partition/partition_builder/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-09 09:43:00.910049 sage_lib-0.1.5.0/sage_lib/single_run/
--rw-rw-r--   0 dimitry    (501) staff       (20)     6596 2023-11-24 15:31:44.000000 sage_lib-0.1.5.0/sage_lib/single_run/FF_Gap.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     1803 2024-01-17 15:01:44.000000 sage_lib-0.1.5.0/sage_lib/single_run/SingleRun.py
--rw-rw-r--   0 dimitry    (501) staff       (20)    13356 2024-03-12 14:35:36.000000 sage_lib-0.1.5.0/sage_lib/single_run/SingleRunDFT.py
--rw-rw-r--   0 dimitry    (501) staff       (20)     3098 2024-01-17 14:12:18.000000 sage_lib-0.1.5.0/sage_lib/single_run/SingleRunManager.py
--rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.0/sage_lib/single_run/__init__.py
-drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-09 09:43:00.910193 sage_lib-0.1.5.0/sage_lib.egg-info/
--rw-r--r--   0 dimitry    (501) staff       (20)      122 2024-05-09 09:43:00.000000 sage_lib-0.1.5.0/sage_lib.egg-info/PKG-INFO
--rw-rw-r--   0 dimitry    (501) staff       (20)     3657 2024-05-09 09:43:00.000000 sage_lib-0.1.5.0/sage_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 dimitry    (501) staff       (20)        1 2024-05-09 09:43:00.000000 sage_lib-0.1.5.0/sage_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 dimitry    (501) staff       (20)       44 2024-05-09 09:43:00.000000 sage_lib-0.1.5.0/sage_lib.egg-info/entry_points.txt
--rw-rw-r--   0 dimitry    (501) staff       (20)       23 2024-05-09 09:43:00.000000 sage_lib-0.1.5.0/sage_lib.egg-info/requires.txt
--rw-rw-r--   0 dimitry    (501) staff       (20)        9 2024-05-09 09:43:00.000000 sage_lib-0.1.5.0/sage_lib.egg-info/top_level.txt
--rw-r--r--   0 dimitry    (501) staff       (20)       38 2024-05-09 09:43:00.910658 sage_lib-0.1.5.0/setup.cfg
--rw-rw-r--   0 dimitry    (501) staff       (20)      394 2024-05-09 09:42:07.000000 sage_lib-0.1.5.0/setup.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-11 07:21:27.976934 sage_lib-0.1.5.1/
+-rw-r--r--   0 dimitry    (501) staff       (20)      122 2024-05-11 07:21:27.976754 sage_lib-0.1.5.1/PKG-INFO
+-rw-rw-r--   0 dimitry    (501) staff       (20)        7 2023-11-24 15:31:44.000000 sage_lib-0.1.5.1/README.md
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-11 07:21:27.955518 sage_lib-0.1.5.1/sage_lib/
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-11 07:21:27.959659 sage_lib-0.1.5.1/sage_lib/IO/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5213 2023-11-26 10:15:10.000000 sage_lib-0.1.5.1/sage_lib/IO/BashScriptManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     4088 2023-11-26 10:15:54.000000 sage_lib-0.1.5.1/sage_lib/IO/BinaryDataHandler.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     3145 2023-11-26 10:15:38.000000 sage_lib-0.1.5.1/sage_lib/IO/ChargeFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     6402 2023-11-30 08:47:00.000000 sage_lib-0.1.5.1/sage_lib/IO/DOSManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     9400 2023-11-30 16:58:50.000000 sage_lib-0.1.5.1/sage_lib/IO/EigenvalueFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)      559 2023-11-26 11:22:04.000000 sage_lib-0.1.5.1/sage_lib/IO/ForceFieldManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     8862 2023-11-30 09:14:10.000000 sage_lib-0.1.5.1/sage_lib/IO/KPointsManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    17982 2024-05-10 17:27:54.000000 sage_lib-0.1.5.1/sage_lib/IO/OutFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5292 2023-11-26 10:15:38.000000 sage_lib-0.1.5.1/sage_lib/IO/PROFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     8151 2023-11-26 10:16:36.000000 sage_lib-0.1.5.1/sage_lib/IO/PotentialManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     2756 2023-11-26 10:15:40.000000 sage_lib-0.1.5.1/sage_lib/IO/WaveFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.1/sage_lib/IO/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-11 07:21:27.961056 sage_lib-0.1.5.1/sage_lib/IO/input_handling_tools/
+-rw-rw-r--   0 dimitry    (501) staff       (20)      609 2024-01-17 11:45:45.000000 sage_lib-0.1.5.1/sage_lib/IO/input_handling_tools/InputClassic.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    24368 2024-01-17 11:45:39.000000 sage_lib-0.1.5.1/sage_lib/IO/input_handling_tools/InputDFT.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     1168 2024-01-17 11:45:21.000000 sage_lib-0.1.5.1/sage_lib/IO/input_handling_tools/InputFile.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)      873 2023-11-26 10:17:02.000000 sage_lib-0.1.5.1/sage_lib/IO/input_handling_tools/InputFileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.1/sage_lib/IO/input_handling_tools/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-11 07:21:27.963962 sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     2622 2024-01-17 11:44:29.000000 sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/AtomPosition.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     4991 2024-01-17 15:22:15.000000 sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/AtomPositionLoader.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5924 2023-12-29 02:33:08.000000 sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/AtomPositionMaker.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    23500 2024-05-10 17:27:44.000000 sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/AtomPositionManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    47828 2024-04-29 15:23:19.000000 sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/AtomPositionOperator.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)      666 2024-01-30 15:22:44.000000 sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/NonPeriodicSystem.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    31224 2024-05-02 06:40:23.000000 sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/PeriodicSystem.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/__init__.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    10187 2024-01-25 08:34:17.000000 sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/plot.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-11 07:21:27.966535 sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/structural_file_readers/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5733 2023-12-12 15:25:04.000000 sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/structural_file_readers/AIMS.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     4702 2023-12-18 08:26:38.000000 sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/structural_file_readers/ASE.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     3458 2023-11-28 08:43:18.000000 sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/structural_file_readers/CIF.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     6036 2024-01-17 16:13:47.000000 sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/structural_file_readers/GEN.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     7960 2024-04-03 12:15:20.000000 sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/structural_file_readers/PDB.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5298 2024-05-10 17:25:34.000000 sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/structural_file_readers/POSCAR.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     2583 2023-11-28 07:46:02.000000 sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/structural_file_readers/SI.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    12012 2024-04-29 15:28:10.000000 sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/structural_file_readers/XYZ.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/structural_file_readers/__init__.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5409 2024-01-17 14:07:15.000000 sage_lib-0.1.5.1/sage_lib/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-11 07:21:27.967413 sage_lib-0.1.5.1/sage_lib/descriptor/
+-rw-rw-r--   0 dimitry    (501) staff       (20)    22605 2024-01-30 14:35:03.000000 sage_lib-0.1.5.1/sage_lib/descriptor/MBTR.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    12332 2024-01-26 13:40:44.000000 sage_lib-0.1.5.1/sage_lib/descriptor/MDTR_rev.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.1/sage_lib/descriptor/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-11 07:21:27.968091 sage_lib-0.1.5.1/sage_lib/ensemble/
+-rw-rw-r--   0 dimitry    (501) staff       (20)      723 2023-11-30 08:05:18.000000 sage_lib-0.1.5.1/sage_lib/ensemble/DFTEnsemble.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     1943 2023-11-30 08:04:04.000000 sage_lib-0.1.5.1/sage_lib/ensemble/FFEnsembleManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.1/sage_lib/ensemble/__init__.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    60962 2024-05-10 13:07:36.000000 sage_lib-0.1.5.1/sage_lib/main.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-11 07:21:27.969190 sage_lib-0.1.5.1/sage_lib/master/
+-rw-rw-r--   0 dimitry    (501) staff       (20)    56677 2024-04-03 13:00:04.000000 sage_lib-0.1.5.1/sage_lib/master/AtomicProperties.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    12789 2024-01-17 14:49:37.000000 sage_lib-0.1.5.1/sage_lib/master/FileManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.1/sage_lib/master/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-11 07:21:27.970142 sage_lib-0.1.5.1/sage_lib/miscellaneous/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     7176 2024-01-17 14:09:09.000000 sage_lib-0.1.5.1/sage_lib/miscellaneous/BandPathGenerator.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    24192 2024-03-27 14:48:16.000000 sage_lib-0.1.5.1/sage_lib/miscellaneous/MD_tools.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.1/sage_lib/miscellaneous/__init__.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    22279 2024-01-31 09:07:23.000000 sage_lib-0.1.5.1/sage_lib/miscellaneous/periodic_kdtree.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-11 07:21:27.970960 sage_lib-0.1.5.1/sage_lib/partition/
+-rw-rw-r--   0 dimitry    (501) staff       (20)    18091 2024-03-31 12:51:40.000000 sage_lib-0.1.5.1/sage_lib/partition/Partition.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    27088 2024-05-10 17:27:44.000000 sage_lib-0.1.5.1/sage_lib/partition/PartitionManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.1/sage_lib/partition/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-11 07:21:27.975300 sage_lib-0.1.5.1/sage_lib/partition/partition_builder/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     7189 2024-02-23 12:29:06.000000 sage_lib-0.1.5.1/sage_lib/partition/partition_builder/AbInitioThermodynamics_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     2503 2023-11-26 11:03:08.000000 sage_lib-0.1.5.1/sage_lib/partition/partition_builder/BandStructure_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    24419 2024-04-30 06:33:56.000000 sage_lib-0.1.5.1/sage_lib/partition/partition_builder/Blender_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    11799 2024-04-15 15:59:15.000000 sage_lib-0.1.5.1/sage_lib/partition/partition_builder/Config_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    11764 2024-01-30 14:29:29.000000 sage_lib-0.1.5.1/sage_lib/partition/partition_builder/CrystalDefect_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)      614 2023-11-26 10:15:36.000000 sage_lib-0.1.5.1/sage_lib/partition/partition_builder/Crystal_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     2714 2024-02-28 10:50:31.000000 sage_lib-0.1.5.1/sage_lib/partition/partition_builder/Dataset_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    14023 2024-02-28 09:01:31.000000 sage_lib-0.1.5.1/sage_lib/partition/partition_builder/Filter_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    35233 2024-05-02 11:31:03.000000 sage_lib-0.1.5.1/sage_lib/partition/partition_builder/MolecularDynamic_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    13519 2024-03-15 18:00:18.000000 sage_lib-0.1.5.1/sage_lib/partition/partition_builder/MoleculeCluster_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     3669 2024-01-17 14:10:13.000000 sage_lib-0.1.5.1/sage_lib/partition/partition_builder/Molecule_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     4199 2024-04-02 14:56:25.000000 sage_lib-0.1.5.1/sage_lib/partition/partition_builder/PositionEditor_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    11331 2024-01-17 14:16:35.000000 sage_lib-0.1.5.1/sage_lib/partition/partition_builder/SupercellEmbedding_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     5375 2023-11-26 12:34:42.000000 sage_lib-0.1.5.1/sage_lib/partition/partition_builder/SurfaceStates_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     6358 2024-02-23 08:00:39.000000 sage_lib-0.1.5.1/sage_lib/partition/partition_builder/VacuumStates_builder.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.1/sage_lib/partition/partition_builder/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-11 07:21:27.976400 sage_lib-0.1.5.1/sage_lib/single_run/
+-rw-rw-r--   0 dimitry    (501) staff       (20)     6596 2023-11-24 15:31:44.000000 sage_lib-0.1.5.1/sage_lib/single_run/FF_Gap.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     1803 2024-01-17 15:01:44.000000 sage_lib-0.1.5.1/sage_lib/single_run/SingleRun.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)    13356 2024-03-12 14:35:36.000000 sage_lib-0.1.5.1/sage_lib/single_run/SingleRunDFT.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)     3098 2024-01-17 14:12:18.000000 sage_lib-0.1.5.1/sage_lib/single_run/SingleRunManager.py
+-rw-rw-r--   0 dimitry    (501) staff       (20)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.5.1/sage_lib/single_run/__init__.py
+drwxr-xr-x   0 dimitry    (501) staff       (20)        0 2024-05-11 07:21:27.976560 sage_lib-0.1.5.1/sage_lib.egg-info/
+-rw-r--r--   0 dimitry    (501) staff       (20)      122 2024-05-11 07:21:27.000000 sage_lib-0.1.5.1/sage_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 dimitry    (501) staff       (20)     3657 2024-05-11 07:21:27.000000 sage_lib-0.1.5.1/sage_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 dimitry    (501) staff       (20)        1 2024-05-11 07:21:27.000000 sage_lib-0.1.5.1/sage_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 dimitry    (501) staff       (20)       44 2024-05-11 07:21:27.000000 sage_lib-0.1.5.1/sage_lib.egg-info/entry_points.txt
+-rw-rw-r--   0 dimitry    (501) staff       (20)       23 2024-05-11 07:21:27.000000 sage_lib-0.1.5.1/sage_lib.egg-info/requires.txt
+-rw-rw-r--   0 dimitry    (501) staff       (20)        9 2024-05-11 07:21:27.000000 sage_lib-0.1.5.1/sage_lib.egg-info/top_level.txt
+-rw-r--r--   0 dimitry    (501) staff       (20)       38 2024-05-11 07:21:27.976972 sage_lib-0.1.5.1/setup.cfg
+-rw-rw-r--   0 dimitry    (501) staff       (20)      394 2024-05-11 07:21:06.000000 sage_lib-0.1.5.1/setup.py
```

### Comparing `sage_lib-0.1.5.0/sage_lib/IO/BashScriptManager.py` & `sage_lib-0.1.5.1/sage_lib/IO/BashScriptManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/IO/BinaryDataHandler.py` & `sage_lib-0.1.5.1/sage_lib/IO/BinaryDataHandler.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/IO/ChargeFileManager.py` & `sage_lib-0.1.5.1/sage_lib/IO/ChargeFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/IO/DOSManager.py` & `sage_lib-0.1.5.1/sage_lib/IO/DOSManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/IO/EigenvalueFileManager.py` & `sage_lib-0.1.5.1/sage_lib/IO/EigenvalueFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/IO/ForceFieldManager.py` & `sage_lib-0.1.5.1/sage_lib/IO/ForceFieldManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/IO/KPointsManager.py` & `sage_lib-0.1.5.1/sage_lib/IO/KPointsManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/IO/OutFileManager.py` & `sage_lib-0.1.5.1/sage_lib/IO/OutFileManager.py`

 * *Files 15% similar despite different names*

```diff
@@ -103,14 +103,55 @@
                                 'LWAVE', 'LCHARG', 'LVTOT', 'LVHAR', 'LELF', 'LORBIT', 'Dipole corrections', 
                                 'LMONO', 'LDIPOL', 'IDIPOL', 'EPSILON', 'Exchange correlation treatment:', 'GGA', 
                                 'LEXCH', 'VOSKOWN', 'LHFCALC', 'LHFONE', 'AEXX', 'Linear response parameters', 
                                 'LEPSILON', 'LRPA', 'LNABLA', 'LVEL', 'LINTERFAST', 'KINTER', 'CSHIFT', 'OMEGAMAX', 
                                 'DEG_THRESHOLD', 'RTIME', 'Orbital magnetization related:', 'ORBITALMAG', 'LCHIMAG', 'TITEL', 
                                 'DQ','type', 'uniqueAtomLabels', 'NIONS', 'atomCountByType']
 
+        self._dynamical_eigenvalues = None  # IR positions for a finite diference avaluation. Type: FxNx3
+
+        self._dynamical_eigenvector = None  # IR positions for a finite diference avaluation. Type: FxNx3
+        self._dynamical_eigenvector_fractional = None  # IR displacement. Type: np.array or None
+
+        self._dynamical_eigenvector_diff = None  # IR positions for a finite diference avaluation. Type: FxNx3
+        self._dynamical_eigenvector_diff_fractional = None  # IR displacement. Type: np.array or None
+
+    @property
+    def dynamical_eigenvalues(self):
+        """
+
+        """
+        if isinstance(self._dynamical_eigenvalues, list):
+            self._dynamical_eigenvalues = np.array(self._dynamical_eigenvalues, dtype=np.float64)
+            return self._dynamical_eigenvalues
+        else:
+            return self._dynamical_eigenvalues
+
+    @property
+    def dynamical_eigenvector(self):
+        """
+
+        """
+        if isinstance(self._dynamical_eigenvector, list):
+            self._dynamical_eigenvector = np.array(self._dynamical_eigenvector, dtype=np.float64)
+            return self._dynamical_eigenvector
+        else:
+            return self._dynamical_eigenvector
+
+    @property
+    def dynamical_eigenvector_diff(self):
+        """
+
+        """
+        if isinstance(self._dynamical_eigenvector_diff, list):
+            self._dynamical_eigenvector_diff = np.array(self._dynamical_eigenvector_diff, dtype=np.float64)
+            return self._dynamical_eigenvector_diff
+        else:
+            return self._dynamical_eigenvector_diff
+
     def _extract_variables(self, value):
         """
         Extracts variables from a string, recognizing and converting T/F to True/False, 
         and handles numerical and string values accordingly.
 
         Parameters:
         value (str): The string from which variables are to be extracted.
@@ -157,25 +198,27 @@
             initial_j (int): The initial line offset from the current line to start reading data.
             columns_slice (slice, optional): The slice of columns to be extracted from each line.
 
             Returns:
             AtomPosition: The updated AtomPosition object.
             """
             j = initial_j
-            setattr(APM, APM_attribute, [])
+            data = []
             while True:
                 if not lines[i + j].strip():break
                 try:
-                    getattr(APM, APM_attribute).append( list(map(float, lines[i + j].split()))[columns_slice] )
+                    data.append( list(map(float, lines[i + j].split()))[columns_slice] )
                     j += 1
                 except:
                     break
-            setattr(APM, APM_attribute, np.array(getattr(APM, APM_attribute)))
 
-            return APM
+            if isinstance(APM_attribute, str):
+                setattr(APM, APM_attribute, np.array(data) )
+    
+            return data
 
         file_location = file_location if type(file_location) == str else self.file_location
         lines =list(self.read_file(file_location,strip=False))
         
         # Make frequently used methods local
         local_strip = str.strip
         local_split = str.split
@@ -183,15 +226,15 @@
         read_parameters = True
         APM_holder = []
         APM = None 
         uniqueAtomLabels = []
 
         # Precompile regular expressions for faster matching
         param_re = re.compile(r"(\w+)\s*=\s*([^=]+)(?:\s+|$)")
-        keyword_re = re.compile(r'E-fermi|POTCAR|total charge|magnetization|TOTAL-FORCE|energy  without entropy=|Edisp|Ionic step|direct lattice vectors')
+        keyword_re = re.compile(r'E-fermi|POTCAR|total charge|magnetization|TOTAL-FORCE|energy  without entropy=|Edisp|Ionic step|direct lattice vectors|2PiTHz')
         keyword_ion = re.compile(r'E-Ionic step|Iteration')
 
         for i, line in enumerate(lines):
             stripped_line = line.strip()
             line_vec = [x for x in line.strip().split(' ') if x]
             
             if read_parameters:
@@ -253,16 +296,29 @@
 
                 elif 'TOTAL-FORCE' in line: 
                     # Extracting total forces and atom positions
                     _extract_parameter('_total_force', 2, slice(3, None))
                     _extract_parameter('_atomPositions', 2, slice(0, 3))
 
                 elif '2PiTHz' in line: 
-                    # Extracting IR displacement
-                    _extract_parameter('_IRdisplacement', 2, slice(3, None))
+
+                    if not hasattr(self, '_dynamical_eigenvalues') or not isinstance(self._dynamical_eigenvalues, list):
+                        setattr(self, '_dynamical_eigenvalues', [re.findall(r'\d+\.\d+', line)])
+                    else:
+                        self._dynamical_eigenvalues.append( re.findall(r'\d+\.\d+', line) )
+
+                    if not hasattr(self, '_dynamical_eigenvector') or not isinstance(self._dynamical_eigenvector, list):
+                        setattr(self, '_dynamical_eigenvector', [_extract_parameter(None, 2, slice(0, 3))])
+                    else:
+                        self._dynamical_eigenvector.append( _extract_parameter(None, 2, slice(0, 3)) )
+
+                    if not hasattr(self, '_dynamical_eigenvector_diff') or not isinstance(self._dynamical_eigenvector_diff, list):
+                        setattr(self, '_dynamical_eigenvector_diff', [_extract_parameter(None, 2, slice(3, None))] )
+                    else:
+                        self._dynamical_eigenvector_diff.append( _extract_parameter(None, 2, slice(3, None)) ) 
 
         # Append the final APM object if it exists and is not already in APM_holder
         if isinstance(APM, AtomPosition) and not APM in APM_holder: 
             APM_holder.append(APM)
 
         # Updating the instance's AtomPositionManager with the extracted data
         self._AtomPositionManager = APM_holder
@@ -292,15 +348,15 @@
 
         This method is responsible for extracting and setting values like Fermi energy, number of ions, 
         POTCAR information, lattice vectors, etc., based on the content of a given line.
 
         Parameters:
         line_vec (list): The list of words in the current line.
         line (str): The current line being processed.
-        """
+        """         
         if 'E-fermi' in line:
             # Extract and set Fermi energy
             self.E_fermi = float(line_vec[2])
         elif 'NIONS' in line:
             # Extract and set the number of ions
             self.NIONS = int(line_vec[11])
             self._AtomPositionManager[-1]._atomCount = int(line_vec[11])
```

### Comparing `sage_lib-0.1.5.0/sage_lib/IO/PROFileManager.py` & `sage_lib-0.1.5.1/sage_lib/IO/PROFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/IO/PotentialManager.py` & `sage_lib-0.1.5.1/sage_lib/IO/PotentialManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/IO/WaveFileManager.py` & `sage_lib-0.1.5.1/sage_lib/IO/WaveFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/IO/input_handling_tools/InputClassic.py` & `sage_lib-0.1.5.1/sage_lib/IO/input_handling_tools/InputClassic.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/IO/input_handling_tools/InputDFT.py` & `sage_lib-0.1.5.1/sage_lib/IO/input_handling_tools/InputDFT.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/IO/input_handling_tools/InputFile.py` & `sage_lib-0.1.5.1/sage_lib/IO/input_handling_tools/InputFile.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/IO/input_handling_tools/InputFileManager.py` & `sage_lib-0.1.5.1/sage_lib/IO/input_handling_tools/InputFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/AtomPosition.py` & `sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/AtomPosition.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/AtomPositionLoader.py` & `sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/AtomPositionLoader.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/AtomPositionMaker.py` & `sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/AtomPositionMaker.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/AtomPositionManager.py` & `sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/AtomPositionManager.py`

 * *Files 12% similar despite different names*

```diff
@@ -175,15 +175,17 @@
 
         self._magnetization = None  # Magnetization. Type: float or None
         self._total_force = None  # Total force. Type: np.array or None
         self._force = None  # Total force. Type: np.array or None
 
         self._E = None  # Total energy. Type: float or None
         self._Edisp = None  # Dispersion energy. Type: float or None
-        self._IRdisplacement = None  # IR displacement. Type: np.array or None
+
+        self._IR_position = None  # IR positions for a finite diference avaluation. Type: FxNx3
+        self._IR_displacement = None  # IR displacement. Type: np.array or None
 
         self._mass = None # 
         self._mass_list = None # 
 
         self.info_system = {}
         self.info_atoms = {}
         
@@ -456,14 +458,69 @@
         """
         if self._graph_representation is None:
             self._graph_representation = self.find_related_atoms_groups()
             return self._graph_representation
         else:
             return self._graph_representation
 
+    @property
+    def dynamical_eigenvalues(self):
+        """
+
+        """
+        if isinstance(self._dynamical_eigenvalues, list):
+            self._dynamical_eigenvalues = np.array(self._dynamical_eigenvalues, dtype=np.float64)
+            return self._dynamical_eigenvalues
+        else:
+            return self._dynamical_eigenvalues
+
+    @property
+    def dynamical_eigenvector(self):
+        """
+
+        """
+        if isinstance(self._dynamical_eigenvector, list):
+            self._dynamical_eigenvector = np.array(self._dynamical_eigenvector, dtype=np.float64)
+            return self._dynamical_eigenvector
+        else:
+            return self._dynamical_eigenvector
+
+    @property
+    def dynamical_eigenvector_diff(self):
+        """
+
+        """
+        if isinstance(self._dynamical_eigenvector_diff, list):
+            self._dynamical_eigenvector_diff = np.array(self._dynamical_eigenvector_diff, dtype=np.float64)
+            return self._dynamical_eigenvector_diff
+        else:
+            return self._dynamical_eigenvector_diff
+
+    @property
+    def dynamical_eigenvector(self):
+        """
+
+        """
+        if isinstance(self._dynamical_eigenvector, list):
+            self._dynamical_eigenvector = np.array(self._dynamical_eigenvector, dtype=np.float64)
+            return self._dynamical_eigenvector
+        else:
+            return self._dynamical_eigenvector
+
+    @property
+    def dynamical_eigenvector_diff_fractional(self):
+        """
+
+        """
+        if isinstance(self._dynamical_eigenvector_diff_fractional, list):
+            self._dynamical_eigenvector_diff_fractional = np.array(self._dynamical_eigenvector_diff_fractional, dtype=np.float64)
+            return self._dynamical_eigenvector_diff_fractional
+        else:
+            return self._dynamical_eigenvector_diff_fractional
+
     def get_atomic_numbers(self, ):
         return self.atomLabelsList
     
     def get_cell(self, ):
         return self.la
 
     def get_MBTR_representation(self, grid:int=500, get_dev:bool=True):
```

### Comparing `sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/AtomPositionOperator.py` & `sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/AtomPositionOperator.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/NonPeriodicSystem.py` & `sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/NonPeriodicSystem.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/PeriodicSystem.py` & `sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/PeriodicSystem.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/plot.py` & `sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/plot.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/structural_file_readers/AIMS.py` & `sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/structural_file_readers/AIMS.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/structural_file_readers/ASE.py` & `sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/structural_file_readers/ASE.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/structural_file_readers/CIF.py` & `sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/structural_file_readers/CIF.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/structural_file_readers/GEN.py` & `sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/structural_file_readers/GEN.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/structural_file_readers/PDB.py` & `sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/structural_file_readers/PDB.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/structural_file_readers/POSCAR.py` & `sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/structural_file_readers/POSCAR.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     del sys
 
 class POSCAR(FileManager, AtomicProperties):
     def __init__(self, file_location:str=None, name:str=None, **kwargs):
         FileManager.__init__(self, name=name, file_location=file_location)
         AtomicProperties.__init__(self)
 
-    def export_as_POSCAR(self, file_location:str=None, v:bool=False) -> bool:
+    def export_as_POSCAR(self, file_location:str=None, dimer:int=False, v:bool=False) -> bool:
         file_location  = file_location  if not file_location  is None else self.file_location+'POSCAR' if self.file_location is str else self.file_location
 
         self.group_elements_and_positions()
 
         with open(file_location, 'w') as file:
             # Comentario inicial
             file.write(f'POSCAR : JML code \n')
@@ -60,17 +60,22 @@
 
             # Coordenadas atómicas y sus restricciones
             for i, atom in enumerate(self.atomPositions if self.atomCoordinateType[0].capitalize() in ['C', 'K'] else self.atomPositions_fractional):
                 coords = '\t'.join(['{:>18.15f}'.format(n) for n in atom])
                 constr = '\t'.join(['T' if n else 'F' for n in self.atomicConstraints[i]]) if self.selectiveDynamics else ''
                 file.write(f'\t{coords}\t{constr}\n')
 
-            # Comentario final (opcional)
+            # Comentario final (    opcional)
             file.write('Comment_line\n')
+            if not self.dynamical_eigenvector_diff is None: 
+                for i, atom in enumerate(self.dynamical_eigenvector_diff if self.atomCoordinateType[0].capitalize() in ['C', 'K'] else self.dynamical_eigenvector_diff_fractional):
+                    coords = '\t'.join(['{:>18.15f}'.format(n) for n in atom])
+                    file.write(f'\t{coords}\n')
 
+                
     def read_POSCAR(self, file_location:str=None):
         file_location = file_location if type(file_location) == str else self.file_location
         lines = [n for n in self.read_file(file_location) ]
         
         self._comment = lines[0].strip()
         self._scaleFactor = list(map(float, lines[1].strip().split()))
```

### Comparing `sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/structural_file_readers/SI.py` & `sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/structural_file_readers/SI.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/IO/structure_handling_tools/structural_file_readers/XYZ.py` & `sage_lib-0.1.5.1/sage_lib/IO/structure_handling_tools/structural_file_readers/XYZ.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/__init__.py` & `sage_lib-0.1.5.1/sage_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/descriptor/MBTR.py` & `sage_lib-0.1.5.1/sage_lib/descriptor/MBTR.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/descriptor/MDTR_rev.py` & `sage_lib-0.1.5.1/sage_lib/descriptor/MDTR_rev.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/ensemble/DFTEnsemble.py` & `sage_lib-0.1.5.1/sage_lib/ensemble/DFTEnsemble.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/ensemble/FFEnsembleManager.py` & `sage_lib-0.1.5.1/sage_lib/ensemble/FFEnsembleManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/main.py` & `sage_lib-0.1.5.1/sage_lib/main.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/master/AtomicProperties.py` & `sage_lib-0.1.5.1/sage_lib/master/AtomicProperties.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/master/FileManager.py` & `sage_lib-0.1.5.1/sage_lib/master/FileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/miscellaneous/BandPathGenerator.py` & `sage_lib-0.1.5.1/sage_lib/miscellaneous/BandPathGenerator.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/miscellaneous/MD_tools.py` & `sage_lib-0.1.5.1/sage_lib/miscellaneous/MD_tools.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/miscellaneous/periodic_kdtree.py` & `sage_lib-0.1.5.1/sage_lib/miscellaneous/periodic_kdtree.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/partition/Partition.py` & `sage_lib-0.1.5.1/sage_lib/partition/Partition.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/partition/PartitionManager.py` & `sage_lib-0.1.5.1/sage_lib/partition/PartitionManager.py`

 * *Files 3% similar despite different names*

```diff
@@ -418,35 +418,51 @@
 
     def read_OUTCAR(self, file_location:str=None, add_container:bool=True, verbose=False, **kwargs):
         '''
         '''
         OF = OutFileManager(file_location)
         OF.readOUTCAR()
 
-        for APM in OF.AtomPositionManager:
-            SR = SingleRun(file_location)
-            SR._AtomPositionManager = APM
-            SR._InputFileManager = OF.InputFileManager
-            SR._KPointsManager = OF._KPointsManager
-            SR._PotentialManager = OF._PotentialManager
-            if add_container and SR.AtomPositionManager is not None: 
-                self.add_container(container=SR)
+        if not type(OF.dynamical_eigenvector) is None: 
+
+            for dynamical_eigenvalues, dynamical_eigenvector, dynamical_eigenvector_diff in zip(OF.dynamical_eigenvalues, OF.dynamical_eigenvector, OF.dynamical_eigenvector_diff):
+                SR = SingleRun(file_location)   
+                SR._AtomPositionManager = OF.AtomPositionManager[0]
+                SR._AtomPositionManager._atomPositions = dynamical_eigenvector
+                SR._AtomPositionManager._dynamical_eigenvector = dynamical_eigenvector
+                SR._AtomPositionManager._dynamical_eigenvalues = dynamical_eigenvalues
+                SR._AtomPositionManager._dynamical_eigenvector_diff = dynamical_eigenvector_diff
+                SR._InputFileManager = OF.InputFileManager
+                SR._KPointsManager = OF._KPointsManager
+                SR._PotentialManager = OF._PotentialManager
+                if add_container and SR.AtomPositionManager is not None: 
+                    self.add_container(container=SR)
+
+        else:
+            for APM in OF.AtomPositionManager:
+                SR = SingleRun(file_location)
+                SR._AtomPositionManager = APM
+                SR._InputFileManager = OF.InputFileManager
+                SR._KPointsManager = OF._KPointsManager
+                SR._PotentialManager = OF._PotentialManager
+                if add_container and SR.AtomPositionManager is not None: 
+                    self.add_container(container=SR)
 
     def read_vasp_folder(self, file_location:str=None, add_container:bool=True, verbose:bool=False):
         '''
         '''
         file_location = file_location if type(file_location) == str else self.file_location
         SR = SingleRun(file_location)
         SR.readVASPDirectory(file_location)        
         if add_container and SR.AtomPositionManager is not None: 
             self.add_container(container=SR)
 
         return SR
 
-    def export_files(self, file_location:str=None, source:str=None, label:str=None, bond_factor:float=None, verbose:bool=False):
+    def export_files(self, file_location:str=None, source:str=None, label:str=None, bond_factor:float=None, dimer:bool=None, verbose:bool=False):
         """
         Exports files for each container in a specified format.
 
         The function iterates over all containers and exports them according to the specified format.
         In case of an error during export, it logs the error (if verbose is True) and continues with the next container.
 
         Args:
@@ -475,15 +491,15 @@
                 else:
                     self.create_directories_for_path(file_location)
                     
                 # Export based on the specified source format
                 if source.upper() == 'VASP':
                     container.exportVASP(file_location=file_location_edited)
                 elif source.upper() == 'POSCAR':
-                    container.AtomPositionManager.export_as_POSCAR(file_location=file_location_edited + '/POSCAR')
+                    container.AtomPositionManager.export_as_POSCAR(file_location=file_location_edited + '/POSCAR')                        
                 elif source.upper() == 'XYZ':
                     container.AtomPositionManager.export_as_xyz(file_location=file_location + '/config.xyz', save_to_file='a')
                 elif source.upper() == 'PDB':
                     container.AtomPositionManager.export_as_PDB(file_location=file_location_edited + '/structure.pdb', bond_factor=bond_factor)
                 elif source.upper() == 'ASE':
                     container.AtomPositionManager.export_as_ASE(file_location=file_location_edited + '/ase.obj')
                 else:
```

### Comparing `sage_lib-0.1.5.0/sage_lib/partition/partition_builder/AbInitioThermodynamics_builder.py` & `sage_lib-0.1.5.1/sage_lib/partition/partition_builder/AbInitioThermodynamics_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/partition/partition_builder/BandStructure_builder.py` & `sage_lib-0.1.5.1/sage_lib/partition/partition_builder/BandStructure_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/partition/partition_builder/Blender_builder.py` & `sage_lib-0.1.5.1/sage_lib/partition/partition_builder/Blender_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/partition/partition_builder/Config_builder.py` & `sage_lib-0.1.5.1/sage_lib/partition/partition_builder/Config_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/partition/partition_builder/CrystalDefect_builder.py` & `sage_lib-0.1.5.1/sage_lib/partition/partition_builder/CrystalDefect_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/partition/partition_builder/Crystal_builder.py` & `sage_lib-0.1.5.1/sage_lib/partition/partition_builder/Crystal_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/partition/partition_builder/Dataset_builder.py` & `sage_lib-0.1.5.1/sage_lib/partition/partition_builder/Dataset_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/partition/partition_builder/Filter_builder.py` & `sage_lib-0.1.5.1/sage_lib/partition/partition_builder/Filter_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/partition/partition_builder/MolecularDynamic_builder.py` & `sage_lib-0.1.5.1/sage_lib/partition/partition_builder/MolecularDynamic_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/partition/partition_builder/MoleculeCluster_builder.py` & `sage_lib-0.1.5.1/sage_lib/partition/partition_builder/MoleculeCluster_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/partition/partition_builder/Molecule_builder.py` & `sage_lib-0.1.5.1/sage_lib/partition/partition_builder/Molecule_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/partition/partition_builder/PositionEditor_builder.py` & `sage_lib-0.1.5.1/sage_lib/partition/partition_builder/PositionEditor_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/partition/partition_builder/SupercellEmbedding_builder.py` & `sage_lib-0.1.5.1/sage_lib/partition/partition_builder/SupercellEmbedding_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/partition/partition_builder/SurfaceStates_builder.py` & `sage_lib-0.1.5.1/sage_lib/partition/partition_builder/SurfaceStates_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/partition/partition_builder/VacuumStates_builder.py` & `sage_lib-0.1.5.1/sage_lib/partition/partition_builder/VacuumStates_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/single_run/FF_Gap.py` & `sage_lib-0.1.5.1/sage_lib/single_run/FF_Gap.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/single_run/SingleRun.py` & `sage_lib-0.1.5.1/sage_lib/single_run/SingleRun.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/single_run/SingleRunDFT.py` & `sage_lib-0.1.5.1/sage_lib/single_run/SingleRunDFT.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib/single_run/SingleRunManager.py` & `sage_lib-0.1.5.1/sage_lib/single_run/SingleRunManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.5.0/sage_lib.egg-info/SOURCES.txt` & `sage_lib-0.1.5.1/sage_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

