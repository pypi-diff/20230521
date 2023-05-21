# Comparing `tmp/kikuchipy-0.8.4.tar.gz` & `tmp/kikuchipy-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kikuchipy-0.8.4.tar", last modified: Fri Apr  7 13:46:12 2023, max compression
+gzip compressed data, was "kikuchipy-0.8.5.tar", last modified: Sun May 21 11:44:59 2023, max compression
```

## Comparing `kikuchipy-0.8.4.tar` & `kikuchipy-0.8.5.tar`

### file list

```diff
@@ -1,261 +1,261 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.219895 kikuchipy-0.8.4/
--rw-r--r--   0 runner    (1001) docker     (123)    52167 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-04-07 13:46:12.219895 kikuchipy-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/RELEASE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.171895 kikuchipy-0.8.4/kikuchipy/
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.175895 kikuchipy-0.8.4/kikuchipy/_rotation/
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/_rotation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.175895 kikuchipy-0.8.4/kikuchipy/_rotation/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/_rotation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/_rotation/tests/test_rotation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.175895 kikuchipy-0.8.4/kikuchipy/_util/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/_util/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/_util/_transfer_axes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.175895 kikuchipy-0.8.4/kikuchipy/_util/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/_util/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/_util/tests/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)    10912 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/_util/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/_util/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    14809 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.175895 kikuchipy-0.8.4/kikuchipy/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27984 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.175895 kikuchipy-0.8.4/kikuchipy/data/bruker_h5ebsd/
--rw-r--r--   0 runner    (1001) docker     (123)    16614 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/bruker_h5ebsd/create_bruker_h5ebsd_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    73176 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/bruker_h5ebsd/patterns.h5
--rw-r--r--   0 runner    (1001) docker     (123)    59696 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/bruker_h5ebsd/patterns_roi.h5
--rw-r--r--   0 runner    (1001) docker     (123)    55824 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/bruker_h5ebsd/patterns_roi_nonrectangular.h5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.179895 kikuchipy-0.8.4/kikuchipy/data/edax_binary/
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/edax_binary/create_dummy_edax_binary_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    32416 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/edax_binary/edax_binary.up1
--rw-r--r--   0 runner    (1001) docker     (123)    72042 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/edax_binary/edax_binary.up2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.179895 kikuchipy-0.8.4/kikuchipy/data/edax_h5ebsd/
--rw-r--r--   0 runner    (1001) docker     (123)   938661 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/edax_h5ebsd/patterns.h5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.179895 kikuchipy-0.8.4/kikuchipy/data/emsoft_ebsd/
--rw-r--r--   0 runner    (1001) docker     (123)   351168 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/emsoft_ebsd/EBSD_TEST_Ni.h5
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/emsoft_ebsd/create_dummy_emsoft_ebsd_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    35624 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/emsoft_ebsd/simulated_ebsd.h5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.183895 kikuchipy-0.8.4/kikuchipy/data/emsoft_ebsd_master_pattern/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/emsoft_ebsd_master_pattern/BetheParameters.nml
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/emsoft_ebsd_master_pattern/convert_emsoft_ebsd_masterpattern_file_uint8_gzip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/emsoft_ebsd_master_pattern/create_dummy_emsoft_ebsd_master_pattern_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    61872 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/emsoft_ebsd_master_pattern/master_patterns.h5
--rw-r--r--   0 runner    (1001) docker     (123)    12680 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/emsoft_ebsd_master_pattern/ni.xtal
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/emsoft_ebsd_master_pattern/ni_ebsdmaster.nml
--rw-r--r--   0 runner    (1001) docker     (123)    19638 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mc.out
--rw-r--r--   0 runner    (1001) docker     (123)   908492 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mc_mp_20kv_uint8_gzip_opts9.h5
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mcopencl.nml
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mp.out
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.183895 kikuchipy-0.8.4/kikuchipy/data/emsoft_ecp_master_pattern/
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/emsoft_ecp_master_pattern/create_dummy_emsoft_ecp_master_pattern_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    62296 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/emsoft_ecp_master_pattern/ecp_master_pattern.h5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.187895 kikuchipy-0.8.4/kikuchipy/data/emsoft_tkd_master_pattern/
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/emsoft_tkd_master_pattern/create_dummy_emsoft_tkd_master_pattern_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    61600 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/emsoft_tkd_master_pattern/tkd_master_pattern.h5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.187895 kikuchipy-0.8.4/kikuchipy/data/kikuchipy_h5ebsd/
--rw-r--r--   0 runner    (1001) docker     (123)   149400 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/kikuchipy_h5ebsd/patterns.h5
--rw-r--r--   0 runner    (1001) docker     (123)    46480 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/kikuchipy_h5ebsd/patterns_nochunks.h5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.187895 kikuchipy-0.8.4/kikuchipy/data/nordif/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4678 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/nordif/Background acquisition pattern.bmp
--rwxr-xr-x   0 runner    (1001) docker     (123)     4678 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/nordif/Background calibration pattern.bmp
--rwxr-xr-x   0 runner    (1001) docker     (123)     4678 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/nordif/Calibration (294,532).bmp
--rwxr-xr-x   0 runner    (1001) docker     (123)     4678 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/nordif/Calibration (425,447).bmp
--rw-r--r--   0 runner    (1001) docker     (123)    32400 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/nordif/Pattern.dat
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/nordif/Setting.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/nordif/Setting_bad1.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/nordif/Setting_bad2.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/nordif/Setting_bad3.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.187895 kikuchipy-0.8.4/kikuchipy/data/oxford_binary/
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/oxford_binary/create_dummy_oxford_binary_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    32786 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/oxford_binary/patterns.ebsp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.187895 kikuchipy-0.8.4/kikuchipy/data/oxford_h5ebsd/
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/oxford_h5ebsd/create_oxford_h5ebsd_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    59152 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/oxford_h5ebsd/patterns.h5oina
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.187895 kikuchipy-0.8.4/kikuchipy/data/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12182 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/data/tests/test_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.191895 kikuchipy-0.8.4/kikuchipy/detectors/
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/detectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14225 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/detectors/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)    67124 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/detectors/ebsd_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.191895 kikuchipy-0.8.4/kikuchipy/detectors/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/detectors/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/detectors/tests/test_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)    39863 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/detectors/tests/test_ebsd_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.191895 kikuchipy-0.8.4/kikuchipy/draw/
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/draw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/draw/_navigators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/draw/_plot_pattern_positions_in_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/draw/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/draw/markers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.191895 kikuchipy-0.8.4/kikuchipy/draw/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/draw/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/draw/tests/test_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10741 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/draw/tests/test_markers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/draw/tests/test_navigators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/draw/tests/test_plot_pattern_positions_in_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.195895 kikuchipy-0.8.4/kikuchipy/filters/
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/filters/fft_barnes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.195895 kikuchipy-0.8.4/kikuchipy/filters/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/filters/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/filters/tests/test_fft_barnes.py
--rw-r--r--   0 runner    (1001) docker     (123)    15640 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/filters/tests/test_window.py
--rw-r--r--   0 runner    (1001) docker     (123)    17866 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/filters/window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.195895 kikuchipy-0.8.4/kikuchipy/generators/
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.195895 kikuchipy-0.8.4/kikuchipy/generators/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/generators/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10012 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/generators/tests/test_virtual_bse_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13349 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/generators/virtual_bse_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/hyperspy_extension.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.195895 kikuchipy-0.8.4/kikuchipy/imaging/
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/imaging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.195895 kikuchipy-0.8.4/kikuchipy/imaging/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/imaging/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9960 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/imaging/tests/test_virtual_bse_imager.py
--rw-r--r--   0 runner    (1001) docker     (123)    16325 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/imaging/vbse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.195895 kikuchipy-0.8.4/kikuchipy/indexing/
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/indexing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/indexing/_dictionary_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)    12343 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/indexing/_hough_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)    13895 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/indexing/_merge_crystal_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/indexing/_orientation_similarity_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.199895 kikuchipy-0.8.4/kikuchipy/indexing/_refinement/
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/indexing/_refinement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/indexing/_refinement/_objective_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    44415 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/indexing/_refinement/_refinement.py
--rw-r--r--   0 runner    (1001) docker     (123)    21304 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/indexing/_refinement/_solvers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.199895 kikuchipy-0.8.4/kikuchipy/indexing/similarity_metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/indexing/similarity_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/indexing/similarity_metrics/_normalized_cross_correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/indexing/similarity_metrics/_normalized_dot_product.py
--rw-r--r--   0 runner    (1001) docker     (123)     8831 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/indexing/similarity_metrics/_similarity_metric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.199895 kikuchipy-0.8.4/kikuchipy/indexing/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/indexing/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/indexing/tests/test_dictionary_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)    47403 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/indexing/tests/test_ebsd_refinement.py
--rw-r--r--   0 runner    (1001) docker     (123)    22250 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/indexing/tests/test_merge_crystal_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/indexing/tests/test_orientation_similarity_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/indexing/tests/test_similarity_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.199895 kikuchipy-0.8.4/kikuchipy/io/
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14667 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/io/_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/io/_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.203895 kikuchipy-0.8.4/kikuchipy/io/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/io/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/io/plugins/_emsoft_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)    16167 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/io/plugins/_h5ebsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     8571 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/io/plugins/bruker_h5ebsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/io/plugins/ebsd_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     8266 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/io/plugins/edax_binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/io/plugins/edax_h5ebsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/io/plugins/emsoft_ebsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/io/plugins/emsoft_ebsd_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/io/plugins/emsoft_ecp_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/io/plugins/emsoft_tkd_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)    17736 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/io/plugins/kikuchipy_h5ebsd.py
--rw-r--r--   0 runner    (1001) docker     (123)    14826 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/io/plugins/nordif.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/io/plugins/nordif_calibration_patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)    19627 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/io/plugins/oxford_binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/io/plugins/oxford_h5ebsd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.207895 kikuchipy-0.8.4/kikuchipy/io/plugins/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/io/plugins/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/io/plugins/tests/test_bruker_h5ebsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/io/plugins/tests/test_ebsd_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/io/plugins/tests/test_edax_binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/io/plugins/tests/test_edax_h5ebsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/io/plugins/tests/test_emsoft_ebsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/io/plugins/tests/test_emsoft_ebsd_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/io/plugins/tests/test_emsoft_ecp_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/io/plugins/tests/test_emsoft_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/io/plugins/tests/test_emsoft_tkd_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)    14640 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/io/plugins/tests/test_kikuchipy_h5ebsd.py
--rw-r--r--   0 runner    (1001) docker     (123)    13546 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/io/plugins/tests/test_nordif.py
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/io/plugins/tests/test_nordif_calibration_patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/io/plugins/tests/test_oxford_binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/io/plugins/tests/test_oxford_h5ebsd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.207895 kikuchipy-0.8.4/kikuchipy/io/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/io/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/io/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/io/tests/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.207895 kikuchipy-0.8.4/kikuchipy/pattern/
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/pattern/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25808 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/pattern/_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/pattern/chunk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.207895 kikuchipy-0.8.4/kikuchipy/pattern/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/pattern/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/pattern/tests/test_chunk.py
--rw-r--r--   0 runner    (1001) docker     (123)    18683 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/pattern/tests/test_pattern.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.211895 kikuchipy-0.8.4/kikuchipy/projections/
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/projections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/projections/gnomonic_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/projections/hesse_normal_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/projections/lambert_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/projections/spherical_projection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.211895 kikuchipy-0.8.4/kikuchipy/projections/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/projections/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/projections/tests/test_gnomonic_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/projections/tests/test_hesse_normal_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/projections/tests/test_lambert_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/projections/tests/test_spherical_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.211895 kikuchipy-0.8.4/kikuchipy/signals/
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13111 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/signals/_kikuchi_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)    22408 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/signals/_kikuchipy_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)   131373 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/signals/ebsd.py
--rw-r--r--   0 runner    (1001) docker     (123)    18279 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/signals/ebsd_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/signals/ecp_master_pattern.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.215895 kikuchipy-0.8.4/kikuchipy/signals/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/signals/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    87955 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/signals/tests/test_ebsd.py
--rw-r--r--   0 runner    (1001) docker     (123)    12409 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/signals/tests/test_ebsd_hough_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)    27376 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/signals/tests/test_ebsd_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/signals/tests/test_ecp_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/signals/tests/test_kikuchi_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/signals/tests/test_virtual_bse_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.215895 kikuchipy-0.8.4/kikuchipy/signals/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/signals/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/signals/util/_crystal_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    11236 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/signals/util/_dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/signals/util/_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)    10639 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/signals/util/_map_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    22702 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/signals/util/_master_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/signals/util/_overwrite_hyperspy_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/signals/util/array_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.215895 kikuchipy-0.8.4/kikuchipy/signals/util/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/signals/util/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/signals/util/tests/test_array_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/signals/util/tests/test_dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/signals/util/tests/test_overwrite_hyperspy_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/signals/virtual_bse_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.219895 kikuchipy-0.8.4/kikuchipy/simulations/
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/simulations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/simulations/_kikuchi_pattern_features.py
--rw-r--r--   0 runner    (1001) docker     (123)    26644 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/simulations/_kikuchi_pattern_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    27443 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/simulations/kikuchi_pattern_simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.219895 kikuchipy-0.8.4/kikuchipy/simulations/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/simulations/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11778 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/simulations/tests/test_kikuchi_pattern_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    14664 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/kikuchipy/simulations/tests/test_kikuchi_pattern_simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 13:46:12.175895 kikuchipy-0.8.4/kikuchipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-04-07 13:46:12.000000 kikuchipy-0.8.4/kikuchipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-04-07 13:46:12.000000 kikuchipy-0.8.4/kikuchipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 13:46:12.000000 kikuchipy-0.8.4/kikuchipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-07 13:46:12.000000 kikuchipy-0.8.4/kikuchipy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-07 13:46:12.000000 kikuchipy-0.8.4/kikuchipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-07 13:46:12.000000 kikuchipy-0.8.4/kikuchipy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 13:46:11.000000 kikuchipy-0.8.4/kikuchipy.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-07 13:46:12.219895 kikuchipy-0.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-04-07 13:45:58.000000 kikuchipy-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.369459 kikuchipy-0.8.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    52350 2023-05-21 11:44:47.000000 kikuchipy-0.8.5/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-05-21 11:44:47.000000 kikuchipy-0.8.5/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-21 11:44:47.000000 kikuchipy-0.8.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-21 11:44:47.000000 kikuchipy-0.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-21 11:44:47.000000 kikuchipy-0.8.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-05-21 11:44:59.369459 kikuchipy-0.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-05-21 11:44:47.000000 kikuchipy-0.8.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-21 11:44:47.000000 kikuchipy-0.8.5/RELEASE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.341459 kikuchipy-0.8.5/kikuchipy/
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.341459 kikuchipy-0.8.5/kikuchipy/_rotation/
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/_rotation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.341459 kikuchipy-0.8.5/kikuchipy/_rotation/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/_rotation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/_rotation/tests/test_rotation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.341459 kikuchipy-0.8.5/kikuchipy/_util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/_util/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/_util/_transfer_axes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.345459 kikuchipy-0.8.5/kikuchipy/_util/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/_util/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/_util/tests/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10912 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/_util/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/_util/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14809 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.345459 kikuchipy-0.8.5/kikuchipy/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27984 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.345459 kikuchipy-0.8.5/kikuchipy/data/bruker_h5ebsd/
+-rw-r--r--   0 runner    (1001) docker     (123)    16614 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/bruker_h5ebsd/create_bruker_h5ebsd_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73176 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/bruker_h5ebsd/patterns.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    59696 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/bruker_h5ebsd/patterns_roi.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    55824 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/bruker_h5ebsd/patterns_roi_nonrectangular.h5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.345459 kikuchipy-0.8.5/kikuchipy/data/edax_binary/
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/edax_binary/create_dummy_edax_binary_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32416 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/edax_binary/edax_binary.up1
+-rw-r--r--   0 runner    (1001) docker     (123)    72042 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/edax_binary/edax_binary.up2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.345459 kikuchipy-0.8.5/kikuchipy/data/edax_h5ebsd/
+-rw-r--r--   0 runner    (1001) docker     (123)   938661 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/edax_h5ebsd/patterns.h5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.345459 kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd/
+-rw-r--r--   0 runner    (1001) docker     (123)   351168 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd/EBSD_TEST_Ni.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd/create_dummy_emsoft_ebsd_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35624 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd/simulated_ebsd.h5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.349459 kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd_master_pattern/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd_master_pattern/BetheParameters.nml
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd_master_pattern/convert_emsoft_ebsd_masterpattern_file_uint8_gzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd_master_pattern/create_dummy_emsoft_ebsd_master_pattern_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61872 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd_master_pattern/master_patterns.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    12680 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd_master_pattern/ni.xtal
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd_master_pattern/ni_ebsdmaster.nml
+-rw-r--r--   0 runner    (1001) docker     (123)    19638 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mc.out
+-rw-r--r--   0 runner    (1001) docker     (123)   908492 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mc_mp_20kv_uint8_gzip_opts9.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mcopencl.nml
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mp.out
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.349459 kikuchipy-0.8.5/kikuchipy/data/emsoft_ecp_master_pattern/
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/emsoft_ecp_master_pattern/create_dummy_emsoft_ecp_master_pattern_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62296 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/emsoft_ecp_master_pattern/ecp_master_pattern.h5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.349459 kikuchipy-0.8.5/kikuchipy/data/emsoft_tkd_master_pattern/
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/emsoft_tkd_master_pattern/create_dummy_emsoft_tkd_master_pattern_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61600 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/emsoft_tkd_master_pattern/tkd_master_pattern.h5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.349459 kikuchipy-0.8.5/kikuchipy/data/kikuchipy_h5ebsd/
+-rw-r--r--   0 runner    (1001) docker     (123)   149400 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/kikuchipy_h5ebsd/patterns.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    46480 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/kikuchipy_h5ebsd/patterns_nochunks.h5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.349459 kikuchipy-0.8.5/kikuchipy/data/nordif/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4678 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/nordif/Background acquisition pattern.bmp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4678 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/nordif/Background calibration pattern.bmp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4678 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/nordif/Calibration (294,532).bmp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4678 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/nordif/Calibration (425,447).bmp
+-rw-r--r--   0 runner    (1001) docker     (123)    32400 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/nordif/Pattern.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/nordif/Setting.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/nordif/Setting_bad1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/nordif/Setting_bad2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/nordif/Setting_bad3.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.349459 kikuchipy-0.8.5/kikuchipy/data/oxford_binary/
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/oxford_binary/create_dummy_oxford_binary_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32786 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/oxford_binary/patterns.ebsp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.353459 kikuchipy-0.8.5/kikuchipy/data/oxford_h5ebsd/
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/oxford_h5ebsd/create_oxford_h5ebsd_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59152 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/oxford_h5ebsd/patterns.h5oina
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.353459 kikuchipy-0.8.5/kikuchipy/data/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12182 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/data/tests/test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.353459 kikuchipy-0.8.5/kikuchipy/detectors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/detectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14225 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/detectors/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67124 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/detectors/ebsd_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.353459 kikuchipy-0.8.5/kikuchipy/detectors/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/detectors/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/detectors/tests/test_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39863 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/detectors/tests/test_ebsd_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.353459 kikuchipy-0.8.5/kikuchipy/draw/
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/draw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/draw/_navigators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/draw/_plot_pattern_positions_in_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/draw/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/draw/markers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.353459 kikuchipy-0.8.5/kikuchipy/draw/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/draw/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/draw/tests/test_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10741 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/draw/tests/test_markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/draw/tests/test_navigators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/draw/tests/test_plot_pattern_positions_in_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.353459 kikuchipy-0.8.5/kikuchipy/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/filters/fft_barnes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.353459 kikuchipy-0.8.5/kikuchipy/filters/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/filters/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/filters/tests/test_fft_barnes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15640 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/filters/tests/test_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17866 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/filters/window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.353459 kikuchipy-0.8.5/kikuchipy/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.353459 kikuchipy-0.8.5/kikuchipy/generators/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/generators/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10012 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/generators/tests/test_virtual_bse_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13349 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/generators/virtual_bse_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/hyperspy_extension.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.353459 kikuchipy-0.8.5/kikuchipy/imaging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/imaging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.353459 kikuchipy-0.8.5/kikuchipy/imaging/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/imaging/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9960 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/imaging/tests/test_virtual_bse_imager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16325 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/imaging/vbse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.357459 kikuchipy-0.8.5/kikuchipy/indexing/
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/indexing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/indexing/_dictionary_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12343 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/indexing/_hough_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14530 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/indexing/_merge_crystal_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/indexing/_orientation_similarity_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.357459 kikuchipy-0.8.5/kikuchipy/indexing/_refinement/
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/indexing/_refinement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/indexing/_refinement/_objective_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44415 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/indexing/_refinement/_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21304 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/indexing/_refinement/_solvers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.357459 kikuchipy-0.8.5/kikuchipy/indexing/similarity_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/indexing/similarity_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/indexing/similarity_metrics/_normalized_cross_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/indexing/similarity_metrics/_normalized_dot_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8831 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/indexing/similarity_metrics/_similarity_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.357459 kikuchipy-0.8.5/kikuchipy/indexing/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/indexing/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/indexing/tests/test_dictionary_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47403 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/indexing/tests/test_ebsd_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23728 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/indexing/tests/test_merge_crystal_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/indexing/tests/test_orientation_similarity_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/indexing/tests/test_similarity_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.357459 kikuchipy-0.8.5/kikuchipy/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14667 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.361459 kikuchipy-0.8.5/kikuchipy/io/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/_emsoft_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16167 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/_h5ebsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8571 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/bruker_h5ebsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/ebsd_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8266 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/edax_binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/edax_h5ebsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/emsoft_ebsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/emsoft_ebsd_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/emsoft_ecp_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/emsoft_tkd_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17736 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/kikuchipy_h5ebsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14826 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/nordif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/nordif_calibration_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19627 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/oxford_binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/oxford_h5ebsd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.361459 kikuchipy-0.8.5/kikuchipy/io/plugins/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_bruker_h5ebsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_ebsd_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_edax_binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_edax_h5ebsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_emsoft_ebsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_emsoft_ebsd_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_emsoft_ecp_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_emsoft_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_emsoft_tkd_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14640 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_kikuchipy_h5ebsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13546 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_nordif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_nordif_calibration_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_oxford_binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_oxford_h5ebsd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.361459 kikuchipy-0.8.5/kikuchipy/io/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/io/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.361459 kikuchipy-0.8.5/kikuchipy/pattern/
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/pattern/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25808 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/pattern/_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/pattern/chunk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.361459 kikuchipy-0.8.5/kikuchipy/pattern/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/pattern/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/pattern/tests/test_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18739 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/pattern/tests/test_pattern.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.361459 kikuchipy-0.8.5/kikuchipy/projections/
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/projections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/projections/gnomonic_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/projections/hesse_normal_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/projections/lambert_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/projections/spherical_projection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.365459 kikuchipy-0.8.5/kikuchipy/projections/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/projections/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/projections/tests/test_gnomonic_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/projections/tests/test_hesse_normal_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/projections/tests/test_lambert_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/projections/tests/test_spherical_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.365459 kikuchipy-0.8.5/kikuchipy/signals/
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13111 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/_kikuchi_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22408 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/_kikuchipy_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131373 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/ebsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18279 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/ebsd_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/ecp_master_pattern.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.365459 kikuchipy-0.8.5/kikuchipy/signals/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88067 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/tests/test_ebsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12409 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/tests/test_ebsd_hough_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27376 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/tests/test_ebsd_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/tests/test_ecp_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/tests/test_kikuchi_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/tests/test_virtual_bse_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.365459 kikuchipy-0.8.5/kikuchipy/signals/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/util/_crystal_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11236 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/util/_dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/util/_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10639 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/util/_map_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22702 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/util/_master_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/util/_overwrite_hyperspy_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/util/array_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.365459 kikuchipy-0.8.5/kikuchipy/signals/util/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/util/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/util/tests/test_array_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/util/tests/test_dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/util/tests/test_overwrite_hyperspy_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/signals/virtual_bse_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.369459 kikuchipy-0.8.5/kikuchipy/simulations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/simulations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/simulations/_kikuchi_pattern_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26644 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/simulations/_kikuchi_pattern_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27443 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/simulations/kikuchi_pattern_simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.369459 kikuchipy-0.8.5/kikuchipy/simulations/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/simulations/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11778 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/simulations/tests/test_kikuchi_pattern_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14664 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/kikuchipy/simulations/tests/test_kikuchi_pattern_simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:44:59.341459 kikuchipy-0.8.5/kikuchipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-05-21 11:44:59.000000 kikuchipy-0.8.5/kikuchipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-05-21 11:44:59.000000 kikuchipy-0.8.5/kikuchipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 11:44:59.000000 kikuchipy-0.8.5/kikuchipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-21 11:44:59.000000 kikuchipy-0.8.5/kikuchipy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-21 11:44:59.000000 kikuchipy-0.8.5/kikuchipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-21 11:44:59.000000 kikuchipy-0.8.5/kikuchipy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 11:44:59.000000 kikuchipy-0.8.5/kikuchipy.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-21 11:44:59.369459 kikuchipy-0.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-05-21 11:44:48.000000 kikuchipy-0.8.5/setup.py
```

### Comparing `kikuchipy-0.8.4/CHANGELOG.rst` & `kikuchipy-0.8.5/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,22 @@
 All user facing changes to this project are documented in this file. The format is based
 on `Keep a Changelog <https://keepachangelog.com/en/1.1.0>`__, and this project tries
 its best to adhere to `Semantic Versioning <https://semver.org/spec/v2.0.0.html>`__.
 
 List entries are sorted in descending chronological order. Contributors to each release
 were listed in alphabetical order by first name until version 0.7.0.
 
