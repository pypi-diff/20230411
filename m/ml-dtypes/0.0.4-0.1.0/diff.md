# Comparing `tmp/ml_dtypes-0.0.4.tar.gz` & `tmp/ml_dtypes-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_dtypes-0.0.4.tar", last modified: Mon Mar 27 19:05:13 2023, max compression
+gzip compressed data, was "ml_dtypes-0.1.0.tar", last modified: Tue Apr 11 20:49:30 2023, max compression
```

## Comparing `ml_dtypes-0.0.4.tar` & `ml_dtypes-0.1.0.tar`

### file list

```diff
@@ -1,238 +1,238 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:05:13.533271 ml_dtypes-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-03-27 19:04:56.000000 ml_dtypes-0.0.4/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-27 19:04:56.000000 ml_dtypes-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16727 2023-03-27 19:04:56.000000 ml_dtypes-0.0.4/LICENSE.eigen
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-27 19:04:56.000000 ml_dtypes-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15565 2023-03-27 19:05:13.533271 ml_dtypes-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-03-27 19:04:56.000000 ml_dtypes-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:05:13.501271 ml_dtypes-0.0.4/ml_dtypes/
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-03-27 19:04:56.000000 ml_dtypes-0.0.4/ml_dtypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-03-27 19:04:56.000000 ml_dtypes-0.0.4/ml_dtypes/_finfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:05:13.505271 ml_dtypes-0.0.4/ml_dtypes/_src/
--rw-r--r--   0 runner    (1001) docker     (123)    57117 2023-03-27 19:04:56.000000 ml_dtypes-0.0.4/ml_dtypes/_src/custom_float.h
--rw-r--r--   0 runner    (1001) docker     (123)     9022 2023-03-27 19:04:56.000000 ml_dtypes-0.0.4/ml_dtypes/_src/dtypes.cc
--rw-r--r--   0 runner    (1001) docker     (123)    37555 2023-03-27 19:04:56.000000 ml_dtypes-0.0.4/ml_dtypes/_src/float8.h
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-03-27 19:04:56.000000 ml_dtypes-0.0.4/ml_dtypes/_src/numpy.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-03-27 19:04:56.000000 ml_dtypes-0.0.4/ml_dtypes/_src/numpy.h
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 19:04:56.000000 ml_dtypes-0.0.4/ml_dtypes/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:05:13.505271 ml_dtypes-0.0.4/ml_dtypes/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    28910 2023-03-27 19:04:56.000000 ml_dtypes-0.0.4/ml_dtypes/tests/custom_float_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-03-27 19:04:56.000000 ml_dtypes-0.0.4/ml_dtypes/tests/finfo_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-03-27 19:04:56.000000 ml_dtypes-0.0.4/ml_dtypes/tests/metadata_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:05:13.501271 ml_dtypes-0.0.4/ml_dtypes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15565 2023-03-27 19:05:13.000000 ml_dtypes-0.0.4/ml_dtypes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10618 2023-03-27 19:05:13.000000 ml_dtypes-0.0.4/ml_dtypes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 19:05:13.000000 ml_dtypes-0.0.4/ml_dtypes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-03-27 19:05:13.000000 ml_dtypes-0.0.4/ml_dtypes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-27 19:05:13.000000 ml_dtypes-0.0.4/ml_dtypes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-03-27 19:04:56.000000 ml_dtypes-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 19:05:13.533271 ml_dtypes-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-03-27 19:04:56.000000 ml_dtypes-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:05:13.493271 ml_dtypes-0.0.4/third_party/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:05:13.493271 ml_dtypes-0.0.4/third_party/eigen/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:05:13.505271 ml_dtypes-0.0.4/third_party/eigen/Eigen/
--rw-r--r--   0 runner    (1001) docker     (123)    13374 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/Core
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:05:13.497271 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:05:13.521271 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/
--rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/ArithmeticSequence.h
--rw-r--r--   0 runner    (1001) docker     (123)    16400 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Array.h
--rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/ArrayBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/ArrayWrapper.h
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Assign.h
--rw-r--r--   0 runner    (1001) docker     (123)    41912 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/AssignEvaluator.h
--rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Assign_MKL.h
--rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/BandMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    19246 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Block.h
--rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/CommaInitializer.h
--rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/ConditionEstimator.h
--rw-r--r--   0 runner    (1001) docker     (123)    63843 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/CoreEvaluators.h
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/CoreIterators.h
--rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/CwiseBinaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)    37759 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/CwiseNullaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     8034 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/CwiseTernaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/CwiseUnaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/CwiseUnaryView.h
--rw-r--r--   0 runner    (1001) docker     (123)    32035 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/DenseBase.h
--rw-r--r--   0 runner    (1001) docker     (123)    24436 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/DenseCoeffsBase.h
--rw-r--r--   0 runner    (1001) docker     (123)    28937 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/DenseStorage.h
--rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Diagonal.h
--rw-r--r--   0 runner    (1001) docker     (123)    18129 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/DiagonalMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/DiagonalProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)    11413 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Dot.h
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/EigenBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/ForceAlignedAccess.h
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Fuzzy.h
--rw-r--r--   0 runner    (1001) docker     (123)    21625 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/GeneralProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)    49384 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/GenericPacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)    12188 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/GlobalFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/IO.h
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/IndexedView.h
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/InternalHeaderCheck.h
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Inverse.h
--rw-r--r--   0 runner    (1001) docker     (123)     7127 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Map.h
--rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/MapBase.h
--rw-r--r--   0 runner    (1001) docker     (123)    61532 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    13345 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/MathFunctionsImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)    24419 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Matrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    23983 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/MatrixBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/NestByValue.h
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/NoAlias.h
--rw-r--r--   0 runner    (1001) docker     (123)    13346 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/NumTraits.h
--rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/PartialReduxEvaluator.h
--rw-r--r--   0 runner    (1001) docker     (123)    20771 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/PermutationMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    48620 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/PlainObjectBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Product.h
--rw-r--r--   0 runner    (1001) docker     (123)    55121 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/ProductEvaluators.h
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Random.h
--rw-r--r--   0 runner    (1001) docker     (123)    19216 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Redux.h
--rw-r--r--   0 runner    (1001) docker     (123)    17769 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Ref.h
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Replicate.h
--rw-r--r--   0 runner    (1001) docker     (123)    16983 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Reshaped.h
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/ReturnByValue.h
--rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Reverse.h
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Select.h
--rw-r--r--   0 runner    (1001) docker     (123)    14908 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/SelfAdjointView.h
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/SelfCwiseBinaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)    16006 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/SkewSymmetricMatrix3.h
--rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Solve.h
--rw-r--r--   0 runner    (1001) docker     (123)     9332 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/SolveTriangular.h
--rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/SolverBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/StableNorm.h
--rw-r--r--   0 runner    (1001) docker     (123)    21245 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/StlIterators.h
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Stride.h
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Swap.h
--rw-r--r--   0 runner    (1001) docker     (123)    17669 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Transpose.h
--rw-r--r--   0 runner    (1001) docker     (123)    13603 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Transpositions.h
--rw-r--r--   0 runner    (1001) docker     (123)    38143 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/TriangularMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/VectorBlock.h
--rw-r--r--   0 runner    (1001) docker     (123)    35183 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/VectorwiseOp.h
--rw-r--r--   0 runner    (1001) docker     (123)    35231 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Visitor.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:05:13.497271 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:05:13.521271 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/AVX/
--rw-r--r--   0 runner    (1001) docker     (123)    14975 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/AVX/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/AVX/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    83727 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/AVX/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/AVX/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:05:13.521271 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/AVX512/
--rw-r--r--   0 runner    (1001) docker     (123)    15797 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/AVX512/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)    47758 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/AVX512/GemmKernel.h
--rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/AVX512/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)   110036 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/AVX512/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)    26497 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/AVX512/PacketMathFP16.h
--rw-r--r--   0 runner    (1001) docker     (123)    56830 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/AVX512/TrsmKernel.h
--rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/AVX512/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:05:13.521271 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/AltiVec/
--rw-r--r--   0 runner    (1001) docker     (123)    20546 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/AltiVec/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/AltiVec/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)   129018 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h
--rw-r--r--   0 runner    (1001) docker     (123)    28128 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h
--rw-r--r--   0 runner    (1001) docker     (123)    15819 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMAbfloat16.h
--rw-r--r--   0 runner    (1001) docker     (123)    91478 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixVectorProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)   119359 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/AltiVec/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:05:13.525271 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/Default/
--rw-r--r--   0 runner    (1001) docker     (123)    34597 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/Default/BFloat16.h
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/Default/ConjHelper.h
--rw-r--r--   0 runner    (1001) docker     (123)    94749 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h
--rw-r--r--   0 runner    (1001) docker     (123)    39550 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/Default/Half.h
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/Default/Settings.h
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/Default/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:05:13.525271 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/GPU/
--rw-r--r--   0 runner    (1001) docker     (123)    17981 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/GPU/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/GPU/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    58287 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/GPU/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)     9694 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/GPU/Tuple.h
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/GPU/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:05:13.497271 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/HIP/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:05:13.525271 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/HIP/hcc/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/HIP/hcc/math_constants.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:05:13.525271 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/MSA/
--rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/MSA/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)    16053 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/MSA/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    33649 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/MSA/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:05:13.525271 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/NEON/
--rw-r--r--   0 runner    (1001) docker     (123)    22034 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/NEON/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)     9906 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/NEON/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)   194432 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/NEON/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)    51898 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/NEON/TypeCasting.h
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/NEON/UnaryFunctors.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:05:13.525271 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/SSE/
--rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/SSE/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/SSE/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    72921 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/SSE/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/SSE/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:05:13.525271 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/SVE/
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/SVE/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    21184 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/SVE/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/SVE/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:05:13.525271 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/SYCL/
--rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/SYCL/InteropHeaders.h
--rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/SYCL/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    16205 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/SYCL/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)    21994 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/SYCL/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:05:13.529271 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/ZVector/
--rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/ZVector/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)     7927 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/ZVector/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    36916 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/ZVector/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:05:13.529271 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/functors/
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/functors/AssignmentFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)    31940 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/functors/BinaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/functors/NullaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/functors/StlFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/functors/TernaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)    45622 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/functors/UnaryFunctors.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:05:13.529271 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/
--rw-r--r--   0 runner    (1001) docker     (123)   140899 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/GeneralBlockPanelKernel.h
--rw-r--r--   0 runner    (1001) docker     (123)    19832 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    15819 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)    21745 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/GeneralMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/Parallelizer.h
--rw-r--r--   0 runner    (1001) docker     (123)    21343 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    11607 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/SelfadjointProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/SelfadjointRank2Update.h
--rw-r--r--   0 runner    (1001) docker     (123)    20980 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/TriangularMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    13904 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)    14886 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/TriangularMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)    19090 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/TriangularSolverMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/TriangularSolverVector.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:05:13.533271 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/util/
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/util/Assert.h
--rw-r--r--   0 runner    (1001) docker     (123)    26278 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/util/BlasUtil.h
--rw-r--r--   0 runner    (1001) docker     (123)    19362 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/util/ConfigureVectorization.h
--rw-r--r--   0 runner    (1001) docker     (123)    22214 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/util/Constants.h
--rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/util/DisableStupidWarnings.h
--rw-r--r--   0 runner    (1001) docker     (123)    15929 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/util/ForwardDeclarations.h
--rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/util/IndexedViewHelper.h
--rw-r--r--   0 runner    (1001) docker     (123)     9567 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/util/IntegralConstant.h
--rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/util/MKL_support.h
--rw-r--r--   0 runner    (1001) docker     (123)    48039 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/util/Macros.h
--rw-r--r--   0 runner    (1001) docker     (123)    49577 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/util/Memory.h
--rw-r--r--   0 runner    (1001) docker     (123)    20264 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/util/Meta.h
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/util/ReenableStupidWarnings.h
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/util/ReshapedHelper.h
--rw-r--r--   0 runner    (1001) docker     (123)     7810 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/util/Serializer.h
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/util/StaticAssert.h
--rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/util/SymbolicIndex.h
--rw-r--r--   0 runner    (1001) docker     (123)    35298 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/util/XprHelper.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:05:13.533271 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)    13721 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/plugins/ArrayCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)    22938 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/plugins/ArrayCwiseUnaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)    58948 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/plugins/BlockMethods.h
--rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/plugins/CommonCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/plugins/CommonCwiseUnaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)    12022 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/plugins/IndexedViewMethods.h
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/plugins/InternalHeaderCheck.h
--rw-r--r--   0 runner    (1001) docker     (123)    16947 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/plugins/MatrixCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/plugins/MatrixCwiseUnaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-03-27 19:05:00.000000 ml_dtypes-0.0.4/third_party/eigen/Eigen/src/plugins/ReshapedMethods.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.150654 ml_dtypes-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-11 20:49:12.000000 ml_dtypes-0.1.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-11 20:49:12.000000 ml_dtypes-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-04-11 20:49:12.000000 ml_dtypes-0.1.0/LICENSE.eigen
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-11 20:49:12.000000 ml_dtypes-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15618 2023-04-11 20:49:30.150654 ml_dtypes-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-11 20:49:12.000000 ml_dtypes-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.118654 ml_dtypes-0.1.0/ml_dtypes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-11 20:49:12.000000 ml_dtypes-0.1.0/ml_dtypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13399 2023-04-11 20:49:12.000000 ml_dtypes-0.1.0/ml_dtypes/_finfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.118654 ml_dtypes-0.1.0/ml_dtypes/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)    57117 2023-04-11 20:49:12.000000 ml_dtypes-0.1.0/ml_dtypes/_src/custom_float.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-04-11 20:49:12.000000 ml_dtypes-0.1.0/ml_dtypes/_src/dtypes.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    52762 2023-04-11 20:49:12.000000 ml_dtypes-0.1.0/ml_dtypes/_src/float8.h
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-11 20:49:12.000000 ml_dtypes-0.1.0/ml_dtypes/_src/numpy.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-11 20:49:12.000000 ml_dtypes-0.1.0/ml_dtypes/_src/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:12.000000 ml_dtypes-0.1.0/ml_dtypes/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.118654 ml_dtypes-0.1.0/ml_dtypes/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    29497 2023-04-11 20:49:12.000000 ml_dtypes-0.1.0/ml_dtypes/tests/custom_float_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-04-11 20:49:12.000000 ml_dtypes-0.1.0/ml_dtypes/tests/finfo_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-11 20:49:12.000000 ml_dtypes-0.1.0/ml_dtypes/tests/metadata_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.118654 ml_dtypes-0.1.0/ml_dtypes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15618 2023-04-11 20:49:30.000000 ml_dtypes-0.1.0/ml_dtypes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10618 2023-04-11 20:49:30.000000 ml_dtypes-0.1.0/ml_dtypes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 20:49:30.000000 ml_dtypes-0.1.0/ml_dtypes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-11 20:49:30.000000 ml_dtypes-0.1.0/ml_dtypes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-11 20:49:30.000000 ml_dtypes-0.1.0/ml_dtypes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-11 20:49:12.000000 ml_dtypes-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 20:49:30.150654 ml_dtypes-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-11 20:49:12.000000 ml_dtypes-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.114654 ml_dtypes-0.1.0/third_party/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.114654 ml_dtypes-0.1.0/third_party/eigen/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.118654 ml_dtypes-0.1.0/third_party/eigen/Eigen/
+-rw-r--r--   0 runner    (1001) docker     (123)    13374 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/Core
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.114654 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.130654 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/
+-rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/ArithmeticSequence.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16400 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Array.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/ArrayBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/ArrayWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Assign.h
+-rw-r--r--   0 runner    (1001) docker     (123)    41912 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/AssignEvaluator.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Assign_MKL.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/BandMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19246 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Block.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/CommaInitializer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/ConditionEstimator.h
+-rw-r--r--   0 runner    (1001) docker     (123)    63843 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/CoreEvaluators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/CoreIterators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/CwiseBinaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    37759 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/CwiseNullaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8034 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/CwiseTernaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/CwiseUnaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/CwiseUnaryView.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32035 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/DenseBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24436 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/DenseCoeffsBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28937 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/DenseStorage.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Diagonal.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18129 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/DiagonalMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/DiagonalProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11413 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Dot.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/EigenBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/ForceAlignedAccess.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Fuzzy.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21625 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/GeneralProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)    49384 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/GenericPacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12188 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/GlobalFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/IO.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/IndexedView.h
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/InternalHeaderCheck.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Inverse.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7127 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Map.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/MapBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    61532 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13345 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/MathFunctionsImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24419 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Matrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23983 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/MatrixBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/NestByValue.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/NoAlias.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13346 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/NumTraits.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/PartialReduxEvaluator.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20771 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/PermutationMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    48620 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/PlainObjectBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Product.h
+-rw-r--r--   0 runner    (1001) docker     (123)    55121 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/ProductEvaluators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Random.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19216 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Redux.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17769 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Ref.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Replicate.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16983 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Reshaped.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/ReturnByValue.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Reverse.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Select.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14908 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/SelfAdjointView.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/SelfCwiseBinaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16006 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/SkewSymmetricMatrix3.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Solve.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9332 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/SolveTriangular.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/SolverBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/StableNorm.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21245 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/StlIterators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Stride.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Swap.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17669 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Transpose.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13603 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Transpositions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    38143 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/TriangularMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/VectorBlock.h
+-rw-r--r--   0 runner    (1001) docker     (123)    35183 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/VectorwiseOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    35231 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Visitor.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.114654 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.130654 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX/
+-rw-r--r--   0 runner    (1001) docker     (123)    14975 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    83727 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.134654 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX512/
+-rw-r--r--   0 runner    (1001) docker     (123)    15797 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX512/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)    47758 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX512/GemmKernel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX512/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)   110036 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX512/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26497 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX512/PacketMathFP16.h
+-rw-r--r--   0 runner    (1001) docker     (123)    56830 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX512/TrsmKernel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX512/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.134654 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/
+-rw-r--r--   0 runner    (1001) docker     (123)    20546 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)   129018 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28128 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15819 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMAbfloat16.h
+-rw-r--r--   0 runner    (1001) docker     (123)    91478 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixVectorProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)   119359 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.134654 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/Default/
+-rw-r--r--   0 runner    (1001) docker     (123)    34597 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/Default/BFloat16.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/Default/ConjHelper.h
+-rw-r--r--   0 runner    (1001) docker     (123)    94749 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h
+-rw-r--r--   0 runner    (1001) docker     (123)    39550 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/Default/Half.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/Default/Settings.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/Default/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.138654 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/GPU/
+-rw-r--r--   0 runner    (1001) docker     (123)    17981 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/GPU/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/GPU/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    58287 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/GPU/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9694 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/GPU/Tuple.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/GPU/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.114654 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/HIP/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.138654 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/HIP/hcc/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/HIP/hcc/math_constants.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.138654 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/MSA/
+-rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/MSA/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16053 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/MSA/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    33649 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/MSA/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.138654 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/NEON/
+-rw-r--r--   0 runner    (1001) docker     (123)    22034 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/NEON/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9906 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/NEON/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)   194432 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/NEON/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)    51898 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/NEON/TypeCasting.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/NEON/UnaryFunctors.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.138654 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SSE/
+-rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SSE/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SSE/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    72921 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SSE/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SSE/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.138654 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SVE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SVE/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21184 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SVE/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SVE/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.142654 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SYCL/
+-rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SYCL/InteropHeaders.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SYCL/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16205 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SYCL/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21994 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SYCL/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.142654 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/ZVector/
+-rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/ZVector/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7927 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/ZVector/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    36916 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/ZVector/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.142654 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/functors/
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/functors/AssignmentFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31940 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/functors/BinaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/functors/NullaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/functors/StlFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/functors/TernaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)    45622 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/functors/UnaryFunctors.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.146654 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/
+-rw-r--r--   0 runner    (1001) docker     (123)   140899 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/GeneralBlockPanelKernel.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19832 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15819 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21745 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/GeneralMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/Parallelizer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21343 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11607 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/SelfadjointProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/SelfadjointRank2Update.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20980 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/TriangularMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13904 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14886 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/TriangularMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19090 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/TriangularSolverMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/TriangularSolverVector.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.150654 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/Assert.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26278 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/BlasUtil.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19362 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/ConfigureVectorization.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22214 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/Constants.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/DisableStupidWarnings.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15929 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/ForwardDeclarations.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/IndexedViewHelper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9567 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/IntegralConstant.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/MKL_support.h
+-rw-r--r--   0 runner    (1001) docker     (123)    48039 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/Macros.h
+-rw-r--r--   0 runner    (1001) docker     (123)    49577 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/Memory.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20264 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/Meta.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/ReenableStupidWarnings.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/ReshapedHelper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7810 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/Serializer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/StaticAssert.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/SymbolicIndex.h
+-rw-r--r--   0 runner    (1001) docker     (123)    35298 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/XprHelper.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:49:30.150654 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)    13721 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/plugins/ArrayCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22938 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/plugins/ArrayCwiseUnaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)    58948 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/plugins/BlockMethods.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/plugins/CommonCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/plugins/CommonCwiseUnaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12022 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/plugins/IndexedViewMethods.h
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/plugins/InternalHeaderCheck.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16947 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/plugins/MatrixCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/plugins/MatrixCwiseUnaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-04-11 20:49:17.000000 ml_dtypes-0.1.0/third_party/eigen/Eigen/src/plugins/ReshapedMethods.h
```

### Comparing `ml_dtypes-0.0.4/LICENSE` & `ml_dtypes-0.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -195,8 +195,8 @@
 
        http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
