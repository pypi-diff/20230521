# Comparing `tmp/pyglove-0.3.1.dev20230520.tar.gz` & `tmp/pyglove-0.3.1.dev20230521.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyglove-0.3.1.dev20230520.tar", last modified: Sat May 20 08:06:29 2023, max compression
+gzip compressed data, was "pyglove-0.3.1.dev20230521.tar", last modified: Sun May 21 08:06:26 2023, max compression
```

## Comparing `pyglove-0.3.1.dev20230520.tar` & `pyglove-0.3.1.dev20230521.tar`

### file list

```diff
@@ -1,190 +1,192 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:06:29.914126 pyglove-0.3.1.dev20230520/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-20 08:06:29.914126 pyglove-0.3.1.dev20230520/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-20 08:06:29.000000 pyglove-0.3.1.dev20230520/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:06:29.898125 pyglove-0.3.1.dev20230520/pyglove/
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:06:29.898125 pyglove-0.3.1.dev20230520/pyglove/core/
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:06:29.898125 pyglove-0.3.1.dev20230520/pyglove/core/detouring/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/detouring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/detouring/class_detour.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/detouring/class_detour_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:06:29.902125 pyglove-0.3.1.dev20230520/pyglove/core/geno/
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/geno/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64370 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/geno/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    38561 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/geno/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/geno/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/geno/categorical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/geno/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/geno/custom_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/geno/deduping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/geno/deduping_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/geno/dna_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/geno/dna_generator_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/geno/numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/geno/numerical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/geno/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/geno/random_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/geno/space.py
--rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/geno/space_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/geno/sweeping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/geno/sweeping_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:06:29.902125 pyglove-0.3.1.dev20230520/pyglove/core/hyper/
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/hyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/hyper/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23216 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/hyper/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/hyper/categorical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/hyper/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/hyper/custom_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/hyper/derived.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/hyper/derived_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22812 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/hyper/dynamic_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/hyper/dynamic_evaluation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/hyper/evolvable.py
--rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/hyper/evolvable_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/hyper/iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/hyper/iter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/hyper/numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/hyper/numerical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22325 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/hyper/object_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/hyper/object_template_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/logging_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:06:29.906125 pyglove-0.3.1.dev20230520/pyglove/core/object_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/object_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/object_utils/codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/object_utils/codegen_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/object_utils/common_traits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/object_utils/common_traits_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/object_utils/docstr_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/object_utils/docstr_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/object_utils/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/object_utils/formatting_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/object_utils/hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/object_utils/hierarchical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/object_utils/missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/object_utils/missing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/object_utils/thread_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/object_utils/thread_local_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18016 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/object_utils/value_location.py
--rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/object_utils/value_location_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:06:29.906125 pyglove-0.3.1.dev20230520/pyglove/core/patching/
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/patching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/patching/object_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/patching/object_factory_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/patching/pattern_based.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/patching/pattern_based_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/patching/rule_based.py
--rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/patching/rule_based_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:06:29.906125 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/
--rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    69750 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/boilerplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/boilerplate_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22447 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/class_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    21508 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/class_wrapper_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    32373 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    57913 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/dict_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/diff_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/flags_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    24149 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/functor.py
--rw-r--r--   0 runner    (1001) docker     (123)    28989 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/functor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    27197 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/list.py
--rw-r--r--   0 runner    (1001) docker     (123)    51901 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/list_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    33102 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    77608 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/object_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/origin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/origin_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/pure_symbolic.py
--rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/schema_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/symbolize.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/symbolize_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:06:29.910125 pyglove-0.3.1.dev20230520/pyglove/core/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/tuning/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/tuning/backend_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/tuning/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/tuning/local_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/tuning/protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/tuning/protocols_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/tuning/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/tuning/sample_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:06:29.910125 pyglove-0.3.1.dev20230520/pyglove/core/typing/
--rw-r--r--   0 runner    (1001) docker     (123)    12965 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/annotation_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/annotation_conversion_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/callable_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/callable_ext_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12647 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/callable_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/callable_signature_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    49302 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/class_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    25636 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/class_schema_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/class_schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/class_schema_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/custom_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/key_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/key_specs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/pytype_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/type_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/type_conversion_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/typed_missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/typed_missing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    79366 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/value_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)   103891 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/value_specs_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:06:29.910125 pyglove-0.3.1.dev20230520/pyglove/ext/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:06:29.910125 pyglove-0.3.1.dev20230520/pyglove/ext/early_stopping/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/early_stopping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/early_stopping/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/early_stopping/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/early_stopping/step_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/early_stopping/step_wise_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:06:29.914126 pyglove-0.3.1.dev20230520/pyglove/ext/evolution/
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/evolution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/evolution/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    29936 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/evolution/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/evolution/hill_climb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/evolution/hill_climb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/evolution/mutators.py
--rw-r--r--   0 runner    (1001) docker     (123)    17424 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/evolution/mutators_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/evolution/neat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/evolution/neat_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/evolution/nsga2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/evolution/nsga2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    40354 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/evolution/recombinators.py
--rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/evolution/recombinators_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/evolution/regularized_evolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/evolution/regularized_evolution_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/evolution/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/evolution/selectors_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/evolution/where.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/evolution/where_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:06:29.914126 pyglove-0.3.1.dev20230520/pyglove/ext/mutfun/
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/mutfun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/mutfun/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    21312 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/mutfun/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/mutfun/basic_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/mutfun/basic_ops_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:06:29.914126 pyglove-0.3.1.dev20230520/pyglove/ext/scalars/
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/scalars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/scalars/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/scalars/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/scalars/maths.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/scalars/maths_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/scalars/randoms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/scalars/randoms_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/scalars/step_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/scalars/step_wise_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:06:29.898125 pyglove-0.3.1.dev20230520/pyglove.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-20 08:06:29.000000 pyglove-0.3.1.dev20230520/pyglove.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-05-20 08:06:29.000000 pyglove-0.3.1.dev20230520/pyglove.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 08:06:29.000000 pyglove-0.3.1.dev20230520/pyglove.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-20 08:06:29.000000 pyglove-0.3.1.dev20230520/pyglove.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-20 08:06:29.000000 pyglove-0.3.1.dev20230520/pyglove.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 08:06:29.914126 pyglove-0.3.1.dev20230520/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:06:26.239312 pyglove-0.3.1.dev20230521/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-21 08:06:26.239312 pyglove-0.3.1.dev20230521/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-21 08:06:24.000000 pyglove-0.3.1.dev20230521/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:06:26.219312 pyglove-0.3.1.dev20230521/pyglove/
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:06:26.219312 pyglove-0.3.1.dev20230521/pyglove/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     8067 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:06:26.219312 pyglove-0.3.1.dev20230521/pyglove/core/detouring/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/detouring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/detouring/class_detour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/detouring/class_detour_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:06:26.219312 pyglove-0.3.1.dev20230521/pyglove/core/geno/
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/geno/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64370 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/geno/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38561 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/geno/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/geno/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/geno/categorical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/geno/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/geno/custom_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/geno/deduping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/geno/deduping_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/geno/dna_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/geno/dna_generator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/geno/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/geno/numerical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/geno/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/geno/random_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/geno/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/geno/space_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/geno/sweeping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/geno/sweeping_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:06:26.223312 pyglove-0.3.1.dev20230521/pyglove/core/hyper/
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/hyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/hyper/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23216 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/hyper/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/hyper/categorical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/hyper/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/hyper/custom_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/hyper/derived.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/hyper/derived_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22812 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/hyper/dynamic_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/hyper/dynamic_evaluation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/hyper/evolvable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/hyper/evolvable_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/hyper/iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/hyper/iter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/hyper/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/hyper/numerical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22325 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/hyper/object_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/hyper/object_template_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/logging_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:06:26.223312 pyglove-0.3.1.dev20230521/pyglove/core/object_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/object_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/object_utils/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/object_utils/codegen_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/object_utils/common_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/object_utils/common_traits_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/object_utils/docstr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/object_utils/docstr_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/object_utils/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/object_utils/formatting_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/object_utils/hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/object_utils/hierarchical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/object_utils/missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/object_utils/missing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/object_utils/thread_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/object_utils/thread_local_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18016 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/object_utils/value_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/object_utils/value_location_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:06:26.227312 pyglove-0.3.1.dev20230521/pyglove/core/patching/
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/patching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/patching/object_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/patching/object_factory_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/patching/pattern_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/patching/pattern_based_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/patching/rule_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/patching/rule_based_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:06:26.231312 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/
+-rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69750 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/boilerplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/boilerplate_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22447 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/class_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21508 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/class_wrapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/compounding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/compounding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32373 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57913 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/dict_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/diff_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/flags_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23864 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/functor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28989 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/functor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27197 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51901 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/list_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34356 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77608 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/object_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/origin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/origin_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/pure_symbolic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/schema_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/symbolize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/symbolize_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:06:26.231312 pyglove-0.3.1.dev20230521/pyglove/core/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/tuning/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/tuning/backend_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/tuning/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/tuning/local_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/tuning/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/tuning/protocols_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/tuning/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/tuning/sample_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:06:26.231312 pyglove-0.3.1.dev20230521/pyglove/core/typing/
+-rw-r--r--   0 runner    (1001) docker     (123)    12965 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/annotation_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/annotation_conversion_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/callable_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/callable_ext_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12647 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/callable_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/callable_signature_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49302 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/class_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25636 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/class_schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/class_schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/class_schema_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/custom_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/key_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/key_specs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/pytype_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/type_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/type_conversion_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/typed_missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/typed_missing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79366 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/value_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103891 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/value_specs_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:06:26.235312 pyglove-0.3.1.dev20230521/pyglove/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:06:26.235312 pyglove-0.3.1.dev20230521/pyglove/ext/early_stopping/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/early_stopping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/early_stopping/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/early_stopping/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/early_stopping/step_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/early_stopping/step_wise_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:06:26.235312 pyglove-0.3.1.dev20230521/pyglove/ext/evolution/
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/evolution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/evolution/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29936 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/evolution/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/evolution/hill_climb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/evolution/hill_climb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/evolution/mutators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17424 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/evolution/mutators_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/evolution/neat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/evolution/neat_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/evolution/nsga2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/evolution/nsga2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40354 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/evolution/recombinators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/evolution/recombinators_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/evolution/regularized_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/evolution/regularized_evolution_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/evolution/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/evolution/selectors_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/evolution/where.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/evolution/where_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:06:26.235312 pyglove-0.3.1.dev20230521/pyglove/ext/mutfun/
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/mutfun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/mutfun/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21312 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/mutfun/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/mutfun/basic_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/mutfun/basic_ops_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:06:26.239312 pyglove-0.3.1.dev20230521/pyglove/ext/scalars/
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/scalars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/scalars/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/scalars/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/scalars/maths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/scalars/maths_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/scalars/randoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/scalars/randoms_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/scalars/step_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/scalars/step_wise_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:06:26.219312 pyglove-0.3.1.dev20230521/pyglove.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-21 08:06:26.000000 pyglove-0.3.1.dev20230521/pyglove.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-05-21 08:06:26.000000 pyglove-0.3.1.dev20230521/pyglove.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 08:06:26.000000 pyglove-0.3.1.dev20230521/pyglove.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-21 08:06:26.000000 pyglove-0.3.1.dev20230521/pyglove.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-21 08:06:26.000000 pyglove-0.3.1.dev20230521/pyglove.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 08:06:26.239312 pyglove-0.3.1.dev20230521/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/setup.py
```

### Comparing `pyglove-0.3.1.dev20230520/LICENSE` & `pyglove-0.3.1.dev20230521/LICENSE`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/PKG-INFO` & `pyglove-0.3.1.dev20230521/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglove
-Version: 0.3.1.dev20230520
+Version: 0.3.1.dev20230521
 Summary: PyGlove: A library for manipulating Python objects.
 Home-page: https://github.com/google/pyglove
 Author: PyGlove Authors
 Author-email: pyglove-authors@google.com
 License: Apache License 2.0
 Keywords: ai machine learning automl mutable symbolic framework meta-programming
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyglove-0.3.1.dev20230520/README.md` & `pyglove-0.3.1.dev20230521/README.md`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/__init__.py` & `pyglove-0.3.1.dev20230521/pyglove/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/__init__.py` & `pyglove-0.3.1.dev20230521/pyglove/core/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,14 +101,20 @@
 
 # Function for wrapping a single class.
 wrap = symbolic.wrap
 
 # Function for wrapping multiple classes under a module.
 wrap_module = symbolic.wrap_module
 