+0.8.5 (2023-05-21)
+==================
+
+Fixed
+-----
+- Not-indexed points in crystal maps are handled correctly when merging.
+  (`#639 <https://github.com/pyxem/kikuchipy/pull/639>`_)
+
 0.8.4 (2023-04-07)
 ==================
 
 Fixed
 -----
 - Points considered not-indexed in a crystal map are maintained after EBSD refinement.
   (`#632 <https://github.com/pyxem/kikuchipy/pull/632>`_)
```

### Comparing `kikuchipy-0.8.4/CODE_OF_CONDUCT.rst` & `kikuchipy-0.8.5/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/LICENSE` & `kikuchipy-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/PKG-INFO` & `kikuchipy-0.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kikuchipy
-Version: 0.8.4
+Version: 0.8.5
 Summary: Processing, simulating and indexing of electron backscatter diffraction (EBSD) patterns.
 Home-page: https://kikuchipy.org
 Download-URL: https://pypi.python.org/pypi/kikuchipy
 Author: kikuchipy developers
 Author-email: hakon.w.anes@ntnu.no
 Maintainer: Håkon Wiik Ånes
 Maintainer-email: hakon.w.anes@ntnu.no
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kikuchipy Version: 0.8.4 Summary: Processing,
+Metadata-Version: 2.1 Name: kikuchipy Version: 0.8.5 Summary: Processing,
 simulating and indexing of electron backscatter diffraction (EBSD) patterns.
 Home-page: https://kikuchipy.org Download-URL: https://pypi.python.org/pypi/
 kikuchipy Author: kikuchipy developers Author-email: hakon.w.anes@ntnu.no
 Maintainer: HÃ¥kon Wiik Ãnes Maintainer-email: hakon.w.anes@ntnu.no License:
 GPLv3+ Project-URL: Bug Tracker, https://github.com/pyxem/kikuchipy/issues
 Project-URL: Documentation, https://kikuchipy.org Project-URL: Source Code,
 https://github.com/pyxem/kikuchipy Keywords: EBSD,electron backscatter