-   limitations under the License.
+   limitations under the License.
```

### Comparing `ml_dtypes-0.0.4/LICENSE.eigen` & `ml_dtypes-0.1.0/LICENSE.eigen`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         version 1.1 or earlier of the License, but not also under the
         terms of a Secondary License.
 
 1.6. "Executable Form"
     means any form of the work other than Source Code Form.
 
 1.7. "Larger Work"
-    means a work that combines Covered Software with other material, in 
+    means a work that combines Covered Software with other material, in
     a separate file or files, that is not Covered Software.
 
 1.8. "License"
     means this document.
 
 1.9. "Licensable"
     means having the right to grant, to the maximum extent possible,
```

### Comparing `ml_dtypes-0.0.4/PKG-INFO` & `ml_dtypes-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml_dtypes
-Version: 0.0.4
+Version: 0.1.0
 Author-email: ml_dtypes authors <ml_dtypes@google.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -200,14 +200,15 @@
                http://www.apache.org/licenses/LICENSE-2.0
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
+        
 Project-URL: homepage, https://github.com/jax-ml/ml_dtypes
 Project-URL: repository, https://github.com/jax-ml/ml_dtypes
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.7
@@ -229,15 +230,17 @@
 
 - [`bfloat16`](https://en.wikipedia.org/wiki/Bfloat16_floating-point_format):
   an alternative to the standard [`float16`](https://en.wikipedia.org/wiki/Half-precision_floating-point_format) format
 - `float8_*`: several experimental 8-bit floating point representations
   including:
   * `float8_e4m3b11`
   * `float8_e4m3fn`
+  * `float8_e4m3fnuz`
   * `float8_e5m2`
+  * `float8_e5m2fnuz`
 
 ## Installation
 
 The `ml_dtypes` package is tested with Python versions 3.8-3.11, and can be installed
 with the following command:
 ```
 pip install ml_dtypes
```

### Comparing `ml_dtypes-0.0.4/README.md` & `ml_dtypes-0.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 
 - [`bfloat16`](https://en.wikipedia.org/wiki/Bfloat16_floating-point_format):
   an alternative to the standard [`float16`](https://en.wikipedia.org/wiki/Half-precision_floating-point_format) format
 - `float8_*`: several experimental 8-bit floating point representations
   including:
   * `float8_e4m3b11`
   * `float8_e4m3fn`
+  * `float8_e4m3fnuz`
   * `float8_e5m2`
+  * `float8_e5m2fnuz`
 
 ## Installation
 
 The `ml_dtypes` package is tested with Python versions 3.8-3.11, and can be installed
 with the following command:
 ```
 pip install ml_dtypes
```

### Comparing `ml_dtypes-0.0.4/ml_dtypes/_finfo.py` & `ml_dtypes-0.1.0/ml_dtypes/_finfo.py`

 * *Files 27% similar despite different names*

```diff
@@ -15,22 +15,26 @@
 """Overload of numpy.finfo to handle dtypes defined in ml_dtypes."""
 
 from typing import Dict
 
 from ml_dtypes._custom_floats import bfloat16
 from ml_dtypes._custom_floats import float8_e4m3b11
 from ml_dtypes._custom_floats import float8_e4m3fn
+from ml_dtypes._custom_floats import float8_e4m3fnuz
 from ml_dtypes._custom_floats import float8_e5m2
+from ml_dtypes._custom_floats import float8_e5m2fnuz
 
 import numpy as np
 
 _bfloat16_dtype = np.dtype(bfloat16)
 _float8_e4m3b11_dtype = np.dtype(float8_e4m3b11)
 _float8_e4m3fn_dtype = np.dtype(float8_e4m3fn)
+_float8_e4m3fnuz_dtype = np.dtype(float8_e4m3fnuz)
 _float8_e5m2_dtype = np.dtype(float8_e5m2)
+_float8_e5m2fnuz_dtype = np.dtype(float8_e5m2fnuz)
 
 
 class _Bfloat16MachArLike:
 
   def __init__(self):
     smallest_normal = float.fromhex("0x1p-126")
     self.smallest_normal = bfloat16(smallest_normal)
@@ -52,23 +56,41 @@
   def __init__(self):
     smallest_normal = float.fromhex("0x1p-6")
     self.smallest_normal = float8_e4m3fn(smallest_normal)
     smallest_subnormal = float.fromhex("0x1p-9")
     self.smallest_subnormal = float8_e4m3fn(smallest_subnormal)
 
 
+class _Float8E4m3FnuzMachArLike:
+
+  def __init__(self):
+    smallest_normal = float.fromhex("0x1p-7")
+    self.smallest_normal = float8_e4m3fnuz(smallest_normal)
+    smallest_subnormal = float.fromhex("0x1p-10")
+    self.smallest_subnormal = float8_e4m3fnuz(smallest_subnormal)
+
+
 class _Float8E5m2MachArLike:
 
   def __init__(self):
     smallest_normal = float.fromhex("0x1p-14")
     self.smallest_normal = float8_e5m2(smallest_normal)
     smallest_subnormal = float.fromhex("0x1p-16")
     self.smallest_subnormal = float8_e5m2(smallest_subnormal)
 
 
+class _Float8E5m2FnuzMachArLike:
+
+  def __init__(self):
+    smallest_normal = float.fromhex("0x1p-15")
+    self.smallest_normal = float8_e5m2fnuz(smallest_normal)
+    smallest_subnormal = float.fromhex("0x1p-17")
+    self.smallest_subnormal = float8_e5m2fnuz(smallest_subnormal)
+
+
 class finfo(np.finfo):  # pylint: disable=invalid-name,missing-class-docstring
   __doc__ = np.finfo.__doc__
   _finfo_cache: Dict[np.dtype, np.finfo] = {}
 
   @staticmethod
   def _bfloat16_finfo():
     def float_to_str(f):
@@ -89,26 +111,28 @@
     obj.negep = -8
     obj.max = bfloat16(max_)
     obj.min = bfloat16(-max_)
     obj.nexp = 8
     obj.nmant = 7
     obj.iexp = obj.nexp
     obj.maxexp = 128
+    obj.minexp = -126
     obj.precision = 2
     obj.resolution = bfloat16(resolution)
     # pylint: disable=protected-access
     obj._machar = _Bfloat16MachArLike()
     if not hasattr(obj, "tiny"):
       obj.tiny = bfloat16(tiny)
     if not hasattr(obj, "smallest_normal"):
       obj.smallest_normal = obj._machar.smallest_normal
     obj.smallest_subnormal = obj._machar.smallest_subnormal
 
     obj._str_tiny = float_to_str(tiny)
     obj._str_smallest_normal = float_to_str(tiny)
+    obj._str_smallest_subnormal = float_to_str(obj.smallest_subnormal)
     obj._str_max = float_to_str(max_)
     obj._str_epsneg = float_to_str(epsneg)
     obj._str_eps = float_to_str(eps)
     obj._str_resolution = float_to_str(resolution)
     # pylint: enable=protected-access
     return obj
 
@@ -132,26 +156,28 @@
     obj.negep = -4
     obj.max = float8_e4m3b11(max_)
     obj.min = float8_e4m3b11(-max_)
     obj.nexp = 4
     obj.nmant = 3
     obj.iexp = obj.nexp
     obj.maxexp = 5
+    obj.minexp = -10
     obj.precision = 1
     obj.resolution = float8_e4m3b11(resolution)
     # pylint: disable=protected-access
     obj._machar = _Float8E4m3B11MachArLike()
     if not hasattr(obj, "tiny"):
       obj.tiny = float8_e4m3b11(tiny)
     if not hasattr(obj, "smallest_normal"):
       obj.smallest_normal = obj._machar.smallest_normal
     obj.smallest_subnormal = obj._machar.smallest_subnormal
 
     obj._str_tiny = float_to_str(tiny)
     obj._str_smallest_normal = float_to_str(tiny)
+    obj._str_smallest_subnormal = float_to_str(obj.smallest_subnormal)
     obj._str_max = float_to_str(max_)
     obj._str_epsneg = float_to_str(epsneg)
     obj._str_eps = float_to_str(eps)
     obj._str_resolution = float_to_str(resolution)
     # pylint: enable=protected-access
     return obj
 
@@ -175,26 +201,73 @@
     obj.negep = -4
     obj.max = float8_e4m3fn(max_)
     obj.min = float8_e4m3fn(-max_)
     obj.nexp = 4
     obj.nmant = 3
     obj.iexp = obj.nexp
     obj.maxexp = 9
+    obj.minexp = -6
     obj.precision = 1
     obj.resolution = float8_e4m3fn(resolution)
     # pylint: disable=protected-access
     obj._machar = _Float8E4m3FnMachArLike()
     if not hasattr(obj, "tiny"):
       obj.tiny = float8_e4m3fn(tiny)
     if not hasattr(obj, "smallest_normal"):
       obj.smallest_normal = obj._machar.smallest_normal
     obj.smallest_subnormal = obj._machar.smallest_subnormal
 
     obj._str_tiny = float_to_str(tiny)
     obj._str_smallest_normal = float_to_str(tiny)
+    obj._str_smallest_subnormal = float_to_str(obj.smallest_subnormal)
+    obj._str_max = float_to_str(max_)
+    obj._str_epsneg = float_to_str(epsneg)
+    obj._str_eps = float_to_str(eps)
+    obj._str_resolution = float_to_str(resolution)
+    # pylint: enable=protected-access
+    return obj
+
+  @staticmethod
+  def _float8_e4m3fnuz_finfo():
+    def float_to_str(f):
+      return "%6.2e" % float(f)
+
+    tiny = float.fromhex("0x1p-7")
+    resolution = 0.1
+    eps = float.fromhex("0x1p-3")
+    epsneg = float.fromhex("0x1p-4")
+    max_ = float.fromhex("0x1.Ep7")
+
+    obj = object.__new__(np.finfo)
+    obj.dtype = _float8_e4m3fnuz_dtype
+    obj.bits = 8
+    obj.eps = float8_e4m3fnuz(eps)
+    obj.epsneg = float8_e4m3fnuz(epsneg)
+    obj.machep = -3
+    obj.negep = -4
+    obj.max = float8_e4m3fnuz(max_)
+    obj.min = float8_e4m3fnuz(-max_)
+    obj.nexp = 4
+    obj.nmant = 3
+    obj.iexp = obj.nexp
+    obj.maxexp = 8
+    obj.minexp = -7
+    obj.precision = 1
+    obj.resolution = float8_e4m3fnuz(resolution)
+    # pylint: disable=protected-access
+    obj._machar = _Float8E4m3FnuzMachArLike()
+    if not hasattr(obj, "tiny"):
+      obj.tiny = float8_e4m3fnuz(tiny)
+    if not hasattr(obj, "smallest_normal"):
+      obj.smallest_normal = obj._machar.smallest_normal
+    obj.smallest_subnormal = obj._machar.smallest_subnormal
+
+    obj._str_tiny = float_to_str(tiny)
+    obj._str_smallest_normal = float_to_str(tiny)
+    obj._str_smallest_subnormal = float_to_str(obj.smallest_subnormal)
     obj._str_max = float_to_str(max_)
     obj._str_epsneg = float_to_str(epsneg)
     obj._str_eps = float_to_str(eps)
     obj._str_resolution = float_to_str(resolution)
     # pylint: enable=protected-access
     return obj
 
@@ -218,26 +291,73 @@
     obj.negep = -3
     obj.max = float8_e5m2(max_)
     obj.min = float8_e5m2(-max_)
     obj.nexp = 5
     obj.nmant = 2
     obj.iexp = obj.nexp
     obj.maxexp = 16
+    obj.minexp = -14
     obj.precision = 1
     obj.resolution = float8_e5m2(resolution)
     # pylint: disable=protected-access
     obj._machar = _Float8E5m2MachArLike()
     if not hasattr(obj, "tiny"):
       obj.tiny = float8_e5m2(tiny)
     if not hasattr(obj, "smallest_normal"):
       obj.smallest_normal = obj._machar.smallest_normal
     obj.smallest_subnormal = obj._machar.smallest_subnormal
 
     obj._str_tiny = float_to_str(tiny)
     obj._str_smallest_normal = float_to_str(tiny)
+    obj._str_smallest_subnormal = float_to_str(obj.smallest_subnormal)
+    obj._str_max = float_to_str(max_)
+    obj._str_epsneg = float_to_str(epsneg)
+    obj._str_eps = float_to_str(eps)
+    obj._str_resolution = float_to_str(resolution)
+    # pylint: enable=protected-access
+    return obj
+
+  @staticmethod
+  def _float8_e5m2fnuz_finfo():
+    def float_to_str(f):
+      return "%6.2e" % float(f)
+
+    tiny = float.fromhex("0x1p-15")
+    resolution = 0.1
+    eps = float.fromhex("0x1p-2")
+    epsneg = float.fromhex("0x1p-3")
+    max_ = float.fromhex("0x1.Cp15")
+
+    obj = object.__new__(np.finfo)
+    obj.dtype = _float8_e5m2fnuz_dtype
+    obj.bits = 8
+    obj.eps = float8_e5m2fnuz(eps)
+    obj.epsneg = float8_e5m2fnuz(epsneg)
+    obj.machep = -2
+    obj.negep = -3
+    obj.max = float8_e5m2fnuz(max_)
+    obj.min = float8_e5m2fnuz(-max_)
+    obj.nexp = 5
+    obj.nmant = 2
+    obj.iexp = obj.nexp
+    obj.maxexp = 16
+    obj.minexp = -15
+    obj.precision = 1
+    obj.resolution = float8_e5m2fnuz(resolution)
+    # pylint: disable=protected-access
+    obj._machar = _Float8E5m2FnuzMachArLike()
+    if not hasattr(obj, "tiny"):
+      obj.tiny = float8_e5m2fnuz(tiny)
+    if not hasattr(obj, "smallest_normal"):
+      obj.smallest_normal = obj._machar.smallest_normal
+    obj.smallest_subnormal = obj._machar.smallest_subnormal
+
+    obj._str_tiny = float_to_str(tiny)
+    obj._str_smallest_normal = float_to_str(tiny)
+    obj._str_smallest_subnormal = float_to_str(obj.smallest_subnormal)
     obj._str_max = float_to_str(max_)
     obj._str_epsneg = float_to_str(epsneg)
     obj._str_eps = float_to_str(eps)
     obj._str_resolution = float_to_str(resolution)
     # pylint: enable=protected-access
     return obj
 
@@ -264,14 +384,30 @@
         or dtype == _float8_e4m3fn_dtype
     ):
       if _float8_e4m3fn_dtype not in cls._finfo_cache:
         cls._finfo_cache[_float8_e4m3fn_dtype] = cls._float8_e4m3fn_finfo()
       return cls._finfo_cache[_float8_e4m3fn_dtype]
     if (
         isinstance(dtype, str)
+        and dtype == "float8_e4m3fnuz"
+        or dtype == _float8_e4m3fnuz_dtype
+    ):
+      if _float8_e4m3fnuz_dtype not in cls._finfo_cache:
+        cls._finfo_cache[_float8_e4m3fnuz_dtype] = cls._float8_e4m3fnuz_finfo()
+      return cls._finfo_cache[_float8_e4m3fnuz_dtype]
+    if (
+        isinstance(dtype, str)
         and dtype == "float8_e5m2"
         or dtype == _float8_e5m2_dtype
     ):
       if _float8_e5m2_dtype not in cls._finfo_cache:
         cls._finfo_cache[_float8_e5m2_dtype] = cls._float8_e5m2_finfo()
       return cls._finfo_cache[_float8_e5m2_dtype]
+    if (
+        isinstance(dtype, str)
+        and dtype == "float8_e5m2fnuz"
+        or dtype == _float8_e5m2fnuz_dtype
+    ):
+      if _float8_e5m2fnuz_dtype not in cls._finfo_cache:
+        cls._finfo_cache[_float8_e5m2fnuz_dtype] = cls._float8_e5m2fnuz_finfo()
+      return cls._finfo_cache[_float8_e5m2fnuz_dtype]
     return super().__new__(cls, dtype)
```

### Comparing `ml_dtypes-0.0.4/ml_dtypes/_src/custom_float.h` & `ml_dtypes-0.1.0/ml_dtypes/_src/custom_float.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/ml_dtypes/_src/dtypes.cc` & `ml_dtypes-0.1.0/ml_dtypes/_src/dtypes.cc`

 * *Files 18% similar despite different names*

```diff
@@ -89,27 +89,55 @@
   // TODO(phawkins): there doesn't seem to be a way of guaranteeing a type
   // character is unique.
   static constexpr char kNpyDescrType = '4';
   static constexpr char kNpyDescrByteorder = '=';
 };
 
 template <>
+struct TypeDescriptor<float8_e4m3fnuz>
+    : CustomFloatTypeDescriptor<float8_e4m3fnuz> {
+  typedef float8_e4m3fnuz T;
+  static constexpr const char* kTypeName = "float8_e4m3fnuz";
+  static constexpr const char* kQualifiedTypeName = "ml_dtypes.float8_e4m3fnuz";
+  static constexpr const char* kTpDoc = "float8_e4m3fnuz floating-point values";
+  static constexpr char kNpyDescrKind = 'V';
+  // TODO(phawkins): there doesn't seem to be a way of guaranteeing a type
+  // character is unique.
+  static constexpr char kNpyDescrType = 'G';
+  static constexpr char kNpyDescrByteorder = '=';
+};
+
+template <>
 struct TypeDescriptor<float8_e5m2> : CustomFloatTypeDescriptor<float8_e5m2> {
   typedef float8_e5m2 T;
   static constexpr const char* kTypeName = "float8_e5m2";
   static constexpr const char* kQualifiedTypeName = "ml_dtypes.float8_e5m2";
   static constexpr const char* kTpDoc = "float8_e5m2 floating-point values";
   // Treating e5m2 as the natural "float" type since it is IEEE-754 compliant.
   static constexpr char kNpyDescrKind = 'f';
   // TODO(phawkins): there doesn't seem to be a way of guaranteeing a type
   // character is unique.
   static constexpr char kNpyDescrType = '5';
   static constexpr char kNpyDescrByteorder = '=';
 };
 
+template <>
+struct TypeDescriptor<float8_e5m2fnuz>
+    : CustomFloatTypeDescriptor<float8_e5m2fnuz> {
+  typedef float8_e5m2fnuz T;
+  static constexpr const char* kTypeName = "float8_e5m2fnuz";
+  static constexpr const char* kQualifiedTypeName = "ml_dtypes.float8_e5m2fnuz";
+  static constexpr const char* kTpDoc = "float8_e5m2fnuz floating-point values";
+  static constexpr char kNpyDescrKind = 'V';
+  // TODO(phawkins): there doesn't seem to be a way of guaranteeing a type
+  // character is unique.
+  static constexpr char kNpyDescrType = 'C';
+  static constexpr char kNpyDescrByteorder = '=';
+};
+
 namespace {
 
 // Performs a NumPy array cast from type 'From' to 'To' via float.
 template <typename From, typename To>
 void FloatPyCast(void* from_void, void* to_void, npy_intp n, void* fromarr,
                  void* toarr) {
   const auto* from = static_cast<From*>(from_void);
@@ -161,40 +189,63 @@
     return false;
   }
   bool float8_e4m3fn_already_registered;
   if (!ml_dtypes::RegisterNumpyDtype<float8_e4m3fn>(
           numpy.get(), &float8_e4m3fn_already_registered)) {
     return false;
   }
+  bool float8_e4m3fnuz_already_registered;
+  if (!ml_dtypes::RegisterNumpyDtype<float8_e4m3fnuz>(
+          numpy.get(), &float8_e4m3fnuz_already_registered)) {
+    return false;
+  }
   bool float8_e5m2_already_registered;
   if (!ml_dtypes::RegisterNumpyDtype<float8_e5m2>(
           numpy.get(), &float8_e5m2_already_registered)) {
     return false;
   }
+  bool float8_e5m2fnuz_already_registered;
+  if (!ml_dtypes::RegisterNumpyDtype<float8_e5m2fnuz>(
+          numpy.get(), &float8_e5m2fnuz_already_registered)) {
+    return false;
+  }
 
   // Casts between bfloat16 and float8_e4m3b11. Only perform the cast if
   // float8_e4m3b11 hasn't been previously registered, presumably by a different
   // library. In this case, we assume the cast has also already been registered,
   // and registering it again can cause segfaults due to accessing an
   // uninitialized type descriptor in this library.
   if (!float8_e4m3b11_already_registered &&
       !RegisterCustomFloatCast<float8_e4m3b11, bfloat16>()) {
     return false;
   }
+  if (!float8_e4m3fnuz_already_registered &&
+      !float8_e5m2fnuz_already_registered &&
+      !RegisterTwoWayCustomCast<float8_e4m3fnuz, float8_e5m2fnuz>()) {
+    return false;
+  }
   if (!float8_e4m3fn_already_registered && !float8_e5m2_already_registered &&
       !RegisterCustomFloatCast<float8_e4m3fn, float8_e5m2>()) {
     return false;
   }
   bool success = true;
   // Continue trying to register casts, just in case some types are not
   // registered (i.e. float8_e4m3b11)
   success &= RegisterTwoWayCustomCast<float8_e4m3b11, float8_e4m3fn>();
   success &= RegisterTwoWayCustomCast<float8_e4m3b11, float8_e5m2>();
   success &= RegisterTwoWayCustomCast<bfloat16, float8_e4m3fn>();
   success &= RegisterTwoWayCustomCast<bfloat16, float8_e5m2>();
+  success &= RegisterTwoWayCustomCast<float8_e4m3fnuz, bfloat16>();
+  success &= RegisterTwoWayCustomCast<float8_e5m2fnuz, bfloat16>();
+  success &= RegisterTwoWayCustomCast<float8_e4m3fnuz, float8_e4m3b11>();
+  success &= RegisterTwoWayCustomCast<float8_e5m2fnuz, float8_e4m3b11>();
+  success &= RegisterTwoWayCustomCast<float8_e4m3fnuz, float8_e4m3fn>();
+  success &= RegisterTwoWayCustomCast<float8_e5m2fnuz, float8_e4m3fn>();
+  success &= RegisterTwoWayCustomCast<float8_e4m3fnuz, float8_e5m2>();
+  success &= RegisterTwoWayCustomCast<float8_e5m2fnuz, float8_e5m2>();
   return success;
 }
 
 static PyModuleDef module_def = {
     PyModuleDef_HEAD_INIT,
     "_custom_floats",
 };
@@ -227,19 +278,31 @@
   }
   if (PyObject_SetAttrString(m.get(), "float8_e4m3fn",
                              reinterpret_cast<PyObject*>(
                                  TypeDescriptor<float8_e4m3fn>::type_ptr)) <
       0) {
     return nullptr;
   }
+  if (PyObject_SetAttrString(m.get(), "float8_e4m3fnuz",
+                             reinterpret_cast<PyObject*>(
+                                 TypeDescriptor<float8_e4m3fnuz>::type_ptr)) <
+      0) {
+    return nullptr;
+  }
   if (PyObject_SetAttrString(m.get(), "float8_e5m2",
                              reinterpret_cast<PyObject*>(
                                  TypeDescriptor<float8_e5m2>::type_ptr)) < 0) {
     return nullptr;
   }
+  if (PyObject_SetAttrString(m.get(), "float8_e5m2fnuz",
+                             reinterpret_cast<PyObject*>(
+                                 TypeDescriptor<float8_e5m2fnuz>::type_ptr)) <
+      0) {
+    return nullptr;
+  }
   if (PyObject_SetAttrString(m.get(), "bfloat16",
                              reinterpret_cast<PyObject*>(
                                  TypeDescriptor<bfloat16>::type_ptr)) < 0) {
     return nullptr;
   }
   return m.release();
 }
```

### Comparing `ml_dtypes-0.0.4/ml_dtypes/_src/float8.h` & `ml_dtypes-0.1.0/ml_dtypes/_src/float8.h`

 * *Files 18% similar despite different names*

```diff
@@ -29,16 +29,18 @@
 
 namespace ml_dtypes {
 
 namespace float8_internal {
 
 // Forward-declarations of classes.
 class float8_e4m3fn;
+class float8_e4m3fnuz;
 class float8_e4m3b11;
 class float8_e5m2;
+class float8_e5m2fnuz;
 
 template <typename Derived>
 class float8_base {
  protected:
   // Constructor tag to allow constexpr construction from bit representation.
   struct ConstructFromRepTag {};
 
@@ -179,16 +181,20 @@
       : float8_e4m3fn(ConvertFrom(f32)) {}
   explicit EIGEN_DEVICE_FUNC float8_e4m3fn(Eigen::bfloat16 bf16)
       : float8_e4m3fn(ConvertFrom(bf16)) {}
   explicit EIGEN_DEVICE_FUNC float8_e4m3fn(Eigen::half f16)
       : float8_e4m3fn(ConvertFrom(f16)) {}
   explicit EIGEN_DEVICE_FUNC float8_e4m3fn(const float8_e5m2& f8)
       : float8_e4m3fn(ConvertFrom(f8)) {}
+  explicit EIGEN_DEVICE_FUNC float8_e4m3fn(const float8_e5m2fnuz& f8)
+      : float8_e4m3fn(ConvertFrom(f8)) {}
   explicit EIGEN_DEVICE_FUNC float8_e4m3fn(const float8_e4m3b11& f8)
       : float8_e4m3fn(ConvertFrom(f8)) {}
+  explicit EIGEN_DEVICE_FUNC float8_e4m3fn(const float8_e4m3fnuz& f8)
+      : float8_e4m3fn(ConvertFrom(f8)) {}
 
   template <typename T,
             typename EnableIf = std::enable_if<std::is_arithmetic_v<T>>>
   explicit EIGEN_DEVICE_FUNC operator T() const {
     return static_cast<T>(static_cast<float>(*this));
   }
   explicit EIGEN_DEVICE_FUNC operator double() const {
@@ -231,16 +237,20 @@
       : float8_e4m3b11(ConvertFrom(f32)) {}
   explicit EIGEN_DEVICE_FUNC float8_e4m3b11(Eigen::bfloat16 bf16)
       : float8_e4m3b11(ConvertFrom(bf16)) {}
   explicit EIGEN_DEVICE_FUNC float8_e4m3b11(Eigen::half f16)
       : float8_e4m3b11(ConvertFrom(f16)) {}
   explicit EIGEN_DEVICE_FUNC float8_e4m3b11(const float8_e5m2& f8)
       : float8_e4m3b11(ConvertFrom(f8)) {}
+  explicit EIGEN_DEVICE_FUNC float8_e4m3b11(const float8_e5m2fnuz& f8)
+      : float8_e4m3b11(ConvertFrom(f8)) {}
   explicit EIGEN_DEVICE_FUNC float8_e4m3b11(const float8_e4m3fn& f8)
       : float8_e4m3b11(ConvertFrom(f8)) {}
+  explicit EIGEN_DEVICE_FUNC float8_e4m3b11(const float8_e4m3fnuz& f8)
+      : float8_e4m3b11(ConvertFrom(f8)) {}
 
   constexpr float8_e4m3b11 operator-() const {
     if ((rep() & 0x7f) == 0x00) {
       return float8_e4m3b11(rep(), ConstructFromRepTag{});
     }
     return Base::operator-();
   }
@@ -265,14 +275,92 @@
   }
   explicit EIGEN_DEVICE_FUNC operator Eigen::half() const {
     return ConvertTo<Eigen::half>(*this);
   }
   explicit EIGEN_DEVICE_FUNC operator bool() const { return rep() != 0; }
 };
 
+class float8_e4m3fnuz : public float8_base<float8_e4m3fnuz> {
+  // 8-bit floating point with 3 bit mantissa.
+  //
+  // An 8-bit floating point type with 1 sign bit, 4 bits exponent and 3 bits
+  // mantissa. The suffix "fnuz" is consistent with LLVM/MLIR naming and is
+  // derived from the differences to IEEE floating point conventions. `F` is
+  // for "finite" (no infinities), `N` for with special NaN encoding, `UZ` for
+  // unsigned zero.
+  //
+  // This type has the following characteristics:
+  // * bit encoding: S1E4M3 - `0bSEEEEMMM`
+  // * exponent bias: 8
+  // * infinities: Not supported
+  // * NaNs: Supported with sign bit set to 1, exponent bits and mantissa bits
+  // set to all 0s - `0b10000000`
+  // * denormals when exponent is 0
+ private:
+  using Base = float8_base<float8_e4m3fnuz>;
+  friend class float8_base<float8_e4m3fnuz>;
+
+  constexpr float8_e4m3fnuz(uint8_t rep, ConstructFromRepTag)
+      : Base(rep, ConstructFromRepTag{}) {}
+
+ public:
+  constexpr float8_e4m3fnuz() = default;
+
+  template <typename T,
+            typename EnableIf = std::enable_if<std::is_arithmetic_v<T>>>
+  explicit EIGEN_DEVICE_FUNC float8_e4m3fnuz(T f)
+      : float8_e4m3fnuz(ConvertFrom(static_cast<float>(f))) {}
+  explicit EIGEN_DEVICE_FUNC float8_e4m3fnuz(double f64)
+      : float8_e4m3fnuz(ConvertFrom(f64)) {}
+  explicit EIGEN_DEVICE_FUNC float8_e4m3fnuz(float f32)
+      : float8_e4m3fnuz(ConvertFrom(f32)) {}
+  explicit EIGEN_DEVICE_FUNC float8_e4m3fnuz(Eigen::bfloat16 bf16)
+      : float8_e4m3fnuz(ConvertFrom(bf16)) {}
+  explicit EIGEN_DEVICE_FUNC float8_e4m3fnuz(Eigen::half f16)
+      : float8_e4m3fnuz(ConvertFrom(f16)) {}
+  explicit EIGEN_DEVICE_FUNC float8_e4m3fnuz(const float8_e5m2& f8)
+      : float8_e4m3fnuz(ConvertFrom(f8)) {}
+  explicit EIGEN_DEVICE_FUNC float8_e4m3fnuz(const float8_e5m2fnuz& f8)
+      : float8_e4m3fnuz(ConvertFrom(f8)) {}
+  explicit EIGEN_DEVICE_FUNC float8_e4m3fnuz(const float8_e4m3b11& f8)
+      : float8_e4m3fnuz(ConvertFrom(f8)) {}
+  explicit EIGEN_DEVICE_FUNC float8_e4m3fnuz(const float8_e4m3fn& f8)
+      : float8_e4m3fnuz(ConvertFrom(f8)) {}
+
+  constexpr float8_e4m3fnuz operator-() const {
+    if ((rep() & 0x7f) == 0x00) {
+      return float8_e4m3fnuz(rep(), ConstructFromRepTag{});
+    }
+    return Base::operator-();
+  }
+
+  float8_e4m3fnuz operator-(const float8_e4m3fnuz& other) const {
+    return Base::operator-(other);
+  }
+
+  template <typename T,
+            typename EnableIf = std::enable_if<std::is_arithmetic_v<T>>>
+  explicit EIGEN_DEVICE_FUNC operator T() const {
+    return static_cast<T>(static_cast<float>(*this));
+  }
+  explicit EIGEN_DEVICE_FUNC operator double() const {
+    return ConvertTo<double>(*this);
+  }
+  explicit EIGEN_DEVICE_FUNC operator float() const {
+    return ConvertTo<float>(*this);
+  }
+  explicit EIGEN_DEVICE_FUNC operator Eigen::bfloat16() const {
+    return ConvertTo<Eigen::bfloat16>(*this);
+  }
+  explicit EIGEN_DEVICE_FUNC operator Eigen::half() const {
+    return ConvertTo<Eigen::half>(*this);
+  }
+  explicit EIGEN_DEVICE_FUNC operator bool() const { return rep() != 0; }
+};
+
 class float8_e5m2 : public float8_base<float8_e5m2> {
   // Exponent: 5, Mantissa: 2, bias: 15.
   // IEEE 754.
  private:
   using Base = float8_base<float8_e5m2>;
   friend class float8_base<float8_e5m2>;
 
@@ -292,16 +380,20 @@
       : float8_e5m2(ConvertFrom(f32)) {}
   explicit EIGEN_DEVICE_FUNC float8_e5m2(Eigen::bfloat16 bf16)
       : float8_e5m2(ConvertFrom(bf16)) {}
   explicit EIGEN_DEVICE_FUNC float8_e5m2(Eigen::half f16)
       : float8_e5m2(ConvertFrom(f16)) {}
   explicit EIGEN_DEVICE_FUNC float8_e5m2(float8_e4m3fn f8)
       : float8_e5m2(ConvertFrom(f8)) {}
+  explicit EIGEN_DEVICE_FUNC float8_e5m2(float8_e4m3fnuz f8)
+      : float8_e5m2(ConvertFrom(f8)) {}
   explicit EIGEN_DEVICE_FUNC float8_e5m2(float8_e4m3b11 f8)
       : float8_e5m2(ConvertFrom(f8)) {}
+  explicit EIGEN_DEVICE_FUNC float8_e5m2(float8_e5m2fnuz& f8)
+      : float8_e5m2(ConvertFrom(f8)) {}
 
   template <typename T,
             typename EnableIf = std::enable_if<std::is_arithmetic_v<T>>>
   explicit EIGEN_DEVICE_FUNC operator T() const {
     return static_cast<T>(static_cast<float>(*this));
   }
   explicit EIGEN_DEVICE_FUNC operator double() const {
@@ -317,14 +409,92 @@
     return ConvertTo<Eigen::half>(*this);
   }
   explicit EIGEN_DEVICE_FUNC operator bool() const {
     return (rep() & 0x7F) != 0;
   }
 };
 
+class float8_e5m2fnuz : public float8_base<float8_e5m2fnuz> {
+  // 8-bit floating point with 2 bit mantissa.
+  //
+  // An 8-bit floating point type with 1 sign bit, 5 bits exponent and 2 bits
+  // mantissa. The suffix "fnuz" is consistent with LLVM/MLIR naming and is
+  // derived from the differences to IEEE floating point conventions. `F` is
+  // for "finite" (no infinities), `N` for with special NaN encoding, `UZ` for
+  // unsigned zero.
+  //
+  // This type has the following characteristics:
+  // * bit encoding: S1E5M2 - `0bSEEEEEMM`
+  // * exponent bias: 16
+  // * infinities: Not supported
+  // * NaNs: Supported with sign bit set to 1, exponent bits and mantissa bits
+  // set to all 0s - `0b10000000`
+  // * denormals when exponent is 0
+ private:
+  using Base = float8_base<float8_e5m2fnuz>;
+  friend class float8_base<float8_e5m2fnuz>;
+
+  constexpr float8_e5m2fnuz(uint8_t rep, ConstructFromRepTag)
+      : Base(rep, ConstructFromRepTag{}) {}
+
+ public:
+  constexpr float8_e5m2fnuz() = default;
+
+  template <typename T,
+            typename EnableIf = std::enable_if<std::is_arithmetic_v<T>>>
+  explicit EIGEN_DEVICE_FUNC float8_e5m2fnuz(T f)
+      : float8_e5m2fnuz(ConvertFrom(static_cast<float>(f))) {}
+  explicit EIGEN_DEVICE_FUNC float8_e5m2fnuz(double f64)
+      : float8_e5m2fnuz(ConvertFrom(f64)) {}
+  explicit EIGEN_DEVICE_FUNC float8_e5m2fnuz(float f32)
+      : float8_e5m2fnuz(ConvertFrom(f32)) {}
+  explicit EIGEN_DEVICE_FUNC float8_e5m2fnuz(Eigen::bfloat16 bf16)
+      : float8_e5m2fnuz(ConvertFrom(bf16)) {}
+  explicit EIGEN_DEVICE_FUNC float8_e5m2fnuz(Eigen::half f16)
+      : float8_e5m2fnuz(ConvertFrom(f16)) {}
+  explicit EIGEN_DEVICE_FUNC float8_e5m2fnuz(const float8_e5m2& f8)
+      : float8_e5m2fnuz(ConvertFrom(f8)) {}
+  explicit EIGEN_DEVICE_FUNC float8_e5m2fnuz(const float8_e4m3b11& f8)
+      : float8_e5m2fnuz(ConvertFrom(f8)) {}
+  explicit EIGEN_DEVICE_FUNC float8_e5m2fnuz(const float8_e4m3fn& f8)
+      : float8_e5m2fnuz(ConvertFrom(f8)) {}
+  explicit EIGEN_DEVICE_FUNC float8_e5m2fnuz(const float8_e4m3fnuz& f8)
+      : float8_e5m2fnuz(ConvertFrom(f8)) {}
+
+  constexpr float8_e5m2fnuz operator-() const {
+    if ((rep() & 0x7f) == 0x00) {
+      return float8_e5m2fnuz(rep(), ConstructFromRepTag{});
+    }
+    return Base::operator-();
+  }
+
+  float8_e5m2fnuz operator-(const float8_e5m2fnuz& other) const {
+    return Base::operator-(other);
+  }
+
+  template <typename T,
+            typename EnableIf = std::enable_if<std::is_arithmetic_v<T>>>
+  explicit EIGEN_DEVICE_FUNC operator T() const {
+    return static_cast<T>(static_cast<float>(*this));
+  }
+  explicit EIGEN_DEVICE_FUNC operator double() const {
+    return ConvertTo<double>(*this);
+  }
+  explicit EIGEN_DEVICE_FUNC operator float() const {
+    return ConvertTo<float>(*this);
+  }
+  explicit EIGEN_DEVICE_FUNC operator Eigen::bfloat16() const {
+    return ConvertTo<Eigen::bfloat16>(*this);
+  }
+  explicit EIGEN_DEVICE_FUNC operator Eigen::half() const {
+    return ConvertTo<Eigen::half>(*this);
+  }
+  explicit EIGEN_DEVICE_FUNC operator bool() const { return rep() != 0; }
+};
+
 // Structures for use in specializing std::numeric_limits.
 struct numeric_limits_float8_base {
   // NOLINTBEGIN: these names must match std::numeric_limits.
   static inline constexpr const bool is_specialized = true;
   static inline constexpr const bool is_signed = true;
   static inline constexpr const bool is_integer = false;
   static inline constexpr const bool is_exact = false;
@@ -448,14 +618,64 @@
   }
   static constexpr float8_e4m3b11 denorm_min() {
     return float8_e4m3b11::FromRep(0x01);
   }
 };
 
 template <>
+struct numeric_limits_float8<float8_e4m3fnuz>
+    : public numeric_limits_float8_base {
+  // NOLINTBEGIN: these names must match std::numeric_limits.
+  static inline constexpr const int digits = 4;
+  static inline constexpr const int digits10 = 0;      // floor(3 * log10(2));
+  static inline constexpr const int max_digits10 = 3;  // ceil(4 * log10(2) + 1)
+  static inline constexpr const int min_exponent = -6;
+  static inline constexpr const int min_exponent10 = -2;
+  static inline constexpr const int max_exponent = 7;
+  static inline constexpr const int max_exponent10 = 2;
+  static inline constexpr const bool is_iec559 = false;
+  static inline constexpr const bool has_infinity = false;
+  static inline constexpr const bool has_signaling_NaN = false;
+  // NOLINTEND
+
+  static constexpr float8_e4m3fnuz min() {
+    return float8_e4m3fnuz::FromRep(0x08);
+  }
+  static constexpr float8_e4m3fnuz lowest() {
+    return float8_e4m3fnuz::FromRep(0xFF);
+  }
+  static constexpr float8_e4m3fnuz max() {
+    return float8_e4m3fnuz::FromRep(0x7F);
+  }
+  static constexpr float8_e4m3fnuz epsilon() {
+    constexpr int kExponentBias = 8;
+    constexpr int kMantissaBits = 3;
+    return float8_e4m3fnuz::FromRep((kExponentBias - kMantissaBits)
+                                    << kMantissaBits);
+  }
+  static constexpr float8_e4m3fnuz round_error() {
+    constexpr int kExponentBias = 8;
+    constexpr int kMantissaBits = 3;
+    return float8_e4m3fnuz::FromRep((kExponentBias - 1) << kMantissaBits);
+  }
+  static constexpr float8_e4m3fnuz infinity() {
+    return float8_e4m3fnuz::FromRep(0x80);
+  }  // NaN.
+  static constexpr float8_e4m3fnuz quiet_NaN() {
+    return float8_e4m3fnuz::FromRep(0x80);
+  }
+  static constexpr float8_e4m3fnuz signaling_NaN() {
+    return float8_e4m3fnuz::FromRep(0x80);
+  }
+  static constexpr float8_e4m3fnuz denorm_min() {
+    return float8_e4m3fnuz::FromRep(0x01);
+  }
+};
+
+template <>
 struct numeric_limits_float8<float8_e5m2> : public numeric_limits_float8_base {
   // NOLINTBEGIN: these names must match std::numeric_limits.
   static inline constexpr const int digits = 3;
   static inline constexpr const int digits10 = 0;      // floor(2 * log10(2))
   static inline constexpr const int max_digits10 = 2;  // ceil(3 * log10(2) + 1)
   static inline constexpr const int min_exponent = -13;
   static inline constexpr const int min_exponent10 = -4;
@@ -481,14 +701,64 @@
     return float8_e5m2::FromRep(0x7D);
   }
   static constexpr float8_e5m2 denorm_min() {
     return float8_e5m2::FromRep(0x01);
   }
 };
 
+template <>
+struct numeric_limits_float8<float8_e5m2fnuz>
+    : public numeric_limits_float8_base {
+  // NOLINTBEGIN: these names must match std::numeric_limits.
+  static inline constexpr const int digits = 3;
+  static inline constexpr const int digits10 = 0;      // floor(2 * log10(2))
+  static inline constexpr const int max_digits10 = 2;  // ceil(3 * log10(2) + 1)
+  static inline constexpr const int min_exponent = -14;
+  static inline constexpr const int min_exponent10 = -4;
+  static inline constexpr const int max_exponent = 16;
+  static inline constexpr const int max_exponent10 = 4;
+  static inline constexpr const bool is_iec559 = false;
+  static inline constexpr const bool has_infinity = false;
+  static inline constexpr const bool has_signaling_NaN = false;
+  // NOLINTEND
+
+  static constexpr float8_e5m2fnuz min() {
+    return float8_e5m2fnuz::FromRep(0x08);
+  }
+  static constexpr float8_e5m2fnuz lowest() {
+    return float8_e5m2fnuz::FromRep(0xFF);
+  }
+  static constexpr float8_e5m2fnuz max() {
+    return float8_e5m2fnuz::FromRep(0x7F);
+  }
+  static constexpr float8_e5m2fnuz epsilon() {
+    constexpr int kExponentBias = 16;
+    constexpr int kMantissaBits = 2;
+    return float8_e5m2fnuz::FromRep((kExponentBias - kMantissaBits)
+                                    << kMantissaBits);
+  }
+  static constexpr float8_e5m2fnuz round_error() {
+    constexpr int kExponentBias = 16;
+    constexpr int kMantissaBits = 2;
+    return float8_e5m2fnuz::FromRep((kExponentBias - 1) << kMantissaBits);
+  }
+  static constexpr float8_e5m2fnuz infinity() {
+    return float8_e5m2fnuz::FromRep(0x80);
+  }  // NaN.
+  static constexpr float8_e5m2fnuz quiet_NaN() {
+    return float8_e5m2fnuz::FromRep(0x80);
+  }
+  static constexpr float8_e5m2fnuz signaling_NaN() {
+    return float8_e5m2fnuz::FromRep(0x80);
+  }
+  static constexpr float8_e5m2fnuz denorm_min() {
+    return float8_e5m2fnuz::FromRep(0x01);
+  }
+};
+
 }  // namespace float8_internal
 }  // namespace ml_dtypes
 
 namespace std {
 // Standard-library overrides.  Note that these are picked up by Eigen as well.
 template <>
 struct numeric_limits<ml_dtypes::float8_internal::float8_e4m3fn>
@@ -497,17 +767,27 @@
 
 template <>
 struct numeric_limits<ml_dtypes::float8_internal::float8_e4m3b11>
     : public ml_dtypes::float8_internal::numeric_limits_float8<
           ml_dtypes::float8_internal::float8_e4m3b11> {};
 
 template <>
+struct numeric_limits<ml_dtypes::float8_internal::float8_e4m3fnuz>
+    : public ml_dtypes::float8_internal::numeric_limits_float8<
+          ml_dtypes::float8_internal::float8_e4m3fnuz> {};
+
+template <>
 struct numeric_limits<ml_dtypes::float8_internal::float8_e5m2>
     : public ml_dtypes::float8_internal::numeric_limits_float8<
           ml_dtypes::float8_internal::float8_e5m2> {};
+
+template <>
+struct numeric_limits<ml_dtypes::float8_internal::float8_e5m2fnuz>
+    : public ml_dtypes::float8_internal::numeric_limits_float8<
+          ml_dtypes::float8_internal::float8_e5m2fnuz> {};
 }  // namespace std
 
 namespace ml_dtypes {
 namespace float8_internal {
 
 // Free-functions for use with ADL and in Eigen.
 constexpr inline float8_e4m3fn abs(const float8_e4m3fn& a) {
@@ -537,14 +817,31 @@
   return false;  // No inf representation.
 }
 
 constexpr inline bool isfinite(const float8_e4m3b11& a) {
   return !isnan(a) && !isinf(a);
 }
 
+constexpr inline float8_e4m3fnuz abs(const float8_e4m3fnuz& a) {
+  return (a.rep() & 0x7F) == 0 ? float8_e4m3fnuz::FromRep(a.rep())
+                               : float8_e4m3fnuz::FromRep(a.rep() & 0x7F);
+}
+
+constexpr inline bool isnan(const float8_e4m3fnuz& a) {
+  return a.rep() == 0x80;
+}
+
+constexpr inline bool isinf(const float8_e4m3fnuz& a) {
+  return false;  // No inf representation.
+}
+
+constexpr inline bool isfinite(const float8_e4m3fnuz& a) {
+  return !isnan(a) && !isinf(a);
+}
+
 constexpr inline float8_e5m2 abs(const float8_e5m2& a) {
   return float8_e5m2::FromRep(a.rep() & 0x7F);
 }
 
 constexpr inline bool isnan(const float8_e5m2& a) {
   return (a.rep() & 0x7F) > 0x7C;
 }
@@ -553,14 +850,31 @@
   return (a.rep() & 0x7F) == 0x7C;
 }
 
 constexpr inline bool isfinite(const float8_e5m2& a) {
   return !isnan(a) && !isinf(a);
 }
 
+constexpr inline float8_e5m2fnuz abs(const float8_e5m2fnuz& a) {
+  return (a.rep() & 0x7F) == 0 ? float8_e5m2fnuz::FromRep(a.rep())
+                               : float8_e5m2fnuz::FromRep(a.rep() & 0x7F);
+}
+
+constexpr inline bool isnan(const float8_e5m2fnuz& a) {
+  return a.rep() == 0x80;
+}
+
+constexpr inline bool isinf(const float8_e5m2fnuz& a) {
+  return false;  // No inf representation.
+}
+
+constexpr inline bool isfinite(const float8_e5m2fnuz& a) {
+  return !isnan(a) && !isinf(a);
+}
+
 template <typename Float8>
 std::ostream& operator<<(std::ostream& os, const float8_base<Float8>& f8) {
   os << static_cast<float>(f8.derived());
   return os;
 }
 
 //==============================================================================
@@ -652,14 +966,46 @@
       sign = 0;
     }
     return Eigen::numext::bit_cast<float8_e4m3b11>(
         static_cast<typename Base::BitsType>(bits | sign));
   }
 };
 
+template <>
+struct Traits<float8_e4m3fnuz> : public TraitsBase<float8_e4m3fnuz> {
+  using Base = TraitsBase<float8_e4m3fnuz>;
+  static constexpr int kExponentBias = 8;
+  static EIGEN_DEVICE_FUNC float8_e4m3fnuz ConstructFromSignAndBits(
+      typename Base::BitsType sign, typename Base::BitsType bits) {
+    // float8_e4m3fnuz does not support signed zero, ignore the sign if we try
+    // to make one.
+    if (bits == 0) {
+      sign = 0;
+    }
+    return Eigen::numext::bit_cast<float8_e4m3fnuz>(
+        static_cast<typename Base::BitsType>(bits | sign));
+  }
+};
+
+template <>
+struct Traits<float8_e5m2fnuz> : public TraitsBase<float8_e5m2fnuz> {
+  using Base = TraitsBase<float8_e5m2fnuz>;
+  static constexpr int kExponentBias = 16;
+  static EIGEN_DEVICE_FUNC float8_e5m2fnuz ConstructFromSignAndBits(
+      typename Base::BitsType sign, typename Base::BitsType bits) {
+    // float8_e5m2fnuz does not support signed zero, ignore the sign if we try
+    // to make one.
+    if (bits == 0) {
+      sign = 0;
+    }
+    return Eigen::numext::bit_cast<float8_e5m2fnuz>(
+        static_cast<typename Base::BitsType>(bits | sign));
+  }
+};
+
 // Shift bits in the appropriate directions and add the exponent offset
 // to convert between bit representations.  The input `in` must be a
 // positive normalized value.
 template <typename From, typename To,
           typename FromBits = typename Traits<From>::BitsType,
           typename ToBits = typename Traits<To>::BitsType>
 constexpr FromBits ToFromBits(ToBits in) {
@@ -926,14 +1272,33 @@
     if constexpr (!kTruncate) {
       from_bits = RoundBitsToNearestEven(from_bits, 8);
     }
     return float8_e5m2::FromRep(from_bits >> 8);
   }
 };
 
+template <bool kTruncate, bool kSaturate>
+struct ConvertImpl<Eigen::half, float8_e5m2fnuz, kTruncate, kSaturate> {
+  static EIGEN_DEVICE_FUNC inline float8_e5m2fnuz run(const Eigen::half& from) {
+    // Cast via float because float8_e5m2fnuz and Eigen::half have overlapping
+    // subnormal range.
+    return ConvertImpl<float, float8_e5m2fnuz, kTruncate, kSaturate>::run(from);
+  }
+};
+
+template <bool kTruncate, bool kSaturate>
+struct ConvertImpl<float8_e5m2fnuz, Eigen::half, kTruncate, kSaturate> {
+  static EIGEN_DEVICE_FUNC inline Eigen::half run(const float8_e5m2fnuz& from) {
+    // Cast via float because float8_e5m2fnuz and Eigen::half have overlapping
+    // subnormal range.
+    return static_cast<Eigen::half>(
+        ConvertImpl<float8_e5m2fnuz, float, kTruncate, kSaturate>::run(from));
+  }
+};
+
 // Saturation has no impact when casting Eigen::half to e5m2.
 template <bool kTruncate>
 struct ConvertImpl<Eigen::half, float8_e5m2, /*kSaturate=*/true, kTruncate> {
   static EIGEN_DEVICE_FUNC inline float8_e5m2 run(const Eigen::half& from) {
     return ConvertImpl<Eigen::half, float8_e5m2, /*kSaturate=*/false,
                        kTruncate>::run(from);
   }
@@ -969,16 +1334,18 @@
   return ConvertImpl<Derived, To, kSaturate, kTruncate>::run(from);
 }
 
 }  // namespace float8_internal
 
 // Exported types.
 using float8_e4m3fn = float8_internal::float8_e4m3fn;
+using float8_e4m3fnuz = float8_internal::float8_e4m3fnuz;
 using float8_e4m3b11 = float8_internal::float8_e4m3b11;
 using float8_e5m2 = float8_internal::float8_e5m2;
+using float8_e5m2fnuz = float8_internal::float8_e5m2fnuz;
 
 }  // namespace ml_dtypes
 
 // Eigen-specific overrides.
 namespace Eigen {
 namespace numext {
 
@@ -1020,52 +1387,88 @@
 template <>
 EIGEN_DEVICE_FUNC inline bool isinf_impl<ml_dtypes::float8_e4m3b11>(
     const ml_dtypes::float8_e4m3b11& x) {
   return ml_dtypes::float8_internal::isinf(x);
 }
 
 template <>
+EIGEN_DEVICE_FUNC inline bool isinf_impl<ml_dtypes::float8_e4m3fnuz>(
+    const ml_dtypes::float8_e4m3fnuz& x) {
+  return ml_dtypes::float8_internal::isinf(x);
+}
+
+template <>
 EIGEN_DEVICE_FUNC inline bool isinf_impl<ml_dtypes::float8_e5m2>(
     const ml_dtypes::float8_e5m2& x) {
   return ml_dtypes::float8_internal::isinf(x);
 }
 
 template <>
+EIGEN_DEVICE_FUNC inline bool isinf_impl<ml_dtypes::float8_e5m2fnuz>(
+    const ml_dtypes::float8_e5m2fnuz& x) {
+  return ml_dtypes::float8_internal::isinf(x);
+}
+
+template <>
 EIGEN_DEVICE_FUNC inline bool isnan_impl<ml_dtypes::float8_e4m3fn>(
     const ml_dtypes::float8_e4m3fn& x) {
   return ml_dtypes::float8_internal::isnan(x);
 }
 
 template <>
 EIGEN_DEVICE_FUNC inline bool isnan_impl<ml_dtypes::float8_e4m3b11>(
     const ml_dtypes::float8_e4m3b11& x) {
   return ml_dtypes::float8_internal::isnan(x);
 }
 
 template <>
+EIGEN_DEVICE_FUNC inline bool isnan_impl<ml_dtypes::float8_e4m3fnuz>(
+    const ml_dtypes::float8_e4m3fnuz& x) {
+  return ml_dtypes::float8_internal::isnan(x);
+}
+
+template <>
 EIGEN_DEVICE_FUNC inline bool isnan_impl<ml_dtypes::float8_e5m2>(
     const ml_dtypes::float8_e5m2& x) {
   return ml_dtypes::float8_internal::isnan(x);
 }
 
 template <>
+EIGEN_DEVICE_FUNC inline bool isnan_impl<ml_dtypes::float8_e5m2fnuz>(
+    const ml_dtypes::float8_e5m2fnuz& x) {
+  return ml_dtypes::float8_internal::isnan(x);
+}
+
+template <>
 EIGEN_DEVICE_FUNC inline bool isfinite_impl<ml_dtypes::float8_e4m3fn>(
     const ml_dtypes::float8_e4m3fn& x) {
   return ml_dtypes::float8_internal::isfinite(x);
 }
 
 template <>
 EIGEN_DEVICE_FUNC inline bool isfinite_impl<ml_dtypes::float8_e4m3b11>(
     const ml_dtypes::float8_e4m3b11& x) {
   return ml_dtypes::float8_internal::isfinite(x);
 }
 
 template <>
+EIGEN_DEVICE_FUNC inline bool isfinite_impl<ml_dtypes::float8_e4m3fnuz>(
+    const ml_dtypes::float8_e4m3fnuz& x) {
+  return ml_dtypes::float8_internal::isfinite(x);
+}
+
+template <>
 EIGEN_DEVICE_FUNC inline bool isfinite_impl<ml_dtypes::float8_e5m2>(
     const ml_dtypes::float8_e5m2& x) {
   return ml_dtypes::float8_internal::isfinite(x);
 }
 
+template <>
+EIGEN_DEVICE_FUNC inline bool isfinite_impl<ml_dtypes::float8_e5m2fnuz>(
+    const ml_dtypes::float8_e5m2fnuz& x) {
+  return ml_dtypes::float8_internal::isfinite(x);
+}
+
 }  // namespace internal
 }  // namespace Eigen
 
 #endif  // ML_DTYPES_FLOAT8_H_
```

### Comparing `ml_dtypes-0.0.4/ml_dtypes/_src/numpy.cc` & `ml_dtypes-0.1.0/ml_dtypes/_src/numpy.cc`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/ml_dtypes/_src/numpy.h` & `ml_dtypes-0.1.0/ml_dtypes/_src/numpy.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/ml_dtypes/tests/custom_float_test.py` & `ml_dtypes-0.1.0/ml_dtypes/tests/custom_float_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,17 @@
 import ml_dtypes
 
 import numpy as np
 
 bfloat16 = ml_dtypes.bfloat16
 float8_e4m3b11 = ml_dtypes.float8_e4m3b11
 float8_e4m3fn = ml_dtypes.float8_e4m3fn
+float8_e4m3fnuz = ml_dtypes.float8_e4m3fnuz
 float8_e5m2 = ml_dtypes.float8_e5m2
+float8_e5m2fnuz = ml_dtypes.float8_e5m2fnuz
 
 
 @contextlib.contextmanager
 def ignore_warning(**kw):
   with warnings.catch_warnings():
     warnings.filterwarnings("ignore", **kw)
     yield
@@ -47,16 +49,19 @@
 def numpy_assert_allclose(a, b, float_type, **kwargs):
   a = a.astype(np.float32) if a.dtype == float_type else a
   b = b.astype(np.float32) if b.dtype == float_type else b
   return np.testing.assert_allclose(a, b, **kwargs)
 
 
 def numpy_promote_types(
-    a: Type[np.generic], b: Type[np.generic], float_type: Type[np.generic],
-    next_largest_fp_type: Type[np.generic]) -> Type[np.generic]:
+    a: Type[np.generic],
+    b: Type[np.generic],
+    float_type: Type[np.generic],
+    next_largest_fp_type: Type[np.generic],
+) -> Type[np.generic]:
   if a == float_type and b == float_type:
     return float_type
   if a == float_type:
     a = next_largest_fp_type
   if b == float_type:
     b = next_largest_fp_type
   return np.promote_types(a, b)
@@ -75,132 +80,123 @@
   expected = op(np.float32(a), np.float32(b))
   result = op(a, b)
   if math.isnan(expected):
     if not math.isnan(result):
       raise AssertionError("%s expected to be nan." % repr(result))
   else:
     np.testing.assert_equal(
-        truncate(expected, float_type=float_type), float(result))
+        truncate(expected, float_type=float_type), float(result)
+    )
 
 
 def dtype_has_inf(dtype):
   """Determines if the dtype has an `inf` representation."""
   inf = float("inf")
   is_inf = False
   try:
     x = dtype(inf)
     is_inf = np.isinf(x)
   except (OverflowError, ValueError):
     pass
   return is_inf
 
 
-# Configure bounds and properties for our custom types, to be used in tests
-# below.
-FLOAT_EPSILON = {
-    bfloat16: float.fromhex("1.0p-7"),
-    float8_e4m3b11: float.fromhex("1.0p-3"),
-    float8_e4m3fn: float.fromhex("1.0p-3"),
-    float8_e5m2: float.fromhex("1.0p-2"),
-}
-
-FLOAT_MAX = {
-    bfloat16: float.fromhex("1.FEp127"),
-    float8_e4m3b11: float.fromhex("1.Ep4"),
-    float8_e4m3fn: float.fromhex("1.Cp8"),
-    float8_e5m2: float.fromhex("1.Cp15"),
-}
-
-FLOAT_SMALLEST_SUBNORMAL = {
-    bfloat16: float.fromhex("1.0p-133"),
-    float8_e4m3b11: float.fromhex("1.0p-13"),
-    float8_e4m3fn: float.fromhex("1.0p-9"),
-    float8_e5m2: float.fromhex("1.0p-16"),
-}
-
-FLOAT_SMALLEST_NORMAL = {
-    bfloat16: float.fromhex("1.0p-126"),
-    float8_e4m3b11: float.fromhex("1.0p-10"),
-    float8_e4m3fn: float.fromhex("1.0p-6"),
-    float8_e5m2: float.fromhex("1.0p-14"),
-}
+FLOAT_DTYPES = [
+    bfloat16,
+    float8_e4m3b11,
+    float8_e4m3fn,
+    float8_e4m3fnuz,
+    float8_e5m2,
+    float8_e5m2fnuz,
+]
 
 # Values that should round trip exactly to float and back.
 # pylint: disable=g-complex-comprehension
 FLOAT_VALUES = {
     dtype: [
         0.0,
         1.0,
         -1.0,
         0.5,
         -0.5,
-        FLOAT_EPSILON[dtype],
-        1.0 + FLOAT_EPSILON[dtype],
-        1.0 - FLOAT_EPSILON[dtype],
-        -1.0 - FLOAT_EPSILON[dtype],
-        -1.0 + FLOAT_EPSILON[dtype],
+        float(ml_dtypes.finfo(dtype).eps),
+        1.0 + float(ml_dtypes.finfo(dtype).eps),
+        1.0 - float(ml_dtypes.finfo(dtype).eps),
+        -1.0 - float(ml_dtypes.finfo(dtype).eps),
+        -1.0 + float(ml_dtypes.finfo(dtype).eps),
         3.5,
         4,
         5,
         7,
-        FLOAT_MAX[dtype],
-        -FLOAT_MAX[dtype],
+        float(ml_dtypes.finfo(dtype).max),
+        -float(ml_dtypes.finfo(dtype).max),
         float("nan"),
         float("-nan"),
         float("inf") if dtype_has_inf(dtype) else 0.0,
         float("-inf") if dtype_has_inf(dtype) else 0.0,
     ]
-    for dtype in FLOAT_EPSILON.keys()
+    for dtype in FLOAT_DTYPES
 }
 
 # Values that should round trip exactly to integer and back.
 INT_VALUES = {
     bfloat16: [0, 1, 2, 10, 34, 47, 128, 255, 256, 512],
     float8_e4m3b11: [*range(16), *range(16, 30, 2)],
     float8_e4m3fn: list(
         itertools.chain.from_iterable(
             range(1 << n, 2 << n, 1 << max(0, n - 3)) for n in range(9)
         )
     )[:-1],
+    float8_e4m3fnuz: list(
+        itertools.chain.from_iterable(
+            range(1 << n, 2 << n, 1 << max(0, n - 3)) for n in range(8)
+        )
+    )[:-1],
     float8_e5m2: list(
         itertools.chain.from_iterable(
             range(1 << n, 2 << n, 1 << max(0, n - 2)) for n in range(16)
         )
     ),
+    float8_e5m2fnuz: list(
+        itertools.chain.from_iterable(
+            range(1 << n, 2 << n, 1 << max(0, n - 2)) for n in range(16)
+        )
+    ),
 }
 
 BITS_TYPE = {
     bfloat16: np.uint16,
     float8_e4m3b11: np.uint8,
     float8_e4m3fn: np.uint8,
+    float8_e4m3fnuz: np.uint8,
     float8_e5m2: np.uint8,
+    float8_e5m2fnuz: np.uint8,
 }
 
 
 # pylint: disable=g-complex-comprehension
 @parameterized.named_parameters(
     (
         {"testcase_name": "_" + dtype.__name__, "float_type": dtype}
-        for dtype in [bfloat16, float8_e4m3b11, float8_e4m3fn, float8_e5m2]
+        for dtype in FLOAT_DTYPES
     )
 )
 class CustomFloatTest(parameterized.TestCase):
   """Tests the non-numpy Python methods of the custom float type."""
 
   def testModuleName(self, float_type):
     self.assertEqual(float_type.__module__, "ml_dtypes")
 
   def testPickleable(self, float_type):
     # https://github.com/google/jax/discussions/8505
     x = np.arange(10, dtype=float_type)
     serialized = pickle.dumps(x)
     x_out = pickle.loads(serialized)
     self.assertEqual(x_out.dtype, x.dtype)
-    np.testing.assert_array_equal(
-        x_out.astype("float32"), x.astype("float32"))
+    np.testing.assert_array_equal(x_out.astype("float32"), x.astype("float32"))
 
   def testRoundTripToFloat(self, float_type):
     for v in FLOAT_VALUES[float_type]:
       np.testing.assert_equal(v, float(float_type(v)))
 
   @ignore_warning(category=RuntimeWarning, message="overflow encountered")
   def testRoundTripNumpyTypes(self, float_type):
@@ -219,70 +215,81 @@
     for v in INT_VALUES[float_type]:
       self.assertEqual(v, int(float_type(v)))
       self.assertEqual(-v, int(float_type(-v)))
 
   @ignore_warning(category=RuntimeWarning, message="overflow encountered")
   def testRoundTripToNumpy(self, float_type):
     for dtype in [
-        float_type, np.float16, np.float32, np.float64, np.longdouble
+        float_type,
+        np.float16,
+        np.float32,
+        np.float64,
+        np.longdouble,
     ]:
       with self.subTest(dtype.__name__):
         for v in FLOAT_VALUES[float_type]:
           np.testing.assert_equal(dtype(v), dtype(float_type(dtype(v))))
           np.testing.assert_equal(dtype(v), dtype(float_type(dtype(v))))
           np.testing.assert_equal(
               dtype(v), dtype(float_type(np.array(v, dtype)))
           )
         if dtype != float_type:
           np.testing.assert_equal(
               np.array(FLOAT_VALUES[float_type], dtype),
-              float_type(np.array(FLOAT_VALUES[float_type],
-                                  dtype)).astype(dtype))
+              float_type(np.array(FLOAT_VALUES[float_type], dtype)).astype(
+                  dtype
+              ),
+          )
 
   def testBetweenCustomTypes(self, float_type):
-    for dtype in [bfloat16, float8_e4m3b11, float8_e4m3fn, float8_e5m2]:
+    for dtype in FLOAT_DTYPES:
       x = np.array(FLOAT_VALUES[float_type], dtype=dtype)
       y = x.astype(float_type)
       z = x.astype(float).astype(float_type)
       numpy_assert_allclose(y, z, float_type=float_type)
 
   def testStr(self, float_type):
     for value in FLOAT_VALUES[float_type]:
-      self.assertEqual("%.6g" % float(float_type(value)),
-                       str(float_type(value)))
+      self.assertEqual(
+          "%.6g" % float(float_type(value)), str(float_type(value))
+      )
 
   def testFromStr(self, float_type):
     self.assertEqual(float_type(1.2), float_type("1.2"))
     self.assertTrue(np.isnan(float_type("nan")))
     self.assertTrue(np.isnan(float_type("-nan")))
     if dtype_has_inf(float_type):
       self.assertEqual(float_type(float("inf")), float_type("inf"))
       self.assertEqual(float_type(float("-inf")), float_type("-inf"))
 
   def testRepr(self, float_type):
     for value in FLOAT_VALUES[float_type]:
-      self.assertEqual("%.6g" % float(float_type(value)),
-                       repr(float_type(value)))
+      self.assertEqual(
+          "%.6g" % float(float_type(value)), repr(float_type(value))
+      )
 
   def testItem(self, float_type):
     self.assertIsInstance(float_type(0).item(), float)
 
   def testHashZero(self, float_type):
     """Tests that negative zero and zero hash to the same value."""
     self.assertEqual(hash(float_type(-0.0)), hash(float_type(0.0)))
 
   def testHashNumbers(self, float_type):
     for value in np.extract(
-        np.isfinite(FLOAT_VALUES[float_type]), FLOAT_VALUES[float_type]):
+        np.isfinite(FLOAT_VALUES[float_type]), FLOAT_VALUES[float_type]
+    ):
       with self.subTest(value):
         self.assertEqual(hash(value), hash(float_type(value)), str(value))
 
   def testHashNan(self, float_type):
