# Comparing `tmp/squander-1.8.2.tar.gz` & `tmp/squander-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squander-1.8.2.tar", last modified: Thu May 18 07:29:19 2023, max compression
+gzip compressed data, was "squander-1.8.3.tar", last modified: Sun May 21 05:00:47 2023, max compression
```

## Comparing `squander-1.8.2.tar` & `squander-1.8.3.tar`

### file list

```diff
@@ -1,195 +1,195 @@
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.908699 squander-1.8.2/
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.880699 squander-1.8.2/.pytest_cache/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)      302 2023-05-18 07:01:34.000000 squander-1.8.2/.pytest_cache/README.md
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    14939 2023-05-18 07:00:48.000000 squander-1.8.2/CMakeLists.txt
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    35149 2023-05-18 07:00:49.000000 squander-1.8.2/LICENSE
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)      121 2023-05-18 07:00:49.000000 squander-1.8.2/MANIFEST.in
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    15001 2023-05-18 07:29:19.908699 squander-1.8.2/PKG-INFO
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    14413 2023-05-18 07:00:49.000000 squander-1.8.2/README.md
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.880699 squander-1.8.2/cmake/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4306 2023-05-18 07:00:49.000000 squander-1.8.2/cmake/check_AVX.cmake
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.884699 squander-1.8.2/common/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     6776 2023-05-18 07:00:49.000000 squander-1.8.2/common/Adam.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8316 2023-05-18 07:00:49.000000 squander-1.8.2/common/common.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5293 2023-05-18 07:00:49.000000 squander-1.8.2/common/common_DFE.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5524 2023-05-18 07:00:49.000000 squander-1.8.2/common/config_element.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    14292 2023-05-18 07:00:49.000000 squander-1.8.2/common/dot.cpp
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.884699 squander-1.8.2/common/include/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3441 2023-05-18 07:00:49.000000 squander-1.8.2/common/include/Adam.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)      166 2023-05-18 07:01:12.000000 squander-1.8.2/common/include/Config.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)      216 2023-05-18 07:00:49.000000 squander-1.8.2/common/include/Config.h.in
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2109 2023-05-18 07:00:49.000000 squander-1.8.2/common/include/QGDTypes.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5293 2023-05-18 07:00:49.000000 squander-1.8.2/common/include/common.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3026 2023-05-18 07:00:49.000000 squander-1.8.2/common/include/common_DFE.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3423 2023-05-18 07:00:49.000000 squander-1.8.2/common/include/config_element.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7626 2023-05-18 07:00:49.000000 squander-1.8.2/common/include/dot.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     9130 2023-05-18 07:00:49.000000 squander-1.8.2/common/include/lbfgs.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2443 2023-05-18 07:00:49.000000 squander-1.8.2/common/include/logging.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3812 2023-05-18 07:00:49.000000 squander-1.8.2/common/include/matrix.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    13485 2023-05-18 07:00:49.000000 squander-1.8.2/common/include/matrix_base.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3746 2023-05-18 07:00:49.000000 squander-1.8.2/common/include/matrix_real.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1393 2023-05-18 07:00:49.000000 squander-1.8.2/common/include/mpi_base.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1468 2023-05-18 07:00:49.000000 squander-1.8.2/common/include/numpy_interface.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     9251 2023-05-18 07:00:49.000000 squander-1.8.2/common/include/tolmin.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)   156010 2023-05-18 07:00:49.000000 squander-1.8.2/common/lbfgs.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2515 2023-05-18 07:00:49.000000 squander-1.8.2/common/logging.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5065 2023-05-18 07:00:49.000000 squander-1.8.2/common/matrix.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4491 2023-05-18 07:00:49.000000 squander-1.8.2/common/matrix_real.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1095 2023-05-18 07:00:49.000000 squander-1.8.2/common/mpi_base.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4808 2023-05-18 07:00:49.000000 squander-1.8.2/common/numpy_interface.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    58244 2023-05-18 07:00:49.000000 squander-1.8.2/common/tolmin.cpp
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.888699 squander-1.8.2/decomposition/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    57706 2023-05-18 07:00:49.000000 squander-1.8.2/decomposition/Decomposition_Base.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    37081 2023-05-18 07:00:49.000000 squander-1.8.2/decomposition/N_Qubit_Decomposition.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)   100513 2023-05-18 07:00:49.000000 squander-1.8.2/decomposition/N_Qubit_Decomposition_Base.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    16714 2023-05-18 07:00:49.000000 squander-1.8.2/decomposition/N_Qubit_Decomposition_Cost_Function.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    77317 2023-05-18 07:00:49.000000 squander-1.8.2/decomposition/N_Qubit_Decomposition_adaptive.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    12741 2023-05-18 07:00:49.000000 squander-1.8.2/decomposition/N_Qubit_Decomposition_custom.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    23502 2023-05-18 07:00:49.000000 squander-1.8.2/decomposition/Sub_Matrix_Decomposition.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8536 2023-05-18 07:00:49.000000 squander-1.8.2/decomposition/Sub_Matrix_Decomposition_Cost_Function.cpp
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.888699 squander-1.8.2/decomposition/include/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    16035 2023-05-18 07:00:49.000000 squander-1.8.2/decomposition/include/Decomposition_Base.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7166 2023-05-18 07:00:49.000000 squander-1.8.2/decomposition/include/N_Qubit_Decomposition.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    15865 2023-05-18 07:00:49.000000 squander-1.8.2/decomposition/include/N_Qubit_Decomposition_Base.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5077 2023-05-18 07:00:49.000000 squander-1.8.2/decomposition/include/N_Qubit_Decomposition_Cost_Function.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8301 2023-05-18 07:00:49.000000 squander-1.8.2/decomposition/include/N_Qubit_Decomposition_adaptive.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3393 2023-05-18 07:00:49.000000 squander-1.8.2/decomposition/include/N_Qubit_Decomposition_custom.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     6922 2023-05-18 07:00:49.000000 squander-1.8.2/decomposition/include/Sub_Matrix_Decomposition.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3723 2023-05-18 07:00:49.000000 squander-1.8.2/decomposition/include/Sub_Matrix_Decomposition_Cost_Function.h
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.892699 squander-1.8.2/gates/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5728 2023-05-18 07:00:49.000000 squander-1.8.2/gates/Adaptive.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4900 2023-05-18 07:00:49.000000 squander-1.8.2/gates/CH.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4937 2023-05-18 07:00:49.000000 squander-1.8.2/gates/CNOT.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5839 2023-05-18 07:00:49.000000 squander-1.8.2/gates/CRY.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4841 2023-05-18 07:00:49.000000 squander-1.8.2/gates/CZ.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7781 2023-05-18 07:00:49.000000 squander-1.8.2/gates/Composite.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    11545 2023-05-18 07:00:49.000000 squander-1.8.2/gates/Gate.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)   120998 2023-05-18 07:00:49.000000 squander-1.8.2/gates/Gates_block.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8547 2023-05-18 07:00:49.000000 squander-1.8.2/gates/ON.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     6819 2023-05-18 07:00:49.000000 squander-1.8.2/gates/RX.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     6815 2023-05-18 07:00:49.000000 squander-1.8.2/gates/RY.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7110 2023-05-18 07:00:49.000000 squander-1.8.2/gates/RZ.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8697 2023-05-18 07:00:49.000000 squander-1.8.2/gates/SX.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     9587 2023-05-18 07:00:49.000000 squander-1.8.2/gates/SYC.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    15472 2023-05-18 07:00:49.000000 squander-1.8.2/gates/U3.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8769 2023-05-18 07:00:49.000000 squander-1.8.2/gates/UN.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7950 2023-05-18 07:00:49.000000 squander-1.8.2/gates/X.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5671 2023-05-18 07:00:49.000000 squander-1.8.2/gates/Y.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5672 2023-05-18 07:00:49.000000 squander-1.8.2/gates/Z.cpp
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.896699 squander-1.8.2/gates/include/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3395 2023-05-18 07:00:49.000000 squander-1.8.2/gates/include/Adaptive.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2428 2023-05-18 07:00:49.000000 squander-1.8.2/gates/include/CH.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2504 2023-05-18 07:00:49.000000 squander-1.8.2/gates/include/CNOT.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3113 2023-05-18 07:00:49.000000 squander-1.8.2/gates/include/CRY.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2427 2023-05-18 07:00:49.000000 squander-1.8.2/gates/include/CZ.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3594 2023-05-18 07:00:49.000000 squander-1.8.2/gates/include/Composite.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5097 2023-05-18 07:00:49.000000 squander-1.8.2/gates/include/Gate.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    15824 2023-05-18 07:00:49.000000 squander-1.8.2/gates/include/Gates_block.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3412 2023-05-18 07:00:49.000000 squander-1.8.2/gates/include/ON.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2812 2023-05-18 07:00:49.000000 squander-1.8.2/gates/include/RX.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3088 2023-05-18 07:00:49.000000 squander-1.8.2/gates/include/RY.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2808 2023-05-18 07:00:49.000000 squander-1.8.2/gates/include/RZ.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2783 2023-05-18 07:00:49.000000 squander-1.8.2/gates/include/SX.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2428 2023-05-18 07:00:49.000000 squander-1.8.2/gates/include/SYC.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     6017 2023-05-18 07:00:49.000000 squander-1.8.2/gates/include/U3.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3412 2023-05-18 07:00:49.000000 squander-1.8.2/gates/include/UN.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2774 2023-05-18 07:00:49.000000 squander-1.8.2/gates/include/X.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2772 2023-05-18 07:00:49.000000 squander-1.8.2/gates/include/Y.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2772 2023-05-18 07:00:49.000000 squander-1.8.2/gates/include/Z.h
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.896699 squander-1.8.2/gates/kernels/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    23561 2023-05-18 07:00:49.000000 squander-1.8.2/gates/kernels/apply_kernel_to_input_AVX.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    32382 2023-05-18 07:00:49.000000 squander-1.8.2/gates/kernels/apply_kernel_to_state_vector_input.cpp
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.896699 squander-1.8.2/gates/kernels/include/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1786 2023-05-18 07:00:49.000000 squander-1.8.2/gates/kernels/include/apply_kernel_to_input_AVX.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2099 2023-05-18 07:00:49.000000 squander-1.8.2/gates/kernels/include/apply_kernel_to_state_vector_input.h
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.896699 squander-1.8.2/nn/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    18464 2023-05-18 07:00:49.000000 squander-1.8.2/nn/NN.cpp
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.896699 squander-1.8.2/nn/include/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5274 2023-05-18 07:00:49.000000 squander-1.8.2/nn/include/NN.h
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.896699 squander-1.8.2/optimization_engines/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     9698 2023-05-18 07:00:49.000000 squander-1.8.2/optimization_engines/RL_experience.cpp
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.896699 squander-1.8.2/optimization_engines/include/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3549 2023-05-18 07:00:49.000000 squander-1.8.2/optimization_engines/include/RL_experience.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)      123 2023-05-18 07:00:49.000000 squander-1.8.2/pyproject.toml
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.900699 squander-1.8.2/qgd_python/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)       27 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/__init__.py
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.900699 squander-1.8.2/qgd_python/decomposition/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4386 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/decomposition/CMakeLists.txt
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)       27 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/decomposition/__init__.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7661 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/decomposition/qgd_N_Qubit_Decomposition.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    36730 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/decomposition/qgd_N_Qubit_Decomposition_Wrapper.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    25000 2023-05-18 07:01:03.000000 squander-1.8.2/qgd_python/decomposition/qgd_N_Qubit_Decomposition_adaptive.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    82645 2023-05-18 07:01:03.000000 squander-1.8.2/qgd_python/decomposition/qgd_N_Qubit_Decomposition_adaptive_Wrapper.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    14278 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/decomposition/qgd_N_Qubit_Decomposition_custom.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    41007 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/decomposition/qgd_N_Qubit_Decomposition_custom_Wrapper.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3367 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/decomposition/qgd_N_Qubit_State_Preparation_adaptive.py
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.900699 squander-1.8.2/qgd_python/decomposition/test/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/decomposition/test/__init__.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    11024 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/decomposition/test/test_Compression.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1927 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/decomposition/test/test_Global_Phase.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7037 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/decomposition/test/test_IBM.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1777 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/decomposition/test/test_Project_Name.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5616 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/decomposition/test/test_QX2.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4399 2023-05-18 07:24:24.000000 squander-1.8.2/qgd_python/decomposition/test/test_State_Preparation.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1656 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/decomposition/test/test_Unitary.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4672 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/decomposition/test/test_decomposition.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7190 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/decomposition/test/test_fmo.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7018 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/decomposition/test/test_heavy_hex.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5222 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/decomposition/test/test_optmization_problem_combined.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4905 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/decomposition/test/test_parametric_circuit.py
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.904699 squander-1.8.2/qgd_python/gates/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    13547 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/CMakeLists.txt
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/__init__.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8219 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/qgd_CH.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8160 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/qgd_CNOT.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8033 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/qgd_CZ.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    28536 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/qgd_Gates_Block.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8529 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/qgd_RX.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8528 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/qgd_RY.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8527 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/qgd_RZ.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7771 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/qgd_SX.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7801 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/qgd_SYC.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     9054 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/qgd_U3.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7489 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/qgd_X.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8367 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/qgd_Y.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8367 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/qgd_Z.cpp
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.908699 squander-1.8.2/qgd_python/gates/test/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/test/__init__.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3364 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/test/test_CH.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3409 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/test/test_CNOT.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3444 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/test/test_CZ.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3466 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/test/test_RX.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3348 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/test/test_RY.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3919 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/test/test_RZ.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3278 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/test/test_SX.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3676 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/test/test_U3.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3182 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/test/test_X.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3179 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/test/test_Y.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3232 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/test/test_Z.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     6878 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/gates/test/test_gates.py
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.908699 squander-1.8.2/qgd_python/nn/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1304 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/nn/CMakeLists.txt
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)       27 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/nn/__init__.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2387 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/nn/qgd_nn.py
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     9635 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/nn/qgd_nn_Wrapper.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1573 2023-05-18 07:00:49.000000 squander-1.8.2/qgd_python/utils.py
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.908699 squander-1.8.2/random_unitary/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     6628 2023-05-18 07:00:49.000000 squander-1.8.2/random_unitary/Random_Orthogonal.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    11039 2023-05-18 07:00:49.000000 squander-1.8.2/random_unitary/Random_Unitary.cpp
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.908699 squander-1.8.2/random_unitary/include/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1927 2023-05-18 07:00:49.000000 squander-1.8.2/random_unitary/include/Random_Orthogonal.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4476 2023-05-18 07:00:49.000000 squander-1.8.2/random_unitary/include/Random_Unitary.h
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)       38 2023-05-18 07:29:19.908699 squander-1.8.2/setup.cfg
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1898 2023-05-18 07:28:49.000000 squander-1.8.2/setup.py
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.908699 squander-1.8.2/squander/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1442 2023-05-18 07:00:49.000000 squander-1.8.2/squander/__init__.py
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.908699 squander-1.8.2/squander.egg-info/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    15001 2023-05-18 07:29:19.000000 squander-1.8.2/squander.egg-info/PKG-INFO
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5181 2023-05-18 07:29:19.000000 squander-1.8.2/squander.egg-info/SOURCES.txt
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)        1 2023-05-18 07:29:19.000000 squander-1.8.2/squander.egg-info/dependency_links.txt
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)       50 2023-05-18 07:29:19.000000 squander-1.8.2/squander.egg-info/requires.txt
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)       20 2023-05-18 07:29:19.000000 squander-1.8.2/squander.egg-info/top_level.txt
-drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-18 07:29:19.908699 squander-1.8.2/test_standalone/
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1996 2023-05-18 07:00:49.000000 squander-1.8.2/test_standalone/CMakeLists.txt
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     6325 2023-05-18 07:00:49.000000 squander-1.8.2/test_standalone/custom_gate_structure_test.cpp
--rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4837 2023-05-18 07:00:49.000000 squander-1.8.2/test_standalone/decomposition_test.cpp
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.319089 squander-1.8.3/
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.295089 squander-1.8.3/.pytest_cache/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)      302 2023-05-20 20:13:53.000000 squander-1.8.3/.pytest_cache/README.md
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    15412 2023-05-21 04:59:59.000000 squander-1.8.3/CMakeLists.txt
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    35149 2023-05-20 20:06:21.000000 squander-1.8.3/LICENSE
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)      121 2023-05-20 20:06:21.000000 squander-1.8.3/MANIFEST.in
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    15887 2023-05-21 05:00:47.319089 squander-1.8.3/PKG-INFO
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    15299 2023-05-20 20:07:48.000000 squander-1.8.3/README.md
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.295089 squander-1.8.3/cmake/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4306 2023-05-20 20:06:21.000000 squander-1.8.3/cmake/check_AVX.cmake
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.295089 squander-1.8.3/common/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     6776 2023-05-20 20:06:21.000000 squander-1.8.3/common/Adam.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8316 2023-05-20 20:06:21.000000 squander-1.8.3/common/common.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5293 2023-05-20 20:06:21.000000 squander-1.8.3/common/common_DFE.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5524 2023-05-20 20:06:21.000000 squander-1.8.3/common/config_element.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    14292 2023-05-20 20:06:21.000000 squander-1.8.3/common/dot.cpp
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.299089 squander-1.8.3/common/include/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3441 2023-05-20 20:06:21.000000 squander-1.8.3/common/include/Adam.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)      166 2023-05-20 20:08:18.000000 squander-1.8.3/common/include/Config.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)      216 2023-05-20 20:06:21.000000 squander-1.8.3/common/include/Config.h.in
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2109 2023-05-20 20:06:21.000000 squander-1.8.3/common/include/QGDTypes.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5357 2023-05-20 20:07:48.000000 squander-1.8.3/common/include/common.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3026 2023-05-20 20:06:21.000000 squander-1.8.3/common/include/common_DFE.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3423 2023-05-20 20:06:21.000000 squander-1.8.3/common/include/config_element.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7798 2023-05-20 20:07:48.000000 squander-1.8.3/common/include/dot.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     9130 2023-05-20 20:06:21.000000 squander-1.8.3/common/include/lbfgs.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2443 2023-05-20 20:06:21.000000 squander-1.8.3/common/include/logging.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3812 2023-05-20 20:06:21.000000 squander-1.8.3/common/include/matrix.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    13831 2023-05-20 20:07:48.000000 squander-1.8.3/common/include/matrix_base.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3752 2023-05-20 20:07:48.000000 squander-1.8.3/common/include/matrix_real.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1393 2023-05-20 20:06:21.000000 squander-1.8.3/common/include/mpi_base.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1468 2023-05-20 20:06:21.000000 squander-1.8.3/common/include/numpy_interface.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     9234 2023-05-20 20:07:48.000000 squander-1.8.3/common/include/tolmin.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)   156010 2023-05-20 20:06:21.000000 squander-1.8.3/common/lbfgs.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2515 2023-05-20 20:06:21.000000 squander-1.8.3/common/logging.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5065 2023-05-20 20:06:21.000000 squander-1.8.3/common/matrix.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4497 2023-05-20 20:07:48.000000 squander-1.8.3/common/matrix_real.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1095 2023-05-20 20:06:21.000000 squander-1.8.3/common/mpi_base.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4808 2023-05-20 20:06:21.000000 squander-1.8.3/common/numpy_interface.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    58339 2023-05-20 20:07:48.000000 squander-1.8.3/common/tolmin.cpp
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.299089 squander-1.8.3/decomposition/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    57710 2023-05-20 20:07:48.000000 squander-1.8.3/decomposition/Decomposition_Base.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    37081 2023-05-20 20:06:21.000000 squander-1.8.3/decomposition/N_Qubit_Decomposition.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)   103422 2023-05-20 20:07:48.000000 squander-1.8.3/decomposition/N_Qubit_Decomposition_Base.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    16714 2023-05-20 20:06:21.000000 squander-1.8.3/decomposition/N_Qubit_Decomposition_Cost_Function.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    70942 2023-05-21 04:51:46.000000 squander-1.8.3/decomposition/N_Qubit_Decomposition_adaptive.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    12741 2023-05-20 20:06:21.000000 squander-1.8.3/decomposition/N_Qubit_Decomposition_custom.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    23508 2023-05-20 20:07:48.000000 squander-1.8.3/decomposition/Sub_Matrix_Decomposition.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8536 2023-05-20 20:06:21.000000 squander-1.8.3/decomposition/Sub_Matrix_Decomposition_Cost_Function.cpp
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.303089 squander-1.8.3/decomposition/include/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    16528 2023-05-20 20:07:48.000000 squander-1.8.3/decomposition/include/Decomposition_Base.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7166 2023-05-20 20:06:21.000000 squander-1.8.3/decomposition/include/N_Qubit_Decomposition.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    15866 2023-05-20 20:07:48.000000 squander-1.8.3/decomposition/include/N_Qubit_Decomposition_Base.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5077 2023-05-20 20:06:21.000000 squander-1.8.3/decomposition/include/N_Qubit_Decomposition_Cost_Function.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8301 2023-05-20 20:06:21.000000 squander-1.8.3/decomposition/include/N_Qubit_Decomposition_adaptive.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3393 2023-05-20 20:06:21.000000 squander-1.8.3/decomposition/include/N_Qubit_Decomposition_custom.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     6924 2023-05-20 20:07:48.000000 squander-1.8.3/decomposition/include/Sub_Matrix_Decomposition.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3723 2023-05-20 20:06:21.000000 squander-1.8.3/decomposition/include/Sub_Matrix_Decomposition_Cost_Function.h
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.307089 squander-1.8.3/gates/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5728 2023-05-20 20:06:21.000000 squander-1.8.3/gates/Adaptive.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4900 2023-05-20 20:06:21.000000 squander-1.8.3/gates/CH.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4937 2023-05-20 20:06:21.000000 squander-1.8.3/gates/CNOT.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5839 2023-05-20 20:06:21.000000 squander-1.8.3/gates/CRY.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4841 2023-05-20 20:06:21.000000 squander-1.8.3/gates/CZ.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7781 2023-05-20 20:06:21.000000 squander-1.8.3/gates/Composite.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    11545 2023-05-20 20:06:21.000000 squander-1.8.3/gates/Gate.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)   120998 2023-05-20 20:06:21.000000 squander-1.8.3/gates/Gates_block.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8547 2023-05-20 20:06:21.000000 squander-1.8.3/gates/ON.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     6819 2023-05-20 20:06:21.000000 squander-1.8.3/gates/RX.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     6815 2023-05-20 20:06:21.000000 squander-1.8.3/gates/RY.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7110 2023-05-20 20:06:21.000000 squander-1.8.3/gates/RZ.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8697 2023-05-20 20:06:21.000000 squander-1.8.3/gates/SX.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     9587 2023-05-20 20:06:21.000000 squander-1.8.3/gates/SYC.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    15472 2023-05-20 20:06:21.000000 squander-1.8.3/gates/U3.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8769 2023-05-20 20:06:21.000000 squander-1.8.3/gates/UN.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7950 2023-05-20 20:06:21.000000 squander-1.8.3/gates/X.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5671 2023-05-20 20:06:21.000000 squander-1.8.3/gates/Y.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5672 2023-05-20 20:06:21.000000 squander-1.8.3/gates/Z.cpp
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.307089 squander-1.8.3/gates/include/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3421 2023-05-20 20:07:48.000000 squander-1.8.3/gates/include/Adaptive.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2454 2023-05-20 20:07:48.000000 squander-1.8.3/gates/include/CH.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2530 2023-05-20 20:07:48.000000 squander-1.8.3/gates/include/CNOT.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3139 2023-05-20 20:07:48.000000 squander-1.8.3/gates/include/CRY.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2453 2023-05-20 20:07:48.000000 squander-1.8.3/gates/include/CZ.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3594 2023-05-20 20:06:21.000000 squander-1.8.3/gates/include/Composite.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5097 2023-05-20 20:06:21.000000 squander-1.8.3/gates/include/Gate.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    15824 2023-05-20 20:06:21.000000 squander-1.8.3/gates/include/Gates_block.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3412 2023-05-20 20:06:21.000000 squander-1.8.3/gates/include/ON.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2838 2023-05-20 20:07:48.000000 squander-1.8.3/gates/include/RX.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3114 2023-05-20 20:07:48.000000 squander-1.8.3/gates/include/RY.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2834 2023-05-20 20:07:48.000000 squander-1.8.3/gates/include/RZ.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2809 2023-05-20 20:07:48.000000 squander-1.8.3/gates/include/SX.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2454 2023-05-20 20:07:48.000000 squander-1.8.3/gates/include/SYC.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     6043 2023-05-20 20:07:48.000000 squander-1.8.3/gates/include/U3.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3412 2023-05-20 20:06:21.000000 squander-1.8.3/gates/include/UN.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2800 2023-05-20 20:07:48.000000 squander-1.8.3/gates/include/X.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2798 2023-05-20 20:07:48.000000 squander-1.8.3/gates/include/Y.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2798 2023-05-20 20:07:48.000000 squander-1.8.3/gates/include/Z.h
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.307089 squander-1.8.3/gates/kernels/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    23630 2023-05-20 20:06:21.000000 squander-1.8.3/gates/kernels/apply_kernel_to_input_AVX.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    32382 2023-05-20 20:06:21.000000 squander-1.8.3/gates/kernels/apply_kernel_to_state_vector_input.cpp
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.307089 squander-1.8.3/gates/kernels/include/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1786 2023-05-20 20:06:21.000000 squander-1.8.3/gates/kernels/include/apply_kernel_to_input_AVX.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2099 2023-05-20 20:06:21.000000 squander-1.8.3/gates/kernels/include/apply_kernel_to_state_vector_input.h
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.311089 squander-1.8.3/nn/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    18465 2023-05-20 20:07:48.000000 squander-1.8.3/nn/NN.cpp
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.311089 squander-1.8.3/nn/include/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5212 2023-05-20 20:07:48.000000 squander-1.8.3/nn/include/NN.h
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.311089 squander-1.8.3/optimization_engines/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     9698 2023-05-20 20:06:21.000000 squander-1.8.3/optimization_engines/RL_experience.cpp
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.311089 squander-1.8.3/optimization_engines/include/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3549 2023-05-20 20:06:21.000000 squander-1.8.3/optimization_engines/include/RL_experience.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)      123 2023-05-20 20:06:21.000000 squander-1.8.3/pyproject.toml
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.311089 squander-1.8.3/qgd_python/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)       27 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/__init__.py
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.311089 squander-1.8.3/qgd_python/decomposition/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4472 2023-05-20 20:07:48.000000 squander-1.8.3/qgd_python/decomposition/CMakeLists.txt
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)       27 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/decomposition/__init__.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7661 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/decomposition/qgd_N_Qubit_Decomposition.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    36701 2023-05-20 20:07:48.000000 squander-1.8.3/qgd_python/decomposition/qgd_N_Qubit_Decomposition_Wrapper.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    25000 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/decomposition/qgd_N_Qubit_Decomposition_adaptive.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    82737 2023-05-20 20:07:48.000000 squander-1.8.3/qgd_python/decomposition/qgd_N_Qubit_Decomposition_adaptive_Wrapper.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    14278 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/decomposition/qgd_N_Qubit_Decomposition_custom.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    40978 2023-05-20 20:07:48.000000 squander-1.8.3/qgd_python/decomposition/qgd_N_Qubit_Decomposition_custom_Wrapper.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3367 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/decomposition/qgd_N_Qubit_State_Preparation_adaptive.py
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.315089 squander-1.8.3/qgd_python/decomposition/test/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)        0 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/decomposition/test/__init__.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    11024 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/decomposition/test/test_Compression.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1927 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/decomposition/test/test_Global_Phase.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7037 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/decomposition/test/test_IBM.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1777 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/decomposition/test/test_Project_Name.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5616 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/decomposition/test/test_QX2.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4399 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/decomposition/test/test_State_Preparation.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1656 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/decomposition/test/test_Unitary.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4672 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/decomposition/test/test_decomposition.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7190 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/decomposition/test/test_fmo.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7018 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/decomposition/test/test_heavy_hex.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     6583 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/decomposition/test/test_optmization_problem_combined.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4905 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/decomposition/test/test_parametric_circuit.py
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.315089 squander-1.8.3/qgd_python/gates/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    13911 2023-05-20 20:07:48.000000 squander-1.8.3/qgd_python/gates/CMakeLists.txt
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)        0 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/gates/__init__.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8355 2023-05-20 20:07:48.000000 squander-1.8.3/qgd_python/gates/qgd_CH.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8292 2023-05-20 20:07:48.000000 squander-1.8.3/qgd_python/gates/qgd_CNOT.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8165 2023-05-20 20:07:48.000000 squander-1.8.3/qgd_python/gates/qgd_CZ.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    28668 2023-05-20 20:07:48.000000 squander-1.8.3/qgd_python/gates/qgd_Gates_Block.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8661 2023-05-20 20:07:48.000000 squander-1.8.3/qgd_python/gates/qgd_RX.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8660 2023-05-20 20:07:48.000000 squander-1.8.3/qgd_python/gates/qgd_RY.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8659 2023-05-20 20:07:48.000000 squander-1.8.3/qgd_python/gates/qgd_RZ.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7903 2023-05-20 20:07:48.000000 squander-1.8.3/qgd_python/gates/qgd_SX.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7941 2023-05-20 20:07:48.000000 squander-1.8.3/qgd_python/gates/qgd_SYC.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     9186 2023-05-20 20:07:48.000000 squander-1.8.3/qgd_python/gates/qgd_U3.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     7621 2023-05-20 20:07:48.000000 squander-1.8.3/qgd_python/gates/qgd_X.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8499 2023-05-20 20:07:48.000000 squander-1.8.3/qgd_python/gates/qgd_Y.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     8499 2023-05-20 20:07:48.000000 squander-1.8.3/qgd_python/gates/qgd_Z.cpp
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.319089 squander-1.8.3/qgd_python/gates/test/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)        0 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/gates/test/__init__.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3364 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/gates/test/test_CH.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3409 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/gates/test/test_CNOT.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3444 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/gates/test/test_CZ.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3466 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/gates/test/test_RX.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3348 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/gates/test/test_RY.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3919 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/gates/test/test_RZ.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3278 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/gates/test/test_SX.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3676 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/gates/test/test_U3.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3182 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/gates/test/test_X.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3179 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/gates/test/test_Y.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     3232 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/gates/test/test_Z.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     6878 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/gates/test/test_gates.py
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.319089 squander-1.8.3/qgd_python/nn/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1332 2023-05-20 20:07:48.000000 squander-1.8.3/qgd_python/nn/CMakeLists.txt
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)       27 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/nn/__init__.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     2387 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/nn/qgd_nn.py
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     9606 2023-05-20 20:07:48.000000 squander-1.8.3/qgd_python/nn/qgd_nn_Wrapper.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1573 2023-05-20 20:06:21.000000 squander-1.8.3/qgd_python/utils.py
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.319089 squander-1.8.3/random_unitary/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     6628 2023-05-20 20:06:21.000000 squander-1.8.3/random_unitary/Random_Orthogonal.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    11039 2023-05-20 20:06:21.000000 squander-1.8.3/random_unitary/Random_Unitary.cpp
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.319089 squander-1.8.3/random_unitary/include/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1927 2023-05-20 20:06:21.000000 squander-1.8.3/random_unitary/include/Random_Orthogonal.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4476 2023-05-20 20:06:21.000000 squander-1.8.3/random_unitary/include/Random_Unitary.h
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)       38 2023-05-21 05:00:47.319089 squander-1.8.3/setup.cfg
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1898 2023-05-21 05:00:10.000000 squander-1.8.3/setup.py
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.319089 squander-1.8.3/squander/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1442 2023-05-20 20:06:21.000000 squander-1.8.3/squander/__init__.py
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.319089 squander-1.8.3/squander.egg-info/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)    15887 2023-05-21 05:00:47.000000 squander-1.8.3/squander.egg-info/PKG-INFO
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     5181 2023-05-21 05:00:47.000000 squander-1.8.3/squander.egg-info/SOURCES.txt
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)        1 2023-05-21 05:00:47.000000 squander-1.8.3/squander.egg-info/dependency_links.txt
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)       50 2023-05-21 05:00:47.000000 squander-1.8.3/squander.egg-info/requires.txt
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)       20 2023-05-21 05:00:47.000000 squander-1.8.3/squander.egg-info/top_level.txt
+drwxrwxr-x   0 rakytap   (1002) rakytap   (1002)        0 2023-05-21 05:00:47.319089 squander-1.8.3/test_standalone/
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     1996 2023-05-20 20:06:21.000000 squander-1.8.3/test_standalone/CMakeLists.txt
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     6325 2023-05-20 20:06:21.000000 squander-1.8.3/test_standalone/custom_gate_structure_test.cpp
+-rw-rw-r--   0 rakytap   (1002) rakytap   (1002)     4837 2023-05-20 20:06:21.000000 squander-1.8.3/test_standalone/decomposition_test.cpp
```

### Comparing `squander-1.8.2/CMakeLists.txt` & `squander-1.8.3/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 cmake_minimum_required(VERSION 3.10.2)
 
 # CMAKE to create the shared library of the quantum gate decomposition project
 
 # set the project name and version