```

### Comparing `kikuchipy-0.8.4/README.md` & `kikuchipy-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/RELEASE.rst` & `kikuchipy-0.8.5/RELEASE.rst`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/__init__.py` & `kikuchipy-0.8.5/kikuchipy/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/_rotation/__init__.py` & `kikuchipy-0.8.5/kikuchipy/_rotation/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/_rotation/tests/__init__.py` & `kikuchipy-0.8.5/kikuchipy/_rotation/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/_rotation/tests/test_rotation.py` & `kikuchipy-0.8.5/kikuchipy/_rotation/tests/test_rotation.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/_util/__init__.py` & `kikuchipy-0.8.5/kikuchipy/_util/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/_util/_deprecated.py` & `kikuchipy-0.8.5/kikuchipy/_util/_deprecated.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/_util/_transfer_axes.py` & `kikuchipy-0.8.5/kikuchipy/_util/_transfer_axes.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/_util/tests/__init__.py` & `kikuchipy-0.8.5/kikuchipy/_util/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/_util/tests/test_deprecated.py` & `kikuchipy-0.8.5/kikuchipy/_util/tests/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/_util/tests/test_import.py` & `kikuchipy-0.8.5/kikuchipy/_util/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/_util/tests/test_logging.py` & `kikuchipy-0.8.5/kikuchipy/_util/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/conftest.py` & `kikuchipy-0.8.5/kikuchipy/conftest.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/__init__.py` & `kikuchipy-0.8.5/kikuchipy/data/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/_data.py` & `kikuchipy-0.8.5/kikuchipy/data/_data.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/_registry.py` & `kikuchipy-0.8.5/kikuchipy/data/_registry.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/bruker_h5ebsd/create_bruker_h5ebsd_file.py` & `kikuchipy-0.8.5/kikuchipy/data/bruker_h5ebsd/create_bruker_h5ebsd_file.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/bruker_h5ebsd/patterns.h5` & `kikuchipy-0.8.5/kikuchipy/data/bruker_h5ebsd/patterns.h5`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/bruker_h5ebsd/patterns_roi.h5` & `kikuchipy-0.8.5/kikuchipy/data/bruker_h5ebsd/patterns_roi.h5`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/bruker_h5ebsd/patterns_roi_nonrectangular.h5` & `kikuchipy-0.8.5/kikuchipy/data/bruker_h5ebsd/patterns_roi_nonrectangular.h5`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/edax_binary/create_dummy_edax_binary_file.py` & `kikuchipy-0.8.5/kikuchipy/data/edax_binary/create_dummy_edax_binary_file.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/edax_binary/edax_binary.up1` & `kikuchipy-0.8.5/kikuchipy/data/edax_binary/edax_binary.up1`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/edax_binary/edax_binary.up2` & `kikuchipy-0.8.5/kikuchipy/data/edax_binary/edax_binary.up2`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/edax_h5ebsd/patterns.h5` & `kikuchipy-0.8.5/kikuchipy/data/edax_h5ebsd/patterns.h5`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/emsoft_ebsd/EBSD_TEST_Ni.h5` & `kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd/EBSD_TEST_Ni.h5`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/emsoft_ebsd/create_dummy_emsoft_ebsd_file.py` & `kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd/create_dummy_emsoft_ebsd_file.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/emsoft_ebsd/simulated_ebsd.h5` & `kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd/simulated_ebsd.h5`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/emsoft_ebsd_master_pattern/convert_emsoft_ebsd_masterpattern_file_uint8_gzip.py` & `kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd_master_pattern/convert_emsoft_ebsd_masterpattern_file_uint8_gzip.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/emsoft_ebsd_master_pattern/create_dummy_emsoft_ebsd_master_pattern_file.py` & `kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd_master_pattern/create_dummy_emsoft_ebsd_master_pattern_file.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/emsoft_ebsd_master_pattern/master_patterns.h5` & `kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd_master_pattern/master_patterns.h5`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/emsoft_ebsd_master_pattern/ni.xtal` & `kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd_master_pattern/ni.xtal`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/emsoft_ebsd_master_pattern/ni_ebsdmaster.nml` & `kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd_master_pattern/ni_ebsdmaster.nml`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mc.out` & `kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mc.out`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mc_mp_20kv_uint8_gzip_opts9.h5` & `kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mc_mp_20kv_uint8_gzip_opts9.h5`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mcopencl.nml` & `kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mcopencl.nml`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mp.out` & `kikuchipy-0.8.5/kikuchipy/data/emsoft_ebsd_master_pattern/ni_mp.out`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/emsoft_ecp_master_pattern/create_dummy_emsoft_ecp_master_pattern_file.py` & `kikuchipy-0.8.5/kikuchipy/data/emsoft_ecp_master_pattern/create_dummy_emsoft_ecp_master_pattern_file.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/emsoft_ecp_master_pattern/ecp_master_pattern.h5` & `kikuchipy-0.8.5/kikuchipy/data/emsoft_ecp_master_pattern/ecp_master_pattern.h5`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/emsoft_tkd_master_pattern/create_dummy_emsoft_tkd_master_pattern_file.py` & `kikuchipy-0.8.5/kikuchipy/data/emsoft_tkd_master_pattern/create_dummy_emsoft_tkd_master_pattern_file.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/emsoft_tkd_master_pattern/tkd_master_pattern.h5` & `kikuchipy-0.8.5/kikuchipy/data/emsoft_tkd_master_pattern/tkd_master_pattern.h5`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/kikuchipy_h5ebsd/patterns.h5` & `kikuchipy-0.8.5/kikuchipy/data/kikuchipy_h5ebsd/patterns.h5`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/kikuchipy_h5ebsd/patterns_nochunks.h5` & `kikuchipy-0.8.5/kikuchipy/data/kikuchipy_h5ebsd/patterns_nochunks.h5`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/nordif/Background acquisition pattern.bmp` & `kikuchipy-0.8.5/kikuchipy/data/nordif/Background acquisition pattern.bmp`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/nordif/Background calibration pattern.bmp` & `kikuchipy-0.8.5/kikuchipy/data/nordif/Background calibration pattern.bmp`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/nordif/Calibration (294,532).bmp` & `kikuchipy-0.8.5/kikuchipy/data/nordif/Calibration (294,532).bmp`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/nordif/Calibration (425,447).bmp` & `kikuchipy-0.8.5/kikuchipy/data/nordif/Calibration (425,447).bmp`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/nordif/Pattern.dat` & `kikuchipy-0.8.5/kikuchipy/data/nordif/Pattern.dat`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/nordif/Setting.txt` & `kikuchipy-0.8.5/kikuchipy/data/nordif/Setting.txt`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/nordif/Setting_bad1.txt` & `kikuchipy-0.8.5/kikuchipy/data/nordif/Setting_bad1.txt`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/nordif/Setting_bad2.txt` & `kikuchipy-0.8.5/kikuchipy/data/nordif/Setting_bad2.txt`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/nordif/Setting_bad3.txt` & `kikuchipy-0.8.5/kikuchipy/data/nordif/Setting_bad3.txt`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/oxford_binary/create_dummy_oxford_binary_file.py` & `kikuchipy-0.8.5/kikuchipy/data/oxford_binary/create_dummy_oxford_binary_file.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/oxford_binary/patterns.ebsp` & `kikuchipy-0.8.5/kikuchipy/data/oxford_binary/patterns.ebsp`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/oxford_h5ebsd/create_oxford_h5ebsd_file.py` & `kikuchipy-0.8.5/kikuchipy/data/oxford_h5ebsd/create_oxford_h5ebsd_file.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/oxford_h5ebsd/patterns.h5oina` & `kikuchipy-0.8.5/kikuchipy/data/oxford_h5ebsd/patterns.h5oina`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/tests/__init__.py` & `kikuchipy-0.8.5/kikuchipy/data/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/data/tests/test_data.py` & `kikuchipy-0.8.5/kikuchipy/data/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/detectors/__init__.py` & `kikuchipy-0.8.5/kikuchipy/detectors/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/detectors/calibration.py` & `kikuchipy-0.8.5/kikuchipy/detectors/calibration.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/detectors/ebsd_detector.py` & `kikuchipy-0.8.5/kikuchipy/detectors/ebsd_detector.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/detectors/tests/__init__.py` & `kikuchipy-0.8.5/kikuchipy/detectors/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/detectors/tests/test_calibration.py` & `kikuchipy-0.8.5/kikuchipy/detectors/tests/test_calibration.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/detectors/tests/test_ebsd_detector.py` & `kikuchipy-0.8.5/kikuchipy/detectors/tests/test_ebsd_detector.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/draw/__init__.py` & `kikuchipy-0.8.5/kikuchipy/draw/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/draw/_navigators.py` & `kikuchipy-0.8.5/kikuchipy/draw/_navigators.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/draw/_plot_pattern_positions_in_map.py` & `kikuchipy-0.8.5/kikuchipy/draw/_plot_pattern_positions_in_map.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/draw/colors.py` & `kikuchipy-0.8.5/kikuchipy/draw/colors.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/draw/markers.py` & `kikuchipy-0.8.5/kikuchipy/draw/markers.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/draw/tests/__init__.py` & `kikuchipy-0.8.5/kikuchipy/draw/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/draw/tests/test_colors.py` & `kikuchipy-0.8.5/kikuchipy/draw/tests/test_colors.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/draw/tests/test_markers.py` & `kikuchipy-0.8.5/kikuchipy/draw/tests/test_markers.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/draw/tests/test_navigators.py` & `kikuchipy-0.8.5/kikuchipy/draw/tests/test_navigators.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/draw/tests/test_plot_pattern_positions_in_map.py` & `kikuchipy-0.8.5/kikuchipy/draw/tests/test_plot_pattern_positions_in_map.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/filters/__init__.py` & `kikuchipy-0.8.5/kikuchipy/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/filters/fft_barnes.py` & `kikuchipy-0.8.5/kikuchipy/filters/fft_barnes.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/filters/tests/__init__.py` & `kikuchipy-0.8.5/kikuchipy/filters/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/filters/tests/test_fft_barnes.py` & `kikuchipy-0.8.5/kikuchipy/filters/tests/test_fft_barnes.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/filters/tests/test_window.py` & `kikuchipy-0.8.5/kikuchipy/filters/tests/test_window.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/filters/window.py` & `kikuchipy-0.8.5/kikuchipy/filters/window.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/generators/__init__.py` & `kikuchipy-0.8.5/kikuchipy/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/generators/tests/__init__.py` & `kikuchipy-0.8.5/kikuchipy/generators/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/generators/tests/test_virtual_bse_generator.py` & `kikuchipy-0.8.5/kikuchipy/generators/tests/test_virtual_bse_generator.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/generators/virtual_bse_generator.py` & `kikuchipy-0.8.5/kikuchipy/generators/virtual_bse_generator.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/hyperspy_extension.yaml` & `kikuchipy-0.8.5/kikuchipy/hyperspy_extension.yaml`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/imaging/__init__.py` & `kikuchipy-0.8.5/kikuchipy/imaging/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/imaging/tests/__init__.py` & `kikuchipy-0.8.5/kikuchipy/imaging/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/imaging/tests/test_virtual_bse_imager.py` & `kikuchipy-0.8.5/kikuchipy/imaging/tests/test_virtual_bse_imager.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/imaging/vbse.py` & `kikuchipy-0.8.5/kikuchipy/imaging/vbse.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/indexing/__init__.py` & `kikuchipy-0.8.5/kikuchipy/indexing/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/indexing/_dictionary_indexing.py` & `kikuchipy-0.8.5/kikuchipy/indexing/_dictionary_indexing.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/indexing/_hough_indexing.py` & `kikuchipy-0.8.5/kikuchipy/indexing/_hough_indexing.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/indexing/_merge_crystal_maps.py` & `kikuchipy-0.8.5/kikuchipy/indexing/_merge_crystal_maps.py`

 * *Files 4% similar despite different names*

```diff
@@ -190,15 +190,17 @@
     comb_shape = (map_size,)
     if n_scores_per_point > 1:
         comb_shape += (n_scores_per_point,)
     comb_shape += (n_maps,)
 
     # Combined (unsorted) scores array of shape (M, N, K) or (M, K)
     scores_dtype = crystal_maps[0].prop[scores_prop].dtype