-    for name, nan in [("PositiveNan", float_type(float("nan"))),
-                      ("NegativeNan", float_type(float("-nan")))]:
+    for name, nan in [
+        ("PositiveNan", float_type(float("nan"))),
+        ("NegativeNan", float_type(float("-nan"))),
+    ]:
       with self.subTest(name):
         nan_hash = hash(nan)
         nan_object_hash = object.__hash__(nan)
         # The hash of a NaN is either 0 or a hash of the object pointer.
         self.assertIn(nan_hash, (sys.hash_info.nan, nan_object_hash), str(nan))
 
   def testHashInf(self, float_type):
@@ -292,20 +299,28 @@
           -sys.hash_info.inf, hash(float_type(float("-inf"))), "-inf"
       )
 
   # Tests for Python operations
   def testNegate(self, float_type):
     for v in FLOAT_VALUES[float_type]:
       np.testing.assert_equal(
-          float(float_type(-float(float_type(v)))), float(-float_type(v)))
+          float(float_type(-float(float_type(v)))), float(-float_type(v))
+      )
 
   def testAdd(self, float_type):
-    for a, b in [(0, 0), (1, 0), (1, -1), (2, 3.5), (3.5, -2.25),
-                 (float("inf"), -2.25), (float("-inf"), -2.25),
-                 (3.5, float("nan"))]:
+    for a, b in [
+        (0, 0),
+        (1, 0),
+        (1, -1),
+        (2, 3.5),
+        (3.5, -2.25),
+        (float("inf"), -2.25),
+        (float("-inf"), -2.25),
+        (3.5, float("nan")),
+    ]:
       binary_operation_test(a, b, op=lambda a, b: a + b, float_type=float_type)
 
   def testAddScalarTypePromotion(self, float_type):
     """Tests type promotion against Numpy scalar values."""
     types = [float_type, np.float16, np.float32, np.float64, np.longdouble]
     for lhs_type in types:
       for rhs_type in types:
@@ -315,36 +330,59 @@
             float_type=float_type,
             next_largest_fp_type=np.float32,
         )
         actual_type = type(lhs_type(3.5) + rhs_type(2.25))
         self.assertEqual(expected_type, actual_type)
 
   def testAddArrayTypePromotion(self, float_type):
-    self.assertEqual(np.float32,
-                     type(float_type(3.5) + np.array(2.25, np.float32)))
-    self.assertEqual(np.float32,
-                     type(np.array(3.5, np.float32) + float_type(2.25)))
+    self.assertEqual(
+        np.float32, type(float_type(3.5) + np.array(2.25, np.float32))
+    )
+    self.assertEqual(
+        np.float32, type(np.array(3.5, np.float32) + float_type(2.25))
+    )
 
   def testSub(self, float_type):
-    for a, b in [(0, 0), (1, 0), (1, -1), (2, 3.5), (3.5, -2.25),
-                 (-2.25, float("inf")), (-2.25, float("-inf")),
-                 (3.5, float("nan"))]:
+    for a, b in [
+        (0, 0),
+        (1, 0),
+        (1, -1),
+        (2, 3.5),
+        (3.5, -2.25),
+        (-2.25, float("inf")),
+        (-2.25, float("-inf")),
+        (3.5, float("nan")),
+    ]:
       binary_operation_test(a, b, op=lambda a, b: a - b, float_type=float_type)
 
   def testMul(self, float_type):
