# Comparing `tmp/roboticstoolbox-python-1.1.0.tar.gz` & `tmp/roboticstoolbox_python-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roboticstoolbox-python-1.1.0.tar", last modified: Sun May 14 06:46:54 2023, max compression
+gzip compressed data, was "roboticstoolbox_python-1.1.1.tar", last modified: Sat May 11 10:56:55 2024, max compression
```

## Comparing `roboticstoolbox-python-1.1.0.tar` & `roboticstoolbox_python-1.1.1.tar`

### file list

```diff
@@ -1,627 +1,664 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.660790 roboticstoolbox-python-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18903 2023-05-14 06:46:54.660790 roboticstoolbox-python-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16486 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.568786 roboticstoolbox-python-1.1.0/roboticstoolbox/
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.572786 roboticstoolbox-python-1.1.0/roboticstoolbox/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/backends/Connector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.572786 roboticstoolbox-python-1.1.0/roboticstoolbox/backends/PyPlot/
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/backends/PyPlot/EllipsePlot.py
--rw-r--r--   0 runner    (1001) docker     (123)    18326 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/backends/PyPlot/PyPlot.py
--rw-r--r--   0 runner    (1001) docker     (123)    10941 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/backends/PyPlot/PyPlot2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7531 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/backends/PyPlot/RobotPlot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/backends/PyPlot/RobotPlot2.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/backends/PyPlot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.572786 roboticstoolbox-python-1.1.0/roboticstoolbox/backends/swift/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/backends/swift/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.572786 roboticstoolbox-python-1.1.0/roboticstoolbox/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/bin/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7761 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/bin/rtbtool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.572786 roboticstoolbox-python-1.1.0/roboticstoolbox/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41249 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/blocks/arm.py
--rw-r--r--   0 runner    (1001) docker     (123)    13588 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/blocks/mobile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/blocks/quad_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/blocks/spatial.py
--rw-r--r--   0 runner    (1001) docker     (123)    31034 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/blocks/uav.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.572786 roboticstoolbox-python-1.1.0/roboticstoolbox/core/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.580787 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/Cholesky
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/CholmodSupport
--rw-r--r--   0 runner    (1001) docker     (123)    12799 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/Core
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/Dense
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/Eigen
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/Eigenvalues
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/Geometry
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/Householder
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/IterativeLinearSolvers
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/Jacobi
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/KLUSupport
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/LU
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/MetisSupport
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/OrderingMethods
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/PaStiXSupport
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/PardisoSupport
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/QR
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/QtAlignedMalloc
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/SPQRSupport
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/SVD
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/Sparse
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/SparseCholesky
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/SparseCore
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/SparseLU
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/SparseQR
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/StdDeque
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/StdList
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/StdVector
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/SuperLUSupport
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/UmfPackSupport
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.568786 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.580787 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Cholesky/
--rw-r--r--   0 runner    (1001) docker     (123)    24934 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Cholesky/LDLT.h
--rw-r--r--   0 runner    (1001) docker     (123)    18760 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Cholesky/LLT.h
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Cholesky/LLT_LAPACKE.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.580787 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/CholmodSupport/
--rw-r--r--   0 runner    (1001) docker     (123)    25441 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/CholmodSupport/CholmodSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.592787 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/
--rw-r--r--   0 runner    (1001) docker     (123)    19214 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/ArithmeticSequence.h
--rw-r--r--   0 runner    (1001) docker     (123)    16782 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Array.h
--rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/ArrayBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     7018 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/ArrayWrapper.h
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Assign.h
--rw-r--r--   0 runner    (1001) docker     (123)    41673 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/AssignEvaluator.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    12488 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Assign_MKL.h
--rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/BandMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    18648 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Block.h
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/BooleanRedux.h
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/CommaInitializer.h
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/ConditionEstimator.h
--rw-r--r--   0 runner    (1001) docker     (123)    63841 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/CoreEvaluators.h
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/CoreIterators.h
--rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/CwiseBinaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)    36282 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/CwiseNullaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/CwiseTernaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/CwiseUnaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/CwiseUnaryView.h
--rw-r--r--   0 runner    (1001) docker     (123)    31529 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/DenseBase.h
--rw-r--r--   0 runner    (1001) docker     (123)    24484 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/DenseCoeffsBase.h
--rw-r--r--   0 runner    (1001) docker     (123)    25360 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/DenseStorage.h
--rw-r--r--   0 runner    (1001) docker     (123)     9870 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Diagonal.h
--rw-r--r--   0 runner    (1001) docker     (123)    14670 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/DiagonalMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/DiagonalProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)    11654 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Dot.h
--rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/EigenBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/ForceAlignedAccess.h
--rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Fuzzy.h
--rw-r--r--   0 runner    (1001) docker     (123)    21679 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/GeneralProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)    38812 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/GenericPacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)    11543 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/GlobalFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/IO.h
--rw-r--r--   0 runner    (1001) docker     (123)     9620 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/IndexedView.h
--rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Inverse.h
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Map.h
--rw-r--r--   0 runner    (1001) docker     (123)    11281 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/MapBase.h
--rw-r--r--   0 runner    (1001) docker     (123)    60784 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)     7156 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/MathFunctionsImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)    24343 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Matrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    23856 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/MatrixBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/NestByValue.h
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/NoAlias.h
--rw-r--r--   0 runner    (1001) docker     (123)    12884 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/NumTraits.h
--rw-r--r--   0 runner    (1001) docker     (123)     9207 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/PartialReduxEvaluator.h
--rw-r--r--   0 runner    (1001) docker     (123)    20748 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/PermutationMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    49193 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/PlainObjectBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Product.h
--rw-r--r--   0 runner    (1001) docker     (123)    53832 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/ProductEvaluators.h
--rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Random.h
--rw-r--r--   0 runner    (1001) docker     (123)    19195 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Redux.h
--rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Ref.h
--rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Replicate.h
--rw-r--r--   0 runner    (1001) docker     (123)    17033 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Reshaped.h
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/ReturnByValue.h
--rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Reverse.h
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Select.h
--rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/SelfAdjointView.h
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/SelfCwiseBinaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Solve.h
--rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/SolveTriangular.h
--rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/SolverBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     8700 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/StableNorm.h
--rw-r--r--   0 runner    (1001) docker     (123)    21641 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/StlIterators.h
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Stride.h
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Swap.h
--rw-r--r--   0 runner    (1001) docker     (123)    17606 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Transpose.h
--rw-r--r--   0 runner    (1001) docker     (123)    13567 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Transpositions.h
--rw-r--r--   0 runner    (1001) docker     (123)    38277 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/TriangularMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/VectorBlock.h
--rw-r--r--   0 runner    (1001) docker     (123)    35168 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/VectorwiseOp.h
--rw-r--r--   0 runner    (1001) docker     (123)    11997 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Visitor.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.564786 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.592787 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/AVX/
--rw-r--r--   0 runner    (1001) docker     (123)    15223 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/AVX/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/AVX/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    64608 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/AVX/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/AVX/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.592787 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/AVX512/
--rw-r--r--   0 runner    (1001) docker     (123)    17160 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/AVX512/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)    13344 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/AVX512/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    87891 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/AVX512/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/AVX512/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.592787 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/AltiVec/
--rw-r--r--   0 runner    (1001) docker     (123)    16540 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/AltiVec/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/AltiVec/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)   119355 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/AltiVec/MatrixProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h
--rw-r--r--   0 runner    (1001) docker     (123)    24820 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h
--rwxr-xr-x   0 runner    (1001) docker     (123)   102394 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/AltiVec/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.592787 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/CUDA/
--rw-r--r--   0 runner    (1001) docker     (123)    17317 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/CUDA/Complex.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.596787 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/Default/
--rw-r--r--   0 runner    (1001) docker     (123)    26903 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/Default/BFloat16.h
--rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/Default/ConjHelper.h
--rw-r--r--   0 runner    (1001) docker     (123)    67696 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h
--rw-r--r--   0 runner    (1001) docker     (123)    35534 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/Default/Half.h
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/Default/Settings.h
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/Default/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.596787 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/GPU/
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/GPU/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    57047 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/GPU/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/GPU/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.564786 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/HIP/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.596787 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/HIP/hcc/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/HIP/hcc/math_constants.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.596787 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/MSA/
--rw-r--r--   0 runner    (1001) docker     (123)    17541 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/MSA/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)    16159 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/MSA/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    33615 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/MSA/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.596787 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/NEON/
--rw-r--r--   0 runner    (1001) docker     (123)    22503 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/NEON/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/NEON/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)   189525 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/NEON/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)    51286 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/NEON/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.600787 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/SSE/
--rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/SSE/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/SSE/MathFunctions.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    64465 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/SSE/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/SSE/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.600787 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/SVE/
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/SVE/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    21200 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/SVE/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/SVE/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.600787 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/SYCL/
--rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/SYCL/InteropHeaders.h
--rw-r--r--   0 runner    (1001) docker     (123)    12539 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/SYCL/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    27786 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/SYCL/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)    21856 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/SYCL/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.600787 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/ZVector/
--rw-r--r--   0 runner    (1001) docker     (123)    16728 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/ZVector/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/ZVector/MathFunctions.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    36894 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/ZVector/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.604788 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/functors/
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/functors/AssignmentFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)    20921 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/functors/BinaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)     8334 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/functors/NullaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/functors/StlFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/functors/TernaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)    40146 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/functors/UnaryFunctors.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.604788 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/
--rw-r--r--   0 runner    (1001) docker     (123)   108448 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/GeneralBlockPanelKernel.h
--rw-r--r--   0 runner    (1001) docker     (123)    20104 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/GeneralMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    15948 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
--rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)    21724 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/GeneralMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/Parallelizer.h
--rw-r--r--   0 runner    (1001) docker     (123)    21354 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    11570 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/SelfadjointMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/SelfadjointProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/SelfadjointRank2Update.h
--rw-r--r--   0 runner    (1001) docker     (123)    20987 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/TriangularMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    13867 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)    14722 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/TriangularMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)    14678 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/TriangularSolverMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/TriangularSolverVector.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.608788 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/util/
--rwxr-xr-x   0 runner    (1001) docker     (123)    23156 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/util/BlasUtil.h
--rw-r--r--   0 runner    (1001) docker     (123)    19876 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/util/ConfigureVectorization.h
--rw-r--r--   0 runner    (1001) docker     (123)    21931 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/util/Constants.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     4892 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/util/DisableStupidWarnings.h
--rw-r--r--   0 runner    (1001) docker     (123)    15555 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/util/ForwardDeclarations.h
--rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/util/IndexedViewHelper.h
--rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/util/IntegralConstant.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     4268 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/util/MKL_support.h
--rw-r--r--   0 runner    (1001) docker     (123)    52909 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/util/Macros.h
--rw-r--r--   0 runner    (1001) docker     (123)    46661 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/util/Memory.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    29336 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/util/Meta.h
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/util/NonMPL2.h
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/util/ReenableStupidWarnings.h
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/util/ReshapedHelper.h
--rw-r--r--   0 runner    (1001) docker     (123)    10676 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/util/StaticAssert.h
--rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/util/SymbolicIndex.h
--rw-r--r--   0 runner    (1001) docker     (123)    35762 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/util/XprHelper.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.608788 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Eigenvalues/
--rw-r--r--   0 runner    (1001) docker     (123)    12559 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Eigenvalues/ComplexEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)    17274 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Eigenvalues/ComplexSchur.h
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (123)    22970 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Eigenvalues/EigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)    17176 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)     9716 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)    14349 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Eigenvalues/HessenbergDecomposition.h
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
--rw-r--r--   0 runner    (1001) docker     (123)    23640 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Eigenvalues/RealQZ.h
--rw-r--r--   0 runner    (1001) docker     (123)    21078 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Eigenvalues/RealSchur.h
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (123)    35182 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (123)    22764 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Eigenvalues/Tridiagonalization.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.612788 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Geometry/
--rw-r--r--   0 runner    (1001) docker     (123)    18939 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Geometry/AlignedBox.h
--rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Geometry/AngleAxis.h
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Geometry/EulerAngles.h
--rw-r--r--   0 runner    (1001) docker     (123)    20726 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Geometry/Homogeneous.h
--rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Geometry/Hyperplane.h
--rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Geometry/OrthoMethods.h
--rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Geometry/ParametrizedLine.h
--rw-r--r--   0 runner    (1001) docker     (123)    34367 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Geometry/Quaternion.h
--rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Geometry/Rotation2D.h
--rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Geometry/RotationBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Geometry/Scaling.h
--rw-r--r--   0 runner    (1001) docker     (123)    61930 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Geometry/Transform.h
--rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Geometry/Translation.h
--rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Geometry/Umeyama.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.612788 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Geometry/arch/
--rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Geometry/arch/Geometry_SIMD.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.612788 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Householder/
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Householder/BlockHouseholder.h
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Householder/Householder.h
--rw-r--r--   0 runner    (1001) docker     (123)    23611 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Householder/HouseholderSequence.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.612788 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/IterativeLinearSolvers/
--rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
--rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
--rw-r--r--   0 runner    (1001) docker     (123)    15036 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
--rw-r--r--   0 runner    (1001) docker     (123)    14940 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
--rw-r--r--   0 runner    (1001) docker     (123)    13379 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     7349 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.612788 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Jacobi/
--rw-r--r--   0 runner    (1001) docker     (123)    16383 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Jacobi/Jacobi.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.612788 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/KLUSupport/
--rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/KLUSupport/KLUSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.616788 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/LU/
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/LU/Determinant.h
--rw-r--r--   0 runner    (1001) docker     (123)    32383 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/LU/FullPivLU.h
--rw-r--r--   0 runner    (1001) docker     (123)    15727 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/LU/InverseImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)    22069 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/LU/PartialPivLU.h
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/LU/PartialPivLU_LAPACKE.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.616788 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/LU/arch/
--rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/LU/arch/InverseSize4.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.616788 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/MetisSupport/
--rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/MetisSupport/MetisSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.616788 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/OrderingMethods/
--rw-r--r--   0 runner    (1001) docker     (123)    16105 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/OrderingMethods/Amd.h
--rw-r--r--   0 runner    (1001) docker     (123)    61681 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/OrderingMethods/Eigen_Colamd.h
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/OrderingMethods/Ordering.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.616788 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/PaStiXSupport/
--rw-r--r--   0 runner    (1001) docker     (123)    22249 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/PaStiXSupport/PaStiXSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.616788 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/PardisoSupport/
--rw-r--r--   0 runner    (1001) docker     (123)    20092 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/PardisoSupport/PardisoSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.616788 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/QR/
--rw-r--r--   0 runner    (1001) docker     (123)    25498 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/QR/ColPivHouseholderQR.h
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (123)    23429 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/QR/CompleteOrthogonalDecomposition.h
--rw-r--r--   0 runner    (1001) docker     (123)    26768 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/QR/FullPivHouseholderQR.h
--rw-r--r--   0 runner    (1001) docker     (123)    14641 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/QR/HouseholderQR.h
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/QR/HouseholderQR_LAPACKE.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.616788 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SPQRSupport/
--rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.616788 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SVD/
--rw-r--r--   0 runner    (1001) docker     (123)    54214 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SVD/BDCSVD.h
--rw-r--r--   0 runner    (1001) docker     (123)    32988 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SVD/JacobiSVD.h
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SVD/JacobiSVD_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (123)    14743 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SVD/SVDBase.h
--rw-r--r--   0 runner    (1001) docker     (123)    15957 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SVD/UpperBidiagonalization.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.616788 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCholesky/
--rw-r--r--   0 runner    (1001) docker     (123)    24216 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCholesky/SimplicialCholesky.h
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.624789 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/
--rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/AmbiVector.h
--rw-r--r--   0 runner    (1001) docker     (123)     8743 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/CompressedStorage.h
--rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/MappedSparseMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseAssign.h
--rw-r--r--   0 runner    (1001) docker     (123)    24360 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseBlock.h
--rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseColEtree.h
--rw-r--r--   0 runner    (1001) docker     (123)    13606 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseCompressedBase.h
--rw-r--r--   0 runner    (1001) docker     (123)    25524 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)    13256 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseDenseProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseDiagonalProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseDot.h
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseFuzzy.h
--rw-r--r--   0 runner    (1001) docker     (123)    12589 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseMap.h
--rw-r--r--   0 runner    (1001) docker     (123)    57475 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    17451 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseMatrixBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparsePermutation.h
--rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseRedux.h
--rw-r--r--   0 runner    (1001) docker     (123)    15600 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseRef.h
--rw-r--r--   0 runner    (1001) docker     (123)    25889 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseSelfAdjointView.h
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseSolverBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseTranspose.h
--rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseTriangularView.h
--rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseUtil.h
--rw-r--r--   0 runner    (1001) docker     (123)    14832 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseVector.h
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseView.h
--rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/TriangularSolver.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.624789 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseLU/
--rw-r--r--   0 runner    (1001) docker     (123)    33316 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU.h
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseLU/SparseLUImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_Memory.h
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_Structs.h
--rw-r--r--   0 runner    (1001) docker     (123)    12837 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_Utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_column_bmod.h
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_column_dfs.h
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
--rw-r--r--   0 runner    (1001) docker     (123)    10217 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
--rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_panel_bmod.h
--rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_panel_dfs.h
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_pivotL.h
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_pruneL.h
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_relax_snode.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.624789 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseQR/
--rw-r--r--   0 runner    (1001) docker     (123)    29167 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseQR/SparseQR.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.624789 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/StlSupport/
--rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/StlSupport/StdDeque.h
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/StlSupport/StdList.h
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/StlSupport/StdVector.h
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/StlSupport/details.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.628789 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SuperLUSupport/
--rw-r--r--   0 runner    (1001) docker     (123)    34324 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SuperLUSupport/SuperLUSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.628789 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/UmfPackSupport/
--rw-r--r--   0 runner    (1001) docker     (123)    24456 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/UmfPackSupport/UmfPackSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.628789 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/misc/
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/misc/Image.h
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/misc/Kernel.h
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/misc/RealSvd2x2.h
--rw-r--r--   0 runner    (1001) docker     (123)    30560 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/misc/blas.h
--rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/misc/lapack.h
--rwxr-xr-x   0 runner    (1001) docker     (123)  1058369 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/misc/lapacke.h
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/misc/lapacke_mangling.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.632789 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)    14060 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/plugins/ArrayCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)    21431 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/plugins/ArrayCwiseUnaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)    59020 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/plugins/BlockMethods.h
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/plugins/CommonCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/plugins/CommonCwiseUnaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/plugins/IndexedViewMethods.h
--rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/plugins/MatrixCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/plugins/MatrixCwiseUnaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/plugins/ReshapedMethods.h
--rw-r--r--   0 runner    (1001) docker     (123)    43461 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/fknm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/fknm.h
--rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/frne.c
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/frne.h
--rw-r--r--   0 runner    (1001) docker     (123)    18728 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/ik.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/ik.h
--rw-r--r--   0 runner    (1001) docker     (123)     8905 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/linalg.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/linalg.h
--rw-r--r--   0 runner    (1001) docker     (123)    11510 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/methods.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/methods.h
--rw-r--r--   0 runner    (1001) docker     (123)    11495 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/ne.c
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/structs.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/structs.h
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/vmath.c
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/core/vmath.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.636789 roboticstoolbox-python-1.1.0/roboticstoolbox/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/examples/RRMC.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/examples/RRMC_swift.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/examples/baur.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/examples/branched_robot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/examples/eigdemo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/examples/fetch_vision.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/examples/holistic_mm_non_holonomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/examples/holistic_mm_omni.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/examples/icra2021.py
--rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/examples/ik_exp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/examples/ik_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/examples/ikine_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/examples/ikine_evaluate2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/examples/mexican-wave.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/examples/mmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/examples/mobile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/examples/neo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/examples/park.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/examples/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/examples/plot_swift.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/examples/puma_fdyn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/examples/puma_jtraj.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/examples/puma_swift.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/examples/readme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/examples/robots.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/examples/swift_recording.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/examples/teach.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/examples/teach_swift.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/examples/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/examples/tripleangledemo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/examples/twistdemo.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/examples/vehicle1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.640789 roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/
--rw-r--r--   0 runner    (1001) docker     (123)    15450 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/Animations.py
--rw-r--r--   0 runner    (1001) docker     (123)    14510 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/Bug2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/CurvaturePolyPlanner.py
--rw-r--r--   0 runner    (1001) docker     (123)    12236 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/DistanceTransformPlanner.py
--rw-r--r--   0 runner    (1001) docker     (123)    19218 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/DstarPlanner.py
--rw-r--r--   0 runner    (1001) docker     (123)    14088 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/DubinsPlanner.py
--rw-r--r--   0 runner    (1001) docker     (123)    52492 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/EKF.py
--rw-r--r--   0 runner    (1001) docker     (123)    13825 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/LatticePlanner.py
--rw-r--r--   0 runner    (1001) docker     (123)    17934 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/OccGrid.py
--rw-r--r--   0 runner    (1001) docker     (123)    10665 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/PRMPlanner.py
--rw-r--r--   0 runner    (1001) docker     (123)    22378 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/ParticleFilter.py
--rw-r--r--   0 runner    (1001) docker     (123)    34471 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/PlannerBase.py
--rw-r--r--   0 runner    (1001) docker     (123)    17075 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/PoseGraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/QuinticPolyPlanner.py
--rw-r--r--   0 runner    (1001) docker     (123)    11746 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/RRTPlanner.py
--rw-r--r--   0 runner    (1001) docker     (123)    16612 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/ReedsSheppPlanner.py
--rw-r--r--   0 runner    (1001) docker     (123)    43135 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/Vehicle.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/drivers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/landmarkmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    23859 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/sensors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.640789 roboticstoolbox-python-1.1.0/roboticstoolbox/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.644790 roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/AL5D.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2134 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/Ball.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/Baxter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1562 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/Cobra600.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/Coil.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/Hyper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/Hyper3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/IRB140.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/Jaco.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/KR5.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2402 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/LWR4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/Mico.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2345 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/Orion5.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2161 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/P8.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4772 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/Panda.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/Planar2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/Planar3.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11242 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/Puma560.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/Sawyer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3909 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/Stanford.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/TwoLink.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/UR10.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/UR3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/UR5.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/Uprighttl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.644790 roboticstoolbox-python-1.1.0/roboticstoolbox/models/ETS/
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/ETS/Frankie.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/ETS/GenericSeven.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/ETS/Omni.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/ETS/Panda.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/ETS/Planar2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/ETS/Planar_Y.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/ETS/Puma560.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/ETS/XYPanda.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/ETS/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.648790 roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/AL5D.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/Fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/FetchCamera.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/Frankie.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/FrankieOmni.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/KinovaGen3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/LBR.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/Mico.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/PR2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/Panda.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/Puma560.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/UR10.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/UR3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/UR5.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/Valkyrie.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/YuMi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/px100.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/px150.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/rx150.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/rx200.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/vx300.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/vx300s.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1438 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/wx200.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/wx250.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/wx250s.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/models/list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.652790 roboticstoolbox-python-1.1.0/roboticstoolbox/robot/
--rw-r--r--   0 runner    (1001) docker     (123)    89944 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/robot/BaseRobot.py
--rw-r--r--   0 runner    (1001) docker     (123)    16031 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/robot/DHFactor.py
--rw-r--r--   0 runner    (1001) docker     (123)    28433 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/robot/DHLink.py
--rw-r--r--   0 runner    (1001) docker     (123)    86411 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/robot/DHRobot.py
--rw-r--r--   0 runner    (1001) docker     (123)    50606 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/robot/Dynamics.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/robot/ELink.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/robot/ERobot.py
--rw-r--r--   0 runner    (1001) docker     (123)    27949 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/robot/ET.py
--rw-r--r--   0 runner    (1001) docker     (123)   110367 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/robot/ETS.py
--rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/robot/Gripper.py
--rw-r--r--   0 runner    (1001) docker     (123)    44773 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/robot/IK.py
--rw-r--r--   0 runner    (1001) docker     (123)    46629 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/robot/Link.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/robot/PoERobot.py
--rw-r--r--   0 runner    (1001) docker     (123)    66239 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/robot/Robot.py
--rw-r--r--   0 runner    (1001) docker     (123)    61150 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/robot/RobotKinematics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/robot/RobotProto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/robot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.652790 roboticstoolbox-python-1.1.0/roboticstoolbox/tools/
--rw-r--r--   0 runner    (1001) docker     (123)    11529 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/tools/DHFactor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/tools/Ticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/tools/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/tools/jsingu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/tools/null.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/tools/numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/tools/p_servo.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/tools/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/tools/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    34205 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/tools/trajectory.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/tools/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.652790 roboticstoolbox-python-1.1.0/roboticstoolbox/tools/urdf/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/tools/urdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59882 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/tools/urdf/urdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/tools/urdf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.652790 roboticstoolbox-python-1.1.0/roboticstoolbox/tools/xacro/
--rw-r--r--   0 runner    (1001) docker     (123)    37597 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/tools/xacro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/tools/xacro/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/tools/xacro/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-05-14 06:46:40.000000 roboticstoolbox-python-1.1.0/roboticstoolbox/tools/xacro/xmlutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.656790 roboticstoolbox-python-1.1.0/roboticstoolbox_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18903 2023-05-14 06:46:54.000000 roboticstoolbox-python-1.1.0/roboticstoolbox_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26690 2023-05-14 06:46:54.000000 roboticstoolbox-python-1.1.0/roboticstoolbox_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 06:46:54.000000 roboticstoolbox-python-1.1.0/roboticstoolbox_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-14 06:46:54.000000 roboticstoolbox-python-1.1.0/roboticstoolbox_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-14 06:46:54.000000 roboticstoolbox-python-1.1.0/roboticstoolbox_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-14 06:46:54.000000 roboticstoolbox-python-1.1.0/roboticstoolbox_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 06:46:54.660790 roboticstoolbox-python-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-14 06:46:41.000000 roboticstoolbox-python-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 06:46:54.660790 roboticstoolbox-python-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    18692 2023-05-14 06:46:41.000000 roboticstoolbox-python-1.1.0/tests/test_BaseRobot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1816 2023-05-14 06:46:41.000000 roboticstoolbox-python-1.1.0/tests/test_CustomXacro.py
--rw-r--r--   0 runner    (1001) docker     (123)    47963 2023-05-14 06:46:41.000000 roboticstoolbox-python-1.1.0/tests/test_DHRobot.py
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-05-14 06:46:41.000000 roboticstoolbox-python-1.1.0/tests/test_ELink.py
--rw-r--r--   0 runner    (1001) docker     (123)     7658 2023-05-14 06:46:41.000000 roboticstoolbox-python-1.1.0/tests/test_ERobot.py
--rw-r--r--   0 runner    (1001) docker     (123)    11833 2023-05-14 06:46:41.000000 roboticstoolbox-python-1.1.0/tests/test_ET.py
--rw-r--r--   0 runner    (1001) docker     (123)   160085 2023-05-14 06:46:41.000000 roboticstoolbox-python-1.1.0/tests/test_ETS.py
--rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-05-14 06:46:41.000000 roboticstoolbox-python-1.1.0/tests/test_ETS2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-05-14 06:46:41.000000 roboticstoolbox-python-1.1.0/tests/test_Gripper.py
--rw-r--r--   0 runner    (1001) docker     (123)    18588 2023-05-14 06:46:41.000000 roboticstoolbox-python-1.1.0/tests/test_IK.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-05-14 06:46:41.000000 roboticstoolbox-python-1.1.0/tests/test_Link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-14 06:46:41.000000 roboticstoolbox-python-1.1.0/tests/test_PyPlot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-14 06:46:41.000000 roboticstoolbox-python-1.1.0/tests/test_PyPlot2.py
--rw-r--r--   0 runner    (1001) docker     (123)    47186 2023-05-14 06:46:41.000000 roboticstoolbox-python-1.1.0/tests/test_Robot.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-14 06:46:41.000000 roboticstoolbox-python-1.1.0/tests/test_Ticker.py
--rw-r--r--   0 runner    (1001) docker     (123)    36283 2023-05-14 06:46:41.000000 roboticstoolbox-python-1.1.0/tests/test_VPython.py
--rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-05-14 06:46:41.000000 roboticstoolbox-python-1.1.0/tests/test_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-14 06:46:41.000000 roboticstoolbox-python-1.1.0/tests/test_fknm.py
--rw-r--r--   0 runner    (1001) docker     (123)    12212 2023-05-14 06:46:41.000000 roboticstoolbox-python-1.1.0/tests/test_jacob.py
--rw-r--r--   0 runner    (1001) docker     (123)    14492 2023-05-14 06:46:41.000000 roboticstoolbox-python-1.1.0/tests/test_mobile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-05-14 06:46:41.000000 roboticstoolbox-python-1.1.0/tests/test_mobile_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-14 06:46:41.000000 roboticstoolbox-python-1.1.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-14 06:46:41.000000 roboticstoolbox-python-1.1.0/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    20275 2023-05-14 06:46:41.000000 roboticstoolbox-python-1.1.0/tests/test_trajectory.py
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.774769 roboticstoolbox_python-1.1.1/
+-rw-r--r--   0 pic        (503) staff       (20)     1062 2020-09-08 21:12:15.000000 roboticstoolbox_python-1.1.1/LICENSE
+-rw-r--r--   0 pic        (503) staff       (20)    19896 2024-05-11 10:56:55.774005 roboticstoolbox_python-1.1.1/PKG-INFO
+-rw-rw----   0 pic        (503) staff       (20)    16484 2024-05-11 07:21:42.000000 roboticstoolbox_python-1.1.1/README.md
+-rw-rw----   0 pic        (503) staff       (20)     4357 2024-05-11 10:51:23.000000 roboticstoolbox_python-1.1.1/pyproject.toml
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.259514 roboticstoolbox_python-1.1.1/roboticstoolbox/
+-rw-rw----   0 pic        (503) staff       (20)     1864 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/__init__.py
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.261104 roboticstoolbox_python-1.1.1/roboticstoolbox/backends/
+-rw-r--r--   0 pic        (503) staff       (20)     2463 2020-12-06 00:07:37.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/backends/Connector.py
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.266154 roboticstoolbox_python-1.1.1/roboticstoolbox/backends/PyPlot/
+-rw-rw----   0 pic        (503) staff       (20)     5539 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/backends/PyPlot/EllipsePlot.py
+-rw-rw----   0 pic        (503) staff       (20)    18326 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/backends/PyPlot/PyPlot.py
+-rw-rw----   0 pic        (503) staff       (20)    10941 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/backends/PyPlot/PyPlot2.py
+-rw-rw----   0 pic        (503) staff       (20)     7531 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/backends/PyPlot/RobotPlot.py
+-rw-r--r--   0 pic        (503) staff       (20)     3526 2021-04-18 03:38:54.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/backends/PyPlot/RobotPlot2.py
+-rw-r--r--   0 pic        (503) staff       (20)      161 2020-11-09 03:39:51.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/backends/PyPlot/__init__.py
+-rw-r--r--   0 pic        (503) staff       (20)     1233 2021-05-09 11:01:23.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/backends/PyPlot/test1.py
+-rw-r--r--   0 pic        (503) staff       (20)      162 2023-04-25 04:22:11.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/backends/PyPlot/test2.py
+-rw-rw----   0 pic        (503) staff       (20)        0 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/backends/__init__.py
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.266690 roboticstoolbox_python-1.1.1/roboticstoolbox/backends/swift/
+-rw-r--r--   0 pic        (503) staff       (20)      388 2021-04-04 02:40:52.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/backends/swift/__init__.py
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.267814 roboticstoolbox_python-1.1.1/roboticstoolbox/bin/
+-rw-rw----   0 pic        (503) staff       (20)        0 2023-01-16 21:49:07.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/bin/__init__.py
+-rwxrwx---   0 pic        (503) staff       (20)     7761 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/bin/rtbtool.py
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.272973 roboticstoolbox_python-1.1.1/roboticstoolbox/blocks/
+-rw-rw----   0 pic        (503) staff       (20)      160 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/blocks/__init__.py
+-rw-rw----   0 pic        (503) staff       (20)    41249 2024-05-11 07:21:42.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/blocks/arm.py
+-rw-rw----   0 pic        (503) staff       (20)    13588 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/blocks/mobile.py
+-rw-rw----   0 pic        (503) staff       (20)     4407 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/blocks/quad_model.py
+-rw-rw----   0 pic        (503) staff       (20)     5260 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/blocks/spatial.py
+-rw-r--r--   0 pic        (503) staff       (20)     5467 2023-01-20 06:06:49.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/blocks/test.py
+-rw-rw----   0 pic        (503) staff       (20)    31034 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/blocks/uav.py
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.277078 roboticstoolbox_python-1.1.1/roboticstoolbox/core/
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.291016 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/
+-rw-r--r--   0 pic        (503) staff       (20)     1161 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/Cholesky
+-rw-r--r--   0 pic        (503) staff       (20)     1900 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/CholmodSupport
+-rw-r--r--   0 pic        (503) staff       (20)    12799 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/Core
+-rw-r--r--   0 pic        (503) staff       (20)      122 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/Dense
+-rw-r--r--   0 pic        (503) staff       (20)       35 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/Eigen
+-rw-r--r--   0 pic        (503) staff       (20)     1777 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/Eigenvalues
+-rw-r--r--   0 pic        (503) staff       (20)     1940 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/Geometry
+-rw-r--r--   0 pic        (503) staff       (20)      829 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/Householder
+-rw-r--r--   0 pic        (503) staff       (20)     2083 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/IterativeLinearSolvers
+-rw-r--r--   0 pic        (503) staff       (20)      894 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/Jacobi
+-rw-r--r--   0 pic        (503) staff       (20)     1389 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/KLUSupport
+-rw-r--r--   0 pic        (503) staff       (20)     1268 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/LU
+-rw-r--r--   0 pic        (503) staff       (20)      991 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/MetisSupport
+-rw-r--r--   0 pic        (503) staff       (20)     2451 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/OrderingMethods
+-rw-r--r--   0 pic        (503) staff       (20)     1751 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/PaStiXSupport
+-rw-r--r--   0 pic        (503) staff       (20)     1116 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/PardisoSupport
+-rw-r--r--   0 pic        (503) staff       (20)     1272 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/QR
+-rw-r--r--   0 pic        (503) staff       (20)      900 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/QtAlignedMalloc
+-rw-r--r--   0 pic        (503) staff       (20)     1162 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/SPQRSupport
+-rw-r--r--   0 pic        (503) staff       (20)     1584 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/SVD
+-rw-r--r--   0 pic        (503) staff       (20)      888 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/Sparse
+-rw-r--r--   0 pic        (503) staff       (20)     1235 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/SparseCholesky
+-rw-r--r--   0 pic        (503) staff       (20)     2240 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/SparseCore
+-rw-r--r--   0 pic        (503) staff       (20)     1814 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/SparseLU
+-rw-r--r--   0 pic        (503) staff       (20)     1195 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/SparseQR
+-rw-r--r--   0 pic        (503) staff       (20)      797 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/StdDeque
+-rw-r--r--   0 pic        (503) staff       (20)      726 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/StdList
+-rw-r--r--   0 pic        (503) staff       (20)      803 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/StdVector
+-rw-r--r--   0 pic        (503) staff       (20)     2243 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/SuperLUSupport
+-rw-r--r--   0 pic        (503) staff       (20)     1382 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/UmfPackSupport
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.249307 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.293824 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Cholesky/
+-rw-r--r--   0 pic        (503) staff       (20)    24934 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Cholesky/LDLT.h
+-rw-r--r--   0 pic        (503) staff       (20)    18760 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Cholesky/LLT.h
+-rw-r--r--   0 pic        (503) staff       (20)     3974 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Cholesky/LLT_LAPACKE.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.294962 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/CholmodSupport/
+-rw-r--r--   0 pic        (503) staff       (20)    25441 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/CholmodSupport/CholmodSupport.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.397513 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/
+-rw-r--r--   0 pic        (503) staff       (20)    19214 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/ArithmeticSequence.h
+-rw-r--r--   0 pic        (503) staff       (20)    16782 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Array.h
+-rw-r--r--   0 pic        (503) staff       (20)     8217 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/ArrayBase.h
+-rw-r--r--   0 pic        (503) staff       (20)     7018 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/ArrayWrapper.h
+-rw-r--r--   0 pic        (503) staff       (20)     2738 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Assign.h
+-rw-r--r--   0 pic        (503) staff       (20)    41673 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/AssignEvaluator.h
+-rwxr--r--   0 pic        (503) staff       (20)    12488 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Assign_MKL.h
+-rw-r--r--   0 pic        (503) staff       (20)    14075 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/BandMatrix.h
+-rw-r--r--   0 pic        (503) staff       (20)    18648 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Block.h
+-rw-r--r--   0 pic        (503) staff       (20)     4429 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/BooleanRedux.h
+-rw-r--r--   0 pic        (503) staff       (20)     5981 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/CommaInitializer.h
+-rw-r--r--   0 pic        (503) staff       (20)     6990 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/ConditionEstimator.h
+-rw-r--r--   0 pic        (503) staff       (20)    63841 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/CoreEvaluators.h
+-rw-r--r--   0 pic        (503) staff       (20)     4745 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/CoreIterators.h
+-rw-r--r--   0 pic        (503) staff       (20)     7909 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/CwiseBinaryOp.h
+-rw-r--r--   0 pic        (503) staff       (20)    36282 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/CwiseNullaryOp.h
+-rw-r--r--   0 pic        (503) staff       (20)     8256 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/CwiseTernaryOp.h
+-rw-r--r--   0 pic        (503) staff       (20)     3937 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/CwiseUnaryOp.h
+-rw-r--r--   0 pic        (503) staff       (20)     5551 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/CwiseUnaryView.h
+-rw-r--r--   0 pic        (503) staff       (20)    31529 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/DenseBase.h
+-rw-r--r--   0 pic        (503) staff       (20)    24484 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/DenseCoeffsBase.h
+-rw-r--r--   0 pic        (503) staff       (20)    25360 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/DenseStorage.h
+-rw-r--r--   0 pic        (503) staff       (20)     9870 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Diagonal.h
+-rw-r--r--   0 pic        (503) staff       (20)    14670 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/DiagonalMatrix.h
+-rw-r--r--   0 pic        (503) staff       (20)      988 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/DiagonalProduct.h
+-rw-r--r--   0 pic        (503) staff       (20)    11654 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Dot.h
+-rw-r--r--   0 pic        (503) staff       (20)     5841 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/EigenBase.h
+-rw-r--r--   0 pic        (503) staff       (20)     4909 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/ForceAlignedAccess.h
+-rw-r--r--   0 pic        (503) staff       (20)     5759 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Fuzzy.h
+-rw-r--r--   0 pic        (503) staff       (20)    21679 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/GeneralProduct.h
+-rw-r--r--   0 pic        (503) staff       (20)    38812 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/GenericPacketMath.h
+-rw-r--r--   0 pic        (503) staff       (20)    11543 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/GlobalFunctions.h
+-rw-r--r--   0 pic        (503) staff       (20)     8238 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/IO.h
+-rw-r--r--   0 pic        (503) staff       (20)     9620 2022-09-20 06:23:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/IndexedView.h
+-rw-r--r--   0 pic        (503) staff       (20)     3503 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Inverse.h
+-rw-r--r--   0 pic        (503) staff       (20)     7256 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Map.h
+-rw-r--r--   0 pic        (503) staff       (20)    11281 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/MapBase.h
+-rw-r--r--   0 pic        (503) staff       (20)    60784 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/MathFunctions.h
+-rw-r--r--   0 pic        (503) staff       (20)     7156 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/MathFunctionsImpl.h
+-rw-r--r--   0 pic        (503) staff       (20)    24343 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Matrix.h
+-rw-r--r--   0 pic        (503) staff       (20)    23856 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/MatrixBase.h
+-rw-r--r--   0 pic        (503) staff       (20)     2520 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/NestByValue.h
+-rw-r--r--   0 pic        (503) staff       (20)     3620 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/NoAlias.h
+-rw-r--r--   0 pic        (503) staff       (20)    12884 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/NumTraits.h
+-rw-r--r--   0 pic        (503) staff       (20)     9207 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/PartialReduxEvaluator.h
+-rw-r--r--   0 pic        (503) staff       (20)    20748 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/PermutationMatrix.h
+-rw-r--r--   0 pic        (503) staff       (20)    49193 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/PlainObjectBase.h
+-rw-r--r--   0 pic        (503) staff       (20)     7336 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Product.h
+-rw-r--r--   0 pic        (503) staff       (20)    53832 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/ProductEvaluators.h
+-rw-r--r--   0 pic        (503) staff       (20)     7756 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Random.h
+-rw-r--r--   0 pic        (503) staff       (20)    19195 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Redux.h
+-rw-r--r--   0 pic        (503) staff       (20)    17821 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Ref.h
+-rw-r--r--   0 pic        (503) staff       (20)     5656 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Replicate.h
+-rw-r--r--   0 pic        (503) staff       (20)    17033 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Reshaped.h
+-rw-r--r--   0 pic        (503) staff       (20)     4284 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/ReturnByValue.h
+-rw-r--r--   0 pic        (503) staff       (20)     7522 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Reverse.h
+-rw-r--r--   0 pic        (503) staff       (20)     6143 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Select.h
+-rw-r--r--   0 pic        (503) staff       (20)    14999 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/SelfAdjointView.h
+-rw-r--r--   0 pic        (503) staff       (20)     1697 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/SelfCwiseBinaryOp.h
+-rw-r--r--   0 pic        (503) staff       (20)     6837 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Solve.h
+-rw-r--r--   0 pic        (503) staff       (20)     9368 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/SolveTriangular.h
+-rw-r--r--   0 pic        (503) staff       (20)     6170 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/SolverBase.h
+-rw-r--r--   0 pic        (503) staff       (20)     8700 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/StableNorm.h
+-rw-r--r--   0 pic        (503) staff       (20)    21641 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/StlIterators.h
+-rw-r--r--   0 pic        (503) staff       (20)     4212 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Stride.h
+-rw-r--r--   0 pic        (503) staff       (20)     2765 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Swap.h
+-rw-r--r--   0 pic        (503) staff       (20)    17606 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Transpose.h
+-rw-r--r--   0 pic        (503) staff       (20)    13567 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Transpositions.h
+-rw-r--r--   0 pic        (503) staff       (20)    38277 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/TriangularMatrix.h
+-rw-r--r--   0 pic        (503) staff       (20)     3488 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/VectorBlock.h
+-rw-r--r--   0 pic        (503) staff       (20)    35168 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/VectorwiseOp.h
+-rw-r--r--   0 pic        (503) staff       (20)    11997 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Visitor.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.223291 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.401458 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/AVX/
+-rw-r--r--   0 pic        (503) staff       (20)    15223 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/AVX/Complex.h
+-rw-r--r--   0 pic        (503) staff       (20)     8102 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/AVX/MathFunctions.h
+-rw-r--r--   0 pic        (503) staff       (20)    64608 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/AVX/PacketMath.h
+-rw-r--r--   0 pic        (503) staff       (20)     2564 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/AVX/TypeCasting.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.404976 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/AVX512/
+-rw-r--r--   0 pic        (503) staff       (20)    17160 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/AVX512/Complex.h
+-rw-r--r--   0 pic        (503) staff       (20)    13344 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/AVX512/MathFunctions.h
+-rw-r--r--   0 pic        (503) staff       (20)    87891 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/AVX512/PacketMath.h
+-rw-r--r--   0 pic        (503) staff       (20)     2134 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/AVX512/TypeCasting.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.410044 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/AltiVec/
+-rw-r--r--   0 pic        (503) staff       (20)    16540 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/AltiVec/Complex.h
+-rw-r--r--   0 pic        (503) staff       (20)     2323 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/AltiVec/MathFunctions.h
+-rw-r--r--   0 pic        (503) staff       (20)   119355 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/AltiVec/MatrixProduct.h
+-rw-r--r--   0 pic        (503) staff       (20)     9490 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h
+-rw-r--r--   0 pic        (503) staff       (20)    24820 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h
+-rwxr--r--   0 pic        (503) staff       (20)   102394 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/AltiVec/PacketMath.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.411023 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/CUDA/
+-rw-r--r--   0 pic        (503) staff       (20)    17317 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/CUDA/Complex.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.417706 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/Default/
+-rw-r--r--   0 pic        (503) staff       (20)    26903 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/Default/BFloat16.h
+-rw-r--r--   0 pic        (503) staff       (20)     5251 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/Default/ConjHelper.h
+-rw-r--r--   0 pic        (503) staff       (20)    67696 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
+-rw-r--r--   0 pic        (503) staff       (20)     3770 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h
+-rw-r--r--   0 pic        (503) staff       (20)    35534 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/Default/Half.h
+-rw-r--r--   0 pic        (503) staff       (20)     1746 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/Default/Settings.h
+-rw-r--r--   0 pic        (503) staff       (20)     3746 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/Default/TypeCasting.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.419725 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/GPU/
+-rw-r--r--   0 pic        (503) staff       (20)     2695 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/GPU/MathFunctions.h
+-rw-r--r--   0 pic        (503) staff       (20)    57047 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/GPU/PacketMath.h
+-rw-r--r--   0 pic        (503) staff       (20)     2256 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/GPU/TypeCasting.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.202336 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/HIP/
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.420341 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/HIP/hcc/
+-rw-r--r--   0 pic        (503) staff       (20)      691 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/HIP/hcc/math_constants.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.422935 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/MSA/
+-rw-r--r--   0 pic        (503) staff       (20)    17541 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/MSA/Complex.h
+-rw-r--r--   0 pic        (503) staff       (20)    16159 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/MSA/MathFunctions.h
+-rw-r--r--   0 pic        (503) staff       (20)    33615 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/MSA/PacketMath.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.428521 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/NEON/
+-rw-r--r--   0 pic        (503) staff       (20)    22503 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/NEON/Complex.h
+-rw-r--r--   0 pic        (503) staff       (20)     6815 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h
+-rw-r--r--   0 pic        (503) staff       (20)     3083 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/NEON/MathFunctions.h
+-rw-r--r--   0 pic        (503) staff       (20)   189525 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/NEON/PacketMath.h
+-rw-r--r--   0 pic        (503) staff       (20)    51286 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/NEON/TypeCasting.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.432954 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/SSE/
+-rw-r--r--   0 pic        (503) staff       (20)    14251 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/SSE/Complex.h
+-rw-r--r--   0 pic        (503) staff       (20)     6765 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/SSE/MathFunctions.h
+-rwxr--r--   0 pic        (503) staff       (20)    64465 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/SSE/PacketMath.h
+-rw-r--r--   0 pic        (503) staff       (20)     3650 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/SSE/TypeCasting.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.435096 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/SVE/
+-rw-r--r--   0 pic        (503) staff       (20)     1194 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/SVE/MathFunctions.h
+-rw-r--r--   0 pic        (503) staff       (20)    21200 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/SVE/PacketMath.h
+-rw-r--r--   0 pic        (503) staff       (20)     1351 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/SVE/TypeCasting.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.441029 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/SYCL/
+-rw-r--r--   0 pic        (503) staff       (20)     7428 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/SYCL/InteropHeaders.h
+-rw-r--r--   0 pic        (503) staff       (20)    12539 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/SYCL/MathFunctions.h
+-rw-r--r--   0 pic        (503) staff       (20)    27786 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/SYCL/PacketMath.h
+-rw-r--r--   0 pic        (503) staff       (20)    21856 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
+-rw-r--r--   0 pic        (503) staff       (20)     2626 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/SYCL/TypeCasting.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.443316 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/ZVector/
+-rw-r--r--   0 pic        (503) staff       (20)    16728 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/ZVector/Complex.h
+-rw-r--r--   0 pic        (503) staff       (20)     8024 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/ZVector/MathFunctions.h
+-rwxr--r--   0 pic        (503) staff       (20)    36894 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/ZVector/PacketMath.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.448201 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/functors/
+-rw-r--r--   0 pic        (503) staff       (20)     6686 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/functors/AssignmentFunctors.h
+-rw-r--r--   0 pic        (503) staff       (20)    20921 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/functors/BinaryFunctors.h
+-rw-r--r--   0 pic        (503) staff       (20)     8334 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/functors/NullaryFunctors.h
+-rw-r--r--   0 pic        (503) staff       (20)     4998 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/functors/StlFunctors.h
+-rw-r--r--   0 pic        (503) staff       (20)      607 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/functors/TernaryFunctors.h
+-rw-r--r--   0 pic        (503) staff       (20)    40146 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/functors/UnaryFunctors.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.466670 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/
+-rw-r--r--   0 pic        (503) staff       (20)   108448 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/GeneralBlockPanelKernel.h
+-rw-r--r--   0 pic        (503) staff       (20)    20104 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/GeneralMatrixMatrix.h
+-rw-r--r--   0 pic        (503) staff       (20)    15948 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
+-rw-r--r--   0 pic        (503) staff       (20)     6936 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
+-rw-r--r--   0 pic        (503) staff       (20)     5106 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
+-rw-r--r--   0 pic        (503) staff       (20)    21724 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/GeneralMatrixVector.h
+-rw-r--r--   0 pic        (503) staff       (20)     6368 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
+-rw-r--r--   0 pic        (503) staff       (20)     5582 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/Parallelizer.h
+-rw-r--r--   0 pic        (503) staff       (20)    21354 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
+-rw-r--r--   0 pic        (503) staff       (20)    11570 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
+-rw-r--r--   0 pic        (503) staff       (20)     9958 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/SelfadjointMatrixVector.h
+-rw-r--r--   0 pic        (503) staff       (20)     5209 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
+-rw-r--r--   0 pic        (503) staff       (20)     6164 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/SelfadjointProduct.h
+-rw-r--r--   0 pic        (503) staff       (20)     4126 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/SelfadjointRank2Update.h
+-rw-r--r--   0 pic        (503) staff       (20)    20987 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/TriangularMatrixMatrix.h
+-rw-r--r--   0 pic        (503) staff       (20)    13867 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
+-rw-r--r--   0 pic        (503) staff       (20)    14722 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/TriangularMatrixVector.h
+-rw-r--r--   0 pic        (503) staff       (20)    10571 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
+-rw-r--r--   0 pic        (503) staff       (20)    14678 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/TriangularSolverMatrix.h
+-rw-r--r--   0 pic        (503) staff       (20)     6707 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
+-rw-r--r--   0 pic        (503) staff       (20)     5882 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/TriangularSolverVector.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.499096 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/util/
+-rwxr--r--   0 pic        (503) staff       (20)    23156 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/util/BlasUtil.h
+-rw-r--r--   0 pic        (503) staff       (20)    19876 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/util/ConfigureVectorization.h
+-rw-r--r--   0 pic        (503) staff       (20)    21931 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/util/Constants.h
+-rwxr--r--   0 pic        (503) staff       (20)     4892 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/util/DisableStupidWarnings.h
+-rw-r--r--   0 pic        (503) staff       (20)    15555 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/util/ForwardDeclarations.h
+-rw-r--r--   0 pic        (503) staff       (20)     6696 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/util/IndexedViewHelper.h
+-rw-r--r--   0 pic        (503) staff       (20)    10949 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/util/IntegralConstant.h
+-rwxr--r--   0 pic        (503) staff       (20)     4268 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/util/MKL_support.h
+-rw-r--r--   0 pic        (503) staff       (20)    52909 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/util/Macros.h
+-rw-r--r--   0 pic        (503) staff       (20)    46661 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/util/Memory.h
+-rwxr--r--   0 pic        (503) staff       (20)    29336 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/util/Meta.h
+-rw-r--r--   0 pic        (503) staff       (20)       85 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/util/NonMPL2.h
+-rw-r--r--   0 pic        (503) staff       (20)     1024 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/util/ReenableStupidWarnings.h
+-rw-r--r--   0 pic        (503) staff       (20)     1432 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/util/ReshapedHelper.h
+-rw-r--r--   0 pic        (503) staff       (20)    10676 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/util/StaticAssert.h
+-rw-r--r--   0 pic        (503) staff       (20)    12003 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/util/SymbolicIndex.h
+-rw-r--r--   0 pic        (503) staff       (20)    35762 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/util/XprHelper.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.532429 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Eigenvalues/
+-rw-r--r--   0 pic        (503) staff       (20)    12559 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Eigenvalues/ComplexEigenSolver.h
+-rw-r--r--   0 pic        (503) staff       (20)    17274 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Eigenvalues/ComplexSchur.h
+-rw-r--r--   0 pic        (503) staff       (20)     4178 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
+-rw-r--r--   0 pic        (503) staff       (20)    22970 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Eigenvalues/EigenSolver.h
+-rw-r--r--   0 pic        (503) staff       (20)    17176 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
+-rw-r--r--   0 pic        (503) staff       (20)     9716 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
+-rw-r--r--   0 pic        (503) staff       (20)    14349 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Eigenvalues/HessenbergDecomposition.h
+-rw-r--r--   0 pic        (503) staff       (20)     5575 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
+-rw-r--r--   0 pic        (503) staff       (20)    23640 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Eigenvalues/RealQZ.h
+-rw-r--r--   0 pic        (503) staff       (20)    21078 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Eigenvalues/RealSchur.h
+-rw-r--r--   0 pic        (503) staff       (20)     3650 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
+-rw-r--r--   0 pic        (503) staff       (20)    35182 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
+-rw-r--r--   0 pic        (503) staff       (20)     4104 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
+-rw-r--r--   0 pic        (503) staff       (20)    22764 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Eigenvalues/Tridiagonalization.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.539598 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Geometry/
+-rw-r--r--   0 pic        (503) staff       (20)    18939 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Geometry/AlignedBox.h
+-rw-r--r--   0 pic        (503) staff       (20)     8403 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Geometry/AngleAxis.h
+-rw-r--r--   0 pic        (503) staff       (20)     3624 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Geometry/EulerAngles.h
+-rw-r--r--   0 pic        (503) staff       (20)    20726 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Geometry/Homogeneous.h
+-rw-r--r--   0 pic        (503) staff       (20)    11962 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Geometry/Hyperplane.h
+-rw-r--r--   0 pic        (503) staff       (20)     8955 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Geometry/OrthoMethods.h
+-rw-r--r--   0 pic        (503) staff       (20)     9812 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Geometry/ParametrizedLine.h
+-rw-r--r--   0 pic        (503) staff       (20)    34367 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Geometry/Quaternion.h
+-rw-r--r--   0 pic        (503) staff       (20)     6862 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Geometry/Rotation2D.h
+-rw-r--r--   0 pic        (503) staff       (20)     8063 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Geometry/RotationBase.h
+-rw-r--r--   0 pic        (503) staff       (20)     6724 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Geometry/Scaling.h
+-rw-r--r--   0 pic        (503) staff       (20)    61930 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Geometry/Transform.h
+-rw-r--r--   0 pic        (503) staff       (20)     7664 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Geometry/Translation.h
+-rw-r--r--   0 pic        (503) staff       (20)     6190 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Geometry/Umeyama.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.540095 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Geometry/arch/
+-rw-r--r--   0 pic        (503) staff       (20)     5945 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Geometry/arch/Geometry_SIMD.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.541213 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Householder/
+-rw-r--r--   0 pic        (503) staff       (20)     4784 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Householder/BlockHouseholder.h
+-rw-r--r--   0 pic        (503) staff       (20)     5365 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Householder/Householder.h
+-rw-r--r--   0 pic        (503) staff       (20)    23611 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Householder/HouseholderSequence.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.545572 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/IterativeLinearSolvers/
+-rw-r--r--   0 pic        (503) staff       (20)     6771 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
+-rw-r--r--   0 pic        (503) staff       (20)     6850 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
+-rw-r--r--   0 pic        (503) staff       (20)     8887 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
+-rw-r--r--   0 pic        (503) staff       (20)    15036 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
+-rw-r--r--   0 pic        (503) staff       (20)    14940 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
+-rw-r--r--   0 pic        (503) staff       (20)    13379 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
+-rw-r--r--   0 pic        (503) staff       (20)     7349 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
+-rw-r--r--   0 pic        (503) staff       (20)     4212 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.545944 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Jacobi/
+-rw-r--r--   0 pic        (503) staff       (20)    16383 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Jacobi/Jacobi.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.546635 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/KLUSupport/
+-rw-r--r--   0 pic        (503) staff       (20)    11555 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/KLUSupport/KLUSupport.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.548996 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/LU/
+-rw-r--r--   0 pic        (503) staff       (20)     3439 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/LU/Determinant.h
+-rw-r--r--   0 pic        (503) staff       (20)    32383 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/LU/FullPivLU.h
+-rw-r--r--   0 pic        (503) staff       (20)    15727 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/LU/InverseImpl.h
+-rw-r--r--   0 pic        (503) staff       (20)    22069 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/LU/PartialPivLU.h
+-rw-r--r--   0 pic        (503) staff       (20)     3555 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/LU/PartialPivLU_LAPACKE.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.549393 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/LU/arch/
+-rw-r--r--   0 pic        (503) staff       (20)    13693 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/LU/arch/InverseSize4.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.549892 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/MetisSupport/
+-rw-r--r--   0 pic        (503) staff       (20)     4588 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/MetisSupport/MetisSupport.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.551847 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/OrderingMethods/
+-rw-r--r--   0 pic        (503) staff       (20)    16105 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/OrderingMethods/Amd.h
+-rw-r--r--   0 pic        (503) staff       (20)    61681 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/OrderingMethods/Eigen_Colamd.h
+-rw-r--r--   0 pic        (503) staff       (20)     5248 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/OrderingMethods/Ordering.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.552178 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/PaStiXSupport/
+-rw-r--r--   0 pic        (503) staff       (20)    22249 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/PaStiXSupport/PaStiXSupport.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.552930 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/PardisoSupport/
+-rw-r--r--   0 pic        (503) staff       (20)    20092 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/PardisoSupport/PardisoSupport.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.578862 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/QR/
+-rw-r--r--   0 pic        (503) staff       (20)    25498 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/QR/ColPivHouseholderQR.h
+-rw-r--r--   0 pic        (503) staff       (20)     4662 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
+-rw-r--r--   0 pic        (503) staff       (20)    23429 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/QR/CompleteOrthogonalDecomposition.h
+-rw-r--r--   0 pic        (503) staff       (20)    26768 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/QR/FullPivHouseholderQR.h
+-rw-r--r--   0 pic        (503) staff       (20)    14641 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/QR/HouseholderQR.h
+-rw-r--r--   0 pic        (503) staff       (20)     2993 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/QR/HouseholderQR_LAPACKE.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.579243 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SPQRSupport/
+-rw-r--r--   0 pic        (503) staff       (20)    11826 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.582444 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SVD/
+-rw-r--r--   0 pic        (503) staff       (20)    54214 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SVD/BDCSVD.h
+-rw-r--r--   0 pic        (503) staff       (20)    32988 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SVD/JacobiSVD.h
+-rw-r--r--   0 pic        (503) staff       (20)     5099 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SVD/JacobiSVD_LAPACKE.h
+-rw-r--r--   0 pic        (503) staff       (20)    14743 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SVD/SVDBase.h
+-rw-r--r--   0 pic        (503) staff       (20)    15957 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SVD/UpperBidiagonalization.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.583968 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCholesky/
+-rw-r--r--   0 pic        (503) staff       (20)    24216 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCholesky/SimplicialCholesky.h
+-rw-r--r--   0 pic        (503) staff       (20)     5830 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.598746 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/
+-rw-r--r--   0 pic        (503) staff       (20)    10670 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/AmbiVector.h
+-rw-r--r--   0 pic        (503) staff       (20)     8743 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/CompressedStorage.h
+-rw-r--r--   0 pic        (503) staff       (20)    13166 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
+-rw-r--r--   0 pic        (503) staff       (20)     2191 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/MappedSparseMatrix.h
+-rw-r--r--   0 pic        (503) staff       (20)    11368 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseAssign.h
+-rw-r--r--   0 pic        (503) staff       (20)    24360 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseBlock.h
+-rw-r--r--   0 pic        (503) staff       (20)     6485 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseColEtree.h
+-rw-r--r--   0 pic        (503) staff       (20)    13606 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseCompressedBase.h
+-rw-r--r--   0 pic        (503) staff       (20)    25524 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
+-rw-r--r--   0 pic        (503) staff       (20)     4757 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
+-rw-r--r--   0 pic        (503) staff       (20)    13256 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseDenseProduct.h
+-rw-r--r--   0 pic        (503) staff       (20)     5808 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseDiagonalProduct.h
+-rw-r--r--   0 pic        (503) staff       (20)     3080 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseDot.h
+-rw-r--r--   0 pic        (503) staff       (20)     1107 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseFuzzy.h
+-rw-r--r--   0 pic        (503) staff       (20)    12589 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseMap.h
+-rw-r--r--   0 pic        (503) staff       (20)    57475 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseMatrix.h
+-rw-r--r--   0 pic        (503) staff       (20)    17451 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseMatrixBase.h
+-rw-r--r--   0 pic        (503) staff       (20)     7329 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparsePermutation.h
+-rw-r--r--   0 pic        (503) staff       (20)     7593 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseProduct.h
+-rw-r--r--   0 pic        (503) staff       (20)     1699 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseRedux.h
+-rw-r--r--   0 pic        (503) staff       (20)    15600 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseRef.h
+-rw-r--r--   0 pic        (503) staff       (20)    25889 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseSelfAdjointView.h
+-rw-r--r--   0 pic        (503) staff       (20)     4424 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseSolverBase.h
+-rw-r--r--   0 pic        (503) staff       (20)     8704 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
+-rw-r--r--   0 pic        (503) staff       (20)     3175 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseTranspose.h
+-rw-r--r--   0 pic        (503) staff       (20)     6437 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseTriangularView.h
+-rw-r--r--   0 pic        (503) staff       (20)     6827 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseUtil.h
+-rw-r--r--   0 pic        (503) staff       (20)    14832 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseVector.h
+-rw-r--r--   0 pic        (503) staff       (20)     8127 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseView.h
+-rw-r--r--   0 pic        (503) staff       (20)     9657 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/TriangularSolver.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.606678 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseLU/
+-rw-r--r--   0 pic        (503) staff       (20)    33316 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU.h
+-rw-r--r--   0 pic        (503) staff       (20)     4303 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseLU/SparseLUImpl.h
+-rw-r--r--   0 pic        (503) staff       (20)     7602 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_Memory.h
+-rw-r--r--   0 pic        (503) staff       (20)     4974 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_Structs.h
+-rw-r--r--   0 pic        (503) staff       (20)    12837 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
+-rw-r--r--   0 pic        (503) staff       (20)     2049 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_Utils.h
+-rw-r--r--   0 pic        (503) staff       (20)     6712 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_column_bmod.h
+-rw-r--r--   0 pic        (503) staff       (20)     6584 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_column_dfs.h
+-rw-r--r--   0 pic        (503) staff       (20)     3681 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
+-rw-r--r--   0 pic        (503) staff       (20)    10217 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
+-rw-r--r--   0 pic        (503) staff       (20)     4181 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
+-rw-r--r--   0 pic        (503) staff       (20)     5723 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
+-rw-r--r--   0 pic        (503) staff       (20)     8485 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_panel_bmod.h
+-rw-r--r--   0 pic        (503) staff       (20)     9028 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_panel_dfs.h
+-rw-r--r--   0 pic        (503) staff       (20)     4979 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_pivotL.h
+-rw-r--r--   0 pic        (503) staff       (20)     4545 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_pruneL.h
+-rw-r--r--   0 pic        (503) staff       (20)     2889 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_relax_snode.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.607080 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseQR/
+-rw-r--r--   0 pic        (503) staff       (20)    29167 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseQR/SparseQR.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.608914 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/StlSupport/
+-rw-r--r--   0 pic        (503) staff       (20)     4730 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/StlSupport/StdDeque.h
+-rw-r--r--   0 pic        (503) staff       (20)     4155 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/StlSupport/StdList.h
+-rw-r--r--   0 pic        (503) staff       (20)     5338 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/StlSupport/StdVector.h
+-rw-r--r--   0 pic        (503) staff       (20)     2809 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/StlSupport/details.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.609295 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SuperLUSupport/
+-rw-r--r--   0 pic        (503) staff       (20)    34324 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SuperLUSupport/SuperLUSupport.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.609873 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/UmfPackSupport/
+-rw-r--r--   0 pic        (503) staff       (20)    24456 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/UmfPackSupport/UmfPackSupport.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.615972 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/misc/
+-rw-r--r--   0 pic        (503) staff       (20)     2913 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/misc/Image.h
+-rw-r--r--   0 pic        (503) staff       (20)     2742 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/misc/Kernel.h
+-rw-r--r--   0 pic        (503) staff       (20)     1748 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/misc/RealSvd2x2.h
+-rw-r--r--   0 pic        (503) staff       (20)    30560 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/misc/blas.h
+-rw-r--r--   0 pic        (503) staff       (20)     7834 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/misc/lapack.h
+-rwxr--r--   0 pic        (503) staff       (20)  1058369 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/misc/lapacke.h
+-rw-r--r--   0 pic        (503) staff       (20)      474 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/misc/lapacke_mangling.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.620356 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/plugins/
+-rw-r--r--   0 pic        (503) staff       (20)    14060 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/plugins/ArrayCwiseBinaryOps.h
+-rw-r--r--   0 pic        (503) staff       (20)    21431 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/plugins/ArrayCwiseUnaryOps.h
+-rw-r--r--   0 pic        (503) staff       (20)    59020 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/plugins/BlockMethods.h
+-rw-r--r--   0 pic        (503) staff       (20)     4828 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/plugins/CommonCwiseBinaryOps.h
+-rw-r--r--   0 pic        (503) staff       (20)     6089 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/plugins/CommonCwiseUnaryOps.h
+-rw-r--r--   0 pic        (503) staff       (20)    12283 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/plugins/IndexedViewMethods.h
+-rw-r--r--   0 pic        (503) staff       (20)     6387 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/plugins/MatrixCwiseBinaryOps.h
+-rw-r--r--   0 pic        (503) staff       (20)     3350 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/plugins/MatrixCwiseUnaryOps.h
+-rw-r--r--   0 pic        (503) staff       (20)     6915 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/plugins/ReshapedMethods.h
+-rw-rw----   0 pic        (503) staff       (20)    43461 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/fknm.cpp
+-rw-rw----   0 pic        (503) staff       (20)     1778 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/fknm.h
+-rw-r--r--   0 pic        (503) staff       (20)     8986 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/frne.c
+-rw-r--r--   0 pic        (503) staff       (20)     3220 2020-09-08 21:12:15.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/frne.h
+-rw-rw----   0 pic        (503) staff       (20)    18728 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/ik.cpp
+-rw-r--r--   0 pic        (503) staff       (20)     1780 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/ik.h
+-rw-r--r--   0 pic        (503) staff       (20)     8905 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/linalg.cpp
+-rw-r--r--   0 pic        (503) staff       (20)     1862 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/linalg.h
+-rw-rw----   0 pic        (503) staff       (20)    11510 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/methods.cpp
+-rw-r--r--   0 pic        (503) staff       (20)      767 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/methods.h
+-rw-r--r--   0 pic        (503) staff       (20)    11495 2020-09-08 21:12:15.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/ne.c
+-rw-r--r--   0 pic        (503) staff       (20)      660 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/structs.cpp
+-rw-rw----   0 pic        (503) staff       (20)     1550 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/structs.h
+-rw-r--r--   0 pic        (503) staff       (20)     3092 2020-09-08 21:12:15.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/vmath.c
+-rw-r--r--   0 pic        (503) staff       (20)      776 2020-09-08 21:12:15.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/core/vmath.h
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.637725 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/
+-rw-r--r--   0 pic        (503) staff       (20)      761 2021-04-04 02:40:52.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/RRMC.py
+-rw-r--r--   0 pic        (503) staff       (20)      572 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/RRMC_swift.py
+-rw-r--r--   0 pic        (503) staff       (20)        0 2020-09-08 21:12:15.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/__init__.py
+-rw-r--r--   0 pic        (503) staff       (20)     1661 2021-08-18 02:22:57.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/armer.py
+-rw-r--r--   0 pic        (503) staff       (20)     2886 2021-03-21 05:55:43.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/aside.py
+-rw-r--r--   0 pic        (503) staff       (20)     2476 2021-04-04 02:40:52.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/baur.py
+-rw-r--r--   0 pic        (503) staff       (20)     1647 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/branched_robot.py
+-rw-r--r--   0 pic        (503) staff       (20)      731 2020-11-09 20:54:58.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/colors.py
+-rw-r--r--   0 pic        (503) staff       (20)       84 2020-11-15 03:03:16.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/eg2.py
+-rw-rw----   0 pic        (503) staff       (20)     2446 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/eigdemo.py
+-rw-r--r--   0 pic        (503) staff       (20)      172 2020-11-01 12:12:57.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/erobot-test.py
+-rw-r--r--   0 pic        (503) staff       (20)     6336 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/fetch_vision.py
+-rw-r--r--   0 pic        (503) staff       (20)     2728 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/holistic_mm_non_holonomic.py
+-rw-r--r--   0 pic        (503) staff       (20)     2732 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/holistic_mm_omni.py
+-rw-r--r--   0 pic        (503) staff       (20)     3357 2021-05-09 04:28:39.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/icra2021.py
+-rw-r--r--   0 pic        (503) staff       (20)     6307 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/ik_exp.py
+-rw-r--r--   0 pic        (503) staff       (20)     2512 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/ik_speed.py
+-rw-rw----   0 pic        (503) staff       (20)     2670 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/ikine_evaluate.py
+-rw-rw----   0 pic        (503) staff       (20)     2145 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/ikine_evaluate2.py
+-rw-r--r--   0 pic        (503) staff       (20)     1029 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/mexican-wave.py
+-rw-r--r--   0 pic        (503) staff       (20)     2524 2021-04-04 02:40:52.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/mmc.py
+-rw-r--r--   0 pic        (503) staff       (20)     2792 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/mobile.py
+-rw-r--r--   0 pic        (503) staff       (20)     3705 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/neo.py
+-rw-r--r--   0 pic        (503) staff       (20)     1724 2021-04-04 02:40:52.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/park.py
+-rw-r--r--   0 pic        (503) staff       (20)      502 2021-04-04 02:40:52.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/plot.py
+-rw-r--r--   0 pic        (503) staff       (20)      133 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/plot_swift.py
+-rw-r--r--   0 pic        (503) staff       (20)     2403 2020-12-30 03:50:37.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/poly_example.py
+-rw-rw----   0 pic        (503) staff       (20)      478 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/puma_fdyn.py
+-rw-r--r--   0 pic        (503) staff       (20)     1323 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/puma_jtraj.py
+-rw-r--r--   0 pic        (503) staff       (20)      848 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/puma_swift.py
+-rw-r--r--   0 pic        (503) staff       (20)     1103 2021-04-04 02:40:52.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/readme.py
+-rw-r--r--   0 pic        (503) staff       (20)     1710 2021-04-04 02:40:52.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/robots.py
+-rw-r--r--   0 pic        (503) staff       (20)     3308 2022-03-07 01:56:36.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/swift_recording.py
+-rw-r--r--   0 pic        (503) staff       (20)      251 2021-04-04 02:40:52.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/teach.py
+-rw-r--r--   0 pic        (503) staff       (20)     1544 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/teach_swift.py
+-rw-rw----   0 pic        (503) staff       (20)      426 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/test.py
+-rw-r--r--   0 pic        (503) staff       (20)      140 2021-03-06 23:56:48.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/test1.py
+-rw-r--r--   0 pic        (503) staff       (20)     2070 2020-09-08 05:18:28.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/test_et.py
+-rwxr--r--   0 pic        (503) staff       (20)     1449 2020-10-27 05:29:24.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/timing.py
+-rw-r--r--   0 pic        (503) staff       (20)     5397 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/tripleangledemo.py
+-rw-r--r--   0 pic        (503) staff       (20)     3215 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/twistdemo.py
+-rw-r--r--   0 pic        (503) staff       (20)      766 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/examples/vehicle1.py
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.659412 roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/
+-rw-rw----   0 pic        (503) staff       (20)    15450 2024-05-11 07:21:42.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/Animations.py
+-rw-rw----   0 pic        (503) staff       (20)    14510 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/Bug2.py
+-rw-r--r--   0 pic        (503) staff       (20)     5462 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/CurvaturePolyPlanner.py
+-rw-r--r--   0 pic        (503) staff       (20)     5206 2023-03-15 08:31:16.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/CurvaturePolyPlanner.py-new.py
+-rw-rw----   0 pic        (503) staff       (20)    12236 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/DistanceTransformPlanner.py
+-rw-r--r--   0 pic        (503) staff       (20)    15753 2023-03-15 08:31:17.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/DstarPlanner-nearly.py
+-rw-r--r--   0 pic        (503) staff       (20)    12993 2023-03-15 08:31:17.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/DstarPlanner-old.py
+-rw-rw----   0 pic        (503) staff       (20)    19218 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/DstarPlanner.py
+-rw-rw----   0 pic        (503) staff       (20)    14088 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/DubinsPlanner.py
+-rw-rw----   0 pic        (503) staff       (20)    52486 2024-05-11 07:22:01.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/EKF.py
+-rw-rw----   0 pic        (503) staff       (20)    13825 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/LatticePlanner.py
+-rw-rw----   0 pic        (503) staff       (20)    17934 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/OccGrid.py
+-rw-rw----   0 pic        (503) staff       (20)    10665 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/PRMPlanner.py
+-rw-rw----   0 pic        (503) staff       (20)    22378 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/ParticleFilter.py
+-rw-rw----   0 pic        (503) staff       (20)    34471 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/PlannerBase.py
+-rw-rw----   0 pic        (503) staff       (20)    17075 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/PoseGraph.py
+-rw-rw----   0 pic        (503) staff       (20)    10359 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/QuinticPolyPlanner.py
+-rw-rw----   0 pic        (503) staff       (20)    11746 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/RRTPlanner.py
+-rw-rw----   0 pic        (503) staff       (20)    16612 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/ReedsSheppPlanner.py
+-rw-rw----   0 pic        (503) staff       (20)    43135 2024-05-11 07:21:42.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/Vehicle.py
+-rw-rw----   0 pic        (503) staff       (20)     5627 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/__init__.py
+-rw-r--r--   0 pic        (503) staff       (20)    12481 2023-03-15 08:31:17.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/bug.py
+-rw-r--r--   0 pic        (503) staff       (20)        0 2020-12-27 06:33:23.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/distancexform.py
+-rw-rw----   0 pic        (503) staff       (20)     8943 2024-05-11 07:21:42.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/drivers.py
+-rw-r--r--   0 pic        (503) staff       (20)    10504 2023-03-15 08:31:17.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/dubins_path_planning.py
+-rw-rw----   0 pic        (503) staff       (20)     5091 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/landmarkmap.py
+-rw-r--r--   0 pic        (503) staff       (20)      373 2023-03-15 08:31:16.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/new.py
+-rw-r--r--   0 pic        (503) staff       (20)     1195 2023-03-15 08:31:16.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/plot_vehicle.py
+-rw-r--r--   0 pic        (503) staff       (20)     7383 2023-03-15 08:31:17.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/probabilistic_road_map.py
+-rw-r--r--   0 pic        (503) staff       (20)     1975 2023-03-15 08:31:16.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/qtiming.py
+-rw-r--r--   0 pic        (503) staff       (20)     7711 2023-03-15 08:31:17.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/reedsshepp-old.py
+-rw-r--r--   0 pic        (503) staff       (20)     7997 2023-03-15 08:31:17.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/rrt.py
+-rw-r--r--   0 pic        (503) staff       (20)     7244 2023-03-15 08:31:17.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/rrt_dubins.py
+-rw-r--r--   0 pic        (503) staff       (20)     9059 2023-03-15 08:31:17.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/rrt_star.py
+-rw-r--r--   0 pic        (503) staff       (20)     3378 2023-03-15 08:31:17.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/rrt_with_pathsmoothing.py
+-rw-rw----   0 pic        (503) staff       (20)    23859 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/sensors.py
+-rw-r--r--   0 pic        (503) staff       (20)     8769 2023-03-15 08:31:17.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/state_lattice_planner.py
+-rw-r--r--   0 pic        (503) staff       (20)      696 2023-03-15 08:31:16.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/test2.py
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.660381 roboticstoolbox_python-1.1.1/roboticstoolbox/models/
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.693245 roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/
+-rw-r--r--   0 pic        (503) staff       (20)     2941 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/AL5D.py
+-rwxr--r--   0 pic        (503) staff       (20)     2134 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/Ball.py
+-rw-r--r--   0 pic        (503) staff       (20)     2855 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/Baxter.py
+-rwxr--r--   0 pic        (503) staff       (20)     1562 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/Cobra600.py
+-rw-r--r--   0 pic        (503) staff       (20)     2110 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/Coil.py
+-rw-r--r--   0 pic        (503) staff       (20)     2133 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/Hyper.py
+-rw-r--r--   0 pic        (503) staff       (20)     2181 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/Hyper3d.py
+-rw-r--r--   0 pic        (503) staff       (20)     4452 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/IRB140.py
+-rw-r--r--   0 pic        (503) staff       (20)     2742 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/Jaco.py
+-rw-r--r--   0 pic        (503) staff       (20)     2943 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/KR5.py
+-rwxr--r--   0 pic        (503) staff       (20)     2402 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/LWR4.py
+-rw-r--r--   0 pic        (503) staff       (20)     2736 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/Mico.py
+-rwxr--r--   0 pic        (503) staff       (20)     2345 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/Orion5.py
+-rwxr--r--   0 pic        (503) staff       (20)     2161 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/P8.py
+-rwxr--r--   0 pic        (503) staff       (20)     4772 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/Panda.py
+-rw-r--r--   0 pic        (503) staff       (20)     1673 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/Planar2.py
+-rw-r--r--   0 pic        (503) staff       (20)     1085 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/Planar3.py
+-rwxr--r--   0 pic        (503) staff       (20)    11242 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/Puma560.py
+-rw-rw----   0 pic        (503) staff       (20)     2085 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/Sawyer.py
+-rwxr--r--   0 pic        (503) staff       (20)     3909 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/Stanford.py
+-rw-r--r--   0 pic        (503) staff       (20)     3353 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/TwoLink.py
+-rw-r--r--   0 pic        (503) staff       (20)     2513 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/UR10.py
+-rw-r--r--   0 pic        (503) staff       (20)     2484 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/UR3.py
+-rw-r--r--   0 pic        (503) staff       (20)     2535 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/UR5.py
+-rw-r--r--   0 pic        (503) staff       (20)      571 2020-10-21 02:33:26.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/Uprighttl.py
+-rw-r--r--   0 pic        (503) staff       (20)     1540 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/__init__.py
+-rw-r--r--   0 pic        (503) staff       (20)     6961 2020-10-19 05:48:52.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/arte_parse.py
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.697773 roboticstoolbox_python-1.1.1/roboticstoolbox/models/ETS/
+-rw-rw----   0 pic        (503) staff       (20)     2861 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/ETS/Frankie.py
+-rw-rw----   0 pic        (503) staff       (20)     1537 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/ETS/GenericSeven.py
+-rw-rw----   0 pic        (503) staff       (20)     2229 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/ETS/Omni.py
+-rw-rw----   0 pic        (503) staff       (20)     1941 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/ETS/Panda.py
+-rw-rw----   0 pic        (503) staff       (20)     1210 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/ETS/Planar2.py
+-rw-rw----   0 pic        (503) staff       (20)     1717 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/ETS/Planar_Y.py
+-rw-rw----   0 pic        (503) staff       (20)     2004 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/ETS/Puma560.py
+-rw-r--r--   0 pic        (503) staff       (20)     3005 2021-03-15 20:45:21.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/ETS/Puma560dh.py
+-rw-rw----   0 pic        (503) staff       (20)     2556 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/ETS/XYPanda.py
+-rw-r--r--   0 pic        (503) staff       (20)      583 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/ETS/__init__.py
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.709706 roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/
+-rw-rw----   0 pic        (503) staff       (20)     1364 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/AL5D.py
+-rw-rw----   0 pic        (503) staff       (20)     1760 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/Fetch.py
+-rw-rw----   0 pic        (503) staff       (20)     1736 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/FetchCamera.py
+-rw-rw----   0 pic        (503) staff       (20)     1957 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/Frankie.py
+-rw-rw----   0 pic        (503) staff       (20)     2487 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/FrankieOmni.py
+-rw-rw----   0 pic        (503) staff       (20)     1593 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/KinovaGen3.py
+-rw-rw----   0 pic        (503) staff       (20)     1583 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/LBR.py
+-rw-rw----   0 pic        (503) staff       (20)     1801 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/Mico.py
+-rw-rw----   0 pic        (503) staff       (20)     1519 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/PR2.py
+-rw-rw----   0 pic        (503) staff       (20)     1725 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/Panda.py
+-rw-rw----   0 pic        (503) staff       (20)     3052 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/Puma560.py
+-rw-rw----   0 pic        (503) staff       (20)     1346 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/UR10.py
+-rw-rw----   0 pic        (503) staff       (20)     1339 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/UR3.py
+-rw-rw----   0 pic        (503) staff       (20)     1957 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/UR5.py
+-rw-rw----   0 pic        (503) staff       (20)     2749 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/Valkyrie.py
+-rw-rw----   0 pic        (503) staff       (20)     3245 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/YuMi.py
+-rw-r--r--   0 pic        (503) staff       (20)     1682 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/__init__.py
+-rw-rw----   0 pic        (503) staff       (20)     1435 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/px100.py
+-rw-rw----   0 pic        (503) staff       (20)     1438 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/px150.py
+-rw-rw----   0 pic        (503) staff       (20)     1438 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/rx150.py
+-rw-rw----   0 pic        (503) staff       (20)     1438 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/rx200.py
+-rw-rw----   0 pic        (503) staff       (20)     1438 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/vx300.py
+-rw-rw----   0 pic        (503) staff       (20)     1449 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/vx300s.py
+-rwxrwx---   0 pic        (503) staff       (20)     1438 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/wx200.py
+-rw-rw----   0 pic        (503) staff       (20)     1438 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/wx250.py
+-rw-rw----   0 pic        (503) staff       (20)     1449 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/wx250s.py
+-rw-r--r--   0 pic        (503) staff       (20)      222 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/__init__.py
+-rw-r--r--   0 pic        (503) staff       (20)     4146 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/models/list.py
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.725253 roboticstoolbox_python-1.1.1/roboticstoolbox/robot/
+-rw-rw----   0 pic        (503) staff       (20)    89944 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/robot/BaseRobot.py
+-rw-rw----   0 pic        (503) staff       (20)    16031 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/robot/DHFactor.py
+-rw-rw----   0 pic        (503) staff       (20)    28433 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/robot/DHLink.py
+-rw-rw----   0 pic        (503) staff       (20)    86411 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/robot/DHRobot.py
+-rw-rw----   0 pic        (503) staff       (20)    50606 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/robot/Dynamics.py
+-rw-r--r--   0 pic        (503) staff       (20)      525 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/robot/ELink.py
+-rw-rw----   0 pic        (503) staff       (20)      567 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/robot/ERobot.py
+-rw-rw----   0 pic        (503) staff       (20)    27949 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/robot/ET.py
+-rw-rw----   0 pic        (503) staff       (20)   110367 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/robot/ETS.py
+-rw-rw----   0 pic        (503) staff       (20)     7241 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/robot/Gripper.py
+-rw-rw----   0 pic        (503) staff       (20)    44773 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/robot/IK.py
+-rw-rw----   0 pic        (503) staff       (20)    46629 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/robot/Link.py
+-rw-rw----   0 pic        (503) staff       (20)     5201 2024-05-11 07:21:42.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/robot/PoERobot.py
+-rw-rw----   0 pic        (503) staff       (20)    66239 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/robot/Robot.py
+-rw-rw----   0 pic        (503) staff       (20)    61150 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/robot/RobotKinematics.py
+-rw-rw----   0 pic        (503) staff       (20)     2439 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/robot/RobotProto.py
+-rw-rw----   0 pic        (503) staff       (20)     1223 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/robot/__init__.py
+-rw-r--r--   0 pic        (503) staff       (20)     2925 2020-10-15 09:46:26.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/robot/symsimp.py
+-rw-r--r--   0 pic        (503) staff       (20)     1380 2020-10-13 09:43:13.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/robot/symsimp2.py
+-rw-r--r--   0 pic        (503) staff       (20)      155 2023-03-26 05:49:41.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/robot/test-plot.py
+-rw-r--r--   0 pic        (503) staff       (20)      221 2020-10-10 23:01:18.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/robot/test_fkine.py
+-rw-r--r--   0 pic        (503) staff       (20)     2871 2021-03-21 10:25:12.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/robot/test_invdyn.py
+-rw-r--r--   0 pic        (503) staff       (20)     1470 2021-06-27 07:29:41.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/robot/timing_dynamics.py
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.731455 roboticstoolbox_python-1.1.1/roboticstoolbox/tools/
+-rw-r--r--   0 pic        (503) staff       (20)    11529 2020-11-16 08:46:05.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/tools/DHFactor.py
+-rw-r--r--   0 pic        (503) staff       (20)     1201 2020-11-16 08:46:05.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/tools/Ticker.py
+-rw-rw----   0 pic        (503) staff       (20)     1335 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/tools/__init__.py
+-rw-rw----   0 pic        (503) staff       (20)     4886 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/tools/data.py
+-rw-r--r--   0 pic        (503) staff       (20)     1399 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/tools/jsingu.py
+-rw-r--r--   0 pic        (503) staff       (20)     1507 2020-11-16 06:09:43.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/tools/null.py
+-rw-r--r--   0 pic        (503) staff       (20)     2508 2020-12-22 09:05:39.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/tools/numerical.py
+-rw-rw----   0 pic        (503) staff       (20)     2764 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/tools/p_servo.py
+-rw-r--r--   0 pic        (503) staff       (20)      149 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/tools/params.py
+-rw-rw----   0 pic        (503) staff       (20)     2895 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/tools/plot.py
+-rw-rw----   0 pic        (503) staff       (20)    34205 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/tools/trajectory.py
+-rw-rw----   0 pic        (503) staff       (20)      243 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/tools/types.py
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.733518 roboticstoolbox_python-1.1.1/roboticstoolbox/tools/urdf/
+-rw-r--r--   0 pic        (503) staff       (20)      574 2020-11-09 03:39:53.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/tools/urdf/__init__.py
+-rw-r--r--   0 pic        (503) staff       (20)    59882 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/tools/urdf/urdf.py
+-rw-r--r--   0 pic        (503) staff       (20)     1483 2020-11-16 06:09:43.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/tools/urdf/utils.py
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.735808 roboticstoolbox_python-1.1.1/roboticstoolbox/tools/xacro/
+-rw-r--r--   0 pic        (503) staff       (20)    37597 2021-01-04 02:16:55.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/tools/xacro/__init__.py
+-rw-r--r--   0 pic        (503) staff       (20)     4713 2020-11-09 03:39:53.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/tools/xacro/cli.py
+-rw-r--r--   0 pic        (503) staff       (20)     2751 2020-11-09 03:39:53.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/tools/xacro/color.py
+-rw-r--r--   0 pic        (503) staff       (20)     5367 2020-11-09 03:39:52.000000 roboticstoolbox_python-1.1.1/roboticstoolbox/tools/xacro/xmlutils.py
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.752854 roboticstoolbox_python-1.1.1/roboticstoolbox_python.egg-info/
+-rw-r--r--   0 pic        (503) staff       (20)    19896 2024-05-11 10:56:55.000000 roboticstoolbox_python-1.1.1/roboticstoolbox_python.egg-info/PKG-INFO
+-rw-rw----   0 pic        (503) staff       (20)    28104 2024-05-11 10:56:55.000000 roboticstoolbox_python-1.1.1/roboticstoolbox_python.egg-info/SOURCES.txt
+-rw-rw----   0 pic        (503) staff       (20)        1 2024-05-11 10:56:55.000000 roboticstoolbox_python-1.1.1/roboticstoolbox_python.egg-info/dependency_links.txt
+-rw-rw----   0 pic        (503) staff       (20)      225 2024-05-11 10:56:55.000000 roboticstoolbox_python-1.1.1/roboticstoolbox_python.egg-info/entry_points.txt
+-rw-rw----   0 pic        (503) staff       (20)      351 2024-05-11 10:56:55.000000 roboticstoolbox_python-1.1.1/roboticstoolbox_python.egg-info/requires.txt
+-rw-rw----   0 pic        (503) staff       (20)       16 2024-05-11 10:56:55.000000 roboticstoolbox_python-1.1.1/roboticstoolbox_python.egg-info/top_level.txt
+-rw-rw----   0 pic        (503) staff       (20)       38 2024-05-11 10:56:55.774892 roboticstoolbox_python-1.1.1/setup.cfg
+-rw-rw----   0 pic        (503) staff       (20)     1074 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/setup.py
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-11 10:56:55.752194 roboticstoolbox_python-1.1.1/tests/
+-rw-rw----   0 pic        (503) staff       (20)    18692 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/tests/test_BaseRobot.py
+-rwxrwx---   0 pic        (503) staff       (20)     1816 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/tests/test_CustomXacro.py
+-rw-rw----   0 pic        (503) staff       (20)    47963 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/tests/test_DHRobot.py
+-rw-rw----   0 pic        (503) staff       (20)     9005 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/tests/test_ELink.py
+-rw-rw----   0 pic        (503) staff       (20)     7658 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/tests/test_ERobot.py
+-rw-rw----   0 pic        (503) staff       (20)    11833 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/tests/test_ET.py
+-rw-rw----   0 pic        (503) staff       (20)   160085 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/tests/test_ETS.py
+-rw-rw----   0 pic        (503) staff       (20)    13366 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/tests/test_ETS2.py
+-rw-rw----   0 pic        (503) staff       (20)     3870 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/tests/test_Gripper.py
+-rw-rw----   0 pic        (503) staff       (20)    18588 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/tests/test_IK.py
+-rw-rw----   0 pic        (503) staff       (20)     5298 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/tests/test_Link.py
+-rw-r--r--   0 pic        (503) staff       (20)     1059 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/tests/test_PyPlot.py
+-rw-r--r--   0 pic        (503) staff       (20)     1058 2021-03-10 06:37:56.000000 roboticstoolbox_python-1.1.1/tests/test_PyPlot2.py
+-rw-rw----   0 pic        (503) staff       (20)    47186 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/tests/test_Robot.py
+-rw-r--r--   0 pic        (503) staff       (20)      352 2020-11-16 08:46:05.000000 roboticstoolbox_python-1.1.1/tests/test_Ticker.py
+-rw-r--r--   0 pic        (503) staff       (20)    36283 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/tests/test_VPython.py
+-rw-rw----   0 pic        (503) staff       (20)    12516 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/tests/test_blocks.py
+-rw-r--r--   0 pic        (503) staff       (20)     2492 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/tests/test_fknm.py
+-rw-rw----   0 pic        (503) staff       (20)    12212 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/tests/test_jacob.py
+-rw-rw----   0 pic        (503) staff       (20)    14492 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/tests/test_mobile.py
+-rw-rw----   0 pic        (503) staff       (20)     5485 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/tests/test_mobile_planner.py
+-rw-r--r--   0 pic        (503) staff       (20)     2668 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/tests/test_models.py
+-rw-rw----   0 pic        (503) staff       (20)     2852 2023-11-11 22:02:44.000000 roboticstoolbox_python-1.1.1/tests/test_tools.py
+-rw-r--r--   0 pic        (503) staff       (20)    20275 2022-09-20 06:23:02.000000 roboticstoolbox_python-1.1.1/tests/test_trajectory.py
```

### Comparing `roboticstoolbox-python-1.1.0/LICENSE` & `roboticstoolbox_python-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/PKG-INFO` & `roboticstoolbox_python-1.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,53 +1,7 @@
-Metadata-Version: 2.1
-Name: roboticstoolbox-python
-Version: 1.1.0
-Summary: A Python library for robotics education and research
-Author-email: Jesse Haviland <j.haviland@qut.edu.au>, Peter Corke <rvc@petercorke.com>
-License: MIT License
-        
-        Copyright (c) 2020 jhavl
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: homepage, https://github.com/petercorke/robotics-toolbox-python
-Project-URL: documentation, https://petercorke.github.io/robotics-toolbox-python/
-Project-URL: repository, https://github.com/petercorke/robotics-toolbox-python
-Keywords: python,robotics,robotics-toolbox,kinematics,dynamics,motion-planning,trajectory-generation,jacobian,hessian,control,simulation,robot-manipulator,mobile-robot
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: collision
-Provides-Extra: dev
-Provides-Extra: docs
-License-File: LICENSE
-
 # Robotics Toolbox for Python
 
 [![A Python Robotics Package](https://raw.githubusercontent.com/petercorke/robotics-toolbox-python/master/.github/svg/py_collection.min.svg)](https://github.com/petercorke/robotics-toolbox-python)
 [![Powered by Spatial Maths](https://raw.githubusercontent.com/petercorke/spatialmath-python/master/.github/svg/sm_powered.min.svg)](https://github.com/petercorke/spatialmath-python)
 [![QUT Centre for Robotics Open Source](https://github.com/qcr/qcr.github.io/raw/master/misc/badge.svg)](https://qcr.github.io)
 
 [![PyPI version](https://badge.fury.io/py/roboticstoolbox-python.svg)](https://badge.fury.io/py/roboticstoolbox-python)
@@ -239,15 +193,15 @@
 defined in terms of position and orientation (end-effector z-axis down (A=-Z) and finger
 orientation parallel to y-axis (O=+Y)).
 
 ```python
 from spatialmath import SE3
 
 Tep = SE3.Trans(0.6, -0.3, 0.1) * SE3.OA([0, 1, 0], [0, 0, -1])
-sol = robot.ik_lm_chan(Tep)         # solve IK
+sol = robot.ik_LM(Tep)         # solve IK
 print(sol)
 
 	(array([ 0.20592815,  0.86609481, -0.79473206, -1.68254794,  0.74872915,
 			2.21764746, -0.10255606]), 1, 114, 7, 2.890164057230228e-07)
 
 q_pickup = sol[0]
 print(robot.fkine(q_pickup))    # FK shows that desired end-effector pose was achieved
@@ -281,34 +235,34 @@
 	<img src="./docs/figs/panda2.gif">
 </p>
 
 We can also experiment with velocity controllers in Swift. Here is a resolved-rate motion control example
 
 ```python
 import swift
-import roboticstoolbox as rp
+import roboticstoolbox as rtb
 import spatialmath as sm
 import numpy as np
 
 env = swift.Swift()
 env.launch(realtime=True)
 
-panda = rp.models.Panda()
+panda = rtb.models.Panda()
 panda.q = panda.qr
 
 Tep = panda.fkine(panda.q) * sm.SE3.Trans(0.2, 0.2, 0.45)
 
 arrived = False
 env.add(panda)
 
 dt = 0.05
 
 while not arrived:
 
-    v, arrived = rp.p_servo(panda.fkine(panda.q), Tep, 1)
+    v, arrived = rtb.p_servo(panda.fkine(panda.q), Tep, 1)
     panda.qd = np.linalg.pinv(panda.jacobe(panda.q)) @ v
     env.step(dt)
 
 # Uncomment to stop the browser tab from closing
 # env.hold()
 ```
```

#### html2text {}

```diff
@@ -1,58 +1,28 @@
-Metadata-Version: 2.1 Name: roboticstoolbox-python Version: 1.1.0 Summary: A
-Python library for robotics education and research Author-email: Jesse Haviland
-qut.edu.au>, Peter Corke
-petercorke.com> License: MIT License Copyright (c) 2020 jhavl Permission is
-hereby granted, free of charge, to any person obtaining a copy of this software
-and associated documentation files (the "Software"), to deal in the Software
-without restriction, including without limitation the rights to use, copy,
-modify, merge, publish, distribute, sublicense, and/or sell copies of the
-Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions: The above copyright notice and this
-permission notice shall be included in all copies or substantial portions of
-the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
-EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
-OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
-ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE. Project-URL: homepage, https://github.com/petercorke/
-robotics-toolbox-python Project-URL: documentation, https://
-petercorke.github.io/robotics-toolbox-python/ Project-URL: repository, https://
-github.com/petercorke/robotics-toolbox-python Keywords:
-python,robotics,robotics-toolbox,kinematics,dynamics,motion-
-planning,trajectory-generation,jacobian,hessian,control,simulation,robot-
-manipulator,mobile-robot Classifier: Development Status :: 5 - Production/
-Stable Classifier: Intended Audience :: Developers Classifier: License :: OSI
-Approved :: MIT License Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.7
-Description-Content-Type: text/markdown Provides-Extra: collision Provides-
-Extra: dev Provides-Extra: docs License-File: LICENSE # Robotics Toolbox for
-Python [![A Python Robotics Package](https://raw.githubusercontent.com/
-petercorke/robotics-toolbox-python/master/.github/svg/py_collection.min.svg)]
-(https://github.com/petercorke/robotics-toolbox-python) [![Powered by Spatial
-Maths](https://raw.githubusercontent.com/petercorke/spatialmath-python/
-master/.github/svg/sm_powered.min.svg)](https://github.com/petercorke/
-spatialmath-python) [![QUT Centre for Robotics Open Source](https://github.com/
-qcr/qcr.github.io/raw/master/misc/badge.svg)](https://qcr.github.io) [![PyPI
-version](https://badge.fury.io/py/roboticstoolbox-python.svg)](https://
-badge.fury.io/py/roboticstoolbox-python) [![Anaconda version](https://
-anaconda.org/conda-forge/roboticstoolbox-python/badges/version.svg)](https://
-anaconda.org/conda-forge/roboticstoolbox-python) ![PyPI - Python Version]
-(https://img.shields.io/pypi/pyversions/roboticstoolbox-python.svg) [![Build
-Status](https://github.com/petercorke/robotics-toolbox-python/workflows/Test/
-badge.svg?branch=master)](https://github.com/petercorke/robotics-toolbox-
-python/actions?query=workflow%3ATest) [![Coverage](https://codecov.io/gh/
-petercorke/robotics-toolbox-python/branch/master/graph/badge.svg)](https://
-codecov.io/gh/petercorke/robotics-toolbox-python) [![PyPI - Downloads](https://
-img.shields.io/pypi/dw/roboticstoolbox-python)](https://pypistats.org/packages/
-roboticstoolbox-python) [![License: MIT](https://img.shields.io/badge/License-
-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+# Robotics Toolbox for Python [![A Python Robotics Package](https://
+raw.githubusercontent.com/petercorke/robotics-toolbox-python/master/.github/
+svg/py_collection.min.svg)](https://github.com/petercorke/robotics-toolbox-
+python) [![Powered by Spatial Maths](https://raw.githubusercontent.com/
+petercorke/spatialmath-python/master/.github/svg/sm_powered.min.svg)](https://
+github.com/petercorke/spatialmath-python) [![QUT Centre for Robotics Open
+Source](https://github.com/qcr/qcr.github.io/raw/master/misc/badge.svg)](https:
+//qcr.github.io) [![PyPI version](https://badge.fury.io/py/roboticstoolbox-
+python.svg)](https://badge.fury.io/py/roboticstoolbox-python) [![Anaconda
+version](https://anaconda.org/conda-forge/roboticstoolbox-python/badges/
+version.svg)](https://anaconda.org/conda-forge/roboticstoolbox-python) ![PyPI -
+Python Version](https://img.shields.io/pypi/pyversions/roboticstoolbox-
+python.svg) [![Build Status](https://github.com/petercorke/robotics-toolbox-
+python/workflows/Test/badge.svg?branch=master)](https://github.com/petercorke/
+robotics-toolbox-python/actions?query=workflow%3ATest) [![Coverage](https://
+codecov.io/gh/petercorke/robotics-toolbox-python/branch/master/graph/
+badge.svg)](https://codecov.io/gh/petercorke/robotics-toolbox-python) [![PyPI -
+Downloads](https://img.shields.io/pypi/dw/roboticstoolbox-python)](https://
+pypistats.org/packages/roboticstoolbox-python) [![License: MIT](https://
+img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/
+MIT)
                                      A Python implementation of the _R_o_b_o_t_i_c_s
 [https://github.com/petercorke/      _T_o_o_l_b_o_x_ _f_o_r_ _M_A_T_L_A_B_®
 robotics-toolbox-python/raw/master/      * _G_i_t_H_u_b_ _r_e_p_o_s_i_t_o_r_y
 docs/figs/RobToolBox_RoundLogoB.png]     * _D_o_c_u_m_e_n_t_a_t_i_o_n
                                          * _I_C_R_A_ _P_a_p_e_r
                                          * _W_i_k_i_ _(_e_x_a_m_p_l_e_s_ _a_n_d_ _d_e_t_a_i_l_s_)
 ## Contents - [Synopsis](#1) - [Getting going](#2) - [Tutorials](#3) - [Code
@@ -139,34 +109,34 @@
 code, console output is indented). We will compute the forward kinematics next
 ``` Te = robot.fkine(robot.qr) # forward kinematics print(Te) 0.995 0 0.09983
 0.484 0 -1 0 0 0.09983 0 -0.995 0.4126 0 0 0 1 ``` We can solve inverse
 kinematics very easily. We first choose an SE(3) pose defined in terms of
 position and orientation (end-effector z-axis down (A=-Z) and finger
 orientation parallel to y-axis (O=+Y)). ```python from spatialmath import SE3
 Tep = SE3.Trans(0.6, -0.3, 0.1) * SE3.OA([0, 1, 0], [0, 0, -1]) sol =
-robot.ik_lm_chan(Tep) # solve IK print(sol) (array([ 0.20592815, 0.86609481, -
+robot.ik_LM(Tep) # solve IK print(sol) (array([ 0.20592815, 0.86609481, -
 0.79473206, -1.68254794, 0.74872915, 2.21764746, -0.10255606]), 1, 114, 7,
 2.890164057230228e-07) q_pickup = sol[0] print(robot.fkine(q_pickup)) # FK
 shows that desired end-effector pose was achieved 1 -8.913e-05 -0.0003334
 0.5996 -8.929e-05 -1 -0.0004912 -0.2998 -0.0003334 0.0004912 -1 0.1001 0 0 0 1
 ``` We can animate a path from the ready pose `qr` configuration to this pickup
 configuration ```python qt = rtb.jtraj(robot.qr, q_pickup, 50) robot.plot(qt.q,
 backend='pyplot', movie='panda1.gif') ```
                            [./docs/figs/panda1.gif]
 where we have specified the matplotlib `pyplot` backend. Blue arrows show the
 joint axes and the coloured frame shows the end-effector pose. We can also plot
 the trajectory in the Swift simulator (a browser-based 3d-simulation
 environment built to work with the Toolbox) ```python robot.plot(qt.q) ```
                            [./docs/figs/panda2.gif]
 We can also experiment with velocity controllers in Swift. Here is a resolved-
-rate motion control example ```python import swift import roboticstoolbox as rp
-import spatialmath as sm import numpy as np env = swift.Swift() env.launch
-(realtime=True) panda = rp.models.Panda() panda.q = panda.qr Tep = panda.fkine
+rate motion control example ```python import swift import roboticstoolbox as
+rtb import spatialmath as sm import numpy as np env = swift.Swift() env.launch
+(realtime=True) panda = rtb.models.Panda() panda.q = panda.qr Tep = panda.fkine
 (panda.q) * sm.SE3.Trans(0.2, 0.2, 0.45) arrived = False env.add(panda) dt =
-0.05 while not arrived: v, arrived = rp.p_servo(panda.fkine(panda.q), Tep, 1)
+0.05 while not arrived: v, arrived = rtb.p_servo(panda.fkine(panda.q), Tep, 1)
 panda.qd = np.linalg.pinv(panda.jacobe(panda.q)) @ v env.step(dt) # Uncomment
 to stop the browser tab from closing # env.hold() ```
                            [./docs/figs/panda3.gif]
 ### Run some examples The [`notebooks`](https://github.com/petercorke/robotics-
 toolbox-python/tree/master/notebooks) folder contains some tutorial Jupyter
 notebooks which you can browse on GitHub. Additionally, have a look in the
 [`examples`](https://github.com/petercorke/robotics-toolbox-python/tree/master/
```

### Comparing `roboticstoolbox-python-1.1.0/README.md` & `roboticstoolbox_python-1.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,1031 +1,1244 @@
-00000000: 2320 526f 626f 7469 6373 2054 6f6f 6c62  # Robotics Toolb
-00000010: 6f78 2066 6f72 2050 7974 686f 6e0a 0a5b  ox for Python..[
-00000020: 215b 4120 5079 7468 6f6e 2052 6f62 6f74  ![A Python Robot
-00000030: 6963 7320 5061 636b 6167 655d 2868 7474  ics Package](htt
-00000040: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
-00000050: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f70  sercontent.com/p
-00000060: 6574 6572 636f 726b 652f 726f 626f 7469  etercorke/roboti
-00000070: 6373 2d74 6f6f 6c62 6f78 2d70 7974 686f  cs-toolbox-pytho
-00000080: 6e2f 6d61 7374 6572 2f2e 6769 7468 7562  n/master/.github
-00000090: 2f73 7667 2f70 795f 636f 6c6c 6563 7469  /svg/py_collecti
-000000a0: 6f6e 2e6d 696e 2e73 7667 295d 2868 7474  on.min.svg)](htt
-000000b0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000000c0: 7065 7465 7263 6f72 6b65 2f72 6f62 6f74  petercorke/robot
-000000d0: 6963 732d 746f 6f6c 626f 782d 7079 7468  ics-toolbox-pyth
-000000e0: 6f6e 290a 5b21 5b50 6f77 6572 6564 2062  on).[![Powered b
-000000f0: 7920 5370 6174 6961 6c20 4d61 7468 735d  y Spatial Maths]
-00000100: 2868 7474 7073 3a2f 2f72 6177 2e67 6974  (https://raw.git
-00000110: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-00000120: 6f6d 2f70 6574 6572 636f 726b 652f 7370  om/petercorke/sp
-00000130: 6174 6961 6c6d 6174 682d 7079 7468 6f6e  atialmath-python
-00000140: 2f6d 6173 7465 722f 2e67 6974 6875 622f  /master/.github/
-00000150: 7376 672f 736d 5f70 6f77 6572 6564 2e6d  svg/sm_powered.m
-00000160: 696e 2e73 7667 295d 2868 7474 7073 3a2f  in.svg)](https:/
-00000170: 2f67 6974 6875 622e 636f 6d2f 7065 7465  /github.com/pete
-00000180: 7263 6f72 6b65 2f73 7061 7469 616c 6d61  rcorke/spatialma
-00000190: 7468 2d70 7974 686f 6e29 0a5b 215b 5155  th-python).[![QU
-000001a0: 5420 4365 6e74 7265 2066 6f72 2052 6f62  T Centre for Rob
-000001b0: 6f74 6963 7320 4f70 656e 2053 6f75 7263  otics Open Sourc
-000001c0: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
-000001d0: 622e 636f 6d2f 7163 722f 7163 722e 6769  b.com/qcr/qcr.gi
-000001e0: 7468 7562 2e69 6f2f 7261 772f 6d61 7374  thub.io/raw/mast
-000001f0: 6572 2f6d 6973 632f 6261 6467 652e 7376  er/misc/badge.sv
-00000200: 6729 5d28 6874 7470 733a 2f2f 7163 722e  g)](https://qcr.
-00000210: 6769 7468 7562 2e69 6f29 0a0a 5b21 5b50  github.io)..[![P
-00000220: 7950 4920 7665 7273 696f 6e5d 2868 7474  yPI version](htt
-00000230: 7073 3a2f 2f62 6164 6765 2e66 7572 792e  ps://badge.fury.
-00000240: 696f 2f70 792f 726f 626f 7469 6373 746f  io/py/roboticsto
-00000250: 6f6c 626f 782d 7079 7468 6f6e 2e73 7667  olbox-python.svg
-00000260: 295d 2868 7474 7073 3a2f 2f62 6164 6765  )](https://badge
-00000270: 2e66 7572 792e 696f 2f70 792f 726f 626f  .fury.io/py/robo
-00000280: 7469 6373 746f 6f6c 626f 782d 7079 7468  ticstoolbox-pyth
-00000290: 6f6e 290a 5b21 5b41 6e61 636f 6e64 6120  on).[![Anaconda 
-000002a0: 7665 7273 696f 6e5d 2868 7474 7073 3a2f  version](https:/
-000002b0: 2f61 6e61 636f 6e64 612e 6f72 672f 636f  /anaconda.org/co
-000002c0: 6e64 612d 666f 7267 652f 726f 626f 7469  nda-forge/roboti
-000002d0: 6373 746f 6f6c 626f 782d 7079 7468 6f6e  cstoolbox-python
-000002e0: 2f62 6164 6765 732f 7665 7273 696f 6e2e  /badges/version.
-000002f0: 7376 6729 5d28 6874 7470 733a 2f2f 616e  svg)](https://an
-00000300: 6163 6f6e 6461 2e6f 7267 2f63 6f6e 6461  aconda.org/conda
-00000310: 2d66 6f72 6765 2f72 6f62 6f74 6963 7374  -forge/roboticst
-00000320: 6f6f 6c62 6f78 2d70 7974 686f 6e29 0a21  oolbox-python).!
-00000330: 5b50 7950 4920 2d20 5079 7468 6f6e 2056  [PyPI - Python V
-00000340: 6572 7369 6f6e 5d28 6874 7470 733a 2f2f  ersion](https://
-00000350: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
-00000360: 7970 692f 7079 7665 7273 696f 6e73 2f72  ypi/pyversions/r
-00000370: 6f62 6f74 6963 7374 6f6f 6c62 6f78 2d70  oboticstoolbox-p
-00000380: 7974 686f 6e2e 7376 6729 0a0a 5b21 5b42  ython.svg)..[![B
-00000390: 7569 6c64 2053 7461 7475 735d 2868 7474  uild Status](htt
-000003a0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000003b0: 7065 7465 7263 6f72 6b65 2f72 6f62 6f74  petercorke/robot
-000003c0: 6963 732d 746f 6f6c 626f 782d 7079 7468  ics-toolbox-pyth
-000003d0: 6f6e 2f77 6f72 6b66 6c6f 7773 2f54 6573  on/workflows/Tes
-000003e0: 742f 6261 6467 652e 7376 673f 6272 616e  t/badge.svg?bran
-000003f0: 6368 3d6d 6173 7465 7229 5d28 6874 7470  ch=master)](http
-00000400: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
-00000410: 6574 6572 636f 726b 652f 726f 626f 7469  etercorke/roboti
-00000420: 6373 2d74 6f6f 6c62 6f78 2d70 7974 686f  cs-toolbox-pytho
-00000430: 6e2f 6163 7469 6f6e 733f 7175 6572 793d  n/actions?query=
-00000440: 776f 726b 666c 6f77 2533 4154 6573 7429  workflow%3ATest)
-00000450: 0a5b 215b 436f 7665 7261 6765 5d28 6874  .[![Coverage](ht
-00000460: 7470 733a 2f2f 636f 6465 636f 762e 696f  tps://codecov.io
-00000470: 2f67 682f 7065 7465 7263 6f72 6b65 2f72  /gh/petercorke/r
-00000480: 6f62 6f74 6963 732d 746f 6f6c 626f 782d  obotics-toolbox-
-00000490: 7079 7468 6f6e 2f62 7261 6e63 682f 6d61  python/branch/ma
-000004a0: 7374 6572 2f67 7261 7068 2f62 6164 6765  ster/graph/badge
-000004b0: 2e73 7667 295d 2868 7474 7073 3a2f 2f63  .svg)](https://c
-000004c0: 6f64 6563 6f76 2e69 6f2f 6768 2f70 6574  odecov.io/gh/pet
-000004d0: 6572 636f 726b 652f 726f 626f 7469 6373  ercorke/robotics
-000004e0: 2d74 6f6f 6c62 6f78 2d70 7974 686f 6e29  -toolbox-python)
-000004f0: 0a5b 215b 5079 5049 202d 2044 6f77 6e6c  .[![PyPI - Downl
-00000500: 6f61 6473 5d28 6874 7470 733a 2f2f 696d  oads](https://im
-00000510: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
-00000520: 692f 6477 2f72 6f62 6f74 6963 7374 6f6f  i/dw/roboticstoo
-00000530: 6c62 6f78 2d70 7974 686f 6e29 5d28 6874  lbox-python)](ht
-00000540: 7470 733a 2f2f 7079 7069 7374 6174 732e  tps://pypistats.
-00000550: 6f72 672f 7061 636b 6167 6573 2f72 6f62  org/packages/rob
-00000560: 6f74 6963 7374 6f6f 6c62 6f78 2d70 7974  oticstoolbox-pyt
-00000570: 686f 6e29 0a5b 215b 4c69 6365 6e73 653a  hon).[![License:
-00000580: 204d 4954 5d28 6874 7470 733a 2f2f 696d   MIT](https://im
-00000590: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-000005a0: 6765 2f4c 6963 656e 7365 2d4d 4954 2d79  ge/License-MIT-y
-000005b0: 656c 6c6f 772e 7376 6729 5d28 6874 7470  ellow.svg)](http
-000005c0: 733a 2f2f 6f70 656e 736f 7572 6365 2e6f  s://opensource.o
-000005d0: 7267 2f6c 6963 656e 7365 732f 4d49 5429  rg/licenses/MIT)
-000005e0: 0a0a 3c74 6162 6c65 2073 7479 6c65 3d22  ..<table style="
-000005f0: 626f 7264 6572 3a30 7078 223e 0a3c 7472  border:0px">.<tr
-00000600: 2073 7479 6c65 3d22 626f 7264 6572 3a30   style="border:0
-00000610: 7078 223e 0a3c 7464 2073 7479 6c65 3d22  px">.<td style="
-00000620: 626f 7264 6572 3a30 7078 223e 0a3c 696d  border:0px">.<im
-00000630: 6720 7372 633d 2268 7474 7073 3a2f 2f67  g src="https://g
-00000640: 6974 6875 622e 636f 6d2f 7065 7465 7263  ithub.com/peterc
-00000650: 6f72 6b65 2f72 6f62 6f74 6963 732d 746f  orke/robotics-to
-00000660: 6f6c 626f 782d 7079 7468 6f6e 2f72 6177  olbox-python/raw
-00000670: 2f6d 6173 7465 722f 646f 6373 2f66 6967  /master/docs/fig
-00000680: 732f 526f 6254 6f6f 6c42 6f78 5f52 6f75  s/RobToolBox_Rou
-00000690: 6e64 4c6f 676f 422e 706e 6722 2077 6964  ndLogoB.png" wid
-000006a0: 7468 3d22 3230 3022 3e3c 2f74 643e 0a3c  th="200"></td>.<
-000006b0: 7464 2073 7479 6c65 3d22 626f 7264 6572  td style="border
-000006c0: 3a30 7078 223e 0a41 2050 7974 686f 6e20  :0px">.A Python 
-000006d0: 696d 706c 656d 656e 7461 7469 6f6e 206f  implementation o
-000006e0: 6620 7468 6520 3c61 2068 7265 663d 2268  f the <a href="h
-000006f0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000700: 6d2f 7065 7465 7263 6f72 6b65 2f72 6f62  m/petercorke/rob
-00000710: 6f74 6963 732d 746f 6f6c 626f 782d 6d61  otics-toolbox-ma
-00000720: 746c 6162 223e 526f 626f 7469 6373 2054  tlab">Robotics T
-00000730: 6f6f 6c62 6f78 2066 6f72 204d 4154 4c41  oolbox for MATLA
-00000740: 423c 7375 703e 2672 6567 3b3c 2f73 7570  B<sup>&reg;</sup
-00000750: 3e3c 2f61 3e0a 3c75 6c3e 0a3c 6c69 3e3c  ></a>.<ul>.<li><
-00000760: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00000770: 6769 7468 7562 2e63 6f6d 2f70 6574 6572  github.com/peter
-00000780: 636f 726b 652f 726f 626f 7469 6373 2d74  corke/robotics-t
-00000790: 6f6f 6c62 6f78 2d70 7974 686f 6e22 3e47  oolbox-python">G
-000007a0: 6974 4875 6220 7265 706f 7369 746f 7279  itHub repository
-000007b0: 203c 2f61 3e3c 2f6c 693e 0a3c 6c69 3e3c   </a></li>.<li><
-000007c0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-000007d0: 7065 7465 7263 6f72 6b65 2e67 6974 6875  petercorke.githu
-000007e0: 622e 696f 2f72 6f62 6f74 6963 732d 746f  b.io/robotics-to
-000007f0: 6f6c 626f 782d 7079 7468 6f6e 223e 446f  olbox-python">Do
-00000800: 6375 6d65 6e74 6174 696f 6e3c 2f61 3e3c  cumentation</a><
-00000810: 2f6c 693e 0a3c 6c69 3e3c 6120 6872 6566  /li>.<li><a href
-00000820: 3d22 2336 223e 4943 5241 2050 6170 6572  ="#6">ICRA Paper
-00000830: 3c2f 613e 3c2f 6c69 3e0a 3c6c 693e 3c61  </a></li>.<li><a
-00000840: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
-00000850: 6974 6875 622e 636f 6d2f 7065 7465 7263  ithub.com/peterc
-00000860: 6f72 6b65 2f72 6f62 6f74 6963 732d 746f  orke/robotics-to
-00000870: 6f6c 626f 782d 7079 7468 6f6e 2f77 696b  olbox-python/wik
-00000880: 6922 3e57 696b 6920 2865 7861 6d70 6c65  i">Wiki (example
-00000890: 7320 616e 6420 6465 7461 696c 7329 3c2f  s and details)</
-000008a0: 613e 3c2f 6c69 3e0a 3c2f 756c 3e0a 3c2f  a></li>.</ul>.</
-000008b0: 7464 3e0a 3c2f 7472 3e0a 3c2f 7461 626c  td>.</tr>.</tabl
-000008c0: 653e 0a0a 3c21 2d2d 203c 6272 3e20 2d2d  e>..<!-- <br> --
-000008d0: 3e0a 0a23 2320 436f 6e74 656e 7473 0a0a  >..## Contents..
-000008e0: 2d20 5b53 796e 6f70 7369 735d 2823 3129  - [Synopsis](#1)
-000008f0: 0a2d 205b 4765 7474 696e 6720 676f 696e  .- [Getting goin
-00000900: 675d 2823 3229 0a2d 205b 5475 746f 7269  g](#2).- [Tutori
-00000910: 616c 735d 2823 3329 0a2d 205b 436f 6465  als](#3).- [Code
-00000920: 2045 7861 6d70 6c65 735d 2823 3429 0a2d   Examples](#4).-
-00000930: 205b 546f 6f6c 626f 7820 5265 7365 6172   [Toolbox Resear
-00000940: 6368 2041 7070 6c69 6361 7469 6f6e 735d  ch Applications]
-00000950: 2823 3529 0a2d 205b 546f 6f6c 626f 7820  (#5).- [Toolbox 
-00000960: 4943 5241 2050 6170 6572 2061 6e64 2043  ICRA Paper and C
-00000970: 6974 6174 696f 6e20 496e 666f 5d28 2336  itation Info](#6
-00000980: 290a 2d20 5b55 7369 6e67 2074 6865 2054  ).- [Using the T
-00000990: 6f6f 6c62 6f78 2069 6e20 796f 7572 204f  oolbox in your O
-000009a0: 7065 6e20 536f 7572 6365 2043 6f64 653f  pen Source Code?
-000009b0: 5d28 2337 290a 2d20 5b43 6f6d 6d6f 6e20  ](#7).- [Common 
-000009c0: 4973 7375 6573 2061 6e64 2053 6f6c 7574  Issues and Solut
-000009d0: 696f 6e73 5d28 2338 290a 0a3c 6272 3e0a  ions](#8)..<br>.
-000009e0: 0a3c 6120 6964 3d27 3127 3e3c 2f61 3e0a  .<a id='1'></a>.
-000009f0: 0a23 2320 5379 6e6f 7073 6973 0a0a 5468  .## Synopsis..Th
-00000a00: 6973 2074 6f6f 6c62 6f78 2062 7269 6e67  is toolbox bring
-00000a10: 7320 726f 626f 7469 6373 2d73 7065 6369  s robotics-speci
-00000a20: 6669 6320 6675 6e63 7469 6f6e 616c 6974  fic functionalit
-00000a30: 7920 746f 2050 7974 686f 6e2c 2061 6e64  y to Python, and
-00000a40: 206c 6576 6572 6167 6573 0a50 7974 686f   leverages.Pytho
-00000a50: 6e27 7320 6164 7661 6e74 6167 6573 206f  n's advantages o
-00000a60: 6620 706f 7274 6162 696c 6974 792c 2075  f portability, u
-00000a70: 6269 7175 6974 7920 616e 6420 7375 7070  biquity and supp
-00000a80: 6f72 742c 2061 6e64 2074 6865 2063 6170  ort, and the cap
-00000a90: 6162 696c 6974 7920 6f66 0a74 6865 206f  ability of.the o
-00000aa0: 7065 6e2d 736f 7572 6365 2065 636f 7379  pen-source ecosy
-00000ab0: 7374 656d 2066 6f72 206c 696e 6561 7220  stem for linear 
-00000ac0: 616c 6765 6272 6120 286e 756d 7079 2c20  algebra (numpy, 
-00000ad0: 7363 6970 7929 2c20 6772 6170 6869 6373  scipy), graphics
-00000ae0: 0a28 6d61 7470 6c6f 746c 6962 2c20 7468  .(matplotlib, th
-00000af0: 7265 652e 6a73 2c20 5765 6247 4c29 2c20  ree.js, WebGL), 
-00000b00: 696e 7465 7261 6374 6976 6520 6465 7665  interactive deve
-00000b10: 6c6f 706d 656e 7420 286a 7570 7974 6572  lopment (jupyter
-00000b20: 2c20 6a75 7079 7465 726c 6162 2c0a 6d79  , jupyterlab,.my
-00000b30: 6269 6e64 6572 2e6f 7267 292c 2061 6e64  binder.org), and
-00000b40: 2064 6f63 756d 656e 7461 7469 6f6e 2028   documentation (
-00000b50: 7370 6869 6e78 292e 0a0a 5468 6520 546f  sphinx)...The To
-00000b60: 6f6c 626f 7820 7072 6f76 6964 6573 2074  olbox provides t
-00000b70: 6f6f 6c73 2066 6f72 2072 6570 7265 7365  ools for represe
-00000b80: 6e74 696e 6720 7468 6520 6b69 6e65 6d61  nting the kinema
-00000b90: 7469 6373 2061 6e64 2064 796e 616d 6963  tics and dynamic
-00000ba0: 7320 6f66 0a73 6572 6961 6c2d 6c69 6e6b  s of.serial-link
-00000bb0: 206d 616e 6970 756c 6174 6f72 7320 2d20   manipulators - 
-00000bc0: 796f 7520 6361 6e20 6561 7369 6c79 2063  you can easily c
-00000bd0: 7265 6174 6520 796f 7572 206f 776e 2069  reate your own i
-00000be0: 6e20 4465 6e61 7669 742d 4861 7274 656e  n Denavit-Harten
-00000bf0: 6265 7267 0a66 6f72 6d2c 2069 6d70 6f72  berg.form, impor
-00000c00: 7420 6120 5552 4446 2066 696c 652c 206f  t a URDF file, o
-00000c10: 7220 7573 6520 6f76 6572 2033 3020 7375  r use over 30 su
-00000c20: 7070 6c69 6564 206d 6f64 656c 7320 666f  pplied models fo
-00000c30: 7220 7765 6c6c 2d6b 6e6f 776e 0a63 6f6e  r well-known.con
-00000c40: 7465 6d70 6f72 6172 7920 726f 626f 7473  temporary robots
-00000c50: 2066 726f 6d20 4672 616e 6b61 2d45 6d69   from Franka-Emi
-00000c60: 6b61 2c20 4b69 6e6f 7661 2c20 556e 6976  ka, Kinova, Univ
-00000c70: 6572 7361 6c20 526f 626f 7469 6373 2c20  ersal Robotics, 
-00000c80: 5265 7468 696e 6b20 6173 0a77 656c 6c20  Rethink as.well 
-00000c90: 6173 2063 6c61 7373 6963 616c 2072 6f62  as classical rob
-00000ca0: 6f74 7320 7375 6368 2061 7320 7468 6520  ots such as the 
-00000cb0: 5075 6d61 2035 3630 2061 6e64 2074 6865  Puma 560 and the
-00000cc0: 2053 7461 6e66 6f72 6420 6172 6d2e 0a0a   Stanford arm...
-00000cd0: 5468 6520 546f 6f6c 626f 7820 636f 6e74  The Toolbox cont
-00000ce0: 6169 6e73 2066 6173 7420 696d 706c 656d  ains fast implem
-00000cf0: 656e 7461 7469 6f6e 7320 6f66 206b 696e  entations of kin
-00000d00: 656d 6174 6963 206f 7065 7261 7469 6f6e  ematic operation
-00000d10: 732e 2054 6865 2066 6f72 7761 7264 0a6b  s. The forward.k
-00000d20: 696e 656d 6174 6963 7320 616e 6420 7468  inematics and th
-00000d30: 6520 6d61 6e69 7075 6c61 746f 7220 4a61  e manipulator Ja
-00000d40: 636f 6269 616e 2063 616e 2062 6520 636f  cobian can be co
-00000d50: 6d70 7574 6564 2069 6e20 6c65 7373 2074  mputed in less t
-00000d60: 6861 6e20 3120 6d69 6372 6f73 6563 6f6e  han 1 microsecon
-00000d70: 640a 7768 696c 6520 6e75 6d65 7269 6361  d.while numerica
-00000d80: 6c20 696e 7665 7273 6520 6b69 6e65 6d61  l inverse kinema
-00000d90: 7469 6373 2063 616e 2062 6520 736f 6c76  tics can be solv
-00000da0: 6564 2069 6e20 6173 206c 6974 746c 6520  ed in as little 
-00000db0: 6173 2034 206d 6963 726f 7365 636f 6e64  as 4 microsecond
-00000dc0: 732e 0a0a 5468 6520 746f 6f6c 626f 7820  s...The toolbox 
-00000dd0: 616c 736f 2073 7570 706f 7274 7320 6d6f  also supports mo
-00000de0: 6269 6c65 2072 6f62 6f74 7320 7769 7468  bile robots with
-00000df0: 2066 756e 6374 696f 6e73 2066 6f72 2072   functions for r
-00000e00: 6f62 6f74 206d 6f74 696f 6e20 6d6f 6465  obot motion mode
-00000e10: 6c73 0a28 756e 6963 7963 6c65 2c20 6269  ls.(unicycle, bi
-00000e20: 6379 636c 6529 2c20 7061 7468 2070 6c61  cycle), path pla
-00000e30: 6e6e 696e 6720 616c 676f 7269 7468 6d73  nning algorithms
-00000e40: 2028 6275 672c 2064 6973 7461 6e63 6520   (bug, distance 
-00000e50: 7472 616e 7366 6f72 6d2c 2044 5c2a 2c0a  transform, D\*,.
-00000e60: 5052 4d29 2c20 6b69 6e6f 6479 6e61 6d69  PRM), kinodynami
-00000e70: 6320 706c 616e 6e69 6e67 2028 6c61 7474  c planning (latt
-00000e80: 6963 652c 2052 5254 292c 206c 6f63 616c  ice, RRT), local
-00000e90: 697a 6174 696f 6e20 2845 4b46 2c20 7061  ization (EKF, pa
-00000ea0: 7274 6963 6c65 2066 696c 7465 7229 2c0a  rticle filter),.
-00000eb0: 6d61 7020 6275 696c 6469 6e67 2028 454b  map building (EK
-00000ec0: 4629 2061 6e64 2073 696d 756c 7461 6e65  F) and simultane
-00000ed0: 6f75 7320 6c6f 6361 6c69 7a61 7469 6f6e  ous localization
-00000ee0: 2061 6e64 206d 6170 7069 6e67 2028 454b   and mapping (EK
-00000ef0: 4629 2e0a 0a54 6865 2054 6f6f 6c62 6f78  F)...The Toolbox
-00000f00: 2070 726f 7669 6465 733a 0a0a 2d20 636f   provides:..- co
-00000f10: 6465 2074 6861 7420 6973 206d 6174 7572  de that is matur
-00000f20: 6520 616e 6420 7072 6f76 6964 6573 2061  e and provides a
-00000f30: 2070 6f69 6e74 206f 6620 636f 6d70 6172   point of compar
-00000f40: 6973 6f6e 2066 6f72 206f 7468 6572 0a20  ison for other. 
-00000f50: 2069 6d70 6c65 6d65 6e74 6174 696f 6e73   implementations
-00000f60: 206f 6620 7468 6520 7361 6d65 2061 6c67   of the same alg
-00000f70: 6f72 6974 686d 733b 0a2d 2072 6f75 7469  orithms;.- routi
-00000f80: 6e65 7320 7768 6963 6820 6172 6520 6765  nes which are ge
-00000f90: 6e65 7261 6c6c 7920 7772 6974 7465 6e20  nerally written 
-00000fa0: 696e 2061 2073 7472 6169 6768 7466 6f72  in a straightfor
-00000fb0: 7761 7264 206d 616e 6e65 7220 7768 6963  ward manner whic
-00000fc0: 680a 2020 616c 6c6f 7773 2066 6f72 2065  h.  allows for e
-00000fd0: 6173 7920 756e 6465 7273 7461 6e64 696e  asy understandin
-00000fe0: 672c 2070 6572 6861 7073 2061 7420 7468  g, perhaps at th
-00000ff0: 6520 6578 7065 6e73 6520 6f66 2063 6f6d  e expense of com
-00001000: 7075 7461 7469 6f6e 616c 0a20 2065 6666  putational.  eff
-00001010: 6963 6965 6e63 793b 0a2d 2073 6f75 7263  iciency;.- sourc
-00001020: 6520 636f 6465 2077 6869 6368 2063 616e  e code which can
-00001030: 2062 6520 7265 6164 2066 6f72 206c 6561   be read for lea
-00001040: 726e 696e 6720 616e 6420 7465 6163 6869  rning and teachi
-00001050: 6e67 3b0a 2d20 6261 636b 7761 7264 2063  ng;.- backward c
-00001060: 6f6d 7061 7461 6269 6c69 7479 2077 6974  ompatability wit
-00001070: 6820 7468 6520 526f 626f 7469 6373 2054  h the Robotics T
-00001080: 6f6f 6c62 6f78 2066 6f72 204d 4154 4c41  oolbox for MATLA
-00001090: 420a 0a54 6865 2054 6f6f 6c62 6f78 206c  B..The Toolbox l
-000010a0: 6576 6572 6167 6573 2074 6865 205b 5370  everages the [Sp
-000010b0: 6174 6961 6c20 4d61 7468 7320 546f 6f6c  atial Maths Tool
-000010c0: 626f 7820 666f 7220 5079 7468 6f6e 5d28  box for Python](
-000010d0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000010e0: 6f6d 2f70 6574 6572 636f 726b 652f 7370  om/petercorke/sp
-000010f0: 6174 6961 6c6d 6174 682d 7079 7468 6f6e  atialmath-python
-00001100: 2920 746f 0a70 726f 7669 6465 2073 7570  ) to.provide sup
-00001110: 706f 7274 2066 6f72 2064 6174 6120 7479  port for data ty
-00001120: 7065 7320 7375 6368 2061 7320 534f 286e  pes such as SO(n
-00001130: 2920 616e 6420 5345 286e 2920 6d61 7472  ) and SE(n) matr
-00001140: 6963 6573 2c20 7175 6174 6572 6e69 6f6e  ices, quaternion
-00001150: 732c 2074 7769 7374 7320 616e 6420 7370  s, twists and sp
-00001160: 6174 6961 6c20 7665 6374 6f72 732e 0a0a  atial vectors...
-00001170: 3c62 723e 0a0a 3c61 2069 643d 2732 273e  <br>..<a id='2'>
-00001180: 3c2f 613e 0a0a 2323 2047 6574 7469 6e67  </a>..## Getting
-00001190: 2067 6f69 6e67 0a0a 596f 7520 7769 6c6c   going..You will
-000011a0: 206e 6565 6420 5079 7468 6f6e 203e 3d20   need Python >= 
-000011b0: 332e 360a 0a23 2323 2055 7369 6e67 2070  3.6..### Using p
-000011c0: 6970 0a0a 496e 7374 616c 6c20 6120 736e  ip..Install a sn
-000011d0: 6170 7368 6f74 2066 726f 6d20 5079 5049  apshot from PyPI
-000011e0: 0a0a 6060 6073 6865 6c6c 2073 6372 6970  ..```shell scrip
-000011f0: 740a 7069 7033 2069 6e73 7461 6c6c 2072  t.pip3 install r
-00001200: 6f62 6f74 6963 7374 6f6f 6c62 6f78 2d70  oboticstoolbox-p
-00001210: 7974 686f 6e0a 6060 600a 0a41 7661 696c  ython.```..Avail
-00001220: 6162 6c65 206f 7074 696f 6e73 2061 7265  able options are
-00001230: 3a0a 0a2d 2060 636f 6c6c 6973 696f 6e60  :..- `collision`
-00001240: 2069 6e73 7461 6c6c 2063 6f6c 6c69 7369   install collisi
-00001250: 6f6e 2063 6865 636b 696e 6720 7769 7468  on checking with
-00001260: 205b 7079 6275 6c6c 6574 5d28 6874 7470   [pybullet](http
-00001270: 733a 2f2f 7079 6275 6c6c 6574 2e6f 7267  s://pybullet.org
-00001280: 290a 0a50 7574 2074 6865 206f 7074 696f  )..Put the optio
-00001290: 6e73 2069 6e20 6120 636f 6d6d 6120 7365  ns in a comma se
-000012a0: 7061 7261 7465 6420 6c69 7374 206c 696b  parated list lik
-000012b0: 650a 0a60 6060 7368 656c 6c20 7363 7269  e..```shell scri
-000012c0: 7074 0a70 6970 3320 696e 7374 616c 6c20  pt.pip3 install 
-000012d0: 726f 626f 7469 6373 746f 6f6c 626f 782d  roboticstoolbox-
-000012e0: 7079 7468 6f6e 5b6f 7074 696f 6e6c 6973  python[optionlis
-000012f0: 745d 0a60 6060 0a0a 5b53 7769 6674 5d28  t].```..[Swift](
-00001300: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001310: 6f6d 2f6a 6861 766c 2f73 7769 6674 292c  om/jhavl/swift),
-00001320: 2061 2077 6562 2d62 6173 6564 2076 6973   a web-based vis
-00001330: 7561 6c69 7a65 722c 2069 730a 696e 7374  ualizer, is.inst
-00001340: 616c 6c65 6420 6173 2070 6172 7420 6f66  alled as part of
-00001350: 2052 6f62 6f74 6963 7320 546f 6f6c 626f   Robotics Toolbo
-00001360: 782e 0a0a 2323 2320 4672 6f6d 2047 6974  x...### From Git
-00001370: 4875 620a 0a54 6f20 696e 7374 616c 6c20  Hub..To install 
-00001380: 7468 6520 626c 6565 6469 6e67 2d65 6467  the bleeding-edg
-00001390: 6520 7665 7273 696f 6e20 6672 6f6d 2047  e version from G
-000013a0: 6974 4875 620a 0a60 6060 7368 656c 6c20  itHub..```shell 
-000013b0: 7363 7269 7074 0a67 6974 2063 6c6f 6e65  script.git clone
-000013c0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-000013d0: 636f 6d2f 7065 7465 7263 6f72 6b65 2f72  com/petercorke/r
-000013e0: 6f62 6f74 6963 732d 746f 6f6c 626f 782d  obotics-toolbox-
-000013f0: 7079 7468 6f6e 2e67 6974 0a63 6420 726f  python.git.cd ro
-00001400: 626f 7469 6373 2d74 6f6f 6c62 6f78 2d70  botics-toolbox-p
-00001410: 7974 686f 6e0a 7069 7033 2069 6e73 7461  ython.pip3 insta
-00001420: 6c6c 202d 6520 2e0a 6060 600a 0a3c 6272  ll -e ..```..<br
-00001430: 3e0a 0a3c 6120 6964 3d27 3327 3e3c 2f61  >..<a id='3'></a
-00001440: 3e0a 0a23 2320 5475 746f 7269 616c 730a  >..## Tutorials.
-00001450: 0a3c 7461 626c 6520 7374 796c 653d 2262  .<table style="b
-00001460: 6f72 6465 723a 3070 7822 3e0a 3c74 7220  order:0px">.<tr 
-00001470: 7374 796c 653d 2262 6f72 6465 723a 3070  style="border:0p
-00001480: 7822 3e0a 3c74 6420 7374 796c 653d 2262  x">.<td style="b
-00001490: 6f72 6465 723a 3070 7822 3e3c 6120 6872  order:0px"><a hr
-000014a0: 6566 3d22 6874 7470 733a 2f2f 6269 742e  ef="https://bit.
-000014b0: 6c79 2f33 616b 3547 4469 223e 3c69 6d67  ly/3ak5GDi"><img
-000014c0: 2073 7263 3d22 6874 7470 733a 2f2f 6769   src="https://gi
-000014d0: 7468 7562 2e63 6f6d 2f6a 6861 766c 2f64  thub.com/jhavl/d
-000014e0: 6b74 2f72 6177 2f6d 6169 6e2f 696d 672f  kt/raw/main/img/
-000014f0: 6172 7469 636c 6531 2e70 6e67 2220 7769  article1.png" wi
-00001500: 6474 683d 2234 3030 223e 3c2f 613e 3c2f  dth="400"></a></
-00001510: 7464 3e0a 3c74 6420 7374 796c 653d 2262  td>.<td style="b
-00001520: 6f72 6465 723a 3070 7822 3e3c 6120 6872  order:0px"><a hr
-00001530: 6566 3d22 6874 7470 733a 2f2f 6269 742e  ef="https://bit.
-00001540: 6c79 2f33 616b 3547 4469 223e 3c69 6d67  ly/3ak5GDi"><img
-00001550: 2073 7263 3d22 6874 7470 733a 2f2f 6769   src="https://gi
-00001560: 7468 7562 2e63 6f6d 2f6a 6861 766c 2f64  thub.com/jhavl/d
-00001570: 6b74 2f72 6177 2f6d 6169 6e2f 696d 672f  kt/raw/main/img/
-00001580: 6172 7469 636c 6532 2e70 6e67 2220 7769  article2.png" wi
-00001590: 6474 683d 2234 3030 223e 3c2f 613e 3c2f  dth="400"></a></
-000015a0: 7464 3e0a 3c74 6420 7374 796c 653d 2262  td>.<td style="b
-000015b0: 6f72 6465 723a 3070 7822 3e0a 446f 2079  order:0px">.Do y
-000015c0: 6f75 2077 616e 7420 746f 206c 6561 726e  ou want to learn
-000015d0: 2061 626f 7574 206d 616e 6970 756c 6174   about manipulat
-000015e0: 6f72 206b 696e 656d 6174 6963 732c 2064  or kinematics, d
-000015f0: 6966 6665 7265 6e74 6961 6c20 6b69 6e65  ifferential kine
-00001600: 6d61 7469 6373 2c20 696e 7665 7273 652d  matics, inverse-
-00001610: 6b69 6e65 6d61 7469 6373 2061 6e64 206d  kinematics and m
-00001620: 6f74 696f 6e20 636f 6e74 726f 6c3f 2048  otion control? H
-00001630: 6176 6520 6120 6c6f 6f6b 2061 7420 6f75  ave a look at ou
-00001640: 720a 3c61 2068 7265 663d 2268 7474 7073  r.<a href="https
-00001650: 3a2f 2f62 6974 2e6c 792f 3361 6b35 4744  ://bit.ly/3ak5GD
-00001660: 6922 3e74 7574 6f72 6961 6c3c 2f61 3e2e  i">tutorial</a>.
-00001670: 0a54 6869 7320 7475 746f 7269 616c 2063  .This tutorial c
-00001680: 6f6d 6573 2077 6974 6820 7477 6f20 6172  omes with two ar
-00001690: 7469 636c 6573 2074 6f20 636f 7665 7220  ticles to cover 
-000016a0: 7468 6520 7468 656f 7279 2061 6e64 2031  the theory and 1
-000016b0: 3220 4a75 7079 7465 7220 4e6f 7465 626f  2 Jupyter Notebo
-000016c0: 6f6b 7320 7072 6f76 6964 696e 6720 6675  oks providing fu
-000016d0: 6c6c 2063 6f64 6520 696d 706c 656d 656e  ll code implemen
-000016e0: 7461 7469 6f6e 7320 616e 6420 6578 616d  tations and exam
-000016f0: 706c 6573 2e20 4d6f 7374 206f 6620 7468  ples. Most of th
-00001700: 6520 4e6f 7465 626f 6f6b 7320 6172 6520  e Notebooks are 
-00001710: 616c 736f 2047 6f6f 676c 6520 436f 6c61  also Google Cola
-00001720: 6220 636f 6d70 6174 6962 6c65 2061 6c6c  b compatible all
-00001730: 6f77 696e 6720 7468 656d 2074 6f20 7275  owing them to ru
-00001740: 6e20 6f6e 6c69 6e65 2e0a 3c2f 7464 3e0a  n online..</td>.
-00001750: 3c2f 7472 3e0a 3c2f 7461 626c 653e 0a0a  </tr>.</table>..
-00001760: 3c62 723e 0a0a 3c61 2069 643d 2734 273e  <br>..<a id='4'>
-00001770: 3c2f 613e 0a0a 2323 2043 6f64 6520 4578  </a>..## Code Ex
-00001780: 616d 706c 6573 0a0a 5765 2077 696c 6c20  amples..We will 
-00001790: 6c6f 6164 2061 206d 6f64 656c 206f 6620  load a model of 
-000017a0: 7468 6520 4672 616e 6b61 2d45 6d69 6b61  the Franka-Emika
-000017b0: 2050 616e 6461 2072 6f62 6f74 2064 6566   Panda robot def
-000017c0: 696e 6564 2062 7920 6120 5552 4446 2066  ined by a URDF f
-000017d0: 696c 650a 0a60 6060 7079 7468 6f6e 0a69  ile..```python.i
-000017e0: 6d70 6f72 7420 726f 626f 7469 6373 746f  mport roboticsto
-000017f0: 6f6c 626f 7820 6173 2072 7462 0a72 6f62  olbox as rtb.rob
-00001800: 6f74 203d 2072 7462 2e6d 6f64 656c 732e  ot = rtb.models.
-00001810: 5061 6e64 6128 290a 7072 696e 7428 726f  Panda().print(ro
-00001820: 626f 7429 0a0a 0945 526f 626f 743a 2070  bot)...ERobot: p
-00001830: 616e 6461 2028 6279 2046 7261 6e6b 6120  anda (by Franka 
-00001840: 456d 696b 6129 2c20 3720 6a6f 696e 7473  Emika), 7 joints
-00001850: 2028 5252 5252 5252 5229 2c20 3120 6772   (RRRRRRR), 1 gr
-00001860: 6970 7065 722c 2067 656f 6d65 7472 792c  ipper, geometry,
-00001870: 2063 6f6c 6c69 7369 6f6e 0a09 e294 8ce2   collision......
-00001880: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001890: ace2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000018a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000018b0: 9480 e294 80e2 9480 e294 80e2 94ac e294  ................
-000018c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000018d0: e294 80e2 94ac e294 80e2 9480 e294 80e2  ................
-000018e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000018f0: 80e2 9480 e294 80e2 9480 e294 80e2 94ac  ................
-00001900: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001910: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001920: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001930: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001940: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001950: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001960: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001970: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001980: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001990: e294 900a 09e2 9482 6c69 6e6b 20e2 9482  ........link ...
-000019a0: 2020 2020 206c 696e 6b20 2020 2020 e294       link     ..
-000019b0: 8220 6a6f 696e 7420 e294 8220 2020 7061  . joint ...   pa
-000019c0: 7265 6e74 2020 2020 e294 8220 2020 2020  rent    ...     
-000019d0: 2020 2020 2020 2020 2045 5453 3a20 7061           ETS: pa
-000019e0: 7265 6e74 2074 6f20 6c69 6e6b 2020 2020  rent to link    
-000019f0: 2020 2020 2020 2020 2020 20e2 9482 0a09             .....
-00001a00: e294 9ce2 9480 e294 80e2 9480 e294 80e2  ................
-00001a10: 9480 e294 bce2 9480 e294 80e2 9480 e294  ................
-00001a20: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001a30: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001a40: 94bc e294 80e2 9480 e294 80e2 9480 e294  ................
-00001a50: 80e2 9480 e294 80e2 94bc e294 80e2 9480  ................
-00001a60: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001a70: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001a80: 80e2 94bc e294 80e2 9480 e294 80e2 9480  ................
-00001a90: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001aa0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001ab0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001ac0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001ad0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001ae0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001af0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001b00: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001b10: 80e2 9480 e294 a40a 09e2 9482 2020 2030  ............   0
-00001b20: 20e2 9482 2070 616e 6461 5f6c 696e 6b30   ... panda_link0
-00001b30: 2020 e294 8220 2020 2020 2020 e294 8220    ...       ... 
-00001b40: 4241 5345 2020 2020 2020 2020 e294 8220  BASE        ... 
-00001b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b70: 2020 2020 2020 2020 2020 2020 2020 20e2                 .
-00001b80: 9482 0a09 e294 8220 2020 3120 e294 8220  .......   1 ... 
-00001b90: 7061 6e64 615f 6c69 6e6b 3120 20e2 9482  panda_link1  ...
-00001ba0: 2020 2020 2030 20e2 9482 2070 616e 6461       0 ... panda
-00001bb0: 5f6c 696e 6b30 20e2 9482 2053 4533 2830  _link0 ... SE3(0
-00001bc0: 2c20 302c 2030 2e33 3333 2920 e28a 9520  , 0, 0.333) ... 
-00001bd0: 527a 2871 3029 2020 2020 2020 2020 2020  Rz(q0)          
-00001be0: 2020 2020 2020 2020 2020 2020 e294 820a              ....
-00001bf0: 09e2 9482 2020 2032 20e2 9482 2070 616e  ....   2 ... pan
-00001c00: 6461 5f6c 696e 6b32 2020 e294 8220 2020  da_link2  ...   
-00001c10: 2020 3120 e294 8220 7061 6e64 615f 6c69    1 ... panda_li
-00001c20: 6e6b 3120 e294 8220 5345 3328 2d39 30c2  nk1 ... SE3(-90.
-00001c30: b02c 202d 30c2 b02c 2030 c2b0 2920 e28a  ., -0.., 0..) ..
-00001c40: 9520 527a 2871 3129 2020 2020 2020 2020  . Rz(q1)        
-00001c50: 2020 2020 2020 2020 2020 2020 e294 820a              ....
-00001c60: 09e2 9482 2020 2033 20e2 9482 2070 616e  ....   3 ... pan
-00001c70: 6461 5f6c 696e 6b33 2020 e294 8220 2020  da_link3  ...   
-00001c80: 2020 3220 e294 8220 7061 6e64 615f 6c69    2 ... panda_li
-00001c90: 6e6b 3220 e294 8220 5345 3328 302c 202d  nk2 ... SE3(0, -
-00001ca0: 302e 3331 362c 2030 3b20 3930 c2b0 2c20  0.316, 0; 90.., 
-00001cb0: 2d30 c2b0 2c20 30c2 b029 20e2 8a95 2052  -0.., 0..) ... R
-00001cc0: 7a28 7132 2920 2020 2020 2020 e294 820a  z(q2)       ....
-00001cd0: 09e2 9482 2020 2034 20e2 9482 2070 616e  ....   4 ... pan
-00001ce0: 6461 5f6c 696e 6b34 2020 e294 8220 2020  da_link4  ...   
-00001cf0: 2020 3320 e294 8220 7061 6e64 615f 6c69    3 ... panda_li
-00001d00: 6e6b 3320 e294 8220 5345 3328 302e 3038  nk3 ... SE3(0.08
-00001d10: 3235 2c20 302c 2030 3b20 3930 c2b0 2c20  25, 0, 0; 90.., 
-00001d20: 2d30 c2b0 2c20 30c2 b029 20e2 8a95 2052  -0.., 0..) ... R
-00001d30: 7a28 7133 2920 2020 2020 2020 e294 820a  z(q3)       ....
-00001d40: 09e2 9482 2020 2035 20e2 9482 2070 616e  ....   5 ... pan
-00001d50: 6461 5f6c 696e 6b35 2020 e294 8220 2020  da_link5  ...   
-00001d60: 2020 3420 e294 8220 7061 6e64 615f 6c69    4 ... panda_li
-00001d70: 6e6b 3420 e294 8220 5345 3328 2d30 2e30  nk4 ... SE3(-0.0
-00001d80: 3832 352c 2030 2e33 3834 2c20 303b 202d  825, 0.384, 0; -
-00001d90: 3930 c2b0 2c20 2d30 c2b0 2c20 30c2 b029  90.., -0.., 0..)
-00001da0: 20e2 8a95 2052 7a28 7134 2920 e294 820a   ... Rz(q4) ....
-00001db0: 09e2 9482 2020 2036 20e2 9482 2070 616e  ....   6 ... pan
-00001dc0: 6461 5f6c 696e 6b36 2020 e294 8220 2020  da_link6  ...   
-00001dd0: 2020 3520 e294 8220 7061 6e64 615f 6c69    5 ... panda_li
-00001de0: 6e6b 3520 e294 8220 5345 3328 3930 c2b0  nk5 ... SE3(90..
-00001df0: 2c20 2d30 c2b0 2c20 30c2 b029 20e2 8a95  , -0.., 0..) ...
-00001e00: 2052 7a28 7135 2920 2020 2020 2020 2020   Rz(q5)         
-00001e10: 2020 2020 2020 2020 2020 2020 e294 820a              ....
-00001e20: 09e2 9482 2020 2037 20e2 9482 2070 616e  ....   7 ... pan
-00001e30: 6461 5f6c 696e 6b37 2020 e294 8220 2020  da_link7  ...   
-00001e40: 2020 3620 e294 8220 7061 6e64 615f 6c69    6 ... panda_li
-00001e50: 6e6b 3620 e294 8220 5345 3328 302e 3038  nk6 ... SE3(0.08
-00001e60: 382c 2030 2c20 303b 2039 30c2 b02c 202d  8, 0, 0; 90.., -
-00001e70: 30c2 b02c 2030 c2b0 2920 e28a 9520 527a  0.., 0..) ... Rz
-00001e80: 2871 3629 2020 2020 2020 2020 e294 820a  (q6)        ....
-00001e90: 09e2 9482 2020 2038 20e2 9482 2040 7061  ....   8 ... @pa
-00001ea0: 6e64 615f 6c69 6e6b 3820 e294 8220 2020  nda_link8 ...   
-00001eb0: 2020 2020 e294 8220 7061 6e64 615f 6c69      ... panda_li
-00001ec0: 6e6b 3720 e294 8220 5345 3328 302c 2030  nk7 ... SE3(0, 0
-00001ed0: 2c20 302e 3130 3729 2020 2020 2020 2020  , 0.107)        
-00001ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ef0: 2020 2020 2020 20e2 9482 0a09 e294 94e2         .........
-00001f00: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001f10: b4e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001f20: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001f30: 9480 e294 80e2 9480 e294 80e2 94b4 e294  ................
-00001f40: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001f50: e294 80e2 94b4 e294 80e2 9480 e294 80e2  ................
-00001f60: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001f70: 80e2 9480 e294 80e2 9480 e294 80e2 94b4  ................
-00001f80: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001f90: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001fa0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001fb0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001fc0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001fd0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001fe0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001ff0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002000: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002010: e294 980a 0a09 e294 8ce2 9480 e294 80e2  ................
-00002020: 9480 e294 80e2 9480 e294 ace2 9480 e294  ................
-00002030: 80e2 9480 e294 80e2 9480 e294 ace2 9480  ................
-00002040: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002050: 9480 e294 80e2 94ac e294 80e2 9480 e294  ................
-00002060: 80e2 9480 e294 80e2 94ac e294 80e2 9480  ................
-00002070: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002080: 94ac e294 80e2 9480 e294 80e2 9480 e294  ................
-00002090: 80e2 94ac e294 80e2 9480 e294 80e2 9480  ................
-000020a0: e294 80e2 9480 e294 80e2 94ac e294 80e2  ................
-000020b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000020c0: 900a 09e2 9482 6e61 6d65 20e2 9482 2071  ......name ... q
-000020d0: 3020 20e2 9482 2071 3120 2020 2020 e294  0  ... q1     ..
-000020e0: 8220 7132 2020 e294 8220 7133 2020 2020  . q2  ... q3    
-000020f0: e294 8220 7134 2020 e294 8220 7135 2020  ... q4  ... q5  
-00002100: 2020 e294 8220 7136 2020 20e2 9482 0a09    ... q6   .....
-00002110: e294 9ce2 9480 e294 80e2 9480 e294 80e2  ................
-00002120: 9480 e294 bce2 9480 e294 80e2 9480 e294  ................
-00002130: 80e2 9480 e294 bce2 9480 e294 80e2 9480  ................
-00002140: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002150: 94bc e294 80e2 9480 e294 80e2 9480 e294  ................
-00002160: 80e2 94bc e294 80e2 9480 e294 80e2 9480  ................
-00002170: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
-00002180: 9480 e294 80e2 9480 e294 80e2 94bc e294  ................
-00002190: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000021a0: e294 80e2 94bc e294 80e2 9480 e294 80e2  ................
-000021b0: 9480 e294 80e2 9480 e294 a40a 09e2 9482  ................
-000021c0: 2020 7172 20e2 9482 2020 30c2 b020 e294    qr ...  0.. ..
-000021d0: 8220 2d31 372e 32c2 b020 e294 8220 2030  . -17.2.. ...  0
-000021e0: c2b0 20e2 9482 202d 3132 36c2 b020 e294  .. ... -126.. ..
-000021f0: 8220 2030 c2b0 20e2 9482 2020 3131 35c2  .  0.. ...  115.
-00002200: b020 e294 8220 2034 35c2 b020 e294 820a  . ...  45.. ....
-00002210: 09e2 9482 2020 717a 20e2 9482 2020 30c2  ....  qz ...  0.
-00002220: b020 e294 8220 2030 c2b0 2020 2020 e294  . ...  0..    ..
-00002230: 8220 2030 c2b0 20e2 9482 2020 30c2 b020  .  0.. ...  0.. 
-00002240: 2020 e294 8220 2030 c2b0 20e2 9482 2020    ...  0.. ...  
-00002250: 30c2 b020 2020 e294 8220 2030 c2b0 2020  0..   ...  0..  
-00002260: e294 820a 09e2 9494 e294 80e2 9480 e294  ................
-00002270: 80e2 9480 e294 80e2 94b4 e294 80e2 9480  ................
-00002280: e294 80e2 9480 e294 80e2 94b4 e294 80e2  ................
-00002290: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000022a0: 80e2 9480 e294 b4e2 9480 e294 80e2 9480  ................
-000022b0: e294 80e2 9480 e294 b4e2 9480 e294 80e2  ................
-000022c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000022d0: b4e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000022e0: e294 b4e2 9480 e294 80e2 9480 e294 80e2  ................
-000022f0: 9480 e294 80e2 9480 e294 b4e2 9480 e294  ................
-00002300: 80e2 9480 e294 80e2 9480 e294 80e2 9498  ................
-00002310: 0a60 6060 0a0a 5468 6520 7379 6d62 6f6c  .```..The symbol
-00002320: 2060 4060 2069 6e64 6963 6174 6573 2074   `@` indicates t
-00002330: 6865 206c 696e 6b20 6173 2061 6e20 656e  he link as an en
-00002340: 642d 6566 6665 6374 6f72 2c20 6120 6c65  d-effector, a le
-00002350: 6166 206e 6f64 6520 696e 2074 6865 2072  af node in the r
-00002360: 6967 6964 2d62 6f64 790a 7472 6565 2028  igid-body.tree (
-00002370: 5079 7468 6f6e 2070 726f 6d70 7473 2061  Python prompts a
-00002380: 7265 206e 6f74 2073 686f 776e 2074 6f20  re not shown to 
-00002390: 6d61 6b65 2069 7420 6561 7379 2074 6f20  make it easy to 
-000023a0: 636f 7079 2b70 6173 7465 2074 6865 2063  copy+paste the c
-000023b0: 6f64 652c 2063 6f6e 736f 6c65 206f 7574  ode, console out
-000023c0: 7075 7420 6973 2069 6e64 656e 7465 6429  put is indented)
-000023d0: 2e0a 5765 2077 696c 6c20 636f 6d70 7574  ..We will comput
-000023e0: 6520 7468 6520 666f 7277 6172 6420 6b69  e the forward ki
-000023f0: 6e65 6d61 7469 6373 206e 6578 740a 0a60  nematics next..`
-00002400: 6060 0a54 6520 3d20 726f 626f 742e 666b  ``.Te = robot.fk
-00002410: 696e 6528 726f 626f 742e 7172 2920 2023  ine(robot.qr)  #
-00002420: 2066 6f72 7761 7264 206b 696e 656d 6174   forward kinemat
-00002430: 6963 730a 7072 696e 7428 5465 290a 0a09  ics.print(Te)...
-00002440: 302e 3939 3520 2020 2020 3020 2020 2020  0.995     0     
-00002450: 2020 2020 302e 3039 3938 3320 2020 302e      0.09983   0.
-00002460: 3438 340a 0930 2020 2020 2020 2020 2d31  484..0        -1
-00002470: 2020 2020 2020 2020 2030 2020 2020 2020           0      
-00002480: 2020 2030 0a09 302e 3039 3938 3320 2020     0..0.09983   
-00002490: 3020 2020 2020 2020 202d 302e 3939 3520  0        -0.995 
-000024a0: 2020 2020 302e 3431 3236 0a09 3020 2020      0.4126..0   
-000024b0: 2020 2020 2020 3020 2020 2020 2020 2020        0         
-000024c0: 3020 2020 2020 2020 2020 310a 6060 600a  0         1.```.
-000024d0: 0a57 6520 6361 6e20 736f 6c76 6520 696e  .We can solve in
-000024e0: 7665 7273 6520 6b69 6e65 6d61 7469 6373  verse kinematics
-000024f0: 2076 6572 7920 6561 7369 6c79 2e20 5765   very easily. We
-00002500: 2066 6972 7374 2063 686f 6f73 6520 616e   first choose an
-00002510: 2053 4528 3329 2070 6f73 650a 6465 6669   SE(3) pose.defi
-00002520: 6e65 6420 696e 2074 6572 6d73 206f 6620  ned in terms of 
-00002530: 706f 7369 7469 6f6e 2061 6e64 206f 7269  position and ori
-00002540: 656e 7461 7469 6f6e 2028 656e 642d 6566  entation (end-ef
-00002550: 6665 6374 6f72 207a 2d61 7869 7320 646f  fector z-axis do
-00002560: 776e 2028 413d 2d5a 2920 616e 6420 6669  wn (A=-Z) and fi
-00002570: 6e67 6572 0a6f 7269 656e 7461 7469 6f6e  nger.orientation
-00002580: 2070 6172 616c 6c65 6c20 746f 2079 2d61   parallel to y-a
-00002590: 7869 7320 284f 3d2b 5929 292e 0a0a 6060  xis (O=+Y))...``
-000025a0: 6070 7974 686f 6e0a 6672 6f6d 2073 7061  `python.from spa
-000025b0: 7469 616c 6d61 7468 2069 6d70 6f72 7420  tialmath import 
-000025c0: 5345 330a 0a54 6570 203d 2053 4533 2e54  SE3..Tep = SE3.T
-000025d0: 7261 6e73 2830 2e36 2c20 2d30 2e33 2c20  rans(0.6, -0.3, 
-000025e0: 302e 3129 202a 2053 4533 2e4f 4128 5b30  0.1) * SE3.OA([0
-000025f0: 2c20 312c 2030 5d2c 205b 302c 2030 2c20  , 1, 0], [0, 0, 
-00002600: 2d31 5d29 0a73 6f6c 203d 2072 6f62 6f74  -1]).sol = robot
-00002610: 2e69 6b5f 6c6d 5f63 6861 6e28 5465 7029  .ik_lm_chan(Tep)
-00002620: 2020 2020 2020 2020 2023 2073 6f6c 7665           # solve
-00002630: 2049 4b0a 7072 696e 7428 736f 6c29 0a0a   IK.print(sol)..
-00002640: 0928 6172 7261 7928 5b20 302e 3230 3539  .(array([ 0.2059
-00002650: 3238 3135 2c20 2030 2e38 3636 3039 3438  2815,  0.8660948
-00002660: 312c 202d 302e 3739 3437 3332 3036 2c20  1, -0.79473206, 
-00002670: 2d31 2e36 3832 3534 3739 342c 2020 302e  -1.68254794,  0.
-00002680: 3734 3837 3239 3135 2c0a 0909 0932 2e32  74872915,....2.2
-00002690: 3137 3634 3734 362c 202d 302e 3130 3235  1764746, -0.1025
-000026a0: 3536 3036 5d29 2c20 312c 2031 3134 2c20  5606]), 1, 114, 
-000026b0: 372c 2032 2e38 3930 3136 3430 3537 3233  7, 2.89016405723
-000026c0: 3032 3238 652d 3037 290a 0a71 5f70 6963  0228e-07)..q_pic
-000026d0: 6b75 7020 3d20 736f 6c5b 305d 0a70 7269  kup = sol[0].pri
-000026e0: 6e74 2872 6f62 6f74 2e66 6b69 6e65 2871  nt(robot.fkine(q
-000026f0: 5f70 6963 6b75 7029 2920 2020 2023 2046  _pickup))    # F
-00002700: 4b20 7368 6f77 7320 7468 6174 2064 6573  K shows that des
-00002710: 6972 6564 2065 6e64 2d65 6666 6563 746f  ired end-effecto
-00002720: 7220 706f 7365 2077 6173 2061 6368 6965  r pose was achie
-00002730: 7665 640a 0a09 2031 2020 2020 2020 2020  ved... 1        
-00002740: 202d 382e 3931 3365 2d30 3520 202d 302e   -8.913e-05  -0.
-00002750: 3030 3033 3333 3420 2030 2e35 3939 360a  0003334  0.5996.
-00002760: 092d 382e 3932 3965 2d30 3520 2d31 2020  .-8.929e-05 -1  
-00002770: 2020 2020 2020 2020 2d30 2e30 3030 3439          -0.00049
-00002780: 3132 202d 302e 3239 3938 0a09 2d30 2e30  12 -0.2998..-0.0
-00002790: 3030 3333 3334 2020 302e 3030 3034 3931  003334  0.000491
-000027a0: 3220 202d 3120 2020 2020 2020 2020 2030  2  -1          0
-000027b0: 2e31 3030 310a 0920 3020 2020 2020 2020  .1001.. 0       
-000027c0: 2020 2030 2020 2020 2020 2020 2020 2030     0           0
-000027d0: 2020 2020 2020 2020 2020 310a 6060 600a            1.```.
-000027e0: 0a57 6520 6361 6e20 616e 696d 6174 6520  .We can animate 
-000027f0: 6120 7061 7468 2066 726f 6d20 7468 6520  a path from the 
-00002800: 7265 6164 7920 706f 7365 2060 7172 6020  ready pose `qr` 
-00002810: 636f 6e66 6967 7572 6174 696f 6e20 746f  configuration to
-00002820: 2074 6869 7320 7069 636b 7570 2063 6f6e   this pickup con
-00002830: 6669 6775 7261 7469 6f6e 0a0a 6060 6070  figuration..```p
-00002840: 7974 686f 6e0a 7174 203d 2072 7462 2e6a  ython.qt = rtb.j
-00002850: 7472 616a 2872 6f62 6f74 2e71 722c 2071  traj(robot.qr, q
-00002860: 5f70 6963 6b75 702c 2035 3029 0a72 6f62  _pickup, 50).rob
-00002870: 6f74 2e70 6c6f 7428 7174 2e71 2c20 6261  ot.plot(qt.q, ba
-00002880: 636b 656e 643d 2770 7970 6c6f 7427 2c20  ckend='pyplot', 
-00002890: 6d6f 7669 653d 2770 616e 6461 312e 6769  movie='panda1.gi
-000028a0: 6627 290a 6060 600a 0a3c 7020 616c 6967  f').```..<p alig
-000028b0: 6e3d 2263 656e 7465 7222 3e0a 093c 696d  n="center">..<im
-000028c0: 6720 7372 633d 222e 2f64 6f63 732f 6669  g src="./docs/fi
-000028d0: 6773 2f70 616e 6461 312e 6769 6622 3e0a  gs/panda1.gif">.
-000028e0: 3c2f 703e 0a0a 7768 6572 6520 7765 2068  </p>..where we h
-000028f0: 6176 6520 7370 6563 6966 6965 6420 7468  ave specified th
-00002900: 6520 6d61 7470 6c6f 746c 6962 2060 7079  e matplotlib `py
-00002910: 706c 6f74 6020 6261 636b 656e 642e 2042  plot` backend. B
-00002920: 6c75 6520 6172 726f 7773 2073 686f 7720  lue arrows show 
-00002930: 7468 6520 6a6f 696e 7420 6178 6573 2061  the joint axes a
-00002940: 6e64 2074 6865 2063 6f6c 6f75 7265 6420  nd the coloured 
-00002950: 6672 616d 6520 7368 6f77 7320 7468 6520  frame shows the 
-00002960: 656e 642d 6566 6665 6374 6f72 2070 6f73  end-effector pos
-00002970: 652e 0a0a 5765 2063 616e 2061 6c73 6f20  e...We can also 
-00002980: 706c 6f74 2074 6865 2074 7261 6a65 6374  plot the traject
-00002990: 6f72 7920 696e 2074 6865 2053 7769 6674  ory in the Swift
-000029a0: 2073 696d 756c 6174 6f72 2028 6120 6272   simulator (a br
-000029b0: 6f77 7365 722d 6261 7365 6420 3364 2d73  owser-based 3d-s
-000029c0: 696d 756c 6174 696f 6e20 656e 7669 726f  imulation enviro
-000029d0: 6e6d 656e 7420 6275 696c 7420 746f 2077  nment built to w
-000029e0: 6f72 6b20 7769 7468 2074 6865 2054 6f6f  ork with the Too
-000029f0: 6c62 6f78 290a 0a60 6060 7079 7468 6f6e  lbox)..```python
-00002a00: 0a72 6f62 6f74 2e70 6c6f 7428 7174 2e71  .robot.plot(qt.q
-00002a10: 290a 6060 600a 0a3c 7020 616c 6967 6e3d  ).```..<p align=
-00002a20: 2263 656e 7465 7222 3e0a 093c 696d 6720  "center">..<img 
-00002a30: 7372 633d 222e 2f64 6f63 732f 6669 6773  src="./docs/figs
-00002a40: 2f70 616e 6461 322e 6769 6622 3e0a 3c2f  /panda2.gif">.</
-00002a50: 703e 0a0a 5765 2063 616e 2061 6c73 6f20  p>..We can also 
-00002a60: 6578 7065 7269 6d65 6e74 2077 6974 6820  experiment with 
-00002a70: 7665 6c6f 6369 7479 2063 6f6e 7472 6f6c  velocity control
-00002a80: 6c65 7273 2069 6e20 5377 6966 742e 2048  lers in Swift. H
-00002a90: 6572 6520 6973 2061 2072 6573 6f6c 7665  ere is a resolve
-00002aa0: 642d 7261 7465 206d 6f74 696f 6e20 636f  d-rate motion co
-00002ab0: 6e74 726f 6c20 6578 616d 706c 650a 0a60  ntrol example..`
-00002ac0: 6060 7079 7468 6f6e 0a69 6d70 6f72 7420  ``python.import 
-00002ad0: 7377 6966 740a 696d 706f 7274 2072 6f62  swift.import rob
-00002ae0: 6f74 6963 7374 6f6f 6c62 6f78 2061 7320  oticstoolbox as 
-00002af0: 7270 0a69 6d70 6f72 7420 7370 6174 6961  rp.import spatia
-00002b00: 6c6d 6174 6820 6173 2073 6d0a 696d 706f  lmath as sm.impo
-00002b10: 7274 206e 756d 7079 2061 7320 6e70 0a0a  rt numpy as np..
-00002b20: 656e 7620 3d20 7377 6966 742e 5377 6966  env = swift.Swif
-00002b30: 7428 290a 656e 762e 6c61 756e 6368 2872  t().env.launch(r
-00002b40: 6561 6c74 696d 653d 5472 7565 290a 0a70  ealtime=True)..p
-00002b50: 616e 6461 203d 2072 702e 6d6f 6465 6c73  anda = rp.models
-00002b60: 2e50 616e 6461 2829 0a70 616e 6461 2e71  .Panda().panda.q
-00002b70: 203d 2070 616e 6461 2e71 720a 0a54 6570   = panda.qr..Tep
-00002b80: 203d 2070 616e 6461 2e66 6b69 6e65 2870   = panda.fkine(p
-00002b90: 616e 6461 2e71 2920 2a20 736d 2e53 4533  anda.q) * sm.SE3
-00002ba0: 2e54 7261 6e73 2830 2e32 2c20 302e 322c  .Trans(0.2, 0.2,
-00002bb0: 2030 2e34 3529 0a0a 6172 7269 7665 6420   0.45)..arrived 
-00002bc0: 3d20 4661 6c73 650a 656e 762e 6164 6428  = False.env.add(
-00002bd0: 7061 6e64 6129 0a0a 6474 203d 2030 2e30  panda)..dt = 0.0
-00002be0: 350a 0a77 6869 6c65 206e 6f74 2061 7272  5..while not arr
-00002bf0: 6976 6564 3a0a 0a20 2020 2076 2c20 6172  ived:..    v, ar
-00002c00: 7269 7665 6420 3d20 7270 2e70 5f73 6572  rived = rp.p_ser
-00002c10: 766f 2870 616e 6461 2e66 6b69 6e65 2870  vo(panda.fkine(p
-00002c20: 616e 6461 2e71 292c 2054 6570 2c20 3129  anda.q), Tep, 1)
-00002c30: 0a20 2020 2070 616e 6461 2e71 6420 3d20  .    panda.qd = 
-00002c40: 6e70 2e6c 696e 616c 672e 7069 6e76 2870  np.linalg.pinv(p
-00002c50: 616e 6461 2e6a 6163 6f62 6528 7061 6e64  anda.jacobe(pand
-00002c60: 612e 7129 2920 4020 760a 2020 2020 656e  a.q)) @ v.    en
-00002c70: 762e 7374 6570 2864 7429 0a0a 2320 556e  v.step(dt)..# Un
-00002c80: 636f 6d6d 656e 7420 746f 2073 746f 7020  comment to stop 
-00002c90: 7468 6520 6272 6f77 7365 7220 7461 6220  the browser tab 
-00002ca0: 6672 6f6d 2063 6c6f 7369 6e67 0a23 2065  from closing.# e
-00002cb0: 6e76 2e68 6f6c 6428 290a 6060 600a 0a3c  nv.hold().```..<
-00002cc0: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
-00002cd0: 3e0a 093c 696d 6720 7372 633d 222e 2f64  >..<img src="./d
-00002ce0: 6f63 732f 6669 6773 2f70 616e 6461 332e  ocs/figs/panda3.
-00002cf0: 6769 6622 3e0a 3c2f 703e 0a0a 2323 2320  gif">.</p>..### 
-00002d00: 5275 6e20 736f 6d65 2065 7861 6d70 6c65  Run some example
-00002d10: 730a 0a54 6865 205b 606e 6f74 6562 6f6f  s..The [`noteboo
-00002d20: 6b73 605d 2868 7474 7073 3a2f 2f67 6974  ks`](https://git
-00002d30: 6875 622e 636f 6d2f 7065 7465 7263 6f72  hub.com/petercor
-00002d40: 6b65 2f72 6f62 6f74 6963 732d 746f 6f6c  ke/robotics-tool
-00002d50: 626f 782d 7079 7468 6f6e 2f74 7265 652f  box-python/tree/
-00002d60: 6d61 7374 6572 2f6e 6f74 6562 6f6f 6b73  master/notebooks
-00002d70: 2920 666f 6c64 6572 2063 6f6e 7461 696e  ) folder contain
-00002d80: 7320 736f 6d65 2074 7574 6f72 6961 6c20  s some tutorial 
-00002d90: 4a75 7079 7465 7220 6e6f 7465 626f 6f6b  Jupyter notebook
-00002da0: 7320 7768 6963 6820 796f 7520 6361 6e20  s which you can 
-00002db0: 6272 6f77 7365 206f 6e20 4769 7448 7562  browse on GitHub
-00002dc0: 2e20 4164 6469 7469 6f6e 616c 6c79 2c20  . Additionally, 
-00002dd0: 6861 7665 2061 206c 6f6f 6b20 696e 2074  have a look in t
-00002de0: 6865 205b 6065 7861 6d70 6c65 7360 5d28  he [`examples`](
-00002df0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00002e00: 6f6d 2f70 6574 6572 636f 726b 652f 726f  om/petercorke/ro
-00002e10: 626f 7469 6373 2d74 6f6f 6c62 6f78 2d70  botics-toolbox-p
-00002e20: 7974 686f 6e2f 7472 6565 2f6d 6173 7465  ython/tree/maste
-00002e30: 722f 726f 626f 7469 6373 746f 6f6c 626f  r/roboticstoolbo
-00002e40: 782f 6578 616d 706c 6573 2920 666f 6c64  x/examples) fold
-00002e50: 6572 2066 6f72 206d 616e 7920 7265 6164  er for many read
-00002e60: 7920 746f 2072 756e 2065 7861 6d70 6c65  y to run example
-00002e70: 732e 0a0a 3c62 723e 0a0a 3c61 2069 643d  s...<br>..<a id=
-00002e80: 2735 273e 3c2f 613e 0a0a 2323 2054 6f6f  '5'></a>..## Too
-00002e90: 6c62 6f78 2052 6573 6561 7263 6820 4170  lbox Research Ap
-00002ea0: 706c 6963 6174 696f 6e73 0a0a 5468 6520  plications..The 
-00002eb0: 746f 6f6c 626f 7820 6973 2069 6e63 7265  toolbox is incre
-00002ec0: 6469 626c 7920 7573 6566 756c 2066 6f72  dibly useful for
-00002ed0: 2064 6576 656c 6f70 696e 6720 616e 6420   developing and 
-00002ee0: 7072 6f74 6f74 7970 696e 6720 616c 676f  prototyping algo
-00002ef0: 7269 7468 6d73 2066 6f72 2072 6573 6561  rithms for resea
-00002f00: 7263 682c 2074 6861 6e6b 7320 746f 2074  rch, thanks to t
-00002f10: 6865 2065 7868 6175 7374 6976 6520 7365  he exhaustive se
-00002f20: 7420 6f66 2077 656c 6c20 646f 6375 6d65  t of well docume
-00002f30: 6e74 6564 2061 6e64 206d 6174 7572 6520  nted and mature 
-00002f40: 726f 626f 7469 6320 6675 6e63 7469 6f6e  robotic function
-00002f50: 7320 6578 706f 7365 6420 7468 726f 7567  s exposed throug
-00002f60: 6820 636c 6561 6e20 616e 6420 7061 696e  h clean and pain
-00002f70: 6c65 7373 2041 5049 732e 2041 6464 6974  less APIs. Addit
-00002f80: 696f 6e61 6c6c 792c 2074 6865 2065 6173  ionally, the eas
-00002f90: 6520 6174 2077 6869 6368 2061 2075 7365  e at which a use
-00002fa0: 7220 6361 6e20 7669 7375 616c 697a 6520  r can visualize 
-00002fb0: 7468 6569 7220 616c 676f 7269 7468 6d20  their algorithm 
-00002fc0: 7375 7070 6f72 7473 2061 2072 6170 6964  supports a rapid
-00002fd0: 2070 726f 746f 7479 7069 6e67 2070 6172   prototyping par
-00002fe0: 6164 6967 6d2e 0a0a 2323 2320 5075 626c  adigm...### Publ
-00002ff0: 6963 6174 696f 6e20 4c69 7374 0a0a 4a2e  ication List..J.
-00003000: 2048 6176 696c 616e 642c 204e 2e20 53c3   Haviland, N. S.
-00003010: bc6e 6465 7268 6175 6620 616e 6420 502e  .nderhauf and P.
-00003020: 2043 6f72 6b65 2c20 222a 2a41 2048 6f6c   Corke, "**A Hol
-00003030: 6973 7469 6320 4170 7072 6f61 6368 2074  istic Approach t
-00003040: 6f20 5265 6163 7469 7665 204d 6f62 696c  o Reactive Mobil
-00003050: 6520 4d61 6e69 7075 6c61 7469 6f6e 2a2a  e Manipulation**
-00003060: 2c22 2069 6e20 5f49 4545 4520 526f 626f  ," in _IEEE Robo
-00003070: 7469 6373 2061 6e64 2041 7574 6f6d 6174  tics and Automat
-00003080: 696f 6e20 4c65 7474 6572 735f 2c20 646f  ion Letters_, do
-00003090: 693a 2031 302e 3131 3039 2f4c 5241 2e32  i: 10.1109/LRA.2
-000030a0: 3032 322e 3331 3436 3535 342e 2049 6e20  022.3146554. In 
-000030b0: 7468 6520 7669 6465 6f2c 2074 6865 2072  the video, the r
-000030c0: 6f62 6f74 2069 7320 636f 6e74 726f 6c6c  obot is controll
-000030d0: 6564 2075 7369 6e67 2074 6865 2052 6f62  ed using the Rob
-000030e0: 6f74 6963 7320 746f 6f6c 626f 7820 666f  otics toolbox fo
-000030f0: 7220 5079 7468 6f6e 2061 6e64 2066 6561  r Python and fea
-00003100: 7475 7265 7320 6120 7265 636f 7264 696e  tures a recordin
-00003110: 6720 6672 6f6d 2074 6865 205b 5377 6966  g from the [Swif
-00003120: 745d 2868 7474 7073 3a2f 2f67 6974 6875  t](https://githu
-00003130: 622e 636f 6d2f 6a68 6176 6c2f 7377 6966  b.com/jhavl/swif
-00003140: 7429 2053 696d 756c 6174 6f72 2e0a 0a5b  t) Simulator...[
-00003150: 5b41 7278 6976 2050 6170 6572 5d28 6874  [Arxiv Paper](ht
-00003160: 7470 733a 2f2f 6172 7869 762e 6f72 672f  tps://arxiv.org/
-00003170: 6162 732f 3231 3039 2e30 3437 3439 295d  abs/2109.04749)]
-00003180: 205b 5b49 4545 4520 5870 6c6f 7265 5d28   [[IEEE Xplore](
-00003190: 6874 7470 733a 2f2f 6965 6565 7870 6c6f  https://ieeexplo
-000031a0: 7265 2e69 6565 652e 6f72 672f 6162 7374  re.ieee.org/abst
-000031b0: 7261 6374 2f64 6f63 756d 656e 742f 3936  ract/document/96
-000031c0: 3935 3239 3829 5d20 5b5b 5072 6f6a 6563  95298)] [[Projec
-000031d0: 7420 5765 6273 6974 655d 2868 7474 7073  t Website](https
-000031e0: 3a2f 2f6a 6861 766c 2e67 6974 6875 622e  ://jhavl.github.
-000031f0: 696f 2f68 6f6c 6973 7469 632f 295d 205b  io/holistic/)] [
-00003200: 5b56 6964 656f 5d28 6874 7470 733a 2f2f  [Video](https://
-00003210: 796f 7574 752e 6265 2f2d 4458 4251 5065  youtu.be/-DXBQPe
-00003220: 4c49 5634 295d 205b 5b43 6f64 6520 4578  LIV4)] [[Code Ex
-00003230: 616d 706c 655d 2868 7474 7073 3a2f 2f67  ample](https://g
-00003240: 6974 6875 622e 636f 6d2f 7065 7465 7263  ithub.com/peterc
-00003250: 6f72 6b65 2f72 6f62 6f74 6963 732d 746f  orke/robotics-to
-00003260: 6f6c 626f 782d 7079 7468 6f6e 2f62 6c6f  olbox-python/blo
-00003270: 622f 6d61 7374 6572 2f72 6f62 6f74 6963  b/master/robotic
-00003280: 7374 6f6f 6c62 6f78 2f65 7861 6d70 6c65  stoolbox/example
-00003290: 732f 686f 6c69 7374 6963 5f6d 6d5f 6e6f  s/holistic_mm_no
-000032a0: 6e5f 686f 6c6f 6e6f 6d69 632e 7079 295d  n_holonomic.py)]
-000032b0: 0a0a 3c70 3e0a 2020 3c61 2068 7265 663d  ..<p>.  <a href=
-000032c0: 2268 7474 7073 3a2f 2f79 6f75 7475 2e62  "https://youtu.b
-000032d0: 652f 2d44 5842 5150 654c 4956 3422 3e0a  e/-DXBQPeLIV4">.
-000032e0: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
-000032f0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00003300: 2f70 6574 6572 636f 726b 652f 726f 626f  /petercorke/robo
-00003310: 7469 6373 2d74 6f6f 6c62 6f78 2d70 7974  tics-toolbox-pyt
-00003320: 686f 6e2f 7261 772f 6d61 7374 6572 2f64  hon/raw/master/d
-00003330: 6f63 732f 6669 6773 2f68 6f6c 6973 7469  ocs/figs/holisti
-00003340: 635f 796f 7574 7562 652e 706e 6722 2077  c_youtube.png" w
-00003350: 6964 7468 3d22 3536 3022 3e0a 2020 3c2f  idth="560">.  </
-00003360: 613e 0a3c 2f70 3e0a 0a4a 2e20 4861 7669  a>.</p>..J. Havi
-00003370: 6c61 6e64 2061 6e64 2050 2e20 436f 726b  land and P. Cork
-00003380: 652c 2022 2a2a 4e45 4f3a 2041 204e 6f76  e, "**NEO: A Nov
-00003390: 656c 2045 7870 6564 6974 696f 7573 204f  el Expeditious O
-000033a0: 7074 696d 6973 6174 696f 6e20 416c 676f  ptimisation Algo
-000033b0: 7269 7468 6d20 666f 7220 5265 6163 7469  rithm for Reacti
-000033c0: 7665 204d 6f74 696f 6e20 436f 6e74 726f  ve Motion Contro
-000033d0: 6c20 6f66 204d 616e 6970 756c 6174 6f72  l of Manipulator
-000033e0: 732a 2a2c 2220 696e 205f 4945 4545 2052  s**," in _IEEE R
-000033f0: 6f62 6f74 6963 7320 616e 6420 4175 746f  obotics and Auto
-00003400: 6d61 7469 6f6e 204c 6574 7465 7273 5f2c  mation Letters_,
-00003410: 2064 6f69 3a20 3130 2e31 3130 392f 4c52   doi: 10.1109/LR
-00003420: 412e 3230 3231 2e33 3035 3630 3630 2e20  A.2021.3056060. 
-00003430: 496e 2074 6865 2076 6964 656f 2c20 7468  In the video, th
-00003440: 6520 726f 626f 7420 6973 2063 6f6e 7472  e robot is contr
-00003450: 6f6c 6c65 6420 7573 696e 6720 7468 6520  olled using the 
-00003460: 526f 626f 7469 6373 2074 6f6f 6c62 6f78  Robotics toolbox
-00003470: 2066 6f72 2050 7974 686f 6e20 616e 6420   for Python and 
-00003480: 6665 6174 7572 6573 2061 2072 6563 6f72  features a recor
-00003490: 6469 6e67 2066 726f 6d20 7468 6520 5b53  ding from the [S
-000034a0: 7769 6674 5d28 6874 7470 733a 2f2f 6769  wift](https://gi
-000034b0: 7468 7562 2e63 6f6d 2f6a 6861 766c 2f73  thub.com/jhavl/s
-000034c0: 7769 6674 2920 5369 6d75 6c61 746f 722e  wift) Simulator.
-000034d0: 0a0a 5b5b 4172 7869 7620 5061 7065 725d  ..[[Arxiv Paper]
-000034e0: 2868 7474 7073 3a2f 2f61 7278 6976 2e6f  (https://arxiv.o
-000034f0: 7267 2f61 6273 2f32 3031 302e 3038 3638  rg/abs/2010.0868
-00003500: 3629 5d20 5b5b 4945 4545 2058 706c 6f72  6)] [[IEEE Xplor
-00003510: 655d 2868 7474 7073 3a2f 2f69 6565 6578  e](https://ieeex
-00003520: 706c 6f72 652e 6965 6565 2e6f 7267 2f64  plore.ieee.org/d
-00003530: 6f63 756d 656e 742f 3933 3433 3731 3829  ocument/9343718)
-00003540: 5d20 5b5b 5072 6f6a 6563 7420 5765 6273  ] [[Project Webs
-00003550: 6974 655d 2868 7474 7073 3a2f 2f6a 6861  ite](https://jha
-00003560: 766c 2e67 6974 6875 622e 696f 2f6e 656f  vl.github.io/neo
-00003570: 2f29 5d20 5b5b 5669 6465 6f5d 2868 7474  /)] [[Video](htt
-00003580: 7073 3a2f 2f79 6f75 7475 2e62 652f 6a53  ps://youtu.be/jS
-00003590: 4c50 4a42 7238 5154 5929 5d20 5b5b 436f  LPJBr8QTY)] [[Co
-000035a0: 6465 2045 7861 6d70 6c65 5d28 6874 7470  de Example](http
-000035b0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
-000035c0: 6574 6572 636f 726b 652f 726f 626f 7469  etercorke/roboti
-000035d0: 6373 2d74 6f6f 6c62 6f78 2d70 7974 686f  cs-toolbox-pytho
-000035e0: 6e2f 626c 6f62 2f6d 6173 7465 722f 726f  n/blob/master/ro
-000035f0: 626f 7469 6373 746f 6f6c 626f 782f 6578  boticstoolbox/ex
-00003600: 616d 706c 6573 2f6e 656f 2e70 7929 5d0a  amples/neo.py)].
-00003610: 0a3c 703e 0a20 203c 6120 6872 6566 3d22  .<p>.  <a href="
-00003620: 6874 7470 733a 2f2f 796f 7574 752e 6265  https://youtu.be
-00003630: 2f6a 534c 504a 4272 3851 5459 223e 0a20  /jSLPJBr8QTY">. 
-00003640: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
-00003650: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00003660: 7065 7465 7263 6f72 6b65 2f72 6f62 6f74  petercorke/robot
-00003670: 6963 732d 746f 6f6c 626f 782d 7079 7468  ics-toolbox-pyth
-00003680: 6f6e 2f72 6177 2f6d 6173 7465 722f 646f  on/raw/master/do
-00003690: 6373 2f66 6967 732f 6e65 6f5f 796f 7574  cs/figs/neo_yout
-000036a0: 7562 652e 706e 6722 2077 6964 7468 3d22  ube.png" width="
-000036b0: 3536 3022 3e0a 2020 3c2f 613e 0a3c 2f70  560">.  </a>.</p
-000036c0: 3e0a 0a2a 2a41 2050 7572 656c 792d 5265  >..**A Purely-Re
-000036d0: 6163 7469 7665 204d 616e 6970 756c 6162  active Manipulab
-000036e0: 696c 6974 792d 4d61 7869 6d69 7369 6e67  ility-Maximising
-000036f0: 204d 6f74 696f 6e20 436f 6e74 726f 6c6c   Motion Controll
-00003700: 6572 2a2a 2c20 4a2e 2048 6176 696c 616e  er**, J. Havilan
-00003710: 6420 616e 6420 502e 2043 6f72 6b65 2e20  d and P. Corke. 
-00003720: 496e 2074 6865 2076 6964 656f 2c20 7468  In the video, th
-00003730: 6520 726f 626f 7420 6973 2063 6f6e 7472  e robot is contr
-00003740: 6f6c 6c65 6420 7573 696e 6720 7468 6520  olled using the 
-00003750: 526f 626f 7469 6373 2074 6f6f 6c62 6f78  Robotics toolbox
-00003760: 2066 6f72 2050 7974 686f 6e2e 0a0a 5b5b   for Python...[[
-00003770: 5061 7065 725d 2868 7474 7073 3a2f 2f61  Paper](https://a
-00003780: 7278 6976 2e6f 7267 2f61 6273 2f32 3030  rxiv.org/abs/200
-00003790: 322e 3131 3930 3129 5d20 5b5b 5072 6f6a  2.11901)] [[Proj
-000037a0: 6563 7420 5765 6273 6974 655d 2868 7474  ect Website](htt
-000037b0: 7073 3a2f 2f6a 6861 766c 2e67 6974 6875  ps://jhavl.githu
-000037c0: 622e 696f 2f6d 6d63 2f29 5d20 5b5b 5669  b.io/mmc/)] [[Vi
-000037d0: 6465 6f5d 2868 7474 7073 3a2f 2f79 6f75  deo](https://you
-000037e0: 7475 2e62 652f 5675 5f72 6350 6c61 4144  tu.be/Vu_rcPlaAD
-000037f0: 4929 5d20 5b5b 436f 6465 2045 7861 6d70  I)] [[Code Examp
-00003800: 6c65 5d28 6874 7470 733a 2f2f 6769 7468  le](https://gith
-00003810: 7562 2e63 6f6d 2f70 6574 6572 636f 726b  ub.com/petercork
-00003820: 652f 726f 626f 7469 6373 2d74 6f6f 6c62  e/robotics-toolb
-00003830: 6f78 2d70 7974 686f 6e2f 626c 6f62 2f6d  ox-python/blob/m
-00003840: 6173 7465 722f 726f 626f 7469 6373 746f  aster/roboticsto
-00003850: 6f6c 626f 782f 6578 616d 706c 6573 2f6d  olbox/examples/m
-00003860: 6d63 2e70 7929 5d0a 0a3c 703e 0a20 203c  mc.py)]..<p>.  <
-00003870: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00003880: 796f 7574 752e 6265 2f56 755f 7263 506c  youtu.be/Vu_rcPl
-00003890: 6141 4449 223e 0a20 2020 203c 696d 6720  aADI">.    <img 
-000038a0: 7372 633d 2268 7474 7073 3a2f 2f67 6974  src="https://git
-000038b0: 6875 622e 636f 6d2f 7065 7465 7263 6f72  hub.com/petercor
-000038c0: 6b65 2f72 6f62 6f74 6963 732d 746f 6f6c  ke/robotics-tool
-000038d0: 626f 782d 7079 7468 6f6e 2f72 6177 2f6d  box-python/raw/m
-000038e0: 6173 7465 722f 646f 6373 2f66 6967 732f  aster/docs/figs/
-000038f0: 6d6d 635f 796f 7574 7562 652e 706e 6722  mmc_youtube.png"
-00003900: 2077 6964 7468 3d22 3536 3022 3e0a 2020   width="560">.  
-00003910: 3c2f 613e 0a3c 2f70 3e0a 0a3c 6272 3e0a  </a>.</p>..<br>.
-00003920: 0a3c 6272 3e0a 0a3c 6120 6964 3d27 3627  .<br>..<a id='6'
-00003930: 3e3c 2f61 3e0a 0a23 2320 546f 6f6c 626f  ></a>..## Toolbo
-00003940: 7820 4943 5241 2050 6170 6572 2061 6e64  x ICRA Paper and
-00003950: 2043 6974 6174 696f 6e20 496e 666f 0a0a   Citation Info..
-00003960: 4368 6563 6b20 6f75 7420 6f75 7220 4943  Check out our IC
-00003970: 5241 2032 3032 3120 7061 7065 7220 6f6e  RA 2021 paper on
-00003980: 205b 4945 4545 2058 706c 6f72 655d 2868   [IEEE Xplore](h
-00003990: 7474 7073 3a2f 2f69 6565 6578 706c 6f72  ttps://ieeexplor
-000039a0: 652e 6965 6565 2e6f 7267 2f64 6f63 756d  e.ieee.org/docum
-000039b0: 656e 742f 3935 3631 3336 3629 206f 7220  ent/9561366) or 
-000039c0: 6765 7420 7468 6520 5044 4620 6672 6f6d  get the PDF from
-000039d0: 205b 5065 7465 7227 7320 7765 6273 6974   [Peter's websit
-000039e0: 655d 2868 7474 7073 3a2f 2f62 6974 2e6c  e](https://bit.l
-000039f0: 792f 3343 6863 794e 7029 2e0a 0a49 6620  y/3ChcyNp)...If 
-00003a00: 7468 6520 746f 6f6c 626f 7820 6865 6c70  the toolbox help
-00003a10: 6564 2079 6f75 2069 6e20 796f 7572 2072  ed you in your r
-00003a20: 6573 6561 7263 682c 2070 6c65 6173 6520  esearch, please 
-00003a30: 6369 7465 0a0a 6060 600a 4069 6e70 726f  cite..```.@inpro
-00003a40: 6365 6564 696e 6773 7b72 7462 2c0a 2020  ceedings{rtb,.  
-00003a50: 7469 746c 653d 7b4e 6f74 2079 6f75 7220  title={Not your 
-00003a60: 6772 616e 646d 6f74 6865 72e2 8099 7320  grandmother...s 
-00003a70: 746f 6f6c 626f 782d 2d74 6865 2052 6f62  toolbox--the Rob
-00003a80: 6f74 6963 7320 546f 6f6c 626f 7820 7265  otics Toolbox re
-00003a90: 696e 7665 6e74 6564 2066 6f72 2050 7974  invented for Pyt
-00003aa0: 686f 6e7d 2c0a 2020 6175 7468 6f72 3d7b  hon},.  author={
-00003ab0: 436f 726b 652c 2050 6574 6572 2061 6e64  Corke, Peter and
-00003ac0: 2048 6176 696c 616e 642c 204a 6573 7365   Haviland, Jesse
-00003ad0: 7d2c 0a20 2062 6f6f 6b74 6974 6c65 3d7b  },.  booktitle={
-00003ae0: 3230 3231 2049 4545 4520 496e 7465 726e  2021 IEEE Intern
-00003af0: 6174 696f 6e61 6c20 436f 6e66 6572 656e  ational Conferen
-00003b00: 6365 206f 6e20 526f 626f 7469 6373 2061  ce on Robotics a
-00003b10: 6e64 2041 7574 6f6d 6174 696f 6e20 2849  nd Automation (I
-00003b20: 4352 4129 7d2c 0a20 2070 6167 6573 3d7b  CRA)},.  pages={
-00003b30: 3131 3335 372d 2d31 3133 3633 7d2c 0a20  11357--11363},. 
-00003b40: 2079 6561 723d 7b32 3032 317d 2c0a 2020   year={2021},.  
-00003b50: 6f72 6761 6e69 7a61 7469 6f6e 3d7b 4945  organization={IE
-00003b60: 4545 7d0a 7d0a 6060 600a 0a3c 6272 3e0a  EE}.}.```..<br>.
-00003b70: 0a3c 6120 6964 3d27 3727 3e3c 2f61 3e0a  .<a id='7'></a>.
-00003b80: 0a23 2320 5573 696e 6720 7468 6520 546f  .## Using the To
-00003b90: 6f6c 626f 7820 696e 2079 6f75 7220 4f70  olbox in your Op
-00003ba0: 656e 2053 6f75 7263 6520 436f 6465 3f0a  en Source Code?.
-00003bb0: 0a49 6620 796f 7520 6172 6520 7573 696e  .If you are usin
-00003bc0: 6720 7468 6520 546f 6f6c 626f 7820 696e  g the Toolbox in
-00003bd0: 2079 6f75 7220 6f70 656e 2073 6f75 7263   your open sourc
-00003be0: 6520 636f 6465 2c20 6665 656c 2066 7265  e code, feel fre
-00003bf0: 6520 746f 2061 6464 206f 7572 2062 6164  e to add our bad
-00003c00: 6765 2074 6f20 796f 7572 2072 6561 646d  ge to your readm
-00003c10: 6521 0a0a 466f 7220 7468 6520 706f 7765  e!..For the powe
-00003c20: 7265 6420 6279 2072 6f62 6f74 6963 7320  red by robotics 
-00003c30: 746f 6f6c 626f 7820 6261 6467 650a 0a5b  toolbox badge..[
-00003c40: 215b 506f 7765 7265 6420 6279 2074 6865  ![Powered by the
-00003c50: 2052 6f62 6f74 6963 7320 546f 6f6c 626f   Robotics Toolbo
-00003c60: 785d 2868 7474 7073 3a2f 2f72 6177 2e67  x](https://raw.g
-00003c70: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
-00003c80: 2e63 6f6d 2f70 6574 6572 636f 726b 652f  .com/petercorke/
-00003c90: 726f 626f 7469 6373 2d74 6f6f 6c62 6f78  robotics-toolbox
-00003ca0: 2d70 7974 686f 6e2f 6d61 7374 6572 2f2e  -python/master/.
-00003cb0: 6769 7468 7562 2f73 7667 2f72 7462 5f70  github/svg/rtb_p
-00003cc0: 6f77 6572 6564 2e6d 696e 2e73 7667 295d  owered.min.svg)]
-00003cd0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00003ce0: 636f 6d2f 7065 7465 7263 6f72 6b65 2f72  com/petercorke/r
-00003cf0: 6f62 6f74 6963 732d 746f 6f6c 626f 782d  obotics-toolbox-
-00003d00: 7079 7468 6f6e 290a 0a63 6f70 7920 7468  python)..copy th
-00003d10: 6520 666f 6c6c 6f77 696e 670a 0a60 6060  e following..```
-00003d20: 0a5b 215b 506f 7765 7265 6420 6279 2074  .[![Powered by t
-00003d30: 6865 2052 6f62 6f74 6963 7320 546f 6f6c  he Robotics Tool
-00003d40: 626f 785d 2868 7474 7073 3a2f 2f72 6177  box](https://raw
-00003d50: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
-00003d60: 6e74 2e63 6f6d 2f70 6574 6572 636f 726b  nt.com/petercork
-00003d70: 652f 726f 626f 7469 6373 2d74 6f6f 6c62  e/robotics-toolb
-00003d80: 6f78 2d70 7974 686f 6e2f 6d61 7374 6572  ox-python/master
-00003d90: 2f2e 6769 7468 7562 2f73 7667 2f72 7462  /.github/svg/rtb
-00003da0: 5f70 6f77 6572 6564 2e6d 696e 2e73 7667  _powered.min.svg
-00003db0: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
-00003dc0: 622e 636f 6d2f 7065 7465 7263 6f72 6b65  b.com/petercorke
-00003dd0: 2f72 6f62 6f74 6963 732d 746f 6f6c 626f  /robotics-toolbo
-00003de0: 782d 7079 7468 6f6e 290a 6060 600a 0a46  x-python).```..F
-00003df0: 6f72 2074 6865 2070 6f77 6572 6564 2062  or the powered b
-00003e00: 7920 7079 7468 6f6e 2072 6f62 6f74 6963  y python robotic
-00003e10: 7320 6261 6467 650a 0a5b 215b 506f 7765  s badge..[![Powe
-00003e20: 7265 6420 6279 2050 7974 686f 6e20 526f  red by Python Ro
-00003e30: 626f 7469 6373 5d28 6874 7470 733a 2f2f  botics](https://
-00003e40: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
-00003e50: 6e74 656e 742e 636f 6d2f 7065 7465 7263  ntent.com/peterc
-00003e60: 6f72 6b65 2f72 6f62 6f74 6963 732d 746f  orke/robotics-to
-00003e70: 6f6c 626f 782d 7079 7468 6f6e 2f6d 6173  olbox-python/mas
-00003e80: 7465 722f 2e67 6974 6875 622f 7376 672f  ter/.github/svg/
-00003e90: 7072 5f70 6f77 6572 6564 2e6d 696e 2e73  pr_powered.min.s
-00003ea0: 7667 295d 2868 7474 7073 3a2f 2f67 6974  vg)](https://git
-00003eb0: 6875 622e 636f 6d2f 7065 7465 7263 6f72  hub.com/petercor
-00003ec0: 6b65 2f72 6f62 6f74 6963 732d 746f 6f6c  ke/robotics-tool
-00003ed0: 626f 782d 7079 7468 6f6e 290a 0a63 6f70  box-python)..cop
-00003ee0: 7920 7468 6520 666f 6c6c 6f77 696e 670a  y the following.
-00003ef0: 0a60 6060 0a5b 215b 506f 7765 7265 6420  .```.[![Powered 
-00003f00: 6279 2050 7974 686f 6e20 526f 626f 7469  by Python Roboti
-00003f10: 6373 5d28 6874 7470 733a 2f2f 7261 772e  cs](https://raw.
-00003f20: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
-00003f30: 742e 636f 6d2f 7065 7465 7263 6f72 6b65  t.com/petercorke
-00003f40: 2f72 6f62 6f74 6963 732d 746f 6f6c 626f  /robotics-toolbo
-00003f50: 782d 7079 7468 6f6e 2f6d 6173 7465 722f  x-python/master/
-00003f60: 2e67 6974 6875 622f 7376 672f 7072 5f70  .github/svg/pr_p
-00003f70: 6f77 6572 6564 2e6d 696e 2e73 7667 295d  owered.min.svg)]
-00003f80: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00003f90: 636f 6d2f 7065 7465 7263 6f72 6b65 2f72  com/petercorke/r
-00003fa0: 6f62 6f74 6963 732d 746f 6f6c 626f 782d  obotics-toolbox-
-00003fb0: 7079 7468 6f6e 290a 6060 600a 0a3c 6272  python).```..<br
-00003fc0: 3e0a 0a3c 6120 6964 3d27 3827 3e3c 2f61  >..<a id='8'></a
-00003fd0: 3e0a 0a23 2320 436f 6d6d 6f6e 2049 7373  >..## Common Iss
-00003fe0: 7565 7320 616e 6420 536f 6c75 7469 6f6e  ues and Solution
-00003ff0: 730a 0a53 6565 2074 6865 2063 6f6d 6d6f  s..See the commo
-00004000: 6e20 6973 7375 6573 2077 6974 6820 6669  n issues with fi
-00004010: 7865 7320 5b68 6572 655d 2868 7474 7073  xes [here](https
-00004020: 3a2f 2f67 6974 6875 622e 636f 6d2f 7065  ://github.com/pe
-00004030: 7465 7263 6f72 6b65 2f72 6f62 6f74 6963  tercorke/robotic
-00004040: 732d 746f 6f6c 626f 782d 7079 7468 6f6e  s-toolbox-python
-00004050: 2f77 696b 692f 436f 6d6d 6f6e 2d49 7373  /wiki/Common-Iss
-00004060: 7565 7329 2e0a                           ues)..
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 726f 626f  : 2.1.Name: robo
+00000020: 7469 6373 746f 6f6c 626f 782d 7079 7468  ticstoolbox-pyth
+00000030: 6f6e 0a56 6572 7369 6f6e 3a20 312e 312e  on.Version: 1.1.
+00000040: 310a 5375 6d6d 6172 793a 2041 2050 7974  1.Summary: A Pyt
+00000050: 686f 6e20 6c69 6272 6172 7920 666f 7220  hon library for 
+00000060: 726f 626f 7469 6373 2065 6475 6361 7469  robotics educati
+00000070: 6f6e 2061 6e64 2072 6573 6561 7263 680a  on and research.
+00000080: 4175 7468 6f72 2d65 6d61 696c 3a20 4a65  Author-email: Je
+00000090: 7373 6520 4861 7669 6c61 6e64 203c 6a2e  sse Haviland <j.
+000000a0: 6861 7669 6c61 6e64 4071 7574 2e65 6475  haviland@qut.edu
+000000b0: 2e61 753e 2c20 5065 7465 7220 436f 726b  .au>, Peter Cork
+000000c0: 6520 3c72 7663 4070 6574 6572 636f 726b  e <rvc@petercork
+000000d0: 652e 636f 6d3e 0a4c 6963 656e 7365 3a20  e.com>.License: 
+000000e0: 4d49 5420 4c69 6365 6e73 650a 2020 2020  MIT License.    
+000000f0: 2020 2020 0a20 2020 2020 2020 2043 6f70      .        Cop
+00000100: 7972 6967 6874 2028 6329 2032 3032 3020  yright (c) 2020 
+00000110: 6a68 6176 6c0a 2020 2020 2020 2020 0a20  jhavl.        . 
+00000120: 2020 2020 2020 2050 6572 6d69 7373 696f         Permissio
+00000130: 6e20 6973 2068 6572 6562 7920 6772 616e  n is hereby gran
+00000140: 7465 642c 2066 7265 6520 6f66 2063 6861  ted, free of cha
+00000150: 7267 652c 2074 6f20 616e 7920 7065 7273  rge, to any pers
+00000160: 6f6e 206f 6274 6169 6e69 6e67 2061 2063  on obtaining a c
+00000170: 6f70 790a 2020 2020 2020 2020 6f66 2074  opy.        of t
+00000180: 6869 7320 736f 6674 7761 7265 2061 6e64  his software and
+00000190: 2061 7373 6f63 6961 7465 6420 646f 6375   associated docu
+000001a0: 6d65 6e74 6174 696f 6e20 6669 6c65 7320  mentation files 
+000001b0: 2874 6865 2022 536f 6674 7761 7265 2229  (the "Software")
+000001c0: 2c20 746f 2064 6561 6c0a 2020 2020 2020  , to deal.      
+000001d0: 2020 696e 2074 6865 2053 6f66 7477 6172    in the Softwar
+000001e0: 6520 7769 7468 6f75 7420 7265 7374 7269  e without restri
+000001f0: 6374 696f 6e2c 2069 6e63 6c75 6469 6e67  ction, including
+00000200: 2077 6974 686f 7574 206c 696d 6974 6174   without limitat
+00000210: 696f 6e20 7468 6520 7269 6768 7473 0a20  ion the rights. 
+00000220: 2020 2020 2020 2074 6f20 7573 652c 2063         to use, c
+00000230: 6f70 792c 206d 6f64 6966 792c 206d 6572  opy, modify, mer
+00000240: 6765 2c20 7075 626c 6973 682c 2064 6973  ge, publish, dis
+00000250: 7472 6962 7574 652c 2073 7562 6c69 6365  tribute, sublice
+00000260: 6e73 652c 2061 6e64 2f6f 7220 7365 6c6c  nse, and/or sell
+00000270: 0a20 2020 2020 2020 2063 6f70 6965 7320  .        copies 
+00000280: 6f66 2074 6865 2053 6f66 7477 6172 652c  of the Software,
+00000290: 2061 6e64 2074 6f20 7065 726d 6974 2070   and to permit p
+000002a0: 6572 736f 6e73 2074 6f20 7768 6f6d 2074  ersons to whom t
+000002b0: 6865 2053 6f66 7477 6172 6520 6973 0a20  he Software is. 
+000002c0: 2020 2020 2020 2066 7572 6e69 7368 6564         furnished
+000002d0: 2074 6f20 646f 2073 6f2c 2073 7562 6a65   to do so, subje
+000002e0: 6374 2074 6f20 7468 6520 666f 6c6c 6f77  ct to the follow
+000002f0: 696e 6720 636f 6e64 6974 696f 6e73 3a0a  ing conditions:.
+00000300: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00000310: 2054 6865 2061 626f 7665 2063 6f70 7972   The above copyr
+00000320: 6967 6874 206e 6f74 6963 6520 616e 6420  ight notice and 
+00000330: 7468 6973 2070 6572 6d69 7373 696f 6e20  this permission 
+00000340: 6e6f 7469 6365 2073 6861 6c6c 2062 6520  notice shall be 
+00000350: 696e 636c 7564 6564 2069 6e20 616c 6c0a  included in all.
+00000360: 2020 2020 2020 2020 636f 7069 6573 206f          copies o
+00000370: 7220 7375 6273 7461 6e74 6961 6c20 706f  r substantial po
+00000380: 7274 696f 6e73 206f 6620 7468 6520 536f  rtions of the So
+00000390: 6674 7761 7265 2e0a 2020 2020 2020 2020  ftware..        
+000003a0: 0a20 2020 2020 2020 2054 4845 2053 4f46  .        THE SOF
+000003b0: 5457 4152 4520 4953 2050 524f 5649 4445  TWARE IS PROVIDE
+000003c0: 4420 2241 5320 4953 222c 2057 4954 484f  D "AS IS", WITHO
+000003d0: 5554 2057 4152 5241 4e54 5920 4f46 2041  UT WARRANTY OF A
+000003e0: 4e59 204b 494e 442c 2045 5850 5245 5353  NY KIND, EXPRESS
+000003f0: 204f 520a 2020 2020 2020 2020 494d 504c   OR.        IMPL
+00000400: 4945 442c 2049 4e43 4c55 4449 4e47 2042  IED, INCLUDING B
+00000410: 5554 204e 4f54 204c 494d 4954 4544 2054  UT NOT LIMITED T
+00000420: 4f20 5448 4520 5741 5252 414e 5449 4553  O THE WARRANTIES
+00000430: 204f 4620 4d45 5243 4841 4e54 4142 494c   OF MERCHANTABIL
+00000440: 4954 592c 0a20 2020 2020 2020 2046 4954  ITY,.        FIT
+00000450: 4e45 5353 2046 4f52 2041 2050 4152 5449  NESS FOR A PARTI
+00000460: 4355 4c41 5220 5055 5250 4f53 4520 414e  CULAR PURPOSE AN
+00000470: 4420 4e4f 4e49 4e46 5249 4e47 454d 454e  D NONINFRINGEMEN
+00000480: 542e 2049 4e20 4e4f 2045 5645 4e54 2053  T. IN NO EVENT S
+00000490: 4841 4c4c 2054 4845 0a20 2020 2020 2020  HALL THE.       
+000004a0: 2041 5554 484f 5253 204f 5220 434f 5059   AUTHORS OR COPY
+000004b0: 5249 4748 5420 484f 4c44 4552 5320 4245  RIGHT HOLDERS BE
+000004c0: 204c 4941 424c 4520 464f 5220 414e 5920   LIABLE FOR ANY 
+000004d0: 434c 4149 4d2c 2044 414d 4147 4553 204f  CLAIM, DAMAGES O
+000004e0: 5220 4f54 4845 520a 2020 2020 2020 2020  R OTHER.        
+000004f0: 4c49 4142 494c 4954 592c 2057 4845 5448  LIABILITY, WHETH
+00000500: 4552 2049 4e20 414e 2041 4354 494f 4e20  ER IN AN ACTION 
+00000510: 4f46 2043 4f4e 5452 4143 542c 2054 4f52  OF CONTRACT, TOR
+00000520: 5420 4f52 204f 5448 4552 5749 5345 2c20  T OR OTHERWISE, 
+00000530: 4152 4953 494e 4720 4652 4f4d 2c0a 2020  ARISING FROM,.  
+00000540: 2020 2020 2020 4f55 5420 4f46 204f 5220        OUT OF OR 
+00000550: 494e 2043 4f4e 4e45 4354 494f 4e20 5749  IN CONNECTION WI
+00000560: 5448 2054 4845 2053 4f46 5457 4152 4520  TH THE SOFTWARE 
+00000570: 4f52 2054 4845 2055 5345 204f 5220 4f54  OR THE USE OR OT
+00000580: 4845 5220 4445 414c 494e 4753 2049 4e20  HER DEALINGS IN 
+00000590: 5448 450a 2020 2020 2020 2020 534f 4654  THE.        SOFT
+000005a0: 5741 5245 2e0a 2020 2020 2020 2020 0a50  WARE..        .P
+000005b0: 726f 6a65 6374 2d55 524c 3a20 686f 6d65  roject-URL: home
+000005c0: 7061 6765 2c20 6874 7470 733a 2f2f 6769  page, https://gi
+000005d0: 7468 7562 2e63 6f6d 2f70 6574 6572 636f  thub.com/peterco
+000005e0: 726b 652f 726f 626f 7469 6373 2d74 6f6f  rke/robotics-too
+000005f0: 6c62 6f78 2d70 7974 686f 6e0a 5072 6f6a  lbox-python.Proj
+00000600: 6563 742d 5552 4c3a 2064 6f63 756d 656e  ect-URL: documen
+00000610: 7461 7469 6f6e 2c20 6874 7470 733a 2f2f  tation, https://
+00000620: 7065 7465 7263 6f72 6b65 2e67 6974 6875  petercorke.githu
+00000630: 622e 696f 2f72 6f62 6f74 6963 732d 746f  b.io/robotics-to
+00000640: 6f6c 626f 782d 7079 7468 6f6e 2f0a 5072  olbox-python/.Pr
+00000650: 6f6a 6563 742d 5552 4c3a 2072 6570 6f73  oject-URL: repos
+00000660: 6974 6f72 792c 2068 7474 7073 3a2f 2f67  itory, https://g
+00000670: 6974 6875 622e 636f 6d2f 7065 7465 7263  ithub.com/peterc
+00000680: 6f72 6b65 2f72 6f62 6f74 6963 732d 746f  orke/robotics-to
+00000690: 6f6c 626f 782d 7079 7468 6f6e 0a4b 6579  olbox-python.Key
+000006a0: 776f 7264 733a 2070 7974 686f 6e2c 726f  words: python,ro
+000006b0: 626f 7469 6373 2c72 6f62 6f74 6963 732d  botics,robotics-
+000006c0: 746f 6f6c 626f 782c 6b69 6e65 6d61 7469  toolbox,kinemati
+000006d0: 6373 2c64 796e 616d 6963 732c 6d6f 7469  cs,dynamics,moti
+000006e0: 6f6e 2d70 6c61 6e6e 696e 672c 7472 616a  on-planning,traj
+000006f0: 6563 746f 7279 2d67 656e 6572 6174 696f  ectory-generatio
+00000700: 6e2c 6a61 636f 6269 616e 2c68 6573 7369  n,jacobian,hessi
+00000710: 616e 2c63 6f6e 7472 6f6c 2c73 696d 756c  an,control,simul
+00000720: 6174 696f 6e2c 726f 626f 742d 6d61 6e69  ation,robot-mani
+00000730: 7075 6c61 746f 722c 6d6f 6269 6c65 2d72  pulator,mobile-r
+00000740: 6f62 6f74 0a43 6c61 7373 6966 6965 723a  obot.Classifier:
+00000750: 2044 6576 656c 6f70 6d65 6e74 2053 7461   Development Sta
+00000760: 7475 7320 3a3a 2035 202d 2050 726f 6475  tus :: 5 - Produ
+00000770: 6374 696f 6e2f 5374 6162 6c65 0a43 6c61  ction/Stable.Cla
+00000780: 7373 6966 6965 723a 2049 6e74 656e 6465  ssifier: Intende
+00000790: 6420 4175 6469 656e 6365 203a 3a20 4465  d Audience :: De
+000007a0: 7665 6c6f 7065 7273 0a43 6c61 7373 6966  velopers.Classif
+000007b0: 6965 723a 204c 6963 656e 7365 203a 3a20  ier: License :: 
+000007c0: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
+000007d0: 4d49 5420 4c69 6365 6e73 650a 436c 6173  MIT License.Clas
+000007e0: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+000007f0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000800: 5079 7468 6f6e 203a 3a20 332e 370a 436c  Python :: 3.7.Cl
+00000810: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+00000820: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000830: 3a20 5079 7468 6f6e 203a 3a20 332e 380a  : Python :: 3.8.
+00000840: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+00000850: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000860: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000870: 390a 436c 6173 7369 6669 6572 3a20 5072  9.Classifier: Pr
+00000880: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000890: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+000008a0: 332e 3130 0a43 6c61 7373 6966 6965 723a  3.10.Classifier:
+000008b0: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+000008c0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+000008d0: 3a3a 2033 2e31 310a 5265 7175 6972 6573  :: 3.11.Requires
+000008e0: 2d50 7974 686f 6e3a 203e 3d33 2e37 0a44  -Python: >=3.7.D
+000008f0: 6573 6372 6970 7469 6f6e 2d43 6f6e 7465  escription-Conte
+00000900: 6e74 2d54 7970 653a 2074 6578 742f 6d61  nt-Type: text/ma
+00000910: 726b 646f 776e 0a4c 6963 656e 7365 2d46  rkdown.License-F
+00000920: 696c 653a 204c 4943 454e 5345 0a52 6571  ile: LICENSE.Req
+00000930: 7569 7265 732d 4469 7374 3a20 6e75 6d70  uires-Dist: nump
+00000940: 793e 3d31 2e31 372e 340a 5265 7175 6972  y>=1.17.4.Requir
+00000950: 6573 2d44 6973 743a 2073 7061 7469 616c  es-Dist: spatial
+00000960: 6d61 7468 2d70 7974 686f 6e3e 3d31 2e31  math-python>=1.1
+00000970: 2e35 0a52 6571 7569 7265 732d 4469 7374  .5.Requires-Dist
+00000980: 3a20 7370 6174 6961 6c67 656f 6d65 7472  : spatialgeometr
+00000990: 793e 3d31 2e30 2e30 0a52 6571 7569 7265  y>=1.0.0.Require
+000009a0: 732d 4469 7374 3a20 7067 7261 7068 2d70  s-Dist: pgraph-p
+000009b0: 7974 686f 6e0a 5265 7175 6972 6573 2d44  ython.Requires-D
+000009c0: 6973 743a 2073 6369 7079 0a52 6571 7569  ist: scipy.Requi
+000009d0: 7265 732d 4469 7374 3a20 6d61 7470 6c6f  res-Dist: matplo
+000009e0: 746c 6962 0a52 6571 7569 7265 732d 4469  tlib.Requires-Di
+000009f0: 7374 3a20 616e 7369 7461 626c 650a 5265  st: ansitable.Re
+00000a00: 7175 6972 6573 2d44 6973 743a 2073 7769  quires-Dist: swi
+00000a10: 6674 2d73 696d 3e3d 312e 302e 300a 5265  ft-sim>=1.0.0.Re
+00000a20: 7175 6972 6573 2d44 6973 743a 2072 7462  quires-Dist: rtb
+00000a30: 2d64 6174 610a 5265 7175 6972 6573 2d44  -data.Requires-D
+00000a40: 6973 743a 2070 726f 6772 6573 730a 5265  ist: progress.Re
+00000a50: 7175 6972 6573 2d44 6973 743a 2074 7970  quires-Dist: typ
+00000a60: 696e 675f 6578 7465 6e73 696f 6e73 0a50  ing_extensions.P
+00000a70: 726f 7669 6465 732d 4578 7472 613a 2063  rovides-Extra: c
+00000a80: 6f6c 6c69 7369 6f6e 0a52 6571 7569 7265  ollision.Require
+00000a90: 732d 4469 7374 3a20 7079 6275 6c6c 6574  s-Dist: pybullet
+00000aa0: 3b20 6578 7472 6120 3d3d 2022 636f 6c6c  ; extra == "coll
+00000ab0: 6973 696f 6e22 0a50 726f 7669 6465 732d  ision".Provides-
+00000ac0: 4578 7472 613a 2064 6576 0a52 6571 7569  Extra: dev.Requi
+00000ad0: 7265 732d 4469 7374 3a20 626c 6163 6b3b  res-Dist: black;
+00000ae0: 2065 7874 7261 203d 3d20 2264 6576 220a   extra == "dev".
+00000af0: 5265 7175 6972 6573 2d44 6973 743a 2070  Requires-Dist: p
+00000b00: 7974 6573 743b 2065 7874 7261 203d 3d20  ytest; extra == 
+00000b10: 2264 6576 220a 5265 7175 6972 6573 2d44  "dev".Requires-D
+00000b20: 6973 743a 2070 7974 6573 742d 636f 763b  ist: pytest-cov;
+00000b30: 2065 7874 7261 203d 3d20 2264 6576 220a   extra == "dev".
+00000b40: 5265 7175 6972 6573 2d44 6973 743a 2066  Requires-Dist: f
+00000b50: 6c61 6b65 383b 2065 7874 7261 203d 3d20  lake8; extra == 
+00000b60: 2264 6576 220a 5265 7175 6972 6573 2d44  "dev".Requires-D
+00000b70: 6973 743a 2070 7979 616d 6c3b 2065 7874  ist: pyyaml; ext
+00000b80: 7261 203d 3d20 2264 6576 220a 5265 7175  ra == "dev".Requ
+00000b90: 6972 6573 2d44 6973 743a 2073 796d 7079  ires-Dist: sympy
+00000ba0: 3b20 6578 7472 6120 3d3d 2022 6465 7622  ; extra == "dev"
+00000bb0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000bc0: 7170 736f 6c76 6572 733b 2065 7874 7261  qpsolvers; extra
+00000bd0: 203d 3d20 2264 6576 220a 5265 7175 6972   == "dev".Requir
+00000be0: 6573 2d44 6973 743a 2071 7561 6470 726f  es-Dist: quadpro
+00000bf0: 673b 2065 7874 7261 203d 3d20 2264 6576  g; extra == "dev
+00000c00: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+00000c10: 2070 7962 756c 6c65 743b 2065 7874 7261   pybullet; extra
+00000c20: 203d 3d20 2264 6576 220a 5265 7175 6972   == "dev".Requir
+00000c30: 6573 2d44 6973 743a 2062 6473 696d 3b20  es-Dist: bdsim; 
+00000c40: 6578 7472 6120 3d3d 2022 6465 7622 0a50  extra == "dev".P
+00000c50: 726f 7669 6465 732d 4578 7472 613a 2064  rovides-Extra: d
+00000c60: 6f63 730a 5265 7175 6972 6573 2d44 6973  ocs.Requires-Dis
+00000c70: 743a 2073 7068 696e 783b 2065 7874 7261  t: sphinx; extra
+00000c80: 203d 3d20 2264 6f63 7322 0a52 6571 7569   == "docs".Requi
+00000c90: 7265 732d 4469 7374 3a20 7370 6869 6e78  res-Dist: sphinx
+00000ca0: 5f72 7464 5f74 6865 6d65 3b20 6578 7472  _rtd_theme; extr
+00000cb0: 6120 3d3d 2022 646f 6373 220a 5265 7175  a == "docs".Requ
+00000cc0: 6972 6573 2d44 6973 743a 2073 7068 696e  ires-Dist: sphin
+00000cd0: 782d 6175 746f 7275 6e3b 2065 7874 7261  x-autorun; extra
+00000ce0: 203d 3d20 2264 6f63 7322 0a52 6571 7569   == "docs".Requi
+00000cf0: 7265 732d 4469 7374 3a20 7370 6869 6e78  res-Dist: sphinx
+00000d00: 5f61 7574 6f64 6f63 5f74 7970 6568 696e  _autodoc_typehin
+00000d10: 7473 3b20 6578 7472 6120 3d3d 2022 646f  ts; extra == "do
+00000d20: 6373 220a 5265 7175 6972 6573 2d44 6973  cs".Requires-Dis
+00000d30: 743a 2073 7068 696e 782d 6661 7669 636f  t: sphinx-favico
+00000d40: 6e3b 2065 7874 7261 203d 3d20 2264 6f63  n; extra == "doc
+00000d50: 7322 0a0a 2320 526f 626f 7469 6373 2054  s"..# Robotics T
+00000d60: 6f6f 6c62 6f78 2066 6f72 2050 7974 686f  oolbox for Pytho
+00000d70: 6e0a 0a5b 215b 4120 5079 7468 6f6e 2052  n..[![A Python R
+00000d80: 6f62 6f74 6963 7320 5061 636b 6167 655d  obotics Package]
+00000d90: 2868 7474 7073 3a2f 2f72 6177 2e67 6974  (https://raw.git
+00000da0: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+00000db0: 6f6d 2f70 6574 6572 636f 726b 652f 726f  om/petercorke/ro
+00000dc0: 626f 7469 6373 2d74 6f6f 6c62 6f78 2d70  botics-toolbox-p
+00000dd0: 7974 686f 6e2f 6d61 7374 6572 2f2e 6769  ython/master/.gi
+00000de0: 7468 7562 2f73 7667 2f70 795f 636f 6c6c  thub/svg/py_coll
+00000df0: 6563 7469 6f6e 2e6d 696e 2e73 7667 295d  ection.min.svg)]
+00000e00: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000e10: 636f 6d2f 7065 7465 7263 6f72 6b65 2f72  com/petercorke/r
+00000e20: 6f62 6f74 6963 732d 746f 6f6c 626f 782d  obotics-toolbox-
+00000e30: 7079 7468 6f6e 290a 5b21 5b50 6f77 6572  python).[![Power
+00000e40: 6564 2062 7920 5370 6174 6961 6c20 4d61  ed by Spatial Ma
+00000e50: 7468 735d 2868 7474 7073 3a2f 2f72 6177  ths](https://raw
+00000e60: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+00000e70: 6e74 2e63 6f6d 2f70 6574 6572 636f 726b  nt.com/petercork
+00000e80: 652f 7370 6174 6961 6c6d 6174 682d 7079  e/spatialmath-py
+00000e90: 7468 6f6e 2f6d 6173 7465 722f 2e67 6974  thon/master/.git
+00000ea0: 6875 622f 7376 672f 736d 5f70 6f77 6572  hub/svg/sm_power
+00000eb0: 6564 2e6d 696e 2e73 7667 295d 2868 7474  ed.min.svg)](htt
+00000ec0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000ed0: 7065 7465 7263 6f72 6b65 2f73 7061 7469  petercorke/spati
+00000ee0: 616c 6d61 7468 2d70 7974 686f 6e29 0a5b  almath-python).[
+00000ef0: 215b 5155 5420 4365 6e74 7265 2066 6f72  ![QUT Centre for
+00000f00: 2052 6f62 6f74 6963 7320 4f70 656e 2053   Robotics Open S
+00000f10: 6f75 7263 655d 2868 7474 7073 3a2f 2f67  ource](https://g
+00000f20: 6974 6875 622e 636f 6d2f 7163 722f 7163  ithub.com/qcr/qc
+00000f30: 722e 6769 7468 7562 2e69 6f2f 7261 772f  r.github.io/raw/
+00000f40: 6d61 7374 6572 2f6d 6973 632f 6261 6467  master/misc/badg
+00000f50: 652e 7376 6729 5d28 6874 7470 733a 2f2f  e.svg)](https://
+00000f60: 7163 722e 6769 7468 7562 2e69 6f29 0a0a  qcr.github.io)..
+00000f70: 5b21 5b50 7950 4920 7665 7273 696f 6e5d  [![PyPI version]
+00000f80: 2868 7474 7073 3a2f 2f62 6164 6765 2e66  (https://badge.f
+00000f90: 7572 792e 696f 2f70 792f 726f 626f 7469  ury.io/py/roboti
+00000fa0: 6373 746f 6f6c 626f 782d 7079 7468 6f6e  cstoolbox-python
+00000fb0: 2e73 7667 295d 2868 7474 7073 3a2f 2f62  .svg)](https://b
+00000fc0: 6164 6765 2e66 7572 792e 696f 2f70 792f  adge.fury.io/py/
+00000fd0: 726f 626f 7469 6373 746f 6f6c 626f 782d  roboticstoolbox-
+00000fe0: 7079 7468 6f6e 290a 5b21 5b41 6e61 636f  python).[![Anaco
+00000ff0: 6e64 6120 7665 7273 696f 6e5d 2868 7474  nda version](htt
+00001000: 7073 3a2f 2f61 6e61 636f 6e64 612e 6f72  ps://anaconda.or
+00001010: 672f 636f 6e64 612d 666f 7267 652f 726f  g/conda-forge/ro
+00001020: 626f 7469 6373 746f 6f6c 626f 782d 7079  boticstoolbox-py
+00001030: 7468 6f6e 2f62 6164 6765 732f 7665 7273  thon/badges/vers
+00001040: 696f 6e2e 7376 6729 5d28 6874 7470 733a  ion.svg)](https:
+00001050: 2f2f 616e 6163 6f6e 6461 2e6f 7267 2f63  //anaconda.org/c
+00001060: 6f6e 6461 2d66 6f72 6765 2f72 6f62 6f74  onda-forge/robot
+00001070: 6963 7374 6f6f 6c62 6f78 2d70 7974 686f  icstoolbox-pytho
+00001080: 6e29 0a21 5b50 7950 4920 2d20 5079 7468  n).![PyPI - Pyth
+00001090: 6f6e 2056 6572 7369 6f6e 5d28 6874 7470  on Version](http
+000010a0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+000010b0: 696f 2f70 7970 692f 7079 7665 7273 696f  io/pypi/pyversio
+000010c0: 6e73 2f72 6f62 6f74 6963 7374 6f6f 6c62  ns/roboticstoolb
+000010d0: 6f78 2d70 7974 686f 6e2e 7376 6729 0a0a  ox-python.svg)..
+000010e0: 5b21 5b42 7569 6c64 2053 7461 7475 735d  [![Build Status]
+000010f0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00001100: 636f 6d2f 7065 7465 7263 6f72 6b65 2f72  com/petercorke/r
+00001110: 6f62 6f74 6963 732d 746f 6f6c 626f 782d  obotics-toolbox-
+00001120: 7079 7468 6f6e 2f77 6f72 6b66 6c6f 7773  python/workflows
+00001130: 2f54 6573 742f 6261 6467 652e 7376 673f  /Test/badge.svg?
+00001140: 6272 616e 6368 3d6d 6173 7465 7229 5d28  branch=master)](
+00001150: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001160: 6f6d 2f70 6574 6572 636f 726b 652f 726f  om/petercorke/ro
+00001170: 626f 7469 6373 2d74 6f6f 6c62 6f78 2d70  botics-toolbox-p
+00001180: 7974 686f 6e2f 6163 7469 6f6e 733f 7175  ython/actions?qu
+00001190: 6572 793d 776f 726b 666c 6f77 2533 4154  ery=workflow%3AT
+000011a0: 6573 7429 0a5b 215b 436f 7665 7261 6765  est).[![Coverage
+000011b0: 5d28 6874 7470 733a 2f2f 636f 6465 636f  ](https://codeco
+000011c0: 762e 696f 2f67 682f 7065 7465 7263 6f72  v.io/gh/petercor
+000011d0: 6b65 2f72 6f62 6f74 6963 732d 746f 6f6c  ke/robotics-tool
+000011e0: 626f 782d 7079 7468 6f6e 2f62 7261 6e63  box-python/branc
+000011f0: 682f 6d61 7374 6572 2f67 7261 7068 2f62  h/master/graph/b
+00001200: 6164 6765 2e73 7667 295d 2868 7474 7073  adge.svg)](https
+00001210: 3a2f 2f63 6f64 6563 6f76 2e69 6f2f 6768  ://codecov.io/gh
+00001220: 2f70 6574 6572 636f 726b 652f 726f 626f  /petercorke/robo
+00001230: 7469 6373 2d74 6f6f 6c62 6f78 2d70 7974  tics-toolbox-pyt
+00001240: 686f 6e29 0a5b 215b 5079 5049 202d 2044  hon).[![PyPI - D
+00001250: 6f77 6e6c 6f61 6473 5d28 6874 7470 733a  ownloads](https:
+00001260: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00001270: 2f70 7970 692f 6477 2f72 6f62 6f74 6963  /pypi/dw/robotic
+00001280: 7374 6f6f 6c62 6f78 2d70 7974 686f 6e29  stoolbox-python)
+00001290: 5d28 6874 7470 733a 2f2f 7079 7069 7374  ](https://pypist
+000012a0: 6174 732e 6f72 672f 7061 636b 6167 6573  ats.org/packages
+000012b0: 2f72 6f62 6f74 6963 7374 6f6f 6c62 6f78  /roboticstoolbox
+000012c0: 2d70 7974 686f 6e29 0a5b 215b 4c69 6365  -python).[![Lice
+000012d0: 6e73 653a 204d 4954 5d28 6874 7470 733a  nse: MIT](https:
+000012e0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000012f0: 2f62 6164 6765 2f4c 6963 656e 7365 2d4d  /badge/License-M
+00001300: 4954 2d79 656c 6c6f 772e 7376 6729 5d28  IT-yellow.svg)](
+00001310: 6874 7470 733a 2f2f 6f70 656e 736f 7572  https://opensour
+00001320: 6365 2e6f 7267 2f6c 6963 656e 7365 732f  ce.org/licenses/
+00001330: 4d49 5429 0a0a 3c74 6162 6c65 2073 7479  MIT)..<table sty
+00001340: 6c65 3d22 626f 7264 6572 3a30 7078 223e  le="border:0px">
+00001350: 0a3c 7472 2073 7479 6c65 3d22 626f 7264  .<tr style="bord
+00001360: 6572 3a30 7078 223e 0a3c 7464 2073 7479  er:0px">.<td sty
+00001370: 6c65 3d22 626f 7264 6572 3a30 7078 223e  le="border:0px">
+00001380: 0a3c 696d 6720 7372 633d 2268 7474 7073  .<img src="https
+00001390: 3a2f 2f67 6974 6875 622e 636f 6d2f 7065  ://github.com/pe
+000013a0: 7465 7263 6f72 6b65 2f72 6f62 6f74 6963  tercorke/robotic
+000013b0: 732d 746f 6f6c 626f 782d 7079 7468 6f6e  s-toolbox-python
+000013c0: 2f72 6177 2f6d 6173 7465 722f 646f 6373  /raw/master/docs
+000013d0: 2f66 6967 732f 526f 6254 6f6f 6c42 6f78  /figs/RobToolBox
+000013e0: 5f52 6f75 6e64 4c6f 676f 422e 706e 6722  _RoundLogoB.png"
+000013f0: 2077 6964 7468 3d22 3230 3022 3e3c 2f74   width="200"></t
+00001400: 643e 0a3c 7464 2073 7479 6c65 3d22 626f  d>.<td style="bo
+00001410: 7264 6572 3a30 7078 223e 0a41 2050 7974  rder:0px">.A Pyt
+00001420: 686f 6e20 696d 706c 656d 656e 7461 7469  hon implementati
+00001430: 6f6e 206f 6620 7468 6520 3c61 2068 7265  on of the <a hre
+00001440: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
+00001450: 622e 636f 6d2f 7065 7465 7263 6f72 6b65  b.com/petercorke
+00001460: 2f72 6f62 6f74 6963 732d 746f 6f6c 626f  /robotics-toolbo
+00001470: 782d 6d61 746c 6162 223e 526f 626f 7469  x-matlab">Roboti
+00001480: 6373 2054 6f6f 6c62 6f78 2066 6f72 204d  cs Toolbox for M
+00001490: 4154 4c41 423c 7375 703e 2672 6567 3b3c  ATLAB<sup>&reg;<
+000014a0: 2f73 7570 3e3c 2f61 3e0a 3c75 6c3e 0a3c  /sup></a>.<ul>.<
+000014b0: 6c69 3e3c 6120 6872 6566 3d22 6874 7470  li><a href="http
+000014c0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
+000014d0: 6574 6572 636f 726b 652f 726f 626f 7469  etercorke/roboti
+000014e0: 6373 2d74 6f6f 6c62 6f78 2d70 7974 686f  cs-toolbox-pytho
+000014f0: 6e22 3e47 6974 4875 6220 7265 706f 7369  n">GitHub reposi
+00001500: 746f 7279 203c 2f61 3e3c 2f6c 693e 0a3c  tory </a></li>.<
+00001510: 6c69 3e3c 6120 6872 6566 3d22 6874 7470  li><a href="http
+00001520: 733a 2f2f 7065 7465 7263 6f72 6b65 2e67  s://petercorke.g
+00001530: 6974 6875 622e 696f 2f72 6f62 6f74 6963  ithub.io/robotic
+00001540: 732d 746f 6f6c 626f 782d 7079 7468 6f6e  s-toolbox-python
+00001550: 223e 446f 6375 6d65 6e74 6174 696f 6e3c  ">Documentation<
+00001560: 2f61 3e3c 2f6c 693e 0a3c 6c69 3e3c 6120  /a></li>.<li><a 
+00001570: 6872 6566 3d22 2336 223e 4943 5241 2050  href="#6">ICRA P
+00001580: 6170 6572 3c2f 613e 3c2f 6c69 3e0a 3c6c  aper</a></li>.<l
+00001590: 693e 3c61 2068 7265 663d 2268 7474 7073  i><a href="https
+000015a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7065  ://github.com/pe
+000015b0: 7465 7263 6f72 6b65 2f72 6f62 6f74 6963  tercorke/robotic
+000015c0: 732d 746f 6f6c 626f 782d 7079 7468 6f6e  s-toolbox-python
+000015d0: 2f77 696b 6922 3e57 696b 6920 2865 7861  /wiki">Wiki (exa
+000015e0: 6d70 6c65 7320 616e 6420 6465 7461 696c  mples and detail
+000015f0: 7329 3c2f 613e 3c2f 6c69 3e0a 3c2f 756c  s)</a></li>.</ul
+00001600: 3e0a 3c2f 7464 3e0a 3c2f 7472 3e0a 3c2f  >.</td>.</tr>.</
+00001610: 7461 626c 653e 0a0a 3c21 2d2d 203c 6272  table>..<!-- <br
+00001620: 3e20 2d2d 3e0a 0a23 2320 436f 6e74 656e  > -->..## Conten
+00001630: 7473 0a0a 2d20 5b53 796e 6f70 7369 735d  ts..- [Synopsis]
+00001640: 2823 3129 0a2d 205b 4765 7474 696e 6720  (#1).- [Getting 
+00001650: 676f 696e 675d 2823 3229 0a2d 205b 5475  going](#2).- [Tu
+00001660: 746f 7269 616c 735d 2823 3329 0a2d 205b  torials](#3).- [
+00001670: 436f 6465 2045 7861 6d70 6c65 735d 2823  Code Examples](#
+00001680: 3429 0a2d 205b 546f 6f6c 626f 7820 5265  4).- [Toolbox Re
+00001690: 7365 6172 6368 2041 7070 6c69 6361 7469  search Applicati
+000016a0: 6f6e 735d 2823 3529 0a2d 205b 546f 6f6c  ons](#5).- [Tool
+000016b0: 626f 7820 4943 5241 2050 6170 6572 2061  box ICRA Paper a
+000016c0: 6e64 2043 6974 6174 696f 6e20 496e 666f  nd Citation Info
+000016d0: 5d28 2336 290a 2d20 5b55 7369 6e67 2074  ](#6).- [Using t
+000016e0: 6865 2054 6f6f 6c62 6f78 2069 6e20 796f  he Toolbox in yo
+000016f0: 7572 204f 7065 6e20 536f 7572 6365 2043  ur Open Source C
+00001700: 6f64 653f 5d28 2337 290a 2d20 5b43 6f6d  ode?](#7).- [Com
+00001710: 6d6f 6e20 4973 7375 6573 2061 6e64 2053  mon Issues and S
+00001720: 6f6c 7574 696f 6e73 5d28 2338 290a 0a3c  olutions](#8)..<
+00001730: 6272 3e0a 0a3c 6120 6964 3d27 3127 3e3c  br>..<a id='1'><
+00001740: 2f61 3e0a 0a23 2320 5379 6e6f 7073 6973  /a>..## Synopsis
+00001750: 0a0a 5468 6973 2074 6f6f 6c62 6f78 2062  ..This toolbox b
+00001760: 7269 6e67 7320 726f 626f 7469 6373 2d73  rings robotics-s
+00001770: 7065 6369 6669 6320 6675 6e63 7469 6f6e  pecific function
+00001780: 616c 6974 7920 746f 2050 7974 686f 6e2c  ality to Python,
+00001790: 2061 6e64 206c 6576 6572 6167 6573 0a50   and leverages.P
+000017a0: 7974 686f 6e27 7320 6164 7661 6e74 6167  ython's advantag
+000017b0: 6573 206f 6620 706f 7274 6162 696c 6974  es of portabilit
+000017c0: 792c 2075 6269 7175 6974 7920 616e 6420  y, ubiquity and 
+000017d0: 7375 7070 6f72 742c 2061 6e64 2074 6865  support, and the
+000017e0: 2063 6170 6162 696c 6974 7920 6f66 0a74   capability of.t
+000017f0: 6865 206f 7065 6e2d 736f 7572 6365 2065  he open-source e
+00001800: 636f 7379 7374 656d 2066 6f72 206c 696e  cosystem for lin
+00001810: 6561 7220 616c 6765 6272 6120 286e 756d  ear algebra (num
+00001820: 7079 2c20 7363 6970 7929 2c20 6772 6170  py, scipy), grap
+00001830: 6869 6373 0a28 6d61 7470 6c6f 746c 6962  hics.(matplotlib
+00001840: 2c20 7468 7265 652e 6a73 2c20 5765 6247  , three.js, WebG
+00001850: 4c29 2c20 696e 7465 7261 6374 6976 6520  L), interactive 
+00001860: 6465 7665 6c6f 706d 656e 7420 286a 7570  development (jup
+00001870: 7974 6572 2c20 6a75 7079 7465 726c 6162  yter, jupyterlab
+00001880: 2c0a 6d79 6269 6e64 6572 2e6f 7267 292c  ,.mybinder.org),
+00001890: 2061 6e64 2064 6f63 756d 656e 7461 7469   and documentati
+000018a0: 6f6e 2028 7370 6869 6e78 292e 0a0a 5468  on (sphinx)...Th
+000018b0: 6520 546f 6f6c 626f 7820 7072 6f76 6964  e Toolbox provid
+000018c0: 6573 2074 6f6f 6c73 2066 6f72 2072 6570  es tools for rep
+000018d0: 7265 7365 6e74 696e 6720 7468 6520 6b69  resenting the ki
+000018e0: 6e65 6d61 7469 6373 2061 6e64 2064 796e  nematics and dyn
+000018f0: 616d 6963 7320 6f66 0a73 6572 6961 6c2d  amics of.serial-
+00001900: 6c69 6e6b 206d 616e 6970 756c 6174 6f72  link manipulator
+00001910: 7320 2d20 796f 7520 6361 6e20 6561 7369  s - you can easi
+00001920: 6c79 2063 7265 6174 6520 796f 7572 206f  ly create your o
+00001930: 776e 2069 6e20 4465 6e61 7669 742d 4861  wn in Denavit-Ha
+00001940: 7274 656e 6265 7267 0a66 6f72 6d2c 2069  rtenberg.form, i
+00001950: 6d70 6f72 7420 6120 5552 4446 2066 696c  mport a URDF fil
+00001960: 652c 206f 7220 7573 6520 6f76 6572 2033  e, or use over 3
+00001970: 3020 7375 7070 6c69 6564 206d 6f64 656c  0 supplied model
+00001980: 7320 666f 7220 7765 6c6c 2d6b 6e6f 776e  s for well-known
+00001990: 0a63 6f6e 7465 6d70 6f72 6172 7920 726f  .contemporary ro
+000019a0: 626f 7473 2066 726f 6d20 4672 616e 6b61  bots from Franka
+000019b0: 2d45 6d69 6b61 2c20 4b69 6e6f 7661 2c20  -Emika, Kinova, 
+000019c0: 556e 6976 6572 7361 6c20 526f 626f 7469  Universal Roboti
+000019d0: 6373 2c20 5265 7468 696e 6b20 6173 0a77  cs, Rethink as.w
+000019e0: 656c 6c20 6173 2063 6c61 7373 6963 616c  ell as classical
+000019f0: 2072 6f62 6f74 7320 7375 6368 2061 7320   robots such as 
+00001a00: 7468 6520 5075 6d61 2035 3630 2061 6e64  the Puma 560 and
+00001a10: 2074 6865 2053 7461 6e66 6f72 6420 6172   the Stanford ar
+00001a20: 6d2e 0a0a 5468 6520 546f 6f6c 626f 7820  m...The Toolbox 
+00001a30: 636f 6e74 6169 6e73 2066 6173 7420 696d  contains fast im
+00001a40: 706c 656d 656e 7461 7469 6f6e 7320 6f66  plementations of
+00001a50: 206b 696e 656d 6174 6963 206f 7065 7261   kinematic opera
+00001a60: 7469 6f6e 732e 2054 6865 2066 6f72 7761  tions. The forwa
+00001a70: 7264 0a6b 696e 656d 6174 6963 7320 616e  rd.kinematics an
+00001a80: 6420 7468 6520 6d61 6e69 7075 6c61 746f  d the manipulato
+00001a90: 7220 4a61 636f 6269 616e 2063 616e 2062  r Jacobian can b
+00001aa0: 6520 636f 6d70 7574 6564 2069 6e20 6c65  e computed in le
+00001ab0: 7373 2074 6861 6e20 3120 6d69 6372 6f73  ss than 1 micros
+00001ac0: 6563 6f6e 640a 7768 696c 6520 6e75 6d65  econd.while nume
+00001ad0: 7269 6361 6c20 696e 7665 7273 6520 6b69  rical inverse ki
+00001ae0: 6e65 6d61 7469 6373 2063 616e 2062 6520  nematics can be 
+00001af0: 736f 6c76 6564 2069 6e20 6173 206c 6974  solved in as lit
+00001b00: 746c 6520 6173 2034 206d 6963 726f 7365  tle as 4 microse
+00001b10: 636f 6e64 732e 0a0a 5468 6520 746f 6f6c  conds...The tool
+00001b20: 626f 7820 616c 736f 2073 7570 706f 7274  box also support
+00001b30: 7320 6d6f 6269 6c65 2072 6f62 6f74 7320  s mobile robots 
+00001b40: 7769 7468 2066 756e 6374 696f 6e73 2066  with functions f
+00001b50: 6f72 2072 6f62 6f74 206d 6f74 696f 6e20  or robot motion 
+00001b60: 6d6f 6465 6c73 0a28 756e 6963 7963 6c65  models.(unicycle
+00001b70: 2c20 6269 6379 636c 6529 2c20 7061 7468  , bicycle), path
+00001b80: 2070 6c61 6e6e 696e 6720 616c 676f 7269   planning algori
+00001b90: 7468 6d73 2028 6275 672c 2064 6973 7461  thms (bug, dista
+00001ba0: 6e63 6520 7472 616e 7366 6f72 6d2c 2044  nce transform, D
+00001bb0: 5c2a 2c0a 5052 4d29 2c20 6b69 6e6f 6479  \*,.PRM), kinody
+00001bc0: 6e61 6d69 6320 706c 616e 6e69 6e67 2028  namic planning (
+00001bd0: 6c61 7474 6963 652c 2052 5254 292c 206c  lattice, RRT), l
+00001be0: 6f63 616c 697a 6174 696f 6e20 2845 4b46  ocalization (EKF
+00001bf0: 2c20 7061 7274 6963 6c65 2066 696c 7465  , particle filte
+00001c00: 7229 2c0a 6d61 7020 6275 696c 6469 6e67  r),.map building
+00001c10: 2028 454b 4629 2061 6e64 2073 696d 756c   (EKF) and simul
+00001c20: 7461 6e65 6f75 7320 6c6f 6361 6c69 7a61  taneous localiza
+00001c30: 7469 6f6e 2061 6e64 206d 6170 7069 6e67  tion and mapping
+00001c40: 2028 454b 4629 2e0a 0a54 6865 2054 6f6f   (EKF)...The Too
+00001c50: 6c62 6f78 2070 726f 7669 6465 733a 0a0a  lbox provides:..
+00001c60: 2d20 636f 6465 2074 6861 7420 6973 206d  - code that is m
+00001c70: 6174 7572 6520 616e 6420 7072 6f76 6964  ature and provid
+00001c80: 6573 2061 2070 6f69 6e74 206f 6620 636f  es a point of co
+00001c90: 6d70 6172 6973 6f6e 2066 6f72 206f 7468  mparison for oth
+00001ca0: 6572 0a20 2069 6d70 6c65 6d65 6e74 6174  er.  implementat
+00001cb0: 696f 6e73 206f 6620 7468 6520 7361 6d65  ions of the same
+00001cc0: 2061 6c67 6f72 6974 686d 733b 0a2d 2072   algorithms;.- r
+00001cd0: 6f75 7469 6e65 7320 7768 6963 6820 6172  outines which ar
+00001ce0: 6520 6765 6e65 7261 6c6c 7920 7772 6974  e generally writ
+00001cf0: 7465 6e20 696e 2061 2073 7472 6169 6768  ten in a straigh
+00001d00: 7466 6f72 7761 7264 206d 616e 6e65 7220  tforward manner 
+00001d10: 7768 6963 680a 2020 616c 6c6f 7773 2066  which.  allows f
+00001d20: 6f72 2065 6173 7920 756e 6465 7273 7461  or easy understa
+00001d30: 6e64 696e 672c 2070 6572 6861 7073 2061  nding, perhaps a
+00001d40: 7420 7468 6520 6578 7065 6e73 6520 6f66  t the expense of
+00001d50: 2063 6f6d 7075 7461 7469 6f6e 616c 0a20   computational. 
+00001d60: 2065 6666 6963 6965 6e63 793b 0a2d 2073   efficiency;.- s
+00001d70: 6f75 7263 6520 636f 6465 2077 6869 6368  ource code which
+00001d80: 2063 616e 2062 6520 7265 6164 2066 6f72   can be read for
+00001d90: 206c 6561 726e 696e 6720 616e 6420 7465   learning and te
+00001da0: 6163 6869 6e67 3b0a 2d20 6261 636b 7761  aching;.- backwa
+00001db0: 7264 2063 6f6d 7061 7461 6269 6c69 7479  rd compatability
+00001dc0: 2077 6974 6820 7468 6520 526f 626f 7469   with the Roboti
+00001dd0: 6373 2054 6f6f 6c62 6f78 2066 6f72 204d  cs Toolbox for M
+00001de0: 4154 4c41 420a 0a54 6865 2054 6f6f 6c62  ATLAB..The Toolb
+00001df0: 6f78 206c 6576 6572 6167 6573 2074 6865  ox leverages the
+00001e00: 205b 5370 6174 6961 6c20 4d61 7468 7320   [Spatial Maths 
+00001e10: 546f 6f6c 626f 7820 666f 7220 5079 7468  Toolbox for Pyth
+00001e20: 6f6e 5d28 6874 7470 733a 2f2f 6769 7468  on](https://gith
+00001e30: 7562 2e63 6f6d 2f70 6574 6572 636f 726b  ub.com/petercork
+00001e40: 652f 7370 6174 6961 6c6d 6174 682d 7079  e/spatialmath-py
+00001e50: 7468 6f6e 2920 746f 0a70 726f 7669 6465  thon) to.provide
+00001e60: 2073 7570 706f 7274 2066 6f72 2064 6174   support for dat
+00001e70: 6120 7479 7065 7320 7375 6368 2061 7320  a types such as 
+00001e80: 534f 286e 2920 616e 6420 5345 286e 2920  SO(n) and SE(n) 
+00001e90: 6d61 7472 6963 6573 2c20 7175 6174 6572  matrices, quater
+00001ea0: 6e69 6f6e 732c 2074 7769 7374 7320 616e  nions, twists an
+00001eb0: 6420 7370 6174 6961 6c20 7665 6374 6f72  d spatial vector
+00001ec0: 732e 0a0a 3c62 723e 0a0a 3c61 2069 643d  s...<br>..<a id=
+00001ed0: 2732 273e 3c2f 613e 0a0a 2323 2047 6574  '2'></a>..## Get
+00001ee0: 7469 6e67 2067 6f69 6e67 0a0a 596f 7520  ting going..You 
+00001ef0: 7769 6c6c 206e 6565 6420 5079 7468 6f6e  will need Python
+00001f00: 203e 3d20 332e 360a 0a23 2323 2055 7369   >= 3.6..### Usi
+00001f10: 6e67 2070 6970 0a0a 496e 7374 616c 6c20  ng pip..Install 
+00001f20: 6120 736e 6170 7368 6f74 2066 726f 6d20  a snapshot from 
+00001f30: 5079 5049 0a0a 6060 6073 6865 6c6c 2073  PyPI..```shell s
+00001f40: 6372 6970 740a 7069 7033 2069 6e73 7461  cript.pip3 insta
+00001f50: 6c6c 2072 6f62 6f74 6963 7374 6f6f 6c62  ll roboticstoolb
+00001f60: 6f78 2d70 7974 686f 6e0a 6060 600a 0a41  ox-python.```..A
+00001f70: 7661 696c 6162 6c65 206f 7074 696f 6e73  vailable options
+00001f80: 2061 7265 3a0a 0a2d 2060 636f 6c6c 6973   are:..- `collis
+00001f90: 696f 6e60 2069 6e73 7461 6c6c 2063 6f6c  ion` install col
+00001fa0: 6c69 7369 6f6e 2063 6865 636b 696e 6720  lision checking 
+00001fb0: 7769 7468 205b 7079 6275 6c6c 6574 5d28  with [pybullet](
+00001fc0: 6874 7470 733a 2f2f 7079 6275 6c6c 6574  https://pybullet
+00001fd0: 2e6f 7267 290a 0a50 7574 2074 6865 206f  .org)..Put the o
+00001fe0: 7074 696f 6e73 2069 6e20 6120 636f 6d6d  ptions in a comm
+00001ff0: 6120 7365 7061 7261 7465 6420 6c69 7374  a separated list
+00002000: 206c 696b 650a 0a60 6060 7368 656c 6c20   like..```shell 
+00002010: 7363 7269 7074 0a70 6970 3320 696e 7374  script.pip3 inst
+00002020: 616c 6c20 726f 626f 7469 6373 746f 6f6c  all roboticstool
+00002030: 626f 782d 7079 7468 6f6e 5b6f 7074 696f  box-python[optio
+00002040: 6e6c 6973 745d 0a60 6060 0a0a 5b53 7769  nlist].```..[Swi
+00002050: 6674 5d28 6874 7470 733a 2f2f 6769 7468  ft](https://gith
+00002060: 7562 2e63 6f6d 2f6a 6861 766c 2f73 7769  ub.com/jhavl/swi
+00002070: 6674 292c 2061 2077 6562 2d62 6173 6564  ft), a web-based
+00002080: 2076 6973 7561 6c69 7a65 722c 2069 730a   visualizer, is.
+00002090: 696e 7374 616c 6c65 6420 6173 2070 6172  installed as par
+000020a0: 7420 6f66 2052 6f62 6f74 6963 7320 546f  t of Robotics To
+000020b0: 6f6c 626f 782e 0a0a 2323 2320 4672 6f6d  olbox...### From
+000020c0: 2047 6974 4875 620a 0a54 6f20 696e 7374   GitHub..To inst
+000020d0: 616c 6c20 7468 6520 626c 6565 6469 6e67  all the bleeding
+000020e0: 2d65 6467 6520 7665 7273 696f 6e20 6672  -edge version fr
+000020f0: 6f6d 2047 6974 4875 620a 0a60 6060 7368  om GitHub..```sh
+00002100: 656c 6c20 7363 7269 7074 0a67 6974 2063  ell script.git c
+00002110: 6c6f 6e65 2068 7474 7073 3a2f 2f67 6974  lone https://git
+00002120: 6875 622e 636f 6d2f 7065 7465 7263 6f72  hub.com/petercor
+00002130: 6b65 2f72 6f62 6f74 6963 732d 746f 6f6c  ke/robotics-tool
+00002140: 626f 782d 7079 7468 6f6e 2e67 6974 0a63  box-python.git.c
+00002150: 6420 726f 626f 7469 6373 2d74 6f6f 6c62  d robotics-toolb
+00002160: 6f78 2d70 7974 686f 6e0a 7069 7033 2069  ox-python.pip3 i
+00002170: 6e73 7461 6c6c 202d 6520 2e0a 6060 600a  nstall -e ..```.
+00002180: 0a3c 6272 3e0a 0a3c 6120 6964 3d27 3327  .<br>..<a id='3'
+00002190: 3e3c 2f61 3e0a 0a23 2320 5475 746f 7269  ></a>..## Tutori
+000021a0: 616c 730a 0a3c 7461 626c 6520 7374 796c  als..<table styl
+000021b0: 653d 2262 6f72 6465 723a 3070 7822 3e0a  e="border:0px">.
+000021c0: 3c74 7220 7374 796c 653d 2262 6f72 6465  <tr style="borde
+000021d0: 723a 3070 7822 3e0a 3c74 6420 7374 796c  r:0px">.<td styl
+000021e0: 653d 2262 6f72 6465 723a 3070 7822 3e3c  e="border:0px"><
+000021f0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00002200: 6269 742e 6c79 2f33 616b 3547 4469 223e  bit.ly/3ak5GDi">
+00002210: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00002220: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 6861  //github.com/jha
+00002230: 766c 2f64 6b74 2f72 6177 2f6d 6169 6e2f  vl/dkt/raw/main/
+00002240: 696d 672f 6172 7469 636c 6531 2e70 6e67  img/article1.png
+00002250: 2220 7769 6474 683d 2234 3030 223e 3c2f  " width="400"></
+00002260: 613e 3c2f 7464 3e0a 3c74 6420 7374 796c  a></td>.<td styl
+00002270: 653d 2262 6f72 6465 723a 3070 7822 3e3c  e="border:0px"><
+00002280: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00002290: 6269 742e 6c79 2f33 616b 3547 4469 223e  bit.ly/3ak5GDi">
+000022a0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+000022b0: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 6861  //github.com/jha
+000022c0: 766c 2f64 6b74 2f72 6177 2f6d 6169 6e2f  vl/dkt/raw/main/
+000022d0: 696d 672f 6172 7469 636c 6532 2e70 6e67  img/article2.png
+000022e0: 2220 7769 6474 683d 2234 3030 223e 3c2f  " width="400"></
+000022f0: 613e 3c2f 7464 3e0a 3c74 6420 7374 796c  a></td>.<td styl
+00002300: 653d 2262 6f72 6465 723a 3070 7822 3e0a  e="border:0px">.
+00002310: 446f 2079 6f75 2077 616e 7420 746f 206c  Do you want to l
+00002320: 6561 726e 2061 626f 7574 206d 616e 6970  earn about manip
+00002330: 756c 6174 6f72 206b 696e 656d 6174 6963  ulator kinematic
+00002340: 732c 2064 6966 6665 7265 6e74 6961 6c20  s, differential 
+00002350: 6b69 6e65 6d61 7469 6373 2c20 696e 7665  kinematics, inve
+00002360: 7273 652d 6b69 6e65 6d61 7469 6373 2061  rse-kinematics a
+00002370: 6e64 206d 6f74 696f 6e20 636f 6e74 726f  nd motion contro
+00002380: 6c3f 2048 6176 6520 6120 6c6f 6f6b 2061  l? Have a look a
+00002390: 7420 6f75 720a 3c61 2068 7265 663d 2268  t our.<a href="h
+000023a0: 7474 7073 3a2f 2f62 6974 2e6c 792f 3361  ttps://bit.ly/3a
+000023b0: 6b35 4744 6922 3e74 7574 6f72 6961 6c3c  k5GDi">tutorial<
+000023c0: 2f61 3e2e 0a54 6869 7320 7475 746f 7269  /a>..This tutori
+000023d0: 616c 2063 6f6d 6573 2077 6974 6820 7477  al comes with tw
+000023e0: 6f20 6172 7469 636c 6573 2074 6f20 636f  o articles to co
+000023f0: 7665 7220 7468 6520 7468 656f 7279 2061  ver the theory a
+00002400: 6e64 2031 3220 4a75 7079 7465 7220 4e6f  nd 12 Jupyter No
+00002410: 7465 626f 6f6b 7320 7072 6f76 6964 696e  tebooks providin
+00002420: 6720 6675 6c6c 2063 6f64 6520 696d 706c  g full code impl
+00002430: 656d 656e 7461 7469 6f6e 7320 616e 6420  ementations and 
+00002440: 6578 616d 706c 6573 2e20 4d6f 7374 206f  examples. Most o
+00002450: 6620 7468 6520 4e6f 7465 626f 6f6b 7320  f the Notebooks 
+00002460: 6172 6520 616c 736f 2047 6f6f 676c 6520  are also Google 
+00002470: 436f 6c61 6220 636f 6d70 6174 6962 6c65  Colab compatible
+00002480: 2061 6c6c 6f77 696e 6720 7468 656d 2074   allowing them t
+00002490: 6f20 7275 6e20 6f6e 6c69 6e65 2e0a 3c2f  o run online..</
+000024a0: 7464 3e0a 3c2f 7472 3e0a 3c2f 7461 626c  td>.</tr>.</tabl
+000024b0: 653e 0a0a 3c62 723e 0a0a 3c61 2069 643d  e>..<br>..<a id=
+000024c0: 2734 273e 3c2f 613e 0a0a 2323 2043 6f64  '4'></a>..## Cod
+000024d0: 6520 4578 616d 706c 6573 0a0a 5765 2077  e Examples..We w
+000024e0: 696c 6c20 6c6f 6164 2061 206d 6f64 656c  ill load a model
+000024f0: 206f 6620 7468 6520 4672 616e 6b61 2d45   of the Franka-E
+00002500: 6d69 6b61 2050 616e 6461 2072 6f62 6f74  mika Panda robot
+00002510: 2064 6566 696e 6564 2062 7920 6120 5552   defined by a UR
+00002520: 4446 2066 696c 650a 0a60 6060 7079 7468  DF file..```pyth
+00002530: 6f6e 0a69 6d70 6f72 7420 726f 626f 7469  on.import roboti
+00002540: 6373 746f 6f6c 626f 7820 6173 2072 7462  cstoolbox as rtb
+00002550: 0a72 6f62 6f74 203d 2072 7462 2e6d 6f64  .robot = rtb.mod
+00002560: 656c 732e 5061 6e64 6128 290a 7072 696e  els.Panda().prin
+00002570: 7428 726f 626f 7429 0a0a 0945 526f 626f  t(robot)...ERobo
+00002580: 743a 2070 616e 6461 2028 6279 2046 7261  t: panda (by Fra
+00002590: 6e6b 6120 456d 696b 6129 2c20 3720 6a6f  nka Emika), 7 jo
+000025a0: 696e 7473 2028 5252 5252 5252 5229 2c20  ints (RRRRRRR), 
+000025b0: 3120 6772 6970 7065 722c 2067 656f 6d65  1 gripper, geome
+000025c0: 7472 792c 2063 6f6c 6c69 7369 6f6e 0a09  try, collision..
+000025d0: e294 8ce2 9480 e294 80e2 9480 e294 80e2  ................
+000025e0: 9480 e294 ace2 9480 e294 80e2 9480 e294  ................
+000025f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002600: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002610: 94ac e294 80e2 9480 e294 80e2 9480 e294  ................
+00002620: 80e2 9480 e294 80e2 94ac e294 80e2 9480  ................
+00002630: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002640: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002650: 80e2 94ac e294 80e2 9480 e294 80e2 9480  ................
+00002660: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002670: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002680: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002690: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000026a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000026b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000026c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000026d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000026e0: 80e2 9480 e294 900a 09e2 9482 6c69 6e6b  ............link
+000026f0: 20e2 9482 2020 2020 206c 696e 6b20 2020   ...     link   
+00002700: 2020 e294 8220 6a6f 696e 7420 e294 8220    ... joint ... 
+00002710: 2020 7061 7265 6e74 2020 2020 e294 8220    parent    ... 
+00002720: 2020 2020 2020 2020 2020 2020 2045 5453               ETS
+00002730: 3a20 7061 7265 6e74 2074 6f20 6c69 6e6b  : parent to link
+00002740: 2020 2020 2020 2020 2020 2020 2020 20e2                 .
+00002750: 9482 0a09 e294 9ce2 9480 e294 80e2 9480  ................
+00002760: e294 80e2 9480 e294 bce2 9480 e294 80e2  ................
+00002770: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002780: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002790: e294 80e2 94bc e294 80e2 9480 e294 80e2  ................
+000027a0: 9480 e294 80e2 9480 e294 80e2 94bc e294  ................
+000027b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000027c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000027d0: 9480 e294 80e2 94bc e294 80e2 9480 e294  ................
+000027e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000027f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002800: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002810: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002820: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002830: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002840: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002850: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002860: 9480 e294 80e2 9480 e294 a40a 09e2 9482  ................
+00002870: 2020 2030 20e2 9482 2070 616e 6461 5f6c     0 ... panda_l
+00002880: 696e 6b30 2020 e294 8220 2020 2020 2020  ink0  ...       
+00002890: e294 8220 4241 5345 2020 2020 2020 2020  ... BASE        
+000028a0: e294 8220 2020 2020 2020 2020 2020 2020  ...             
+000028b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028d0: 2020 20e2 9482 0a09 e294 8220 2020 3120     ........   1 
+000028e0: e294 8220 7061 6e64 615f 6c69 6e6b 3120  ... panda_link1 
+000028f0: 20e2 9482 2020 2020 2030 20e2 9482 2070   ...     0 ... p
+00002900: 616e 6461 5f6c 696e 6b30 20e2 9482 2053  anda_link0 ... S
+00002910: 4533 2830 2c20 302c 2030 2e33 3333 2920  E3(0, 0, 0.333) 
+00002920: e28a 9520 527a 2871 3029 2020 2020 2020  ... Rz(q0)      
+00002930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002940: e294 820a 09e2 9482 2020 2032 20e2 9482  ........   2 ...
+00002950: 2070 616e 6461 5f6c 696e 6b32 2020 e294   panda_link2  ..
+00002960: 8220 2020 2020 3120 e294 8220 7061 6e64  .     1 ... pand
+00002970: 615f 6c69 6e6b 3120 e294 8220 5345 3328  a_link1 ... SE3(
+00002980: 2d39 30c2 b02c 202d 30c2 b02c 2030 c2b0  -90.., -0.., 0..
+00002990: 2920 e28a 9520 527a 2871 3129 2020 2020  ) ... Rz(q1)    
+000029a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029b0: e294 820a 09e2 9482 2020 2033 20e2 9482  ........   3 ...
+000029c0: 2070 616e 6461 5f6c 696e 6b33 2020 e294   panda_link3  ..
+000029d0: 8220 2020 2020 3220 e294 8220 7061 6e64  .     2 ... pand
+000029e0: 615f 6c69 6e6b 3220 e294 8220 5345 3328  a_link2 ... SE3(
+000029f0: 302c 202d 302e 3331 362c 2030 3b20 3930  0, -0.316, 0; 90
+00002a00: c2b0 2c20 2d30 c2b0 2c20 30c2 b029 20e2  .., -0.., 0..) .
+00002a10: 8a95 2052 7a28 7132 2920 2020 2020 2020  .. Rz(q2)       
+00002a20: e294 820a 09e2 9482 2020 2034 20e2 9482  ........   4 ...
+00002a30: 2070 616e 6461 5f6c 696e 6b34 2020 e294   panda_link4  ..
+00002a40: 8220 2020 2020 3320 e294 8220 7061 6e64  .     3 ... pand
+00002a50: 615f 6c69 6e6b 3320 e294 8220 5345 3328  a_link3 ... SE3(
+00002a60: 302e 3038 3235 2c20 302c 2030 3b20 3930  0.0825, 0, 0; 90
+00002a70: c2b0 2c20 2d30 c2b0 2c20 30c2 b029 20e2  .., -0.., 0..) .
+00002a80: 8a95 2052 7a28 7133 2920 2020 2020 2020  .. Rz(q3)       
+00002a90: e294 820a 09e2 9482 2020 2035 20e2 9482  ........   5 ...
+00002aa0: 2070 616e 6461 5f6c 696e 6b35 2020 e294   panda_link5  ..
+00002ab0: 8220 2020 2020 3420 e294 8220 7061 6e64  .     4 ... pand
+00002ac0: 615f 6c69 6e6b 3420 e294 8220 5345 3328  a_link4 ... SE3(
+00002ad0: 2d30 2e30 3832 352c 2030 2e33 3834 2c20  -0.0825, 0.384, 
+00002ae0: 303b 202d 3930 c2b0 2c20 2d30 c2b0 2c20  0; -90.., -0.., 
+00002af0: 30c2 b029 20e2 8a95 2052 7a28 7134 2920  0..) ... Rz(q4) 
+00002b00: e294 820a 09e2 9482 2020 2036 20e2 9482  ........   6 ...
+00002b10: 2070 616e 6461 5f6c 696e 6b36 2020 e294   panda_link6  ..
+00002b20: 8220 2020 2020 3520 e294 8220 7061 6e64  .     5 ... pand
+00002b30: 615f 6c69 6e6b 3520 e294 8220 5345 3328  a_link5 ... SE3(
+00002b40: 3930 c2b0 2c20 2d30 c2b0 2c20 30c2 b029  90.., -0.., 0..)
+00002b50: 20e2 8a95 2052 7a28 7135 2920 2020 2020   ... Rz(q5)     
+00002b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b70: e294 820a 09e2 9482 2020 2037 20e2 9482  ........   7 ...
+00002b80: 2070 616e 6461 5f6c 696e 6b37 2020 e294   panda_link7  ..
+00002b90: 8220 2020 2020 3620 e294 8220 7061 6e64  .     6 ... pand
+00002ba0: 615f 6c69 6e6b 3620 e294 8220 5345 3328  a_link6 ... SE3(
+00002bb0: 302e 3038 382c 2030 2c20 303b 2039 30c2  0.088, 0, 0; 90.
+00002bc0: b02c 202d 30c2 b02c 2030 c2b0 2920 e28a  ., -0.., 0..) ..
+00002bd0: 9520 527a 2871 3629 2020 2020 2020 2020  . Rz(q6)        
+00002be0: e294 820a 09e2 9482 2020 2038 20e2 9482  ........   8 ...
+00002bf0: 2040 7061 6e64 615f 6c69 6e6b 3820 e294   @panda_link8 ..
+00002c00: 8220 2020 2020 2020 e294 8220 7061 6e64  .       ... pand
+00002c10: 615f 6c69 6e6b 3720 e294 8220 5345 3328  a_link7 ... SE3(
+00002c20: 302c 2030 2c20 302e 3130 3729 2020 2020  0, 0, 0.107)    
+00002c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c40: 2020 2020 2020 2020 2020 20e2 9482 0a09             .....
+00002c50: e294 94e2 9480 e294 80e2 9480 e294 80e2  ................
+00002c60: 9480 e294 b4e2 9480 e294 80e2 9480 e294  ................
+00002c70: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002c80: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002c90: 94b4 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002ca0: 80e2 9480 e294 80e2 94b4 e294 80e2 9480  ................
+00002cb0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002cc0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002cd0: 80e2 94b4 e294 80e2 9480 e294 80e2 9480  ................
+00002ce0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002cf0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002d00: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002d10: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002d20: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002d30: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002d40: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002d50: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002d60: 80e2 9480 e294 980a 0a09 e294 8ce2 9480  ................
+00002d70: e294 80e2 9480 e294 80e2 9480 e294 ace2  ................
+00002d80: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002d90: ace2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002da0: e294 80e2 9480 e294 80e2 94ac e294 80e2  ................
+00002db0: 9480 e294 80e2 9480 e294 80e2 94ac e294  ................
+00002dc0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002dd0: e294 80e2 94ac e294 80e2 9480 e294 80e2  ................
+00002de0: 9480 e294 80e2 94ac e294 80e2 9480 e294  ................
+00002df0: 80e2 9480 e294 80e2 9480 e294 80e2 94ac  ................
+00002e00: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002e10: 9480 e294 900a 09e2 9482 6e61 6d65 20e2  ..........name .
+00002e20: 9482 2071 3020 20e2 9482 2071 3120 2020  .. q0  ... q1   
+00002e30: 2020 e294 8220 7132 2020 e294 8220 7133    ... q2  ... q3
+00002e40: 2020 2020 e294 8220 7134 2020 e294 8220      ... q4  ... 
+00002e50: 7135 2020 2020 e294 8220 7136 2020 20e2  q5    ... q6   .
+00002e60: 9482 0a09 e294 9ce2 9480 e294 80e2 9480  ................
+00002e70: e294 80e2 9480 e294 bce2 9480 e294 80e2  ................
+00002e80: 9480 e294 80e2 9480 e294 bce2 9480 e294  ................
+00002e90: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002ea0: e294 80e2 94bc e294 80e2 9480 e294 80e2  ................
+00002eb0: 9480 e294 80e2 94bc e294 80e2 9480 e294  ................
+00002ec0: 80e2 9480 e294 80e2 9480 e294 80e2 94bc  ................
+00002ed0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002ee0: 94bc e294 80e2 9480 e294 80e2 9480 e294  ................
+00002ef0: 80e2 9480 e294 80e2 94bc e294 80e2 9480  ................
+00002f00: e294 80e2 9480 e294 80e2 9480 e294 a40a  ................
+00002f10: 09e2 9482 2020 7172 20e2 9482 2020 30c2  ....  qr ...  0.
+00002f20: b020 e294 8220 2d31 372e 32c2 b020 e294  . ... -17.2.. ..
+00002f30: 8220 2030 c2b0 20e2 9482 202d 3132 36c2  .  0.. ... -126.
+00002f40: b020 e294 8220 2030 c2b0 20e2 9482 2020  . ...  0.. ...  
+00002f50: 3131 35c2 b020 e294 8220 2034 35c2 b020  115.. ...  45.. 
+00002f60: e294 820a 09e2 9482 2020 717a 20e2 9482  ........  qz ...
+00002f70: 2020 30c2 b020 e294 8220 2030 c2b0 2020    0.. ...  0..  
+00002f80: 2020 e294 8220 2030 c2b0 20e2 9482 2020    ...  0.. ...  
+00002f90: 30c2 b020 2020 e294 8220 2030 c2b0 20e2  0..   ...  0.. .
+00002fa0: 9482 2020 30c2 b020 2020 e294 8220 2030  ..  0..   ...  0
+00002fb0: c2b0 2020 e294 820a 09e2 9494 e294 80e2  ..  ............
+00002fc0: 9480 e294 80e2 9480 e294 80e2 94b4 e294  ................
+00002fd0: 80e2 9480 e294 80e2 9480 e294 80e2 94b4  ................
+00002fe0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002ff0: 9480 e294 80e2 9480 e294 b4e2 9480 e294  ................
+00003000: 80e2 9480 e294 80e2 9480 e294 b4e2 9480  ................
+00003010: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003020: 9480 e294 b4e2 9480 e294 80e2 9480 e294  ................
+00003030: 80e2 9480 e294 b4e2 9480 e294 80e2 9480  ................
+00003040: e294 80e2 9480 e294 80e2 9480 e294 b4e2  ................
+00003050: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003060: 80e2 9498 0a60 6060 0a0a 5468 6520 7379  .....```..The sy
+00003070: 6d62 6f6c 2060 4060 2069 6e64 6963 6174  mbol `@` indicat
+00003080: 6573 2074 6865 206c 696e 6b20 6173 2061  es the link as a
+00003090: 6e20 656e 642d 6566 6665 6374 6f72 2c20  n end-effector, 
+000030a0: 6120 6c65 6166 206e 6f64 6520 696e 2074  a leaf node in t
+000030b0: 6865 2072 6967 6964 2d62 6f64 790a 7472  he rigid-body.tr
+000030c0: 6565 2028 5079 7468 6f6e 2070 726f 6d70  ee (Python promp
+000030d0: 7473 2061 7265 206e 6f74 2073 686f 776e  ts are not shown
+000030e0: 2074 6f20 6d61 6b65 2069 7420 6561 7379   to make it easy
+000030f0: 2074 6f20 636f 7079 2b70 6173 7465 2074   to copy+paste t
+00003100: 6865 2063 6f64 652c 2063 6f6e 736f 6c65  he code, console
+00003110: 206f 7574 7075 7420 6973 2069 6e64 656e   output is inden
+00003120: 7465 6429 2e0a 5765 2077 696c 6c20 636f  ted)..We will co
+00003130: 6d70 7574 6520 7468 6520 666f 7277 6172  mpute the forwar
+00003140: 6420 6b69 6e65 6d61 7469 6373 206e 6578  d kinematics nex
+00003150: 740a 0a60 6060 0a54 6520 3d20 726f 626f  t..```.Te = robo
+00003160: 742e 666b 696e 6528 726f 626f 742e 7172  t.fkine(robot.qr
+00003170: 2920 2023 2066 6f72 7761 7264 206b 696e  )  # forward kin
+00003180: 656d 6174 6963 730a 7072 696e 7428 5465  ematics.print(Te
+00003190: 290a 0a09 302e 3939 3520 2020 2020 3020  )...0.995     0 
+000031a0: 2020 2020 2020 2020 302e 3039 3938 3320          0.09983 
+000031b0: 2020 302e 3438 340a 0930 2020 2020 2020    0.484..0      
+000031c0: 2020 2d31 2020 2020 2020 2020 2030 2020    -1         0  
+000031d0: 2020 2020 2020 2030 0a09 302e 3039 3938         0..0.0998
+000031e0: 3320 2020 3020 2020 2020 2020 202d 302e  3   0        -0.
+000031f0: 3939 3520 2020 2020 302e 3431 3236 0a09  995     0.4126..
+00003200: 3020 2020 2020 2020 2020 3020 2020 2020  0         0     
+00003210: 2020 2020 3020 2020 2020 2020 2020 310a      0         1.
+00003220: 6060 600a 0a57 6520 6361 6e20 736f 6c76  ```..We can solv
+00003230: 6520 696e 7665 7273 6520 6b69 6e65 6d61  e inverse kinema
+00003240: 7469 6373 2076 6572 7920 6561 7369 6c79  tics very easily
+00003250: 2e20 5765 2066 6972 7374 2063 686f 6f73  . We first choos
+00003260: 6520 616e 2053 4528 3329 2070 6f73 650a  e an SE(3) pose.
+00003270: 6465 6669 6e65 6420 696e 2074 6572 6d73  defined in terms
+00003280: 206f 6620 706f 7369 7469 6f6e 2061 6e64   of position and
+00003290: 206f 7269 656e 7461 7469 6f6e 2028 656e   orientation (en
+000032a0: 642d 6566 6665 6374 6f72 207a 2d61 7869  d-effector z-axi
+000032b0: 7320 646f 776e 2028 413d 2d5a 2920 616e  s down (A=-Z) an
+000032c0: 6420 6669 6e67 6572 0a6f 7269 656e 7461  d finger.orienta
+000032d0: 7469 6f6e 2070 6172 616c 6c65 6c20 746f  tion parallel to
+000032e0: 2079 2d61 7869 7320 284f 3d2b 5929 292e   y-axis (O=+Y)).
+000032f0: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
+00003300: 2073 7061 7469 616c 6d61 7468 2069 6d70   spatialmath imp
+00003310: 6f72 7420 5345 330a 0a54 6570 203d 2053  ort SE3..Tep = S
+00003320: 4533 2e54 7261 6e73 2830 2e36 2c20 2d30  E3.Trans(0.6, -0
+00003330: 2e33 2c20 302e 3129 202a 2053 4533 2e4f  .3, 0.1) * SE3.O
+00003340: 4128 5b30 2c20 312c 2030 5d2c 205b 302c  A([0, 1, 0], [0,
+00003350: 2030 2c20 2d31 5d29 0a73 6f6c 203d 2072   0, -1]).sol = r
+00003360: 6f62 6f74 2e69 6b5f 4c4d 2854 6570 2920  obot.ik_LM(Tep) 
+00003370: 2020 2020 2020 2020 2320 736f 6c76 6520          # solve 
+00003380: 494b 0a70 7269 6e74 2873 6f6c 290a 0a09  IK.print(sol)...
+00003390: 2861 7272 6179 285b 2030 2e32 3035 3932  (array([ 0.20592
+000033a0: 3831 352c 2020 302e 3836 3630 3934 3831  815,  0.86609481
+000033b0: 2c20 2d30 2e37 3934 3733 3230 362c 202d  , -0.79473206, -
+000033c0: 312e 3638 3235 3437 3934 2c20 2030 2e37  1.68254794,  0.7
+000033d0: 3438 3732 3931 352c 0a09 0909 322e 3231  4872915,....2.21
+000033e0: 3736 3437 3436 2c20 2d30 2e31 3032 3535  764746, -0.10255
+000033f0: 3630 365d 292c 2031 2c20 3131 342c 2037  606]), 1, 114, 7
+00003400: 2c20 322e 3839 3031 3634 3035 3732 3330  , 2.890164057230
+00003410: 3232 3865 2d30 3729 0a0a 715f 7069 636b  228e-07)..q_pick
+00003420: 7570 203d 2073 6f6c 5b30 5d0a 7072 696e  up = sol[0].prin
+00003430: 7428 726f 626f 742e 666b 696e 6528 715f  t(robot.fkine(q_
+00003440: 7069 636b 7570 2929 2020 2020 2320 464b  pickup))    # FK
+00003450: 2073 686f 7773 2074 6861 7420 6465 7369   shows that desi
+00003460: 7265 6420 656e 642d 6566 6665 6374 6f72  red end-effector
+00003470: 2070 6f73 6520 7761 7320 6163 6869 6576   pose was achiev
+00003480: 6564 0a0a 0920 3120 2020 2020 2020 2020  ed... 1         
+00003490: 2d38 2e39 3133 652d 3035 2020 2d30 2e30  -8.913e-05  -0.0
+000034a0: 3030 3333 3334 2020 302e 3539 3936 0a09  003334  0.5996..
+000034b0: 2d38 2e39 3239 652d 3035 202d 3120 2020  -8.929e-05 -1   
+000034c0: 2020 2020 2020 202d 302e 3030 3034 3931         -0.000491
+000034d0: 3220 2d30 2e32 3939 380a 092d 302e 3030  2 -0.2998..-0.00
+000034e0: 3033 3333 3420 2030 2e30 3030 3439 3132  03334  0.0004912
+000034f0: 2020 2d31 2020 2020 2020 2020 2020 302e    -1          0.
+00003500: 3130 3031 0a09 2030 2020 2020 2020 2020  1001.. 0        
+00003510: 2020 3020 2020 2020 2020 2020 2020 3020    0           0 
+00003520: 2020 2020 2020 2020 2031 0a60 6060 0a0a           1.```..
+00003530: 5765 2063 616e 2061 6e69 6d61 7465 2061  We can animate a
+00003540: 2070 6174 6820 6672 6f6d 2074 6865 2072   path from the r
+00003550: 6561 6479 2070 6f73 6520 6071 7260 2063  eady pose `qr` c
+00003560: 6f6e 6669 6775 7261 7469 6f6e 2074 6f20  onfiguration to 
+00003570: 7468 6973 2070 6963 6b75 7020 636f 6e66  this pickup conf
+00003580: 6967 7572 6174 696f 6e0a 0a60 6060 7079  iguration..```py
+00003590: 7468 6f6e 0a71 7420 3d20 7274 622e 6a74  thon.qt = rtb.jt
+000035a0: 7261 6a28 726f 626f 742e 7172 2c20 715f  raj(robot.qr, q_
+000035b0: 7069 636b 7570 2c20 3530 290a 726f 626f  pickup, 50).robo
+000035c0: 742e 706c 6f74 2871 742e 712c 2062 6163  t.plot(qt.q, bac
+000035d0: 6b65 6e64 3d27 7079 706c 6f74 272c 206d  kend='pyplot', m
+000035e0: 6f76 6965 3d27 7061 6e64 6131 2e67 6966  ovie='panda1.gif
+000035f0: 2729 0a60 6060 0a0a 3c70 2061 6c69 676e  ').```..<p align
+00003600: 3d22 6365 6e74 6572 223e 0a09 3c69 6d67  ="center">..<img
+00003610: 2073 7263 3d22 2e2f 646f 6373 2f66 6967   src="./docs/fig
+00003620: 732f 7061 6e64 6131 2e67 6966 223e 0a3c  s/panda1.gif">.<
+00003630: 2f70 3e0a 0a77 6865 7265 2077 6520 6861  /p>..where we ha
+00003640: 7665 2073 7065 6369 6669 6564 2074 6865  ve specified the
+00003650: 206d 6174 706c 6f74 6c69 6220 6070 7970   matplotlib `pyp
+00003660: 6c6f 7460 2062 6163 6b65 6e64 2e20 426c  lot` backend. Bl
+00003670: 7565 2061 7272 6f77 7320 7368 6f77 2074  ue arrows show t
+00003680: 6865 206a 6f69 6e74 2061 7865 7320 616e  he joint axes an
+00003690: 6420 7468 6520 636f 6c6f 7572 6564 2066  d the coloured f
+000036a0: 7261 6d65 2073 686f 7773 2074 6865 2065  rame shows the e
+000036b0: 6e64 2d65 6666 6563 746f 7220 706f 7365  nd-effector pose
+000036c0: 2e0a 0a57 6520 6361 6e20 616c 736f 2070  ...We can also p
+000036d0: 6c6f 7420 7468 6520 7472 616a 6563 746f  lot the trajecto
+000036e0: 7279 2069 6e20 7468 6520 5377 6966 7420  ry in the Swift 
+000036f0: 7369 6d75 6c61 746f 7220 2861 2062 726f  simulator (a bro
+00003700: 7773 6572 2d62 6173 6564 2033 642d 7369  wser-based 3d-si
+00003710: 6d75 6c61 7469 6f6e 2065 6e76 6972 6f6e  mulation environ
+00003720: 6d65 6e74 2062 7569 6c74 2074 6f20 776f  ment built to wo
+00003730: 726b 2077 6974 6820 7468 6520 546f 6f6c  rk with the Tool
+00003740: 626f 7829 0a0a 6060 6070 7974 686f 6e0a  box)..```python.
+00003750: 726f 626f 742e 706c 6f74 2871 742e 7129  robot.plot(qt.q)
+00003760: 0a60 6060 0a0a 3c70 2061 6c69 676e 3d22  .```..<p align="
+00003770: 6365 6e74 6572 223e 0a09 3c69 6d67 2073  center">..<img s
+00003780: 7263 3d22 2e2f 646f 6373 2f66 6967 732f  rc="./docs/figs/
+00003790: 7061 6e64 6132 2e67 6966 223e 0a3c 2f70  panda2.gif">.</p
+000037a0: 3e0a 0a57 6520 6361 6e20 616c 736f 2065  >..We can also e
+000037b0: 7870 6572 696d 656e 7420 7769 7468 2076  xperiment with v
+000037c0: 656c 6f63 6974 7920 636f 6e74 726f 6c6c  elocity controll
+000037d0: 6572 7320 696e 2053 7769 6674 2e20 4865  ers in Swift. He
+000037e0: 7265 2069 7320 6120 7265 736f 6c76 6564  re is a resolved
+000037f0: 2d72 6174 6520 6d6f 7469 6f6e 2063 6f6e  -rate motion con
+00003800: 7472 6f6c 2065 7861 6d70 6c65 0a0a 6060  trol example..``
+00003810: 6070 7974 686f 6e0a 696d 706f 7274 2073  `python.import s
+00003820: 7769 6674 0a69 6d70 6f72 7420 726f 626f  wift.import robo
+00003830: 7469 6373 746f 6f6c 626f 7820 6173 2072  ticstoolbox as r
+00003840: 7462 0a69 6d70 6f72 7420 7370 6174 6961  tb.import spatia
+00003850: 6c6d 6174 6820 6173 2073 6d0a 696d 706f  lmath as sm.impo
+00003860: 7274 206e 756d 7079 2061 7320 6e70 0a0a  rt numpy as np..
+00003870: 656e 7620 3d20 7377 6966 742e 5377 6966  env = swift.Swif
+00003880: 7428 290a 656e 762e 6c61 756e 6368 2872  t().env.launch(r
+00003890: 6561 6c74 696d 653d 5472 7565 290a 0a70  ealtime=True)..p
+000038a0: 616e 6461 203d 2072 7462 2e6d 6f64 656c  anda = rtb.model
+000038b0: 732e 5061 6e64 6128 290a 7061 6e64 612e  s.Panda().panda.
+000038c0: 7120 3d20 7061 6e64 612e 7172 0a0a 5465  q = panda.qr..Te
+000038d0: 7020 3d20 7061 6e64 612e 666b 696e 6528  p = panda.fkine(
+000038e0: 7061 6e64 612e 7129 202a 2073 6d2e 5345  panda.q) * sm.SE
+000038f0: 332e 5472 616e 7328 302e 322c 2030 2e32  3.Trans(0.2, 0.2
+00003900: 2c20 302e 3435 290a 0a61 7272 6976 6564  , 0.45)..arrived
+00003910: 203d 2046 616c 7365 0a65 6e76 2e61 6464   = False.env.add
+00003920: 2870 616e 6461 290a 0a64 7420 3d20 302e  (panda)..dt = 0.
+00003930: 3035 0a0a 7768 696c 6520 6e6f 7420 6172  05..while not ar
+00003940: 7269 7665 643a 0a0a 2020 2020 762c 2061  rived:..    v, a
+00003950: 7272 6976 6564 203d 2072 7462 2e70 5f73  rrived = rtb.p_s
+00003960: 6572 766f 2870 616e 6461 2e66 6b69 6e65  ervo(panda.fkine
+00003970: 2870 616e 6461 2e71 292c 2054 6570 2c20  (panda.q), Tep, 
+00003980: 3129 0a20 2020 2070 616e 6461 2e71 6420  1).    panda.qd 
+00003990: 3d20 6e70 2e6c 696e 616c 672e 7069 6e76  = np.linalg.pinv
+000039a0: 2870 616e 6461 2e6a 6163 6f62 6528 7061  (panda.jacobe(pa
+000039b0: 6e64 612e 7129 2920 4020 760a 2020 2020  nda.q)) @ v.    
+000039c0: 656e 762e 7374 6570 2864 7429 0a0a 2320  env.step(dt)..# 
+000039d0: 556e 636f 6d6d 656e 7420 746f 2073 746f  Uncomment to sto
+000039e0: 7020 7468 6520 6272 6f77 7365 7220 7461  p the browser ta
+000039f0: 6220 6672 6f6d 2063 6c6f 7369 6e67 0a23  b from closing.#
+00003a00: 2065 6e76 2e68 6f6c 6428 290a 6060 600a   env.hold().```.
+00003a10: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+00003a20: 7222 3e0a 093c 696d 6720 7372 633d 222e  r">..<img src=".
+00003a30: 2f64 6f63 732f 6669 6773 2f70 616e 6461  /docs/figs/panda
+00003a40: 332e 6769 6622 3e0a 3c2f 703e 0a0a 2323  3.gif">.</p>..##
+00003a50: 2320 5275 6e20 736f 6d65 2065 7861 6d70  # Run some examp
+00003a60: 6c65 730a 0a54 6865 205b 606e 6f74 6562  les..The [`noteb
+00003a70: 6f6f 6b73 605d 2868 7474 7073 3a2f 2f67  ooks`](https://g
+00003a80: 6974 6875 622e 636f 6d2f 7065 7465 7263  ithub.com/peterc
+00003a90: 6f72 6b65 2f72 6f62 6f74 6963 732d 746f  orke/robotics-to
+00003aa0: 6f6c 626f 782d 7079 7468 6f6e 2f74 7265  olbox-python/tre
+00003ab0: 652f 6d61 7374 6572 2f6e 6f74 6562 6f6f  e/master/noteboo
+00003ac0: 6b73 2920 666f 6c64 6572 2063 6f6e 7461  ks) folder conta
+00003ad0: 696e 7320 736f 6d65 2074 7574 6f72 6961  ins some tutoria
+00003ae0: 6c20 4a75 7079 7465 7220 6e6f 7465 626f  l Jupyter notebo
+00003af0: 6f6b 7320 7768 6963 6820 796f 7520 6361  oks which you ca
+00003b00: 6e20 6272 6f77 7365 206f 6e20 4769 7448  n browse on GitH
+00003b10: 7562 2e20 4164 6469 7469 6f6e 616c 6c79  ub. Additionally
+00003b20: 2c20 6861 7665 2061 206c 6f6f 6b20 696e  , have a look in
+00003b30: 2074 6865 205b 6065 7861 6d70 6c65 7360   the [`examples`
+00003b40: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00003b50: 2e63 6f6d 2f70 6574 6572 636f 726b 652f  .com/petercorke/
+00003b60: 726f 626f 7469 6373 2d74 6f6f 6c62 6f78  robotics-toolbox
+00003b70: 2d70 7974 686f 6e2f 7472 6565 2f6d 6173  -python/tree/mas
+00003b80: 7465 722f 726f 626f 7469 6373 746f 6f6c  ter/roboticstool
+00003b90: 626f 782f 6578 616d 706c 6573 2920 666f  box/examples) fo
+00003ba0: 6c64 6572 2066 6f72 206d 616e 7920 7265  lder for many re
+00003bb0: 6164 7920 746f 2072 756e 2065 7861 6d70  ady to run examp
+00003bc0: 6c65 732e 0a0a 3c62 723e 0a0a 3c61 2069  les...<br>..<a i
+00003bd0: 643d 2735 273e 3c2f 613e 0a0a 2323 2054  d='5'></a>..## T
+00003be0: 6f6f 6c62 6f78 2052 6573 6561 7263 6820  oolbox Research 
+00003bf0: 4170 706c 6963 6174 696f 6e73 0a0a 5468  Applications..Th
+00003c00: 6520 746f 6f6c 626f 7820 6973 2069 6e63  e toolbox is inc
+00003c10: 7265 6469 626c 7920 7573 6566 756c 2066  redibly useful f
+00003c20: 6f72 2064 6576 656c 6f70 696e 6720 616e  or developing an
+00003c30: 6420 7072 6f74 6f74 7970 696e 6720 616c  d prototyping al
+00003c40: 676f 7269 7468 6d73 2066 6f72 2072 6573  gorithms for res
+00003c50: 6561 7263 682c 2074 6861 6e6b 7320 746f  earch, thanks to
+00003c60: 2074 6865 2065 7868 6175 7374 6976 6520   the exhaustive 
+00003c70: 7365 7420 6f66 2077 656c 6c20 646f 6375  set of well docu
+00003c80: 6d65 6e74 6564 2061 6e64 206d 6174 7572  mented and matur
+00003c90: 6520 726f 626f 7469 6320 6675 6e63 7469  e robotic functi
+00003ca0: 6f6e 7320 6578 706f 7365 6420 7468 726f  ons exposed thro
+00003cb0: 7567 6820 636c 6561 6e20 616e 6420 7061  ugh clean and pa
+00003cc0: 696e 6c65 7373 2041 5049 732e 2041 6464  inless APIs. Add
+00003cd0: 6974 696f 6e61 6c6c 792c 2074 6865 2065  itionally, the e
+00003ce0: 6173 6520 6174 2077 6869 6368 2061 2075  ase at which a u
+00003cf0: 7365 7220 6361 6e20 7669 7375 616c 697a  ser can visualiz
+00003d00: 6520 7468 6569 7220 616c 676f 7269 7468  e their algorith
+00003d10: 6d20 7375 7070 6f72 7473 2061 2072 6170  m supports a rap
+00003d20: 6964 2070 726f 746f 7479 7069 6e67 2070  id prototyping p
+00003d30: 6172 6164 6967 6d2e 0a0a 2323 2320 5075  aradigm...### Pu
+00003d40: 626c 6963 6174 696f 6e20 4c69 7374 0a0a  blication List..
+00003d50: 4a2e 2048 6176 696c 616e 642c 204e 2e20  J. Haviland, N. 
+00003d60: 53c3 bc6e 6465 7268 6175 6620 616e 6420  S..nderhauf and 
+00003d70: 502e 2043 6f72 6b65 2c20 222a 2a41 2048  P. Corke, "**A H
+00003d80: 6f6c 6973 7469 6320 4170 7072 6f61 6368  olistic Approach
+00003d90: 2074 6f20 5265 6163 7469 7665 204d 6f62   to Reactive Mob
+00003da0: 696c 6520 4d61 6e69 7075 6c61 7469 6f6e  ile Manipulation
+00003db0: 2a2a 2c22 2069 6e20 5f49 4545 4520 526f  **," in _IEEE Ro
+00003dc0: 626f 7469 6373 2061 6e64 2041 7574 6f6d  botics and Autom
+00003dd0: 6174 696f 6e20 4c65 7474 6572 735f 2c20  ation Letters_, 
+00003de0: 646f 693a 2031 302e 3131 3039 2f4c 5241  doi: 10.1109/LRA
+00003df0: 2e32 3032 322e 3331 3436 3535 342e 2049  .2022.3146554. I
+00003e00: 6e20 7468 6520 7669 6465 6f2c 2074 6865  n the video, the
+00003e10: 2072 6f62 6f74 2069 7320 636f 6e74 726f   robot is contro
+00003e20: 6c6c 6564 2075 7369 6e67 2074 6865 2052  lled using the R
+00003e30: 6f62 6f74 6963 7320 746f 6f6c 626f 7820  obotics toolbox 
+00003e40: 666f 7220 5079 7468 6f6e 2061 6e64 2066  for Python and f
+00003e50: 6561 7475 7265 7320 6120 7265 636f 7264  eatures a record
+00003e60: 696e 6720 6672 6f6d 2074 6865 205b 5377  ing from the [Sw
+00003e70: 6966 745d 2868 7474 7073 3a2f 2f67 6974  ift](https://git
+00003e80: 6875 622e 636f 6d2f 6a68 6176 6c2f 7377  hub.com/jhavl/sw
+00003e90: 6966 7429 2053 696d 756c 6174 6f72 2e0a  ift) Simulator..
+00003ea0: 0a5b 5b41 7278 6976 2050 6170 6572 5d28  .[[Arxiv Paper](
+00003eb0: 6874 7470 733a 2f2f 6172 7869 762e 6f72  https://arxiv.or
+00003ec0: 672f 6162 732f 3231 3039 2e30 3437 3439  g/abs/2109.04749
+00003ed0: 295d 205b 5b49 4545 4520 5870 6c6f 7265  )] [[IEEE Xplore
+00003ee0: 5d28 6874 7470 733a 2f2f 6965 6565 7870  ](https://ieeexp
+00003ef0: 6c6f 7265 2e69 6565 652e 6f72 672f 6162  lore.ieee.org/ab
+00003f00: 7374 7261 6374 2f64 6f63 756d 656e 742f  stract/document/
+00003f10: 3936 3935 3239 3829 5d20 5b5b 5072 6f6a  9695298)] [[Proj
+00003f20: 6563 7420 5765 6273 6974 655d 2868 7474  ect Website](htt
+00003f30: 7073 3a2f 2f6a 6861 766c 2e67 6974 6875  ps://jhavl.githu
+00003f40: 622e 696f 2f68 6f6c 6973 7469 632f 295d  b.io/holistic/)]
+00003f50: 205b 5b56 6964 656f 5d28 6874 7470 733a   [[Video](https:
+00003f60: 2f2f 796f 7574 752e 6265 2f2d 4458 4251  //youtu.be/-DXBQ
+00003f70: 5065 4c49 5634 295d 205b 5b43 6f64 6520  PeLIV4)] [[Code 
+00003f80: 4578 616d 706c 655d 2868 7474 7073 3a2f  Example](https:/
+00003f90: 2f67 6974 6875 622e 636f 6d2f 7065 7465  /github.com/pete
+00003fa0: 7263 6f72 6b65 2f72 6f62 6f74 6963 732d  rcorke/robotics-
+00003fb0: 746f 6f6c 626f 782d 7079 7468 6f6e 2f62  toolbox-python/b
+00003fc0: 6c6f 622f 6d61 7374 6572 2f72 6f62 6f74  lob/master/robot
+00003fd0: 6963 7374 6f6f 6c62 6f78 2f65 7861 6d70  icstoolbox/examp
+00003fe0: 6c65 732f 686f 6c69 7374 6963 5f6d 6d5f  les/holistic_mm_
+00003ff0: 6e6f 6e5f 686f 6c6f 6e6f 6d69 632e 7079  non_holonomic.py
+00004000: 295d 0a0a 3c70 3e0a 2020 3c61 2068 7265  )]..<p>.  <a hre
+00004010: 663d 2268 7474 7073 3a2f 2f79 6f75 7475  f="https://youtu
+00004020: 2e62 652f 2d44 5842 5150 654c 4956 3422  .be/-DXBQPeLIV4"
+00004030: 3e0a 2020 2020 3c69 6d67 2073 7263 3d22  >.    <img src="
+00004040: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00004050: 6f6d 2f70 6574 6572 636f 726b 652f 726f  om/petercorke/ro
+00004060: 626f 7469 6373 2d74 6f6f 6c62 6f78 2d70  botics-toolbox-p
+00004070: 7974 686f 6e2f 7261 772f 6d61 7374 6572  ython/raw/master
+00004080: 2f64 6f63 732f 6669 6773 2f68 6f6c 6973  /docs/figs/holis
+00004090: 7469 635f 796f 7574 7562 652e 706e 6722  tic_youtube.png"
+000040a0: 2077 6964 7468 3d22 3536 3022 3e0a 2020   width="560">.  
+000040b0: 3c2f 613e 0a3c 2f70 3e0a 0a4a 2e20 4861  </a>.</p>..J. Ha
+000040c0: 7669 6c61 6e64 2061 6e64 2050 2e20 436f  viland and P. Co
+000040d0: 726b 652c 2022 2a2a 4e45 4f3a 2041 204e  rke, "**NEO: A N
+000040e0: 6f76 656c 2045 7870 6564 6974 696f 7573  ovel Expeditious
+000040f0: 204f 7074 696d 6973 6174 696f 6e20 416c   Optimisation Al
+00004100: 676f 7269 7468 6d20 666f 7220 5265 6163  gorithm for Reac
+00004110: 7469 7665 204d 6f74 696f 6e20 436f 6e74  tive Motion Cont
+00004120: 726f 6c20 6f66 204d 616e 6970 756c 6174  rol of Manipulat
+00004130: 6f72 732a 2a2c 2220 696e 205f 4945 4545  ors**," in _IEEE
+00004140: 2052 6f62 6f74 6963 7320 616e 6420 4175   Robotics and Au
+00004150: 746f 6d61 7469 6f6e 204c 6574 7465 7273  tomation Letters
+00004160: 5f2c 2064 6f69 3a20 3130 2e31 3130 392f  _, doi: 10.1109/
+00004170: 4c52 412e 3230 3231 2e33 3035 3630 3630  LRA.2021.3056060
+00004180: 2e20 496e 2074 6865 2076 6964 656f 2c20  . In the video, 
+00004190: 7468 6520 726f 626f 7420 6973 2063 6f6e  the robot is con
+000041a0: 7472 6f6c 6c65 6420 7573 696e 6720 7468  trolled using th
+000041b0: 6520 526f 626f 7469 6373 2074 6f6f 6c62  e Robotics toolb
+000041c0: 6f78 2066 6f72 2050 7974 686f 6e20 616e  ox for Python an
+000041d0: 6420 6665 6174 7572 6573 2061 2072 6563  d features a rec
+000041e0: 6f72 6469 6e67 2066 726f 6d20 7468 6520  ording from the 
+000041f0: 5b53 7769 6674 5d28 6874 7470 733a 2f2f  [Swift](https://
+00004200: 6769 7468 7562 2e63 6f6d 2f6a 6861 766c  github.com/jhavl
+00004210: 2f73 7769 6674 2920 5369 6d75 6c61 746f  /swift) Simulato
+00004220: 722e 0a0a 5b5b 4172 7869 7620 5061 7065  r...[[Arxiv Pape
+00004230: 725d 2868 7474 7073 3a2f 2f61 7278 6976  r](https://arxiv
+00004240: 2e6f 7267 2f61 6273 2f32 3031 302e 3038  .org/abs/2010.08
+00004250: 3638 3629 5d20 5b5b 4945 4545 2058 706c  686)] [[IEEE Xpl
+00004260: 6f72 655d 2868 7474 7073 3a2f 2f69 6565  ore](https://iee
+00004270: 6578 706c 6f72 652e 6965 6565 2e6f 7267  explore.ieee.org
+00004280: 2f64 6f63 756d 656e 742f 3933 3433 3731  /document/934371
+00004290: 3829 5d20 5b5b 5072 6f6a 6563 7420 5765  8)] [[Project We
+000042a0: 6273 6974 655d 2868 7474 7073 3a2f 2f6a  bsite](https://j
+000042b0: 6861 766c 2e67 6974 6875 622e 696f 2f6e  havl.github.io/n
+000042c0: 656f 2f29 5d20 5b5b 5669 6465 6f5d 2868  eo/)] [[Video](h
+000042d0: 7474 7073 3a2f 2f79 6f75 7475 2e62 652f  ttps://youtu.be/
+000042e0: 6a53 4c50 4a42 7238 5154 5929 5d20 5b5b  jSLPJBr8QTY)] [[
+000042f0: 436f 6465 2045 7861 6d70 6c65 5d28 6874  Code Example](ht
+00004300: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00004310: 2f70 6574 6572 636f 726b 652f 726f 626f  /petercorke/robo
+00004320: 7469 6373 2d74 6f6f 6c62 6f78 2d70 7974  tics-toolbox-pyt
+00004330: 686f 6e2f 626c 6f62 2f6d 6173 7465 722f  hon/blob/master/
+00004340: 726f 626f 7469 6373 746f 6f6c 626f 782f  roboticstoolbox/
+00004350: 6578 616d 706c 6573 2f6e 656f 2e70 7929  examples/neo.py)
+00004360: 5d0a 0a3c 703e 0a20 203c 6120 6872 6566  ]..<p>.  <a href
+00004370: 3d22 6874 7470 733a 2f2f 796f 7574 752e  ="https://youtu.
+00004380: 6265 2f6a 534c 504a 4272 3851 5459 223e  be/jSLPJBr8QTY">
+00004390: 0a20 2020 203c 696d 6720 7372 633d 2268  .    <img src="h
+000043a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000043b0: 6d2f 7065 7465 7263 6f72 6b65 2f72 6f62  m/petercorke/rob
+000043c0: 6f74 6963 732d 746f 6f6c 626f 782d 7079  otics-toolbox-py
+000043d0: 7468 6f6e 2f72 6177 2f6d 6173 7465 722f  thon/raw/master/
+000043e0: 646f 6373 2f66 6967 732f 6e65 6f5f 796f  docs/figs/neo_yo
+000043f0: 7574 7562 652e 706e 6722 2077 6964 7468  utube.png" width
+00004400: 3d22 3536 3022 3e0a 2020 3c2f 613e 0a3c  ="560">.  </a>.<
+00004410: 2f70 3e0a 0a2a 2a41 2050 7572 656c 792d  /p>..**A Purely-
+00004420: 5265 6163 7469 7665 204d 616e 6970 756c  Reactive Manipul
+00004430: 6162 696c 6974 792d 4d61 7869 6d69 7369  ability-Maximisi
+00004440: 6e67 204d 6f74 696f 6e20 436f 6e74 726f  ng Motion Contro
+00004450: 6c6c 6572 2a2a 2c20 4a2e 2048 6176 696c  ller**, J. Havil
+00004460: 616e 6420 616e 6420 502e 2043 6f72 6b65  and and P. Corke
+00004470: 2e20 496e 2074 6865 2076 6964 656f 2c20  . In the video, 
+00004480: 7468 6520 726f 626f 7420 6973 2063 6f6e  the robot is con
+00004490: 7472 6f6c 6c65 6420 7573 696e 6720 7468  trolled using th
+000044a0: 6520 526f 626f 7469 6373 2074 6f6f 6c62  e Robotics toolb
+000044b0: 6f78 2066 6f72 2050 7974 686f 6e2e 0a0a  ox for Python...
+000044c0: 5b5b 5061 7065 725d 2868 7474 7073 3a2f  [[Paper](https:/
+000044d0: 2f61 7278 6976 2e6f 7267 2f61 6273 2f32  /arxiv.org/abs/2
+000044e0: 3030 322e 3131 3930 3129 5d20 5b5b 5072  002.11901)] [[Pr
+000044f0: 6f6a 6563 7420 5765 6273 6974 655d 2868  oject Website](h
+00004500: 7474 7073 3a2f 2f6a 6861 766c 2e67 6974  ttps://jhavl.git
+00004510: 6875 622e 696f 2f6d 6d63 2f29 5d20 5b5b  hub.io/mmc/)] [[
+00004520: 5669 6465 6f5d 2868 7474 7073 3a2f 2f79  Video](https://y
+00004530: 6f75 7475 2e62 652f 5675 5f72 6350 6c61  outu.be/Vu_rcPla
+00004540: 4144 4929 5d20 5b5b 436f 6465 2045 7861  ADI)] [[Code Exa
+00004550: 6d70 6c65 5d28 6874 7470 733a 2f2f 6769  mple](https://gi
+00004560: 7468 7562 2e63 6f6d 2f70 6574 6572 636f  thub.com/peterco
+00004570: 726b 652f 726f 626f 7469 6373 2d74 6f6f  rke/robotics-too
+00004580: 6c62 6f78 2d70 7974 686f 6e2f 626c 6f62  lbox-python/blob
+00004590: 2f6d 6173 7465 722f 726f 626f 7469 6373  /master/robotics
+000045a0: 746f 6f6c 626f 782f 6578 616d 706c 6573  toolbox/examples
+000045b0: 2f6d 6d63 2e70 7929 5d0a 0a3c 703e 0a20  /mmc.py)]..<p>. 
+000045c0: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+000045d0: 2f2f 796f 7574 752e 6265 2f56 755f 7263  //youtu.be/Vu_rc
+000045e0: 506c 6141 4449 223e 0a20 2020 203c 696d  PlaADI">.    <im
+000045f0: 6720 7372 633d 2268 7474 7073 3a2f 2f67  g src="https://g
+00004600: 6974 6875 622e 636f 6d2f 7065 7465 7263  ithub.com/peterc
+00004610: 6f72 6b65 2f72 6f62 6f74 6963 732d 746f  orke/robotics-to
+00004620: 6f6c 626f 782d 7079 7468 6f6e 2f72 6177  olbox-python/raw
+00004630: 2f6d 6173 7465 722f 646f 6373 2f66 6967  /master/docs/fig
+00004640: 732f 6d6d 635f 796f 7574 7562 652e 706e  s/mmc_youtube.pn
+00004650: 6722 2077 6964 7468 3d22 3536 3022 3e0a  g" width="560">.
+00004660: 2020 3c2f 613e 0a3c 2f70 3e0a 0a3c 6272    </a>.</p>..<br
+00004670: 3e0a 0a3c 6272 3e0a 0a3c 6120 6964 3d27  >..<br>..<a id='
+00004680: 3627 3e3c 2f61 3e0a 0a23 2320 546f 6f6c  6'></a>..## Tool
+00004690: 626f 7820 4943 5241 2050 6170 6572 2061  box ICRA Paper a
+000046a0: 6e64 2043 6974 6174 696f 6e20 496e 666f  nd Citation Info
+000046b0: 0a0a 4368 6563 6b20 6f75 7420 6f75 7220  ..Check out our 
+000046c0: 4943 5241 2032 3032 3120 7061 7065 7220  ICRA 2021 paper 
+000046d0: 6f6e 205b 4945 4545 2058 706c 6f72 655d  on [IEEE Xplore]
+000046e0: 2868 7474 7073 3a2f 2f69 6565 6578 706c  (https://ieeexpl
+000046f0: 6f72 652e 6965 6565 2e6f 7267 2f64 6f63  ore.ieee.org/doc
+00004700: 756d 656e 742f 3935 3631 3336 3629 206f  ument/9561366) o
+00004710: 7220 6765 7420 7468 6520 5044 4620 6672  r get the PDF fr
+00004720: 6f6d 205b 5065 7465 7227 7320 7765 6273  om [Peter's webs
+00004730: 6974 655d 2868 7474 7073 3a2f 2f62 6974  ite](https://bit
+00004740: 2e6c 792f 3343 6863 794e 7029 2e0a 0a49  .ly/3ChcyNp)...I
+00004750: 6620 7468 6520 746f 6f6c 626f 7820 6865  f the toolbox he
+00004760: 6c70 6564 2079 6f75 2069 6e20 796f 7572  lped you in your
+00004770: 2072 6573 6561 7263 682c 2070 6c65 6173   research, pleas
+00004780: 6520 6369 7465 0a0a 6060 600a 4069 6e70  e cite..```.@inp
+00004790: 726f 6365 6564 696e 6773 7b72 7462 2c0a  roceedings{rtb,.
+000047a0: 2020 7469 746c 653d 7b4e 6f74 2079 6f75    title={Not you
+000047b0: 7220 6772 616e 646d 6f74 6865 72e2 8099  r grandmother...
+000047c0: 7320 746f 6f6c 626f 782d 2d74 6865 2052  s toolbox--the R
+000047d0: 6f62 6f74 6963 7320 546f 6f6c 626f 7820  obotics Toolbox 
+000047e0: 7265 696e 7665 6e74 6564 2066 6f72 2050  reinvented for P
+000047f0: 7974 686f 6e7d 2c0a 2020 6175 7468 6f72  ython},.  author
+00004800: 3d7b 436f 726b 652c 2050 6574 6572 2061  ={Corke, Peter a
+00004810: 6e64 2048 6176 696c 616e 642c 204a 6573  nd Haviland, Jes
+00004820: 7365 7d2c 0a20 2062 6f6f 6b74 6974 6c65  se},.  booktitle
+00004830: 3d7b 3230 3231 2049 4545 4520 496e 7465  ={2021 IEEE Inte
+00004840: 726e 6174 696f 6e61 6c20 436f 6e66 6572  rnational Confer
+00004850: 656e 6365 206f 6e20 526f 626f 7469 6373  ence on Robotics
+00004860: 2061 6e64 2041 7574 6f6d 6174 696f 6e20   and Automation 
+00004870: 2849 4352 4129 7d2c 0a20 2070 6167 6573  (ICRA)},.  pages
+00004880: 3d7b 3131 3335 372d 2d31 3133 3633 7d2c  ={11357--11363},
+00004890: 0a20 2079 6561 723d 7b32 3032 317d 2c0a  .  year={2021},.
+000048a0: 2020 6f72 6761 6e69 7a61 7469 6f6e 3d7b    organization={
+000048b0: 4945 4545 7d0a 7d0a 6060 600a 0a3c 6272  IEEE}.}.```..<br
+000048c0: 3e0a 0a3c 6120 6964 3d27 3727 3e3c 2f61  >..<a id='7'></a
+000048d0: 3e0a 0a23 2320 5573 696e 6720 7468 6520  >..## Using the 
+000048e0: 546f 6f6c 626f 7820 696e 2079 6f75 7220  Toolbox in your 
+000048f0: 4f70 656e 2053 6f75 7263 6520 436f 6465  Open Source Code
+00004900: 3f0a 0a49 6620 796f 7520 6172 6520 7573  ?..If you are us
+00004910: 696e 6720 7468 6520 546f 6f6c 626f 7820  ing the Toolbox 
+00004920: 696e 2079 6f75 7220 6f70 656e 2073 6f75  in your open sou
+00004930: 7263 6520 636f 6465 2c20 6665 656c 2066  rce code, feel f
+00004940: 7265 6520 746f 2061 6464 206f 7572 2062  ree to add our b
+00004950: 6164 6765 2074 6f20 796f 7572 2072 6561  adge to your rea
+00004960: 646d 6521 0a0a 466f 7220 7468 6520 706f  dme!..For the po
+00004970: 7765 7265 6420 6279 2072 6f62 6f74 6963  wered by robotic
+00004980: 7320 746f 6f6c 626f 7820 6261 6467 650a  s toolbox badge.
+00004990: 0a5b 215b 506f 7765 7265 6420 6279 2074  .[![Powered by t
+000049a0: 6865 2052 6f62 6f74 6963 7320 546f 6f6c  he Robotics Tool
+000049b0: 626f 785d 2868 7474 7073 3a2f 2f72 6177  box](https://raw
+000049c0: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+000049d0: 6e74 2e63 6f6d 2f70 6574 6572 636f 726b  nt.com/petercork
+000049e0: 652f 726f 626f 7469 6373 2d74 6f6f 6c62  e/robotics-toolb
+000049f0: 6f78 2d70 7974 686f 6e2f 6d61 7374 6572  ox-python/master
+00004a00: 2f2e 6769 7468 7562 2f73 7667 2f72 7462  /.github/svg/rtb
+00004a10: 5f70 6f77 6572 6564 2e6d 696e 2e73 7667  _powered.min.svg
+00004a20: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
+00004a30: 622e 636f 6d2f 7065 7465 7263 6f72 6b65  b.com/petercorke
+00004a40: 2f72 6f62 6f74 6963 732d 746f 6f6c 626f  /robotics-toolbo
+00004a50: 782d 7079 7468 6f6e 290a 0a63 6f70 7920  x-python)..copy 
+00004a60: 7468 6520 666f 6c6c 6f77 696e 670a 0a60  the following..`
+00004a70: 6060 0a5b 215b 506f 7765 7265 6420 6279  ``.[![Powered by
+00004a80: 2074 6865 2052 6f62 6f74 6963 7320 546f   the Robotics To
+00004a90: 6f6c 626f 785d 2868 7474 7073 3a2f 2f72  olbox](https://r
+00004aa0: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
+00004ab0: 7465 6e74 2e63 6f6d 2f70 6574 6572 636f  tent.com/peterco
+00004ac0: 726b 652f 726f 626f 7469 6373 2d74 6f6f  rke/robotics-too
+00004ad0: 6c62 6f78 2d70 7974 686f 6e2f 6d61 7374  lbox-python/mast
+00004ae0: 6572 2f2e 6769 7468 7562 2f73 7667 2f72  er/.github/svg/r
+00004af0: 7462 5f70 6f77 6572 6564 2e6d 696e 2e73  tb_powered.min.s
+00004b00: 7667 295d 2868 7474 7073 3a2f 2f67 6974  vg)](https://git
+00004b10: 6875 622e 636f 6d2f 7065 7465 7263 6f72  hub.com/petercor
+00004b20: 6b65 2f72 6f62 6f74 6963 732d 746f 6f6c  ke/robotics-tool
+00004b30: 626f 782d 7079 7468 6f6e 290a 6060 600a  box-python).```.
+00004b40: 0a46 6f72 2074 6865 2070 6f77 6572 6564  .For the powered
+00004b50: 2062 7920 7079 7468 6f6e 2072 6f62 6f74   by python robot
+00004b60: 6963 7320 6261 6467 650a 0a5b 215b 506f  ics badge..[![Po
+00004b70: 7765 7265 6420 6279 2050 7974 686f 6e20  wered by Python 
+00004b80: 526f 626f 7469 6373 5d28 6874 7470 733a  Robotics](https:
+00004b90: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
+00004ba0: 636f 6e74 656e 742e 636f 6d2f 7065 7465  content.com/pete
+00004bb0: 7263 6f72 6b65 2f72 6f62 6f74 6963 732d  rcorke/robotics-
+00004bc0: 746f 6f6c 626f 782d 7079 7468 6f6e 2f6d  toolbox-python/m
+00004bd0: 6173 7465 722f 2e67 6974 6875 622f 7376  aster/.github/sv
+00004be0: 672f 7072 5f70 6f77 6572 6564 2e6d 696e  g/pr_powered.min
+00004bf0: 2e73 7667 295d 2868 7474 7073 3a2f 2f67  .svg)](https://g
+00004c00: 6974 6875 622e 636f 6d2f 7065 7465 7263  ithub.com/peterc
+00004c10: 6f72 6b65 2f72 6f62 6f74 6963 732d 746f  orke/robotics-to
+00004c20: 6f6c 626f 782d 7079 7468 6f6e 290a 0a63  olbox-python)..c
+00004c30: 6f70 7920 7468 6520 666f 6c6c 6f77 696e  opy the followin
+00004c40: 670a 0a60 6060 0a5b 215b 506f 7765 7265  g..```.[![Powere
+00004c50: 6420 6279 2050 7974 686f 6e20 526f 626f  d by Python Robo
+00004c60: 7469 6373 5d28 6874 7470 733a 2f2f 7261  tics](https://ra
+00004c70: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
+00004c80: 656e 742e 636f 6d2f 7065 7465 7263 6f72  ent.com/petercor
+00004c90: 6b65 2f72 6f62 6f74 6963 732d 746f 6f6c  ke/robotics-tool
+00004ca0: 626f 782d 7079 7468 6f6e 2f6d 6173 7465  box-python/maste
+00004cb0: 722f 2e67 6974 6875 622f 7376 672f 7072  r/.github/svg/pr
+00004cc0: 5f70 6f77 6572 6564 2e6d 696e 2e73 7667  _powered.min.svg
+00004cd0: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
+00004ce0: 622e 636f 6d2f 7065 7465 7263 6f72 6b65  b.com/petercorke
+00004cf0: 2f72 6f62 6f74 6963 732d 746f 6f6c 626f  /robotics-toolbo
+00004d00: 782d 7079 7468 6f6e 290a 6060 600a 0a3c  x-python).```..<
+00004d10: 6272 3e0a 0a3c 6120 6964 3d27 3827 3e3c  br>..<a id='8'><
+00004d20: 2f61 3e0a 0a23 2320 436f 6d6d 6f6e 2049  /a>..## Common I
+00004d30: 7373 7565 7320 616e 6420 536f 6c75 7469  ssues and Soluti
+00004d40: 6f6e 730a 0a53 6565 2074 6865 2063 6f6d  ons..See the com
+00004d50: 6d6f 6e20 6973 7375 6573 2077 6974 6820  mon issues with 
+00004d60: 6669 7865 7320 5b68 6572 655d 2868 7474  fixes [here](htt
+00004d70: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00004d80: 7065 7465 7263 6f72 6b65 2f72 6f62 6f74  petercorke/robot
+00004d90: 6963 732d 746f 6f6c 626f 782d 7079 7468  ics-toolbox-pyth
+00004da0: 6f6e 2f77 696b 692f 436f 6d6d 6f6e 2d49  on/wiki/Common-I
+00004db0: 7373 7565 7329 2e0a                      ssues)..
```

### Comparing `roboticstoolbox-python-1.1.0/pyproject.toml` & `roboticstoolbox_python-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 
 name = "roboticstoolbox-python"
 
 description = "A Python library for robotics education and research"
 
-version = "1.1.0"
+version = "1.1.1"
 
 authors = [
     { name = "Jesse Haviland", email = "j.haviland@qut.edu.au" },
     { name = "Peter Corke", email = "rvc@petercorke.com" },
 ]
 
 dependencies = [
@@ -86,15 +86,15 @@
 ]
 
 docs = [
     "sphinx",
     "sphinx_rtd_theme",
     "sphinx-autorun",
     "sphinx_autodoc_typehints",
-    "sphinx-favicon"
+    "sphinx-favicon",
 ]
 
 
 [project.scripts]
 
 eigdemo = "roboticstoolbox.examples.eigdemo:main"
 tripleangledemo = "roboticstoolbox.examples.tripleangledemo:main"
```

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/__init__.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/backends/Connector.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/backends/Connector.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/backends/PyPlot/EllipsePlot.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/backends/PyPlot/EllipsePlot.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/backends/PyPlot/PyPlot.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/backends/PyPlot/PyPlot.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/backends/PyPlot/PyPlot2.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/backends/PyPlot/PyPlot2.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/backends/PyPlot/RobotPlot.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/backends/PyPlot/RobotPlot.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/backends/PyPlot/RobotPlot2.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/backends/PyPlot/RobotPlot2.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/bin/rtbtool.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/bin/rtbtool.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/blocks/arm.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/blocks/arm.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/blocks/mobile.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/blocks/mobile.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/blocks/quad_model.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/blocks/quad_model.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/blocks/spatial.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/blocks/spatial.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/blocks/uav.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/blocks/uav.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/Cholesky` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/Cholesky`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/CholmodSupport` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/CholmodSupport`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/Core` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/Core`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/Eigenvalues` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/Eigenvalues`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/Geometry` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/Geometry`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/Householder` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/Householder`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/IterativeLinearSolvers` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/IterativeLinearSolvers`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/Jacobi` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/Jacobi`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/KLUSupport` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/KLUSupport`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/LU` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/LU`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/MetisSupport` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/MetisSupport`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/OrderingMethods` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/OrderingMethods`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/PaStiXSupport` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/PaStiXSupport`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/PardisoSupport` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/PardisoSupport`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/QR` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/QR`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/QtAlignedMalloc` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/QtAlignedMalloc`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/SPQRSupport` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/SPQRSupport`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/SVD` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/SVD`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/Sparse` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/Sparse`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/SparseCholesky` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/SparseCholesky`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/SparseCore` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/SparseCore`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/SparseLU` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/SparseLU`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/SparseQR` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/SparseQR`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/StdDeque` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/StdDeque`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/StdList` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/StdList`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/StdVector` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/StdVector`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/SuperLUSupport` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/SuperLUSupport`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/UmfPackSupport` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/UmfPackSupport`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Cholesky/LDLT.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Cholesky/LDLT.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Cholesky/LLT.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Cholesky/LLT.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Cholesky/LLT_LAPACKE.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Cholesky/LLT_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/CholmodSupport/CholmodSupport.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/CholmodSupport/CholmodSupport.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/ArithmeticSequence.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/ArithmeticSequence.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Array.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Array.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/ArrayBase.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/ArrayBase.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/ArrayWrapper.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/ArrayWrapper.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Assign.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Assign.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/AssignEvaluator.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/AssignEvaluator.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Assign_MKL.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Assign_MKL.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/BandMatrix.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/BandMatrix.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Block.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Block.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/BooleanRedux.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/BooleanRedux.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/CommaInitializer.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/CommaInitializer.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/ConditionEstimator.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/ConditionEstimator.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/CoreEvaluators.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/CoreEvaluators.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/CoreIterators.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/CoreIterators.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/CwiseBinaryOp.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/CwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/CwiseNullaryOp.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/CwiseNullaryOp.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/CwiseTernaryOp.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/CwiseTernaryOp.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/CwiseUnaryOp.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/CwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/CwiseUnaryView.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/CwiseUnaryView.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/DenseBase.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/DenseBase.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/DenseCoeffsBase.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/DenseCoeffsBase.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/DenseStorage.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/DenseStorage.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Diagonal.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Diagonal.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/DiagonalMatrix.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/DiagonalMatrix.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/DiagonalProduct.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/DiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Dot.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Dot.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/EigenBase.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/EigenBase.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/ForceAlignedAccess.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/ForceAlignedAccess.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Fuzzy.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Fuzzy.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/GeneralProduct.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/GeneralProduct.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/GenericPacketMath.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/GenericPacketMath.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/GlobalFunctions.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/GlobalFunctions.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/IO.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/IO.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/IndexedView.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/IndexedView.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Inverse.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Inverse.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Map.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Map.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/MapBase.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/MapBase.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/MathFunctions.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/MathFunctionsImpl.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/MathFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Matrix.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Matrix.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/MatrixBase.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/MatrixBase.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/NestByValue.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/NestByValue.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/NoAlias.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/NoAlias.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/NumTraits.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/NumTraits.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/PartialReduxEvaluator.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/PartialReduxEvaluator.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/PermutationMatrix.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/PermutationMatrix.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/PlainObjectBase.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/PlainObjectBase.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Product.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Product.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/ProductEvaluators.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/ProductEvaluators.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Random.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Random.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Redux.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Redux.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Ref.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Ref.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Replicate.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Replicate.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Reshaped.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Reshaped.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/ReturnByValue.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/ReturnByValue.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Reverse.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Reverse.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Select.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Select.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/SelfAdjointView.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/SelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/SelfCwiseBinaryOp.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/SelfCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Solve.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Solve.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/SolveTriangular.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/SolveTriangular.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/SolverBase.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/SolverBase.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/StableNorm.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/StableNorm.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/StlIterators.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/StlIterators.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Stride.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Stride.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Swap.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Swap.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Transpose.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Transpose.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Transpositions.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Transpositions.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/TriangularMatrix.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/TriangularMatrix.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/VectorBlock.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/VectorBlock.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/VectorwiseOp.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/VectorwiseOp.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/Visitor.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/Visitor.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/AVX/Complex.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/AVX/Complex.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/AVX/MathFunctions.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/AVX/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/AVX/PacketMath.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/AVX/PacketMath.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/AVX/TypeCasting.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/AVX/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/AVX512/Complex.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/AVX512/Complex.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/AVX512/MathFunctions.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/AVX512/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/AVX512/PacketMath.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/AVX512/PacketMath.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/AVX512/TypeCasting.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/AVX512/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/AltiVec/Complex.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/AltiVec/Complex.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/AltiVec/MathFunctions.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/AltiVec/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/AltiVec/MatrixProduct.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/AltiVec/MatrixProduct.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/AltiVec/PacketMath.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/AltiVec/PacketMath.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/CUDA/Complex.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/CUDA/Complex.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/Default/BFloat16.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/Default/BFloat16.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/Default/ConjHelper.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/Default/ConjHelper.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/Default/Half.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/Default/Half.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/Default/Settings.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/Default/Settings.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/Default/TypeCasting.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/Default/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/GPU/MathFunctions.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/GPU/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/GPU/PacketMath.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/GPU/PacketMath.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/GPU/TypeCasting.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/GPU/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/HIP/hcc/math_constants.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/HIP/hcc/math_constants.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/MSA/Complex.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/MSA/Complex.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/MSA/MathFunctions.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/MSA/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/MSA/PacketMath.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/MSA/PacketMath.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/NEON/Complex.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/NEON/Complex.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/NEON/MathFunctions.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/NEON/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/NEON/PacketMath.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/NEON/PacketMath.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/NEON/TypeCasting.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/NEON/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/SSE/Complex.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/SSE/Complex.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/SSE/MathFunctions.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/SSE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/SSE/PacketMath.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/SSE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/SSE/TypeCasting.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/SSE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/SVE/MathFunctions.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/SVE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/SVE/PacketMath.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/SVE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/SVE/TypeCasting.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/SVE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/SYCL/InteropHeaders.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/SYCL/InteropHeaders.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/SYCL/MathFunctions.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/SYCL/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/SYCL/PacketMath.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/SYCL/PacketMath.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/SYCL/TypeCasting.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/SYCL/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/ZVector/Complex.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/ZVector/Complex.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/ZVector/MathFunctions.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/ZVector/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/arch/ZVector/PacketMath.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/arch/ZVector/PacketMath.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/functors/AssignmentFunctors.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/functors/AssignmentFunctors.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/functors/BinaryFunctors.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/functors/BinaryFunctors.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/functors/NullaryFunctors.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/functors/NullaryFunctors.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/functors/StlFunctors.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/functors/StlFunctors.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/functors/TernaryFunctors.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/functors/TernaryFunctors.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/functors/UnaryFunctors.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/functors/UnaryFunctors.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/GeneralBlockPanelKernel.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/GeneralMatrixMatrix.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/GeneralMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/GeneralMatrixVector.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/GeneralMatrixVector.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/Parallelizer.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/Parallelizer.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/SelfadjointMatrixMatrix.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/SelfadjointMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/SelfadjointMatrixVector.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/SelfadjointMatrixVector.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/SelfadjointProduct.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/SelfadjointProduct.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/SelfadjointRank2Update.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/SelfadjointRank2Update.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/TriangularMatrixMatrix.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/TriangularMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/TriangularMatrixVector.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/TriangularMatrixVector.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/TriangularSolverMatrix.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/TriangularSolverMatrix.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/products/TriangularSolverVector.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/products/TriangularSolverVector.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/util/BlasUtil.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/util/BlasUtil.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/util/ConfigureVectorization.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/util/ConfigureVectorization.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/util/Constants.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/util/Constants.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/util/DisableStupidWarnings.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/util/DisableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/util/ForwardDeclarations.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/util/ForwardDeclarations.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/util/IndexedViewHelper.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/util/IndexedViewHelper.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/util/IntegralConstant.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/util/IntegralConstant.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/util/MKL_support.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/util/MKL_support.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/util/Macros.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/util/Macros.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/util/Memory.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/util/Memory.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/util/Meta.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/util/Meta.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/util/ReenableStupidWarnings.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/util/ReenableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/util/ReshapedHelper.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/util/ReshapedHelper.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/util/StaticAssert.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/util/StaticAssert.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/util/SymbolicIndex.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/util/SymbolicIndex.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Core/util/XprHelper.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Core/util/XprHelper.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Eigenvalues/ComplexEigenSolver.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Eigenvalues/ComplexEigenSolver.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Eigenvalues/ComplexSchur.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Eigenvalues/ComplexSchur.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Eigenvalues/EigenSolver.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Eigenvalues/EigenSolver.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Eigenvalues/HessenbergDecomposition.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Eigenvalues/HessenbergDecomposition.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Eigenvalues/RealQZ.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Eigenvalues/RealQZ.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Eigenvalues/RealSchur.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Eigenvalues/RealSchur.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Eigenvalues/Tridiagonalization.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Eigenvalues/Tridiagonalization.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Geometry/AlignedBox.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Geometry/AlignedBox.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Geometry/AngleAxis.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Geometry/AngleAxis.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Geometry/EulerAngles.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Geometry/EulerAngles.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Geometry/Homogeneous.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Geometry/Homogeneous.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Geometry/Hyperplane.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Geometry/Hyperplane.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Geometry/OrthoMethods.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Geometry/OrthoMethods.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Geometry/ParametrizedLine.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Geometry/ParametrizedLine.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Geometry/Quaternion.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Geometry/Quaternion.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Geometry/Rotation2D.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Geometry/Rotation2D.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Geometry/RotationBase.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Geometry/RotationBase.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Geometry/Scaling.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Geometry/Scaling.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Geometry/Transform.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Geometry/Transform.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Geometry/Translation.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Geometry/Translation.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Geometry/Umeyama.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Geometry/Umeyama.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Geometry/arch/Geometry_SIMD.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Geometry/arch/Geometry_SIMD.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Householder/BlockHouseholder.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Householder/BlockHouseholder.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Householder/Householder.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Householder/Householder.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Householder/HouseholderSequence.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Householder/HouseholderSequence.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/Jacobi/Jacobi.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/Jacobi/Jacobi.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/KLUSupport/KLUSupport.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/KLUSupport/KLUSupport.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/LU/Determinant.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/LU/Determinant.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/LU/FullPivLU.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/LU/FullPivLU.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/LU/InverseImpl.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/LU/InverseImpl.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/LU/PartialPivLU.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/LU/PartialPivLU.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/LU/PartialPivLU_LAPACKE.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/LU/PartialPivLU_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/LU/arch/InverseSize4.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/LU/arch/InverseSize4.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/MetisSupport/MetisSupport.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/MetisSupport/MetisSupport.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/OrderingMethods/Amd.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/OrderingMethods/Amd.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/OrderingMethods/Eigen_Colamd.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/OrderingMethods/Eigen_Colamd.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/OrderingMethods/Ordering.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/OrderingMethods/Ordering.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/PaStiXSupport/PaStiXSupport.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/PaStiXSupport/PaStiXSupport.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/PardisoSupport/PardisoSupport.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/PardisoSupport/PardisoSupport.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/QR/ColPivHouseholderQR.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/QR/ColPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/QR/CompleteOrthogonalDecomposition.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/QR/CompleteOrthogonalDecomposition.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/QR/FullPivHouseholderQR.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/QR/FullPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/QR/HouseholderQR.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/QR/HouseholderQR.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/QR/HouseholderQR_LAPACKE.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/QR/HouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SVD/BDCSVD.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SVD/BDCSVD.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SVD/JacobiSVD.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SVD/JacobiSVD.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SVD/JacobiSVD_LAPACKE.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SVD/JacobiSVD_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SVD/SVDBase.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SVD/SVDBase.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SVD/UpperBidiagonalization.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SVD/UpperBidiagonalization.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCholesky/SimplicialCholesky.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCholesky/SimplicialCholesky.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/AmbiVector.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/AmbiVector.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/CompressedStorage.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/CompressedStorage.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/MappedSparseMatrix.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/MappedSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseAssign.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseAssign.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseBlock.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseBlock.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseColEtree.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseColEtree.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseCompressedBase.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseCompressedBase.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseCwiseBinaryOp.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseCwiseUnaryOp.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseCwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseDenseProduct.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseDenseProduct.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseDiagonalProduct.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseDiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseDot.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseDot.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseFuzzy.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseFuzzy.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseMap.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseMap.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseMatrix.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseMatrix.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseMatrixBase.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseMatrixBase.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparsePermutation.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparsePermutation.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseProduct.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseProduct.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseRedux.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseRedux.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseRef.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseRef.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseSelfAdjointView.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseSelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseSolverBase.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseSolverBase.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseSparseProductWithPruning.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseSparseProductWithPruning.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseTranspose.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseTranspose.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseTriangularView.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseTriangularView.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseUtil.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseUtil.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseVector.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseVector.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/SparseView.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/SparseView.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseCore/TriangularSolver.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseCore/TriangularSolver.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseLU/SparseLUImpl.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseLU/SparseLUImpl.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_Memory.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_Memory.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_Structs.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_Structs.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_Utils.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_Utils.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_column_bmod.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_column_bmod.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_column_dfs.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_column_dfs.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_gemm_kernel.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_gemm_kernel.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_kernel_bmod.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_kernel_bmod.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_panel_bmod.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_panel_bmod.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_panel_dfs.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_panel_dfs.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_pivotL.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_pivotL.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_pruneL.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_pruneL.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_relax_snode.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseLU/SparseLU_relax_snode.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SparseQR/SparseQR.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SparseQR/SparseQR.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/StlSupport/StdDeque.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/StlSupport/StdDeque.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/StlSupport/StdList.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/StlSupport/StdList.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/StlSupport/StdVector.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/StlSupport/StdVector.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/StlSupport/details.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/StlSupport/details.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/SuperLUSupport/SuperLUSupport.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/SuperLUSupport/SuperLUSupport.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/UmfPackSupport/UmfPackSupport.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/UmfPackSupport/UmfPackSupport.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/misc/Image.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/misc/Image.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/misc/Kernel.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/misc/Kernel.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/misc/RealSvd2x2.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/misc/RealSvd2x2.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/misc/blas.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/misc/blas.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/misc/lapack.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/misc/lapack.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/misc/lapacke.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/misc/lapacke.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/plugins/ArrayCwiseBinaryOps.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/plugins/ArrayCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/plugins/ArrayCwiseUnaryOps.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/plugins/ArrayCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/plugins/BlockMethods.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/plugins/BlockMethods.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/plugins/CommonCwiseBinaryOps.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/plugins/CommonCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/plugins/CommonCwiseUnaryOps.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/plugins/CommonCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/plugins/IndexedViewMethods.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/plugins/IndexedViewMethods.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/plugins/MatrixCwiseBinaryOps.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/plugins/MatrixCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/plugins/MatrixCwiseUnaryOps.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/plugins/MatrixCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/Eigen/src/plugins/ReshapedMethods.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/Eigen/src/plugins/ReshapedMethods.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/fknm.cpp` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/fknm.cpp`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/fknm.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/fknm.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/frne.c` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/frne.c`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/frne.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/frne.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/ik.cpp` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/ik.cpp`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/ik.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/ik.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/linalg.cpp` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/linalg.cpp`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/linalg.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/linalg.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/methods.cpp` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/methods.cpp`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/methods.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/methods.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/ne.c` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/ne.c`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/structs.cpp` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/structs.cpp`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/structs.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/structs.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/vmath.c` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/vmath.c`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/core/vmath.h` & `roboticstoolbox_python-1.1.1/roboticstoolbox/core/vmath.h`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/examples/RRMC.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/examples/RRMC.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/examples/RRMC_swift.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/examples/RRMC_swift.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/examples/baur.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/examples/baur.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/examples/branched_robot.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/examples/branched_robot.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/examples/eigdemo.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/examples/eigdemo.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/examples/fetch_vision.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/examples/fetch_vision.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/examples/holistic_mm_non_holonomic.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/examples/holistic_mm_non_holonomic.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/examples/holistic_mm_omni.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/examples/holistic_mm_omni.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/examples/icra2021.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/examples/icra2021.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/examples/ik_exp.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/examples/ik_exp.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/examples/ik_speed.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/examples/ik_speed.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/examples/ikine_evaluate.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/examples/ikine_evaluate.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/examples/ikine_evaluate2.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/examples/ikine_evaluate2.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/examples/mexican-wave.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/examples/mexican-wave.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/examples/mmc.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/examples/mmc.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/examples/mobile.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/examples/mobile.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/examples/neo.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/examples/neo.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/examples/park.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/examples/park.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/examples/puma_jtraj.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/examples/puma_jtraj.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/examples/puma_swift.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/examples/puma_swift.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/examples/readme.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/examples/readme.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/examples/robots.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/examples/robots.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/examples/swift_recording.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/examples/swift_recording.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/examples/teach_swift.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/examples/teach_swift.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/examples/tripleangledemo.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/examples/tripleangledemo.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/examples/twistdemo.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/examples/twistdemo.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/examples/vehicle1.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/examples/vehicle1.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/Animations.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/Animations.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/Bug2.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/Bug2.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/CurvaturePolyPlanner.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/CurvaturePolyPlanner.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/DistanceTransformPlanner.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/DistanceTransformPlanner.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/DstarPlanner.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/DstarPlanner.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/DubinsPlanner.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/DubinsPlanner.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/EKF.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/EKF.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 Python EKF Planner
 @Author: Peter Corke, original MATLAB code and Python version
 @Author: Kristian Gibson, initial MATLAB port
 """
+
 from collections import namedtuple
 import numpy as np
 from math import pi
-from scipy import integrate, randn
+from scipy import integrate
 from scipy.linalg import sqrtm, block_diag
 from scipy.stats.distributions import chi2
 import matplotlib.pyplot as plt
 from matplotlib import animation
 
 from spatialmath.base.animate import Animate
 from spatialmath import base, SE2
```

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/LatticePlanner.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/LatticePlanner.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/OccGrid.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/OccGrid.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/PRMPlanner.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/PRMPlanner.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/ParticleFilter.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/ParticleFilter.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/PlannerBase.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/PlannerBase.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/PoseGraph.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/PoseGraph.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/QuinticPolyPlanner.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/QuinticPolyPlanner.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/RRTPlanner.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/RRTPlanner.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/ReedsSheppPlanner.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/ReedsSheppPlanner.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/Vehicle.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/Vehicle.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/__init__.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/__init__.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/drivers.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/drivers.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/landmarkmap.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/landmarkmap.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/mobile/sensors.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/mobile/sensors.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/AL5D.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/AL5D.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/Ball.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/Ball.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/Baxter.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/Baxter.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/Cobra600.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/Cobra600.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/Coil.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/Coil.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/Hyper.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/Hyper.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/Hyper3d.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/Hyper3d.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/IRB140.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/IRB140.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/Jaco.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/Jaco.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/KR5.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/KR5.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/LWR4.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/LWR4.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/Mico.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/Mico.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/Orion5.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/Orion5.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/P8.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/P8.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/Panda.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/Panda.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/Planar2.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/Planar2.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/Planar3.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/Planar3.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/Puma560.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/Puma560.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/Sawyer.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/Sawyer.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/Stanford.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/Stanford.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/TwoLink.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/TwoLink.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/UR10.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/UR10.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/UR3.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/UR3.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/UR5.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/UR5.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/Uprighttl.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/Uprighttl.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/DH/__init__.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/DH/__init__.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/ETS/Frankie.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/ETS/Frankie.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/ETS/GenericSeven.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/ETS/GenericSeven.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/ETS/Omni.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/ETS/Omni.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/ETS/Panda.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/ETS/Panda.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/ETS/Planar2.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/ETS/Planar2.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/ETS/Planar_Y.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/ETS/Planar_Y.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/ETS/Puma560.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/ETS/Puma560.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/ETS/XYPanda.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/ETS/XYPanda.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/ETS/__init__.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/ETS/__init__.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/AL5D.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/AL5D.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/Fetch.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/Fetch.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/FetchCamera.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/FetchCamera.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/Frankie.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/Frankie.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/FrankieOmni.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/FrankieOmni.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/KinovaGen3.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/KinovaGen3.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/LBR.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/LBR.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/Mico.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/Mico.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/PR2.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/PR2.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/Panda.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/Panda.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/Puma560.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/Puma560.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/UR10.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/UR10.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/UR3.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/UR3.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/UR5.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/UR5.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/Valkyrie.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/Valkyrie.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/YuMi.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/YuMi.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/__init__.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/__init__.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/px100.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/px100.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/px150.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/px150.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/rx150.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/rx150.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/rx200.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/rx200.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/vx300.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/vx300.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/vx300s.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/vx300s.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/wx200.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/wx200.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/wx250.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/wx250.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/URDF/wx250s.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/URDF/wx250s.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/models/list.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/models/list.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/robot/BaseRobot.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/robot/BaseRobot.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/robot/DHFactor.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/robot/DHFactor.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/robot/DHLink.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/robot/DHLink.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/robot/DHRobot.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/robot/DHRobot.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/robot/Dynamics.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/robot/Dynamics.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/robot/ELink.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/robot/ELink.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/robot/ERobot.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/robot/ERobot.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/robot/ET.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/robot/ET.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/robot/ETS.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/robot/ETS.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/robot/Gripper.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/robot/Gripper.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/robot/IK.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/robot/IK.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/robot/Link.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/robot/Link.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/robot/PoERobot.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/robot/PoERobot.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/robot/Robot.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/robot/Robot.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/robot/RobotKinematics.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/robot/RobotKinematics.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/robot/RobotProto.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/robot/RobotProto.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/robot/__init__.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/robot/__init__.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/tools/DHFactor.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/tools/DHFactor.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/tools/Ticker.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/tools/Ticker.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/tools/__init__.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/tools/data.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/tools/data.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/tools/jsingu.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/tools/jsingu.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/tools/null.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/tools/null.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/tools/numerical.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/tools/numerical.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/tools/p_servo.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/tools/p_servo.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/tools/plot.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/tools/plot.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/tools/trajectory.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/tools/trajectory.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/tools/urdf/__init__.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/tools/urdf/__init__.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/tools/urdf/urdf.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/tools/urdf/urdf.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/tools/urdf/utils.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/tools/urdf/utils.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/tools/xacro/__init__.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/tools/xacro/__init__.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/tools/xacro/cli.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/tools/xacro/cli.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/tools/xacro/color.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/tools/xacro/color.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox/tools/xacro/xmlutils.py` & `roboticstoolbox_python-1.1.1/roboticstoolbox/tools/xacro/xmlutils.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox_python.egg-info/PKG-INFO` & `roboticstoolbox_python-1.1.1/roboticstoolbox_python.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 726f 626f  : 2.1.Name: robo
 00000020: 7469 6373 746f 6f6c 626f 782d 7079 7468  ticstoolbox-pyth
 00000030: 6f6e 0a56 6572 7369 6f6e 3a20 312e 312e  on.Version: 1.1.
-00000040: 300a 5375 6d6d 6172 793a 2041 2050 7974  0.Summary: A Pyt
+00000040: 310a 5375 6d6d 6172 793a 2041 2050 7974  1.Summary: A Pyt
 00000050: 686f 6e20 6c69 6272 6172 7920 666f 7220  hon library for 
 00000060: 726f 626f 7469 6373 2065 6475 6361 7469  robotics educati
 00000070: 6f6e 2061 6e64 2072 6573 6561 7263 680a  on and research.
 00000080: 4175 7468 6f72 2d65 6d61 696c 3a20 4a65  Author-email: Je
 00000090: 7373 6520 4861 7669 6c61 6e64 203c 6a2e  sse Haviland <j.
 000000a0: 6861 7669 6c61 6e64 4071 7574 2e65 6475  haviland@qut.edu
 000000b0: 2e61 753e 2c20 5065 7465 7220 436f 726b  .au>, Peter Cork
@@ -139,1044 +139,1106 @@
 000008a0: 332e 3130 0a43 6c61 7373 6966 6965 723a  3.10.Classifier:
 000008b0: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
 000008c0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
 000008d0: 3a3a 2033 2e31 310a 5265 7175 6972 6573  :: 3.11.Requires
 000008e0: 2d50 7974 686f 6e3a 203e 3d33 2e37 0a44  -Python: >=3.7.D
 000008f0: 6573 6372 6970 7469 6f6e 2d43 6f6e 7465  escription-Conte
 00000900: 6e74 2d54 7970 653a 2074 6578 742f 6d61  nt-Type: text/ma
-00000910: 726b 646f 776e 0a50 726f 7669 6465 732d  rkdown.Provides-
-00000920: 4578 7472 613a 2063 6f6c 6c69 7369 6f6e  Extra: collision
-00000930: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-00000940: 2064 6576 0a50 726f 7669 6465 732d 4578   dev.Provides-Ex
-00000950: 7472 613a 2064 6f63 730a 4c69 6365 6e73  tra: docs.Licens
-00000960: 652d 4669 6c65 3a20 4c49 4345 4e53 450a  e-File: LICENSE.
-00000970: 0a23 2052 6f62 6f74 6963 7320 546f 6f6c  .# Robotics Tool
-00000980: 626f 7820 666f 7220 5079 7468 6f6e 0a0a  box for Python..
-00000990: 5b21 5b41 2050 7974 686f 6e20 526f 626f  [![A Python Robo
-000009a0: 7469 6373 2050 6163 6b61 6765 5d28 6874  tics Package](ht
-000009b0: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
-000009c0: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-000009d0: 7065 7465 7263 6f72 6b65 2f72 6f62 6f74  petercorke/robot
-000009e0: 6963 732d 746f 6f6c 626f 782d 7079 7468  ics-toolbox-pyth
-000009f0: 6f6e 2f6d 6173 7465 722f 2e67 6974 6875  on/master/.githu
-00000a00: 622f 7376 672f 7079 5f63 6f6c 6c65 6374  b/svg/py_collect
-00000a10: 696f 6e2e 6d69 6e2e 7376 6729 5d28 6874  ion.min.svg)](ht
-00000a20: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000a30: 2f70 6574 6572 636f 726b 652f 726f 626f  /petercorke/robo
-00000a40: 7469 6373 2d74 6f6f 6c62 6f78 2d70 7974  tics-toolbox-pyt
-00000a50: 686f 6e29 0a5b 215b 506f 7765 7265 6420  hon).[![Powered 
-00000a60: 6279 2053 7061 7469 616c 204d 6174 6873  by Spatial Maths
-00000a70: 5d28 6874 7470 733a 2f2f 7261 772e 6769  ](https://raw.gi
-00000a80: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
-00000a90: 636f 6d2f 7065 7465 7263 6f72 6b65 2f73  com/petercorke/s
-00000aa0: 7061 7469 616c 6d61 7468 2d70 7974 686f  patialmath-pytho
-00000ab0: 6e2f 6d61 7374 6572 2f2e 6769 7468 7562  n/master/.github
-00000ac0: 2f73 7667 2f73 6d5f 706f 7765 7265 642e  /svg/sm_powered.
-00000ad0: 6d69 6e2e 7376 6729 5d28 6874 7470 733a  min.svg)](https:
-00000ae0: 2f2f 6769 7468 7562 2e63 6f6d 2f70 6574  //github.com/pet
-00000af0: 6572 636f 726b 652f 7370 6174 6961 6c6d  ercorke/spatialm
-00000b00: 6174 682d 7079 7468 6f6e 290a 5b21 5b51  ath-python).[![Q
-00000b10: 5554 2043 656e 7472 6520 666f 7220 526f  UT Centre for Ro
-00000b20: 626f 7469 6373 204f 7065 6e20 536f 7572  botics Open Sour
-00000b30: 6365 5d28 6874 7470 733a 2f2f 6769 7468  ce](https://gith
-00000b40: 7562 2e63 6f6d 2f71 6372 2f71 6372 2e67  ub.com/qcr/qcr.g
-00000b50: 6974 6875 622e 696f 2f72 6177 2f6d 6173  ithub.io/raw/mas
-00000b60: 7465 722f 6d69 7363 2f62 6164 6765 2e73  ter/misc/badge.s
-00000b70: 7667 295d 2868 7474 7073 3a2f 2f71 6372  vg)](https://qcr
-00000b80: 2e67 6974 6875 622e 696f 290a 0a5b 215b  .github.io)..[![
-00000b90: 5079 5049 2076 6572 7369 6f6e 5d28 6874  PyPI version](ht
-00000ba0: 7470 733a 2f2f 6261 6467 652e 6675 7279  tps://badge.fury
-00000bb0: 2e69 6f2f 7079 2f72 6f62 6f74 6963 7374  .io/py/roboticst
-00000bc0: 6f6f 6c62 6f78 2d70 7974 686f 6e2e 7376  oolbox-python.sv
-00000bd0: 6729 5d28 6874 7470 733a 2f2f 6261 6467  g)](https://badg
-00000be0: 652e 6675 7279 2e69 6f2f 7079 2f72 6f62  e.fury.io/py/rob
-00000bf0: 6f74 6963 7374 6f6f 6c62 6f78 2d70 7974  oticstoolbox-pyt
-00000c00: 686f 6e29 0a5b 215b 416e 6163 6f6e 6461  hon).[![Anaconda
-00000c10: 2076 6572 7369 6f6e 5d28 6874 7470 733a   version](https:
-00000c20: 2f2f 616e 6163 6f6e 6461 2e6f 7267 2f63  //anaconda.org/c
-00000c30: 6f6e 6461 2d66 6f72 6765 2f72 6f62 6f74  onda-forge/robot
-00000c40: 6963 7374 6f6f 6c62 6f78 2d70 7974 686f  icstoolbox-pytho
-00000c50: 6e2f 6261 6467 6573 2f76 6572 7369 6f6e  n/badges/version
-00000c60: 2e73 7667 295d 2868 7474 7073 3a2f 2f61  .svg)](https://a
-00000c70: 6e61 636f 6e64 612e 6f72 672f 636f 6e64  naconda.org/cond
-00000c80: 612d 666f 7267 652f 726f 626f 7469 6373  a-forge/robotics
-00000c90: 746f 6f6c 626f 782d 7079 7468 6f6e 290a  toolbox-python).
-00000ca0: 215b 5079 5049 202d 2050 7974 686f 6e20  ![PyPI - Python 
-00000cb0: 5665 7273 696f 6e5d 2868 7474 7073 3a2f  Version](https:/
-00000cc0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000cd0: 7079 7069 2f70 7976 6572 7369 6f6e 732f  pypi/pyversions/
-00000ce0: 726f 626f 7469 6373 746f 6f6c 626f 782d  roboticstoolbox-
-00000cf0: 7079 7468 6f6e 2e73 7667 290a 0a5b 215b  python.svg)..[![
-00000d00: 4275 696c 6420 5374 6174 7573 5d28 6874  Build Status](ht
-00000d10: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000d20: 2f70 6574 6572 636f 726b 652f 726f 626f  /petercorke/robo
-00000d30: 7469 6373 2d74 6f6f 6c62 6f78 2d70 7974  tics-toolbox-pyt
-00000d40: 686f 6e2f 776f 726b 666c 6f77 732f 5465  hon/workflows/Te
-00000d50: 7374 2f62 6164 6765 2e73 7667 3f62 7261  st/badge.svg?bra
-00000d60: 6e63 683d 6d61 7374 6572 295d 2868 7474  nch=master)](htt
-00000d70: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000d80: 7065 7465 7263 6f72 6b65 2f72 6f62 6f74  petercorke/robot
-00000d90: 6963 732d 746f 6f6c 626f 782d 7079 7468  ics-toolbox-pyth
-00000da0: 6f6e 2f61 6374 696f 6e73 3f71 7565 7279  on/actions?query
-00000db0: 3d77 6f72 6b66 6c6f 7725 3341 5465 7374  =workflow%3ATest
-00000dc0: 290a 5b21 5b43 6f76 6572 6167 655d 2868  ).[![Coverage](h
-00000dd0: 7474 7073 3a2f 2f63 6f64 6563 6f76 2e69  ttps://codecov.i
-00000de0: 6f2f 6768 2f70 6574 6572 636f 726b 652f  o/gh/petercorke/
-00000df0: 726f 626f 7469 6373 2d74 6f6f 6c62 6f78  robotics-toolbox
-00000e00: 2d70 7974 686f 6e2f 6272 616e 6368 2f6d  -python/branch/m
-00000e10: 6173 7465 722f 6772 6170 682f 6261 6467  aster/graph/badg
-00000e20: 652e 7376 6729 5d28 6874 7470 733a 2f2f  e.svg)](https://
-00000e30: 636f 6465 636f 762e 696f 2f67 682f 7065  codecov.io/gh/pe
-00000e40: 7465 7263 6f72 6b65 2f72 6f62 6f74 6963  tercorke/robotic
-00000e50: 732d 746f 6f6c 626f 782d 7079 7468 6f6e  s-toolbox-python
-00000e60: 290a 5b21 5b50 7950 4920 2d20 446f 776e  ).[![PyPI - Down
-00000e70: 6c6f 6164 735d 2868 7474 7073 3a2f 2f69  loads](https://i
-00000e80: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
-00000e90: 7069 2f64 772f 726f 626f 7469 6373 746f  pi/dw/roboticsto
-00000ea0: 6f6c 626f 782d 7079 7468 6f6e 295d 2868  olbox-python)](h
-00000eb0: 7474 7073 3a2f 2f70 7970 6973 7461 7473  ttps://pypistats
-00000ec0: 2e6f 7267 2f70 6163 6b61 6765 732f 726f  .org/packages/ro
-00000ed0: 626f 7469 6373 746f 6f6c 626f 782d 7079  boticstoolbox-py
-00000ee0: 7468 6f6e 290a 5b21 5b4c 6963 656e 7365  thon).[![License
-00000ef0: 3a20 4d49 545d 2868 7474 7073 3a2f 2f69  : MIT](https://i
-00000f00: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
-00000f10: 6467 652f 4c69 6365 6e73 652d 4d49 542d  dge/License-MIT-
-00000f20: 7965 6c6c 6f77 2e73 7667 295d 2868 7474  yellow.svg)](htt
-00000f30: 7073 3a2f 2f6f 7065 6e73 6f75 7263 652e  ps://opensource.
-00000f40: 6f72 672f 6c69 6365 6e73 6573 2f4d 4954  org/licenses/MIT
-00000f50: 290a 0a3c 7461 626c 6520 7374 796c 653d  )..<table style=
-00000f60: 2262 6f72 6465 723a 3070 7822 3e0a 3c74  "border:0px">.<t
-00000f70: 7220 7374 796c 653d 2262 6f72 6465 723a  r style="border:
-00000f80: 3070 7822 3e0a 3c74 6420 7374 796c 653d  0px">.<td style=
-00000f90: 2262 6f72 6465 723a 3070 7822 3e0a 3c69  "border:0px">.<i
-00000fa0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00000fb0: 6769 7468 7562 2e63 6f6d 2f70 6574 6572  github.com/peter
-00000fc0: 636f 726b 652f 726f 626f 7469 6373 2d74  corke/robotics-t
-00000fd0: 6f6f 6c62 6f78 2d70 7974 686f 6e2f 7261  oolbox-python/ra
-00000fe0: 772f 6d61 7374 6572 2f64 6f63 732f 6669  w/master/docs/fi
-00000ff0: 6773 2f52 6f62 546f 6f6c 426f 785f 526f  gs/RobToolBox_Ro
-00001000: 756e 644c 6f67 6f42 2e70 6e67 2220 7769  undLogoB.png" wi
-00001010: 6474 683d 2232 3030 223e 3c2f 7464 3e0a  dth="200"></td>.
-00001020: 3c74 6420 7374 796c 653d 2262 6f72 6465  <td style="borde
-00001030: 723a 3070 7822 3e0a 4120 5079 7468 6f6e  r:0px">.A Python
-00001040: 2069 6d70 6c65 6d65 6e74 6174 696f 6e20   implementation 
-00001050: 6f66 2074 6865 203c 6120 6872 6566 3d22  of the <a href="
-00001060: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001070: 6f6d 2f70 6574 6572 636f 726b 652f 726f  om/petercorke/ro
-00001080: 626f 7469 6373 2d74 6f6f 6c62 6f78 2d6d  botics-toolbox-m
-00001090: 6174 6c61 6222 3e52 6f62 6f74 6963 7320  atlab">Robotics 
-000010a0: 546f 6f6c 626f 7820 666f 7220 4d41 544c  Toolbox for MATL
-000010b0: 4142 3c73 7570 3e26 7265 673b 3c2f 7375  AB<sup>&reg;</su
-000010c0: 703e 3c2f 613e 0a3c 756c 3e0a 3c6c 693e  p></a>.<ul>.<li>
-000010d0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-000010e0: 2f67 6974 6875 622e 636f 6d2f 7065 7465  /github.com/pete
-000010f0: 7263 6f72 6b65 2f72 6f62 6f74 6963 732d  rcorke/robotics-
-00001100: 746f 6f6c 626f 782d 7079 7468 6f6e 223e  toolbox-python">
-00001110: 4769 7448 7562 2072 6570 6f73 6974 6f72  GitHub repositor
-00001120: 7920 3c2f 613e 3c2f 6c69 3e0a 3c6c 693e  y </a></li>.<li>
-00001130: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00001140: 2f70 6574 6572 636f 726b 652e 6769 7468  /petercorke.gith
-00001150: 7562 2e69 6f2f 726f 626f 7469 6373 2d74  ub.io/robotics-t
-00001160: 6f6f 6c62 6f78 2d70 7974 686f 6e22 3e44  oolbox-python">D
-00001170: 6f63 756d 656e 7461 7469 6f6e 3c2f 613e  ocumentation</a>
-00001180: 3c2f 6c69 3e0a 3c6c 693e 3c61 2068 7265  </li>.<li><a hre
-00001190: 663d 2223 3622 3e49 4352 4120 5061 7065  f="#6">ICRA Pape
-000011a0: 723c 2f61 3e3c 2f6c 693e 0a3c 6c69 3e3c  r</a></li>.<li><
-000011b0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-000011c0: 6769 7468 7562 2e63 6f6d 2f70 6574 6572  github.com/peter
-000011d0: 636f 726b 652f 726f 626f 7469 6373 2d74  corke/robotics-t
-000011e0: 6f6f 6c62 6f78 2d70 7974 686f 6e2f 7769  oolbox-python/wi
-000011f0: 6b69 223e 5769 6b69 2028 6578 616d 706c  ki">Wiki (exampl
-00001200: 6573 2061 6e64 2064 6574 6169 6c73 293c  es and details)<
-00001210: 2f61 3e3c 2f6c 693e 0a3c 2f75 6c3e 0a3c  /a></li>.</ul>.<
-00001220: 2f74 643e 0a3c 2f74 723e 0a3c 2f74 6162  /td>.</tr>.</tab
-00001230: 6c65 3e0a 0a3c 212d 2d20 3c62 723e 202d  le>..<!-- <br> -
-00001240: 2d3e 0a0a 2323 2043 6f6e 7465 6e74 730a  ->..## Contents.
-00001250: 0a2d 205b 5379 6e6f 7073 6973 5d28 2331  .- [Synopsis](#1
-00001260: 290a 2d20 5b47 6574 7469 6e67 2067 6f69  ).- [Getting goi
-00001270: 6e67 5d28 2332 290a 2d20 5b54 7574 6f72  ng](#2).- [Tutor
-00001280: 6961 6c73 5d28 2333 290a 2d20 5b43 6f64  ials](#3).- [Cod
-00001290: 6520 4578 616d 706c 6573 5d28 2334 290a  e Examples](#4).
-000012a0: 2d20 5b54 6f6f 6c62 6f78 2052 6573 6561  - [Toolbox Resea
-000012b0: 7263 6820 4170 706c 6963 6174 696f 6e73  rch Applications
-000012c0: 5d28 2335 290a 2d20 5b54 6f6f 6c62 6f78  ](#5).- [Toolbox
-000012d0: 2049 4352 4120 5061 7065 7220 616e 6420   ICRA Paper and 
-000012e0: 4369 7461 7469 6f6e 2049 6e66 6f5d 2823  Citation Info](#
-000012f0: 3629 0a2d 205b 5573 696e 6720 7468 6520  6).- [Using the 
-00001300: 546f 6f6c 626f 7820 696e 2079 6f75 7220  Toolbox in your 
-00001310: 4f70 656e 2053 6f75 7263 6520 436f 6465  Open Source Code
-00001320: 3f5d 2823 3729 0a2d 205b 436f 6d6d 6f6e  ?](#7).- [Common
-00001330: 2049 7373 7565 7320 616e 6420 536f 6c75   Issues and Solu
-00001340: 7469 6f6e 735d 2823 3829 0a0a 3c62 723e  tions](#8)..<br>
-00001350: 0a0a 3c61 2069 643d 2731 273e 3c2f 613e  ..<a id='1'></a>
-00001360: 0a0a 2323 2053 796e 6f70 7369 730a 0a54  ..## Synopsis..T
-00001370: 6869 7320 746f 6f6c 626f 7820 6272 696e  his toolbox brin
-00001380: 6773 2072 6f62 6f74 6963 732d 7370 6563  gs robotics-spec
-00001390: 6966 6963 2066 756e 6374 696f 6e61 6c69  ific functionali
-000013a0: 7479 2074 6f20 5079 7468 6f6e 2c20 616e  ty to Python, an
-000013b0: 6420 6c65 7665 7261 6765 730a 5079 7468  d leverages.Pyth
-000013c0: 6f6e 2773 2061 6476 616e 7461 6765 7320  on's advantages 
-000013d0: 6f66 2070 6f72 7461 6269 6c69 7479 2c20  of portability, 
-000013e0: 7562 6971 7569 7479 2061 6e64 2073 7570  ubiquity and sup
-000013f0: 706f 7274 2c20 616e 6420 7468 6520 6361  port, and the ca
-00001400: 7061 6269 6c69 7479 206f 660a 7468 6520  pability of.the 
-00001410: 6f70 656e 2d73 6f75 7263 6520 6563 6f73  open-source ecos
-00001420: 7973 7465 6d20 666f 7220 6c69 6e65 6172  ystem for linear
-00001430: 2061 6c67 6562 7261 2028 6e75 6d70 792c   algebra (numpy,
-00001440: 2073 6369 7079 292c 2067 7261 7068 6963   scipy), graphic
-00001450: 730a 286d 6174 706c 6f74 6c69 622c 2074  s.(matplotlib, t
-00001460: 6872 6565 2e6a 732c 2057 6562 474c 292c  hree.js, WebGL),
-00001470: 2069 6e74 6572 6163 7469 7665 2064 6576   interactive dev
-00001480: 656c 6f70 6d65 6e74 2028 6a75 7079 7465  elopment (jupyte
-00001490: 722c 206a 7570 7974 6572 6c61 622c 0a6d  r, jupyterlab,.m
-000014a0: 7962 696e 6465 722e 6f72 6729 2c20 616e  ybinder.org), an
-000014b0: 6420 646f 6375 6d65 6e74 6174 696f 6e20  d documentation 
-000014c0: 2873 7068 696e 7829 2e0a 0a54 6865 2054  (sphinx)...The T
-000014d0: 6f6f 6c62 6f78 2070 726f 7669 6465 7320  oolbox provides 
-000014e0: 746f 6f6c 7320 666f 7220 7265 7072 6573  tools for repres
-000014f0: 656e 7469 6e67 2074 6865 206b 696e 656d  enting the kinem
-00001500: 6174 6963 7320 616e 6420 6479 6e61 6d69  atics and dynami
-00001510: 6373 206f 660a 7365 7269 616c 2d6c 696e  cs of.serial-lin
-00001520: 6b20 6d61 6e69 7075 6c61 746f 7273 202d  k manipulators -
-00001530: 2079 6f75 2063 616e 2065 6173 696c 7920   you can easily 
-00001540: 6372 6561 7465 2079 6f75 7220 6f77 6e20  create your own 
-00001550: 696e 2044 656e 6176 6974 2d48 6172 7465  in Denavit-Harte
-00001560: 6e62 6572 670a 666f 726d 2c20 696d 706f  nberg.form, impo
-00001570: 7274 2061 2055 5244 4620 6669 6c65 2c20  rt a URDF file, 
-00001580: 6f72 2075 7365 206f 7665 7220 3330 2073  or use over 30 s
-00001590: 7570 706c 6965 6420 6d6f 6465 6c73 2066  upplied models f
-000015a0: 6f72 2077 656c 6c2d 6b6e 6f77 6e0a 636f  or well-known.co
-000015b0: 6e74 656d 706f 7261 7279 2072 6f62 6f74  ntemporary robot
-000015c0: 7320 6672 6f6d 2046 7261 6e6b 612d 456d  s from Franka-Em
-000015d0: 696b 612c 204b 696e 6f76 612c 2055 6e69  ika, Kinova, Uni
-000015e0: 7665 7273 616c 2052 6f62 6f74 6963 732c  versal Robotics,
-000015f0: 2052 6574 6869 6e6b 2061 730a 7765 6c6c   Rethink as.well
-00001600: 2061 7320 636c 6173 7369 6361 6c20 726f   as classical ro
-00001610: 626f 7473 2073 7563 6820 6173 2074 6865  bots such as the
-00001620: 2050 756d 6120 3536 3020 616e 6420 7468   Puma 560 and th
-00001630: 6520 5374 616e 666f 7264 2061 726d 2e0a  e Stanford arm..
-00001640: 0a54 6865 2054 6f6f 6c62 6f78 2063 6f6e  .The Toolbox con
-00001650: 7461 696e 7320 6661 7374 2069 6d70 6c65  tains fast imple
-00001660: 6d65 6e74 6174 696f 6e73 206f 6620 6b69  mentations of ki
-00001670: 6e65 6d61 7469 6320 6f70 6572 6174 696f  nematic operatio
-00001680: 6e73 2e20 5468 6520 666f 7277 6172 640a  ns. The forward.
-00001690: 6b69 6e65 6d61 7469 6373 2061 6e64 2074  kinematics and t
-000016a0: 6865 206d 616e 6970 756c 6174 6f72 204a  he manipulator J
-000016b0: 6163 6f62 6961 6e20 6361 6e20 6265 2063  acobian can be c
-000016c0: 6f6d 7075 7465 6420 696e 206c 6573 7320  omputed in less 
-000016d0: 7468 616e 2031 206d 6963 726f 7365 636f  than 1 microseco
-000016e0: 6e64 0a77 6869 6c65 206e 756d 6572 6963  nd.while numeric
-000016f0: 616c 2069 6e76 6572 7365 206b 696e 656d  al inverse kinem
-00001700: 6174 6963 7320 6361 6e20 6265 2073 6f6c  atics can be sol
-00001710: 7665 6420 696e 2061 7320 6c69 7474 6c65  ved in as little
-00001720: 2061 7320 3420 6d69 6372 6f73 6563 6f6e   as 4 microsecon
-00001730: 6473 2e0a 0a54 6865 2074 6f6f 6c62 6f78  ds...The toolbox
-00001740: 2061 6c73 6f20 7375 7070 6f72 7473 206d   also supports m
-00001750: 6f62 696c 6520 726f 626f 7473 2077 6974  obile robots wit
-00001760: 6820 6675 6e63 7469 6f6e 7320 666f 7220  h functions for 
-00001770: 726f 626f 7420 6d6f 7469 6f6e 206d 6f64  robot motion mod
-00001780: 656c 730a 2875 6e69 6379 636c 652c 2062  els.(unicycle, b
-00001790: 6963 7963 6c65 292c 2070 6174 6820 706c  icycle), path pl
-000017a0: 616e 6e69 6e67 2061 6c67 6f72 6974 686d  anning algorithm
-000017b0: 7320 2862 7567 2c20 6469 7374 616e 6365  s (bug, distance
-000017c0: 2074 7261 6e73 666f 726d 2c20 445c 2a2c   transform, D\*,
-000017d0: 0a50 524d 292c 206b 696e 6f64 796e 616d  .PRM), kinodynam
-000017e0: 6963 2070 6c61 6e6e 696e 6720 286c 6174  ic planning (lat
-000017f0: 7469 6365 2c20 5252 5429 2c20 6c6f 6361  tice, RRT), loca
-00001800: 6c69 7a61 7469 6f6e 2028 454b 462c 2070  lization (EKF, p
-00001810: 6172 7469 636c 6520 6669 6c74 6572 292c  article filter),
-00001820: 0a6d 6170 2062 7569 6c64 696e 6720 2845  .map building (E
-00001830: 4b46 2920 616e 6420 7369 6d75 6c74 616e  KF) and simultan
-00001840: 656f 7573 206c 6f63 616c 697a 6174 696f  eous localizatio
-00001850: 6e20 616e 6420 6d61 7070 696e 6720 2845  n and mapping (E
-00001860: 4b46 292e 0a0a 5468 6520 546f 6f6c 626f  KF)...The Toolbo
-00001870: 7820 7072 6f76 6964 6573 3a0a 0a2d 2063  x provides:..- c
-00001880: 6f64 6520 7468 6174 2069 7320 6d61 7475  ode that is matu
-00001890: 7265 2061 6e64 2070 726f 7669 6465 7320  re and provides 
-000018a0: 6120 706f 696e 7420 6f66 2063 6f6d 7061  a point of compa
-000018b0: 7269 736f 6e20 666f 7220 6f74 6865 720a  rison for other.
-000018c0: 2020 696d 706c 656d 656e 7461 7469 6f6e    implementation
-000018d0: 7320 6f66 2074 6865 2073 616d 6520 616c  s of the same al
-000018e0: 676f 7269 7468 6d73 3b0a 2d20 726f 7574  gorithms;.- rout
-000018f0: 696e 6573 2077 6869 6368 2061 7265 2067  ines which are g
-00001900: 656e 6572 616c 6c79 2077 7269 7474 656e  enerally written
-00001910: 2069 6e20 6120 7374 7261 6967 6874 666f   in a straightfo
-00001920: 7277 6172 6420 6d61 6e6e 6572 2077 6869  rward manner whi
-00001930: 6368 0a20 2061 6c6c 6f77 7320 666f 7220  ch.  allows for 
-00001940: 6561 7379 2075 6e64 6572 7374 616e 6469  easy understandi
-00001950: 6e67 2c20 7065 7268 6170 7320 6174 2074  ng, perhaps at t
-00001960: 6865 2065 7870 656e 7365 206f 6620 636f  he expense of co
-00001970: 6d70 7574 6174 696f 6e61 6c0a 2020 6566  mputational.  ef
-00001980: 6669 6369 656e 6379 3b0a 2d20 736f 7572  ficiency;.- sour
-00001990: 6365 2063 6f64 6520 7768 6963 6820 6361  ce code which ca
-000019a0: 6e20 6265 2072 6561 6420 666f 7220 6c65  n be read for le
-000019b0: 6172 6e69 6e67 2061 6e64 2074 6561 6368  arning and teach
-000019c0: 696e 673b 0a2d 2062 6163 6b77 6172 6420  ing;.- backward 
-000019d0: 636f 6d70 6174 6162 696c 6974 7920 7769  compatability wi
-000019e0: 7468 2074 6865 2052 6f62 6f74 6963 7320  th the Robotics 
-000019f0: 546f 6f6c 626f 7820 666f 7220 4d41 544c  Toolbox for MATL
-00001a00: 4142 0a0a 5468 6520 546f 6f6c 626f 7820  AB..The Toolbox 
-00001a10: 6c65 7665 7261 6765 7320 7468 6520 5b53  leverages the [S
-00001a20: 7061 7469 616c 204d 6174 6873 2054 6f6f  patial Maths Too
-00001a30: 6c62 6f78 2066 6f72 2050 7974 686f 6e5d  lbox for Python]
-00001a40: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00001a50: 636f 6d2f 7065 7465 7263 6f72 6b65 2f73  com/petercorke/s
-00001a60: 7061 7469 616c 6d61 7468 2d70 7974 686f  patialmath-pytho
-00001a70: 6e29 2074 6f0a 7072 6f76 6964 6520 7375  n) to.provide su
-00001a80: 7070 6f72 7420 666f 7220 6461 7461 2074  pport for data t
-00001a90: 7970 6573 2073 7563 6820 6173 2053 4f28  ypes such as SO(
-00001aa0: 6e29 2061 6e64 2053 4528 6e29 206d 6174  n) and SE(n) mat
-00001ab0: 7269 6365 732c 2071 7561 7465 726e 696f  rices, quaternio
-00001ac0: 6e73 2c20 7477 6973 7473 2061 6e64 2073  ns, twists and s
-00001ad0: 7061 7469 616c 2076 6563 746f 7273 2e0a  patial vectors..
-00001ae0: 0a3c 6272 3e0a 0a3c 6120 6964 3d27 3227  .<br>..<a id='2'
-00001af0: 3e3c 2f61 3e0a 0a23 2320 4765 7474 696e  ></a>..## Gettin
-00001b00: 6720 676f 696e 670a 0a59 6f75 2077 696c  g going..You wil
-00001b10: 6c20 6e65 6564 2050 7974 686f 6e20 3e3d  l need Python >=
-00001b20: 2033 2e36 0a0a 2323 2320 5573 696e 6720   3.6..### Using 
-00001b30: 7069 700a 0a49 6e73 7461 6c6c 2061 2073  pip..Install a s
-00001b40: 6e61 7073 686f 7420 6672 6f6d 2050 7950  napshot from PyP
-00001b50: 490a 0a60 6060 7368 656c 6c20 7363 7269  I..```shell scri
-00001b60: 7074 0a70 6970 3320 696e 7374 616c 6c20  pt.pip3 install 
-00001b70: 726f 626f 7469 6373 746f 6f6c 626f 782d  roboticstoolbox-
-00001b80: 7079 7468 6f6e 0a60 6060 0a0a 4176 6169  python.```..Avai
-00001b90: 6c61 626c 6520 6f70 7469 6f6e 7320 6172  lable options ar
-00001ba0: 653a 0a0a 2d20 6063 6f6c 6c69 7369 6f6e  e:..- `collision
-00001bb0: 6020 696e 7374 616c 6c20 636f 6c6c 6973  ` install collis
-00001bc0: 696f 6e20 6368 6563 6b69 6e67 2077 6974  ion checking wit
-00001bd0: 6820 5b70 7962 756c 6c65 745d 2868 7474  h [pybullet](htt
-00001be0: 7073 3a2f 2f70 7962 756c 6c65 742e 6f72  ps://pybullet.or
-00001bf0: 6729 0a0a 5075 7420 7468 6520 6f70 7469  g)..Put the opti
-00001c00: 6f6e 7320 696e 2061 2063 6f6d 6d61 2073  ons in a comma s
-00001c10: 6570 6172 6174 6564 206c 6973 7420 6c69  eparated list li
-00001c20: 6b65 0a0a 6060 6073 6865 6c6c 2073 6372  ke..```shell scr
-00001c30: 6970 740a 7069 7033 2069 6e73 7461 6c6c  ipt.pip3 install
-00001c40: 2072 6f62 6f74 6963 7374 6f6f 6c62 6f78   roboticstoolbox
-00001c50: 2d70 7974 686f 6e5b 6f70 7469 6f6e 6c69  -python[optionli
-00001c60: 7374 5d0a 6060 600a 0a5b 5377 6966 745d  st].```..[Swift]
-00001c70: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00001c80: 636f 6d2f 6a68 6176 6c2f 7377 6966 7429  com/jhavl/swift)
-00001c90: 2c20 6120 7765 622d 6261 7365 6420 7669  , a web-based vi
-00001ca0: 7375 616c 697a 6572 2c20 6973 0a69 6e73  sualizer, is.ins
-00001cb0: 7461 6c6c 6564 2061 7320 7061 7274 206f  talled as part o
-00001cc0: 6620 526f 626f 7469 6373 2054 6f6f 6c62  f Robotics Toolb
-00001cd0: 6f78 2e0a 0a23 2323 2046 726f 6d20 4769  ox...### From Gi
-00001ce0: 7448 7562 0a0a 546f 2069 6e73 7461 6c6c  tHub..To install
-00001cf0: 2074 6865 2062 6c65 6564 696e 672d 6564   the bleeding-ed
-00001d00: 6765 2076 6572 7369 6f6e 2066 726f 6d20  ge version from 
-00001d10: 4769 7448 7562 0a0a 6060 6073 6865 6c6c  GitHub..```shell
-00001d20: 2073 6372 6970 740a 6769 7420 636c 6f6e   script.git clon
-00001d30: 6520 6874 7470 733a 2f2f 6769 7468 7562  e https://github
-00001d40: 2e63 6f6d 2f70 6574 6572 636f 726b 652f  .com/petercorke/
-00001d50: 726f 626f 7469 6373 2d74 6f6f 6c62 6f78  robotics-toolbox
-00001d60: 2d70 7974 686f 6e2e 6769 740a 6364 2072  -python.git.cd r
-00001d70: 6f62 6f74 6963 732d 746f 6f6c 626f 782d  obotics-toolbox-
-00001d80: 7079 7468 6f6e 0a70 6970 3320 696e 7374  python.pip3 inst
-00001d90: 616c 6c20 2d65 202e 0a60 6060 0a0a 3c62  all -e ..```..<b
-00001da0: 723e 0a0a 3c61 2069 643d 2733 273e 3c2f  r>..<a id='3'></
-00001db0: 613e 0a0a 2323 2054 7574 6f72 6961 6c73  a>..## Tutorials
-00001dc0: 0a0a 3c74 6162 6c65 2073 7479 6c65 3d22  ..<table style="
-00001dd0: 626f 7264 6572 3a30 7078 223e 0a3c 7472  border:0px">.<tr
-00001de0: 2073 7479 6c65 3d22 626f 7264 6572 3a30   style="border:0
-00001df0: 7078 223e 0a3c 7464 2073 7479 6c65 3d22  px">.<td style="
-00001e00: 626f 7264 6572 3a30 7078 223e 3c61 2068  border:0px"><a h
-00001e10: 7265 663d 2268 7474 7073 3a2f 2f62 6974  ref="https://bit
-00001e20: 2e6c 792f 3361 6b35 4744 6922 3e3c 696d  .ly/3ak5GDi"><im
-00001e30: 6720 7372 633d 2268 7474 7073 3a2f 2f67  g src="https://g
-00001e40: 6974 6875 622e 636f 6d2f 6a68 6176 6c2f  ithub.com/jhavl/
-00001e50: 646b 742f 7261 772f 6d61 696e 2f69 6d67  dkt/raw/main/img
-00001e60: 2f61 7274 6963 6c65 312e 706e 6722 2077  /article1.png" w
-00001e70: 6964 7468 3d22 3430 3022 3e3c 2f61 3e3c  idth="400"></a><
-00001e80: 2f74 643e 0a3c 7464 2073 7479 6c65 3d22  /td>.<td style="
-00001e90: 626f 7264 6572 3a30 7078 223e 3c61 2068  border:0px"><a h
-00001ea0: 7265 663d 2268 7474 7073 3a2f 2f62 6974  ref="https://bit
-00001eb0: 2e6c 792f 3361 6b35 4744 6922 3e3c 696d  .ly/3ak5GDi"><im
-00001ec0: 6720 7372 633d 2268 7474 7073 3a2f 2f67  g src="https://g
-00001ed0: 6974 6875 622e 636f 6d2f 6a68 6176 6c2f  ithub.com/jhavl/
-00001ee0: 646b 742f 7261 772f 6d61 696e 2f69 6d67  dkt/raw/main/img
-00001ef0: 2f61 7274 6963 6c65 322e 706e 6722 2077  /article2.png" w
-00001f00: 6964 7468 3d22 3430 3022 3e3c 2f61 3e3c  idth="400"></a><
-00001f10: 2f74 643e 0a3c 7464 2073 7479 6c65 3d22  /td>.<td style="
-00001f20: 626f 7264 6572 3a30 7078 223e 0a44 6f20  border:0px">.Do 
-00001f30: 796f 7520 7761 6e74 2074 6f20 6c65 6172  you want to lear
-00001f40: 6e20 6162 6f75 7420 6d61 6e69 7075 6c61  n about manipula
-00001f50: 746f 7220 6b69 6e65 6d61 7469 6373 2c20  tor kinematics, 
-00001f60: 6469 6666 6572 656e 7469 616c 206b 696e  differential kin
-00001f70: 656d 6174 6963 732c 2069 6e76 6572 7365  ematics, inverse
-00001f80: 2d6b 696e 656d 6174 6963 7320 616e 6420  -kinematics and 
-00001f90: 6d6f 7469 6f6e 2063 6f6e 7472 6f6c 3f20  motion control? 
-00001fa0: 4861 7665 2061 206c 6f6f 6b20 6174 206f  Have a look at o
-00001fb0: 7572 0a3c 6120 6872 6566 3d22 6874 7470  ur.<a href="http
-00001fc0: 733a 2f2f 6269 742e 6c79 2f33 616b 3547  s://bit.ly/3ak5G
-00001fd0: 4469 223e 7475 746f 7269 616c 3c2f 613e  Di">tutorial</a>
-00001fe0: 2e0a 5468 6973 2074 7574 6f72 6961 6c20  ..This tutorial 
-00001ff0: 636f 6d65 7320 7769 7468 2074 776f 2061  comes with two a
-00002000: 7274 6963 6c65 7320 746f 2063 6f76 6572  rticles to cover
-00002010: 2074 6865 2074 6865 6f72 7920 616e 6420   the theory and 
-00002020: 3132 204a 7570 7974 6572 204e 6f74 6562  12 Jupyter Noteb
-00002030: 6f6f 6b73 2070 726f 7669 6469 6e67 2066  ooks providing f
-00002040: 756c 6c20 636f 6465 2069 6d70 6c65 6d65  ull code impleme
-00002050: 6e74 6174 696f 6e73 2061 6e64 2065 7861  ntations and exa
-00002060: 6d70 6c65 732e 204d 6f73 7420 6f66 2074  mples. Most of t
-00002070: 6865 204e 6f74 6562 6f6f 6b73 2061 7265  he Notebooks are
-00002080: 2061 6c73 6f20 476f 6f67 6c65 2043 6f6c   also Google Col
-00002090: 6162 2063 6f6d 7061 7469 626c 6520 616c  ab compatible al
-000020a0: 6c6f 7769 6e67 2074 6865 6d20 746f 2072  lowing them to r
-000020b0: 756e 206f 6e6c 696e 652e 0a3c 2f74 643e  un online..</td>
-000020c0: 0a3c 2f74 723e 0a3c 2f74 6162 6c65 3e0a  .</tr>.</table>.
-000020d0: 0a3c 6272 3e0a 0a3c 6120 6964 3d27 3427  .<br>..<a id='4'
-000020e0: 3e3c 2f61 3e0a 0a23 2320 436f 6465 2045  ></a>..## Code E
-000020f0: 7861 6d70 6c65 730a 0a57 6520 7769 6c6c  xamples..We will
-00002100: 206c 6f61 6420 6120 6d6f 6465 6c20 6f66   load a model of
-00002110: 2074 6865 2046 7261 6e6b 612d 456d 696b   the Franka-Emik
-00002120: 6120 5061 6e64 6120 726f 626f 7420 6465  a Panda robot de
-00002130: 6669 6e65 6420 6279 2061 2055 5244 4620  fined by a URDF 
-00002140: 6669 6c65 0a0a 6060 6070 7974 686f 6e0a  file..```python.
-00002150: 696d 706f 7274 2072 6f62 6f74 6963 7374  import roboticst
-00002160: 6f6f 6c62 6f78 2061 7320 7274 620a 726f  oolbox as rtb.ro
-00002170: 626f 7420 3d20 7274 622e 6d6f 6465 6c73  bot = rtb.models
-00002180: 2e50 616e 6461 2829 0a70 7269 6e74 2872  .Panda().print(r
-00002190: 6f62 6f74 290a 0a09 4552 6f62 6f74 3a20  obot)...ERobot: 
-000021a0: 7061 6e64 6120 2862 7920 4672 616e 6b61  panda (by Franka
-000021b0: 2045 6d69 6b61 292c 2037 206a 6f69 6e74   Emika), 7 joint
-000021c0: 7320 2852 5252 5252 5252 292c 2031 2067  s (RRRRRRR), 1 g
-000021d0: 7269 7070 6572 2c20 6765 6f6d 6574 7279  ripper, geometry
-000021e0: 2c20 636f 6c6c 6973 696f 6e0a 09e2 948c  , collision.....
-000021f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002200: 94ac e294 80e2 9480 e294 80e2 9480 e294  ................
-00002210: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002220: e294 80e2 9480 e294 80e2 9480 e294 ace2  ................
-00002230: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002240: 80e2 9480 e294 ace2 9480 e294 80e2 9480  ................
-00002250: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002260: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002270: ace2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002280: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002290: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000022a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000022b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000022c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000022d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000022e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000022f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002300: 80e2 9490 0a09 e294 826c 696e 6b20 e294  .........link ..
-00002310: 8220 2020 2020 6c69 6e6b 2020 2020 20e2  .     link     .
-00002320: 9482 206a 6f69 6e74 20e2 9482 2020 2070  .. joint ...   p
-00002330: 6172 656e 7420 2020 20e2 9482 2020 2020  arent    ...    
-00002340: 2020 2020 2020 2020 2020 4554 533a 2070            ETS: p
-00002350: 6172 656e 7420 746f 206c 696e 6b20 2020  arent to link   
-00002360: 2020 2020 2020 2020 2020 2020 e294 820a              ....
-00002370: 09e2 949c e294 80e2 9480 e294 80e2 9480  ................
-00002380: e294 80e2 94bc e294 80e2 9480 e294 80e2  ................
-00002390: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000023a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000023b0: e294 bce2 9480 e294 80e2 9480 e294 80e2  ................
-000023c0: 9480 e294 80e2 9480 e294 bce2 9480 e294  ................
-000023d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000023e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000023f0: 9480 e294 bce2 9480 e294 80e2 9480 e294  ................
-00002400: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002410: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002420: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002430: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002440: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002450: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002460: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002470: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002480: 9480 e294 80e2 94a4 0a09 e294 8220 2020  .............   
-00002490: 3020 e294 8220 7061 6e64 615f 6c69 6e6b  0 ... panda_link
-000024a0: 3020 20e2 9482 2020 2020 2020 20e2 9482  0  ...       ...
-000024b0: 2042 4153 4520 2020 2020 2020 20e2 9482   BASE        ...
-000024c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024f0: e294 820a 09e2 9482 2020 2031 20e2 9482  ........   1 ...
-00002500: 2070 616e 6461 5f6c 696e 6b31 2020 e294   panda_link1  ..
-00002510: 8220 2020 2020 3020 e294 8220 7061 6e64  .     0 ... pand
-00002520: 615f 6c69 6e6b 3020 e294 8220 5345 3328  a_link0 ... SE3(
-00002530: 302c 2030 2c20 302e 3333 3329 20e2 8a95  0, 0, 0.333) ...
-00002540: 2052 7a28 7130 2920 2020 2020 2020 2020   Rz(q0)         
-00002550: 2020 2020 2020 2020 2020 2020 20e2 9482               ...
-00002560: 0a09 e294 8220 2020 3220 e294 8220 7061  .....   2 ... pa
-00002570: 6e64 615f 6c69 6e6b 3220 20e2 9482 2020  nda_link2  ...  
-00002580: 2020 2031 20e2 9482 2070 616e 6461 5f6c     1 ... panda_l
-00002590: 696e 6b31 20e2 9482 2053 4533 282d 3930  ink1 ... SE3(-90
-000025a0: c2b0 2c20 2d30 c2b0 2c20 30c2 b029 20e2  .., -0.., 0..) .
-000025b0: 8a95 2052 7a28 7131 2920 2020 2020 2020  .. Rz(q1)       
-000025c0: 2020 2020 2020 2020 2020 2020 20e2 9482               ...
-000025d0: 0a09 e294 8220 2020 3320 e294 8220 7061  .....   3 ... pa
-000025e0: 6e64 615f 6c69 6e6b 3320 20e2 9482 2020  nda_link3  ...  
-000025f0: 2020 2032 20e2 9482 2070 616e 6461 5f6c     2 ... panda_l
-00002600: 696e 6b32 20e2 9482 2053 4533 2830 2c20  ink2 ... SE3(0, 
-00002610: 2d30 2e33 3136 2c20 303b 2039 30c2 b02c  -0.316, 0; 90..,
-00002620: 202d 30c2 b02c 2030 c2b0 2920 e28a 9520   -0.., 0..) ... 
-00002630: 527a 2871 3229 2020 2020 2020 20e2 9482  Rz(q2)       ...
-00002640: 0a09 e294 8220 2020 3420 e294 8220 7061  .....   4 ... pa
-00002650: 6e64 615f 6c69 6e6b 3420 20e2 9482 2020  nda_link4  ...  
-00002660: 2020 2033 20e2 9482 2070 616e 6461 5f6c     3 ... panda_l
-00002670: 696e 6b33 20e2 9482 2053 4533 2830 2e30  ink3 ... SE3(0.0
-00002680: 3832 352c 2030 2c20 303b 2039 30c2 b02c  825, 0, 0; 90..,
-00002690: 202d 30c2 b02c 2030 c2b0 2920 e28a 9520   -0.., 0..) ... 
-000026a0: 527a 2871 3329 2020 2020 2020 20e2 9482  Rz(q3)       ...
-000026b0: 0a09 e294 8220 2020 3520 e294 8220 7061  .....   5 ... pa
-000026c0: 6e64 615f 6c69 6e6b 3520 20e2 9482 2020  nda_link5  ...  
-000026d0: 2020 2034 20e2 9482 2070 616e 6461 5f6c     4 ... panda_l
-000026e0: 696e 6b34 20e2 9482 2053 4533 282d 302e  ink4 ... SE3(-0.
-000026f0: 3038 3235 2c20 302e 3338 342c 2030 3b20  0825, 0.384, 0; 
-00002700: 2d39 30c2 b02c 202d 30c2 b02c 2030 c2b0  -90.., -0.., 0..
-00002710: 2920 e28a 9520 527a 2871 3429 20e2 9482  ) ... Rz(q4) ...
-00002720: 0a09 e294 8220 2020 3620 e294 8220 7061  .....   6 ... pa
-00002730: 6e64 615f 6c69 6e6b 3620 20e2 9482 2020  nda_link6  ...  
-00002740: 2020 2035 20e2 9482 2070 616e 6461 5f6c     5 ... panda_l
-00002750: 696e 6b35 20e2 9482 2053 4533 2839 30c2  ink5 ... SE3(90.
-00002760: b02c 202d 30c2 b02c 2030 c2b0 2920 e28a  ., -0.., 0..) ..
-00002770: 9520 527a 2871 3529 2020 2020 2020 2020  . Rz(q5)        
-00002780: 2020 2020 2020 2020 2020 2020 20e2 9482               ...
-00002790: 0a09 e294 8220 2020 3720 e294 8220 7061  .....   7 ... pa
-000027a0: 6e64 615f 6c69 6e6b 3720 20e2 9482 2020  nda_link7  ...  
-000027b0: 2020 2036 20e2 9482 2070 616e 6461 5f6c     6 ... panda_l
-000027c0: 696e 6b36 20e2 9482 2053 4533 2830 2e30  ink6 ... SE3(0.0
-000027d0: 3838 2c20 302c 2030 3b20 3930 c2b0 2c20  88, 0, 0; 90.., 
-000027e0: 2d30 c2b0 2c20 30c2 b029 20e2 8a95 2052  -0.., 0..) ... R
-000027f0: 7a28 7136 2920 2020 2020 2020 20e2 9482  z(q6)        ...
-00002800: 0a09 e294 8220 2020 3820 e294 8220 4070  .....   8 ... @p
-00002810: 616e 6461 5f6c 696e 6b38 20e2 9482 2020  anda_link8 ...  
-00002820: 2020 2020 20e2 9482 2070 616e 6461 5f6c       ... panda_l
-00002830: 696e 6b37 20e2 9482 2053 4533 2830 2c20  ink7 ... SE3(0, 
-00002840: 302c 2030 2e31 3037 2920 2020 2020 2020  0, 0.107)       
-00002850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002860: 2020 2020 2020 2020 e294 820a 09e2 9494          ........
-00002870: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002880: 94b4 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002890: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000028a0: e294 80e2 9480 e294 80e2 9480 e294 b4e2  ................
-000028b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000028c0: 80e2 9480 e294 b4e2 9480 e294 80e2 9480  ................
-000028d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000028e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000028f0: b4e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002900: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002910: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002920: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002930: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002940: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002950: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002960: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002970: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002980: 80e2 9498 0a0a 09e2 948c e294 80e2 9480  ................
-00002990: e294 80e2 9480 e294 80e2 94ac e294 80e2  ................
-000029a0: 9480 e294 80e2 9480 e294 80e2 94ac e294  ................
-000029b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000029c0: e294 80e2 9480 e294 ace2 9480 e294 80e2  ................
-000029d0: 9480 e294 80e2 9480 e294 ace2 9480 e294  ................
-000029e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000029f0: e294 ace2 9480 e294 80e2 9480 e294 80e2  ................
-00002a00: 9480 e294 ace2 9480 e294 80e2 9480 e294  ................
-00002a10: 80e2 9480 e294 80e2 9480 e294 ace2 9480  ................
-00002a20: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002a30: 9490 0a09 e294 826e 616d 6520 e294 8220  .......name ... 
-00002a40: 7130 2020 e294 8220 7131 2020 2020 20e2  q0  ... q1     .
-00002a50: 9482 2071 3220 20e2 9482 2071 3320 2020  .. q2  ... q3   
-00002a60: 20e2 9482 2071 3420 20e2 9482 2071 3520   ... q4  ... q5 
-00002a70: 2020 20e2 9482 2071 3620 2020 e294 820a     ... q6   ....
-00002a80: 09e2 949c e294 80e2 9480 e294 80e2 9480  ................
-00002a90: e294 80e2 94bc e294 80e2 9480 e294 80e2  ................
-00002aa0: 9480 e294 80e2 94bc e294 80e2 9480 e294  ................
-00002ab0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002ac0: e294 bce2 9480 e294 80e2 9480 e294 80e2  ................
-00002ad0: 9480 e294 bce2 9480 e294 80e2 9480 e294  ................
-00002ae0: 80e2 9480 e294 80e2 9480 e294 bce2 9480  ................
-00002af0: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
-00002b00: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002b10: 80e2 9480 e294 bce2 9480 e294 80e2 9480  ................
-00002b20: e294 80e2 9480 e294 80e2 94a4 0a09 e294  ................
-00002b30: 8220 2071 7220 e294 8220 2030 c2b0 20e2  .  qr ...  0.. .
-00002b40: 9482 202d 3137 2e32 c2b0 20e2 9482 2020  .. -17.2.. ...  
-00002b50: 30c2 b020 e294 8220 2d31 3236 c2b0 20e2  0.. ... -126.. .
-00002b60: 9482 2020 30c2 b020 e294 8220 2031 3135  ..  0.. ...  115
-00002b70: c2b0 20e2 9482 2020 3435 c2b0 20e2 9482  .. ...  45.. ...
-00002b80: 0a09 e294 8220 2071 7a20 e294 8220 2030  .....  qz ...  0
-00002b90: c2b0 20e2 9482 2020 30c2 b020 2020 20e2  .. ...  0..    .
-00002ba0: 9482 2020 30c2 b020 e294 8220 2030 c2b0  ..  0.. ...  0..
-00002bb0: 2020 20e2 9482 2020 30c2 b020 e294 8220     ...  0.. ... 
-00002bc0: 2030 c2b0 2020 20e2 9482 2020 30c2 b020   0..   ...  0.. 
-00002bd0: 20e2 9482 0a09 e294 94e2 9480 e294 80e2   ...............
-00002be0: 9480 e294 80e2 9480 e294 b4e2 9480 e294  ................
-00002bf0: 80e2 9480 e294 80e2 9480 e294 b4e2 9480  ................
-00002c00: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002c10: 9480 e294 80e2 94b4 e294 80e2 9480 e294  ................
-00002c20: 80e2 9480 e294 80e2 94b4 e294 80e2 9480  ................
-00002c30: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002c40: 94b4 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002c50: 80e2 94b4 e294 80e2 9480 e294 80e2 9480  ................
-00002c60: e294 80e2 9480 e294 80e2 94b4 e294 80e2  ................
-00002c70: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002c80: 980a 6060 600a 0a54 6865 2073 796d 626f  ..```..The symbo
-00002c90: 6c20 6040 6020 696e 6469 6361 7465 7320  l `@` indicates 
-00002ca0: 7468 6520 6c69 6e6b 2061 7320 616e 2065  the link as an e
-00002cb0: 6e64 2d65 6666 6563 746f 722c 2061 206c  nd-effector, a l
-00002cc0: 6561 6620 6e6f 6465 2069 6e20 7468 6520  eaf node in the 
-00002cd0: 7269 6769 642d 626f 6479 0a74 7265 6520  rigid-body.tree 
-00002ce0: 2850 7974 686f 6e20 7072 6f6d 7074 7320  (Python prompts 
-00002cf0: 6172 6520 6e6f 7420 7368 6f77 6e20 746f  are not shown to
-00002d00: 206d 616b 6520 6974 2065 6173 7920 746f   make it easy to
-00002d10: 2063 6f70 792b 7061 7374 6520 7468 6520   copy+paste the 
-00002d20: 636f 6465 2c20 636f 6e73 6f6c 6520 6f75  code, console ou
-00002d30: 7470 7574 2069 7320 696e 6465 6e74 6564  tput is indented
-00002d40: 292e 0a57 6520 7769 6c6c 2063 6f6d 7075  )..We will compu
-00002d50: 7465 2074 6865 2066 6f72 7761 7264 206b  te the forward k
-00002d60: 696e 656d 6174 6963 7320 6e65 7874 0a0a  inematics next..
-00002d70: 6060 600a 5465 203d 2072 6f62 6f74 2e66  ```.Te = robot.f
-00002d80: 6b69 6e65 2872 6f62 6f74 2e71 7229 2020  kine(robot.qr)  
-00002d90: 2320 666f 7277 6172 6420 6b69 6e65 6d61  # forward kinema
-00002da0: 7469 6373 0a70 7269 6e74 2854 6529 0a0a  tics.print(Te)..
-00002db0: 0930 2e39 3935 2020 2020 2030 2020 2020  .0.995     0    
-00002dc0: 2020 2020 2030 2e30 3939 3833 2020 2030       0.09983   0
-00002dd0: 2e34 3834 0a09 3020 2020 2020 2020 202d  .484..0        -
-00002de0: 3120 2020 2020 2020 2020 3020 2020 2020  1         0     
-00002df0: 2020 2020 300a 0930 2e30 3939 3833 2020      0..0.09983  
-00002e00: 2030 2020 2020 2020 2020 2d30 2e39 3935   0        -0.995
-00002e10: 2020 2020 2030 2e34 3132 360a 0930 2020       0.4126..0  
-00002e20: 2020 2020 2020 2030 2020 2020 2020 2020         0        
-00002e30: 2030 2020 2020 2020 2020 2031 0a60 6060   0         1.```
-00002e40: 0a0a 5765 2063 616e 2073 6f6c 7665 2069  ..We can solve i
-00002e50: 6e76 6572 7365 206b 696e 656d 6174 6963  nverse kinematic
-00002e60: 7320 7665 7279 2065 6173 696c 792e 2057  s very easily. W
-00002e70: 6520 6669 7273 7420 6368 6f6f 7365 2061  e first choose a
-00002e80: 6e20 5345 2833 2920 706f 7365 0a64 6566  n SE(3) pose.def
-00002e90: 696e 6564 2069 6e20 7465 726d 7320 6f66  ined in terms of
-00002ea0: 2070 6f73 6974 696f 6e20 616e 6420 6f72   position and or
-00002eb0: 6965 6e74 6174 696f 6e20 2865 6e64 2d65  ientation (end-e
-00002ec0: 6666 6563 746f 7220 7a2d 6178 6973 2064  ffector z-axis d
-00002ed0: 6f77 6e20 2841 3d2d 5a29 2061 6e64 2066  own (A=-Z) and f
-00002ee0: 696e 6765 720a 6f72 6965 6e74 6174 696f  inger.orientatio
-00002ef0: 6e20 7061 7261 6c6c 656c 2074 6f20 792d  n parallel to y-
-00002f00: 6178 6973 2028 4f3d 2b59 2929 2e0a 0a60  axis (O=+Y))...`
-00002f10: 6060 7079 7468 6f6e 0a66 726f 6d20 7370  ``python.from sp
-00002f20: 6174 6961 6c6d 6174 6820 696d 706f 7274  atialmath import
-00002f30: 2053 4533 0a0a 5465 7020 3d20 5345 332e   SE3..Tep = SE3.
-00002f40: 5472 616e 7328 302e 362c 202d 302e 332c  Trans(0.6, -0.3,
-00002f50: 2030 2e31 2920 2a20 5345 332e 4f41 285b   0.1) * SE3.OA([
-00002f60: 302c 2031 2c20 305d 2c20 5b30 2c20 302c  0, 1, 0], [0, 0,
-00002f70: 202d 315d 290a 736f 6c20 3d20 726f 626f   -1]).sol = robo
-00002f80: 742e 696b 5f6c 6d5f 6368 616e 2854 6570  t.ik_lm_chan(Tep
-00002f90: 2920 2020 2020 2020 2020 2320 736f 6c76  )         # solv
-00002fa0: 6520 494b 0a70 7269 6e74 2873 6f6c 290a  e IK.print(sol).
-00002fb0: 0a09 2861 7272 6179 285b 2030 2e32 3035  ..(array([ 0.205
-00002fc0: 3932 3831 352c 2020 302e 3836 3630 3934  92815,  0.866094
-00002fd0: 3831 2c20 2d30 2e37 3934 3733 3230 362c  81, -0.79473206,
-00002fe0: 202d 312e 3638 3235 3437 3934 2c20 2030   -1.68254794,  0
-00002ff0: 2e37 3438 3732 3931 352c 0a09 0909 322e  .74872915,....2.
-00003000: 3231 3736 3437 3436 2c20 2d30 2e31 3032  21764746, -0.102
-00003010: 3535 3630 365d 292c 2031 2c20 3131 342c  55606]), 1, 114,
-00003020: 2037 2c20 322e 3839 3031 3634 3035 3732   7, 2.8901640572
-00003030: 3330 3232 3865 2d30 3729 0a0a 715f 7069  30228e-07)..q_pi
-00003040: 636b 7570 203d 2073 6f6c 5b30 5d0a 7072  ckup = sol[0].pr
-00003050: 696e 7428 726f 626f 742e 666b 696e 6528  int(robot.fkine(
-00003060: 715f 7069 636b 7570 2929 2020 2020 2320  q_pickup))    # 
-00003070: 464b 2073 686f 7773 2074 6861 7420 6465  FK shows that de
-00003080: 7369 7265 6420 656e 642d 6566 6665 6374  sired end-effect
-00003090: 6f72 2070 6f73 6520 7761 7320 6163 6869  or pose was achi
-000030a0: 6576 6564 0a0a 0920 3120 2020 2020 2020  eved... 1       
-000030b0: 2020 2d38 2e39 3133 652d 3035 2020 2d30    -8.913e-05  -0
-000030c0: 2e30 3030 3333 3334 2020 302e 3539 3936  .0003334  0.5996
-000030d0: 0a09 2d38 2e39 3239 652d 3035 202d 3120  ..-8.929e-05 -1 
-000030e0: 2020 2020 2020 2020 202d 302e 3030 3034           -0.0004
-000030f0: 3931 3220 2d30 2e32 3939 380a 092d 302e  912 -0.2998..-0.
-00003100: 3030 3033 3333 3420 2030 2e30 3030 3439  0003334  0.00049
-00003110: 3132 2020 2d31 2020 2020 2020 2020 2020  12  -1          
-00003120: 302e 3130 3031 0a09 2030 2020 2020 2020  0.1001.. 0      
-00003130: 2020 2020 3020 2020 2020 2020 2020 2020      0           
-00003140: 3020 2020 2020 2020 2020 2031 0a60 6060  0          1.```
-00003150: 0a0a 5765 2063 616e 2061 6e69 6d61 7465  ..We can animate
-00003160: 2061 2070 6174 6820 6672 6f6d 2074 6865   a path from the
-00003170: 2072 6561 6479 2070 6f73 6520 6071 7260   ready pose `qr`
-00003180: 2063 6f6e 6669 6775 7261 7469 6f6e 2074   configuration t
-00003190: 6f20 7468 6973 2070 6963 6b75 7020 636f  o this pickup co
-000031a0: 6e66 6967 7572 6174 696f 6e0a 0a60 6060  nfiguration..```
-000031b0: 7079 7468 6f6e 0a71 7420 3d20 7274 622e  python.qt = rtb.
-000031c0: 6a74 7261 6a28 726f 626f 742e 7172 2c20  jtraj(robot.qr, 
-000031d0: 715f 7069 636b 7570 2c20 3530 290a 726f  q_pickup, 50).ro
-000031e0: 626f 742e 706c 6f74 2871 742e 712c 2062  bot.plot(qt.q, b
-000031f0: 6163 6b65 6e64 3d27 7079 706c 6f74 272c  ackend='pyplot',
-00003200: 206d 6f76 6965 3d27 7061 6e64 6131 2e67   movie='panda1.g
-00003210: 6966 2729 0a60 6060 0a0a 3c70 2061 6c69  if').```..<p ali
-00003220: 676e 3d22 6365 6e74 6572 223e 0a09 3c69  gn="center">..<i
-00003230: 6d67 2073 7263 3d22 2e2f 646f 6373 2f66  mg src="./docs/f
-00003240: 6967 732f 7061 6e64 6131 2e67 6966 223e  igs/panda1.gif">
-00003250: 0a3c 2f70 3e0a 0a77 6865 7265 2077 6520  .</p>..where we 
-00003260: 6861 7665 2073 7065 6369 6669 6564 2074  have specified t
-00003270: 6865 206d 6174 706c 6f74 6c69 6220 6070  he matplotlib `p
-00003280: 7970 6c6f 7460 2062 6163 6b65 6e64 2e20  yplot` backend. 
-00003290: 426c 7565 2061 7272 6f77 7320 7368 6f77  Blue arrows show
-000032a0: 2074 6865 206a 6f69 6e74 2061 7865 7320   the joint axes 
-000032b0: 616e 6420 7468 6520 636f 6c6f 7572 6564  and the coloured
-000032c0: 2066 7261 6d65 2073 686f 7773 2074 6865   frame shows the
-000032d0: 2065 6e64 2d65 6666 6563 746f 7220 706f   end-effector po
-000032e0: 7365 2e0a 0a57 6520 6361 6e20 616c 736f  se...We can also
-000032f0: 2070 6c6f 7420 7468 6520 7472 616a 6563   plot the trajec
-00003300: 746f 7279 2069 6e20 7468 6520 5377 6966  tory in the Swif
-00003310: 7420 7369 6d75 6c61 746f 7220 2861 2062  t simulator (a b
-00003320: 726f 7773 6572 2d62 6173 6564 2033 642d  rowser-based 3d-
-00003330: 7369 6d75 6c61 7469 6f6e 2065 6e76 6972  simulation envir
-00003340: 6f6e 6d65 6e74 2062 7569 6c74 2074 6f20  onment built to 
-00003350: 776f 726b 2077 6974 6820 7468 6520 546f  work with the To
-00003360: 6f6c 626f 7829 0a0a 6060 6070 7974 686f  olbox)..```pytho
-00003370: 6e0a 726f 626f 742e 706c 6f74 2871 742e  n.robot.plot(qt.
-00003380: 7129 0a60 6060 0a0a 3c70 2061 6c69 676e  q).```..<p align
-00003390: 3d22 6365 6e74 6572 223e 0a09 3c69 6d67  ="center">..<img
-000033a0: 2073 7263 3d22 2e2f 646f 6373 2f66 6967   src="./docs/fig
-000033b0: 732f 7061 6e64 6132 2e67 6966 223e 0a3c  s/panda2.gif">.<
-000033c0: 2f70 3e0a 0a57 6520 6361 6e20 616c 736f  /p>..We can also
-000033d0: 2065 7870 6572 696d 656e 7420 7769 7468   experiment with
-000033e0: 2076 656c 6f63 6974 7920 636f 6e74 726f   velocity contro
-000033f0: 6c6c 6572 7320 696e 2053 7769 6674 2e20  llers in Swift. 
-00003400: 4865 7265 2069 7320 6120 7265 736f 6c76  Here is a resolv
-00003410: 6564 2d72 6174 6520 6d6f 7469 6f6e 2063  ed-rate motion c
-00003420: 6f6e 7472 6f6c 2065 7861 6d70 6c65 0a0a  ontrol example..
-00003430: 6060 6070 7974 686f 6e0a 696d 706f 7274  ```python.import
-00003440: 2073 7769 6674 0a69 6d70 6f72 7420 726f   swift.import ro
-00003450: 626f 7469 6373 746f 6f6c 626f 7820 6173  boticstoolbox as
-00003460: 2072 700a 696d 706f 7274 2073 7061 7469   rp.import spati
-00003470: 616c 6d61 7468 2061 7320 736d 0a69 6d70  almath as sm.imp
-00003480: 6f72 7420 6e75 6d70 7920 6173 206e 700a  ort numpy as np.
-00003490: 0a65 6e76 203d 2073 7769 6674 2e53 7769  .env = swift.Swi
-000034a0: 6674 2829 0a65 6e76 2e6c 6175 6e63 6828  ft().env.launch(
-000034b0: 7265 616c 7469 6d65 3d54 7275 6529 0a0a  realtime=True)..
-000034c0: 7061 6e64 6120 3d20 7270 2e6d 6f64 656c  panda = rp.model
-000034d0: 732e 5061 6e64 6128 290a 7061 6e64 612e  s.Panda().panda.
-000034e0: 7120 3d20 7061 6e64 612e 7172 0a0a 5465  q = panda.qr..Te
-000034f0: 7020 3d20 7061 6e64 612e 666b 696e 6528  p = panda.fkine(
-00003500: 7061 6e64 612e 7129 202a 2073 6d2e 5345  panda.q) * sm.SE
-00003510: 332e 5472 616e 7328 302e 322c 2030 2e32  3.Trans(0.2, 0.2
-00003520: 2c20 302e 3435 290a 0a61 7272 6976 6564  , 0.45)..arrived
-00003530: 203d 2046 616c 7365 0a65 6e76 2e61 6464   = False.env.add
-00003540: 2870 616e 6461 290a 0a64 7420 3d20 302e  (panda)..dt = 0.
-00003550: 3035 0a0a 7768 696c 6520 6e6f 7420 6172  05..while not ar
-00003560: 7269 7665 643a 0a0a 2020 2020 762c 2061  rived:..    v, a
-00003570: 7272 6976 6564 203d 2072 702e 705f 7365  rrived = rp.p_se
-00003580: 7276 6f28 7061 6e64 612e 666b 696e 6528  rvo(panda.fkine(
-00003590: 7061 6e64 612e 7129 2c20 5465 702c 2031  panda.q), Tep, 1
-000035a0: 290a 2020 2020 7061 6e64 612e 7164 203d  ).    panda.qd =
-000035b0: 206e 702e 6c69 6e61 6c67 2e70 696e 7628   np.linalg.pinv(
-000035c0: 7061 6e64 612e 6a61 636f 6265 2870 616e  panda.jacobe(pan
-000035d0: 6461 2e71 2929 2040 2076 0a20 2020 2065  da.q)) @ v.    e
-000035e0: 6e76 2e73 7465 7028 6474 290a 0a23 2055  nv.step(dt)..# U
-000035f0: 6e63 6f6d 6d65 6e74 2074 6f20 7374 6f70  ncomment to stop
-00003600: 2074 6865 2062 726f 7773 6572 2074 6162   the browser tab
-00003610: 2066 726f 6d20 636c 6f73 696e 670a 2320   from closing.# 
-00003620: 656e 762e 686f 6c64 2829 0a60 6060 0a0a  env.hold().```..
-00003630: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
-00003640: 223e 0a09 3c69 6d67 2073 7263 3d22 2e2f  ">..<img src="./
-00003650: 646f 6373 2f66 6967 732f 7061 6e64 6133  docs/figs/panda3
-00003660: 2e67 6966 223e 0a3c 2f70 3e0a 0a23 2323  .gif">.</p>..###
-00003670: 2052 756e 2073 6f6d 6520 6578 616d 706c   Run some exampl
-00003680: 6573 0a0a 5468 6520 5b60 6e6f 7465 626f  es..The [`notebo
-00003690: 6f6b 7360 5d28 6874 7470 733a 2f2f 6769  oks`](https://gi
-000036a0: 7468 7562 2e63 6f6d 2f70 6574 6572 636f  thub.com/peterco
-000036b0: 726b 652f 726f 626f 7469 6373 2d74 6f6f  rke/robotics-too
-000036c0: 6c62 6f78 2d70 7974 686f 6e2f 7472 6565  lbox-python/tree
-000036d0: 2f6d 6173 7465 722f 6e6f 7465 626f 6f6b  /master/notebook
-000036e0: 7329 2066 6f6c 6465 7220 636f 6e74 6169  s) folder contai
-000036f0: 6e73 2073 6f6d 6520 7475 746f 7269 616c  ns some tutorial
-00003700: 204a 7570 7974 6572 206e 6f74 6562 6f6f   Jupyter noteboo
-00003710: 6b73 2077 6869 6368 2079 6f75 2063 616e  ks which you can
-00003720: 2062 726f 7773 6520 6f6e 2047 6974 4875   browse on GitHu
-00003730: 622e 2041 6464 6974 696f 6e61 6c6c 792c  b. Additionally,
-00003740: 2068 6176 6520 6120 6c6f 6f6b 2069 6e20   have a look in 
-00003750: 7468 6520 5b60 6578 616d 706c 6573 605d  the [`examples`]
-00003760: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00003770: 636f 6d2f 7065 7465 7263 6f72 6b65 2f72  com/petercorke/r
-00003780: 6f62 6f74 6963 732d 746f 6f6c 626f 782d  obotics-toolbox-
-00003790: 7079 7468 6f6e 2f74 7265 652f 6d61 7374  python/tree/mast
-000037a0: 6572 2f72 6f62 6f74 6963 7374 6f6f 6c62  er/roboticstoolb
-000037b0: 6f78 2f65 7861 6d70 6c65 7329 2066 6f6c  ox/examples) fol
-000037c0: 6465 7220 666f 7220 6d61 6e79 2072 6561  der for many rea
-000037d0: 6479 2074 6f20 7275 6e20 6578 616d 706c  dy to run exampl
-000037e0: 6573 2e0a 0a3c 6272 3e0a 0a3c 6120 6964  es...<br>..<a id
-000037f0: 3d27 3527 3e3c 2f61 3e0a 0a23 2320 546f  ='5'></a>..## To
-00003800: 6f6c 626f 7820 5265 7365 6172 6368 2041  olbox Research A
-00003810: 7070 6c69 6361 7469 6f6e 730a 0a54 6865  pplications..The
-00003820: 2074 6f6f 6c62 6f78 2069 7320 696e 6372   toolbox is incr
-00003830: 6564 6962 6c79 2075 7365 6675 6c20 666f  edibly useful fo
-00003840: 7220 6465 7665 6c6f 7069 6e67 2061 6e64  r developing and
-00003850: 2070 726f 746f 7479 7069 6e67 2061 6c67   prototyping alg
-00003860: 6f72 6974 686d 7320 666f 7220 7265 7365  orithms for rese
-00003870: 6172 6368 2c20 7468 616e 6b73 2074 6f20  arch, thanks to 
-00003880: 7468 6520 6578 6861 7573 7469 7665 2073  the exhaustive s
-00003890: 6574 206f 6620 7765 6c6c 2064 6f63 756d  et of well docum
-000038a0: 656e 7465 6420 616e 6420 6d61 7475 7265  ented and mature
-000038b0: 2072 6f62 6f74 6963 2066 756e 6374 696f   robotic functio
-000038c0: 6e73 2065 7870 6f73 6564 2074 6872 6f75  ns exposed throu
-000038d0: 6768 2063 6c65 616e 2061 6e64 2070 6169  gh clean and pai
-000038e0: 6e6c 6573 7320 4150 4973 2e20 4164 6469  nless APIs. Addi
-000038f0: 7469 6f6e 616c 6c79 2c20 7468 6520 6561  tionally, the ea
-00003900: 7365 2061 7420 7768 6963 6820 6120 7573  se at which a us
-00003910: 6572 2063 616e 2076 6973 7561 6c69 7a65  er can visualize
-00003920: 2074 6865 6972 2061 6c67 6f72 6974 686d   their algorithm
-00003930: 2073 7570 706f 7274 7320 6120 7261 7069   supports a rapi
-00003940: 6420 7072 6f74 6f74 7970 696e 6720 7061  d prototyping pa
-00003950: 7261 6469 676d 2e0a 0a23 2323 2050 7562  radigm...### Pub
-00003960: 6c69 6361 7469 6f6e 204c 6973 740a 0a4a  lication List..J
-00003970: 2e20 4861 7669 6c61 6e64 2c20 4e2e 2053  . Haviland, N. S
-00003980: c3bc 6e64 6572 6861 7566 2061 6e64 2050  ..nderhauf and P
-00003990: 2e20 436f 726b 652c 2022 2a2a 4120 486f  . Corke, "**A Ho
-000039a0: 6c69 7374 6963 2041 7070 726f 6163 6820  listic Approach 
-000039b0: 746f 2052 6561 6374 6976 6520 4d6f 6269  to Reactive Mobi
-000039c0: 6c65 204d 616e 6970 756c 6174 696f 6e2a  le Manipulation*
-000039d0: 2a2c 2220 696e 205f 4945 4545 2052 6f62  *," in _IEEE Rob
-000039e0: 6f74 6963 7320 616e 6420 4175 746f 6d61  otics and Automa
-000039f0: 7469 6f6e 204c 6574 7465 7273 5f2c 2064  tion Letters_, d
-00003a00: 6f69 3a20 3130 2e31 3130 392f 4c52 412e  oi: 10.1109/LRA.
-00003a10: 3230 3232 2e33 3134 3635 3534 2e20 496e  2022.3146554. In
-00003a20: 2074 6865 2076 6964 656f 2c20 7468 6520   the video, the 
-00003a30: 726f 626f 7420 6973 2063 6f6e 7472 6f6c  robot is control
-00003a40: 6c65 6420 7573 696e 6720 7468 6520 526f  led using the Ro
-00003a50: 626f 7469 6373 2074 6f6f 6c62 6f78 2066  botics toolbox f
-00003a60: 6f72 2050 7974 686f 6e20 616e 6420 6665  or Python and fe
-00003a70: 6174 7572 6573 2061 2072 6563 6f72 6469  atures a recordi
-00003a80: 6e67 2066 726f 6d20 7468 6520 5b53 7769  ng from the [Swi
-00003a90: 6674 5d28 6874 7470 733a 2f2f 6769 7468  ft](https://gith
-00003aa0: 7562 2e63 6f6d 2f6a 6861 766c 2f73 7769  ub.com/jhavl/swi
-00003ab0: 6674 2920 5369 6d75 6c61 746f 722e 0a0a  ft) Simulator...
-00003ac0: 5b5b 4172 7869 7620 5061 7065 725d 2868  [[Arxiv Paper](h
-00003ad0: 7474 7073 3a2f 2f61 7278 6976 2e6f 7267  ttps://arxiv.org
-00003ae0: 2f61 6273 2f32 3130 392e 3034 3734 3929  /abs/2109.04749)
-00003af0: 5d20 5b5b 4945 4545 2058 706c 6f72 655d  ] [[IEEE Xplore]
-00003b00: 2868 7474 7073 3a2f 2f69 6565 6578 706c  (https://ieeexpl
-00003b10: 6f72 652e 6965 6565 2e6f 7267 2f61 6273  ore.ieee.org/abs
-00003b20: 7472 6163 742f 646f 6375 6d65 6e74 2f39  tract/document/9
-00003b30: 3639 3532 3938 295d 205b 5b50 726f 6a65  695298)] [[Proje
-00003b40: 6374 2057 6562 7369 7465 5d28 6874 7470  ct Website](http
-00003b50: 733a 2f2f 6a68 6176 6c2e 6769 7468 7562  s://jhavl.github
-00003b60: 2e69 6f2f 686f 6c69 7374 6963 2f29 5d20  .io/holistic/)] 
-00003b70: 5b5b 5669 6465 6f5d 2868 7474 7073 3a2f  [[Video](https:/
-00003b80: 2f79 6f75 7475 2e62 652f 2d44 5842 5150  /youtu.be/-DXBQP
-00003b90: 654c 4956 3429 5d20 5b5b 436f 6465 2045  eLIV4)] [[Code E
-00003ba0: 7861 6d70 6c65 5d28 6874 7470 733a 2f2f  xample](https://
-00003bb0: 6769 7468 7562 2e63 6f6d 2f70 6574 6572  github.com/peter
-00003bc0: 636f 726b 652f 726f 626f 7469 6373 2d74  corke/robotics-t
-00003bd0: 6f6f 6c62 6f78 2d70 7974 686f 6e2f 626c  oolbox-python/bl
-00003be0: 6f62 2f6d 6173 7465 722f 726f 626f 7469  ob/master/roboti
-00003bf0: 6373 746f 6f6c 626f 782f 6578 616d 706c  cstoolbox/exampl
-00003c00: 6573 2f68 6f6c 6973 7469 635f 6d6d 5f6e  es/holistic_mm_n
-00003c10: 6f6e 5f68 6f6c 6f6e 6f6d 6963 2e70 7929  on_holonomic.py)
-00003c20: 5d0a 0a3c 703e 0a20 203c 6120 6872 6566  ]..<p>.  <a href
-00003c30: 3d22 6874 7470 733a 2f2f 796f 7574 752e  ="https://youtu.
-00003c40: 6265 2f2d 4458 4251 5065 4c49 5634 223e  be/-DXBQPeLIV4">
-00003c50: 0a20 2020 203c 696d 6720 7372 633d 2268  .    <img src="h
-00003c60: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00003c70: 6d2f 7065 7465 7263 6f72 6b65 2f72 6f62  m/petercorke/rob
-00003c80: 6f74 6963 732d 746f 6f6c 626f 782d 7079  otics-toolbox-py
-00003c90: 7468 6f6e 2f72 6177 2f6d 6173 7465 722f  thon/raw/master/
-00003ca0: 646f 6373 2f66 6967 732f 686f 6c69 7374  docs/figs/holist
-00003cb0: 6963 5f79 6f75 7475 6265 2e70 6e67 2220  ic_youtube.png" 
-00003cc0: 7769 6474 683d 2235 3630 223e 0a20 203c  width="560">.  <
-00003cd0: 2f61 3e0a 3c2f 703e 0a0a 4a2e 2048 6176  /a>.</p>..J. Hav
-00003ce0: 696c 616e 6420 616e 6420 502e 2043 6f72  iland and P. Cor
-00003cf0: 6b65 2c20 222a 2a4e 454f 3a20 4120 4e6f  ke, "**NEO: A No
-00003d00: 7665 6c20 4578 7065 6469 7469 6f75 7320  vel Expeditious 
-00003d10: 4f70 7469 6d69 7361 7469 6f6e 2041 6c67  Optimisation Alg
-00003d20: 6f72 6974 686d 2066 6f72 2052 6561 6374  orithm for React
-00003d30: 6976 6520 4d6f 7469 6f6e 2043 6f6e 7472  ive Motion Contr
-00003d40: 6f6c 206f 6620 4d61 6e69 7075 6c61 746f  ol of Manipulato
-00003d50: 7273 2a2a 2c22 2069 6e20 5f49 4545 4520  rs**," in _IEEE 
-00003d60: 526f 626f 7469 6373 2061 6e64 2041 7574  Robotics and Aut
-00003d70: 6f6d 6174 696f 6e20 4c65 7474 6572 735f  omation Letters_
-00003d80: 2c20 646f 693a 2031 302e 3131 3039 2f4c  , doi: 10.1109/L
-00003d90: 5241 2e32 3032 312e 3330 3536 3036 302e  RA.2021.3056060.
-00003da0: 2049 6e20 7468 6520 7669 6465 6f2c 2074   In the video, t
-00003db0: 6865 2072 6f62 6f74 2069 7320 636f 6e74  he robot is cont
-00003dc0: 726f 6c6c 6564 2075 7369 6e67 2074 6865  rolled using the
-00003dd0: 2052 6f62 6f74 6963 7320 746f 6f6c 626f   Robotics toolbo
-00003de0: 7820 666f 7220 5079 7468 6f6e 2061 6e64  x for Python and
-00003df0: 2066 6561 7475 7265 7320 6120 7265 636f   features a reco
-00003e00: 7264 696e 6720 6672 6f6d 2074 6865 205b  rding from the [
-00003e10: 5377 6966 745d 2868 7474 7073 3a2f 2f67  Swift](https://g
-00003e20: 6974 6875 622e 636f 6d2f 6a68 6176 6c2f  ithub.com/jhavl/
-00003e30: 7377 6966 7429 2053 696d 756c 6174 6f72  swift) Simulator
-00003e40: 2e0a 0a5b 5b41 7278 6976 2050 6170 6572  ...[[Arxiv Paper
-00003e50: 5d28 6874 7470 733a 2f2f 6172 7869 762e  ](https://arxiv.
-00003e60: 6f72 672f 6162 732f 3230 3130 2e30 3836  org/abs/2010.086
-00003e70: 3836 295d 205b 5b49 4545 4520 5870 6c6f  86)] [[IEEE Xplo
-00003e80: 7265 5d28 6874 7470 733a 2f2f 6965 6565  re](https://ieee
-00003e90: 7870 6c6f 7265 2e69 6565 652e 6f72 672f  xplore.ieee.org/
-00003ea0: 646f 6375 6d65 6e74 2f39 3334 3337 3138  document/9343718
-00003eb0: 295d 205b 5b50 726f 6a65 6374 2057 6562  )] [[Project Web
-00003ec0: 7369 7465 5d28 6874 7470 733a 2f2f 6a68  site](https://jh
-00003ed0: 6176 6c2e 6769 7468 7562 2e69 6f2f 6e65  avl.github.io/ne
-00003ee0: 6f2f 295d 205b 5b56 6964 656f 5d28 6874  o/)] [[Video](ht
-00003ef0: 7470 733a 2f2f 796f 7574 752e 6265 2f6a  tps://youtu.be/j
-00003f00: 534c 504a 4272 3851 5459 295d 205b 5b43  SLPJBr8QTY)] [[C
-00003f10: 6f64 6520 4578 616d 706c 655d 2868 7474  ode Example](htt
-00003f20: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00003f30: 7065 7465 7263 6f72 6b65 2f72 6f62 6f74  petercorke/robot
-00003f40: 6963 732d 746f 6f6c 626f 782d 7079 7468  ics-toolbox-pyth
-00003f50: 6f6e 2f62 6c6f 622f 6d61 7374 6572 2f72  on/blob/master/r
-00003f60: 6f62 6f74 6963 7374 6f6f 6c62 6f78 2f65  oboticstoolbox/e
-00003f70: 7861 6d70 6c65 732f 6e65 6f2e 7079 295d  xamples/neo.py)]
-00003f80: 0a0a 3c70 3e0a 2020 3c61 2068 7265 663d  ..<p>.  <a href=
-00003f90: 2268 7474 7073 3a2f 2f79 6f75 7475 2e62  "https://youtu.b
-00003fa0: 652f 6a53 4c50 4a42 7238 5154 5922 3e0a  e/jSLPJBr8QTY">.
-00003fb0: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
-00003fc0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00003fd0: 2f70 6574 6572 636f 726b 652f 726f 626f  /petercorke/robo
-00003fe0: 7469 6373 2d74 6f6f 6c62 6f78 2d70 7974  tics-toolbox-pyt
-00003ff0: 686f 6e2f 7261 772f 6d61 7374 6572 2f64  hon/raw/master/d
-00004000: 6f63 732f 6669 6773 2f6e 656f 5f79 6f75  ocs/figs/neo_you
-00004010: 7475 6265 2e70 6e67 2220 7769 6474 683d  tube.png" width=
-00004020: 2235 3630 223e 0a20 203c 2f61 3e0a 3c2f  "560">.  </a>.</
-00004030: 703e 0a0a 2a2a 4120 5075 7265 6c79 2d52  p>..**A Purely-R
-00004040: 6561 6374 6976 6520 4d61 6e69 7075 6c61  eactive Manipula
-00004050: 6269 6c69 7479 2d4d 6178 696d 6973 696e  bility-Maximisin
-00004060: 6720 4d6f 7469 6f6e 2043 6f6e 7472 6f6c  g Motion Control
-00004070: 6c65 722a 2a2c 204a 2e20 4861 7669 6c61  ler**, J. Havila
-00004080: 6e64 2061 6e64 2050 2e20 436f 726b 652e  nd and P. Corke.
-00004090: 2049 6e20 7468 6520 7669 6465 6f2c 2074   In the video, t
-000040a0: 6865 2072 6f62 6f74 2069 7320 636f 6e74  he robot is cont
-000040b0: 726f 6c6c 6564 2075 7369 6e67 2074 6865  rolled using the
-000040c0: 2052 6f62 6f74 6963 7320 746f 6f6c 626f   Robotics toolbo
-000040d0: 7820 666f 7220 5079 7468 6f6e 2e0a 0a5b  x for Python...[
-000040e0: 5b50 6170 6572 5d28 6874 7470 733a 2f2f  [Paper](https://
-000040f0: 6172 7869 762e 6f72 672f 6162 732f 3230  arxiv.org/abs/20
-00004100: 3032 2e31 3139 3031 295d 205b 5b50 726f  02.11901)] [[Pro
-00004110: 6a65 6374 2057 6562 7369 7465 5d28 6874  ject Website](ht
-00004120: 7470 733a 2f2f 6a68 6176 6c2e 6769 7468  tps://jhavl.gith
-00004130: 7562 2e69 6f2f 6d6d 632f 295d 205b 5b56  ub.io/mmc/)] [[V
-00004140: 6964 656f 5d28 6874 7470 733a 2f2f 796f  ideo](https://yo
-00004150: 7574 752e 6265 2f56 755f 7263 506c 6141  utu.be/Vu_rcPlaA
-00004160: 4449 295d 205b 5b43 6f64 6520 4578 616d  DI)] [[Code Exam
-00004170: 706c 655d 2868 7474 7073 3a2f 2f67 6974  ple](https://git
-00004180: 6875 622e 636f 6d2f 7065 7465 7263 6f72  hub.com/petercor
-00004190: 6b65 2f72 6f62 6f74 6963 732d 746f 6f6c  ke/robotics-tool
-000041a0: 626f 782d 7079 7468 6f6e 2f62 6c6f 622f  box-python/blob/
-000041b0: 6d61 7374 6572 2f72 6f62 6f74 6963 7374  master/roboticst
-000041c0: 6f6f 6c62 6f78 2f65 7861 6d70 6c65 732f  oolbox/examples/
-000041d0: 6d6d 632e 7079 295d 0a0a 3c70 3e0a 2020  mmc.py)]..<p>.  
-000041e0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-000041f0: 2f79 6f75 7475 2e62 652f 5675 5f72 6350  /youtu.be/Vu_rcP
-00004200: 6c61 4144 4922 3e0a 2020 2020 3c69 6d67  laADI">.    <img
-00004210: 2073 7263 3d22 6874 7470 733a 2f2f 6769   src="https://gi
-00004220: 7468 7562 2e63 6f6d 2f70 6574 6572 636f  thub.com/peterco
-00004230: 726b 652f 726f 626f 7469 6373 2d74 6f6f  rke/robotics-too
-00004240: 6c62 6f78 2d70 7974 686f 6e2f 7261 772f  lbox-python/raw/
-00004250: 6d61 7374 6572 2f64 6f63 732f 6669 6773  master/docs/figs
-00004260: 2f6d 6d63 5f79 6f75 7475 6265 2e70 6e67  /mmc_youtube.png
-00004270: 2220 7769 6474 683d 2235 3630 223e 0a20  " width="560">. 
-00004280: 203c 2f61 3e0a 3c2f 703e 0a0a 3c62 723e   </a>.</p>..<br>
-00004290: 0a0a 3c62 723e 0a0a 3c61 2069 643d 2736  ..<br>..<a id='6
-000042a0: 273e 3c2f 613e 0a0a 2323 2054 6f6f 6c62  '></a>..## Toolb
-000042b0: 6f78 2049 4352 4120 5061 7065 7220 616e  ox ICRA Paper an
-000042c0: 6420 4369 7461 7469 6f6e 2049 6e66 6f0a  d Citation Info.
-000042d0: 0a43 6865 636b 206f 7574 206f 7572 2049  .Check out our I
-000042e0: 4352 4120 3230 3231 2070 6170 6572 206f  CRA 2021 paper o
-000042f0: 6e20 5b49 4545 4520 5870 6c6f 7265 5d28  n [IEEE Xplore](
-00004300: 6874 7470 733a 2f2f 6965 6565 7870 6c6f  https://ieeexplo
-00004310: 7265 2e69 6565 652e 6f72 672f 646f 6375  re.ieee.org/docu
-00004320: 6d65 6e74 2f39 3536 3133 3636 2920 6f72  ment/9561366) or
-00004330: 2067 6574 2074 6865 2050 4446 2066 726f   get the PDF fro
-00004340: 6d20 5b50 6574 6572 2773 2077 6562 7369  m [Peter's websi
-00004350: 7465 5d28 6874 7470 733a 2f2f 6269 742e  te](https://bit.
-00004360: 6c79 2f33 4368 6379 4e70 292e 0a0a 4966  ly/3ChcyNp)...If
-00004370: 2074 6865 2074 6f6f 6c62 6f78 2068 656c   the toolbox hel
-00004380: 7065 6420 796f 7520 696e 2079 6f75 7220  ped you in your 
-00004390: 7265 7365 6172 6368 2c20 706c 6561 7365  research, please
-000043a0: 2063 6974 650a 0a60 6060 0a40 696e 7072   cite..```.@inpr
-000043b0: 6f63 6565 6469 6e67 737b 7274 622c 0a20  oceedings{rtb,. 
-000043c0: 2074 6974 6c65 3d7b 4e6f 7420 796f 7572   title={Not your
-000043d0: 2067 7261 6e64 6d6f 7468 6572 e280 9973   grandmother...s
-000043e0: 2074 6f6f 6c62 6f78 2d2d 7468 6520 526f   toolbox--the Ro
-000043f0: 626f 7469 6373 2054 6f6f 6c62 6f78 2072  botics Toolbox r
-00004400: 6569 6e76 656e 7465 6420 666f 7220 5079  einvented for Py
-00004410: 7468 6f6e 7d2c 0a20 2061 7574 686f 723d  thon},.  author=
-00004420: 7b43 6f72 6b65 2c20 5065 7465 7220 616e  {Corke, Peter an
-00004430: 6420 4861 7669 6c61 6e64 2c20 4a65 7373  d Haviland, Jess
-00004440: 657d 2c0a 2020 626f 6f6b 7469 746c 653d  e},.  booktitle=
-00004450: 7b32 3032 3120 4945 4545 2049 6e74 6572  {2021 IEEE Inter
-00004460: 6e61 7469 6f6e 616c 2043 6f6e 6665 7265  national Confere
-00004470: 6e63 6520 6f6e 2052 6f62 6f74 6963 7320  nce on Robotics 
-00004480: 616e 6420 4175 746f 6d61 7469 6f6e 2028  and Automation (
-00004490: 4943 5241 297d 2c0a 2020 7061 6765 733d  ICRA)},.  pages=
-000044a0: 7b31 3133 3537 2d2d 3131 3336 337d 2c0a  {11357--11363},.
-000044b0: 2020 7965 6172 3d7b 3230 3231 7d2c 0a20    year={2021},. 
-000044c0: 206f 7267 616e 697a 6174 696f 6e3d 7b49   organization={I
-000044d0: 4545 457d 0a7d 0a60 6060 0a0a 3c62 723e  EEE}.}.```..<br>
-000044e0: 0a0a 3c61 2069 643d 2737 273e 3c2f 613e  ..<a id='7'></a>
-000044f0: 0a0a 2323 2055 7369 6e67 2074 6865 2054  ..## Using the T
-00004500: 6f6f 6c62 6f78 2069 6e20 796f 7572 204f  oolbox in your O
-00004510: 7065 6e20 536f 7572 6365 2043 6f64 653f  pen Source Code?
-00004520: 0a0a 4966 2079 6f75 2061 7265 2075 7369  ..If you are usi
-00004530: 6e67 2074 6865 2054 6f6f 6c62 6f78 2069  ng the Toolbox i
-00004540: 6e20 796f 7572 206f 7065 6e20 736f 7572  n your open sour
-00004550: 6365 2063 6f64 652c 2066 6565 6c20 6672  ce code, feel fr
-00004560: 6565 2074 6f20 6164 6420 6f75 7220 6261  ee to add our ba
-00004570: 6467 6520 746f 2079 6f75 7220 7265 6164  dge to your read
-00004580: 6d65 210a 0a46 6f72 2074 6865 2070 6f77  me!..For the pow
-00004590: 6572 6564 2062 7920 726f 626f 7469 6373  ered by robotics
-000045a0: 2074 6f6f 6c62 6f78 2062 6164 6765 0a0a   toolbox badge..
-000045b0: 5b21 5b50 6f77 6572 6564 2062 7920 7468  [![Powered by th
-000045c0: 6520 526f 626f 7469 6373 2054 6f6f 6c62  e Robotics Toolb
-000045d0: 6f78 5d28 6874 7470 733a 2f2f 7261 772e  ox](https://raw.
-000045e0: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
-000045f0: 742e 636f 6d2f 7065 7465 7263 6f72 6b65  t.com/petercorke
-00004600: 2f72 6f62 6f74 6963 732d 746f 6f6c 626f  /robotics-toolbo
-00004610: 782d 7079 7468 6f6e 2f6d 6173 7465 722f  x-python/master/
-00004620: 2e67 6974 6875 622f 7376 672f 7274 625f  .github/svg/rtb_
-00004630: 706f 7765 7265 642e 6d69 6e2e 7376 6729  powered.min.svg)
-00004640: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00004650: 2e63 6f6d 2f70 6574 6572 636f 726b 652f  .com/petercorke/
-00004660: 726f 626f 7469 6373 2d74 6f6f 6c62 6f78  robotics-toolbox
-00004670: 2d70 7974 686f 6e29 0a0a 636f 7079 2074  -python)..copy t
-00004680: 6865 2066 6f6c 6c6f 7769 6e67 0a0a 6060  he following..``
-00004690: 600a 5b21 5b50 6f77 6572 6564 2062 7920  `.[![Powered by 
-000046a0: 7468 6520 526f 626f 7469 6373 2054 6f6f  the Robotics Too
-000046b0: 6c62 6f78 5d28 6874 7470 733a 2f2f 7261  lbox](https://ra
-000046c0: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-000046d0: 656e 742e 636f 6d2f 7065 7465 7263 6f72  ent.com/petercor
-000046e0: 6b65 2f72 6f62 6f74 6963 732d 746f 6f6c  ke/robotics-tool
-000046f0: 626f 782d 7079 7468 6f6e 2f6d 6173 7465  box-python/maste
-00004700: 722f 2e67 6974 6875 622f 7376 672f 7274  r/.github/svg/rt
-00004710: 625f 706f 7765 7265 642e 6d69 6e2e 7376  b_powered.min.sv
-00004720: 6729 5d28 6874 7470 733a 2f2f 6769 7468  g)](https://gith
-00004730: 7562 2e63 6f6d 2f70 6574 6572 636f 726b  ub.com/petercork
-00004740: 652f 726f 626f 7469 6373 2d74 6f6f 6c62  e/robotics-toolb
-00004750: 6f78 2d70 7974 686f 6e29 0a60 6060 0a0a  ox-python).```..
-00004760: 466f 7220 7468 6520 706f 7765 7265 6420  For the powered 
-00004770: 6279 2070 7974 686f 6e20 726f 626f 7469  by python roboti
-00004780: 6373 2062 6164 6765 0a0a 5b21 5b50 6f77  cs badge..[![Pow
-00004790: 6572 6564 2062 7920 5079 7468 6f6e 2052  ered by Python R
-000047a0: 6f62 6f74 6963 735d 2868 7474 7073 3a2f  obotics](https:/
-000047b0: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
-000047c0: 6f6e 7465 6e74 2e63 6f6d 2f70 6574 6572  ontent.com/peter
-000047d0: 636f 726b 652f 726f 626f 7469 6373 2d74  corke/robotics-t
-000047e0: 6f6f 6c62 6f78 2d70 7974 686f 6e2f 6d61  oolbox-python/ma
-000047f0: 7374 6572 2f2e 6769 7468 7562 2f73 7667  ster/.github/svg
-00004800: 2f70 725f 706f 7765 7265 642e 6d69 6e2e  /pr_powered.min.
-00004810: 7376 6729 5d28 6874 7470 733a 2f2f 6769  svg)](https://gi
-00004820: 7468 7562 2e63 6f6d 2f70 6574 6572 636f  thub.com/peterco
-00004830: 726b 652f 726f 626f 7469 6373 2d74 6f6f  rke/robotics-too
-00004840: 6c62 6f78 2d70 7974 686f 6e29 0a0a 636f  lbox-python)..co
-00004850: 7079 2074 6865 2066 6f6c 6c6f 7769 6e67  py the following
-00004860: 0a0a 6060 600a 5b21 5b50 6f77 6572 6564  ..```.[![Powered
-00004870: 2062 7920 5079 7468 6f6e 2052 6f62 6f74   by Python Robot
-00004880: 6963 735d 2868 7474 7073 3a2f 2f72 6177  ics](https://raw
-00004890: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
-000048a0: 6e74 2e63 6f6d 2f70 6574 6572 636f 726b  nt.com/petercork
-000048b0: 652f 726f 626f 7469 6373 2d74 6f6f 6c62  e/robotics-toolb
-000048c0: 6f78 2d70 7974 686f 6e2f 6d61 7374 6572  ox-python/master
-000048d0: 2f2e 6769 7468 7562 2f73 7667 2f70 725f  /.github/svg/pr_
-000048e0: 706f 7765 7265 642e 6d69 6e2e 7376 6729  powered.min.svg)
-000048f0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00004900: 2e63 6f6d 2f70 6574 6572 636f 726b 652f  .com/petercorke/
-00004910: 726f 626f 7469 6373 2d74 6f6f 6c62 6f78  robotics-toolbox
-00004920: 2d70 7974 686f 6e29 0a60 6060 0a0a 3c62  -python).```..<b
-00004930: 723e 0a0a 3c61 2069 643d 2738 273e 3c2f  r>..<a id='8'></
-00004940: 613e 0a0a 2323 2043 6f6d 6d6f 6e20 4973  a>..## Common Is
-00004950: 7375 6573 2061 6e64 2053 6f6c 7574 696f  sues and Solutio
-00004960: 6e73 0a0a 5365 6520 7468 6520 636f 6d6d  ns..See the comm
-00004970: 6f6e 2069 7373 7565 7320 7769 7468 2066  on issues with f
-00004980: 6978 6573 205b 6865 7265 5d28 6874 7470  ixes [here](http
-00004990: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
-000049a0: 6574 6572 636f 726b 652f 726f 626f 7469  etercorke/roboti
-000049b0: 6373 2d74 6f6f 6c62 6f78 2d70 7974 686f  cs-toolbox-pytho
-000049c0: 6e2f 7769 6b69 2f43 6f6d 6d6f 6e2d 4973  n/wiki/Common-Is
-000049d0: 7375 6573 292e 0a                        sues)..
+00000910: 726b 646f 776e 0a4c 6963 656e 7365 2d46  rkdown.License-F
+00000920: 696c 653a 204c 4943 454e 5345 0a52 6571  ile: LICENSE.Req
+00000930: 7569 7265 732d 4469 7374 3a20 6e75 6d70  uires-Dist: nump
+00000940: 793e 3d31 2e31 372e 340a 5265 7175 6972  y>=1.17.4.Requir
+00000950: 6573 2d44 6973 743a 2073 7061 7469 616c  es-Dist: spatial
+00000960: 6d61 7468 2d70 7974 686f 6e3e 3d31 2e31  math-python>=1.1
+00000970: 2e35 0a52 6571 7569 7265 732d 4469 7374  .5.Requires-Dist
+00000980: 3a20 7370 6174 6961 6c67 656f 6d65 7472  : spatialgeometr
+00000990: 793e 3d31 2e30 2e30 0a52 6571 7569 7265  y>=1.0.0.Require
+000009a0: 732d 4469 7374 3a20 7067 7261 7068 2d70  s-Dist: pgraph-p
+000009b0: 7974 686f 6e0a 5265 7175 6972 6573 2d44  ython.Requires-D
+000009c0: 6973 743a 2073 6369 7079 0a52 6571 7569  ist: scipy.Requi
+000009d0: 7265 732d 4469 7374 3a20 6d61 7470 6c6f  res-Dist: matplo
+000009e0: 746c 6962 0a52 6571 7569 7265 732d 4469  tlib.Requires-Di
+000009f0: 7374 3a20 616e 7369 7461 626c 650a 5265  st: ansitable.Re
+00000a00: 7175 6972 6573 2d44 6973 743a 2073 7769  quires-Dist: swi
+00000a10: 6674 2d73 696d 3e3d 312e 302e 300a 5265  ft-sim>=1.0.0.Re
+00000a20: 7175 6972 6573 2d44 6973 743a 2072 7462  quires-Dist: rtb
+00000a30: 2d64 6174 610a 5265 7175 6972 6573 2d44  -data.Requires-D
+00000a40: 6973 743a 2070 726f 6772 6573 730a 5265  ist: progress.Re
+00000a50: 7175 6972 6573 2d44 6973 743a 2074 7970  quires-Dist: typ
+00000a60: 696e 675f 6578 7465 6e73 696f 6e73 0a50  ing_extensions.P
+00000a70: 726f 7669 6465 732d 4578 7472 613a 2063  rovides-Extra: c
+00000a80: 6f6c 6c69 7369 6f6e 0a52 6571 7569 7265  ollision.Require
+00000a90: 732d 4469 7374 3a20 7079 6275 6c6c 6574  s-Dist: pybullet
+00000aa0: 3b20 6578 7472 6120 3d3d 2022 636f 6c6c  ; extra == "coll
+00000ab0: 6973 696f 6e22 0a50 726f 7669 6465 732d  ision".Provides-
+00000ac0: 4578 7472 613a 2064 6576 0a52 6571 7569  Extra: dev.Requi
+00000ad0: 7265 732d 4469 7374 3a20 626c 6163 6b3b  res-Dist: black;
+00000ae0: 2065 7874 7261 203d 3d20 2264 6576 220a   extra == "dev".
+00000af0: 5265 7175 6972 6573 2d44 6973 743a 2070  Requires-Dist: p
+00000b00: 7974 6573 743b 2065 7874 7261 203d 3d20  ytest; extra == 
+00000b10: 2264 6576 220a 5265 7175 6972 6573 2d44  "dev".Requires-D
+00000b20: 6973 743a 2070 7974 6573 742d 636f 763b  ist: pytest-cov;
+00000b30: 2065 7874 7261 203d 3d20 2264 6576 220a   extra == "dev".
+00000b40: 5265 7175 6972 6573 2d44 6973 743a 2066  Requires-Dist: f
+00000b50: 6c61 6b65 383b 2065 7874 7261 203d 3d20  lake8; extra == 
+00000b60: 2264 6576 220a 5265 7175 6972 6573 2d44  "dev".Requires-D
+00000b70: 6973 743a 2070 7979 616d 6c3b 2065 7874  ist: pyyaml; ext
+00000b80: 7261 203d 3d20 2264 6576 220a 5265 7175  ra == "dev".Requ
+00000b90: 6972 6573 2d44 6973 743a 2073 796d 7079  ires-Dist: sympy
+00000ba0: 3b20 6578 7472 6120 3d3d 2022 6465 7622  ; extra == "dev"
+00000bb0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000bc0: 7170 736f 6c76 6572 733b 2065 7874 7261  qpsolvers; extra
+00000bd0: 203d 3d20 2264 6576 220a 5265 7175 6972   == "dev".Requir
+00000be0: 6573 2d44 6973 743a 2071 7561 6470 726f  es-Dist: quadpro
+00000bf0: 673b 2065 7874 7261 203d 3d20 2264 6576  g; extra == "dev
+00000c00: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+00000c10: 2070 7962 756c 6c65 743b 2065 7874 7261   pybullet; extra
+00000c20: 203d 3d20 2264 6576 220a 5265 7175 6972   == "dev".Requir
+00000c30: 6573 2d44 6973 743a 2062 6473 696d 3b20  es-Dist: bdsim; 
+00000c40: 6578 7472 6120 3d3d 2022 6465 7622 0a50  extra == "dev".P
+00000c50: 726f 7669 6465 732d 4578 7472 613a 2064  rovides-Extra: d
+00000c60: 6f63 730a 5265 7175 6972 6573 2d44 6973  ocs.Requires-Dis
+00000c70: 743a 2073 7068 696e 783b 2065 7874 7261  t: sphinx; extra
+00000c80: 203d 3d20 2264 6f63 7322 0a52 6571 7569   == "docs".Requi
+00000c90: 7265 732d 4469 7374 3a20 7370 6869 6e78  res-Dist: sphinx
+00000ca0: 5f72 7464 5f74 6865 6d65 3b20 6578 7472  _rtd_theme; extr
+00000cb0: 6120 3d3d 2022 646f 6373 220a 5265 7175  a == "docs".Requ
+00000cc0: 6972 6573 2d44 6973 743a 2073 7068 696e  ires-Dist: sphin
+00000cd0: 782d 6175 746f 7275 6e3b 2065 7874 7261  x-autorun; extra
+00000ce0: 203d 3d20 2264 6f63 7322 0a52 6571 7569   == "docs".Requi
+00000cf0: 7265 732d 4469 7374 3a20 7370 6869 6e78  res-Dist: sphinx
+00000d00: 5f61 7574 6f64 6f63 5f74 7970 6568 696e  _autodoc_typehin
+00000d10: 7473 3b20 6578 7472 6120 3d3d 2022 646f  ts; extra == "do
+00000d20: 6373 220a 5265 7175 6972 6573 2d44 6973  cs".Requires-Dis
+00000d30: 743a 2073 7068 696e 782d 6661 7669 636f  t: sphinx-favico
+00000d40: 6e3b 2065 7874 7261 203d 3d20 2264 6f63  n; extra == "doc
+00000d50: 7322 0a0a 2320 526f 626f 7469 6373 2054  s"..# Robotics T
+00000d60: 6f6f 6c62 6f78 2066 6f72 2050 7974 686f  oolbox for Pytho
+00000d70: 6e0a 0a5b 215b 4120 5079 7468 6f6e 2052  n..[![A Python R
+00000d80: 6f62 6f74 6963 7320 5061 636b 6167 655d  obotics Package]
+00000d90: 2868 7474 7073 3a2f 2f72 6177 2e67 6974  (https://raw.git
+00000da0: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+00000db0: 6f6d 2f70 6574 6572 636f 726b 652f 726f  om/petercorke/ro
+00000dc0: 626f 7469 6373 2d74 6f6f 6c62 6f78 2d70  botics-toolbox-p
+00000dd0: 7974 686f 6e2f 6d61 7374 6572 2f2e 6769  ython/master/.gi
+00000de0: 7468 7562 2f73 7667 2f70 795f 636f 6c6c  thub/svg/py_coll
+00000df0: 6563 7469 6f6e 2e6d 696e 2e73 7667 295d  ection.min.svg)]
+00000e00: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000e10: 636f 6d2f 7065 7465 7263 6f72 6b65 2f72  com/petercorke/r
+00000e20: 6f62 6f74 6963 732d 746f 6f6c 626f 782d  obotics-toolbox-
+00000e30: 7079 7468 6f6e 290a 5b21 5b50 6f77 6572  python).[![Power
+00000e40: 6564 2062 7920 5370 6174 6961 6c20 4d61  ed by Spatial Ma
+00000e50: 7468 735d 2868 7474 7073 3a2f 2f72 6177  ths](https://raw
+00000e60: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+00000e70: 6e74 2e63 6f6d 2f70 6574 6572 636f 726b  nt.com/petercork
+00000e80: 652f 7370 6174 6961 6c6d 6174 682d 7079  e/spatialmath-py
+00000e90: 7468 6f6e 2f6d 6173 7465 722f 2e67 6974  thon/master/.git
+00000ea0: 6875 622f 7376 672f 736d 5f70 6f77 6572  hub/svg/sm_power
+00000eb0: 6564 2e6d 696e 2e73 7667 295d 2868 7474  ed.min.svg)](htt
+00000ec0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000ed0: 7065 7465 7263 6f72 6b65 2f73 7061 7469  petercorke/spati
+00000ee0: 616c 6d61 7468 2d70 7974 686f 6e29 0a5b  almath-python).[
+00000ef0: 215b 5155 5420 4365 6e74 7265 2066 6f72  ![QUT Centre for
+00000f00: 2052 6f62 6f74 6963 7320 4f70 656e 2053   Robotics Open S
+00000f10: 6f75 7263 655d 2868 7474 7073 3a2f 2f67  ource](https://g
+00000f20: 6974 6875 622e 636f 6d2f 7163 722f 7163  ithub.com/qcr/qc
+00000f30: 722e 6769 7468 7562 2e69 6f2f 7261 772f  r.github.io/raw/
+00000f40: 6d61 7374 6572 2f6d 6973 632f 6261 6467  master/misc/badg
+00000f50: 652e 7376 6729 5d28 6874 7470 733a 2f2f  e.svg)](https://
+00000f60: 7163 722e 6769 7468 7562 2e69 6f29 0a0a  qcr.github.io)..
+00000f70: 5b21 5b50 7950 4920 7665 7273 696f 6e5d  [![PyPI version]
+00000f80: 2868 7474 7073 3a2f 2f62 6164 6765 2e66  (https://badge.f
+00000f90: 7572 792e 696f 2f70 792f 726f 626f 7469  ury.io/py/roboti
+00000fa0: 6373 746f 6f6c 626f 782d 7079 7468 6f6e  cstoolbox-python
+00000fb0: 2e73 7667 295d 2868 7474 7073 3a2f 2f62  .svg)](https://b
+00000fc0: 6164 6765 2e66 7572 792e 696f 2f70 792f  adge.fury.io/py/
+00000fd0: 726f 626f 7469 6373 746f 6f6c 626f 782d  roboticstoolbox-
+00000fe0: 7079 7468 6f6e 290a 5b21 5b41 6e61 636f  python).[![Anaco
+00000ff0: 6e64 6120 7665 7273 696f 6e5d 2868 7474  nda version](htt
+00001000: 7073 3a2f 2f61 6e61 636f 6e64 612e 6f72  ps://anaconda.or
+00001010: 672f 636f 6e64 612d 666f 7267 652f 726f  g/conda-forge/ro
+00001020: 626f 7469 6373 746f 6f6c 626f 782d 7079  boticstoolbox-py
+00001030: 7468 6f6e 2f62 6164 6765 732f 7665 7273  thon/badges/vers
+00001040: 696f 6e2e 7376 6729 5d28 6874 7470 733a  ion.svg)](https:
+00001050: 2f2f 616e 6163 6f6e 6461 2e6f 7267 2f63  //anaconda.org/c
+00001060: 6f6e 6461 2d66 6f72 6765 2f72 6f62 6f74  onda-forge/robot
+00001070: 6963 7374 6f6f 6c62 6f78 2d70 7974 686f  icstoolbox-pytho
+00001080: 6e29 0a21 5b50 7950 4920 2d20 5079 7468  n).![PyPI - Pyth
+00001090: 6f6e 2056 6572 7369 6f6e 5d28 6874 7470  on Version](http
+000010a0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+000010b0: 696f 2f70 7970 692f 7079 7665 7273 696f  io/pypi/pyversio
+000010c0: 6e73 2f72 6f62 6f74 6963 7374 6f6f 6c62  ns/roboticstoolb
+000010d0: 6f78 2d70 7974 686f 6e2e 7376 6729 0a0a  ox-python.svg)..
+000010e0: 5b21 5b42 7569 6c64 2053 7461 7475 735d  [![Build Status]
+000010f0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00001100: 636f 6d2f 7065 7465 7263 6f72 6b65 2f72  com/petercorke/r
+00001110: 6f62 6f74 6963 732d 746f 6f6c 626f 782d  obotics-toolbox-
+00001120: 7079 7468 6f6e 2f77 6f72 6b66 6c6f 7773  python/workflows
+00001130: 2f54 6573 742f 6261 6467 652e 7376 673f  /Test/badge.svg?
+00001140: 6272 616e 6368 3d6d 6173 7465 7229 5d28  branch=master)](
+00001150: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001160: 6f6d 2f70 6574 6572 636f 726b 652f 726f  om/petercorke/ro
+00001170: 626f 7469 6373 2d74 6f6f 6c62 6f78 2d70  botics-toolbox-p
+00001180: 7974 686f 6e2f 6163 7469 6f6e 733f 7175  ython/actions?qu
+00001190: 6572 793d 776f 726b 666c 6f77 2533 4154  ery=workflow%3AT
+000011a0: 6573 7429 0a5b 215b 436f 7665 7261 6765  est).[![Coverage
+000011b0: 5d28 6874 7470 733a 2f2f 636f 6465 636f  ](https://codeco
+000011c0: 762e 696f 2f67 682f 7065 7465 7263 6f72  v.io/gh/petercor
+000011d0: 6b65 2f72 6f62 6f74 6963 732d 746f 6f6c  ke/robotics-tool
+000011e0: 626f 782d 7079 7468 6f6e 2f62 7261 6e63  box-python/branc
+000011f0: 682f 6d61 7374 6572 2f67 7261 7068 2f62  h/master/graph/b
+00001200: 6164 6765 2e73 7667 295d 2868 7474 7073  adge.svg)](https
+00001210: 3a2f 2f63 6f64 6563 6f76 2e69 6f2f 6768  ://codecov.io/gh
+00001220: 2f70 6574 6572 636f 726b 652f 726f 626f  /petercorke/robo
+00001230: 7469 6373 2d74 6f6f 6c62 6f78 2d70 7974  tics-toolbox-pyt
+00001240: 686f 6e29 0a5b 215b 5079 5049 202d 2044  hon).[![PyPI - D
+00001250: 6f77 6e6c 6f61 6473 5d28 6874 7470 733a  ownloads](https:
+00001260: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00001270: 2f70 7970 692f 6477 2f72 6f62 6f74 6963  /pypi/dw/robotic
+00001280: 7374 6f6f 6c62 6f78 2d70 7974 686f 6e29  stoolbox-python)
+00001290: 5d28 6874 7470 733a 2f2f 7079 7069 7374  ](https://pypist
+000012a0: 6174 732e 6f72 672f 7061 636b 6167 6573  ats.org/packages
+000012b0: 2f72 6f62 6f74 6963 7374 6f6f 6c62 6f78  /roboticstoolbox
+000012c0: 2d70 7974 686f 6e29 0a5b 215b 4c69 6365  -python).[![Lice
+000012d0: 6e73 653a 204d 4954 5d28 6874 7470 733a  nse: MIT](https:
+000012e0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000012f0: 2f62 6164 6765 2f4c 6963 656e 7365 2d4d  /badge/License-M
+00001300: 4954 2d79 656c 6c6f 772e 7376 6729 5d28  IT-yellow.svg)](
+00001310: 6874 7470 733a 2f2f 6f70 656e 736f 7572  https://opensour
+00001320: 6365 2e6f 7267 2f6c 6963 656e 7365 732f  ce.org/licenses/
+00001330: 4d49 5429 0a0a 3c74 6162 6c65 2073 7479  MIT)..<table sty
+00001340: 6c65 3d22 626f 7264 6572 3a30 7078 223e  le="border:0px">
+00001350: 0a3c 7472 2073 7479 6c65 3d22 626f 7264  .<tr style="bord
+00001360: 6572 3a30 7078 223e 0a3c 7464 2073 7479  er:0px">.<td sty
+00001370: 6c65 3d22 626f 7264 6572 3a30 7078 223e  le="border:0px">
+00001380: 0a3c 696d 6720 7372 633d 2268 7474 7073  .<img src="https
+00001390: 3a2f 2f67 6974 6875 622e 636f 6d2f 7065  ://github.com/pe
+000013a0: 7465 7263 6f72 6b65 2f72 6f62 6f74 6963  tercorke/robotic
+000013b0: 732d 746f 6f6c 626f 782d 7079 7468 6f6e  s-toolbox-python
+000013c0: 2f72 6177 2f6d 6173 7465 722f 646f 6373  /raw/master/docs
+000013d0: 2f66 6967 732f 526f 6254 6f6f 6c42 6f78  /figs/RobToolBox
+000013e0: 5f52 6f75 6e64 4c6f 676f 422e 706e 6722  _RoundLogoB.png"
+000013f0: 2077 6964 7468 3d22 3230 3022 3e3c 2f74   width="200"></t
+00001400: 643e 0a3c 7464 2073 7479 6c65 3d22 626f  d>.<td style="bo
+00001410: 7264 6572 3a30 7078 223e 0a41 2050 7974  rder:0px">.A Pyt
+00001420: 686f 6e20 696d 706c 656d 656e 7461 7469  hon implementati
+00001430: 6f6e 206f 6620 7468 6520 3c61 2068 7265  on of the <a hre
+00001440: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
+00001450: 622e 636f 6d2f 7065 7465 7263 6f72 6b65  b.com/petercorke
+00001460: 2f72 6f62 6f74 6963 732d 746f 6f6c 626f  /robotics-toolbo
+00001470: 782d 6d61 746c 6162 223e 526f 626f 7469  x-matlab">Roboti
+00001480: 6373 2054 6f6f 6c62 6f78 2066 6f72 204d  cs Toolbox for M
+00001490: 4154 4c41 423c 7375 703e 2672 6567 3b3c  ATLAB<sup>&reg;<
+000014a0: 2f73 7570 3e3c 2f61 3e0a 3c75 6c3e 0a3c  /sup></a>.<ul>.<
+000014b0: 6c69 3e3c 6120 6872 6566 3d22 6874 7470  li><a href="http
+000014c0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
+000014d0: 6574 6572 636f 726b 652f 726f 626f 7469  etercorke/roboti
+000014e0: 6373 2d74 6f6f 6c62 6f78 2d70 7974 686f  cs-toolbox-pytho
+000014f0: 6e22 3e47 6974 4875 6220 7265 706f 7369  n">GitHub reposi
+00001500: 746f 7279 203c 2f61 3e3c 2f6c 693e 0a3c  tory </a></li>.<
+00001510: 6c69 3e3c 6120 6872 6566 3d22 6874 7470  li><a href="http
+00001520: 733a 2f2f 7065 7465 7263 6f72 6b65 2e67  s://petercorke.g
+00001530: 6974 6875 622e 696f 2f72 6f62 6f74 6963  ithub.io/robotic
+00001540: 732d 746f 6f6c 626f 782d 7079 7468 6f6e  s-toolbox-python
+00001550: 223e 446f 6375 6d65 6e74 6174 696f 6e3c  ">Documentation<
+00001560: 2f61 3e3c 2f6c 693e 0a3c 6c69 3e3c 6120  /a></li>.<li><a 
+00001570: 6872 6566 3d22 2336 223e 4943 5241 2050  href="#6">ICRA P
+00001580: 6170 6572 3c2f 613e 3c2f 6c69 3e0a 3c6c  aper</a></li>.<l
+00001590: 693e 3c61 2068 7265 663d 2268 7474 7073  i><a href="https
+000015a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7065  ://github.com/pe
+000015b0: 7465 7263 6f72 6b65 2f72 6f62 6f74 6963  tercorke/robotic
+000015c0: 732d 746f 6f6c 626f 782d 7079 7468 6f6e  s-toolbox-python
+000015d0: 2f77 696b 6922 3e57 696b 6920 2865 7861  /wiki">Wiki (exa
+000015e0: 6d70 6c65 7320 616e 6420 6465 7461 696c  mples and detail
+000015f0: 7329 3c2f 613e 3c2f 6c69 3e0a 3c2f 756c  s)</a></li>.</ul
+00001600: 3e0a 3c2f 7464 3e0a 3c2f 7472 3e0a 3c2f  >.</td>.</tr>.</
+00001610: 7461 626c 653e 0a0a 3c21 2d2d 203c 6272  table>..<!-- <br
+00001620: 3e20 2d2d 3e0a 0a23 2320 436f 6e74 656e  > -->..## Conten
+00001630: 7473 0a0a 2d20 5b53 796e 6f70 7369 735d  ts..- [Synopsis]
+00001640: 2823 3129 0a2d 205b 4765 7474 696e 6720  (#1).- [Getting 
+00001650: 676f 696e 675d 2823 3229 0a2d 205b 5475  going](#2).- [Tu
+00001660: 746f 7269 616c 735d 2823 3329 0a2d 205b  torials](#3).- [
+00001670: 436f 6465 2045 7861 6d70 6c65 735d 2823  Code Examples](#
+00001680: 3429 0a2d 205b 546f 6f6c 626f 7820 5265  4).- [Toolbox Re
+00001690: 7365 6172 6368 2041 7070 6c69 6361 7469  search Applicati
+000016a0: 6f6e 735d 2823 3529 0a2d 205b 546f 6f6c  ons](#5).- [Tool
+000016b0: 626f 7820 4943 5241 2050 6170 6572 2061  box ICRA Paper a
+000016c0: 6e64 2043 6974 6174 696f 6e20 496e 666f  nd Citation Info
+000016d0: 5d28 2336 290a 2d20 5b55 7369 6e67 2074  ](#6).- [Using t
+000016e0: 6865 2054 6f6f 6c62 6f78 2069 6e20 796f  he Toolbox in yo
+000016f0: 7572 204f 7065 6e20 536f 7572 6365 2043  ur Open Source C
+00001700: 6f64 653f 5d28 2337 290a 2d20 5b43 6f6d  ode?](#7).- [Com
+00001710: 6d6f 6e20 4973 7375 6573 2061 6e64 2053  mon Issues and S
+00001720: 6f6c 7574 696f 6e73 5d28 2338 290a 0a3c  olutions](#8)..<
+00001730: 6272 3e0a 0a3c 6120 6964 3d27 3127 3e3c  br>..<a id='1'><
+00001740: 2f61 3e0a 0a23 2320 5379 6e6f 7073 6973  /a>..## Synopsis
+00001750: 0a0a 5468 6973 2074 6f6f 6c62 6f78 2062  ..This toolbox b
+00001760: 7269 6e67 7320 726f 626f 7469 6373 2d73  rings robotics-s
+00001770: 7065 6369 6669 6320 6675 6e63 7469 6f6e  pecific function
+00001780: 616c 6974 7920 746f 2050 7974 686f 6e2c  ality to Python,
+00001790: 2061 6e64 206c 6576 6572 6167 6573 0a50   and leverages.P
+000017a0: 7974 686f 6e27 7320 6164 7661 6e74 6167  ython's advantag
+000017b0: 6573 206f 6620 706f 7274 6162 696c 6974  es of portabilit
+000017c0: 792c 2075 6269 7175 6974 7920 616e 6420  y, ubiquity and 
+000017d0: 7375 7070 6f72 742c 2061 6e64 2074 6865  support, and the
+000017e0: 2063 6170 6162 696c 6974 7920 6f66 0a74   capability of.t
+000017f0: 6865 206f 7065 6e2d 736f 7572 6365 2065  he open-source e
+00001800: 636f 7379 7374 656d 2066 6f72 206c 696e  cosystem for lin
+00001810: 6561 7220 616c 6765 6272 6120 286e 756d  ear algebra (num
+00001820: 7079 2c20 7363 6970 7929 2c20 6772 6170  py, scipy), grap
+00001830: 6869 6373 0a28 6d61 7470 6c6f 746c 6962  hics.(matplotlib
+00001840: 2c20 7468 7265 652e 6a73 2c20 5765 6247  , three.js, WebG
+00001850: 4c29 2c20 696e 7465 7261 6374 6976 6520  L), interactive 
+00001860: 6465 7665 6c6f 706d 656e 7420 286a 7570  development (jup
+00001870: 7974 6572 2c20 6a75 7079 7465 726c 6162  yter, jupyterlab
+00001880: 2c0a 6d79 6269 6e64 6572 2e6f 7267 292c  ,.mybinder.org),
+00001890: 2061 6e64 2064 6f63 756d 656e 7461 7469   and documentati
+000018a0: 6f6e 2028 7370 6869 6e78 292e 0a0a 5468  on (sphinx)...Th
+000018b0: 6520 546f 6f6c 626f 7820 7072 6f76 6964  e Toolbox provid
+000018c0: 6573 2074 6f6f 6c73 2066 6f72 2072 6570  es tools for rep
+000018d0: 7265 7365 6e74 696e 6720 7468 6520 6b69  resenting the ki
+000018e0: 6e65 6d61 7469 6373 2061 6e64 2064 796e  nematics and dyn
+000018f0: 616d 6963 7320 6f66 0a73 6572 6961 6c2d  amics of.serial-
+00001900: 6c69 6e6b 206d 616e 6970 756c 6174 6f72  link manipulator
+00001910: 7320 2d20 796f 7520 6361 6e20 6561 7369  s - you can easi
+00001920: 6c79 2063 7265 6174 6520 796f 7572 206f  ly create your o
+00001930: 776e 2069 6e20 4465 6e61 7669 742d 4861  wn in Denavit-Ha
+00001940: 7274 656e 6265 7267 0a66 6f72 6d2c 2069  rtenberg.form, i
+00001950: 6d70 6f72 7420 6120 5552 4446 2066 696c  mport a URDF fil
+00001960: 652c 206f 7220 7573 6520 6f76 6572 2033  e, or use over 3
+00001970: 3020 7375 7070 6c69 6564 206d 6f64 656c  0 supplied model
+00001980: 7320 666f 7220 7765 6c6c 2d6b 6e6f 776e  s for well-known
+00001990: 0a63 6f6e 7465 6d70 6f72 6172 7920 726f  .contemporary ro
+000019a0: 626f 7473 2066 726f 6d20 4672 616e 6b61  bots from Franka
+000019b0: 2d45 6d69 6b61 2c20 4b69 6e6f 7661 2c20  -Emika, Kinova, 
+000019c0: 556e 6976 6572 7361 6c20 526f 626f 7469  Universal Roboti
+000019d0: 6373 2c20 5265 7468 696e 6b20 6173 0a77  cs, Rethink as.w
+000019e0: 656c 6c20 6173 2063 6c61 7373 6963 616c  ell as classical
+000019f0: 2072 6f62 6f74 7320 7375 6368 2061 7320   robots such as 
+00001a00: 7468 6520 5075 6d61 2035 3630 2061 6e64  the Puma 560 and
+00001a10: 2074 6865 2053 7461 6e66 6f72 6420 6172   the Stanford ar
+00001a20: 6d2e 0a0a 5468 6520 546f 6f6c 626f 7820  m...The Toolbox 
+00001a30: 636f 6e74 6169 6e73 2066 6173 7420 696d  contains fast im
+00001a40: 706c 656d 656e 7461 7469 6f6e 7320 6f66  plementations of
+00001a50: 206b 696e 656d 6174 6963 206f 7065 7261   kinematic opera
+00001a60: 7469 6f6e 732e 2054 6865 2066 6f72 7761  tions. The forwa
+00001a70: 7264 0a6b 696e 656d 6174 6963 7320 616e  rd.kinematics an
+00001a80: 6420 7468 6520 6d61 6e69 7075 6c61 746f  d the manipulato
+00001a90: 7220 4a61 636f 6269 616e 2063 616e 2062  r Jacobian can b
+00001aa0: 6520 636f 6d70 7574 6564 2069 6e20 6c65  e computed in le
+00001ab0: 7373 2074 6861 6e20 3120 6d69 6372 6f73  ss than 1 micros
+00001ac0: 6563 6f6e 640a 7768 696c 6520 6e75 6d65  econd.while nume
+00001ad0: 7269 6361 6c20 696e 7665 7273 6520 6b69  rical inverse ki
+00001ae0: 6e65 6d61 7469 6373 2063 616e 2062 6520  nematics can be 
+00001af0: 736f 6c76 6564 2069 6e20 6173 206c 6974  solved in as lit
+00001b00: 746c 6520 6173 2034 206d 6963 726f 7365  tle as 4 microse
+00001b10: 636f 6e64 732e 0a0a 5468 6520 746f 6f6c  conds...The tool
+00001b20: 626f 7820 616c 736f 2073 7570 706f 7274  box also support
+00001b30: 7320 6d6f 6269 6c65 2072 6f62 6f74 7320  s mobile robots 
+00001b40: 7769 7468 2066 756e 6374 696f 6e73 2066  with functions f
+00001b50: 6f72 2072 6f62 6f74 206d 6f74 696f 6e20  or robot motion 
+00001b60: 6d6f 6465 6c73 0a28 756e 6963 7963 6c65  models.(unicycle
+00001b70: 2c20 6269 6379 636c 6529 2c20 7061 7468  , bicycle), path
+00001b80: 2070 6c61 6e6e 696e 6720 616c 676f 7269   planning algori
+00001b90: 7468 6d73 2028 6275 672c 2064 6973 7461  thms (bug, dista
+00001ba0: 6e63 6520 7472 616e 7366 6f72 6d2c 2044  nce transform, D
+00001bb0: 5c2a 2c0a 5052 4d29 2c20 6b69 6e6f 6479  \*,.PRM), kinody
+00001bc0: 6e61 6d69 6320 706c 616e 6e69 6e67 2028  namic planning (
+00001bd0: 6c61 7474 6963 652c 2052 5254 292c 206c  lattice, RRT), l
+00001be0: 6f63 616c 697a 6174 696f 6e20 2845 4b46  ocalization (EKF
+00001bf0: 2c20 7061 7274 6963 6c65 2066 696c 7465  , particle filte
+00001c00: 7229 2c0a 6d61 7020 6275 696c 6469 6e67  r),.map building
+00001c10: 2028 454b 4629 2061 6e64 2073 696d 756c   (EKF) and simul
+00001c20: 7461 6e65 6f75 7320 6c6f 6361 6c69 7a61  taneous localiza
+00001c30: 7469 6f6e 2061 6e64 206d 6170 7069 6e67  tion and mapping
+00001c40: 2028 454b 4629 2e0a 0a54 6865 2054 6f6f   (EKF)...The Too
+00001c50: 6c62 6f78 2070 726f 7669 6465 733a 0a0a  lbox provides:..
+00001c60: 2d20 636f 6465 2074 6861 7420 6973 206d  - code that is m
+00001c70: 6174 7572 6520 616e 6420 7072 6f76 6964  ature and provid
+00001c80: 6573 2061 2070 6f69 6e74 206f 6620 636f  es a point of co
+00001c90: 6d70 6172 6973 6f6e 2066 6f72 206f 7468  mparison for oth
+00001ca0: 6572 0a20 2069 6d70 6c65 6d65 6e74 6174  er.  implementat
+00001cb0: 696f 6e73 206f 6620 7468 6520 7361 6d65  ions of the same
+00001cc0: 2061 6c67 6f72 6974 686d 733b 0a2d 2072   algorithms;.- r
+00001cd0: 6f75 7469 6e65 7320 7768 6963 6820 6172  outines which ar
+00001ce0: 6520 6765 6e65 7261 6c6c 7920 7772 6974  e generally writ
+00001cf0: 7465 6e20 696e 2061 2073 7472 6169 6768  ten in a straigh
+00001d00: 7466 6f72 7761 7264 206d 616e 6e65 7220  tforward manner 
+00001d10: 7768 6963 680a 2020 616c 6c6f 7773 2066  which.  allows f
+00001d20: 6f72 2065 6173 7920 756e 6465 7273 7461  or easy understa
+00001d30: 6e64 696e 672c 2070 6572 6861 7073 2061  nding, perhaps a
+00001d40: 7420 7468 6520 6578 7065 6e73 6520 6f66  t the expense of
+00001d50: 2063 6f6d 7075 7461 7469 6f6e 616c 0a20   computational. 
+00001d60: 2065 6666 6963 6965 6e63 793b 0a2d 2073   efficiency;.- s
+00001d70: 6f75 7263 6520 636f 6465 2077 6869 6368  ource code which
+00001d80: 2063 616e 2062 6520 7265 6164 2066 6f72   can be read for
+00001d90: 206c 6561 726e 696e 6720 616e 6420 7465   learning and te
+00001da0: 6163 6869 6e67 3b0a 2d20 6261 636b 7761  aching;.- backwa
+00001db0: 7264 2063 6f6d 7061 7461 6269 6c69 7479  rd compatability
+00001dc0: 2077 6974 6820 7468 6520 526f 626f 7469   with the Roboti
+00001dd0: 6373 2054 6f6f 6c62 6f78 2066 6f72 204d  cs Toolbox for M
+00001de0: 4154 4c41 420a 0a54 6865 2054 6f6f 6c62  ATLAB..The Toolb
+00001df0: 6f78 206c 6576 6572 6167 6573 2074 6865  ox leverages the
+00001e00: 205b 5370 6174 6961 6c20 4d61 7468 7320   [Spatial Maths 
+00001e10: 546f 6f6c 626f 7820 666f 7220 5079 7468  Toolbox for Pyth
+00001e20: 6f6e 5d28 6874 7470 733a 2f2f 6769 7468  on](https://gith
+00001e30: 7562 2e63 6f6d 2f70 6574 6572 636f 726b  ub.com/petercork
+00001e40: 652f 7370 6174 6961 6c6d 6174 682d 7079  e/spatialmath-py
+00001e50: 7468 6f6e 2920 746f 0a70 726f 7669 6465  thon) to.provide
+00001e60: 2073 7570 706f 7274 2066 6f72 2064 6174   support for dat
+00001e70: 6120 7479 7065 7320 7375 6368 2061 7320  a types such as 
+00001e80: 534f 286e 2920 616e 6420 5345 286e 2920  SO(n) and SE(n) 
+00001e90: 6d61 7472 6963 6573 2c20 7175 6174 6572  matrices, quater
+00001ea0: 6e69 6f6e 732c 2074 7769 7374 7320 616e  nions, twists an
+00001eb0: 6420 7370 6174 6961 6c20 7665 6374 6f72  d spatial vector
+00001ec0: 732e 0a0a 3c62 723e 0a0a 3c61 2069 643d  s...<br>..<a id=
+00001ed0: 2732 273e 3c2f 613e 0a0a 2323 2047 6574  '2'></a>..## Get
+00001ee0: 7469 6e67 2067 6f69 6e67 0a0a 596f 7520  ting going..You 
+00001ef0: 7769 6c6c 206e 6565 6420 5079 7468 6f6e  will need Python
+00001f00: 203e 3d20 332e 360a 0a23 2323 2055 7369   >= 3.6..### Usi
+00001f10: 6e67 2070 6970 0a0a 496e 7374 616c 6c20  ng pip..Install 
+00001f20: 6120 736e 6170 7368 6f74 2066 726f 6d20  a snapshot from 
+00001f30: 5079 5049 0a0a 6060 6073 6865 6c6c 2073  PyPI..```shell s
+00001f40: 6372 6970 740a 7069 7033 2069 6e73 7461  cript.pip3 insta
+00001f50: 6c6c 2072 6f62 6f74 6963 7374 6f6f 6c62  ll roboticstoolb
+00001f60: 6f78 2d70 7974 686f 6e0a 6060 600a 0a41  ox-python.```..A
+00001f70: 7661 696c 6162 6c65 206f 7074 696f 6e73  vailable options
+00001f80: 2061 7265 3a0a 0a2d 2060 636f 6c6c 6973   are:..- `collis
+00001f90: 696f 6e60 2069 6e73 7461 6c6c 2063 6f6c  ion` install col
+00001fa0: 6c69 7369 6f6e 2063 6865 636b 696e 6720  lision checking 
+00001fb0: 7769 7468 205b 7079 6275 6c6c 6574 5d28  with [pybullet](
+00001fc0: 6874 7470 733a 2f2f 7079 6275 6c6c 6574  https://pybullet
+00001fd0: 2e6f 7267 290a 0a50 7574 2074 6865 206f  .org)..Put the o
+00001fe0: 7074 696f 6e73 2069 6e20 6120 636f 6d6d  ptions in a comm
+00001ff0: 6120 7365 7061 7261 7465 6420 6c69 7374  a separated list
+00002000: 206c 696b 650a 0a60 6060 7368 656c 6c20   like..```shell 
+00002010: 7363 7269 7074 0a70 6970 3320 696e 7374  script.pip3 inst
+00002020: 616c 6c20 726f 626f 7469 6373 746f 6f6c  all roboticstool
+00002030: 626f 782d 7079 7468 6f6e 5b6f 7074 696f  box-python[optio
+00002040: 6e6c 6973 745d 0a60 6060 0a0a 5b53 7769  nlist].```..[Swi
+00002050: 6674 5d28 6874 7470 733a 2f2f 6769 7468  ft](https://gith
+00002060: 7562 2e63 6f6d 2f6a 6861 766c 2f73 7769  ub.com/jhavl/swi
+00002070: 6674 292c 2061 2077 6562 2d62 6173 6564  ft), a web-based
+00002080: 2076 6973 7561 6c69 7a65 722c 2069 730a   visualizer, is.
+00002090: 696e 7374 616c 6c65 6420 6173 2070 6172  installed as par
+000020a0: 7420 6f66 2052 6f62 6f74 6963 7320 546f  t of Robotics To
+000020b0: 6f6c 626f 782e 0a0a 2323 2320 4672 6f6d  olbox...### From
+000020c0: 2047 6974 4875 620a 0a54 6f20 696e 7374   GitHub..To inst
+000020d0: 616c 6c20 7468 6520 626c 6565 6469 6e67  all the bleeding
+000020e0: 2d65 6467 6520 7665 7273 696f 6e20 6672  -edge version fr
+000020f0: 6f6d 2047 6974 4875 620a 0a60 6060 7368  om GitHub..```sh
+00002100: 656c 6c20 7363 7269 7074 0a67 6974 2063  ell script.git c
+00002110: 6c6f 6e65 2068 7474 7073 3a2f 2f67 6974  lone https://git
+00002120: 6875 622e 636f 6d2f 7065 7465 7263 6f72  hub.com/petercor
+00002130: 6b65 2f72 6f62 6f74 6963 732d 746f 6f6c  ke/robotics-tool
+00002140: 626f 782d 7079 7468 6f6e 2e67 6974 0a63  box-python.git.c
+00002150: 6420 726f 626f 7469 6373 2d74 6f6f 6c62  d robotics-toolb
+00002160: 6f78 2d70 7974 686f 6e0a 7069 7033 2069  ox-python.pip3 i
+00002170: 6e73 7461 6c6c 202d 6520 2e0a 6060 600a  nstall -e ..```.
+00002180: 0a3c 6272 3e0a 0a3c 6120 6964 3d27 3327  .<br>..<a id='3'
+00002190: 3e3c 2f61 3e0a 0a23 2320 5475 746f 7269  ></a>..## Tutori
+000021a0: 616c 730a 0a3c 7461 626c 6520 7374 796c  als..<table styl
+000021b0: 653d 2262 6f72 6465 723a 3070 7822 3e0a  e="border:0px">.
+000021c0: 3c74 7220 7374 796c 653d 2262 6f72 6465  <tr style="borde
+000021d0: 723a 3070 7822 3e0a 3c74 6420 7374 796c  r:0px">.<td styl
+000021e0: 653d 2262 6f72 6465 723a 3070 7822 3e3c  e="border:0px"><
+000021f0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00002200: 6269 742e 6c79 2f33 616b 3547 4469 223e  bit.ly/3ak5GDi">
+00002210: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00002220: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 6861  //github.com/jha
+00002230: 766c 2f64 6b74 2f72 6177 2f6d 6169 6e2f  vl/dkt/raw/main/
+00002240: 696d 672f 6172 7469 636c 6531 2e70 6e67  img/article1.png
+00002250: 2220 7769 6474 683d 2234 3030 223e 3c2f  " width="400"></
+00002260: 613e 3c2f 7464 3e0a 3c74 6420 7374 796c  a></td>.<td styl
+00002270: 653d 2262 6f72 6465 723a 3070 7822 3e3c  e="border:0px"><
+00002280: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00002290: 6269 742e 6c79 2f33 616b 3547 4469 223e  bit.ly/3ak5GDi">
+000022a0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+000022b0: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 6861  //github.com/jha
+000022c0: 766c 2f64 6b74 2f72 6177 2f6d 6169 6e2f  vl/dkt/raw/main/
+000022d0: 696d 672f 6172 7469 636c 6532 2e70 6e67  img/article2.png
+000022e0: 2220 7769 6474 683d 2234 3030 223e 3c2f  " width="400"></
+000022f0: 613e 3c2f 7464 3e0a 3c74 6420 7374 796c  a></td>.<td styl
+00002300: 653d 2262 6f72 6465 723a 3070 7822 3e0a  e="border:0px">.
+00002310: 446f 2079 6f75 2077 616e 7420 746f 206c  Do you want to l
+00002320: 6561 726e 2061 626f 7574 206d 616e 6970  earn about manip
+00002330: 756c 6174 6f72 206b 696e 656d 6174 6963  ulator kinematic
+00002340: 732c 2064 6966 6665 7265 6e74 6961 6c20  s, differential 
+00002350: 6b69 6e65 6d61 7469 6373 2c20 696e 7665  kinematics, inve
+00002360: 7273 652d 6b69 6e65 6d61 7469 6373 2061  rse-kinematics a
+00002370: 6e64 206d 6f74 696f 6e20 636f 6e74 726f  nd motion contro
+00002380: 6c3f 2048 6176 6520 6120 6c6f 6f6b 2061  l? Have a look a
+00002390: 7420 6f75 720a 3c61 2068 7265 663d 2268  t our.<a href="h
+000023a0: 7474 7073 3a2f 2f62 6974 2e6c 792f 3361  ttps://bit.ly/3a
+000023b0: 6b35 4744 6922 3e74 7574 6f72 6961 6c3c  k5GDi">tutorial<
+000023c0: 2f61 3e2e 0a54 6869 7320 7475 746f 7269  /a>..This tutori
+000023d0: 616c 2063 6f6d 6573 2077 6974 6820 7477  al comes with tw
+000023e0: 6f20 6172 7469 636c 6573 2074 6f20 636f  o articles to co
+000023f0: 7665 7220 7468 6520 7468 656f 7279 2061  ver the theory a
+00002400: 6e64 2031 3220 4a75 7079 7465 7220 4e6f  nd 12 Jupyter No
+00002410: 7465 626f 6f6b 7320 7072 6f76 6964 696e  tebooks providin
+00002420: 6720 6675 6c6c 2063 6f64 6520 696d 706c  g full code impl
+00002430: 656d 656e 7461 7469 6f6e 7320 616e 6420  ementations and 
+00002440: 6578 616d 706c 6573 2e20 4d6f 7374 206f  examples. Most o
+00002450: 6620 7468 6520 4e6f 7465 626f 6f6b 7320  f the Notebooks 
+00002460: 6172 6520 616c 736f 2047 6f6f 676c 6520  are also Google 
+00002470: 436f 6c61 6220 636f 6d70 6174 6962 6c65  Colab compatible
+00002480: 2061 6c6c 6f77 696e 6720 7468 656d 2074   allowing them t
+00002490: 6f20 7275 6e20 6f6e 6c69 6e65 2e0a 3c2f  o run online..</
+000024a0: 7464 3e0a 3c2f 7472 3e0a 3c2f 7461 626c  td>.</tr>.</tabl
+000024b0: 653e 0a0a 3c62 723e 0a0a 3c61 2069 643d  e>..<br>..<a id=
+000024c0: 2734 273e 3c2f 613e 0a0a 2323 2043 6f64  '4'></a>..## Cod
+000024d0: 6520 4578 616d 706c 6573 0a0a 5765 2077  e Examples..We w
+000024e0: 696c 6c20 6c6f 6164 2061 206d 6f64 656c  ill load a model
+000024f0: 206f 6620 7468 6520 4672 616e 6b61 2d45   of the Franka-E
+00002500: 6d69 6b61 2050 616e 6461 2072 6f62 6f74  mika Panda robot
+00002510: 2064 6566 696e 6564 2062 7920 6120 5552   defined by a UR
+00002520: 4446 2066 696c 650a 0a60 6060 7079 7468  DF file..```pyth
+00002530: 6f6e 0a69 6d70 6f72 7420 726f 626f 7469  on.import roboti
+00002540: 6373 746f 6f6c 626f 7820 6173 2072 7462  cstoolbox as rtb
+00002550: 0a72 6f62 6f74 203d 2072 7462 2e6d 6f64  .robot = rtb.mod
+00002560: 656c 732e 5061 6e64 6128 290a 7072 696e  els.Panda().prin
+00002570: 7428 726f 626f 7429 0a0a 0945 526f 626f  t(robot)...ERobo
+00002580: 743a 2070 616e 6461 2028 6279 2046 7261  t: panda (by Fra
+00002590: 6e6b 6120 456d 696b 6129 2c20 3720 6a6f  nka Emika), 7 jo
+000025a0: 696e 7473 2028 5252 5252 5252 5229 2c20  ints (RRRRRRR), 
+000025b0: 3120 6772 6970 7065 722c 2067 656f 6d65  1 gripper, geome
+000025c0: 7472 792c 2063 6f6c 6c69 7369 6f6e 0a09  try, collision..
+000025d0: e294 8ce2 9480 e294 80e2 9480 e294 80e2  ................
+000025e0: 9480 e294 ace2 9480 e294 80e2 9480 e294  ................
+000025f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002600: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002610: 94ac e294 80e2 9480 e294 80e2 9480 e294  ................
+00002620: 80e2 9480 e294 80e2 94ac e294 80e2 9480  ................
+00002630: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002640: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002650: 80e2 94ac e294 80e2 9480 e294 80e2 9480  ................
+00002660: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002670: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002680: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002690: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000026a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000026b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000026c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000026d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000026e0: 80e2 9480 e294 900a 09e2 9482 6c69 6e6b  ............link
+000026f0: 20e2 9482 2020 2020 206c 696e 6b20 2020   ...     link   
+00002700: 2020 e294 8220 6a6f 696e 7420 e294 8220    ... joint ... 
+00002710: 2020 7061 7265 6e74 2020 2020 e294 8220    parent    ... 
+00002720: 2020 2020 2020 2020 2020 2020 2045 5453               ETS
+00002730: 3a20 7061 7265 6e74 2074 6f20 6c69 6e6b  : parent to link
+00002740: 2020 2020 2020 2020 2020 2020 2020 20e2                 .
+00002750: 9482 0a09 e294 9ce2 9480 e294 80e2 9480  ................
+00002760: e294 80e2 9480 e294 bce2 9480 e294 80e2  ................
+00002770: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002780: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002790: e294 80e2 94bc e294 80e2 9480 e294 80e2  ................
+000027a0: 9480 e294 80e2 9480 e294 80e2 94bc e294  ................
+000027b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000027c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000027d0: 9480 e294 80e2 94bc e294 80e2 9480 e294  ................
+000027e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000027f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002800: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002810: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002820: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002830: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002840: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002850: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002860: 9480 e294 80e2 9480 e294 a40a 09e2 9482  ................
+00002870: 2020 2030 20e2 9482 2070 616e 6461 5f6c     0 ... panda_l
+00002880: 696e 6b30 2020 e294 8220 2020 2020 2020  ink0  ...       
+00002890: e294 8220 4241 5345 2020 2020 2020 2020  ... BASE        
+000028a0: e294 8220 2020 2020 2020 2020 2020 2020  ...             
+000028b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028d0: 2020 20e2 9482 0a09 e294 8220 2020 3120     ........   1 
+000028e0: e294 8220 7061 6e64 615f 6c69 6e6b 3120  ... panda_link1 
+000028f0: 20e2 9482 2020 2020 2030 20e2 9482 2070   ...     0 ... p
+00002900: 616e 6461 5f6c 696e 6b30 20e2 9482 2053  anda_link0 ... S
+00002910: 4533 2830 2c20 302c 2030 2e33 3333 2920  E3(0, 0, 0.333) 
+00002920: e28a 9520 527a 2871 3029 2020 2020 2020  ... Rz(q0)      
+00002930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002940: e294 820a 09e2 9482 2020 2032 20e2 9482  ........   2 ...
+00002950: 2070 616e 6461 5f6c 696e 6b32 2020 e294   panda_link2  ..
+00002960: 8220 2020 2020 3120 e294 8220 7061 6e64  .     1 ... pand
+00002970: 615f 6c69 6e6b 3120 e294 8220 5345 3328  a_link1 ... SE3(
+00002980: 2d39 30c2 b02c 202d 30c2 b02c 2030 c2b0  -90.., -0.., 0..
+00002990: 2920 e28a 9520 527a 2871 3129 2020 2020  ) ... Rz(q1)    
+000029a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029b0: e294 820a 09e2 9482 2020 2033 20e2 9482  ........   3 ...
+000029c0: 2070 616e 6461 5f6c 696e 6b33 2020 e294   panda_link3  ..
+000029d0: 8220 2020 2020 3220 e294 8220 7061 6e64  .     2 ... pand
+000029e0: 615f 6c69 6e6b 3220 e294 8220 5345 3328  a_link2 ... SE3(
+000029f0: 302c 202d 302e 3331 362c 2030 3b20 3930  0, -0.316, 0; 90
+00002a00: c2b0 2c20 2d30 c2b0 2c20 30c2 b029 20e2  .., -0.., 0..) .
+00002a10: 8a95 2052 7a28 7132 2920 2020 2020 2020  .. Rz(q2)       
+00002a20: e294 820a 09e2 9482 2020 2034 20e2 9482  ........   4 ...
+00002a30: 2070 616e 6461 5f6c 696e 6b34 2020 e294   panda_link4  ..
+00002a40: 8220 2020 2020 3320 e294 8220 7061 6e64  .     3 ... pand
+00002a50: 615f 6c69 6e6b 3320 e294 8220 5345 3328  a_link3 ... SE3(
+00002a60: 302e 3038 3235 2c20 302c 2030 3b20 3930  0.0825, 0, 0; 90
+00002a70: c2b0 2c20 2d30 c2b0 2c20 30c2 b029 20e2  .., -0.., 0..) .
+00002a80: 8a95 2052 7a28 7133 2920 2020 2020 2020  .. Rz(q3)       
+00002a90: e294 820a 09e2 9482 2020 2035 20e2 9482  ........   5 ...
+00002aa0: 2070 616e 6461 5f6c 696e 6b35 2020 e294   panda_link5  ..
+00002ab0: 8220 2020 2020 3420 e294 8220 7061 6e64  .     4 ... pand
+00002ac0: 615f 6c69 6e6b 3420 e294 8220 5345 3328  a_link4 ... SE3(
+00002ad0: 2d30 2e30 3832 352c 2030 2e33 3834 2c20  -0.0825, 0.384, 
+00002ae0: 303b 202d 3930 c2b0 2c20 2d30 c2b0 2c20  0; -90.., -0.., 
+00002af0: 30c2 b029 20e2 8a95 2052 7a28 7134 2920  0..) ... Rz(q4) 
+00002b00: e294 820a 09e2 9482 2020 2036 20e2 9482  ........   6 ...
+00002b10: 2070 616e 6461 5f6c 696e 6b36 2020 e294   panda_link6  ..
+00002b20: 8220 2020 2020 3520 e294 8220 7061 6e64  .     5 ... pand
+00002b30: 615f 6c69 6e6b 3520 e294 8220 5345 3328  a_link5 ... SE3(
+00002b40: 3930 c2b0 2c20 2d30 c2b0 2c20 30c2 b029  90.., -0.., 0..)
+00002b50: 20e2 8a95 2052 7a28 7135 2920 2020 2020   ... Rz(q5)     
+00002b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b70: e294 820a 09e2 9482 2020 2037 20e2 9482  ........   7 ...
+00002b80: 2070 616e 6461 5f6c 696e 6b37 2020 e294   panda_link7  ..
+00002b90: 8220 2020 2020 3620 e294 8220 7061 6e64  .     6 ... pand
+00002ba0: 615f 6c69 6e6b 3620 e294 8220 5345 3328  a_link6 ... SE3(
+00002bb0: 302e 3038 382c 2030 2c20 303b 2039 30c2  0.088, 0, 0; 90.
+00002bc0: b02c 202d 30c2 b02c 2030 c2b0 2920 e28a  ., -0.., 0..) ..
+00002bd0: 9520 527a 2871 3629 2020 2020 2020 2020  . Rz(q6)        
+00002be0: e294 820a 09e2 9482 2020 2038 20e2 9482  ........   8 ...
+00002bf0: 2040 7061 6e64 615f 6c69 6e6b 3820 e294   @panda_link8 ..
+00002c00: 8220 2020 2020 2020 e294 8220 7061 6e64  .       ... pand
+00002c10: 615f 6c69 6e6b 3720 e294 8220 5345 3328  a_link7 ... SE3(
+00002c20: 302c 2030 2c20 302e 3130 3729 2020 2020  0, 0, 0.107)    
+00002c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c40: 2020 2020 2020 2020 2020 20e2 9482 0a09             .....
+00002c50: e294 94e2 9480 e294 80e2 9480 e294 80e2  ................
+00002c60: 9480 e294 b4e2 9480 e294 80e2 9480 e294  ................
+00002c70: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002c80: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002c90: 94b4 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002ca0: 80e2 9480 e294 80e2 94b4 e294 80e2 9480  ................
+00002cb0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002cc0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002cd0: 80e2 94b4 e294 80e2 9480 e294 80e2 9480  ................
+00002ce0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002cf0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002d00: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002d10: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002d20: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002d30: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002d40: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002d50: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002d60: 80e2 9480 e294 980a 0a09 e294 8ce2 9480  ................
+00002d70: e294 80e2 9480 e294 80e2 9480 e294 ace2  ................
+00002d80: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002d90: ace2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002da0: e294 80e2 9480 e294 80e2 94ac e294 80e2  ................
+00002db0: 9480 e294 80e2 9480 e294 80e2 94ac e294  ................
+00002dc0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002dd0: e294 80e2 94ac e294 80e2 9480 e294 80e2  ................
+00002de0: 9480 e294 80e2 94ac e294 80e2 9480 e294  ................
+00002df0: 80e2 9480 e294 80e2 9480 e294 80e2 94ac  ................
+00002e00: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002e10: 9480 e294 900a 09e2 9482 6e61 6d65 20e2  ..........name .
+00002e20: 9482 2071 3020 20e2 9482 2071 3120 2020  .. q0  ... q1   
+00002e30: 2020 e294 8220 7132 2020 e294 8220 7133    ... q2  ... q3
+00002e40: 2020 2020 e294 8220 7134 2020 e294 8220      ... q4  ... 
+00002e50: 7135 2020 2020 e294 8220 7136 2020 20e2  q5    ... q6   .
+00002e60: 9482 0a09 e294 9ce2 9480 e294 80e2 9480  ................
+00002e70: e294 80e2 9480 e294 bce2 9480 e294 80e2  ................
+00002e80: 9480 e294 80e2 9480 e294 bce2 9480 e294  ................
+00002e90: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002ea0: e294 80e2 94bc e294 80e2 9480 e294 80e2  ................
+00002eb0: 9480 e294 80e2 94bc e294 80e2 9480 e294  ................
+00002ec0: 80e2 9480 e294 80e2 9480 e294 80e2 94bc  ................
+00002ed0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002ee0: 94bc e294 80e2 9480 e294 80e2 9480 e294  ................
+00002ef0: 80e2 9480 e294 80e2 94bc e294 80e2 9480  ................
+00002f00: e294 80e2 9480 e294 80e2 9480 e294 a40a  ................
+00002f10: 09e2 9482 2020 7172 20e2 9482 2020 30c2  ....  qr ...  0.
+00002f20: b020 e294 8220 2d31 372e 32c2 b020 e294  . ... -17.2.. ..
+00002f30: 8220 2030 c2b0 20e2 9482 202d 3132 36c2  .  0.. ... -126.
+00002f40: b020 e294 8220 2030 c2b0 20e2 9482 2020  . ...  0.. ...  
+00002f50: 3131 35c2 b020 e294 8220 2034 35c2 b020  115.. ...  45.. 
+00002f60: e294 820a 09e2 9482 2020 717a 20e2 9482  ........  qz ...
+00002f70: 2020 30c2 b020 e294 8220 2030 c2b0 2020    0.. ...  0..  
+00002f80: 2020 e294 8220 2030 c2b0 20e2 9482 2020    ...  0.. ...  
+00002f90: 30c2 b020 2020 e294 8220 2030 c2b0 20e2  0..   ...  0.. .
+00002fa0: 9482 2020 30c2 b020 2020 e294 8220 2030  ..  0..   ...  0
+00002fb0: c2b0 2020 e294 820a 09e2 9494 e294 80e2  ..  ............
+00002fc0: 9480 e294 80e2 9480 e294 80e2 94b4 e294  ................
+00002fd0: 80e2 9480 e294 80e2 9480 e294 80e2 94b4  ................
+00002fe0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002ff0: 9480 e294 80e2 9480 e294 b4e2 9480 e294  ................
+00003000: 80e2 9480 e294 80e2 9480 e294 b4e2 9480  ................
+00003010: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003020: 9480 e294 b4e2 9480 e294 80e2 9480 e294  ................
+00003030: 80e2 9480 e294 b4e2 9480 e294 80e2 9480  ................
+00003040: e294 80e2 9480 e294 80e2 9480 e294 b4e2  ................
+00003050: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003060: 80e2 9498 0a60 6060 0a0a 5468 6520 7379  .....```..The sy
+00003070: 6d62 6f6c 2060 4060 2069 6e64 6963 6174  mbol `@` indicat
+00003080: 6573 2074 6865 206c 696e 6b20 6173 2061  es the link as a
+00003090: 6e20 656e 642d 6566 6665 6374 6f72 2c20  n end-effector, 
+000030a0: 6120 6c65 6166 206e 6f64 6520 696e 2074  a leaf node in t
+000030b0: 6865 2072 6967 6964 2d62 6f64 790a 7472  he rigid-body.tr
+000030c0: 6565 2028 5079 7468 6f6e 2070 726f 6d70  ee (Python promp
+000030d0: 7473 2061 7265 206e 6f74 2073 686f 776e  ts are not shown
+000030e0: 2074 6f20 6d61 6b65 2069 7420 6561 7379   to make it easy
+000030f0: 2074 6f20 636f 7079 2b70 6173 7465 2074   to copy+paste t
+00003100: 6865 2063 6f64 652c 2063 6f6e 736f 6c65  he code, console
+00003110: 206f 7574 7075 7420 6973 2069 6e64 656e   output is inden
+00003120: 7465 6429 2e0a 5765 2077 696c 6c20 636f  ted)..We will co
+00003130: 6d70 7574 6520 7468 6520 666f 7277 6172  mpute the forwar
+00003140: 6420 6b69 6e65 6d61 7469 6373 206e 6578  d kinematics nex
+00003150: 740a 0a60 6060 0a54 6520 3d20 726f 626f  t..```.Te = robo
+00003160: 742e 666b 696e 6528 726f 626f 742e 7172  t.fkine(robot.qr
+00003170: 2920 2023 2066 6f72 7761 7264 206b 696e  )  # forward kin
+00003180: 656d 6174 6963 730a 7072 696e 7428 5465  ematics.print(Te
+00003190: 290a 0a09 302e 3939 3520 2020 2020 3020  )...0.995     0 
+000031a0: 2020 2020 2020 2020 302e 3039 3938 3320          0.09983 
+000031b0: 2020 302e 3438 340a 0930 2020 2020 2020    0.484..0      
+000031c0: 2020 2d31 2020 2020 2020 2020 2030 2020    -1         0  
+000031d0: 2020 2020 2020 2030 0a09 302e 3039 3938         0..0.0998
+000031e0: 3320 2020 3020 2020 2020 2020 202d 302e  3   0        -0.
+000031f0: 3939 3520 2020 2020 302e 3431 3236 0a09  995     0.4126..
+00003200: 3020 2020 2020 2020 2020 3020 2020 2020  0         0     
+00003210: 2020 2020 3020 2020 2020 2020 2020 310a      0         1.
+00003220: 6060 600a 0a57 6520 6361 6e20 736f 6c76  ```..We can solv
+00003230: 6520 696e 7665 7273 6520 6b69 6e65 6d61  e inverse kinema
+00003240: 7469 6373 2076 6572 7920 6561 7369 6c79  tics very easily
+00003250: 2e20 5765 2066 6972 7374 2063 686f 6f73  . We first choos
+00003260: 6520 616e 2053 4528 3329 2070 6f73 650a  e an SE(3) pose.
+00003270: 6465 6669 6e65 6420 696e 2074 6572 6d73  defined in terms
+00003280: 206f 6620 706f 7369 7469 6f6e 2061 6e64   of position and
+00003290: 206f 7269 656e 7461 7469 6f6e 2028 656e   orientation (en
+000032a0: 642d 6566 6665 6374 6f72 207a 2d61 7869  d-effector z-axi
+000032b0: 7320 646f 776e 2028 413d 2d5a 2920 616e  s down (A=-Z) an
+000032c0: 6420 6669 6e67 6572 0a6f 7269 656e 7461  d finger.orienta
+000032d0: 7469 6f6e 2070 6172 616c 6c65 6c20 746f  tion parallel to
+000032e0: 2079 2d61 7869 7320 284f 3d2b 5929 292e   y-axis (O=+Y)).
+000032f0: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
+00003300: 2073 7061 7469 616c 6d61 7468 2069 6d70   spatialmath imp
+00003310: 6f72 7420 5345 330a 0a54 6570 203d 2053  ort SE3..Tep = S
+00003320: 4533 2e54 7261 6e73 2830 2e36 2c20 2d30  E3.Trans(0.6, -0
+00003330: 2e33 2c20 302e 3129 202a 2053 4533 2e4f  .3, 0.1) * SE3.O
+00003340: 4128 5b30 2c20 312c 2030 5d2c 205b 302c  A([0, 1, 0], [0,
+00003350: 2030 2c20 2d31 5d29 0a73 6f6c 203d 2072   0, -1]).sol = r
+00003360: 6f62 6f74 2e69 6b5f 4c4d 2854 6570 2920  obot.ik_LM(Tep) 
+00003370: 2020 2020 2020 2020 2320 736f 6c76 6520          # solve 
+00003380: 494b 0a70 7269 6e74 2873 6f6c 290a 0a09  IK.print(sol)...
+00003390: 2861 7272 6179 285b 2030 2e32 3035 3932  (array([ 0.20592
+000033a0: 3831 352c 2020 302e 3836 3630 3934 3831  815,  0.86609481
+000033b0: 2c20 2d30 2e37 3934 3733 3230 362c 202d  , -0.79473206, -
+000033c0: 312e 3638 3235 3437 3934 2c20 2030 2e37  1.68254794,  0.7
+000033d0: 3438 3732 3931 352c 0a09 0909 322e 3231  4872915,....2.21
+000033e0: 3736 3437 3436 2c20 2d30 2e31 3032 3535  764746, -0.10255
+000033f0: 3630 365d 292c 2031 2c20 3131 342c 2037  606]), 1, 114, 7
+00003400: 2c20 322e 3839 3031 3634 3035 3732 3330  , 2.890164057230
+00003410: 3232 3865 2d30 3729 0a0a 715f 7069 636b  228e-07)..q_pick
+00003420: 7570 203d 2073 6f6c 5b30 5d0a 7072 696e  up = sol[0].prin
+00003430: 7428 726f 626f 742e 666b 696e 6528 715f  t(robot.fkine(q_
+00003440: 7069 636b 7570 2929 2020 2020 2320 464b  pickup))    # FK
+00003450: 2073 686f 7773 2074 6861 7420 6465 7369   shows that desi
+00003460: 7265 6420 656e 642d 6566 6665 6374 6f72  red end-effector
+00003470: 2070 6f73 6520 7761 7320 6163 6869 6576   pose was achiev
+00003480: 6564 0a0a 0920 3120 2020 2020 2020 2020  ed... 1         
+00003490: 2d38 2e39 3133 652d 3035 2020 2d30 2e30  -8.913e-05  -0.0
+000034a0: 3030 3333 3334 2020 302e 3539 3936 0a09  003334  0.5996..
+000034b0: 2d38 2e39 3239 652d 3035 202d 3120 2020  -8.929e-05 -1   
+000034c0: 2020 2020 2020 202d 302e 3030 3034 3931         -0.000491
+000034d0: 3220 2d30 2e32 3939 380a 092d 302e 3030  2 -0.2998..-0.00
+000034e0: 3033 3333 3420 2030 2e30 3030 3439 3132  03334  0.0004912
+000034f0: 2020 2d31 2020 2020 2020 2020 2020 302e    -1          0.
+00003500: 3130 3031 0a09 2030 2020 2020 2020 2020  1001.. 0        
+00003510: 2020 3020 2020 2020 2020 2020 2020 3020    0           0 
+00003520: 2020 2020 2020 2020 2031 0a60 6060 0a0a           1.```..
+00003530: 5765 2063 616e 2061 6e69 6d61 7465 2061  We can animate a
+00003540: 2070 6174 6820 6672 6f6d 2074 6865 2072   path from the r
+00003550: 6561 6479 2070 6f73 6520 6071 7260 2063  eady pose `qr` c
+00003560: 6f6e 6669 6775 7261 7469 6f6e 2074 6f20  onfiguration to 
+00003570: 7468 6973 2070 6963 6b75 7020 636f 6e66  this pickup conf
+00003580: 6967 7572 6174 696f 6e0a 0a60 6060 7079  iguration..```py
+00003590: 7468 6f6e 0a71 7420 3d20 7274 622e 6a74  thon.qt = rtb.jt
+000035a0: 7261 6a28 726f 626f 742e 7172 2c20 715f  raj(robot.qr, q_
+000035b0: 7069 636b 7570 2c20 3530 290a 726f 626f  pickup, 50).robo
+000035c0: 742e 706c 6f74 2871 742e 712c 2062 6163  t.plot(qt.q, bac
+000035d0: 6b65 6e64 3d27 7079 706c 6f74 272c 206d  kend='pyplot', m
+000035e0: 6f76 6965 3d27 7061 6e64 6131 2e67 6966  ovie='panda1.gif
+000035f0: 2729 0a60 6060 0a0a 3c70 2061 6c69 676e  ').```..<p align
+00003600: 3d22 6365 6e74 6572 223e 0a09 3c69 6d67  ="center">..<img
+00003610: 2073 7263 3d22 2e2f 646f 6373 2f66 6967   src="./docs/fig
+00003620: 732f 7061 6e64 6131 2e67 6966 223e 0a3c  s/panda1.gif">.<
+00003630: 2f70 3e0a 0a77 6865 7265 2077 6520 6861  /p>..where we ha
+00003640: 7665 2073 7065 6369 6669 6564 2074 6865  ve specified the
+00003650: 206d 6174 706c 6f74 6c69 6220 6070 7970   matplotlib `pyp
+00003660: 6c6f 7460 2062 6163 6b65 6e64 2e20 426c  lot` backend. Bl
+00003670: 7565 2061 7272 6f77 7320 7368 6f77 2074  ue arrows show t
+00003680: 6865 206a 6f69 6e74 2061 7865 7320 616e  he joint axes an
+00003690: 6420 7468 6520 636f 6c6f 7572 6564 2066  d the coloured f
+000036a0: 7261 6d65 2073 686f 7773 2074 6865 2065  rame shows the e
+000036b0: 6e64 2d65 6666 6563 746f 7220 706f 7365  nd-effector pose
+000036c0: 2e0a 0a57 6520 6361 6e20 616c 736f 2070  ...We can also p
+000036d0: 6c6f 7420 7468 6520 7472 616a 6563 746f  lot the trajecto
+000036e0: 7279 2069 6e20 7468 6520 5377 6966 7420  ry in the Swift 
+000036f0: 7369 6d75 6c61 746f 7220 2861 2062 726f  simulator (a bro
+00003700: 7773 6572 2d62 6173 6564 2033 642d 7369  wser-based 3d-si
+00003710: 6d75 6c61 7469 6f6e 2065 6e76 6972 6f6e  mulation environ
+00003720: 6d65 6e74 2062 7569 6c74 2074 6f20 776f  ment built to wo
+00003730: 726b 2077 6974 6820 7468 6520 546f 6f6c  rk with the Tool
+00003740: 626f 7829 0a0a 6060 6070 7974 686f 6e0a  box)..```python.
+00003750: 726f 626f 742e 706c 6f74 2871 742e 7129  robot.plot(qt.q)
+00003760: 0a60 6060 0a0a 3c70 2061 6c69 676e 3d22  .```..<p align="
+00003770: 6365 6e74 6572 223e 0a09 3c69 6d67 2073  center">..<img s
+00003780: 7263 3d22 2e2f 646f 6373 2f66 6967 732f  rc="./docs/figs/
+00003790: 7061 6e64 6132 2e67 6966 223e 0a3c 2f70  panda2.gif">.</p
+000037a0: 3e0a 0a57 6520 6361 6e20 616c 736f 2065  >..We can also e
+000037b0: 7870 6572 696d 656e 7420 7769 7468 2076  xperiment with v
+000037c0: 656c 6f63 6974 7920 636f 6e74 726f 6c6c  elocity controll
+000037d0: 6572 7320 696e 2053 7769 6674 2e20 4865  ers in Swift. He
+000037e0: 7265 2069 7320 6120 7265 736f 6c76 6564  re is a resolved
+000037f0: 2d72 6174 6520 6d6f 7469 6f6e 2063 6f6e  -rate motion con
+00003800: 7472 6f6c 2065 7861 6d70 6c65 0a0a 6060  trol example..``
+00003810: 6070 7974 686f 6e0a 696d 706f 7274 2073  `python.import s
+00003820: 7769 6674 0a69 6d70 6f72 7420 726f 626f  wift.import robo
+00003830: 7469 6373 746f 6f6c 626f 7820 6173 2072  ticstoolbox as r
+00003840: 7462 0a69 6d70 6f72 7420 7370 6174 6961  tb.import spatia
+00003850: 6c6d 6174 6820 6173 2073 6d0a 696d 706f  lmath as sm.impo
+00003860: 7274 206e 756d 7079 2061 7320 6e70 0a0a  rt numpy as np..
+00003870: 656e 7620 3d20 7377 6966 742e 5377 6966  env = swift.Swif
+00003880: 7428 290a 656e 762e 6c61 756e 6368 2872  t().env.launch(r
+00003890: 6561 6c74 696d 653d 5472 7565 290a 0a70  ealtime=True)..p
+000038a0: 616e 6461 203d 2072 7462 2e6d 6f64 656c  anda = rtb.model
+000038b0: 732e 5061 6e64 6128 290a 7061 6e64 612e  s.Panda().panda.
+000038c0: 7120 3d20 7061 6e64 612e 7172 0a0a 5465  q = panda.qr..Te
+000038d0: 7020 3d20 7061 6e64 612e 666b 696e 6528  p = panda.fkine(
+000038e0: 7061 6e64 612e 7129 202a 2073 6d2e 5345  panda.q) * sm.SE
+000038f0: 332e 5472 616e 7328 302e 322c 2030 2e32  3.Trans(0.2, 0.2
+00003900: 2c20 302e 3435 290a 0a61 7272 6976 6564  , 0.45)..arrived
+00003910: 203d 2046 616c 7365 0a65 6e76 2e61 6464   = False.env.add
+00003920: 2870 616e 6461 290a 0a64 7420 3d20 302e  (panda)..dt = 0.
+00003930: 3035 0a0a 7768 696c 6520 6e6f 7420 6172  05..while not ar
+00003940: 7269 7665 643a 0a0a 2020 2020 762c 2061  rived:..    v, a
+00003950: 7272 6976 6564 203d 2072 7462 2e70 5f73  rrived = rtb.p_s
+00003960: 6572 766f 2870 616e 6461 2e66 6b69 6e65  ervo(panda.fkine
+00003970: 2870 616e 6461 2e71 292c 2054 6570 2c20  (panda.q), Tep, 
+00003980: 3129 0a20 2020 2070 616e 6461 2e71 6420  1).    panda.qd 
+00003990: 3d20 6e70 2e6c 696e 616c 672e 7069 6e76  = np.linalg.pinv
+000039a0: 2870 616e 6461 2e6a 6163 6f62 6528 7061  (panda.jacobe(pa
+000039b0: 6e64 612e 7129 2920 4020 760a 2020 2020  nda.q)) @ v.    
+000039c0: 656e 762e 7374 6570 2864 7429 0a0a 2320  env.step(dt)..# 
+000039d0: 556e 636f 6d6d 656e 7420 746f 2073 746f  Uncomment to sto
+000039e0: 7020 7468 6520 6272 6f77 7365 7220 7461  p the browser ta
+000039f0: 6220 6672 6f6d 2063 6c6f 7369 6e67 0a23  b from closing.#
+00003a00: 2065 6e76 2e68 6f6c 6428 290a 6060 600a   env.hold().```.
+00003a10: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+00003a20: 7222 3e0a 093c 696d 6720 7372 633d 222e  r">..<img src=".
+00003a30: 2f64 6f63 732f 6669 6773 2f70 616e 6461  /docs/figs/panda
+00003a40: 332e 6769 6622 3e0a 3c2f 703e 0a0a 2323  3.gif">.</p>..##
+00003a50: 2320 5275 6e20 736f 6d65 2065 7861 6d70  # Run some examp
+00003a60: 6c65 730a 0a54 6865 205b 606e 6f74 6562  les..The [`noteb
+00003a70: 6f6f 6b73 605d 2868 7474 7073 3a2f 2f67  ooks`](https://g
+00003a80: 6974 6875 622e 636f 6d2f 7065 7465 7263  ithub.com/peterc
+00003a90: 6f72 6b65 2f72 6f62 6f74 6963 732d 746f  orke/robotics-to
+00003aa0: 6f6c 626f 782d 7079 7468 6f6e 2f74 7265  olbox-python/tre
+00003ab0: 652f 6d61 7374 6572 2f6e 6f74 6562 6f6f  e/master/noteboo
+00003ac0: 6b73 2920 666f 6c64 6572 2063 6f6e 7461  ks) folder conta
+00003ad0: 696e 7320 736f 6d65 2074 7574 6f72 6961  ins some tutoria
+00003ae0: 6c20 4a75 7079 7465 7220 6e6f 7465 626f  l Jupyter notebo
+00003af0: 6f6b 7320 7768 6963 6820 796f 7520 6361  oks which you ca
+00003b00: 6e20 6272 6f77 7365 206f 6e20 4769 7448  n browse on GitH
+00003b10: 7562 2e20 4164 6469 7469 6f6e 616c 6c79  ub. Additionally
+00003b20: 2c20 6861 7665 2061 206c 6f6f 6b20 696e  , have a look in
+00003b30: 2074 6865 205b 6065 7861 6d70 6c65 7360   the [`examples`
+00003b40: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00003b50: 2e63 6f6d 2f70 6574 6572 636f 726b 652f  .com/petercorke/
+00003b60: 726f 626f 7469 6373 2d74 6f6f 6c62 6f78  robotics-toolbox
+00003b70: 2d70 7974 686f 6e2f 7472 6565 2f6d 6173  -python/tree/mas
+00003b80: 7465 722f 726f 626f 7469 6373 746f 6f6c  ter/roboticstool
+00003b90: 626f 782f 6578 616d 706c 6573 2920 666f  box/examples) fo
+00003ba0: 6c64 6572 2066 6f72 206d 616e 7920 7265  lder for many re
+00003bb0: 6164 7920 746f 2072 756e 2065 7861 6d70  ady to run examp
+00003bc0: 6c65 732e 0a0a 3c62 723e 0a0a 3c61 2069  les...<br>..<a i
+00003bd0: 643d 2735 273e 3c2f 613e 0a0a 2323 2054  d='5'></a>..## T
+00003be0: 6f6f 6c62 6f78 2052 6573 6561 7263 6820  oolbox Research 
+00003bf0: 4170 706c 6963 6174 696f 6e73 0a0a 5468  Applications..Th
+00003c00: 6520 746f 6f6c 626f 7820 6973 2069 6e63  e toolbox is inc
+00003c10: 7265 6469 626c 7920 7573 6566 756c 2066  redibly useful f
+00003c20: 6f72 2064 6576 656c 6f70 696e 6720 616e  or developing an
+00003c30: 6420 7072 6f74 6f74 7970 696e 6720 616c  d prototyping al
+00003c40: 676f 7269 7468 6d73 2066 6f72 2072 6573  gorithms for res
+00003c50: 6561 7263 682c 2074 6861 6e6b 7320 746f  earch, thanks to
+00003c60: 2074 6865 2065 7868 6175 7374 6976 6520   the exhaustive 
+00003c70: 7365 7420 6f66 2077 656c 6c20 646f 6375  set of well docu
+00003c80: 6d65 6e74 6564 2061 6e64 206d 6174 7572  mented and matur
+00003c90: 6520 726f 626f 7469 6320 6675 6e63 7469  e robotic functi
+00003ca0: 6f6e 7320 6578 706f 7365 6420 7468 726f  ons exposed thro
+00003cb0: 7567 6820 636c 6561 6e20 616e 6420 7061  ugh clean and pa
+00003cc0: 696e 6c65 7373 2041 5049 732e 2041 6464  inless APIs. Add
+00003cd0: 6974 696f 6e61 6c6c 792c 2074 6865 2065  itionally, the e
+00003ce0: 6173 6520 6174 2077 6869 6368 2061 2075  ase at which a u
+00003cf0: 7365 7220 6361 6e20 7669 7375 616c 697a  ser can visualiz
+00003d00: 6520 7468 6569 7220 616c 676f 7269 7468  e their algorith
+00003d10: 6d20 7375 7070 6f72 7473 2061 2072 6170  m supports a rap
+00003d20: 6964 2070 726f 746f 7479 7069 6e67 2070  id prototyping p
+00003d30: 6172 6164 6967 6d2e 0a0a 2323 2320 5075  aradigm...### Pu
+00003d40: 626c 6963 6174 696f 6e20 4c69 7374 0a0a  blication List..
+00003d50: 4a2e 2048 6176 696c 616e 642c 204e 2e20  J. Haviland, N. 
+00003d60: 53c3 bc6e 6465 7268 6175 6620 616e 6420  S..nderhauf and 
+00003d70: 502e 2043 6f72 6b65 2c20 222a 2a41 2048  P. Corke, "**A H
+00003d80: 6f6c 6973 7469 6320 4170 7072 6f61 6368  olistic Approach
+00003d90: 2074 6f20 5265 6163 7469 7665 204d 6f62   to Reactive Mob
+00003da0: 696c 6520 4d61 6e69 7075 6c61 7469 6f6e  ile Manipulation
+00003db0: 2a2a 2c22 2069 6e20 5f49 4545 4520 526f  **," in _IEEE Ro
+00003dc0: 626f 7469 6373 2061 6e64 2041 7574 6f6d  botics and Autom
+00003dd0: 6174 696f 6e20 4c65 7474 6572 735f 2c20  ation Letters_, 
+00003de0: 646f 693a 2031 302e 3131 3039 2f4c 5241  doi: 10.1109/LRA
+00003df0: 2e32 3032 322e 3331 3436 3535 342e 2049  .2022.3146554. I
+00003e00: 6e20 7468 6520 7669 6465 6f2c 2074 6865  n the video, the
+00003e10: 2072 6f62 6f74 2069 7320 636f 6e74 726f   robot is contro
+00003e20: 6c6c 6564 2075 7369 6e67 2074 6865 2052  lled using the R
+00003e30: 6f62 6f74 6963 7320 746f 6f6c 626f 7820  obotics toolbox 
+00003e40: 666f 7220 5079 7468 6f6e 2061 6e64 2066  for Python and f
+00003e50: 6561 7475 7265 7320 6120 7265 636f 7264  eatures a record
+00003e60: 696e 6720 6672 6f6d 2074 6865 205b 5377  ing from the [Sw
+00003e70: 6966 745d 2868 7474 7073 3a2f 2f67 6974  ift](https://git
+00003e80: 6875 622e 636f 6d2f 6a68 6176 6c2f 7377  hub.com/jhavl/sw
+00003e90: 6966 7429 2053 696d 756c 6174 6f72 2e0a  ift) Simulator..
+00003ea0: 0a5b 5b41 7278 6976 2050 6170 6572 5d28  .[[Arxiv Paper](
+00003eb0: 6874 7470 733a 2f2f 6172 7869 762e 6f72  https://arxiv.or
+00003ec0: 672f 6162 732f 3231 3039 2e30 3437 3439  g/abs/2109.04749
+00003ed0: 295d 205b 5b49 4545 4520 5870 6c6f 7265  )] [[IEEE Xplore
+00003ee0: 5d28 6874 7470 733a 2f2f 6965 6565 7870  ](https://ieeexp
+00003ef0: 6c6f 7265 2e69 6565 652e 6f72 672f 6162  lore.ieee.org/ab
+00003f00: 7374 7261 6374 2f64 6f63 756d 656e 742f  stract/document/
+00003f10: 3936 3935 3239 3829 5d20 5b5b 5072 6f6a  9695298)] [[Proj
+00003f20: 6563 7420 5765 6273 6974 655d 2868 7474  ect Website](htt
+00003f30: 7073 3a2f 2f6a 6861 766c 2e67 6974 6875  ps://jhavl.githu
+00003f40: 622e 696f 2f68 6f6c 6973 7469 632f 295d  b.io/holistic/)]
+00003f50: 205b 5b56 6964 656f 5d28 6874 7470 733a   [[Video](https:
+00003f60: 2f2f 796f 7574 752e 6265 2f2d 4458 4251  //youtu.be/-DXBQ
+00003f70: 5065 4c49 5634 295d 205b 5b43 6f64 6520  PeLIV4)] [[Code 
+00003f80: 4578 616d 706c 655d 2868 7474 7073 3a2f  Example](https:/
+00003f90: 2f67 6974 6875 622e 636f 6d2f 7065 7465  /github.com/pete
+00003fa0: 7263 6f72 6b65 2f72 6f62 6f74 6963 732d  rcorke/robotics-
+00003fb0: 746f 6f6c 626f 782d 7079 7468 6f6e 2f62  toolbox-python/b
+00003fc0: 6c6f 622f 6d61 7374 6572 2f72 6f62 6f74  lob/master/robot
+00003fd0: 6963 7374 6f6f 6c62 6f78 2f65 7861 6d70  icstoolbox/examp
+00003fe0: 6c65 732f 686f 6c69 7374 6963 5f6d 6d5f  les/holistic_mm_
+00003ff0: 6e6f 6e5f 686f 6c6f 6e6f 6d69 632e 7079  non_holonomic.py
+00004000: 295d 0a0a 3c70 3e0a 2020 3c61 2068 7265  )]..<p>.  <a hre
+00004010: 663d 2268 7474 7073 3a2f 2f79 6f75 7475  f="https://youtu
+00004020: 2e62 652f 2d44 5842 5150 654c 4956 3422  .be/-DXBQPeLIV4"
+00004030: 3e0a 2020 2020 3c69 6d67 2073 7263 3d22  >.    <img src="
+00004040: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00004050: 6f6d 2f70 6574 6572 636f 726b 652f 726f  om/petercorke/ro
+00004060: 626f 7469 6373 2d74 6f6f 6c62 6f78 2d70  botics-toolbox-p
+00004070: 7974 686f 6e2f 7261 772f 6d61 7374 6572  ython/raw/master
+00004080: 2f64 6f63 732f 6669 6773 2f68 6f6c 6973  /docs/figs/holis
+00004090: 7469 635f 796f 7574 7562 652e 706e 6722  tic_youtube.png"
+000040a0: 2077 6964 7468 3d22 3536 3022 3e0a 2020   width="560">.  
+000040b0: 3c2f 613e 0a3c 2f70 3e0a 0a4a 2e20 4861  </a>.</p>..J. Ha
+000040c0: 7669 6c61 6e64 2061 6e64 2050 2e20 436f  viland and P. Co
+000040d0: 726b 652c 2022 2a2a 4e45 4f3a 2041 204e  rke, "**NEO: A N
+000040e0: 6f76 656c 2045 7870 6564 6974 696f 7573  ovel Expeditious
+000040f0: 204f 7074 696d 6973 6174 696f 6e20 416c   Optimisation Al
+00004100: 676f 7269 7468 6d20 666f 7220 5265 6163  gorithm for Reac
+00004110: 7469 7665 204d 6f74 696f 6e20 436f 6e74  tive Motion Cont
+00004120: 726f 6c20 6f66 204d 616e 6970 756c 6174  rol of Manipulat
+00004130: 6f72 732a 2a2c 2220 696e 205f 4945 4545  ors**," in _IEEE
+00004140: 2052 6f62 6f74 6963 7320 616e 6420 4175   Robotics and Au
+00004150: 746f 6d61 7469 6f6e 204c 6574 7465 7273  tomation Letters
+00004160: 5f2c 2064 6f69 3a20 3130 2e31 3130 392f  _, doi: 10.1109/
+00004170: 4c52 412e 3230 3231 2e33 3035 3630 3630  LRA.2021.3056060
+00004180: 2e20 496e 2074 6865 2076 6964 656f 2c20  . In the video, 
+00004190: 7468 6520 726f 626f 7420 6973 2063 6f6e  the robot is con
+000041a0: 7472 6f6c 6c65 6420 7573 696e 6720 7468  trolled using th
+000041b0: 6520 526f 626f 7469 6373 2074 6f6f 6c62  e Robotics toolb
+000041c0: 6f78 2066 6f72 2050 7974 686f 6e20 616e  ox for Python an
+000041d0: 6420 6665 6174 7572 6573 2061 2072 6563  d features a rec
+000041e0: 6f72 6469 6e67 2066 726f 6d20 7468 6520  ording from the 
+000041f0: 5b53 7769 6674 5d28 6874 7470 733a 2f2f  [Swift](https://
+00004200: 6769 7468 7562 2e63 6f6d 2f6a 6861 766c  github.com/jhavl
+00004210: 2f73 7769 6674 2920 5369 6d75 6c61 746f  /swift) Simulato
+00004220: 722e 0a0a 5b5b 4172 7869 7620 5061 7065  r...[[Arxiv Pape
+00004230: 725d 2868 7474 7073 3a2f 2f61 7278 6976  r](https://arxiv
+00004240: 2e6f 7267 2f61 6273 2f32 3031 302e 3038  .org/abs/2010.08
+00004250: 3638 3629 5d20 5b5b 4945 4545 2058 706c  686)] [[IEEE Xpl
+00004260: 6f72 655d 2868 7474 7073 3a2f 2f69 6565  ore](https://iee
+00004270: 6578 706c 6f72 652e 6965 6565 2e6f 7267  explore.ieee.org
+00004280: 2f64 6f63 756d 656e 742f 3933 3433 3731  /document/934371
+00004290: 3829 5d20 5b5b 5072 6f6a 6563 7420 5765  8)] [[Project We
+000042a0: 6273 6974 655d 2868 7474 7073 3a2f 2f6a  bsite](https://j
+000042b0: 6861 766c 2e67 6974 6875 622e 696f 2f6e  havl.github.io/n
+000042c0: 656f 2f29 5d20 5b5b 5669 6465 6f5d 2868  eo/)] [[Video](h
+000042d0: 7474 7073 3a2f 2f79 6f75 7475 2e62 652f  ttps://youtu.be/
+000042e0: 6a53 4c50 4a42 7238 5154 5929 5d20 5b5b  jSLPJBr8QTY)] [[
+000042f0: 436f 6465 2045 7861 6d70 6c65 5d28 6874  Code Example](ht
+00004300: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00004310: 2f70 6574 6572 636f 726b 652f 726f 626f  /petercorke/robo
+00004320: 7469 6373 2d74 6f6f 6c62 6f78 2d70 7974  tics-toolbox-pyt
+00004330: 686f 6e2f 626c 6f62 2f6d 6173 7465 722f  hon/blob/master/
+00004340: 726f 626f 7469 6373 746f 6f6c 626f 782f  roboticstoolbox/
+00004350: 6578 616d 706c 6573 2f6e 656f 2e70 7929  examples/neo.py)
+00004360: 5d0a 0a3c 703e 0a20 203c 6120 6872 6566  ]..<p>.  <a href
+00004370: 3d22 6874 7470 733a 2f2f 796f 7574 752e  ="https://youtu.
+00004380: 6265 2f6a 534c 504a 4272 3851 5459 223e  be/jSLPJBr8QTY">
+00004390: 0a20 2020 203c 696d 6720 7372 633d 2268  .    <img src="h
+000043a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000043b0: 6d2f 7065 7465 7263 6f72 6b65 2f72 6f62  m/petercorke/rob
+000043c0: 6f74 6963 732d 746f 6f6c 626f 782d 7079  otics-toolbox-py
+000043d0: 7468 6f6e 2f72 6177 2f6d 6173 7465 722f  thon/raw/master/
+000043e0: 646f 6373 2f66 6967 732f 6e65 6f5f 796f  docs/figs/neo_yo
+000043f0: 7574 7562 652e 706e 6722 2077 6964 7468  utube.png" width
+00004400: 3d22 3536 3022 3e0a 2020 3c2f 613e 0a3c  ="560">.  </a>.<
+00004410: 2f70 3e0a 0a2a 2a41 2050 7572 656c 792d  /p>..**A Purely-
+00004420: 5265 6163 7469 7665 204d 616e 6970 756c  Reactive Manipul
+00004430: 6162 696c 6974 792d 4d61 7869 6d69 7369  ability-Maximisi
+00004440: 6e67 204d 6f74 696f 6e20 436f 6e74 726f  ng Motion Contro
+00004450: 6c6c 6572 2a2a 2c20 4a2e 2048 6176 696c  ller**, J. Havil
+00004460: 616e 6420 616e 6420 502e 2043 6f72 6b65  and and P. Corke
+00004470: 2e20 496e 2074 6865 2076 6964 656f 2c20  . In the video, 
+00004480: 7468 6520 726f 626f 7420 6973 2063 6f6e  the robot is con
+00004490: 7472 6f6c 6c65 6420 7573 696e 6720 7468  trolled using th
+000044a0: 6520 526f 626f 7469 6373 2074 6f6f 6c62  e Robotics toolb
+000044b0: 6f78 2066 6f72 2050 7974 686f 6e2e 0a0a  ox for Python...
+000044c0: 5b5b 5061 7065 725d 2868 7474 7073 3a2f  [[Paper](https:/
+000044d0: 2f61 7278 6976 2e6f 7267 2f61 6273 2f32  /arxiv.org/abs/2
+000044e0: 3030 322e 3131 3930 3129 5d20 5b5b 5072  002.11901)] [[Pr
+000044f0: 6f6a 6563 7420 5765 6273 6974 655d 2868  oject Website](h
+00004500: 7474 7073 3a2f 2f6a 6861 766c 2e67 6974  ttps://jhavl.git
+00004510: 6875 622e 696f 2f6d 6d63 2f29 5d20 5b5b  hub.io/mmc/)] [[
+00004520: 5669 6465 6f5d 2868 7474 7073 3a2f 2f79  Video](https://y
+00004530: 6f75 7475 2e62 652f 5675 5f72 6350 6c61  outu.be/Vu_rcPla
+00004540: 4144 4929 5d20 5b5b 436f 6465 2045 7861  ADI)] [[Code Exa
+00004550: 6d70 6c65 5d28 6874 7470 733a 2f2f 6769  mple](https://gi
+00004560: 7468 7562 2e63 6f6d 2f70 6574 6572 636f  thub.com/peterco
+00004570: 726b 652f 726f 626f 7469 6373 2d74 6f6f  rke/robotics-too
+00004580: 6c62 6f78 2d70 7974 686f 6e2f 626c 6f62  lbox-python/blob
+00004590: 2f6d 6173 7465 722f 726f 626f 7469 6373  /master/robotics
+000045a0: 746f 6f6c 626f 782f 6578 616d 706c 6573  toolbox/examples
+000045b0: 2f6d 6d63 2e70 7929 5d0a 0a3c 703e 0a20  /mmc.py)]..<p>. 
+000045c0: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+000045d0: 2f2f 796f 7574 752e 6265 2f56 755f 7263  //youtu.be/Vu_rc
+000045e0: 506c 6141 4449 223e 0a20 2020 203c 696d  PlaADI">.    <im
+000045f0: 6720 7372 633d 2268 7474 7073 3a2f 2f67  g src="https://g
+00004600: 6974 6875 622e 636f 6d2f 7065 7465 7263  ithub.com/peterc
+00004610: 6f72 6b65 2f72 6f62 6f74 6963 732d 746f  orke/robotics-to
+00004620: 6f6c 626f 782d 7079 7468 6f6e 2f72 6177  olbox-python/raw
+00004630: 2f6d 6173 7465 722f 646f 6373 2f66 6967  /master/docs/fig
+00004640: 732f 6d6d 635f 796f 7574 7562 652e 706e  s/mmc_youtube.pn
+00004650: 6722 2077 6964 7468 3d22 3536 3022 3e0a  g" width="560">.
+00004660: 2020 3c2f 613e 0a3c 2f70 3e0a 0a3c 6272    </a>.</p>..<br
+00004670: 3e0a 0a3c 6272 3e0a 0a3c 6120 6964 3d27  >..<br>..<a id='
+00004680: 3627 3e3c 2f61 3e0a 0a23 2320 546f 6f6c  6'></a>..## Tool
+00004690: 626f 7820 4943 5241 2050 6170 6572 2061  box ICRA Paper a
+000046a0: 6e64 2043 6974 6174 696f 6e20 496e 666f  nd Citation Info
+000046b0: 0a0a 4368 6563 6b20 6f75 7420 6f75 7220  ..Check out our 
+000046c0: 4943 5241 2032 3032 3120 7061 7065 7220  ICRA 2021 paper 
+000046d0: 6f6e 205b 4945 4545 2058 706c 6f72 655d  on [IEEE Xplore]
+000046e0: 2868 7474 7073 3a2f 2f69 6565 6578 706c  (https://ieeexpl
+000046f0: 6f72 652e 6965 6565 2e6f 7267 2f64 6f63  ore.ieee.org/doc
+00004700: 756d 656e 742f 3935 3631 3336 3629 206f  ument/9561366) o
+00004710: 7220 6765 7420 7468 6520 5044 4620 6672  r get the PDF fr
+00004720: 6f6d 205b 5065 7465 7227 7320 7765 6273  om [Peter's webs
+00004730: 6974 655d 2868 7474 7073 3a2f 2f62 6974  ite](https://bit
+00004740: 2e6c 792f 3343 6863 794e 7029 2e0a 0a49  .ly/3ChcyNp)...I
+00004750: 6620 7468 6520 746f 6f6c 626f 7820 6865  f the toolbox he
+00004760: 6c70 6564 2079 6f75 2069 6e20 796f 7572  lped you in your
+00004770: 2072 6573 6561 7263 682c 2070 6c65 6173   research, pleas
+00004780: 6520 6369 7465 0a0a 6060 600a 4069 6e70  e cite..```.@inp
+00004790: 726f 6365 6564 696e 6773 7b72 7462 2c0a  roceedings{rtb,.
+000047a0: 2020 7469 746c 653d 7b4e 6f74 2079 6f75    title={Not you
+000047b0: 7220 6772 616e 646d 6f74 6865 72e2 8099  r grandmother...
+000047c0: 7320 746f 6f6c 626f 782d 2d74 6865 2052  s toolbox--the R
+000047d0: 6f62 6f74 6963 7320 546f 6f6c 626f 7820  obotics Toolbox 
+000047e0: 7265 696e 7665 6e74 6564 2066 6f72 2050  reinvented for P
+000047f0: 7974 686f 6e7d 2c0a 2020 6175 7468 6f72  ython},.  author
+00004800: 3d7b 436f 726b 652c 2050 6574 6572 2061  ={Corke, Peter a
+00004810: 6e64 2048 6176 696c 616e 642c 204a 6573  nd Haviland, Jes
+00004820: 7365 7d2c 0a20 2062 6f6f 6b74 6974 6c65  se},.  booktitle
+00004830: 3d7b 3230 3231 2049 4545 4520 496e 7465  ={2021 IEEE Inte
+00004840: 726e 6174 696f 6e61 6c20 436f 6e66 6572  rnational Confer
+00004850: 656e 6365 206f 6e20 526f 626f 7469 6373  ence on Robotics
+00004860: 2061 6e64 2041 7574 6f6d 6174 696f 6e20   and Automation 
+00004870: 2849 4352 4129 7d2c 0a20 2070 6167 6573  (ICRA)},.  pages
+00004880: 3d7b 3131 3335 372d 2d31 3133 3633 7d2c  ={11357--11363},
+00004890: 0a20 2079 6561 723d 7b32 3032 317d 2c0a  .  year={2021},.
+000048a0: 2020 6f72 6761 6e69 7a61 7469 6f6e 3d7b    organization={
+000048b0: 4945 4545 7d0a 7d0a 6060 600a 0a3c 6272  IEEE}.}.```..<br
+000048c0: 3e0a 0a3c 6120 6964 3d27 3727 3e3c 2f61  >..<a id='7'></a
+000048d0: 3e0a 0a23 2320 5573 696e 6720 7468 6520  >..## Using the 
+000048e0: 546f 6f6c 626f 7820 696e 2079 6f75 7220  Toolbox in your 
+000048f0: 4f70 656e 2053 6f75 7263 6520 436f 6465  Open Source Code
+00004900: 3f0a 0a49 6620 796f 7520 6172 6520 7573  ?..If you are us
+00004910: 696e 6720 7468 6520 546f 6f6c 626f 7820  ing the Toolbox 
+00004920: 696e 2079 6f75 7220 6f70 656e 2073 6f75  in your open sou
+00004930: 7263 6520 636f 6465 2c20 6665 656c 2066  rce code, feel f
+00004940: 7265 6520 746f 2061 6464 206f 7572 2062  ree to add our b
+00004950: 6164 6765 2074 6f20 796f 7572 2072 6561  adge to your rea
+00004960: 646d 6521 0a0a 466f 7220 7468 6520 706f  dme!..For the po
+00004970: 7765 7265 6420 6279 2072 6f62 6f74 6963  wered by robotic
+00004980: 7320 746f 6f6c 626f 7820 6261 6467 650a  s toolbox badge.
+00004990: 0a5b 215b 506f 7765 7265 6420 6279 2074  .[![Powered by t
+000049a0: 6865 2052 6f62 6f74 6963 7320 546f 6f6c  he Robotics Tool
+000049b0: 626f 785d 2868 7474 7073 3a2f 2f72 6177  box](https://raw
+000049c0: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+000049d0: 6e74 2e63 6f6d 2f70 6574 6572 636f 726b  nt.com/petercork
+000049e0: 652f 726f 626f 7469 6373 2d74 6f6f 6c62  e/robotics-toolb
+000049f0: 6f78 2d70 7974 686f 6e2f 6d61 7374 6572  ox-python/master
+00004a00: 2f2e 6769 7468 7562 2f73 7667 2f72 7462  /.github/svg/rtb
+00004a10: 5f70 6f77 6572 6564 2e6d 696e 2e73 7667  _powered.min.svg
+00004a20: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
+00004a30: 622e 636f 6d2f 7065 7465 7263 6f72 6b65  b.com/petercorke
+00004a40: 2f72 6f62 6f74 6963 732d 746f 6f6c 626f  /robotics-toolbo
+00004a50: 782d 7079 7468 6f6e 290a 0a63 6f70 7920  x-python)..copy 
+00004a60: 7468 6520 666f 6c6c 6f77 696e 670a 0a60  the following..`
+00004a70: 6060 0a5b 215b 506f 7765 7265 6420 6279  ``.[![Powered by
+00004a80: 2074 6865 2052 6f62 6f74 6963 7320 546f   the Robotics To
+00004a90: 6f6c 626f 785d 2868 7474 7073 3a2f 2f72  olbox](https://r
+00004aa0: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
+00004ab0: 7465 6e74 2e63 6f6d 2f70 6574 6572 636f  tent.com/peterco
+00004ac0: 726b 652f 726f 626f 7469 6373 2d74 6f6f  rke/robotics-too
+00004ad0: 6c62 6f78 2d70 7974 686f 6e2f 6d61 7374  lbox-python/mast
+00004ae0: 6572 2f2e 6769 7468 7562 2f73 7667 2f72  er/.github/svg/r
+00004af0: 7462 5f70 6f77 6572 6564 2e6d 696e 2e73  tb_powered.min.s
+00004b00: 7667 295d 2868 7474 7073 3a2f 2f67 6974  vg)](https://git
+00004b10: 6875 622e 636f 6d2f 7065 7465 7263 6f72  hub.com/petercor
+00004b20: 6b65 2f72 6f62 6f74 6963 732d 746f 6f6c  ke/robotics-tool
+00004b30: 626f 782d 7079 7468 6f6e 290a 6060 600a  box-python).```.
+00004b40: 0a46 6f72 2074 6865 2070 6f77 6572 6564  .For the powered
+00004b50: 2062 7920 7079 7468 6f6e 2072 6f62 6f74   by python robot
+00004b60: 6963 7320 6261 6467 650a 0a5b 215b 506f  ics badge..[![Po
+00004b70: 7765 7265 6420 6279 2050 7974 686f 6e20  wered by Python 
+00004b80: 526f 626f 7469 6373 5d28 6874 7470 733a  Robotics](https:
+00004b90: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
+00004ba0: 636f 6e74 656e 742e 636f 6d2f 7065 7465  content.com/pete
+00004bb0: 7263 6f72 6b65 2f72 6f62 6f74 6963 732d  rcorke/robotics-
+00004bc0: 746f 6f6c 626f 782d 7079 7468 6f6e 2f6d  toolbox-python/m
+00004bd0: 6173 7465 722f 2e67 6974 6875 622f 7376  aster/.github/sv
+00004be0: 672f 7072 5f70 6f77 6572 6564 2e6d 696e  g/pr_powered.min
+00004bf0: 2e73 7667 295d 2868 7474 7073 3a2f 2f67  .svg)](https://g
+00004c00: 6974 6875 622e 636f 6d2f 7065 7465 7263  ithub.com/peterc
+00004c10: 6f72 6b65 2f72 6f62 6f74 6963 732d 746f  orke/robotics-to
+00004c20: 6f6c 626f 782d 7079 7468 6f6e 290a 0a63  olbox-python)..c
+00004c30: 6f70 7920 7468 6520 666f 6c6c 6f77 696e  opy the followin
+00004c40: 670a 0a60 6060 0a5b 215b 506f 7765 7265  g..```.[![Powere
+00004c50: 6420 6279 2050 7974 686f 6e20 526f 626f  d by Python Robo
+00004c60: 7469 6373 5d28 6874 7470 733a 2f2f 7261  tics](https://ra
+00004c70: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
+00004c80: 656e 742e 636f 6d2f 7065 7465 7263 6f72  ent.com/petercor
+00004c90: 6b65 2f72 6f62 6f74 6963 732d 746f 6f6c  ke/robotics-tool
+00004ca0: 626f 782d 7079 7468 6f6e 2f6d 6173 7465  box-python/maste
+00004cb0: 722f 2e67 6974 6875 622f 7376 672f 7072  r/.github/svg/pr
+00004cc0: 5f70 6f77 6572 6564 2e6d 696e 2e73 7667  _powered.min.svg
+00004cd0: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
+00004ce0: 622e 636f 6d2f 7065 7465 7263 6f72 6b65  b.com/petercorke
+00004cf0: 2f72 6f62 6f74 6963 732d 746f 6f6c 626f  /robotics-toolbo
+00004d00: 782d 7079 7468 6f6e 290a 6060 600a 0a3c  x-python).```..<
+00004d10: 6272 3e0a 0a3c 6120 6964 3d27 3827 3e3c  br>..<a id='8'><
+00004d20: 2f61 3e0a 0a23 2320 436f 6d6d 6f6e 2049  /a>..## Common I
+00004d30: 7373 7565 7320 616e 6420 536f 6c75 7469  ssues and Soluti
+00004d40: 6f6e 730a 0a53 6565 2074 6865 2063 6f6d  ons..See the com
+00004d50: 6d6f 6e20 6973 7375 6573 2077 6974 6820  mon issues with 
+00004d60: 6669 7865 7320 5b68 6572 655d 2868 7474  fixes [here](htt
+00004d70: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00004d80: 7065 7465 7263 6f72 6b65 2f72 6f62 6f74  petercorke/robot
+00004d90: 6963 732d 746f 6f6c 626f 782d 7079 7468  ics-toolbox-pyth
+00004da0: 6f6e 2f77 696b 692f 436f 6d6d 6f6e 2d49  on/wiki/Common-I
+00004db0: 7373 7565 7329 2e0a                      ssues)..
```

### Comparing `roboticstoolbox-python-1.1.0/roboticstoolbox_python.egg-info/SOURCES.txt` & `roboticstoolbox_python-1.1.1/roboticstoolbox_python.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -14,22 +14,25 @@
 roboticstoolbox/backends/__init__.py
 roboticstoolbox/backends/PyPlot/EllipsePlot.py
 roboticstoolbox/backends/PyPlot/PyPlot.py
 roboticstoolbox/backends/PyPlot/PyPlot2.py
 roboticstoolbox/backends/PyPlot/RobotPlot.py
 roboticstoolbox/backends/PyPlot/RobotPlot2.py
 roboticstoolbox/backends/PyPlot/__init__.py
+roboticstoolbox/backends/PyPlot/test1.py
+roboticstoolbox/backends/PyPlot/test2.py
 roboticstoolbox/backends/swift/__init__.py
 roboticstoolbox/bin/__init__.py
 roboticstoolbox/bin/rtbtool.py
 roboticstoolbox/blocks/__init__.py
 roboticstoolbox/blocks/arm.py
 roboticstoolbox/blocks/mobile.py
 roboticstoolbox/blocks/quad_model.py
 roboticstoolbox/blocks/spatial.py
+roboticstoolbox/blocks/test.py
 roboticstoolbox/blocks/uav.py
 roboticstoolbox/core/fknm.cpp
 roboticstoolbox/core/fknm.h
 roboticstoolbox/core/frne.c
 roboticstoolbox/core/frne.h
 roboticstoolbox/core/ik.cpp
 roboticstoolbox/core/ik.h
@@ -378,17 +381,22 @@
 roboticstoolbox/core/Eigen/src/plugins/IndexedViewMethods.h
 roboticstoolbox/core/Eigen/src/plugins/MatrixCwiseBinaryOps.h
 roboticstoolbox/core/Eigen/src/plugins/MatrixCwiseUnaryOps.h
 roboticstoolbox/core/Eigen/src/plugins/ReshapedMethods.h
 roboticstoolbox/examples/RRMC.py
 roboticstoolbox/examples/RRMC_swift.py
 roboticstoolbox/examples/__init__.py
+roboticstoolbox/examples/armer.py
+roboticstoolbox/examples/aside.py
 roboticstoolbox/examples/baur.py
 roboticstoolbox/examples/branched_robot.py
+roboticstoolbox/examples/colors.py
+roboticstoolbox/examples/eg2.py
 roboticstoolbox/examples/eigdemo.py
+roboticstoolbox/examples/erobot-test.py
 roboticstoolbox/examples/fetch_vision.py
 roboticstoolbox/examples/holistic_mm_non_holonomic.py
 roboticstoolbox/examples/holistic_mm_omni.py
 roboticstoolbox/examples/icra2021.py
 roboticstoolbox/examples/ik_exp.py
 roboticstoolbox/examples/ik_speed.py
 roboticstoolbox/examples/ikine_evaluate.py
@@ -396,47 +404,68 @@
 roboticstoolbox/examples/mexican-wave.py
 roboticstoolbox/examples/mmc.py
 roboticstoolbox/examples/mobile.py
 roboticstoolbox/examples/neo.py
 roboticstoolbox/examples/park.py
 roboticstoolbox/examples/plot.py
 roboticstoolbox/examples/plot_swift.py
+roboticstoolbox/examples/poly_example.py
 roboticstoolbox/examples/puma_fdyn.py
 roboticstoolbox/examples/puma_jtraj.py
 roboticstoolbox/examples/puma_swift.py
 roboticstoolbox/examples/readme.py
 roboticstoolbox/examples/robots.py
 roboticstoolbox/examples/swift_recording.py
 roboticstoolbox/examples/teach.py
 roboticstoolbox/examples/teach_swift.py
 roboticstoolbox/examples/test.py
+roboticstoolbox/examples/test1.py
+roboticstoolbox/examples/test_et.py
+roboticstoolbox/examples/timing.py
 roboticstoolbox/examples/tripleangledemo.py
 roboticstoolbox/examples/twistdemo.py
 roboticstoolbox/examples/vehicle1.py
 roboticstoolbox/mobile/Animations.py
 roboticstoolbox/mobile/Bug2.py
 roboticstoolbox/mobile/CurvaturePolyPlanner.py
+roboticstoolbox/mobile/CurvaturePolyPlanner.py-new.py
 roboticstoolbox/mobile/DistanceTransformPlanner.py
+roboticstoolbox/mobile/DstarPlanner-nearly.py
+roboticstoolbox/mobile/DstarPlanner-old.py
 roboticstoolbox/mobile/DstarPlanner.py
 roboticstoolbox/mobile/DubinsPlanner.py
 roboticstoolbox/mobile/EKF.py
 roboticstoolbox/mobile/LatticePlanner.py
 roboticstoolbox/mobile/OccGrid.py
 roboticstoolbox/mobile/PRMPlanner.py
 roboticstoolbox/mobile/ParticleFilter.py
 roboticstoolbox/mobile/PlannerBase.py
 roboticstoolbox/mobile/PoseGraph.py
 roboticstoolbox/mobile/QuinticPolyPlanner.py
 roboticstoolbox/mobile/RRTPlanner.py
 roboticstoolbox/mobile/ReedsSheppPlanner.py
 roboticstoolbox/mobile/Vehicle.py
 roboticstoolbox/mobile/__init__.py
+roboticstoolbox/mobile/bug.py
+roboticstoolbox/mobile/distancexform.py
 roboticstoolbox/mobile/drivers.py
+roboticstoolbox/mobile/dubins_path_planning.py
 roboticstoolbox/mobile/landmarkmap.py
+roboticstoolbox/mobile/new.py
+roboticstoolbox/mobile/plot_vehicle.py
+roboticstoolbox/mobile/probabilistic_road_map.py
+roboticstoolbox/mobile/qtiming.py
+roboticstoolbox/mobile/reedsshepp-old.py
+roboticstoolbox/mobile/rrt.py
+roboticstoolbox/mobile/rrt_dubins.py
+roboticstoolbox/mobile/rrt_star.py
+roboticstoolbox/mobile/rrt_with_pathsmoothing.py
 roboticstoolbox/mobile/sensors.py
+roboticstoolbox/mobile/state_lattice_planner.py
+roboticstoolbox/mobile/test2.py
 roboticstoolbox/models/__init__.py
 roboticstoolbox/models/list.py
 roboticstoolbox/models/DH/AL5D.py
 roboticstoolbox/models/DH/Ball.py
 roboticstoolbox/models/DH/Baxter.py
 roboticstoolbox/models/DH/Cobra600.py
 roboticstoolbox/models/DH/Coil.py
@@ -457,21 +486,23 @@
 roboticstoolbox/models/DH/Stanford.py
 roboticstoolbox/models/DH/TwoLink.py
 roboticstoolbox/models/DH/UR10.py
 roboticstoolbox/models/DH/UR3.py
 roboticstoolbox/models/DH/UR5.py
 roboticstoolbox/models/DH/Uprighttl.py
 roboticstoolbox/models/DH/__init__.py
+roboticstoolbox/models/DH/arte_parse.py
 roboticstoolbox/models/ETS/Frankie.py
 roboticstoolbox/models/ETS/GenericSeven.py
 roboticstoolbox/models/ETS/Omni.py
 roboticstoolbox/models/ETS/Panda.py
 roboticstoolbox/models/ETS/Planar2.py
 roboticstoolbox/models/ETS/Planar_Y.py
 roboticstoolbox/models/ETS/Puma560.py
+roboticstoolbox/models/ETS/Puma560dh.py
 roboticstoolbox/models/ETS/XYPanda.py
 roboticstoolbox/models/ETS/__init__.py
 roboticstoolbox/models/URDF/AL5D.py
 roboticstoolbox/models/URDF/Fetch.py
 roboticstoolbox/models/URDF/FetchCamera.py
 roboticstoolbox/models/URDF/Frankie.py
 roboticstoolbox/models/URDF/FrankieOmni.py
@@ -509,14 +540,20 @@
 roboticstoolbox/robot/IK.py
 roboticstoolbox/robot/Link.py
 roboticstoolbox/robot/PoERobot.py
 roboticstoolbox/robot/Robot.py
 roboticstoolbox/robot/RobotKinematics.py
 roboticstoolbox/robot/RobotProto.py
 roboticstoolbox/robot/__init__.py
+roboticstoolbox/robot/symsimp.py
+roboticstoolbox/robot/symsimp2.py
+roboticstoolbox/robot/test-plot.py
+roboticstoolbox/robot/test_fkine.py
+roboticstoolbox/robot/test_invdyn.py
+roboticstoolbox/robot/timing_dynamics.py
 roboticstoolbox/tools/DHFactor.py
 roboticstoolbox/tools/Ticker.py
 roboticstoolbox/tools/__init__.py
 roboticstoolbox/tools/data.py
 roboticstoolbox/tools/jsingu.py
 roboticstoolbox/tools/null.py
 roboticstoolbox/tools/numerical.py
```

### Comparing `roboticstoolbox-python-1.1.0/setup.py` & `roboticstoolbox_python-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/tests/test_BaseRobot.py` & `roboticstoolbox_python-1.1.1/tests/test_BaseRobot.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/tests/test_CustomXacro.py` & `roboticstoolbox_python-1.1.1/tests/test_CustomXacro.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/tests/test_DHRobot.py` & `roboticstoolbox_python-1.1.1/tests/test_DHRobot.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/tests/test_ELink.py` & `roboticstoolbox_python-1.1.1/tests/test_ELink.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/tests/test_ERobot.py` & `roboticstoolbox_python-1.1.1/tests/test_ERobot.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/tests/test_ET.py` & `roboticstoolbox_python-1.1.1/tests/test_ET.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/tests/test_ETS.py` & `roboticstoolbox_python-1.1.1/tests/test_ETS.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/tests/test_ETS2.py` & `roboticstoolbox_python-1.1.1/tests/test_ETS2.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/tests/test_Gripper.py` & `roboticstoolbox_python-1.1.1/tests/test_Gripper.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/tests/test_IK.py` & `roboticstoolbox_python-1.1.1/tests/test_IK.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/tests/test_Link.py` & `roboticstoolbox_python-1.1.1/tests/test_Link.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/tests/test_PyPlot.py` & `roboticstoolbox_python-1.1.1/tests/test_PyPlot.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/tests/test_PyPlot2.py` & `roboticstoolbox_python-1.1.1/tests/test_PyPlot2.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/tests/test_Robot.py` & `roboticstoolbox_python-1.1.1/tests/test_Robot.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/tests/test_VPython.py` & `roboticstoolbox_python-1.1.1/tests/test_VPython.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/tests/test_blocks.py` & `roboticstoolbox_python-1.1.1/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/tests/test_fknm.py` & `roboticstoolbox_python-1.1.1/tests/test_fknm.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/tests/test_jacob.py` & `roboticstoolbox_python-1.1.1/tests/test_jacob.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/tests/test_mobile.py` & `roboticstoolbox_python-1.1.1/tests/test_mobile.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/tests/test_mobile_planner.py` & `roboticstoolbox_python-1.1.1/tests/test_mobile_planner.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/tests/test_models.py` & `roboticstoolbox_python-1.1.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/tests/test_tools.py` & `roboticstoolbox_python-1.1.1/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `roboticstoolbox-python-1.1.0/tests/test_trajectory.py` & `roboticstoolbox_python-1.1.1/tests/test_trajectory.py`

 * *Files identical despite different names*