-    combined_scores = np.full(comb_shape, np.nan, dtype=scores_dtype)
+    combined_scores = np.full(
+        comb_shape, np.nan, dtype=np.dtype(f"f{scores_dtype.itemsize}")
+    )
     for i, (mask, xmap) in enumerate(zip(navigation_masks1d, crystal_maps)):
         if mask is not None:
             combined_scores[mask, ..., i] = xmap.prop[scores_prop]
         else:
             combined_scores[..., i] = xmap.prop[scores_prop]
 
     # Best score in each map point
@@ -208,43 +210,59 @@
             best_scores = np.nanmean(best_scores, axis=1)
     else:  # (M, K)
         best_scores = combined_scores
 
     # Phase of best score in each map point
     phase_id = np.nanargmax(sign * best_scores, axis=1)
 
+    # Set the phase ID of points marked as not-indexed in all maps to -1
+    not_indexed = np.zeros((n_maps, map_size), dtype=bool)
+    for i in range(n_maps):
+        mask = navigation_masks1d[i]
+        xmap = crystal_maps[i]
+        if mask is not None:
+            not_indexed[i, mask][xmap.phase_id == -1] = True
+        else:
+            not_indexed[i, xmap.phase_id == -1] = True
+    not_indexed = np.logical_and.reduce(not_indexed)
+    phase_id[not_indexed] = -1
+
     # Get the new crystal map's rotations, scores and indices,
     # restricted to one phase per point (uncombined)
     new_rotations = np.zeros(comb_shape[:-1] + (4,), dtype="float")
     new_scores = np.zeros(comb_shape[:-1], dtype=scores_dtype)
 
     if simulation_indices_prop is not None:
         new_indices = np.zeros(comb_shape[:-1], dtype="int32")
 
     phase_list = PhaseList()