-    for a, b in [(0, 0), (1, 0), (1, -1), (3.5, -2.25), (float("inf"), -2.25),
-                 (float("-inf"), -2.25), (3.5, float("nan"))]:
+    for a, b in [
+        (0, 0),
+        (1, 0),
+        (1, -1),
+        (3.5, -2.25),
+        (float("inf"), -2.25),
+        (float("-inf"), -2.25),
+        (3.5, float("nan")),
+    ]:
       binary_operation_test(a, b, op=lambda a, b: a * b, float_type=float_type)
 
   @ignore_warning(category=RuntimeWarning, message="invalid value encountered")
   @ignore_warning(category=RuntimeWarning, message="divide by zero encountered")
   def testDiv(self, float_type):
-    for a, b in [(0, 0), (1, 0), (1, -1), (2, 3.5), (3.5, -2.25),
-                 (float("inf"), -2.25), (float("-inf"), -2.25),
-                 (3.5, float("nan"))]:
+    for a, b in [
+        (0, 0),
+        (1, 0),
+        (1, -1),
+        (2, 3.5),
+        (3.5, -2.25),
+        (float("inf"), -2.25),
+        (float("-inf"), -2.25),
+        (3.5, float("nan")),
+    ]:
       binary_operation_test(a, b, op=lambda a, b: a / b, float_type=float_type)
 
   def testLess(self, float_type):
     for v in FLOAT_VALUES[float_type]:
       for w in FLOAT_VALUES[float_type]:
         self.assertEqual(v < w, float_type(v) < float_type(w))
 
