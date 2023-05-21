# Comparing `tmp/pyerrors-2.7.0.tar.gz` & `tmp/pyerrors-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyerrors-2.7.0.tar", last modified: Tue Mar 21 09:45:33 2023, max compression
+gzip compressed data, was "pyerrors-2.8.0.tar", last modified: Sun May 21 16:09:27 2023, max compression
```

## Comparing `pyerrors-2.7.0.tar` & `pyerrors-2.8.0.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-03-21 09:45:33.342071 pyerrors-2.7.0/
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-03-21 09:45:33.326071 pyerrors-2.7.0/.github/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      113 2023-03-11 21:38:08.000000 pyerrors-2.7.0/.github/CODEOWNERS
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-03-21 09:45:33.326071 pyerrors-2.7.0/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1051 2023-03-21 09:29:24.000000 pyerrors-2.7.0/.github/ISSUE_TEMPLATE/bug-report.yml
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-03-21 09:45:33.330071 pyerrors-2.7.0/.github/workflows/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      386 2023-03-11 21:38:08.000000 pyerrors-2.7.0/.github/workflows/binder.yml
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      737 2023-03-11 21:38:08.000000 pyerrors-2.7.0/.github/workflows/codeql.yml
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1012 2023-03-11 21:38:08.000000 pyerrors-2.7.0/.github/workflows/docs.yml
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1022 2023-03-21 09:29:24.000000 pyerrors-2.7.0/.github/workflows/examples.yml
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      547 2023-03-21 09:29:24.000000 pyerrors-2.7.0/.github/workflows/flake8.yml
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1043 2023-03-11 21:38:08.000000 pyerrors-2.7.0/.github/workflows/pytest.yml
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      211 2023-03-21 09:29:24.000000 pyerrors-2.7.0/.gitignore
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    15978 2023-03-21 09:29:24.000000 pyerrors-2.7.0/CHANGELOG.md
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      740 2023-03-11 21:38:08.000000 pyerrors-2.7.0/CITATION.cff
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1842 2023-03-21 09:29:24.000000 pyerrors-2.7.0/CONTRIBUTING.md
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1070 2023-03-11 21:38:08.000000 pyerrors-2.7.0/LICENSE
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2736 2023-03-21 09:45:33.342071 pyerrors-2.7.0/PKG-INFO
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1641 2023-03-21 09:29:24.000000 pyerrors-2.7.0/README.md
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)        0 2023-03-11 21:38:08.000000 pyerrors-2.7.0/conftest.py
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-03-21 09:45:33.330071 pyerrors-2.7.0/examples/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    87858 2023-03-11 21:38:08.000000 pyerrors-2.7.0/examples/01_basic_example.ipynb
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    62623 2023-03-11 21:38:08.000000 pyerrors-2.7.0/examples/02_correlators.ipynb
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    97653 2023-03-11 21:38:08.000000 pyerrors-2.7.0/examples/03_pcac_example.ipynb
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   129847 2023-03-11 21:38:08.000000 pyerrors-2.7.0/examples/04_fit_example.ipynb
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     9053 2023-03-11 21:38:08.000000 pyerrors-2.7.0/examples/05_matrix_operations.ipynb
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    30851 2023-03-11 21:38:08.000000 pyerrors-2.7.0/examples/06_gevp.ipynb
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    10604 2023-03-11 21:38:08.000000 pyerrors-2.7.0/examples/07_data_management.ipynb
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    21826 2023-03-21 09:29:24.000000 pyerrors-2.7.0/examples/08_combined_fit_example.ipynb
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      757 2023-03-11 21:38:08.000000 pyerrors-2.7.0/examples/base_style.mplstyle
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-03-21 09:45:33.334071 pyerrors-2.7.0/examples/data/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     7407 2023-03-11 21:38:08.000000 pyerrors-2.7.0/examples/data/correlator_test.json.gz
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    15009 2023-03-11 21:38:08.000000 pyerrors-2.7.0/examples/data/f_A.json.gz
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    15072 2023-03-11 21:38:08.000000 pyerrors-2.7.0/examples/data/f_P.json.gz
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   266539 2023-03-11 21:38:08.000000 pyerrors-2.7.0/examples/data/matrix_correlator.json.gz
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   266778 2023-03-11 21:38:08.000000 pyerrors-2.7.0/examples/data/matrix_correlator_V1V1.json.gz
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   266803 2023-03-11 21:38:08.000000 pyerrors-2.7.0/examples/data/matrix_correlator_V2V2.json.gz
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   266702 2023-03-11 21:38:08.000000 pyerrors-2.7.0/examples/data/matrix_correlator_V3V3.json.gz
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     8575 2023-03-11 21:38:08.000000 pyerrors-2.7.0/examples/json_schema.json
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-03-21 09:45:33.334071 pyerrors-2.7.0/pyerrors/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    29941 2023-03-21 09:29:24.000000 pyerrors-2.7.0/pyerrors/__init__.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    57431 2023-03-21 09:29:24.000000 pyerrors-2.7.0/pyerrors/correlators.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     3609 2023-03-11 21:38:08.000000 pyerrors-2.7.0/pyerrors/covobs.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2909 2023-03-11 21:38:08.000000 pyerrors-2.7.0/pyerrors/dirac.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    30996 2023-03-21 09:29:24.000000 pyerrors-2.7.0/pyerrors/fits.py
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-03-21 09:45:33.334071 pyerrors-2.7.0/pyerrors/input/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      560 2023-03-11 21:38:08.000000 pyerrors-2.7.0/pyerrors/input/__init__.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    25145 2023-03-11 21:38:08.000000 pyerrors-2.7.0/pyerrors/input/bdio.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    30913 2023-03-11 21:38:08.000000 pyerrors-2.7.0/pyerrors/input/dobs.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    16843 2023-03-11 21:38:08.000000 pyerrors-2.7.0/pyerrors/input/hadrons.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    25828 2023-03-11 21:38:08.000000 pyerrors-2.7.0/pyerrors/input/json.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     4055 2023-03-11 21:38:08.000000 pyerrors-2.7.0/pyerrors/input/misc.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    45711 2023-03-21 09:29:24.000000 pyerrors-2.7.0/pyerrors/input/openQCD.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     5718 2023-03-21 09:29:24.000000 pyerrors-2.7.0/pyerrors/input/pandas.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    16290 2023-03-21 09:29:24.000000 pyerrors-2.7.0/pyerrors/input/sfcf.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2250 2023-03-21 09:29:24.000000 pyerrors-2.7.0/pyerrors/input/utils.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    10177 2023-03-11 21:38:08.000000 pyerrors-2.7.0/pyerrors/linalg.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     5381 2023-03-21 09:29:24.000000 pyerrors-2.7.0/pyerrors/misc.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2273 2023-03-11 21:38:08.000000 pyerrors-2.7.0/pyerrors/mpm.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    67261 2023-03-21 09:29:24.000000 pyerrors-2.7.0/pyerrors/obs.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1466 2023-03-11 21:38:08.000000 pyerrors-2.7.0/pyerrors/roots.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)       22 2023-03-21 09:29:24.000000 pyerrors-2.7.0/pyerrors/version.py
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-03-21 09:45:33.334071 pyerrors-2.7.0/pyerrors.egg-info/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2736 2023-03-21 09:45:33.000000 pyerrors-2.7.0/pyerrors.egg-info/PKG-INFO
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2700 2023-03-21 09:45:33.000000 pyerrors-2.7.0/pyerrors.egg-info/SOURCES.txt
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)        1 2023-03-21 09:45:33.000000 pyerrors-2.7.0/pyerrors.egg-info/dependency_links.txt
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      196 2023-03-21 09:45:33.000000 pyerrors-2.7.0/pyerrors.egg-info/requires.txt
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)        9 2023-03-21 09:45:33.000000 pyerrors-2.7.0/pyerrors.egg-info/top_level.txt
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      100 2023-03-11 21:38:08.000000 pyerrors-2.7.0/pyproject.toml
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)       38 2023-03-21 09:45:33.342071 pyerrors-2.7.0/setup.cfg
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1882 2023-03-11 21:38:08.000000 pyerrors-2.7.0/setup.py
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-03-21 09:45:33.338070 pyerrors-2.7.0/tests/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1159 2023-03-11 21:38:08.000000 pyerrors-2.7.0/tests/benchmark_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    17752 2023-03-11 21:38:08.000000 pyerrors-2.7.0/tests/correlators_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     3470 2023-03-11 21:38:08.000000 pyerrors-2.7.0/tests/covobs_test.py
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-03-21 09:45:33.326071 pyerrors-2.7.0/tests/data/
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-03-21 09:45:33.338070 pyerrors-2.7.0/tests/data/openqcd_test/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    38800 2023-03-21 09:29:24.000000 pyerrors-2.7.0/tests/data/openqcd_test/ms5_xsf_T24L16r1.ms5_xsf_dd.dat
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    38800 2023-03-21 09:29:24.000000 pyerrors-2.7.0/tests/data/openqcd_test/ms5_xsf_T24L16r2.ms5_xsf_dd.dat
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    38800 2023-03-21 09:29:24.000000 pyerrors-2.7.0/tests/data/openqcd_test/ms5_xsf_T24L16r3.ms5_xsf_dd.dat
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    87320 2023-03-11 21:38:08.000000 pyerrors-2.7.0/tests/data/openqcd_test/openqcd2r1.ms.dat
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2076 2023-03-11 21:38:08.000000 pyerrors-2.7.0/tests/data/openqcd_test/openqcd2r1.ms1.dat
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   157504 2023-03-11 21:38:08.000000 pyerrors-2.7.0/tests/data/openqcd_test/sfqcdr1.gfms.dat
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      252 2023-03-11 21:38:08.000000 pyerrors-2.7.0/tests/data/openqcd_test/sfqcdr1.rwms.dat
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-03-21 09:45:33.326071 pyerrors-2.7.0/tests/data/sfcf_test/
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-03-21 09:45:33.326071 pyerrors-2.7.0/tests/data/sfcf_test/broken_data_c/
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-03-21 09:45:33.338070 pyerrors-2.7.0/tests/data/sfcf_test/broken_data_c/data_c_r0/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     8712 2023-03-21 09:29:24.000000 pyerrors-2.7.0/tests/data/sfcf_test/broken_data_c/data_c_r0/data_c_r0_n1
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-03-21 09:45:33.338070 pyerrors-2.7.0/tests/data/sfcf_test/data_a/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    24665 2023-03-11 21:38:08.000000 pyerrors-2.7.0/tests/data/sfcf_test/data_a/data_a_r0.F_V0
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    14670 2023-03-11 21:38:08.000000 pyerrors-2.7.0/tests/data/sfcf_test/data_a/data_a_r0.f_1
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     9090 2023-03-11 21:38:08.000000 pyerrors-2.7.0/tests/data/sfcf_test/data_a/data_a_r0.f_A
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-03-21 09:45:33.326071 pyerrors-2.7.0/tests/data/sfcf_test/data_c/
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-03-21 09:45:33.338070 pyerrors-2.7.0/tests/data/sfcf_test/data_c/data_c_r0/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     8918 2023-03-11 21:38:08.000000 pyerrors-2.7.0/tests/data/sfcf_test/data_c/data_c_r0/data_c_r0_n1
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-03-21 09:45:33.326071 pyerrors-2.7.0/tests/data/sfcf_test/data_o/
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-03-21 09:45:33.326071 pyerrors-2.7.0/tests/data/sfcf_test/data_o/test_r0/
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-03-21 09:45:33.338070 pyerrors-2.7.0/tests/data/sfcf_test/data_o/test_r0/cfg1/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     4926 2023-03-11 21:38:08.000000 pyerrors-2.7.0/tests/data/sfcf_test/data_o/test_r0/cfg1/F_V0
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2927 2023-03-11 21:38:08.000000 pyerrors-2.7.0/tests/data/sfcf_test/data_o/test_r0/cfg1/f_1
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1811 2023-03-11 21:38:08.000000 pyerrors-2.7.0/tests/data/sfcf_test/data_o/test_r0/cfg1/f_A
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-03-21 09:45:33.342071 pyerrors-2.7.0/tests/data/sfcf_test/param/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   142045 2023-03-11 21:38:08.000000 pyerrors-2.7.0/tests/data/sfcf_test/param/out.out
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1661 2023-03-11 21:38:08.000000 pyerrors-2.7.0/tests/data/sfcf_test/param/parameters_a
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1661 2023-03-11 21:38:08.000000 pyerrors-2.7.0/tests/data/sfcf_test/param/parameters_c
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1661 2023-03-11 21:38:08.000000 pyerrors-2.7.0/tests/data/sfcf_test/param/parameters_o
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1885 2023-03-11 21:38:08.000000 pyerrors-2.7.0/tests/dirac_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    44785 2023-03-21 09:29:24.000000 pyerrors-2.7.0/tests/fits_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    15342 2023-03-11 21:38:08.000000 pyerrors-2.7.0/tests/json_io_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    14226 2023-03-11 21:38:08.000000 pyerrors-2.7.0/tests/linalg_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      543 2023-03-11 21:38:08.000000 pyerrors-2.7.0/tests/misc_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      314 2023-03-11 21:38:08.000000 pyerrors-2.7.0/tests/mpm_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    40682 2023-03-21 09:29:24.000000 pyerrors-2.7.0/tests/obs_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     7382 2023-03-21 09:29:24.000000 pyerrors-2.7.0/tests/openQCD_in_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     3582 2023-03-21 09:29:24.000000 pyerrors-2.7.0/tests/pandas_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1262 2023-03-11 21:38:08.000000 pyerrors-2.7.0/tests/roots_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     6431 2023-03-21 09:29:24.000000 pyerrors-2.7.0/tests/sfcf_in_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      422 2023-03-21 09:29:24.000000 pyerrors-2.7.0/tests/utils_in_test.py
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.504111 pyerrors-2.8.0/
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.492111 pyerrors-2.8.0/.github/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      113 2023-03-21 12:48:56.000000 pyerrors-2.8.0/.github/CODEOWNERS
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.492111 pyerrors-2.8.0/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1051 2023-03-21 12:48:56.000000 pyerrors-2.8.0/.github/ISSUE_TEMPLATE/bug-report.yml
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.492111 pyerrors-2.8.0/.github/workflows/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      386 2023-03-21 12:48:56.000000 pyerrors-2.8.0/.github/workflows/binder.yml
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      737 2023-03-21 12:48:56.000000 pyerrors-2.8.0/.github/workflows/codeql.yml
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1012 2023-03-21 12:48:56.000000 pyerrors-2.8.0/.github/workflows/docs.yml
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1022 2023-03-21 12:48:56.000000 pyerrors-2.8.0/.github/workflows/examples.yml
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      547 2023-03-21 12:48:56.000000 pyerrors-2.8.0/.github/workflows/flake8.yml
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1043 2023-03-21 12:48:56.000000 pyerrors-2.8.0/.github/workflows/pytest.yml
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      211 2023-03-21 12:48:56.000000 pyerrors-2.8.0/.gitignore
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    16537 2023-05-21 16:06:57.000000 pyerrors-2.8.0/CHANGELOG.md
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1278 2023-05-21 16:06:57.000000 pyerrors-2.8.0/CITATION.cff
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1842 2023-03-21 12:48:56.000000 pyerrors-2.8.0/CONTRIBUTING.md
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1070 2023-03-11 21:38:08.000000 pyerrors-2.8.0/LICENSE
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2705 2023-05-21 16:09:27.504111 pyerrors-2.8.0/PKG-INFO
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1610 2023-05-21 16:06:57.000000 pyerrors-2.8.0/README.md
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)        0 2023-03-11 21:38:08.000000 pyerrors-2.8.0/conftest.py
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.496111 pyerrors-2.8.0/examples/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    87858 2023-03-21 12:48:56.000000 pyerrors-2.8.0/examples/01_basic_example.ipynb
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    62623 2023-03-21 12:48:56.000000 pyerrors-2.8.0/examples/02_correlators.ipynb
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    97653 2023-03-21 12:48:56.000000 pyerrors-2.8.0/examples/03_pcac_example.ipynb
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   129847 2023-03-21 12:48:56.000000 pyerrors-2.8.0/examples/04_fit_example.ipynb
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     9053 2023-03-11 21:38:08.000000 pyerrors-2.8.0/examples/05_matrix_operations.ipynb
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    30851 2023-03-21 12:48:56.000000 pyerrors-2.8.0/examples/06_gevp.ipynb
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    10604 2023-03-21 12:48:56.000000 pyerrors-2.8.0/examples/07_data_management.ipynb
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    21826 2023-03-21 12:48:56.000000 pyerrors-2.8.0/examples/08_combined_fit_example.ipynb
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      757 2023-03-11 21:38:08.000000 pyerrors-2.8.0/examples/base_style.mplstyle
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.496111 pyerrors-2.8.0/examples/data/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     7407 2023-03-11 21:38:08.000000 pyerrors-2.8.0/examples/data/correlator_test.json.gz
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    15009 2023-03-11 21:38:08.000000 pyerrors-2.8.0/examples/data/f_A.json.gz
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    15072 2023-03-11 21:38:08.000000 pyerrors-2.8.0/examples/data/f_P.json.gz
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   266539 2023-03-11 21:38:08.000000 pyerrors-2.8.0/examples/data/matrix_correlator.json.gz
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   266778 2023-03-11 21:38:08.000000 pyerrors-2.8.0/examples/data/matrix_correlator_V1V1.json.gz
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   266803 2023-03-11 21:38:08.000000 pyerrors-2.8.0/examples/data/matrix_correlator_V2V2.json.gz
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   266702 2023-03-11 21:38:08.000000 pyerrors-2.8.0/examples/data/matrix_correlator_V3V3.json.gz
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     8575 2023-03-11 21:38:08.000000 pyerrors-2.8.0/examples/json_schema.json
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.500111 pyerrors-2.8.0/pyerrors/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    29950 2023-05-21 16:06:57.000000 pyerrors-2.8.0/pyerrors/__init__.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    57481 2023-05-21 16:06:57.000000 pyerrors-2.8.0/pyerrors/correlators.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     3609 2023-03-11 21:38:08.000000 pyerrors-2.8.0/pyerrors/covobs.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2909 2023-03-21 12:48:56.000000 pyerrors-2.8.0/pyerrors/dirac.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    30996 2023-03-21 12:48:56.000000 pyerrors-2.8.0/pyerrors/fits.py
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.500111 pyerrors-2.8.0/pyerrors/input/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      579 2023-05-21 16:06:57.000000 pyerrors-2.8.0/pyerrors/input/__init__.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    25145 2023-03-21 12:48:56.000000 pyerrors-2.8.0/pyerrors/input/bdio.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    30913 2023-03-21 12:48:56.000000 pyerrors-2.8.0/pyerrors/input/dobs.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    19262 2023-05-21 16:06:57.000000 pyerrors-2.8.0/pyerrors/input/hadrons.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    26602 2023-05-21 16:06:57.000000 pyerrors-2.8.0/pyerrors/input/json.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     8064 2023-05-21 16:06:57.000000 pyerrors-2.8.0/pyerrors/input/misc.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    49814 2023-05-21 16:06:57.000000 pyerrors-2.8.0/pyerrors/input/openQCD.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     6509 2023-05-21 16:06:57.000000 pyerrors-2.8.0/pyerrors/input/pandas.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    16290 2023-03-21 12:48:56.000000 pyerrors-2.8.0/pyerrors/input/sfcf.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2257 2023-05-21 16:06:57.000000 pyerrors-2.8.0/pyerrors/input/utils.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    10177 2023-03-11 21:38:08.000000 pyerrors-2.8.0/pyerrors/linalg.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     5381 2023-03-21 12:48:56.000000 pyerrors-2.8.0/pyerrors/misc.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2273 2023-03-21 12:48:56.000000 pyerrors-2.8.0/pyerrors/mpm.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    67811 2023-05-21 16:06:57.000000 pyerrors-2.8.0/pyerrors/obs.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1466 2023-03-21 12:48:56.000000 pyerrors-2.8.0/pyerrors/roots.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)       22 2023-05-21 16:06:57.000000 pyerrors-2.8.0/pyerrors/version.py
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.500111 pyerrors-2.8.0/pyerrors.egg-info/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2705 2023-05-21 16:09:27.000000 pyerrors-2.8.0/pyerrors.egg-info/PKG-INFO
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2700 2023-05-21 16:09:27.000000 pyerrors-2.8.0/pyerrors.egg-info/SOURCES.txt
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)        1 2023-05-21 16:09:27.000000 pyerrors-2.8.0/pyerrors.egg-info/dependency_links.txt
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      196 2023-05-21 16:09:27.000000 pyerrors-2.8.0/pyerrors.egg-info/requires.txt
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)        9 2023-05-21 16:09:27.000000 pyerrors-2.8.0/pyerrors.egg-info/top_level.txt
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      100 2023-03-21 12:48:56.000000 pyerrors-2.8.0/pyproject.toml
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)       38 2023-05-21 16:09:27.504111 pyerrors-2.8.0/setup.cfg
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1882 2023-03-21 12:48:56.000000 pyerrors-2.8.0/setup.py
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.500111 pyerrors-2.8.0/tests/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1159 2023-03-11 21:38:08.000000 pyerrors-2.8.0/tests/benchmark_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    17752 2023-03-21 12:48:56.000000 pyerrors-2.8.0/tests/correlators_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     3470 2023-03-11 21:38:08.000000 pyerrors-2.8.0/tests/covobs_test.py
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.488111 pyerrors-2.8.0/tests/data/
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.500111 pyerrors-2.8.0/tests/data/openqcd_test/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    38800 2023-03-21 12:48:56.000000 pyerrors-2.8.0/tests/data/openqcd_test/ms5_xsf_T24L16r1.ms5_xsf_dd.dat
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    38800 2023-03-21 12:48:56.000000 pyerrors-2.8.0/tests/data/openqcd_test/ms5_xsf_T24L16r2.ms5_xsf_dd.dat
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    38800 2023-03-21 12:48:56.000000 pyerrors-2.8.0/tests/data/openqcd_test/ms5_xsf_T24L16r3.ms5_xsf_dd.dat
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    87320 2023-03-11 21:38:08.000000 pyerrors-2.8.0/tests/data/openqcd_test/openqcd2r1.ms.dat
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2076 2023-03-11 21:38:08.000000 pyerrors-2.8.0/tests/data/openqcd_test/openqcd2r1.ms1.dat
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   157504 2023-03-11 21:38:08.000000 pyerrors-2.8.0/tests/data/openqcd_test/sfqcdr1.gfms.dat
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      252 2023-03-11 21:38:08.000000 pyerrors-2.8.0/tests/data/openqcd_test/sfqcdr1.rwms.dat
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.492111 pyerrors-2.8.0/tests/data/sfcf_test/
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.488111 pyerrors-2.8.0/tests/data/sfcf_test/broken_data_c/
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.500111 pyerrors-2.8.0/tests/data/sfcf_test/broken_data_c/data_c_r0/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     8712 2023-03-21 12:48:56.000000 pyerrors-2.8.0/tests/data/sfcf_test/broken_data_c/data_c_r0/data_c_r0_n1
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.500111 pyerrors-2.8.0/tests/data/sfcf_test/data_a/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    24665 2023-03-11 21:38:08.000000 pyerrors-2.8.0/tests/data/sfcf_test/data_a/data_a_r0.F_V0
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    14670 2023-03-11 21:38:08.000000 pyerrors-2.8.0/tests/data/sfcf_test/data_a/data_a_r0.f_1
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     9090 2023-03-11 21:38:08.000000 pyerrors-2.8.0/tests/data/sfcf_test/data_a/data_a_r0.f_A
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.488111 pyerrors-2.8.0/tests/data/sfcf_test/data_c/
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.500111 pyerrors-2.8.0/tests/data/sfcf_test/data_c/data_c_r0/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     8918 2023-03-11 21:38:08.000000 pyerrors-2.8.0/tests/data/sfcf_test/data_c/data_c_r0/data_c_r0_n1
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.492111 pyerrors-2.8.0/tests/data/sfcf_test/data_o/
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.492111 pyerrors-2.8.0/tests/data/sfcf_test/data_o/test_r0/
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.500111 pyerrors-2.8.0/tests/data/sfcf_test/data_o/test_r0/cfg1/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     4926 2023-03-11 21:38:08.000000 pyerrors-2.8.0/tests/data/sfcf_test/data_o/test_r0/cfg1/F_V0
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2927 2023-03-11 21:38:08.000000 pyerrors-2.8.0/tests/data/sfcf_test/data_o/test_r0/cfg1/f_1
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1811 2023-03-11 21:38:08.000000 pyerrors-2.8.0/tests/data/sfcf_test/data_o/test_r0/cfg1/f_A
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.504111 pyerrors-2.8.0/tests/data/sfcf_test/param/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   142045 2023-03-11 21:38:08.000000 pyerrors-2.8.0/tests/data/sfcf_test/param/out.out
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1661 2023-03-11 21:38:08.000000 pyerrors-2.8.0/tests/data/sfcf_test/param/parameters_a
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1661 2023-03-11 21:38:08.000000 pyerrors-2.8.0/tests/data/sfcf_test/param/parameters_c
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1661 2023-03-11 21:38:08.000000 pyerrors-2.8.0/tests/data/sfcf_test/param/parameters_o
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1885 2023-03-11 21:38:08.000000 pyerrors-2.8.0/tests/dirac_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    44785 2023-03-21 12:48:56.000000 pyerrors-2.8.0/tests/fits_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    15556 2023-05-21 16:06:57.000000 pyerrors-2.8.0/tests/json_io_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    14226 2023-03-21 12:48:56.000000 pyerrors-2.8.0/tests/linalg_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      543 2023-03-21 12:48:56.000000 pyerrors-2.8.0/tests/misc_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      314 2023-03-11 21:38:08.000000 pyerrors-2.8.0/tests/mpm_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    45834 2023-05-21 16:06:57.000000 pyerrors-2.8.0/tests/obs_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     7967 2023-05-21 16:06:57.000000 pyerrors-2.8.0/tests/openQCD_in_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    10938 2023-05-21 16:06:57.000000 pyerrors-2.8.0/tests/pandas_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1262 2023-03-21 12:48:56.000000 pyerrors-2.8.0/tests/roots_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     6431 2023-03-21 12:48:56.000000 pyerrors-2.8.0/tests/sfcf_in_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1415 2023-05-21 16:06:57.000000 pyerrors-2.8.0/tests/utils_in_test.py
```

### Comparing `pyerrors-2.7.0/.github/ISSUE_TEMPLATE/bug-report.yml` & `pyerrors-2.8.0/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/.github/workflows/codeql.yml` & `pyerrors-2.8.0/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/.github/workflows/docs.yml` & `pyerrors-2.8.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/.github/workflows/examples.yml` & `pyerrors-2.8.0/.github/workflows/examples.yml`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/.github/workflows/flake8.yml` & `pyerrors-2.8.0/.github/workflows/flake8.yml`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/.github/workflows/pytest.yml` & `pyerrors-2.8.0/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/CHANGELOG.md` & `pyerrors-2.8.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,27 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## [2.8.0] - 2023-05-21
+### Added
+- `pyerrors` can now deal with replica with different gapsizes.
+- String formatting method for `Obs` added.
+- `t0` can now be extracted from hadrons files.
+- `w0` can now be extracted from openQCD files.
+- `pandas` SQL export can now deal with `None` entries in columns with `pyerrors` datatypes.
+
+
+### Fixed
+- `dobs` submodule is now correctly imported.
+- Bug in merging of `Obs` fixed.
+- Bug in `rapidjson` dict output fixed.
+- String conversion of `Obs` can now handle special `dvalue`s
+- Bug in sfcf name sorting fixed.
+
 ## [2.7.0] - 2023-03-21
 ### Added
 - Alternative way of specifying priors in `least_squares` added.
 - Correlated fits now also work with priors.
 - Lists of `Obs` can now be serialized and deserialized in pandas.to_sql
 - `print_config` function for debugging purposes added.
 - `Corr.show` can now visualize results of combined fits.