+    if -1 in phase_id:
+        phase_list.add_not_indexed()
     for i, (nav_mask1d, xmap) in enumerate(zip(navigation_masks1d, crystal_maps)):
         phase_mask = phase_id == i
 
         if phase_mask.any():
-            current_id = xmap.phases_in_data.ids[0]
-            phase = xmap.phases_in_data[current_id].deepcopy()
+            phase_ids = xmap.phases_in_data.ids
+            if -1 in phase_ids:
+                phase_ids.remove(-1)
+            phase = xmap.phases_in_data[phase_ids[0]].deepcopy()
             if phase.name in phase_list.names:
                 # If they are equal, do not duplicate it in the phase
                 # list but update the phase ID
                 equal_phases, different = _equal_phase(phase, phase_list[phase.name])
                 if equal_phases:
                     phase_id[phase_mask] = phase_list.id_from_name(phase.name)
                 else:
                     name = phase.name
+                    phase.name = name + str(i)
                     warnings.warn(
                         f"There are duplicates of phase '{name}' but the phases have "
                         f"different {different}, will therefore rename this phase's "
-                        f"name to '{name + str(i)}' in the merged PhaseList",
+                        f"name to '{phase.name}' in the merged PhaseList",
                     )
-                    phase.name = name + str(i)
                     phase_list.add(phase)
             else:
                 phase_list.add(phase)
         else:
             continue
 
         if nav_mask1d is not None:
```

### Comparing `kikuchipy-0.8.4/kikuchipy/indexing/_orientation_similarity_map.py` & `kikuchipy-0.8.5/kikuchipy/indexing/_orientation_similarity_map.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/indexing/_refinement/__init__.py` & `kikuchipy-0.8.5/kikuchipy/indexing/_refinement/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/indexing/_refinement/_objective_functions.py` & `kikuchipy-0.8.5/kikuchipy/indexing/_refinement/_objective_functions.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/indexing/_refinement/_refinement.py` & `kikuchipy-0.8.5/kikuchipy/indexing/_refinement/_refinement.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/indexing/_refinement/_solvers.py` & `kikuchipy-0.8.5/kikuchipy/indexing/_refinement/_solvers.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/indexing/similarity_metrics/__init__.py` & `kikuchipy-0.8.5/kikuchipy/indexing/similarity_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/indexing/similarity_metrics/_normalized_cross_correlation.py` & `kikuchipy-0.8.5/kikuchipy/indexing/similarity_metrics/_normalized_cross_correlation.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/indexing/similarity_metrics/_normalized_dot_product.py` & `kikuchipy-0.8.5/kikuchipy/indexing/similarity_metrics/_normalized_dot_product.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/indexing/similarity_metrics/_similarity_metric.py` & `kikuchipy-0.8.5/kikuchipy/indexing/similarity_metrics/_similarity_metric.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/indexing/tests/__init__.py` & `kikuchipy-0.8.5/kikuchipy/indexing/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/indexing/tests/test_dictionary_indexing.py` & `kikuchipy-0.8.5/kikuchipy/indexing/tests/test_dictionary_indexing.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/indexing/tests/test_ebsd_refinement.py` & `kikuchipy-0.8.5/kikuchipy/indexing/tests/test_ebsd_refinement.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/indexing/tests/test_merge_crystal_maps.py` & `kikuchipy-0.8.5/kikuchipy/indexing/tests/test_merge_crystal_maps.py`

 * *Files 5% similar despite different names*

```diff
@@ -555,15 +555,15 @@
                 12, 13, 14, 15,
                 16,  5,  6,  7,
                 20,  9, 10, 11,
             ]
         )
         # fmt: on
 