+# Decorator for creating compound class.
+compound = symbolic.compound
+
+# Function for making compound class.
+compound_class = symbolic.compound_class
+
 # Method for declaring a boilerplated class from a symbolic instance.
 boilerplate_class = symbolic.boilerplate_class
 
 #
 # Context manager for swapping wrapped class with their wrappers.
 #
 
@@ -274,12 +280,11 @@
 #
 # Symbols from `logging.py`.
 #
 
 from pyglove.core import logging
 
 
-
 # pylint: enable=g-import-not-at-top
 # pylint: enable=reimported
 # pylint: enable=unused-import
 # pylint: enable=g-bad-import-order
```

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/detouring/__init__.py` & `pyglove-0.3.1.dev20230521/pyglove/core/detouring/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/detouring/class_detour.py` & `pyglove-0.3.1.dev20230521/pyglove/core/detouring/class_detour.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/detouring/class_detour_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/detouring/class_detour_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/geno/__init__.py` & `pyglove-0.3.1.dev20230521/pyglove/core/geno/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/geno/base.py` & `pyglove-0.3.1.dev20230521/pyglove/core/geno/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/geno/base_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/geno/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/geno/categorical.py` & `pyglove-0.3.1.dev20230521/pyglove/core/geno/categorical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/geno/categorical_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/geno/categorical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/geno/custom.py` & `pyglove-0.3.1.dev20230521/pyglove/core/geno/custom.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/geno/custom_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/geno/custom_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/geno/deduping.py` & `pyglove-0.3.1.dev20230521/pyglove/core/geno/deduping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/geno/deduping_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/geno/deduping_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/geno/dna_generator.py` & `pyglove-0.3.1.dev20230521/pyglove/core/geno/dna_generator.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/geno/dna_generator_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/geno/dna_generator_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/geno/numerical.py` & `pyglove-0.3.1.dev20230521/pyglove/core/geno/numerical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/geno/numerical_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/geno/numerical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/geno/random.py` & `pyglove-0.3.1.dev20230521/pyglove/core/geno/random.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/geno/random_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/geno/random_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/geno/space.py` & `pyglove-0.3.1.dev20230521/pyglove/core/geno/space.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/geno/space_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/geno/space_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/geno/sweeping.py` & `pyglove-0.3.1.dev20230521/pyglove/core/geno/sweeping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/geno/sweeping_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/geno/sweeping_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/hyper/__init__.py` & `pyglove-0.3.1.dev20230521/pyglove/core/hyper/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/hyper/base.py` & `pyglove-0.3.1.dev20230521/pyglove/core/hyper/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/hyper/categorical.py` & `pyglove-0.3.1.dev20230521/pyglove/core/hyper/categorical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/hyper/categorical_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/hyper/categorical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/hyper/custom.py` & `pyglove-0.3.1.dev20230521/pyglove/core/hyper/custom.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/hyper/custom_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/hyper/custom_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/hyper/derived.py` & `pyglove-0.3.1.dev20230521/pyglove/core/hyper/derived.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/hyper/derived_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/hyper/derived_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/hyper/dynamic_evaluation.py` & `pyglove-0.3.1.dev20230521/pyglove/core/hyper/dynamic_evaluation.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/hyper/dynamic_evaluation_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/hyper/dynamic_evaluation_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/hyper/evolvable.py` & `pyglove-0.3.1.dev20230521/pyglove/core/hyper/evolvable.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/hyper/evolvable_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/hyper/evolvable_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/hyper/iter.py` & `pyglove-0.3.1.dev20230521/pyglove/core/hyper/iter.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/hyper/iter_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/hyper/iter_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/hyper/numerical.py` & `pyglove-0.3.1.dev20230521/pyglove/core/hyper/numerical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/hyper/numerical_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/hyper/numerical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/hyper/object_template.py` & `pyglove-0.3.1.dev20230521/pyglove/core/hyper/object_template.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/hyper/object_template_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/hyper/object_template_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/logging.py` & `pyglove-0.3.1.dev20230521/pyglove/core/logging.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/logging_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/logging_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/object_utils/__init__.py` & `pyglove-0.3.1.dev20230521/pyglove/core/object_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/object_utils/codegen.py` & `pyglove-0.3.1.dev20230521/pyglove/core/object_utils/codegen.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/object_utils/codegen_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/object_utils/codegen_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/object_utils/common_traits.py` & `pyglove-0.3.1.dev20230521/pyglove/core/object_utils/common_traits.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/object_utils/common_traits_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/object_utils/common_traits_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/object_utils/docstr_utils.py` & `pyglove-0.3.1.dev20230521/pyglove/core/object_utils/docstr_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/object_utils/docstr_utils_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/object_utils/docstr_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/object_utils/formatting.py` & `pyglove-0.3.1.dev20230521/pyglove/core/object_utils/formatting.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/object_utils/formatting_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/object_utils/formatting_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/object_utils/hierarchical.py` & `pyglove-0.3.1.dev20230521/pyglove/core/object_utils/hierarchical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/object_utils/hierarchical_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/object_utils/hierarchical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/object_utils/missing.py` & `pyglove-0.3.1.dev20230521/pyglove/core/object_utils/missing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/object_utils/missing_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/object_utils/missing_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/object_utils/thread_local.py` & `pyglove-0.3.1.dev20230521/pyglove/core/object_utils/thread_local.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/object_utils/thread_local_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/object_utils/thread_local_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/object_utils/value_location.py` & `pyglove-0.3.1.dev20230521/pyglove/core/object_utils/value_location.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/object_utils/value_location_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/object_utils/value_location_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/patching/__init__.py` & `pyglove-0.3.1.dev20230521/pyglove/core/patching/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/patching/object_factory.py` & `pyglove-0.3.1.dev20230521/pyglove/core/patching/object_factory.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/patching/object_factory_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/patching/object_factory_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/patching/pattern_based.py` & `pyglove-0.3.1.dev20230521/pyglove/core/patching/pattern_based.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/patching/pattern_based_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/patching/pattern_based_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/patching/rule_based.py` & `pyglove-0.3.1.dev20230521/pyglove/core/patching/rule_based.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/patching/rule_based_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/patching/rule_based_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/__init__.py` & `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,17 @@
 
 from pyglove.core.symbolic.class_wrapper import ClassWrapper
 from pyglove.core.symbolic.class_wrapper import wrap
 from pyglove.core.symbolic.class_wrapper import wrap_module
 from pyglove.core.symbolic.class_wrapper import apply_wrappers
 
 from pyglove.core.symbolic.symbolize import symbolize
+
+from pyglove.core.symbolic.compounding import compound
+from pyglove.core.symbolic.compounding import compound_class
 from pyglove.core.symbolic.boilerplate import boilerplate_class
 
 # Symbolic operations.
 from pyglove.core.symbolic.base import traverse
 from pyglove.core.symbolic.base import query
 
 from pyglove.core.symbolic.base import eq
```

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/base.py` & `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/base_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/boilerplate.py` & `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/boilerplate.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/boilerplate_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/boilerplate_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/class_wrapper.py` & `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/class_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/class_wrapper_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/class_wrapper_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/dict.py` & `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/dict.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/dict_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/dict_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/diff.py` & `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/diff.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/diff_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/diff_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/flags.py` & `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/flags.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/flags_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/flags_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/functor.py` & `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/functor.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,44 +25,15 @@
 from pyglove.core import typing as pg_typing
 from pyglove.core.symbolic import base
 from pyglove.core.symbolic import flags
 from pyglove.core.symbolic import object as pg_object
 from pyglove.core.symbolic import schema_utils
 
 