```

### Comparing `pyerrors-2.7.0/CITATION.cff` & `pyerrors-2.8.0/CITATION.cff`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 cff-version: 1.2.0
-title: >-
-  pyerrors: a python framework for error analysis of
-  Monte Carlo data
+title: "pyerrors"
 message: >-
   If you use this software, please cite it using the
   metadata from this file.
 type: software
 authors:
   - given-names: Fabian
     family-names: Joswig
@@ -15,11 +13,30 @@
     orcid: 'https://orcid.org/0000-0002-0955-9228'
   - given-names: Justus T.
     family-names: Kuhlmann
     orcid: 'https://orcid.org/0000-0001-5291-1939'
   - given-names: Jan
     family-names: Neuendorf
     orcid: 'https://orcid.org/0000-0001-6177-7014'
-identifiers:
-  - type: doi
-    value: 10.48550/arXiv.2209.14371
 repository-code: 'https://github.com/fjosw/pyerrors'
+preferred-citation:
+  type: article
+  authors:
+  - given-names: Fabian
+    family-names: Joswig
+    orcid: 'https://orcid.org/0000-0003-0740-6524'
+  - given-names: Simon
+    family-names: Kuberski
+    orcid: 'https://orcid.org/0000-0002-0955-9228'
+  - given-names: Justus T.
+    family-names: Kuhlmann
+    orcid: 'https://orcid.org/0000-0001-5291-1939'
+  - given-names: Jan
+    family-names: Neuendorf
+    orcid: 'https://orcid.org/0000-0001-6177-7014'
+  doi: "10.1016/j.cpc.2023.108750"
+  journal: "Computer Physics Communications"
+  month: 7
+  start: 108750
+  title: "pyerrors: A python framework for error analysis of Monte Carlo data"
+  volume: 288
+  year: 2023
```