@@ -373,115 +411,173 @@
       for w in FLOAT_VALUES[float_type]:
         self.assertEqual(v != w, float_type(v) != float_type(w))
 
   def testNan(self, float_type):
     a = np.isnan(float_type(float("nan")))
     self.assertTrue(a)
     numpy_assert_allclose(
-        np.array([1.0, a]), np.array([1.0, a]), float_type=float_type)
+        np.array([1.0, a]), np.array([1.0, a]), float_type=float_type
+    )
 
     a = np.array(
-        [float_type(1.34375),
-         float_type(1.4375),
-         float_type(float("nan"))],
-        dtype=float_type)
+        [float_type(1.34375), float_type(1.4375), float_type(float("nan"))],
+        dtype=float_type,
+    )
     b = np.array(
-        [float_type(1.3359375),
-         float_type(1.4375),
-         float_type(float("nan"))],
-        dtype=float_type)
+        [float_type(1.3359375), float_type(1.4375), float_type(float("nan"))],
+        dtype=float_type,
+    )
     numpy_assert_allclose(
         a,
         b,
         rtol=0.1,
         atol=0.1,
         equal_nan=True,
         err_msg="",
         verbose=True,
-        float_type=float_type)
+        float_type=float_type,
+    )
 
   def testSort(self, float_type):
     # Note: np.sort doesn't work properly with NaNs since they always compare
     # False.
     values_to_sort = np.float32(
         [x for x in FLOAT_VALUES[float_type] if not np.isnan(x)]
     )
     sorted_f32 = np.sort(values_to_sort)
     sorted_float_type = np.sort(values_to_sort.astype(float_type))  # pylint: disable=too-many-function-args
     np.testing.assert_equal(sorted_f32, np.float32(sorted_float_type))
 
   def testArgmax(self, float_type):
     values_to_sort = np.float32(
-        float_type(np.float32(FLOAT_VALUES[float_type])))
+        float_type(np.float32(FLOAT_VALUES[float_type]))
+    )
     argmax_f32 = np.argmax(values_to_sort)
     argmax_float_type = np.argmax(values_to_sort.astype(float_type))  # pylint: disable=too-many-function-args
     np.testing.assert_equal(argmax_f32, argmax_float_type)
 
   def testArgmaxOnNan(self, float_type):
     """Ensures we return the right thing for multiple NaNs."""
     one_with_nans = np.array(
-        [1.0, float("nan"), float("nan")], dtype=np.float32)
+        [1.0, float("nan"), float("nan")], dtype=np.float32
+    )
     np.testing.assert_equal(
-        np.argmax(one_with_nans.astype(float_type)), np.argmax(one_with_nans))
+        np.argmax(one_with_nans.astype(float_type)), np.argmax(one_with_nans)
+    )
 
   def testArgmaxOnNegativeInfinity(self, float_type):
     """Ensures we return the right thing for negative infinities."""
     inf = np.array([float("-inf")], dtype=np.float32)
     np.testing.assert_equal(np.argmax(inf.astype(float_type)), np.argmax(inf))
 
   def testArgmin(self, float_type):
     values_to_sort = np.float32(
-        float_type(np.float32(FLOAT_VALUES[float_type])))
+        float_type(np.float32(FLOAT_VALUES[float_type]))
+    )
     argmin_f32 = np.argmin(values_to_sort)
     argmin_float_type = np.argmin(values_to_sort.astype(float_type))  # pylint: disable=too-many-function-args
     np.testing.assert_equal(argmin_f32, argmin_float_type)
 
   def testArgminOnNan(self, float_type):
     """Ensures we return the right thing for multiple NaNs."""
     one_with_nans = np.array(
-        [1.0, float("nan"), float("nan")], dtype=np.float32)
+        [1.0, float("nan"), float("nan")], dtype=np.float32
+    )
     np.testing.assert_equal(
-        np.argmin(one_with_nans.astype(float_type)), np.argmin(one_with_nans))
+        np.argmin(one_with_nans.astype(float_type)), np.argmin(one_with_nans)
+    )
 
   def testArgminOnPositiveInfinity(self, float_type):
     """Ensures we return the right thing for positive infinities."""
     inf = np.array([float("inf")], dtype=np.float32)
     np.testing.assert_equal(np.argmin(inf.astype(float_type)), np.argmin(inf))
 
   def testDtypeFromString(self, float_type):
     assert np.dtype(float_type.__name__) == np.dtype(float_type)
 
 
 BinaryOp = collections.namedtuple("BinaryOp", ["op"])
 
 UNARY_UFUNCS = [
-    np.negative, np.positive, np.absolute, np.fabs, np.rint, np.sign,
-    np.conjugate, np.exp, np.exp2, np.expm1, np.log, np.log10, np.log1p,
-    np.log2, np.sqrt, np.square, np.cbrt, np.reciprocal, np.sin, np.cos, np.tan,
-    np.arcsin, np.arccos, np.arctan, np.sinh, np.cosh, np.tanh, np.arcsinh,
-    np.arccosh, np.arctanh, np.deg2rad, np.rad2deg, np.floor, np.ceil, np.trunc
+    np.negative,
+    np.positive,
+    np.absolute,
+    np.fabs,
+    np.rint,
+    np.sign,
+    np.conjugate,
+    np.exp,
+    np.exp2,
+    np.expm1,
+    np.log,
+    np.log10,
+    np.log1p,
+    np.log2,
+    np.sqrt,
+    np.square,
+    np.cbrt,
+    np.reciprocal,
+    np.sin,
+    np.cos,
+    np.tan,
+    np.arcsin,
+    np.arccos,
+    np.arctan,
+    np.sinh,
+    np.cosh,
+    np.tanh,
+    np.arcsinh,
+    np.arccosh,
+    np.arctanh,
+    np.deg2rad,
+    np.rad2deg,
+    np.floor,
+    np.ceil,
+    np.trunc,
 ]
 
 BINARY_UFUNCS = [
-    np.add, np.subtract, np.multiply, np.divide, np.logaddexp, np.logaddexp2,
-    np.floor_divide, np.power, np.remainder, np.fmod, np.heaviside, np.arctan2,
-    np.hypot, np.maximum, np.minimum, np.fmax, np.fmin, np.copysign
+    np.add,
+    np.subtract,
+    np.multiply,
+    np.divide,
+    np.logaddexp,
+    np.logaddexp2,
+    np.floor_divide,
+    np.power,
+    np.remainder,
+    np.fmod,
+    np.heaviside,
+    np.arctan2,
+    np.hypot,
+    np.maximum,
+    np.minimum,
+    np.fmax,
+    np.fmin,
+    np.copysign,
 ]
 
 BINARY_PREDICATE_UFUNCS = [
-    np.equal, np.not_equal, np.less, np.greater, np.less_equal,
-    np.greater_equal, np.logical_and, np.logical_or, np.logical_xor
+    np.equal,
+    np.not_equal,
+    np.less,
+    np.greater,
+    np.less_equal,
+    np.greater_equal,
+    np.logical_and,
+    np.logical_or,
+    np.logical_xor,
 ]
 
 
 # pylint: disable=g-complex-comprehension
 @parameterized.named_parameters(
     (
         {"testcase_name": "_" + dtype.__name__, "float_type": dtype}
-        for dtype in [bfloat16, float8_e4m3b11, float8_e4m3fn, float8_e5m2]
+        for dtype in FLOAT_DTYPES
     )
 )
 class CustomFloatNumPyTest(parameterized.TestCase):
   """Tests NumPy integration of the custom float types."""
 
   def testDtype(self, float_type):
     self.assertEqual(float_type, np.dtype(float_type))