-class FunctorMeta(pg_object.ObjectMeta):
-  """Functor meta class."""
-
-  def _on_schema_update(cls) -> None:   # pylint: disable=no-self-argument
-    super()._on_schema_update()
-    cls._update_init_signature()
-    cls._update_call_signature()
-
-  def _update_call_signature(cls) -> None:  # pylint: disable=no-self-argument
-    """Updates call signature."""
-    call_signature = pg_typing.Signature.from_schema(
-        cls.schema, name='__call__',
-        module_name=cls.__module__, qualname=cls.__qualname__,
-        is_method=False)
-    setattr(cls, 'signature', call_signature)
-
-  def _update_init_signature(cls) -> None:  # pylint: disable=no-self-argument
-    """Updates __init__ signature."""
-    init_signature = pg_typing.Signature.from_schema(
-        cls.schema, name='__init__',
-        module_name=cls.__module__, qualname=cls.__qualname__)
-
-    pseudo_init = init_signature.make_function(['pass'])
-    @functools.wraps(pseudo_init)
-    def _init(self, *args, **kwargs):
-      Functor.__init__(self, *args, **kwargs)
-    setattr(cls, '__init__', _init)
-
-
-class Functor(pg_object.Object, object_utils.Functor, metaclass=FunctorMeta):
+class Functor(pg_object.Object, object_utils.Functor):
   """Symbolic functions (Functors).
 
   A symbolic function is a symbolic class with a ``__call__`` method, whose
   arguments can be bound partially, incrementally bound by attribute
   assignment, or provided at call time.
 
   Another useful trait is that a symbolic function is serializable, when
@@ -106,14 +77,46 @@
   # `pg.functor` or `pg.symbolize`. Therefore we do not infer the schema
   # automatically during class creation.
   auto_schema = False
 
   # Signature of this function.
   signature: pg_typing.Signature
 
+  #
+  # Customizable class traits.
+  #
+
+  @classmethod
+  def _update_signatures_based_on_schema(cls):
+    # Update __init_ signature.
+    init_signature = pg_typing.Signature.from_schema(
+        cls.schema,
+        name='__init__',
+        module_name=cls.__module__,
+        qualname=cls.__qualname__,
+    )
+
+    pseudo_init = init_signature.make_function(['pass'])
+
+    @functools.wraps(pseudo_init)
+    def _init(self, *args, **kwargs):
+      Functor.__init__(self, *args, **kwargs)
+
+    setattr(cls, '__init__', _init)
+
+    # Update __call__ signature.
+    call_signature = pg_typing.Signature.from_schema(
+        cls.schema,
+        name='__call__',
+        module_name=cls.__module__,
+        qualname=cls.__qualname__,
+        is_method=False,
+    )
+    setattr(cls, 'signature', call_signature)
+
   def __new__(cls, *args, **kwargs):
     instance = object.__new__(cls)
     if flags.should_call_functors_during_init():
       instance.__init__(*args, **kwargs)
       return instance()
     return instance
```

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/functor_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/functor_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/list.py` & `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/list.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/list_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/list_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/object.py` & `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/object.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
     # Update `init_arg_list`` based on the updated schema.
     init_arg_list = schema.metadata.get('init_arg_list', None)
     if init_arg_list is None:
       init_arg_list = schema_utils.auto_init_arg_list(cls)
       cls.schema.metadata['init_arg_list'] = init_arg_list
     schema_utils.validate_init_arg_list(init_arg_list, cls.schema)
-    cls._on_schema_update()  # pylint: disable=no-value-for-parameter
+    cls._on_schema_update()  # pytype: disable=attribute-error
 
   def register_for_deserialization(
       cls,
       serialization_key: Optional[str] = None,
       additional_keys: Optional[List[str]] = None,
   ) -> None:
     """Register current symbolic class for deserialization."""
@@ -96,32 +96,22 @@
 
     # Register class with 'type' property.
     for key in serialization_keys:
       object_utils.JSONConvertible.register(
           key, cls, flags.is_repeated_class_registration_allowed()
       )
 
-  def _on_schema_update(cls):
-    """Triggers when the schema for the class has been updated."""
-    # Update the default value for each field after schema is updated. This is
-    # because that users may change a field's default value via class attribute.
-    cls._update_default_values_from_class_attributes()  # pylint: disable=no-value-for-parameter
-
-    # Update the signature of __init__.
-    cls._update_init_signature_based_on_schema()  # pylint: disable=no-value-for-parameter
-
-    # Expose symbolic attributes as object attributes when being asked.
-    if cls.allow_symbolic_attribute:  # pytype: disable=attribute-error
-      cls._generate_sym_attributes()  # pylint: disable=no-value-for-parameter
-
   def _infer_fields_from_annotations(cls) -> List[pg_typing.Field]:
     """Infers symbolic fields from class annotations."""
     if not cls.infer_symbolic_fields_from_annotations:  # pytype: disable=attribute-error
       return []
 
+    # Trigger event so users could modify annotations.
+    cls._begin_annotation_inference()  # pytype: disable=attribute-error
+
     # NOTE(daiyip): refer to https://docs.python.org/3/howto/annotations.html.
     if hasattr(inspect, 'get_annotations'):
       annotations = inspect.get_annotations(cls)
     else:
       annotations = cls.__dict__.get('__annotations__', {})
 
     fields = []
@@ -141,80 +131,31 @@
 
       field = pg_typing.Field.from_annotation(key, attr_annotation)
       if isinstance(key, pg_typing.ConstStrKey):
         attr_value = getattr(cls, attr_name, pg_typing.MISSING_VALUE)
         if attr_value != pg_typing.MISSING_VALUE:
           field.value.set_default(attr_value)
       fields.append(field)
-    return fields
-
-  def _update_init_signature_based_on_schema(cls):
-    """Updates the signature of `__init__` if needed."""
-    if cls.__init__ is not Object.__init__ and not hasattr(
-        cls.__init__, '__sym_generated_init__'
-    ):
-      # We only generate `__init__` from pg.Object subclass which does not
-      # override the `__init__` method.
-      # Functor and ClassWrapper override their `__init__` methods, therefore
-      # they need to synchronize the __init__ signature by themselves.
-      return
-    signature = pg_typing.Signature.from_schema(
-        cls.schema, cls.__module__, '__init__', f'{cls.__name__}.__init__'
-    )
-    pseudo_init = signature.make_function(['pass'])
-
-    # Create a new `__init__` that passes through all the arguments to
-    # in `pg.Object.__init__`. This is needed for each class to use different
-    # signature.
-    @functools.wraps(pseudo_init)
-    def _init(self, *args, **kwargs):
-      # We pass through the arguments to `Object.__init__` instead of
-      # `super()` since the parent class uses a generated `__init__` will
-      # be delegated to `Object.__init__` eventually. Therefore, directly
-      # calling `Object.__init__` is equivalent to calling `super().__init__`.
-      Object.__init__(self, *args, **kwargs)
 
-    setattr(_init, '__sym_generated_init__', True)
-    setattr(cls, '__init__', _init)
+    # Trigger event so subclass could modify the fields.
+    fields = cls._end_annotation_inference(fields)  # pytype: disable=attribute-error
+    return fields
 
   def _update_default_values_from_class_attributes(cls):
     for field in cls.schema.fields.values():
       if isinstance(field.key, pg_typing.ConstStrKey):
         attr_name = field.key.text
         attr_value = getattr(cls, attr_name, pg_typing.MISSING_VALUE)
         if (
             attr_value != pg_typing.MISSING_VALUE
             and not isinstance(attr_value, property)
             and not inspect.isfunction(attr_value)
         ):
           field.value.set_default(attr_value)
 
-  def _generate_sym_attributes(cls):
-    """Generates symbolic attributes based on schema if they are enabled."""
-
-    def _create_sym_attribute(attr_name, field):
-      return property(
-          object_utils.make_function(
-              attr_name,
-              ['self'],
-              [f"return self._sym_attributes['{attr_name}']"],
-              return_type=field.value.annotation,
-          )
-      )
-
-    for key, field in cls.schema.fields.items():
-      if isinstance(key, pg_typing.ConstStrKey):
-        attr_name = str(key)
-        attr_value = getattr(cls, attr_name, pg_typing.MISSING_VALUE)
-        if attr_value == pg_typing.MISSING_VALUE or (
-            not inspect.isfunction(attr_value)
-            and not isinstance(attr_value, property)
-        ):
-          setattr(cls, attr_name, _create_sym_attribute(attr_name, field))
-
 
 # Use ObjectMeta as meta class to inherit schema and type_name property.
 class Object(base.Symbolic, metaclass=ObjectMeta):
   """Base class for symbolic user classes.
 
   PyGlove allow symbolic programming interfaces to be easily added to most
   Python classes in two ways:
@@ -301,53 +242,157 @@
   # Please note that class attributes in UPPER_CASE or starting with '_' will
   # not be considered as symbolic fields even if they have annotations.
   infer_symbolic_fields_from_annotations = True
 
   # Automatically infer schema during subclass creation time.
   auto_schema = True
 
+  #
+  # Customizable class behaviors.
+  #
+
   @classmethod
-  def __init_subclass__(cls):
+  def __init_subclass__(cls, user_cls=None):
+    """Initializes subclass.
+
+    `pg.Object` allows child classes to explicit call
+    `pg.Object.__init_subclass__` in their `__init_subclass__`, to bypass other
+    classes' `__init__subclass__` in multi-inheritance use cases.
+
+    Example:
+
+      class Subclass(pg.Object, UserClass):
+        def __init_subclass__(cls):
+          # This bypasses UserClass.__init_subclass__
+          pg.Object.__init_subclass__(cls)
+
+    Args:
+      user_cls: The source class that calls this class method.
+    """
     super().__init_subclass__()
 
-    if cls.auto_schema:
+    user_cls = user_cls or cls
+    if user_cls.auto_schema:
       # Inherit schema from base classes that have schema
       # in the ordered of inheritance.
       # TODO(daiyip): size of base_schema_list can be reduced
       # by looking at their inheritance chains.
       base_schema_list = []