### Comparing `pyerrors-2.7.0/CONTRIBUTING.md` & `pyerrors-2.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/LICENSE` & `pyerrors-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/PKG-INFO` & `pyerrors-2.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyerrors
-Version: 2.7.0
+Version: 2.8.0
 Summary: Error propagation and statistical analysis for Monte Carlo simulations
 Home-page: https://github.com/fjosw/pyerrors
 Author: Fabian Joswig
 Author-email: fabian.joswig@ed.ac.uk
 License: MIT
 Project-URL: Documentation, https://fjosw.github.io/pyerrors/pyerrors.html
 Project-URL: Bug Tracker, https://github.com/fjosw/pyerrors/issues
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-[![flake8](https://github.com/fjosw/pyerrors/actions/workflows/flake8.yml/badge.svg)](https://github.com/fjosw/pyerrors/actions/workflows/flake8.yml) [![pytest](https://github.com/fjosw/pyerrors/actions/workflows/pytest.yml/badge.svg)](https://github.com/fjosw/pyerrors/actions/workflows/pytest.yml) [![](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![arXiv](https://img.shields.io/badge/arXiv-2209.14371-b31b1b.svg)](https://arxiv.org/abs/2209.14371)
+[![pytest](https://github.com/fjosw/pyerrors/actions/workflows/pytest.yml/badge.svg)](https://github.com/fjosw/pyerrors/actions/workflows/pytest.yml) [![](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![arXiv](https://img.shields.io/badge/arXiv-2209.14371-b31b1b.svg)](https://arxiv.org/abs/2209.14371) [![DOI](https://img.shields.io/badge/DOI-10.1016%2Fj.cpc.2023.108750-blue)](https://doi.org/10.1016/j.cpc.2023.108750)
 # pyerrors
 `pyerrors` is a python framework for error computation and propagation of Markov chain Monte Carlo data from lattice field theory and statistical mechanics simulations.
 
 - **Documentation:** https://fjosw.github.io/pyerrors/pyerrors.html
 - **Examples:** https://github.com/fjosw/pyerrors/tree/develop/examples
 - **Bug reports:** https://github.com/fjosw/pyerrors/issues
```

### Comparing `pyerrors-2.7.0/README.md` & `pyerrors-2.8.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![flake8](https://github.com/fjosw/pyerrors/actions/workflows/flake8.yml/badge.svg)](https://github.com/fjosw/pyerrors/actions/workflows/flake8.yml) [![pytest](https://github.com/fjosw/pyerrors/actions/workflows/pytest.yml/badge.svg)](https://github.com/fjosw/pyerrors/actions/workflows/pytest.yml) [![](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![arXiv](https://img.shields.io/badge/arXiv-2209.14371-b31b1b.svg)](https://arxiv.org/abs/2209.14371)
+[![pytest](https://github.com/fjosw/pyerrors/actions/workflows/pytest.yml/badge.svg)](https://github.com/fjosw/pyerrors/actions/workflows/pytest.yml) [![](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![arXiv](https://img.shields.io/badge/arXiv-2209.14371-b31b1b.svg)](https://arxiv.org/abs/2209.14371) [![DOI](https://img.shields.io/badge/DOI-10.1016%2Fj.cpc.2023.108750-blue)](https://doi.org/10.1016/j.cpc.2023.108750)
 # pyerrors
 `pyerrors` is a python framework for error computation and propagation of Markov chain Monte Carlo data from lattice field theory and statistical mechanics simulations.
 
 - **Documentation:** https://fjosw.github.io/pyerrors/pyerrors.html
 - **Examples:** https://github.com/fjosw/pyerrors/tree/develop/examples
 - **Bug reports:** https://github.com/fjosw/pyerrors/issues
```

### Comparing `pyerrors-2.7.0/examples/01_basic_example.ipynb` & `pyerrors-2.8.0/examples/01_basic_example.ipynb`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/examples/02_correlators.ipynb` & `pyerrors-2.8.0/examples/02_correlators.ipynb`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/examples/03_pcac_example.ipynb` & `pyerrors-2.8.0/examples/03_pcac_example.ipynb`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/examples/04_fit_example.ipynb` & `pyerrors-2.8.0/examples/04_fit_example.ipynb`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/examples/05_matrix_operations.ipynb` & `pyerrors-2.8.0/examples/05_matrix_operations.ipynb`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/examples/06_gevp.ipynb` & `pyerrors-2.8.0/examples/06_gevp.ipynb`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/examples/07_data_management.ipynb` & `pyerrors-2.8.0/examples/07_data_management.ipynb`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/examples/08_combined_fit_example.ipynb` & `pyerrors-2.8.0/examples/08_combined_fit_example.ipynb`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/examples/base_style.mplstyle` & `pyerrors-2.8.0/examples/base_style.mplstyle`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/examples/data/correlator_test.json.gz` & `pyerrors-2.8.0/examples/data/correlator_test.json.gz`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/examples/data/f_A.json.gz` & `pyerrors-2.8.0/examples/data/f_A.json.gz`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/examples/data/f_P.json.gz` & `pyerrors-2.8.0/examples/data/f_P.json.gz`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/examples/data/matrix_correlator.json.gz` & `pyerrors-2.8.0/examples/data/matrix_correlator.json.gz`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/examples/data/matrix_correlator_V1V1.json.gz` & `pyerrors-2.8.0/examples/data/matrix_correlator_V1V1.json.gz`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/examples/data/matrix_correlator_V2V2.json.gz` & `pyerrors-2.8.0/examples/data/matrix_correlator_V2V2.json.gz`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/examples/data/matrix_correlator_V3V3.json.gz` & `pyerrors-2.8.0/examples/data/matrix_correlator_V3V3.json.gz`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/examples/json_schema.json` & `pyerrors-2.8.0/examples/json_schema.json`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/pyerrors/__init__.py` & `pyerrors-2.8.0/pyerrors/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 - coherent error propagation for data from different Markov chains.
 - non-linear fits with x- and y-errors and exact linear error propagation based on automatic differentiation as introduced in [arXiv:1809.01289](https://arxiv.org/abs/1809.01289).
 - real and complex matrix operations and their error propagation based on automatic differentiation (Matrix inverse, Cholesky decomposition, calculation of eigenvalues and eigenvectors, singular value decomposition...).
 
 More detailed examples can found in the [GitHub repository](https://github.com/fjosw/pyerrors/tree/develop/examples) [![badge](https://img.shields.io/badge/-try%20it%20out-579ACA.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAFkAAABZCAMAAABi1XidAAAB8lBMVEX///9XmsrmZYH1olJXmsr1olJXmsrmZYH1olJXmsr1olJXmsrmZYH1olL1olJXmsr1olJXmsrmZYH1olL1olJXmsrmZYH1olJXmsr1olL1olJXmsrmZYH1olL1olJXmsrmZYH1olL1olL0nFf1olJXmsrmZYH1olJXmsq8dZb1olJXmsrmZYH1olJXmspXmspXmsr1olL1olJXmsrmZYH1olJXmsr1olL1olJXmsrmZYH1olL1olLeaIVXmsrmZYH1olL1olL1olJXmsrmZYH1olLna31Xmsr1olJXmsr1olJXmsrmZYH1olLqoVr1olJXmsr1olJXmsrmZYH1olL1olKkfaPobXvviGabgadXmsqThKuofKHmZ4Dobnr1olJXmsr1olJXmspXmsr1olJXmsrfZ4TuhWn1olL1olJXmsqBi7X1olJXmspZmslbmMhbmsdemsVfl8ZgmsNim8Jpk8F0m7R4m7F5nLB6jbh7jbiDirOEibOGnKaMhq+PnaCVg6qWg6qegKaff6WhnpKofKGtnomxeZy3noG6dZi+n3vCcpPDcpPGn3bLb4/Mb47UbIrVa4rYoGjdaIbeaIXhoWHmZYHobXvpcHjqdHXreHLroVrsfG/uhGnuh2bwj2Hxk17yl1vzmljzm1j0nlX1olL3AJXWAAAAbXRSTlMAEBAQHx8gICAuLjAwMDw9PUBAQEpQUFBXV1hgYGBkcHBwcXl8gICAgoiIkJCQlJicnJ2goKCmqK+wsLC4usDAwMjP0NDQ1NbW3Nzg4ODi5+3v8PDw8/T09PX29vb39/f5+fr7+/z8/Pz9/v7+zczCxgAABC5JREFUeAHN1ul3k0UUBvCb1CTVpmpaitAGSLSpSuKCLWpbTKNJFGlcSMAFF63iUmRccNG6gLbuxkXU66JAUef/9LSpmXnyLr3T5AO/rzl5zj137p136BISy44fKJXuGN/d19PUfYeO67Znqtf2KH33Id1psXoFdW30sPZ1sMvs2D060AHqws4FHeJojLZqnw53cmfvg+XR8mC0OEjuxrXEkX5ydeVJLVIlV0e10PXk5k7dYeHu7Cj1j+49uKg7uLU61tGLw1lq27ugQYlclHC4bgv7VQ+TAyj5Zc/UjsPvs1sd5cWryWObtvWT2EPa4rtnWW3JkpjggEpbOsPr7F7EyNewtpBIslA7p43HCsnwooXTEc3UmPmCNn5lrqTJxy6nRmcavGZVt/3Da2pD5NHvsOHJCrdc1G2r3DITpU7yic7w/7Rxnjc0kt5GC4djiv2Sz3Fb2iEZg41/ddsFDoyuYrIkmFehz0HR2thPgQqMyQYb2OtB0WxsZ3BeG3+wpRb1vzl2UYBog8FfGhttFKjtAclnZYrRo9ryG9uG/FZQU4AEg8ZE9LjGMzTmqKXPLnlWVnIlQQTvxJf8ip7VgjZjyVPrjw1te5otM7RmP7xm+sK2Gv9I8Gi++BRbEkR9EBw8zRUcKxwp73xkaLiqQb+kGduJTNHG72zcW9LoJgqQxpP3/Tj//c3yB0tqzaml05/+orHLksVO+95kX7/7qgJvnjlrfr2Ggsyx0eoy9uPzN5SPd86aXggOsEKW2Prz7du3VID3/tzs/sSRs2w7ovVHKtjrX2pd7ZMlTxAYfBAL9jiDwfLkq55Tm7ifhMlTGPyCAs7RFRhn47JnlcB9RM5T97ASuZXIcVNuUDIndpDbdsfrqsOppeXl5Y+XVKdjFCTh+zGaVuj0d9zy05PPK3QzBamxdwtTCrzyg/2Rvf2EstUjordGwa/kx9mSJLr8mLLtCW8HHGJc2R5hS219IiF6PnTusOqcMl57gm0Z8kanKMAQg0qSyuZfn7zItsbGyO9QlnxY0eCuD1XL2ys/MsrQhltE7Ug0uFOzufJFE2PxBo/YAx8XPPdDwWN0MrDRYIZF0mSMKCNHgaIVFoBbNoLJ7tEQDKxGF0kcLQimojCZopv0OkNOyWCCg9XMVAi7ARJzQdM2QUh0gmBozjc3Skg6dSBRqDGYSUOu66Zg+I2fNZs/M3/f/Grl/XnyF1Gw3VKCez0PN5IUfFLqvgUN4C0qNqYs5YhPL+aVZYDE4IpUk57oSFnJm4FyCqqOE0jhY2SMyLFoo56zyo6becOS5UVDdj7Vih0zp+tcMhwRpBeLyqtIjlJKAIZSbI8SGSF3k0pA3mR5tHuwPFoa7N7reoq2bqCsAk1HqCu5uvI1n6JuRXI+S1Mco54YmYTwcn6Aeic+kssXi8XpXC4V3t7/ADuTNKaQJdScAAAAAElFTkSuQmCC)](https://mybinder.org/v2/gh/fjosw/pyerrors/HEAD?labpath=examples).
 
 If you use `pyerrors` for research that leads to a publication please consider citing:
-- Fabian Joswig, Simon Kuberski, Justus T. Kuhlmann, Jan Neuendorf, *pyerrors: a python framework for error analysis of Monte Carlo data*. [arXiv:2209.14371 [hep-lat]].
+- Fabian Joswig, Simon Kuberski, Justus T. Kuhlmann, Jan Neuendorf, *pyerrors: a python framework for error analysis of Monte Carlo data*. Comput.Phys.Commun. 288 (2023) 108750.
 - Ulli Wolff, *Monte Carlo errors with less errors*. Comput.Phys.Commun. 156 (2004) 143-153, Comput.Phys.Commun. 176 (2007) 383 (erratum).
 - Alberto Ramos, *Automatic differentiation for error analysis of Monte Carlo data*. Comput.Phys.Commun. 238 (2019) 19-35.
 
 and
 
 - Stefan Schaefer, Rainer Sommer, Francesco Virotta, *Critical slowing down and error analysis in lattice QCD simulations*. Nucl.Phys.B 845 (2011) 93-119.
```

### Comparing `pyerrors-2.7.0/pyerrors/correlators.py` & `pyerrors-2.8.0/pyerrors/correlators.py`

 * *Files 0% similar despite different names*

```diff
@@ -876,16 +876,16 @@
             if isinstance(references, list):
                 for ref in references:
                     ax1.axhline(y=ref, linewidth=1, color=plt.rcParams['text.color'], alpha=0.6, marker=',', ls='--')
             else:
                 raise Exception("'references' must be a list of floating pint values.")
 
         if self.prange:
-            ax1.axvline(self.prange[0], 0, 1, ls='-', marker=',')
-            ax1.axvline(self.prange[1], 0, 1, ls='-', marker=',')
+            ax1.axvline(self.prange[0], 0, 1, ls='-', marker=',', color="black", zorder=0)
+            ax1.axvline(self.prange[1], 0, 1, ls='-', marker=',', color="black", zorder=0)
 
         if fit_res:
             x_samples = np.arange(x_range[0], x_range[1] + 1, 0.05)
             if isinstance(fit_res.fit_function, dict):
                 if fit_key:
                     ax1.plot(x_samples, fit_res.fit_function[fit_key]([o.value for o in fit_res.fit_parameters], x_samples), ls='-', marker=',', lw=2)
                 else:
```

### Comparing `pyerrors-2.7.0/pyerrors/covobs.py` & `pyerrors-2.8.0/pyerrors/covobs.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/pyerrors/dirac.py` & `pyerrors-2.8.0/pyerrors/dirac.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/pyerrors/fits.py` & `pyerrors-2.8.0/pyerrors/fits.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/pyerrors/input/__init__.py` & `pyerrors-2.8.0/pyerrors/input/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,13 +2,14 @@
 `pyerrors` includes an `input` submodule in which input routines and parsers for the output of various numerical programs are contained.
 
 # Jackknife samples
 For comparison with other analysis workflows `pyerrors` can also generate jackknife samples from an `Obs` object or import jackknife samples into an `Obs` object.
 See `pyerrors.obs.Obs.export_jackknife` and `pyerrors.obs.import_jackknife` for details.
 '''
 from . import bdio
+from . import dobs
 from . import hadrons
 from . import json
 from . import misc
 from . import openQCD
 from . import pandas
 from . import sfcf
```

### Comparing `pyerrors-2.7.0/pyerrors/input/bdio.py` & `pyerrors-2.8.0/pyerrors/input/bdio.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/pyerrors/input/dobs.py` & `pyerrors-2.8.0/pyerrors/input/dobs.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/pyerrors/input/hadrons.py` & `pyerrors-2.8.0/pyerrors/input/hadrons.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from collections import Counter
 import h5py
 from pathlib import Path
 import numpy as np
 from ..obs import Obs, CObs
 from ..correlators import Corr
 from ..dirac import epsilon_tensor_rank4
+from .misc import fit_t0
 
 
 def _get_files(path, filestem, idl):
     ls = os.listdir(path)
 
     # Clean up file list
     files = list(filter(lambda x: x.startswith(filestem + "."), ls))
@@ -117,14 +118,80 @@
         l_obs.append(Obs([c], [ens_id], idl=[idx]))
 
     corr = Corr(l_obs)
     corr.tag = r", ".join(infos)
     return corr
 
 
+def _extract_real_arrays(path, files, tree, keys):
+    corr_data = {}
+    for key in keys:
+        corr_data[key] = []
+    for hd5_file in files:
+        h5file = h5py.File(path + '/' + hd5_file, "r")
+        for key in keys:
+            if not tree + '/' + key in h5file:
+                raise Exception("Entry '" + key + "' not contained in the files.")
+            raw_data = h5file[tree + '/' + key + '/data']
+            real_data = raw_data[:].astype(np.double)
+            corr_data[key].append(real_data)
+        h5file.close()
+    for key in keys:
+        corr_data[key] = np.array(corr_data[key])
+    return corr_data
+
+
+def extract_t0_hd5(path, filestem, ens_id, obs='Clover energy density', fit_range=5, idl=None, **kwargs):
+    r'''Read hadrons FlowObservables hdf5 file and extract t0
+
+    Parameters
+    -----------------
+    path : str
+        path to the files to read
+    filestem : str
+        namestem of the files to read
+    ens_id : str
+        name of the ensemble, required for internal bookkeeping
+    obs : str
+        label of the observable from which t0 should be extracted.
+        Options: 'Clover energy density' and 'Plaquette energy density'
+    fit_range : int
+        Number of data points left and right of the zero
+        crossing to be included in the linear fit. (Default: 5)
+    idl : range
+        If specified only configurations in the given range are read in.
+    plot_fit : bool
+        If true, the fit for the extraction of t0 is shown together with the data.
+    '''
+
+    files, idx = _get_files(path, filestem, idl)
+    tree = "FlowObservables"
+
+    h5file = h5py.File(path + '/' + files[0], "r")
+    obs_key = None
+    for key in h5file[tree].keys():
+        if obs == h5file[tree][key].attrs["description"][0].decode():
+            obs_key = key
+            break
+    h5file.close()
+    if obs_key is None:
+        raise Exception(f"Observable {obs} not found.")
+
+    corr_data = _extract_real_arrays(path, files, tree, ["FlowObservables_0", obs_key])
+
+    if not np.allclose(corr_data["FlowObservables_0"][0], corr_data["FlowObservables_0"][:]):
+        raise Exception("Not all flow times were equal.")
+
+    t2E_dict = {}
+    for t2, dat in zip(corr_data["FlowObservables_0"][0], corr_data[obs_key].T):
+        t2E_dict[t2] = Obs([dat], [ens_id], idl=[idx]) - 0.3
+
+    return fit_t0(t2E_dict, fit_range, plot_fit=kwargs.get('plot_fit'))
+
+
 def read_DistillationContraction_hd5(path, ens_id, diagrams=["direct"], idl=None):
     """Read hadrons DistillationContraction hdf5 files in given directory structure
 
     Parameters
     -----------------
     path : str
         path to the directories to read
```

### Comparing `pyerrors-2.7.0/pyerrors/input/json.py` & `pyerrors-2.8.0/pyerrors/input/json.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,27 +184,45 @@
         elif isinstance(io, np.ndarray):
             d['obsdata'].append(write_Array_to_dict(io))
         elif isinstance(io, Corr):
             d['obsdata'].append(write_Corr_to_dict(io))
         else:
             raise Exception("Unkown datatype.")
 
-    def _jsonifier(o):
-        if isinstance(o, np.int64):
-            return int(o)
-        raise TypeError('%r is not JSON serializable' % o)
+    def _jsonifier(obj):
+        if isinstance(obj, dict):
+            result = {}
+            for key in obj:
+                if key is True:
+                    result['true'] = obj[key]
+                elif key is False:
+                    result['false'] = obj[key]
+                elif key is None:
+                    result['null'] = obj[key]
+                elif isinstance(key, (int, float, np.floating, np.integer)):
+                    result[str(key)] = obj[key]
+                else:
+                    raise TypeError('keys must be str, int, float, bool or None')
+            return result
+        elif isinstance(obj, np.integer):
+            return int(obj)
+        elif isinstance(obj, np.floating):
+            return float(obj)
+        else:
+            raise ValueError('%r is not JSON serializable' % (obj,))
 
     if indent:
         return json.dumps(d, indent=indent, ensure_ascii=False, default=_jsonifier, write_mode=json.WM_SINGLE_LINE_ARRAY)
     else:
         return json.dumps(d, indent=indent, ensure_ascii=False, default=_jsonifier, write_mode=json.WM_COMPACT)
 
 
 def dump_to_json(ol, fname, description='', indent=1, gz=True):
-    """Export a list of Obs or structures containing Obs to a .json(.gz) file
+    """Export a list of Obs or structures containing Obs to a .json(.gz) file.
+    Dict keys that are not JSON-serializable such as floats are converted to strings.
 
     Parameters
     ----------
     ol : list
         List of objects that will be exported. At the moment, these objects can be
         either of: Obs, list, numpy.ndarray, Corr.
         All Obs inside a structure have to be defined on the same set of configurations.
@@ -475,15 +493,14 @@
     or
     result : Obs
         only one observable if the list only has one entry
     or
     result : dict
         if full_output=True
     """
-
     return _parse_json_dict(json.loads(json_string), verbose, full_output)
 
 
 def load_json(fname, verbose=True, gz=True, full_output=False):
     """Import a list of Obs or structures containing Obs from a .json(.gz) file.
 
     The following structures are supported: Obs, list, numpy.ndarray, Corr
@@ -562,15 +579,15 @@
                 v = list_replace_obs(v)
             elif isinstance(v, obstypes):
                 ol.append(v)
                 v = reps + '%d' % (counter)
                 counter += 1
             elif isinstance(v, str):
                 if bool(re.match(r'%s[0-9]+' % (reps), v)):
-                    raise Exception('Dict contains string %s that matches the placeholder! %s Cannot be savely exported.' % (v, reps))
+                    raise Exception('Dict contains string %s that matches the placeholder! %s Cannot be safely exported.' % (v, reps))
             x[k] = v
         return x
 
     def list_replace_obs(li):
         nonlocal ol
         nonlocal counter
         x = []
@@ -583,15 +600,15 @@
                 e = dict_replace_obs(e)
             elif isinstance(e, obstypes):
                 ol.append(e)
                 e = reps + '%d' % (counter)
                 counter += 1
             elif isinstance(e, str):
                 if bool(re.match(r'%s[0-9]+' % (reps), e)):
-                    raise Exception('Dict contains string %s that matches the placeholder! %s Cannot be savely exported.' % (e, reps))
+                    raise Exception('Dict contains string %s that matches the placeholder! %s Cannot be safely exported.' % (e, reps))
             x.append(e)
         return x
 
     def obslist_replace_obs(li):
         nonlocal ol
         nonlocal counter
         il = []
```

### Comparing `pyerrors-2.7.0/pyerrors/input/openQCD.py` & `pyerrors-2.8.0/pyerrors/input/openQCD.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import os
 import fnmatch
 import struct
 import warnings
 import numpy as np  # Thinly-wrapped numpy
-import matplotlib.pyplot as plt
-from matplotlib import gridspec
 from ..obs import Obs
-from ..fits import fit_lin
 from ..obs import CObs
 from ..correlators import Corr
+from .misc import fit_t0
 from .utils import sort_names
 
 
 def read_rwms(path, prefix, version='2.0', names=None, **kwargs):
     """Read rwms format from given folder structure. Returns a list of length nrw
 
     Parameters
@@ -227,22 +225,20 @@
     idl = [range(configlist[rep][r_start_index[rep]], configlist[rep][r_stop_index[rep]] + 1, r_step) for rep in range(replica)]
 
     for t in range(nrw):
         result.append(Obs(deltas[t], rep_names, idl=idl))
     return result
 
 
-def extract_t0(path, prefix, dtr_read, xmin, spatial_extent, fit_range=5, **kwargs):
-    """Extract t0 from given .ms.dat files. Returns t0 as Obs.
+def _extract_flowed_energy_density(path, prefix, dtr_read, xmin, spatial_extent, postfix='ms', **kwargs):
+    """Extract a dictionary with the flowed Yang-Mills action density from given .ms.dat files.
+    Returns a dictionary with Obs as values and flow times as keys.
 
     It is assumed that all boundary effects have
     sufficiently decayed at x0=xmin.
-    The data around the zero crossing of t^2<E> - 0.3
-    is fitted with a linear function
-    from which the exact root is extracted.
 
     It is assumed that one measurement is performed for each config.
     If this is not the case, the resulting idl, as well as the handling
     of r_start, r_stop and r_step is wrong and the user has to correct
     this in the resulting observable.
 
     Parameters
@@ -256,17 +252,16 @@
         when reading the ms.dat files.
         Corresponds to dtr_cnfg / dtr_ms in the openQCD input file.
     xmin : int
         First timeslice where the boundary
         effects have sufficiently decayed.
     spatial_extent : int
         spatial extent of the lattice, required for normalization.
-    fit_range : int
-        Number of data points left and right of the zero
-        crossing to be included in the linear fit. (Default: 5)
+    postfix : str
+        Postfix of measurement file (Default: ms)
     r_start : list
         list which contains the first config to be read for each replicum.
     r_stop : list
         list which contains the last config to be read for each replicum.
     r_step : int
         integer that defines a fixed step size between two measurements (in units of configs)
         If not given, r_step=1 is assumed.
@@ -274,34 +269,32 @@
         If true extract the plaquette estimate of t0 instead.
     names : list
         list of names that is assigned to the data according according
         to the order in the file list. Use careful, if you do not provide file names!
     files : list
         list which contains the filenames to be read. No automatic detection of
         files performed if given.
-    plot_fit : bool
-        If true, the fit for the extraction of t0 is shown together with the data.
     assume_thermalization : bool
         If True: If the first record divided by the distance between two measurements is larger than
         1, it is assumed that this is due to thermalization and the first measurement belongs
         to the first config (default).
         If False: The config numbers are assumed to be traj_number // difference
 
     Returns
     -------
-    t0 : Obs
-        Extracted t0
+    E_dict : dictionary
+        Dictionary with the flowed action density at flow times t
     """
 
     if 'files' in kwargs:
         known_files = kwargs.get('files')
     else:
         known_files = []
 
-    ls = _find_files(path, prefix, 'ms', 'dat', known_files=known_files)
+    ls = _find_files(path, prefix, postfix, 'dat', known_files=known_files)
 
     replica = len(ls)
 
     if 'r_start' in kwargs:
         r_start = kwargs.get('r_start')
         if len(r_start) != replica:
             raise Exception('r_start does not match number of replicas')
@@ -317,15 +310,15 @@
         r_stop = [None] * replica
 
     if 'r_step' in kwargs:
         r_step = kwargs.get('r_step')
     else:
         r_step = 1
 
-    print('Extract t0 from', prefix, ',', replica, 'replica')
+    print('Extract flowed Yang-Mills action density from', prefix, ',', replica, 'replica')
 
     if 'names' in kwargs:
         rep_names = kwargs.get('names')
     else:
         rep_names = []
         for entry in ls:
             truncated_entry = entry.split('.')[0]
@@ -411,70 +404,181 @@
     if np.any([len(np.unique(np.diff(cl))) != 1 for cl in configlist]):
         raise Exception('Irregular spaced data in input file!', [len(np.unique(np.diff(cl))) for cl in configlist])
     stepsizes = [list(np.unique(np.diff(cl)))[0] for cl in configlist]
     if np.any([step != 1 for step in stepsizes]):
         warnings.warn('Stepsize between configurations is greater than one!' + str(stepsizes), RuntimeWarning)
 
     idl = [range(configlist[rep][r_start_index[rep]], configlist[rep][r_stop_index[rep]] + 1, r_step) for rep in range(replica)]
-    t2E_dict = {}
+    E_dict = {}
     for n in range(nn + 1):
         samples = []
         for nrep, rep in enumerate(Ysum):
             samples.append([])
             for cnfg in rep:
                 samples[-1].append(cnfg[n])
             samples[-1] = samples[-1][r_start_index[nrep]:r_stop_index[nrep] + 1][::r_step]
         new_obs = Obs(samples, rep_names, idl=idl)
-        t2E_dict[n * dn * eps] = (n * dn * eps) ** 2 * new_obs / (spatial_extent ** 3) - 0.3
+        E_dict[n * dn * eps] = new_obs / (spatial_extent ** 3)
+
+    return E_dict
+
+
+def extract_t0(path, prefix, dtr_read, xmin, spatial_extent, fit_range=5, postfix='ms', c=0.3, **kwargs):
+    """Extract t0/a^2 from given .ms.dat files. Returns t0 as Obs.
+
+    It is assumed that all boundary effects have
+    sufficiently decayed at x0=xmin.
+    The data around the zero crossing of t^2<E> - c (where c=0.3 by default)
+    is fitted with a linear function
+    from which the exact root is extracted.
+
+    It is assumed that one measurement is performed for each config.
+    If this is not the case, the resulting idl, as well as the handling
+    of r_start, r_stop and r_step is wrong and the user has to correct
+    this in the resulting observable.
+
+    Parameters
+    ----------
+    path : str
+        Path to .ms.dat files
+    prefix : str
+        Ensemble prefix
+    dtr_read : int
+        Determines how many trajectories should be skipped
+        when reading the ms.dat files.
+        Corresponds to dtr_cnfg / dtr_ms in the openQCD input file.
+    xmin : int
+        First timeslice where the boundary
+        effects have sufficiently decayed.
+    spatial_extent : int
+        spatial extent of the lattice, required for normalization.
+    fit_range : int
+        Number of data points left and right of the zero
+        crossing to be included in the linear fit. (Default: 5)
+    postfix : str
+        Postfix of measurement file (Default: ms)
+    c: float
+        Constant that defines the flow scale. Default 0.3 for t_0, choose 2./3 for t_1.
+    r_start : list
+        list which contains the first config to be read for each replicum.
+    r_stop : list
+        list which contains the last config to be read for each replicum.
+    r_step : int
+        integer that defines a fixed step size between two measurements (in units of configs)
+        If not given, r_step=1 is assumed.
+    plaquette : bool
+        If true extract the plaquette estimate of t0 instead.
+    names : list
+        list of names that is assigned to the data according according
+        to the order in the file list. Use careful, if you do not provide file names!
+    files : list
+        list which contains the filenames to be read. No automatic detection of
+        files performed if given.
+    plot_fit : bool
+        If true, the fit for the extraction of t0 is shown together with the data.
+    assume_thermalization : bool
+        If True: If the first record divided by the distance between two measurements is larger than
+        1, it is assumed that this is due to thermalization and the first measurement belongs
+        to the first config (default).
+        If False: The config numbers are assumed to be traj_number // difference
 
-    zero_crossing = np.argmax(np.array(
-        [o.value for o in t2E_dict.values()]) > 0.0)
+    Returns
+    -------
+    t0 : Obs
+        Extracted t0
+    """
+
+    E_dict = _extract_flowed_energy_density(path, prefix, dtr_read, xmin, spatial_extent, postfix, **kwargs)
+    t2E_dict = {}
+    for t in sorted(E_dict.keys()):
+        t2E_dict[t] = t ** 2 * E_dict[t] - c
+
+    return fit_t0(t2E_dict, fit_range, plot_fit=kwargs.get('plot_fit'))
+
+
+def extract_w0(path, prefix, dtr_read, xmin, spatial_extent, fit_range=5, postfix='ms', c=0.3, **kwargs):
+    """Extract w0/a from given .ms.dat files. Returns w0 as Obs.
+
+    It is assumed that all boundary effects have
+    sufficiently decayed at x0=xmin.
+    The data around the zero crossing of t d(t^2<E>)/dt -  (where c=0.3 by default)
+    is fitted with a linear function
+    from which the exact root is extracted.
+
+    It is assumed that one measurement is performed for each config.
+    If this is not the case, the resulting idl, as well as the handling
+    of r_start, r_stop and r_step is wrong and the user has to correct
+    this in the resulting observable.
+
+    Parameters
+    ----------
+    path : str
+        Path to .ms.dat files
+    prefix : str
+        Ensemble prefix
+    dtr_read : int
+        Determines how many trajectories should be skipped
+        when reading the ms.dat files.
+        Corresponds to dtr_cnfg / dtr_ms in the openQCD input file.
+    xmin : int
+        First timeslice where the boundary
+        effects have sufficiently decayed.
+    spatial_extent : int
+        spatial extent of the lattice, required for normalization.
+    fit_range : int
+        Number of data points left and right of the zero
+        crossing to be included in the linear fit. (Default: 5)
+    postfix : str
+        Postfix of measurement file (Default: ms)
+    c: float
+        Constant that defines the flow scale. Default 0.3 for w_0, choose 2./3 for w_1.
+    r_start : list
+        list which contains the first config to be read for each replicum.
+    r_stop : list
+        list which contains the last config to be read for each replicum.
+    r_step : int
+        integer that defines a fixed step size between two measurements (in units of configs)
+        If not given, r_step=1 is assumed.
+    plaquette : bool
+        If true extract the plaquette estimate of w0 instead.
+    names : list
+        list of names that is assigned to the data according according
+        to the order in the file list. Use careful, if you do not provide file names!
+    files : list
+        list which contains the filenames to be read. No automatic detection of
+        files performed if given.
+    plot_fit : bool
+        If true, the fit for the extraction of w0 is shown together with the data.
+    assume_thermalization : bool
+        If True: If the first record divided by the distance between two measurements is larger than
+        1, it is assumed that this is due to thermalization and the first measurement belongs
+        to the first config (default).
+        If False: The config numbers are assumed to be traj_number // difference
+
+    Returns
+    -------
+    w0 : Obs
+        Extracted w0
+    """
+
+    E_dict = _extract_flowed_energy_density(path, prefix, dtr_read, xmin, spatial_extent, postfix, **kwargs)
+
+    ftimes = sorted(E_dict.keys())
+
+    t2E_dict = {}
+    for t in ftimes:
+        t2E_dict[t] = t ** 2 * E_dict[t]
 
-    x = list(t2E_dict.keys())[zero_crossing - fit_range:
-                              zero_crossing + fit_range]
-    y = list(t2E_dict.values())[zero_crossing - fit_range:
-                                zero_crossing + fit_range]
-    [o.gamma_method() for o in y]
-
-    fit_result = fit_lin(x, y)
-
-    if kwargs.get('plot_fit'):
-        plt.figure()
-        gs = gridspec.GridSpec(2, 1, height_ratios=[3, 1], wspace=0.0, hspace=0.0)
-        ax0 = plt.subplot(gs[0])
-        xmore = list(t2E_dict.keys())[zero_crossing - fit_range - 2: zero_crossing + fit_range + 2]
-        ymore = list(t2E_dict.values())[zero_crossing - fit_range - 2: zero_crossing + fit_range + 2]
-        [o.gamma_method() for o in ymore]
-        ax0.errorbar(xmore, [yi.value for yi in ymore], yerr=[yi.dvalue for yi in ymore], fmt='x')
-        xplot = np.linspace(np.min(x), np.max(x))
-        yplot = [fit_result[0] + fit_result[1] * xi for xi in xplot]
-        [yi.gamma_method() for yi in yplot]
-        ax0.fill_between(xplot, y1=[yi.value - yi.dvalue for yi in yplot], y2=[yi.value + yi.dvalue for yi in yplot])
-        retval = (-fit_result[0] / fit_result[1])
-        retval.gamma_method()
-        ylim = ax0.get_ylim()
-        ax0.fill_betweenx(ylim, x1=retval.value - retval.dvalue, x2=retval.value + retval.dvalue, color='gray', alpha=0.4)
-        ax0.set_ylim(ylim)
-        ax0.set_ylabel(r'$t^2 \langle E(t) \rangle - 0.3 $')
-        xlim = ax0.get_xlim()
-
-        fit_res = [fit_result[0] + fit_result[1] * xi for xi in x]
-        residuals = (np.asarray([o.value for o in y]) - [o.value for o in fit_res]) / np.asarray([o.dvalue for o in y])
-        ax1 = plt.subplot(gs[1])
-        ax1.plot(x, residuals, 'ko', ls='none', markersize=5)
-        ax1.tick_params(direction='out')
-        ax1.tick_params(axis="x", bottom=True, top=True, labelbottom=True)
-        ax1.axhline(y=0.0, ls='--', color='k')
-        ax1.fill_between(xlim, -1.0, 1.0, alpha=0.1, facecolor='k')
-        ax1.set_xlim(xlim)
-        ax1.set_ylabel('Residuals')
-        ax1.set_xlabel(r'$t/a^2$')
+    tdtt2E_dict = {}
+    tdtt2E_dict[ftimes[0]] = ftimes[0] * (t2E_dict[ftimes[1]] - t2E_dict[ftimes[0]]) / (ftimes[1] - ftimes[0]) - c
+    for i in range(1, len(ftimes) - 1):
+        tdtt2E_dict[ftimes[i]] = ftimes[i] * (t2E_dict[ftimes[i + 1]] - t2E_dict[ftimes[i - 1]]) / (ftimes[i + 1] - ftimes[i - 1]) - c
+    tdtt2E_dict[ftimes[-1]] = ftimes[-1] * (t2E_dict[ftimes[-1]] - t2E_dict[ftimes[-2]]) / (ftimes[-1] - ftimes[-2]) - c
 
-        plt.draw()
-    return -fit_result[0] / fit_result[1]
+    return np.sqrt(fit_t0(tdtt2E_dict, fit_range, plot_fit=kwargs.get('plot_fit'), observable='w0'))
 
 
 def _parse_array_openQCD2(d, n, size, wa, quadrupel=False):
     arr = []
     if d == 2:
         for i in range(n[0]):
             tmp = wa[i * n[1]:(i + 1) * n[1]]
```

### Comparing `pyerrors-2.7.0/pyerrors/input/pandas.py` & `pyerrors-2.8.0/pyerrors/input/pandas.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import warnings
 import gzip
 import sqlite3
 import pandas as pd
 from ..obs import Obs
 from ..correlators import Corr
 from .json import create_json_string, import_json_string
+import numpy as np
 
 
 def to_sql(df, table_name, db, if_exists='fail', gz=True, **kwargs):
     """Write DataFrame including Obs or Corr valued columns to sqlite database.
 
     Parameters
     ----------
@@ -72,14 +73,21 @@
     gz : bool
         If True, the output is a gzipped csv file. If False, the output is a csv file.
 
     Returns
     -------
     None
     """
+    for column in df:
+        serialize = _need_to_serialize(df[column])
+        if not serialize:
+            if all(isinstance(entry, (int, np.integer, float, np.floating)) for entry in df[column]):
+                if any([np.isnan(entry) for entry in df[column]]):
+                    warnings.warn("nan value in column " + column + " will be replaced by None", UserWarning)
+
     out = _serialize_df(df, gz=False)
 
     if not fname.endswith('.csv'):
         fname += '.csv'
 
     if gz is True:
         if not fname.endswith('.gz'):
@@ -110,19 +118,19 @@
     if not fname.endswith('.csv') and not fname.endswith('.gz'):
         fname += '.csv'
 
     if gz is True:
         if not fname.endswith('.gz'):
             fname += '.gz'
         with gzip.open(fname) as f:
-            re_import = pd.read_csv(f)
+            re_import = pd.read_csv(f, keep_default_na=False)
     else:
         if fname.endswith('.gz'):
             warnings.warn("Trying to read from %s without unzipping!" % fname, UserWarning)
-        re_import = pd.read_csv(fname)
+        re_import = pd.read_csv(fname, keep_default_na=False)
 
     return _deserialize_df(re_import, auto_gamma=auto_gamma)
 
 
 def _serialize_df(df, gz=False):
     """Serializes all Obs or Corr valued columns into json strings according to the pyerrors json specification.
 
@@ -131,25 +139,20 @@
     df : pandas.DataFrame
         DataFrame to be serilized.
     gz: bool
         gzip the json string representation. Default False.
     """
     out = df.copy()
     for column in out:
-        serialize = False
-        if isinstance(out[column][0], (Obs, Corr)):
-            serialize = True
-        elif isinstance(out[column][0], list):
-            if all(isinstance(o, Obs) for o in out[column][0]):
-                serialize = True
+        serialize = _need_to_serialize(out[column])
 
         if serialize is True:
-            out[column] = out[column].transform(lambda x: create_json_string(x, indent=0))
+            out[column] = out[column].transform(lambda x: create_json_string(x, indent=0) if x is not None else None)
             if gz is True:
-                out[column] = out[column].transform(lambda x: gzip.compress(x.encode('utf-8')))
+                out[column] = out[column].transform(lambda x: gzip.compress((x if x is not None else '').encode('utf-8')))
     return out
 
 
 def _deserialize_df(df, auto_gamma=False):
     """Deserializes all pyerrors json strings into Obs or Corr objects according to the pyerrors json specification.
 
     Parameters
@@ -164,16 +167,33 @@
     ------
     In case any column of the DataFrame is gzipped it is gunzipped in the process.
     """
     for column in df.select_dtypes(include="object"):
         if isinstance(df[column][0], bytes):
             if df[column][0].startswith(b"\x1f\x8b\x08\x00"):
                 df[column] = df[column].transform(lambda x: gzip.decompress(x).decode('utf-8'))
-        if isinstance(df[column][0], str):
-            if '"program":' in df[column][0][:20]:
-                df[column] = df[column].transform(lambda x: import_json_string(x, verbose=False))
+        df = df.replace({r'^$': None}, regex=True)
+        i = 0
+        while df[column][i] is None:
+            i += 1
+        if isinstance(df[column][i], str):
+            if '"program":' in df[column][i][:20]:
+                df[column] = df[column].transform(lambda x: import_json_string(x, verbose=False) if x is not None else None)
                 if auto_gamma is True:
-                    if isinstance(df[column][0], list):
-                        df[column].apply(lambda x: [o.gm() for o in x])
+                    if isinstance(df[column][i], list):
+                        df[column].apply(lambda x: [o.gm() if o is not None else x for o in x])
                     else:
-                        df[column].apply(lambda x: x.gamma_method())
+                        df[column].apply(lambda x: x.gm() if x is not None else x)
     return df
+
+
+def _need_to_serialize(col):
+    serialize = False
+    i = 0
+    while col[i] is None:
+        i += 1
+    if isinstance(col[i], (Obs, Corr)):
+        serialize = True
+    elif isinstance(col[i], list):
+        if all(isinstance(o, Obs) for o in col[i]):
+            serialize = True
+    return serialize
```

### Comparing `pyerrors-2.7.0/pyerrors/input/sfcf.py` & `pyerrors-2.8.0/pyerrors/input/sfcf.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/pyerrors/input/utils.py` & `pyerrors-2.8.0/pyerrors/input/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,38 +14,40 @@
 
     Returns
     -------
     ll: list
         sorted list
     """
     if len(ll) > 1:
+        sorted = False
         r_pattern = r'r(\d+)'
         id_pattern = r'id(\d+)'
 
         # sort list by id first
         if all([re.search(id_pattern, entry) for entry in ll]):
             ll.sort(key=lambda x: int(re.findall(id_pattern, x)[0]))
+            sorted = True
         # then by replikum
         if all([re.search(r_pattern, entry) for entry in ll]):
             ll.sort(key=lambda x: int(re.findall(r_pattern, x)[0]))
+            sorted = True
         # as the rearrangements by one key let the other key untouched, the list is sorted now
 
-        else:
+        if not sorted:
             # fallback
             sames = ''
-            if len(ll) > 1:
-                for i in range(len(ll[0])):
-                    checking = ll[0][i]
-                    for rn in ll[1:]:
-                        is_same = (rn[i] == checking)
-                    if is_same:
-                        sames += checking
-                    else:
-                        break
-                print("Using prefix:", ll[0][len(sames):])
+            for i in range(len(ll[0])):
+                checking = ll[0][i]
+                for rn in ll[1:]:
+                    is_same = (rn[i] == checking)
+                if is_same:
+                    sames += checking
+                else:
+                    break
+            print("Using prefix:", sames)
             ll.sort(key=lambda x: int(re.findall(r'\d+', x[len(sames):])[0]))
     return ll
 
 
 def check_idl(idl, che):
     """Checks if list of configurations is contained in an idl
```

### Comparing `pyerrors-2.7.0/pyerrors/linalg.py` & `pyerrors-2.8.0/pyerrors/linalg.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/pyerrors/misc.py` & `pyerrors-2.8.0/pyerrors/misc.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/pyerrors/mpm.py` & `pyerrors-2.8.0/pyerrors/mpm.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/pyerrors/obs.py` & `pyerrors-2.8.0/pyerrors/obs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import warnings
 import hashlib
 import pickle
-from math import gcd
-from functools import reduce
 import numpy as np
 import autograd.numpy as anp  # Thinly-wrapped numpy
 from autograd import jacobian
 import matplotlib.pyplot as plt
 from scipy.stats import skew, skewtest, kurtosis, kurtosistest
 import numdifftools as nd
 from itertools import groupby
@@ -234,107 +232,96 @@
                         getattr(self, kwarg_name)[e_name] = getattr(Obs, kwarg_name + '_global')
 
         _parse_kwarg('S')
         _parse_kwarg('tau_exp')
         _parse_kwarg('N_sigma')
 
         for e, e_name in enumerate(self.mc_names):
+            gapsize = _determine_gap(self, e_content, e_name)
+
             r_length = []
             for r_name in e_content[e_name]:
                 if isinstance(self.idl[r_name], range):
-                    r_length.append(len(self.idl[r_name]))
+                    r_length.append(len(self.idl[r_name]) * self.idl[r_name].step // gapsize)
                 else:
-                    r_length.append((self.idl[r_name][-1] - self.idl[r_name][0] + 1))
+                    r_length.append((self.idl[r_name][-1] - self.idl[r_name][0] + 1) // gapsize)
 
             e_N = np.sum([self.shape[r_name] for r_name in e_content[e_name]])
             w_max = max(r_length) // 2
             e_gamma[e_name] = np.zeros(w_max)
             self.e_rho[e_name] = np.zeros(w_max)
             self.e_drho[e_name] = np.zeros(w_max)
 
             for r_name in e_content[e_name]:
-                e_gamma[e_name] += self._calc_gamma(self.deltas[r_name], self.idl[r_name], self.shape[r_name], w_max, fft)
+                e_gamma[e_name] += self._calc_gamma(self.deltas[r_name], self.idl[r_name], self.shape[r_name], w_max, fft, gapsize)
 
             gamma_div = np.zeros(w_max)
             for r_name in e_content[e_name]:
-                gamma_div += self._calc_gamma(np.ones((self.shape[r_name])), self.idl[r_name], self.shape[r_name], w_max, fft)
+                gamma_div += self._calc_gamma(np.ones((self.shape[r_name])), self.idl[r_name], self.shape[r_name], w_max, fft, gapsize)
             gamma_div[gamma_div < 1] = 1.0
             e_gamma[e_name] /= gamma_div[:w_max]
 
             if np.abs(e_gamma[e_name][0]) < 10 * np.finfo(float).tiny:  # Prevent division by zero
                 self.e_tauint[e_name] = 0.5
                 self.e_dtauint[e_name] = 0.0
                 self.e_dvalue[e_name] = 0.0
                 self.e_ddvalue[e_name] = 0.0
                 self.e_windowsize[e_name] = 0
                 continue
 
-            gaps = []
-            for r_name in e_content[e_name]:
-                if isinstance(self.idl[r_name], range):
-                    gaps.append(1)
-                else:
-                    gaps.append(np.min(np.diff(self.idl[r_name])))
-
-            if not np.all([gi == gaps[0] for gi in gaps]):
-                raise Exception(f"Replica for ensemble {e_name} are not equally spaced.", gaps)
-            else:
-                gapsize = gaps[0]
-
             self.e_rho[e_name] = e_gamma[e_name][:w_max] / e_gamma[e_name][0]
             self.e_n_tauint[e_name] = np.cumsum(np.concatenate(([0.5], self.e_rho[e_name][1:])))
             # Make sure no entry of tauint is smaller than 0.5
             self.e_n_tauint[e_name][self.e_n_tauint[e_name] <= 0.5] = 0.5 + np.finfo(np.float64).eps
             # hep-lat/0306017 eq. (42)
-            self.e_n_dtauint[e_name] = self.e_n_tauint[e_name] * 2 * np.sqrt(np.abs(np.arange(w_max) / gapsize + 0.5 - self.e_n_tauint[e_name]) / e_N)
+            self.e_n_dtauint[e_name] = self.e_n_tauint[e_name] * 2 * np.sqrt(np.abs(np.arange(w_max) + 0.5 - self.e_n_tauint[e_name]) / e_N)
             self.e_n_dtauint[e_name][0] = 0.0
 
             def _compute_drho(i):
                 tmp = (self.e_rho[e_name][i + 1:w_max]
-                       + np.concatenate([self.e_rho[e_name][i - 1:None if i - w_max // 2 < 0 else 2 * (i - w_max // 2):-1],
+                       + np.concatenate([self.e_rho[e_name][i - 1:None if i - w_max // 2 <= 0 else 2 * (i - w_max // 2):-1],
                                          self.e_rho[e_name][1:max(1, w_max - 2 * i)]])
                        - 2 * self.e_rho[e_name][i] * self.e_rho[e_name][1:w_max - i])
                 self.e_drho[e_name][i] = np.sqrt(np.sum(tmp ** 2) / e_N)
 
             if self.tau_exp[e_name] > 0:
-                _compute_drho(gapsize)
+                _compute_drho(1)
                 texp = self.tau_exp[e_name]
                 # Critical slowing down analysis
                 if w_max // 2 <= 1:
                     raise Exception("Need at least 8 samples for tau_exp error analysis")
-                for n in range(gapsize, w_max // 2, gapsize):
-                    _compute_drho(n + gapsize)
+                for n in range(1, w_max // 2):
+                    _compute_drho(n + 1)
                     if (self.e_rho[e_name][n] - self.N_sigma[e_name] * self.e_drho[e_name][n]) < 0 or n >= w_max // 2 - 2:
                         # Bias correction hep-lat/0306017 eq. (49) included
-                        self.e_tauint[e_name] = self.e_n_tauint[e_name][n] * (1 + (2 * n / gapsize + 1) / e_N) / (1 + 1 / e_N) + texp * np.abs(self.e_rho[e_name][n + 1])  # The absolute makes sure, that the tail contribution is always positive
+                        self.e_tauint[e_name] = self.e_n_tauint[e_name][n] * (1 + (2 * n + 1) / e_N) / (1 + 1 / e_N) + texp * np.abs(self.e_rho[e_name][n + 1])  # The absolute makes sure, that the tail contribution is always positive
                         self.e_dtauint[e_name] = np.sqrt(self.e_n_dtauint[e_name][n] ** 2 + texp ** 2 * self.e_drho[e_name][n + 1] ** 2)
                         # Error of tau_exp neglected so far, missing term: self.e_rho[e_name][n + 1] ** 2 * d_tau_exp ** 2
                         self.e_dvalue[e_name] = np.sqrt(2 * self.e_tauint[e_name] * e_gamma[e_name][0] * (1 + 1 / e_N) / e_N)
-                        self.e_ddvalue[e_name] = self.e_dvalue[e_name] * np.sqrt((n / gapsize + 0.5) / e_N)
+                        self.e_ddvalue[e_name] = self.e_dvalue[e_name] * np.sqrt((n + 0.5) / e_N)
                         self.e_windowsize[e_name] = n
                         break
             else:
                 if self.S[e_name] == 0.0:
                     self.e_tauint[e_name] = 0.5
                     self.e_dtauint[e_name] = 0.0
                     self.e_dvalue[e_name] = np.sqrt(e_gamma[e_name][0] / (e_N - 1))
                     self.e_ddvalue[e_name] = self.e_dvalue[e_name] * np.sqrt(0.5 / e_N)
                     self.e_windowsize[e_name] = 0
                 else:
                     # Standard automatic windowing procedure
-                    tau = self.S[e_name] / np.log((2 * self.e_n_tauint[e_name][gapsize::gapsize] + 1) / (2 * self.e_n_tauint[e_name][gapsize::gapsize] - 1))
+                    tau = self.S[e_name] / np.log((2 * self.e_n_tauint[e_name][1:] + 1) / (2 * self.e_n_tauint[e_name][1:] - 1))
                     g_w = np.exp(- np.arange(1, len(tau) + 1) / tau) - tau / np.sqrt(np.arange(1, len(tau) + 1) * e_N)
-                    for n in range(1, w_max // gapsize):
-                        if g_w[n - 1] < 0 or n >= w_max // gapsize - 1:
-                            _compute_drho(gapsize * n)
-                            n *= gapsize
-                            self.e_tauint[e_name] = self.e_n_tauint[e_name][n] * (1 + (2 * n / gapsize + 1) / e_N) / (1 + 1 / e_N)  # Bias correction hep-lat/0306017 eq. (49)
+                    for n in range(1, w_max):
+                        if g_w[n - 1] < 0 or n >= w_max - 1:
+                            _compute_drho(n)
+                            self.e_tauint[e_name] = self.e_n_tauint[e_name][n] * (1 + (2 * n + 1) / e_N) / (1 + 1 / e_N)  # Bias correction hep-lat/0306017 eq. (49)
                             self.e_dtauint[e_name] = self.e_n_dtauint[e_name][n]
                             self.e_dvalue[e_name] = np.sqrt(2 * self.e_tauint[e_name] * e_gamma[e_name][0] * (1 + 1 / e_N) / e_N)
-                            self.e_ddvalue[e_name] = self.e_dvalue[e_name] * np.sqrt((n / gapsize + 0.5) / e_N)
+                            self.e_ddvalue[e_name] = self.e_dvalue[e_name] * np.sqrt((n + 0.5) / e_N)
                             self.e_windowsize[e_name] = n
                             break
 
             self._dvalue += self.e_dvalue[e_name] ** 2
             self.ddvalue += (self.e_dvalue[e_name] * self.e_ddvalue[e_name]) ** 2
 
         for e_name in self.cov_names:
@@ -347,15 +334,15 @@
             self.ddvalue = 0.0
         else:
             self.ddvalue = np.sqrt(self.ddvalue) / self._dvalue
         return
 
     gm = gamma_method
 
-    def _calc_gamma(self, deltas, idx, shape, w_max, fft):
+    def _calc_gamma(self, deltas, idx, shape, w_max, fft, gapsize):
         """Calculate Gamma_{AA} from the deltas, which are defined on idx.
            idx is assumed to be a contiguous range (possibly with a stepsize != 1)
 
         Parameters
         ----------
         deltas : list
             List of fluctuations
@@ -364,17 +351,20 @@
         shape : int
             Number of configurations in idx.
         w_max : int
             Upper bound for the summation window.
         fft : bool
             determines whether the fft algorithm is used for the computation
             of the autocorrelation function.
+        gapsize : int
+            The target distance between two configurations. If longer distances
+            are found in idx, the data is expanded.
         """
         gamma = np.zeros(w_max)
-        deltas = _expand_deltas(deltas, idx, shape)
+        deltas = _expand_deltas(deltas, idx, shape, gapsize)
         new_shape = len(deltas)
         if fft:
             max_gamma = min(new_shape, w_max)
             # The padding for the fft has to be even
             padding = new_shape + max_gamma + (new_shape + max_gamma) % 2
             gamma[:max_gamma] += np.fft.irfft(np.abs(np.fft.rfft(deltas, padding)) ** 2)[:max_gamma]
         else:
@@ -402,18 +392,15 @@
             else:
                 percentage = np.abs(self._dvalue / self.value) * 100
             print('Result\t %3.8e +/- %3.8e +/- %3.8e (%3.3f%%)' % (self.value, self._dvalue, self.ddvalue, percentage))
             if len(self.e_names) > 1:
                 print(' Ensemble errors:')
             e_content = self.e_content
             for e_name in self.mc_names:
-                if isinstance(self.idl[e_content[e_name][0]], range):
-                    gap = self.idl[e_content[e_name][0]].step
-                else:
-                    gap = np.min(np.diff(self.idl[e_content[e_name][0]]))
+                gap = _determine_gap(self, e_content, e_name)
 
                 if len(self.e_names) > 1:
                     print('', e_name, '\t %3.6e +/- %3.6e' % (self.e_dvalue[e_name], self.e_ddvalue[e_name]))
                 tau_string = " \N{GREEK SMALL LETTER TAU}_int\t " + _format_uncertainty(self.e_tauint[e_name], self.e_dtauint[e_name])
                 tau_string += f" in units of {gap} config"
                 if gap > 1:
                     tau_string += "s"
@@ -598,15 +585,15 @@
             plt.figure()
             r_length = []
             tmp = []
             tmp_expanded = []
             for r, r_name in enumerate(self.e_content[e_name]):
                 tmp.append(self.deltas[r_name] + self.r_values[r_name])
                 if expand:
-                    tmp_expanded.append(_expand_deltas(self.deltas[r_name], list(self.idl[r_name]), self.shape[r_name]) + self.r_values[r_name])
+                    tmp_expanded.append(_expand_deltas(self.deltas[r_name], list(self.idl[r_name]), self.shape[r_name], 1) + self.r_values[r_name])
                     r_length.append(len(tmp_expanded[-1]))
                 else:
                     r_length.append(len(tmp[-1]))
             e_N = np.sum(r_length)
             x = np.arange(e_N)
             y_test = np.concatenate(tmp, axis=0)
             if expand:
@@ -702,14 +689,23 @@
 
     def __repr__(self):
         return 'Obs[' + str(self) + ']'
 
     def __str__(self):
         return _format_uncertainty(self.value, self._dvalue)
 
+    def __format__(self, format_type):
+        my_str = _format_uncertainty(self.value, self._dvalue,
+                                     significance=int(float(format_type.replace("+", "").replace("-", ""))))
+        for char in ["+", " "]:
+            if format_type.startswith(char):
+                if my_str[0] != "-":
+                    my_str = char + my_str
+        return my_str
+
     def __hash__(self):
         hash_tuple = (np.array([self.value]).astype(np.float32).data.tobytes(),)
         hash_tuple += tuple([o.astype(np.float32).data.tobytes() for o in self.deltas.values()])
         hash_tuple += tuple([np.array([o.errsq()]).astype(np.float32).data.tobytes() for o in self.covobs.values()])
         hash_tuple += tuple([o.encode() for o in self.names])
         m = hashlib.md5()
         [m.update(o) for o in hash_tuple]
@@ -976,107 +972,104 @@
     def __str__(self):
         return '(' + str(self.real) + int(self.imag >= 0.0) * '+' + str(self.imag) + 'j)'
 
     def __repr__(self):
         return 'CObs[' + str(self) + ']'
 
 
-def _format_uncertainty(value, dvalue):
+def _format_uncertainty(value, dvalue, significance=2):
     """Creates a string of a value and its error in paranthesis notation, e.g., 13.02(45)"""
-    if dvalue == 0.0:
+    if dvalue == 0.0 or (not np.isfinite(dvalue)):
         return str(value)
+    if not isinstance(significance, int):
+        raise TypeError("significance needs to be an integer.")
+    if significance < 1:
+        raise ValueError("significance needs to be larger than zero.")
     fexp = np.floor(np.log10(dvalue))
     if fexp < 0.0:
-        return '{:{form}}({:2.0f})'.format(value, dvalue * 10 ** (-fexp + 1), form='.' + str(-int(fexp) + 1) + 'f')
+        return '{:{form}}({:1.0f})'.format(value, dvalue * 10 ** (-fexp + significance - 1), form='.' + str(-int(fexp) + significance - 1) + 'f')
     elif fexp == 0.0:
-        return '{:.1f}({:1.1f})'.format(value, dvalue)
+        return f"{value:.{significance - 1}f}({dvalue:1.{significance - 1}f})"
     else:
-        return '{:.0f}({:2.0f})'.format(value, dvalue)
+        return f"{value:.{max(0, int(significance - fexp - 1))}f}({dvalue:2.{max(0, int(significance - fexp - 1))}f})"
 
 
-def _expand_deltas(deltas, idx, shape):
-    """Expand deltas defined on idx to a regular, contiguous range, where holes are filled by 0.
-       If idx is of type range, the deltas are not changed
+def _expand_deltas(deltas, idx, shape, gapsize):
+    """Expand deltas defined on idx to a regular range with spacing gapsize between two
+       configurations and where holes are filled by 0.
+       If idx is of type range, the deltas are not changed if the idx.step == gapsize.
 
     Parameters
     ----------
     deltas : list
         List of fluctuations
     idx : list
         List or range of configs on which the deltas are defined, has to be sorted in ascending order.
     shape : int
         Number of configs in idx.
+    gapsize : int
+        The target distance between two configurations. If longer distances
+        are found in idx, the data is expanded.
     """
     if isinstance(idx, range):
-        return deltas
-    else:
-        ret = np.zeros(idx[-1] - idx[0] + 1)
-        for i in range(shape):
-            ret[idx[i] - idx[0]] = deltas[i]
-        return ret
+        if (idx.step == gapsize):
+            return deltas
+    ret = np.zeros((idx[-1] - idx[0] + gapsize) // gapsize)
+    for i in range(shape):
+        ret[(idx[i] - idx[0]) // gapsize] = deltas[i]
+    return ret
 
 
 def _merge_idx(idl):
-    """Returns the union of all lists in idl as sorted list
+    """Returns the union of all lists in idl as range or sorted list
 
     Parameters
     ----------
     idl : list
         List of lists or ranges.
     """
 
-    # Use groupby to efficiently check whether all elements of idl are identical
-    try:
-        g = groupby(idl)
-        if next(g, True) and not next(g, False):
-            return idl[0]
-    except Exception:
-        pass
+    if _check_lists_equal(idl):
+        return idl[0]
 
-    if np.all([type(idx) is range for idx in idl]):
-        if len(set([idx[0] for idx in idl])) == 1:
-            idstart = min([idx.start for idx in idl])
-            idstop = max([idx.stop for idx in idl])
-            idstep = min([idx.step for idx in idl])
-            return range(idstart, idstop, idstep)
+    idunion = sorted(set().union(*idl))
 
-    return sorted(set().union(*idl))
+    # Check whether idunion can be expressed as range
+    idrange = range(idunion[0], idunion[-1] + 1, idunion[1] - idunion[0])
+    idtest = [list(idrange), idunion]
+    if _check_lists_equal(idtest):
+        return idrange
+
+    return idunion
 
 
 def _intersection_idx(idl):
-    """Returns the intersection of all lists in idl as sorted list
+    """Returns the intersection of all lists in idl as range or sorted list
 
     Parameters
     ----------
     idl : list
         List of lists or ranges.
     """
 
-    def _lcm(*args):
-        """Returns the lowest common multiple of args.
+    if _check_lists_equal(idl):
+        return idl[0]
 
-        From python 3.9 onwards the math library contains an lcm function."""
-        return reduce(lambda a, b: a * b // gcd(a, b), args)
+    idinter = sorted(set.intersection(*[set(o) for o in idl]))
 
-    # Use groupby to efficiently check whether all elements of idl are identical
+    # Check whether idinter can be expressed as range
     try:
-        g = groupby(idl)
-        if next(g, True) and not next(g, False):
-            return idl[0]
-    except Exception:
+        idrange = range(idinter[0], idinter[-1] + 1, idinter[1] - idinter[0])
+        idtest = [list(idrange), idinter]
+        if _check_lists_equal(idtest):
+            return idrange
+    except IndexError:
         pass
 
-    if np.all([type(idx) is range for idx in idl]):
-        if len(set([idx[0] for idx in idl])) == 1:
-            idstart = max([idx.start for idx in idl])
-            idstop = min([idx.stop for idx in idl])
-            idstep = _lcm(*[idx.step for idx in idl])
-            return range(idstart, idstop, idstep)
-
-    return sorted(set.intersection(*[set(o) for o in idl]))
+    return idinter
 
 
 def _expand_deltas_for_merge(deltas, idx, shape, new_idx):
     """Expand deltas defined on idx to the list of configs that is defined by new_idx.
        New, empty entries are filled by 0. If idx and new_idx are of type range, the smallest
        common divisor of the step sizes is used as new step size.
 
@@ -1289,21 +1282,16 @@
         Has to be a subset of idx_old.
     """
     if not len(deltas) == len(idx_old):
         raise Exception('Length of deltas and idx_old have to be the same: %d != %d' % (len(deltas), len(idx_old)))
     if type(idx_old) is range and type(idx_new) is range:
         if idx_old == idx_new:
             return deltas
-    # Use groupby to efficiently check whether all elements of idx_old and idx_new are identical
-    try:
-        g = groupby([idx_old, idx_new])
-        if next(g, True) and not next(g, False):
-            return deltas
-    except Exception:
-        pass
+    if _check_lists_equal([idx_old, idx_new]):
+        return deltas
     indices = np.intersect1d(idx_old, idx_new, assume_unique=True, return_indices=True)[1]
     if len(indices) < len(idx_new):
         raise Exception('Error in _reduce_deltas: Config of idx_new not in idx_old')
     return np.array(deltas)[indices]
 
 
 def reweight(weight, obs, **kwargs):
@@ -1625,7 +1613,37 @@
     for i in range(len(means)):
         ol.append(covobs_to_obs(Covobs(means[i], cov, name, pos=i, grad=grad)))
     if ol[0].covobs[name].N != len(means):
         raise Exception('You have to provide %d mean values!' % (ol[0].N))
     if len(ol) == 1:
         return ol[0]
     return ol
+
+
+def _determine_gap(o, e_content, e_name):
+    gaps = []
+    for r_name in e_content[e_name]:
+        if isinstance(o.idl[r_name], range):
+            gaps.append(o.idl[r_name].step)
+        else:
+            gaps.append(np.min(np.diff(o.idl[r_name])))
+
+    gap = min(gaps)
+    if not np.all([gi % gap == 0 for gi in gaps]):
+        raise Exception(f"Replica for ensemble {e_name} do not have a common spacing.", gaps)
+
+    return gap
+
+
+def _check_lists_equal(idl):
+    '''
+    Use groupby to efficiently check whether all elements of idl are identical.
+    Returns True if all elements are equal, otherwise False.
+
+    Parameters
+    ----------
+    idl : list of lists, ranges or np.ndarrays
+    '''
+    g = groupby([np.nditer(el) if isinstance(el, np.ndarray) else el for el in idl])
+    if next(g, True) and not next(g, False):
+        return True
+    return False
```

### Comparing `pyerrors-2.7.0/pyerrors/roots.py` & `pyerrors-2.8.0/pyerrors/roots.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/pyerrors.egg-info/PKG-INFO` & `pyerrors-2.8.0/pyerrors.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyerrors
-Version: 2.7.0
+Version: 2.8.0
 Summary: Error propagation and statistical analysis for Monte Carlo simulations
 Home-page: https://github.com/fjosw/pyerrors
 Author: Fabian Joswig
 Author-email: fabian.joswig@ed.ac.uk
 License: MIT
 Project-URL: Documentation, https://fjosw.github.io/pyerrors/pyerrors.html
 Project-URL: Bug Tracker, https://github.com/fjosw/pyerrors/issues
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-[![flake8](https://github.com/fjosw/pyerrors/actions/workflows/flake8.yml/badge.svg)](https://github.com/fjosw/pyerrors/actions/workflows/flake8.yml) [![pytest](https://github.com/fjosw/pyerrors/actions/workflows/pytest.yml/badge.svg)](https://github.com/fjosw/pyerrors/actions/workflows/pytest.yml) [![](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![arXiv](https://img.shields.io/badge/arXiv-2209.14371-b31b1b.svg)](https://arxiv.org/abs/2209.14371)
+[![pytest](https://github.com/fjosw/pyerrors/actions/workflows/pytest.yml/badge.svg)](https://github.com/fjosw/pyerrors/actions/workflows/pytest.yml) [![](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![arXiv](https://img.shields.io/badge/arXiv-2209.14371-b31b1b.svg)](https://arxiv.org/abs/2209.14371) [![DOI](https://img.shields.io/badge/DOI-10.1016%2Fj.cpc.2023.108750-blue)](https://doi.org/10.1016/j.cpc.2023.108750)
 # pyerrors
 `pyerrors` is a python framework for error computation and propagation of Markov chain Monte Carlo data from lattice field theory and statistical mechanics simulations.
 
 - **Documentation:** https://fjosw.github.io/pyerrors/pyerrors.html
 - **Examples:** https://github.com/fjosw/pyerrors/tree/develop/examples
 - **Bug reports:** https://github.com/fjosw/pyerrors/issues
```

### Comparing `pyerrors-2.7.0/pyerrors.egg-info/SOURCES.txt` & `pyerrors-2.8.0/pyerrors.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/setup.py` & `pyerrors-2.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/tests/benchmark_test.py` & `pyerrors-2.8.0/tests/benchmark_test.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/tests/correlators_test.py` & `pyerrors-2.8.0/tests/correlators_test.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/tests/covobs_test.py` & `pyerrors-2.8.0/tests/covobs_test.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/tests/data/openqcd_test/ms5_xsf_T24L16r1.ms5_xsf_dd.dat` & `pyerrors-2.8.0/tests/data/openqcd_test/ms5_xsf_T24L16r1.ms5_xsf_dd.dat`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/tests/data/openqcd_test/ms5_xsf_T24L16r2.ms5_xsf_dd.dat` & `pyerrors-2.8.0/tests/data/openqcd_test/ms5_xsf_T24L16r2.ms5_xsf_dd.dat`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/tests/data/openqcd_test/ms5_xsf_T24L16r3.ms5_xsf_dd.dat` & `pyerrors-2.8.0/tests/data/openqcd_test/ms5_xsf_T24L16r3.ms5_xsf_dd.dat`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/tests/data/openqcd_test/openqcd2r1.ms.dat` & `pyerrors-2.8.0/tests/data/openqcd_test/openqcd2r1.ms.dat`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/tests/data/openqcd_test/openqcd2r1.ms1.dat` & `pyerrors-2.8.0/tests/data/openqcd_test/openqcd2r1.ms1.dat`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/tests/data/openqcd_test/sfqcdr1.gfms.dat` & `pyerrors-2.8.0/tests/data/openqcd_test/sfqcdr1.gfms.dat`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/tests/data/sfcf_test/broken_data_c/data_c_r0/data_c_r0_n1` & `pyerrors-2.8.0/tests/data/sfcf_test/broken_data_c/data_c_r0/data_c_r0_n1`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/tests/data/sfcf_test/data_a/data_a_r0.F_V0` & `pyerrors-2.8.0/tests/data/sfcf_test/data_a/data_a_r0.F_V0`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/tests/data/sfcf_test/data_a/data_a_r0.f_1` & `pyerrors-2.8.0/tests/data/sfcf_test/data_a/data_a_r0.f_1`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/tests/data/sfcf_test/data_a/data_a_r0.f_A` & `pyerrors-2.8.0/tests/data/sfcf_test/data_a/data_a_r0.f_A`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/tests/data/sfcf_test/data_c/data_c_r0/data_c_r0_n1` & `pyerrors-2.8.0/tests/data/sfcf_test/data_c/data_c_r0/data_c_r0_n1`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/tests/data/sfcf_test/data_o/test_r0/cfg1/F_V0` & `pyerrors-2.8.0/tests/data/sfcf_test/data_o/test_r0/cfg1/F_V0`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/tests/data/sfcf_test/data_o/test_r0/cfg1/f_1` & `pyerrors-2.8.0/tests/data/sfcf_test/data_o/test_r0/cfg1/f_1`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/tests/data/sfcf_test/data_o/test_r0/cfg1/f_A` & `pyerrors-2.8.0/tests/data/sfcf_test/data_o/test_r0/cfg1/f_A`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/tests/data/sfcf_test/param/out.out` & `pyerrors-2.8.0/tests/data/sfcf_test/param/out.out`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/tests/data/sfcf_test/param/parameters_a` & `pyerrors-2.8.0/tests/data/sfcf_test/param/parameters_a`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/tests/data/sfcf_test/param/parameters_c` & `pyerrors-2.8.0/tests/data/sfcf_test/param/parameters_c`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/tests/data/sfcf_test/param/parameters_o` & `pyerrors-2.8.0/tests/data/sfcf_test/param/parameters_o`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/tests/dirac_test.py` & `pyerrors-2.8.0/tests/dirac_test.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/tests/fits_test.py` & `pyerrors-2.8.0/tests/fits_test.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/tests/json_io_test.py` & `pyerrors-2.8.0/tests/json_io_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,14 +245,18 @@
     with pytest.raises(Exception):
         jsonio.dump_dict_to_json(od, fname, description=desc)
 
     od['k'] = ['DICTOBS2']
     with pytest.raises(Exception):
         jsonio.dump_dict_to_json(od, fname, description=desc)
 
+    od = {1: 'test', False: 'True', None: 'None'}
+    jsonio.dump_dict_to_json(od, fname, description={np.int64(1): np.float64(2.444444)})
+    jsonio.dump_dict_to_json(od, fname, description=np.float32(2.444444))
+
     os.remove(fname + '.json.gz')
 
 
 def test_renorm_deriv_of_corr(tmp_path):
     c = pe.Corr([pe.pseudo_Obs(i, .1, 'test') for i in range(10)])
     c *= pe.cov_Obs(1., .1, '#ren')
     c = c.deriv()
```

### Comparing `pyerrors-2.7.0/tests/linalg_test.py` & `pyerrors-2.8.0/tests/linalg_test.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/tests/misc_test.py` & `pyerrors-2.8.0/tests/misc_test.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/tests/obs_test.py` & `pyerrors-2.8.0/tests/obs_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -533,25 +533,57 @@
     r_obs = pe.reweight(my_obs1, [my_obs1])[0]
     with pytest.warns(RuntimeWarning):
         pe.correlate(r_obs, r_obs)
 
 
 def test_merge_idx():
     assert pe.obs._merge_idx([range(10, 1010, 10), range(10, 1010, 50)]) == range(10, 1010, 10)
-    assert pe.obs._merge_idx([range(500, 6050, 50), range(500, 6250, 250)]) == range(500, 6250, 50)
+    assert isinstance(pe.obs._merge_idx([range(10, 1010, 10), range(10, 1010, 50)]), range)
+    assert pe.obs._merge_idx([range(500, 6050, 50), range(500, 6250, 250)]) == range(500, 6001, 50)
+    assert isinstance(pe.obs._merge_idx([range(500, 6050, 50), range(500, 6250, 250)]), range)
+    assert pe.obs._merge_idx([range(1, 1011, 2), range(1, 1010, 1)]) == range(1, 1010, 1)
+    assert isinstance(pe.obs._merge_idx([range(1, 1011, 2), range(1, 1010, 1)]), range)
+    assert pe.obs._merge_idx([range(1, 100, 2), range(2, 100, 2)]) == range(1, 100, 1)
+    assert isinstance(pe.obs._merge_idx([range(1, 100, 2), range(2, 100, 2)]), range)
+
+    for j in range(5):
+        idll = [range(1, int(round(np.random.uniform(300, 700))), int(round(np.random.uniform(1, 14)))) for i in range(10)]
+        assert pe.obs._merge_idx(idll) == sorted(set().union(*idll))
+
+    for j in range(5):
+        idll = [range(int(round(np.random.uniform(1, 28))), int(round(np.random.uniform(300, 700))), int(round(np.random.uniform(1, 14)))) for i in range(10)]
+        assert pe.obs._merge_idx(idll) == sorted(set().union(*idll))
+
+    idl = [list(np.arange(1, 14)) + list(range(16, 100, 4)), range(4, 604, 4), [2, 4, 5, 6, 8, 9, 12, 24], range(1, 20, 1), range(50, 789, 7)]
+    new_idx = pe.obs._merge_idx(idl)
+    assert(new_idx[-1] > new_idx[0])
+    for i in range(1, len(new_idx)):
+        assert(new_idx[i - 1] < new_idx[i])
 
 
 def test_intersection_idx():
     assert pe.obs._intersection_idx([range(1, 100), range(1, 100), range(1, 100)]) == range(1, 100)
     assert pe.obs._intersection_idx([range(1, 100, 10), range(1, 100, 2)]) == range(1, 100, 10)
     assert pe.obs._intersection_idx([range(10, 1010, 10), range(10, 1010, 50)]) == range(10, 1010, 50)
-    assert pe.obs._intersection_idx([range(500, 6050, 50), range(500, 6250, 250)]) == range(500, 6050, 250)
+    assert pe.obs._intersection_idx([range(500, 6050, 50), range(500, 6250, 250)]) == range(500, 6001, 250)
+    assert pe.obs._intersection_idx([range(1, 1011, 2), range(1, 1010, 1)]) == range(1, 1010, 2)
+    idll = [range(1, 100, 2), range(5, 105, 1)]
+    assert pe.obs._intersection_idx(idll) == range(5, 100, 2)
+    assert isinstance(pe.obs._intersection_idx(idll), range)
+    idll = [range(1, 100, 2), list(range(5, 105, 1))]
+    assert pe.obs._intersection_idx(idll) == range(5, 100, 2)
+    assert isinstance(pe.obs._intersection_idx(idll), range)
 
     for ids in [[list(range(1, 80, 3)), list(range(1, 100, 2))], [range(1, 80, 3), range(1, 100, 2), range(1, 100, 7)]]:
-        assert list(pe.obs._intersection_idx(ids)) == pe.obs._intersection_idx([list(o) for o in ids])
+        interlist = pe.obs._intersection_idx([list(o) for o in ids])
+        listinter = list(pe.obs._intersection_idx(ids))
+        assert len(interlist) == len(listinter)
+        assert all([o in listinter for o in interlist])
+        assert all([o in interlist for o in listinter])
+
 
 def test_merge_intersection():
     for idl_list in [[range(1, 100), range(1, 100), range(1, 100)],
                      [range(4, 80, 6), range(4, 80, 6)],
                      [[0, 2, 8, 19, 205], [0, 2, 8, 19, 205]]]:
         assert pe.obs._merge_idx(idl_list) == pe.obs._intersection_idx(idl_list)
 
@@ -581,14 +613,26 @@
             assert obs1 == (obs1 / obs2) * obs2
             assert obs1 == (obs1 * obs2) / obs2
             assert obs1 == obs1 * (obs2 / obs2)
             assert obs1 == (obs1 + obs2) - obs2
             assert obs1 == obs1 + (obs2 - obs2)
 
 
+def test_gamma_method_consistent():
+    dat = np.sin(np.arange(100) / 100)
+    for idl in [np.arange(100), np.arange(0, 1000, 10)]:
+        my_obs = pe.Obs([dat], ["test_ens"], idl=[idl])
+        assert np.isclose(my_obs.value, 0.4554865083873183)
+
+        my_obs.gm(S=0)
+        assert np.isclose(my_obs.dvalue, 0.02495954189079061)
+        my_obs.gm()
+        assert np.isclose(my_obs.dvalue, 0.11817931680985193)
+
+
 def test_gamma_method_irregular():
     N = 20000
     arr = np.random.normal(1, .2, size=N)
     afull = pe.Obs([arr], ['a'])
 
     configs = np.ones_like(arr)
     for i in np.random.uniform(0, len(arr), size=int(.8 * N)):
@@ -686,30 +730,84 @@
 
     ob = pe.Obs([dat], ["ens1"], idl=[idl_b])
     ob.gamma_method()
     tau_b = ob.e_tauint["ens1"]
 
     assert np.isclose(tau_a, tau_b)
 
+    dat = [np.random.normal(loc=1., size=10) for i in range(2)]
+    idl = [[0, 2, 4, 8, 10, 12, 14, 16, 18, 20], np.arange(0, 20, 2)]
+    o = pe.Obs(dat, ['A|r1', 'A|r2'], idl=idl)
+    o.gm()
+    assert(pe.obs._determine_gap(o, o.e_content, 'A') == 2)
+    dat = [np.random.normal(loc=1., size=10) for i in range(3)]
+    idl = [[0, 2, 4, 8, 10, 12, 14, 16, 18, 20], np.arange(0, 20, 2), range(10)]
+    o = pe.Obs(dat, ['A|r1', 'A|r2', 'A|r5'], idl=idl)
+    o.gm()
+    assert(pe.obs._determine_gap(o, o.e_content, 'A') == 1)
+
+    dat = np.sin(np.arange(100) / 100)
+
+    idl = [np.arange(100), np.arange(0, 1000, 10), list(np.arange(0, 100, 10)) + list(np.arange(180, 1080, 10)), range(1, 500, 5)]
+    my_obs = pe.Obs([dat for i in range(len(idl))], ['%s|%d' % ('A', i) for i in range(len(idl))], idl=idl)
+    my_obs.gm()
+    idl = idl[1:]
+    my_obs = pe.Obs([dat for i in range(len(idl))], ['%s|%d' % ('A', i) for i in range(len(idl))], idl=idl)
+    my_obs.gm()
+    idl += [range(1, 400, 4)]
+    my_obs = pe.Obs([dat for i in range(len(idl))], ['%s|%d' % ('A', i) for i in range(len(idl))], idl=idl)
+    with pytest.raises(Exception):
+        my_obs.gm()
+
+    # check cases where tau is large compared to the chain length
+    N = 15
+    for i in range(10):
+        arr = np.random.normal(1, .2, size=N)
+        for rho in .1 * np.arange(20):
+            carr = gen_autocorrelated_array(arr, rho)
+            a = pe.Obs([carr], ['a'])
+            a.gm()
+
 
 def test_irregular_gapped_dtauint():
     my_idl = list(range(0, 5010, 10))
     my_idl.remove(400)
     my_idl2 = list(range(0, 501, 1))
     my_idl2.remove(40)
 
-    my_data = np.random.normal(1.1, 0.2, 500)
-    obs = pe.Obs([my_data], ["B1"], idl=[my_idl])
-    obs.gamma_method()
-
-    obs2 = pe.Obs([my_data], ["B2"], idl=[my_idl2])
-    obs2.gamma_method()
-
-    assert np.isclose(obs.e_tauint["B1"], obs2.e_tauint["B2"])
-    assert np.isclose(obs.e_dtauint["B1"], obs2.e_dtauint["B2"])
+    for i in range(42):
+        my_data = np.random.normal(1.1, 0.2, 500)
+        obs = pe.Obs([my_data], ["B1"], idl=[my_idl])
+        obs.gamma_method()
+
+        obs2 = pe.Obs([my_data], ["B2"], idl=[my_idl2])
+        obs2.gamma_method()
+
+        assert np.isclose(obs.e_tauint["B1"], obs2.e_tauint["B2"])
+        assert np.isclose(obs.e_dtauint["B1"], obs2.e_dtauint["B2"])
+        assert np.isclose(obs.e_dvalue["B1"], obs2.e_dvalue["B2"])
+        assert np.isclose(obs.e_ddvalue["B1"], obs2.e_ddvalue["B2"])
+        assert len(obs.e_rho["B1"]) == len(obs2.e_rho["B2"])
+
+        obs.gamma_method(tau_exp=1)
+        obs2.gamma_method(tau_exp=1)
+
+        assert np.isclose(obs.e_tauint["B1"], obs2.e_tauint["B2"])
+        assert np.isclose(obs.e_dtauint["B1"], obs2.e_dtauint["B2"])
+        assert np.isclose(obs.e_dvalue["B1"], obs2.e_dvalue["B2"])
+        assert np.isclose(obs.e_ddvalue["B1"], obs2.e_ddvalue["B2"])
+        assert len(obs.e_rho["B1"]) == len(obs2.e_rho["B2"])
+
+        obs.gamma_method(S=0)
+        obs2.gamma_method(S=0)
+
+        assert np.isclose(obs.e_tauint["B1"], obs2.e_tauint["B2"])
+        assert np.isclose(obs.e_dtauint["B1"], obs2.e_dtauint["B2"])
+        assert np.isclose(obs.e_dvalue["B1"], obs2.e_dvalue["B2"])
+        assert np.isclose(obs.e_ddvalue["B1"], obs2.e_ddvalue["B2"])
 
 
 def test_covariance_is_variance():
     value = np.random.normal(5, 10)
     dvalue = np.abs(np.random.normal(0, 1))
     test_obs = pe.pseudo_Obs(value, dvalue, 't')
     test_obs.gamma_method()
@@ -850,14 +948,15 @@
     obs = []
     for i in range(5):
         obs.append(pe.pseudo_Obs(1.0, 0.1, 'test', 5))
 
     with pytest.warns(RuntimeWarning):
         pe.covariance(obs)
 
+
 def test_covariance_idl():
     range1 = range(10, 1010, 10)
     range2 = range(10, 1010, 50)
 
     obs1 = pe.Obs([np.random.normal(1.0, 0.1, len(range1))], ["ens"], idl=[range1])
     obs2 = pe.Obs([np.random.normal(1.0, 0.1, len(range2))], ["ens"], idl=[range2])
     obs1.gamma_method()
@@ -996,22 +1095,14 @@
     ]
     for idx_new in idl:
         new = pe.obs._reduce_deltas(deltas, idx_old, idx_new)
         print(new)
         assert(np.alltrue([float(i) for i in idx_new] == new))
 
 
-def test_merge_idx():
-    idl = [list(np.arange(1, 14)) + list(range(16, 100, 4)), range(4, 604, 4), [2, 4, 5, 6, 8, 9, 12, 24], range(1, 20, 1), range(50, 789, 7)]
-    new_idx = pe.obs._merge_idx(idl)
-    assert(new_idx[-1] > new_idx[0])
-    for i in range(1, len(new_idx)):
-        assert(new_idx[i - 1] < new_idx[i])
-
-
 def test_cobs_array():
     cobs = pe.Obs([np.random.normal(1.0, 0.1, 100)], ['t']) * (1 + 2j)
     np.identity(4) + cobs
     cobs + np.identity(4)
     np.identity(4) - cobs
     cobs - np.identity(4)
     np.identity(4) * cobs
@@ -1152,7 +1243,23 @@
     o = pe.pseudo_Obs(1, .1, 'test')
     no = np.nan * o
     no.gamma_method()
 
     o.idl['test'] = [1, 5] + list(range(7, 2002, 2))
     no = np.NaN * o
     no.gamma_method()
+
+
+def test_format_uncertainty():
+    assert pe.obs._format_uncertainty(0.548, 0.248976, 4) == '0.5480(2490)'
+    assert pe.obs._format_uncertainty(0.548, 2.48497, 2) == '0.5(2.5)'
+    assert pe.obs._format_uncertainty(0.548, 2.48497, 4) == '0.548(2.485)'
+    assert pe.obs._format_uncertainty(0.548, 20078.3, 9) == '0.5480(20078.3000)'
+    pe.obs._format_uncertainty(np.NaN, 1)
+    pe.obs._format_uncertainty(1, np.NaN)
+    pe.obs._format_uncertainty(np.NaN, np.inf)
+
+def test_format():
+    o1 = pe.pseudo_Obs(0.348, 0.0123, "test")
+    assert o1.__format__("+3") == '+0.3480(123)'
+    assert o1.__format__("+2") == '+0.348(12)'
+    assert o1.__format__(" 2") == ' 0.348(12)'
```

### Comparing `pyerrors-2.7.0/tests/openQCD_in_test.py` & `pyerrors-2.8.0/tests/openQCD_in_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,24 +50,35 @@
     # t0
     prefix = 'openqcd'
 
     t0 = pe.input.openQCD.extract_t0(path, prefix, dtr_read=3, xmin=0, spatial_extent=4)
     files = ['openqcd2r1.ms.dat']
     names = ['openqcd2|r1']
     t0 = pe.input.openQCD.extract_t0(path, '', dtr_read=3, xmin=0, spatial_extent=4, files=files, names=names, fit_range=2)
+    assert(np.isclose(t0.value, 0.3816208266076627))
     t0 = pe.input.openQCD.extract_t0(path, prefix, dtr_read=3, xmin=0, spatial_extent=4, r_start=[1])
     repname = list(rwfo[0].idl.keys())[0]
     assert(t0.idl[repname] == range(1, 10))
     t0 = pe.input.openQCD.extract_t0(path, prefix, dtr_read=3, xmin=0, spatial_extent=4, r_start=[2], r_stop=[8])
     repname = list(rwfo[0].idl.keys())[0]
     assert(t0.idl[repname] == range(2, 9))
     t0 = pe.input.openQCD.extract_t0(path, prefix, dtr_read=3, xmin=0, spatial_extent=4, fit_range=2, plaquette=True, assume_thermalization=True)
 
     pe.input.openQCD.extract_t0(path, '', dtr_read=3, xmin=0, spatial_extent=4, files=files, names=names, fit_range=2, plot_fit=True)
 
+    with pytest.raises(Exception):
+        pe.input.openQCD.extract_t0(path, '', dtr_read=3, xmin=0, spatial_extent=4, files=files, names=names, fit_range=2, c=14)
+    # w0
+
+    w0 = pe.input.openQCD.extract_w0(path, '', dtr_read=3, xmin=0, spatial_extent=4, files=files, names=names, fit_range=2, plot_fit=True)
+    assert(np.isclose(w0.value, 0.5220124285820434))
+
+    with pytest.raises(Exception):
+        pe.input.openQCD.extract_w0(path, '', dtr_read=3, xmin=0, spatial_extent=4, files=files, names=names, fit_range=2, c=14)
+
 
 def test_Qtop():
     path = './tests//data/openqcd_test/'
     prefix = 'sfqcd'
 
     qtop = pe.input.openQCD.read_qtop(path, prefix, c=0.3, version='sfqcd')
     repname = list(qtop.idl.keys())[0]
```

### Comparing `pyerrors-2.7.0/tests/roots_test.py` & `pyerrors-2.8.0/tests/roots_test.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.7.0/tests/sfcf_in_test.py` & `pyerrors-2.8.0/tests/sfcf_in_test.py`

 * *Files identical despite different names*