-project(CQGD VERSION 1.8.1)
+project(CQGD VERSION 1.8.3)
 
 # reuse compilation time linking for use runtime linking 
 SET(CMAKE_INSTALL_RPATH_USE_LINK_PATH TRUE)
 
 # specify the C++ standard
 set(CMAKE_CXX_STANDARD 11)
 set(CMAKE_CXX_STANDARD_REQUIRED True)
+set(CMAKE_WINDOWS_EXPORT_ALL_SYMBOLS ON) #for lib not just dll when no exports
 
 # include CMAKE modules
 include(CheckIncludeFile)
 include(CheckIncludeFileCXX)
 include(CheckFunctionExists)
 include(cmake/check_AVX.cmake)
 
@@ -42,15 +43,15 @@
              RETURN_VALUE PLATLIB_NOT_FOUND
             )
 if(PLATLIB_NOT_FOUND)
     message(FATAL_ERROR "Python platlib not found")
 endif()
 
 set(ENV{PYTHONPATH} "$ENV{PYTHONPATH};${PYTHON_PLAT_LIB}")
-message("PYTHONPATH is set to "$ENV{PYTHONPATH})
+message("PYTHONPATH is set to $ENV{PYTHONPATH}")
 
 # contruct library directories
 exec_program(${PYTHON_EXECUTABLE}
              ARGS "-c \"from distutils.sysconfig import get_python_lib; tmp = [s + '/../..' for s in [get_python_lib()]]; ret=';'.join(tmp); print(ret)\""
              OUTPUT_VARIABLE PYTHON_SYS_PATH
              RETURN_VALUE SYSPATH_NOT_FOUND
             )
@@ -223,52 +224,65 @@
   endif()
 
 endif()
 
 
 
 
+
 ############################################################xx
 # checking TBB libraries and headers
 
 # adding TBB library dir if given by environment variable
 if(DEFINED ENV{TBB_LIB_DIR})
-
-  find_library(TBB_LIB tbb
-               PATHS $ENV{TBB_LIB_DIR}
-               NO_DEFAULT_PATH
-               REQUIRED)
+  if (WIN32)
+    find_library(TBB_LIB tbb12
+                 PATHS $ENV{TBB_LIB_DIR}
+                 NO_DEFAULT_PATH
+                 REQUIRED)
+  else()
+    find_library(TBB_LIB tbb
+                 PATHS $ENV{TBB_LIB_DIR}
+                 NO_DEFAULT_PATH
+                 REQUIRED)
+  endif()
 
   find_library(TBBMALLOC_LIB tbbmalloc
                PATHS $ENV{TBB_LIB_DIR}
                NO_DEFAULT_PATH
                REQUIRED)
 
   find_library(TBBMALLOC_PROXY_LIB tbbmalloc_proxy
                PATHS $ENV{TBB_LIB_DIR}
                NO_DEFAULT_PATH
                REQUIRED)
 
 else()
 
-  find_library(TBB_LIB tbb
-               PATHS ${PYTHON_SYS_PATH}
-               NO_DEFAULT_PATH
-               REQUIRED)
+  if (WIN32)
+    find_library(TBB_LIB tbb12
+                 PATHS ${PYTHON_SYS_PATH}
+                 NO_DEFAULT_PATH
+                 REQUIRED)
+  else()
+    find_library(TBB_LIB tbb
+                 PATHS ${PYTHON_SYS_PATH}
+                 NO_DEFAULT_PATH
+                 REQUIRED)  
+  endif()
 
   find_library(TBBMALLOC_LIB tbbmalloc
                PATHS ${PYTHON_SYS_PATH}
                NO_DEFAULT_PATH
                REQUIRED)
 
   find_library(TBBMALLOC_PROXY_LIB tbbmalloc_proxy
                PATHS ${PYTHON_SYS_PATH}
                NO_DEFAULT_PATH
                REQUIRED)
-  
 endif()
 
 
 # adding TBB include dir
 if(DEFINED ENV{TBB_INC_DIR})
 
   set(CMAKE_REQUIRED_FLAGS "-c")
@@ -287,14 +301,15 @@
   check_include_file_cxx(tbb/tbb.h TBB_HEADER )
   list(APPEND EXTRA_INCLUDES "${CMAKE_REQUIRED_INCLUDES}") 
 
   if(NOT TBB_HEADER)
     message(FATAL_ERROR "TBB header tbb.h not found")
   endif()
 