-      for base_cls in cls.__bases__:
+      for base_cls in user_cls.__bases__:
         base_schema = getattr(base_cls, 'schema', None)
         if isinstance(base_schema, pg_typing.Schema):
           base_schema_list.append(base_schema)
 
-      new_fields = cls._infer_fields_from_annotations()
+      new_fields = user_cls._infer_fields_from_annotations()
       cls_schema = schema_utils.formalize_schema(
           pg_typing.create_schema(
               maybe_field_list=new_fields,
-              name=cls.type_name,
+              name=user_cls.type_name,
               base_schema_list=base_schema_list,
               allow_nonconst_keys=True,
               metadata={},
           )
       )
-
       # NOTE(daiyip): When new fields are added through class attributes.
       # We invalidate `init_arg_list` so PyGlove could recompute it based
       # on its schema during `apply_schema`. Otherwise, we inherit the
       # `init_arg_list` from the base class.
       # TODO(daiyip): detect new fields based on the differences from the base
       # schema.
       if new_fields:
         cls_schema.metadata['init_arg_list'] = None
-      cls.apply_schema(cls_schema)
+      user_cls.apply_schema(cls_schema)
 
     setattr(cls, '__serialization_key__', cls.type_name)
 
   @classmethod
+  def _on_schema_update(cls):
+    """Customizable trait: handling schema change."""
+    # Update the default value for each field after schema is updated. This is
+    # because that users may change a field's default value via class attribute.
+    cls._update_default_values_from_class_attributes()  # pylint: disable=no-value-for-parameter
+
+    # Update all schema-based signatures.
+    cls._update_signatures_based_on_schema()
+
+    # Expose symbolic attributes as object attributes when being asked.
+    if cls.allow_symbolic_attribute:
+      cls._generate_sym_attributes()
+
+  @classmethod
+  def _update_signatures_based_on_schema(cls):
+    """Customizable trait: updates method signatures upon schema change."""
+    if cls.__init__ is not Object.__init__ and not hasattr(
+        cls.__init__, '__sym_generated_init__'
+    ):
+      # We only generate `__init__` from pg.Object subclass which does not
+      # override the `__init__` method.
+      # Functor and ClassWrapper override their `__init__` methods, therefore
+      # they need to synchronize the __init__ signature by themselves.
+      return
+    signature = pg_typing.Signature.from_schema(
+        cls.schema, cls.__module__, '__init__', f'{cls.__name__}.__init__'
+    )
+    pseudo_init = signature.make_function(['pass'])
+
+    # Create a new `__init__` that passes through all the arguments to
+    # in `pg.Object.__init__`. This is needed for each class to use different
+    # signature.
+    @functools.wraps(pseudo_init)
+    def _init(self, *args, **kwargs):
+      # We pass through the arguments to `Object.__init__` instead of
+      # `super()` since the parent class uses a generated `__init__` will
+      # be delegated to `Object.__init__` eventually. Therefore, directly
+      # calling `Object.__init__` is equivalent to calling `super().__init__`.
+      Object.__init__(self, *args, **kwargs)
+
+    setattr(_init, '__sym_generated_init__', True)
+    setattr(cls, '__init__', _init)
+
+  @classmethod
+  def _generate_sym_attributes(cls):
+    """Customizable trait: logics for generating symbolic attributes.."""
+    for key, field in cls.schema.fields.items():
+      if isinstance(key, pg_typing.ConstStrKey):
+        attr_name = str(key)
+        attr_value = getattr(cls, attr_name, pg_typing.MISSING_VALUE)
+        if attr_value == pg_typing.MISSING_VALUE or (
+            not inspect.isfunction(attr_value)
+            and not isinstance(attr_value, property)
+        ):
+          setattr(cls, attr_name, cls._create_sym_attribute(attr_name, field))
+
+  @classmethod
+  def _create_sym_attribute(cls, attr_name, field):
+    """Customizable trait: template of single symbolic attribute."""
+    return property(
+        object_utils.make_function(
+            attr_name,
+            ['self'],
+            [f"return self._sym_attributes['{attr_name}']"],
+            return_type=field.value.annotation,
+        )
+    )
+
+  @classmethod
+  def _begin_annotation_inference(cls) -> None:
+    """Event that is triggered before annotation infererence begins."""
+
+  @classmethod
+  def _end_annotation_inference(
+      cls, fields: List[pg_typing.Field]
+  ) -> List[pg_typing.Field]:
+    """Event that is triggered before annotation infererence begins."""
+    return fields
+
+  #
+  # Class methods.
+  #
+
+  @classmethod
   def partial(cls, *args, **kwargs) -> 'Object':
     """Class method that creates a partial object of current class."""
     return cls(*args, allow_partial=True, **kwargs)
 
   @classmethod
   def from_json(
       cls,
```

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/object_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/object_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/origin.py` & `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/origin.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/origin_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/origin_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/pure_symbolic.py` & `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/pure_symbolic.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/schema_utils.py` & `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/schema_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/schema_utils_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/schema_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/symbolize.py` & `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/symbolize.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/symbolize_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/symbolize_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/tuning/__init__.py` & `pyglove-0.3.1.dev20230521/pyglove/core/tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/tuning/backend.py` & `pyglove-0.3.1.dev20230521/pyglove/core/tuning/backend.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/tuning/backend_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/tuning/backend_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/tuning/early_stopping.py` & `pyglove-0.3.1.dev20230521/pyglove/core/tuning/early_stopping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/tuning/local_backend.py` & `pyglove-0.3.1.dev20230521/pyglove/core/tuning/local_backend.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/tuning/protocols.py` & `pyglove-0.3.1.dev20230521/pyglove/core/tuning/protocols.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/tuning/protocols_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/tuning/protocols_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/tuning/sample.py` & `pyglove-0.3.1.dev20230521/pyglove/core/tuning/sample.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/tuning/sample_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/tuning/sample_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/typing/__init__.py` & `pyglove-0.3.1.dev20230521/pyglove/core/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/typing/annotation_conversion.py` & `pyglove-0.3.1.dev20230521/pyglove/core/typing/annotation_conversion.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/typing/annotation_conversion_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/typing/annotation_conversion_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/typing/callable_ext.py` & `pyglove-0.3.1.dev20230521/pyglove/core/typing/callable_ext.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/typing/callable_ext_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/typing/callable_ext_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/typing/callable_signature.py` & `pyglove-0.3.1.dev20230521/pyglove/core/typing/callable_signature.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/typing/callable_signature_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/typing/callable_signature_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/typing/class_schema.py` & `pyglove-0.3.1.dev20230521/pyglove/core/typing/class_schema.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/typing/class_schema_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/typing/class_schema_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/typing/class_schema_utils.py` & `pyglove-0.3.1.dev20230521/pyglove/core/typing/class_schema_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/typing/class_schema_utils_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/typing/class_schema_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/typing/custom_typing.py` & `pyglove-0.3.1.dev20230521/pyglove/core/typing/custom_typing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/typing/key_specs.py` & `pyglove-0.3.1.dev20230521/pyglove/core/typing/key_specs.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/typing/key_specs_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/typing/key_specs_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/typing/pytype_support.py` & `pyglove-0.3.1.dev20230521/pyglove/core/typing/pytype_support.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/typing/type_conversion.py` & `pyglove-0.3.1.dev20230521/pyglove/core/typing/type_conversion.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/typing/type_conversion_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/typing/type_conversion_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/typing/typed_missing.py` & `pyglove-0.3.1.dev20230521/pyglove/core/typing/typed_missing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/typing/typed_missing_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/typing/typed_missing_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/typing/value_specs.py` & `pyglove-0.3.1.dev20230521/pyglove/core/typing/value_specs.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/core/typing/value_specs_test.py` & `pyglove-0.3.1.dev20230521/pyglove/core/typing/value_specs_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/ext/__init__.py` & `pyglove-0.3.1.dev20230521/pyglove/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/ext/early_stopping/__init__.py` & `pyglove-0.3.1.dev20230521/pyglove/ext/early_stopping/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/ext/early_stopping/base.py` & `pyglove-0.3.1.dev20230521/pyglove/ext/early_stopping/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/ext/early_stopping/base_test.py` & `pyglove-0.3.1.dev20230521/pyglove/ext/early_stopping/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/ext/early_stopping/step_wise.py` & `pyglove-0.3.1.dev20230521/pyglove/ext/early_stopping/step_wise.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/ext/early_stopping/step_wise_test.py` & `pyglove-0.3.1.dev20230521/pyglove/ext/early_stopping/step_wise_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/ext/evolution/__init__.py` & `pyglove-0.3.1.dev20230521/pyglove/ext/evolution/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/ext/evolution/base.py` & `pyglove-0.3.1.dev20230521/pyglove/ext/evolution/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/ext/evolution/base_test.py` & `pyglove-0.3.1.dev20230521/pyglove/ext/evolution/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/ext/evolution/hill_climb.py` & `pyglove-0.3.1.dev20230521/pyglove/ext/evolution/hill_climb.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/ext/evolution/hill_climb_test.py` & `pyglove-0.3.1.dev20230521/pyglove/ext/evolution/hill_climb_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/ext/evolution/mutators.py` & `pyglove-0.3.1.dev20230521/pyglove/ext/evolution/mutators.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/ext/evolution/mutators_test.py` & `pyglove-0.3.1.dev20230521/pyglove/ext/evolution/mutators_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/ext/evolution/neat.py` & `pyglove-0.3.1.dev20230521/pyglove/ext/evolution/neat.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/ext/evolution/neat_test.py` & `pyglove-0.3.1.dev20230521/pyglove/ext/evolution/neat_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/ext/evolution/nsga2.py` & `pyglove-0.3.1.dev20230521/pyglove/ext/evolution/nsga2.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/ext/evolution/nsga2_test.py` & `pyglove-0.3.1.dev20230521/pyglove/ext/evolution/nsga2_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/ext/evolution/recombinators.py` & `pyglove-0.3.1.dev20230521/pyglove/ext/evolution/recombinators.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/ext/evolution/recombinators_test.py` & `pyglove-0.3.1.dev20230521/pyglove/ext/evolution/recombinators_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/ext/evolution/regularized_evolution.py` & `pyglove-0.3.1.dev20230521/pyglove/ext/evolution/regularized_evolution.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/ext/evolution/regularized_evolution_test.py` & `pyglove-0.3.1.dev20230521/pyglove/ext/evolution/regularized_evolution_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/ext/evolution/selectors.py` & `pyglove-0.3.1.dev20230521/pyglove/ext/evolution/selectors.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/ext/evolution/selectors_test.py` & `pyglove-0.3.1.dev20230521/pyglove/ext/evolution/selectors_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/ext/evolution/where.py` & `pyglove-0.3.1.dev20230521/pyglove/ext/evolution/where.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/ext/evolution/where_test.py` & `pyglove-0.3.1.dev20230521/pyglove/ext/evolution/where_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/ext/mutfun/__init__.py` & `pyglove-0.3.1.dev20230521/pyglove/ext/mutfun/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/ext/mutfun/base.py` & `pyglove-0.3.1.dev20230521/pyglove/ext/mutfun/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/ext/mutfun/base_test.py` & `pyglove-0.3.1.dev20230521/pyglove/ext/mutfun/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/ext/mutfun/basic_ops.py` & `pyglove-0.3.1.dev20230521/pyglove/ext/mutfun/basic_ops.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/ext/mutfun/basic_ops_test.py` & `pyglove-0.3.1.dev20230521/pyglove/ext/mutfun/basic_ops_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/ext/scalars/__init__.py` & `pyglove-0.3.1.dev20230521/pyglove/ext/scalars/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/ext/scalars/base.py` & `pyglove-0.3.1.dev20230521/pyglove/ext/scalars/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/ext/scalars/base_test.py` & `pyglove-0.3.1.dev20230521/pyglove/ext/scalars/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/ext/scalars/maths.py` & `pyglove-0.3.1.dev20230521/pyglove/ext/scalars/maths.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/ext/scalars/maths_test.py` & `pyglove-0.3.1.dev20230521/pyglove/ext/scalars/maths_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/ext/scalars/randoms.py` & `pyglove-0.3.1.dev20230521/pyglove/ext/scalars/randoms.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/ext/scalars/randoms_test.py` & `pyglove-0.3.1.dev20230521/pyglove/ext/scalars/randoms_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/ext/scalars/step_wise.py` & `pyglove-0.3.1.dev20230521/pyglove/ext/scalars/step_wise.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove/ext/scalars/step_wise_test.py` & `pyglove-0.3.1.dev20230521/pyglove/ext/scalars/step_wise_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230520/pyglove.egg-info/PKG-INFO` & `pyglove-0.3.1.dev20230521/pyglove.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglove
-Version: 0.3.1.dev20230520
+Version: 0.3.1.dev20230521
 Summary: PyGlove: A library for manipulating Python objects.
 Home-page: https://github.com/google/pyglove
 Author: PyGlove Authors
 Author-email: pyglove-authors@google.com
 License: Apache License 2.0
 Keywords: ai machine learning automl mutable symbolic framework meta-programming
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyglove-0.3.1.dev20230520/pyglove.egg-info/SOURCES.txt` & `pyglove-0.3.1.dev20230521/pyglove.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -77,14 +77,16 @@
 pyglove/core/symbolic/__init__.py
 pyglove/core/symbolic/base.py
 pyglove/core/symbolic/base_test.py
 pyglove/core/symbolic/boilerplate.py
 pyglove/core/symbolic/boilerplate_test.py
 pyglove/core/symbolic/class_wrapper.py
 pyglove/core/symbolic/class_wrapper_test.py
+pyglove/core/symbolic/compounding.py
+pyglove/core/symbolic/compounding_test.py
 pyglove/core/symbolic/dict.py
 pyglove/core/symbolic/dict_test.py
 pyglove/core/symbolic/diff.py
 pyglove/core/symbolic/diff_test.py
 pyglove/core/symbolic/flags.py
 pyglove/core/symbolic/flags_test.py
 pyglove/core/symbolic/functor.py
```

### Comparing `pyglove-0.3.1.dev20230520/setup.py` & `pyglove-0.3.1.dev20230521/setup.py`

 * *Files identical despite different names*