@@ -529,32 +625,66 @@
         (float_type, np.float64),
         (float_type, np.longdouble),
         (float_type, np.complex64),
         (float_type, np.complex128),
         (float_type, np.clongdouble),
     ]
     all_dtypes = [
-        np.float16, np.float32, np.float64, np.longdouble, np.int8, np.int16,
-        np.int32, np.int64, np.complex64, np.complex128, np.clongdouble,
-        np.uint8, np.uint16, np.uint32, np.uint64, np.intc, np.int_,
-        np.longlong, np.uintc, np.ulonglong
+        np.float16,
+        np.float32,
+        np.float64,
+        np.longdouble,
+        np.int8,
+        np.int16,
+        np.int32,
+        np.int64,
+        np.complex64,
+        np.complex128,
+        np.clongdouble,
+        np.uint8,
+        np.uint16,
+        np.uint32,
+        np.uint64,
+        np.intc,
+        np.int_,
+        np.longlong,
+        np.uintc,
+        np.ulonglong,
     ]
     for d in all_dtypes:
       with self.subTest(d.__name__):
-        self.assertEqual((float_type, d) in allowed_casts,
-                         np.can_cast(float_type, d))
-        self.assertEqual((d, float_type) in allowed_casts,
-                         np.can_cast(d, float_type))
+        self.assertEqual(
+            (float_type, d) in allowed_casts, np.can_cast(float_type, d)
+        )
+        self.assertEqual(
+            (d, float_type) in allowed_casts, np.can_cast(d, float_type)
+        )
 
   def testCasts(self, float_type):
     for dtype in [
-        np.float16, np.float32, np.float64, np.longdouble, np.int8, np.int16,
-        np.int32, np.int64, np.complex64, np.complex128, np.clongdouble,
-        np.uint8, np.uint16, np.uint32, np.uint64, np.intc, np.int_,
-        np.longlong, np.uintc, np.ulonglong
+        np.float16,
+        np.float32,
+        np.float64,
+        np.longdouble,
+        np.int8,
+        np.int16,
+        np.int32,
+        np.int64,
+        np.complex64,
+        np.complex128,
+        np.clongdouble,
+        np.uint8,
+        np.uint16,
+        np.uint32,
+        np.uint64,
+        np.intc,
+        np.int_,
+        np.longlong,
+        np.uintc,
+        np.ulonglong,
     ]:
       x = np.array([[1, 2, 3]], dtype=dtype)
       y = x.astype(float_type)
       z = y.astype(dtype)
       self.assertTrue(np.all(x == y))
       self.assertEqual(float_type, y.dtype)
       self.assertTrue(np.all(x == z))
@@ -571,15 +701,16 @@
       z_np = y_np.astype(dtype)
       z_tf = y_tf.astype(dtype)
       numpy_assert_allclose(z_np, z_tf, atol=2e-2, float_type=float_type)
 
   def testArange(self, float_type):
     np.testing.assert_equal(
         np.arange(100, dtype=np.float32).astype(float_type),
-        np.arange(100, dtype=float_type))
+        np.arange(100, dtype=float_type),
+    )
     np.testing.assert_equal(
         np.arange(-8, 8, 1, dtype=np.float32).astype(float_type),
         np.arange(-8, 8, 1, dtype=float_type),
     )
     np.testing.assert_equal(
         np.arange(-0.0, -2.0, -0.25, dtype=np.float32).astype(float_type),
         np.arange(-0.0, -2.0, -0.25, dtype=float_type),
@@ -596,40 +727,44 @@
       with self.subTest(op.__name__):
         rng = np.random.RandomState(seed=42)
         x = rng.randn(3, 7, 10).astype(float_type)
         numpy_assert_allclose(
             op(x).astype(np.float32),
             truncate(op(x.astype(np.float32)), float_type=float_type),
             rtol=1e-4,
-            float_type=float_type)
+            float_type=float_type,
+        )
 
   @ignore_warning(category=RuntimeWarning, message="invalid value encountered")
   @ignore_warning(category=RuntimeWarning, message="divide by zero encountered")
   def testBinaryUfunc(self, float_type):
     for op in BINARY_UFUNCS:
       with self.subTest(op.__name__):
         rng = np.random.RandomState(seed=42)
         x = rng.randn(3, 7, 10).astype(float_type)
         y = rng.randn(4, 1, 7, 10).astype(float_type)
         numpy_assert_allclose(
             op(x, y).astype(np.float32),
             truncate(
                 op(x.astype(np.float32), y.astype(np.float32)),
-                float_type=float_type),
+                float_type=float_type,
+            ),
             rtol=1e-4,
-            float_type=float_type)
+            float_type=float_type,
+        )
 
   def testBinaryPredicateUfunc(self, float_type):
     for op in BINARY_PREDICATE_UFUNCS:
       with self.subTest(op.__name__):
         rng = np.random.RandomState(seed=42)
         x = rng.randn(3, 7).astype(float_type)
         y = rng.randn(4, 1, 7).astype(float_type)
         np.testing.assert_equal(
-            op(x, y), op(x.astype(np.float32), y.astype(np.float32)))
+            op(x, y), op(x.astype(np.float32), y.astype(np.float32))
+        )
 
   def testPredicateUfunc(self, float_type):
     for op in [np.isfinite, np.isinf, np.isnan, np.signbit, np.logical_not]:
       with self.subTest(op.__name__):
         rng = np.random.RandomState(seed=42)
         shape = (3, 7, 10)
         posinf_flips = rng.rand(*shape) < 0.1
@@ -648,49 +783,54 @@
     y = rng.randn(4, 1, 7).astype(float_type)
     o1, o2 = np.divmod(x, y)
     e1, e2 = np.divmod(x.astype(np.float32), y.astype(np.float32))
     numpy_assert_allclose(
         o1,
         truncate(e1, float_type=float_type),
         rtol=1e-2,
-        float_type=float_type)
+        float_type=float_type,
+    )
     numpy_assert_allclose(
         o2,
         truncate(e2, float_type=float_type),
         rtol=1e-2,
-        float_type=float_type)
+        float_type=float_type,
+    )
 
   def testModf(self, float_type):
     rng = np.random.RandomState(seed=42)
     x = rng.randn(3, 7).astype(float_type)
     o1, o2 = np.modf(x)
     e1, e2 = np.modf(x.astype(np.float32))
     numpy_assert_allclose(
         o1.astype(np.float32),
         truncate(e1, float_type=float_type),
         rtol=1e-2,
-        float_type=float_type)
+        float_type=float_type,
+    )
     numpy_assert_allclose(
         o2.astype(np.float32),
         truncate(e2, float_type=float_type),
         rtol=1e-2,
-        float_type=float_type)
+        float_type=float_type,
+    )
 
   @ignore_warning(category=RuntimeWarning, message="invalid value encountered")
   def testLdexp(self, float_type):
     rng = np.random.RandomState(seed=42)
     x = rng.randn(3, 7).astype(float_type)
     y = rng.randint(-50, 50, (1, 7)).astype(np.int32)
     self.assertEqual(np.ldexp(x, y).dtype, x.dtype)
     numpy_assert_allclose(
         np.ldexp(x, y).astype(np.float32),
         truncate(np.ldexp(x.astype(np.float32), y), float_type=float_type),
         rtol=1e-2,
         atol=1e-6,
-        float_type=float_type)
+        float_type=float_type,
+    )
 
   def testFrexp(self, float_type):
     rng = np.random.RandomState(seed=42)
     x = rng.randn(3, 7).astype(float_type)
     mant1, exp1 = np.frexp(x)
     mant2, exp2 = np.frexp(x.astype(np.float32))
     np.testing.assert_equal(exp1, exp2)
@@ -705,57 +845,60 @@
         val_with_sign_bits = val_with_sign.view(bits_type)
         num_bits = np.iinfo(bits_type).bits
         np.testing.assert_equal(
             bits | (1 << (num_bits - 1)), val_with_sign_bits
         )
 
   def testNextAfter(self, float_type):
