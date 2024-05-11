# Comparing `tmp/probreg-0.3.7.tar.gz` & `tmp/probreg-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "probreg-0.3.7.tar", last modified: Fri Feb 23 12:01:22 2024, max compression
+gzip compressed data, was "probreg-0.3.8.tar", last modified: Sat May 11 06:21:55 2024, max compression
```

## Comparing `probreg-0.3.7.tar` & `probreg-0.3.8.tar`

### file list

```diff
@@ -1,451 +1,451 @@
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.106643 probreg-0.3.7/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1064 2023-12-11 12:34:34.000000 probreg-0.3.7/LICENSE
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      113 2023-12-11 12:34:34.000000 probreg-0.3.7/MANIFEST.in
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     7826 2024-02-23 12:01:22.106643 probreg-0.3.7/PKG-INFO
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6279 2024-02-23 11:59:54.000000 probreg-0.3.7/README.md
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.090643 probreg-0.3.7/probreg/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      151 2023-12-11 12:34:34.000000 probreg-0.3.7/probreg/__init__.py
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     7716 2023-12-11 12:34:34.000000 probreg-0.3.7/probreg/bcpd.py
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     3854 2023-12-11 12:34:34.000000 probreg-0.3.7/probreg/callbacks.py
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.090643 probreg-0.3.7/probreg/cc/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     8238 2023-12-11 12:34:34.000000 probreg-0.3.7/probreg/cc/gmmtree.cc
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1049 2023-12-11 12:34:34.000000 probreg-0.3.7/probreg/cc/gmmtree.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      502 2023-12-11 12:34:34.000000 probreg-0.3.7/probreg/cc/gmmtree_py.cc
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5846 2023-12-11 12:34:34.000000 probreg-0.3.7/probreg/cc/ifgt.cc
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      611 2023-12-11 12:34:34.000000 probreg-0.3.7/probreg/cc/ifgt.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      678 2023-12-11 12:34:34.000000 probreg-0.3.7/probreg/cc/ifgt_py.cc
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4092 2023-12-11 12:34:34.000000 probreg-0.3.7/probreg/cc/kabsch.cc
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      569 2023-12-11 12:34:34.000000 probreg-0.3.7/probreg/cc/kabsch.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      487 2023-12-11 12:34:34.000000 probreg-0.3.7/probreg/cc/kabsch_py.cc
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2445 2023-12-11 12:34:34.000000 probreg-0.3.7/probreg/cc/kcenter_clustering.cc
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      949 2023-12-11 12:34:34.000000 probreg-0.3.7/probreg/cc/kcenter_clustering.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1275 2023-12-11 12:34:34.000000 probreg-0.3.7/probreg/cc/math_utils.cc
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      651 2023-12-11 12:34:34.000000 probreg-0.3.7/probreg/cc/math_utils.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      621 2023-12-11 12:34:34.000000 probreg-0.3.7/probreg/cc/math_utils_py.cc
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1150 2023-12-11 12:34:34.000000 probreg-0.3.7/probreg/cc/permutohedral_lattice_py.cc
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1550 2023-12-11 12:34:34.000000 probreg-0.3.7/probreg/cc/point_to_plane.cc
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      454 2023-12-11 12:34:34.000000 probreg-0.3.7/probreg/cc/point_to_plane.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      457 2023-12-11 12:34:34.000000 probreg-0.3.7/probreg/cc/point_to_plane_py.cc
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      929 2023-12-11 12:34:34.000000 probreg-0.3.7/probreg/cc/types.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     3788 2023-12-11 12:34:34.000000 probreg-0.3.7/probreg/cost_functions.py
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    18097 2024-02-23 11:52:33.000000 probreg-0.3.7/probreg/cpd.py
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1588 2023-12-11 12:34:34.000000 probreg-0.3.7/probreg/cupy_utils.py
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     3043 2023-12-11 12:34:34.000000 probreg-0.3.7/probreg/features.py
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    12913 2023-12-11 12:34:34.000000 probreg-0.3.7/probreg/filterreg.py
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1955 2023-12-11 12:34:34.000000 probreg-0.3.7/probreg/gauss_transform.py
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      479 2023-12-11 12:34:34.000000 probreg-0.3.7/probreg/gaussian_filtering.py
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5011 2023-12-11 12:34:34.000000 probreg-0.3.7/probreg/gmmtree.py
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     8297 2023-12-11 12:34:34.000000 probreg-0.3.7/probreg/l2dist_regs.py
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      126 2023-12-11 12:34:34.000000 probreg-0.3.7/probreg/log.py
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1520 2023-12-11 12:34:34.000000 probreg-0.3.7/probreg/math_utils.py
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4305 2023-12-11 12:34:34.000000 probreg-0.3.7/probreg/se3_op.py
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6484 2023-12-11 12:34:34.000000 probreg-0.3.7/probreg/transformation.py
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)       22 2024-02-23 11:57:33.000000 probreg-0.3.7/probreg/version.py
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.090643 probreg-0.3.7/probreg.egg-info/
--rw-r--r--   0 nekanat   (1000) nekanat   (1000)     7826 2024-02-23 12:01:22.000000 probreg-0.3.7/probreg.egg-info/PKG-INFO
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    19280 2024-02-23 12:01:22.000000 probreg-0.3.7/probreg.egg-info/SOURCES.txt
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)        1 2024-02-23 12:01:22.000000 probreg-0.3.7/probreg.egg-info/dependency_links.txt
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)        1 2024-02-02 07:41:05.000000 probreg-0.3.7/probreg.egg-info/not-zip-safe
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)       68 2024-02-23 12:01:22.000000 probreg-0.3.7/probreg.egg-info/requires.txt
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)        8 2024-02-23 12:01:22.000000 probreg-0.3.7/probreg.egg-info/top_level.txt
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      856 2024-02-23 11:55:46.000000 probreg-0.3.7/pyproject.toml
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)       38 2024-02-23 12:01:22.106643 probreg-0.3.7/setup.cfg
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     8602 2023-12-11 12:34:34.000000 probreg-0.3.7/setup.py
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.090643 probreg-0.3.7/tests/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      971 2023-12-11 12:34:34.000000 probreg-0.3.7/tests/test_cpd.py
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1772 2023-12-11 12:34:34.000000 probreg-0.3.7/tests/test_filterreg.py
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1081 2023-12-11 12:34:34.000000 probreg-0.3.7/tests/test_gauss_transform.py
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      883 2023-12-11 12:34:34.000000 probreg-0.3.7/tests/test_gaussian_filtering.py
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      572 2023-12-11 12:34:34.000000 probreg-0.3.7/tests/test_math_utils.py
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1496 2023-12-11 12:34:34.000000 probreg-0.3.7/tests/test_point_to_plane.py
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      957 2023-12-11 12:34:34.000000 probreg-0.3.7/tests/test_svr.py
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.090643 probreg-0.3.7/third_party/
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.086643 probreg-0.3.7/third_party/eigen/
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.090643 probreg-0.3.7/third_party/eigen/Eigen/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1161 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/Cholesky
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1900 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/CholmodSupport
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    12799 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/Core
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      122 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/Dense
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)       35 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/Eigen
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1777 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/Eigenvalues
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1940 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/Geometry
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      829 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/Householder
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2083 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/IterativeLinearSolvers
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      894 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/Jacobi
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1389 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/KLUSupport
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1268 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/LU
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      991 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/MetisSupport
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2451 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/OrderingMethods
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1751 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/PaStiXSupport
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1116 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/PardisoSupport
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1272 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/QR
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      900 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/QtAlignedMalloc
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1162 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/SPQRSupport
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1584 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/SVD
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      888 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/Sparse
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1235 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/SparseCholesky
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2240 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/SparseCore
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1814 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/SparseLU
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1195 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/SparseQR
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      797 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/StdDeque
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      726 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/StdList
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      803 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/StdVector
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2243 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/SuperLUSupport
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1382 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/UmfPackSupport
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.090643 probreg-0.3.7/third_party/eigen/Eigen/src/
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.090643 probreg-0.3.7/third_party/eigen/Eigen/src/Cholesky/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    24934 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Cholesky/LDLT.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    18760 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Cholesky/LLT.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     3974 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Cholesky/LLT_LAPACKE.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.090643 probreg-0.3.7/third_party/eigen/Eigen/src/CholmodSupport/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    25441 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/CholmodSupport/CholmodSupport.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.094643 probreg-0.3.7/third_party/eigen/Eigen/src/Core/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    19214 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/ArithmeticSequence.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    16782 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/Array.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     8217 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/ArrayBase.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     7018 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/ArrayWrapper.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2738 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/Assign.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    41673 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/AssignEvaluator.h
--rwxrwxr-x   0 nekanat   (1000) nekanat   (1000)    12488 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/Assign_MKL.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    14075 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/BandMatrix.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    18648 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/Block.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4429 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/BooleanRedux.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5981 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/CommaInitializer.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6990 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/ConditionEstimator.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    63841 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/CoreEvaluators.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4745 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/CoreIterators.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     7909 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/CwiseBinaryOp.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    36282 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/CwiseNullaryOp.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     8256 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/CwiseTernaryOp.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     3937 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/CwiseUnaryOp.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5551 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/CwiseUnaryView.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    31529 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/DenseBase.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    24484 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/DenseCoeffsBase.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    25360 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/DenseStorage.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     9870 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/Diagonal.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    14670 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/DiagonalMatrix.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      988 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/DiagonalProduct.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    11654 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/Dot.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5841 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/EigenBase.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4909 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/ForceAlignedAccess.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5759 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/Fuzzy.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    21679 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/GeneralProduct.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    38812 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/GenericPacketMath.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    11543 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/GlobalFunctions.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     8238 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/IO.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     9620 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/IndexedView.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     3503 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/Inverse.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     7256 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/Map.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    11281 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/MapBase.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    60784 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/MathFunctions.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     7156 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/MathFunctionsImpl.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    24343 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/Matrix.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    23856 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/MatrixBase.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2520 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/NestByValue.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     3620 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/NoAlias.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    12884 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/NumTraits.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     9207 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/PartialReduxEvaluator.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    20748 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/PermutationMatrix.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    49193 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/PlainObjectBase.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     7336 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/Product.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    53832 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/ProductEvaluators.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     7756 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/Random.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    19195 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/Redux.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    17821 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/Ref.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5656 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/Replicate.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    17033 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/Reshaped.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4284 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/ReturnByValue.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     7522 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/Reverse.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6143 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/Select.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    14999 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/SelfAdjointView.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1697 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/SelfCwiseBinaryOp.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6837 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/Solve.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     9368 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/SolveTriangular.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6170 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/SolverBase.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     8700 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/StableNorm.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    21641 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/StlIterators.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4212 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/Stride.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2765 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/Swap.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    17606 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/Transpose.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    13567 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/Transpositions.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    38277 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/TriangularMatrix.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     3488 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/VectorBlock.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    35168 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/VectorwiseOp.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    11997 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/Visitor.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.086643 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.094643 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/AVX/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    15223 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/AVX/Complex.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     8102 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/AVX/MathFunctions.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    64608 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/AVX/PacketMath.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2564 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/AVX/TypeCasting.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.094643 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/AVX512/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    17160 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/AVX512/Complex.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    13344 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/AVX512/MathFunctions.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    87891 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/AVX512/PacketMath.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2134 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/AVX512/TypeCasting.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.094643 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/AltiVec/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    16540 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/AltiVec/Complex.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2323 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/AltiVec/MathFunctions.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)   119355 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProduct.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     9490 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    24820 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h
--rwxrwxr-x   0 nekanat   (1000) nekanat   (1000)   102394 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/AltiVec/PacketMath.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.094643 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/CUDA/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    17317 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/CUDA/Complex.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.094643 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/Default/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    26903 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/Default/BFloat16.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5251 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/Default/ConjHelper.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    67696 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     3770 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    35534 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/Default/Half.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1746 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/Default/Settings.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     3746 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/Default/TypeCasting.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.094643 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/GPU/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2695 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/GPU/MathFunctions.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    57047 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/GPU/PacketMath.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2256 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/GPU/TypeCasting.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.086643 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/HIP/
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.094643 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/HIP/hcc/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      691 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/HIP/hcc/math_constants.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.094643 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/MSA/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    17541 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/MSA/Complex.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    16159 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/MSA/MathFunctions.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    33615 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/MSA/PacketMath.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.094643 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/NEON/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    22503 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/NEON/Complex.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6815 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     3083 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/NEON/MathFunctions.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)   189525 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/NEON/PacketMath.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    51286 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/NEON/TypeCasting.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.098643 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/SSE/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    14251 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/SSE/Complex.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6765 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/SSE/MathFunctions.h
--rwxrwxr-x   0 nekanat   (1000) nekanat   (1000)    64465 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/SSE/PacketMath.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     3650 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/SSE/TypeCasting.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.098643 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/SVE/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1194 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/SVE/MathFunctions.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    21200 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/SVE/PacketMath.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1351 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/SVE/TypeCasting.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.098643 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/SYCL/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     7428 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/SYCL/InteropHeaders.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    12539 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/SYCL/MathFunctions.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    27786 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/SYCL/PacketMath.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    21856 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2626 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/SYCL/TypeCasting.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.098643 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/ZVector/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    16728 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/ZVector/Complex.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     8024 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/ZVector/MathFunctions.h
--rwxrwxr-x   0 nekanat   (1000) nekanat   (1000)    36894 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/ZVector/PacketMath.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.098643 probreg-0.3.7/third_party/eigen/Eigen/src/Core/functors/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6686 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/functors/AssignmentFunctors.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    20921 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/functors/BinaryFunctors.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     8334 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/functors/NullaryFunctors.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4998 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/functors/StlFunctors.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      607 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/functors/TernaryFunctors.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    40146 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/functors/UnaryFunctors.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.098643 probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)   108448 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/GeneralBlockPanelKernel.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    20104 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrix.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    15948 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6936 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5106 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    21724 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/GeneralMatrixVector.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6368 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5582 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/Parallelizer.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    21354 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    11570 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     9958 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixVector.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5209 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6164 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/SelfadjointProduct.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4126 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/SelfadjointRank2Update.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    20987 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/TriangularMatrixMatrix.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    13867 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    14722 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/TriangularMatrixVector.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    10571 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    14678 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/TriangularSolverMatrix.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6707 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5882 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/TriangularSolverVector.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.098643 probreg-0.3.7/third_party/eigen/Eigen/src/Core/util/
--rwxrwxr-x   0 nekanat   (1000) nekanat   (1000)    23156 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/util/BlasUtil.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    19876 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/util/ConfigureVectorization.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    21931 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/util/Constants.h
--rwxrwxr-x   0 nekanat   (1000) nekanat   (1000)     4892 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/util/DisableStupidWarnings.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    15555 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/util/ForwardDeclarations.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6696 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/util/IndexedViewHelper.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    10949 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/util/IntegralConstant.h
--rwxrwxr-x   0 nekanat   (1000) nekanat   (1000)     4268 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/util/MKL_support.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    52909 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/util/Macros.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    46661 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/util/Memory.h
--rwxrwxr-x   0 nekanat   (1000) nekanat   (1000)    29336 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/util/Meta.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)       85 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/util/NonMPL2.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1024 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/util/ReenableStupidWarnings.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1432 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/util/ReshapedHelper.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    10676 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/util/StaticAssert.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    12003 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/util/SymbolicIndex.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    35762 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Core/util/XprHelper.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.102643 probreg-0.3.7/third_party/eigen/Eigen/src/Eigenvalues/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    12559 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Eigenvalues/ComplexEigenSolver.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    17274 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Eigenvalues/ComplexSchur.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4178 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    22970 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Eigenvalues/EigenSolver.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    17176 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     9716 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    14349 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Eigenvalues/HessenbergDecomposition.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5575 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    23640 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Eigenvalues/RealQZ.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    21078 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Eigenvalues/RealSchur.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     3650 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    35182 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4104 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    22764 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Eigenvalues/Tridiagonalization.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.102643 probreg-0.3.7/third_party/eigen/Eigen/src/Geometry/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    18939 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Geometry/AlignedBox.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     8403 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Geometry/AngleAxis.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     3624 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Geometry/EulerAngles.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    20726 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Geometry/Homogeneous.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    11962 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Geometry/Hyperplane.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     8955 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Geometry/OrthoMethods.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     9812 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Geometry/ParametrizedLine.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    34367 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Geometry/Quaternion.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6862 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Geometry/Rotation2D.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     8063 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Geometry/RotationBase.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6724 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Geometry/Scaling.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    61930 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Geometry/Transform.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     7664 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Geometry/Translation.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6190 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Geometry/Umeyama.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.102643 probreg-0.3.7/third_party/eigen/Eigen/src/Geometry/arch/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5945 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Geometry/arch/Geometry_SIMD.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.102643 probreg-0.3.7/third_party/eigen/Eigen/src/Householder/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4784 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Householder/BlockHouseholder.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5365 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Householder/Householder.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    23611 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Householder/HouseholderSequence.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.102643 probreg-0.3.7/third_party/eigen/Eigen/src/IterativeLinearSolvers/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6771 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6850 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     8887 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    15036 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    14940 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    13379 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     7349 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4212 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.102643 probreg-0.3.7/third_party/eigen/Eigen/src/Jacobi/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    16383 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/Jacobi/Jacobi.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.102643 probreg-0.3.7/third_party/eigen/Eigen/src/KLUSupport/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    11555 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/KLUSupport/KLUSupport.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.102643 probreg-0.3.7/third_party/eigen/Eigen/src/LU/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     3439 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/LU/Determinant.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    32383 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/LU/FullPivLU.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    15727 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/LU/InverseImpl.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    22069 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/LU/PartialPivLU.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     3555 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/LU/PartialPivLU_LAPACKE.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.102643 probreg-0.3.7/third_party/eigen/Eigen/src/LU/arch/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    13693 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/LU/arch/InverseSize4.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.102643 probreg-0.3.7/third_party/eigen/Eigen/src/MetisSupport/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4588 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/MetisSupport/MetisSupport.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.102643 probreg-0.3.7/third_party/eigen/Eigen/src/OrderingMethods/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    16105 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/OrderingMethods/Amd.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    61681 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/OrderingMethods/Eigen_Colamd.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5248 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/OrderingMethods/Ordering.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.102643 probreg-0.3.7/third_party/eigen/Eigen/src/PaStiXSupport/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    22249 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/PaStiXSupport/PaStiXSupport.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.102643 probreg-0.3.7/third_party/eigen/Eigen/src/PardisoSupport/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    20092 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/PardisoSupport/PardisoSupport.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.102643 probreg-0.3.7/third_party/eigen/Eigen/src/QR/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    25498 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/QR/ColPivHouseholderQR.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4662 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    23429 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/QR/CompleteOrthogonalDecomposition.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    26768 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/QR/FullPivHouseholderQR.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    14641 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/QR/HouseholderQR.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2993 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/QR/HouseholderQR_LAPACKE.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.102643 probreg-0.3.7/third_party/eigen/Eigen/src/SPQRSupport/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    11826 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.102643 probreg-0.3.7/third_party/eigen/Eigen/src/SVD/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    54214 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SVD/BDCSVD.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    32988 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SVD/JacobiSVD.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5099 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SVD/JacobiSVD_LAPACKE.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    14743 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SVD/SVDBase.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    15957 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SVD/UpperBidiagonalization.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.102643 probreg-0.3.7/third_party/eigen/Eigen/src/SparseCholesky/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    24216 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseCholesky/SimplicialCholesky.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5830 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.102643 probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    10670 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/AmbiVector.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     8743 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/CompressedStorage.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    13166 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2191 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/MappedSparseMatrix.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    11368 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseAssign.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    24360 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseBlock.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6485 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseColEtree.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    13606 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseCompressedBase.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    25524 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4757 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    13256 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseDenseProduct.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5808 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseDiagonalProduct.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     3080 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseDot.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1107 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseFuzzy.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    12589 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseMap.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    57475 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseMatrix.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    17451 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseMatrixBase.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     7329 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparsePermutation.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     7593 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseProduct.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1699 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseRedux.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    15600 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseRef.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    25889 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseSelfAdjointView.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4424 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseSolverBase.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     8704 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     3175 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseTranspose.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6437 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseTriangularView.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6827 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseUtil.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    14832 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseVector.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     8127 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseView.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     9657 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/TriangularSolver.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.102643 probreg-0.3.7/third_party/eigen/Eigen/src/SparseLU/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    33316 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseLU/SparseLU.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4303 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseLU/SparseLUImpl.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     7602 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseLU/SparseLU_Memory.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4974 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseLU/SparseLU_Structs.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    12837 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2049 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseLU/SparseLU_Utils.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6712 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseLU/SparseLU_column_bmod.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6584 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseLU/SparseLU_column_dfs.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     3681 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    10217 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4181 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5723 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     8485 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseLU/SparseLU_panel_bmod.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     9028 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseLU/SparseLU_panel_dfs.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4979 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseLU/SparseLU_pivotL.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4545 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseLU/SparseLU_pruneL.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2889 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseLU/SparseLU_relax_snode.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.102643 probreg-0.3.7/third_party/eigen/Eigen/src/SparseQR/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    29167 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SparseQR/SparseQR.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.106643 probreg-0.3.7/third_party/eigen/Eigen/src/StlSupport/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4730 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/StlSupport/StdDeque.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4155 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/StlSupport/StdList.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5338 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/StlSupport/StdVector.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2809 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/StlSupport/details.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.106643 probreg-0.3.7/third_party/eigen/Eigen/src/SuperLUSupport/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    34324 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/SuperLUSupport/SuperLUSupport.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.106643 probreg-0.3.7/third_party/eigen/Eigen/src/UmfPackSupport/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    24456 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/UmfPackSupport/UmfPackSupport.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.106643 probreg-0.3.7/third_party/eigen/Eigen/src/misc/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2913 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/misc/Image.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2742 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/misc/Kernel.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1748 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/misc/RealSvd2x2.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    30560 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/misc/blas.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     7834 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/misc/lapack.h
--rwxrwxr-x   0 nekanat   (1000) nekanat   (1000)  1058369 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/misc/lapacke.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      474 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/misc/lapacke_mangling.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.106643 probreg-0.3.7/third_party/eigen/Eigen/src/plugins/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    14060 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/plugins/ArrayCwiseBinaryOps.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    21431 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/plugins/ArrayCwiseUnaryOps.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    59020 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/plugins/BlockMethods.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4828 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/plugins/CommonCwiseBinaryOps.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6089 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/plugins/CommonCwiseUnaryOps.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    12283 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/plugins/IndexedViewMethods.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6387 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/plugins/MatrixCwiseBinaryOps.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     3350 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/plugins/MatrixCwiseUnaryOps.h
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6915 2023-12-11 12:35:20.000000 probreg-0.3.7/third_party/eigen/Eigen/src/plugins/ReshapedMethods.h
-drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-02-23 12:01:22.106643 probreg-0.3.7/third_party/permutohedral/
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    19166 2023-12-11 12:34:34.000000 probreg-0.3.7/third_party/permutohedral/permutohedral.cpp
--rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2761 2023-12-11 12:34:34.000000 probreg-0.3.7/third_party/permutohedral/permutohedral.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.620782 probreg-0.3.8/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1064 2023-12-11 12:34:34.000000 probreg-0.3.8/LICENSE
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      113 2023-12-11 12:34:34.000000 probreg-0.3.8/MANIFEST.in
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     7910 2024-05-11 06:21:55.620782 probreg-0.3.8/PKG-INFO
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6355 2024-05-11 06:09:08.000000 probreg-0.3.8/README.md
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.604781 probreg-0.3.8/probreg/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      134 2024-05-11 06:07:34.000000 probreg-0.3.8/probreg/__init__.py
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     7713 2024-05-11 06:07:34.000000 probreg-0.3.8/probreg/bcpd.py
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4067 2024-05-11 06:07:34.000000 probreg-0.3.8/probreg/callbacks.py
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.608781 probreg-0.3.8/probreg/cc/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     8247 2024-05-11 06:07:34.000000 probreg-0.3.8/probreg/cc/gmmtree.cc
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1049 2023-12-11 12:34:34.000000 probreg-0.3.8/probreg/cc/gmmtree.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      502 2023-12-11 12:34:34.000000 probreg-0.3.8/probreg/cc/gmmtree_py.cc
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5846 2023-12-11 12:34:34.000000 probreg-0.3.8/probreg/cc/ifgt.cc
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      611 2023-12-11 12:34:34.000000 probreg-0.3.8/probreg/cc/ifgt.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      678 2023-12-11 12:34:34.000000 probreg-0.3.8/probreg/cc/ifgt_py.cc
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4092 2023-12-11 12:34:34.000000 probreg-0.3.8/probreg/cc/kabsch.cc
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      569 2023-12-11 12:34:34.000000 probreg-0.3.8/probreg/cc/kabsch.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      487 2023-12-11 12:34:34.000000 probreg-0.3.8/probreg/cc/kabsch_py.cc
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2445 2023-12-11 12:34:34.000000 probreg-0.3.8/probreg/cc/kcenter_clustering.cc
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      949 2023-12-11 12:34:34.000000 probreg-0.3.8/probreg/cc/kcenter_clustering.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1275 2023-12-11 12:34:34.000000 probreg-0.3.8/probreg/cc/math_utils.cc
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      651 2023-12-11 12:34:34.000000 probreg-0.3.8/probreg/cc/math_utils.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      621 2023-12-11 12:34:34.000000 probreg-0.3.8/probreg/cc/math_utils_py.cc
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1150 2023-12-11 12:34:34.000000 probreg-0.3.8/probreg/cc/permutohedral_lattice_py.cc
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1550 2023-12-11 12:34:34.000000 probreg-0.3.8/probreg/cc/point_to_plane.cc
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      454 2023-12-11 12:34:34.000000 probreg-0.3.8/probreg/cc/point_to_plane.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      457 2023-12-11 12:34:34.000000 probreg-0.3.8/probreg/cc/point_to_plane_py.cc
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      929 2024-05-11 06:09:08.000000 probreg-0.3.8/probreg/cc/types.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     3784 2024-05-11 06:09:08.000000 probreg-0.3.8/probreg/cost_functions.py
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    20797 2024-05-11 06:16:43.000000 probreg-0.3.8/probreg/cpd.py
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1588 2023-12-11 12:34:34.000000 probreg-0.3.8/probreg/cupy_utils.py
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     3041 2024-05-11 06:09:08.000000 probreg-0.3.8/probreg/features.py
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    12913 2024-02-23 12:10:36.000000 probreg-0.3.8/probreg/filterreg.py
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1955 2024-02-23 12:10:36.000000 probreg-0.3.8/probreg/gauss_transform.py
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      479 2024-02-23 12:10:36.000000 probreg-0.3.8/probreg/gaussian_filtering.py
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5011 2024-02-23 12:10:36.000000 probreg-0.3.8/probreg/gmmtree.py
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     8297 2024-05-11 06:09:08.000000 probreg-0.3.8/probreg/l2dist_regs.py
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      126 2023-12-11 12:34:34.000000 probreg-0.3.8/probreg/log.py
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1520 2023-12-11 12:34:34.000000 probreg-0.3.8/probreg/math_utils.py
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4305 2023-12-11 12:34:34.000000 probreg-0.3.8/probreg/se3_op.py
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6694 2024-05-11 06:07:34.000000 probreg-0.3.8/probreg/transformation.py
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)       22 2024-05-11 06:21:37.000000 probreg-0.3.8/probreg/version.py
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.608781 probreg-0.3.8/probreg.egg-info/
+-rw-r--r--   0 nekanat   (1000) nekanat   (1000)     7910 2024-05-11 06:21:55.000000 probreg-0.3.8/probreg.egg-info/PKG-INFO
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    19280 2024-05-11 06:21:55.000000 probreg-0.3.8/probreg.egg-info/SOURCES.txt
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)        1 2024-05-11 06:21:55.000000 probreg-0.3.8/probreg.egg-info/dependency_links.txt
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)        1 2024-02-02 07:41:05.000000 probreg-0.3.8/probreg.egg-info/not-zip-safe
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)       68 2024-05-11 06:21:55.000000 probreg-0.3.8/probreg.egg-info/requires.txt
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)        8 2024-05-11 06:21:55.000000 probreg-0.3.8/probreg.egg-info/top_level.txt
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      862 2024-05-11 06:21:15.000000 probreg-0.3.8/pyproject.toml
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)       38 2024-05-11 06:21:55.620782 probreg-0.3.8/setup.cfg
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     8602 2024-05-11 06:09:08.000000 probreg-0.3.8/setup.py
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.608781 probreg-0.3.8/tests/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      971 2023-12-11 12:34:34.000000 probreg-0.3.8/tests/test_cpd.py
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1772 2023-12-11 12:34:34.000000 probreg-0.3.8/tests/test_filterreg.py
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1081 2023-12-11 12:34:34.000000 probreg-0.3.8/tests/test_gauss_transform.py
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      883 2023-12-11 12:34:34.000000 probreg-0.3.8/tests/test_gaussian_filtering.py
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      572 2023-12-11 12:34:34.000000 probreg-0.3.8/tests/test_math_utils.py
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1496 2023-12-11 12:34:34.000000 probreg-0.3.8/tests/test_point_to_plane.py
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      957 2023-12-11 12:34:34.000000 probreg-0.3.8/tests/test_svr.py
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.604781 probreg-0.3.8/third_party/
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.604781 probreg-0.3.8/third_party/eigen/
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.608781 probreg-0.3.8/third_party/eigen/Eigen/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1161 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/Cholesky
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1900 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/CholmodSupport
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    12799 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/Core
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      122 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/Dense
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)       35 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/Eigen
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1777 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/Eigenvalues
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1940 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/Geometry
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      829 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/Householder
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2083 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/IterativeLinearSolvers
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      894 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/Jacobi
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1389 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/KLUSupport
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1268 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/LU
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      991 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/MetisSupport
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2451 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/OrderingMethods
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1751 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/PaStiXSupport
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1116 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/PardisoSupport
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1272 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/QR
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      900 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/QtAlignedMalloc
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1162 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/SPQRSupport
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1584 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/SVD
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      888 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/Sparse
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1235 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/SparseCholesky
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2240 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/SparseCore
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1814 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/SparseLU
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1195 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/SparseQR
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      797 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/StdDeque
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      726 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/StdList
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      803 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/StdVector
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2243 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/SuperLUSupport
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1382 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/UmfPackSupport
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.604781 probreg-0.3.8/third_party/eigen/Eigen/src/
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.608781 probreg-0.3.8/third_party/eigen/Eigen/src/Cholesky/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    24934 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Cholesky/LDLT.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    18760 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Cholesky/LLT.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     3974 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Cholesky/LLT_LAPACKE.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.608781 probreg-0.3.8/third_party/eigen/Eigen/src/CholmodSupport/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    25441 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/CholmodSupport/CholmodSupport.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.612782 probreg-0.3.8/third_party/eigen/Eigen/src/Core/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    19214 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/ArithmeticSequence.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    16782 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/Array.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     8217 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/ArrayBase.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     7018 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/ArrayWrapper.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2738 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/Assign.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    41673 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/AssignEvaluator.h
+-rwxrwxr-x   0 nekanat   (1000) nekanat   (1000)    12488 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/Assign_MKL.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    14075 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/BandMatrix.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    18648 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/Block.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4429 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/BooleanRedux.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5981 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/CommaInitializer.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6990 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/ConditionEstimator.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    63841 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/CoreEvaluators.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4745 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/CoreIterators.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     7909 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/CwiseBinaryOp.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    36282 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/CwiseNullaryOp.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     8256 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/CwiseTernaryOp.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     3937 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/CwiseUnaryOp.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5551 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/CwiseUnaryView.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    31529 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/DenseBase.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    24484 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/DenseCoeffsBase.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    25360 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/DenseStorage.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     9870 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/Diagonal.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    14670 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/DiagonalMatrix.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      988 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/DiagonalProduct.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    11654 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/Dot.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5841 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/EigenBase.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4909 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/ForceAlignedAccess.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5759 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/Fuzzy.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    21679 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/GeneralProduct.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    38812 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/GenericPacketMath.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    11543 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/GlobalFunctions.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     8238 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/IO.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     9620 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/IndexedView.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     3503 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/Inverse.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     7256 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/Map.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    11281 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/MapBase.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    60784 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/MathFunctions.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     7156 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/MathFunctionsImpl.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    24343 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/Matrix.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    23856 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/MatrixBase.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2520 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/NestByValue.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     3620 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/NoAlias.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    12884 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/NumTraits.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     9207 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/PartialReduxEvaluator.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    20748 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/PermutationMatrix.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    49193 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/PlainObjectBase.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     7336 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/Product.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    53832 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/ProductEvaluators.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     7756 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/Random.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    19195 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/Redux.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    17821 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/Ref.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5656 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/Replicate.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    17033 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/Reshaped.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4284 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/ReturnByValue.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     7522 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/Reverse.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6143 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/Select.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    14999 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/SelfAdjointView.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1697 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/SelfCwiseBinaryOp.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6837 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/Solve.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     9368 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/SolveTriangular.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6170 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/SolverBase.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     8700 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/StableNorm.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    21641 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/StlIterators.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4212 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/Stride.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2765 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/Swap.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    17606 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/Transpose.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    13567 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/Transpositions.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    38277 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/TriangularMatrix.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     3488 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/VectorBlock.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    35168 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/VectorwiseOp.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    11997 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/Visitor.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.604781 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.612782 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/AVX/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    15223 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/AVX/Complex.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     8102 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/AVX/MathFunctions.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    64608 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/AVX/PacketMath.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2564 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/AVX/TypeCasting.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.612782 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/AVX512/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    17160 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/AVX512/Complex.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    13344 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/AVX512/MathFunctions.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    87891 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/AVX512/PacketMath.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2134 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/AVX512/TypeCasting.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.612782 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/AltiVec/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    16540 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/AltiVec/Complex.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2323 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/AltiVec/MathFunctions.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)   119355 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProduct.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     9490 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    24820 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h
+-rwxrwxr-x   0 nekanat   (1000) nekanat   (1000)   102394 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/AltiVec/PacketMath.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.612782 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/CUDA/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    17317 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/CUDA/Complex.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.612782 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/Default/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    26903 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/Default/BFloat16.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5251 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/Default/ConjHelper.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    67696 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     3770 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    35534 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/Default/Half.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1746 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/Default/Settings.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     3746 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/Default/TypeCasting.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.612782 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/GPU/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2695 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/GPU/MathFunctions.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    57047 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/GPU/PacketMath.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2256 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/GPU/TypeCasting.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.604781 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/HIP/
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.612782 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/HIP/hcc/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      691 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/HIP/hcc/math_constants.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.612782 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/MSA/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    17541 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/MSA/Complex.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    16159 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/MSA/MathFunctions.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    33615 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/MSA/PacketMath.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.612782 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/NEON/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    22503 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/NEON/Complex.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6815 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     3083 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/NEON/MathFunctions.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)   189525 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/NEON/PacketMath.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    51286 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/NEON/TypeCasting.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.612782 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/SSE/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    14251 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/SSE/Complex.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6765 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/SSE/MathFunctions.h
+-rwxrwxr-x   0 nekanat   (1000) nekanat   (1000)    64465 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/SSE/PacketMath.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     3650 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/SSE/TypeCasting.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.612782 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/SVE/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1194 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/SVE/MathFunctions.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    21200 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/SVE/PacketMath.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1351 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/SVE/TypeCasting.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.612782 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/SYCL/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     7428 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/SYCL/InteropHeaders.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    12539 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/SYCL/MathFunctions.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    27786 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/SYCL/PacketMath.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    21856 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2626 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/SYCL/TypeCasting.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.612782 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/ZVector/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    16728 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/ZVector/Complex.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     8024 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/ZVector/MathFunctions.h
+-rwxrwxr-x   0 nekanat   (1000) nekanat   (1000)    36894 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/ZVector/PacketMath.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.612782 probreg-0.3.8/third_party/eigen/Eigen/src/Core/functors/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6686 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/functors/AssignmentFunctors.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    20921 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/functors/BinaryFunctors.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     8334 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/functors/NullaryFunctors.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4998 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/functors/StlFunctors.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      607 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/functors/TernaryFunctors.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    40146 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/functors/UnaryFunctors.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.616782 probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)   108448 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/GeneralBlockPanelKernel.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    20104 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrix.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    15948 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6936 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5106 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    21724 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/GeneralMatrixVector.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6368 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5582 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/Parallelizer.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    21354 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    11570 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     9958 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixVector.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5209 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6164 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/SelfadjointProduct.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4126 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/SelfadjointRank2Update.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    20987 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/TriangularMatrixMatrix.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    13867 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    14722 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/TriangularMatrixVector.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    10571 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    14678 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/TriangularSolverMatrix.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6707 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5882 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/TriangularSolverVector.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.616782 probreg-0.3.8/third_party/eigen/Eigen/src/Core/util/
+-rwxrwxr-x   0 nekanat   (1000) nekanat   (1000)    23156 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/util/BlasUtil.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    19876 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/util/ConfigureVectorization.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    21931 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/util/Constants.h
+-rwxrwxr-x   0 nekanat   (1000) nekanat   (1000)     4892 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/util/DisableStupidWarnings.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    15555 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/util/ForwardDeclarations.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6696 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/util/IndexedViewHelper.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    10949 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/util/IntegralConstant.h
+-rwxrwxr-x   0 nekanat   (1000) nekanat   (1000)     4268 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/util/MKL_support.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    52909 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/util/Macros.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    46661 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/util/Memory.h
+-rwxrwxr-x   0 nekanat   (1000) nekanat   (1000)    29336 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/util/Meta.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)       85 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/util/NonMPL2.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1024 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/util/ReenableStupidWarnings.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1432 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/util/ReshapedHelper.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    10676 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/util/StaticAssert.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    12003 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/util/SymbolicIndex.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    35762 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Core/util/XprHelper.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.616782 probreg-0.3.8/third_party/eigen/Eigen/src/Eigenvalues/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    12559 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Eigenvalues/ComplexEigenSolver.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    17274 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Eigenvalues/ComplexSchur.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4178 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    22970 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Eigenvalues/EigenSolver.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    17176 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     9716 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    14349 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Eigenvalues/HessenbergDecomposition.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5575 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    23640 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Eigenvalues/RealQZ.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    21078 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Eigenvalues/RealSchur.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     3650 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    35182 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4104 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    22764 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Eigenvalues/Tridiagonalization.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.616782 probreg-0.3.8/third_party/eigen/Eigen/src/Geometry/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    18939 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Geometry/AlignedBox.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     8403 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Geometry/AngleAxis.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     3624 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Geometry/EulerAngles.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    20726 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Geometry/Homogeneous.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    11962 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Geometry/Hyperplane.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     8955 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Geometry/OrthoMethods.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     9812 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Geometry/ParametrizedLine.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    34367 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Geometry/Quaternion.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6862 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Geometry/Rotation2D.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     8063 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Geometry/RotationBase.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6724 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Geometry/Scaling.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    61930 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Geometry/Transform.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     7664 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Geometry/Translation.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6190 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Geometry/Umeyama.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.616782 probreg-0.3.8/third_party/eigen/Eigen/src/Geometry/arch/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5945 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Geometry/arch/Geometry_SIMD.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.616782 probreg-0.3.8/third_party/eigen/Eigen/src/Householder/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4784 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Householder/BlockHouseholder.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5365 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Householder/Householder.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    23611 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Householder/HouseholderSequence.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.616782 probreg-0.3.8/third_party/eigen/Eigen/src/IterativeLinearSolvers/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6771 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6850 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     8887 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    15036 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    14940 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    13379 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     7349 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4212 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.616782 probreg-0.3.8/third_party/eigen/Eigen/src/Jacobi/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    16383 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/Jacobi/Jacobi.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.616782 probreg-0.3.8/third_party/eigen/Eigen/src/KLUSupport/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    11555 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/KLUSupport/KLUSupport.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.616782 probreg-0.3.8/third_party/eigen/Eigen/src/LU/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     3439 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/LU/Determinant.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    32383 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/LU/FullPivLU.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    15727 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/LU/InverseImpl.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    22069 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/LU/PartialPivLU.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     3555 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/LU/PartialPivLU_LAPACKE.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.616782 probreg-0.3.8/third_party/eigen/Eigen/src/LU/arch/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    13693 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/LU/arch/InverseSize4.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.616782 probreg-0.3.8/third_party/eigen/Eigen/src/MetisSupport/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4588 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/MetisSupport/MetisSupport.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.616782 probreg-0.3.8/third_party/eigen/Eigen/src/OrderingMethods/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    16105 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/OrderingMethods/Amd.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    61681 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/OrderingMethods/Eigen_Colamd.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5248 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/OrderingMethods/Ordering.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.616782 probreg-0.3.8/third_party/eigen/Eigen/src/PaStiXSupport/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    22249 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/PaStiXSupport/PaStiXSupport.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.616782 probreg-0.3.8/third_party/eigen/Eigen/src/PardisoSupport/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    20092 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/PardisoSupport/PardisoSupport.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.616782 probreg-0.3.8/third_party/eigen/Eigen/src/QR/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    25498 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/QR/ColPivHouseholderQR.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4662 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    23429 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/QR/CompleteOrthogonalDecomposition.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    26768 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/QR/FullPivHouseholderQR.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    14641 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/QR/HouseholderQR.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2993 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/QR/HouseholderQR_LAPACKE.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.616782 probreg-0.3.8/third_party/eigen/Eigen/src/SPQRSupport/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    11826 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.620782 probreg-0.3.8/third_party/eigen/Eigen/src/SVD/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    54214 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SVD/BDCSVD.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    32988 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SVD/JacobiSVD.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5099 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SVD/JacobiSVD_LAPACKE.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    14743 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SVD/SVDBase.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    15957 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SVD/UpperBidiagonalization.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.620782 probreg-0.3.8/third_party/eigen/Eigen/src/SparseCholesky/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    24216 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseCholesky/SimplicialCholesky.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5830 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.620782 probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    10670 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/AmbiVector.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     8743 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/CompressedStorage.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    13166 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2191 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/MappedSparseMatrix.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    11368 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseAssign.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    24360 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseBlock.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6485 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseColEtree.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    13606 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseCompressedBase.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    25524 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4757 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    13256 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseDenseProduct.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5808 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseDiagonalProduct.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     3080 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseDot.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1107 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseFuzzy.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    12589 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseMap.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    57475 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseMatrix.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    17451 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseMatrixBase.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     7329 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparsePermutation.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     7593 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseProduct.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1699 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseRedux.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    15600 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseRef.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    25889 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseSelfAdjointView.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4424 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseSolverBase.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     8704 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     3175 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseTranspose.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6437 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseTriangularView.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6827 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseUtil.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    14832 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseVector.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     8127 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseView.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     9657 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/TriangularSolver.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.620782 probreg-0.3.8/third_party/eigen/Eigen/src/SparseLU/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    33316 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseLU/SparseLU.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4303 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseLU/SparseLUImpl.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     7602 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseLU/SparseLU_Memory.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4974 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseLU/SparseLU_Structs.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    12837 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2049 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseLU/SparseLU_Utils.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6712 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseLU/SparseLU_column_bmod.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6584 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseLU/SparseLU_column_dfs.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     3681 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    10217 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4181 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5723 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     8485 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseLU/SparseLU_panel_bmod.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     9028 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseLU/SparseLU_panel_dfs.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4979 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseLU/SparseLU_pivotL.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4545 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseLU/SparseLU_pruneL.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2889 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseLU/SparseLU_relax_snode.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.620782 probreg-0.3.8/third_party/eigen/Eigen/src/SparseQR/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    29167 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SparseQR/SparseQR.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.620782 probreg-0.3.8/third_party/eigen/Eigen/src/StlSupport/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4730 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/StlSupport/StdDeque.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4155 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/StlSupport/StdList.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     5338 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/StlSupport/StdVector.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2809 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/StlSupport/details.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.620782 probreg-0.3.8/third_party/eigen/Eigen/src/SuperLUSupport/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    34324 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/SuperLUSupport/SuperLUSupport.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.620782 probreg-0.3.8/third_party/eigen/Eigen/src/UmfPackSupport/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    24456 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/UmfPackSupport/UmfPackSupport.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.620782 probreg-0.3.8/third_party/eigen/Eigen/src/misc/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2913 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/misc/Image.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2742 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/misc/Kernel.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     1748 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/misc/RealSvd2x2.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    30560 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/misc/blas.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     7834 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/misc/lapack.h
+-rwxrwxr-x   0 nekanat   (1000) nekanat   (1000)  1058369 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/misc/lapacke.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)      474 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/misc/lapacke_mangling.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.620782 probreg-0.3.8/third_party/eigen/Eigen/src/plugins/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    14060 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/plugins/ArrayCwiseBinaryOps.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    21431 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/plugins/ArrayCwiseUnaryOps.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    59020 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/plugins/BlockMethods.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     4828 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/plugins/CommonCwiseBinaryOps.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6089 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/plugins/CommonCwiseUnaryOps.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    12283 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/plugins/IndexedViewMethods.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6387 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/plugins/MatrixCwiseBinaryOps.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     3350 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/plugins/MatrixCwiseUnaryOps.h
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     6915 2023-12-11 12:35:20.000000 probreg-0.3.8/third_party/eigen/Eigen/src/plugins/ReshapedMethods.h
+drwxrwxr-x   0 nekanat   (1000) nekanat   (1000)        0 2024-05-11 06:21:55.620782 probreg-0.3.8/third_party/permutohedral/
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)    19166 2023-12-11 12:34:34.000000 probreg-0.3.8/third_party/permutohedral/permutohedral.cpp
+-rw-rw-r--   0 nekanat   (1000) nekanat   (1000)     2761 2023-12-11 12:34:34.000000 probreg-0.3.8/third_party/permutohedral/permutohedral.h
```

### Comparing `probreg-0.3.7/LICENSE` & `probreg-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/PKG-INFO` & `probreg-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: probreg
-Version: 0.3.7
+Version: 0.3.8
 Summary: Probablistic point cloud resitration algorithms
 Home-page: https://github.com/neka-nat/probreg
 Author: neka-nat
 Author-email: nekanat.stock@gmail.com
 License: UNKNOWN
 Description: # ![logo](https://raw.githubusercontent.com/neka-nat/probreg/master/images/logo.png)
         [![Build status](https://github.com/neka-nat/probreg/actions/workflows/build-and-test.yaml/badge.svg)](https://github.com/neka-nat/probreg/actions/workflows/build-and-test.yaml/badge.svg)
@@ -24,14 +24,15 @@
         * Rigid and non-rigid transformation
         
         ## Algorithms
         
         * Maximum likelihood when the target or source point cloud is observation data
             * [Coherent Point Drift (2010)](https://arxiv.org/pdf/0905.2635.pdf)
             * [Extended Coherent Point Drift (2016)](https://ieeexplore.ieee.org/abstract/document/7477719) (add correspondence priors to CPD)
+            * [Color Coherent Point Drift (2018)](https://arxiv.org/pdf/1802.01516)
             * [FilterReg (CVPR2019)](https://arxiv.org/pdf/1811.10136.pdf)
         * Variational Bayesian inference
             * [Bayesian Coherent Point Drift (2020)](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=8985307)
         * Distance minimization of two probabilistic distributions
             * [GMMReg (2011)](https://ieeexplore.ieee.org/document/5674050)
             * [Support Vector Registration (2015)](https://arxiv.org/pdf/1511.04240.pdf)
         * Hierarchical Stocastic model
```

### Comparing `probreg-0.3.7/README.md` & `probreg-0.3.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 * Rigid and non-rigid transformation
 
 ## Algorithms
 
 * Maximum likelihood when the target or source point cloud is observation data
     * [Coherent Point Drift (2010)](https://arxiv.org/pdf/0905.2635.pdf)
     * [Extended Coherent Point Drift (2016)](https://ieeexplore.ieee.org/abstract/document/7477719) (add correspondence priors to CPD)
+    * [Color Coherent Point Drift (2018)](https://arxiv.org/pdf/1802.01516)
     * [FilterReg (CVPR2019)](https://arxiv.org/pdf/1811.10136.pdf)
 * Variational Bayesian inference
     * [Bayesian Coherent Point Drift (2020)](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=8985307)
 * Distance minimization of two probabilistic distributions
     * [GMMReg (2011)](https://ieeexplore.ieee.org/document/5674050)
     * [Support Vector Registration (2015)](https://arxiv.org/pdf/1511.04240.pdf)
 * Hierarchical Stocastic model
```

### Comparing `probreg-0.3.7/probreg/bcpd.py` & `probreg-0.3.8/probreg/bcpd.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         """Expectation step for BCPD"""
         assert t_source.ndim == 2 and target.ndim == 2, "source and target must have 2 dimensions."
         dim = t_source.shape[1]
         pmat = np.stack([np.sum(np.square(target - ts), axis=1) for ts in t_source])
         pmat = np.exp(-pmat / (2.0 * sigma2))
         pmat /= (2.0 * np.pi * sigma2) ** (dim * 0.5)
         pmat = pmat.T
-        pmat *= np.exp(-(scale ** 2) / (2 * sigma2) * np.diag(sigma_mat) * dim)
+        pmat *= np.exp(-(scale**2) / (2 * sigma2) * np.diag(sigma_mat) * dim)
         pmat *= (1.0 - w) * alpha
         den = w / target.shape[0] + np.sum(pmat, axis=1)
         den[den == 0] = np.finfo(np.float32).eps
         pmat = np.divide(pmat.T, den)
 
         nu_d = np.sum(pmat, axis=0)
         nu = np.sum(pmat, axis=1)
@@ -122,15 +122,15 @@
         )
 
     @staticmethod
     def _maximization_step(source, target, rigid_trans, estep_res, gmat_inv, lmd, k, sigma2_p=None):
         nu_d, nu, n_p, px, x_hat = estep_res
         dim = source.shape[1]
         m = source.shape[0]
-        s2s2 = rigid_trans.scale ** 2 / (sigma2_p ** 2)
+        s2s2 = rigid_trans.scale**2 / (sigma2_p**2)
         sigma_mat_inv = lmd * gmat_inv + s2s2 * np.diag(nu)
         sigma_mat = np.linalg.inv(sigma_mat_inv)
         residual = rigid_trans.inverse().transform(x_hat) - source
         v_hat = s2s2 * np.matmul(
             np.multiply(np.kron(sigma_mat, np.identity(dim)), np.kron(nu, np.ones(dim))), residual.ravel()
         ).reshape(-1, dim)
         u_hat = source + v_hat
@@ -148,15 +148,15 @@
         tr_rsxu = np.trace(np.matmul(rot, s_xu))
         scale = tr_rsxu / np.trace(s_uu)
         t = x_m - scale * np.dot(rot, u_m)
         y_hat = rigid_trans.transform(source + v_hat)
         s1 = np.dot(target.ravel(), np.kron(nu_d, np.ones(dim)) * target.ravel())
         s2 = np.dot(px.ravel(), y_hat.ravel())
         s3 = np.dot(y_hat.ravel(), np.kron(nu, np.ones(dim)) * y_hat.ravel())
-        sigma2 = (s1 - 2.0 * s2 + s3) / (n_p * dim) + scale ** 2 * sigma2_m
+        sigma2 = (s1 - 2.0 * s2 + s3) / (n_p * dim) + scale**2 * sigma2_m
         return MstepResult(tf.CombinedTransformation(rot, t, scale, v_hat), u_hat, sigma_mat, alpha, sigma2)
 
 
 def registration_bcpd(
     source: Union[np.ndarray, o3.geometry.PointCloud],
     target: Union[np.ndarray, o3.geometry.PointCloud],
     w: float = 0.0,
@@ -178,8 +178,8 @@
 
     Returns:
         probreg.Transformation: Estimated transformation.
     """
     cv = lambda x: np.asarray(x.points if isinstance(x, o3.geometry.PointCloud) else x)
     bcpd = CombinedBCPD(cv(source), **kwargs)
     bcpd.set_callbacks(callbacks)
-    return bcpd.registration(cv(target), w, maxiter)
+    return bcpd.registration(cv(target), w, maxiter, tol)
```

### Comparing `probreg-0.3.7/probreg/callbacks.py` & `probreg-0.3.8/probreg/callbacks.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     def asnumpy(x):
         return x
 
 
 from .transformation import Transformation
 
 
-class Plot2DCallback(object):
+class Plot2DCallback:
     """Display the 2D registration result of each iteration.
 
     Args:
         source (numpy.ndarray): Source point cloud data.
         target (numpy.ndarray): Target point cloud data.
         save (bool, optional): If this flag is True,
             each iteration image is saved in a sequential number.
@@ -58,40 +58,48 @@
         if self._save:
             plt.savefig("image_%04d.png" % self._cnt)
         plt.draw()
         plt.pause(0.001)
         self._cnt += 1
 
 
-class Open3dVisualizerCallback(object):
+class Open3dVisualizerCallback:
     """Display the 3D registration result of each iteration.
 
     Args:
-        source (numpy.ndarray): Source point cloud data.
-        target (numpy.ndarray): Target point cloud data.
+        source (open3d.geometry.PointCloud): Source point cloud data.
+        target (open3d.geometry.PointCloud): Target point cloud data.
         save (bool, optional): If this flag is True,
             each iteration image is saved in a sequential number.
         keep_window (bool, optional): If this flag is True,
             the drawing window blocks after registration is finished.
         fov: Field of view (degree).
     """
 
     def __init__(
-        self, source: np.ndarray, target: np.ndarray, save: bool = False, keep_window: bool = True, fov: Any = None
+        self,
+        source: o3.geometry.PointCloud,
+        target: o3.geometry.PointCloud,
+        save: bool = False,
+        keep_window: bool = True,
+        fov: Any = None,
     ):
         self._vis = o3.visualization.Visualizer()
         self._vis.create_window()
         self._source = source
         self._target = target
         self._result = copy.deepcopy(self._source)
         self._save = save
         self._keep_window = keep_window
-        self._source.paint_uniform_color([1, 0, 0])
-        self._target.paint_uniform_color([0, 1, 0])
-        self._result.paint_uniform_color([0, 0, 1])
+        if not self._source.has_colors():
+            self._source.paint_uniform_color([1, 0, 0])
+        if not self._target.has_colors():
+            self._target.paint_uniform_color([0, 1, 0])
+        if not self._result.has_colors():
+            self._result.paint_uniform_color([0, 0, 1])
         self._vis.add_geometry(self._source)
         self._vis.add_geometry(self._target)
         self._vis.add_geometry(self._result)
         if not fov is None:
             ctr = self._vis.get_view_control()
             ctr.change_field_of_view(step=fov)
         self._cnt = 0
```

### Comparing `probreg-0.3.7/probreg/cc/gmmtree.cc` & `probreg-0.3.8/probreg/cc/gmmtree.cc`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 }
 
 Integer child(Integer j) { return (j + 1) * N_NODE; }
 
 Integer level(Integer l) { return N_NODE * (std::pow(N_NODE, l) - 1) / (N_NODE - 1); }
 
 void initializeNodes(NodeParamArray& nodes, const MatrixX3& points, Integer max_tree_level) {
-    const auto idxs = (points.rows() * Vector::Random(max_tree_level * N_NODE)).array().abs().cast<Integer>();
+    const auto idxs = (points.rows() * Vector::Random(std::pow(N_NODE, max_tree_level))).array().abs().cast<Integer>();
     const Integer lf_idx = level(max_tree_level - 1);
     for (Integer j = 0; j < std::pow(N_NODE, max_tree_level); ++j) {
         std::get<0>(nodes[lf_idx + j]) = 1.0 / N_NODE;
         std::get<1>(nodes[lf_idx + j]) = points.row(idxs[j]);
         const MatrixX3 diff = (points.rowwise() - points.row(idxs[j])).matrix();
         std::get<2>(nodes[lf_idx + j]) = diff.transpose() * diff / points.rows();
     }
```

### Comparing `probreg-0.3.7/probreg/cc/gmmtree.h` & `probreg-0.3.8/probreg/cc/gmmtree.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/probreg/cc/ifgt.cc` & `probreg-0.3.8/probreg/cc/ifgt.cc`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/probreg/cc/ifgt.h` & `probreg-0.3.8/probreg/cc/ifgt.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/probreg/cc/ifgt_py.cc` & `probreg-0.3.8/probreg/cc/ifgt_py.cc`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/probreg/cc/kabsch.cc` & `probreg-0.3.8/probreg/cc/kabsch.cc`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/probreg/cc/kabsch.h` & `probreg-0.3.8/probreg/cc/kabsch.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/probreg/cc/kcenter_clustering.cc` & `probreg-0.3.8/probreg/cc/kcenter_clustering.cc`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/probreg/cc/kcenter_clustering.h` & `probreg-0.3.8/probreg/cc/kcenter_clustering.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/probreg/cc/math_utils.cc` & `probreg-0.3.8/probreg/cc/math_utils.cc`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/probreg/cc/math_utils.h` & `probreg-0.3.8/probreg/cc/math_utils.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/probreg/cc/math_utils_py.cc` & `probreg-0.3.8/probreg/cc/math_utils_py.cc`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/probreg/cc/permutohedral_lattice_py.cc` & `probreg-0.3.8/probreg/cc/permutohedral_lattice_py.cc`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/probreg/cc/point_to_plane.cc` & `probreg-0.3.8/probreg/cc/point_to_plane.cc`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/probreg/cc/types.h` & `probreg-0.3.8/probreg/cc/types.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/probreg/cost_functions.py` & `probreg-0.3.8/probreg/cost_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,19 +29,19 @@
     def __call__(self, theta: np.ndarray, *args):
         return None, None
 
 
 def compute_l2_dist(
     mu_source: np.ndarray, phi_source: np.ndarray, mu_target: np.ndarray, phi_target: np.ndarray, sigma: float
 ):
-    z = np.power(2.0 * np.pi * sigma ** 2, mu_source.shape[1] * 0.5)
+    z = np.power(2.0 * np.pi * sigma**2, mu_source.shape[1] * 0.5)
     gtrans = gt.GaussTransform(mu_target, np.sqrt(2.0) * sigma)
     phi_j_e = gtrans.compute(mu_source, phi_target / z)
     phi_mu_j_e = gtrans.compute(mu_source, phi_target * mu_target.T / z).T
-    g = (phi_source * phi_j_e * mu_source.T - phi_source * phi_mu_j_e.T).T / (2.0 * sigma ** 2)
+    g = (phi_source * phi_j_e * mu_source.T - phi_source * phi_mu_j_e.T).T / (2.0 * sigma**2)
     return -np.dot(phi_source, phi_j_e), g
 
 
 class RigidCostFunction(CostFunction):
     def __init__(self):
         self._tf_type = tf.RigidTransformation
```

### Comparing `probreg-0.3.7/probreg/cpd.py` & `probreg-0.3.8/probreg/cpd.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,40 +21,52 @@
     Attributes:
         transformation (tf.Transformation): Transformation from source to target.
         sigma2 (float): Variance of Gaussian distribution.
         q (float): Result of likelihood.
 """
 
 
+class DistModule:
+    def __init__(self, xp):
+        self.xp = xp
+
+    def cdist(self, x1, x2, metric):
+        return self.xp.stack([self.xp.sum(self.xp.square(x2 - ts), axis=1) for ts in x1])
+
+
 @six.add_metaclass(abc.ABCMeta)
 class CoherentPointDrift:
     """Coherent Point Drift algorithm.
     This is an abstract class.
     Based on this class, it is inherited by rigid, affine, nonrigid classes
     according to the type of transformation.
     In this class, Estimation step in EM algorithm is implemented and
     Maximazation step is implemented in the inherited classes.
 
     Args:
         source (numpy.ndarray, optional): Source point cloud data.
+        use_color (bool, optional): Use color information (if available).
         use_cuda (bool, optional): Use CUDA.
     """
 
-    def __init__(self, source: Optional[np.ndarray] = None, use_cuda: bool = False) -> None:
+    _N_DIM = 3
+    _N_COLOR = 3
+
+    def __init__(self, source: Optional[np.ndarray] = None, use_color: bool = False, use_cuda: bool = False) -> None:
         self._source = source
         self._tf_type = None
         self._callbacks = []
+        self._use_color = use_color
         if use_cuda:
             import cupy as cp
-            from cupyx.scipy.spatial import distance as cupy_distance
 
             from . import cupy_utils
 
             self.xp = cp
-            self.distance_module = cupy_distance
+            self.distance_module = DistModule(cp)
             self.cupy_utils = cupy_utils
             self._squared_kernel_sum = cupy_utils.squared_kernel_sum
         else:
             self.xp = np
             self.distance_module = scipy_distance
             self._squared_kernel_sum = mu.squared_kernel_sum
 
@@ -64,56 +76,83 @@
     def set_callbacks(self, callbacks: List[Callable]) -> None:
         self._callbacks.extend(callbacks)
 
     @abc.abstractmethod
     def _initialize(self, target: np.ndarray) -> MstepResult:
         return MstepResult(None, None, None)
 
-    def expectation_step(self, t_source: np.ndarray, target: np.ndarray, sigma2: float, w: float = 0.0) -> EstepResult:
-        """Expectation step for CPD"""
-        assert t_source.ndim == 2 and target.ndim == 2, "source and target must have 2 dimensions."
+    def _compute_pmat_numerator(self, t_source: np.ndarray, target: np.ndarray, sigma2: float) -> np.ndarray:
         pmat = self.distance_module.cdist(t_source, target, "sqeuclidean")
-        # pmat = self.xp.stack([self.xp.sum(self.xp.square(target - ts), axis=1) for ts in t_source])
         pmat = self.xp.exp(-pmat / (2.0 * sigma2))
+        return pmat
+
+    def expectation_step(
+        self,
+        t_source: np.ndarray,
+        target: np.ndarray,
+        sigma2: float,
+        sigma2_c: float,
+        w: float = 0.0,
+    ) -> EstepResult:
+        """Expectation step for CPD"""
+        assert t_source.ndim == 2 and target.ndim == 2, "source and target must have 2 dimensions."
+        pmat = self._compute_pmat_numerator(t_source[:, : self._N_DIM], target[:, : self._N_DIM], sigma2)
 
-        c = (2.0 * np.pi * sigma2) ** (t_source.shape[1] * 0.5)
+        c = (2.0 * np.pi * sigma2) ** (self._N_DIM * 0.5)
         c *= w / (1.0 - w) * t_source.shape[0] / target.shape[0]
         den = self.xp.sum(pmat, axis=0)
         den[den == 0] = self.xp.finfo(np.float32).eps
+        if self._use_color:
+            pmat_c = self._compute_pmat_numerator(t_source[:, self._N_DIM :], target[:, self._N_DIM :], sigma2_c)
+            den_c = self.xp.sum(pmat_c, axis=0)
+            den_c[den_c == 0] = self.xp.finfo(np.float32).eps
+            den = np.multiply(den, den_c)
+            o_c = t_source.shape[0] * (2 * np.pi * sigma2_c) ** (0.5 * (self._N_DIM + self._N_COLOR - 1))
+            o_c *= self.xp.exp(
+                -1.0 / t_source.shape[0] * self.xp.square(self.xp.sum(pmat_c, axis=0)) / (2.0 * sigma2_c)
+            )
+            den += o_c
+            c *= (2.0 * np.pi * sigma2_c) ** (self._N_COLOR * 0.5)
+            pmat = self.xp.multiply(pmat, pmat_c)
         den += c
 
         pmat = self.xp.divide(pmat, den)
         pt1 = self.xp.sum(pmat, axis=0)
         p1 = self.xp.sum(pmat, axis=1)
-        px = self.xp.dot(pmat, target)
+        px = self.xp.dot(pmat, target[:, : self._N_DIM])
         return EstepResult(pt1, p1, px, np.sum(p1))
 
     def maximization_step(
         self, target: np.ndarray, estep_res: EstepResult, sigma2_p: Optional[float] = None
     ) -> Optional[MstepResult]:
-        return self._maximization_step(self._source, target, estep_res, sigma2_p, xp=self.xp)
+        return self._maximization_step(
+            self._source[:, : self._N_DIM], target[:, : self._N_DIM], estep_res, sigma2_p, xp=self.xp
+        )
 
     @staticmethod
     @abc.abstractmethod
     def _maximization_step(
         source: np.ndarray,
         target: np.ndarray,
         estep_res: EstepResult,
         sigma2_p: Optional[float] = None,
         xp: ModuleType = np,
     ) -> Optional[MstepResult]:
         return None
 
     def registration(self, target: np.ndarray, w: float = 0.0, maxiter: int = 50, tol: float = 0.001) -> MstepResult:
         assert not self._tf_type is None, "transformation type is None."
-        res = self._initialize(target)
+        res = self._initialize(target[:, : self._N_DIM])
+        sigma2_c = 0.0
+        if self._use_color:
+            sigma2_c = self._squared_kernel_sum(self._source[:, self._N_DIM :], target[:, self._N_DIM :])
         q = res.q
         for i in range(maxiter):
             t_source = res.transformation.transform(self._source)
-            estep_res = self.expectation_step(t_source, target, res.sigma2, w)
+            estep_res = self.expectation_step(t_source, target, res.sigma2, sigma2_c, w)
             res = self.maximization_step(target, estep_res, res.sigma2)
             for c in self._callbacks:
                 c(res.transformation)
             log.debug("Iteration: {}, Criteria: {}".format(i, res.q))
             if abs(res.q - q) < tol:
                 break
             q = res.q
@@ -123,55 +162,59 @@
 class RigidCPD(CoherentPointDrift):
     """Coherent Point Drift for rigid transformation.
 
     Args:
         source (numpy.ndarray, optional): Source point cloud data.
         update_scale (bool, optional): If this flag is True, compute the scale parameter.
         tf_init_params (dict, optional): Parameters to initialize transformation.
+        use_color (bool, optional): Use color information (if available).
         use_cuda (bool, optional): Use CUDA.
     """
 
     def __init__(
         self,
         source: Optional[np.ndarray] = None,
         update_scale: bool = True,
         tf_init_params: Dict = {},
+        use_color: bool = False,
         use_cuda: bool = False,
     ) -> None:
-        super(RigidCPD, self).__init__(source, use_cuda)
+        super(RigidCPD, self).__init__(source, use_color, use_cuda)
         self._tf_type = tf.RigidTransformation
         self._update_scale = update_scale
         self._tf_init_params = tf_init_params
 
     def _initialize(self, target: np.ndarray) -> MstepResult:
-        dim = self._source.shape[1]
+        dim = self._N_DIM
         sigma2 = self._squared_kernel_sum(self._source, target)
         q = 1.0 + target.shape[0] * dim * 0.5 * np.log(sigma2)
         if len(self._tf_init_params) == 0:
             self._tf_init_params = {"rot": self.xp.identity(dim), "t": self.xp.zeros(dim)}
         if not "xp" in self._tf_init_params:
             self._tf_init_params["xp"] = self.xp
         return MstepResult(self._tf_type(**self._tf_init_params), sigma2, q)
 
     def maximization_step(
         self, target: np.ndarray, estep_res: EstepResult, sigma2_p: Optional[float] = None
     ) -> MstepResult:
-        return self._maximization_step(self._source, target, estep_res, sigma2_p, self._update_scale, self.xp)
+        return self._maximization_step(
+            self._source[:, : self._N_DIM], target[:, : self._N_DIM], estep_res, sigma2_p, self._update_scale, self.xp
+        )
 
     @staticmethod
     def _maximization_step(
         source: np.ndarray,
         target: np.ndarray,
         estep_res: EstepResult,
         sigma2_p: Optional[float] = None,
         update_scale: bool = True,
         xp: ModuleType = np,
     ) -> MstepResult:
         pt1, p1, px, n_p = estep_res
-        dim = source.shape[1]
+        dim = CoherentPointDrift._N_DIM
         mu_x = xp.sum(px, axis=0) / n_p
         mu_y = xp.dot(source.T, p1) / n_p
         target_hat = target - mu_x
         source_hat = source - mu_y
         a = xp.dot(px.T, source_hat) - xp.outer(mu_x, xp.dot(p1.T, source_hat))
         u, _, vh = np.linalg.svd(a, full_matrices=True)
         c = xp.ones(dim)
@@ -183,35 +226,42 @@
         t = mu_x - scale * xp.dot(rot, mu_y)
         tr_xp1x = xp.trace(xp.dot(target_hat.T * pt1, target_hat))
         if update_scale:
             sigma2 = (tr_xp1x - scale * tr_atr) / (n_p * dim)
         else:
             sigma2 = (tr_xp1x + tr_yp1y - scale * tr_atr) / (n_p * dim)
         sigma2 = max(sigma2, np.finfo(np.float32).eps)
-        q = (tr_xp1x - 2.0 * scale * tr_atr + (scale ** 2) * tr_yp1y) / (2.0 * sigma2)
+        q = (tr_xp1x - 2.0 * scale * tr_atr + (scale**2) * tr_yp1y) / (2.0 * sigma2)
         q += dim * n_p * 0.5 * np.log(sigma2)
         return MstepResult(tf.RigidTransformation(rot, t, scale, xp=xp), sigma2, q)
 
 
 class AffineCPD(CoherentPointDrift):
     """Coherent Point Drift for affine transformation.
 
     Args:
         source (numpy.ndarray, optional): Source point cloud data.
         tf_init_params (dict, optional): Parameters to initialize transformation.
+        use_color (bool, optional): Use color information (if available).
         use_cuda (bool, optional): Use CUDA.
     """
 
-    def __init__(self, source: Optional[np.ndarray] = None, tf_init_params: Dict = {}, use_cuda: bool = False) -> None:
-        super(AffineCPD, self).__init__(source, use_cuda)
+    def __init__(
+        self,
+        source: Optional[np.ndarray] = None,
+        tf_init_params: Dict = {},
+        use_color: bool = False,
+        use_cuda: bool = False,
+    ) -> None:
+        super(AffineCPD, self).__init__(source, use_color, use_cuda)
         self._tf_type = tf.AffineTransformation
         self._tf_init_params = tf_init_params
 
     def _initialize(self, target: np.ndarray) -> MstepResult:
-        dim = self._source.shape[1]
+        dim = self._N_DIM
         sigma2 = self._squared_kernel_sum(self._source, target)
         q = 1.0 + target.shape[0] * dim * 0.5 * np.log(sigma2)
         if len(self._tf_init_params) == 0:
             self._tf_init_params = {"b": self.xp.identity(dim), "t": self.xp.zeros(dim)}
         if not "xp" in self._tf_init_params:
             self._tf_init_params["xp"] = self.xp
         return MstepResult(self._tf_type(**self._tf_init_params), sigma2, q)
@@ -221,15 +271,15 @@
         source: np.ndarray,
         target: np.ndarray,
         estep_res: EstepResult,
         sigma2_p: Optional[float] = None,
         xp: ModuleType = np,
     ) -> MstepResult:
         pt1, p1, px, n_p = estep_res
-        dim = source.shape[1]
+        dim = CoherentPointDrift._N_DIM
         mu_x = xp.sum(px, axis=0) / n_p
         mu_y = xp.dot(source.T, p1) / n_p
         target_hat = target - mu_x
         source_hat = source - mu_y
         a = xp.dot(px.T, source_hat) - xp.outer(mu_x, xp.dot(p1.T, source_hat))
         yp1y = xp.dot(source_hat.T * p1, source_hat)
         b = xp.linalg.solve(yp1y.T, a.T).T
@@ -237,49 +287,63 @@
         tr_xp1x = xp.trace(xp.dot(target_hat.T * pt1, target_hat))
         tr_xpyb = xp.trace(xp.dot(a, b.T))
         sigma2 = (tr_xp1x - tr_xpyb) / (n_p * dim)
         tr_ab = xp.trace(xp.dot(a, b.T))
         sigma2 = max(sigma2, np.finfo(np.float32).eps)
         q = (tr_xp1x - 2 * tr_ab + tr_xpyb) / (2.0 * sigma2)
         q += dim * n_p * 0.5 * np.log(sigma2)
-        return MstepResult(tf.AffineTransformation(b, t), sigma2, q)
+        return MstepResult(tf.AffineTransformation(b, t, xp=xp), sigma2, q)
 
 
 class NonRigidCPD(CoherentPointDrift):
     """Coherent Point Drift for nonrigid transformation.
 
     Args:
         source (numpy.ndarray, optional): Source point cloud data.
         beta (float, optional): Parameter of RBF kernel.
         lmd (float, optional): Parameter for regularization term.
+        use_color (bool, optional): Use color information (if available).
         use_cuda (bool, optional): Use CUDA.
     """
 
     def __init__(
-        self, source: Optional[np.ndarray] = None, beta: float = 2.0, lmd: float = 2.0, use_cuda: bool = False
+        self,
+        source: Optional[np.ndarray] = None,
+        beta: float = 2.0,
+        lmd: float = 2.0,
+        use_color: bool = False,
+        use_cuda: bool = False,
     ) -> None:
-        super(NonRigidCPD, self).__init__(source, use_cuda)
+        super(NonRigidCPD, self).__init__(source, use_color, use_cuda)
         self._tf_type = tf.NonRigidTransformation
         self._beta = beta
         self._lmd = lmd
         self._tf_obj = None
         if not self._source is None:
             self._tf_obj = self._tf_type(None, self._source, self._beta, self.xp)
 
     def set_source(self, source: np.ndarray) -> None:
         self._source = source
-        self._tf_obj = self._tf_type(None, self._source, self._beta)
+        self._tf_obj = self._tf_type(None, self._source, self._beta, xp=self.xp)
 
     def maximization_step(
         self, target: np.ndarray, estep_res: EstepResult, sigma2_p: Optional[float] = None
     ) -> MstepResult:
-        return self._maximization_step(self._source, target, estep_res, sigma2_p, self._tf_obj, self._lmd, self.xp)
+        return self._maximization_step(
+            self._source[:, : self._N_DIM],
+            target[:, : self._N_DIM],
+            estep_res,
+            sigma2_p,
+            self._tf_obj,
+            self._lmd,
+            self.xp,
+        )
 
     def _initialize(self, target: np.ndarray) -> MstepResult:
-        dim = self._source.shape[1]
+        dim = self._N_DIM
         sigma2 = self._squared_kernel_sum(self._source, target)
         q = 1.0 + target.shape[0] * dim * 0.5 * np.log(sigma2)
         self._tf_obj.w = self.xp.zeros_like(self._source)
         return MstepResult(self._tf_obj, sigma2, q)
 
     @staticmethod
     def _maximization_step(
@@ -288,15 +352,15 @@
         estep_res: EstepResult,
         sigma2_p: float,
         tf_obj: tf.NonRigidTransformation,
         lmd: float,
         xp: ModuleType = np,
     ) -> MstepResult:
         pt1, p1, px, n_p = estep_res
-        dim = source.shape[1]
+        dim = CoherentPointDrift._N_DIM
         w = xp.linalg.solve((p1 * tf_obj.g).T + lmd * sigma2_p * xp.identity(source.shape[0]), px - (source.T * p1).T)
         t = source + xp.dot(tf_obj.g, w)
         tr_xp1x = xp.trace(xp.dot(target.T * pt1, target))
         tr_pxt = xp.trace(xp.dot(px.T, t))
         tr_tpt = xp.trace(xp.dot(t.T * p1, t))
         sigma2 = (tr_xp1x - 2.0 * tr_pxt + tr_tpt) / (n_p * dim)
         tf_obj.w = w
@@ -312,31 +376,33 @@
     Args:
         source (numpy.ndarray, optional): Source point cloud data.
         beta (float, optional): Parameter of RBF kernel.
         lmd (float, optional): Parameter for regularization term.
         alpha (float): Degree of reliability of priors.
             Approximately between 1e-8 (highly reliable) and 1 (highly unreliable)
         use_cuda (bool, optional): Use CUDA.
+        use_color (bool, optional): Use color information (if available).
         idx_source (numpy.ndarray of ints, optional): Indices in source matrix
             for which a correspondance is known
         idx_target (numpy.ndarray of ints, optional): Indices in target matrix
             for which a correspondance is known
     """
 
     def __init__(
         self,
         source: Optional[np.ndarray] = None,
         beta: float = 2.0,
         lmd: float = 2.0,
         alpha: float = 1e-8,
+        use_color: bool = False,
         use_cuda: bool = False,
         idx_source: Optional[np.ndarray] = None,
         idx_target: Optional[np.ndarray] = None,
     ):
-        super(ConstrainedNonRigidCPD, self).__init__(source, use_cuda)
+        super(ConstrainedNonRigidCPD, self).__init__(source, use_color, use_cuda)
         self._tf_type = tf.NonRigidTransformation
         self._beta = beta
         self._lmd = lmd
         self.alpha = alpha
         self._tf_obj = None
         self.idx_source, self.idx_target = idx_source, idx_target
         if not self._source is None:
@@ -346,28 +412,28 @@
         self._source = source
         self._tf_obj = self._tf_type(None, self._source, self._beta)
 
     def maximization_step(
         self, target: np.ndarray, estep_res: EstepResult, sigma2_p: Optional[float] = None
     ) -> MstepResult:
         return self._maximization_step(
-            self._source,
-            target,
+            self._source[:, : self._N_DIM],
+            target[:, : self._N_DIM],
             estep_res,
             sigma2_p,
             self._tf_obj,
             self._lmd,
             self.alpha,
             self.p1_tilde,
             self.px_tilde,
             self.xp,
         )
 
     def _initialize(self, target: np.ndarray) -> MstepResult:
-        dim = self._source.shape[1]
+        dim = self._N_DIM
         sigma2 = self._squared_kernel_sum(self._source, target)
         q = 1.0 + target.shape[0] * dim * 0.5 * np.log(sigma2)
         self._tf_obj.w = self.xp.zeros_like(self._source)
         self.p_tilde = self.xp.zeros((self._source.shape[0], target.shape[0]))
         if self.idx_source is not None and self.idx_target is not None:
             self.p_tilde[self.idx_source, self.idx_target] = 1
         self.p1_tilde = self.xp.sum(self.p_tilde, axis=1)
@@ -384,15 +450,15 @@
         lmd: float,
         alpha: float,
         p1_tilde: float,
         px_tilde: float,
         xp: ModuleType = np,
     ) -> MstepResult:
         pt1, p1, px, n_p = estep_res
-        dim = source.shape[1]
+        dim = CoherentPointDrift._N_DIM
         w = xp.linalg.solve(
             (p1 * tf_obj.g).T
             + sigma2_p / alpha * (p1_tilde * tf_obj.g).T
             + lmd * sigma2_p * xp.identity(source.shape[0]),
             px - (source.T * p1).T + sigma2_p / alpha * (px_tilde - (source.T * p1_tilde).T),
         )
         t = source + xp.dot(tf_obj.g, w)
@@ -408,28 +474,30 @@
     source: Union[np.ndarray, o3.geometry.PointCloud],
     target: Union[np.ndarray, o3.geometry.PointCloud],
     tf_type_name: str = "rigid",
     w: float = 0.0,
     maxiter: int = 50,
     tol: float = 0.001,
     callbacks: List[Callable] = [],
+    use_color: bool = False,
     use_cuda: bool = False,
     **kwargs: Any,
 ) -> MstepResult:
     """CPD Registraion.
 
     Args:
         source (numpy.ndarray): Source point cloud data.
         target (numpy.ndarray): Target point cloud data.
         tf_type_name (str, optional): Transformation type('rigid', 'affine', 'nonrigid', 'nonrigid_constrained')
         w (float, optional): Weight of the uniform distribution, 0 < `w` < 1.
         maxitr (int, optional): Maximum number of iterations to EM algorithm.
         tol (float, optional): Tolerance for termination.
         callback (:obj:`list` of :obj:`function`, optional): Called after each iteration.
             `callback(probreg.Transformation)`
+        use_color (bool, optional): Use color information (if available).
         use_cuda (bool, optional): Use CUDA.
 
     Keyword Args:
         update_scale (bool, optional): If this flag is true and tf_type is rigid transformation,
             then the scale is treated. The default is true.
         tf_init_params (dict, optional): Parameters to initialize transformation (for rigid or affine).
 
@@ -437,20 +505,29 @@
         MstepResult: Result of the registration (transformation, sigma2, q)
     """
     xp = np
     if use_cuda:
         import cupy as cp
 
         xp = cp
-    cv = lambda x: xp.asarray(x.points if isinstance(x, o3.geometry.PointCloud) else x)
+    if use_color:
+        cv = (
+            lambda x: xp.c_[xp.asarray(x.points), xp.asarray(x.colors)]
+            if isinstance(x, o3.geometry.PointCloud)
+            else xp.asanyarray(x)[:, :6]
+        )
+    else:
+        cv = lambda x: xp.asarray(x.points if isinstance(x, o3.geometry.PointCloud) else x)[
+            :, : CoherentPointDrift._N_DIM
+        ]
     if tf_type_name == "rigid":
-        cpd = RigidCPD(cv(source), use_cuda=use_cuda, **kwargs)
+        cpd = RigidCPD(cv(source), use_color=use_color, use_cuda=use_cuda, **kwargs)
     elif tf_type_name == "affine":
-        cpd = AffineCPD(cv(source), use_cuda=use_cuda, **kwargs)
+        cpd = AffineCPD(cv(source), use_color=use_color, use_cuda=use_cuda, **kwargs)
     elif tf_type_name == "nonrigid":
-        cpd = NonRigidCPD(cv(source), use_cuda=use_cuda, **kwargs)
+        cpd = NonRigidCPD(cv(source), use_color=use_color, use_cuda=use_cuda, **kwargs)
     elif tf_type_name == "nonrigid_constrained":
-        cpd = ConstrainedNonRigidCPD(cv(source), use_cuda=use_cuda, **kwargs)
+        cpd = ConstrainedNonRigidCPD(cv(source), use_color=use_color, use_cuda=use_cuda, **kwargs)
     else:
         raise ValueError("Unknown transformation type %s" % tf_type_name)
     cpd.set_callbacks(callbacks)
     return cpd.registration(cv(target), w, maxiter, tol)
```

### Comparing `probreg-0.3.7/probreg/cupy_utils.py` & `probreg-0.3.8/probreg/cupy_utils.py`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/probreg/features.py` & `probreg-0.3.8/probreg/features.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,12 +89,12 @@
         self._delta = delta
 
     def init(self):
         self._clf = svm.OneClassSVM(nu=self._nu, kernel="rbf", gamma=self._gamma)
 
     def compute(self, data: np.ndarray):
         self._clf.fit(data)
-        z = np.power(2.0 * np.pi * self._sigma ** 2, self._dim * 0.5)
+        z = np.power(2.0 * np.pi * self._sigma**2, self._dim * 0.5)
         return self._clf.support_vectors_, self._clf.dual_coef_[0] * z
 
     def annealing(self):
         self._gamma *= self._delta
```

### Comparing `probreg-0.3.7/probreg/filterreg.py` & `probreg-0.3.8/probreg/filterreg.py`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/probreg/gauss_transform.py` & `probreg-0.3.8/probreg/gauss_transform.py`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/probreg/gmmtree.py` & `probreg-0.3.8/probreg/gmmtree.py`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/probreg/l2dist_regs.py` & `probreg-0.3.8/probreg/l2dist_regs.py`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/probreg/math_utils.py` & `probreg-0.3.8/probreg/math_utils.py`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/probreg/se3_op.py` & `probreg-0.3.8/probreg/se3_op.py`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/probreg/transformation.py` & `probreg-0.3.8/probreg/transformation.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,16 +18,22 @@
 @six.add_metaclass(abc.ABCMeta)
 class Transformation:
     def __init__(self, xp=np):
         self.xp = xp
 
     def transform(self, points, array_type=o3.utility.Vector3dVector):
         if isinstance(points, array_type):
-            return array_type(self._transform(self.xp.asarray(points)))
-        return self._transform(points)
+            _array_after_transform = self._transform(self.xp.asarray(points))
+
+            if self.xp.__name__ == "cupy":
+                _array_after_transform = _array_after_transform.get()
+
+            return array_type(_array_after_transform)
+
+        return self.xp.c_[self._transform(points[:, :3]), points[:, 3:]]
 
     @abc.abstractmethod
     def _transform(self, points):
         return points
 
 
 class RigidTransformation(Transformation):
```

### Comparing `probreg-0.3.7/probreg.egg-info/PKG-INFO` & `probreg-0.3.8/probreg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: probreg
-Version: 0.3.7
+Version: 0.3.8
 Summary: Probablistic point cloud resitration algorithms
 Home-page: https://github.com/neka-nat/probreg
 Author: neka-nat
 Author-email: nekanat.stock@gmail.com
 License: UNKNOWN
 Description: # ![logo](https://raw.githubusercontent.com/neka-nat/probreg/master/images/logo.png)
         [![Build status](https://github.com/neka-nat/probreg/actions/workflows/build-and-test.yaml/badge.svg)](https://github.com/neka-nat/probreg/actions/workflows/build-and-test.yaml/badge.svg)
@@ -24,14 +24,15 @@
         * Rigid and non-rigid transformation
         
         ## Algorithms
         
         * Maximum likelihood when the target or source point cloud is observation data
             * [Coherent Point Drift (2010)](https://arxiv.org/pdf/0905.2635.pdf)
             * [Extended Coherent Point Drift (2016)](https://ieeexplore.ieee.org/abstract/document/7477719) (add correspondence priors to CPD)
+            * [Color Coherent Point Drift (2018)](https://arxiv.org/pdf/1802.01516)
             * [FilterReg (CVPR2019)](https://arxiv.org/pdf/1811.10136.pdf)
         * Variational Bayesian inference
             * [Bayesian Coherent Point Drift (2020)](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=8985307)
         * Distance minimization of two probabilistic distributions
             * [GMMReg (2011)](https://ieeexplore.ieee.org/document/5674050)
             * [Support Vector Registration (2015)](https://arxiv.org/pdf/1511.04240.pdf)
         * Hierarchical Stocastic model
```

### Comparing `probreg-0.3.7/probreg.egg-info/SOURCES.txt` & `probreg-0.3.8/probreg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/pyproject.toml` & `probreg-0.3.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [tool.poetry]
 name = "probreg"
-version = "0.3.7"
+version = "0.3.8"
 description = "Probablistic point cloud resitration algorithms"
 authors = ["nekanat <nekanat.stock@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0"
+python = ">=3.9,<4.0"
 pybind11 = "^2.6.2"
 six = "^1.15.0"
 scipy = "^1.6.0"
-transforms3d = "^0.3.1"
+transforms3d = "^0.4.0"
 scikit-learn = "^1.0"
 matplotlib = "^3.3.3"
 open3d = "0.18.0"
 dq3d = {version = "^0.3.6", optional = true}
-cupy = {version = "^9.5.0", optional = true}
+cupy = {version = "^12.0.0", optional = true}
 pyyaml = "^6.0"
 addict = "^2.4.0"
 pandas = "^2.0.0"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 Sphinx = "^3.4.3"
 flake8 = "^3.8.4"
 sphinx-rtd-theme = "^0.5.1"
 twine = "^3.3.0"
 setuptools = "^52.0.0"
 isort = "^5.9.3"
-black = "^21.9b0"
+black = "22.3.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "setuptools", "pybind11"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry.extras]
 experimental = ["dq3d"]
```

### Comparing `probreg-0.3.7/setup.py` & `probreg-0.3.8/setup.py`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/tests/test_cpd.py` & `probreg-0.3.8/tests/test_cpd.py`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/tests/test_filterreg.py` & `probreg-0.3.8/tests/test_filterreg.py`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/tests/test_gauss_transform.py` & `probreg-0.3.8/tests/test_gauss_transform.py`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/tests/test_gaussian_filtering.py` & `probreg-0.3.8/tests/test_gaussian_filtering.py`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/tests/test_math_utils.py` & `probreg-0.3.8/tests/test_math_utils.py`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/tests/test_point_to_plane.py` & `probreg-0.3.8/tests/test_point_to_plane.py`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/tests/test_svr.py` & `probreg-0.3.8/tests/test_svr.py`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/Cholesky` & `probreg-0.3.8/third_party/eigen/Eigen/Cholesky`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/CholmodSupport` & `probreg-0.3.8/third_party/eigen/Eigen/CholmodSupport`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/Core` & `probreg-0.3.8/third_party/eigen/Eigen/Core`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/Eigenvalues` & `probreg-0.3.8/third_party/eigen/Eigen/Eigenvalues`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/Geometry` & `probreg-0.3.8/third_party/eigen/Eigen/Geometry`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/Householder` & `probreg-0.3.8/third_party/eigen/Eigen/Householder`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/IterativeLinearSolvers` & `probreg-0.3.8/third_party/eigen/Eigen/IterativeLinearSolvers`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/Jacobi` & `probreg-0.3.8/third_party/eigen/Eigen/Jacobi`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/KLUSupport` & `probreg-0.3.8/third_party/eigen/Eigen/KLUSupport`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/LU` & `probreg-0.3.8/third_party/eigen/Eigen/LU`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/MetisSupport` & `probreg-0.3.8/third_party/eigen/Eigen/MetisSupport`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/OrderingMethods` & `probreg-0.3.8/third_party/eigen/Eigen/OrderingMethods`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/PaStiXSupport` & `probreg-0.3.8/third_party/eigen/Eigen/PaStiXSupport`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/PardisoSupport` & `probreg-0.3.8/third_party/eigen/Eigen/PardisoSupport`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/QR` & `probreg-0.3.8/third_party/eigen/Eigen/QR`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/QtAlignedMalloc` & `probreg-0.3.8/third_party/eigen/Eigen/QtAlignedMalloc`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/SPQRSupport` & `probreg-0.3.8/third_party/eigen/Eigen/SPQRSupport`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/SVD` & `probreg-0.3.8/third_party/eigen/Eigen/SVD`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/Sparse` & `probreg-0.3.8/third_party/eigen/Eigen/Sparse`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/SparseCholesky` & `probreg-0.3.8/third_party/eigen/Eigen/SparseCholesky`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/SparseCore` & `probreg-0.3.8/third_party/eigen/Eigen/SparseCore`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/SparseLU` & `probreg-0.3.8/third_party/eigen/Eigen/SparseLU`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/SparseQR` & `probreg-0.3.8/third_party/eigen/Eigen/SparseQR`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/StdDeque` & `probreg-0.3.8/third_party/eigen/Eigen/StdDeque`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/StdList` & `probreg-0.3.8/third_party/eigen/Eigen/StdList`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/StdVector` & `probreg-0.3.8/third_party/eigen/Eigen/StdVector`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/SuperLUSupport` & `probreg-0.3.8/third_party/eigen/Eigen/SuperLUSupport`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/UmfPackSupport` & `probreg-0.3.8/third_party/eigen/Eigen/UmfPackSupport`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Cholesky/LDLT.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Cholesky/LDLT.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Cholesky/LLT.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Cholesky/LLT.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Cholesky/LLT_LAPACKE.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Cholesky/LLT_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/CholmodSupport/CholmodSupport.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/CholmodSupport/CholmodSupport.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/ArithmeticSequence.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/ArithmeticSequence.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/Array.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/Array.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/ArrayBase.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/ArrayBase.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/ArrayWrapper.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/ArrayWrapper.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/Assign.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/Assign.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/AssignEvaluator.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/AssignEvaluator.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/Assign_MKL.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/Assign_MKL.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/BandMatrix.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/BandMatrix.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/Block.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/Block.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/BooleanRedux.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/BooleanRedux.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/CommaInitializer.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/CommaInitializer.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/ConditionEstimator.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/ConditionEstimator.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/CoreEvaluators.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/CoreEvaluators.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/CoreIterators.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/CoreIterators.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/CwiseBinaryOp.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/CwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/CwiseNullaryOp.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/CwiseNullaryOp.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/CwiseTernaryOp.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/CwiseTernaryOp.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/CwiseUnaryOp.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/CwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/CwiseUnaryView.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/CwiseUnaryView.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/DenseBase.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/DenseBase.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/DenseCoeffsBase.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/DenseCoeffsBase.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/DenseStorage.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/DenseStorage.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/Diagonal.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/Diagonal.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/DiagonalMatrix.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/DiagonalMatrix.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/DiagonalProduct.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/DiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/Dot.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/Dot.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/EigenBase.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/EigenBase.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/ForceAlignedAccess.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/ForceAlignedAccess.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/Fuzzy.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/Fuzzy.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/GeneralProduct.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/GeneralProduct.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/GenericPacketMath.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/GenericPacketMath.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/GlobalFunctions.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/GlobalFunctions.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/IO.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/IO.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/IndexedView.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/IndexedView.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/Inverse.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/Inverse.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/Map.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/Map.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/MapBase.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/MapBase.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/MathFunctions.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/MathFunctionsImpl.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/MathFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/Matrix.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/Matrix.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/MatrixBase.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/MatrixBase.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/NestByValue.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/NestByValue.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/NoAlias.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/NoAlias.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/NumTraits.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/NumTraits.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/PartialReduxEvaluator.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/PartialReduxEvaluator.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/PermutationMatrix.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/PermutationMatrix.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/PlainObjectBase.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/PlainObjectBase.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/Product.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/Product.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/ProductEvaluators.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/ProductEvaluators.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/Random.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/Random.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/Redux.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/Redux.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/Ref.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/Ref.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/Replicate.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/Replicate.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/Reshaped.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/Reshaped.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/ReturnByValue.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/ReturnByValue.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/Reverse.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/Reverse.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/Select.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/Select.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/SelfAdjointView.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/SelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/SelfCwiseBinaryOp.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/SelfCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/Solve.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/Solve.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/SolveTriangular.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/SolveTriangular.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/SolverBase.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/SolverBase.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/StableNorm.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/StableNorm.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/StlIterators.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/StlIterators.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/Stride.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/Stride.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/Swap.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/Swap.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/Transpose.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/Transpose.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/Transpositions.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/Transpositions.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/TriangularMatrix.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/TriangularMatrix.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/VectorBlock.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/VectorBlock.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/VectorwiseOp.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/VectorwiseOp.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/Visitor.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/Visitor.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/AVX/Complex.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/AVX/Complex.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/AVX/MathFunctions.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/AVX/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/AVX/PacketMath.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/AVX/PacketMath.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/AVX/TypeCasting.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/AVX/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/AVX512/Complex.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/AVX512/Complex.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/AVX512/MathFunctions.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/AVX512/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/AVX512/PacketMath.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/AVX512/PacketMath.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/AVX512/TypeCasting.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/AVX512/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/AltiVec/Complex.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/AltiVec/Complex.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/AltiVec/MathFunctions.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/AltiVec/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProduct.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProduct.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/AltiVec/PacketMath.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/AltiVec/PacketMath.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/CUDA/Complex.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/CUDA/Complex.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/Default/BFloat16.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/Default/BFloat16.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/Default/ConjHelper.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/Default/ConjHelper.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/Default/Half.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/Default/Half.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/Default/Settings.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/Default/Settings.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/Default/TypeCasting.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/Default/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/GPU/MathFunctions.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/GPU/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/GPU/PacketMath.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/GPU/PacketMath.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/GPU/TypeCasting.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/GPU/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/HIP/hcc/math_constants.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/HIP/hcc/math_constants.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/MSA/Complex.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/MSA/Complex.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/MSA/MathFunctions.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/MSA/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/MSA/PacketMath.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/MSA/PacketMath.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/NEON/Complex.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/NEON/Complex.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/NEON/MathFunctions.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/NEON/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/NEON/PacketMath.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/NEON/PacketMath.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/NEON/TypeCasting.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/NEON/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/SSE/Complex.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/SSE/Complex.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/SSE/MathFunctions.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/SSE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/SSE/PacketMath.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/SSE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/SSE/TypeCasting.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/SSE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/SVE/MathFunctions.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/SVE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/SVE/PacketMath.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/SVE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/SVE/TypeCasting.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/SVE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/SYCL/InteropHeaders.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/SYCL/InteropHeaders.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/SYCL/MathFunctions.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/SYCL/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/SYCL/PacketMath.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/SYCL/PacketMath.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/SYCL/TypeCasting.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/SYCL/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/ZVector/Complex.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/ZVector/Complex.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/ZVector/MathFunctions.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/ZVector/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/arch/ZVector/PacketMath.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/arch/ZVector/PacketMath.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/functors/AssignmentFunctors.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/functors/AssignmentFunctors.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/functors/BinaryFunctors.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/functors/BinaryFunctors.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/functors/NullaryFunctors.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/functors/NullaryFunctors.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/functors/StlFunctors.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/functors/StlFunctors.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/functors/TernaryFunctors.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/functors/TernaryFunctors.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/functors/UnaryFunctors.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/functors/UnaryFunctors.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/GeneralBlockPanelKernel.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrix.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/GeneralMatrixVector.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/GeneralMatrixVector.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/Parallelizer.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/Parallelizer.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixVector.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixVector.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/SelfadjointProduct.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/SelfadjointProduct.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/SelfadjointRank2Update.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/SelfadjointRank2Update.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/TriangularMatrixMatrix.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/TriangularMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/TriangularMatrixVector.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/TriangularMatrixVector.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/TriangularSolverMatrix.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/TriangularSolverMatrix.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/products/TriangularSolverVector.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/products/TriangularSolverVector.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/util/BlasUtil.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/util/BlasUtil.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/util/ConfigureVectorization.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/util/ConfigureVectorization.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/util/Constants.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/util/Constants.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/util/DisableStupidWarnings.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/util/DisableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/util/ForwardDeclarations.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/util/ForwardDeclarations.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/util/IndexedViewHelper.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/util/IndexedViewHelper.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/util/IntegralConstant.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/util/IntegralConstant.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/util/MKL_support.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/util/MKL_support.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/util/Macros.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/util/Macros.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/util/Memory.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/util/Memory.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/util/Meta.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/util/Meta.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/util/ReenableStupidWarnings.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/util/ReenableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/util/ReshapedHelper.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/util/ReshapedHelper.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/util/StaticAssert.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/util/StaticAssert.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/util/SymbolicIndex.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/util/SymbolicIndex.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Core/util/XprHelper.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Core/util/XprHelper.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Eigenvalues/ComplexEigenSolver.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Eigenvalues/ComplexEigenSolver.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Eigenvalues/ComplexSchur.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Eigenvalues/ComplexSchur.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Eigenvalues/EigenSolver.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Eigenvalues/EigenSolver.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Eigenvalues/HessenbergDecomposition.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Eigenvalues/HessenbergDecomposition.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Eigenvalues/RealQZ.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Eigenvalues/RealQZ.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Eigenvalues/RealSchur.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Eigenvalues/RealSchur.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Eigenvalues/Tridiagonalization.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Eigenvalues/Tridiagonalization.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Geometry/AlignedBox.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Geometry/AlignedBox.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Geometry/AngleAxis.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Geometry/AngleAxis.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Geometry/EulerAngles.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Geometry/EulerAngles.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Geometry/Homogeneous.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Geometry/Homogeneous.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Geometry/Hyperplane.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Geometry/Hyperplane.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Geometry/OrthoMethods.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Geometry/OrthoMethods.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Geometry/ParametrizedLine.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Geometry/ParametrizedLine.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Geometry/Quaternion.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Geometry/Quaternion.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Geometry/Rotation2D.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Geometry/Rotation2D.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Geometry/RotationBase.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Geometry/RotationBase.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Geometry/Scaling.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Geometry/Scaling.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Geometry/Transform.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Geometry/Transform.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Geometry/Translation.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Geometry/Translation.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Geometry/Umeyama.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Geometry/Umeyama.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Geometry/arch/Geometry_SIMD.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Geometry/arch/Geometry_SIMD.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Householder/BlockHouseholder.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Householder/BlockHouseholder.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Householder/Householder.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Householder/Householder.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Householder/HouseholderSequence.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Householder/HouseholderSequence.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/Jacobi/Jacobi.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/Jacobi/Jacobi.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/KLUSupport/KLUSupport.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/KLUSupport/KLUSupport.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/LU/Determinant.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/LU/Determinant.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/LU/FullPivLU.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/LU/FullPivLU.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/LU/InverseImpl.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/LU/InverseImpl.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/LU/PartialPivLU.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/LU/PartialPivLU.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/LU/PartialPivLU_LAPACKE.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/LU/PartialPivLU_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/LU/arch/InverseSize4.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/LU/arch/InverseSize4.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/MetisSupport/MetisSupport.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/MetisSupport/MetisSupport.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/OrderingMethods/Amd.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/OrderingMethods/Amd.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/OrderingMethods/Eigen_Colamd.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/OrderingMethods/Eigen_Colamd.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/OrderingMethods/Ordering.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/OrderingMethods/Ordering.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/PaStiXSupport/PaStiXSupport.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/PaStiXSupport/PaStiXSupport.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/PardisoSupport/PardisoSupport.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/PardisoSupport/PardisoSupport.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/QR/ColPivHouseholderQR.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/QR/ColPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/QR/CompleteOrthogonalDecomposition.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/QR/CompleteOrthogonalDecomposition.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/QR/FullPivHouseholderQR.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/QR/FullPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/QR/HouseholderQR.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/QR/HouseholderQR.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/QR/HouseholderQR_LAPACKE.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/QR/HouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SVD/BDCSVD.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SVD/BDCSVD.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SVD/JacobiSVD.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SVD/JacobiSVD.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SVD/JacobiSVD_LAPACKE.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SVD/JacobiSVD_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SVD/SVDBase.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SVD/SVDBase.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SVD/UpperBidiagonalization.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SVD/UpperBidiagonalization.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseCholesky/SimplicialCholesky.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseCholesky/SimplicialCholesky.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/AmbiVector.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/AmbiVector.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/CompressedStorage.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/CompressedStorage.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/MappedSparseMatrix.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/MappedSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseAssign.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseAssign.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseBlock.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseBlock.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseColEtree.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseColEtree.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseCompressedBase.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseCompressedBase.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseCwiseBinaryOp.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseCwiseUnaryOp.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseCwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseDenseProduct.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseDenseProduct.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseDiagonalProduct.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseDiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseDot.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseDot.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseFuzzy.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseFuzzy.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseMap.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseMap.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseMatrix.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseMatrix.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseMatrixBase.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseMatrixBase.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparsePermutation.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparsePermutation.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseProduct.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseProduct.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseRedux.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseRedux.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseRef.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseRef.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseSelfAdjointView.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseSelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseSolverBase.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseSolverBase.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseSparseProductWithPruning.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseSparseProductWithPruning.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseTranspose.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseTranspose.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseTriangularView.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseTriangularView.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseUtil.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseUtil.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseVector.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseVector.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/SparseView.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/SparseView.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseCore/TriangularSolver.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseCore/TriangularSolver.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseLU/SparseLU.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseLU/SparseLU.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseLU/SparseLUImpl.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseLU/SparseLUImpl.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseLU/SparseLU_Memory.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseLU/SparseLU_Memory.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseLU/SparseLU_Structs.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseLU/SparseLU_Structs.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseLU/SparseLU_Utils.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseLU/SparseLU_Utils.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseLU/SparseLU_column_bmod.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseLU/SparseLU_column_bmod.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseLU/SparseLU_column_dfs.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseLU/SparseLU_column_dfs.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseLU/SparseLU_gemm_kernel.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseLU/SparseLU_gemm_kernel.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseLU/SparseLU_kernel_bmod.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseLU/SparseLU_kernel_bmod.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseLU/SparseLU_panel_bmod.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseLU/SparseLU_panel_bmod.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseLU/SparseLU_panel_dfs.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseLU/SparseLU_panel_dfs.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseLU/SparseLU_pivotL.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseLU/SparseLU_pivotL.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseLU/SparseLU_pruneL.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseLU/SparseLU_pruneL.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseLU/SparseLU_relax_snode.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseLU/SparseLU_relax_snode.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SparseQR/SparseQR.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SparseQR/SparseQR.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/StlSupport/StdDeque.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/StlSupport/StdDeque.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/StlSupport/StdList.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/StlSupport/StdList.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/StlSupport/StdVector.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/StlSupport/StdVector.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/StlSupport/details.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/StlSupport/details.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/SuperLUSupport/SuperLUSupport.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/SuperLUSupport/SuperLUSupport.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/UmfPackSupport/UmfPackSupport.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/UmfPackSupport/UmfPackSupport.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/misc/Image.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/misc/Image.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/misc/Kernel.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/misc/Kernel.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/misc/RealSvd2x2.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/misc/RealSvd2x2.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/misc/blas.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/misc/blas.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/misc/lapack.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/misc/lapack.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/misc/lapacke.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/misc/lapacke.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/plugins/ArrayCwiseBinaryOps.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/plugins/ArrayCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/plugins/ArrayCwiseUnaryOps.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/plugins/ArrayCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/plugins/BlockMethods.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/plugins/BlockMethods.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/plugins/CommonCwiseBinaryOps.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/plugins/CommonCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/plugins/CommonCwiseUnaryOps.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/plugins/CommonCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/plugins/IndexedViewMethods.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/plugins/IndexedViewMethods.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/plugins/MatrixCwiseBinaryOps.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/plugins/MatrixCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/plugins/MatrixCwiseUnaryOps.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/plugins/MatrixCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/eigen/Eigen/src/plugins/ReshapedMethods.h` & `probreg-0.3.8/third_party/eigen/Eigen/src/plugins/ReshapedMethods.h`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/permutohedral/permutohedral.cpp` & `probreg-0.3.8/third_party/permutohedral/permutohedral.cpp`

 * *Files identical despite different names*

### Comparing `probreg-0.3.7/third_party/permutohedral/permutohedral.h` & `probreg-0.3.8/third_party/permutohedral/permutohedral.h`

 * *Files identical despite different names*