+  list(APPEND EXTRA_INCLUDES "${TBB_HEADER}")
 
 endif()
 
 
 list(APPEND qgd_files 
     ${PROJECT_SOURCE_DIR}/common/common.cpp
     ${PROJECT_SOURCE_DIR}/common/config_element.cpp
@@ -368,21 +383,19 @@
 # adding compile options
 target_compile_options(qgd PUBLIC
     ${CXX_FLAGS}
     "$<$<CONFIG:Debug>:${CXX_FLAGS_DEBUG}>"
     "$<$<CONFIG:Release>:${CXX_FLAGS_RELEASE}>"
 )
 
-
-
 # adding linking options
 target_link_libraries( qgd PRIVATE
-    ${BLAS_LIBRARIES}
-    ${LAPACK_LIBRARIES}
-    ${LAPACKE_LIBRARIES}
+    "${BLAS_LIBRARIES}"
+    "${LAPACK_LIBRARIES}"
+    "${LAPACKE_LIBRARIES}"
     ${TBBMALLOC_LIB}
     ${TBBMALLOC_PROXY_LIB}
     ${TBB_LIB}
     ${MPI_C_LIBRARIES}
     )
```

### Comparing `squander-1.8.2/LICENSE` & `squander-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/PKG-INFO` & `squander-1.8.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squander
-Version: 1.8.2
+Version: 1.8.3
 Summary: Package to decompose unitaries into a quantum circuit and for quantum state preparation.
 Home-page: https://github.com/rakytap/sequential-quantum-gate-decomposer
 Maintainer: Peter Rakyta
 Maintainer-email: peter.rakyta@ttk.elte.hu
 License: GNU General Public License v3.0
 Keywords: test,cmake,extension
 Classifier: Intended Audience :: Developers
@@ -78,22 +78,20 @@
 
 Since version 1.7.1 the SQUANDER package is accessible at Python Package Index (PyPI). The package can be installed on linux systems following the steps outlined below:
 
 $ pip install numpy swig tbb-devel wheel scikit-build ninja qiskit
 
 $ pip install squander
 
-
-
 ### Download the SQUANDER package
 
 The developer version of the Quantum Gate Decomposer package can be downloaded from github repository [https://github.com/rakytap/quantum-gate-decomposer/tree/master](https://github.com/rakytap/quantum-gate-decomposer/tree/master).
 After the package is downloaded into the directory **path/to/SQUANDER/package** (which would be the path to the source code of the SQUANDER package), one can proceed to the compilation steps described in the next section.
 
-### How to build the SQUANDER package
+### How to build the SQUANDER package on Unix/Linux/MacOS
 
 The SQUANDER package is equipped with a Python build script and CMake tools to ease the compilation and the deployment of the package.
 The SQUANDER package is parallelized via Threading Building Block (TBB) libraries. If TBB is not present in the system, it can be easily installed via python package [tbb-devel](https://pypi.org/project/tbb-devel/).
 Alternatively the TBB libraries can be installed via apt or yum utility (sudo apt install libtbb-dev) or it can be downloaded from [https://github.com/oneapi-src/oneTBB](https://github.com/oneapi-src/oneTBB)   and built from source. 
 In this case one should supply the necessary environment variables pointing to the header and library files of the TBB package. For newer
 Intel compilers the TBB package is part of the Intel compiler package, similarly to the MKL package. If the TBB library is located at non-standrad path or the SQUANDER package is compiled with GNU compiler, then setting the
 
@@ -103,15 +101,43 @@
 
 environment variables are sufficient for successful compilation. 
 When the TBB library is installed via a python package, setting the environment variables above is not necessary.
 The SQUANDER package with C++ Python extensions can be compiled via the Python script **setup.py** located in the root directory of the SQUANDER package.
 The script automatically finds out the CBLAS library working behind the numpy package and uses it in further linking. 
 The **setup.py** script also build the C++ library of the SQUANDER package by making the appropriate CMake calls. 
 
+### Build and Install on Microsoft Windows with Microsoft Visual C++
+
+CMake must be in the path and able to find the MSVC compiler e.g.
+
+$ set PATH=%PATH%;C:\Program Files\cmake\bin
+
+Now set the TBB and BLAS folders and build via:
+
+$ set TBB_LOCATION=<Python_Folder>/LocalCache/local-packages
+
+$ set TBB_INC_DIR=%TBB_LOCATION%/Library/include
+
+$ set TBB_LIB_DIR=%TBB_LOCATION%/Library/lib
+
+$ set LIB=<BLAS_Location>/lib;<LAPACK_Location>/lib
+
+$ python setup.py build_ext -DTBB_HEADER=<TBB_Location>\Library\include\
+
+Installation merely requires copying DLL files (if they are not in the path):
+
+$ copy _skbuild\win-amd64-3.9\cmake-install\bin .\qgd_python\decomposition
+
+$ copy "%TBB_LOCATION%\Library\bin\tbb12.dll" .\qgd_python\decomposition
+
+$ copy "%TBB_LOCATION%\Library\bin\tbbmalloc.dll" .\qgd_python\decomposition
+
+Verify the installation:
 
+$ python -m pytest
 
 ### Developer build
 
 
 We recommend to install the SQUANDER package in the Anaconda environment. In order to install the necessary requirements, follow the steps below:
 
 Creating new python environment:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: squander Version: 1.8.2 Summary: Package to
+Metadata-Version: 2.1 Name: squander Version: 1.8.3 Summary: Package to
 decompose unitaries into a quantum circuit and for quantum state preparation.
 Home-page: https://github.com/rakytap/sequential-quantum-gate-decomposer
 Maintainer: Peter Rakyta Maintainer-email: peter.rakyta@ttk.elte.hu License:
 GNU General Public License v3.0 Keywords: test,cmake,extension Classifier:
 Intended Audience :: Developers Classifier: Natural Language :: English
 Classifier: Programming Language :: C Classifier: Programming Language :: C++
 Description-Content-Type: text/markdown License-File: LICENSE [![DOI](https://
@@ -63,41 +63,52 @@
 numpy swig tbb-devel wheel scikit-build ninja qiskit $ pip install squander ###
 Download the SQUANDER package The developer version of the Quantum Gate
 Decomposer package can be downloaded from github repository [https://
 github.com/rakytap/quantum-gate-decomposer/tree/master](https://github.com/
 rakytap/quantum-gate-decomposer/tree/master). After the package is downloaded
 into the directory **path/to/SQUANDER/package** (which would be the path to the
 source code of the SQUANDER package), one can proceed to the compilation steps
-described in the next section. ### How to build the SQUANDER package The
-SQUANDER package is equipped with a Python build script and CMake tools to ease
-the compilation and the deployment of the package. The SQUANDER package is
-parallelized via Threading Building Block (TBB) libraries. If TBB is not
-present in the system, it can be easily installed via python package [tbb-
-devel](https://pypi.org/project/tbb-devel/). Alternatively the TBB libraries
-can be installed via apt or yum utility (sudo apt install libtbb-dev) or it can
-be downloaded from [https://github.com/oneapi-src/oneTBB](https://github.com/
-oneapi-src/oneTBB) and built from source. In this case one should supply the
-necessary environment variables pointing to the header and library files of the
-TBB package. For newer Intel compilers the TBB package is part of the Intel
-compiler package, similarly to the MKL package. If the TBB library is located
-at non-standrad path or the SQUANDER package is compiled with GNU compiler,
-then setting the $ export TBB_LIB_DIR=path/to/TBB/lib(64) $ export
+described in the next section. ### How to build the SQUANDER package on Unix/
+Linux/MacOS The SQUANDER package is equipped with a Python build script and
+CMake tools to ease the compilation and the deployment of the package. The
+SQUANDER package is parallelized via Threading Building Block (TBB) libraries.
+If TBB is not present in the system, it can be easily installed via python
+package [tbb-devel](https://pypi.org/project/tbb-devel/). Alternatively the TBB
+libraries can be installed via apt or yum utility (sudo apt install libtbb-dev)
+or it can be downloaded from [https://github.com/oneapi-src/oneTBB](https://
+github.com/oneapi-src/oneTBB) and built from source. In this case one should
+supply the necessary environment variables pointing to the header and library
+files of the TBB package. For newer Intel compilers the TBB package is part of
+the Intel compiler package, similarly to the MKL package. If the TBB library is
+located at non-standrad path or the SQUANDER package is compiled with GNU
+compiler, then setting the $ export TBB_LIB_DIR=path/to/TBB/lib(64) $ export
 TBB_INC_DIR=path/to/TBB/include environment variables are sufficient for
 successful compilation. When the TBB library is installed via a python package,
 setting the environment variables above is not necessary. The SQUANDER package
 with C++ Python extensions can be compiled via the Python script **setup.py**
 located in the root directory of the SQUANDER package. The script automatically
 finds out the CBLAS library working behind the numpy package and uses it in
 further linking. The **setup.py** script also build the C++ library of the
-SQUANDER package by making the appropriate CMake calls. ### Developer build We
-recommend to install the SQUANDER package in the Anaconda environment. In order
-to install the necessary requirements, follow the steps below: Creating new
-python environment: $ conda create -n qgd Activate the new anaconda environment
-$ conda activate qgd Install dependencies: $ conda install numpy scipy pip
-pytest scikit-build tbb-devel $ pip install qiskit matplotlib After the basic
+SQUANDER package by making the appropriate CMake calls. ### Build and Install
+on Microsoft Windows with Microsoft Visual C++ CMake must be in the path and
+able to find the MSVC compiler e.g. $ set PATH=%PATH%;C:\Program
+Files\cmake\bin Now set the TBB and BLAS folders and build via: $ set
+TBB_LOCATION=/LocalCache/local-packages $ set TBB_INC_DIR=%TBB_LOCATION%/
+Library/include $ set TBB_LIB_DIR=%TBB_LOCATION%/Library/lib $ set LIB=/lib;/
+lib $ python setup.py build_ext -DTBB_HEADER=\Library\include\ Installation
+merely requires copying DLL files (if they are not in the path): $ copy
+_skbuild\win-amd64-3.9\cmake-install\bin .\qgd_python\decomposition $ copy
+"%TBB_LOCATION%\Library\bin\tbb12.dll" .\qgd_python\decomposition $ copy
+"%TBB_LOCATION%\Library\bin\tbbmalloc.dll" .\qgd_python\decomposition Verify
+the installation: $ python -m pytest ### Developer build We recommend to
+install the SQUANDER package in the Anaconda environment. In order to install
+the necessary requirements, follow the steps below: Creating new python
+environment: $ conda create -n qgd Activate the new anaconda environment $
+conda activate qgd Install dependencies: $ conda install numpy scipy pip pytest
+scikit-build tbb-devel $ pip install qiskit matplotlib After the basic
 environment variables are set and the dependencies are installed, the
 compilation of the package can be started by the Python command: $ python3
 setup.py build_ext The command above starts the compilation of the SQUANDER C++
 library and builds the necessary C++ Python interface extensions of the
 SQUANDER package in place. After a successful build, one can register the
 SQUANDER package in the Python distribution in developer (i.e. editable) mode
 by command: $ python -m pip install -e . ### Binary distribution After the
```

### Comparing `squander-1.8.2/README.md` & `squander-1.8.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -62,22 +62,20 @@
 
 Since version 1.7.1 the SQUANDER package is accessible at Python Package Index (PyPI). The package can be installed on linux systems following the steps outlined below:
 
 $ pip install numpy swig tbb-devel wheel scikit-build ninja qiskit
 
 $ pip install squander
 
-
-
 ### Download the SQUANDER package
 
 The developer version of the Quantum Gate Decomposer package can be downloaded from github repository [https://github.com/rakytap/quantum-gate-decomposer/tree/master](https://github.com/rakytap/quantum-gate-decomposer/tree/master).
 After the package is downloaded into the directory **path/to/SQUANDER/package** (which would be the path to the source code of the SQUANDER package), one can proceed to the compilation steps described in the next section.
 
-### How to build the SQUANDER package
+### How to build the SQUANDER package on Unix/Linux/MacOS
 
 The SQUANDER package is equipped with a Python build script and CMake tools to ease the compilation and the deployment of the package.
 The SQUANDER package is parallelized via Threading Building Block (TBB) libraries. If TBB is not present in the system, it can be easily installed via python package [tbb-devel](https://pypi.org/project/tbb-devel/).
 Alternatively the TBB libraries can be installed via apt or yum utility (sudo apt install libtbb-dev) or it can be downloaded from [https://github.com/oneapi-src/oneTBB](https://github.com/oneapi-src/oneTBB)   and built from source. 
 In this case one should supply the necessary environment variables pointing to the header and library files of the TBB package. For newer
 Intel compilers the TBB package is part of the Intel compiler package, similarly to the MKL package. If the TBB library is located at non-standrad path or the SQUANDER package is compiled with GNU compiler, then setting the
 
@@ -87,15 +85,43 @@
 
 environment variables are sufficient for successful compilation. 
 When the TBB library is installed via a python package, setting the environment variables above is not necessary.
 The SQUANDER package with C++ Python extensions can be compiled via the Python script **setup.py** located in the root directory of the SQUANDER package.
 The script automatically finds out the CBLAS library working behind the numpy package and uses it in further linking. 
 The **setup.py** script also build the C++ library of the SQUANDER package by making the appropriate CMake calls. 
 
+### Build and Install on Microsoft Windows with Microsoft Visual C++
+
+CMake must be in the path and able to find the MSVC compiler e.g.
+
+$ set PATH=%PATH%;C:\Program Files\cmake\bin
+
+Now set the TBB and BLAS folders and build via:
+
+$ set TBB_LOCATION=<Python_Folder>/LocalCache/local-packages
+
+$ set TBB_INC_DIR=%TBB_LOCATION%/Library/include
+
+$ set TBB_LIB_DIR=%TBB_LOCATION%/Library/lib
+
+$ set LIB=<BLAS_Location>/lib;<LAPACK_Location>/lib
+
+$ python setup.py build_ext -DTBB_HEADER=<TBB_Location>\Library\include\
+
+Installation merely requires copying DLL files (if they are not in the path):
+
+$ copy _skbuild\win-amd64-3.9\cmake-install\bin .\qgd_python\decomposition
+
+$ copy "%TBB_LOCATION%\Library\bin\tbb12.dll" .\qgd_python\decomposition
+
+$ copy "%TBB_LOCATION%\Library\bin\tbbmalloc.dll" .\qgd_python\decomposition
+
+Verify the installation:
 
+$ python -m pytest
 
 ### Developer build
 
 
 We recommend to install the SQUANDER package in the Anaconda environment. In order to install the necessary requirements, follow the steps below:
 
 Creating new python environment:
```

#### html2text {}

```diff
@@ -55,41 +55,52 @@
 numpy swig tbb-devel wheel scikit-build ninja qiskit $ pip install squander ###
 Download the SQUANDER package The developer version of the Quantum Gate
 Decomposer package can be downloaded from github repository [https://
 github.com/rakytap/quantum-gate-decomposer/tree/master](https://github.com/
 rakytap/quantum-gate-decomposer/tree/master). After the package is downloaded
 into the directory **path/to/SQUANDER/package** (which would be the path to the
 source code of the SQUANDER package), one can proceed to the compilation steps
-described in the next section. ### How to build the SQUANDER package The
-SQUANDER package is equipped with a Python build script and CMake tools to ease
-the compilation and the deployment of the package. The SQUANDER package is
-parallelized via Threading Building Block (TBB) libraries. If TBB is not
-present in the system, it can be easily installed via python package [tbb-
-devel](https://pypi.org/project/tbb-devel/). Alternatively the TBB libraries
-can be installed via apt or yum utility (sudo apt install libtbb-dev) or it can
-be downloaded from [https://github.com/oneapi-src/oneTBB](https://github.com/
-oneapi-src/oneTBB) and built from source. In this case one should supply the
-necessary environment variables pointing to the header and library files of the
-TBB package. For newer Intel compilers the TBB package is part of the Intel
-compiler package, similarly to the MKL package. If the TBB library is located
-at non-standrad path or the SQUANDER package is compiled with GNU compiler,
-then setting the $ export TBB_LIB_DIR=path/to/TBB/lib(64) $ export
+described in the next section. ### How to build the SQUANDER package on Unix/
+Linux/MacOS The SQUANDER package is equipped with a Python build script and
+CMake tools to ease the compilation and the deployment of the package. The
+SQUANDER package is parallelized via Threading Building Block (TBB) libraries.
+If TBB is not present in the system, it can be easily installed via python
+package [tbb-devel](https://pypi.org/project/tbb-devel/). Alternatively the TBB
+libraries can be installed via apt or yum utility (sudo apt install libtbb-dev)
+or it can be downloaded from [https://github.com/oneapi-src/oneTBB](https://
+github.com/oneapi-src/oneTBB) and built from source. In this case one should
+supply the necessary environment variables pointing to the header and library
+files of the TBB package. For newer Intel compilers the TBB package is part of
+the Intel compiler package, similarly to the MKL package. If the TBB library is
+located at non-standrad path or the SQUANDER package is compiled with GNU
+compiler, then setting the $ export TBB_LIB_DIR=path/to/TBB/lib(64) $ export
 TBB_INC_DIR=path/to/TBB/include environment variables are sufficient for
 successful compilation. When the TBB library is installed via a python package,
 setting the environment variables above is not necessary. The SQUANDER package
 with C++ Python extensions can be compiled via the Python script **setup.py**
 located in the root directory of the SQUANDER package. The script automatically
 finds out the CBLAS library working behind the numpy package and uses it in
 further linking. The **setup.py** script also build the C++ library of the
-SQUANDER package by making the appropriate CMake calls. ### Developer build We
-recommend to install the SQUANDER package in the Anaconda environment. In order
-to install the necessary requirements, follow the steps below: Creating new
-python environment: $ conda create -n qgd Activate the new anaconda environment
-$ conda activate qgd Install dependencies: $ conda install numpy scipy pip
-pytest scikit-build tbb-devel $ pip install qiskit matplotlib After the basic
+SQUANDER package by making the appropriate CMake calls. ### Build and Install
+on Microsoft Windows with Microsoft Visual C++ CMake must be in the path and
+able to find the MSVC compiler e.g. $ set PATH=%PATH%;C:\Program
+Files\cmake\bin Now set the TBB and BLAS folders and build via: $ set
+TBB_LOCATION=/LocalCache/local-packages $ set TBB_INC_DIR=%TBB_LOCATION%/
+Library/include $ set TBB_LIB_DIR=%TBB_LOCATION%/Library/lib $ set LIB=/lib;/
+lib $ python setup.py build_ext -DTBB_HEADER=\Library\include\ Installation
+merely requires copying DLL files (if they are not in the path): $ copy
+_skbuild\win-amd64-3.9\cmake-install\bin .\qgd_python\decomposition $ copy
+"%TBB_LOCATION%\Library\bin\tbb12.dll" .\qgd_python\decomposition $ copy
+"%TBB_LOCATION%\Library\bin\tbbmalloc.dll" .\qgd_python\decomposition Verify
+the installation: $ python -m pytest ### Developer build We recommend to
+install the SQUANDER package in the Anaconda environment. In order to install
+the necessary requirements, follow the steps below: Creating new python
+environment: $ conda create -n qgd Activate the new anaconda environment $
+conda activate qgd Install dependencies: $ conda install numpy scipy pip pytest
+scikit-build tbb-devel $ pip install qiskit matplotlib After the basic
 environment variables are set and the dependencies are installed, the
 compilation of the package can be started by the Python command: $ python3
 setup.py build_ext The command above starts the compilation of the SQUANDER C++
 library and builds the necessary C++ Python interface extensions of the
 SQUANDER package in place. After a successful build, one can register the
 SQUANDER package in the Python distribution in developer (i.e. editable) mode
 by command: $ python -m pip install -e . ### Binary distribution After the
```

### Comparing `squander-1.8.2/cmake/check_AVX.cmake` & `squander-1.8.3/cmake/check_AVX.cmake`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/common/Adam.cpp` & `squander-1.8.3/common/Adam.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/common/common.cpp` & `squander-1.8.3/common/common.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/common/common_DFE.cpp` & `squander-1.8.3/common/common_DFE.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/common/config_element.cpp` & `squander-1.8.3/common/config_element.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/common/dot.cpp` & `squander-1.8.3/common/dot.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/common/include/Adam.h` & `squander-1.8.3/common/include/Adam.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/common/include/QGDTypes.h` & `squander-1.8.3/common/include/QGDTypes.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/common/include/common.h` & `squander-1.8.3/common/include/common.h`

 * *Files 2% similar despite different names*

```diff
@@ -20,24 +20,27 @@
 /*! \file common.h
     \brief Header file for commonly used functions and wrappers to CBLAS functions.
 */
 
 #ifndef common_H
 #define common_H
 
+#define _USE_MATH_DEFINES
+#include <cmath>
+#define NOMINMAX
+#include <algorithm>
 
 #include <omp.h>
 #include "QGDTypes.h"
 #include "dot.h"
 
 
 #include <string>
 #include <stdio.h>
 #include <iostream>
-#include <cmath>
 #include <vector>
 #include <cstring>
 #include <sstream>
 
 #ifdef __cplusplus
 extern "C"
 {
```

### Comparing `squander-1.8.2/common/include/common_DFE.h` & `squander-1.8.3/common/include/common_DFE.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/common/include/config_element.h` & `squander-1.8.3/common/include/config_element.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/common/include/dot.h` & `squander-1.8.3/common/include/dot.h`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 #endif
 
 #ifdef __cplusplus
 extern "C"
 {
 #endif
 
-#include "gsl/gsl_blas_types.h"
+typedef enum CBLAS_ORDER     {CblasRowMajor=101, CblasColMajor=102} CBLAS_ORDER;
+typedef enum CBLAS_TRANSPOSE {CblasNoTrans=111, CblasTrans=112, CblasConjTrans=113, CblasConjNoTrans=114} CBLAS_TRANSPOSE;
 
 /// Definition of the zgemm function from CBLAS
 void cblas_zgemm(const enum CBLAS_ORDER Order, const enum CBLAS_TRANSPOSE TransA, const enum CBLAS_TRANSPOSE TransB, const int M, const int N, const int K,
 		 const void *alpha, const void *A, const int lda, const void *B, const int ldb, const void *beta, void *C, const int ldc);
 
 /// Definition of the zgemv function from CBLAS to calculate matrix-vector product
 void cblas_zgemv(const enum CBLAS_ORDER Order, const enum CBLAS_TRANSPOSE TransA, const int M, const int N, const void *alpha, const void *A, const int lda,
```

### Comparing `squander-1.8.2/common/include/lbfgs.h` & `squander-1.8.3/common/include/lbfgs.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/common/include/logging.h` & `squander-1.8.3/common/include/logging.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/common/include/matrix.h` & `squander-1.8.3/common/include/matrix.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/common/include/matrix_base.h` & `squander-1.8.3/common/include/matrix_base.h`

 * *Files 2% similar despite different names*

```diff
@@ -416,15 +416,15 @@
 }
 
 
 /**
 @brief Call to create a copy of the matrix
 @return Returns with the instance of the class.
 */
-matrix_base<scalar> copy() {
+matrix_base<scalar> copy() const {
 
   matrix_base<scalar> ret = matrix_base<scalar>(rows, cols, stride);
 
   // logical variable indicating whether the matrix needs to be conjugated in CBLAS operations
   ret.conjugated = conjugated;
   // logical variable indicating whether the matrix needs to be transposed in CBLAS operations
   ret.transposed = transposed;
@@ -433,14 +433,21 @@
 
   memcpy( ret.data, data, rows*stride*sizeof(scalar));
 
   return ret;
 
 }
 
+void ensure_aligned() {
+    if (((uintptr_t)(void*)data & (CACHELINE-1)) == 0) return; //CACHELINE must be power of 2, 16 sufficient, 64 is okay though
+    scalar* newdata = (scalar*)scalable_aligned_malloc( rows*stride*sizeof(scalar), CACHELINE);
+    memcpy( newdata, data, rows*stride*sizeof(scalar));
+    replace_data(newdata, true);
+}
+
 
 
 /**
 @brief Call to get the number of the allocated elements
 @return Returns with the number of the allocated elements (rows*cols)
 */
 int size() const {
```

### Comparing `squander-1.8.2/common/include/matrix_real.h` & `squander-1.8.3/common/include/matrix_real.h`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 Matrix_real(const Matrix_real &in);
 
 
 /**
 @brief Call to create a copy of the matrix
 @return Returns with the instance of the class.
 */
-Matrix_real copy();
+Matrix_real copy() const;
 
 
 /**
 @brief Call to check the array for NaN entries.
 @return Returns with true if the array has at least one NaN entry.
 */
 bool isnan();
```

### Comparing `squander-1.8.2/common/include/mpi_base.h` & `squander-1.8.3/common/include/mpi_base.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/common/include/numpy_interface.h` & `squander-1.8.3/common/include/numpy_interface.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/common/include/tolmin.h` & `squander-1.8.3/common/include/tolmin.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 /*
 This code is credited to the OPTIMUS project of Ioannis G. Tsoulos
 */
 
 # ifndef __TOLMIN__H
 # define __TOLMIN__H
-using namespace std;
 
 #include "matrix_real.h"
 typedef Matrix_real Data;
 
 #ifndef PROBLEM_H
 #define PROBLEM_H
 #define integer long
@@ -20,25 +19,25 @@
  */
 class Problem
 {
 private:
     int dimension;
     double lmargin, rmargin;
     double (* f) (Data x, void * params);
-    void (* df) (Data x, void * params, Data g);
-    void (* fdf) (Data x, void * params, double * f, Data g);
+    void (* df) (Data x, void * params, Data& g);
+    void (* fdf) (Data x, void * params, double * f, Data& g);
     void* void_instance;
 
 public:
     /** @brief Problem the constructor of the class.
      * 	@param p is the objective problem to be minimized
      * **/
     Problem(int dimension, double lmargin, double rmargin, double (* f) (Data, void *),
-        void (* df) (Data, void *, Data),
-        void (* fdf) (Data, void *, double *, Data),
+        void (* df) (Data, void *, Data&),
+        void (* fdf) (Data, void *, double *, Data&),
         void* void_instance)
     {
         this->dimension = dimension;
         this->lmargin = lmargin;
         this->rmargin = rmargin;
         this->f = f;
         this->df = df;
```

### Comparing `squander-1.8.2/common/lbfgs.cpp` & `squander-1.8.3/common/lbfgs.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/common/logging.cpp` & `squander-1.8.3/common/logging.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/common/matrix.cpp` & `squander-1.8.3/common/matrix.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/common/matrix_real.cpp` & `squander-1.8.3/common/matrix_real.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
 
 /**
 @brief Call to create a copy of the matrix
 @return Returns with the instance of the class.
 */
 Matrix_real
-Matrix_real::copy() {
+Matrix_real::copy() const {
 
   Matrix_real ret = Matrix_real(rows, cols, stride);
 
   // logical variable indicating whether the matrix needs to be conjugated in CBLAS operations
   ret.conjugated = conjugated;
   // logical variable indicating whether the matrix needs to be transposed in CBLAS operations
   ret.transposed = transposed;
```

### Comparing `squander-1.8.2/common/mpi_base.cpp` & `squander-1.8.3/common/mpi_base.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/common/numpy_interface.cpp` & `squander-1.8.3/common/numpy_interface.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/common/tolmin.cpp` & `squander-1.8.3/common/tolmin.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -400,19 +400,19 @@
 	    if (ratio < (float)0. || temp < ratio) {
 		ratio = temp;
 	    }
 	}
 /* L10: */
     }
     amx = (float)1.;
-    *step = min(amx,*stepcb);
+    *step = std::min(amx,*stepcb);
 /* Computing MAX */
     d__1 = *relacc * ratio, d__2 = *step * (float)1e-19;
-    stpmin = max(d__1,d__2);
-    *step = max(stpmin,*step);
+    stpmin = std::max(d__1,d__2);
+    *step = std::max(stpmin,*step);
     sbase = (float)0.;
     fbase = *f;
     ddotgb = *ddotg;
     stplow = (float)0.;
     flow = *f;
     dglow = *ddotg;
     stphgh = (float)0.;
@@ -485,24 +485,24 @@
 	}
 	temp = (float)10.;
 	if (dgmid > *ddotg * (float).9) {
 	    temp = *ddotg / (*ddotg - dgmid);
 	}
 /* Computing MIN */
 	d__1 = temp * *step;
-	*step = min(d__1,*stepcb);
+	*step = std::min(d__1,*stepcb);
 	goto L20;
     } else if (icount == 1 || stplow > (float)0.) {
 	dgknot = (fhgh - flow) * (float)2. / (stphgh - stplow) - (dglow + 
 		dghgh) * (float).5;
 	if (dgknot >= (float)0.) {
 	    amx = (float).1;
 /* Computing MAX */
 	    d__1 = amx, d__2 = dglow * (float).5 / (dglow - dgknot);
-	    ratio = max(d__1,d__2);
+	    ratio = std::max(d__1,d__2);
 	} else {
 	    ratio = (dghgh * (float).5 - dgknot) / (dghgh - dgknot);
 	}
 	*step = stplow + ratio * (stphgh - stplow);
 	goto L20;
     } else {
 	*step *= (float).1;
@@ -587,15 +587,15 @@
     }
 
 /*     Check the bounds on N, M and MEQ. */
 
     *info = 4;
 /* Computing MAX */
     i__1 = 1 - *n, i__2 = *meq * (*meq - *m);
-    if (max(i__1,i__2) > 0) {
+    if (std::max(i__1,i__2) > 0) {
 	if (*iprint != 0) {
 	    //io___56.ciunit = units_1.iuout;
 	    //s_wsfe(&io___56);
 	    //e_wsfe();
 	}
 	goto L40;
     }
@@ -603,15 +603,15 @@
 /*     Initialize RELACC, Z, U and TOL. */
 
     initzu_(n, m, &xl[1], &xu[1], &x[1], &iact[1], &meql, info, &z__[1], &u[1]
 	    , &xbig[1], &relacc);
     amx = (float).01;
 /* Computing MAX */
     d__1 = amx, d__2 = relacc * (float)10.;
-    tol = max(d__1,d__2);
+    tol = std::max(d__1,d__2);
     if (*info == 4) {
 	if (*iprint != 0) {
 	    //io___61.ciunit = units_1.iuout;
 	    //s_wsfe(&io___61);
 	    //e_wsfe();
 	}
 	goto L40;
@@ -848,15 +848,15 @@
 	goto L70;
     }
 
 /*     Test whether to reduce TOL and to provide printing. */
 
 /* Computing MAX */
     d__1 = diff, d__2 = ddotg * (float)-.5;
-    if (*tol > *relacc && *iterc > iterk && relaxf * (float).1 >= max(d__1,
+    if (*tol > *relacc && *iterc > iterk && relaxf * (float).1 >= std::max(d__1,
 	    d__2)) {
 	goto L70;
     }
     if (iterp == *iterc) {
     iterp = *iterc + abs(*iprint);
 	goto L80;
     }
@@ -884,15 +884,15 @@
 /*     Revise XBIG. */
 
     i__1 = *n;
     for (i__ = 1; i__ <= i__1; ++i__) {
 /* L60: */
 /* Computing MAX */
 	d__2 = xbig[i__], d__3 = (d__1 = x[i__], fabs(d__1));
-	xbig[i__] = max(d__2,d__3);
+	xbig[i__] = std::max(d__2,d__3);
     }
 
 /*     Revise the second derivative approximation. */
 
     zbfgs_(n, &x[1], nact, &g[1], &z__[1], &ztg[1], &xs[1], &gs[1], zznorm);
 
 /*     Add a constraint to the active set if it restricts the step. */
@@ -1095,16 +1095,16 @@
     i__1 = *n;
     for (i__ = 1; i__ <= i__1; ++i__) {
 	temp = d__[i__] * gmnew[i__];
 	sum += temp;
 /* L110: */
 	sumabs += fabs(temp);
     }
-    savsum = min(savsum,sum);
-    savabs = max(savabs,sumabs);
+    savsum = std::min(savsum,sum);
+    savabs = std::max(savabs,sumabs);
     --k;
     if (k >= 1) {
 	goto L80;
     }
 
 /*     Add the new constraint to the active set if the constraint */
 /*       violation is still significant. */
@@ -1227,15 +1227,15 @@
 		i__2 = *n;
 		for (i__ = 1; i__ <= i__2; ++i__) {
 		    x[i__] += scale * z__[iz];
 		    iz += *n;
 /* L20: */
 /* Computing MAX */
 		    d__2 = xbig[i__], d__3 = (d__1 = x[i__], fabs(d__1));
-		    xbig[i__] = max(d__2,d__3);
+		    xbig[i__] = std::max(d__2,d__3);
 		}
 		if (j > *m) {
 		    x[jx] = savex;
 		}
 
 /*     Else flag a constraint deletion if necessary. */
 
@@ -1368,15 +1368,15 @@
     }
     temp *= u[k];
     parnew[k] = par[k] + temp;
     amx = (float)0.;
     if (k == *nact) {
 /* Computing MIN */
 	d__1 = parnew[k];
-	parnew[k] = min(d__1,amx);
+	parnew[k] = std::min(d__1,amx);
     }
     j = iact[k];
     if (j <= *m) {
 	i__1 = *n;
 	for (i__ = 1; i__ <= i__1; ++i__) {
 /* L70: */
 	    gmnew[i__] -= temp * a[i__ + j * a_dim1];
@@ -1414,15 +1414,15 @@
     theta = (float)1. - ratio;
     amx = (float)0.;
     i__1 = *nact;
     for (k = mp; k <= i__1; ++k) {
 /* L90: */
 /* Computing MIN */
 	d__1 = theta * parnew[k] + ratio * par[k];
-	par[k] = min(d__1,amx);
+	par[k] = std::min(d__1,amx);
     }
     i__1 = *n;
     for (i__ = 1; i__ <= i__1; ++i__) {
 /* L100: */
 	gm[i__] = theta * gmnew[i__] + ratio * gm[i__];
     }
 
@@ -1734,18 +1734,18 @@
 
 /*     Update the value of ZZNORM. */
 
     if (*zznorm < (float)0.) {
 	*zznorm = dd / dg;
     } else {
 	temp = sqrt(*zznorm * dd / dg);
-	*zznorm = min(*zznorm,temp);
+	*zznorm = std::min(*zznorm,temp);
 /* Computing MAX */
 	d__1 = *zznorm, d__2 = temp * (float).1;
-	*zznorm = max(d__1,d__2);
+	*zznorm = std::max(d__1,d__2);
     }
 
 /*     Complete the updating of Z. */
 
     np = *nact + 1;
     temp = sqrt(dg);
     iz = np;
@@ -1937,15 +1937,15 @@
     if (stepcb > (float)0.) {
 	i__1 = *n;
 	for (i__ = 1; i__ <= i__1; ++i__) {
 	    x[i__] += stepcb * d__[i__];
 /* L40: */
 /* Computing MAX */
 	    d__2 = xbig[i__], d__3 = (d__1 = x[i__], fabs(d__1));
-	    xbig[i__] = max(d__2,d__3);
+	    xbig[i__] = std::max(d__2,d__3);
 	}
 	addcon_(n, m, &a[a_offset], ia, &iact[1], nact, &z__[1], &u[1], 
 		relacc, &indxbd, &gmnew[1], &cgrad[1]);
     }
 
 /*     Test whether to continue the search for feasibility. */
 
@@ -2219,23 +2219,23 @@
 		    res = xu[jm] - x[jm];
 		    resabs = xbig[jm] + (d__1 = xu[jm], fabs(d__1));
 		}
 	    }
 	    if (res > (float)0.) {
 /* Computing MAX */
 		d__1 = viol, d__2 = res / resabs;
-		viol = max(d__1,d__2);
+		viol = std::max(d__1,d__2);
 	    }
 /* L20: */
 	}
     }
 
 /*     Adjust TOL. */
 
-    *tol = min(*tol,viol) * (float).1;
+    *tol = std::min(*tol,viol) * (float).1;
     if (*tol <= *relacc + *relacc) {
 	*tol = *relacc;
 	i__1 = *n;
 	for (i__ = 1; i__ <= i__1; ++i__) {
 /* L30: */
 	    xbig[i__] = (d__1 = x[i__], fabs(d__1));
 	}
```

### Comparing `squander-1.8.2/decomposition/Decomposition_Base.cpp` & `squander-1.8.3/decomposition/Decomposition_Base.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -19,16 +19,14 @@
 */
 /*! \file Decomposition_Base.cpp
     \brief Class containing basic methods for the decomposition process.
 */
 
 #include "Decomposition_Base.h"
 
-
-
 // default layer numbers
 std::map<int,int> Decomposition_Base::max_layer_num_def;
 
 
 /** Nullary constructor of the class
 @return An instance of the class
 */
@@ -388,15 +386,15 @@
 	
 
         if ( gates.size() == 0 ) {
             return;
         }
 
         // array containing minimums to check convergence of the solution
-        int min_vec_num = 20;
+        const int min_vec_num = 20;
         double minimum_vec[min_vec_num];
         for ( int idx=0; idx<min_vec_num; idx++) {
             minimum_vec[idx] = 0;
         }
 
         // setting the initial value for the current minimum
         current_minimum = 1e8;
```

### Comparing `squander-1.8.2/decomposition/N_Qubit_Decomposition.cpp` & `squander-1.8.3/decomposition/N_Qubit_Decomposition.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/decomposition/N_Qubit_Decomposition_Base.cpp` & `squander-1.8.3/decomposition/N_Qubit_Decomposition_Base.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -443,14 +443,23 @@
         long long max_inner_iterations_loc;
         if ( config.count("max_inner_iterations") > 0 ) {
              config["max_inner_iterations"].get_property( max_inner_iterations_loc );  
         }
         else {
             max_inner_iterations_loc = max_inner_iterations;
         }
+        
+        
+        long long export_circuit_2_binary_loc;
+        if ( config.count("export_circuit_2_binary") > 0 ) {
+             config["export_circuit_2_binary"].get_property( export_circuit_2_binary_loc );  
+        }
+        else {
+            export_circuit_2_binary_loc = 0;
+        }        
 
 
         double optimization_tolerance_loc;
         if ( config.count("optimization_tolerance") > 0 ) {
              config["optimization_tolerance"].get_property( optimization_tolerance_loc );  
         }
         else {
@@ -662,16 +671,21 @@
             // update the current cost function
             //current_minimum = optimization_problem( solution_guess_tmp_mtx );
 
             if ( iter_idx % 1000 == 0 ) {
                 std::stringstream sstream;
                 sstream << "COSINE: processed iterations " << (double)iter_idx/max_inner_iterations_loc*100 << "\%, current minimum:" << current_minimum << std::endl;
                 print(sstream, 0);   
-                std::string filename("initial_circuit_iteration.binary");
-                export_gate_list_to_binary(solution_guess_tmp_mtx, this, filename, verbose);
+                if ( export_circuit_2_binary_loc > 0 ) {
+                    std::string filename("initial_circuit_iteration.binary");
+                    if (project_name != "") { 
+                        filename=project_name+ "_"  +filename;
+                    }
+                    export_gate_list_to_binary(solution_guess_tmp_mtx, this, filename, verbose);
+                }
 
 
             }
 
             if (current_minimum < optimization_tolerance_loc ) {
                 break;
             }
@@ -690,16 +704,21 @@
 
 
      
             if ( std::abs( f0_mean - current_minimum) < 1e-7  && var_f0/f0_mean < 1e-7 ) {
                 std::stringstream sstream;
                 sstream << "COSINE: converged to minimum at iterations " << (double)iter_idx/max_inner_iterations_loc*100 << "\%, current minimum:" << current_minimum << std::endl;
                 print(sstream, 0);   
-                std::string filename("initial_circuit_iteration.binary");
-                export_gate_list_to_binary(solution_guess_tmp_mtx, this, filename, verbose);
+                if ( export_circuit_2_binary_loc > 0 ) {
+                    std::string filename("initial_circuit_iteration.binary");
+                    if (project_name != "") { 
+                        filename=project_name+ "_"  +filename;
+                    }
+                    export_gate_list_to_binary(solution_guess_tmp_mtx, this, filename, verbose);
+                }
                 
 
                 break;
             }
 
         }
         
@@ -798,14 +817,22 @@
         if ( config.count("optimization_tolerance_agent") > 0 ) {
              double value;
              config["optimization_tolerance_agent"].get_property( optimization_tolerance_loc );
         }
         else {
             optimization_tolerance_loc = optimization_tolerance;
         }
+        
+        long long export_circuit_2_binary_loc;
+        if ( config.count("export_circuit_2_binary") > 0 ) {
+             config["export_circuit_2_binary"].get_property( export_circuit_2_binary_loc );  
+        }
+        else {
+            export_circuit_2_binary_loc = 0;
+        }            
 
         
         int agent_lifetime_loc;
         if ( config.count("agent_lifetime") > 0 ) {
              long long agent_lifetime_loc_tmp;
              config["agent_lifetime"].get_property( agent_lifetime_loc_tmp );  
              agent_lifetime_loc = (int)agent_lifetime_loc_tmp;
@@ -1115,19 +1142,21 @@
                     if ( current_minimum_agent <= current_minimum ) {
 
                         most_successfull_agent = agent_idx;
                     
                         // export the parameters of the curremt, most successful agent
                         memcpy(optimized_parameters_mtx.get_data(), solution_guess_mtx_agent.get_data(), num_of_parameters*sizeof(double) );
 
-                        std::string filename("initial_circuit_iteration.binary");
-                        if (project_name != "") { 
-                            filename=project_name+ "_"  +filename;
+                        if ( export_circuit_2_binary_loc > 0 ) {
+                            std::string filename("initial_circuit_iteration.binary");
+                            if (project_name != "") { 
+                                filename=project_name+ "_"  +filename;
+                            }
+                            export_gate_list_to_binary(optimized_parameters_mtx, this, filename, verbose);
                         }
-                        export_gate_list_to_binary(optimized_parameters_mtx, this, filename, verbose);
 
                         
                         current_minimum = current_minimum_agent;      
                         
                                    
                         
                     }
@@ -1163,14 +1192,15 @@
                                 // keep the current state  of the agent                    
                             }
 
 #ifdef __MPI__        
                         }
                         
                         MPI_Bcast( (void*)solution_guess_mtx_agent.get_data(), num_of_parameters, MPI_DOUBLE, 0, MPI_COMM_WORLD);
+                        MPI_Bcast( (void*)current_minimum_agents.get_data(), agent_num, MPI_DOUBLE, 0, MPI_COMM_WORLD);
 #endif     
                                                                                   
                     }
                  
 
                     // test global convergence 
                     if ( agent_idx == 0 ) {
@@ -1318,14 +1348,23 @@
         long long max_inner_iterations_loc;
         if ( config.count("max_inner_iterations_agent") > 0 ) {
              config["max_inner_iterations_agent"].get_property( max_inner_iterations_loc );  
         }
         else {
             max_inner_iterations_loc = max_inner_iterations;
         }
+        
+        
+        long long export_circuit_2_binary_loc;
+        if ( config.count("export_circuit_2_binary") > 0 ) {
+             config["export_circuit_2_binary"].get_property( export_circuit_2_binary_loc );  
+        }
+        else {
+            export_circuit_2_binary_loc = 0;
+        }            
 
         double f0 = DBL_MAX;
         std::stringstream sstream;
         sstream << "iter_max: " << max_inner_iterations_loc << ", randomization threshold: " << iteration_threshold_of_randomization << ", randomization radius: " << radius << std::endl;
         print(sstream, 2); 
 
         int ADAM_status = 0;
@@ -1397,16 +1436,22 @@
 
                     Matrix matrix_new = get_transformed_matrix( optimized_parameters_mtx, gates.begin(), gates.size(), Umtx );
 
                     std::stringstream sstream;
                     sstream << "ADAM: processed iterations " << (double)iter_idx/max_inner_iterations_loc*100;
                     sstream << "\%, current minimum:" << current_minimum << ", pure cost function:" << get_cost_function(matrix_new, trace_offset) << std::endl;
                     print(sstream, 0);   
-                    std::string filename("initial_circuit_iteration.binary");
-                    export_gate_list_to_binary(optimized_parameters_mtx, this, filename, verbose);
+                    
+                    if ( export_circuit_2_binary_loc > 0 ) {
+                        std::string filename("initial_circuit_iteration.binary");
+                        if (project_name != "") { 
+                            filename=project_name+ "_"  +filename;
+                        }
+                        export_gate_list_to_binary(optimized_parameters_mtx, this, filename, verbose);
+                    }
 
                 }
 
 //std::cout << grad_norm  << std::endl;
                 if (f0 < optimization_tolerance || random_shift_count > random_shift_count_max ) {
                     break;
                 }
@@ -1549,14 +1594,22 @@
         if ( config.count("randomization_threshold") > 0 ) {
             config["randomization_threshold"].get_property( iteration_threshold_of_randomization_loc );  
         }
         else {
             iteration_threshold_of_randomization_loc = iteration_threshold_of_randomization;
         }
         
+        long long export_circuit_2_binary_loc;
+        if ( config.count("export_circuit_2_binary") > 0 ) {
+             config["export_circuit_2_binary"].get_property( export_circuit_2_binary_loc );  
+        }
+        else {
+            export_circuit_2_binary_loc = 0;
+        }            
+        
         
         double optimization_tolerance_loc;
         if ( config.count("optimization_tolerance") > 0 ) {
              config["optimization_tolerance"].get_property( optimization_tolerance_loc );  
         }
         else {
             optimization_tolerance_loc = optimization_tolerance;
@@ -1613,16 +1666,22 @@
             if ( iter_idx % 5000 == 0 ) {
 
                 Matrix matrix_new = get_transformed_matrix( solution_guess_tmp, gates.begin(), gates.size(), Umtx );
 
                 std::stringstream sstream;
                 sstream << "ADAM: processed iterations " << (double)iter_idx/max_inner_iterations_loc*100 << "\%, current minimum:" << current_minimum << ", current cost function:" << get_cost_function(matrix_new, trace_offset) << ", sub_iter_idx:" << sub_iter_idx <<std::endl;
                 print(sstream, 0);   
-                std::string filename("initial_circuit_iteration.binary");
-                export_gate_list_to_binary(optimized_parameters_mtx, this, filename, verbose);
+                
+                if ( export_circuit_2_binary_loc > 0 ) {
+                    std::string filename("initial_circuit_iteration.binary");
+                    if (project_name != "") { 
+                        filename=project_name+ "_"  +filename;
+                    }
+                    export_gate_list_to_binary(optimized_parameters_mtx, this, filename, verbose);
+                }
             }
 
 //std::cout << grad_norm  << std::endl;
             if (f0 < optimization_tolerance_loc || random_shift_count > random_shift_count_max ) {
                 break;
             }
 
@@ -1865,14 +1924,23 @@
             config["max_inner_iterations"].get_property( max_inner_iterations_loc );  
         }
         else {
             max_inner_iterations_loc =max_inner_iterations;
         }
 
 
+        long long export_circuit_2_binary_loc;
+        if ( config.count("export_circuit_2_binary") > 0 ) {
+             config["export_circuit_2_binary"].get_property( export_circuit_2_binary_loc );  
+        }
+        else {
+            export_circuit_2_binary_loc = 0;
+        }    
+        
+
         long long iteration_threshold_of_randomization_loc;
         if ( config.count("randomization_threshold") > 0 ) {
             config["randomization_threshold"].get_property( iteration_threshold_of_randomization_loc );  
         }
         else {
             iteration_threshold_of_randomization_loc = iteration_threshold_of_randomization;
         }
@@ -1909,16 +1977,21 @@
     
 
                 if ( iter_idx % 5000 == 0 ) {
                      std::stringstream sstream;
                      sstream << "BFGS2: processed iterations " << (double)iter_idx/max_inner_iterations_loc*100 << "\%, current minimum:" << current_minimum << std::endl;
                      print(sstream, 2);  
 
-                     std::string filename("initial_circuit_iteration.binary");
-                     export_gate_list_to_binary(optimized_parameters_mtx, this, filename, verbose);
+                     if ( export_circuit_2_binary_loc>0) {
+                         std::string filename("initial_circuit_iteration.binary");
+                         if (project_name != "") { 
+                             filename=project_name+ "_"  +filename;
+                         }
+                         export_gate_list_to_binary(optimized_parameters_mtx, this, filename, verbose);
+                     }
                 }
 
 
                 if (f < optimization_tolerance || random_shift_count > random_shift_count_max ) {
                     break;
                 }
 
@@ -2285,15 +2358,15 @@
 /**
 @brief Call to calculate both the cost function and the its gradient components.
 @param parameters Array containing the free parameters to be optimized.
 @param void_instance A void pointer pointing to the instance of the current class.
 @param f0 The value of the cost function at x0.
 @param grad Array containing the calculated gradient components.
 */
-void N_Qubit_Decomposition_Base::optimization_problem_combined( Matrix_real parameters, void* void_instance, double* f0, Matrix_real grad ) {
+void N_Qubit_Decomposition_Base::optimization_problem_combined( Matrix_real parameters, void* void_instance, double* f0, Matrix_real& grad ) {
 
     N_Qubit_Decomposition_Base* instance = reinterpret_cast<N_Qubit_Decomposition_Base*>(void_instance);
 
     // the number of free parameters
     int parameter_num_loc = instance->get_parameter_num();
 
     // the variant of the cost function
```

### Comparing `squander-1.8.2/decomposition/N_Qubit_Decomposition_Cost_Function.cpp` & `squander-1.8.3/decomposition/N_Qubit_Decomposition_Cost_Function.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/decomposition/N_Qubit_Decomposition_adaptive.cpp` & `squander-1.8.3/decomposition/N_Qubit_Decomposition_adaptive.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -189,259 +189,35 @@
     std::stringstream sstream;
     sstream << "***************************************************************" << std::endl;
     sstream << "Starting to disentangle " << qbit_num << "-qubit matrix" << std::endl;
     sstream << "***************************************************************" << std::endl << std::endl << std::endl;
 
     print(sstream, 1);   
 
-
-    // temporarily turn off OpenMP parallelism
-#if BLAS==0 // undefined BLAS
-    num_threads = omp_get_max_threads();
-    omp_set_num_threads(1);
-#elif BLAS==1 // MKL
-    num_threads = mkl_get_max_threads();
-    MKL_Set_Num_Threads(1);
-#elif BLAS==2 //OpenBLAS
-    num_threads = openblas_get_num_threads();
-    openblas_set_num_threads(1);
-#endif
-
-    //measure the time for the decompositin
-    tbb::tick_count start_time = tbb::tick_count::now();
-
-    if (level_limit == 0 ) {
-        std::stringstream sstream;
-	sstream << "please increase level limit" << std::endl;
-        print(sstream, 0);	
-        return;
-    }
-
-
-
-    double optimization_tolerance_orig = optimization_tolerance;
-
-
-    Gates_block* gate_structure_loc = NULL;
-    if ( gates.size() > 0 ) {
-        std::stringstream sstream;
-        sstream << "Using imported gate structure for the decomposition." << std::endl;
-        print(sstream, 1);	
-	        
-        gate_structure_loc = optimize_imported_gate_structure(optimized_parameters_mtx);
-    }
-    else {
-        std::stringstream sstream;
-        sstream << "Construct initial gate structure for the decomposition." << std::endl;
-        print(sstream, 1);
-        gate_structure_loc = determine_initial_gate_structure(optimized_parameters_mtx);
-    }
-
-
-    std::string filename("circuit_squander.binary");
-    if (project_name != "") {
-        filename = project_name+ "_" +filename;
-    }
-
-    export_gate_list_to_binary(optimized_parameters_mtx, gate_structure_loc, filename, verbose);
-
-    sstream.str("");
-    sstream << std::endl;
-    sstream << std::endl;
-    sstream << "**************************************************************" << std::endl;
-    sstream << "***************** Compressing Gate structure *****************" << std::endl;
-    sstream << "**************************************************************" << std::endl;
-    print(sstream, 1);	    	
+    // get the initial circuit including redundand 2-qbit blocks.
+    get_initial_circuit();
     
+    // comppress the gate structure
+    compress_circuit();
 
-    int iter = 0;
-    int uncompressed_iter_num = 0;
-    while ( iter<25 || uncompressed_iter_num <= 5 ) {
-
-        sstream.str("");
-        sstream << "iteration " << iter+1 << ": ";
-        print(sstream, 1);	
-
-       
-        Gates_block* gate_structure_compressed = compress_gate_structure( gate_structure_loc );
-
-        if ( gate_structure_compressed->get_gate_num() < gate_structure_loc->get_gate_num() ) {
-            uncompressed_iter_num = 0;
-        }
-        else {
-            uncompressed_iter_num++;
-        }
-
-        if ( gate_structure_compressed != gate_structure_loc ) {
-            delete( gate_structure_loc );
-            gate_structure_loc = gate_structure_compressed;
-            gate_structure_compressed = NULL;
-            
-
-            std::string filename("circuit_compression.binary");
-            if (project_name != "") { 
-                filename=project_name+ "_"  +filename;
-            }
-
-            export_gate_list_to_binary(optimized_parameters_mtx, gate_structure_loc, filename, verbose);    
-            std::string filename_unitary("unitary_compression_unitary");
-            export_unitary(filename_unitary);
-        }
-
-        iter++;
-
-        if (uncompressed_iter_num>10) break;
-
-    }
-    
-
-    sstream.str("");
-    sstream << "**************************************************************" << std::endl;
-    sstream << "************ Final tuning of the Gate structure **************" << std::endl;
-    sstream << "**************************************************************" << std::endl;
-    print(sstream, 1);	    	
-    
-
-    optimization_tolerance = optimization_tolerance_orig;
-
-    // store the decomposing gate structure   
-    release_gates();
-    combine( gate_structure_loc );
-    optimization_block = get_gate_num();
-
-
-    sstream.str("");
-    sstream << optimization_problem(optimized_parameters_mtx.get_data()) << std::endl;
-    print(sstream, 3);	
-    	
-    Gates_block* gate_structure_tmp = replace_trivial_CRY_gates( gate_structure_loc, optimized_parameters_mtx );
-    Matrix_real optimized_parameters_save = optimized_parameters_mtx;
-
-    release_gates();
-    optimized_parameters_mtx = optimized_parameters_save;
-
-    // solve the optimization problem
-    N_Qubit_Decomposition_custom cDecomp_custom;
-
-
-    std::map<std::string, Config_Element> config_copy;
-    config_copy.insert(config.begin(), config.end());
-    if ( config.count("max_inner_iterations_final") > 0 ) {
-        long long val;
-        config["max_inner_iterations_final"].get_property( val ); 
-        Config_Element element;
-        element.set_property( "max_inner_iterations", val ); 
-        config_copy["max_inner_iterations"] = element;
-    }
-
-
-    // solve the optimization problem in isolated optimization process
-    cDecomp_custom = N_Qubit_Decomposition_custom( Umtx.copy(), qbit_num, false, config_copy, initial_guess, accelerator_num);
-    cDecomp_custom.set_custom_gate_structure( gate_structure_tmp );
-    cDecomp_custom.set_optimized_parameters( optimized_parameters_mtx.get_data(), optimized_parameters_mtx.size() );
-    cDecomp_custom.set_optimization_blocks( gate_structure_loc->get_gate_num() );
-    cDecomp_custom.set_max_iteration( max_outer_iterations );
-    cDecomp_custom.set_verbose(verbose);
-    cDecomp_custom.set_cost_function_variant( cost_fnc );
-    cDecomp_custom.set_debugfile("");
-    cDecomp_custom.set_iteration_loops( iteration_loops );
-    cDecomp_custom.set_optimization_tolerance( optimization_tolerance ); 
-    cDecomp_custom.set_trace_offset( trace_offset ); 
-    cDecomp_custom.set_optimizer( alg );  
-    if (alg==ADAM || alg==BFGS2) { 
-        int param_num_loc = gate_structure_loc->get_parameter_num();
-        int max_inner_iterations_loc = (double)param_num_loc/852 * 1e7;
-        cDecomp_custom.set_max_inner_iterations( max_inner_iterations_loc );  
-        cDecomp_custom.set_random_shift_count_max( 10000 );   
-        cDecomp_custom.set_adaptive_eta( true );      
-        cDecomp_custom.set_randomized_radius( radius );             
-    }
-    else if ( alg==ADAM_BATCHED ) {
-        cDecomp_custom.set_optimizer( alg );  
-        int max_inner_iterations_loc = 2500;
-        cDecomp_custom.set_max_inner_iterations( max_inner_iterations_loc );  
-        cDecomp_custom.set_random_shift_count_max( 5 );   
-        cDecomp_custom.set_adaptive_eta( true );      
-        cDecomp_custom.set_randomized_radius( radius );   
-    }
-    else if ( alg==BFGS ) {
-        cDecomp_custom.set_optimizer( alg );  
-        int max_inner_iterations_loc = 10000;
-        cDecomp_custom.set_max_inner_iterations( max_inner_iterations_loc );    
-        cDecomp_custom.set_randomized_radius( radius );   
-    }
-    cDecomp_custom.set_iteration_threshold_of_randomization( iteration_threshold_of_randomization );
-    cDecomp_custom.start_decomposition(true);
-    number_of_iters += cDecomp_custom.get_num_iters();
-
-    current_minimum = cDecomp_custom.get_current_minimum();
-    optimized_parameters_mtx = cDecomp_custom.get_optimized_parameters();
-
-
-    combine( gate_structure_tmp );
-    delete( gate_structure_tmp );
-    delete( gate_structure_loc );
-
-    sstream.str("");
-    sstream << optimization_problem(optimized_parameters_mtx.get_data()) << std::endl;
-    print(sstream, 3);	
-    	
-    std::string filename2("circuit_final.binary");
-
-    if (project_name != "") {
-        filename2=project_name+ "_"  +filename2;
-    }
+ 
+    // finalyzing the gate structure by turning CRY gates inti CNOT gates and do optimization cycles to correct approximation in this transformation 
+    // (CRY gates with small rotation angles are expressed with a single CNOT gate
+    finalize_circuit(prepare_export);
 
-    export_gate_list_to_binary(optimized_parameters_mtx, this, filename2, verbose);  
+}
 
-    // prepare gates to export
-    if (prepare_export) {
-        prepare_gates_to_export();
-    }
-    
-    decomposition_error = optimization_problem(optimized_parameters_mtx);
-    
-    // get the number of gates used in the decomposition
-    gates_num gates_num = get_gate_nums();
 
-    
-    sstream.str("");
-    sstream << "In the decomposition with error = " << decomposition_error << " were used " << layer_num << " gates with:" << std::endl;
-      
-        if ( gates_num.u3>0 ) sstream << gates_num.u3 << " U3 gates," << std::endl;
-        if ( gates_num.rx>0 ) sstream << gates_num.rx << " RX gates," << std::endl;
-        if ( gates_num.ry>0 ) sstream << gates_num.ry << " RY gates," << std::endl;
-        if ( gates_num.rz>0 ) sstream << gates_num.rz << " RZ gates," << std::endl;
-        if ( gates_num.cnot>0 ) sstream << gates_num.cnot << " CNOT gates," << std::endl;
-        if ( gates_num.cz>0 ) sstream << gates_num.cz << " CZ gates," << std::endl;
-        if ( gates_num.ch>0 ) sstream << gates_num.ch << " CH gates," << std::endl;
-        if ( gates_num.x>0 ) sstream << gates_num.x << " X gates," << std::endl;
-        if ( gates_num.sx>0 ) sstream << gates_num.sx << " SX gates," << std::endl; 
-        if ( gates_num.syc>0 ) sstream << gates_num.syc << " Sycamore gates," << std::endl;   
-        if ( gates_num.un>0 ) sstream << gates_num.un << " UN gates," << std::endl;
-        if ( gates_num.cry>0 ) sstream << gates_num.cry << " CRY gates," << std::endl;  
-        if ( gates_num.adap>0 ) sstream << gates_num.adap << " Adaptive gates," << std::endl;
-    
-        sstream << std::endl;
-        tbb::tick_count current_time = tbb::tick_count::now();
 
-	sstream << "--- In total " << (current_time - start_time).seconds() << " seconds elapsed during the decomposition ---" << std::endl;
-    	print(sstream, 1);	    	
-    	
 
-#if BLAS==0 // undefined BLAS
-    omp_set_num_threads(num_threads);
-#elif BLAS==1 //MKL
-    MKL_Set_Num_Threads(num_threads);
-#elif BLAS==2 //OpenBLAS
-    openblas_set_num_threads(num_threads);
-#endif
 
-}
-void N_Qubit_Decomposition_adaptive::get_initial_circuit(){
+/**
+@brief ???????????????????
+*/
+void N_Qubit_Decomposition_adaptive::get_initial_circuit() {
 // temporarily turn off OpenMP parallelism
 #if BLAS==0 // undefined BLAS
     num_threads = omp_get_max_threads();
     omp_set_num_threads(1);
 #elif BLAS==1 // MKL
     num_threads = mkl_get_max_threads();
     MKL_Set_Num_Threads(1);
@@ -457,16 +233,14 @@
 	sstream << "please increase level limit" << std::endl;
         print(sstream, 0);	
         return;
     }
 
 
 
-    double optimization_tolerance_orig = optimization_tolerance;
-
 
     Gates_block* gate_structure_loc = NULL;
     if ( gates.size() > 0 ) {
         std::stringstream sstream;
         sstream << "Using imported gate structure for the decomposition." << std::endl;
         print(sstream, 1);	
 	        
@@ -476,38 +250,60 @@
         std::stringstream sstream;
         sstream << "Construct initial gate structure for the decomposition." << std::endl;
         print(sstream, 1);
         gate_structure_loc = determine_initial_gate_structure(optimized_parameters_mtx);
     }
 
 
-    std::string filename("circuit_squander.binary");
-    if (project_name != "") {
-        filename = project_name+ "_" +filename;
+    long long export_circuit_2_binary_loc;
+    if ( config.count("export_circuit_2_binary") > 0 ) {
+        config["export_circuit_2_binary"].get_property( export_circuit_2_binary_loc );  
     }
-
-    export_gate_list_to_binary(optimized_parameters_mtx, gate_structure_loc, filename, verbose);
-    std::string unitaryname("unitary_squander.binary");
-    if (project_name != "") {
-        filename = project_name+ "_" +unitaryname;
+    else {
+        export_circuit_2_binary_loc = 0;
+    }     
+        
+        
+    if ( export_circuit_2_binary_loc > 0 ) {
+        std::string filename("circuit_squander.binary");
+        if (project_name != "") {
+            filename = project_name+ "_" +filename;
+        }
+        export_gate_list_to_binary(optimized_parameters_mtx, gate_structure_loc, filename, verbose);
+        
+        std::string unitaryname("unitary_squander.binary");
+        if (project_name != "") {
+            filename = project_name+ "_" +unitaryname;
+        }
+        export_unitary(unitaryname);
+        
     }
-    export_unitary(unitaryname);
+    
+    // store the created gate structure
     release_gates();
 	combine( gate_structure_loc );
 	delete( gate_structure_loc );
+	
+	
 #if BLAS==0 // undefined BLAS
     omp_set_num_threads(num_threads);
 #elif BLAS==1 //MKL
     MKL_Set_Num_Threads(num_threads);
 #elif BLAS==2 //OpenBLAS
     openblas_set_num_threads(num_threads);
 #endif
 }
 
-void N_Qubit_Decomposition_adaptive::compress_circuit(){
+
+
+
+/**
+@brief ???????????????????
+*/
+void N_Qubit_Decomposition_adaptive::compress_circuit() {
 // temporarily turn off OpenMP parallelism
 #if BLAS==0 // undefined BLAS
     num_threads = omp_get_max_threads();
     omp_set_num_threads(1);
 #elif BLAS==1 // MKL
     num_threads = mkl_get_max_threads();
     MKL_Set_Num_Threads(1);
@@ -533,16 +329,28 @@
     }
     else {
         std::stringstream sstream;
         sstream << "No circuit initalised." << std::endl;
         print(sstream, 1);
         return;
     }
+    
+    
     int iter = 0;
     int uncompressed_iter_num = 0;
+    
+    long long export_circuit_2_binary_loc;
+    if ( config.count("export_circuit_2_binary") > 0 ) {
+        config["export_circuit_2_binary"].get_property( export_circuit_2_binary_loc );  
+    }
+    else {
+        export_circuit_2_binary_loc = 0;
+    }      
+    
+        
     while ( iter<25 || uncompressed_iter_num <= 5 ) {
         std::stringstream sstream;
         sstream.str("");
         sstream << "iteration " << iter+1 << ": ";
         print(sstream, 1);	
 
        
@@ -557,22 +365,31 @@
 
         if ( gate_structure_compressed != gate_structure_loc ) {
             delete( gate_structure_loc );
             gate_structure_loc = gate_structure_compressed;
             gate_structure_compressed = NULL;
             
 
-            std::string filename("circuit_compression.binary");
-            if (project_name != "") { 
-                filename=project_name+ "_"  +filename;
-            }
 
-            export_gate_list_to_binary(optimized_parameters_mtx, gate_structure_loc, filename, verbose); 
-            std::string filename_unitary("unitary_compression.binary");
-            export_unitary(filename_unitary);
+            if ( export_circuit_2_binary_loc > 0 ) {
+                std::string filename("circuit_compression.binary");
+                if (project_name != "") { 
+                    filename=project_name+ "_"  +filename;
+                }
+                export_gate_list_to_binary(optimized_parameters_mtx, gate_structure_loc, filename, verbose); 
+            
+            
+                std::string filename_unitary("unitary_compression.binary");
+                if (project_name != "") { 
+                    filename_unitary=project_name+ "_"  +filename_unitary;
+                }  
+                export_unitary(filename_unitary);
+                
+                
+            }
         }
 
         iter++;
 
         if (uncompressed_iter_num>10) break;
             // store the decomposing gate structure
     }
@@ -584,40 +401,55 @@
 #elif BLAS==1 //MKL
     MKL_Set_Num_Threads(num_threads);
 #elif BLAS==2 //OpenBLAS
     openblas_set_num_threads(num_threads);
 #endif
 }
 
-void N_Qubit_Decomposition_adaptive::finalize_circuit(bool prepare_export){
+
+
+
+
+
+
+/**
+@brief ???????????????????
+*/
+void N_Qubit_Decomposition_adaptive::finalize_circuit(bool prepare_export) {
+
+
 // temporarily turn off OpenMP parallelism
 #if BLAS==0 // undefined BLAS
     num_threads = omp_get_max_threads();
     omp_set_num_threads(1);
 #elif BLAS==1 // MKL
     num_threads = mkl_get_max_threads();
     MKL_Set_Num_Threads(1);
 #elif BLAS==2 //OpenBLAS
     num_threads = openblas_get_num_threads();
     openblas_set_num_threads(1);
 #endif
+
+
 	Gates_block* gate_structure_loc = NULL;
     if ( gates.size() > 0 ) {
         std::stringstream sstream;
         sstream << "Using imported gate structure for the compression." << std::endl;
         print(sstream, 1);	
 	        
         gate_structure_loc =  static_cast<Gates_block*>(this)->clone();
     }
     else {
         std::stringstream sstream;
         sstream << "No circuit initalised." << std::endl;
         print(sstream, 1);
         return;
     }
+    
+    
     std::stringstream sstream;
     sstream.str("");
     sstream << "**************************************************************" << std::endl;
     sstream << "************ Final tuning of the Gate structure **************" << std::endl;
     sstream << "**************************************************************" << std::endl;
     print(sstream, 1);	    	
     
@@ -705,22 +537,34 @@
     combine( gate_structure_tmp );
     delete( gate_structure_tmp );
     delete( gate_structure_loc );
 
     sstream.str("");
     sstream << optimization_problem(optimized_parameters_mtx.get_data()) << std::endl;
     print(sstream, 3);	
+    
+    long long export_circuit_2_binary_loc;
+    if ( config.count("export_circuit_2_binary") > 0 ) {
+        config["export_circuit_2_binary"].get_property( export_circuit_2_binary_loc );  
+    }
+    else {
+        export_circuit_2_binary_loc = 0;
+    }       
     	
-    std::string filename2("circuit_final.binary");
+    	
+    if ( export_circuit_2_binary_loc > 0 ) {
+        std::string filename2("circuit_final.binary");
 
-    if (project_name != "") {
-        filename2=project_name+ "_"  +filename2;
-    }
+        if (project_name != "") {
+            filename2=project_name+ "_"  +filename2;
+        }
 
-    export_gate_list_to_binary(optimized_parameters_mtx, this, filename2, verbose);  
+        export_gate_list_to_binary(optimized_parameters_mtx, this, filename2, verbose);  
+    
+    }
 
     // prepare gates to export
     if (prepare_export) {
         prepare_gates_to_export();
     }
     
     decomposition_error = optimization_problem(optimized_parameters_mtx);
@@ -769,28 +613,36 @@
 
     //measure the time for the decompositin
     tbb::tick_count start_time_loc = tbb::tick_count::now();
 
     std::stringstream sstream;
     sstream << "Starting optimization with " << gate_structure_loc->get_gate_num() << " decomposing layers." << std::endl;
     print(sstream, 1);	
+    
+    double optimization_tolerance_loc;
+    if ( config.count("optimization_tolerance") > 0 ) {
+        config["optimization_tolerance"].get_property( optimization_tolerance_loc );  
+    }
+    else {
+        optimization_tolerance_loc = optimization_tolerance;
+    }      
 
     // solve the optimization problem
     N_Qubit_Decomposition_custom cDecomp_custom;
     // solve the optimization problem in isolated optimization process
     cDecomp_custom = N_Qubit_Decomposition_custom( Umtx.copy(), qbit_num, false, config, initial_guess, accelerator_num);
     cDecomp_custom.set_custom_gate_structure( gate_structure_loc );
     cDecomp_custom.set_optimized_parameters( optimized_parameters_mtx_loc.get_data(), optimized_parameters_mtx_loc.size() );
     cDecomp_custom.set_optimization_blocks( gate_structure_loc->get_gate_num() );
     cDecomp_custom.set_max_iteration( max_outer_iterations );
     cDecomp_custom.set_verbose(verbose);
     cDecomp_custom.set_cost_function_variant( cost_fnc );
     cDecomp_custom.set_debugfile("");
     cDecomp_custom.set_iteration_loops( iteration_loops );
-    cDecomp_custom.set_optimization_tolerance( optimization_tolerance ); 
+    cDecomp_custom.set_optimization_tolerance( optimization_tolerance_loc ); 
     cDecomp_custom.set_trace_offset( trace_offset ); 
     cDecomp_custom.set_optimizer( alg );  
     cDecomp_custom.set_project_name( project_name );
     if (alg==ADAM || alg==BFGS2) { 
         int param_num_loc = gate_structure_loc->get_parameter_num();
         int max_inner_iterations_loc = (double)param_num_loc/852 * 1e7;
         cDecomp_custom.set_max_inner_iterations( max_inner_iterations_loc );  
@@ -820,30 +672,30 @@
     tbb::tick_count end_time_loc = tbb::tick_count::now();
 
     current_minimum = cDecomp_custom.get_current_minimum();
     optimized_parameters_mtx_loc = cDecomp_custom.get_optimized_parameters();
 
 
 
-    if ( cDecomp_custom.get_current_minimum() < optimization_tolerance ) {
+    if ( cDecomp_custom.get_current_minimum() < optimization_tolerance_loc ) {
         std::stringstream sstream;
 	sstream << "Optimization problem solved with " << gate_structure_loc->get_gate_num() << " decomposing layers in " << (end_time_loc-start_time_loc).seconds() << " seconds." << std::endl;
         print(sstream, 1);	
     }   
     else {
         std::stringstream sstream;
 	sstream << "Optimization problem converged to " << cDecomp_custom.get_current_minimum() << " with " <<  gate_structure_loc->get_gate_num() << " decomposing layers in "   << (end_time_loc-start_time_loc).seconds() << " seconds." << std::endl;
         print(sstream, 1);       
     }
 
-    if (current_minimum > optimization_tolerance) {
+    if (current_minimum > optimization_tolerance_loc) {
         std::stringstream sstream;
 	sstream << "Decomposition did not reached prescribed high numerical precision." << std::endl; 
         print(sstream, 1);             
-        optimization_tolerance = 1.5*current_minimum < 1e-2 ? 1.5*current_minimum : 1e-2;
+        optimization_tolerance_loc = 1.5*current_minimum < 1e-2 ? 1.5*current_minimum : 1e-2;
     }
 
     sstream.str("");
     sstream << "Continue with the compression of gate structure consisting of " << gate_structure_loc->get_gate_num() << " decomposing layers." << std::endl;
     print(sstream, 1);	
     return gate_structure_loc;
 
@@ -858,18 +710,27 @@
 N_Qubit_Decomposition_adaptive::determine_initial_gate_structure(Matrix_real& optimized_parameters_mtx_loc) {
 
     // strages to store the optimized minimums in case of different cirquit depths
     std::vector<double> minimum_vec;
     std::vector<Gates_block*> gate_structure_vec;
     std::vector<Matrix_real> optimized_parameters_vec;
     
+    double optimization_tolerance_loc;
+    if ( config.count("optimization_tolerance") > 0 ) {
+        config["optimization_tolerance"].get_property( optimization_tolerance_loc );  
+    }
+    else {
+        optimization_tolerance_loc = optimization_tolerance;
+    }         
+        
+    
 
 
     int level = level_limit_min;
-    while ( current_minimum > optimization_tolerance && level <= level_limit) {
+    while ( current_minimum > optimization_tolerance_loc && level <= level_limit) {
 
         // create gate structure to be optimized
         Gates_block* gate_structure_loc = new Gates_block(qbit_num);  
         
         optimized_parameters_mtx_loc = Matrix_real(0,0);
                    
         for (int idx=0; idx<level; idx++) {
@@ -909,15 +770,15 @@
 #ifndef __DFE__
                 cDecomp_custom_random.set_verbose(verbose);
 #else
                 cDecomp_custom_random.set_verbose(0);
 #endif
                 cDecomp_custom_random.set_cost_function_variant( cost_fnc );
                 cDecomp_custom_random.set_debugfile("");
-                cDecomp_custom_random.set_optimization_tolerance( optimization_tolerance );
+                cDecomp_custom_random.set_optimization_tolerance( optimization_tolerance_loc );
                 cDecomp_custom_random.set_trace_offset( trace_offset ); 
                 cDecomp_custom_random.set_optimizer( alg );
                 cDecomp_custom_random.set_project_name( project_name );
                 if ( alg == ADAM || alg == BFGS2 ) {
                     int param_num_loc = gate_structure_loc->get_parameter_num();
                     int max_inner_iterations_loc = (double)param_num_loc/852 * 1e7;
                     cDecomp_custom_random.set_max_inner_iterations( max_inner_iterations_loc );  
@@ -985,25 +846,25 @@
 */
          double current_minimum_random         = cDecomp_custom_random.get_current_minimum();
          double current_minimum_close_to_zero = cDecomp_custom_close_to_zero.get_current_minimum();
          double current_minimum_loc;
 
 
          // select between the results obtained for different initial value strategy
-         if ( current_minimum_random < optimization_tolerance && current_minimum_close_to_zero > optimization_tolerance ) {
+         if ( current_minimum_random < optimization_tolerance_loc && current_minimum_close_to_zero > optimization_tolerance_loc ) {
              current_minimum_loc = current_minimum_random;
              optimized_parameters_mtx_loc = cDecomp_custom_random.get_optimized_parameters();
              initial_guess = RANDOM;
          }
-         else if ( current_minimum_random > optimization_tolerance && current_minimum_close_to_zero < optimization_tolerance ) {
+         else if ( current_minimum_random > optimization_tolerance_loc && current_minimum_close_to_zero < optimization_tolerance_loc ) {
              current_minimum_loc = current_minimum_close_to_zero;
              optimized_parameters_mtx_loc = cDecomp_custom_close_to_zero.get_optimized_parameters();
              initial_guess = CLOSE_TO_ZERO;
          }
-         else if ( current_minimum_random < optimization_tolerance && current_minimum_close_to_zero < optimization_tolerance ) {
+         else if ( current_minimum_random < optimization_tolerance_loc && current_minimum_close_to_zero < optimization_tolerance_loc ) {
              Matrix_real optimized_parameters_mtx_random = cDecomp_custom_random.get_optimized_parameters();
              Matrix_real optimized_parameters_mtx_close_to_zero = cDecomp_custom_close_to_zero.get_optimized_parameters();
 
              int panelty_random         = get_panelty(gate_structure_loc, optimized_parameters_mtx_random);
              int panelty_close_to_zero = get_panelty(gate_structure_loc, optimized_parameters_mtx_close_to_zero );
 
              if ( panelty_random < panelty_close_to_zero ) {
@@ -1034,15 +895,15 @@
 
         minimum_vec.push_back(current_minimum_loc);
         gate_structure_vec.push_back(gate_structure_loc);
         optimized_parameters_vec.push_back(optimized_parameters_mtx_loc);
 
 
 
-        if ( current_minimum_loc < optimization_tolerance ) {
+        if ( current_minimum_loc < optimization_tolerance_loc ) {
 	    std::stringstream sstream;
             sstream << "Optimization problem solved with " << gate_structure_loc->get_gate_num() << " decomposing layers in " << (end_time_loc-start_time_loc).seconds() << " seconds." << std::endl;
             print(sstream, 1);	       
             break;
         }   
         else {
             std::stringstream sstream;
@@ -1077,19 +938,20 @@
         delete( gate_structure_vec[idx] );
     }    
     minimum_vec.clear();
     gate_structure_vec.clear();
     optimized_parameters_vec.clear();
     
 
-    if (current_minimum > optimization_tolerance) {
+
+    if (current_minimum > optimization_tolerance_loc) {
        std::stringstream sstream;
        sstream << "Decomposition did not reached prescribed high numerical precision." << std::endl;
        print(sstream, 1);              
-       optimization_tolerance = 1.5*current_minimum < 1e-2 ? 1.5*current_minimum : 1e-2;
+       optimization_tolerance_loc = 1.5*current_minimum < 1e-2 ? 1.5*current_minimum : 1e-2;
     }
     
     std::stringstream sstream;
     sstream << "Continue with the compression of gate structure consisting of " << gate_structure_loc->get_gate_num() << " decomposing layers." << std::endl;
     print(sstream, 1);	
     return gate_structure_loc;
        
@@ -1112,14 +974,23 @@
 
     // create a list of layers to be tested for removal.
     std::vector<int> layers_to_remove;
     layers_to_remove.reserve(layer_num_orig);
     for (int idx=0; idx<layer_num_orig; idx++ ) {
         layers_to_remove.push_back(idx+1);
     }   
+    
+    
+    double optimization_tolerance_loc;
+    if ( config.count("optimization_tolerance") > 0 ) {
+        config["optimization_tolerance"].get_property( optimization_tolerance_loc );  
+    }
+    else {
+        optimization_tolerance_loc = optimization_tolerance;
+    }         
 
     // random generator of integers   
     std::uniform_int_distribution<> distrib_int(0, 5000);  
 
     while ( (int)layers_to_remove.size() > layer_num_max ) {
         int remove_idx = distrib_int(gen) % layers_to_remove.size();
        
@@ -1158,26 +1029,27 @@
         Gates_block* gate_structure_tmp;
         if ( gate_structure_reduced->get_gate_num() ==  gate_structure->get_gate_num() ) {
             gate_structure_tmp = gate_structure_reduced->clone();
         }
         else {
             gate_structure_tmp = remove_trivial_gates( gate_structure_reduced, optimized_parameters_loc, current_minimum_loc );
         }
+      
         panelties[idx] = get_panelty(gate_structure_tmp, optimized_parameters_loc);
         gate_structures_vec[idx] = gate_structure_tmp;
         optimized_parameters_vec[idx] = optimized_parameters_loc;
         current_minimum_vec[idx] = current_minimum_loc;
         iteration_num_vec[idx] = iteration_num;
         Umtx_vec[idx] = Umtx;
         
 
         delete(gate_structure_reduced);
 
 #ifdef __DFE__
-        if ( current_minimum_vec[idx] < optimization_tolerance ) {
+        if ( current_minimum_vec[idx] < optimization_tolerance_loc ) {
             break;
         }
 #endif
     }
 
 
 //panelties.print_matrix();
@@ -1270,28 +1142,36 @@
     if ( config.count("max_inner_iterations_compression") > 0 ) {
         long long val;
         config["max_inner_iterations_compression"].get_property( val ); 
         Config_Element element;
         element.set_property( "max_inner_iterations", val ); 
         config_copy["max_inner_iterations"] = element;
     }
+    
+    double optimization_tolerance_loc;
+    if ( config.count("optimization_tolerance") > 0 ) {
+        config["optimization_tolerance"].get_property( optimization_tolerance_loc );  
+    }
+    else {
+        optimization_tolerance_loc = optimization_tolerance;
+    }       
 
 
        
     // solve the optimization problem in isolated optimization process
     cDecomp_custom = N_Qubit_Decomposition_custom( Umtx.copy(), qbit_num, false, config_copy, initial_guess, accelerator_num);
     cDecomp_custom.set_custom_gate_structure( gate_structure_reduced );
     cDecomp_custom.set_optimized_parameters( parameters_reduced.get_data(), parameters_reduced.size() );
     cDecomp_custom.set_verbose(0);
     cDecomp_custom.set_cost_function_variant( cost_fnc );
     cDecomp_custom.set_debugfile("");
     cDecomp_custom.set_max_iteration( max_outer_iterations );
     cDecomp_custom.set_iteration_loops( iteration_loops );
     cDecomp_custom.set_optimization_blocks( gate_structure_reduced->get_gate_num() ) ;
-    cDecomp_custom.set_optimization_tolerance( optimization_tolerance );
+    cDecomp_custom.set_optimization_tolerance( optimization_tolerance_loc );
     cDecomp_custom.set_trace_offset( trace_offset ); 
     cDecomp_custom.set_optimizer( alg );
     if ( alg == ADAM || alg==BFGS2) {
         cDecomp_custom.set_max_inner_iterations( 1e5 );  
         cDecomp_custom.set_random_shift_count_max( 1 );     
         cDecomp_custom.set_adaptive_eta( false );
         cDecomp_custom.set_randomized_radius( radius );        
@@ -1303,15 +1183,15 @@
         cDecomp_custom.set_randomized_radius( radius );   
     }
     cDecomp_custom.set_iteration_threshold_of_randomization( 2500 );
     cDecomp_custom.start_decomposition(true);
     iteration_num = cDecomp_custom.get_num_iters();
     double current_minimum_tmp = cDecomp_custom.get_current_minimum();
 
-    if ( current_minimum_tmp < optimization_tolerance ) {
+    if ( current_minimum_tmp < optimization_tolerance_loc ) {
         //cDecomp_custom.list_gates(0);
         optimized_parameters = cDecomp_custom.get_optimized_parameters();
         current_minimum_loc = current_minimum_tmp;
         return gate_structure_reduced;
     }
 
 
@@ -1338,19 +1218,19 @@
         
         if ( std::abs(std::sin(parameter)) < 0.999 && std::abs(std::cos(parameter)) < 1e-3 ) {
             // Condition of pure CNOT gate
             panelty += 1;
         }
         else if ( std::abs(std::sin(parameter)) < 1e-3 && std::abs(1-std::cos(parameter)) < 1e-3 ) {
             // Condition of pure Identity gate
-            panelty++;
+            //panelty++;
         }
         else {
             // Condition of controlled rotation gate
-            panelty += 1;
+            panelty += 2;
         }
 
         Gate* gate = gate_structure->get_gate( idx );
         parameter_idx += gate->get_parameter_num();
 
     }
```

### Comparing `squander-1.8.2/decomposition/N_Qubit_Decomposition_custom.cpp` & `squander-1.8.3/decomposition/N_Qubit_Decomposition_custom.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/decomposition/Sub_Matrix_Decomposition.cpp` & `squander-1.8.3/decomposition/Sub_Matrix_Decomposition.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -448,15 +448,15 @@
 
         // random generator of real numbers   
         std::uniform_real_distribution<> distrib_real(0.0, 2*M_PI);
 
         // do the optimization loops
         for (long long idx=0; idx<iteration_loops_max; idx++) {
 
-            Problem p(num_of_parameters, 0, 2*M_PI, optimization_problem, optimization_problem_grad, optimization_problem_combined, (void*)this);
+            Problem p(num_of_parameters, -1e100, 1e100, optimization_problem, optimization_problem_grad, optimization_problem_combined, (void*)this);
             Tolmin tolmin(&p);
 
             Matrix_real x(solution_guess.get_data(), num_of_parameters, 1); 
 
             double f = tolmin.Solve(x, false, max_inner_iterations);
 
             if (current_minimum > f) {
@@ -554,15 +554,15 @@
 
 /**
 @brief Calculate the approximate derivative (f-f0)/(x-x0) of the cost function with respect to the free parameters.
 @param parameters A GNU Scientific Library vector containing the free parameters to be optimized.
 @param void_instance A void pointer pointing to the instance of the current class.
 @param grad A GNU Scientific Library vector containing the calculated gradient components.
 */
-void Sub_Matrix_Decomposition::optimization_problem_grad( Matrix_real parameters, void* void_instance, Matrix_real grad ) {
+void Sub_Matrix_Decomposition::optimization_problem_grad( Matrix_real parameters, void* void_instance, Matrix_real& grad ) {
 
     // The function value at x0
     double f0;
 
     // calculate the approximate gradient
     optimization_problem_combined( parameters, void_instance, &f0, grad);
 
@@ -573,15 +573,15 @@
 /**
 @brief Call to calculate both the cost function and the its gradient components.
 @param parameters A GNU Scientific Library vector containing the free parameters to be optimized.
 @param void_instance A void pointer pointing to the instance of the current class.
 @param f0 The value of the cost function at x0.
 @param grad A GNU Scientific Library vector containing the calculated gradient components.
 */
-void Sub_Matrix_Decomposition::optimization_problem_combined( Matrix_real parameters, void* void_instance, double* f0, Matrix_real grad ) {
+void Sub_Matrix_Decomposition::optimization_problem_combined( Matrix_real parameters, void* void_instance, double* f0, Matrix_real& grad ) {
 
     Sub_Matrix_Decomposition* instance = reinterpret_cast<Sub_Matrix_Decomposition*>(void_instance);
 
     int parameter_num_loc = instance->get_parameter_num();
 
     // storage for the function values calculated at the displaced points x
     Matrix_real f(1, grad.size());
```

### Comparing `squander-1.8.2/decomposition/Sub_Matrix_Decomposition_Cost_Function.cpp` & `squander-1.8.3/decomposition/Sub_Matrix_Decomposition_Cost_Function.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/decomposition/include/Decomposition_Base.h` & `squander-1.8.3/decomposition/include/Decomposition_Base.h`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,32 @@
 #include "config_element.h"
 
 #include <random>
 
 /// @brief Type definition of the types of the initial guess
 typedef enum guess_type {ZEROS, RANDOM, CLOSE_TO_ZERO} guess_type;
 
+#ifndef OPENBLAS_CONST
+# define OPENBLAS_CONST const
+#endif
+#if defined(OS_WINDOWS) && defined(__64BIT__)
+typedef long long BLASLONG;
+typedef unsigned long long BLASULONG;
+#else
+typedef long BLASLONG;
+typedef unsigned long BLASULONG;
+#endif
+typedef BLASLONG blasint;
+#if defined(OS_WINDOWS) && defined(__64BIT__)
+#define blasabs(x) llabs(x)
+#else
+#define blasabs(x) labs(x)
+#endif
+
+extern "C" double cblas_dznrm2(OPENBLAS_CONST blasint N, OPENBLAS_CONST void *X, OPENBLAS_CONST blasint incX);
 
 /**
 @brief A class containing basic methods for the decomposition process.
 */
 class Decomposition_Base : public Gates_block {
```

### Comparing `squander-1.8.2/decomposition/include/N_Qubit_Decomposition.h` & `squander-1.8.3/decomposition/include/N_Qubit_Decomposition.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/decomposition/include/N_Qubit_Decomposition_Base.h` & `squander-1.8.3/decomposition/include/N_Qubit_Decomposition_Base.h`

 * *Files 0% similar despite different names*

```diff
@@ -309,15 +309,15 @@
 /**
 @brief Call to calculate both the cost function and the its gradient components.
 @param parameters Array containing the free parameters to be optimized.
 @param void_instance A void pointer pointing to the instance of the current class.
 @param f0 The value of the cost function at x0.
 @param grad Array containing the calculated gradient components.
 */
-static void optimization_problem_combined( Matrix_real parameters, void* void_instance, double* f0, Matrix_real grad );
+static void optimization_problem_combined( Matrix_real parameters, void* void_instance, double* f0, Matrix_real& grad );
 
 
 
 
 /**
 @brief Call to calculate both the cost function and the its gradient components.
 @param parameters The parameters for which the cost fuction shoule be calculated
```

### Comparing `squander-1.8.2/decomposition/include/N_Qubit_Decomposition_Cost_Function.h` & `squander-1.8.3/decomposition/include/N_Qubit_Decomposition_Cost_Function.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/decomposition/include/N_Qubit_Decomposition_adaptive.h` & `squander-1.8.3/decomposition/include/N_Qubit_Decomposition_adaptive.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/decomposition/include/N_Qubit_Decomposition_custom.h` & `squander-1.8.3/decomposition/include/N_Qubit_Decomposition_custom.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/decomposition/include/Sub_Matrix_Decomposition.h` & `squander-1.8.3/decomposition/include/Sub_Matrix_Decomposition.h`

 * *Files 0% similar despite different names*

```diff
@@ -134,25 +134,25 @@
 
 /**
 @brief Calculate the approximate derivative (f-f0)/(x-x0) of the cost function with respect to the free parameters.
 @param parameters A GNU Scientific Library vector containing the free parameters to be optimized.
 @param void_instance A void pointer pointing to the instance of the current class.
 @param grad A GNU Scientific Library vector containing the calculated gradient components.
 */
-static void optimization_problem_grad( Matrix_real parameters, void* void_instance, Matrix_real grad  );
+static void optimization_problem_grad( Matrix_real parameters, void* void_instance, Matrix_real& grad  );
 
 
 /**
 @brief Call to calculate both the cost function and the its gradient components.
 @param parameters A GNU Scientific Library vector containing the free parameters to be optimized.
 @param void_instance A void pointer pointing to the instance of the current class.
 @param f0 The value of the cost function at x0.
 @param grad A GNU Scientific Library vector containing the calculated gradient components.
 */
-static void optimization_problem_combined( Matrix_real parameters, void* void_instance, double* f0, Matrix_real grad );
+static void optimization_problem_combined( Matrix_real parameters, void* void_instance, double* f0, Matrix_real& grad );
 
 /**
 @brief Set the number of identical successive blocks during the subdecomposition of the qbit-th qubit.
 @param qbit The number of qubits for which the maximal number of layers should be used in the subdecomposition.
 @param identical_blocks_in The number of successive identical layers used in the subdecomposition.
 @return Returns with zero in case of success.
 */
```

### Comparing `squander-1.8.2/decomposition/include/Sub_Matrix_Decomposition_Cost_Function.h` & `squander-1.8.3/decomposition/include/Sub_Matrix_Decomposition_Cost_Function.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/gates/Adaptive.cpp` & `squander-1.8.3/gates/Adaptive.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/gates/CH.cpp` & `squander-1.8.3/gates/CH.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/gates/CNOT.cpp` & `squander-1.8.3/gates/CNOT.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/gates/CRY.cpp` & `squander-1.8.3/gates/CRY.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/gates/CZ.cpp` & `squander-1.8.3/gates/CZ.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/gates/Composite.cpp` & `squander-1.8.3/gates/Composite.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/gates/Gate.cpp` & `squander-1.8.3/gates/Gate.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/gates/Gates_block.cpp` & `squander-1.8.3/gates/Gates_block.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/gates/ON.cpp` & `squander-1.8.3/gates/ON.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/gates/RX.cpp` & `squander-1.8.3/gates/RX.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/gates/RY.cpp` & `squander-1.8.3/gates/RY.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/gates/RZ.cpp` & `squander-1.8.3/gates/RZ.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/gates/SX.cpp` & `squander-1.8.3/gates/SX.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/gates/SYC.cpp` & `squander-1.8.3/gates/SYC.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/gates/U3.cpp` & `squander-1.8.3/gates/U3.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/gates/UN.cpp` & `squander-1.8.3/gates/UN.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/gates/X.cpp` & `squander-1.8.3/gates/X.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/gates/Y.cpp` & `squander-1.8.3/gates/Y.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/gates/Z.cpp` & `squander-1.8.3/gates/Z.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/gates/include/Adaptive.h` & `squander-1.8.3/gates/include/Adaptive.h`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 #ifndef ADAPTIVE_H
 #define ADAPTIVE_H
 
 #include "CRY.h"
 #include "matrix.h"
 #include "matrix_real.h"
+#define _USE_MATH_DEFINES
 #include <math.h>
 
 
 /**
 @brief A class representing a CRY gate.
 */
 class Adaptive: public CRY {
```

### Comparing `squander-1.8.2/gates/include/CH.h` & `squander-1.8.3/gates/include/CH.h`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 */
 
 #ifndef CH_H
 #define CH_H
 
 #include "matrix.h"
 #include "Gate.h"
+#define _USE_MATH_DEFINES
 #include <math.h>
 #include "CNOT.h"
 
 
 /**
 @brief A class representing a CH operation.
 */
```

### Comparing `squander-1.8.2/gates/include/CNOT.h` & `squander-1.8.3/gates/include/CNOT.h`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 */
 
 #ifndef CNOT_H
 #define CNOT_H
 
 #include "matrix.h"
 #include "Gate.h"
+#define _USE_MATH_DEFINES
 #include <math.h>
 #include <U3.h>
 
 
 /**
 @brief A class representing a CNOT operation.
 */
```

### Comparing `squander-1.8.2/gates/include/CRY.h` & `squander-1.8.3/gates/include/CRY.h`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 #ifndef CRZ_H
 #define CRZ_H
 
 #include "RY.h"
 #include "CNOT.h"
 #include "matrix.h"
 #include "matrix_real.h"
+#define _USE_MATH_DEFINES
 #include <math.h>
 
 
 /**
 @brief A class representing a CRY gate.
 */
 class CRY: public RY {
```

### Comparing `squander-1.8.2/gates/include/CZ.h` & `squander-1.8.3/gates/include/CZ.h`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 */
 
 #ifndef CZ_H
 #define CZ_H
 
 #include "matrix.h"
 #include "Gate.h"
+#define _USE_MATH_DEFINES
 #include <math.h>
 #include "CNOT.h"
 
 
 /**
 @brief A class representing a CZ operation.
 */
```

### Comparing `squander-1.8.2/gates/include/Composite.h` & `squander-1.8.3/gates/include/Composite.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/gates/include/Gate.h` & `squander-1.8.3/gates/include/Gate.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/gates/include/Gates_block.h` & `squander-1.8.3/gates/include/Gates_block.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/gates/include/ON.h` & `squander-1.8.3/gates/include/ON.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/gates/include/RX.h` & `squander-1.8.3/gates/include/RX.h`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 #ifndef RX_H
 #define RX_H
 
 #include "U3.h"
 #include "matrix.h"
 #include "matrix_real.h"
+#define _USE_MATH_DEFINES
 #include <math.h>
 
 
 /**
 @brief A class representing a U3 gate.
 */
 class RX: public U3 {
```

### Comparing `squander-1.8.2/gates/include/RY.h` & `squander-1.8.3/gates/include/RY.h`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 #ifndef RY_H
 #define RY_H
 
 #include "U3.h"
 #include "matrix.h"
 #include "matrix_real.h"
+#define _USE_MATH_DEFINES
 #include <math.h>
 
 
 /**
 @brief A class representing a U3 gate.
 */
 class RY: public U3 {
```

### Comparing `squander-1.8.2/gates/include/RZ.h` & `squander-1.8.3/gates/include/RZ.h`

 * *Files 9% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 #ifndef RZ_H
 #define RZ_H
 
 #include "U3.h"
 #include "matrix.h"
 #include "matrix_real.h"
+#define _USE_MATH_DEFINES
 #include <math.h>
 
 
 /**
 @brief A class representing a RZ gate.
 */
 class RZ: public U3 {
```

### Comparing `squander-1.8.2/gates/include/SX.h` & `squander-1.8.3/gates/include/SX.h`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 #ifndef SX_H
 #define SX_H
 
 
 #include "U3.h"
 //#include "Gate.h"
 #include "matrix.h"
+#define _USE_MATH_DEFINES
 #include <math.h>
 
 
 
 /**
 @brief A class representing a U3 gate.
 */
```

### Comparing `squander-1.8.2/gates/include/SYC.h` & `squander-1.8.3/gates/include/SYC.h`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 */
 
 #ifndef SYC_H
 #define SYC_H
 
 #include "matrix.h"
 #include "Gate.h"
+#define _USE_MATH_DEFINES
 #include <math.h>
 
 
 
 /**
 @brief A class representing a SYC operation.
 */
```

### Comparing `squander-1.8.2/gates/include/U3.h` & `squander-1.8.3/gates/include/U3.h`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 #ifndef U3_H
 #define U3_H
 
 #include "Gate.h"
 #include "matrix.h"
 #include "matrix_real.h"
+#define _USE_MATH_DEFINES
 #include <math.h>
 
 
 /**
 @brief A class representing a U3 gate.
 */
 class U3: public Gate {
```

### Comparing `squander-1.8.2/gates/include/UN.h` & `squander-1.8.3/gates/include/UN.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/gates/include/X.h` & `squander-1.8.3/gates/include/Z.h`

 * *Files 8% similar despite different names*

```diff
@@ -13,55 +13,56 @@
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see http://www.gnu.org/licenses/.
 
 @author: Peter Rakyta, Ph.D.
 */
-/*! \file RX.h
-    \brief Header file for a class representing a rotation gate around the X axis.
+/*! \file Z.h
+    \brief Header file for a class representing a rotation gate around the Z axis.
 */
 
-#ifndef X_H
-#define X_H
+#ifndef Z_H
+#define Z_H
 
 #include "U3.h"
 //#include "Gate.h"
 #include "matrix.h"
+#define _USE_MATH_DEFINES
 #include <math.h>
 
 
 /**
 @brief A class representing a U3 gate.
 */
-class X: public U3 {
+class Z: public U3 {
 
 
 public:
 
 /**
 @brief NullaRX constructor of the class.
 */
-X();
+Z();
 
 
 /**
 @brief Constructor of the class.
 @param qbit_num_in The number of qubits spanning the gate.
 @param target_qbit_in The 0<=ID<qbit_num of the target qubit.
 @param theta_in logical value indicating whether the matrix creation takes an argument theta.
 @param phi_in logical value indicating whether the matrix creation takes an argument phi
 @param lambda_in logical value indicating whether the matrix creation takes an argument lambda
 */
-X(int qbit_num_in, int target_qbit_in);
+Z(int qbit_num_in, int target_qbit_in);
 
 /**
 @brief Destructor of the class
 */
-~X();
+~Z();
 
 /**
 @brief Call to retrieve the gate matrix
 @param parameters An array of parameters to calculate the matrix of the U3 gate.
 @return Returns with a matrix of the gate
 */
 Matrix get_matrix( );
@@ -83,15 +84,15 @@
 void apply_from_right( Matrix& input );
 
 
 /**
 @brief Call to create a clone of the present class
 @return Return with a pointer pointing to the cloned object
 */
-X* clone();
+Z* clone();
 
 
 /**
 @brief Call to set the number of qubits spanning the matrix of the gate
 @param qbit_num_in The number of qubits
 */
 void set_qbit_num(int qbit_num_in);
@@ -104,9 +105,9 @@
 */
 void reorder_qubits( std::vector<int> qbit_list);
 
 
 };
 
 
-#endif //U3
+#endif //Z
```

### Comparing `squander-1.8.2/gates/include/Y.h` & `squander-1.8.3/gates/include/Y.h`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 #ifndef Y_H
 #define Y_H
 
 #include "U3.h"
 //#include "Gate.h"
 #include "matrix.h"
+#define _USE_MATH_DEFINES
 #include <math.h>
 
 
 /**
 @brief A class representing a U3 gate.
 */
 class Y: public U3 {
```

### Comparing `squander-1.8.2/gates/include/Z.h` & `squander-1.8.3/gates/include/X.h`

 * *Files 6% similar despite different names*

```diff
@@ -13,55 +13,56 @@
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see http://www.gnu.org/licenses/.
 
 @author: Peter Rakyta, Ph.D.
 */
-/*! \file Z.h
-    \brief Header file for a class representing a rotation gate around the Z axis.
+/*! \file RX.h
+    \brief Header file for a class representing a rotation gate around the X axis.
 */
 
-#ifndef Z_H
-#define Z_H
+#ifndef X_H
+#define X_H
 
 #include "U3.h"
 //#include "Gate.h"
 #include "matrix.h"
+#define _USE_MATH_DEFINES
 #include <math.h>
 
 
 /**
 @brief A class representing a U3 gate.
 */
-class Z: public U3 {
+class X: public U3 {
 
 
 public:
 
 /**
 @brief NullaRX constructor of the class.
 */
-Z();
+X();
 
 
 /**
 @brief Constructor of the class.
 @param qbit_num_in The number of qubits spanning the gate.
 @param target_qbit_in The 0<=ID<qbit_num of the target qubit.
 @param theta_in logical value indicating whether the matrix creation takes an argument theta.
 @param phi_in logical value indicating whether the matrix creation takes an argument phi
 @param lambda_in logical value indicating whether the matrix creation takes an argument lambda
 */
-Z(int qbit_num_in, int target_qbit_in);
+X(int qbit_num_in, int target_qbit_in);
 
 /**
 @brief Destructor of the class
 */
-~Z();
+~X();
 
 /**
 @brief Call to retrieve the gate matrix
 @param parameters An array of parameters to calculate the matrix of the U3 gate.
 @return Returns with a matrix of the gate
 */
 Matrix get_matrix( );
@@ -83,15 +84,15 @@
 void apply_from_right( Matrix& input );
 
 
 /**
 @brief Call to create a clone of the present class
 @return Return with a pointer pointing to the cloned object
 */
-Z* clone();
+X* clone();
 
 
 /**
 @brief Call to set the number of qubits spanning the matrix of the gate
 @param qbit_num_in The number of qubits
 */
 void set_qbit_num(int qbit_num_in);
@@ -104,9 +105,9 @@
 */
 void reorder_qubits( std::vector<int> qbit_list);
 
 
 };
 
 
-#endif //Z
+#endif //U3
```

### Comparing `squander-1.8.2/gates/kernels/apply_kernel_to_input_AVX.cpp` & `squander-1.8.3/gates/kernels/apply_kernel_to_input_AVX.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 @brief AVX kernel to apply single qubit gate kernel on an input matrix
 @param A matrix on which the householder transformation is applied. (The output is returned via this matrix)
 @param v A matrix instance of the reflection vector
 */
 void
 apply_kernel_to_input_AVX_small(Matrix& u3_1qbit, Matrix& input, const bool& deriv, const int& target_qbit, const int& control_qbit, const int& matrix_size) {
 
+    input.ensure_aligned();
 
     int index_step_target = 1 << target_qbit;
     int current_idx = 0;
 
     // load elements of the U3 unitary into 256bit registers (4 registers)
     __m128d* u3_1qubit_tmp = (__m128d*) & u3_1qbit[0];
     __m256d u3_1qbit_00_vec = _mm256_broadcast_pd(u3_1qubit_tmp);
@@ -72,16 +73,16 @@
 
                 __m256d neg = _mm256_setr_pd(1.0, -1.0, 1.0, -1.0); // 5th register
 
 
                 for (int col_idx = 0; col_idx < 2 * (input.cols - 1); col_idx = col_idx + 4) {
 
                     // extract successive elements from arrays element, element_pair
-                    __m256d element_vec = _mm256_loadu_pd(element + col_idx); // 6th register
-                    __m256d element_pair_vec = _mm256_loadu_pd(element_pair + col_idx); // 7th register
+                    __m256d element_vec = _mm256_load_pd(element + col_idx); // 6th register
+                    __m256d element_pair_vec = _mm256_load_pd(element_pair + col_idx); // 7th register
 
                     //// u3_1qbit_00*element_vec ////
 
                     // 1 calculate the multiplications  u3_1qbit_00*element_vec
                     __m256d vec3 = _mm256_mul_pd(u3_1qbit_00_vec, element_vec); // 8th register
 
                     // 2 Switch the real and imaginary elements of element_vec
@@ -115,15 +116,15 @@
                     vec5 = _mm256_hsub_pd(vec5, vec4);
 
                     //// u3_1qbit_00*element_vec + u3_1qbit_01*element_vec_pair ////
                     vec3 = _mm256_add_pd(vec3, vec5);
 
 
                     // 6 store the transformed elements in vec3
-                    _mm256_storeu_pd(element + col_idx, vec3);
+                    _mm256_store_pd(element + col_idx, vec3);
 
 
                     //// u3_1qbit_10*element_vec ////
 
                     // 1 calculate the multiplications  u3_1qbit_10*element_vec
                     vec3 = _mm256_mul_pd(u3_1qbit_10_vec, element_vec);
 
@@ -145,15 +146,15 @@
                     // 5 Horizontally subtract the elements in vec5 and vec4
                     vec5 = _mm256_hsub_pd(vec5, vec4);
 
                     //// u3_1qbit_10*element_vec + u3_1qbit_11*element_vec_pair ////
                     vec3 = _mm256_add_pd(vec3, vec5);
 
                     // 6 store the transformed elements in vec3
-                    _mm256_storeu_pd(element_pair + col_idx, vec3);
+                    _mm256_store_pd(element_pair + col_idx, vec3);
 
                 }
 
                 if (input.cols % 2 == 1) {
 
                     int col_idx = input.cols - 1;
 
@@ -212,14 +213,15 @@
 /**
 @brief AVX kernel to apply single qubit gate kernel on an input matrix
 @param ???????????????????
 */
 void
 apply_kernel_to_input_AVX(Matrix& u3_1qbit, Matrix& input, const bool& deriv, const int& target_qbit, const int& control_qbit, const int& matrix_size) {
 
+    input.ensure_aligned();
 
     int index_step_target = 1 << target_qbit;
     int current_idx       = 0;
 
     // load elements of the U3 unitary into 256bit registers (8 registers)
     __m256d u3_1bit_00r_vec = _mm256_broadcast_sd(&u3_1qbit[0].real);
     __m256d u3_1bit_00i_vec = _mm256_broadcast_sd(&u3_1qbit[0].imag);
@@ -249,22 +251,22 @@
                         double* element = (double*)input.get_data() + 2 * row_offset;
                         double* element_pair = (double*)input.get_data() + 2 * row_offset_pair;
 
 
                         for (int col_idx = 0; col_idx < 2 * (input.cols - 3); col_idx = col_idx + 8) {
 
                             // extract successive elements from arrays element, element_pair
-                            __m256d element_vec = _mm256_loadu_pd(element + col_idx);
-                            __m256d element_vec2 = _mm256_loadu_pd(element + col_idx + 4);
+                            __m256d element_vec = _mm256_load_pd(element + col_idx);
+                            __m256d element_vec2 = _mm256_load_pd(element + col_idx + 4);
                             __m256d tmp = _mm256_shuffle_pd(element_vec, element_vec2, 0);
                             element_vec2 = _mm256_shuffle_pd(element_vec, element_vec2, 0xf);
                             element_vec = tmp;
 
-                            __m256d element_pair_vec = _mm256_loadu_pd(element_pair + col_idx);
-                            __m256d element_pair_vec2 = _mm256_loadu_pd(element_pair + col_idx + 4);
+                            __m256d element_pair_vec = _mm256_load_pd(element_pair + col_idx);
+                            __m256d element_pair_vec2 = _mm256_load_pd(element_pair + col_idx + 4);
                             tmp = _mm256_shuffle_pd(element_pair_vec, element_pair_vec2, 0);
                             element_pair_vec2 = _mm256_shuffle_pd(element_pair_vec, element_pair_vec2, 0xf);
                             element_pair_vec = tmp;
 
                             __m256d vec3 = _mm256_mul_pd(u3_1bit_00r_vec, element_vec);
                             vec3 = _mm256_fnmadd_pd(u3_1bit_00i_vec, element_vec2, vec3);
                             __m256d vec4 = _mm256_mul_pd(u3_1bit_01r_vec, element_pair_vec);
@@ -276,16 +278,16 @@
                             vec6 = _mm256_fmadd_pd(u3_1bit_01i_vec, element_pair_vec, vec6);
                             vec5 = _mm256_add_pd(vec5, vec6);    
 
                             // 6 store the transformed elements in vec3
                             tmp = _mm256_shuffle_pd(vec3, vec5, 0);
                             vec5 = _mm256_shuffle_pd(vec3, vec5, 0xf);
                             vec3 = tmp;
-                            _mm256_storeu_pd(element + col_idx, vec3);
-                            _mm256_storeu_pd(element + col_idx + 4, vec5);
+                            _mm256_store_pd(element + col_idx, vec3);
+                            _mm256_store_pd(element + col_idx + 4, vec5);
 
                             __m256d vec7 = _mm256_mul_pd(u3_1bit_10r_vec, element_vec);
                             vec7 = _mm256_fnmadd_pd(u3_1bit_10i_vec, element_vec2, vec7);
                             __m256d vec8 = _mm256_mul_pd(u3_1bit_11r_vec, element_pair_vec);
                             vec8 = _mm256_fnmadd_pd(u3_1bit_11i_vec, element_pair_vec2, vec8);
                             vec7 = _mm256_add_pd(vec7, vec8);
                             __m256d vec9 = _mm256_mul_pd(u3_1bit_10r_vec, element_vec2);
@@ -294,16 +296,16 @@
                             vec10 = _mm256_fmadd_pd(u3_1bit_11i_vec, element_pair_vec, vec10);
                             vec9 = _mm256_add_pd(vec9, vec10);
 
                             // 6 store the transformed elements in vec3
                             tmp = _mm256_shuffle_pd(vec7, vec9, 0);
                             vec9 = _mm256_shuffle_pd(vec7, vec9, 0xf);
                             vec7 = tmp;
-                            _mm256_storeu_pd(element_pair + col_idx, vec7);
-                            _mm256_storeu_pd(element_pair + col_idx + 4, vec9);
+                            _mm256_store_pd(element_pair + col_idx, vec7);
+                            _mm256_store_pd(element_pair + col_idx + 4, vec9);
                         }
 
                         int remainder = input.cols % 4;
                         if (remainder != 0) {
 
                             for (int col_idx = input.cols-remainder; col_idx < input.cols; col_idx++) {
                                 int index = row_offset + col_idx;
@@ -341,14 +343,15 @@
 
             //std::cout << current_idx_target << " " << current_idx_target_pair << std::endl;
 
                  
             }
 
 
+
             current_idx = current_idx + (index_step_target << 1);
 
     }
 
 
 
 }
@@ -357,15 +360,16 @@
 /**
 @brief parallel AVX kernel to apply single qubit gate kernel on an input matrix
 @param ???????????????????
 */
 void
 apply_kernel_to_input_AVX_parallel(Matrix& u3_1qbit, Matrix& input, const bool& deriv, const int& target_qbit, const int& control_qbit, const int& matrix_size) {
 
-
+    input.ensure_aligned();
+    
     int index_step_target = 1 << target_qbit;
 
     // load elements of the U3 unitary into 256bit registers (8 registers)
     __m256d u3_1bit_00r_vec = _mm256_broadcast_sd(&u3_1qbit[0].real);
     __m256d u3_1bit_00i_vec = _mm256_broadcast_sd(&u3_1qbit[0].imag);
     __m256d u3_1bit_01r_vec = _mm256_broadcast_sd(&u3_1qbit[1].real);
     __m256d u3_1bit_01i_vec = _mm256_broadcast_sd(&u3_1qbit[1].imag);
@@ -419,22 +423,22 @@
                         double* element = (double*)input.get_data() + 2 * row_offset;
                         double* element_pair = (double*)input.get_data() + 2 * row_offset_pair;
 
 
                         for (int col_idx = 0; col_idx < 2 * (input.cols - 3); col_idx = col_idx + 8) {
 
                             // extract successive elements from arrays element, element_pair
-                            __m256d element_vec = _mm256_loadu_pd(element + col_idx);
-                            __m256d element_vec2 = _mm256_loadu_pd(element + col_idx + 4);
+                            __m256d element_vec = _mm256_load_pd(element + col_idx);
+                            __m256d element_vec2 = _mm256_load_pd(element + col_idx + 4);
                             __m256d tmp = _mm256_shuffle_pd(element_vec, element_vec2, 0);
                             element_vec2 = _mm256_shuffle_pd(element_vec, element_vec2, 0xf);
                             element_vec = tmp;
 
-                            __m256d element_pair_vec = _mm256_loadu_pd(element_pair + col_idx);
-                            __m256d element_pair_vec2 = _mm256_loadu_pd(element_pair + col_idx + 4);
+                            __m256d element_pair_vec = _mm256_load_pd(element_pair + col_idx);
+                            __m256d element_pair_vec2 = _mm256_load_pd(element_pair + col_idx + 4);
                             tmp = _mm256_shuffle_pd(element_pair_vec, element_pair_vec2, 0);
                             element_pair_vec2 = _mm256_shuffle_pd(element_pair_vec, element_pair_vec2, 0xf);
                             element_pair_vec = tmp;
 
                             __m256d vec3 = _mm256_mul_pd(u3_1bit_00r_vec, element_vec);
                             vec3 = _mm256_fnmadd_pd(u3_1bit_00i_vec, element_vec2, vec3);
                             __m256d vec4 = _mm256_mul_pd(u3_1bit_01r_vec, element_pair_vec);
@@ -446,16 +450,16 @@
                             vec6 = _mm256_fmadd_pd(u3_1bit_01i_vec, element_pair_vec, vec6);
                             vec5 = _mm256_add_pd(vec5, vec6);    
 
                             // 6 store the transformed elements in vec3
                             tmp = _mm256_shuffle_pd(vec3, vec5, 0);
                             vec5 = _mm256_shuffle_pd(vec3, vec5, 0xf);
                             vec3 = tmp;
-                            _mm256_storeu_pd(element + col_idx, vec3);
-                            _mm256_storeu_pd(element + col_idx + 4, vec5);
+                            _mm256_store_pd(element + col_idx, vec3);
+                            _mm256_store_pd(element + col_idx + 4, vec5);
 
                             __m256d vec7 = _mm256_mul_pd(u3_1bit_10r_vec, element_vec);
                             vec7 = _mm256_fnmadd_pd(u3_1bit_10i_vec, element_vec2, vec7);
                             __m256d vec8 = _mm256_mul_pd(u3_1bit_11r_vec, element_pair_vec);
                             vec8 = _mm256_fnmadd_pd(u3_1bit_11i_vec, element_pair_vec2, vec8);
                             vec7 = _mm256_add_pd(vec7, vec8);
                             __m256d vec9 = _mm256_mul_pd(u3_1bit_10r_vec, element_vec2);
@@ -464,16 +468,16 @@
                             vec10 = _mm256_fmadd_pd(u3_1bit_11i_vec, element_pair_vec, vec10);
                             vec9 = _mm256_add_pd(vec9, vec10);
 
                             // 6 store the transformed elements in vec3
                             tmp = _mm256_shuffle_pd(vec7, vec9, 0);
                             vec9 = _mm256_shuffle_pd(vec7, vec9, 0xf);
                             vec7 = tmp;
-                            _mm256_storeu_pd(element_pair + col_idx, vec7);
-                            _mm256_storeu_pd(element_pair + col_idx + 4, vec9);
+                            _mm256_store_pd(element_pair + col_idx, vec7);
+                            _mm256_store_pd(element_pair + col_idx + 4, vec9);
                         }
 
                         int remainder = input.cols % 4;
                         if (remainder != 0) {
 
                             for (int col_idx = input.cols-remainder; col_idx < input.cols; col_idx++) {
                                 int index = row_offset + col_idx;
```

### Comparing `squander-1.8.2/gates/kernels/apply_kernel_to_state_vector_input.cpp` & `squander-1.8.3/gates/kernels/apply_kernel_to_state_vector_input.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/gates/kernels/include/apply_kernel_to_input_AVX.h` & `squander-1.8.3/gates/kernels/include/apply_kernel_to_input_AVX.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/gates/kernels/include/apply_kernel_to_state_vector_input.h` & `squander-1.8.3/gates/kernels/include/apply_kernel_to_state_vector_input.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/nn/NN.cpp` & `squander-1.8.3/nn/NN.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     
     //parameters[0:qbit_num*3] = np.random.rand(qbit_num*3)*2*np.pi
     //parameters[2*qbit_num:3*qbit_num] = np.random.rand(qbit_num)*2*np.pi/4
     //parameters[qbit_num:2*qbit_num] = np.random.rand(qbit_num)*2*np.pi/4
     //parameters[3*qbit_num-1] = 0
     //parameters[3*qbit_num-2] = 0
 
-    std::uniform_int_distribution<int8_t> distrib(0, 1);    
+    std::uniform_int_distribution<int16_t> distrib(0, 1);    
     std::uniform_real_distribution<> distrib_real(0.0, 2*M_PI);    
     std::uniform_real_distribution<> distrib_real2(0.0, M_PI);    
 
     
 
 
     for(int idx = 0; idx < 3*qbit_num; idx++) {
```

### Comparing `squander-1.8.2/nn/include/NN.h` & `squander-1.8.3/nn/include/NN.h`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,14 @@
 #include "ON.h"
 #include "Adaptive.h"
 #include "Composite.h"
 #include <map>
 #include <cstdlib>
 #include <time.h>
 #include <ctime>
-#include "gsl/gsl_multimin.h"
-#include "gsl/gsl_statistics.h"
 #include <tbb/cache_aligned_allocator.h>
 
 
 
 
 /**
 @brief A class containing basic methods for the decomposition process.
```

### Comparing `squander-1.8.2/optimization_engines/RL_experience.cpp` & `squander-1.8.3/optimization_engines/RL_experience.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/optimization_engines/include/RL_experience.h` & `squander-1.8.3/optimization_engines/include/RL_experience.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/qgd_python/decomposition/CMakeLists.txt` & `squander-1.8.3/qgd_python/decomposition/CMakeLists.txt`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     ${EXT_DIR}/qgd_N_Qubit_Decomposition_Wrapper.cpp
     ${PROJECT_SOURCE_DIR}/common/numpy_interface.cpp        
 )
 
 
 ADD_DEPENDENCIES (qgd_N_Qubit_Decomposition_Wrapper qgd)
 
-target_link_libraries (qgd_N_Qubit_Decomposition_Wrapper qgd  ${BLAS_LIBRARIES}  ${LAPACKE_LIBRARIES})
+target_link_libraries (qgd_N_Qubit_Decomposition_Wrapper qgd  ${BLAS_LIBRARIES}  ${LAPACKE_LIBRARIES} ${TBB_LIB} ${TBBMALLOC_LIB})
 
 python_extension_module(qgd_N_Qubit_Decomposition_Wrapper)
 
 
 # adding compile options
 target_compile_options(qgd_N_Qubit_Decomposition_Wrapper PRIVATE
     ${CXX_FLAGS}
@@ -53,15 +53,15 @@
     ${EXT_DIR}/qgd_N_Qubit_Decomposition_adaptive_Wrapper.cpp
     ${PROJECT_SOURCE_DIR}/common/numpy_interface.cpp    
 )
 
 
 ADD_DEPENDENCIES (qgd_N_Qubit_Decomposition_adaptive_Wrapper qgd)
 
-target_link_libraries (qgd_N_Qubit_Decomposition_adaptive_Wrapper qgd  ${BLAS_LIBRARIES}  ${LAPACKE_LIBRARIES})
+target_link_libraries (qgd_N_Qubit_Decomposition_adaptive_Wrapper qgd  ${BLAS_LIBRARIES}  ${LAPACKE_LIBRARIES} ${TBB_LIB} ${TBBMALLOC_LIB})
 
 python_extension_module(qgd_N_Qubit_Decomposition_adaptive_Wrapper)
 
 
 # adding compile options
 target_compile_options(qgd_N_Qubit_Decomposition_adaptive_Wrapper PRIVATE
     ${CXX_FLAGS}
@@ -101,15 +101,15 @@
     ${EXT_DIR}/qgd_N_Qubit_Decomposition_custom_Wrapper.cpp
     ${PROJECT_SOURCE_DIR}/common/numpy_interface.cpp        
 )
 
 
 ADD_DEPENDENCIES (qgd_N_Qubit_Decomposition_custom_Wrapper qgd)
 
-target_link_libraries (qgd_N_Qubit_Decomposition_custom_Wrapper qgd  ${BLAS_LIBRARIES}  ${LAPACKE_LIBRARIES})
+target_link_libraries (qgd_N_Qubit_Decomposition_custom_Wrapper qgd  ${BLAS_LIBRARIES}  ${LAPACKE_LIBRARIES}   ${TBB_LIB} ${TBBMALLOC_LIB})
 
 python_extension_module(qgd_N_Qubit_Decomposition_custom_Wrapper)
 
 
 # adding compile options
 target_compile_options(qgd_N_Qubit_Decomposition_custom_Wrapper PRIVATE
     ${CXX_FLAGS}
```

### Comparing `squander-1.8.2/qgd_python/decomposition/qgd_N_Qubit_Decomposition.py` & `squander-1.8.3/qgd_python/decomposition/qgd_N_Qubit_Decomposition.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/qgd_python/decomposition/qgd_N_Qubit_Decomposition_Wrapper.cpp` & `squander-1.8.3/qgd_python/decomposition/qgd_N_Qubit_Decomposition_Wrapper.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -175,21 +175,21 @@
 
     // determine the initial guess type
     PyObject* initial_guess_string = PyObject_Str(initial_guess);
     PyObject* initial_guess_string_unicode = PyUnicode_AsEncodedString(initial_guess_string, "utf-8", "~E~");
     const char* initial_guess_C = PyBytes_AS_STRING(initial_guess_string_unicode);
 
     guess_type qgd_initial_guess;
-    if ( strcmp("zeros", initial_guess_C) == 0 or strcmp("ZEROS", initial_guess_C) == 0) {
+    if ( strcmp("zeros", initial_guess_C) == 0 || strcmp("ZEROS", initial_guess_C) == 0) {
         qgd_initial_guess = ZEROS;        
     }
-    else if ( strcmp("random", initial_guess_C)==0 or strcmp("RANDOM", initial_guess_C)==0) {
+    else if ( strcmp("random", initial_guess_C)==0 || strcmp("RANDOM", initial_guess_C)==0) {
         qgd_initial_guess = RANDOM;        
     }
-    else if ( strcmp("close_to_zero", initial_guess_C)==0 or strcmp("CLOSE_TO_ZERO", initial_guess_C)==0) {
+    else if ( strcmp("close_to_zero", initial_guess_C)==0 || strcmp("CLOSE_TO_ZERO", initial_guess_C)==0) {
         qgd_initial_guess = CLOSE_TO_ZERO;        
     }
     else {
         std::cout << "Wrong initial guess format. Using default ZEROS." << std::endl; 
         qgd_initial_guess = ZEROS;     
     }
 
@@ -1101,17 +1101,17 @@
 };
 
 /**
 @brief Structure containing metadata about the module.
 */
 static PyModuleDef qgd_N_Qubit_Decomposition_Wrapper_Module = {
     PyModuleDef_HEAD_INIT,
-    .m_name = "qgd_N_Qubit_Decomposition_Wrapper",
-    .m_doc = "Python binding for QGD N_Qubit_Decomposition class",
-    .m_size = -1,
+    "qgd_N_Qubit_Decomposition_Wrapper",
+    "Python binding for QGD N_Qubit_Decomposition class",
+    -1,
 };
 
 
 /**
 @brief Method called when the Python module is initialized
 */
 PyMODINIT_FUNC
```

### Comparing `squander-1.8.2/qgd_python/decomposition/qgd_N_Qubit_Decomposition_adaptive.py` & `squander-1.8.3/qgd_python/decomposition/qgd_N_Qubit_Decomposition_adaptive.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/qgd_python/decomposition/qgd_N_Qubit_Decomposition_adaptive_Wrapper.cpp` & `squander-1.8.3/qgd_python/decomposition/qgd_N_Qubit_Decomposition_adaptive_Wrapper.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -993,15 +993,15 @@
 @param self A pointer pointing to an instance of the class qgd_N_Qubit_Decomposition_adaptive_Wrapper.
 @param args  (int) number of max iters.
 */
 static PyObject *
 qgd_N_Qubit_Decomposition_adaptive_Wrapper_set_Max_Iterations(qgd_N_Qubit_Decomposition_adaptive_Wrapper *self, PyObject *args ) {
 
     // initiate variables for input arguments
-    PyObject* max_iters_input; 
+    int max_iters_input; 
 
     // parsing input arguments
     if (!PyArg_ParseTuple(args, "|i", &max_iters_input )) return Py_BuildValue("i", -1);
 
 
     //set the maximum number of iterations
     self->decomp->set_max_inner_iterations(max_iters_input);
@@ -1542,15 +1542,15 @@
     }
 
 
     Matrix_real parameters_mtx = numpy2matrix_real( parameters_arg );
     Matrix_real grad_mtx(parameters_mtx.size(), 1);
 
     try {
-        self->decomp->optimization_problem_grad(parameters_mtx, &self->decomp, grad_mtx );
+        self->decomp->optimization_problem_grad(parameters_mtx, self->decomp, grad_mtx );
     }
     catch (std::string err ) {
         PyErr_SetString(PyExc_Exception, err.c_str());
         return NULL;
     }
     catch (...) {
         std::string err( "Invalid pointer to decomposition class");
@@ -1561,15 +1561,14 @@
     // convert to numpy array
     grad_mtx.set_owner(false);
     PyObject *grad_py = matrix_real_to_numpy( grad_mtx );
 
     Py_DECREF(parameters_arg);
 
 
-    Py_DECREF(grad_py);
     return grad_py;
 }
 
 /**
 @brief Wrapper function to evaluate the cost function an dthe gradient components.
 @return Unitarty numpy matrix
 */
@@ -1993,30 +1992,33 @@
    
 
     PyObject* optimizer_string = PyObject_Str(optimizer_arg);
     PyObject* optimizer_string_unicode = PyUnicode_AsEncodedString(optimizer_string, "utf-8", "~E~");
     const char* optimizer_C = PyBytes_AS_STRING(optimizer_string_unicode);
 
     optimization_aglorithms qgd_optimizer;
-    if ( strcmp("bfgs", optimizer_C) == 0 or strcmp("BFGS", optimizer_C) == 0) {
+    if ( strcmp("bfgs", optimizer_C) == 0 || strcmp("BFGS", optimizer_C) == 0) {
         qgd_optimizer = BFGS;        
     }
-    else if ( strcmp("adam", optimizer_C)==0 or strcmp("ADAM", optimizer_C)==0) {
+    else if ( strcmp("adam", optimizer_C)==0 || strcmp("ADAM", optimizer_C)==0) {
         qgd_optimizer = ADAM;        
     }
-    else if ( strcmp("adam_batched", optimizer_C)==0 or strcmp("ADAM_BATCHED", optimizer_C)==0) {
+    else if ( strcmp("adam_batched", optimizer_C)==0 || strcmp("ADAM_BATCHED", optimizer_C)==0) {
         qgd_optimizer = ADAM_BATCHED;        
     }
-    else if ( strcmp("bfgs2", optimizer_C)==0 or strcmp("BFGS2", optimizer_C)==0) {
+    else if ( strcmp("bfgs2", optimizer_C)==0 || strcmp("BFGS2", optimizer_C)==0) {
         qgd_optimizer = BFGS2;        
     }
-    else if ( strcmp("agents", optimizer_C)==0 or strcmp("AGENTS", optimizer_C)==0) {
+    else if ( strcmp("agents", optimizer_C)==0 || strcmp("AGENTS", optimizer_C)==0) {
         qgd_optimizer = AGENTS;        
     }
-    else if ( strcmp("agents_combined", optimizer_C)==0 or strcmp("AGENTS_COMBINED", optimizer_C)==0) {
+    else if ( strcmp("cosine", optimizer_C)==0 || strcmp("COSINE", optimizer_C)==0) {
+        qgd_optimizer = COSINE;        
+    }
+    else if ( strcmp("agents_combined", optimizer_C)==0 || strcmp("AGENTS_COMBINED", optimizer_C)==0) {
         qgd_optimizer = AGENTS_COMBINED;        
     }
     else {
         std::cout << "Wrong optimizer. Using default: BFGS" << std::endl; 
         qgd_optimizer = BFGS;     
     }
 
@@ -2062,15 +2064,15 @@
 
         std::string err( "Unsuccessful argument parsing");
         PyErr_SetString(PyExc_Exception, err.c_str());
         return NULL;       
  
     }
    
-    cost_function_type qgd_costfnc = costfnc_arg;
+    cost_function_type qgd_costfnc = (cost_function_type)costfnc_arg;
 
 
     try {
         self->decomp->set_cost_function_variant(qgd_costfnc);
     }
     catch (std::string err) {
         PyErr_SetString(PyExc_Exception, err.c_str());
@@ -2509,17 +2511,17 @@
 };
 
 /**
 @brief Structure containing metadata about the module.
 */
 static PyModuleDef qgd_N_Qubit_Decomposition_adaptive_Wrapper_Module = {
     PyModuleDef_HEAD_INIT,
-    .m_name = "qgd_N_Qubit_Decomposition_adaptive_Wrapper",
-    .m_doc = "Python binding for QGD N_Qubit_Decomposition class",
-    .m_size = -1,
+    "qgd_N_Qubit_Decomposition_adaptive_Wrapper",
+    "Python binding for QGD N_Qubit_Decomposition class",
+    -1,
 };
 
 
 /**
 @brief Method called when the Python module is initialized
 */
 PyMODINIT_FUNC
```

### Comparing `squander-1.8.2/qgd_python/decomposition/qgd_N_Qubit_Decomposition_custom.py` & `squander-1.8.3/qgd_python/decomposition/qgd_N_Qubit_Decomposition_custom.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/qgd_python/decomposition/qgd_N_Qubit_Decomposition_custom_Wrapper.cpp` & `squander-1.8.3/qgd_python/decomposition/qgd_N_Qubit_Decomposition_custom_Wrapper.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -174,21 +174,21 @@
 
     // determine the initial guess type
     PyObject* initial_guess_string = PyObject_Str(initial_guess);
     PyObject* initial_guess_string_unicode = PyUnicode_AsEncodedString(initial_guess_string, "utf-8", "~E~");
     const char* initial_guess_C = PyBytes_AS_STRING(initial_guess_string_unicode);
 
     guess_type qgd_initial_guess;
-    if ( strcmp("zeros", initial_guess_C) == 0 or strcmp("ZEROS", initial_guess_C) == 0) {
+    if ( strcmp("zeros", initial_guess_C) == 0 || strcmp("ZEROS", initial_guess_C) == 0) {
         qgd_initial_guess = ZEROS;        
     }
-    else if ( strcmp("random", initial_guess_C)==0 or strcmp("RANDOM", initial_guess_C)==0) {
+    else if ( strcmp("random", initial_guess_C)==0 || strcmp("RANDOM", initial_guess_C)==0) {
         qgd_initial_guess = RANDOM;        
     }
-    else if ( strcmp("close_to_zero", initial_guess_C)==0 or strcmp("CLOSE_TO_ZERO", initial_guess_C)==0) {
+    else if ( strcmp("close_to_zero", initial_guess_C)==0 || strcmp("CLOSE_TO_ZERO", initial_guess_C)==0) {
         qgd_initial_guess = CLOSE_TO_ZERO;        
     }
     else {
         std::cout << "Wrong initial guess format. Using default ZEROS." << std::endl; 
         qgd_initial_guess = ZEROS;     
     }
 
@@ -996,33 +996,33 @@
    
 
     PyObject* optimizer_string = PyObject_Str(optimizer_arg);
     PyObject* optimizer_string_unicode = PyUnicode_AsEncodedString(optimizer_string, "utf-8", "~E~");
     const char* optimizer_C = PyBytes_AS_STRING(optimizer_string_unicode);
 
     optimization_aglorithms qgd_optimizer;
-    if ( strcmp("bfgs", optimizer_C) == 0 or strcmp("BFGS", optimizer_C) == 0) {
+    if ( strcmp("bfgs", optimizer_C) == 0 || strcmp("BFGS", optimizer_C) == 0) {
         qgd_optimizer = BFGS;        
     }
-    else if ( strcmp("adam", optimizer_C)==0 or strcmp("ADAM", optimizer_C)==0) {
+    else if ( strcmp("adam", optimizer_C)==0 || strcmp("ADAM", optimizer_C)==0) {
         qgd_optimizer = ADAM;        
     }
-    else if ( strcmp("adam_batched", optimizer_C)==0 or strcmp("ADAM_BATCHED", optimizer_C)==0) {
+    else if ( strcmp("adam_batched", optimizer_C)==0 || strcmp("ADAM_BATCHED", optimizer_C)==0) {
         qgd_optimizer = ADAM_BATCHED;        
     }
-    else if ( strcmp("agents", optimizer_C)==0 or strcmp("AGENTS", optimizer_C)==0) {
+    else if ( strcmp("agents", optimizer_C)==0 || strcmp("AGENTS", optimizer_C)==0) {
         qgd_optimizer = AGENTS;        
     }
-    else if ( strcmp("cosine", optimizer_C)==0 or strcmp("COSINE", optimizer_C)==0) {
+    else if ( strcmp("cosine", optimizer_C)==0 || strcmp("COSINE", optimizer_C)==0) {
         qgd_optimizer = COSINE;        
     }
-    else if ( strcmp("agents_combined", optimizer_C)==0 or strcmp("AGENTS_COMBINED", optimizer_C)==0) {
+    else if ( strcmp("agents_combined", optimizer_C)==0 || strcmp("AGENTS_COMBINED", optimizer_C)==0) {
         qgd_optimizer = AGENTS_COMBINED;        
     }
-    else if ( strcmp("bfgs2", optimizer_C)==0 or strcmp("BFGS2", optimizer_C)==0) {
+    else if ( strcmp("bfgs2", optimizer_C)==0 || strcmp("BFGS2", optimizer_C)==0) {
         qgd_optimizer = BFGS2;        
     }
     else {
         std::cout << "Wrong optimizer. Using default: BFGS" << std::endl; 
         qgd_optimizer = BFGS;     
     }
 
@@ -1218,17 +1218,17 @@
 };
 
 /**
 @brief Structure containing metadata about the module.
 */
 static PyModuleDef qgd_N_Qubit_Decomposition_custom_Wrapper_Module = {
     PyModuleDef_HEAD_INIT,
-    .m_name = "qgd_N_Qubit_Decomposition_custom_Wrapper",
-    .m_doc = "Python binding for QGD N_Qubit_Decomposition class",
-    .m_size = -1,
+    "qgd_N_Qubit_Decomposition_custom_Wrapper",
+    "Python binding for QGD N_Qubit_Decomposition class",
+    -1,
 };
 
 
 /**
 @brief Method called when the Python module is initialized
 */
 PyMODINIT_FUNC
```

### Comparing `squander-1.8.2/qgd_python/decomposition/qgd_N_Qubit_State_Preparation_adaptive.py` & `squander-1.8.3/qgd_python/decomposition/qgd_N_Qubit_State_Preparation_adaptive.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/qgd_python/decomposition/test/test_Compression.py` & `squander-1.8.3/qgd_python/decomposition/test/test_Compression.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/qgd_python/decomposition/test/test_Global_Phase.py` & `squander-1.8.3/qgd_python/decomposition/test/test_Global_Phase.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/qgd_python/decomposition/test/test_IBM.py` & `squander-1.8.3/qgd_python/decomposition/test/test_IBM.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/qgd_python/decomposition/test/test_Project_Name.py` & `squander-1.8.3/qgd_python/decomposition/test/test_Project_Name.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/qgd_python/decomposition/test/test_QX2.py` & `squander-1.8.3/qgd_python/decomposition/test/test_QX2.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/qgd_python/decomposition/test/test_State_Preparation.py` & `squander-1.8.3/qgd_python/decomposition/test/test_State_Preparation.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/qgd_python/decomposition/test/test_Unitary.py` & `squander-1.8.3/qgd_python/decomposition/test/test_Unitary.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/qgd_python/decomposition/test/test_decomposition.py` & `squander-1.8.3/qgd_python/decomposition/test/test_decomposition.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/qgd_python/decomposition/test/test_fmo.py` & `squander-1.8.3/qgd_python/decomposition/test/test_fmo.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/qgd_python/decomposition/test/test_heavy_hex.py` & `squander-1.8.3/qgd_python/decomposition/test/test_heavy_hex.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/qgd_python/decomposition/test/test_optmization_problem_combined.py` & `squander-1.8.3/qgd_python/decomposition/test/test_optmization_problem_combined.py`

 * *Files 11% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     MPI_imported = False
 
 
 np.set_printoptions(linewidth=200) 
 
 
 # number of qubits
-qbit_num = 9
+qbit_num = 8
 
 # cost function variant
 cost_function_variant = 0
 
 
 # matrix size of the unitary
 matrix_size = 1 << qbit_num #pow(2, qbit_num )
@@ -146,15 +146,15 @@
 
 
         Umtx = cDecompose_createUmtx.get_Matrix( parameters )
 
 
         # cut the matrixt by trace offset
         trace_offset = 80
-        Umtx = Umtx[trace_offset:400, :]
+        Umtx = Umtx[trace_offset:240, :]
 
 
 	###################################################################################
 
 	# test cost function with trace offset 
 
 
@@ -174,13 +174,48 @@
         # setting the cost function variant
         cDecompose_CPU.set_Cost_Function_Variant(cost_function_variant)
 
         t0 = time.time()
         f0_CPU, grad_CPU = cDecompose_CPU.Optimization_Problem_Combined( parameters )
 
         assert( np.abs( f0_CPU ) < 1e-8 )
+        
+        
+        
+
+    def test_grad_batch_unitary_funcs(self):
+        # creating a class to decompose the unitary
+        cDecompose = N_Qubit_Decomposition_adaptive( np.eye(matrix_size, dtype=np.complex128), level_limit_max=5, level_limit_min=0, accelerator_num=0 )
+
+
+        # adding decomposing layers to the gat structure
+        for idx in range(levels):
+            cDecompose.add_Adaptive_Layers()
+
+        cDecompose.add_Finalyzing_Layer_To_Gate_Structure()
+
+
+        # get the number of free parameters
+        num_of_parameters = cDecompose.get_Parameter_Num()
+
+
+        # create randomized parameters
+        parameters, nontrivial_adaptive_layers = create_randomized_parameters( num_of_parameters, real=real )
+
+
+
+        Umtx = cDecompose.get_Matrix( parameters )
+        mat, mat_deriv = cDecompose.Optimization_Problem_Combined_Unitary(parameters)
+        assert np.allclose(Umtx, mat)
+        
+        cost = cDecompose.Optimization_Problem(parameters)
+        assert np.allclose(np.array([cost, cost, cost]), cDecompose.Optimization_Problem_Batch(np.vstack([parameters, parameters, parameters])))
+        grad = cDecompose.Optimization_Problem_Grad(parameters)        
+        f0_CPU, grad_CPU = cDecompose.Optimization_Problem_Combined( parameters )
+        assert np.allclose(grad, grad_CPU)
+        assert np.isclose(f0_CPU, cost)
```

### Comparing `squander-1.8.2/qgd_python/decomposition/test/test_parametric_circuit.py` & `squander-1.8.3/qgd_python/decomposition/test/test_parametric_circuit.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/qgd_python/gates/CMakeLists.txt` & `squander-1.8.3/qgd_python/gates/CMakeLists.txt`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     ${EXT_DIR}/qgd_U3.cpp
     ${PROJECT_SOURCE_DIR}/common/numpy_interface.cpp
 )
 
 
 ADD_DEPENDENCIES (qgd_U3 qgd)
 
-target_link_libraries (qgd_U3 qgd ${BLAS_LIBRARIES})
+target_link_libraries (qgd_U3 qgd ${BLAS_LIBRARIES} ${TBB_LIB} ${TBBMALLOC_LIB})
 
 python_extension_module(qgd_U3)
 
 # adding compile options
 target_compile_options(qgd_U3 PRIVATE
     ${CXX_FLAGS}
     "$<$<CONFIG:Debug>:${CXX_FLAGS_DEBUG}>"
@@ -47,15 +47,15 @@
     ${EXT_DIR}/qgd_CNOT.cpp
     ${PROJECT_SOURCE_DIR}/common/numpy_interface.cpp
 )
 
 
 ADD_DEPENDENCIES (qgd_CNOT qgd)
 
-target_link_libraries (qgd_CNOT qgd ${BLAS_LIBRARIES})
+target_link_libraries (qgd_CNOT qgd ${BLAS_LIBRARIES} ${TBB_LIB} ${TBBMALLOC_LIB})
 
 python_extension_module(qgd_CNOT)
 
 
 # adding compile options
 target_compile_options(qgd_CNOT PRIVATE
     ${CXX_FLAGS}
@@ -89,15 +89,15 @@
     ${EXT_DIR}/qgd_CZ.cpp
     ${PROJECT_SOURCE_DIR}/common/numpy_interface.cpp
 )
 
 
 ADD_DEPENDENCIES (qgd_CZ qgd)
 
-target_link_libraries (qgd_CZ qgd ${BLAS_LIBRARIES})
+target_link_libraries (qgd_CZ qgd ${BLAS_LIBRARIES} ${TBB_LIB} ${TBBMALLOC_LIB})
 
 python_extension_module(qgd_CZ)
 
 
 # adding compile options
 target_compile_options(qgd_CZ PRIVATE
     ${CXX_FLAGS}
@@ -133,15 +133,15 @@
     ${EXT_DIR}/qgd_CH.cpp
     ${PROJECT_SOURCE_DIR}/common/numpy_interface.cpp
 )
 
 
 ADD_DEPENDENCIES (qgd_CH qgd)
 
-target_link_libraries (qgd_CH qgd ${BLAS_LIBRARIES})
+target_link_libraries (qgd_CH qgd ${BLAS_LIBRARIES} ${TBB_LIB} ${TBBMALLOC_LIB})
 
 python_extension_module(qgd_CH)
 
 
 # adding compile options
 target_compile_options(qgd_CH PRIVATE
     ${CXX_FLAGS}
@@ -175,15 +175,15 @@
     ${EXT_DIR}/qgd_Gates_Block.cpp
     ${PROJECT_SOURCE_DIR}/common/numpy_interface.cpp
 )
 
 
 ADD_DEPENDENCIES (qgd_Gates_Block qgd)
 
-target_link_libraries (qgd_Gates_Block qgd ${BLAS_LIBRARIES})
+target_link_libraries (qgd_Gates_Block qgd ${BLAS_LIBRARIES} ${TBB_LIB} ${TBBMALLOC_LIB})
 
 
 python_extension_module(qgd_Gates_Block)
 
 # adding compile options
 target_compile_options(qgd_Gates_Block PRIVATE
     ${CXX_FLAGS}
@@ -221,15 +221,15 @@
     ${EXT_DIR}/qgd_SYC.cpp
     ${PROJECT_SOURCE_DIR}/common/numpy_interface.cpp
 )
 
 
 ADD_DEPENDENCIES (qgd_SYC qgd)
 
-target_link_libraries (qgd_SYC qgd ${BLAS_LIBRARIES})
+target_link_libraries (qgd_SYC qgd ${BLAS_LIBRARIES} ${TBB_LIB} ${TBBMALLOC_LIB})
 
 
 python_extension_module(qgd_SYC)
 
 # adding compile options
 target_compile_options(qgd_SYC PRIVATE
     ${CXX_FLAGS}
@@ -267,15 +267,15 @@
     ${EXT_DIR}/qgd_RY.cpp
     ${PROJECT_SOURCE_DIR}/common/numpy_interface.cpp
 )
 
 
 ADD_DEPENDENCIES (qgd_RY qgd)
 
-target_link_libraries (qgd_RY qgd ${BLAS_LIBRARIES})
+target_link_libraries (qgd_RY qgd ${BLAS_LIBRARIES} ${TBB_LIB} ${TBBMALLOC_LIB})
 
 
 python_extension_module(qgd_RY)
 
 # adding compile options
 target_compile_options(qgd_RY PRIVATE
     ${CXX_FLAGS}
@@ -314,15 +314,15 @@
     ${EXT_DIR}/qgd_RZ.cpp
     ${PROJECT_SOURCE_DIR}/common/numpy_interface.cpp
 )
 
 
 ADD_DEPENDENCIES (qgd_RZ qgd)
 
-target_link_libraries (qgd_RZ qgd ${BLAS_LIBRARIES})
+target_link_libraries (qgd_RZ qgd ${BLAS_LIBRARIES} ${TBB_LIB} ${TBBMALLOC_LIB})
 
 
 python_extension_module(qgd_RZ)
 
 # adding compile options
 target_compile_options(qgd_RZ PRIVATE
     ${CXX_FLAGS}
@@ -361,15 +361,15 @@
     ${EXT_DIR}/qgd_RX.cpp
     ${PROJECT_SOURCE_DIR}/common/numpy_interface.cpp
 )
 
 
 ADD_DEPENDENCIES (qgd_RX qgd)
 
-target_link_libraries (qgd_RX qgd ${BLAS_LIBRARIES})
+target_link_libraries (qgd_RX qgd ${BLAS_LIBRARIES} ${TBB_LIB} ${TBBMALLOC_LIB})
 
 
 python_extension_module(qgd_RX)
 
 # adding compile options
 target_compile_options(qgd_RX PRIVATE
     ${CXX_FLAGS}
@@ -408,15 +408,15 @@
     ${EXT_DIR}/qgd_X.cpp
     ${PROJECT_SOURCE_DIR}/common/numpy_interface.cpp
 )
 
 
 ADD_DEPENDENCIES (qgd_X qgd)
 
-target_link_libraries (qgd_X qgd ${BLAS_LIBRARIES})
+target_link_libraries (qgd_X qgd ${BLAS_LIBRARIES} ${TBB_LIB} ${TBBMALLOC_LIB})
 
 
 python_extension_module(qgd_X)
 
 # adding compile options
 target_compile_options(qgd_X PRIVATE
     ${CXX_FLAGS}
@@ -455,15 +455,15 @@
     ${EXT_DIR}/qgd_Y.cpp
     ${PROJECT_SOURCE_DIR}/common/numpy_interface.cpp
 )
 
 
 ADD_DEPENDENCIES (qgd_Y qgd)
 
-target_link_libraries (qgd_Y qgd ${BLAS_LIBRARIES})
+target_link_libraries (qgd_Y qgd ${BLAS_LIBRARIES} ${TBB_LIB} ${TBBMALLOC_LIB})
 
 
 python_extension_module(qgd_Y)
 
 # adding compile options
 target_compile_options(qgd_Y PRIVATE
     ${CXX_FLAGS}
@@ -501,15 +501,15 @@
     ${EXT_DIR}/qgd_Z.cpp
     ${PROJECT_SOURCE_DIR}/common/numpy_interface.cpp
 )
 
 
 ADD_DEPENDENCIES (qgd_Z qgd)
 
-target_link_libraries (qgd_Z qgd ${BLAS_LIBRARIES})
+target_link_libraries (qgd_Z qgd ${BLAS_LIBRARIES} ${TBB_LIB} ${TBBMALLOC_LIB})
 
 
 python_extension_module(qgd_Z)
 
 # adding compile options
 target_compile_options(qgd_Z PRIVATE
     ${CXX_FLAGS}
@@ -548,15 +548,15 @@
     ${EXT_DIR}/qgd_SX.cpp
     ${PROJECT_SOURCE_DIR}/common/numpy_interface.cpp
 )
 
 
 ADD_DEPENDENCIES (qgd_SX qgd)
 
-target_link_libraries (qgd_SX qgd ${BLAS_LIBRARIES})
+target_link_libraries (qgd_SX qgd ${BLAS_LIBRARIES} ${TBB_LIB} ${TBBMALLOC_LIB})
 
 
 python_extension_module(qgd_SX)
 
 # adding compile options
 target_compile_options(qgd_SX PRIVATE
     ${CXX_FLAGS}
```

### Comparing `squander-1.8.2/qgd_python/gates/qgd_CH.cpp` & `squander-1.8.3/qgd_python/gates/qgd_CH.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -186,14 +186,18 @@
 
 
     // create QGD version of the input matrix
     Matrix unitary_mtx = numpy2matrix(unitary);
 
     self->gate->apply_to( unitary_mtx );
     
+    if (unitary_mtx.data != PyArray_DATA(unitary)) {
+        memcpy(PyArray_DATA(unitary), unitary_mtx.data, unitary_mtx.size() * sizeof(QGD_Complex16));
+    }
+    
     Py_DECREF(unitary);
 
     return Py_BuildValue("i", 0);
 }
 
 
 
@@ -301,17 +305,17 @@
 
 
 /**
 @brief Structure containing metadata about the module.
 */
 static PyModuleDef  qgd_CH_Module = {
     PyModuleDef_HEAD_INIT,
-    .m_name = "qgd_CH",
-    .m_doc = "Python binding for QGD CH gate",
-    .m_size = -1,
+    "qgd_CH",
+    "Python binding for QGD CH gate",
+    -1,
 };
 
 
 /**
 @brief Method called when the Python module is initialized
 */
 PyMODINIT_FUNC
```

### Comparing `squander-1.8.2/qgd_python/gates/qgd_CNOT.cpp` & `squander-1.8.3/qgd_python/gates/qgd_CNOT.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -183,14 +183,18 @@
     }
 
 
     // create QGD version of the input matrix
     Matrix unitary_mtx = numpy2matrix(unitary);
 
     self->gate->apply_to( unitary_mtx );
+
+    if (unitary_mtx.data != PyArray_DATA(unitary)) {
+        memcpy(PyArray_DATA(unitary), unitary_mtx.data, unitary_mtx.size() * sizeof(QGD_Complex16));
+    }
     
     Py_DECREF(unitary);
 
     return Py_BuildValue("i", 0);
 }
 
 
@@ -292,17 +296,17 @@
 
 
 /**
 @brief Structure containing metadata about the module.
 */
 static PyModuleDef  qgd_CNOT_Module = {
     PyModuleDef_HEAD_INIT,
-    .m_name = "qgd_CNOT",
-    .m_doc = "Python binding for QGD CNOT gate",
-    .m_size = -1,
+    "qgd_CNOT",
+    "Python binding for QGD CNOT gate",
+    -1,
 };
 
 
 /**
 @brief Method called when the Python module is initialized
 */
 PyMODINIT_FUNC
```

### Comparing `squander-1.8.2/qgd_python/gates/qgd_CZ.cpp` & `squander-1.8.3/qgd_python/gates/qgd_CZ.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -185,14 +185,18 @@
 
 
     // create QGD version of the input matrix
     Matrix unitary_mtx = numpy2matrix(unitary);
 
     self->gate->apply_to( unitary_mtx );
     
+    if (unitary_mtx.data != PyArray_DATA(unitary)) {
+        memcpy(PyArray_DATA(unitary), unitary_mtx.data, unitary_mtx.size() * sizeof(QGD_Complex16));
+    }
+
     Py_DECREF(unitary);
 
     return Py_BuildValue("i", 0);
 }
 
 
 
@@ -293,17 +297,17 @@
 
 
 /**
 @brief Structure containing metadata about the module.
 */
 static PyModuleDef  qgd_CZ_Module = {
     PyModuleDef_HEAD_INIT,
-    .m_name = "qgd_CZ",
-    .m_doc = "Python binding for QGD CZ gate",
-    .m_size = -1,
+    "qgd_CZ",
+    "Python binding for QGD CZ gate",
+    -1,
 };
 
 
 /**
 @brief Method called when the Python module is initialized
 */
 PyMODINIT_FUNC
```

### Comparing `squander-1.8.2/qgd_python/gates/qgd_Gates_Block.cpp` & `squander-1.8.3/qgd_python/gates/qgd_Gates_Block.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -757,14 +757,18 @@
 
     // create QGD version of the input matrix
     Matrix unitary_mtx = numpy2matrix(unitary);
 
 
     self->gate->apply_to( parameters_mtx, unitary_mtx );
     
+    if (unitary_mtx.data != PyArray_DATA(unitary)) {
+        memcpy(PyArray_DATA(unitary), unitary_mtx.data, unitary_mtx.size() * sizeof(QGD_Complex16));
+    }
+
     Py_DECREF(parameters_arr);
     Py_DECREF(unitary);
 
     return Py_BuildValue("i", 0);
 }
 
 
@@ -908,17 +912,17 @@
 };
 
 /**
 @brief Structure containing metadata about the module.
 */
 static PyModuleDef qgd_Gates_Block_Module = {
     PyModuleDef_HEAD_INIT,
-    .m_name = "qgd_Gates_Block",
-    .m_doc = "Python binding for QGD Gates_block class",
-    .m_size = -1,
+    "qgd_Gates_Block",
+    "Python binding for QGD Gates_block class",
+    -1,
 };
 
 /**
 @brief Method called when the Python module is initialized
 */
 PyMODINIT_FUNC
 PyInit_qgd_Gates_Block(void)
```

### Comparing `squander-1.8.2/qgd_python/gates/qgd_RX.cpp` & `squander-1.8.3/qgd_python/gates/qgd_RX.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -210,14 +210,18 @@
     }
 
     // create QGD version of the input matrix
     Matrix unitary_mtx = numpy2matrix(unitary);
 
     self->gate->apply_to( parameters_mtx, unitary_mtx );
     
+    if (unitary_mtx.data != PyArray_DATA(unitary)) {
+        memcpy(PyArray_DATA(unitary), unitary_mtx.data, unitary_mtx.size() * sizeof(QGD_Complex16));
+    }
+
     Py_DECREF(parameters_arr);
     Py_DECREF(unitary);
 
     return Py_BuildValue("i", 0);
 }
 
 
@@ -318,17 +322,17 @@
 
 
 /**
 @brief Structure containing metadata about the module.
 */
 static PyModuleDef  qgd_RX_Module = {
     PyModuleDef_HEAD_INIT,
-    .m_name = "qgd_RX",
-    .m_doc = "Python binding for QGD RX gate",
-    .m_size = -1,
+    "qgd_RX",
+    "Python binding for QGD RX gate",
+    -1,
 };
 
 
 /**
 @brief Method called when the Python module is initialized
 */
 PyMODINIT_FUNC
```

### Comparing `squander-1.8.2/qgd_python/gates/qgd_RY.cpp` & `squander-1.8.3/qgd_python/gates/qgd_RY.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -210,14 +210,18 @@
     }
 
     // create QGD version of the input matrix
     Matrix unitary_mtx = numpy2matrix(unitary);
 
     self->gate->apply_to( parameters_mtx, unitary_mtx );
     
+    if (unitary_mtx.data != PyArray_DATA(unitary)) {
+        memcpy(PyArray_DATA(unitary), unitary_mtx.data, unitary_mtx.size() * sizeof(QGD_Complex16));
+    }
+
     Py_DECREF(parameters_arr);
     Py_DECREF(unitary);
 
     return Py_BuildValue("i", 0);
 }
 
 
@@ -318,17 +322,17 @@
 
 
 /**
 @brief Structure containing metadata about the module.
 */
 static PyModuleDef  qgd_RY_Module = {
     PyModuleDef_HEAD_INIT,
-    .m_name = "qgd_RY",
-    .m_doc = "Python binding for QGD RY gate",
-    .m_size = -1,
+    "qgd_RY",
+    "Python binding for QGD RY gate",
+    -1,
 };
 
 
 /**
 @brief Method called when the Python module is initialized
 */
 PyMODINIT_FUNC
```

### Comparing `squander-1.8.2/qgd_python/gates/qgd_RZ.cpp` & `squander-1.8.3/qgd_python/gates/qgd_RZ.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -209,14 +209,18 @@
     }
 
     // create QGD version of the input matrix
     Matrix unitary_mtx = numpy2matrix(unitary);
 
     self->gate->apply_to( parameters_mtx, unitary_mtx );
     
+    if (unitary_mtx.data != PyArray_DATA(unitary)) {
+        memcpy(PyArray_DATA(unitary), unitary_mtx.data, unitary_mtx.size() * sizeof(QGD_Complex16));
+    }
+
     Py_DECREF(parameters_arr);
     Py_DECREF(unitary);
 
     return Py_BuildValue("i", 0);
 }
 
 
@@ -317,17 +321,17 @@
 
 
 /**
 @brief Structure containing metadata about the module.
 */
 static PyModuleDef  qgd_RZ_Module = {
     PyModuleDef_HEAD_INIT,
-    .m_name = "qgd_RZ",
-    .m_doc = "Python binding for QGD RZ gate",
-    .m_size = -1,
+    "qgd_RZ",
+    "Python binding for QGD RZ gate",
+    -1,
 };
 
 
 /**
 @brief Method called when the Python module is initialized
 */
 PyMODINIT_FUNC
```

### Comparing `squander-1.8.2/qgd_python/gates/qgd_SX.cpp` & `squander-1.8.3/qgd_python/gates/qgd_SX.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -186,14 +186,18 @@
 
 
     // create QGD version of the input matrix
     Matrix unitary_mtx = numpy2matrix(unitary);
 
     self->gate->apply_to( unitary_mtx );
     
+    if (unitary_mtx.data != PyArray_DATA(unitary)) {
+        memcpy(PyArray_DATA(unitary), unitary_mtx.data, unitary_mtx.size() * sizeof(QGD_Complex16));
+    }
+
     Py_DECREF(unitary);
 
     return Py_BuildValue("i", 0);
 }
 
 
 
@@ -294,17 +298,17 @@
 
 
 /**
 @brief Structure containing metadata about the module.
 */
 static PyModuleDef  qgd_SX_Module = {
     PyModuleDef_HEAD_INIT,
-    .m_name = "qgd_SX",
-    .m_doc = "Python binding for QGD SX gate",
-    .m_size = -1,
+    "qgd_SX",
+    "Python binding for QGD SX gate",
+    -1,
 };
 
 
 /**
 @brief Method called when the Python module is initialized
 */
 PyMODINIT_FUNC
```

### Comparing `squander-1.8.2/qgd_python/gates/qgd_SYC.cpp` & `squander-1.8.3/qgd_python/gates/qgd_SYC.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -179,14 +179,18 @@
 
 
     // create QGD version of the input matrix
     Matrix unitary_mtx = numpy2matrix(unitary_arg);
 
     self->gate->apply_to( unitary_mtx );
     
+    if (unitary_mtx.data != PyArray_DATA(unitary_arg)) {
+        memcpy(PyArray_DATA(unitary_arg), unitary_mtx.data, unitary_mtx.size() * sizeof(QGD_Complex16));
+    }
+
     Py_DECREF(unitary_arg);
 
     return Py_BuildValue("i", 0);
 }
 
 
 
@@ -286,17 +290,17 @@
 
 
 /**
 @brief Structure containing metadata about the module.
 */
 static PyModuleDef  qgd_SYC_Module = {
     PyModuleDef_HEAD_INIT,
-    .m_name = "qgd_SYC",
-    .m_doc = "Python binding for QGD SYC gate",
-    .m_size = -1,
+    "qgd_SYC",
+    "Python binding for QGD SYC gate",
+    -1,
 };
 
 
 /**
 @brief Method called when the Python module is initialized
 */
 PyMODINIT_FUNC
```

### Comparing `squander-1.8.2/qgd_python/gates/qgd_U3.cpp` & `squander-1.8.3/qgd_python/gates/qgd_U3.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -224,14 +224,18 @@
 
     // create QGD version of the input matrix
     Matrix unitary_mtx = numpy2matrix(unitary);
 
 
     self->gate->apply_to( parameters_mtx, unitary_mtx );
     
+    if (unitary_mtx.data != PyArray_DATA(unitary)) {
+        memcpy(PyArray_DATA(unitary), unitary_mtx.data, unitary_mtx.size() * sizeof(QGD_Complex16));
+    }
+
     Py_DECREF(parameters_arr);
     Py_DECREF(unitary);
 
     return Py_BuildValue("i", 0);
 }
 
 
@@ -332,17 +336,17 @@
 
 
 /**
 @brief Structure containing metadata about the module.
 */
 static PyModuleDef  qgd_U3_Module = {
     PyModuleDef_HEAD_INIT,
-    .m_name = "qgd_U3",
-    .m_doc = "Python binding for QGD U3 gate",
-    .m_size = -1,
+    "qgd_U3",
+    "Python binding for QGD U3 gate",
+    -1,
 };
 
 
 /**
 @brief Method called when the Python module is initialized
 */
 PyMODINIT_FUNC
```

### Comparing `squander-1.8.2/qgd_python/gates/qgd_X.cpp` & `squander-1.8.3/qgd_python/gates/qgd_X.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -184,14 +184,18 @@
 
 
     // create QGD version of the input matrix
     Matrix unitary_mtx = numpy2matrix(unitary);
 
     self->gate->apply_to( unitary_mtx );
     
+    if (unitary_mtx.data != PyArray_DATA(unitary)) {
+        memcpy(PyArray_DATA(unitary), unitary_mtx.data, unitary_mtx.size() * sizeof(QGD_Complex16));
+    }
+
     Py_DECREF(unitary);
 
     return Py_BuildValue("i", 0);
 }
 
 
 
@@ -291,17 +295,17 @@
 
 
 /**
 @brief Structure containing metadata about the module.
 */
 static PyModuleDef  qgd_X_Module = {
     PyModuleDef_HEAD_INIT,
-    .m_name = "qgd_X",
-    .m_doc = "Python binding for QGD X gate",
-    .m_size = -1,
+    "qgd_X",
+    "Python binding for QGD X gate",
+    -1,
 };
 
 
 /**
 @brief Method called when the Python module is initialized
 */
 PyMODINIT_FUNC
```

### Comparing `squander-1.8.2/qgd_python/gates/qgd_Y.cpp` & `squander-1.8.3/qgd_python/gates/qgd_Y.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -219,14 +219,18 @@
 
 
     // create QGD version of the input matrix
     Matrix unitary_mtx = numpy2matrix(unitary);
 
     self->gate->apply_to( unitary_mtx );
     
+    if (unitary_mtx.data != PyArray_DATA(unitary)) {
+        memcpy(PyArray_DATA(unitary), unitary_mtx.data, unitary_mtx.size() * sizeof(QGD_Complex16));
+    }
+
     Py_DECREF(unitary);
 
     return Py_BuildValue("i", 0);
 }
 
 
 
@@ -326,17 +330,17 @@
 
 
 /**
 @brief Structure containing metadata about the module.
 */
 static PyModuleDef  qgd_Y_Module = {
     PyModuleDef_HEAD_INIT,
-    .m_name = "qgd_Y",
-    .m_doc = "Python binding for QGD X gate",
-    .m_size = -1,
+    "qgd_Y",
+    "Python binding for QGD X gate",
+    -1,
 };
 
 
 /**
 @brief Method called when the Python module is initialized
 */
 PyMODINIT_FUNC
```

### Comparing `squander-1.8.2/qgd_python/gates/qgd_Z.cpp` & `squander-1.8.3/qgd_python/gates/qgd_Z.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -218,14 +218,18 @@
 
 
     // create QGD version of the input matrix
     Matrix unitary_mtx = numpy2matrix(unitary);
 
     self->gate->apply_to( unitary_mtx );
     
+    if (unitary_mtx.data != PyArray_DATA(unitary)) {
+        memcpy(PyArray_DATA(unitary), unitary_mtx.data, unitary_mtx.size() * sizeof(QGD_Complex16));
+    }
+
     Py_DECREF(unitary);
 
     return Py_BuildValue("i", 0);
 }
 
 
 
@@ -325,17 +329,17 @@
 
 
 /**
 @brief Structure containing metadata about the module.
 */
 static PyModuleDef  qgd_Z_Module = {
     PyModuleDef_HEAD_INIT,
-    .m_name = "qgd_Z",
-    .m_doc = "Python binding for QGD X gate",
-    .m_size = -1,
+    "qgd_Z",
+    "Python binding for QGD X gate",
+    -1,
 };
 
 
 /**
 @brief Method called when the Python module is initialized
 */
 PyMODINIT_FUNC
```

### Comparing `squander-1.8.2/qgd_python/gates/test/test_CH.py` & `squander-1.8.3/qgd_python/gates/test/test_CH.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/qgd_python/gates/test/test_CNOT.py` & `squander-1.8.3/qgd_python/gates/test/test_CNOT.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/qgd_python/gates/test/test_CZ.py` & `squander-1.8.3/qgd_python/gates/test/test_CZ.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/qgd_python/gates/test/test_RX.py` & `squander-1.8.3/qgd_python/gates/test/test_RX.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/qgd_python/gates/test/test_RY.py` & `squander-1.8.3/qgd_python/gates/test/test_RY.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/qgd_python/gates/test/test_RZ.py` & `squander-1.8.3/qgd_python/gates/test/test_RZ.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/qgd_python/gates/test/test_SX.py` & `squander-1.8.3/qgd_python/gates/test/test_SX.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/qgd_python/gates/test/test_U3.py` & `squander-1.8.3/qgd_python/gates/test/test_U3.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/qgd_python/gates/test/test_X.py` & `squander-1.8.3/qgd_python/gates/test/test_X.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/qgd_python/gates/test/test_Y.py` & `squander-1.8.3/qgd_python/gates/test/test_Y.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/qgd_python/gates/test/test_Z.py` & `squander-1.8.3/qgd_python/gates/test/test_Z.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/qgd_python/gates/test/test_gates.py` & `squander-1.8.3/qgd_python/gates/test/test_gates.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/qgd_python/nn/CMakeLists.txt` & `squander-1.8.3/qgd_python/nn/CMakeLists.txt`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     ${EXT_DIR}/qgd_nn_Wrapper.cpp
     ${PROJECT_SOURCE_DIR}/common/numpy_interface.cpp        
 )
 
 
 ADD_DEPENDENCIES (qgd_nn_Wrapper qgd)
 
-target_link_libraries (qgd_nn_Wrapper qgd  ${BLAS_LIBRARIES}  ${LAPACKE_LIBRARIES})
+target_link_libraries (qgd_nn_Wrapper qgd  ${BLAS_LIBRARIES}  ${LAPACKE_LIBRARIES} ${TBB_LIB} ${TBBMALLOC_LIB})
 
 python_extension_module(qgd_nn_Wrapper)
 
 
 # adding compile options
 target_compile_options(qgd_nn_Wrapper PRIVATE
     ${CXX_FLAGS}
```

### Comparing `squander-1.8.2/qgd_python/nn/qgd_nn.py` & `squander-1.8.3/qgd_python/nn/qgd_nn.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/qgd_python/nn/qgd_nn_Wrapper.cpp` & `squander-1.8.3/qgd_python/nn/qgd_nn_Wrapper.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -342,17 +342,17 @@
 };
 
 /**
 @brief Structure containing metadata about the module.
 */
 static PyModuleDef qgd_nn_Wrapper_Module = {
     PyModuleDef_HEAD_INIT,
-    .m_name = "qgd_nn_Wrapper",
-    .m_doc = "Python binding for the neural network component of SQUANDER",
-    .m_size = -1,
+    "qgd_nn_Wrapper",
+    "Python binding for the neural network component of SQUANDER",
+    -1,
 };
 
 
 /**
 @brief Method called when the Python module is initialized
 */
 PyMODINIT_FUNC
```

### Comparing `squander-1.8.2/qgd_python/utils.py` & `squander-1.8.3/qgd_python/utils.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/random_unitary/Random_Orthogonal.cpp` & `squander-1.8.3/random_unitary/Random_Orthogonal.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/random_unitary/Random_Unitary.cpp` & `squander-1.8.3/random_unitary/Random_Unitary.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/random_unitary/include/Random_Orthogonal.h` & `squander-1.8.3/random_unitary/include/Random_Orthogonal.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/random_unitary/include/Random_Unitary.h` & `squander-1.8.3/random_unitary/include/Random_Unitary.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/setup.py` & `squander-1.8.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 setup(
     name="squander",
     packages=find_packages(
         exclude=(
             "test_standalone", "test_standalone.*",
         )
     ),
-    version='1.8.2',
+    version='1.8.3',
     url="https://github.com/rakytap/sequential-quantum-gate-decomposer", 
     maintainer="Peter Rakyta",
     maintainer_email="peter.rakyta@ttk.elte.hu",
     include_package_data=True,
     install_requires=[
         "setuptools>=40.8.0",
         "wheel",
```

### Comparing `squander-1.8.2/squander/__init__.py` & `squander-1.8.3/squander/__init__.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/squander.egg-info/PKG-INFO` & `squander-1.8.3/squander.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squander
-Version: 1.8.2
+Version: 1.8.3
 Summary: Package to decompose unitaries into a quantum circuit and for quantum state preparation.
 Home-page: https://github.com/rakytap/sequential-quantum-gate-decomposer
 Maintainer: Peter Rakyta
 Maintainer-email: peter.rakyta@ttk.elte.hu
 License: GNU General Public License v3.0
 Keywords: test,cmake,extension
 Classifier: Intended Audience :: Developers
@@ -78,22 +78,20 @@
 
 Since version 1.7.1 the SQUANDER package is accessible at Python Package Index (PyPI). The package can be installed on linux systems following the steps outlined below:
 
 $ pip install numpy swig tbb-devel wheel scikit-build ninja qiskit
 
 $ pip install squander
 
-
-
 ### Download the SQUANDER package
 
 The developer version of the Quantum Gate Decomposer package can be downloaded from github repository [https://github.com/rakytap/quantum-gate-decomposer/tree/master](https://github.com/rakytap/quantum-gate-decomposer/tree/master).
 After the package is downloaded into the directory **path/to/SQUANDER/package** (which would be the path to the source code of the SQUANDER package), one can proceed to the compilation steps described in the next section.
 
-### How to build the SQUANDER package
+### How to build the SQUANDER package on Unix/Linux/MacOS
 
 The SQUANDER package is equipped with a Python build script and CMake tools to ease the compilation and the deployment of the package.
 The SQUANDER package is parallelized via Threading Building Block (TBB) libraries. If TBB is not present in the system, it can be easily installed via python package [tbb-devel](https://pypi.org/project/tbb-devel/).
 Alternatively the TBB libraries can be installed via apt or yum utility (sudo apt install libtbb-dev) or it can be downloaded from [https://github.com/oneapi-src/oneTBB](https://github.com/oneapi-src/oneTBB)   and built from source. 
 In this case one should supply the necessary environment variables pointing to the header and library files of the TBB package. For newer
 Intel compilers the TBB package is part of the Intel compiler package, similarly to the MKL package. If the TBB library is located at non-standrad path or the SQUANDER package is compiled with GNU compiler, then setting the
 
@@ -103,15 +101,43 @@
 
 environment variables are sufficient for successful compilation. 
 When the TBB library is installed via a python package, setting the environment variables above is not necessary.
 The SQUANDER package with C++ Python extensions can be compiled via the Python script **setup.py** located in the root directory of the SQUANDER package.
 The script automatically finds out the CBLAS library working behind the numpy package and uses it in further linking. 
 The **setup.py** script also build the C++ library of the SQUANDER package by making the appropriate CMake calls. 
 
+### Build and Install on Microsoft Windows with Microsoft Visual C++
+
+CMake must be in the path and able to find the MSVC compiler e.g.
+
+$ set PATH=%PATH%;C:\Program Files\cmake\bin
+
+Now set the TBB and BLAS folders and build via:
+
+$ set TBB_LOCATION=<Python_Folder>/LocalCache/local-packages
+
+$ set TBB_INC_DIR=%TBB_LOCATION%/Library/include
+
+$ set TBB_LIB_DIR=%TBB_LOCATION%/Library/lib
+
+$ set LIB=<BLAS_Location>/lib;<LAPACK_Location>/lib
+
+$ python setup.py build_ext -DTBB_HEADER=<TBB_Location>\Library\include\
+
+Installation merely requires copying DLL files (if they are not in the path):
+
+$ copy _skbuild\win-amd64-3.9\cmake-install\bin .\qgd_python\decomposition
+
+$ copy "%TBB_LOCATION%\Library\bin\tbb12.dll" .\qgd_python\decomposition
+
+$ copy "%TBB_LOCATION%\Library\bin\tbbmalloc.dll" .\qgd_python\decomposition
+
+Verify the installation:
 
+$ python -m pytest
 
 ### Developer build
 
 
 We recommend to install the SQUANDER package in the Anaconda environment. In order to install the necessary requirements, follow the steps below:
 
 Creating new python environment:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: squander Version: 1.8.2 Summary: Package to
+Metadata-Version: 2.1 Name: squander Version: 1.8.3 Summary: Package to
 decompose unitaries into a quantum circuit and for quantum state preparation.
 Home-page: https://github.com/rakytap/sequential-quantum-gate-decomposer
 Maintainer: Peter Rakyta Maintainer-email: peter.rakyta@ttk.elte.hu License:
 GNU General Public License v3.0 Keywords: test,cmake,extension Classifier:
 Intended Audience :: Developers Classifier: Natural Language :: English
 Classifier: Programming Language :: C Classifier: Programming Language :: C++
 Description-Content-Type: text/markdown License-File: LICENSE [![DOI](https://
@@ -63,41 +63,52 @@
 numpy swig tbb-devel wheel scikit-build ninja qiskit $ pip install squander ###
 Download the SQUANDER package The developer version of the Quantum Gate
 Decomposer package can be downloaded from github repository [https://
 github.com/rakytap/quantum-gate-decomposer/tree/master](https://github.com/
 rakytap/quantum-gate-decomposer/tree/master). After the package is downloaded
 into the directory **path/to/SQUANDER/package** (which would be the path to the
 source code of the SQUANDER package), one can proceed to the compilation steps
-described in the next section. ### How to build the SQUANDER package The
-SQUANDER package is equipped with a Python build script and CMake tools to ease
-the compilation and the deployment of the package. The SQUANDER package is
-parallelized via Threading Building Block (TBB) libraries. If TBB is not
-present in the system, it can be easily installed via python package [tbb-
-devel](https://pypi.org/project/tbb-devel/). Alternatively the TBB libraries
-can be installed via apt or yum utility (sudo apt install libtbb-dev) or it can
-be downloaded from [https://github.com/oneapi-src/oneTBB](https://github.com/
-oneapi-src/oneTBB) and built from source. In this case one should supply the
-necessary environment variables pointing to the header and library files of the
-TBB package. For newer Intel compilers the TBB package is part of the Intel
-compiler package, similarly to the MKL package. If the TBB library is located
-at non-standrad path or the SQUANDER package is compiled with GNU compiler,
-then setting the $ export TBB_LIB_DIR=path/to/TBB/lib(64) $ export
+described in the next section. ### How to build the SQUANDER package on Unix/
+Linux/MacOS The SQUANDER package is equipped with a Python build script and
+CMake tools to ease the compilation and the deployment of the package. The
+SQUANDER package is parallelized via Threading Building Block (TBB) libraries.
+If TBB is not present in the system, it can be easily installed via python
+package [tbb-devel](https://pypi.org/project/tbb-devel/). Alternatively the TBB
+libraries can be installed via apt or yum utility (sudo apt install libtbb-dev)
+or it can be downloaded from [https://github.com/oneapi-src/oneTBB](https://
+github.com/oneapi-src/oneTBB) and built from source. In this case one should
+supply the necessary environment variables pointing to the header and library
+files of the TBB package. For newer Intel compilers the TBB package is part of
+the Intel compiler package, similarly to the MKL package. If the TBB library is
+located at non-standrad path or the SQUANDER package is compiled with GNU
+compiler, then setting the $ export TBB_LIB_DIR=path/to/TBB/lib(64) $ export
 TBB_INC_DIR=path/to/TBB/include environment variables are sufficient for
 successful compilation. When the TBB library is installed via a python package,
 setting the environment variables above is not necessary. The SQUANDER package
 with C++ Python extensions can be compiled via the Python script **setup.py**
 located in the root directory of the SQUANDER package. The script automatically
 finds out the CBLAS library working behind the numpy package and uses it in
 further linking. The **setup.py** script also build the C++ library of the
-SQUANDER package by making the appropriate CMake calls. ### Developer build We
-recommend to install the SQUANDER package in the Anaconda environment. In order
-to install the necessary requirements, follow the steps below: Creating new
-python environment: $ conda create -n qgd Activate the new anaconda environment
-$ conda activate qgd Install dependencies: $ conda install numpy scipy pip
-pytest scikit-build tbb-devel $ pip install qiskit matplotlib After the basic
+SQUANDER package by making the appropriate CMake calls. ### Build and Install
+on Microsoft Windows with Microsoft Visual C++ CMake must be in the path and
+able to find the MSVC compiler e.g. $ set PATH=%PATH%;C:\Program
+Files\cmake\bin Now set the TBB and BLAS folders and build via: $ set
+TBB_LOCATION=/LocalCache/local-packages $ set TBB_INC_DIR=%TBB_LOCATION%/
+Library/include $ set TBB_LIB_DIR=%TBB_LOCATION%/Library/lib $ set LIB=/lib;/
+lib $ python setup.py build_ext -DTBB_HEADER=\Library\include\ Installation
+merely requires copying DLL files (if they are not in the path): $ copy
+_skbuild\win-amd64-3.9\cmake-install\bin .\qgd_python\decomposition $ copy
+"%TBB_LOCATION%\Library\bin\tbb12.dll" .\qgd_python\decomposition $ copy
+"%TBB_LOCATION%\Library\bin\tbbmalloc.dll" .\qgd_python\decomposition Verify
+the installation: $ python -m pytest ### Developer build We recommend to
+install the SQUANDER package in the Anaconda environment. In order to install
+the necessary requirements, follow the steps below: Creating new python
+environment: $ conda create -n qgd Activate the new anaconda environment $
+conda activate qgd Install dependencies: $ conda install numpy scipy pip pytest
+scikit-build tbb-devel $ pip install qiskit matplotlib After the basic
 environment variables are set and the dependencies are installed, the
 compilation of the package can be started by the Python command: $ python3
 setup.py build_ext The command above starts the compilation of the SQUANDER C++
 library and builds the necessary C++ Python interface extensions of the
 SQUANDER package in place. After a successful build, one can register the
 SQUANDER package in the Python distribution in developer (i.e. editable) mode
 by command: $ python -m pip install -e . ### Binary distribution After the
```

### Comparing `squander-1.8.2/squander.egg-info/SOURCES.txt` & `squander-1.8.3/squander.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/test_standalone/CMakeLists.txt` & `squander-1.8.3/test_standalone/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/test_standalone/custom_gate_structure_test.cpp` & `squander-1.8.3/test_standalone/custom_gate_structure_test.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.2/test_standalone/decomposition_test.cpp` & `squander-1.8.3/test_standalone/decomposition_test.cpp`

 * *Files identical despite different names*