-    one = np.array(1., dtype=float_type)
-    two = np.array(2., dtype=float_type)
-    zero = np.array(0., dtype=float_type)
+    one = np.array(1.0, dtype=float_type)
+    two = np.array(2.0, dtype=float_type)
+    zero = np.array(0.0, dtype=float_type)
     nan = np.array(np.nan, dtype=float_type)
     np.testing.assert_equal(
-        np.nextafter(one, two) - one, FLOAT_EPSILON[float_type]
+        np.nextafter(one, two) - one, ml_dtypes.finfo(float_type).eps
     )
     np.testing.assert_equal(
-        np.nextafter(one, zero) - one, -FLOAT_EPSILON[float_type] / 2
+        np.nextafter(one, zero) - one, -ml_dtypes.finfo(float_type).eps / 2
     )
     np.testing.assert_equal(np.isnan(np.nextafter(nan, one)), True)
     np.testing.assert_equal(np.isnan(np.nextafter(one, nan)), True)
     np.testing.assert_equal(np.nextafter(one, one), one)
-    smallest_denormal = FLOAT_SMALLEST_SUBNORMAL[float_type]
+    smallest_denormal = ml_dtypes.finfo(float_type).smallest_subnormal
     np.testing.assert_equal(np.nextafter(zero, one), smallest_denormal)
     np.testing.assert_equal(np.nextafter(zero, -one), -smallest_denormal)
-    for a, b in itertools.permutations([0., nan], 2):
+    for a, b in itertools.permutations([0.0, nan], 2):
       np.testing.assert_equal(
           np.nextafter(
-              np.array(a, dtype=np.float32), np.array(b, dtype=np.float32)),
+              np.array(a, dtype=np.float32), np.array(b, dtype=np.float32)
+          ),
           np.nextafter(
-              np.array(a, dtype=float_type), np.array(b, dtype=float_type)))
+              np.array(a, dtype=float_type), np.array(b, dtype=float_type)
+          ),
+      )
 
   @ignore_warning(category=RuntimeWarning, message="invalid value encountered")
   def testSpacing(self, float_type):
     # Sweep a variety of binades to see that spacing gives the proper ULP.
     with self.subTest(name="Subnormals"):
       for i in range(
-          int(np.log2(FLOAT_SMALLEST_SUBNORMAL[float_type])),
-          int(np.log2(FLOAT_SMALLEST_NORMAL[float_type])),
+          int(np.log2(float(ml_dtypes.finfo(float_type).smallest_subnormal))),
+          int(np.log2(float(ml_dtypes.finfo(float_type).smallest_normal))),
       ):
         power_of_two = float_type(2.0**i)
-        distance = FLOAT_SMALLEST_SUBNORMAL[float_type]
+        distance = ml_dtypes.finfo(float_type).smallest_subnormal
         np.testing.assert_equal(np.spacing(power_of_two), distance)
         np.testing.assert_equal(np.spacing(-power_of_two), -distance)
     # Normals have a distance which depends on their binade.
     with self.subTest(name="Normals"):
       for i in range(
-          int(np.log2(FLOAT_SMALLEST_NORMAL[float_type])),
-          int(np.log2(FLOAT_MAX[float_type])),
+          int(np.log2(float(ml_dtypes.finfo(float_type).smallest_normal))),
+          int(np.log2(float(ml_dtypes.finfo(float_type).max))),
       ):
         power_of_two = float_type(2.0**i)
-        distance = FLOAT_EPSILON[float_type] * power_of_two
+        distance = ml_dtypes.finfo(float_type).eps * power_of_two
         np.testing.assert_equal(np.spacing(power_of_two), distance)
         np.testing.assert_equal(np.spacing(-power_of_two), -distance)
 
     # Check that spacing agrees with arithmetic involving nextafter.
     with self.subTest(name="NextAfter"):
       for x in FLOAT_VALUES[float_type]:
         x_float_type = float_type(x)
```

### Comparing `ml_dtypes-0.0.4/ml_dtypes/tests/metadata_test.py` & `ml_dtypes-0.1.0/ml_dtypes/tests/metadata_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from importlib import metadata
 
 from absl.testing import absltest
 import ml_dtypes
 
 
 class CustomFloatTest(absltest.TestCase):
+
   def test_version_matches_package_metadata(self):
     try:
       ml_dtypes_metadata = metadata.metadata("ml_dtypes")
     except ImportError as err:
       raise absltest.SkipTest("Package metadata not found") from err
 
     metadata_version = ml_dtypes_metadata["version"]
```

### Comparing `ml_dtypes-0.0.4/ml_dtypes.egg-info/PKG-INFO` & `ml_dtypes-0.1.0/ml_dtypes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-dtypes
-Version: 0.0.4
+Version: 0.1.0
 Author-email: ml_dtypes authors <ml_dtypes@google.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -200,14 +200,15 @@
                http://www.apache.org/licenses/LICENSE-2.0
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
+        
 Project-URL: homepage, https://github.com/jax-ml/ml_dtypes
 Project-URL: repository, https://github.com/jax-ml/ml_dtypes
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.7
@@ -229,15 +230,17 @@
 
 - [`bfloat16`](https://en.wikipedia.org/wiki/Bfloat16_floating-point_format):
   an alternative to the standard [`float16`](https://en.wikipedia.org/wiki/Half-precision_floating-point_format) format
 - `float8_*`: several experimental 8-bit floating point representations
   including:
   * `float8_e4m3b11`
   * `float8_e4m3fn`
+  * `float8_e4m3fnuz`
   * `float8_e5m2`
+  * `float8_e5m2fnuz`
 
 ## Installation
 
 The `ml_dtypes` package is tested with Python versions 3.8-3.11, and can be installed
 with the following command:
 ```
 pip install ml_dtypes
```

### Comparing `ml_dtypes-0.0.4/ml_dtypes.egg-info/SOURCES.txt` & `ml_dtypes-0.1.0/ml_dtypes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/pyproject.toml` & `ml_dtypes-0.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ml_dtypes"
-version = "0.0.4"  # Keep in sync with ml_dtypes/__init__.py:__version__
+version = "0.1.0"  # Keep in sync with ml_dtypes/__init__.py:__version__
 description = ""
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 authors = [{name = "ml_dtypes authors", email="ml_dtypes@google.com"}]
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -36,14 +36,16 @@
     "pytest-xdist",
     "pylint>=2.6.0",
     "pyink",
 ]
 
 [tool.pyink]
 # Formatting configuration to follow Google style-guide
+line-length = 80
+preview = true
 pyink-indentation = 2
 pyink-use-majority-quotes = true
 
 [build-system]
 requires = [
     # Build with oldest supported numpy for each Python version.
     "numpy~=1.21.2; python_version<'3.11'",
```

### Comparing `ml_dtypes-0.0.4/setup.py` & `ml_dtypes-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,16 @@
 
 
 class build_py(build_py_orig):  # pylint: disable=invalid-name
 
   def find_package_modules(self, package, package_dir):
     modules = super().find_package_modules(package, package_dir)
     return [  # pylint: disable=g-complex-comprehension
-        (pkg, mod, file) for (pkg, mod, file) in modules
+        (pkg, mod, file)
+        for (pkg, mod, file) in modules
         if not any(
             fnmatch.fnmatchcase(pkg + "." + mod, pat=pattern)
             for pattern in exclude
         )
     ]
```

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/Core` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/Core`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/ArithmeticSequence.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/ArithmeticSequence.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Array.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Array.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/ArrayBase.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/ArrayBase.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/ArrayWrapper.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/ArrayWrapper.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Assign.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Assign.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/AssignEvaluator.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/AssignEvaluator.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Assign_MKL.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Assign_MKL.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/BandMatrix.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/BandMatrix.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Block.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Block.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/CommaInitializer.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/CommaInitializer.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/ConditionEstimator.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/ConditionEstimator.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/CoreEvaluators.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/CoreEvaluators.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/CoreIterators.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/CoreIterators.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/CwiseBinaryOp.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/CwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/CwiseNullaryOp.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/CwiseNullaryOp.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/CwiseTernaryOp.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/CwiseTernaryOp.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/CwiseUnaryOp.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/CwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/CwiseUnaryView.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/CwiseUnaryView.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/DenseBase.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/DenseBase.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/DenseCoeffsBase.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/DenseCoeffsBase.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/DenseStorage.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/DenseStorage.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Diagonal.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Diagonal.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/DiagonalMatrix.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/DiagonalMatrix.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/DiagonalProduct.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/DiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Dot.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Dot.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/EigenBase.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/EigenBase.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/ForceAlignedAccess.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/ForceAlignedAccess.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Fuzzy.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Fuzzy.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/GeneralProduct.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/GeneralProduct.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/GenericPacketMath.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/GenericPacketMath.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/GlobalFunctions.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/GlobalFunctions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/IO.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/IO.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/IndexedView.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/IndexedView.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Inverse.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Inverse.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Map.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Map.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/MapBase.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/MapBase.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/MathFunctions.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/MathFunctionsImpl.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/MathFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Matrix.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Matrix.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/MatrixBase.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/MatrixBase.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/NestByValue.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/NestByValue.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/NoAlias.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/NoAlias.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/NumTraits.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/NumTraits.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/PartialReduxEvaluator.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/PartialReduxEvaluator.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/PermutationMatrix.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/PermutationMatrix.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/PlainObjectBase.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/PlainObjectBase.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Product.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Product.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/ProductEvaluators.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/ProductEvaluators.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Random.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Random.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Redux.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Redux.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Ref.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Ref.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Replicate.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Replicate.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Reshaped.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Reshaped.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/ReturnByValue.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/ReturnByValue.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Reverse.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Reverse.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Select.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Select.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/SelfAdjointView.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/SelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/SelfCwiseBinaryOp.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/SelfCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/SkewSymmetricMatrix3.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/SkewSymmetricMatrix3.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Solve.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Solve.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/SolveTriangular.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/SolveTriangular.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/SolverBase.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/SolverBase.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/StableNorm.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/StableNorm.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/StlIterators.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/StlIterators.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Stride.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Stride.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Swap.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Swap.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Transpose.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Transpose.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Transpositions.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Transpositions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/TriangularMatrix.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/TriangularMatrix.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/VectorBlock.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/VectorBlock.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/VectorwiseOp.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/VectorwiseOp.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/Visitor.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/Visitor.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/AVX/Complex.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX/Complex.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/AVX/MathFunctions.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/AVX/PacketMath.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX/PacketMath.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/AVX/TypeCasting.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/AVX512/Complex.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX512/Complex.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/AVX512/GemmKernel.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX512/GemmKernel.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/AVX512/MathFunctions.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX512/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/AVX512/PacketMath.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX512/PacketMath.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/AVX512/PacketMathFP16.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX512/PacketMathFP16.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/AVX512/TrsmKernel.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX512/TrsmKernel.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/AVX512/TypeCasting.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AVX512/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/AltiVec/Complex.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/Complex.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/AltiVec/MathFunctions.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProduct.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProduct.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMAbfloat16.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMAbfloat16.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixVectorProduct.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/MatrixVectorProduct.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/AltiVec/PacketMath.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/AltiVec/PacketMath.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/Default/BFloat16.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/Default/BFloat16.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/Default/ConjHelper.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/Default/ConjHelper.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/Default/Half.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/Default/Half.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/Default/Settings.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/Default/Settings.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/Default/TypeCasting.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/Default/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/GPU/Complex.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/GPU/Complex.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/GPU/MathFunctions.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/GPU/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/GPU/PacketMath.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/GPU/PacketMath.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/GPU/Tuple.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/GPU/Tuple.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/GPU/TypeCasting.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/GPU/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/HIP/hcc/math_constants.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/HIP/hcc/math_constants.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/MSA/Complex.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/MSA/Complex.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/MSA/MathFunctions.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/MSA/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/MSA/PacketMath.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/MSA/PacketMath.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/NEON/Complex.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/NEON/Complex.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/NEON/MathFunctions.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/NEON/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/NEON/PacketMath.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/NEON/PacketMath.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/NEON/TypeCasting.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/NEON/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/NEON/UnaryFunctors.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/NEON/UnaryFunctors.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/SSE/Complex.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SSE/Complex.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/SSE/MathFunctions.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SSE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/SSE/PacketMath.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SSE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/SSE/TypeCasting.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SSE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/SVE/MathFunctions.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SVE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/SVE/PacketMath.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SVE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/SVE/TypeCasting.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SVE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/SYCL/InteropHeaders.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SYCL/InteropHeaders.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/SYCL/MathFunctions.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SYCL/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/SYCL/PacketMath.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SYCL/PacketMath.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/SYCL/TypeCasting.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/SYCL/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/ZVector/Complex.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/ZVector/Complex.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/ZVector/MathFunctions.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/ZVector/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/arch/ZVector/PacketMath.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/arch/ZVector/PacketMath.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/functors/AssignmentFunctors.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/functors/AssignmentFunctors.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/functors/BinaryFunctors.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/functors/BinaryFunctors.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/functors/NullaryFunctors.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/functors/NullaryFunctors.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/functors/StlFunctors.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/functors/StlFunctors.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/functors/TernaryFunctors.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/functors/TernaryFunctors.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/functors/UnaryFunctors.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/functors/UnaryFunctors.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/GeneralBlockPanelKernel.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrix.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/GeneralMatrixVector.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/GeneralMatrixVector.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/Parallelizer.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/Parallelizer.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixVector.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixVector.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/SelfadjointProduct.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/SelfadjointProduct.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/SelfadjointRank2Update.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/SelfadjointRank2Update.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/TriangularMatrixMatrix.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/TriangularMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/TriangularMatrixVector.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/TriangularMatrixVector.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/TriangularSolverMatrix.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/TriangularSolverMatrix.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/products/TriangularSolverVector.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/products/TriangularSolverVector.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/util/Assert.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/Assert.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/util/BlasUtil.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/BlasUtil.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/util/ConfigureVectorization.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/ConfigureVectorization.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/util/Constants.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/Constants.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/util/DisableStupidWarnings.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/DisableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/util/ForwardDeclarations.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/ForwardDeclarations.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/util/IndexedViewHelper.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/IndexedViewHelper.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/util/IntegralConstant.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/IntegralConstant.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/util/MKL_support.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/MKL_support.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/util/Macros.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/Macros.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/util/Memory.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/Memory.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/util/Meta.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/Meta.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/util/ReenableStupidWarnings.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/ReenableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/util/ReshapedHelper.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/ReshapedHelper.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/util/Serializer.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/Serializer.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/util/StaticAssert.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/StaticAssert.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/util/SymbolicIndex.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/SymbolicIndex.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/Core/util/XprHelper.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/Core/util/XprHelper.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/plugins/ArrayCwiseBinaryOps.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/plugins/ArrayCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/plugins/ArrayCwiseUnaryOps.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/plugins/ArrayCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/plugins/BlockMethods.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/plugins/BlockMethods.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/plugins/CommonCwiseBinaryOps.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/plugins/CommonCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/plugins/CommonCwiseUnaryOps.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/plugins/CommonCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/plugins/IndexedViewMethods.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/plugins/IndexedViewMethods.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/plugins/MatrixCwiseBinaryOps.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/plugins/MatrixCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/plugins/MatrixCwiseUnaryOps.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/plugins/MatrixCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `ml_dtypes-0.0.4/third_party/eigen/Eigen/src/plugins/ReshapedMethods.h` & `ml_dtypes-0.1.0/third_party/eigen/Eigen/src/plugins/ReshapedMethods.h`

 * *Files identical despite different names*