-        # All points in a map should be used, but not in another one:
+        # All points in one map should be used, but not in another:
         # Only consider xmap1 in the first row and first column (mask it
         # out everywhere else)
         xmap6 = merge_crystal_maps(
             [xmap1[nav_mask1.ravel()], xmap2], navigation_masks=[~nav_mask1, None]
         )
         # fmt: off
         assert np.allclose(
@@ -640,7 +640,45 @@
 
         # A mask is not a NumPy array
         with pytest.raises(ValueError, match="1. navigation mask must be a NumPy "):
             _ = merge_crystal_maps(
                 [xmap1[~nav_mask1.ravel()], xmap2[~nav_mask2.ravel()]],
                 navigation_masks=[nav_mask1, list(nav_mask2)],
             )
+
+    def test_not_indexed(self):
+        xmap_a = CrystalMap.empty((4, 3))
+        is_indexed_a = np.array(
+            [[1, 1, 0], [1, 0, 1], [0, 1, 1], [0, 1, 1]], dtype=bool
+        ).ravel()
+        xmap_a.phases.add_not_indexed()
+        xmap_a.phases[0].name = "a"
+        xmap_a[~is_indexed_a].phase_id = -1
+        xmap_a.prop["scores"] = np.array(
+            [[2, 2, 0], [3, 0, 4], [0, 4, 3], [0, 2, 1]], dtype=float
+        ).ravel()
+        xmap_a._rotations = xmap_a.rotations * Rotation.from_axes_angles(
+            [0, 0, 1], 30, degrees=True
+        )
+
+        xmap_b = CrystalMap.empty((4, 3))
+        is_indexed_b = np.array(
+            [[1, 1, 0], [1, 1, 1], [0, 1, 1], [0, 1, 0]], dtype=bool
+        ).ravel()
+        xmap_b.phases.add_not_indexed()
+        xmap_b.phases[0].name = "b"
+        xmap_b[~is_indexed_b].phase_id = -1
+        xmap_b.prop["scores"] = np.array(
+            [[3, 1, 0], [2, 1, 5], [0, 2, 4], [0, 1, 0]], dtype=float
+        ).ravel()
+        xmap_b._rotations = xmap_b.rotations * Rotation.from_axes_angles(
+            [0, 0, 1], 60, degrees=True
+        )
+
+        xmap_ab = merge_crystal_maps([xmap_a, xmap_b])
+
+        assert np.allclose(xmap_ab.phase_id, [1, 0, -1, 0, 1, 1, -1, 0, 1, -1, 0, 0])
+        assert np.allclose(
+            xmap_ab["indexed"].rotations.angle,
+            np.deg2rad([60, 30, 30, 60, 60, 30, 60, 30, 30]),
+        )
+        assert np.allclose(xmap_ab["indexed"].scores, [3, 2, 3, 1, 5, 4, 4, 2, 1])
```

### Comparing `kikuchipy-0.8.4/kikuchipy/indexing/tests/test_orientation_similarity_map.py` & `kikuchipy-0.8.5/kikuchipy/indexing/tests/test_orientation_similarity_map.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/indexing/tests/test_similarity_metrics.py` & `kikuchipy-0.8.5/kikuchipy/indexing/tests/test_similarity_metrics.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/io/__init__.py` & `kikuchipy-0.8.5/kikuchipy/io/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/io/_io.py` & `kikuchipy-0.8.5/kikuchipy/io/_io.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/io/_util.py` & `kikuchipy-0.8.5/kikuchipy/io/_util.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/io/plugins/__init__.py` & `kikuchipy-0.8.5/kikuchipy/io/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/io/plugins/_emsoft_master_pattern.py` & `kikuchipy-0.8.5/kikuchipy/io/plugins/_emsoft_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/io/plugins/_h5ebsd.py` & `kikuchipy-0.8.5/kikuchipy/io/plugins/_h5ebsd.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/io/plugins/bruker_h5ebsd.py` & `kikuchipy-0.8.5/kikuchipy/io/plugins/bruker_h5ebsd.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/io/plugins/ebsd_directory.py` & `kikuchipy-0.8.5/kikuchipy/io/plugins/ebsd_directory.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/io/plugins/edax_binary.py` & `kikuchipy-0.8.5/kikuchipy/io/plugins/edax_binary.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/io/plugins/edax_h5ebsd.py` & `kikuchipy-0.8.5/kikuchipy/io/plugins/edax_h5ebsd.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/io/plugins/emsoft_ebsd.py` & `kikuchipy-0.8.5/kikuchipy/io/plugins/emsoft_ebsd.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/io/plugins/emsoft_ebsd_master_pattern.py` & `kikuchipy-0.8.5/kikuchipy/io/plugins/emsoft_ebsd_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/io/plugins/emsoft_ecp_master_pattern.py` & `kikuchipy-0.8.5/kikuchipy/io/plugins/emsoft_ecp_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/io/plugins/emsoft_tkd_master_pattern.py` & `kikuchipy-0.8.5/kikuchipy/io/plugins/emsoft_tkd_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/io/plugins/kikuchipy_h5ebsd.py` & `kikuchipy-0.8.5/kikuchipy/io/plugins/kikuchipy_h5ebsd.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/io/plugins/nordif.py` & `kikuchipy-0.8.5/kikuchipy/io/plugins/nordif.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/io/plugins/nordif_calibration_patterns.py` & `kikuchipy-0.8.5/kikuchipy/io/plugins/nordif_calibration_patterns.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/io/plugins/oxford_binary.py` & `kikuchipy-0.8.5/kikuchipy/io/plugins/oxford_binary.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/io/plugins/oxford_h5ebsd.py` & `kikuchipy-0.8.5/kikuchipy/io/plugins/oxford_h5ebsd.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/io/plugins/tests/__init__.py` & `kikuchipy-0.8.5/kikuchipy/io/plugins/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/io/plugins/tests/test_bruker_h5ebsd.py` & `kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_bruker_h5ebsd.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/io/plugins/tests/test_ebsd_directory.py` & `kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_ebsd_directory.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/io/plugins/tests/test_edax_binary.py` & `kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_edax_binary.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/io/plugins/tests/test_edax_h5ebsd.py` & `kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_edax_h5ebsd.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/io/plugins/tests/test_emsoft_ebsd.py` & `kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_emsoft_ebsd.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/io/plugins/tests/test_emsoft_ebsd_master_pattern.py` & `kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_emsoft_ebsd_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/io/plugins/tests/test_emsoft_ecp_master_pattern.py` & `kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_emsoft_ecp_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/io/plugins/tests/test_emsoft_master_pattern.py` & `kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_emsoft_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/io/plugins/tests/test_emsoft_tkd_master_pattern.py` & `kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_emsoft_tkd_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/io/plugins/tests/test_kikuchipy_h5ebsd.py` & `kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_kikuchipy_h5ebsd.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/io/plugins/tests/test_nordif.py` & `kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_nordif.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/io/plugins/tests/test_nordif_calibration_patterns.py` & `kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_nordif_calibration_patterns.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/io/plugins/tests/test_oxford_binary.py` & `kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_oxford_binary.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/io/plugins/tests/test_oxford_h5ebsd.py` & `kikuchipy-0.8.5/kikuchipy/io/plugins/tests/test_oxford_h5ebsd.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/io/tests/__init__.py` & `kikuchipy-0.8.5/kikuchipy/io/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/io/tests/test_io.py` & `kikuchipy-0.8.5/kikuchipy/io/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/io/tests/test_util.py` & `kikuchipy-0.8.5/kikuchipy/io/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/pattern/__init__.py` & `kikuchipy-0.8.5/kikuchipy/pattern/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/pattern/_pattern.py` & `kikuchipy-0.8.5/kikuchipy/pattern/_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/pattern/chunk.py` & `kikuchipy-0.8.5/kikuchipy/pattern/chunk.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/pattern/tests/__init__.py` & `kikuchipy-0.8.5/kikuchipy/pattern/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/pattern/tests/test_chunk.py` & `kikuchipy-0.8.5/kikuchipy/pattern/tests/test_chunk.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/pattern/tests/test_pattern.py` & `kikuchipy-0.8.5/kikuchipy/pattern/tests/test_pattern.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,14 +177,15 @@
         p5 = _remove_background_subtract.py_func(p.astype("float32"), bg, 0, 255)
         assert p5.min() == 0
         assert p5.max() == 255
 
         assert np.allclose(p0, p)
         assert p0.dtype == p.dtype
 
+    @pytest.mark.filterwarnings("ignore:invalid value")
     def test_remove_static_background_divide(self, dummy_signal, dummy_background):
         p = dummy_signal.inav[0, 0].data
         dtype_out = p.dtype
         dtype = np.float32
         bg = dummy_background.astype(dtype)
 
         p0 = p.copy()
```

### Comparing `kikuchipy-0.8.4/kikuchipy/projections/__init__.py` & `kikuchipy-0.8.5/kikuchipy/projections/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/projections/gnomonic_projection.py` & `kikuchipy-0.8.5/kikuchipy/projections/gnomonic_projection.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/projections/hesse_normal_form.py` & `kikuchipy-0.8.5/kikuchipy/projections/hesse_normal_form.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/projections/lambert_projection.py` & `kikuchipy-0.8.5/kikuchipy/projections/lambert_projection.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/projections/spherical_projection.py` & `kikuchipy-0.8.5/kikuchipy/projections/spherical_projection.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/projections/tests/__init__.py` & `kikuchipy-0.8.5/kikuchipy/projections/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/projections/tests/test_gnomonic_projection.py` & `kikuchipy-0.8.5/kikuchipy/projections/tests/test_gnomonic_projection.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/projections/tests/test_hesse_normal_form.py` & `kikuchipy-0.8.5/kikuchipy/projections/tests/test_hesse_normal_form.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/projections/tests/test_lambert_projection.py` & `kikuchipy-0.8.5/kikuchipy/projections/tests/test_lambert_projection.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/projections/tests/test_spherical_projection.py` & `kikuchipy-0.8.5/kikuchipy/projections/tests/test_spherical_projection.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/release.py` & `kikuchipy-0.8.5/kikuchipy/release.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,8 +33,8 @@
 ]
 license = "GPLv3+"
 maintainer = "Håkon Wiik Ånes"
 maintainer_email = "hakon.w.anes@ntnu.no"
 name = "kikuchipy"
 platforms = ["Linux", "MacOS X", "Windows"]
 status = "Development"
-version = "0.8.4"
+version = "0.8.5"
```

### Comparing `kikuchipy-0.8.4/kikuchipy/signals/__init__.py` & `kikuchipy-0.8.5/kikuchipy/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/signals/_kikuchi_master_pattern.py` & `kikuchipy-0.8.5/kikuchipy/signals/_kikuchi_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/signals/_kikuchipy_signal.py` & `kikuchipy-0.8.5/kikuchipy/signals/_kikuchipy_signal.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/signals/ebsd.py` & `kikuchipy-0.8.5/kikuchipy/signals/ebsd.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/signals/ebsd_master_pattern.py` & `kikuchipy-0.8.5/kikuchipy/signals/ebsd_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/signals/ecp_master_pattern.py` & `kikuchipy-0.8.5/kikuchipy/signals/ecp_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/signals/tests/__init__.py` & `kikuchipy-0.8.5/kikuchipy/signals/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/signals/tests/test_ebsd.py` & `kikuchipy-0.8.5/kikuchipy/signals/tests/test_ebsd.py`

 * *Files 1% similar despite different names*

```diff
@@ -553,14 +553,15 @@
         assert np.allclose(dummy_signal.inav[0, 0].data, answer, atol=1e-4)
 
     def test_remove_dynamic_background_raises(self, dummy_signal):
         filter_domain = "wildmount"
         with pytest.raises(ValueError, match=f"{filter_domain} must be "):
             dummy_signal.remove_dynamic_background(filter_domain=filter_domain)
 
+    @pytest.mark.filterwarnings("ignore:invalid value")
     def test_inplace(self, dummy_signal):
         # Current signal is unaffected
         s = dummy_signal.deepcopy()
         s2 = dummy_signal.remove_dynamic_background(inplace=False)
         assert np.allclose(s.data, dummy_signal.data)
 
         # Custom properties carry over
@@ -576,14 +577,15 @@
         # Operating on lazy signal returns lazy signal
         s3 = s.as_lazy()
         s4 = s3.remove_dynamic_background(inplace=False)
         assert isinstance(s4, kp.signals.LazyEBSD)
         s4.compute()
         assert np.allclose(s4.data, dummy_signal.data)
 
+    @pytest.mark.filterwarnings("ignore:invalid value")
     def test_lazy_output(self, dummy_signal):
         with pytest.raises(
             ValueError, match="`lazy_output=True` requires `inplace=False`"
         ):
             _ = dummy_signal.remove_dynamic_background(lazy_output=True)
 
         s2 = dummy_signal.remove_dynamic_background(inplace=False, lazy_output=True)
```

### Comparing `kikuchipy-0.8.4/kikuchipy/signals/tests/test_ebsd_hough_indexing.py` & `kikuchipy-0.8.5/kikuchipy/signals/tests/test_ebsd_hough_indexing.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/signals/tests/test_ebsd_master_pattern.py` & `kikuchipy-0.8.5/kikuchipy/signals/tests/test_ebsd_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/signals/tests/test_ecp_master_pattern.py` & `kikuchipy-0.8.5/kikuchipy/signals/tests/test_ecp_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/signals/tests/test_kikuchi_master_pattern.py` & `kikuchipy-0.8.5/kikuchipy/signals/tests/test_kikuchi_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/signals/tests/test_virtual_bse_image.py` & `kikuchipy-0.8.5/kikuchipy/signals/tests/test_virtual_bse_image.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/signals/util/__init__.py` & `kikuchipy-0.8.5/kikuchipy/signals/util/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/signals/util/_crystal_map.py` & `kikuchipy-0.8.5/kikuchipy/signals/util/_crystal_map.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/signals/util/_dask.py` & `kikuchipy-0.8.5/kikuchipy/signals/util/_dask.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/signals/util/_detector.py` & `kikuchipy-0.8.5/kikuchipy/signals/util/_detector.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/signals/util/_map_helper.py` & `kikuchipy-0.8.5/kikuchipy/signals/util/_map_helper.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/signals/util/_master_pattern.py` & `kikuchipy-0.8.5/kikuchipy/signals/util/_master_pattern.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/signals/util/_overwrite_hyperspy_methods.py` & `kikuchipy-0.8.5/kikuchipy/signals/util/_overwrite_hyperspy_methods.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/signals/util/array_tools.py` & `kikuchipy-0.8.5/kikuchipy/signals/util/array_tools.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/signals/util/tests/__init__.py` & `kikuchipy-0.8.5/kikuchipy/signals/util/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/signals/util/tests/test_array_tools.py` & `kikuchipy-0.8.5/kikuchipy/signals/util/tests/test_array_tools.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/signals/util/tests/test_dask.py` & `kikuchipy-0.8.5/kikuchipy/signals/util/tests/test_dask.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/signals/util/tests/test_overwrite_hyperspy_methods.py` & `kikuchipy-0.8.5/kikuchipy/signals/util/tests/test_overwrite_hyperspy_methods.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/signals/virtual_bse_image.py` & `kikuchipy-0.8.5/kikuchipy/signals/virtual_bse_image.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/simulations/__init__.py` & `kikuchipy-0.8.5/kikuchipy/simulations/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/simulations/_kikuchi_pattern_features.py` & `kikuchipy-0.8.5/kikuchipy/simulations/_kikuchi_pattern_features.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/simulations/_kikuchi_pattern_simulation.py` & `kikuchipy-0.8.5/kikuchipy/simulations/_kikuchi_pattern_simulation.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/simulations/kikuchi_pattern_simulator.py` & `kikuchipy-0.8.5/kikuchipy/simulations/kikuchi_pattern_simulator.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/simulations/tests/__init__.py` & `kikuchipy-0.8.5/kikuchipy/simulations/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/simulations/tests/test_kikuchi_pattern_simulation.py` & `kikuchipy-0.8.5/kikuchipy/simulations/tests/test_kikuchi_pattern_simulation.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy/simulations/tests/test_kikuchi_pattern_simulator.py` & `kikuchipy-0.8.5/kikuchipy/simulations/tests/test_kikuchi_pattern_simulator.py`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy.egg-info/PKG-INFO` & `kikuchipy-0.8.5/kikuchipy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kikuchipy
-Version: 0.8.4
+Version: 0.8.5
 Summary: Processing, simulating and indexing of electron backscatter diffraction (EBSD) patterns.
 Home-page: https://kikuchipy.org
 Download-URL: https://pypi.python.org/pypi/kikuchipy
 Author: kikuchipy developers
 Author-email: hakon.w.anes@ntnu.no
 Maintainer: Håkon Wiik Ånes
 Maintainer-email: hakon.w.anes@ntnu.no
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kikuchipy Version: 0.8.4 Summary: Processing,
+Metadata-Version: 2.1 Name: kikuchipy Version: 0.8.5 Summary: Processing,
 simulating and indexing of electron backscatter diffraction (EBSD) patterns.
 Home-page: https://kikuchipy.org Download-URL: https://pypi.python.org/pypi/
 kikuchipy Author: kikuchipy developers Author-email: hakon.w.anes@ntnu.no
 Maintainer: HÃ¥kon Wiik Ãnes Maintainer-email: hakon.w.anes@ntnu.no License:
 GPLv3+ Project-URL: Bug Tracker, https://github.com/pyxem/kikuchipy/issues
 Project-URL: Documentation, https://kikuchipy.org Project-URL: Source Code,
 https://github.com/pyxem/kikuchipy Keywords: EBSD,electron backscatter
```

### Comparing `kikuchipy-0.8.4/kikuchipy.egg-info/SOURCES.txt` & `kikuchipy-0.8.5/kikuchipy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/kikuchipy.egg-info/requires.txt` & `kikuchipy-0.8.5/kikuchipy.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/readthedocs.yaml` & `kikuchipy-0.8.5/readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/setup.cfg` & `kikuchipy-0.8.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `kikuchipy-0.8.4/setup.py` & `kikuchipy-0.8.5/setup.py`

 * *Files identical despite different names*

