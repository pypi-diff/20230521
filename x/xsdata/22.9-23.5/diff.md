# Comparing `tmp/xsdata-22.9.tar.gz` & `tmp/xsdata-23.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xsdata-22.9.tar", last modified: Sat Sep 24 09:45:36 2022, max compression
+gzip compressed data, was "xsdata-23.5.tar", last modified: Sun May 21 10:07:07 2023, max compression
```

## Comparing `xsdata-22.9.tar` & `xsdata-23.5.tar`

### file list

```diff
@@ -1,479 +1,498 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.209812 xsdata-22.9/
--rw-r--r--   0 runner    (1001) docker     (121)    28759 2022-09-24 09:45:21.000000 xsdata-22.9/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-09-24 09:45:21.000000 xsdata-22.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      297 2022-09-24 09:45:21.000000 xsdata-22.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5190 2022-09-24 09:45:36.209812 xsdata-22.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3739 2022-09-24 09:45:21.000000 xsdata-22.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.157811 xsdata-22.9/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      719 2022-09-24 09:45:21.000000 xsdata-22.9/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:21.000000 xsdata-22.9/docs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.157811 xsdata-22.9/docs/_ext/
--rw-r--r--   0 runner    (1001) docker     (121)     3086 2022-09-24 09:45:21.000000 xsdata-22.9/docs/_ext/xsdatadocs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.161811 xsdata-22.9/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)      342 2022-09-24 09:45:21.000000 xsdata-22.9/docs/_static/favicon.png
--rw-r--r--   0 runner    (1001) docker     (121)     3540 2022-09-24 09:45:21.000000 xsdata-22.9/docs/_static/logo-dark.svg
--rw-r--r--   0 runner    (1001) docker     (121)     3535 2022-09-24 09:45:21.000000 xsdata-22.9/docs/_static/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.161811 xsdata-22.9/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-09-24 09:45:21.000000 xsdata-22.9/docs/_templates/dataclass.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.161811 xsdata-22.9/docs/api/
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-09-24 09:45:21.000000 xsdata-22.9/docs/api/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1015 2022-09-24 09:45:21.000000 xsdata-22.9/docs/api/codegen.rst
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-09-24 09:45:21.000000 xsdata-22.9/docs/api/generics.rst
--rw-r--r--   0 runner    (1001) docker     (121)      383 2022-09-24 09:45:21.000000 xsdata-22.9/docs/api/parsing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      418 2022-09-24 09:45:21.000000 xsdata-22.9/docs/api/serializing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      300 2022-09-24 09:45:21.000000 xsdata-22.9/docs/api/utils.rst
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-09-24 09:45:21.000000 xsdata-22.9/docs/api/xml-context.rst
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-09-24 09:45:21.000000 xsdata-22.9/docs/api/xml-datatypes.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1659 2022-09-24 09:45:21.000000 xsdata-22.9/docs/api/xml-handlers.rst
--rw-r--r--   0 runner    (1001) docker     (121)      377 2022-09-24 09:45:21.000000 xsdata-22.9/docs/api/xml-nodes.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1698 2022-09-24 09:45:21.000000 xsdata-22.9/docs/api/xml-writers.rst
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-09-24 09:45:21.000000 xsdata-22.9/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-09-24 09:45:21.000000 xsdata-22.9/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3440 2022-09-24 09:45:21.000000 xsdata-22.9/docs/codegen.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2897 2022-09-24 09:45:21.000000 xsdata-22.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1845 2022-09-24 09:45:21.000000 xsdata-22.9/docs/data-types-table.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5841 2022-09-24 09:45:21.000000 xsdata-22.9/docs/data-types.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.161811 xsdata-22.9/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1166 2022-09-24 09:45:21.000000 xsdata-22.9/docs/examples/compound-fields.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1213 2022-09-24 09:45:21.000000 xsdata-22.9/docs/examples/custom-class-factory.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4373 2022-09-24 09:45:21.000000 xsdata-22.9/docs/examples/custom-property-names.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1210 2022-09-24 09:45:21.000000 xsdata-22.9/docs/examples/dataclasses-features.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-09-24 09:45:21.000000 xsdata-22.9/docs/examples/docstrings.rst
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-09-24 09:45:21.000000 xsdata-22.9/docs/examples/dtd-modeling.rst
--rw-r--r--   0 runner    (1001) docker     (121)      792 2022-09-24 09:45:21.000000 xsdata-22.9/docs/examples/json-modeling.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1305 2022-09-24 09:45:21.000000 xsdata-22.9/docs/examples/pycode-serializer.rst
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-09-24 09:45:21.000000 xsdata-22.9/docs/examples/samples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      879 2022-09-24 09:45:21.000000 xsdata-22.9/docs/examples/w3c-suite.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4426 2022-09-24 09:45:21.000000 xsdata-22.9/docs/examples/working-with-wildcards.rst
--rw-r--r--   0 runner    (1001) docker     (121)      871 2022-09-24 09:45:21.000000 xsdata-22.9/docs/examples/xml-modeling.rst
--rw-r--r--   0 runner    (1001) docker     (121)      620 2022-09-24 09:45:21.000000 xsdata-22.9/docs/examples.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.161811 xsdata-22.9/docs/faq/
--rw-r--r--   0 runner    (1001) docker     (121)      297 2022-09-24 09:45:21.000000 xsdata-22.9/docs/faq/error-parsing-dtd.rst
--rw-r--r--   0 runner    (1001) docker     (121)      650 2022-09-24 09:45:21.000000 xsdata-22.9/docs/faq/why-are-elements-out-of-order.rst
--rw-r--r--   0 runner    (1001) docker     (121)      772 2022-09-24 09:45:21.000000 xsdata-22.9/docs/faq/why-i-get-a-typeerror-requires-a-single-type.rst
--rw-r--r--   0 runner    (1001) docker     (121)      750 2022-09-24 09:45:21.000000 xsdata-22.9/docs/faq/why-non-nullable-fields-are-marked-as-optional.rst
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-09-24 09:45:21.000000 xsdata-22.9/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (121)      936 2022-09-24 09:45:21.000000 xsdata-22.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1472 2022-09-24 09:45:21.000000 xsdata-22.9/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10606 2022-09-24 09:45:21.000000 xsdata-22.9/docs/json.rst
--rw-r--r--   0 runner    (1001) docker     (121)      795 2022-09-24 09:45:21.000000 xsdata-22.9/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)    11841 2022-09-24 09:45:21.000000 xsdata-22.9/docs/models.rst
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-09-24 09:45:21.000000 xsdata-22.9/docs/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.161811 xsdata-22.9/docs/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:21.000000 xsdata-22.9/docs/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1250 2022-09-24 09:45:21.000000 xsdata-22.9/docs/scripts/generate_data_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     3897 2022-09-24 09:45:21.000000 xsdata-22.9/docs/wsdl.rst
--rw-r--r--   0 runner    (1001) docker     (121)    12717 2022-09-24 09:45:21.000000 xsdata-22.9/docs/xml.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2030 2022-09-24 09:45:36.209812 xsdata-22.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-24 09:45:21.000000 xsdata-22.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.161811 xsdata-22.9/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-09-24 09:45:21.000000 xsdata-22.9/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.165811 xsdata-22.9/tests/codegen/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:21.000000 xsdata-22.9/tests/codegen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.165811 xsdata-22.9/tests/codegen/handlers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:21.000000 xsdata-22.9/tests/codegen/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4874 2022-09-24 09:45:21.000000 xsdata-22.9/tests/codegen/handlers/test_add_attribute_substitutions.py
--rw-r--r--   0 runner    (1001) docker     (121)     7776 2022-09-24 09:45:21.000000 xsdata-22.9/tests/codegen/handlers/test_create_compound_fields.py
--rw-r--r--   0 runner    (1001) docker     (121)     8496 2022-09-24 09:45:21.000000 xsdata-22.9/tests/codegen/handlers/test_designate_class_packages.py
--rw-r--r--   0 runner    (1001) docker     (121)     2820 2022-09-24 09:45:21.000000 xsdata-22.9/tests/codegen/handlers/test_filter_classes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3872 2022-09-24 09:45:21.000000 xsdata-22.9/tests/codegen/handlers/test_flatten_attribute_groups.py
--rw-r--r--   0 runner    (1001) docker     (121)    20702 2022-09-24 09:45:21.000000 xsdata-22.9/tests/codegen/handlers/test_flatten_class_extensions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2542 2022-09-24 09:45:21.000000 xsdata-22.9/tests/codegen/handlers/test_merge_attributes.py
--rw-r--r--   0 runner    (1001) docker     (121)    18607 2022-09-24 09:45:21.000000 xsdata-22.9/tests/codegen/handlers/test_process_attributes_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     1763 2022-09-24 09:45:21.000000 xsdata-22.9/tests/codegen/handlers/test_process_mixed_content_class.py
--rw-r--r--   0 runner    (1001) docker     (121)     1880 2022-09-24 09:45:21.000000 xsdata-22.9/tests/codegen/handlers/test_rename_duplicate_attributes.py
--rw-r--r--   0 runner    (1001) docker     (121)     8332 2022-09-24 09:45:21.000000 xsdata-22.9/tests/codegen/handlers/test_rename_duplicate_classes.py
--rw-r--r--   0 runner    (1001) docker     (121)    11967 2022-09-24 09:45:21.000000 xsdata-22.9/tests/codegen/handlers/test_sanitize_attributes_default_value.py
--rw-r--r--   0 runner    (1001) docker     (121)     2805 2022-09-24 09:45:21.000000 xsdata-22.9/tests/codegen/handlers/test_sanitize_enumeration_class.py
--rw-r--r--   0 runner    (1001) docker     (121)     4034 2022-09-24 09:45:21.000000 xsdata-22.9/tests/codegen/handlers/test_unnest_inner_classes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2010 2022-09-24 09:45:21.000000 xsdata-22.9/tests/codegen/handlers/test_update_attributes_effective_choice.py
--rw-r--r--   0 runner    (1001) docker     (121)     4781 2022-09-24 09:45:21.000000 xsdata-22.9/tests/codegen/handlers/test_vacuum_inner_classes.py
--rw-r--r--   0 runner    (1001) docker     (121)     4191 2022-09-24 09:45:21.000000 xsdata-22.9/tests/codegen/handlers/test_validate_attributes_overrides.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.165811 xsdata-22.9/tests/codegen/mappers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:21.000000 xsdata-22.9/tests/codegen/mappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    29553 2022-09-24 09:45:21.000000 xsdata-22.9/tests/codegen/mappers/test_definitions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4098 2022-09-24 09:45:21.000000 xsdata-22.9/tests/codegen/mappers/test_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)    13519 2022-09-24 09:45:21.000000 xsdata-22.9/tests/codegen/mappers/test_dtd.py
--rw-r--r--   0 runner    (1001) docker     (121)     9217 2022-09-24 09:45:21.000000 xsdata-22.9/tests/codegen/mappers/test_element.py
--rw-r--r--   0 runner    (1001) docker     (121)    17857 2022-09-24 09:45:21.000000 xsdata-22.9/tests/codegen/mappers/test_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.169811 xsdata-22.9/tests/codegen/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:21.000000 xsdata-22.9/tests/codegen/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4556 2022-09-24 09:45:21.000000 xsdata-22.9/tests/codegen/models/test_attr.py
--rw-r--r--   0 runner    (1001) docker     (121)      680 2022-09-24 09:45:21.000000 xsdata-22.9/tests/codegen/models/test_attr_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     7606 2022-09-24 09:45:21.000000 xsdata-22.9/tests/codegen/models/test_class.py
--rw-r--r--   0 runner    (1001) docker     (121)     3761 2022-09-24 09:45:21.000000 xsdata-22.9/tests/codegen/models/test_restrictions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.169811 xsdata-22.9/tests/codegen/parsers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:21.000000 xsdata-22.9/tests/codegen/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1534 2022-09-24 09:45:21.000000 xsdata-22.9/tests/codegen/parsers/test_definitions.py
--rw-r--r--   0 runner    (1001) docker     (121)     6593 2022-09-24 09:45:21.000000 xsdata-22.9/tests/codegen/parsers/test_dtd.py
--rw-r--r--   0 runner    (1001) docker     (121)    16367 2022-09-24 09:45:21.000000 xsdata-22.9/tests/codegen/parsers/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     2214 2022-09-24 09:45:21.000000 xsdata-22.9/tests/codegen/test_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (121)     5488 2022-09-24 09:45:21.000000 xsdata-22.9/tests/codegen/test_container.py
--rw-r--r--   0 runner    (1001) docker     (121)     8990 2022-09-24 09:45:21.000000 xsdata-22.9/tests/codegen/test_resolver.py
--rw-r--r--   0 runner    (1001) docker     (121)    17148 2022-09-24 09:45:21.000000 xsdata-22.9/tests/codegen/test_transformer.py
--rw-r--r--   0 runner    (1001) docker     (121)    13776 2022-09-24 09:45:21.000000 xsdata-22.9/tests/codegen/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     6791 2022-09-24 09:45:21.000000 xsdata-22.9/tests/codegen/test_validator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2955 2022-09-24 09:45:21.000000 xsdata-22.9/tests/codegen/test_writer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1228 2022-09-24 09:45:21.000000 xsdata-22.9/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.169811 xsdata-22.9/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.169811 xsdata-22.9/tests/fixtures/annotations/
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      592 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/annotations/model.py
--rw-r--r--   0 runner    (1001) docker     (121)      580 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/annotations/model.xsd
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/annotations/sample.xml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/annotations/units.py
--rw-r--r--   0 runner    (1001) docker     (121)      660 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/annotations/units.xsd
--rw-r--r--   0 runner    (1001) docker     (121)      950 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/annotations/xsdata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.169811 xsdata-22.9/tests/fixtures/artists/
--rw-r--r--   0 runner    (1001) docker     (121)      463 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/artists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4517 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/artists/art001.xml
--rw-r--r--   0 runner    (1001) docker     (121)     1214 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/artists/art002.xml
--rw-r--r--   0 runner    (1001) docker     (121)     2629 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/artists/art003.xml
--rw-r--r--   0 runner    (1001) docker     (121)     8041 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/artists/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.173812 xsdata-22.9/tests/fixtures/books/
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/books/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      272 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/books/bk001.xml
--rw-r--r--   0 runner    (1001) docker     (121)      292 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/books/bk002.xml
--rw-r--r--   0 runner    (1001) docker     (121)      194 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/books/books-xinclude.xml
--rw-r--r--   0 runner    (1001) docker     (121)      485 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/books/books.json
--rw-r--r--   0 runner    (1001) docker     (121)     2171 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/books/books.py
--rw-r--r--   0 runner    (1001) docker     (121)      602 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/books/books.xml
--rw-r--r--   0 runner    (1001) docker     (121)      602 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/books/books_auto_ns.xml
--rw-r--r--   0 runner    (1001) docker     (121)      608 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/books/books_default_ns.xml
--rw-r--r--   0 runner    (1001) docker     (121)     3842 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/books/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (121)     2405 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/books/schema.xsd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.173812 xsdata-22.9/tests/fixtures/calculator/
--rw-r--r--   0 runner    (1001) docker     (121)      290 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/calculator/AddRQ.xml
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/calculator/AddRS.xml
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/calculator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13531 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/calculator/services.py
--rw-r--r--   0 runner    (1001) docker     (121)     7880 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/calculator/services.wsdl
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.173812 xsdata-22.9/tests/fixtures/compound/
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/compound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      920 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/compound/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      260 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/compound/sample.json
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/compound/sample.xml
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/compound/sample.xsdata.xml
--rw-r--r--   0 runner    (1001) docker     (121)      606 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/compound/schema.xsd
--rw-r--r--   0 runner    (1001) docker     (121)      680 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/datatypes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.173812 xsdata-22.9/tests/fixtures/docstrings/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/docstrings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.173812 xsdata-22.9/tests/fixtures/docstrings/accessible/
--rw-r--r--   0 runner    (1001) docker     (121)      287 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/docstrings/accessible/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2933 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/docstrings/accessible/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.173812 xsdata-22.9/tests/fixtures/docstrings/blank/
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/docstrings/blank/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1492 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/docstrings/blank/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.173812 xsdata-22.9/tests/fixtures/docstrings/google/
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/docstrings/google/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2867 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/docstrings/google/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.173812 xsdata-22.9/tests/fixtures/docstrings/numpy/
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/docstrings/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2871 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/docstrings/numpy/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.173812 xsdata-22.9/tests/fixtures/docstrings/rst/
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/docstrings/rst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2797 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/docstrings/rst/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     4081 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/docstrings/schema.xsd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.177811 xsdata-22.9/tests/fixtures/dtd/
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/dtd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/dtd/complete_example.dtd
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/dtd/default_namespace.dtd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.177811 xsdata-22.9/tests/fixtures/dtd/models/
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/dtd/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2112 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/dtd/models/complete_example.py
--rw-r--r--   0 runner    (1001) docker     (121)      131 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/dtd/prefix_namespace.dtd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.177811 xsdata-22.9/tests/fixtures/hello/
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/hello/HelloRQ.xml
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/hello/HelloRS.xml
--rw-r--r--   0 runner    (1001) docker     (121)      489 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/hello/HelloRS_SoapFault.xml
--rw-r--r--   0 runner    (1001) docker     (121)      430 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/hello/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4515 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/hello/hello.py
--rw-r--r--   0 runner    (1001) docker     (121)     3084 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/hello/hello.wsdl
--rw-r--r--   0 runner    (1001) docker     (121)      781 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/hello/hello.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     4264 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.177811 xsdata-22.9/tests/fixtures/primer/
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/primer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4565 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/primer/order.py
--rw-r--r--   0 runner    (1001) docker     (121)     3032 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/primer/order.xsd
--rw-r--r--   0 runner    (1001) docker     (121)      840 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/primer/sample.json
--rw-r--r--   0 runner    (1001) docker     (121)      881 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/primer/sample.xml
--rw-r--r--   0 runner    (1001) docker     (121)      889 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/primer/sample.xsdata.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.177811 xsdata-22.9/tests/fixtures/series/
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/series/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.177811 xsdata-22.9/tests/fixtures/series/samples/
--rw-r--r--   0 runner    (1001) docker     (121)     1263 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/series/samples/show1.json
--rw-r--r--   0 runner    (1001) docker     (121)     1278 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/series/samples/show2.json
--rw-r--r--   0 runner    (1001) docker     (121)     5694 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/series/series.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.177811 xsdata-22.9/tests/fixtures/stripe/
--rw-r--r--   0 runner    (1001) docker     (121)      914 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/stripe/.xsdata.xml
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/stripe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.177811 xsdata-22.9/tests/fixtures/stripe/models/
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/stripe/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2572 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/stripe/models/balance.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.177811 xsdata-22.9/tests/fixtures/stripe/samples/
--rw-r--r--   0 runner    (1001) docker     (121)     2628 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/stripe/samples/balance.json
--rw-r--r--   0 runner    (1001) docker     (121)      137 2022-09-24 09:45:21.000000 xsdata-22.9/tests/fixtures/submodels.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.177811 xsdata-22.9/tests/formats/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:21.000000 xsdata-22.9/tests/formats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.181812 xsdata-22.9/tests/formats/dataclass/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:21.000000 xsdata-22.9/tests/formats/dataclass/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.181812 xsdata-22.9/tests/formats/dataclass/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:21.000000 xsdata-22.9/tests/formats/dataclass/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17403 2022-09-24 09:45:21.000000 xsdata-22.9/tests/formats/dataclass/models/test_builders.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.181812 xsdata-22.9/tests/formats/dataclass/parsers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:21.000000 xsdata-22.9/tests/formats/dataclass/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.181812 xsdata-22.9/tests/formats/dataclass/parsers/handlers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:21.000000 xsdata-22.9/tests/formats/dataclass/parsers/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2894 2022-09-24 09:45:21.000000 xsdata-22.9/tests/formats/dataclass/parsers/handlers/test_lxml.py
--rw-r--r--   0 runner    (1001) docker     (121)     3318 2022-09-24 09:45:21.000000 xsdata-22.9/tests/formats/dataclass/parsers/handlers/test_native.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.181812 xsdata-22.9/tests/formats/dataclass/parsers/nodes/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:21.000000 xsdata-22.9/tests/formats/dataclass/parsers/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18992 2022-09-24 09:45:21.000000 xsdata-22.9/tests/formats/dataclass/parsers/nodes/test_element.py
--rw-r--r--   0 runner    (1001) docker     (121)     2412 2022-09-24 09:45:21.000000 xsdata-22.9/tests/formats/dataclass/parsers/nodes/test_primitive.py
--rw-r--r--   0 runner    (1001) docker     (121)      377 2022-09-24 09:45:21.000000 xsdata-22.9/tests/formats/dataclass/parsers/nodes/test_skip.py
--rw-r--r--   0 runner    (1001) docker     (121)     1676 2022-09-24 09:45:21.000000 xsdata-22.9/tests/formats/dataclass/parsers/nodes/test_standard.py
--rw-r--r--   0 runner    (1001) docker     (121)     3986 2022-09-24 09:45:21.000000 xsdata-22.9/tests/formats/dataclass/parsers/nodes/test_union.py
--rw-r--r--   0 runner    (1001) docker     (121)     2229 2022-09-24 09:45:21.000000 xsdata-22.9/tests/formats/dataclass/parsers/nodes/test_wildcard.py
--rw-r--r--   0 runner    (1001) docker     (121)    13423 2022-09-24 09:45:21.000000 xsdata-22.9/tests/formats/dataclass/parsers/test_json.py
--rw-r--r--   0 runner    (1001) docker     (121)     1261 2022-09-24 09:45:21.000000 xsdata-22.9/tests/formats/dataclass/parsers/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (121)     7777 2022-09-24 09:45:21.000000 xsdata-22.9/tests/formats/dataclass/parsers/test_node.py
--rw-r--r--   0 runner    (1001) docker     (121)      981 2022-09-24 09:45:21.000000 xsdata-22.9/tests/formats/dataclass/parsers/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (121)     3877 2022-09-24 09:45:21.000000 xsdata-22.9/tests/formats/dataclass/parsers/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2290 2022-09-24 09:45:21.000000 xsdata-22.9/tests/formats/dataclass/parsers/test_xml.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.185812 xsdata-22.9/tests/formats/dataclass/serializers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:21.000000 xsdata-22.9/tests/formats/dataclass/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2525 2022-09-24 09:45:21.000000 xsdata-22.9/tests/formats/dataclass/serializers/test_code.py
--rw-r--r--   0 runner    (1001) docker     (121)     4688 2022-09-24 09:45:21.000000 xsdata-22.9/tests/formats/dataclass/serializers/test_json.py
--rw-r--r--   0 runner    (1001) docker     (121)     7163 2022-09-24 09:45:21.000000 xsdata-22.9/tests/formats/dataclass/serializers/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (121)    21902 2022-09-24 09:45:21.000000 xsdata-22.9/tests/formats/dataclass/serializers/test_xml.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.185812 xsdata-22.9/tests/formats/dataclass/serializers/writers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:21.000000 xsdata-22.9/tests/formats/dataclass/serializers/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2364 2022-09-24 09:45:21.000000 xsdata-22.9/tests/formats/dataclass/serializers/writers/test_lxml.py
--rw-r--r--   0 runner    (1001) docker     (121)     2255 2022-09-24 09:45:21.000000 xsdata-22.9/tests/formats/dataclass/serializers/writers/test_native.py
--rw-r--r--   0 runner    (1001) docker     (121)     4739 2022-09-24 09:45:21.000000 xsdata-22.9/tests/formats/dataclass/test_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1195 2022-09-24 09:45:21.000000 xsdata-22.9/tests/formats/dataclass/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (121)     4588 2022-09-24 09:45:21.000000 xsdata-22.9/tests/formats/dataclass/test_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     9552 2022-09-24 09:45:21.000000 xsdata-22.9/tests/formats/dataclass/test_elements.py
--rw-r--r--   0 runner    (1001) docker     (121)    32782 2022-09-24 09:45:21.000000 xsdata-22.9/tests/formats/dataclass/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (121)     7450 2022-09-24 09:45:21.000000 xsdata-22.9/tests/formats/dataclass/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2728 2022-09-24 09:45:21.000000 xsdata-22.9/tests/formats/dataclass/test_transport.py
--rw-r--r--   0 runner    (1001) docker     (121)     6808 2022-09-24 09:45:21.000000 xsdata-22.9/tests/formats/dataclass/test_typing.py
--rw-r--r--   0 runner    (1001) docker     (121)    15611 2022-09-24 09:45:21.000000 xsdata-22.9/tests/formats/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1986 2022-09-24 09:45:21.000000 xsdata-22.9/tests/formats/test_mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.185812 xsdata-22.9/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:21.000000 xsdata-22.9/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.185812 xsdata-22.9/tests/integration/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:21.000000 xsdata-22.9/tests/integration/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4184 2022-09-24 09:45:21.000000 xsdata-22.9/tests/integration/benchmarks/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      876 2022-09-24 09:45:21.000000 xsdata-22.9/tests/integration/benchmarks/test_converters.py
--rw-r--r--   0 runner    (1001) docker     (121)     1340 2022-09-24 09:45:21.000000 xsdata-22.9/tests/integration/benchmarks/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1091 2022-09-24 09:45:21.000000 xsdata-22.9/tests/integration/test_annotations.py
--rw-r--r--   0 runner    (1001) docker     (121)     1166 2022-09-24 09:45:21.000000 xsdata-22.9/tests/integration/test_artists.py
--rw-r--r--   0 runner    (1001) docker     (121)      778 2022-09-24 09:45:21.000000 xsdata-22.9/tests/integration/test_books.py
--rw-r--r--   0 runner    (1001) docker     (121)     1991 2022-09-24 09:45:21.000000 xsdata-22.9/tests/integration/test_calculator.py
--rw-r--r--   0 runner    (1001) docker     (121)      655 2022-09-24 09:45:21.000000 xsdata-22.9/tests/integration/test_compound.py
--rw-r--r--   0 runner    (1001) docker     (121)     1880 2022-09-24 09:45:21.000000 xsdata-22.9/tests/integration/test_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (121)      578 2022-09-24 09:45:21.000000 xsdata-22.9/tests/integration/test_dtd.py
--rw-r--r--   0 runner    (1001) docker     (121)     3781 2022-09-24 09:45:21.000000 xsdata-22.9/tests/integration/test_hello_rpc.py
--rw-r--r--   0 runner    (1001) docker     (121)      690 2022-09-24 09:45:21.000000 xsdata-22.9/tests/integration/test_primer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1279 2022-09-24 09:45:21.000000 xsdata-22.9/tests/integration/test_series.py
--rw-r--r--   0 runner    (1001) docker     (121)     1318 2022-09-24 09:45:21.000000 xsdata-22.9/tests/integration/test_stripe.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.185812 xsdata-22.9/tests/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:21.000000 xsdata-22.9/tests/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.185812 xsdata-22.9/tests/models/enums/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:21.000000 xsdata-22.9/tests/models/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2957 2022-09-24 09:45:21.000000 xsdata-22.9/tests/models/enums/test_datatype.py
--rw-r--r--   0 runner    (1001) docker     (121)     9551 2022-09-24 09:45:21.000000 xsdata-22.9/tests/models/test_config.py
--rw-r--r--   0 runner    (1001) docker     (121)    21921 2022-09-24 09:45:21.000000 xsdata-22.9/tests/models/test_datatype.py
--rw-r--r--   0 runner    (1001) docker     (121)     6013 2022-09-24 09:45:21.000000 xsdata-22.9/tests/models/test_mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.189812 xsdata-22.9/tests/models/wsdl/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:21.000000 xsdata-22.9/tests/models/wsdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      700 2022-09-24 09:45:21.000000 xsdata-22.9/tests/models/wsdl/test_binding.py
--rw-r--r--   0 runner    (1001) docker     (121)     3104 2022-09-24 09:45:21.000000 xsdata-22.9/tests/models/wsdl/test_definitions.py
--rw-r--r--   0 runner    (1001) docker     (121)      569 2022-09-24 09:45:21.000000 xsdata-22.9/tests/models/wsdl/test_port_type.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.189812 xsdata-22.9/tests/models/xsd/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:21.000000 xsdata-22.9/tests/models/xsd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-09-24 09:45:21.000000 xsdata-22.9/tests/models/xsd/test_all.py
--rw-r--r--   0 runner    (1001) docker     (121)      757 2022-09-24 09:45:21.000000 xsdata-22.9/tests/models/xsd/test_alternative.py
--rw-r--r--   0 runner    (1001) docker     (121)     1410 2022-09-24 09:45:21.000000 xsdata-22.9/tests/models/xsd/test_annotation_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1381 2022-09-24 09:45:21.000000 xsdata-22.9/tests/models/xsd/test_any.py
--rw-r--r--   0 runner    (1001) docker     (121)     1411 2022-09-24 09:45:21.000000 xsdata-22.9/tests/models/xsd/test_any_attribute.py
--rw-r--r--   0 runner    (1001) docker     (121)     2237 2022-09-24 09:45:21.000000 xsdata-22.9/tests/models/xsd/test_attribute.py
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-09-24 09:45:21.000000 xsdata-22.9/tests/models/xsd/test_attribute_group.py
--rw-r--r--   0 runner    (1001) docker     (121)      621 2022-09-24 09:45:21.000000 xsdata-22.9/tests/models/xsd/test_choice.py
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-09-24 09:45:21.000000 xsdata-22.9/tests/models/xsd/test_complex_content.py
--rw-r--r--   0 runner    (1001) docker     (121)      533 2022-09-24 09:45:21.000000 xsdata-22.9/tests/models/xsd/test_complex_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     3420 2022-09-24 09:45:21.000000 xsdata-22.9/tests/models/xsd/test_element.py
--rw-r--r--   0 runner    (1001) docker     (121)      691 2022-09-24 09:45:21.000000 xsdata-22.9/tests/models/xsd/test_enumeration.py
--rw-r--r--   0 runner    (1001) docker     (121)      320 2022-09-24 09:45:21.000000 xsdata-22.9/tests/models/xsd/test_extension.py
--rw-r--r--   0 runner    (1001) docker     (121)      567 2022-09-24 09:45:21.000000 xsdata-22.9/tests/models/xsd/test_group.py
--rw-r--r--   0 runner    (1001) docker     (121)      607 2022-09-24 09:45:21.000000 xsdata-22.9/tests/models/xsd/test_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     3119 2022-09-24 09:45:21.000000 xsdata-22.9/tests/models/xsd/test_restriction.py
--rw-r--r--   0 runner    (1001) docker     (121)     1442 2022-09-24 09:45:21.000000 xsdata-22.9/tests/models/xsd/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     1864 2022-09-24 09:45:21.000000 xsdata-22.9/tests/models/xsd/test_simple_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     1960 2022-09-24 09:45:21.000000 xsdata-22.9/tests/models/xsd/test_union.py
--rw-r--r--   0 runner    (1001) docker     (121)     6495 2022-09-24 09:45:21.000000 xsdata-22.9/tests/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.189812 xsdata-22.9/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:21.000000 xsdata-22.9/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-09-24 09:45:21.000000 xsdata-22.9/tests/utils/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (121)     4611 2022-09-24 09:45:21.000000 xsdata-22.9/tests/utils/test_dates.py
--rw-r--r--   0 runner    (1001) docker     (121)     5495 2022-09-24 09:45:21.000000 xsdata-22.9/tests/utils/test_downloader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1244 2022-09-24 09:45:21.000000 xsdata-22.9/tests/utils/test_hooks.py
--rw-r--r--   0 runner    (1001) docker     (121)     5503 2022-09-24 09:45:21.000000 xsdata-22.9/tests/utils/test_namespaces.py
--rw-r--r--   0 runner    (1001) docker     (121)      429 2022-09-24 09:45:21.000000 xsdata-22.9/tests/utils/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (121)      508 2022-09-24 09:45:21.000000 xsdata-22.9/tests/utils/test_testing.py
--rw-r--r--   0 runner    (1001) docker     (121)     8010 2022-09-24 09:45:21.000000 xsdata-22.9/tests/utils/test_text.py
--rw-r--r--   0 runner    (1001) docker     (121)      403 2022-09-24 09:45:21.000000 xsdata-22.9/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.193812 xsdata-22.9/xsdata/
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4659 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.193812 xsdata-22.9/xsdata/codegen/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1639 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/codegen/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (121)     5748 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/codegen/container.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.197812 xsdata-22.9/xsdata/codegen/handlers/
--rw-r--r--   0 runner    (1001) docker     (121)     1579 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/codegen/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3069 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/codegen/handlers/add_attribute_substitutions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4476 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/codegen/handlers/create_compound_fields.py
--rw-r--r--   0 runner    (1001) docker     (121)     6186 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/codegen/handlers/designate_class_packages.py
--rw-r--r--   0 runner    (1001) docker     (121)     1818 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/codegen/handlers/filter_classes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1559 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/codegen/handlers/flatten_attribute_groups.py
--rw-r--r--   0 runner    (1001) docker     (121)    11410 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/codegen/handlers/flatten_class_extensions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1672 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/codegen/handlers/merge_attributes.py
--rw-r--r--   0 runner    (1001) docker     (121)     9624 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/codegen/handlers/process_attributes_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     1614 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/codegen/handlers/process_mixed_content_class.py
--rw-r--r--   0 runner    (1001) docker     (121)      996 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/codegen/handlers/rename_duplicate_attributes.py
--rw-r--r--   0 runner    (1001) docker     (121)     4651 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/codegen/handlers/rename_duplicate_classes.py
--rw-r--r--   0 runner    (1001) docker     (121)     6596 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/codegen/handlers/sanitize_attributes_default_value.py
--rw-r--r--   0 runner    (1001) docker     (121)     1785 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/codegen/handlers/sanitize_enumeration_class.py
--rw-r--r--   0 runner    (1001) docker     (121)     1817 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/codegen/handlers/unnest_inner_classes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/codegen/handlers/update_attributes_effective_choice.py
--rw-r--r--   0 runner    (1001) docker     (121)     2786 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/codegen/handlers/vacuum_inner_classes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2410 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/codegen/handlers/validate_attributes_overrides.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.197812 xsdata-22.9/xsdata/codegen/mappers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/codegen/mappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14428 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/codegen/mappers/definitions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1783 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/codegen/mappers/dict.py
--rw-r--r--   0 runner    (1001) docker     (121)     6537 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/codegen/mappers/dtd.py
--rw-r--r--   0 runner    (1001) docker     (121)     6384 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/codegen/mappers/element.py
--rw-r--r--   0 runner    (1001) docker     (121)    10049 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/codegen/mappers/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     2890 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/codegen/mixins.py
--rw-r--r--   0 runner    (1001) docker     (121)    19766 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/codegen/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.197812 xsdata-22.9/xsdata/codegen/parsers/
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/codegen/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      638 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/codegen/parsers/definitions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2869 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/codegen/parsers/dtd.py
--rw-r--r--   0 runner    (1001) docker     (121)     9823 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/codegen/parsers/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     4884 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/codegen/resolver.py
--rw-r--r--   0 runner    (1001) docker     (121)    11006 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/codegen/transformer.py
--rw-r--r--   0 runner    (1001) docker     (121)    10681 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/codegen/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5284 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/codegen/validator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2239 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/codegen/writer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1352 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.197812 xsdata-22.9/xsdata/formats/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1187 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/bindings.py
--rw-r--r--   0 runner    (1001) docker     (121)    16137 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.197812 xsdata-22.9/xsdata/formats/dataclass/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4376 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     4100 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/compat.py
--rw-r--r--   0 runner    (1001) docker     (121)     7653 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/context.py
--rw-r--r--   0 runner    (1001) docker     (121)    25401 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/filters.py
--rw-r--r--   0 runner    (1001) docker     (121)     5237 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.201812 xsdata-22.9/xsdata/formats/dataclass/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16986 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/models/builders.py
--rw-r--r--   0 runner    (1001) docker     (121)    12972 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/models/elements.py
--rw-r--r--   0 runner    (1001) docker     (121)     1364 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/models/generics.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.201812 xsdata-22.9/xsdata/formats/dataclass/parsers/
--rw-r--r--   0 runner    (1001) docker     (121)      314 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7068 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/parsers/bases.py
--rw-r--r--   0 runner    (1001) docker     (121)     1743 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/parsers/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.201812 xsdata-22.9/xsdata/formats/dataclass/parsers/handlers/
--rw-r--r--   0 runner    (1001) docker     (121)      537 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/parsers/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2652 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/parsers/handlers/lxml.py
--rw-r--r--   0 runner    (1001) docker     (121)     4218 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/parsers/handlers/native.py
--rw-r--r--   0 runner    (1001) docker     (121)    11763 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/parsers/json.py
--rw-r--r--   0 runner    (1001) docker     (121)     5624 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/parsers/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.201812 xsdata-22.9/xsdata/formats/dataclass/parsers/nodes/
--rw-r--r--   0 runner    (1001) docker     (121)      552 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/parsers/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14783 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/parsers/nodes/element.py
--rw-r--r--   0 runner    (1001) docker     (121)     1584 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/parsers/nodes/primitive.py
--rw-r--r--   0 runner    (1001) docker     (121)      649 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/parsers/nodes/skip.py
--rw-r--r--   0 runner    (1001) docker     (121)     1771 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/parsers/nodes/standard.py
--rw-r--r--   0 runner    (1001) docker     (121)     4275 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/parsers/nodes/union.py
--rw-r--r--   0 runner    (1001) docker     (121)     2545 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/parsers/nodes/wildcard.py
--rw-r--r--   0 runner    (1001) docker     (121)     2136 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/parsers/tree.py
--rw-r--r--   0 runner    (1001) docker     (121)     3025 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/parsers/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2985 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/parsers/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.201812 xsdata-22.9/xsdata/formats/dataclass/serializers/
--rw-r--r--   0 runner    (1001) docker     (121)      374 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4298 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/serializers/code.py
--rw-r--r--   0 runner    (1001) docker     (121)     1523 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/serializers/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     3341 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/serializers/json.py
--rw-r--r--   0 runner    (1001) docker     (121)     9610 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/serializers/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.201812 xsdata-22.9/xsdata/formats/dataclass/serializers/writers/
--rw-r--r--   0 runner    (1001) docker     (121)      520 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/serializers/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1485 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/serializers/writers/lxml.py
--rw-r--r--   0 runner    (1001) docker     (121)     2138 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/serializers/writers/native.py
--rw-r--r--   0 runner    (1001) docker     (121)    15537 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/serializers/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.205812 xsdata-22.9/xsdata/formats/dataclass/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     2263 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/templates/class.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/templates/docstrings.accessible.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/templates/docstrings.blank.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)      291 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/templates/docstrings.google.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)      329 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/templates/docstrings.numpy.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)      360 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/templates/docstrings.rst.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)      781 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/templates/enum.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/templates/imports.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/templates/module.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)      298 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/templates/package.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/templates/service.jinja2
--rw-r--r--   0 runner    (1001) docker     (121)     1597 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/transports.py
--rw-r--r--   0 runner    (1001) docker     (121)     3617 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/dataclass/typing.py
--rw-r--r--   0 runner    (1001) docker     (121)     2763 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/formats/mixins.py
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.205812 xsdata-22.9/xsdata/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17478 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/models/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    20268 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/models/datatype.py
--rw-r--r--   0 runner    (1001) docker     (121)     1828 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/models/dtd.py
--rw-r--r--   0 runner    (1001) docker     (121)     9802 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/models/enums.py
--rw-r--r--   0 runner    (1001) docker     (121)     7874 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/models/mixins.py
--rw-r--r--   0 runner    (1001) docker     (121)     5749 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/models/wsdl.py
--rw-r--r--   0 runner    (1001) docker     (121)    36954 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/models/xsd.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.205812 xsdata-22.9/xsdata/schemas/
--rw-r--r--   0 runner    (1001) docker     (121)     4067 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/schemas/mathml3-common.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    28457 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/schemas/mathml3-content.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    84129 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/schemas/mathml3-presentation.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     6846 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/schemas/mathml3-strict-content.xsd
--rw-r--r--   0 runner    (1001) docker     (121)      436 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/schemas/mathml3.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     8051 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/schemas/xlink.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     1206 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/schemas/xml.xsd
--rw-r--r--   0 runner    (1001) docker     (121)      347 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/schemas/xsi.xsd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.209812 xsdata-22.9/xsdata/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4205 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/utils/click.py
--rw-r--r--   0 runner    (1001) docker     (121)     2049 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/utils/collections.py
--rw-r--r--   0 runner    (1001) docker     (121)      489 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     6710 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/utils/dates.py
--rw-r--r--   0 runner    (1001) docker     (121)      742 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (121)     4783 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/utils/downloader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1209 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/utils/graphs.py
--rw-r--r--   0 runner    (1001) docker     (121)      453 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/utils/hooks.py
--rw-r--r--   0 runner    (1001) docker     (121)     5045 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/utils/namespaces.py
--rw-r--r--   0 runner    (1001) docker     (121)      813 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/utils/objects.py
--rw-r--r--   0 runner    (1001) docker     (121)      694 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/utils/package.py
--rw-r--r--   0 runner    (1001) docker     (121)    16992 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (121)     4939 2022-09-24 09:45:21.000000 xsdata-22.9/xsdata/utils/text.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-24 09:45:36.193812 xsdata-22.9/xsdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5190 2022-09-24 09:45:36.000000 xsdata-22.9/xsdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    14787 2022-09-24 09:45:36.000000 xsdata-22.9/xsdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-24 09:45:36.000000 xsdata-22.9/xsdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-09-24 09:45:36.000000 xsdata-22.9/xsdata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      331 2022-09-24 09:45:36.000000 xsdata-22.9/xsdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-09-24 09:45:36.000000 xsdata-22.9/xsdata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.395054 xsdata-23.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    32061 2023-05-21 10:06:58.000000 xsdata-23.5/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-21 10:06:58.000000 xsdata-23.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-21 10:06:58.000000 xsdata-23.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-05-21 10:07:07.395054 xsdata-23.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-05-21 10:06:58.000000 xsdata-23.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.311052 xsdata-23.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-21 10:06:58.000000 xsdata-23.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/docs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.311052 xsdata-23.5/docs/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-21 10:06:58.000000 xsdata-23.5/docs/_ext/xsdatadocs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.311052 xsdata-23.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-21 10:06:58.000000 xsdata-23.5/docs/_static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-21 10:06:58.000000 xsdata-23.5/docs/_static/logo-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-21 10:06:58.000000 xsdata-23.5/docs/_static/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.311052 xsdata-23.5/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-21 10:06:58.000000 xsdata-23.5/docs/_templates/dataclass.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.315052 xsdata-23.5/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-21 10:06:58.000000 xsdata-23.5/docs/api/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-21 10:06:58.000000 xsdata-23.5/docs/api/codegen.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-21 10:06:58.000000 xsdata-23.5/docs/api/generics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-21 10:06:58.000000 xsdata-23.5/docs/api/parsing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-21 10:06:58.000000 xsdata-23.5/docs/api/serializing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-21 10:06:58.000000 xsdata-23.5/docs/api/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-21 10:06:58.000000 xsdata-23.5/docs/api/xml-context.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-21 10:06:58.000000 xsdata-23.5/docs/api/xml-datatypes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-21 10:06:58.000000 xsdata-23.5/docs/api/xml-handlers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-21 10:06:58.000000 xsdata-23.5/docs/api/xml-nodes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-21 10:06:58.000000 xsdata-23.5/docs/api/xml-writers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-21 10:06:58.000000 xsdata-23.5/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-21 10:06:58.000000 xsdata-23.5/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-21 10:06:58.000000 xsdata-23.5/docs/codegen.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-21 10:06:58.000000 xsdata-23.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-21 10:06:58.000000 xsdata-23.5/docs/data-types-table.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-05-21 10:06:58.000000 xsdata-23.5/docs/data-types.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.319052 xsdata-23.5/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-21 10:06:58.000000 xsdata-23.5/docs/examples/compound-fields.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-21 10:06:58.000000 xsdata-23.5/docs/examples/custom-class-factory.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-21 10:06:58.000000 xsdata-23.5/docs/examples/custom-property-names.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-21 10:06:58.000000 xsdata-23.5/docs/examples/custom-type-mapping.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-21 10:06:58.000000 xsdata-23.5/docs/examples/dataclasses-features.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-21 10:06:58.000000 xsdata-23.5/docs/examples/docstrings.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-21 10:06:58.000000 xsdata-23.5/docs/examples/dtd-modeling.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-21 10:06:58.000000 xsdata-23.5/docs/examples/json-modeling.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-21 10:06:58.000000 xsdata-23.5/docs/examples/pycode-serializer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-21 10:06:58.000000 xsdata-23.5/docs/examples/samples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-21 10:06:58.000000 xsdata-23.5/docs/examples/w3c-suite.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-05-21 10:06:58.000000 xsdata-23.5/docs/examples/working-with-wildcards.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-21 10:06:58.000000 xsdata-23.5/docs/examples/wrapped-list.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-21 10:06:58.000000 xsdata-23.5/docs/examples/xml-modeling.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-21 10:06:58.000000 xsdata-23.5/docs/examples.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.319052 xsdata-23.5/docs/faq/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-21 10:06:58.000000 xsdata-23.5/docs/faq/error-parsing-dtd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-21 10:06:58.000000 xsdata-23.5/docs/faq/how-can-i-compare-output-results-between-versions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-21 10:06:58.000000 xsdata-23.5/docs/faq/why-are-elements-out-of-order.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-21 10:06:58.000000 xsdata-23.5/docs/faq/why-i-get-a-typeerror-requires-a-single-type.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-21 10:06:58.000000 xsdata-23.5/docs/faq/why-non-nullable-fields-are-marked-as-optional.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-21 10:06:58.000000 xsdata-23.5/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-21 10:06:58.000000 xsdata-23.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-21 10:06:58.000000 xsdata-23.5/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10679 2023-05-21 10:06:58.000000 xsdata-23.5/docs/json.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-21 10:06:58.000000 xsdata-23.5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-05-21 10:06:58.000000 xsdata-23.5/docs/models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-21 10:06:58.000000 xsdata-23.5/docs/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.319052 xsdata-23.5/docs/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/docs/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-21 10:06:58.000000 xsdata-23.5/docs/scripts/generate_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-05-21 10:06:58.000000 xsdata-23.5/docs/wsdl.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12717 2023-05-21 10:06:58.000000 xsdata-23.5/docs/xml.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-21 10:07:07.395054 xsdata-23.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 10:06:58.000000 xsdata-23.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.323052 xsdata-23.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-21 10:06:58.000000 xsdata-23.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.323052 xsdata-23.5/tests/codegen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.331052 xsdata-23.5/tests/codegen/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/test_add_attribute_substitutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/test_calculate_attribute_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/test_create_compound_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8496 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/test_designate_class_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/test_filter_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/test_flatten_attribute_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20197 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/test_flatten_class_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/test_merge_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18994 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/test_process_attributes_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/test_process_mixed_content_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/test_rename_duplicate_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8332 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/test_rename_duplicate_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/test_reset_attribute_sequence_numbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/test_reset_attribute_sequences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12128 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/test_sanitize_attributes_default_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/test_sanitize_enumeration_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/test_unnest_inner_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/test_update_attributes_effective_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/test_vacuum_inner_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/handlers/test_validate_attributes_overrides.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.331052 xsdata-23.5/tests/codegen/mappers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/mappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29551 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/mappers/test_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/mappers/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15415 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/mappers/test_dtd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/mappers/test_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17815 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/mappers/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.331052 xsdata-23.5/tests/codegen/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/models/test_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/models/test_attr_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/models/test_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/models/test_restrictions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.335052 xsdata-23.5/tests/codegen/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/parsers/test_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/parsers/test_dtd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16367 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/parsers/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/test_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/test_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19370 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/test_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14142 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/test_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-05-21 10:06:58.000000 xsdata-23.5/tests/codegen/test_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-21 10:06:58.000000 xsdata-23.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.335052 xsdata-23.5/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.335052 xsdata-23.5/tests/fixtures/annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/annotations/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/annotations/model.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/annotations/sample.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/annotations/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/annotations/units.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/annotations/xsdata.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.339053 xsdata-23.5/tests/fixtures/artists/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/artists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/artists/art001.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/artists/art002.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/artists/art003.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/artists/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.339053 xsdata-23.5/tests/fixtures/books/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/books/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/books/bk001.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/books/bk002.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/books/books-xinclude.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/books/books.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/books/books.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/books/books.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/books/books_auto_ns.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/books/books_default_ns.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/books/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/books/schema.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.343053 xsdata-23.5/tests/fixtures/calculator/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/calculator/AddRQ.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/calculator/AddRS.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/calculator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/calculator/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7880 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/calculator/services.wsdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.343053 xsdata-23.5/tests/fixtures/compound/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/compound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/compound/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/compound/sample.json
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/compound/sample.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/compound/sample.xsdata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/compound/schema.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/datatypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.343053 xsdata-23.5/tests/fixtures/docstrings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/docstrings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.343053 xsdata-23.5/tests/fixtures/docstrings/accessible/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/docstrings/accessible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/docstrings/accessible/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.343053 xsdata-23.5/tests/fixtures/docstrings/blank/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/docstrings/blank/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/docstrings/blank/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.347053 xsdata-23.5/tests/fixtures/docstrings/google/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/docstrings/google/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/docstrings/google/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.347053 xsdata-23.5/tests/fixtures/docstrings/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/docstrings/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/docstrings/numpy/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.347053 xsdata-23.5/tests/fixtures/docstrings/rst/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/docstrings/rst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/docstrings/rst/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/docstrings/schema.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.347053 xsdata-23.5/tests/fixtures/dtd/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/dtd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/dtd/complete_example.dtd
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/dtd/default_namespace.dtd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.347053 xsdata-23.5/tests/fixtures/dtd/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/dtd/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/dtd/models/complete_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/dtd/prefix_namespace.dtd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.347053 xsdata-23.5/tests/fixtures/hello/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/hello/HelloRQ.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/hello/HelloRS.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/hello/HelloRS_SoapFault.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/hello/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/hello/hello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/hello/hello.wsdl
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/hello/hello.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.347053 xsdata-23.5/tests/fixtures/primer/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/primer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/primer/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/primer/order.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/primer/sample.json
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/primer/sample.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/primer/sample.xsdata.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.347053 xsdata-23.5/tests/fixtures/series/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/series/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.347053 xsdata-23.5/tests/fixtures/series/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/series/samples/show1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/series/samples/show2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/series/series.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.347053 xsdata-23.5/tests/fixtures/stripe/
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/stripe/.xsdata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/stripe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.347053 xsdata-23.5/tests/fixtures/stripe/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/stripe/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/stripe/models/balance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.347053 xsdata-23.5/tests/fixtures/stripe/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/stripe/samples/balance.json
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-21 10:06:58.000000 xsdata-23.5/tests/fixtures/submodels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.351053 xsdata-23.5/tests/formats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.351053 xsdata-23.5/tests/formats/dataclass/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.351053 xsdata-23.5/tests/formats/dataclass/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18738 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/models/test_builders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.351053 xsdata-23.5/tests/formats/dataclass/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.351053 xsdata-23.5/tests/formats/dataclass/parsers/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/parsers/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/parsers/handlers/test_lxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/parsers/handlers/test_native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.351053 xsdata-23.5/tests/formats/dataclass/parsers/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/parsers/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/parsers/nodes/test_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/parsers/nodes/test_primitive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/parsers/nodes/test_skip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/parsers/nodes/test_standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/parsers/nodes/test_union.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/parsers/nodes/test_wildcard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/parsers/nodes/test_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13688 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/parsers/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/parsers/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/parsers/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/parsers/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/parsers/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/parsers/test_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.355053 xsdata-23.5/tests/formats/dataclass/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/serializers/test_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/serializers/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/serializers/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24101 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/serializers/test_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.355053 xsdata-23.5/tests/formats/dataclass/serializers/writers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/serializers/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/serializers/writers/test_lxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/serializers/writers/test_native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9580 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/test_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33895 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/test_transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/dataclass/test_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15785 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-05-21 10:06:58.000000 xsdata-23.5/tests/formats/test_mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.355053 xsdata-23.5/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.355053 xsdata-23.5/tests/integration/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/integration/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-21 10:06:58.000000 xsdata-23.5/tests/integration/benchmarks/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-21 10:06:58.000000 xsdata-23.5/tests/integration/benchmarks/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-21 10:06:58.000000 xsdata-23.5/tests/integration/benchmarks/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-21 10:06:58.000000 xsdata-23.5/tests/integration/benchmarks/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-21 10:06:58.000000 xsdata-23.5/tests/integration/test_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-21 10:06:58.000000 xsdata-23.5/tests/integration/test_artists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-21 10:06:58.000000 xsdata-23.5/tests/integration/test_books.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-21 10:06:58.000000 xsdata-23.5/tests/integration/test_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-21 10:06:58.000000 xsdata-23.5/tests/integration/test_compound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-21 10:06:58.000000 xsdata-23.5/tests/integration/test_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-21 10:06:58.000000 xsdata-23.5/tests/integration/test_dtd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-05-21 10:06:58.000000 xsdata-23.5/tests/integration/test_hello_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-21 10:06:58.000000 xsdata-23.5/tests/integration/test_primer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-21 10:06:58.000000 xsdata-23.5/tests/integration/test_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-21 10:06:58.000000 xsdata-23.5/tests/integration/test_stripe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.355053 xsdata-23.5/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.355053 xsdata-23.5/tests/models/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/enums/test_datatype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21919 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/test_datatype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/test_type_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.355053 xsdata-23.5/tests/models/typemapping/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/typemapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/typemapping/city.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/typemapping/house.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/typemapping/street.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.359053 xsdata-23.5/tests/models/wsdl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/wsdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/wsdl/test_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/wsdl/test_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/wsdl/test_port_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.359053 xsdata-23.5/tests/models/xsd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/test_alternative.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/test_annotation_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/test_any.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/test_any_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/test_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/test_attribute_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/test_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/test_complex_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/test_complex_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/test_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/test_enumeration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/test_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/test_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/test_restriction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/test_simple_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-21 10:06:58.000000 xsdata-23.5/tests/models/xsd/test_union.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-05-21 10:06:58.000000 xsdata-23.5/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.359053 xsdata-23.5/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-21 10:06:58.000000 xsdata-23.5/tests/utils/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-05-21 10:06:58.000000 xsdata-23.5/tests/utils/test_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-05-21 10:06:58.000000 xsdata-23.5/tests/utils/test_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-21 10:06:58.000000 xsdata-23.5/tests/utils/test_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-05-21 10:06:58.000000 xsdata-23.5/tests/utils/test_namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-21 10:06:58.000000 xsdata-23.5/tests/utils/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-21 10:06:58.000000 xsdata-23.5/tests/utils/test_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-05-21 10:06:58.000000 xsdata-23.5/tests/utils/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-21 10:06:58.000000 xsdata-23.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.363053 xsdata-23.5/xsdata/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.363053 xsdata-23.5/xsdata/codegen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.367053 xsdata-23.5/xsdata/codegen/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/add_attribute_substitutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/calculate_attribute_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/create_compound_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/designate_class_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/filter_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/flatten_attribute_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/flatten_class_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/merge_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9846 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/process_attributes_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/process_mixed_content_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/rename_duplicate_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/rename_duplicate_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/reset_attribute_sequence_numbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/reset_attribute_sequences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/sanitize_attributes_default_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/sanitize_enumeration_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/unnest_inner_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/update_attributes_effective_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/vacuum_inner_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/handlers/validate_attributes_overrides.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.371053 xsdata-23.5/xsdata/codegen/mappers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/mappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/mappers/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/mappers/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/mappers/dtd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6501 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/mappers/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10096 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/mappers/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20155 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.371053 xsdata-23.5/xsdata/codegen/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/parsers/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/parsers/dtd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9826 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/parsers/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11953 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11309 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/codegen/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.371053 xsdata-23.5/xsdata/formats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16134 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.375053 xsdata-23.5/xsdata/formats/dataclass/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8222 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26070 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.375053 xsdata-23.5/xsdata/formats/dataclass/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17777 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/models/builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13235 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/models/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/models/generics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.379053 xsdata-23.5/xsdata/formats/dataclass/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/parsers/bases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/parsers/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.379053 xsdata-23.5/xsdata/formats/dataclass/parsers/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/parsers/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/parsers/handlers/lxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/parsers/handlers/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11820 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/parsers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/parsers/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.383054 xsdata-23.5/xsdata/formats/dataclass/parsers/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/parsers/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14972 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/parsers/nodes/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/parsers/nodes/primitive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/parsers/nodes/skip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/parsers/nodes/standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/parsers/nodes/union.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/parsers/nodes/wildcard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/parsers/nodes/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/parsers/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/parsers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/parsers/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.383054 xsdata-23.5/xsdata/formats/dataclass/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/serializers/code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/serializers/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/serializers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9637 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/serializers/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.383054 xsdata-23.5/xsdata/formats/dataclass/serializers/writers/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/serializers/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/serializers/writers/lxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/serializers/writers/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16180 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/serializers/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.387054 xsdata-23.5/xsdata/formats/dataclass/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/templates/class.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/templates/docstrings.accessible.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/templates/docstrings.blank.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/templates/docstrings.google.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/templates/docstrings.numpy.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/templates/docstrings.rst.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/templates/enum.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/templates/imports.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/templates/module.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/templates/package.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/templates/service.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/transports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/dataclass/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/formats/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.391054 xsdata-23.5/xsdata/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17796 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20264 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/models/datatype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/models/dtd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9802 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/models/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/models/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/models/wsdl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36929 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/models/xsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.391054 xsdata-23.5/xsdata/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/schemas/mathml3-common.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    28457 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/schemas/mathml3-content.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    84129 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/schemas/mathml3-presentation.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/schemas/mathml3-strict-content.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/schemas/mathml3.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     8051 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/schemas/xlink.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/schemas/xml.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/schemas/xsi.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.395054 xsdata-23.5/xsdata/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/utils/click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/utils/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/utils/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/utils/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/utils/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/utils/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/utils/namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/utils/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/utils/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17285 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-05-21 10:06:58.000000 xsdata-23.5/xsdata/utils/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 10:07:07.363053 xsdata-23.5/xsdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-05-21 10:07:07.000000 xsdata-23.5/xsdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15612 2023-05-21 10:07:07.000000 xsdata-23.5/xsdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 10:07:07.000000 xsdata-23.5/xsdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-21 10:07:07.000000 xsdata-23.5/xsdata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-21 10:07:07.000000 xsdata-23.5/xsdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-21 10:07:07.000000 xsdata-23.5/xsdata.egg-info/top_level.txt
```

### Comparing `xsdata-22.9/CHANGES.rst` & `xsdata-23.5/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,56 @@
-22.9 (2022-08-24)
+23.5 (2023-05-21)
+------------------
+- Fixed XML meta var index conflicts.
+- Fixed mixed content handling for DTD elements. (`#749 <https://github.com/tefra/xsdata/pull/749>`_, `#762 <https://github.com/tefra/xsdata/pull/762>`_)
+- Fixed an issue with required attributes turning into optional ones.
+- Fixed calculation of min/max occurs when parsing XML/JSON documents. (`#756 <https://github.com/tefra/xsdata/pull/756>`_)
+- Fixed calculation of min/max occurs when parsing DTD choice content types. (`#760 <https://github.com/tefra/xsdata/pull/760>`_)
+- Fixed an issue when parsing tail content for compound wildcard elements.
+- Fixed an issue with the code analyzer not fully processing some classes.
+- Fixed an issue with the code analyzer taking forever to process very large enumerations. (`#776 <https://github.com/tefra/xsdata/issue/776>`_)
+- Fixed an issue in the JSON parser with optional choice elements.
+- Updated the transformer to silently ignore malformed JSON files. (`#750 <https://github.com/tefra/xsdata/pull/750>`_)
+- Updated the override attribute handler to fix naming conflicts.
+- Updated the override attribute handler to allow wildcard overrides.
+- Updated conditions on extensions flattening (over-flattening). (`#754 <https://github.com/tefra/xsdata/pull/754>`_)
+- Updated Group, AttributeGroup handling, skipping a few cases.
+- Updated how min/max occurs are calculated with nested containers.
+- Updated handling of element substitutions to treat them as choices. (`#786 <https://github.com/tefra/xsdata/pull/786>`_)
+- Updated Pycodeserializer to skip default field values.
+- Updated flattening restriction base classes when sequence elements are out of order.
+- Updated docformatter to v1.6.5.
+- Added support to override compound fields.
+- Added support for multiple sequential groups in a class.
+- Added support for non-list compound fields.
+- Added support to mix list and non-list fields with sequence groups.
+- Added an option to include headers in generated files. (`#746 <https://github.com/tefra/xsdata/pull/746>`_)
+- Added an option to cache the initial load and mapping of resources.
+- Added support for regular expressions in config substitutions. (`#755 <https://github.com/tefra/xsdata/pull/755>`_)
+- Added a pretty print indentation option in the serializer config. (`#780 <https://github.com/tefra/xsdata/pull/780>`_)
+- Added an option to set the encoding in the SOAP Client. (`#773 <https://github.com/tefra/xsdata/pull/773>`_)
+- Added a CLI flag to show debug messages.
+- Added a debug message for possible circular references during code generation.
+- Added support to generate prohibited fields when they restrict parent fields. (`#781 <https://github.com/tefra/xsdata/pull/781>`_)
+
+This release is bigger than intended and includes many major changes,
+that's why it took so long.
+
+
+22.12 (2022-12-17)
+------------------
+- Added option to ignore xml pattern restrictions `#727 <https://github.com/tefra/xsdata/pull/727>`_
+- Added globalns support via SerializerConfig `#724 <https://github.com/tefra/xsdata/pull/724>`_
+- Pinned docformatter version to v1.5.0 `#729 <https://github.com/tefra/xsdata/pull/729>`_
+
+22.11 (2022-11-06)
+------------------
+- Added list wrapper for elements and primitive nodes `#710 <https://github.com/tefra/xsdata/pull/710>`_
+
+22.9 (2022-09-24)
 -----------------
 - Fixed code generation inconsistencies in different operating systems.
 - Fixed circular imports error `#706 <https://github.com/tefra/xsdata/pull/706>`_
 - Fixed naming conflicts in imports `#706 <https://github.com/tefra/xsdata/pull/706>`_
 - Fixed issue with wrong occurrences in DTD code generation  `#705 <https://github.com/tefra/xsdata/pull/705>`_
 - Fixed xs:group and xs:attrGroup name conflicts `#702 <https://github.com/tefra/xsdata/pull/702>`_
 - Added mathml3 in standard schemas
```

### Comparing `xsdata-22.9/LICENSE` & `xsdata-23.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/PKG-INFO` & `xsdata-23.5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xsdata
-Version: 22.9
+Version: 23.5
 Summary: Python XML Binding
 Home-page: https://github.com/tefra/xsdata
 Author: Christodoulos Tsoulloftas
 Author-email: "chris@komposta.net",
 License: MIT
 Project-URL: Source, https://github.com/tefra/xsdata
 Project-URL: Documentation, https://xsdata.readthedocs.io/
@@ -131,15 +131,43 @@
   - Handlers and Writers based on lxml and native xml python
   - Support wildcard elements and attributes
   - Support xinclude statements and unknown properties
   - Customize behaviour through config
 
 
 
-Changelog: 22.9 (2022-08-24)
+Changelog: 23.5 (2023-05-21)
 ----------------------------
-- Fixed code generation inconsistencies in different operating systems.
-- Fixed circular imports error `#706 <https://github.com/tefra/xsdata/pull/706>`_
-- Fixed naming conflicts in imports `#706 <https://github.com/tefra/xsdata/pull/706>`_
-- Fixed issue with wrong occurrences in DTD code generation  `#705 <https://github.com/tefra/xsdata/pull/705>`_
-- Fixed xs:group and xs:attrGroup name conflicts `#702 <https://github.com/tefra/xsdata/pull/702>`_
-- Added mathml3 in standard schemas
+- Fixed XML meta var index conflicts.
+- Fixed mixed content handling for DTD elements. (`#749 <https://github.com/tefra/xsdata/pull/749>`_, `#762 <https://github.com/tefra/xsdata/pull/762>`_)
+- Fixed an issue with required attributes turning into optional ones.
+- Fixed calculation of min/max occurs when parsing XML/JSON documents. (`#756 <https://github.com/tefra/xsdata/pull/756>`_)
+- Fixed calculation of min/max occurs when parsing DTD choice content types. (`#760 <https://github.com/tefra/xsdata/pull/760>`_)
+- Fixed an issue when parsing tail content for compound wildcard elements.
+- Fixed an issue with the code analyzer not fully processing some classes.
+- Fixed an issue with the code analyzer taking forever to process very large enumerations. (`#776 <https://github.com/tefra/xsdata/issue/776>`_)
+- Fixed an issue in the JSON parser with optional choice elements.
+- Updated the transformer to silently ignore malformed JSON files. (`#750 <https://github.com/tefra/xsdata/pull/750>`_)
+- Updated the override attribute handler to fix naming conflicts.
+- Updated the override attribute handler to allow wildcard overrides.
+- Updated conditions on extensions flattening (over-flattening). (`#754 <https://github.com/tefra/xsdata/pull/754>`_)
+- Updated Group, AttributeGroup handling, skipping a few cases.
+- Updated how min/max occurs are calculated with nested containers.
+- Updated handling of element substitutions to treat them as choices. (`#786 <https://github.com/tefra/xsdata/pull/786>`_)
+- Updated Pycodeserializer to skip default field values.
+- Updated flattening restriction base classes when sequence elements are out of order.
+- Updated docformatter to v1.6.5.
+- Added support to override compound fields.
+- Added support for multiple sequential groups in a class.
+- Added support for non-list compound fields.
+- Added support to mix list and non-list fields with sequence groups.
+- Added an option to include headers in generated files. (`#746 <https://github.com/tefra/xsdata/pull/746>`_)
+- Added an option to cache the initial load and mapping of resources.
+- Added support for regular expressions in config substitutions. (`#755 <https://github.com/tefra/xsdata/pull/755>`_)
+- Added a pretty print indentation option in the serializer config. (`#780 <https://github.com/tefra/xsdata/pull/780>`_)
+- Added an option to set the encoding in the SOAP Client. (`#773 <https://github.com/tefra/xsdata/pull/773>`_)
+- Added a CLI flag to show debug messages.
+- Added a debug message for possible circular references during code generation.
+- Added support to generate prohibited fields when they restrict parent fields. (`#781 <https://github.com/tefra/xsdata/pull/781>`_)
+
+This release is bigger than intended and includes many major changes,
+that's why it took so long.
```

### Comparing `xsdata-22.9/docs/Makefile` & `xsdata-23.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/docs/_ext/xsdatadocs.py` & `xsdata-23.5/docs/_ext/xsdatadocs.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/docs/_static/logo-dark.svg` & `xsdata-23.5/docs/_static/logo-dark.svg`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/docs/_static/logo.svg` & `xsdata-23.5/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/docs/api/codegen.rst` & `xsdata-23.5/docs/api/codegen.rst`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/docs/api/xml-handlers.rst` & `xsdata-23.5/docs/api/xml-handlers.rst`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/docs/api/xml-writers.rst` & `xsdata-23.5/docs/api/xml-writers.rst`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/docs/codegen.rst` & `xsdata-23.5/docs/codegen.rst`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/docs/conf.py` & `xsdata-23.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/docs/data-types-table.rst` & `xsdata-23.5/docs/data-types-table.rst`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/docs/data-types.rst` & `xsdata-23.5/docs/data-types.rst`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/docs/examples/compound-fields.rst` & `xsdata-23.5/docs/examples/compound-fields.rst`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/docs/examples/custom-class-factory.rst` & `xsdata-23.5/docs/examples/custom-class-factory.rst`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/docs/examples/custom-property-names.rst` & `xsdata-23.5/docs/examples/custom-property-names.rst`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/docs/examples/dataclasses-features.rst` & `xsdata-23.5/docs/examples/dataclasses-features.rst`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/docs/examples/docstrings.rst` & `xsdata-23.5/docs/examples/docstrings.rst`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/docs/examples/json-modeling.rst` & `xsdata-23.5/docs/examples/json-modeling.rst`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/docs/examples/pycode-serializer.rst` & `xsdata-23.5/docs/examples/pycode-serializer.rst`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/docs/examples/w3c-suite.rst` & `xsdata-23.5/docs/examples/w3c-suite.rst`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/docs/examples/working-with-wildcards.rst` & `xsdata-23.5/docs/examples/working-with-wildcards.rst`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/docs/examples/xml-modeling.rst` & `xsdata-23.5/docs/examples/xml-modeling.rst`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/docs/examples.rst` & `xsdata-23.5/docs/examples.rst`

 * *Files 21% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 ==============
 
 .. toctree::
     :maxdepth: 1
 
     examples/custom-property-names
     examples/custom-class-factory
+    examples/wrapped-list
+    examples/custom-type-mapping
 
 
 Test Suites
 ===========
 
 .. toctree::
     :maxdepth: 1
```

### Comparing `xsdata-22.9/docs/faq/why-are-elements-out-of-order.rst` & `xsdata-23.5/docs/faq/why-are-elements-out-of-order.rst`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/docs/faq/why-i-get-a-typeerror-requires-a-single-type.rst` & `xsdata-23.5/docs/faq/why-i-get-a-typeerror-requires-a-single-type.rst`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/docs/faq/why-non-nullable-fields-are-marked-as-optional.rst` & `xsdata-23.5/docs/faq/why-non-nullable-fields-are-marked-as-optional.rst`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/docs/index.rst` & `xsdata-23.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/docs/installation.rst` & `xsdata-23.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/docs/json.rst` & `xsdata-23.5/docs/json.rst`

 * *Files 1% similar despite different names*

```diff
@@ -133,14 +133,15 @@
 
 It's optimal to provide the target model but completely optional. The parser can scan
 all the imported modules to find a matching dataclass.
 
 .. doctest::
 
     >>> from tests.fixtures.books import *  # Import all classes
+    >>> from xsdata.formats.dataclass.parsers.config import ParserConfig
     >>> json_string = """{
     ...   "author": "Hightower, Kim",
     ...   "title": "The First Book",
     ...   "genre": "Fiction",
     ...   "price": 44.95,
     ...   "pub_date": "2000-10-01",
     ...   "review": "An amazing story of nothing.",
```

### Comparing `xsdata-22.9/docs/make.bat` & `xsdata-23.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/docs/models.rst` & `xsdata-23.5/docs/models.rst`

 * *Files 2% similar despite different names*

```diff
@@ -143,18 +143,18 @@
        default: ``Text`` or ``Element``
    * - nillable
      - bool
      - Specifies whether an explicit ``None`` value is allowed, default: False
    * - mixed
      - bool
      - Specifies whether the field supports mixed content. [#M1]_
-   * - sequential
-     - bool
-     - Specifies whether the field value(s) must appear in sequence with other
-       sequential sibling fields. eg ``<a /><b /><a /><b />``
+   * - sequence
+     - int
+     - Specifies the sequence identifier of sibling fields
+       eg ``<a /><b /><a /><b />``
    * - tokens
      - bool
      - Map the field value to a python sequence, [#M2]_
    * - namespace
      - str
      - Specifies the field xml namespace. [#M3]_
    * - format
@@ -300,14 +300,18 @@
      - Format option for types like datetime, or bytes, see :ref:`Data Types`
    * - default
      - Any
      - Default value
    * - default_factory
      - Any
      - Default value factory
+   * - wrapper
+     - str
+     - The element name to wrap a collection of elements or primitives
+
 
 .. warning::
 
     Compound fields preserve elements ordering but instead the direct element name
     association is lost during marshalling. If the choices include multiple elements
     with the same type then it's actually impossible to map correctly values to
     elements.
```

### Comparing `xsdata-22.9/docs/scripts/generate_data_types.py` & `xsdata-23.5/docs/scripts/generate_data_types.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/docs/wsdl.rst` & `xsdata-23.5/docs/wsdl.rst`

 * *Files 3% similar despite different names*

```diff
@@ -65,16 +65,15 @@
 
 The client can be initialized from the an operation class directly
 
 .. code-block::
 
     client = Client.from_service(CalculatorSoapAdd)
     client.config
-    # Config(style='document', location='http://www.dneonline.com/calculator.asmx', transport='http://schemas.xmlsoap.org/soap/http', soap_action='http://tempuri.org/Add', input=<class 'tests.fixtures.calculator.services.CalculatorSoapAddInput'>, output=<class 'tests.fixtures.calculator.services.CalculatorSoapAddOutput'>)
-
+    # Config(style='document', location='http://www.dneonline.com/calculator.asmx', transport='http://schemas.xmlsoap.org/soap/http', soap_action='http://tempuri.org/Add', input=<class 'tests.fixtures.calculator.services.CalculatorSoapAddInput'>, output=<class 'tests.fixtures.calculator.services.CalculatorSoapAddOutput'>, encoding=None)
 
 But you can also override any properties as you see fit
 
 .. code-block::
 
     client = Client.from_service(CalculatorSoapAdd, location="http://testurl.com")
     client.config
@@ -119,7 +118,14 @@
 
 You can also provide a dictionary of custom headers as well, although the headers that
 are needed for the webservice to work can not be overwritten.,
 
 .. code-block::
 
     client.send(params, headers={"User-Agent": "xsdata"})
+
+
+You will need to encode the payload if you intend to send non-ascii characters.
+
+.. code-block::
+
+    client = Client.from_service(encoding="utf-8")
```

### Comparing `xsdata-22.9/docs/xml.rst` & `xsdata-23.5/docs/xml.rst`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/setup.cfg` & `xsdata-23.5/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -42,40 +42,39 @@
 console_scripts = 
 	xsdata=xsdata.__main__:main
 
 [options.extras_require]
 cli = 
 	click>=5.0
 	click-default-group>=1.2
-	docformatter
+	docformatter==1.6.5
 	jinja2>=2.10
 	toposort>=1.5
 docs = 
 	furo
 	sphinx
 	sphinx-autobuild
 	sphinx-autodoc-typehints
 	sphinx-copybutton
 	sphinx-inline-tabs
 lxml = 
 	lxml>=4.4.1
 soap = 
 	requests
 test = 
-	codecov
 	pre-commit
 	pytest
 	pytest-benchmark
 	pytest-cov
 	tox
 
 [flake8]
 exclude = tests/*
 max-line-length = 88
-ignore = W503,ANN101,ANN102,ANN401,E203
+ignore = W503,ANN101,ANN102,ANN401,E203,B028
 
 [doc8]
 max-line-length = 88
 
 [tool:pytest]
 addopts = --color=yes --benchmark-skip
```

### Comparing `xsdata-22.9/tests/codegen/handlers/test_add_attribute_substitutions.py` & `xsdata-23.5/tests/codegen/handlers/test_add_attribute_substitutions.py`

 * *Files 6% similar despite different names*

```diff
@@ -117,7 +117,23 @@
             name=item.name,
             default=None,
             types=[AttrType(qname=build_qname("foo", "bar"))],
             tag=Tag.ELEMENT,
         )
 
         self.assertEqual(expected, actual)
+
+    def test_prepare_substituted(self):
+        attr = AttrFactory.create()
+        attr.restrictions.min_occurs = 1
+        attr.restrictions.path.append(("s", 0, 1, 1))
+
+        self.processor.prepare_substituted(attr)
+
+        self.assertEqual(0, attr.restrictions.min_occurs)
+        self.assertEqual(id(attr), attr.restrictions.choice)
+        self.assertEqual(2, len(attr.restrictions.path))
+        self.assertEqual(("c", id(attr), 1, 1), attr.restrictions.path[-1])
+
+        attr.restrictions.choice = 1
+        self.processor.prepare_substituted(attr)
+        self.assertEqual(("c", id(attr), 1, 1), attr.restrictions.path[-1])
```

### Comparing `xsdata-22.9/tests/codegen/handlers/test_create_compound_fields.py` & `xsdata-23.5/tests/codegen/handlers/test_create_compound_fields.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from unittest import mock
 
 from xsdata.codegen.container import ClassContainer
 from xsdata.codegen.handlers import CreateCompoundFields
-from xsdata.codegen.models import Class
 from xsdata.codegen.models import Restrictions
 from xsdata.models.config import GeneratorConfig
 from xsdata.models.enums import DataType
+from xsdata.models.enums import Tag
 from xsdata.utils.testing import AttrFactory
 from xsdata.utils.testing import AttrTypeFactory
 from xsdata.utils.testing import ClassFactory
 from xsdata.utils.testing import ExtensionFactory
 from xsdata.utils.testing import FactoryTestCase
 
 
@@ -24,15 +24,15 @@
 
     @mock.patch.object(CreateCompoundFields, "group_fields")
     def test_process(self, mock_group_fields):
         target = ClassFactory.elements(8)
         # First group repeating
         target.attrs[0].restrictions.choice = "1"
         target.attrs[1].restrictions.choice = "1"
-        target.attrs[1].restrictions.max_occurs = 2
+        target.attrs[1].restrictions.max_occurs = 1
         # Second group repeating
         target.attrs[2].restrictions.choice = "2"
         target.attrs[3].restrictions.choice = "2"
         target.attrs[3].restrictions.max_occurs = 2
         # Third group optional
         target.attrs[4].restrictions.choice = "3"
         target.attrs[5].restrictions.choice = "3"
@@ -42,51 +42,70 @@
             [
                 mock.call(target, target.attrs[0:2]),
                 mock.call(target, target.attrs[2:4]),
             ]
         )
 
     def test_group_fields(self):
-        target = ClassFactory.create(attrs=AttrFactory.list(2))
-        target.attrs[0].restrictions.choice = "1"
-        target.attrs[1].restrictions.choice = "1"
+        target = ClassFactory.create(attrs=AttrFactory.list(4))
+        target.attrs[0].restrictions.choice = 1
+        target.attrs[1].restrictions.choice = 1
         target.attrs[0].restrictions.min_occurs = 10
         target.attrs[0].restrictions.max_occurs = 15
         target.attrs[1].restrictions.min_occurs = 5
         target.attrs[1].restrictions.max_occurs = 20
+        target.attrs[2].restrictions.min_occurs = 2
+        target.attrs[2].restrictions.max_occurs = 4
+        target.attrs[3].restrictions.min_occurs = 1
+        target.attrs[3].restrictions.max_occurs = 3
+
+        target.attrs[0].restrictions.path = [("g", 0, 1, 1), ("c", 1, 1, 1)]
+        target.attrs[1].restrictions.path = [("g", 0, 1, 1), ("c", 1, 1, 1)]
+        target.attrs[2].restrictions.path = [("g", 0, 1, 1), ("c", 1, 1, 1)]
+        target.attrs[3].restrictions.path = [("g", 0, 1, 1), ("c", 1, 1, 1)]
 
         expected = AttrFactory.create(
-            name="attr_B_Or_attr_C",
+            name="choice",
             tag="Choice",
             index=0,
             types=[AttrTypeFactory.native(DataType.ANY_TYPE)],
             choices=[
                 AttrFactory.create(
                     tag=target.attrs[0].tag,
                     name="attr_B",
                     types=target.attrs[0].types,
                 ),
                 AttrFactory.create(
                     tag=target.attrs[1].tag,
                     name="attr_C",
                     types=target.attrs[1].types,
                 ),
+                AttrFactory.create(
+                    tag=target.attrs[2].tag,
+                    name="attr_D",
+                    types=target.attrs[2].types,
+                ),
+                AttrFactory.create(
+                    tag=target.attrs[3].tag,
+                    name="attr_E",
+                    types=target.attrs[3].types,
+                ),
             ],
         )
-        expected_res = Restrictions(min_occurs=5, max_occurs=20)
+        expected_res = Restrictions(min_occurs=1, max_occurs=20)
 
         self.processor.group_fields(target, list(target.attrs))
         self.assertEqual(1, len(target.attrs))
         self.assertEqual(expected, target.attrs[0])
         self.assertEqual(expected_res, target.attrs[0].restrictions)
 
     def test_group_fields_with_effective_choices_sums_occurs(self):
         target = ClassFactory.create(attrs=AttrFactory.list(2))
-        target.attrs[0].restrictions.choice = "effective_1"
-        target.attrs[1].restrictions.choice = "effective_1"
+        target.attrs[0].restrictions.choice = -1
+        target.attrs[1].restrictions.choice = -1
         target.attrs[0].restrictions.min_occurs = 1
         target.attrs[0].restrictions.max_occurs = 2
         target.attrs[1].restrictions.min_occurs = 3
         target.attrs[1].restrictions.max_occurs = 4
 
         expected_res = Restrictions(min_occurs=4, max_occurs=6)
 
@@ -103,31 +122,58 @@
         actual = self.processor.choose_name(target, ["a", "b", "c", "d"])
         self.assertEqual("choice", actual)
 
         target.attrs.append(AttrFactory.create(name="choice"))
         actual = self.processor.choose_name(target, ["a", "b", "c", "d"])
         self.assertEqual("choice_1", actual)
 
-        base = ClassFactory.create()
-        base.attrs.append(AttrFactory.create(name="Choice!"))
-        target.extensions.append(ExtensionFactory.reference(base.qname))
-        self.container.extend((target, base))
-
-        target.attrs.clear()
         actual = self.processor.choose_name(target, ["a", "b", "c", "d"])
         self.assertEqual("choice_1", actual)
 
         self.processor.config.default_name = "ThisOrThat"
         actual = self.processor.choose_name(target, ["a", "b", "c", "d"])
         self.assertEqual("ThisOrThat", actual)
 
         self.processor.config.force_default_name = True
         actual = self.processor.choose_name(target, ["a", "b", "c"])
         self.assertEqual("ThisOrThat", actual)
 
+    def test_build_reserved_names(self):
+        base = ClassFactory.create(
+            attrs=[
+                AttrFactory.create("standalone"),
+                AttrFactory.create(
+                    name="first",
+                    tag=Tag.CHOICE,
+                    choices=[
+                        AttrFactory.create(name="a"),
+                        AttrFactory.create(name="b"),
+                        AttrFactory.create(name="c"),
+                    ],
+                ),
+                AttrFactory.create(
+                    name="second",
+                    tag=Tag.CHOICE,
+                    choices=[
+                        AttrFactory.create(name="b"),
+                        AttrFactory.create(name="c"),
+                    ],
+                ),
+            ]
+        )
+
+        target = ClassFactory.create()
+        target.extensions.append(ExtensionFactory.reference(qname=base.qname))
+        self.processor.container.extend([base, target])
+
+        actual = self.processor.build_reserved_names(target, names=["b", "c"])
+        expected = {"standalone", "first"}
+
+        self.assertEqual(expected, actual)
+
     def test_build_attr_choice(self):
         attr = AttrFactory.create(
             name="a", namespace="xsdata", default="123", help="help", fixed=True
         )
         attr.local_name = "aaa"
         attr.restrictions = Restrictions(
             min_occurs=1,
@@ -142,60 +188,56 @@
             fraction_digits=2,
             length=5,
             white_space="collapse",
             pattern=r"[A-Z]",
             explicit_timezone="+1",
             nillable=True,
             choice="abc",
-            sequential=True,
+            sequence=1,
         )
         expected_res = attr.restrictions.clone()
         expected_res.min_occurs = None
         expected_res.max_occurs = None
-        expected_res.sequential = None
+        expected_res.sequence = None
 
         actual = self.processor.build_attr_choice(attr)
 
         self.assertEqual(attr.local_name, actual.name)
         self.assertEqual(attr.namespace, actual.namespace)
-        self.assertEqual(attr.default, actual.default)
+        self.assertIsNone(actual.default)
         self.assertEqual(attr.tag, actual.tag)
         self.assertEqual(attr.types, actual.types)
         self.assertEqual(expected_res, actual.restrictions)
         self.assertEqual(attr.help, actual.help)
         self.assertFalse(actual.fixed)
 
-    def test_reset_sequential(self):
-        def len_sequential(target: Class):
-            return len([attr for attr in target.attrs if attr.restrictions.sequential])
-
-        restrictions = Restrictions(max_occurs=2, sequential=True)
-        target = ClassFactory.create(
-            attrs=[
-                AttrFactory.create(restrictions=restrictions.clone()),
-                AttrFactory.create(restrictions=restrictions.clone()),
-            ]
-        )
-
-        attrs_clone = [attr.clone() for attr in target.attrs]
+    def test_sum_counters(self):
+        counters = {
+            ("g", 184, 1, 1): {
+                "min": [],
+                "max": [],
+                ("s", 183, 1, 1): {
+                    "min": [],
+                    "max": [],
+                    ("g", 185, 1, 1): {
+                        "min": [],
+                        "max": [],
+                        ("s", 188, 1, 1): {
+                            "min": [],
+                            "max": [],
+                            ("c", 192, 1, 1): {
+                                "min": [0],
+                                "max": [1],
+                                ("s", 193, 1, 1): {
+                                    "min": [0, 0],
+                                    "max": [1, 1],
+                                    ("c", 200, 1, 1): {"min": [0, 0], "max": [1, 1]},
+                                },
+                            },
+                        },
+                    },
+                },
+            }
+        }
 
-        self.processor.config.enabled = False
-        self.processor.reset_sequential(target, 0)
-        self.assertEqual(2, len_sequential(target))
-
-        target.attrs[0].restrictions.sequential = False
-        self.processor.reset_sequential(target, 0)
-        self.assertEqual(1, len_sequential(target))
-
-        self.processor.reset_sequential(target, 1)
-        self.assertEqual(0, len_sequential(target))
-
-        target.attrs = attrs_clone
-        target.attrs[1].restrictions.sequential = False
-        self.processor.reset_sequential(target, 0)
-        self.assertEqual(0, len_sequential(target))
-
-        target.attrs[0].restrictions.sequential = True
-        target.attrs[0].restrictions.max_occurs = 0
-        target.attrs[1].restrictions.sequential = True
-        self.processor.reset_sequential(target, 0)
-        self.assertEqual(1, len_sequential(target))
+        result = self.processor.sum_counters(counters)
+        self.assertEqual((0, 3), (sum(result[0]), sum(result[1])))
```

### Comparing `xsdata-22.9/tests/codegen/handlers/test_designate_class_packages.py` & `xsdata-23.5/tests/codegen/handlers/test_designate_class_packages.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/codegen/handlers/test_filter_classes.py` & `xsdata-23.5/tests/codegen/handlers/test_filter_classes.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/codegen/handlers/test_flatten_attribute_groups.py` & `xsdata-23.5/tests/codegen/handlers/test_flatten_attribute_groups.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/codegen/handlers/test_flatten_class_extensions.py` & `xsdata-23.5/tests/codegen/handlers/test_flatten_class_extensions.py`

 * *Files 3% similar despite different names*

```diff
@@ -289,15 +289,15 @@
         source = ClassFactory.elements(5)
 
         self.processor.process_complex_extension(source, target, extension)
 
         self.assertEqual(0, len(target.extensions))
         self.assertEqual(1, len(target.attrs))
 
-        mock_should_remove_extension.assert_called_once_with(source, target)
+        mock_should_remove_extension.assert_called_once_with(source, target, extension)
         self.assertEqual(0, mock_copy_attributes.call_count)
         self.assertEqual(0, extension.type.reference)
 
     @mock.patch.object(ClassUtils, "copy_attributes")
     @mock.patch.object(FlattenClassExtensions, "should_flatten_extension")
     def test_process_complex_extension_copies_attributes(
         self, mock_compare_attributes, mock_should_flatten_extension
@@ -339,31 +339,54 @@
         simple = ClassFactory.create(qname="a", tag=Tag.SIMPLE_TYPE)
         self.processor.container.add(simple)
         self.assertEqual(simple, self.processor.find_dependency(attr_type))
 
     def test_should_remove_extension(self):
         source = ClassFactory.create()
         target = ClassFactory.create()
+        extension = ExtensionFactory.create(tag=Tag.EXTENSION)
+        callback = self.processor.should_remove_extension
 
         # source is target
-        self.assertTrue(self.processor.should_remove_extension(source, source))
-        self.assertFalse(self.processor.should_remove_extension(source, target))
+        self.assertTrue(callback(source, source, extension))
+        self.assertFalse(callback(source, target, extension))
 
         # Source is parent class
         source.inner.append(target)
-        self.assertTrue(self.processor.should_remove_extension(target, target))
+        self.assertTrue(callback(target, target, extension))
 
         # MRO Violation
         source.inner.clear()
         target.extensions.append(ExtensionFactory.reference("foo"))
         target.extensions.append(ExtensionFactory.reference("bar"))
-        self.assertFalse(self.processor.should_remove_extension(source, target))
+        self.assertFalse(callback(source, target, extension))
 
         source.extensions.append(ExtensionFactory.reference("bar"))
-        self.assertTrue(self.processor.should_remove_extension(source, target))
+        self.assertTrue(callback(source, target, extension))
+
+        # Sequential violation
+        extension.tag = Tag.RESTRICTION
+        source = ClassFactory.elements(4)
+        target = source.clone()
+        self.assertFalse(callback(source, target, extension))
+
+        for attr in target.attrs:
+            attr.restrictions.sequence = 1
+
+        target.attrs[3].restrictions.max_occurs = 0
+
+        self.assertFalse(callback(source, target, extension))
+
+        target.attrs = [
+            target.attrs[1],
+            target.attrs[0],
+            target.attrs[2],
+            target.attrs[3],
+        ]
+        self.assertTrue(callback(source, target, extension))
 
     def test_should_flatten_extension(self):
         source = ClassFactory.create()
         target = ClassFactory.create()
 
         self.assertFalse(self.processor.should_flatten_extension(source, target))
 
@@ -384,43 +407,14 @@
         self.assertTrue(self.processor.should_flatten_extension(source, target))
 
         # Source is a simple type
         source = ClassFactory.create(attrs=[AttrFactory.create(tag=Tag.SIMPLE_TYPE)])
         target = ClassFactory.elements(1)
         self.assertTrue(self.processor.should_flatten_extension(source, target))
 
-        # Sequential violation
-        source = ClassFactory.elements(3)
-        target = source.clone()
-        self.assertFalse(self.processor.should_flatten_extension(source, target))
-
-        for attr in target.attrs:
-            attr.restrictions.sequential = True
-
-        self.assertFalse(self.processor.should_flatten_extension(source, target))
-
-        target.attrs = [target.attrs[1], target.attrs[0], target.attrs[2]]
-        self.assertTrue(self.processor.should_flatten_extension(source, target))
-
-        # Types violation
-        target = source.clone()
-        target.attrs[1].types = [
-            AttrTypeFactory.native(DataType.INT),
-            AttrTypeFactory.native(DataType.FLOAT),
-        ]
-
-        source.attrs[1].types = [
-            AttrTypeFactory.native(DataType.INT),
-            AttrTypeFactory.native(DataType.FLOAT),
-            AttrTypeFactory.native(DataType.DECIMAL),
-        ]
-        self.assertFalse(self.processor.should_flatten_extension(source, target))
-        target.attrs[1].types.append(AttrTypeFactory.native(DataType.QNAME))
-        self.assertTrue(self.processor.should_flatten_extension(source, target))
-
     def test_replace_attributes_type(self):
         extension = ExtensionFactory.create()
         target = ClassFactory.elements(2)
         target.extensions.append(extension)
 
         FlattenClassExtensions.replace_attributes_type(target, extension)
```

### Comparing `xsdata-22.9/tests/codegen/handlers/test_merge_attributes.py` & `xsdata-23.5/tests/codegen/handlers/test_merge_attributes.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,27 @@
 
 
 class MergeAttributesTests(FactoryTestCase):
     def setUp(self):
         super().setUp()
         self.processor = MergeAttributes
 
-    def test_process(self):
+    def test_process_with_enumeration(self):
+        target = ClassFactory.create()
+        target.attrs = [
+            AttrFactory.enumeration(default=1),
+            AttrFactory.enumeration(default=1),
+            AttrFactory.enumeration(default=2),
+            AttrFactory.enumeration(default=2),
+        ]
+
+        self.processor.process(target)
+        self.assertEqual([1, 2], [x.default for x in target.attrs])
+
+    def test_process_with_non_enumeration(self):
         one = AttrFactory.attribute(fixed=True)
         one_clone = one.clone()
         restrictions = Restrictions(min_occurs=10, max_occurs=15)
         two = AttrFactory.element(restrictions=restrictions, fixed=True)
         two_clone = two.clone()
         two_clone.restrictions.min_occurs = 5
         two_clone.restrictions.max_occurs = 5
@@ -26,14 +38,15 @@
         three = AttrFactory.element()
         four = AttrFactory.enumeration()
         four_clone = four.clone()
         five = AttrFactory.element()
         five.types = [AttrTypeFactory.native(DataType.INT)]
         five_clone = five.clone()
         five_clone_two = five.clone()
+        five_clone_two.restrictions.sequence = 1
         five_clone_two.types.append(AttrTypeFactory.native(DataType.FLOAT))
 
         target = ClassFactory.create(
             attrs=[
                 one,
                 one_clone,
                 two,
@@ -59,10 +72,11 @@
         self.assertFalse(two.fixed)
         self.assertEqual(4, two.restrictions.min_occurs)
         self.assertEqual(24, two.restrictions.max_occurs)
         self.assertIsNone(three.restrictions.min_occurs)
         self.assertIsNone(three.restrictions.max_occurs)
         self.assertIsNone(four.restrictions.min_occurs)
         self.assertIsNone(four.restrictions.max_occurs)
+        self.assertEqual(1, five.restrictions.sequence)
         self.assertEqual(0, five.restrictions.min_occurs)
         self.assertEqual(3, five.restrictions.max_occurs)
         self.assertEqual(["int", "float"], [x.name for x in five.types])
```

### Comparing `xsdata-22.9/tests/codegen/handlers/test_process_attributes_types.py` & `xsdata-23.5/tests/codegen/handlers/test_process_attributes_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,23 @@
 
         mock_process_type.assert_has_calls(
             [mock.call(target, attr, tp) for tp in types]
         )
 
         self.assertEqual(types[:-1], attr.types)
 
+    def test_process_types_with_ignore_patterns(self):
+        target = ClassFactory.create()
+        attr = AttrFactory.native(DataType.DECIMAL)
+        attr.restrictions.pattern = r"\d{2}.\d{2}"
+
+        self.processor.container.config.output.ignore_patterns = True
+        self.processor.process_types(target, attr)
+        self.assertEqual(DataType.DECIMAL, attr.types[0].datatype)
+
     def test_cascade_properties(self):
         target = ClassFactory.create(default="2", fixed=True, nillable=True)
         attr = AttrFactory.native(DataType.STRING, tag=Tag.EXTENSION)
         self.processor.cascade_properties(target, attr)
 
         self.assertEqual(target.default, attr.default)
         self.assertTrue(attr.fixed)
```

### Comparing `xsdata-22.9/tests/codegen/handlers/test_process_mixed_content_class.py` & `xsdata-23.5/tests/codegen/handlers/test_process_mixed_content_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 class ProcessMixedContentClassTests(FactoryTestCase):
     def setUp(self):
         super().setUp()
         self.processor = ProcessMixedContentClass()
 
     def test_process(self):
-        res = Restrictions(min_occurs=1, max_occurs=1, sequential=True)
+        res = Restrictions(min_occurs=1, max_occurs=1, sequence=1)
         attrs = [
             AttrFactory.attribute(),  # keep
             AttrFactory.reference("foo", restrictions=res.clone()),  # choice
             AttrFactory.native(DataType.INT, restrictions=res.clone()),  # choice
             AttrFactory.any(),  # drop
         ]
         item = ClassFactory.create(attrs=attrs)
@@ -39,12 +39,12 @@
         expected.restrictions.min_occurs = 0
         expected.restrictions.max_occurs = sys.maxsize
         choices = []
         for attr in attrs[1:-1]:
             choice = attr.clone()
             choice.restrictions.min_occurs = None
             choice.restrictions.max_occurs = None
-            choice.restrictions.sequential = None
+            choice.restrictions.sequence = None
             choices.append(choice)
 
         self.assertEqual(expected, item.attrs[1])
         self.assertEqual(choices, item.attrs[1].choices)
```

### Comparing `xsdata-22.9/tests/codegen/handlers/test_rename_duplicate_attributes.py` & `xsdata-23.5/tests/codegen/handlers/test_rename_duplicate_attributes.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/codegen/handlers/test_rename_duplicate_classes.py` & `xsdata-23.5/tests/codegen/handlers/test_rename_duplicate_classes.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/codegen/handlers/test_sanitize_attributes_default_value.py` & `xsdata-23.5/tests/codegen/handlers/test_sanitize_attributes_default_value.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from xsdata.codegen.container import ClassContainer
 from xsdata.codegen.handlers import SanitizeAttributesDefaultValue
 from xsdata.codegen.models import Restrictions
 from xsdata.models.config import GeneratorConfig
 from xsdata.models.enums import DataType
 from xsdata.models.enums import Namespace
+from xsdata.models.enums import Tag
 from xsdata.utils.testing import AttrFactory
 from xsdata.utils.testing import AttrTypeFactory
 from xsdata.utils.testing import ClassFactory
 from xsdata.utils.testing import FactoryTestCase
 
 
 class SanitizeAttributesDefaultValueTests(FactoryTestCase):
@@ -58,15 +59,14 @@
 
     @mock.patch.object(SanitizeAttributesDefaultValue, "process_types")
     @mock.patch.object(SanitizeAttributesDefaultValue, "should_reset_default")
     @mock.patch.object(SanitizeAttributesDefaultValue, "should_reset_required")
     def test_process_attribute(
         self, mock_should_reset_required, mock_should_reset_default, mock_process_types
     ):
-
         target = ClassFactory.create()
         mock_should_reset_required.side_effect = [
             True,
             False,
             False,
             False,
             False,
@@ -125,24 +125,27 @@
 
         attr = AttrFactory.create(name="type", namespace=Namespace.XSI.uri)
         self.assertFalse(self.processor.should_reset_default(attr))
 
         attr.default = "abc"
         self.assertTrue(self.processor.should_reset_default(attr))
 
-        attr = AttrFactory.create(
-            default="abc", restrictions=Restrictions(min_occurs=0)
+        attr = AttrFactory.element(
+            default="abc", restrictions=Restrictions(min_occurs=1)
         )
         self.assertFalse(self.processor.should_reset_default(attr))
-
-        attr.restrictions.sequential = True
+        attr.restrictions.max_occurs = 2
         self.assertTrue(self.processor.should_reset_default(attr))
 
-        attr.restrictions.choice = "foo"
-        attr.restrictions.sequential = False
+        attr = AttrFactory.attribute(
+            default="abc", restrictions=Restrictions(min_occurs=0)
+        )
+        self.assertFalse(self.processor.should_reset_default(attr))
+
+        attr.tag = Tag.ELEMENT
         self.assertTrue(self.processor.should_reset_default(attr))
 
     @mock.patch(
         "xsdata.codegen.handlers.sanitize_attributes_default_value.logger.warning"
     )
     @mock.patch.object(SanitizeAttributesDefaultValue, "reset_attribute_types")
     @mock.patch.object(SanitizeAttributesDefaultValue, "is_valid_native_value")
```

### Comparing `xsdata-22.9/tests/codegen/handlers/test_sanitize_enumeration_class.py` & `xsdata-23.5/tests/codegen/handlers/test_sanitize_enumeration_class.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/codegen/handlers/test_unnest_inner_classes.py` & `xsdata-23.5/tests/codegen/handlers/test_unnest_inner_classes.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/codegen/handlers/test_vacuum_inner_classes.py` & `xsdata-23.5/tests/codegen/handlers/test_vacuum_inner_classes.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/codegen/handlers/test_validate_attributes_overrides.py` & `xsdata-23.5/tests/codegen/handlers/test_validate_attributes_overrides.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import sys
 from unittest import mock
 
 from xsdata.codegen.container import ClassContainer
 from xsdata.codegen.handlers import ValidateAttributesOverrides
 from xsdata.codegen.models import Status
 from xsdata.models.config import GeneratorConfig
+from xsdata.models.enums import DataType
 from xsdata.models.enums import Tag
 from xsdata.utils.testing import AttrFactory
 from xsdata.utils.testing import ClassFactory
 from xsdata.utils.testing import ExtensionFactory
 from xsdata.utils.testing import FactoryTestCase
 
 
@@ -46,14 +47,33 @@
         mock_validate_override.assert_called_once_with(
             class_a, class_a.attrs[0], class_c.attrs[0]
         )
         mock_resolve_conflict.assert_called_once_with(
             class_a.attrs[1], class_c.attrs[1]
         )
 
+    def test_process_remove_non_overriding_prohibited_attrs(self):
+        target = ClassFactory.elements(1)
+        target.attrs[0].restrictions.max_occurs = 0
+
+        self.processor.process(target)
+        self.assertEqual(0, len(target.attrs))
+
+    def test_overrides(self):
+        a = AttrFactory.create(tag=Tag.SIMPLE_TYPE)
+        b = a.clone()
+
+        self.assertTrue(self.processor.overrides(a, b))
+
+        b.tag = Tag.EXTENSION
+        self.assertTrue(self.processor.overrides(a, b))
+
+        b.namespace = "foo"
+        self.assertFalse(self.processor.overrides(a, b))
+
     def test_validate_override(self):
         attr_a = AttrFactory.create()
         attr_b = attr_a.clone()
         target = ClassFactory.create()
         target.attrs.append(attr_a)
 
         # 100 Match remove override attrs
@@ -87,22 +107,31 @@
 
         # Restrictions are compatible again
         attr_a.restrictions.tokens = attr_b.restrictions.tokens
         attr_a.restrictions.nillable = attr_b.restrictions.nillable
         self.processor.validate_override(target, attr_a, attr_b)
         self.assertEqual(0, len(target.attrs))
 
+        # Source is list, parent is not
         target.attrs.append(attr_a)
         attr_a.restrictions.min_occurs = None
         attr_a.restrictions.max_occurs = 10
         attr_b.restrictions.min_occurs = None
         attr_b.restrictions.max_occurs = None
         self.processor.validate_override(target, attr_a, attr_b)
         self.assertEqual(sys.maxsize, attr_b.restrictions.max_occurs)
 
+        # Parent is any type, source isn't, skip
+        attr_a = AttrFactory.native(DataType.STRING)
+        attr_b = AttrFactory.native(DataType.ANY_SIMPLE_TYPE)
+        target = ClassFactory.create(attrs=[attr_a])
+
+        self.processor.validate_override(target, attr_a.clone(), attr_b)
+        self.assertEqual(attr_a, target.attrs[0])
+
     def test_resolve_conflicts(self):
         a = AttrFactory.create(name="foo", tag=Tag.ATTRIBUTE)
         b = a.clone()
         b.tag = Tag.ELEMENT
         self.processor.resolve_conflict(a, b)
 
         self.assertEqual("foo_Attribute", a.name)
```

### Comparing `xsdata-22.9/tests/codegen/mappers/test_definitions.py` & `xsdata-23.5/tests/codegen/mappers/test_definitions.py`

 * *Files 0% similar despite different names*

```diff
@@ -721,15 +721,14 @@
             namespace="bar",
             ns_map=message.ns_map,
             attrs=attrs,
         )
         self.assertEqual(expected, actual)
 
     def test_get_or_create_inner_class(self):
-
         target = ClassFactory.create(
             location="foo", package=None, ns_map={"foo": "bar"}
         )
 
         actual = DefinitionsMapper.build_inner_class(target, "body")
         expected = ClassFactory.create(
             qname="{xsdata}body",
@@ -771,15 +770,14 @@
             "Add", qname=build_qname("foobar", "bar"), namespace=target_namespace
         )
 
         self.assertIsInstance(actual, Generator)
         self.assertEqual([expected], list(actual))
 
     def test_operation_namespace(self):
-
         self.assertIsNone(DefinitionsMapper.operation_namespace({}))
         self.assertIsNone(DefinitionsMapper.operation_namespace({"transport": "foo"}))
         self.assertEqual(
             "http://schemas.xmlsoap.org/soap/envelope/",
             DefinitionsMapper.operation_namespace(
                 {"transport": "http://schemas.xmlsoap.org/soap/http"}
             ),
```

### Comparing `xsdata-22.9/tests/codegen/mappers/test_dict.py` & `xsdata-23.5/tests/codegen/mappers/test_dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             tag=Tag.ELEMENT,
             types=[
                 AttrTypeFactory.native(DataType.SHORT, tag=Tag.ELEMENT),
                 AttrTypeFactory.native(DataType.BOOLEAN, tag=Tag.ELEMENT),
                 AttrTypeFactory.native(DataType.FLOAT, tag=Tag.ELEMENT),
             ],
         )
-        restrictions = Restrictions(min_occurs=0, max_occurs=sys.maxsize)
+        restrictions = Restrictions(min_occurs=1, max_occurs=sys.maxsize)
         self.assertEqual(expected, target.attrs[0])
         self.assertEqual(restrictions, target.attrs[0].restrictions)
 
     def test_build_class_attribute_from_empty_list(self):
         target = ClassFactory.create()
         data = []
 
@@ -84,15 +84,15 @@
         expected = AttrFactory.create(
             name="a",
             tag=Tag.ELEMENT,
             types=[
                 AttrTypeFactory.native(DataType.ANY_SIMPLE_TYPE, tag=Tag.ELEMENT),
             ],
         )
-        restrictions = Restrictions(min_occurs=0, max_occurs=sys.maxsize)
+        restrictions = Restrictions(min_occurs=1, max_occurs=sys.maxsize)
         self.assertEqual(expected, target.attrs[0])
         self.assertEqual(restrictions, target.attrs[0].restrictions)
 
     def test_build_class_attribute_from_dict(self):
         target = ClassFactory.create()
         data = {"sub1": 1, "sub2": "value"}
         DictMapper.build_class_attribute(target, "a", data)
```

### Comparing `xsdata-22.9/tests/codegen/mappers/test_dtd.py` & `xsdata-23.5/tests/codegen/mappers/test_dtd.py`

 * *Files 4% similar despite different names*

```diff
@@ -147,23 +147,73 @@
         self.assertEqual(1, attr.restrictions.max_occurs)
         self.assertEqual(1, attr.restrictions.min_occurs)
         self.assertFalse(attr.fixed)
         self.assertEqual("abc", attr.default)
 
     def test_build_elements_with_mixed_element_type(self):
         target = ClassFactory.create(tag=Tag.ELEMENT)
-        element = DtdElementFactory.create(type=DtdElementType.MIXED)
+        left = DtdContentFactory.create(
+            type=DtdContentType.PCDATA, occur=DtdContentOccur.ONCE
+        )
+        right = DtdContentFactory.create(
+            name="rad", type=DtdContentType.ELEMENT, occur=DtdContentOccur.ONCE
+        )
+        element = DtdElementFactory.create(
+            type=DtdElementType.MIXED,
+            content=DtdContentFactory.create(
+                type=DtdContentType.OR, left=left, right=right
+            ),
+        )
 
         DtdMapper.build_elements(target, element)
-        self.assertEqual(0, len(target.attrs))
-        self.assertEqual(1, len(target.extensions))
+        expected = [
+            AttrFactory.create(
+                tag=Tag.ELEMENT,
+                name="rad",
+                index=1,
+                types=[AttrTypeFactory.create(qname="rad")],
+            ),
+        ]
 
+        self.assertTrue(target.mixed)
+        self.assertEqual(expected, target.attrs)
+        self.assertEqual(Tag.COMPLEX_TYPE, target.tag)
+
+        element.content.left = right
+        element.content.right = left
+
+        target.attrs.clear()
+        target.mixed = False
+        DtdMapper.build_elements(target, element)
+        self.assertTrue(target.mixed)
+        self.assertEqual(expected, target.attrs)
+        self.assertEqual(Tag.COMPLEX_TYPE, target.tag)
+
+    def test_build_elements_with_mixed_element_type_with_no_content(self):
+        target = ClassFactory.create(tag=Tag.ELEMENT)
+        element = DtdElementFactory.create(
+            type=DtdElementType.MIXED,
+            content=DtdContentFactory.create(
+                type=DtdContentType.PCDATA,
+            ),
+        )
+
+        DtdMapper.build_elements(target, element)
+        expected = [
+            AttrFactory.create(
+                tag=Tag.EXTENSION,
+                name="value",
+                index=0,
+                types=[AttrTypeFactory.native(DataType.STRING)],
+            ),
+        ]
+
+        self.assertFalse(target.mixed)
+        self.assertEqual(expected, target.attrs)
         self.assertEqual(Tag.COMPLEX_TYPE, target.tag)
-        self.assertEqual(str(DataType.STRING), target.extensions[0].type.qname)
-        self.assertTrue(target.extensions[0].type.native)
 
     def test_build_elements_with_any_element_type(self):
         target = ClassFactory.create()
         element = DtdElementFactory.create(type=DtdElementType.ANY)
 
         DtdMapper.build_elements(target, element)
         self.assertEqual(0, len(target.attrs))
@@ -226,23 +276,25 @@
         self.assertEqual(2, len(target.attrs))
         self.assertTrue(target.attrs[0].restrictions.nillable)
         self.assertTrue(target.attrs[1].restrictions.nillable)
 
     def test_build_content_type_or(self):
         content = DtdContentFactory.create(
             type=DtdContentType.OR,
+            occur=DtdContentOccur.MULT,
             left=DtdContentFactory.create(type=DtdContentType.ELEMENT),
             right=DtdContentFactory.create(type=DtdContentType.ELEMENT),
         )
         target = ClassFactory.create()
         DtdMapper.build_content(target, content, nillable=True)
         self.assertEqual(2, len(target.attrs))
         for attr in target.attrs:
-            self.assertEqual(str(id(content)), attr.restrictions.choice)
+            self.assertEqual(id(content), attr.restrictions.choice)
             self.assertEqual(0, attr.restrictions.min_occurs)
+            self.assertEqual(sys.maxsize, attr.restrictions.max_occurs)
 
     def test_build_content_type_or_nested(self):
         content = DtdContentFactory.create(
             type=DtdContentType.OR,
             left=DtdContentFactory.create(type=DtdContentType.ELEMENT),
             right=DtdContentFactory.create(type=DtdContentType.ELEMENT),
         )
@@ -255,15 +307,24 @@
 
     def test_build_content_type_pcdata(self):
         content = DtdContentFactory.create(
             type=DtdContentType.PCDATA,
         )
         target = ClassFactory.create()
         DtdMapper.build_content(target, content)
-        self.assertEqual(0, len(target.attrs))
+
+        expected = [
+            AttrFactory.create(
+                tag=Tag.EXTENSION,
+                name="value",
+                index=0,
+                types=[AttrTypeFactory.native(DataType.STRING)],
+            )
+        ]
+        self.assertEqual(expected, target.attrs)
 
     @mock.patch.object(DtdMapper, "build_content")
     def test_build_content_tree(self, mock_build_content):
         center = DtdContentFactory.create()
         target = ClassFactory.create()
 
         DtdMapper.build_content_tree(target, center, nillable=True)
```

### Comparing `xsdata-22.9/tests/codegen/mappers/test_element.py` & `xsdata-23.5/tests/codegen/test_resolver.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,259 +1,228 @@
-import sys
 from unittest import mock
 
-from xsdata.codegen.mappers.element import ElementMapper
-from xsdata.codegen.models import Restrictions
-from xsdata.codegen.utils import ClassUtils
-from xsdata.formats.dataclass.models.generics import AnyElement
+from xsdata.codegen.models import Class
+from xsdata.codegen.resolver import DependenciesResolver
+from xsdata.exceptions import ResolverValueError
 from xsdata.models.enums import DataType
-from xsdata.models.enums import QNames
-from xsdata.models.enums import Tag
+from xsdata.utils.namespaces import build_qname
 from xsdata.utils.testing import AttrFactory
 from xsdata.utils.testing import AttrTypeFactory
 from xsdata.utils.testing import ClassFactory
+from xsdata.utils.testing import ExtensionFactory
 from xsdata.utils.testing import FactoryTestCase
+from xsdata.utils.testing import PackageFactory
 
 
-class ElementMapperTests(FactoryTestCase):
-    @mock.patch.object(ClassUtils, "flatten")
-    @mock.patch.object(ElementMapper, "build_class")
-    def test_map(self, mock_build_class, mock_flatten):
-        element = AnyElement(qname="{xsdata}root")
-        root_class = ClassFactory.create()
-        flat_classes = ClassFactory.list(5)
-        iter_flat_classes = iter(flat_classes)
-
-        mock_build_class.return_value = root_class
-        mock_flatten.return_value = iter_flat_classes
-
-        actual = ElementMapper.map(element, "tests")
-
-        self.assertEqual(flat_classes, actual)
-        mock_build_class.assert_called_once_with(element, "xsdata")
-        mock_flatten.assert_called_once_with(root_class, "tests/root")
-
-    def test_build_class_simple_type(self):
-        element = AnyElement(
-            qname="{xsdata}root",
-            attributes={"{foo}bar": "1", "{bar}foo": "2.0"},
-            text="true",
-        )
+class DependenciesResolverTest(FactoryTestCase):
+    def setUp(self):
+        super().setUp()
+        self.resolver = DependenciesResolver({})
+
+    @mock.patch.object(DependenciesResolver, "resolve_imports")
+    @mock.patch.object(DependenciesResolver, "create_class_list")
+    @mock.patch.object(DependenciesResolver, "create_class_map")
+    def test_process(
+        self, mock_create_class_map, create_class_list, mock_resolve_imports
+    ):
+        classes = ClassFactory.list(3)
+
+        mock_create_class_map.return_value = {"b": classes[0]}
+        create_class_list.return_value = classes[::-1]
+
+        self.resolver.imports.append(PackageFactory.create(name="foo", source="bar"))
+        self.resolver.aliases = {"a": "a"}
+
+        self.resolver.process(classes)
+        self.assertEqual([], self.resolver.imports)
+        self.assertEqual({}, self.resolver.aliases)
+
+        self.assertEqual(mock_create_class_map.return_value, self.resolver.class_map)
+        self.assertEqual(create_class_list.return_value, self.resolver.class_list)
+
+        mock_resolve_imports.assert_called_once_with()
+
+    def test_sorted_imports(self):
+        packages = [
+            PackageFactory.create(name=x, alias=None, source="foo") for x in "cab"
+        ]
+        self.resolver.imports = packages
+
+        result = self.resolver.sorted_imports()
+        self.assertIsNot(packages, result)
+
+        self.assertEqual(packages[1], result[0])
+        self.assertEqual(packages[2], result[1])
+        self.assertEqual(packages[0], result[2])
+
+    @mock.patch.object(DependenciesResolver, "apply_aliases")
+    def test_sorted_classes(self, mock_apply_aliases):
+        mock_apply_aliases.side_effect = lambda x: x
+
+        self.resolver.class_list = ["a", "b", "c", "d"]
+        self.resolver.class_map = {x: ClassFactory.create(qname=x) for x in "ca"}
+
+        result = self.resolver.sorted_classes()
+        expected = [self.resolver.class_map[x] for x in "ac"]
+
+        self.assertEqual(expected, result)
+        mock_apply_aliases.assert_has_calls([mock.call(x) for x in expected])
+
+    def test_apply_aliases(self):
+        self.resolver.aliases = {
+            build_qname("xsdata", "d"): "IamD",
+            build_qname("xsdata", "a"): "IamA",
+        }
+        type_a = AttrTypeFactory.create(qname="{xsdata}a")
+        type_b = AttrTypeFactory.create(qname="{xsdata}b")
+        type_c = AttrTypeFactory.create(qname="{xsdata}c")
+        type_d = AttrTypeFactory.create(qname="{xsdata}d")
 
-        actual = ElementMapper.build_class(element, "target")
-        expected = ClassFactory.create(
-            tag=Tag.ELEMENT,
-            qname="{xsdata}root",
-            namespace="xsdata",
-            location="",
-            module=None,
-            ns_map={},
+        obj = ClassFactory.create(
+            qname="a",
             attrs=[
-                AttrFactory.native(
-                    DataType.INT,
-                    tag=Tag.ATTRIBUTE,
-                    name="bar",
-                    namespace="foo",
-                    index=0,
-                ),
-                AttrFactory.native(
-                    DataType.FLOAT,
-                    tag=Tag.ATTRIBUTE,
-                    name="foo",
-                    namespace="bar",
-                    index=1,
-                ),
-                AttrFactory.native(
-                    DataType.BOOLEAN,
-                    tag=Tag.SIMPLE_TYPE,
-                    name="value",
-                    namespace=None,
-                    index=2,
-                ),
-            ],
-        )
-        self.assertEqual(expected, actual)
-
-    def test_build_class_complex_type(self):
-        element = AnyElement(
-            qname="{xsdata}root",
-            children=[
-                AnyElement(qname="{xsdata}child", text="primitive"),
-                AnyElement(
-                    qname="{inner}child", attributes={"{foo}bar": "1", "{bar}foo": "2"}
-                ),
-            ],
-        )
-
-        actual = ElementMapper.build_class(element, "target")
-        expected = ClassFactory.create(
-            tag=Tag.ELEMENT,
-            qname="{xsdata}root",
-            namespace="xsdata",
-            location="",
-            module=None,
-            ns_map={},
-            attrs=[
-                AttrFactory.native(
-                    DataType.STRING,
-                    tag=Tag.ELEMENT,
-                    name="child",
-                    namespace="xsdata",
-                    index=0,
-                ),
-                AttrFactory.element(
-                    name="child",
-                    namespace="inner",
-                    types=[AttrTypeFactory.create(qname="{target}child", forward=True)],
-                    index=1,
-                ),
-            ],
-        )
-        self.assertEqual(1, len(actual.inner))
-
-        actual.inner.clear()
-        self.assertEqual(expected, actual)
-
-    def test_build_class_mixed_content(self):
-        element = AnyElement(
-            qname="{xsdata}root",
-            children=[
-                AnyElement(qname="{xsdata}child", text="primitive"),
-                AnyElement(qname="something", text="foo", tail="bar"),
-            ],
-        )
-
-        actual = ElementMapper.build_class(element, None)
-        expected = ClassFactory.create(
-            tag=Tag.ELEMENT,
-            qname="{xsdata}root",
-            namespace="xsdata",
-            location="",
-            module=None,
-            mixed=True,
-            ns_map={},
-            attrs=[
-                AttrFactory.native(
-                    DataType.STRING,
-                    name="child",
-                    namespace="xsdata",
-                    index=0,
-                    restrictions=Restrictions(min_occurs=0, max_occurs=1),
-                ),
-                AttrFactory.native(
-                    DataType.STRING,
-                    namespace="",
-                    name="something",
-                    index=1,
-                    restrictions=Restrictions(min_occurs=0, max_occurs=1),
-                ),
-            ],
-        )
-        self.assertEqual(expected, actual)
-
-        element = AnyElement(
-            qname="{xsdata}root",
-            text="foo",
-            children=[
-                AnyElement(qname="{xsdata}child", text="primitive"),
-            ],
-        )
-        actual = ElementMapper.build_class(element, None)
-        self.assertTrue(actual.mixed)
-
-    def test_build_class_nillable(self):
-        element = AnyElement(qname="{xsdata}root", attributes={QNames.XSI_NIL: "1"})
-        target = ElementMapper.build_class(element, None)
-        self.assertTrue(target.nillable)
-
-        element.attributes[QNames.XSI_NIL] = " true "
-        target = ElementMapper.build_class(element, None)
-        self.assertTrue(target.nillable)
-
-    def test_build_class_ignore_invalid(self):
-        element = AnyElement(
-            qname="{xsdata}root",
-            children=[
-                AnyElement(text="primitive"),
-                "",
-            ],
-        )
-        actual = ElementMapper.build_class(element, None)
-        self.assertEqual(0, len(actual.attrs))
-
-    def test_build_attribute_type(self):
-        actual = ElementMapper.build_attribute_type(QNames.XSI_TYPE, "")
-        self.assertEqual(str(DataType.QNAME), actual.qname)
-        self.assertTrue(actual.native)
-
-        actual = ElementMapper.build_attribute_type("name", "foo")
-        self.assertEqual(str(DataType.STRING), actual.qname)
-        self.assertTrue(actual.native)
-
-        actual = ElementMapper.build_attribute_type("name", "")
-        self.assertEqual(str(DataType.ANY_SIMPLE_TYPE), actual.qname)
-        self.assertTrue(actual.native)
-
-        actual = ElementMapper.build_attribute_type("name", None)
-        self.assertEqual(str(DataType.ANY_SIMPLE_TYPE), actual.qname)
-        self.assertTrue(actual.native)
-
-        actual = ElementMapper.build_attribute_type("name", 1)
-        self.assertEqual(str(DataType.SHORT), actual.qname)
-        self.assertTrue(actual.native)
-
-        actual = ElementMapper.build_attribute_type("name", "1.9")
-        self.assertEqual(str(DataType.FLOAT), actual.qname)
-        self.assertTrue(actual.native)
-
-    def test_add_attribute(self):
-        target = ClassFactory.elements(2)
-        attr = target.attrs[0].clone()
-        attr.index += 1
-
-        ElementMapper.add_attribute(target, attr)
-
-        self.assertEqual(2, len(target.attrs))
-        self.assertEqual(sys.maxsize, target.attrs[0].restrictions.max_occurs)
-        self.assertEqual(2, len(target.attrs[0].types))
-        self.assertFalse(target.attrs[0].restrictions.sequential)
-
-        attr = target.attrs[1].clone()
-        attr.restrictions.sequential = True
-        ElementMapper.add_attribute(target, attr)
-        self.assertTrue(target.attrs[1].restrictions.sequential)
-
-        attr = AttrFactory.create()
-        ElementMapper.add_attribute(target, attr)
-        self.assertEqual(3, len(target.attrs))
-
-    def test_select_namespace(self):
-        self.assertEqual("a", ElementMapper.select_namespace("a", "a", Tag.ELEMENT))
-        self.assertEqual("b", ElementMapper.select_namespace("b", "a", Tag.ELEMENT))
-        self.assertEqual("", ElementMapper.select_namespace(None, "a", Tag.ELEMENT))
-
-        self.assertEqual("a", ElementMapper.select_namespace("a", "a", Tag.ATTRIBUTE))
-        self.assertEqual("b", ElementMapper.select_namespace("b", "a", Tag.ATTRIBUTE))
-        self.assertIsNone(ElementMapper.select_namespace(None, "a", Tag.ATTRIBUTE))
-
-    def test_sequential_names(self):
-        a = AnyElement(qname="a")
-        b = AnyElement(qname="b")
-        c = AnyElement(qname="c")
-        d = AnyElement(qname="d")
-        e = AnyElement(qname="e")
-
-        p = AnyElement(children=[a, b])
-        actual = ElementMapper.sequential_names(p)
-        self.assertEqual(0, len(actual))
-
-        p = AnyElement(children=[a, b, a])
-        actual = ElementMapper.sequential_names(p)
-        self.assertEqual({"a", "b"}, actual)
-
-        p = AnyElement(children=[a, b, a, c])
-        actual = ElementMapper.sequential_names(p)
-        self.assertEqual({"a", "b"}, actual)
-
-        p = AnyElement(children=[a, b, a, c, d, e, d])
-        actual = ElementMapper.sequential_names(p)
-        self.assertEqual({"a", "b", "d", "e"}, actual)
+                AttrFactory.create(name="a", types=[type_a]),
+                AttrFactory.create(name="b", types=[type_b]),
+                AttrFactory.create(name="c", types=[type_a, type_d]),
+            ],
+            inner=[
+                ClassFactory.create(
+                    qname="b",
+                    attrs=[
+                        AttrFactory.create(name="c", types=[type_c]),
+                        AttrFactory.create(name="d", types=[type_d]),
+                        AttrFactory.create(
+                            name="compound",
+                            types=[AttrTypeFactory.native(DataType.ANY_TYPE)],
+                            choices=[
+                                AttrFactory.create(name="a", types=[type_a, type_d]),
+                            ],
+                        ),
+                    ],
+                )
+            ],
+            extensions=[ExtensionFactory.create(type_a)],
+        )
+
+        self.resolver.apply_aliases(obj)
+
+        self.assertEqual(3, len(obj.attrs))
+        self.assertEqual(1, len(obj.attrs[0].types))
+        self.assertEqual(1, len(obj.attrs[1].types))
+        self.assertEqual(2, len(obj.attrs[2].types))
+
+        self.assertEqual("IamA", obj.attrs[0].types[0].alias)
+        self.assertIsNone(obj.attrs[1].types[0].alias)
+        self.assertEqual("IamA", obj.attrs[2].types[0].alias)
+        self.assertEqual("IamD", obj.attrs[2].types[1].alias)
+        self.assertEqual("IamA", obj.extensions[0].type.alias)
+
+        self.assertEqual(1, len(obj.inner))
+        self.assertEqual(3, len(obj.inner[0].attrs))
+        self.assertEqual(1, len(obj.inner[0].attrs[0].types))
+        self.assertEqual(1, len(obj.inner[0].attrs[1].types))
+
+        self.assertEqual("IamA", obj.inner[0].attrs[2].choices[0].types[0].alias)
+        self.assertEqual("IamD", obj.inner[0].attrs[2].choices[0].types[1].alias)
+
+        self.assertIsNone(obj.inner[0].attrs[0].types[0].alias)
+        self.assertEqual("IamD", obj.inner[0].attrs[1].types[0].alias)
+
+    @mock.patch.object(DependenciesResolver, "set_aliases")
+    @mock.patch.object(DependenciesResolver, "resolve_conflicts")
+    @mock.patch.object(DependenciesResolver, "find_package")
+    @mock.patch.object(DependenciesResolver, "import_classes")
+    def test_resolve_imports(
+        self,
+        mock_import_classes,
+        mock_find_package,
+        mock_resolve_conflicts,
+        mock_set_aliases,
+    ):
+        class_life = ClassFactory.create(qname="life")
+        import_names = [
+            "foo_1",  # cool
+            "bar",  # cool
+            "{another}foo1",  # another foo
+            "{thug}life",  # life class exists add alias
+            "{common}type",  # type class doesn't exist add just the name
+        ]
+        self.resolver.class_map = {class_life.qname: class_life}
+        mock_import_classes.return_value = import_names
+        mock_find_package.side_effect = ["first", "second", "third", "forth", "fifth"]
+
+        self.resolver.resolve_imports()
+        mock_resolve_conflicts.assert_called_once_with(
+            self.resolver.imports, {class_life.slug}
+        )
+        mock_set_aliases.assert_called_once_with()
+
+    def test_resolve_conflicts(self):
+        imports = [
+            PackageFactory.create(qname="{a}a", source="models.aa"),
+            PackageFactory.create(qname="{b}a", source="models.ba"),
+            PackageFactory.create(qname="{c}root", source="models.common"),
+            PackageFactory.create(qname="{c}penalty", source="models.common"),
+        ]
+
+        protected = {"penalty"}
+        self.resolver.resolve_conflicts(imports, protected)
+
+        self.assertEqual("aa:a", imports[0].alias)
+        self.assertEqual("ba:a", imports[1].alias)
+        self.assertEqual(None, imports[2].alias)
+        self.assertEqual("common:penalty", imports[3].alias)
+
+    def test_set_aliases(self):
+        self.resolver.imports = [
+            PackageFactory.create(qname="{a}a", alias="aa"),
+            PackageFactory.create(qname="{b}a", alias="ba"),
+            PackageFactory.create(qname="{c}a"),
+        ]
+        self.resolver.set_aliases()
+        self.assertEqual({"{a}a": "aa", "{b}a": "ba"}, self.resolver.aliases)
+
+    def test_find_package(self):
+        class_a = ClassFactory.create()
+        self.resolver.packages[class_a.qname] = "foo.bar"
+
+        self.assertEqual("foo.bar", self.resolver.find_package(class_a.qname))
+        with self.assertRaises(ResolverValueError):
+            self.resolver.find_package("nope")
+
+    def test_import_classes(self):
+        self.resolver.class_list = [x for x in "abcdefg"]
+        self.resolver.class_map = {x: x for x in "bdg"}
+        self.assertEqual(["a", "c", "e", "f"], self.resolver.import_classes())
+
+    def test_create_class_map(self):
+        classes = [ClassFactory.create(qname=name) for name in "ab"]
+        expected = {obj.qname: obj for obj in classes}
+        self.assertEqual(expected, self.resolver.create_class_map(classes))
+
+    def test_create_class_map_for_duplicate_classes(self):
+        classes = ClassFactory.list(2, qname="a")
+        with self.assertRaises(ResolverValueError) as cm:
+            self.resolver.create_class_map(classes)
+
+        self.assertEqual("Duplicate class: `a`", str(cm.exception))
+
+    @mock.patch.object(Class, "dependencies")
+    def test_create_class_list(self, mock_dependencies):
+        classes = ClassFactory.list(3)
+        mock_dependencies.side_effect = [
+            {build_qname("xsdata", "class_C"), "b"},
+            {"c", "d"},
+            {"e", "d"},
+        ]
+
+        actual = self.resolver.create_class_list(classes)
+        expected = [
+            "b",
+            "c",
+            "d",
+            "e",
+            "{xsdata}class_C",
+            "{xsdata}class_D",
+            "{xsdata}class_B",
+        ]
+        self.assertEqual(expected, list(map(str, actual)))
```

### Comparing `xsdata-22.9/tests/codegen/mappers/test_schema.py` & `xsdata-23.5/tests/codegen/mappers/test_schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -176,34 +176,37 @@
         self.assertEqual(expected, result)
 
     @mock.patch.object(SchemaMapper, "children_extensions")
     def test_build_class_extensions(self, mock_children_extensions):
         bar_type = AttrTypeFactory.create(qname="bar")
         foo_type = AttrTypeFactory.create(qname="foo")
 
-        bar = ExtensionFactory.create(bar_type)
-        double = ExtensionFactory.create(bar_type)
-        foo = ExtensionFactory.create(foo_type)
+        bar = ExtensionFactory.create(bar_type, tag=Tag.RESTRICTION)
+        double = ExtensionFactory.create(bar_type, tag=Tag.RESTRICTION)
+        foo = ExtensionFactory.create(foo_type, tag=Tag.EXTENSION)
 
         mock_children_extensions.return_value = [bar, double, foo]
         self_ext = ExtensionFactory.reference(
             qname="{xsdata}something",
+            tag=Tag.ELEMENT,
             restrictions=Restrictions(min_occurs=1, max_occurs=1),
         )
 
         item = ClassFactory.create()
         element = Element(type="something")
         SchemaMapper.build_class_extensions(element, item)
 
         self.assertEqual(3, len(item.extensions))
         self.assertCountEqual([bar, self_ext, foo], item.extensions)
 
     def test_element_children(self):
         sequence_one = Sequence(elements=[Element(), Element()])
+        sequence_one.index = 1
         sequence_two = Sequence(max_occurs=2, elements=[Element(), Element()])
+        sequence_two.index = 2
         restriction = Restriction(
             enumerations=[Enumeration(value=x) for x in "abc"], sequence=sequence_two
         )
         complex_type = ComplexType(
             attributes=[Attribute(), Attribute()],
             sequence=sequence_one,
             simple_content=SimpleContent(restriction=Restriction()),
@@ -226,43 +229,45 @@
         self.assertEqual(expected, list(children))
 
     def test_element_children_with_parents_restrictions(self):
         choice = Choice(elements=[Element(name="elem1")])
         complex_type = ComplexType(
             sequence=Sequence(choices=[choice], min_occurs=0, max_occurs=3)
         )
+        complex_type.sequence.index = 2
         parent_restrictions = Restrictions.from_element(complex_type)
         children = SchemaMapper.element_children(complex_type, parent_restrictions)
 
         child, restrictions = next(children)
         expected = Restrictions(
-            min_occurs=0, max_occurs=3, sequential=True, choice=str(id(choice))
+            path=[("s", id(complex_type.sequence), 0, 3), ("c", id(choice), 1, 1)]
         )
         self.assertEqual(expected, restrictions)
 
     def test_children_extensions(self):
         complex_type = ComplexType(
             attributes=[Attribute() for _ in range(2)],
             simple_content=SimpleContent(restriction=Restriction(base="bk:b")),
             complex_content=ComplexContent(extension=Extension(base="bk:c")),
         )
         complex_type.simple_content.restriction.index = 4
         complex_type.complex_content.extension.index = 7
 
         item = ClassFactory.create(ns_map={"bk": "book"})
         children = SchemaMapper.children_extensions(complex_type, item)
-        expected = list(
-            map(
-                ExtensionFactory.create,
-                [
-                    AttrTypeFactory.create(qname=build_qname("book", "b")),
-                    AttrTypeFactory.create(qname=build_qname("book", "c")),
-                ],
-            )
-        )
+        expected = [
+            ExtensionFactory.create(
+                AttrTypeFactory.create(qname=build_qname("book", "b")),
+                tag=Tag.RESTRICTION,
+            ),
+            ExtensionFactory.create(
+                AttrTypeFactory.create(qname=build_qname("book", "c")),
+                tag=Tag.EXTENSION,
+            ),
+        ]
 
         self.assertIsInstance(children, GeneratorType)
         self.assertEqual(expected, list(children))
 
     @mock.patch.object(SchemaMapper, "build_class_attribute_types")
     @mock.patch.object(SchemaMapper, "element_namespace")
     @mock.patch.object(Attribute, "get_restrictions")
@@ -312,20 +317,14 @@
             restrictions=Restrictions(min_occurs=1, max_occurs=1),
         )
         self.assertEqual(expected, item.attrs[0])
         self.assertEqual({"bar": "foo", "foo": "bar"}, item.ns_map)
         mock_build_class_attribute_types.assert_called_once_with(item, attribute)
         mock_element_namespace.assert_called_once_with(attribute, item.target_namespace)
 
-    def test_build_class_attribute_skip_prohibited(self):
-        item = ClassFactory.create(ns_map={"bar": "foo"})
-        attribute = Attribute(use=UseType.PROHIBITED)
-        SchemaMapper.build_class_attribute(item, attribute, Restrictions())
-        self.assertEqual(0, len(item.attrs))
-
     @mock.patch.object(Attribute, "attr_types", new_callable=mock.PropertyMock)
     @mock.patch.object(SchemaMapper, "build_inner_classes")
     def test_build_class_attribute_types(
         self, mock_build_inner_classes, mock_attr_types
     ):
         mock_attr_types.return_value = ["xs:integer", "xs:string"]
         mock_build_inner_classes.return_value = []
```

### Comparing `xsdata-22.9/tests/codegen/models/test_attr.py` & `xsdata-23.5/tests/codegen/models/test_attr.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,14 +25,18 @@
 
         attr.index = -1
         self.assertEqual(attr, clone)
 
         attr.namespace = __file__
         self.assertNotEqual(attr, clone)
 
+    def test_property_key(self):
+        attr = AttrFactory.attribute(name="a", namespace="b")
+        self.assertEqual("Attribute.b.a", attr.key)
+
     def test_property_is_property(self):
         self.assertTrue(AttrFactory.attribute().is_attribute)
         self.assertTrue(AttrFactory.any_attribute().is_attribute)
         self.assertFalse(AttrFactory.element().is_attribute)
 
     def test_property_is_enumeration(self):
         self.assertTrue(AttrFactory.enumeration().is_enumeration)
@@ -55,14 +59,21 @@
     def test_property_is_list(self):
         attr = AttrFactory.create(restrictions=Restrictions(max_occurs=2))
         self.assertTrue(attr.is_list)
 
         attr.restrictions.max_occurs = 1
         self.assertFalse(attr.is_list)
 
+    def test_property_is_prohibited(self):
+        attr = AttrFactory.create(restrictions=Restrictions(max_occurs=0))
+        self.assertTrue(attr.is_prohibited)
+
+        attr.restrictions.max_occurs = 1
+        self.assertFalse(attr.is_list)
+
     def test_property_is_optional(self):
         attr = AttrFactory.create(restrictions=Restrictions(min_occurs=0))
         self.assertTrue(attr.is_optional)
 
         attr.restrictions.min_occurs = 1
         self.assertFalse(attr.is_optional)
 
@@ -91,14 +102,26 @@
         self.assertTrue(attr.is_xsi_type)
 
     def test_property_is_nameless(self):
         self.assertFalse(AttrFactory.create(tag=Tag.ELEMENT).is_nameless)
         self.assertFalse(AttrFactory.create(tag=Tag.ATTRIBUTE).is_nameless)
         self.assertTrue(AttrFactory.create(tag=Tag.ANY).is_nameless)
 
+    def test_property_is_any_type(self):
+        attr = AttrFactory.create(
+            types=[
+                AttrTypeFactory.create(qname="foo"),
+                AttrTypeFactory.native(DataType.FLOAT),
+            ]
+        )
+        self.assertFalse(attr.is_any_type)
+
+        attr.types.append(AttrTypeFactory.native(DataType.ANY_SIMPLE_TYPE))
+        self.assertTrue(attr.is_any_type)
+
     def test_property_native_types(self):
         attr = AttrFactory.create(
             types=[
                 AttrTypeFactory.create(qname="foo"),
                 AttrTypeFactory.native(DataType.INT),
                 AttrTypeFactory.native(DataType.SHORT),
                 AttrTypeFactory.native(DataType.INTEGER),
```

### Comparing `xsdata-22.9/tests/codegen/models/test_attr_type.py` & `xsdata-23.5/tests/codegen/models/test_attr_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from xsdata.utils.testing import AttrTypeFactory
 from xsdata.utils.testing import FactoryTestCase
 
 
 class AttrTypeTests(FactoryTestCase):
     def test_property_is_dependency(self):
-
         attr_type = AttrTypeFactory.create(forward=True, native=True, circular=True)
         self.assertFalse(attr_type.is_dependency(False))
 
         attr_type.forward = False
         self.assertFalse(attr_type.is_dependency(False))
 
         attr_type.native = False
```

### Comparing `xsdata-22.9/tests/codegen/models/test_class.py` & `xsdata-23.5/tests/codegen/models/test_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,14 @@
 
         obj.inner.append(ClassFactory.elements(2))
         obj.inner[0].attrs[1].types[0].reference = 6
 
         self.assertEqual(list(range(1, 7)), list(obj.references))
 
     def test_property_target_module(self):
-
         obj = ClassFactory.create(module=None, package=None)
         with self.assertRaises(CodeGenerationError) as cm:
             obj.target_module
 
         self.assertEqual(
             f"Class `{obj.name}` has not been assigned to a module yet!",
             str(cm.exception),
```

### Comparing `xsdata-22.9/tests/codegen/models/test_restrictions.py` & `xsdata-23.5/tests/codegen/models/test_restrictions.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
             total_digits=333,
             fraction_digits=2,
             length=5,
             white_space="collapse",
             pattern=r"[A-Z]",
             explicit_timezone="+1",
             nillable=True,
+            path=[("s", 0, 1, 1)],
         )
 
     def test_property_is_list(self):
         restrictions = Restrictions()
         self.assertFalse(restrictions.is_list)
 
         restrictions.max_occurs = 1
@@ -56,14 +57,29 @@
         child.merge(parent)
         self.assertIsNone(child.nillable)
 
         child.nillable = False
         child.merge(parent)
         self.assertFalse(child.nillable)
 
+    def test_merge_occurs(self):
+        a = Restrictions()
+        b = Restrictions()
+
+        a.merge(b)
+
+        self.assertIsNone(a.min_occurs)
+        self.assertIsNone(a.max_occurs)
+
+        b.min_occurs = 0
+        b.max_occurs = 1
+        a.merge(b)
+        self.assertEqual(0, a.min_occurs)
+        self.assertEqual(1, a.max_occurs)
+
     def test_asdict(self):
         expected = {
             "explicit_timezone": "+1",
             "fraction_digits": 2,
             "length": 5,
             "max_exclusive": "1",
             "max_inclusive": "1.1",
```

### Comparing `xsdata-22.9/tests/codegen/parsers/test_definitions.py` & `xsdata-23.5/tests/codegen/parsers/test_definitions.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/codegen/parsers/test_dtd.py` & `xsdata-23.5/tests/codegen/parsers/test_dtd.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
                     "left": None,
                     "name": "Origin",
                     "occur": DtdContentOccur.ONCE,
                     "right": None,
                     "type": DtdContentType.ELEMENT,
                 },
                 "name": None,
-                "occur": DtdContentOccur.ONCE,
+                "occur": DtdContentOccur.MULT,
                 "right": {
                     "left": None,
                     "name": "Source",
                     "occur": DtdContentOccur.ONCE,
                     "right": None,
                     "type": DtdContentType.ELEMENT,
                 },
```

### Comparing `xsdata-22.9/tests/codegen/parsers/test_schema.py` & `xsdata-23.5/tests/codegen/parsers/test_schema.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/codegen/test_analyzer.py` & `xsdata-23.5/tests/codegen/test_analyzer.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/codegen/test_container.py` & `xsdata-23.5/tests/codegen/test_container.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,56 +23,60 @@
             ClassFactory.create(qname="{xsdata}foo", tag=Tag.COMPLEX_TYPE),
             ClassFactory.create(qname="{xsdata}foobar", tag=Tag.COMPLEX_TYPE),
         ]
         config = GeneratorConfig()
         container = ClassContainer(config)
         container.extend(classes)
 
-        expected = {
-            "{xsdata}foo": classes[:2],
-            "{xsdata}foobar": classes[2:],
-        }
-
         self.assertEqual(2, len(container.data))
         self.assertEqual(3, len(list(container)))
         self.assertEqual(classes, list(container))
 
         actual = {
             step: [processor.__class__.__name__ for processor in processors]
             for step, processors in container.processors.items()
         }
 
         expected = {
             10: [
                 "FlattenAttributeGroups",
+            ],
+            20: [
+                "CalculateAttributePaths",
                 "FlattenClassExtensions",
                 "SanitizeEnumerationClass",
+                "UpdateAttributesEffectiveChoice",
                 "UnnestInnerClasses",
                 "AddAttributeSubstitutions",
                 "ProcessAttributeTypes",
                 "MergeAttributes",
                 "ProcessMixedContentClass",
             ],
-            20: ["UpdateAttributesEffectiveChoice", "SanitizeAttributesDefaultValue"],
-            30: ["ValidateAttributesOverrides", "RenameDuplicateAttributes"],
-            40: ["VacuumInnerClasses", "CreateCompoundFields"],
+            30: ["ResetAttributeSequences", "SanitizeAttributesDefaultValue"],
+            40: ["ValidateAttributesOverrides", "RenameDuplicateAttributes"],
+            50: [
+                "VacuumInnerClasses",
+                "CreateCompoundFields",
+                "ResetAttributeSequenceNumbers",
+            ],
         }
 
         self.assertEqual(expected, actual)
 
     @mock.patch.object(ClassContainer, "process_class")
     def test_find(self, mock_process_class):
         def process_class(x: Class, step: int):
             x.status = Status.FLATTENED
 
         class_a = ClassFactory.create(qname="a")
         class_b = ClassFactory.create(qname="b", status=Status.FLATTENED)
         class_c = ClassFactory.enumeration(2, qname="b", status=Status.FLATTENING)
         mock_process_class.side_effect = process_class
         self.container.extend([class_a, class_b, class_c])
+        self.container.step = Steps.FLATTEN
 
         self.assertIsNone(self.container.find("nope"))
         self.assertEqual(class_a, self.container.find(class_a.qname))
         self.assertEqual(class_b, self.container.find(class_b.qname))
         self.assertEqual(
             class_c, self.container.find(class_b.qname, lambda x: x.is_enumeration)
         )
@@ -85,14 +89,15 @@
         second = ClassFactory.create(qname="{a}b", status=Status.FLATTENED)
         obj.inner.extend((first, second))
 
         def process_class(x: Class, step: int):
             x.status = Status.FLATTENED
 
         mock_process_class.side_effect = process_class
+        self.container.step = Steps.FLATTEN
 
         self.assertEqual(first, self.container.find_inner(obj, "{a}a"))
         self.assertEqual(second, self.container.find_inner(obj, "{a}b"))
         mock_process_class.assert_called_once_with(first, Steps.FLATTEN)
 
     def test_first(self):
         obj = ClassFactory.create()
@@ -139,7 +144,18 @@
 
         container = ClassContainer(config=GeneratorConfig())
         container.extend([complex_type, enum_1, enum_2, simple_type, element])
 
         expected = [complex_type, enum_1]
         container.filter_classes()
         self.assertEqual(expected, list(container))
+
+    def test_remove_groups(self):
+        classes = [
+            ClassFactory.create(tag=Tag.ATTRIBUTE_GROUP),
+            ClassFactory.create(tag=Tag.GROUP),
+            ClassFactory.create(tag=Tag.ELEMENT),
+        ]
+
+        self.container.extend(classes)
+        self.container.remove_groups()
+        self.assertEqual(1, len(list(self.container)))
```

### Comparing `xsdata-22.9/tests/codegen/test_transformer.py` & `xsdata-23.5/tests/codegen/test_transformer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import pickle
 import tempfile
 from pathlib import Path
 from unittest import mock
 
 from xsdata.codegen.analyzer import ClassAnalyzer
 from xsdata.codegen.container import ClassContainer
 from xsdata.codegen.mappers.definitions import DefinitionsMapper
@@ -67,14 +68,53 @@
         mock_process_definitions.assert_called_once_with(uris[:2])
         mock_process_schemas.assert_called_once_with(uris[2:4])
         mock_process_xml_documents.assert_called_once_with(uris[4:6])
         mock_process_json_documents.assert_called_once_with(uris[6:8])
         mock_process_dtds.assert_called_once_with(uris[8:])
         mock_process_classes.assert_called_once_with()
 
+    @mock.patch.object(SchemaTransformer, "process_classes")
+    @mock.patch.object(SchemaTransformer, "process_sources")
+    @mock.patch.object(SchemaTransformer, "get_cache_file")
+    def test_process_from_cache(
+        self, mock_get_cache_file, mock_process_sources, mock_process_classes
+    ):
+        with tempfile.TemporaryDirectory() as tmpdir:
+            cache = Path(tmpdir).joinpath("foo.cache")
+            classes = ClassFactory.list(2)
+            cache.write_bytes(pickle.dumps(classes))
+
+            mock_get_cache_file.return_value = cache
+            uris = ["a.xml", "b.xml"]
+
+            self.transformer.process(uris, cache=True)
+
+            self.assertEqual(classes, self.transformer.classes)
+            self.assertEqual(0, mock_process_sources.call_count)
+            mock_process_classes.assert_called_once_with()
+
+    @mock.patch.object(SchemaTransformer, "process_classes")
+    @mock.patch.object(SchemaTransformer, "process_sources")
+    @mock.patch.object(SchemaTransformer, "get_cache_file")
+    def test_process_with_cache(
+        self, mock_get_cache_file, mock_process_sources, mock_process_classes
+    ):
+        with tempfile.TemporaryDirectory() as tmpdir:
+            cache = Path(tmpdir).joinpath("foo.cache")
+            classes = ClassFactory.list(2)
+            self.transformer.classes = classes
+            mock_get_cache_file.return_value = cache
+            uris = ["a.xml", "b.xml"]
+
+            self.transformer.process(uris, cache=True)
+            self.assertEqual(1, mock_process_sources.call_count)
+
+            self.assertEqual(classes, pickle.loads(cache.read_bytes()))
+            mock_process_classes.assert_called_once_with()
+
     @mock.patch.object(SchemaTransformer, "convert_schema")
     @mock.patch.object(SchemaTransformer, "convert_definitions")
     @mock.patch.object(SchemaTransformer, "parse_definitions")
     def test_process_definitions(
         self,
         mock_parse_definitions,
         mock_convert_definitions,
@@ -129,22 +169,23 @@
 
         mock_from_bytes.assert_has_calls(
             [mock.call(resources[0]), mock.call(resources[2])]
         )
         mock_map.assert_has_calls([mock.call(x, "foo") for x in elements])
         mock_reduce_classes.assert_called_once_with(classes_a + classes_c)
 
+    @mock.patch("xsdata.codegen.transformer.logger.warning")
     @mock.patch.object(ClassUtils, "reduce_classes")
     @mock.patch.object(DictMapper, "map")
     @mock.patch.object(SchemaTransformer, "load_resource")
     def test_process_json_documents(
-        self, mock_load_resource, mock_map, mock_reduce_classes
+        self, mock_load_resource, mock_map, mock_reduce_classes, mock_warning
     ):
-        uris = ["foo/a.json", "foo/b.json", "foo/c.json"]
-        resources = [b'{"foo": 1}', None, b'[{"foo": true}]']
+        uris = ["foo/a.json", "foo/b.json", "foo/c.json", "bar.json"]
+        resources = [b'{"foo": 1}', None, b'[{"foo": true}]', b"notjson"]
 
         classes_a = ClassFactory.list(2)
         classes_c = ClassFactory.list(3)
 
         mock_load_resource.side_effect = resources
         mock_map.side_effect = [classes_a, classes_c]
         mock_reduce_classes.return_value = classes_a + classes_c
@@ -157,14 +198,17 @@
         mock_map.assert_has_calls(
             [
                 mock.call({"foo": 1}, "books", "foo"),
                 mock.call({"foo": True}, "books", "foo"),
             ]
         )
         mock_reduce_classes.assert_called_once_with(classes_a + classes_c)
+        mock_warning.assert_called_once_with(
+            "JSON load failed for file: %s", uris[3], exc_info=mock.ANY
+        )
 
     @mock.patch.object(DtdMapper, "map")
     @mock.patch.object(DtdParser, "parse")
     @mock.patch.object(SchemaTransformer, "load_resource")
     def test_process_dtds(self, mock_load_resource, mock_parse, mock_map):
         uris = ["foo/a.dtd", "foo/b.dtd", "foo/c.dtd"]
         resources = [b"a", None, b"c"]
@@ -441,7 +485,15 @@
         self.assertEqual(1, len(result))
 
         actual = mock_process.call_args[0][0]
 
         self.assertIsInstance(actual, ClassContainer)
         self.assertEqual(2, len(actual.data))
         self.assertEqual(self.transformer.config, actual.config)
+
+    def test_get_cache_file(self):
+        uris = ["a.xml", "b.json"]
+        actual = self.transformer.get_cache_file(uris)
+        tempdir = Path(tempfile.gettempdir())
+        expected = tempdir.joinpath("ae1bed744d3d3611e698a2d2ef5335d2.cache")
+
+        self.assertEqual(expected, actual)
```

### Comparing `xsdata-22.9/tests/codegen/test_utils.py` & `xsdata-23.5/tests/codegen/test_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 
         ClassUtils.clean_inner_classes(target)
 
         self.assertEqual(1, len(target.inner))
         self.assertEqual(survivor, target.inner[0])
 
     def test_is_orphan_inner(self):
-
         inner = ClassFactory.create(qname="thug")
         target = ClassFactory.create(
             attrs=[
                 AttrFactory.create(
                     types=[
                         AttrTypeFactory.create(qname="bar"),
                         AttrTypeFactory.create(qname="foo"),
@@ -111,20 +110,22 @@
     def test_copy_group_attributes(self, mock_clone_attribute, mock_copy_inner_classes):
         mock_clone_attribute.side_effect = lambda x, y: x.clone()
         source = ClassFactory.elements(2)
         source.inner.append(ClassFactory.create())
         target = ClassFactory.elements(3)
         attrs = list(target.attrs)
         attrs[1].name = "bar"
+        attr = target.attrs[1]
 
-        ClassUtils.copy_group_attributes(source, target, target.attrs[1])
+        ClassUtils.copy_group_attributes(source, target, attr)
 
         self.assertEqual(4, len(target.attrs))
         self.assertEqual(source.attrs[0], target.attrs[1])
         self.assertEqual(source.attrs[1], target.attrs[2])
+
         mock_copy_inner_classes.assert_has_calls(
             [
                 mock.call(source, target, source.attrs[0]),
                 mock.call(source, target, source.attrs[1]),
             ]
         )
         mock_clone_attribute.assert_has_calls(
@@ -270,51 +271,51 @@
 
         self.assertEqual(
             ["attr_B", "attr_C", "attr_D"], [x.name for x in result[0].attrs]
         )
         self.assertEqual(["attr_E", "attr_F"], [x.name for x in result[1].attrs])
 
     def test_reduce_attributes(self):
-        attrs = AttrFactory.list(5, prefix="")
-
-        class_a = ClassFactory.create()
-        class_a.attrs = [x.clone() for x in attrs[:2]]
-
-        class_b = ClassFactory.create()
-        class_b.attrs = [x.clone() for x in attrs[2:4]]
-
-        class_c = ClassFactory.create()
-        class_c.attrs = [x.clone() for x in attrs[3:]]
-
-        class_d = ClassFactory.create()
-        class_d.attrs.append(attrs[0].clone())
-        class_d.attrs.append(attrs[4].clone())
-
-        result = ClassUtils.reduce_attributes([class_a, class_b, class_c, class_d])
-        self.assertEqual(["B", "C", "D", "E", "F"], [x.name for x in result])
+        restrictions = Restrictions(min_occurs=1, max_occurs=1)
+        attr_a = AttrFactory.create(name="a", restrictions=restrictions.clone())
+        attr_b = AttrFactory.create(name="b", restrictions=restrictions.clone())
+        attr_c = AttrFactory.create(name="c", restrictions=restrictions.clone())
+        attr_d = AttrFactory.create(name="d", restrictions=restrictions.clone())
+
+        first = ClassFactory.create(qname="alphabet", attrs=[attr_b, attr_c, attr_d])
+        second = ClassFactory.create(qname="alphabet", attrs=[attr_a, attr_b])
+
+        result = ClassUtils.reduce_attributes([first, second])
+        expected_names = ["a", "b", "c", "d"]
+        self.assertEqual(expected_names, [x.name for x in result])
+
+        self.assertEqual(0, result[0].restrictions.min_occurs)
+        self.assertEqual(1, result[1].restrictions.min_occurs)
+        self.assertEqual(0, result[2].restrictions.min_occurs)
+        self.assertEqual(0, result[3].restrictions.min_occurs)
 
     def test_merge_attributes(self):
         a = AttrFactory.native(DataType.INT, name="a")
         c = AttrFactory.native(DataType.FLOAT, name="c")
 
         ClassUtils.merge_attributes(a, c)
         self.assertEqual(["int", "float"], [x.name for x in a.types])
 
         self.assertEqual(0, a.restrictions.min_occurs)
         self.assertEqual(1, a.restrictions.max_occurs)
-        self.assertFalse(a.restrictions.sequential)
+        self.assertIsNone(a.restrictions.sequence)
 
         c.restrictions.min_occurs = 2
-        a.restrictions.sequential = True
+        a.restrictions.sequence = 1
         a.restrictions.max_occurs = 4
 
         ClassUtils.merge_attributes(c, a)
         self.assertEqual(0, c.restrictions.min_occurs)
         self.assertEqual(4, c.restrictions.max_occurs)
-        self.assertTrue(c.restrictions.sequential)
+        self.assertEqual(1, c.restrictions.sequence)
 
     def test_rename_attribute_by_preference(self):
         one = AttrFactory.create(name="a", tag=Tag.ELEMENT)
         two = AttrFactory.create(name="a", tag=Tag.ATTRIBUTE)
 
         ClassUtils.rename_attribute_by_preference(one, two)
         self.assertEqual("a", one.name)
```

### Comparing `xsdata-22.9/tests/codegen/test_validator.py` & `xsdata-23.5/tests/codegen/test_validator.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/codegen/test_writer.py` & `xsdata-23.5/tests/codegen/test_writer.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,40 +12,40 @@
 from xsdata.formats.mixins import GeneratorResult
 from xsdata.models.config import GeneratorConfig
 from xsdata.utils.testing import ClassFactory
 from xsdata.utils.testing import FactoryTestCase
 
 
 class NoneGenerator(AbstractGenerator):
-    def __init__(self):
-        pass
-
     def render(self, classes: List[Class]) -> Iterator[GeneratorResult]:
         pass
 
 
 class CodeWriterTests(FactoryTestCase):
     def setUp(self):
-        generator = NoneGenerator()
+        config = GeneratorConfig()
+        generator = NoneGenerator(config)
         self.writer = CodeWriter(generator)
 
+    @mock.patch.object(NoneGenerator, "render_header")
     @mock.patch.object(NoneGenerator, "render")
     @mock.patch.object(NoneGenerator, "normalize_packages")
-    def test_write(self, mock_normalize_packages, mock_render):
+    def test_write(self, mock_normalize_packages, mock_render, mock_render_header):
         classes = ClassFactory.list(2)
         with TemporaryDirectory() as tmpdir:
             mock_render.return_value = [
                 GeneratorResult(Path(f"{tmpdir}/foo/a.py"), "file", "aAa"),
                 GeneratorResult(Path(f"{tmpdir}/bar/b.py"), "file", "bBb"),
                 GeneratorResult(Path(f"{tmpdir}/c.py"), "file", " "),
             ]
+            mock_render_header.return_value = "// Head\n"
             self.writer.write(classes)
 
-            self.assertEqual("aAa", Path(f"{tmpdir}/foo/a.py").read_text())
-            self.assertEqual("bBb", Path(f"{tmpdir}/bar/b.py").read_text())
+            self.assertEqual("// Head\naAa", Path(f"{tmpdir}/foo/a.py").read_text())
+            self.assertEqual("// Head\nbBb", Path(f"{tmpdir}/bar/b.py").read_text())
             self.assertFalse(Path(f"{tmpdir}/c.py").exists())
             mock_normalize_packages.assert_called_once_with(classes)
 
     @mock.patch.object(NoneGenerator, "render")
     @mock.patch.object(NoneGenerator, "normalize_packages")
     @mock.patch("builtins.print")
     def test_print(self, mock_print, mock_normalize_packages, mock_render):
```

### Comparing `xsdata-22.9/tests/conftest.py` & `xsdata-23.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/fixtures/annotations/model.py` & `xsdata-23.5/tests/fixtures/annotations/model.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/fixtures/annotations/model.xsd` & `xsdata-23.5/tests/fixtures/annotations/model.xsd`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/fixtures/annotations/units.xsd` & `xsdata-23.5/tests/fixtures/annotations/units.xsd`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/fixtures/annotations/xsdata.xml` & `xsdata-23.5/tests/fixtures/annotations/xsdata.xml`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/fixtures/artists/art001.xml` & `xsdata-23.5/tests/fixtures/artists/art001.xml`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/fixtures/artists/art002.xml` & `xsdata-23.5/tests/fixtures/artists/art002.xml`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/fixtures/artists/art003.xml` & `xsdata-23.5/tests/fixtures/artists/art003.xml`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/fixtures/books/books.py` & `xsdata-23.5/tests/fixtures/books/books.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/fixtures/books/books.xml` & `xsdata-23.5/tests/fixtures/books/books.xml`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/fixtures/books/books_auto_ns.xml` & `xsdata-23.5/tests/fixtures/books/books_auto_ns.xml`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/fixtures/books/books_default_ns.xml` & `xsdata-23.5/tests/fixtures/books/books_default_ns.xml`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/fixtures/books/fixtures.py` & `xsdata-23.5/tests/fixtures/books/fixtures.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/fixtures/books/schema.xsd` & `xsdata-23.5/tests/fixtures/books/schema.xsd`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/fixtures/calculator/__init__.py` & `xsdata-23.5/tests/fixtures/calculator/__init__.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/fixtures/calculator/services.py` & `xsdata-23.5/tests/fixtures/calculator/services.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/fixtures/calculator/services.wsdl` & `xsdata-23.5/tests/fixtures/calculator/services.wsdl`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/fixtures/compound/models.py` & `xsdata-23.5/tests/fixtures/compound/models.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/fixtures/compound/schema.xsd` & `xsdata-23.5/tests/fixtures/compound/schema.xsd`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/fixtures/datatypes.py` & `xsdata-23.5/tests/fixtures/datatypes.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/fixtures/docstrings/accessible/schema.py` & `xsdata-23.5/tests/fixtures/docstrings/accessible/schema.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/fixtures/docstrings/blank/schema.py` & `xsdata-23.5/tests/fixtures/docstrings/blank/schema.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/fixtures/docstrings/google/schema.py` & `xsdata-23.5/tests/fixtures/docstrings/google/schema.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/fixtures/docstrings/numpy/schema.py` & `xsdata-23.5/tests/fixtures/docstrings/numpy/schema.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/fixtures/docstrings/rst/schema.py` & `xsdata-23.5/tests/fixtures/docstrings/rst/schema.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/fixtures/docstrings/schema.xsd` & `xsdata-23.5/tests/fixtures/docstrings/schema.xsd`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/fixtures/dtd/models/complete_example.py` & `xsdata-23.5/tests/fixtures/dtd/models/complete_example.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,23 +46,23 @@
     author: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
             "required": True,
         }
     )
-    origin: Optional[str] = field(
-        default=None,
+    origin: List[str] = field(
+        default_factory=list,
         metadata={
             "name": "Origin",
             "type": "Element",
         }
     )
-    source: Optional[str] = field(
-        default=None,
+    source: List[str] = field(
+        default_factory=list,
         metadata={
             "name": "Source",
             "type": "Element",
         }
     )
     title: Optional[str] = field(
         default=None,
```

### Comparing `xsdata-22.9/tests/fixtures/hello/hello.py` & `xsdata-23.5/tests/fixtures/hello/hello.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/fixtures/hello/hello.wsdl` & `xsdata-23.5/tests/fixtures/hello/hello.wsdl`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/fixtures/hello/hello.xsd` & `xsdata-23.5/tests/fixtures/hello/hello.xsd`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/fixtures/models.py` & `xsdata-23.5/tests/fixtures/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,14 +110,27 @@
                     "type": object,
                     "namespace": "http://www.w3.org/1999/xhtml",
                 },
             ),
         }
     )
 
+@dataclass
+class OptionalChoiceType:
+    a_or_b: Optional[object] = field(
+        metadata={
+            "type": "Elements",
+            "choices": (
+                {"name": "a", "type": TypeA},
+                {"name": "b", "type": TypeB},
+            ),
+        }
+    )
+
+
 
 @dataclass
 class UnionType:
     element: Union[TypeA, TypeB, TypeC, TypeD]
 
 
 @dataclass
@@ -137,21 +150,24 @@
     a0: Optional[str] = field(default=None, metadata=dict(type="Attribute"))
     a1: Dict[str, str] = field(default_factory=dict, metadata=dict(type="Attributes"))
     a2: List[str] = field(
         default_factory=list, metadata=dict(type="Attribute", tokens=True)
     )
     x0: Optional[int] = field(default=None)
     x1: List[int] = field(
-        default_factory=list, metadata=dict(type="Element", sequential=True)
+        default_factory=list, metadata=dict(type="Element", sequence=1)
     )
     x2: List[int] = field(
-        default_factory=list, metadata=dict(type="Element", sequential=True)
+        default_factory=list, metadata=dict(type="Element", sequence=1)
     )
     x3: List[int] = field(
-        default_factory=list, metadata=dict(type="Element", sequential=True)
+        default_factory=list, metadata=dict(type="Element", sequence=2)
+    )
+    x4: Optional[int] = field(
+        default=None, metadata=dict(type="Element", sequence=2)
     )
 
 
 @dataclass
 class Span:
     class Meta:
         name = "span"
```

### Comparing `xsdata-22.9/tests/fixtures/primer/order.py` & `xsdata-23.5/tests/fixtures/primer/order.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/fixtures/primer/order.xsd` & `xsdata-23.5/tests/fixtures/primer/order.xsd`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/fixtures/primer/sample.json` & `xsdata-23.5/tests/fixtures/primer/sample.json`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/fixtures/primer/sample.xml` & `xsdata-23.5/tests/fixtures/primer/sample.xml`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/fixtures/primer/sample.xsdata.xml` & `xsdata-23.5/tests/fixtures/primer/sample.xsdata.xml`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/fixtures/series/samples/show1.json` & `xsdata-23.5/tests/fixtures/series/samples/show1.json`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/fixtures/series/samples/show2.json` & `xsdata-23.5/tests/fixtures/series/samples/show2.json`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/fixtures/series/series.py` & `xsdata-23.5/tests/fixtures/series/series.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,20 +8,22 @@
     class Meta:
         name = "country"
 
     name: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
+            "required": True,
         }
     )
     code: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
+            "required": True,
         }
     )
     timezone: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
         }
@@ -33,123 +35,134 @@
     class Meta:
         name = "externals"
 
     tvrage: Optional[int] = field(
         default=None,
         metadata={
             "type": "Element",
+            "required": True,
         }
     )
     thetvdb: Optional[int] = field(
         default=None,
         metadata={
             "type": "Element",
         }
     )
     imdb: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
+            "required": True,
         }
     )
 
 
 @dataclass
 class Image:
     class Meta:
         name = "image"
 
     medium: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
+            "required": True,
         }
     )
     original: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
+            "required": True,
         }
     )
 
 
 @dataclass
 class Previousepisode:
     class Meta:
         name = "previousepisode"
 
     href: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
+            "required": True,
         }
     )
 
 
 @dataclass
 class Rating:
     class Meta:
         name = "rating"
 
     average: Optional[float] = field(
         default=None,
         metadata={
             "type": "Element",
+            "required": True,
         }
     )
 
 
 @dataclass
 class Schedule:
     class Meta:
         name = "schedule"
 
     time: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
+            "required": True,
         }
     )
     days: List[str] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "min_occurs": 1,
         }
     )
 
 
 @dataclass
 class Self:
     class Meta:
         name = "self"
 
     href: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
+            "required": True,
         }
     )
 
 
 @dataclass
 class Links:
     class Meta:
         name = "_links"
 
     self_value: Optional[Self] = field(
         default=None,
         metadata={
             "name": "self",
             "type": "Element",
+            "required": True,
         }
     )
     previousepisode: Optional[Previousepisode] = field(
         default=None,
         metadata={
             "type": "Element",
+            "required": True,
         }
     )
 
 
 @dataclass
 class Network:
     class Meta:
@@ -161,143 +174,160 @@
             "type": "Element",
         }
     )
     name: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
+            "required": True,
         }
     )
     country: Optional[Country] = field(
         default=None,
         metadata={
             "type": "Element",
+            "required": True,
         }
     )
 
 
 @dataclass
 class Series:
     class Meta:
         name = "series"
 
     id: Optional[int] = field(
         default=None,
         metadata={
             "type": "Element",
+            "required": True,
         }
     )
     url: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
         }
     )
     name: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
+            "required": True,
         }
     )
     type: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
+            "required": True,
         }
     )
     language: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
+            "required": True,
         }
     )
     genres: List[str] = field(
         default_factory=list,
         metadata={
             "type": "Element",
+            "min_occurs": 1,
         }
     )
     status: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
+            "required": True,
         }
     )
     runtime: Optional[int] = field(
         default=None,
         metadata={
             "type": "Element",
+            "required": True,
         }
     )
     premiered: Optional[XmlDate] = field(
         default=None,
         metadata={
             "type": "Element",
+            "required": True,
         }
     )
     official_site: Optional[str] = field(
         default=None,
         metadata={
             "name": "officialSite",
             "type": "Element",
+            "required": True,
         }
     )
     schedule: Optional[Schedule] = field(
         default=None,
         metadata={
             "type": "Element",
+            "required": True,
         }
     )
     rating: Optional[Rating] = field(
         default=None,
         metadata={
             "type": "Element",
+            "required": True,
         }
     )
     weight: Optional[int] = field(
         default=None,
         metadata={
             "type": "Element",
         }
     )
     network: Optional[Network] = field(
         default=None,
         metadata={
             "type": "Element",
+            "required": True,
         }
     )
     web_channel: Optional[object] = field(
         default=None,
         metadata={
             "name": "webChannel",
             "type": "Element",
         }
     )
     externals: Optional[Externals] = field(
         default=None,
         metadata={
             "type": "Element",
+            "required": True,
         }
     )
     image: Optional[Image] = field(
         default=None,
         metadata={
             "type": "Element",
         }
     )
     summary: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
+            "required": True,
         }
     )
     updated: Optional[int] = field(
         default=None,
         metadata={
             "type": "Element",
+            "required": True,
         }
     )
     links: Optional[Links] = field(
         default=None,
         metadata={
             "name": "_links",
             "type": "Element",
```

### Comparing `xsdata-22.9/tests/fixtures/stripe/.xsdata.xml` & `xsdata-23.5/tests/fixtures/stripe/.xsdata.xml`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/fixtures/stripe/models/balance.py` & `xsdata-23.5/tests/fixtures/stripe/models/balance.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,122 +7,137 @@
     class Meta:
         name = "connect_reserved"
 
     amount: Optional[int] = field(
         default=None,
         metadata={
             "type": "Element",
+            "required": True,
         }
     )
     currency: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
+            "required": True,
         }
     )
 
 
 @dataclass(order=True, frozen=True)
 class SourceTypes:
     class Meta:
         name = "source_types"
 
     bank_account: Optional[int] = field(
         default=None,
         metadata={
             "type": "Element",
+            "required": True,
         }
     )
     card: Optional[int] = field(
         default=None,
         metadata={
             "type": "Element",
+            "required": True,
         }
     )
 
 
 @dataclass(order=True, frozen=True)
 class Available:
     class Meta:
         name = "available"
 
     amount: Optional[int] = field(
         default=None,
         metadata={
             "type": "Element",
+            "required": True,
         }
     )
     currency: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
+            "required": True,
         }
     )
     source_types: Optional[SourceTypes] = field(
         default=None,
         metadata={
             "type": "Element",
+            "required": True,
         }
     )
 
 
 @dataclass(order=True, frozen=True)
 class Pending:
     class Meta:
         name = "pending"
 
     amount: Optional[int] = field(
         default=None,
         metadata={
             "type": "Element",
+            "required": True,
         }
     )
     currency: Optional[str] = field(
         default=None,
         metadata={
             "type": "Element",
+            "required": True,
         }
     )
     source_types: Optional[SourceTypes] = field(
         default=None,
         metadata={
             "type": "Element",
+            "required": True,
         }
     )
 
 
 @dataclass(order=True, frozen=True)
 class Balance:
     class Meta:
         name = "balance"
 
     object_value: Optional[str] = field(
         default=None,
         metadata={
             "name": "object",
             "type": "Element",
+            "required": True,
         }
     )
     available: Tuple[Available, ...] = field(
         default_factory=tuple,
         metadata={
             "type": "Element",
+            "min_occurs": 1,
         }
     )
     connect_reserved: Tuple[ConnectReserved, ...] = field(
         default_factory=tuple,
         metadata={
             "type": "Element",
+            "min_occurs": 1,
         }
     )
     livemode: Optional[bool] = field(
         default=None,
         metadata={
             "type": "Element",
+            "required": True,
         }
     )
     pending: Tuple[Pending, ...] = field(
         default_factory=tuple,
         metadata={
             "type": "Element",
+            "min_occurs": 1,
         }
     )
```

### Comparing `xsdata-22.9/tests/fixtures/stripe/samples/balance.json` & `xsdata-23.5/tests/fixtures/stripe/samples/balance.json`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/formats/dataclass/models/test_builders.py` & `xsdata-23.5/tests/formats/dataclass/models/test_builders.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from dataclasses import field
 from dataclasses import fields
 from dataclasses import make_dataclass
 from typing import Dict
 from typing import get_type_hints
 from typing import Iterator
 from typing import List
+from typing import Tuple
 from typing import Union
 from unittest import mock
 from unittest import TestCase
 from xml.etree.ElementTree import QName
 
 from tests.fixtures.artists import Artist
 from tests.fixtures.books import BookForm
@@ -23,14 +24,15 @@
 from tests.fixtures.models import UnionType
 from tests.fixtures.series import Country
 from tests.fixtures.submodels import ChoiceTypeChild
 from xsdata.exceptions import XmlContextError
 from xsdata.formats.dataclass.compat import class_types
 from xsdata.formats.dataclass.models.builders import XmlMetaBuilder
 from xsdata.formats.dataclass.models.builders import XmlVarBuilder
+from xsdata.formats.dataclass.models.elements import XmlMeta
 from xsdata.formats.dataclass.models.elements import XmlType
 from xsdata.models.datatype import XmlDate
 from xsdata.utils import text
 from xsdata.utils.constants import return_input
 from xsdata.utils.constants import return_true
 from xsdata.utils.namespaces import build_qname
 from xsdata.utils.testing import FactoryTestCase
@@ -99,14 +101,51 @@
 
         result = self.builder.build(Foo, None)
         self.assertEqual("Foo", result.qname)
 
         result = self.builder.build(Thug, None)
         self.assertEqual("thug", result.qname)
 
+    def test_wrapper(self):
+        @dataclass
+        class PrimitiveType:
+            attr: str = field(metadata={"wrapper": "Items"})
+
+        @dataclass
+        class UnionType:
+            attr: Union[str, int] = field(metadata={"wrapper": "Items"})
+
+        @dataclass
+        class UnionCollection:
+            union_collection: List[Union[str, int]] = field(
+                metadata={"wrapper": "Items"}
+            )
+
+        @dataclass
+        class ListType:
+            attr: List[str] = field(metadata={"wrapper": "Items"})
+
+        @dataclass
+        class TupleType:
+            attr: Tuple[str, ...] = field(metadata={"wrapper": "Items"})
+
+        # @dataclass
+        # class SetType:
+        #     attr: Set[str] = field(metadata={"wrapper": "Items"})
+
+        with self.assertRaises(XmlContextError):
+            self.builder.build(PrimitiveType, None)
+        with self.assertRaises(XmlContextError):
+            self.builder.build(UnionType, None)
+
+        self.assertIsInstance(self.builder.build(ListType, None), XmlMeta)
+        self.assertIsInstance(self.builder.build(TupleType, None), XmlMeta)
+        # not supported by analyze_types
+        # self.assertIsInstance(self.builder.build(SetType, None), XmlMeta)
+
     def test_build_with_no_dataclass_raises_exception(self, *args):
         with self.assertRaises(XmlContextError) as cm:
             self.builder.build(int, None)
 
         self.assertEqual(f"Type '{int}' is not a dataclass.", str(cm.exception))
 
     def test_build_locates_globalns_per_field(self):
@@ -270,135 +309,135 @@
     def test_build_with_choice_field(self):
         globalns = sys.modules[ChoiceType.__module__].__dict__
         type_hints = get_type_hints(ChoiceType)
         class_field = fields(ChoiceType)[0]
 
         self.maxDiff = None
         actual = self.builder.build(
-            66,
             "choice",
             type_hints["choice"],
             class_field.metadata,
             True,
             "bar",
             list,
             globalns,
         )
         expected = XmlVarFactory.create(
-            index=67,
+            index=1,
             name="choice",
             types=(object,),
             factory=list,
             any_type=True,
             default=list,
             xml_type=XmlType.ELEMENTS,
             elements={
                 "{bar}a": XmlVarFactory.create(
-                    index=1,
+                    index=2,
                     name="choice",
                     qname="{bar}a",
                     types=(TypeA,),
                     clazz=TypeA,
                     factory=list,
                     namespaces=("bar",),
                 ),
                 "{bar}b": XmlVarFactory.create(
-                    index=2,
+                    index=3,
                     name="choice",
                     qname="{bar}b",
                     types=(TypeB,),
                     clazz=TypeB,
                     factory=list,
                     namespaces=("bar",),
                 ),
                 "{bar}int": XmlVarFactory.create(
-                    index=3,
+                    index=4,
                     name="choice",
                     qname="{bar}int",
                     types=(int,),
                     factory=list,
                     namespaces=("bar",),
                 ),
                 "{bar}int2": XmlVarFactory.create(
-                    index=4,
+                    index=5,
                     name="choice",
                     qname="{bar}int2",
                     types=(int,),
                     derived=True,
                     nillable=True,
                     factory=list,
                     namespaces=("bar",),
                 ),
                 "{bar}float": XmlVarFactory.create(
-                    index=5,
+                    index=6,
                     name="choice",
                     qname="{bar}float",
                     types=(float,),
                     factory=list,
                     namespaces=("bar",),
                 ),
                 "{bar}qname": XmlVarFactory.create(
-                    index=6,
+                    index=7,
                     name="choice",
                     qname="{bar}qname",
                     types=(QName,),
                     factory=list,
                     namespaces=("bar",),
                 ),
                 "{bar}tokens": XmlVarFactory.create(
-                    index=7,
+                    index=8,
                     name="choice",
                     qname="{bar}tokens",
                     types=(int,),
                     tokens_factory=list,
                     derived=True,
                     factory=list,
                     default=return_true,
                     namespaces=("bar",),
                 ),
                 "{foo}union": XmlVarFactory.create(
-                    index=8,
+                    index=9,
                     name="choice",
                     qname="{foo}union",
                     types=(UnionType,),
                     clazz=UnionType,
                     factory=list,
                     namespaces=("foo",),
                 ),
                 "{bar}p": XmlVarFactory.create(
-                    index=9,
+                    index=10,
                     name="choice",
                     qname="{bar}p",
                     types=(float,),
                     derived=True,
                     factory=list,
                     default=1.1,
                     namespaces=("bar",),
                 ),
             },
             wildcards=[
                 XmlVarFactory.create(
-                    index=10,
+                    index=11,
                     name="choice",
                     xml_type=XmlType.WILDCARD,
                     qname="{http://www.w3.org/1999/xhtml}any",
                     types=(object,),
                     factory=list,
                     default=None,
                     namespaces=("http://www.w3.org/1999/xhtml",),
                 ),
             ],
         )
 
+        self.maxDiff = None
         self.assertEqual(expected, actual)
 
     def test_build_validates_result(self):
         with self.assertRaises(XmlContextError) as cm:
             self.builder.build(
-                1, "foo", List[int], {"type": "Attributes"}, True, None, None, None
+                "foo", List[int], {"type": "Attributes"}, True, None, None, None
             )
 
         self.assertEqual(
             "Xml type 'Attributes' does not support typing: typing.List[int]",
             str(cm.exception),
         )
```

### Comparing `xsdata-22.9/tests/formats/dataclass/parsers/handlers/test_lxml.py` & `xsdata-23.5/tests/formats/dataclass/parsers/handlers/test_lxml.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/formats/dataclass/parsers/handlers/test_native.py` & `xsdata-23.5/tests/formats/dataclass/parsers/handlers/test_native.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/formats/dataclass/parsers/nodes/test_element.py` & `xsdata-23.5/tests/formats/dataclass/parsers/nodes/test_element.py`

 * *Files 2% similar despite different names*

```diff
@@ -397,14 +397,43 @@
         self.assertEqual(10, actual.position)
         self.assertEqual(DerivedElement, actual.derived_factory)
         self.assertIs(mock_ctx_fetch.return_value, actual.meta)
 
         mock_xsi_type.assert_called_once_with(attrs, ns_map)
         mock_ctx_fetch.assert_called_once_with(var.clazz, namespace, xsi_type)
 
+    @mock.patch.object(ParserUtils, "xsi_type", return_value="foo")
+    @mock.patch.object(XmlContext, "fetch")
+    def test_build_node_with_dataclass_var_and_mismatch_xsi_type(
+        self, mock_ctx_fetch, mock_xsi_type
+    ):
+        var = XmlVarFactory.create(
+            xml_type=XmlType.ELEMENT,
+            name="a",
+            qname="a",
+            types=(TypeB,),
+            derived=False,
+        )
+        xsi_type = "foo"
+        namespace = self.meta.namespace
+        mock_ctx_fetch.return_value = self.meta
+        mock_xsi_type.return_value = xsi_type
+
+        attrs = {"a": "b"}
+        ns_map = {"ns0": "xsdata"}
+        actual = self.node.build_node(var, attrs, ns_map, 10)
+
+        self.assertIsInstance(actual, ElementNode)
+        self.assertEqual(10, actual.position)
+        self.assertEqual(DerivedElement, actual.derived_factory)
+        self.assertIs(mock_ctx_fetch.return_value, actual.meta)
+
+        mock_xsi_type.assert_called_once_with(attrs, ns_map)
+        mock_ctx_fetch.assert_called_once_with(var.clazz, namespace, xsi_type)
+
     @mock.patch.object(XmlContext, "fetch")
     def test_build_node_with_dataclass_var_validates_nillable(self, mock_ctx_fetch):
         var = XmlVarFactory.create(xml_type=XmlType.ELEMENT, qname="a", types=(TypeC,))
         ns_map = {}
         nillable_meta = copy.deepcopy(self.meta)
         nillable_meta.nillable = True
         mock_ctx_fetch.side_effect = [self.meta, self.meta, nillable_meta]
@@ -504,7 +533,8 @@
         attrs = {"a": "b"}
         ns_map = {"ns0": "xsdata"}
         actual = self.node.build_node(var, attrs, ns_map, 10)
 
         self.assertIsInstance(actual, PrimitiveNode)
         self.assertEqual(ns_map, actual.ns_map)
         self.assertEqual(var, actual.var)
+        self.assertEqual(self.node.meta.mixed_content, actual.mixed)
```

### Comparing `xsdata-22.9/tests/formats/dataclass/parsers/nodes/test_primitive.py` & `xsdata-23.5/tests/formats/dataclass/parsers/nodes/test_primitive.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     @mock.patch.object(ParserUtils, "parse_value")
     def test_bind(self, mock_parse_value):
         mock_parse_value.return_value = 13
         var = XmlVarFactory.create(
             xml_type=XmlType.TEXT, name="foo", qname="foo", types=(int,), format="Nope"
         )
         ns_map = {"foo": "bar"}
-        node = PrimitiveNode(var, ns_map, DerivedElement)
+        node = PrimitiveNode(var, ns_map, False, DerivedElement)
         objects = []
 
         self.assertTrue(node.bind("foo", "13", "Impossible", objects))
         self.assertEqual(("foo", 13), objects[-1])
 
         mock_parse_value.assert_called_once_with(
             value="13",
@@ -33,34 +33,55 @@
         )
 
     def test_bind_derived_mode(self):
         var = XmlVarFactory.create(
             xml_type=XmlType.TEXT, name="foo", qname="foo", types=(int,), derived=True
         )
         ns_map = {"foo": "bar"}
-        node = PrimitiveNode(var, ns_map, DerivedElement)
+        node = PrimitiveNode(var, ns_map, False, DerivedElement)
         objects = []
 
         self.assertTrue(node.bind("foo", "13", "Impossible", objects))
         self.assertEqual(DerivedElement("foo", 13), objects[-1][1])
 
     def test_bind_nillable_content(self):
         var = XmlVarFactory.create(
             xml_type=XmlType.TEXT, name="foo", qname="foo", types=(str,), nillable=False
         )
         ns_map = {"foo": "bar"}
-        node = PrimitiveNode(var, ns_map, DerivedElement)
+        node = PrimitiveNode(var, ns_map, False, DerivedElement)
         objects = []
 
         self.assertTrue(node.bind("foo", None, None, objects))
         self.assertEqual("", objects[-1][1])
 
         var.nillable = True
         self.assertTrue(node.bind("foo", None, None, objects))
         self.assertIsNone(objects[-1][1])
 
+    def test_bind_mixed_with_tail_content(self):
+        var = XmlVarFactory.create(
+            xml_type=XmlType.TEXT, name="foo", types=(int,), derived=True
+        )
+        node = PrimitiveNode(var, {}, True, DerivedElement)
+        objects = []
+
+        self.assertTrue(node.bind("foo", "13", "tail", objects))
+        self.assertEqual((None, "tail"), objects[-1])
+        self.assertEqual(DerivedElement("foo", 13), objects[-2][1])
+
+    def test_bind_mixed_without_tail_content(self):
+        var = XmlVarFactory.create(
+            xml_type=XmlType.TEXT, name="foo", types=(int,), derived=True
+        )
+        node = PrimitiveNode(var, {}, True, DerivedElement)
+        objects = []
+
+        self.assertTrue(node.bind("foo", "13", "", objects))
+        self.assertEqual(DerivedElement("foo", 13), objects[-1][1])
+
     def test_child(self):
         var = XmlVarFactory.create(xml_type=XmlType.TEXT, name="foo", qname="foo")
-        node = PrimitiveNode(var, {}, DerivedElement)
+        node = PrimitiveNode(var, {}, False, DerivedElement)
 
         with self.assertRaises(XmlContextError):
             node.child("foo", {}, {}, 0)
```

### Comparing `xsdata-22.9/tests/formats/dataclass/parsers/nodes/test_standard.py` & `xsdata-23.5/tests/formats/dataclass/parsers/nodes/test_standard.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/formats/dataclass/parsers/nodes/test_union.py` & `xsdata-23.5/tests/formats/dataclass/parsers/nodes/test_union.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/formats/dataclass/parsers/nodes/test_wildcard.py` & `xsdata-23.5/tests/formats/dataclass/parsers/nodes/test_wildcard.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/formats/dataclass/parsers/test_json.py` & `xsdata-23.5/tests/formats/dataclass/parsers/test_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from tests.fixtures.books import BookForm
 from tests.fixtures.books import Books
 from tests.fixtures.models import AttrsType
 from tests.fixtures.models import BaseC
 from tests.fixtures.models import BaseType
 from tests.fixtures.models import ChoiceType
 from tests.fixtures.models import ExtendedType
+from tests.fixtures.models import OptionalChoiceType
 from tests.fixtures.models import TypeA
 from tests.fixtures.models import TypeB
 from tests.fixtures.models import TypeC
 from tests.fixtures.models import TypeD
 from tests.fixtures.models import UnionType
 from xsdata.exceptions import ParserError
 from xsdata.formats.dataclass.models.generics import AnyElement
@@ -131,15 +132,14 @@
                 f"Invalid clazz argument: {Optional[ChoiceType]}",
             ),
             ("[]", List[int], f"Invalid clazz argument: {List[int]}"),
             ("[]", List, f"Invalid clazz argument: {List}"),
         ]
 
         for json_string, clazz, exc_msg in invalid_cases:
-
             with self.assertRaises(ParserError) as cm:
                 self.parser.from_string(json_string, clazz=clazz)
 
             self.assertEqual(exc_msg, str(cm.exception))
 
     def test_bind_dataclass_with_unknown_property(self):
         data = {"unknown": True}
@@ -262,14 +262,19 @@
             self.parser.bind_dataclass(data, ChoiceType)
 
         self.assertEqual(
             "Failed to bind '!NotAQname' to ChoiceType.choice field",
             str(cm.exception),
         )
 
+    def test_bind_simple_type_with_optional_elements_var(self):
+        data = {"a_or_b": None}
+        actual = self.parser.bind_dataclass(data, OptionalChoiceType)
+        self.assertIsNone(None, actual.a_or_b)
+
     def test_bind_any_element(self):
         data = {
             "wildcard": {
                 "qname": "a",
                 "text": 1,
                 "tail": None,
                 "children": [],
@@ -322,15 +327,14 @@
 
         self.assertEqual(
             "Unable to locate compound element ChoiceType.choice[nope]",
             str(cm.exception),
         )
 
     def test_bind_wildcard_dataclass(self):
-
         data = {"a": None, "wildcard": {"x": 1}}
         expected = ExtendedType(wildcard=TypeA(x=1))
         self.assertEqual(expected, self.parser.bind_dataclass(data, ExtendedType))
 
     def test_bind_wildcard_with_derived_dataclass(self):
         data = {
             "wildcard": {
```

### Comparing `xsdata-22.9/tests/formats/dataclass/parsers/test_mixins.py` & `xsdata-23.5/tests/formats/dataclass/parsers/test_mixins.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,12 +26,11 @@
         self.parser = RecordParser(handler=EventsHandler)
 
     def test_parse(self):
         self.assertEqual(books, self.parser.parse(events, Books))
         self.assertEqual({"brk": "urn:books"}, self.parser.ns_map)
 
     def test_parse_with_unhandled_event(self):
-
         with self.assertRaises(XmlHandlerError) as cm:
             self.parser.parse([("reverse", "")], Books)
 
         self.assertEqual("Unhandled event: `reverse`.", str(cm.exception))
```

### Comparing `xsdata-22.9/tests/formats/dataclass/parsers/test_node.py` & `xsdata-23.5/tests/formats/dataclass/parsers/test_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
     def test_start_with_any_type_root(self):
         parser = self.parser
         queue = []
         objects = []
 
         attrs = {QNames.XSI_TYPE: "bk:books"}
         ns_map = {"bk": "urn:books", "xsi": Namespace.XSI.uri}
-        parser.start(None, queue, objects, "doc", attrs, ns_map)
+        parser.start(None, queue, objects, "whatever", attrs, ns_map)
         actual = queue[0]
 
         self.assertEqual(1, len(queue))
         self.assertEqual(0, actual.position)
         self.assertEqual(self.parser.context, actual.context)
         self.assertEqual(self.parser.context.build(Books), actual.meta)
         self.assertEqual(self.parser.config, actual.config)
@@ -180,15 +180,15 @@
 
     @mock.patch.object(PrimitiveNode, "bind", return_value=True)
     def test_end(self, mock_assemble):
         parser = NodeParser()
         objects = [("q", "result")]
         queue = []
         var = XmlVarFactory.create(xml_type=XmlType.TEXT, name="foo", qname="foo")
-        queue.append(PrimitiveNode(var, ns_map={}, derived_factory=DerivedElement))
+        queue.append(PrimitiveNode(var, {}, False, DerivedElement))
 
         self.assertTrue(parser.end(queue, objects, "author", "foobar", None))
         self.assertEqual(0, len(queue))
         self.assertEqual(("q", "result"), objects[-1])
         mock_assemble.assert_called_once_with("author", "foobar", None, objects)
 
     def test_end_with_no_result(self):
```

### Comparing `xsdata-22.9/tests/formats/dataclass/parsers/test_tree.py` & `xsdata-23.5/tests/formats/dataclass/parsers/test_tree.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/formats/dataclass/parsers/test_utils.py` & `xsdata-23.5/tests/formats/dataclass/parsers/test_utils.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/formats/dataclass/parsers/test_xml.py` & `xsdata-23.5/tests/formats/dataclass/parsers/test_xml.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         )
 
     @mock.patch.object(UserXmlParser, "emit_event")
     def test_end(self, mock_emit_event):
         objects = []
         queue = []
         var = XmlVarFactory.create(xml_type=XmlType.TEXT, name="foo", types=(bool,))
-        queue.append(PrimitiveNode(var, {}, None))
+        queue.append(PrimitiveNode(var, {}, False, None))
 
         result = self.parser.end(queue, objects, "enabled", "true", None)
         self.assertTrue(result)
         self.assertEqual(0, len(queue))
         self.assertEqual(("enabled", True), objects[-1])
         mock_emit_event.assert_called_once_with(EventType.END, "enabled", obj=result)
```

### Comparing `xsdata-22.9/tests/formats/dataclass/serializers/test_code.py` & `xsdata-23.5/tests/formats/dataclass/serializers/test_code.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from unittest import TestCase
 
+from tests.fixtures.books import BookForm
+from tests.fixtures.books import Books
 from tests.fixtures.books.fixtures import books
 from xsdata.formats.dataclass.serializers import PycodeSerializer
 from xsdata.models.enums import Namespace
 
 
 class PycodeSerializerTests(TestCase):
     def setUp(self) -> None:
@@ -40,14 +42,32 @@
             "        ),\n"
             "    ]\n"
             ")\n"
         )
 
         self.assertEqual(expected, result)
 
+    def test_write_class_with_default_values(self):
+        books = Books(book=[BookForm(author="me")])
+        result = self.serializer.render(books, var_name="books")
+        expected = (
+            "from tests.fixtures.books.books import BookForm\n"
+            "from tests.fixtures.books.books import Books\n"
+            "\n"
+            "\n"
+            "books = Books(\n"
+            "    book=[\n"
+            "        BookForm(\n"
+            '            author="me"\n'
+            "        ),\n"
+            "    ]\n"
+            ")\n"
+        )
+        self.assertEqual(expected, result)
+
     def test_write_object_with_empty_array(self):
         iterator = self.serializer.write_object([], 0, set())
         self.assertEqual("[]", "".join(iterator))
 
         iterator = self.serializer.write_object((), 0, set())
         self.assertEqual("()", "".join(iterator))
 
@@ -60,7 +80,14 @@
 
         iterator = self.serializer.write_object({"foo": "bar"}, 0, set())
         self.assertEqual('{\n    "foo": "bar",\n}', "".join(iterator))
 
     def test_write_object_with_enum(self):
         iterator = self.serializer.write_object(Namespace.SOAP11, 0, set())
         self.assertEqual("Namespace.SOAP11", "".join(iterator))
+
+    def test_build_imports_ignores_nested_types(self):
+        class Foo:
+            pass
+
+        actual = self.serializer.build_imports({Foo})
+        self.assertEqual("", actual)
```

### Comparing `xsdata-22.9/tests/formats/dataclass/serializers/test_json.py` & `xsdata-23.5/tests/formats/dataclass/serializers/test_json.py`

 * *Files 15% similar despite different names*

```diff
@@ -134,7 +134,40 @@
         ]
         self.assertEqual(expected, actual)
 
         serializer.config.ignore_default_attributes = True
         expected = expected[:-1]
         actual = [name for name, value in serializer.next_value(book)]
         self.assertEqual(expected, actual)
+
+    def test_pretty_print_indent(self):
+        serializer = JsonSerializer()
+        serializer.config.pretty_print = True
+        serializer.config.pretty_print_indent = "    "
+
+        actual = serializer.render(self.books)
+        expected = f"""{{
+    "book": [
+        {{
+            "author": "{self.expected["book"][0]["author"]}",
+            "title": "{self.expected["book"][0]["title"]}",
+            "genre": "{self.expected["book"][0]["genre"]}",
+            "price": {self.expected["book"][0]["price"]},
+            "pub_date": "{self.expected["book"][0]["pub_date"]}",
+            "review": "{self.expected["book"][0]["review"]}",
+            "id": "{self.expected["book"][0]["id"]}",
+            "lang": "en"
+        }},
+        {{
+            "author": "{self.expected["book"][1]["author"]}",
+            "title": "{self.expected["book"][1]["title"]}",
+            "genre": "{self.expected["book"][1]["genre"]}",
+            "price": null,
+            "pub_date": null,
+            "review": "{self.expected["book"][1]["review"]}",
+            "id": "{self.expected["book"][1]["id"]}",
+            "lang": "en"
+        }}
+    ]
+}}"""
+
+        self.assertEqual(expected, actual)
```

### Comparing `xsdata-22.9/tests/formats/dataclass/serializers/test_mixins.py` & `xsdata-23.5/tests/formats/dataclass/serializers/test_mixins.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from xsdata.formats.dataclass.serializers.mixins import XmlWriter
 from xsdata.formats.dataclass.serializers.mixins import XmlWriterEvent
 from xsdata.models.enums import DataType
 from xsdata.models.enums import QNames
 
 
 class XmlWriterImpl(XmlWriter):
-
     __slots__ = ()
 
     def __init__(self, config: SerializerConfig, output: TextIO, ns_map: Dict):
         super().__init__(config, output, ns_map)
 
         self.handler = XMLGenerator(
             self.output,
```

### Comparing `xsdata-22.9/tests/formats/dataclass/serializers/test_xml.py` & `xsdata-23.5/tests/formats/dataclass/serializers/test_xml.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,13 @@
+import re
+from dataclasses import dataclass
+from dataclasses import field
 from dataclasses import make_dataclass
 from typing import Generator
+from typing import List
 from unittest import TestCase
 from xml.etree.ElementTree import QName
 
 from tests.fixtures.books import BookForm
 from tests.fixtures.datatypes import Telephone
 from tests.fixtures.models import Paragraph
 from tests.fixtures.models import SequentialType
@@ -21,14 +25,66 @@
 from xsdata.utils.testing import XmlVarFactory
 
 
 class XmlSerializerTests(TestCase):
     def setUp(self) -> None:
         self.serializer = XmlSerializer()
 
+    def test_wrapper_primitive(self):
+        @dataclass
+        class PrimitiveWrapper:
+            primitive_list: List[str] = field(
+                metadata={
+                    "wrapper": "PrimitiveList",
+                    "type": "Element",
+                    "name": "Value",
+                }
+            )
+
+        obj = PrimitiveWrapper(primitive_list=["Value 1", "Value 2"])
+        xml = self.serializer.render(obj)
+        expected = r"<PrimitiveWrapper><PrimitiveList><Value>Value 1</Value><Value>Value 2</Value></PrimitiveList></PrimitiveWrapper>"
+        self.assertIsNotNone(re.search(expected, xml))
+
+    def test_wrapper_element(self):
+        @dataclass
+        class ElementObject:
+            content: str = field(metadata={"type": "Element"})
+
+        @dataclass
+        class ElementWrapper:
+            elements: List[ElementObject] = field(
+                metadata={"wrapper": "Elements", "type": "Element", "name": "Object"}
+            )
+
+        obj = ElementWrapper(
+            elements=[ElementObject(content="Hello"), ElementObject(content="World")]
+        )
+        xml = self.serializer.render(obj)
+        expected = "<ElementWrapper><Elements><Object><content>Hello</content></Object><Object><content>World</content></Object></Elements></ElementWrapper>"
+        self.assertIsNotNone(re.search(expected, xml))
+
+    def test_wrapper_namespace(self):
+        @dataclass
+        class NamespaceWrapper:
+            items: List[str] = field(
+                metadata={
+                    "wrapper": "Items",
+                    "type": "Element",
+                    "name": "item",
+                    "namespace": "ns",
+                }
+            )
+
+        ns_map = {"foo": "ns"}
+        obj = NamespaceWrapper(items=["a", "b"])
+        xml = self.serializer.render(obj, ns_map=ns_map)
+        expected = '<NamespaceWrapper xmlns:foo="ns"><foo:Items><foo:item>a</foo:item><foo:item>b</foo:item></foo:Items></NamespaceWrapper>'
+        self.assertIsNotNone(re.search(expected, xml))
+
     def test_write_object_with_derived_element(self):
         book = BookForm(id="123")
         obj = DerivedElement(qname="item", value=book)
 
         result = self.serializer.write_object(obj)
         expected = [
             (XmlWriterEvent.START, "item"),
@@ -510,30 +566,32 @@
         ]
 
         result = self.serializer.write_value(value, var, "xsdata")
         self.assertIsInstance(result, Generator)
         self.assertEqual(expected, list(result))
 
     def test_next_value(self):
-        obj = SequentialType(x0=1, x1=[2, 3, 4, None], x2=[6, 7], x3=[9])
+        obj = SequentialType(x0=1, x1=[2, 3, 4, None], x2=[6, 7], x3=[9], x4=10)
         meta = self.serializer.context.build(SequentialType)
         x0 = meta.text
         x1 = next(meta.find_children("x1"))
         x2 = next(meta.find_children("x2"))
         x3 = next(meta.find_children("x3"))
+        x4 = next(meta.find_children("x4"))
 
         actual = self.serializer.next_value(obj, meta)
         expected = [
             (x0, 1),
             (x1, 2),
             (x2, 6),
-            (x3, 9),
             (x1, 3),
             (x2, 7),
             (x1, 4),
+            (x3, 9),
+            (x4, 10),
         ]
 
         self.assertIsInstance(actual, Generator)
         self.assertEqual(expected, list(actual))
 
     def test_next_attribute(self):
         obj = SequentialType(a0="foo", a1={"b": "c", "d": "e"})
@@ -566,15 +624,14 @@
             ("d", "e"),
         ]
 
         self.assertIsInstance(actual, Generator)
         self.assertEqual(expected, list(actual))
 
     def test_render_mixed_content(self):
-
         obj = Paragraph()
         obj.content.append(AnyElement(qname="b", text="Mr."))
         obj.content.append(Span("chris"))
         obj.content.append("!")
 
         self.serializer.pretty_print = False
         result = self.serializer.render(obj).splitlines()
```

### Comparing `xsdata-22.9/tests/formats/dataclass/serializers/writers/test_lxml.py` & `xsdata-23.5/tests/formats/dataclass/serializers/writers/test_lxml.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,7 +53,16 @@
         self.serializer.config.pretty_print = False
         actual = self.serializer.render(books)
         expected = fixtures_dir.joinpath("books/books_auto_ns.xml").read_text()
 
         _, actual = actual.split("\n", 1)
         _, expected = expected.split("\n", 1)
         self.assertEqual(expected.replace("  ", "").replace("\n", ""), actual)
+
+    def test_pretty_print_indent(self):
+        self.serializer.config.pretty_print_indent = "    "
+        actual = self.serializer.render(books)
+        expected = fixtures_dir.joinpath("books/books_auto_ns.xml").read_text()
+
+        _, actual = actual.split("\n", 1)
+        _, expected = expected.split("\n", 1)
+        self.assertEqual(expected.replace("  ", "    "), actual)
```

### Comparing `xsdata-22.9/tests/formats/dataclass/serializers/writers/test_native.py` & `xsdata-23.5/tests/formats/dataclass/serializers/writers/test_native.py`

 * *Files 10% similar despite different names*

```diff
@@ -47,7 +47,16 @@
         self.serializer.config.pretty_print = False
         actual = self.serializer.render(books)
         expected = fixtures_dir.joinpath("books/books_auto_ns.xml").read_text()
 
         _, actual = actual.split("\n", 1)
         _, expected = expected.split("\n", 1)
         self.assertEqual(expected.replace("  ", "").replace("\n", ""), actual)
+
+    def test_pretty_print_indent(self):
+        self.serializer.config.pretty_print_indent = "    "
+        actual = self.serializer.render(books)
+        expected = fixtures_dir.joinpath("books/books_auto_ns.xml").read_text()
+
+        _, actual = actual.split("\n", 1)
+        _, expected = expected.split("\n", 1)
+        self.assertEqual(expected.replace("  ", "    "), actual)
```

### Comparing `xsdata-22.9/tests/formats/dataclass/test_client.py` & `xsdata-23.5/tests/formats/dataclass/test_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from unittest import mock
 from unittest import TestCase
 
 from tests.fixtures.calculator import Add
 from tests.fixtures.calculator import CalculatorSoapAdd
 from tests.fixtures.calculator import CalculatorSoapAddInput
 from tests.fixtures.calculator import CalculatorSoapAddOutput
+from tests.fixtures.hello import HelloGetHelloAsString
 from xsdata.exceptions import ClientValueError
 from xsdata.formats.dataclass.client import Client
 from xsdata.formats.dataclass.client import Config
 from xsdata.formats.dataclass.client import TransportTypes
 from xsdata.formats.dataclass.transports import DefaultTransport
 
 response = """
@@ -33,14 +34,15 @@
         expected = {
             "style": "document",
             "input": CalculatorSoapAddInput,
             "location": "http://testurl.com",
             "soap_action": "http://tempuri.org/Add",
             "output": CalculatorSoapAddOutput,
             "transport": "http://schemas.xmlsoap.org/soap/http",
+            "encoding": None,
         }
 
         self.assertEqual(expected, actual)
 
     @mock.patch.object(DefaultTransport, "post")
     def test_send_with_dict_params(self, mock_post):
         mock_post.return_value = response.encode()
@@ -84,14 +86,21 @@
             data=request,
             headers={
                 "content-type": "text/xml",
                 "SOAPAction": "http://tempuri.org/Add",
             },
         )
 
+    def test_prepare_payload_with_encoding(self):
+        client = Client.from_service(HelloGetHelloAsString, encoding="utf-8")
+        result = client.prepare_payload(
+            {"Body": {"getHelloAsString": {"arg0": "Χριστόδουλος"}}}
+        )
+        self.assertIn("Χριστόδουλος".encode(), result)
+
     def test_prepare_payload_raises_error_with_type_mismatch(self):
         client = Client.from_service(CalculatorSoapAdd)
 
         with self.assertRaises(ClientValueError) as cm:
             client.prepare_payload(CalculatorSoapAddOutput())
 
         self.assertEqual(
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `xsdata-22.9/tests/formats/dataclass/test_compat.py` & `xsdata-23.5/tests/formats/dataclass/test_compat.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/formats/dataclass/test_context.py` & `xsdata-23.5/tests/formats/dataclass/test_context.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/formats/dataclass/test_elements.py` & `xsdata-23.5/tests/formats/dataclass/test_elements.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,14 +165,15 @@
             "nillable=False, "
             "text=None, "
             "choices=[], "
             "elements={}, "
             "wildcards=[], "
             "attributes={}, "
             "any_attributes=[], "
+            "wrappers={}, "
             "namespace=None, "
             "mixed_content=False)"
         )
         self.assertEqual(expected, repr(self.meta))
 
     def test_property_element_types(self):
         meta = self.context.build(UnionType)
```

### Comparing `xsdata-22.9/tests/formats/dataclass/test_filters.py` & `xsdata-23.5/tests/formats/dataclass/test_filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,20 @@
 
         attr = AttrFactory.create(types=[AttrTypeFactory.create(qname="foo")])
         self.assertEqual("Foo", self.filters.constant_value(attr))
 
         attr = AttrFactory.create(types=[AttrTypeFactory.create(alias="alias")])
         self.assertEqual("Alias", self.filters.constant_value(attr))
 
+    def test_apply_substitutions_with_regexes(self):
+        self.filters.substitutions[ObjectType.CLASS]["(.*)Class"] = "\\1Type"
+
+        actual = self.filters.apply_substitutions("FooClass", ObjectType.CLASS)
+        self.assertEqual("FooType", actual)
+
     @mock.patch.object(Filters, "field_default_value")
     def test_field_definition(self, mock_field_default_value):
         mock_field_default_value.side_effect = [1, False]
         attr = AttrFactory.native(DataType.INT)
 
         result = self.filters.field_definition(attr, {}, None, ["Root"])
         expected = (
@@ -135,14 +141,30 @@
             '            "name": "attr_B",\n'
             '            "type": "Element",\n'
             "        }\n"
             "    )"
         )
         self.assertEqual(expected, result)
 
+    def test_field_definition_with_prohibited_attr(self):
+        attr = AttrFactory.native(DataType.INT)
+        attr.restrictions.max_occurs = 0
+        attr.default = "1"
+
+        result = self.filters.field_definition(attr, {}, None, ["Root"])
+        expected = (
+            "field(\n"
+            "        init=False,\n"
+            "        metadata={\n"
+            '            "type": "Ignore",\n'
+            "        }\n"
+            "    )"
+        )
+        self.assertEqual(expected, result)
+
     @mock.patch.object(Filters, "field_default_value")
     def test_field_definition_with_restriction_pattern(self, mock_field_default_value):
         mock_field_default_value.return_value = None
         str_attr = AttrFactory.create(types=[type_str], tag=Tag.RESTRICTION)
         # intentionally using a double-quote in the pattern to test for a regression in
         # https://github.com/tefra/xsdata/issues/592
         pattern = '([^\\ \\? > < \\* / " ": |]{1,256})'
@@ -528,14 +550,19 @@
             types=[
                 AttrTypeFactory.native(DataType.INT),
                 AttrTypeFactory.native(DataType.POSITIVE_INTEGER),
             ]
         )
         self.assertEqual("Optional[int]", self.filters.field_type(attr, ["a", "b"]))
 
+    def test_field_type_with_prohibited_attr(self):
+        attr = AttrFactory.create(restrictions=Restrictions(max_occurs=0))
+
+        self.assertEqual("Any", self.filters.field_type(attr, ["a", "b"]))
+
     def test_choice_type(self):
         choice = AttrFactory.create(types=[AttrTypeFactory.create("foobar")])
         actual = self.filters.choice_type(choice, ["a", "b"])
         self.assertEqual("Type[Foobar]", actual)
 
     def test_choice_type_with_forward_reference(self):
         choice = AttrFactory.create(
@@ -646,14 +673,18 @@
         expected = "from typing import Union"
         self.assertIn(expected, self.filters.default_imports(output))
 
         output = " Type["
         expected = "from typing import Type"
         self.assertIn(expected, self.filters.default_imports(output))
 
+        output = ": Any = "
+        expected = "from typing import Any"
+        self.assertIn(expected, self.filters.default_imports(output))
+
     def test_default_imports_combo(self):
         output = (
             "@dataclass\n"
             "class Foo:\n"
             "    field: Optional[str] = field(default=None)"
         )
```

### Comparing `xsdata-22.9/tests/formats/dataclass/test_generator.py` & `xsdata-23.5/tests/formats/dataclass/test_generator.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/formats/dataclass/test_transport.py` & `xsdata-23.5/tests/formats/dataclass/test_transport.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/formats/dataclass/test_typing.py` & `xsdata-23.5/tests/formats/dataclass/test_typing.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/formats/test_converter.py` & `xsdata-23.5/tests/formats/test_converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+import sys
 import warnings
 from datetime import date
 from datetime import datetime
 from datetime import time
 from decimal import Decimal
 from enum import Enum
 from typing import Any
 from unittest import TestCase
 from xml.etree.ElementTree import QName
 
+import pytest
+
 from tests.fixtures.datatypes import Telephone
 from xsdata.exceptions import ConverterError
 from xsdata.formats.converter import Converter
 from xsdata.formats.converter import converter
 from xsdata.formats.converter import ProxyConverter
 from xsdata.models.datatype import XmlDuration
 from xsdata.models.datatype import XmlPeriod
@@ -208,15 +211,14 @@
         output = self.converter.serialize(obj, format="base64")
 
         self.assertIsInstance(obj, bytes)
         self.assertEqual(b"1-2-3", obj)
         self.assertEqual("MS0yLTM=", output)
 
     def test_serialize_raises_exception(self):
-
         with self.assertRaises(ConverterError) as cm:
             self.converter.deserialize(1, format="foo")
 
         self.assertEqual("Input value must be 'str' got 'int'", str(cm.exception))
 
         with self.assertRaises(ConverterError):
             self.converter.deserialize("aaa", format="base16")
@@ -355,14 +357,18 @@
     J = (Telephone(1, 2, 3), Telephone(4, 5, 6))
 
 
 class EnumConverterTests(TestCase):
     def setUp(self):
         self.converter = converter.type_converter(Enum)
 
+    @pytest.mark.skipif(
+        sys.version_info == (3, 11, 1, "final", 0),
+        reason="https://github.com/python/cpython/issues/100098",
+    )
     def test_deserialize(self):
         convert = self.converter.deserialize
         self.assertEqual(EnumA.C, convert("2.1", data_type=EnumA))
         self.assertEqual(EnumA.C, convert(2.1, data_type=EnumA))
         self.assertEqual(EnumA.E, convert(["2.1", "a", "NaN"], data_type=EnumA))
         self.assertEqual(EnumA.F, convert([2.1, "a", 2], data_type=EnumA))
         self.assertEqual(EnumA.D, convert("  2.1  a ", data_type=EnumA))
```

### Comparing `xsdata-22.9/tests/integration/benchmarks/test_converters.py` & `xsdata-23.5/tests/integration/benchmarks/test_converters.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/integration/benchmarks/test_handlers.py` & `xsdata-23.5/tests/integration/benchmarks/test_handlers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import random
 
 import pytest
 
 from tests import xsdata_temp_dir
-from tests.integration.benchmarks.conftest import make_books
-from tests.integration.benchmarks.conftest import parse
-from tests.integration.benchmarks.conftest import write
+from tests.integration.benchmarks.utils import make_books
+from tests.integration.benchmarks.utils import parse
+from tests.integration.benchmarks.utils import write
 from xsdata.formats.dataclass.context import XmlContext
 from xsdata.formats.dataclass.parsers import handlers as readers
 from xsdata.formats.dataclass.serializers import writers
 
 context = XmlContext()
 readers_list = list(readers.__all__)
 writers_list = list(writers.__all__)
```

### Comparing `xsdata-22.9/tests/integration/test_annotations.py` & `xsdata-23.5/tests/integration/test_annotations.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/integration/test_artists.py` & `xsdata-23.5/tests/integration/test_artists.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/integration/test_books.py` & `xsdata-23.5/tests/integration/test_books.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/integration/test_calculator.py` & `xsdata-23.5/tests/integration/test_calculator.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/integration/test_compound.py` & `xsdata-23.5/tests/integration/test_compound.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/integration/test_docstrings.py` & `xsdata-23.5/tests/integration/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/integration/test_dtd.py` & `xsdata-23.5/tests/integration/test_dtd.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/integration/test_hello_rpc.py` & `xsdata-23.5/tests/integration/test_hello_rpc.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/integration/test_primer.py` & `xsdata-23.5/tests/integration/test_primer.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/integration/test_series.py` & `xsdata-23.5/tests/integration/test_series.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/integration/test_stripe.py` & `xsdata-23.5/tests/integration/test_stripe.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/models/enums/test_datatype.py` & `xsdata-23.5/tests/models/enums/test_datatype.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,14 @@
         self.assertEqual(DataType.FLOAT, DataType.from_value(-1.175494351e-38))
         self.assertEqual(DataType.FLOAT, DataType.from_value(3.402823466e38))
 
         self.assertEqual(DataType.DOUBLE, DataType.from_value(-1.175494352e-38))
         self.assertEqual(DataType.DOUBLE, DataType.from_value(3.402823467e38))
 
     def test_from_value_period(self):
-
         g_day = XmlPeriod("---20-02:44")
         self.assertEqual(DataType.G_DAY, DataType.from_value(g_day))
 
         g_month_day = XmlPeriod("--12-20-02:44")
         self.assertEqual(DataType.G_MONTH_DAY, DataType.from_value(g_month_day))
 
         g_month = XmlPeriod("--12")
```

### Comparing `xsdata-22.9/tests/models/test_config.py` & `xsdata-23.5/tests/models/test_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,16 @@
             "    <Structure>filenames</Structure>\n"
             "    <DocstringStyle>reStructuredText</DocstringStyle>\n"
             "    <FilterStrategy>allGlobals</FilterStrategy>\n"
             "    <RelativeImports>false</RelativeImports>\n"
             '    <CompoundFields defaultName="choice" forceDefaultName="false">false</CompoundFields>\n'
             "    <PostponedAnnotations>false</PostponedAnnotations>\n"
             "    <UnnestClasses>false</UnnestClasses>\n"
+            "    <IgnorePatterns>false</IgnorePatterns>\n"
+            "    <IncludeHeader>false</IncludeHeader>\n"
             "  </Output>\n"
             "  <Conventions>\n"
             '    <ClassName case="pascalCase" safePrefix="type"/>\n'
             '    <FieldName case="snakeCase" safePrefix="value"/>\n'
             '    <ConstantName case="screamingSnakeCase" safePrefix="value"/>\n'
             '    <ModuleName case="snakeCase" safePrefix="mod"/>\n'
             '    <PackageName case="snakeCase" safePrefix="pkg"/>\n'
@@ -52,15 +54,15 @@
             '    <Substitution type="package" search="http://www.w3.org/2001/XMLSchema-instance" replace="xsi"/>\n'
             '    <Substitution type="package" search="http://www.w3.org/1998/Math/MathML" replace="mathml3"/>\n'
             '    <Substitution type="package" search="http://www.w3.org/1999/xlink" replace="xlink"/>\n'
             '    <Substitution type="package" search="http://www.w3.org/1999/xhtml" replace="xhtml"/>\n'
             '    <Substitution type="package" search="http://schemas.xmlsoap.org/wsdl/soap/" replace="soap"/>\n'
             '    <Substitution type="package" search="http://schemas.xmlsoap.org/wsdl/soap12/" replace="soap12"/>\n'
             '    <Substitution type="package" search="http://schemas.xmlsoap.org/soap/envelope/" replace="soapenv"/>\n'
-            '    <Substitution type="class" search="Class" replace="Type"/>\n'
+            '    <Substitution type="class" search="(.*)Class$" replace="\\1Type"/>\n'
             "  </Substitutions>\n"
             "</Config>\n"
         )
         self.assertEqual(expected, file_path.read_text())
         file_path.unlink()
 
     def test_read(self):
@@ -93,14 +95,16 @@
             "    <Structure>filenames</Structure>\n"
             "    <DocstringStyle>reStructuredText</DocstringStyle>\n"
             "    <FilterStrategy>allGlobals</FilterStrategy>\n"
             "    <RelativeImports>false</RelativeImports>\n"
             '    <CompoundFields defaultName="choice" forceDefaultName="false">false</CompoundFields>\n'
             "    <PostponedAnnotations>false</PostponedAnnotations>\n"
             "    <UnnestClasses>false</UnnestClasses>\n"
+            "    <IgnorePatterns>false</IgnorePatterns>\n"
+            "    <IncludeHeader>false</IncludeHeader>\n"
             "  </Output>\n"
             "  <Conventions>\n"
             '    <ClassName case="pascalCase" safePrefix="type"/>\n'
             '    <FieldName case="snakeCase" safePrefix="value"/>\n'
             '    <ConstantName case="screamingSnakeCase" safePrefix="value"/>\n'
             '    <ModuleName case="snakeCase" safePrefix="mod"/>\n'
             '    <PackageName case="snakeCase" safePrefix="pkg"/>\n'
@@ -122,15 +126,14 @@
         )
         file_path = Path(tempfile.mktemp())
         file_path.write_text(existing, encoding="utf-8")
         with self.assertRaises(ParserError):
             GeneratorConfig.read(file_path)
 
     def test_format_with_invalid_state(self):
-
         with self.assertRaises(GeneratorConfigError) as cm:
             OutputFormat(eq=False, order=True)
 
         self.assertEqual("eq must be true if order is true", str(cm.exception))
 
     def test_format_slots_requires_310(self):
         if sys.version_info < (3, 10):
```

### Comparing `xsdata-22.9/tests/models/test_datatype.py` & `xsdata-23.5/tests/models/test_datatype.py`

 * *Files 0% similar despite different names*

```diff
@@ -413,15 +413,14 @@
         self.assertEqual(5, duration.days)
         self.assertEqual(12, duration.hours)
         self.assertEqual(35, duration.minutes)
         self.assertEqual(30.5, duration.seconds)
         self.assertFalse(duration.negative)
 
     def test_init_valid(self):
-
         fixtures = {
             "P2Y6M5DT12H35M30.5S": {
                 "days": 5,
                 "hours": 12,
                 "minutes": 35,
                 "months": 6,
                 "negative": False,
@@ -493,15 +492,14 @@
         period = XmlPeriod("---20-02:44")
         self.assertIsNone(period.year)
         self.assertIsNone(period.month)
         self.assertEqual(20, period.day)
         self.assertEqual(-164, period.offset)
 
     def test_init_valid(self):
-
         fixtures = {
             "--05---05:00": {"month": 5, "offset": -300},
             "---01 ": {"day": 1},
             "---01Z": {"day": 1, "offset": 0},
             "---01+02:00": {"day": 1, "offset": 120},
             " ---01-04:00": {"day": 1, "offset": -240},
             "---15": {"day": 15},
```

### Comparing `xsdata-22.9/tests/models/test_mixins.py` & `xsdata-23.5/tests/models/test_mixins.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/models/wsdl/test_binding.py` & `xsdata-23.5/tests/models/wsdl/test_binding.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/models/wsdl/test_definitions.py` & `xsdata-23.5/tests/models/wsdl/test_definitions.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/models/wsdl/test_port_type.py` & `xsdata-23.5/tests/models/wsdl/test_port_type.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/models/xsd/test_alternative.py` & `xsdata-23.5/tests/models/xsd/test_list.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 from unittest import TestCase
 
-from xsdata.models.xsd import Alternative
+from xsdata.models.xsd import List
 
 
-class AlternativeTests(TestCase):
-    def test_property_real_name(self):
-        obj = Alternative()
-        self.assertEqual("value", obj.real_name)
-
-        obj.id = "foo"
-        self.assertEqual("foo", obj.real_name)
+class ListTests(TestCase):
+    def test_is_attribute(self):
+        obj = List()
+        self.assertTrue(obj.is_property)
 
-        obj.test = "@type='text'"
-        self.assertEqual("type_text", obj.real_name)
+    def test_real_name(self):
+        obj = List()
+        self.assertEqual("value", obj.real_name)
 
-    def test_property_bases(self):
-        obj = Alternative()
-        self.assertEqual([], list(obj.bases))
+    def test_real_type(self):
+        obj = List()
+        self.assertEqual([], list(obj.attr_types))
 
-        obj.type = "foo"
-        self.assertEqual(["foo"], list(obj.bases))
+        obj.item_type = "foo"
+        self.assertEqual(["foo"], list(obj.attr_types))
 
     def test_get_restrictions(self):
-        obj = Alternative()
-        expected = {"min_occurs": 0, "choice": str(id(obj))}
-        self.assertEqual(expected, obj.get_restrictions())
+        obj = List()
+        self.assertEqual({"tokens": True}, obj.get_restrictions())
```

### Comparing `xsdata-22.9/tests/models/xsd/test_annotation_base.py` & `xsdata-23.5/tests/models/xsd/test_annotation_base.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/models/xsd/test_any.py` & `xsdata-23.5/tests/models/xsd/test_any.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/models/xsd/test_any_attribute.py` & `xsdata-23.5/tests/models/xsd/test_any_attribute.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/models/xsd/test_attribute.py` & `xsdata-23.5/tests/models/xsd/test_attribute.py`

 * *Files 17% similar despite different names*

```diff
@@ -63,7 +63,18 @@
 
         obj.simple_type = SimpleType()
         self.assertEqual([], list(obj.bases))
 
         obj.type = "foo"
         obj.simple_type = None
         self.assertEqual(["foo"], list(obj.bases))
+
+    def test_property_default_type(self):
+        obj = Attribute()
+        self.assertEqual("anySimpleType", obj.default_type)
+
+        obj = Attribute()
+        obj.ns_map["foo"] = Namespace.XS.uri
+        self.assertEqual("foo:anySimpleType", obj.default_type)
+
+        obj.fixed = "aa"
+        self.assertEqual("foo:string", obj.default_type)
```

### Comparing `xsdata-22.9/tests/models/xsd/test_choice.py` & `xsdata-23.5/tests/models/xsd/test_group.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,20 @@
-import sys
 from unittest import TestCase
 
-from xsdata.models.xsd import Choice
+from xsdata.models.xsd import Group
 
 
-class ChoiceTests(TestCase):
-    def test_get_restrictions(self):
-        obj = Choice(min_occurs=1, max_occurs=2)
+class GroupTests(TestCase):
+    def test_property_is_property(self):
+        obj = Group()
+        self.assertTrue(obj.is_property)
+
+    def test_property_attr_types(self):
+        obj = Group()
+        self.assertEqual([], list(obj.attr_types))
 
-        expected = {
-            "choice": str(id(obj)),
-            "min_occurs": 0,
-            "max_occurs": 2,
-        }
-        self.assertEqual(expected, obj.get_restrictions())
-
-        obj = Choice(max_occurs="unbounded")
-        expected = {
-            "choice": str(id(obj)),
-            "min_occurs": 0,
-            "max_occurs": sys.maxsize,
-        }
-        self.assertEqual(expected, obj.get_restrictions())
+        obj.ref = "foo"
+        self.assertEqual(["foo"], list(obj.attr_types))
+
+    def test_get_restrictions(self):
+        obj = Group(min_occurs=1, max_occurs=2)
+        self.assertEqual({"path": [("g", id(obj), 1, 2)]}, obj.get_restrictions())
```

### Comparing `xsdata-22.9/tests/models/xsd/test_complex_type.py` & `xsdata-23.5/tests/models/xsd/test_complex_type.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/models/xsd/test_element.py` & `xsdata-23.5/tests/models/xsd/test_element.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/models/xsd/test_enumeration.py` & `xsdata-23.5/tests/models/xsd/test_enumeration.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/models/xsd/test_group.py` & `xsdata-23.5/tests/models/xsd/test_alternative.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 from unittest import TestCase
 
-from xsdata.models.xsd import Group
+from xsdata.models.xsd import Alternative
 
 
-class GroupTests(TestCase):
-    def test_property_is_property(self):
-        obj = Group()
-        self.assertTrue(obj.is_property)
+class AlternativeTests(TestCase):
+    def test_property_real_name(self):
+        obj = Alternative()
+        self.assertEqual("value", obj.real_name)
 
-    def test_property_attr_types(self):
-        obj = Group()
-        self.assertEqual([], list(obj.attr_types))
+        obj.id = "foo"
+        self.assertEqual("foo", obj.real_name)
 
-        obj.ref = "foo"
-        self.assertEqual(["foo"], list(obj.attr_types))
+        obj.test = "@type='text'"
+        self.assertEqual("type_text", obj.real_name)
+
+    def test_property_bases(self):
+        obj = Alternative()
+        self.assertEqual([], list(obj.bases))
+
+        obj.type = "foo"
+        self.assertEqual(["foo"], list(obj.bases))
 
     def test_get_restrictions(self):
-        obj = Group(min_occurs=1, max_occurs=2)
-        self.assertEqual({"max_occurs": 2, "min_occurs": 1}, obj.get_restrictions())
+        obj = Alternative()
+        self.assertEqual({"path": [("alt", id(obj), 0, 1)]}, obj.get_restrictions())
```

### Comparing `xsdata-22.9/tests/models/xsd/test_restriction.py` & `xsdata-23.5/tests/models/xsd/test_restriction.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/models/xsd/test_schema.py` & `xsdata-23.5/tests/models/xsd/test_schema.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/models/xsd/test_simple_type.py` & `xsdata-23.5/tests/models/xsd/test_simple_type.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/models/xsd/test_union.py` & `xsdata-23.5/tests/models/xsd/test_union.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/test_cli.py` & `xsdata-23.5/tests/test_cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,25 @@
+import logging
+import platform
+import sys
 import tempfile
 from pathlib import Path
 from unittest import mock
 from unittest import TestCase
 
 from click.testing import CliRunner
 
 from tests import fixtures_dir
+from xsdata import __version__
 from xsdata.cli import cli
 from xsdata.cli import resolve_source
 from xsdata.codegen.transformer import SchemaTransformer
 from xsdata.codegen.writer import CodeWriter
 from xsdata.formats.dataclass.generator import DataclassGenerator
+from xsdata.logger import logger
 from xsdata.models.config import GeneratorConfig
 from xsdata.models.config import StructureStyle
 from xsdata.utils.downloader import Downloader
 
 CodeWriter.register_generator("testing", DataclassGenerator)
 
 
@@ -79,24 +84,38 @@
         source = fixtures_dir.joinpath("defxmlschema/chapter03.xsd")
         result = self.runner.invoke(cli, [str(source), "--package", "foo", "--print"])
 
         self.assertIsNone(result.exception)
         self.assertEqual([source.as_uri()], mock_process.call_args[0][0])
         self.assertTrue(mock_init.call_args[1]["print"])
 
+    @mock.patch.object(SchemaTransformer, "process")
+    @mock.patch.object(SchemaTransformer, "__init__", return_value=None)
+    def test_generate_with_debug_mode(self, *args):
+        self.runner.invoke(cli, ["foo.xsd", "--package", "foo", "--debug"])
+        self.assertEqual(logging.DEBUG, logger.level)
+
     @mock.patch("xsdata.cli.logger.info")
     def test_init_config(self, mock_info):
         output = tempfile.mktemp()
         output_path = Path(output)
         result = self.runner.invoke(cli, ["init-config", str(output_path)])
 
         self.assertIsNone(result.exception)
         self.assertEqual(GeneratorConfig.create(), GeneratorConfig.read(output_path))
-        mock_info.assert_called_once_with(
-            "Initializing configuration file %s", str(output_path)
+        mock_info.assert_has_calls(
+            [
+                mock.call(
+                    "========= xsdata v%s / Python %s / Platform %s =========\n",
+                    __version__,
+                    platform.python_version(),
+                    sys.platform,
+                ),
+                mock.call("Initializing configuration file %s", str(output_path)),
+            ]
         )
         output_path.unlink()
 
     @mock.patch("xsdata.cli.logger.info")
     def test_init_config_when_file_exists(self, mock_info):
         output = tempfile.mktemp()
         output_path = Path(output).resolve()
@@ -107,16 +126,24 @@
         with output_path.open("w") as fp:
             config.write(fp, config)
 
         result = self.runner.invoke(cli, ["init-config", str(output_path)])
 
         self.assertIsNone(result.exception)
         self.assertNotEqual("20.8", GeneratorConfig.read(output_path))
-        mock_info.assert_called_once_with(
-            "Updating configuration file %s", str(output_path)
+        mock_info.assert_has_calls(
+            [
+                mock.call(
+                    "========= xsdata v%s / Python %s / Platform %s =========\n",
+                    __version__,
+                    platform.python_version(),
+                    sys.platform,
+                ),
+                mock.call("Updating configuration file %s", str(output_path)),
+            ]
         )
         output_path.unlink()
 
     def test_init_config_with_print_mode(self):
         result = self.runner.invoke(cli, ["init-config", "--print"])
 
         self.assertIsNone(result.exception)
```

### Comparing `xsdata-22.9/tests/utils/test_dates.py` & `xsdata-23.5/tests/utils/test_dates.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/utils/test_downloader.py` & `xsdata-23.5/tests/utils/test_downloader.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/utils/test_hooks.py` & `xsdata-23.5/tests/utils/test_hooks.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/utils/test_namespaces.py` & `xsdata-23.5/tests/utils/test_namespaces.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/tests/utils/test_text.py` & `xsdata-23.5/tests/utils/test_text.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/xsdata/cli.py` & `xsdata-23.5/xsdata/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import platform
 import sys
 import warnings
 from pathlib import Path
 from typing import Any
 from typing import Iterator
 
 import click
@@ -38,18 +39,23 @@
 logging.captureWarnings(True)
 
 
 @click.group(cls=DefaultGroup, default="generate", default_if_no_args=False)
 @click.pass_context
 @click.version_option(__version__)
 def cli(ctx: click.Context, **kwargs: Any):
-    """xsdata command line interface."""
-
+    """Xsdata command line interface."""
     logger.setLevel(logging.INFO)
     formatwarning_orig = warnings.formatwarning
+    logger.info(
+        "========= xsdata v%s / Python %s / Platform %s =========\n",
+        __version__,
+        platform.python_version(),
+        sys.platform,
+    )
 
     def format_warning(message: Any, category: Any, *args: Any) -> str:
         return (
             f"{category.__name__}: {message}" if category else message
         )  # pragma: no cover
 
     def format_warning_restore():
@@ -106,35 +112,43 @@
     "--recursive",
     is_flag=True,
     default=False,
     help="Search files recursively in the source directory",
 )
 @click.option("-c", "--config", default=".xsdata.xml", help="Project configuration")
 @click.option("-pp", "--print", is_flag=True, default=False, help="Print output")
+@click.option("--cache", is_flag=True, default=False, help="Cache sources loading")
+@click.option("--debug", is_flag=True, default=False, help="Show debug messages")
 @model_options(GeneratorOutput)
 def generate(**kwargs: Any):
     """
     Generate code from xml schemas, webservice definitions and any xml or json
     document.
 
     The input source can be either a filepath, uri or a directory
     containing xml, json, xsd and wsdl files.
     """
+
+    debug = kwargs.pop("debug")
+    if debug:
+        logger.setLevel(logging.DEBUG)
+
     source = kwargs.pop("source")
     stdout = kwargs.pop("print")
+    cache = kwargs.pop("cache")
     recursive = kwargs.pop("recursive")
     config_file = Path(kwargs.pop("config")).resolve()
 
     params = {k.replace("__", "."): v for k, v in kwargs.items() if v is not None}
     config = GeneratorConfig.read(config_file)
     config.output.update(**params)
 
     transformer = SchemaTransformer(config=config, print=stdout)
     uris = sorted(resolve_source(source, recursive=recursive))
-    transformer.process(uris)
+    transformer.process(uris, cache=cache)
 
     handler.emit_warnings()
 
 
 def resolve_source(source: str, recursive: bool) -> Iterator[str]:
     if source.find("://") > -1 and not source.startswith("file://"):
         yield source
```

### Comparing `xsdata-22.9/xsdata/codegen/analyzer.py` & `xsdata-23.5/xsdata/codegen/analyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 class ClassAnalyzer:
     """Validate, analyze, sanitize and select the final class list to be
     generated."""
 
     @classmethod
     def process(cls, container: ClassContainer) -> List[Class]:
         """Run all the processes."""
-
         # Run validation checks for duplicate, invalid and redefined types.
         ClassValidator(container).process()
 
         # Run analyzer handlers
         container.process()
 
         classes = list(container)
```

### Comparing `xsdata-22.9/xsdata/codegen/container.py` & `xsdata-23.5/xsdata/codegen/container.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from typing import Callable
 from typing import Dict
 from typing import Iterator
 from typing import List
 from typing import Optional
 
 from xsdata.codegen.handlers import AddAttributeSubstitutions
+from xsdata.codegen.handlers import CalculateAttributePaths
 from xsdata.codegen.handlers import CreateCompoundFields
 from xsdata.codegen.handlers import DesignateClassPackages
 from xsdata.codegen.handlers import FilterClasses
 from xsdata.codegen.handlers import FlattenAttributeGroups
 from xsdata.codegen.handlers import FlattenClassExtensions
 from xsdata.codegen.handlers import MergeAttributes
 from xsdata.codegen.handlers import ProcessAttributeTypes
 from xsdata.codegen.handlers import ProcessMixedContentClass
 from xsdata.codegen.handlers import RenameDuplicateAttributes
 from xsdata.codegen.handlers import RenameDuplicateClasses
+from xsdata.codegen.handlers import ResetAttributeSequenceNumbers
+from xsdata.codegen.handlers import ResetAttributeSequences
 from xsdata.codegen.handlers import SanitizeAttributesDefaultValue
 from xsdata.codegen.handlers import SanitizeEnumerationClass
 from xsdata.codegen.handlers import UnnestInnerClasses
 from xsdata.codegen.handlers import UpdateAttributesEffectiveChoice
 from xsdata.codegen.handlers import VacuumInnerClasses
 from xsdata.codegen.handlers import ValidateAttributesOverrides
 from xsdata.codegen.mixins import ContainerInterface
@@ -27,108 +30,107 @@
 from xsdata.codegen.utils import ClassUtils
 from xsdata.models.config import GeneratorConfig
 from xsdata.utils import collections
 from xsdata.utils.constants import return_true
 
 
 class Steps:
-    FLATTEN = 10
-    SANITIZE = 20
-    RESOLVE = 30
-    FINALIZE = 40
+    UNGROUP = 10
+    FLATTEN = 20
+    SANITIZE = 30
+    RESOLVE = 40
+    FINALIZE = 50
 
 
 class ClassContainer(ContainerInterface):
-
-    __slots__ = ("data", "processors")
+    __slots__ = ("data", "processors", "step")
 
     def __init__(self, config: GeneratorConfig):
         """Initialize a class container instance with its processors based on
         the provided configuration."""
         super().__init__(config)
 
+        self.step: int = 0
         self.data: Dict = {}
 
-        self.processors = {
-            Steps.FLATTEN: [
+        self.processors: Dict[int, List] = {
+            Steps.UNGROUP: [
                 FlattenAttributeGroups(self),
+            ],
+            Steps.FLATTEN: [
+                CalculateAttributePaths(),
                 FlattenClassExtensions(self),
                 SanitizeEnumerationClass(self),
+                UpdateAttributesEffectiveChoice(),
                 UnnestInnerClasses(self),
                 AddAttributeSubstitutions(self),
                 ProcessAttributeTypes(self),
                 MergeAttributes(),
                 ProcessMixedContentClass(),
             ],
             Steps.SANITIZE: [
-                UpdateAttributesEffectiveChoice(),
+                ResetAttributeSequences(),
                 SanitizeAttributesDefaultValue(self),
             ],
             Steps.RESOLVE: [
                 ValidateAttributesOverrides(self),
                 RenameDuplicateAttributes(),
             ],
             Steps.FINALIZE: [
                 VacuumInnerClasses(),
                 CreateCompoundFields(self),
+                # Prettify things!!!
+                ResetAttributeSequenceNumbers(self),
             ],
         }
 
     def __iter__(self) -> Iterator[Class]:
         """Create an iterator for the class map values."""
         for items in list(self.data.values()):
             yield from items
 
     def find(self, qname: str, condition: Callable = return_true) -> Optional[Class]:
         """Search by qualified name for a specific class with an optional
         condition callable."""
         for row in self.data.get(qname, []):
             if condition(row):
-                if row.status == Status.RAW:
-                    self.process_class(row, Steps.FLATTEN)
+                if row.status < self.step:
+                    self.process_class(row, self.step)
                     return self.find(qname, condition)
 
                 return row
         return None
 
     def find_inner(self, source: Class, qname: str) -> Class:
         inner = ClassUtils.find_inner(source, qname)
-        if inner.status == Status.RAW:
-            self.process_class(inner, Steps.FLATTEN)
+        if inner.status < self.step:
+            self.process_class(inner, self.step)
 
         return inner
 
     def first(self, qname: str) -> Class:
         classes = self.data.get(qname)
         if not classes:
             raise KeyError(f"Class {qname} not found")
 
         return classes[0]
 
     def process(self):
-        """
-        Run all the process handlers.
-
-        Steps
-            1. Flatten extensions, attribute types
-            2. Filter classes to be actually generated
-            3. Sanitize attributes and extensions
-            4. Resolve attributes conflicts
-            5. Replace repeatable elements with compound fields
-            6. Designate packages and modules
-        """
-
+        """The hidden naive recipe of processing xsd models."""
+        self.process_classes(Steps.UNGROUP)
+        self.remove_groups()
         self.process_classes(Steps.FLATTEN)
         self.filter_classes()
         self.process_classes(Steps.SANITIZE)
         self.process_classes(Steps.RESOLVE)
         self.process_classes(Steps.FINALIZE)
         self.designate_classes()
 
     def process_classes(self, step: int) -> None:
+        self.step = step
         for obj in self:
             if obj.status < step:
                 self.process_class(obj, step)
 
     def process_class(self, target: Class, step: int):
         target.status = Status(step)
         for processor in self.processors.get(step, []):
@@ -149,14 +151,17 @@
         for designator in designators:
             designator.run()
 
     def filter_classes(self):
         """Filter the classes to be generated."""
         FilterClasses(self).run()
 
+    def remove_groups(self):
+        self.set([x for x in iter(self) if not x.is_group])
+
     def add(self, item: Class):
         """Add class item to the container."""
         self.data.setdefault(item.qname, []).append(item)
 
     def reset(self, item: Class, qname: str):
         self.data[qname].remove(item)
         self.add(item)
```

### Comparing `xsdata-22.9/xsdata/codegen/handlers/__init__.py` & `xsdata-23.5/xsdata/codegen/handlers/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 from .add_attribute_substitutions import AddAttributeSubstitutions
+from .calculate_attribute_paths import CalculateAttributePaths
 from .create_compound_fields import CreateCompoundFields
 from .designate_class_packages import DesignateClassPackages
 from .filter_classes import FilterClasses
 from .flatten_attribute_groups import FlattenAttributeGroups
 from .flatten_class_extensions import FlattenClassExtensions
 from .merge_attributes import MergeAttributes
 from .process_attributes_types import ProcessAttributeTypes
 from .process_mixed_content_class import ProcessMixedContentClass
 from .rename_duplicate_attributes import RenameDuplicateAttributes
 from .rename_duplicate_classes import RenameDuplicateClasses
+from .reset_attribute_sequence_numbers import ResetAttributeSequenceNumbers
+from .reset_attribute_sequences import ResetAttributeSequences
 from .sanitize_attributes_default_value import SanitizeAttributesDefaultValue
 from .sanitize_enumeration_class import SanitizeEnumerationClass
 from .unnest_inner_classes import UnnestInnerClasses
 from .update_attributes_effective_choice import UpdateAttributesEffectiveChoice
 from .vacuum_inner_classes import VacuumInnerClasses
 from .validate_attributes_overrides import ValidateAttributesOverrides
 
 __all__ = [
     "AddAttributeSubstitutions",
+    "CalculateAttributePaths",
     "CreateCompoundFields",
     "DesignateClassPackages",
     "FilterClasses",
     "FlattenAttributeGroups",
     "FlattenClassExtensions",
     "MergeAttributes",
     "ProcessAttributeTypes",
     "ProcessMixedContentClass",
     "RenameDuplicateAttributes",
     "RenameDuplicateClasses",
+    "ResetAttributeSequences",
+    "ResetAttributeSequenceNumbers",
     "SanitizeAttributesDefaultValue",
     "SanitizeEnumerationClass",
     "UnnestInnerClasses",
     "UpdateAttributesEffectiveChoice",
     "VacuumInnerClasses",
     "ValidateAttributesOverrides",
 ]
```

### Comparing `xsdata-22.9/xsdata/codegen/handlers/add_attribute_substitutions.py` & `xsdata-23.5/xsdata/codegen/handlers/add_attribute_substitutions.py`

 * *Files 20% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     def process(self, target: Class):
         """
         Search and process attributes not derived from xs:enumeration or
         xs:any.
 
         Build the substitutions map if it's not initialized yet.
         """
-
         if self.substitutions is None:
             self.create_substitutions()
 
         for attr in list(target.attrs):
             if not (attr.is_enumeration or attr.is_wildcard):
                 self.process_attribute(target, attr)
 
@@ -52,16 +51,19 @@
 
         for attr_type in attr.types:
             if attr_type.substituted:
                 continue
 
             attr_type.substituted = True
             for substitution in self.substitutions.get(attr_type.qname, []):
-                attr.restrictions.min_occurs = 0
+                self.prepare_substituted(attr)
+
                 clone = ClassUtils.clone_attribute(substitution, attr.restrictions)
+                clone.restrictions.min_occurs = 0
+                clone.restrictions.max_occurs = attr.restrictions.max_occurs
 
                 pos = collections.find(target.attrs, clone)
                 index = pos + 1 if pos > -1 else index
                 target.attrs.insert(index, clone)
 
                 self.process_attribute(target, clone)
 
@@ -72,14 +74,22 @@
         self.substitutions = defaultdict(list)
         for obj in self.container:
             for qname in obj.substitutions:
                 attr = self.create_substitution(obj)
                 self.substitutions[qname].append(attr)
 
     @classmethod
+    def prepare_substituted(cls, attr: Attr):
+        attr.restrictions.min_occurs = 0
+        if not attr.restrictions.choice:
+            choice = id(attr)
+            attr.restrictions.choice = choice
+            attr.restrictions.path.append(("c", choice, 1, 1))
+
+    @classmethod
     def create_substitution(cls, source: Class) -> Attr:
         """Create an attribute with type that refers to the given source class
         and namespaced qualified name."""
 
         return Attr(
             name=source.name,
             types=[AttrType(qname=source.qname)],
```

### Comparing `xsdata-22.9/xsdata/codegen/handlers/create_compound_fields.py` & `xsdata-23.5/xsdata/codegen/handlers/create_compound_fields.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,22 @@
+from collections import Counter
+from typing import Dict
 from typing import List
+from typing import Set
+from typing import Tuple
 
 from xsdata.codegen.mixins import ContainerInterface
 from xsdata.codegen.mixins import RelativeHandlerInterface
 from xsdata.codegen.models import Attr
 from xsdata.codegen.models import AttrType
 from xsdata.codegen.models import Class
 from xsdata.codegen.models import get_restriction_choice
-from xsdata.codegen.models import get_slug
 from xsdata.codegen.models import Restrictions
 from xsdata.codegen.utils import ClassUtils
+from xsdata.formats.dataclass.models.elements import XmlType
 from xsdata.models.enums import DataType
 from xsdata.models.enums import Tag
 from xsdata.utils.collections import group_by
 
 
 class CreateCompoundFields(RelativeHandlerInterface):
     """Group attributes that belong in the same choice and replace them by
@@ -25,106 +29,124 @@
 
         self.config = container.config.output.compound_fields
 
     def process(self, target: Class):
         if self.config.enabled:
             groups = group_by(target.attrs, get_restriction_choice)
             for choice, attrs in groups.items():
-                if choice and len(attrs) > 1 and any(attr.is_list for attr in attrs):
+                if choice and len(attrs) > 1:
                     self.group_fields(target, attrs)
 
-        for index in range(len(target.attrs)):
-            self.reset_sequential(target, index)
+    @classmethod
+    def update_counters(cls, attr: Attr, counters: Dict):
+        started = False
+        choice = attr.restrictions.choice
+        for path in attr.restrictions.path:
+            if not started and path[0] != "c" and path[1] != choice:
+                continue
+
+            started = True
+            if path not in counters:
+                counters[path] = {"min": [], "max": []}
+            counters = counters[path]
+
+        counters["min"].append(attr.restrictions.min_occurs)
+        counters["max"].append(attr.restrictions.max_occurs)
 
     def group_fields(self, target: Class, attrs: List[Attr]):
         """Group attributes into a new compound field."""
-
         pos = target.attrs.index(attrs[0])
         choice = attrs[0].restrictions.choice
-        sum_occurs = choice and choice.startswith("effective_")
+
+        assert choice is not None
 
         names = []
         choices = []
-        min_occurs = []
-        max_occurs = []
+        counters: Dict = {"min": [], "max": []}
+
         for attr in attrs:
             ClassUtils.remove_attribute(target, attr)
             names.append(attr.local_name)
-            min_occurs.append(attr.restrictions.min_occurs or 0)
-            max_occurs.append(attr.restrictions.max_occurs or 0)
             choices.append(self.build_attr_choice(attr))
 
+            self.update_counters(attr, counters)
+
+        min_occurs, max_occurs = self.sum_counters(counters)
         name = self.choose_name(target, names)
 
         target.attrs.insert(
             pos,
             Attr(
                 name=name,
                 index=0,
                 types=[AttrType(qname=str(DataType.ANY_TYPE), native=True)],
                 tag=Tag.CHOICE,
                 restrictions=Restrictions(
-                    min_occurs=sum(min_occurs) if sum_occurs else min(min_occurs),
-                    max_occurs=sum(max_occurs) if sum_occurs else max(max_occurs),
+                    min_occurs=sum(min_occurs),
+                    max_occurs=max(max_occurs) if choice > 0 else sum(max_occurs),
                 ),
                 choices=choices,
             ),
         )
 
-    def choose_name(self, target: Class, names: List[str]) -> str:
-        reserved = set(map(get_slug, self.base_attrs(target)))
-        reserved.update(map(get_slug, target.attrs))
+    def sum_counters(self, counters: Dict) -> Tuple[List[int], List[int]]:
+        min_occurs = counters.pop("min", [])
+        max_occurs = counters.pop("max", [])
+
+        for path, counter in counters.items():
+            mi, ma = self.sum_counters(counter)
+
+            if path[0] == "c":
+                min_occurs.append(min(mi))
+                max_occurs.append(max(ma))
+            else:
+                min_occurs.append(sum(mi))
+                max_occurs.append(sum(ma))
 
+        return min_occurs, max_occurs
+
+    def choose_name(self, target: Class, names: List[str]) -> str:
         if (
             self.config.force_default_name
             or len(names) > 3
             or len(names) != len(set(names))
         ):
             name = self.config.default_name
         else:
             name = "_Or_".join(names)
 
+        reserved = self.build_reserved_names(target, names)
         return ClassUtils.unique_name(name, reserved)
 
+    def build_reserved_names(self, target: Class, names: List[str]) -> Set[str]:
+        names_counter = Counter(names)
+        all_attrs = self.base_attrs(target)
+        all_attrs.extend(target.attrs)
+
+        return {
+            attr.slug
+            for attr in all_attrs
+            if attr.xml_type != XmlType.ELEMENTS
+            or Counter([x.local_name for x in attr.choices]) != names_counter
+        }
+
     @classmethod
     def build_attr_choice(cls, attr: Attr) -> Attr:
         """
         Converts the given attr to a choice.
 
         The most important part is the reset of certain restrictions
         that don't make sense as choice metadata like occurrences.
         """
         restrictions = attr.restrictions.clone()
         restrictions.min_occurs = None
         restrictions.max_occurs = None
-        restrictions.sequential = None
+        restrictions.sequence = None
 
         return Attr(
             name=attr.local_name,
             namespace=attr.namespace,
-            default=attr.default,
             types=attr.types,
             tag=attr.tag,
             help=attr.help,
             restrictions=restrictions,
         )
-
-    @classmethod
-    def reset_sequential(cls, target: Class, index: int):
-        """Reset the attribute at the given index if it has no siblings with
-        the sequential restriction."""
-
-        attr = target.attrs[index]
-        before = target.attrs[index - 1] if index - 1 >= 0 else None
-        after = target.attrs[index + 1] if index + 1 < len(target.attrs) else None
-
-        if not attr.is_list:
-            attr.restrictions.sequential = False
-
-        if (
-            not attr.restrictions.sequential
-            or (before and before.restrictions.sequential)
-            or (after and after.restrictions.sequential and after.is_list)
-        ):
-            return
-
-        attr.restrictions.sequential = False
```

### Comparing `xsdata-22.9/xsdata/codegen/handlers/designate_class_packages.py` & `xsdata-23.5/xsdata/codegen/handlers/designate_class_packages.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/xsdata/codegen/handlers/filter_classes.py` & `xsdata-23.5/xsdata/codegen/handlers/filter_classes.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/xsdata/codegen/handlers/flatten_attribute_groups.py` & `xsdata-23.5/xsdata/codegen/handlers/flatten_attribute_groups.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     def process(self, target: Class):
         """
         Iterate over all group attributes and apply handler logic.
 
         Group attributes can refer to attributes or other group
         attributes, repeat until there is no group attribute left.
         """
-
         repeat = False
         for attr in list(target.attrs):
             if attr.is_group:
                 repeat = True
                 self.process_attribute(target, attr)
 
         if repeat:
```

### Comparing `xsdata-22.9/xsdata/codegen/handlers/flatten_class_extensions.py` & `xsdata-23.5/xsdata/codegen/handlers/flatten_class_extensions.py`

 * *Files 6% similar despite different names*

```diff
@@ -147,54 +147,59 @@
         Complex flatten extension handler for primary classes eg ComplexType,
         Element.
 
         Compare source and target classes and either remove the
         extension completely, copy all source attributes to the target
         class or leave the extension alone.
         """
-        if cls.should_remove_extension(source, target):
+        if cls.should_remove_extension(source, target, ext):
             target.extensions.remove(ext)
         elif cls.should_flatten_extension(source, target):
             ClassUtils.copy_attributes(source, target, ext)
         else:
             ext.type.reference = id(source)
-            logger.debug("Ignore extension: %s", ext.type.name)
 
     def find_dependency(self, attr_type: AttrType) -> Optional[Class]:
         """
         Find dependency for the given extension type with priority.
 
         Search priority: xs:SimpleType >  xs:ComplexType
         """
-
         conditions = (
             lambda x: x.tag == Tag.SIMPLE_TYPE,
             lambda x: x.tag == Tag.COMPLEX_TYPE,
         )
 
         for condition in conditions:
             result = self.container.find(attr_type.qname, condition=condition)
             if result:
                 return result
 
         return None
 
     @classmethod
-    def should_remove_extension(cls, source: Class, target: Class) -> bool:
+    def should_remove_extension(
+        cls, source: Class, target: Class, ext: Extension
+    ) -> bool:
         """
         Return whether the extension should be removed because of some
         violation.
 
         Violations:
             - Circular Reference
             - Forward Reference
+            - Unordered sequences
             - MRO Violation A(B), C(B) and extensions includes A, B, C
         """
         # Circular or Forward reference
-        if source is target or target in source.inner:
+        if (
+            source is target
+            or target in source.inner
+            or cls.have_unordered_sequences(source, target, ext)
+        ):
             return True
 
         # MRO Violation
         collision = {ext.type.qname for ext in target.extensions}
         return any(ext.type.qname in collision for ext in source.extensions)
 
     @classmethod
@@ -203,58 +208,56 @@
         Return whether the extension should be flattened because of rules.
 
         Rules:
             1. Source doesn't have a parent class
             2. Source class is a simple type
             3. Source class has a suffix attr and target has its own attrs
             4. Target class has a suffix attr
-            5. Target restrictions parent attrs in different sequential order
+            5. Target restrictions parent attrs in different sequence order
             6. Target restricts parent attr with a not matching type.
         """
-
         if not source.extensions and (
             source.is_simple_type
             or target.has_suffix_attr
             or (source.has_suffix_attr and target.attrs)
-            or not cls.validate_type_overrides(source, target)
-            or not cls.validate_sequential_order(source, target)
         ):
             return True
 
         return False
 
     @classmethod
-    def validate_type_overrides(cls, source: Class, target: Class) -> bool:
-        """Validate every override is using a subset of the parent attr
-        types."""
-        for attr in target.attrs:
-            src_attr = ClassUtils.find_attr(source, attr.name)
-            if src_attr and any(tp not in src_attr.types for tp in attr.types):
-                return False
-
-        return True
-
-    @classmethod
-    def validate_sequential_order(cls, source: Class, target: Class) -> bool:
+    def have_unordered_sequences(
+        cls, source: Class, target: Class, ext: Extension
+    ) -> bool:
         """
-        Validate sequential attributes are in the same order in the parent
-        class.
+        Validate sequence attributes are in the same order in the parent class.
 
         Dataclasses fields ordering follows the python mro pattern, the
-        parent fields are always first and they are updated if the
+        parent fields are always first, and they are updated if the
         subclass is overriding any of them but the overall ordering
         doesn't change!
+
+        @todo This needs a complete rewrite and most likely it needs to
+        @todo move way down in the process chain.
         """
-        sequence = [attr.name for attr in target.attrs if attr.restrictions.sequential]
+
+        if ext.tag == Tag.EXTENSION or source.extensions:
+            return False
+
+        sequence = [
+            attr.name
+            for attr in target.attrs
+            if attr.restrictions.sequence is not None and not attr.is_prohibited
+        ]
         if len(sequence) > 1:
             compare = [attr.name for attr in source.attrs if attr.name in sequence]
             if compare and compare != sequence:
-                return False
+                return True
 
-        return True
+        return False
 
     @classmethod
     def replace_attributes_type(cls, target: Class, extension: Extension):
         """Replace all target attributes types with the extension's type and
         remove it from the target class extensions."""
 
         for attr in target.attrs:
```

### Comparing `xsdata-22.9/xsdata/codegen/handlers/merge_attributes.py` & `xsdata-23.5/xsdata/codegen/handlers/merge_attributes.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,20 +11,31 @@
     """Merge same type attributes and their restrictions."""
 
     __slots__ = ()
 
     @classmethod
     def process(cls, target: Class):
         """
-        Detect same type attributes in order to merge them together with their
-        restrictions.
+        Detect and process duplicate attributes.
 
-        Two attributes are considered equal if they have the same name,
-        tag and namespace.
+        - Remove duplicates for enumerations.
+        - Merge duplicates with restrictions and types.
         """
+        if target.is_enumeration:
+            cls.filter_duplicate_attrs(target)
+        else:
+            cls.merge_duplicate_attrs(target)
+
+    @classmethod
+    def filter_duplicate_attrs(cls, target: Class):
+        attrs = collections.unique_sequence(target.attrs, key="default")
+        target.attrs = attrs
+
+    @classmethod
+    def merge_duplicate_attrs(self, target: Class):
         result: List[Attr] = []
         for attr in target.attrs:
             pos = collections.find(result, attr)
             existing = result[pos] if pos > -1 else None
 
             if not existing:
                 result.append(attr)
@@ -37,13 +48,16 @@
                 min_occurs = e_res.min_occurs or 0
                 max_occurs = e_res.max_occurs or 1
                 attr_min_occurs = a_res.min_occurs or 0
                 attr_max_occurs = a_res.max_occurs or 1
 
                 e_res.min_occurs = min(min_occurs, attr_min_occurs)
                 e_res.max_occurs = max_occurs + attr_max_occurs
-                e_res.sequential = a_res.sequential or e_res.sequential
+
+                if a_res.sequence is not None:
+                    e_res.sequence = a_res.sequence
+
                 existing.fixed = False
                 existing.types.extend(attr.types)
 
         target.attrs = result
         ClassUtils.cleanup_class(target)
```

### Comparing `xsdata-22.9/xsdata/codegen/handlers/process_attributes_types.py` & `xsdata-23.5/xsdata/codegen/handlers/process_attributes_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,17 @@
         """Process the given class attributes and their types."""
         for attr in list(target.attrs):
             self.process_types(target, attr)
             self.cascade_properties(target, attr)
 
     def process_types(self, target: Class, attr: Attr):
         """Process every attr type and filter out duplicates."""
+        if self.container.config.output.ignore_patterns:
+            attr.restrictions.pattern = None
+
         for attr_type in list(attr.types):
             self.process_type(target, attr, attr_type)
 
         attr.types = ClassUtils.filter_types(attr.types)
 
     @classmethod
     def cascade_properties(cls, target: Class, attr: Attr):
@@ -104,15 +107,14 @@
 
     def process_inner_type(self, target: Class, attr: Attr, attr_type: AttrType):
         """
         Process an attributes type that depends on an inner type.
 
         Ignore inner circular references.
         """
-
         if attr_type.circular:
             return
 
         inner = self.container.find_inner(target, attr_type.qname)
         if inner.is_simple_type:
             self.copy_attribute_properties(inner, target, attr, attr_type)
             target.inner.remove(inner)
@@ -123,15 +125,14 @@
 
         Strategies:
             1. Reset absent types with a warning
             2. Copy attribute properties from a simple type
             3. Copy format restriction from an enumeration
             4. Set circular flag for the rest
         """
-
         source = self.find_dependency(attr_type, attr.tag)
         if not source:
             logger.warning("Reset absent type: %s", attr_type.name)
             use_str = not source or not source.is_complex
             self.reset_attribute_type(attr_type, use_str)
         elif source.is_simple_type:
             self.copy_attribute_properties(source, target, attr, attr_type)
@@ -191,14 +192,17 @@
         attr.default = attr.default or source_attr.default
 
     def set_circular_flag(self, source: Class, target: Class, attr_type: AttrType):
         """Update circular reference flag."""
         attr_type.reference = id(source)
         attr_type.circular = self.is_circular_dependency(source, target, set())
 
+        if attr_type.circular:
+            logger.debug("Possible circular reference %s, %s", target.name, source.name)
+
     def is_circular_dependency(self, source: Class, target: Class, seen: Set) -> bool:
         """Check if any source dependencies recursively match the target
         class."""
 
         if source is target or source.status == Status.FLATTENING:
             return True
```

### Comparing `xsdata-22.9/xsdata/codegen/handlers/process_mixed_content_class.py` & `xsdata-23.5/xsdata/codegen/handlers/process_mixed_content_class.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         for attr in list(target.attrs):
             if attr.is_attribute:
                 attrs.append(attr)
             elif attr.tag != Tag.ANY:
                 choice = attr.clone()
                 choice.restrictions.min_occurs = None
                 choice.restrictions.max_occurs = None
-                choice.restrictions.sequential = None
+                choice.restrictions.sequence = None
                 choices.append(choice)
 
         wildcard = Attr(
             name="content",
             types=[AttrType(qname=str(DataType.ANY_TYPE), native=True)],
             tag=Tag.ANY,
             mixed=True,
```

### Comparing `xsdata-22.9/xsdata/codegen/handlers/rename_duplicate_attributes.py` & `xsdata-23.5/xsdata/codegen/handlers/rename_duplicate_attributes.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/xsdata/codegen/handlers/rename_duplicate_classes.py` & `xsdata-23.5/xsdata/codegen/handlers/rename_duplicate_classes.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/xsdata/codegen/handlers/sanitize_attributes_default_value.py` & `xsdata-23.5/xsdata/codegen/handlers/sanitize_attributes_default_value.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 class SanitizeAttributesDefaultValue(RelativeHandlerInterface):
     """
     Sanitize attributes default values.
 
     Cases:
         1. Ignore enumerations.
         2. List fields can not have a default value
-        3. Optional choice/sequential fields can not have a default value
+        3. Optional choice/sequence fields can not have a default value
         4. xsi:type fields are ignored, mark them as optional
         5. Convert string literal default value for enum fields.
     """
 
     __slots__ = ()
 
     def process(self, target: Class):
@@ -98,22 +98,20 @@
 
     @classmethod
     def is_valid_enum_type(cls, source: Class, attr: Attr) -> bool:
         """
         Convert string literal default values to enumeration members
         placeholders and return result.
 
-        The placeholders will be converted to proper references
-        from the generator filters.
+        The placeholders will be converted to proper references from the
+        generator filters.
 
-        Placeholder examples:
-            Single -> @enum@qname::member_name
-            Multiple -> @enum@qname::first_member@second_member
+        Placeholder examples: Single -> @enum@qname::member_name
+        Multiple -> @enum@qname::first_member@second_member
         """
-
         assert attr.default is not None
 
         value_members = {x.default: x.name for x in source.attrs}
         name = value_members.get(attr.default)
         if name:
             attr.default = f"@enum@{source.qname}::{name}"
             return True
@@ -168,38 +166,36 @@
         )
 
     @classmethod
     def should_reset_required(cls, attr: Attr) -> bool:
         """
         Return whether the min occurrences for the attr needs to be reset.
 
-        Cases:
-            1. xs:any(Simple)Type, with no default value that's not a list already!
+        @Todo figure out if wildcards are supposed to be optional!
         """
-        return attr.default is None and object in attr.native_types and not attr.is_list
+        return (
+            not attr.is_attribute
+            and attr.default is None
+            and object in attr.native_types
+            and not attr.is_list
+        )
 
     @classmethod
     def should_reset_default(cls, attr: Attr) -> bool:
         """
         Return whether we should unset the default value of the attribute.
 
         - Default value is not set
         - Attribute is xsi:type (ignorable)
         - Attribute is part of a choice
         """
         return attr.default is not None and (
             attr.is_xsi_type
             or attr.is_list
-            or (
-                attr.is_optional
-                and (
-                    attr.restrictions.sequential is True
-                    or attr.restrictions.choice is not None
-                )
-            )
+            or (not attr.is_attribute and attr.is_optional)
         )
 
     @classmethod
     def reset_attribute_types(cls, attr: Attr):
         attr.types.clear()
         attr.types.append(AttrType(qname=str(DataType.STRING), native=True))
         attr.restrictions.format = None
```

### Comparing `xsdata-22.9/xsdata/codegen/handlers/sanitize_enumeration_class.py` & `xsdata-23.5/xsdata/codegen/handlers/sanitize_enumeration_class.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/xsdata/codegen/handlers/unnest_inner_classes.py` & `xsdata-23.5/xsdata/codegen/handlers/unnest_inner_classes.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/xsdata/codegen/handlers/vacuum_inner_classes.py` & `xsdata-23.5/xsdata/codegen/handlers/vacuum_inner_classes.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/xsdata/codegen/handlers/validate_attributes_overrides.py` & `xsdata-23.5/xsdata/codegen/handlers/validate_attributes_overrides.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,32 +20,40 @@
         2. The attribute is unnecessary remove it
         3. The attribute is an invalid override, rename one of them
     """
 
     __slots__ = ()
 
     def process(self, target: Class):
-
         base_attrs_map = self.base_attrs_map(target)
         for attr in list(target.attrs):
             base_attrs = base_attrs_map.get(attr.slug)
 
             if base_attrs:
                 base_attr = base_attrs[0]
-                if attr.tag == base_attr.tag:
+                if self.overrides(attr, base_attr):
                     self.validate_override(target, attr, base_attr)
                 else:
                     self.resolve_conflict(attr, base_attr)
+            elif attr.is_prohibited:
+                self.remove_attribute(target, attr)
+
+    @classmethod
+    def overrides(cls, a: Attr, b: Attr) -> bool:
+        return a.xml_type == b.xml_type and a.namespace == b.namespace
 
     def base_attrs_map(self, target: Class) -> Dict[str, List[Attr]]:
         base_attrs = self.base_attrs(target)
         return collections.group_by(base_attrs, key=get_slug)
 
     @classmethod
     def validate_override(cls, target: Class, attr: Attr, source_attr: Attr):
+        if source_attr.is_any_type and not attr.is_any_type:
+            return
+
         if attr.is_list and not source_attr.is_list:
             # Hack much??? idk but Optional[str] can't override List[str]
             source_attr.restrictions.max_occurs = sys.maxsize
 
         if (
             attr.default == source_attr.default
             and bool_eq(attr.fixed, source_attr.fixed)
```

### Comparing `xsdata-22.9/xsdata/codegen/mappers/definitions.py` & `xsdata-23.5/xsdata/codegen/mappers/definitions.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,14 @@
 
         if operation.output:
             messages.append(
                 ("output", operation.output, port_type_operation.output, None)
             )
 
         for suffix, binding_message, port_type_message, operation_name in messages:
-
             if style == "rpc":
                 yield cls.build_message_class(definitions, port_type_message)
 
             target = cls.build_envelope_class(
                 definitions,
                 binding_message,
                 port_type_message,
```

### Comparing `xsdata-22.9/xsdata/codegen/mappers/dict.py` & `xsdata-23.5/xsdata/codegen/mappers/dict.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 class DictMapper:
     """Map a dictionary to classes, extensions and attributes."""
 
     @classmethod
     def map(cls, data: Dict, name: str, location: str) -> List[Class]:
         """Convert a dictionary to a list of codegen classes."""
-
         target = cls.build_class(data, name)
         return list(ClassUtils.flatten(target, f"{location}/{name}"))
 
     @classmethod
     def build_class(cls, data: Dict, name: str) -> Class:
         target = Class(qname=name, tag=Tag.ELEMENT, location="")
```

### Comparing `xsdata-22.9/xsdata/codegen/mappers/dtd.py` & `xsdata-23.5/xsdata/codegen/mappers/dtd.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from xsdata.models.dtd import DtdContent
 from xsdata.models.dtd import DtdContentOccur
 from xsdata.models.dtd import DtdContentType
 from xsdata.models.dtd import DtdElement
 from xsdata.models.dtd import DtdElementType
 from xsdata.models.enums import DataType
 from xsdata.models.enums import Tag
+from xsdata.utils.constants import DEFAULT_ATTR_NAME
 
 
 class DtdMapper:
     @classmethod
     def map(cls, dtd: Dtd) -> Iterator[Class]:
         for element in dtd.elements:
             yield cls.build_class(element, dtd.location)
@@ -93,80 +94,118 @@
         return AttrType(qname=str(attribute.data_type), native=True)
 
     @classmethod
     def build_elements(cls, target: Class, element: DtdElement):
         # "undefined", "empty", "any", "mixed", or "element";
         if element.type == DtdElementType.ELEMENT and element.content:
             cls.build_content(target, element.content)
-        elif element.type == DtdElementType.MIXED:
-            target.tag = Tag.COMPLEX_TYPE
-            cls.build_extension(target, DataType.STRING)
+        elif element.type == DtdElementType.MIXED and element.content:
+            cls.build_mixed_content(target, element.content)
         elif element.type == DtdElementType.ANY:
             cls.build_extension(target, DataType.ANY_TYPE)
 
     @classmethod
+    def build_mixed_content(cls, target: Class, content: DtdContent):
+        if content.left and content.left.type == DtdContentType.PCDATA:
+            target.mixed = True
+            content.left = None
+        elif content.right and content.right.type == DtdContentType.PCDATA:
+            target.mixed = True
+            content.right = None
+
+        target.tag = Tag.COMPLEX_TYPE
+        cls.build_content(target, content)
+
+    @classmethod
     def build_extension(cls, target: Class, data_type: DataType):
         ext_type = AttrType(qname=str(data_type), native=True)
-        extension = Extension(type=ext_type, restrictions=Restrictions())
+        extension = Extension(
+            tag=Tag.EXTENSION, type=ext_type, restrictions=Restrictions()
+        )
         target.extensions.append(extension)
 
     @classmethod
     def build_content(cls, target: Class, content: DtdContent, **kwargs: Any):
         content_type = content.type
         if content_type == DtdContentType.ELEMENT:
             restrictions = cls.build_restrictions(content.occur, **kwargs)
             cls.build_element(target, content.name, restrictions)
         elif content_type == DtdContentType.SEQ:
             cls.build_content_tree(target, content, **kwargs)
         elif content_type == DtdContentType.OR:
-            params = {"min_occurs": 0, "choice": str(id(content))}
-            params.update(kwargs)
+            params = cls.build_occurs(content.occur)
+            params.update(
+                {
+                    "choice": id(content),
+                    "min_occurs": 0,
+                }
+            )
+            params.update(**kwargs)
             cls.build_content_tree(target, content, **params)
+        else:  # content_type == DtdContentType.PCDATA:
+            restrictions = cls.build_restrictions(content.occur, **kwargs)
+            cls.build_value(target, restrictions)
 
     @classmethod
     def build_content_tree(cls, target: Class, content: DtdContent, **kwargs: Any):
         if content.left:
             cls.build_content(target, content.left, **kwargs)
 
         if content.right:
             cls.build_content(target, content.right, **kwargs)
 
     @classmethod
-    def build_restrictions(cls, occur: DtdContentOccur, **kwargs: Any) -> Restrictions:
+    def build_occurs(cls, occur: DtdContentOccur) -> Dict:
         if occur == DtdContentOccur.ONCE:
             min_occurs = 1
             max_occurs = 1
         elif occur == DtdContentOccur.OPT:
             min_occurs = 0
             max_occurs = 1
         elif occur == DtdContentOccur.MULT:
             min_occurs = 0
             max_occurs = sys.maxsize
         else:  # occur == DtdContentOccur.PLUS:
             min_occurs = 1
             max_occurs = sys.maxsize
 
-        params: Dict[str, Any] = {
+        return {
             "min_occurs": min_occurs,
             "max_occurs": max_occurs,
         }
+
+    @classmethod
+    def build_restrictions(cls, occur: DtdContentOccur, **kwargs: Any) -> Restrictions:
+        params = cls.build_occurs(occur)
         params.update(kwargs)
 
         return Restrictions(**params)
 
     @classmethod
     def build_element(cls, target: Class, name: str, restrictions: Restrictions):
         types = AttrType(qname=name, native=False)
         attr = Attr(
             name=name, tag=Tag.ELEMENT, types=[types], restrictions=restrictions.clone()
         )
         attr.index = len(target.attrs)
         target.attrs.append(attr)
 
     @classmethod
+    def build_value(cls, target: Class, restrictions: Restrictions):
+        types = AttrType(qname=str(DataType.STRING), native=True)
+        attr = Attr(
+            name=DEFAULT_ATTR_NAME,
+            tag=Tag.EXTENSION,
+            types=[types],
+            restrictions=restrictions.clone(),
+        )
+        attr.index = len(target.attrs)
+        target.attrs.append(attr)
+
+    @classmethod
     def build_enumeration(cls, target: Class, name: str, values: List[str]):
         inner = Class(qname=name, tag=Tag.SIMPLE_TYPE, location=target.location)
         attr_type = AttrType(qname=str(DataType.STRING), native=True)
 
         for value in values:
             inner.attrs.append(
                 Attr(
```

### Comparing `xsdata-22.9/xsdata/codegen/mappers/element.py` & `xsdata-23.5/xsdata/codegen/mappers/element.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import sys
 from collections import defaultdict
 from typing import Any
 from typing import List
 from typing import Optional
-from typing import Set
 
 from xsdata.codegen.models import Attr
 from xsdata.codegen.models import AttrType
 from xsdata.codegen.models import Class
 from xsdata.codegen.utils import ClassUtils
 from xsdata.formats.converter import converter
 from xsdata.formats.dataclass.models.generics import AnyElement
@@ -21,15 +20,14 @@
 
 class ElementMapper:
     """Map a schema instance to classes, extensions and attributes."""
 
     @classmethod
     def map(cls, element: AnyElement, location: str) -> List[Class]:
         """Map schema children elements to classes."""
-
         assert element.qname is not None
 
         uri, name = split_qname(element.qname)
         target = cls.build_class(element, uri)
 
         return list(ClassUtils.flatten(target, f"{location}/{name}"))
 
@@ -53,47 +51,45 @@
         return target
 
     @classmethod
     def build_attributes(
         cls, target: Class, element: AnyElement, namespace: Optional[str]
     ):
         for key, value in element.attributes.items():
-
             if key == QNames.XSI_NIL:
                 target.nillable = value.strip() in ("true", "1")
             else:
                 attr_type = cls.build_attribute_type(key, value)
                 cls.build_attribute(target, key, attr_type, namespace, Tag.ATTRIBUTE)
 
     @classmethod
     def build_elements(
         cls, target: Class, element: AnyElement, namespace: Optional[str]
     ):
-        sequential_set = cls.sequential_names(element)
-        for child in element.children:
+        sequences = cls.sequential_groups(element)
+        for index, child in enumerate(element.children):
             if isinstance(child, AnyElement) and child.qname:
                 if child.tail:
                     target.mixed = True
 
                 if child.attributes or child.children:
                     inner = cls.build_class(child, namespace)
                     attr_type = AttrType(qname=inner.qname, forward=True)
                     target.inner.append(inner)
                 else:
                     attr_type = cls.build_attribute_type(child.qname, child.text)
 
-                sequential = child.qname in sequential_set
-
+                sequence = collections.find_connected_component(sequences, index)
                 cls.build_attribute(
                     target,
                     child.qname,
                     attr_type,
                     namespace,
                     Tag.ELEMENT,
-                    sequential,
+                    sequence + 1,
                 )
 
     @classmethod
     def build_text(cls, target: Class, element: AnyElement):
         if element.text:
             attr_type = cls.build_attribute_type("value", element.text)
             cls.build_attribute(target, "value", attr_type, None, Tag.SIMPLE_TYPE)
@@ -126,39 +122,39 @@
     def build_attribute(
         cls,
         target: Class,
         qname: str,
         attr_type: AttrType,
         parent_namespace: Optional[str] = None,
         tag: str = Tag.ELEMENT,
-        sequential: bool = False,
+        sequence: int = 0,
     ):
-
         namespace, name = split_qname(qname)
         namespace = cls.select_namespace(namespace, parent_namespace, tag)
         index = len(target.attrs)
 
         attr = Attr(index=index, name=name, tag=tag, namespace=namespace)
         attr.types.append(attr_type)
-        attr.restrictions.sequential = sequential or None
-        attr.restrictions.min_occurs = 0
+
+        if sequence:
+            attr.restrictions.path.append(("s", sequence, 1, sys.maxsize))
+
+        attr.restrictions.min_occurs = 1
         attr.restrictions.max_occurs = 1
         cls.add_attribute(target, attr)
 
     @classmethod
     def add_attribute(cls, target: Class, attr: Attr):
         pos = collections.find(target.attrs, attr)
 
         if pos > -1:
             existing = target.attrs[pos]
             existing.restrictions.max_occurs = sys.maxsize
             existing.types.extend(attr.types)
-
-            if attr.restrictions.sequential:
-                existing.restrictions.sequential = True
+            existing.types = collections.unique_sequence(existing.types, key="qname")
         else:
             target.attrs.append(attr)
 
     @classmethod
     def select_namespace(
         cls,
         namespace: Optional[str],
@@ -170,26 +166,25 @@
 
         if namespace is None and parent_namespace is not None:
             return ""
 
         return namespace
 
     @classmethod
-    def sequential_names(cls, element: AnyElement) -> Set[str]:
-        mapping = defaultdict(list)
-        names = [
-            child.qname
-            for child in element.children
-            if isinstance(child, AnyElement) and child.qname
-        ]
-        indices: Set[int] = set()
-
-        for index, name in enumerate(names):
-            mapping[name].append(index)
+    def sequential_groups(cls, element: AnyElement) -> List[List[int]]:
+        groups = cls.group_repeating_attrs(element)
+        return list(collections.connected_components(groups))
 
-        for pos in mapping.values():
-            total = len(pos)
+    @classmethod
+    def group_repeating_attrs(cls, element: AnyElement) -> List[List[int]]:
+        counters = defaultdict(list)
+        for index, child in enumerate(element.children):
+            if isinstance(child, AnyElement) and child.qname:
+                counters[child.qname].append(index)
 
-            if 1 < total < pos[-1] - pos[0] + 1:
-                indices.update(list(range(pos[0], pos[-1] + 1)))
+        groups = []
+        if len(counters) > 1:
+            for x in counters.values():
+                if len(x) > 1:
+                    groups.append(list(range(x[0], x[-1] + 1)))
 
-        return {names[index] for index in indices}
+        return groups
```

### Comparing `xsdata-22.9/xsdata/codegen/mappers/schema.py` & `xsdata-23.5/xsdata/codegen/mappers/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 
 class SchemaMapper:
     """Map a schema instance to classes, extensions and attributes."""
 
     @classmethod
     def map(cls, schema: Schema) -> List[Class]:
         """Map schema children elements to classes."""
-
         assert schema.location is not None
 
         location = schema.location
         target_namespace = schema.target_namespace
 
         return [
             cls.build_class(element, container, location, target_namespace)
@@ -111,15 +110,16 @@
     @classmethod
     def build_class_extensions(cls, obj: ElementBase, target: Class):
         """Build the item class extensions from the given ElementBase
         children."""
 
         restrictions = obj.get_restrictions()
         extensions = [
-            cls.build_class_extension(target, base, restrictions) for base in obj.bases
+            cls.build_class_extension(obj.class_name, target, base, restrictions)
+            for base in obj.bases
         ]
         extensions.extend(cls.children_extensions(obj, target))
         target.extensions = collections.unique_sequence(extensions)
 
     @classmethod
     def build_data_type(
         cls, target: Class, name: str, forward: bool = False
@@ -143,16 +143,16 @@
         """Recursively find and return all child elements that are qualified to
         be class attributes, with all their restrictions."""
 
         for child in obj.children():
             if child.is_property:
                 yield child, parent_restrictions
             else:
-                restrictions = parent_restrictions.clone()
-                restrictions.merge(Restrictions.from_element(child))
+                restrictions = Restrictions.from_element(child)
+                restrictions.merge(parent_restrictions)
                 yield from cls.element_children(child, restrictions)
 
     @classmethod
     def element_namespace(
         cls, obj: ElementBase, target_namespace: Optional[str]
     ) -> Optional[str]:
         """
@@ -195,25 +195,28 @@
         result.
         """
         for child in obj.children():
             if child.is_property:
                 continue
 
             for ext in child.bases:
-                yield cls.build_class_extension(target, ext, child.get_restrictions())
+                yield cls.build_class_extension(
+                    child.class_name, target, ext, child.get_restrictions()
+                )
 
             yield from cls.children_extensions(child, target)
 
     @classmethod
     def build_class_extension(
-        cls, target: Class, name: str, restrictions: Dict
+        cls, tag: str, target: Class, name: str, restrictions: Dict
     ) -> Extension:
         """Create an extension for the target class."""
         return Extension(
             type=cls.build_data_type(target, name),
+            tag=tag,
             restrictions=Restrictions(**restrictions),
         )
 
     @classmethod
     def build_class_attribute(
         cls,
         target: Class,
@@ -225,17 +228,14 @@
         target.ns_map.update(obj.ns_map)
         types = cls.build_class_attribute_types(target, obj)
         restrictions = Restrictions.from_element(obj)
 
         if obj.class_name in (Tag.ELEMENT, Tag.ANY, Tag.GROUP):
             restrictions.merge(parent_restrictions)
 
-        if restrictions.is_prohibited:
-            return
-
         name = obj.real_name
         target.attrs.append(
             Attr(
                 index=obj.index,
                 name=name,
                 default=obj.default_value,
                 fixed=obj.is_fixed,
```

### Comparing `xsdata-22.9/xsdata/codegen/mixins.py` & `xsdata-23.5/xsdata/codegen/mixins.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/xsdata/codegen/models.py` & `xsdata-23.5/xsdata/codegen/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from dataclasses import replace
 from enum import IntEnum
 from typing import Any
 from typing import Dict
 from typing import Iterator
 from typing import List
 from typing import Optional
+from typing import Tuple
 from typing import Type
 
 from xsdata.exceptions import CodeGenerationError
 from xsdata.formats.converter import converter
 from xsdata.formats.dataclass.models.elements import XmlType
 from xsdata.models.enums import DataType
 from xsdata.models.enums import Namespace
@@ -50,15 +51,15 @@
     :param total_digits:
     :param fraction_digits:
     :param length:
     :param white_space:
     :param pattern:
     :param explicit_timezone:
     :param nillable:
-    :param sequential:
+    :param sequence:
     :param tokens:
     :param format:
     :param choice:
     """
 
     min_occurs: Optional[int] = field(default=None)
     max_occurs: Optional[int] = field(default=None)
@@ -71,18 +72,20 @@
     total_digits: Optional[int] = field(default=None)
     fraction_digits: Optional[int] = field(default=None)
     length: Optional[int] = field(default=None)
     white_space: Optional[str] = field(default=None)
     pattern: Optional[str] = field(default=None)
     explicit_timezone: Optional[str] = field(default=None)
     nillable: Optional[bool] = field(default=None)
-    sequential: Optional[bool] = field(default=None)
+    sequence: Optional[int] = field(default=None)
     tokens: Optional[bool] = field(default=None)
     format: Optional[str] = field(default=None)
-    choice: Optional[str] = field(default=None)
+    choice: Optional[int] = field(default=None)
+    group: Optional[int] = field(default=None)
+    path: List[Tuple[str, int, int, int]] = field(default_factory=list)
 
     @property
     def is_list(self) -> bool:
         """Return true if max occurs property is larger than one."""
         return self.max_occurs is not None and self.max_occurs > 1
 
     @property
@@ -92,37 +95,28 @@
 
     @property
     def is_prohibited(self) -> bool:
         return self.max_occurs == 0
 
     def merge(self, source: "Restrictions"):
         """Update properties from another instance."""
-
         self.update(source)
 
-        min_occurs = source.min_occurs
-        max_occurs = source.max_occurs
-        is_list = max_occurs is not None and max_occurs > 1
-
-        # Update the sequential flag if new value is true and restrictions indicate
-        # the field was and still is a list.
-        if source.sequential and (is_list or not self.is_list):
-            self.sequential = source.sequential
-
-        self.choice = source.choice or self.choice
-        self.tokens = source.tokens or self.tokens
-        self.format = source.format or self.format
-
-        # Update min occurs if current value is None or the new value is more than one.
-        if self.min_occurs is None or (min_occurs is not None and min_occurs != 1):
-            self.min_occurs = min_occurs
-
-        # Update max occurs if current value is None or the new value is more than one.
-        if self.max_occurs is None or (max_occurs is not None and max_occurs != 1):
-            self.max_occurs = max_occurs
+        self.path = source.path + self.path
+        self.sequence = self.sequence or source.sequence
+        self.choice = self.choice or source.choice
+        self.tokens = self.tokens or source.tokens
+        self.format = self.format or source.format
+        self.group = self.group or source.group
+
+        if self.min_occurs is None and source.min_occurs is not None:
+            self.min_occurs = source.min_occurs
+
+        if self.max_occurs is None and source.max_occurs is not None:
+            self.max_occurs = source.max_occurs
 
     def update(self, source: "Restrictions"):
         keys = (
             "min_exclusive",
             "min_inclusive",
             "min_length",
             "max_exclusive",
@@ -144,28 +138,33 @@
     def asdict(self, types: Optional[List[Type]] = None) -> Dict:
         """
         Return the initialized only properties as a dictionary.
 
         Skip None or implied values, and optionally use the parent
         attribute types to convert relevant options.
         """
-
         result = {}
         sorted_types = converter.sort_types(types) if types else []
 
         if self.is_list:
             if self.min_occurs is not None and self.min_occurs > 0:
                 result["min_occurs"] = self.min_occurs
             if self.max_occurs is not None and self.max_occurs < sys.maxsize:
                 result["max_occurs"] = self.max_occurs
         elif self.min_occurs == self.max_occurs == 1 and not self.nillable:
             result["required"] = True
 
         for key, value in asdict(self).items():
-            if value is None or key in ("choice", "min_occurs", "max_occurs"):
+            if value is None or key in (
+                "choice",
+                "group",
+                "min_occurs",
+                "max_occurs",
+                "path",
+            ):
                 continue
 
             if key.endswith("clusive") and types:
                 value = converter.deserialize(value, sorted_types)
 
             result[key] = value
 
@@ -263,14 +262,18 @@
     help: Optional[str] = field(default=None, compare=False)
     restrictions: Restrictions = field(default_factory=Restrictions, compare=False)
 
     def __post_init__(self):
         self.local_name = self.name
 
     @property
+    def key(self) -> str:
+        return f"{self.tag}.{self.namespace}.{self.local_name}"
+
+    @property
     def is_attribute(self) -> bool:
         """Return whether this attribute is derived from an xs:attribute or
         xs:anyAttribute."""
         return self.tag in (Tag.ATTRIBUTE, Tag.ANY_ATTRIBUTE)
 
     @property
     def is_enumeration(self) -> bool:
@@ -295,14 +298,19 @@
 
     @property
     def is_list(self) -> bool:
         """Return whether this attribute is a list of values."""
         return self.restrictions.is_list
 
     @property
+    def is_prohibited(self) -> bool:
+        """Return whether this attribute is prohibited."""
+        return self.restrictions.is_prohibited
+
+    @property
     def is_nameless(self) -> bool:
         """Return whether this attribute has a local name that will be used
         during parsing/serialization."""
         return self.tag not in (Tag.ATTRIBUTE, Tag.ELEMENT)
 
     @property
     def is_nillable(self) -> bool:
@@ -333,23 +341,21 @@
     @property
     def is_wildcard(self) -> bool:
         """Return whether this attribute is derived from xs:anyAttribute or
         xs:any."""
         return self.tag in (Tag.ANY_ATTRIBUTE, Tag.ANY)
 
     @property
+    def is_any_type(self) -> bool:
+        return any(tp is object for tp in self.get_native_types())
+
+    @property
     def native_types(self) -> List[Type]:
         """Return a list of all builtin data types."""
-        result = set()
-        for tp in self.types:
-            datatype = tp.datatype
-            if datatype:
-                result.add(datatype.type)
-
-        return list(result)
+        return list(set(self.get_native_types()))
 
     @property
     def user_types(self) -> Iterator[AttrType]:
         """Return an iterator of all the user defined types."""
         for tp in self.types:
             if not tp.native:
                 yield tp
@@ -367,46 +373,56 @@
         """Return a deep cloned instance."""
         return replace(
             self,
             types=[x.clone() for x in self.types],
             restrictions=self.restrictions.clone(),
         )
 
+    def get_native_types(self) -> Iterator[Type]:
+        for tp in self.types:
+            datatype = tp.datatype
+            if datatype:
+                yield datatype.type
+
 
 @dataclass(unsafe_hash=True)
 class Extension:
     """
     Model representation of a dataclass base class.
 
+    :param tag:
     :param type:
     :param restrictions:
     """
 
+    tag: str
     type: AttrType
     restrictions: Restrictions = field(hash=False)
 
     def clone(self) -> "Extension":
         """Return a deep cloned instance."""
         return replace(
             self,
             type=self.type.clone(),
             restrictions=self.restrictions.clone(),
         )
 
 
 class Status(IntEnum):
     RAW = 0
-    FLATTENING = 10
-    FLATTENED = 11
-    SANITIZING = 20
-    SANITIZED = 21
-    RESOLVING = 30
-    RESOLVED = 31
-    FINALIZING = 40
-    FINALIZED = 41
+    UNGROUPING = 10
+    UNGROUPED = 11
+    FLATTENING = 20
+    FLATTENED = 21
+    SANITIZING = 30
+    SANITIZED = 31
+    RESOLVING = 40
+    RESOLVED = 41
+    FINALIZING = 50
+    FINALIZED = 51
 
 
 @dataclass
 class Class:
     """
     Model representation of a dataclass with fields, base/inner classes and
     additional metadata settings.
@@ -587,15 +603,14 @@
             * base classes
             * attribute types
             * attribute choice types
             * recursively go through the inner classes
             * Ignore inner class references
             * Ignore native types.
         """
-
         types = {ext.type for ext in self.extensions}
 
         for attr in self.attrs:
             types.update(attr.types)
             types.update(tp for choice in attr.choices for tp in choice.types)
 
         for tp in types:
@@ -632,11 +647,12 @@
 
 # Getters used all over the codegen process
 get_location = operator.attrgetter("location")
 get_name = operator.attrgetter("name")
 get_qname = operator.attrgetter("qname")
 get_tag = operator.attrgetter("tag")
 get_restriction_choice = operator.attrgetter("restrictions.choice")
+get_restriction_sequence = operator.attrgetter("restrictions.sequence")
 get_slug = operator.attrgetter("slug")
 get_target_namespace = operator.attrgetter("target_namespace")
 is_enumeration = operator.attrgetter("is_enumeration")
 is_group = operator.attrgetter("is_group")
```

### Comparing `xsdata-22.9/xsdata/codegen/parsers/definitions.py` & `xsdata-23.5/xsdata/codegen/parsers/definitions.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/xsdata/codegen/parsers/dtd.py` & `xsdata-23.5/xsdata/codegen/parsers/dtd.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,14 @@
         )
 
     @classmethod
     def build_ns_map(cls, prefix: str, attributes: List[DtdAttribute]) -> dict:
         ns_map = {ns.prefix: ns.uri for ns in Namespace.common()}
 
         for attribute in list(attributes):
-
             if not attribute.default_value:
                 continue
 
             if attribute.prefix == "xmlns":
                 ns_map[attribute.name] = attribute.default_value
                 attributes.remove(attribute)
             elif attribute.name == "xmlns":
```

### Comparing `xsdata-22.9/xsdata/codegen/parsers/schema.py` & `xsdata-23.5/xsdata/codegen/parsers/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 @dataclass
 class SchemaParser(UserXmlParser):
     """
     A simple parser to convert an xsd schema to an easy to handle data
     structure based on dataclasses.
 
-    The parser is a dummy as possible but it will try to normalize
+    The parser is as a dummy as possible, but it will try to normalize
     certain things like apply parent properties to children.
 
     :param location:
     :param element_form:
     :param attribute_form:
     :param target_namespace:
     :param default_attributes:
@@ -230,15 +230,14 @@
             for child in obj.children()
         )
 
     @classmethod
     def set_namespace_map(cls, obj: Any, ns_map: Optional[Dict]):
         """Add common namespaces like xml, xsi, xlink if they are missing."""
         if hasattr(obj, "ns_map"):
-
             if ns_map:
                 obj.ns_map.update(
                     {prefix: uri for prefix, uri in ns_map.items() if uri}
                 )
 
             ns_list = obj.ns_map.values()
             obj.ns_map.update(
```

### Comparing `xsdata-22.9/xsdata/codegen/resolver.py` & `xsdata-23.5/xsdata/codegen/resolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from xsdata.exceptions import ResolverValueError
 from xsdata.utils import collections
 
 logger = logging.getLogger(__name__)
 
 
 class DependenciesResolver:
-
     __slots__ = "packages", "aliases", "imports", "class_list", "class_map", "package"
 
     def __init__(self, packages: Dict[str, str]):
         self.packages = packages
 
         self.aliases: Dict[str, str] = {}
         self.imports: List[Import] = []
@@ -122,15 +121,14 @@
     def create_class_list(classes: List[Class]) -> List[str]:
         """Use topology sort to return a flat list for all the dependencies."""
         return toposort_flatten({obj.qname: set(obj.dependencies()) for obj in classes})
 
     @staticmethod
     def create_class_map(classes: List[Class]) -> Dict[str, Class]:
         """Index the list of classes by name."""
-
         result: Dict[str, Class] = {}
         for obj in classes:
             if obj.qname in result:
                 raise ResolverValueError(f"Duplicate class: `{obj.name}`")
             result[obj.qname] = obj
 
         return result
```

### Comparing `xsdata-22.9/xsdata/codegen/transformer.py` & `xsdata-23.5/xsdata/codegen/transformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+import hashlib
 import io
 import json
 import os
+import pickle
+import tempfile
 from collections import defaultdict
+from pathlib import Path
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import NamedTuple
 from typing import Optional
 from typing import Tuple
 from urllib.request import urlopen
@@ -95,26 +99,39 @@
     def __init__(self, print: bool, config: GeneratorConfig):
         self.print = print
         self.config = config
         self.classes: List[Class] = []
         self.processed: List[str] = []
         self.preloaded: Dict = {}
 
-    def process(self, uris: List[str]):
+    def process(self, uris: List[str], cache: bool = False):
+        cache_file = self.get_cache_file(uris) if cache else None
+        if cache_file and cache_file.exists():
+            logger.info(f"Loading from cache {cache_file}")
+
+            self.classes = pickle.loads(cache_file.read_bytes())
+        else:
+            self.process_sources(uris)
+
+        if cache_file and not cache_file.exists():
+            cache_file.write_bytes(pickle.dumps(self.classes))
+
+        self.process_classes()
+
+    def process_sources(self, uris: List[str]):
         sources = defaultdict(list)
         for uri in uris:
             tp = self.classify_resource(uri)
             sources[tp].append(uri)
 
         self.process_definitions(sources[TYPE_DEFINITION])
         self.process_schemas(sources[TYPE_SCHEMA])
         self.process_dtds(sources[TYPE_DTD])
         self.process_xml_documents(sources[TYPE_XML])
         self.process_json_documents(sources[TYPE_JSON])
-        self.process_classes()
 
     def process_definitions(self, uris: List[str]):
         """Process a list of wsdl resources."""
         definitions = None
         for uri in uris:
             services = self.parse_definitions(uri, namespace=None)
             if definitions is None:
@@ -149,44 +166,45 @@
         """Parse and convert schema to codegen models."""
         schema = self.parse_schema(uri, namespace)
         if schema:
             self.convert_schema(schema)
 
     def process_xml_documents(self, uris: List[str]):
         """Process a list of xml resources."""
-
         classes = []
         parser = TreeParser()
         location = os.path.dirname(uris[0]) if uris else ""
         for uri in uris:
             input_stream = self.load_resource(uri)
             if input_stream:
                 logger.info("Parsing document %s", uri)
                 any_element: AnyElement = parser.from_bytes(input_stream)
                 classes.extend(ElementMapper.map(any_element, location))
 
         self.classes.extend(ClassUtils.reduce_classes(classes))
 
     def process_json_documents(self, uris: List[str]):
         """Process a list of json resources."""
-
         classes = []
         name = self.config.output.package.split(".")[-1]
         dirname = os.path.dirname(uris[0]) if uris else ""
 
         for uri in uris:
             input_stream = self.load_resource(uri)
             if input_stream:
-                data = json.load(io.BytesIO(input_stream))
-                logger.info("Parsing document %s", uri)
-                if isinstance(data, dict):
-                    data = [data]
-
-                for obj in data:
-                    classes.extend(DictMapper.map(obj, name, dirname))
+                try:
+                    data = json.load(io.BytesIO(input_stream))
+                    logger.info("Parsing document %s", uri)
+                    if isinstance(data, dict):
+                        data = [data]
+
+                    for obj in data:
+                        classes.extend(DictMapper.map(obj, name, dirname))
+                except ValueError as exc:
+                    logger.warning("JSON load failed for file: %s", uri, exc_info=exc)
 
         self.classes.extend(ClassUtils.reduce_classes(classes))
 
     def process_classes(self):
         """Process the generated classes and write or print the final
         output."""
         class_num, inner_num = self.count_classes(self.classes)
@@ -232,15 +250,14 @@
         if class_num > 0:
             logger.info("Builder: %d main and %d inner classes", class_num, inner_num)
 
         return classes
 
     def parse_schema(self, uri: str, namespace: Optional[str]) -> Optional[Schema]:
         """Parse the given schema uri and return the schema tree object."""
-
         input_stream = self.load_resource(uri)
         if input_stream is None:
             return None
 
         logger.info("Parsing schema %s", uri)
         parser = SchemaParser(target_namespace=namespace, location=uri)
         return parser.from_bytes(input_stream, Schema)
@@ -318,7 +335,13 @@
         """Return a tuple of counters for the main and inner classes."""
         main = len(classes)
         inner = 0
         for cls in classes:
             inner += sum(self.count_classes(cls.inner))
 
         return main, inner
+
+    @classmethod
+    def get_cache_file(cls, uris: List[str]) -> Path:
+        key = hashlib.md5("".join(uris).encode()).hexdigest()
+        tempdir = tempfile.gettempdir()
+        return Path(tempdir).joinpath(f"{key}.cache")
```

### Comparing `xsdata-22.9/xsdata/codegen/utils.py` & `xsdata-23.5/xsdata/codegen/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -193,37 +193,56 @@
             cls.cleanup_class(target)
             result.append(target)
 
         return result
 
     @classmethod
     def reduce_attributes(cls, classes: List[Class]) -> List[Attr]:
+        result = []
+        for attr in cls.sorted_attrs(classes):
+            added = False
+            optional = False
+            for obj in classes:
+                pos = collections.find(obj.attrs, attr)
+                if pos == -1:
+                    optional = True
+                elif not added:
+                    added = True
+                    result.append(obj.attrs.pop(pos))
+                else:
+                    cls.merge_attributes(result[-1], obj.attrs.pop(pos))
+
+            if optional:
+                result[-1].restrictions.min_occurs = 0
+
+        return result
+
+    @classmethod
+    def sorted_attrs(cls, classes: List[Class]) -> List[Attr]:
         attrs: List[Attr] = []
         classes.sort(key=lambda x: len(x.attrs), reverse=True)
 
         for obj in classes:
             i = 0
-            while obj.attrs:
-                pos = collections.find(attrs, obj.attrs[i])
+            obj_attrs = obj.attrs.copy()
+
+            while obj_attrs:
+                pos = collections.find(attrs, obj_attrs[i])
                 i += 1
 
                 if pos > -1:
-                    insert = obj.attrs[:i]
-                    del obj.attrs[:i]
-
-                    merge = insert.pop()
-                    cls.merge_attributes(attrs[pos], merge)
+                    insert = obj_attrs[: i - 1]
+                    del obj_attrs[:i]
                     while insert:
                         attrs.insert(pos, insert.pop())
 
                     i = 0
-                else:
-                    if i == len(obj.attrs):
-                        attrs.extend(obj.attrs)
-                        obj.attrs.clear()
+                elif i == len(obj_attrs):
+                    attrs.extend(obj_attrs)
+                    obj_attrs.clear()
 
         return attrs
 
     @classmethod
     def merge_attributes(cls, target: Attr, source: Attr):
         target.types.extend(tp for tp in source.types if tp not in target.types)
 
@@ -233,28 +252,29 @@
         )
 
         target.restrictions.max_occurs = max(
             target.restrictions.max_occurs or 1,
             source.restrictions.max_occurs or 1,
         )
 
-        if source.restrictions.sequential:
-            target.restrictions.sequential = True
+        if source.restrictions.sequence is not None:
+            target.restrictions.sequence = source.restrictions.sequence
 
     @classmethod
     def rename_attribute_by_preference(cls, a: Attr, b: Attr):
         """
         Decide and rename one of the two given attributes.
 
-        When both attributes are derived from the same xs:tag and one of the two fields
-        has a specific namespace prepend it to the name. Preferable rename the second
-        attribute.
-
-        Otherwise append the derived from tag to the name of one of the two attributes.
-        Preferably rename the second field or the field derived from xs:attribute.
+        When both attributes are derived from the same xs:tag and one of
+        the two fields has a specific namespace prepend it to the name.
+        Preferable rename the second attribute.
+
+        Otherwise append the derived from tag to the name of one of the
+        two attributes. Preferably rename the second field or the field
+        derived from xs:attribute.
         """
         if a.tag == b.tag and (a.namespace or b.namespace):
             change = b if b.namespace else a
             assert change.namespace is not None
             change.name = f"{namespaces.clean_uri(change.namespace)}_{change.name}"
         else:
             change = b if b.is_attribute else a
```

### Comparing `xsdata-22.9/xsdata/codegen/validator.py` & `xsdata-23.5/xsdata/codegen/validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 
         Steps:
             1. Remove invalid classes
             2. Handle duplicate types
             3. Merge dummy types
         """
         for classes in self.container.data.values():
-
             if len(classes) > 1:
                 self.remove_invalid_classes(classes)
 
             if len(classes) > 1:
                 self.handle_duplicate_types(classes)
 
             if len(classes) > 1:
@@ -102,15 +101,14 @@
     def select_winner(cls, candidates: List[Class]) -> int:
         """
         Returns the index of the class that will survive the duplicate process.
 
         Classes that were extracted from in xs:override/xs:redefined
         containers have priority, otherwise pick the last in the list.
         """
-
         for index, item in enumerate(candidates):
             if item.container in (Tag.OVERRIDE, Tag.REDEFINE):
                 return index
 
         return -1
 
     @classmethod
@@ -136,15 +134,14 @@
 
         Conditions
             1. One of them is derived from xs:element
             2. One of them is derived from xs:complexType
             3. The xs:element is a subclass of the xs:complexType
             4. The xs:element has no attributes (This can't happen in a valid schema)
         """
-
         el = collections.first(x for x in classes if x.tag == Tag.ELEMENT)
         ct = collections.first(x for x in classes if x.tag == Tag.COMPLEX_TYPE)
 
         if (
             el is None
             or ct is None
             or el is ct
```

### Comparing `xsdata-22.9/xsdata/codegen/writer.py` & `xsdata-23.5/xsdata/codegen/writer.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,20 +28,22 @@
         self.generator = generator
 
     def write(self, classes: List[Class]):
         """Iterate over the designated generator outputs and create the
         necessary directories and files."""
 
         self.generator.normalize_packages(classes)
+        header = self.generator.render_header()
+
         for result in self.generator.render(classes):
             if result.source.strip():
                 logger.info("Generating package: %s", result.title)
-
+                src_code = header + result.source
                 result.path.parent.mkdir(parents=True, exist_ok=True)
-                result.path.write_text(result.source, encoding="utf-8")
+                result.path.write_text(src_code, encoding="utf-8")
 
     def print(self, classes: List[Class]):
         """Iterate over the designated generator outputs and print them to the
         console."""
         self.generator.normalize_packages(classes)
         for result in self.generator.render(classes):
             if result.source.strip():
```

### Comparing `xsdata-22.9/xsdata/exceptions.py` & `xsdata-23.5/xsdata/exceptions.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/xsdata/formats/bindings.py` & `xsdata-23.5/xsdata/formats/bindings.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/xsdata/formats/converter.py` & `xsdata-23.5/xsdata/formats/converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,14 @@
         """
         Find a suitable converter for given data type.
 
         Iterate over all but last mro items and check for registered
         converters, fall back to str and issue a warning if there are
         not matches.
         """
-
         try:
             # Quick in and out, without checking the whole mro.
             return self.registry[datatype]
         except KeyError:
             pass
 
         # We tested the first, ignore the object
@@ -420,15 +419,14 @@
 
         raise ConverterError()
 
     @classmethod
     def match(
         cls, value: Any, values: Sequence, length: int, real: Any, **kwargs: Any
     ) -> bool:
-
         if isinstance(value, str) and isinstance(real, str):
             return value == real or " ".join(values) == real
 
         if isinstance(real, (tuple, list)) and not hasattr(real, "_fields"):
             if len(real) == length and cls.match_list(values, real, **kwargs):
                 return True
         elif length == 1 and cls.match_atomic(value, real, **kwargs):
@@ -491,15 +489,14 @@
 
 class DateTimeConverter(DateTimeBase):
     def deserialize(self, value: Any, **kwargs: Any) -> datetime:
         return self.parse(value, **kwargs)
 
 
 class ProxyConverter(Converter):
-
     __slots__ = ("factory",)
 
     def __init__(self, factory: Callable):
         """
         :param factory: factory function used to parse string values
         """
         self.factory = factory
```

### Comparing `xsdata-22.9/xsdata/formats/dataclass/client.py` & `xsdata-23.5/xsdata/formats/dataclass/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,19 +28,19 @@
 
     style: str
     location: str
     transport: str
     soap_action: str
     input: Type
     output: Type
+    encoding: Optional[str] = None
 
     @classmethod
     def from_service(cls, obj: Any, **kwargs: Any) -> "Config":
         """Instantiate from a generated service class."""
-
         params = {
             key: kwargs[key] if key in kwargs else getattr(obj, key, None)
             for key in cls._fields
         }
 
         return cls(**params)
 
@@ -126,8 +126,12 @@
         if not isinstance(obj, self.config.input):
             raise ClientValueError(
                 f"Invalid input service type, "
                 f"expected `{self.config.input.__name__}` "
                 f"got `{type(obj).__name__}`"
             )
 
-        return self.serializer.render(obj)
+        result = self.serializer.render(obj)
+        if self.config.encoding:
+            return result.encode(self.config.encoding)
+
+        return result
```

### Comparing `xsdata-22.9/xsdata/formats/dataclass/compat.py` & `xsdata-23.5/xsdata/formats/dataclass/compat.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import abc
 from dataclasses import Field
 from dataclasses import fields
 from dataclasses import is_dataclass
 from dataclasses import MISSING
 from typing import Any
 from typing import Dict
+from typing import Optional
 from typing import Set
 from typing import Tuple
 from typing import Type
 
 from xsdata.exceptions import XmlContextError
 from xsdata.formats.dataclass.models.generics import AnyElement
 from xsdata.formats.dataclass.models.generics import DerivedElement
 from xsdata.utils.hooks import load_entry_points
 
 
 class ClassType(abc.ABC):
-
     __slots__ = ()
 
     @property
     @abc.abstractmethod
     def any_element(self) -> Type:
         """Return the any type used to bind wildcard element nodes."""
 
@@ -52,15 +52,15 @@
         """
 
     @abc.abstractmethod
     def get_fields(self, obj: Any) -> Tuple[Any, ...]:
         """Return the models fields in the correct mro ordering."""
 
     @abc.abstractmethod
-    def default_value(self, field: Any) -> Any:
+    def default_value(self, field: Any, default: Optional[Any] = None) -> Any:
         """Return the default value or factory of the given model field."""
 
     @abc.abstractmethod
     def default_choice_value(self, choice: Dict) -> Any:
         """Return the default value or factory of the given model field
         choice."""
 
@@ -69,15 +69,14 @@
         Score a binding model instance by its field values types.
 
         Weights:
             1. None: 0
             2. str: 1
             3. *: 1.5
         """
-
         if not obj:
             return -1.0
 
         def score(value: Any) -> float:
             if isinstance(value, str):
                 return 1.0
 
@@ -102,15 +101,14 @@
         self.types[name] = fmt
 
     def get_type(self, name: str) -> ClassType:
         return self.types[name]
 
 
 class Dataclasses(ClassType):
-
     __slots__ = ()
 
     @property
     def any_element(self) -> Type:
         return AnyElement
 
     @property
@@ -123,23 +121,22 @@
     def verify_model(self, obj: Any):
         if not self.is_model(obj):
             raise XmlContextError(f"Type '{obj}' is not a dataclass.")
 
     def get_fields(self, obj: Any) -> Tuple[Any, ...]:
         return fields(obj)
 
-    def default_value(self, field: Field) -> Any:
-        # Ignore type because of https://github.com/python/mypy/issues/6910
-        if field.default_factory is not MISSING:  # type: ignore
-            return field.default_factory  # type: ignore
+    def default_value(self, field: Field, default: Optional[Any] = None) -> Any:
+        if field.default_factory is not MISSING:
+            return field.default_factory
 
         if field.default is not MISSING:
             return field.default
 
-        return None
+        return default
 
     def default_choice_value(self, choice: Dict) -> Any:
         factory = choice.get("default_factory")
         if callable(factory):
             return factory
 
         return choice.get("default")
```

### Comparing `xsdata-22.9/xsdata/formats/dataclass/context.py` & `xsdata-23.5/xsdata/formats/dataclass/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 
     def __init__(
         self,
         element_name_generator: Callable = return_input,
         attribute_name_generator: Callable = return_input,
         class_type: str = "dataclasses",
     ):
-
         self.element_name_generator = element_name_generator
         self.attribute_name_generator = attribute_name_generator
         self.class_type = class_types.get_type(class_type)
 
         self.cache: Dict[Type, XmlMeta] = {}
         self.xsi_cache: Dict[str, List[Type]] = defaultdict(list)
         self.sys_modules = 0
@@ -76,25 +75,28 @@
         if xsi_type and meta.target_qname != xsi_type:
             subclass = self.find_subclass(clazz, xsi_type)
 
         return self.build(subclass, parent_ns) if subclass else meta
 
     def build_xsi_cache(self):
         """Index all imported dataclasses by their xsi:type qualified name."""
-
         if len(sys.modules) == self.sys_modules:
             return
 
         self.xsi_cache.clear()
         builder = XmlMetaBuilder(
             class_type=self.class_type,
             element_name_generator=self.element_name_generator,
             attribute_name_generator=self.attribute_name_generator,
         )
         for clazz in self.get_subclasses(object):
+            # This is new!
+            if clazz.__module__.startswith("_pytest"):
+                continue
+
             if self.class_type.is_model(clazz):
                 meta = builder.build_class_meta(clazz, None)
 
                 if meta.target_qname:
                     self.xsi_cache[meta.target_qname].append(clazz)
 
         self.sys_modules = len(sys.modules)
@@ -129,61 +131,73 @@
         """
         Find a dataclass from all the imported modules that matches the given
         list of field names.
 
         :param field_names: A unique list of field names
         """
 
+        def get_field_diff(clazz: Type) -> int:
+            meta = self.cache[clazz]
+            local_names = {var.local_name for var in meta.get_all_vars()}
+            return len(local_names - field_names)
+
         self.build_xsi_cache()
-        for types in self.xsi_cache.values():
-            for clazz in types:
-                if self.local_names_match(field_names, clazz):
-                    return clazz
+        choices = [
+            (clazz, get_field_diff(clazz))
+            for types in self.xsi_cache.values()
+            for clazz in types
+            if self.local_names_match(field_names, clazz)
+        ]
 
-        return None
+        choices.sort(key=lambda x: (x[1], x[0].__name__))
+        return choices[0][0] if len(choices) > 0 else None
 
     def find_subclass(self, clazz: Type, qname: str) -> Optional[Type]:
         """
         Compare all classes that match the given xsi:type qname and return the
         first one that is either a subclass or shares the same parent class as
         the original class.
 
         :param clazz: The search dataclass type
         :param qname: Qualified name
         """
-
         types: List[Type] = self.find_types(qname)
         for tp in types:
-
             # Why would an xml node with have an xsi:type that points
             # to parent class is beyond me but it happens, let's protect
             # against that scenario <node xsi:type="nodeAbstract" />
             if issubclass(clazz, tp):
                 continue
 
             for tp_mro in tp.__mro__:
                 if tp_mro is not object and tp_mro in clazz.__mro__:
                     return tp
 
         return None
 
-    def build(self, clazz: Type, parent_ns: Optional[str] = None) -> XmlMeta:
+    def build(
+        self,
+        clazz: Type,
+        parent_ns: Optional[str] = None,
+        globalns: Optional[Dict[str, Callable]] = None,
+    ) -> XmlMeta:
         """
         Fetch from cache or build the binding metadata for the given class and
         parent namespace.
 
         :param clazz: A dataclass type
         :param parent_ns: The inherited parent namespace
         """
 
         if clazz not in self.cache:
             builder = XmlMetaBuilder(
                 class_type=self.class_type,
                 element_name_generator=self.element_name_generator,
                 attribute_name_generator=self.attribute_name_generator,
+                globalns=globalns,
             )
             self.cache[clazz] = builder.build(clazz, parent_ns)
         return self.cache[clazz]
 
     def build_recursive(self, clazz: Type, parent_ns: Optional[str] = None):
         """Build the binding metadata for the given class and all of its
         dependencies."""
@@ -207,15 +221,14 @@
     def is_derived(cls, obj: Any, clazz: Type) -> bool:
         """
         Return whether the given obj is derived from the given dataclass type.
 
         :param obj: A dataclass instance
         :param clazz: A dataclass type
         """
-
         if obj is None:
             return False
 
         if isinstance(obj, clazz):
             return True
 
         return any(x is not object and isinstance(obj, x) for x in clazz.__bases__)
```

### Comparing `xsdata-22.9/xsdata/formats/dataclass/filters.py` & `xsdata-23.5/xsdata/formats/dataclass/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 import re
+import sys
 import textwrap
 from collections import defaultdict
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import Iterable
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Type
 
-from docformatter import format_code
+from docformatter import configuration
+from docformatter import format
 from jinja2 import Environment
 
 from xsdata.codegen.models import Attr
 from xsdata.codegen.models import AttrType
 from xsdata.codegen.models import Class
 from xsdata.formats.converter import converter
+from xsdata.formats.dataclass.models.elements import XmlType
 from xsdata.models.config import DocstringStyle
 from xsdata.models.config import GeneratorConfig
 from xsdata.models.config import ObjectType
 from xsdata.models.config import OutputFormat
 from xsdata.utils import collections
 from xsdata.utils import namespaces
 from xsdata.utils import text
 from xsdata.utils.objects import literal_value
 
 
 class Filters:
-
     DEFAULT_KEY = "default"
     FACTORY_KEY = "default_factory"
     UNESCAPED_DBL_QUOTE_REGEX = re.compile(r"([^\\])\"")
 
     __slots__ = (
         "substitutions",
         "class_case",
@@ -142,15 +144,15 @@
         conventions or use an existing alias."""
         name = self.apply_substitutions(name, ObjectType.CLASS)
         name = self.safe_name(name, self.class_safe_prefix, self.class_case)
         return self.apply_substitutions(name, ObjectType.CLASS)
 
     def apply_substitutions(self, name: str, obj_type: ObjectType) -> str:
         for search, replace in self.substitutions[obj_type].items():
-            name = re.sub(search, replace, name)
+            name = re.sub(rf"{search}", rf"{replace}", name)
 
         return name
 
     def field_definition(
         self,
         attr: Attr,
         ns_map: Dict,
@@ -158,18 +160,18 @@
         parents: List[str],
     ) -> str:
         """Return the field definition with any extra metadata."""
         default_value = self.field_default_value(attr, ns_map)
         metadata = self.field_metadata(attr, parent_namespace, parents)
 
         kwargs: Dict[str, Any] = {}
-        if attr.fixed:
+        if attr.fixed or attr.is_prohibited:
             kwargs["init"] = False
 
-        if default_value is not False:
+        if default_value is not False and not attr.is_prohibited:
             key = self.FACTORY_KEY if attr.is_factory else self.DEFAULT_KEY
             kwargs[key] = default_value
 
         if metadata:
             kwargs["metadata"] = metadata
 
         return f"field({self.format_arguments(kwargs, 4)})"
@@ -277,14 +279,17 @@
         return self.class_name(name)
 
     def field_metadata(
         self, attr: Attr, parent_namespace: Optional[str], parents: List[str]
     ) -> Dict:
         """Return a metadata dictionary for the given attribute."""
 
+        if attr.is_prohibited:
+            return {"type": XmlType.IGNORE}
+
         name = namespace = None
 
         if not attr.is_nameless and attr.local_name != self.field_name(
             attr.name, parents[-1]
         ):
             name = attr.local_name
 
@@ -318,15 +323,14 @@
         """
 
         if not attr.choices:
             return None
 
         result = []
         for choice in attr.choices:
-
             types = choice.native_types
             restrictions = choice.restrictions.asdict(types)
             namespace = (
                 choice.namespace if parent_namespace != choice.namespace else None
             )
 
             metadata = {
@@ -367,15 +371,14 @@
             for key, value in data.items()
         ]
 
         return "\n{}\n{}".format(",\n".join(lines), ind) if lines else ""
 
     def format_metadata(self, data: Any, indent: int = 0, key: str = "") -> str:
         """Prettify field metadata for code generation."""
-
         if isinstance(data, dict):
             return self.format_dict(data, indent)
 
         if collections.is_array(data):
             return self.format_iterable(data, indent)
 
         if isinstance(data, str):
@@ -486,34 +489,44 @@
 
             return txt.replace('"""', "'''").strip()
 
         return "\n".join(_clean(line) for line in string.splitlines() if line.strip())
 
     def format_docstring(self, doc_string: str, level: int) -> str:
         """Format doc strings."""
-
         sep_pos = doc_string.rfind('"""')
         if sep_pos == -1:
             return ""
 
         content = doc_string[:sep_pos]
         params = doc_string[sep_pos + 3 :].strip()
 
         if content.strip() == '"""' and not params:
             return ""
 
         content += ' """' if content.endswith('"') else '"""'
 
         max_length = self.max_line_length - level * 4
-        content = format_code(
-            content,
-            summary_wrap_length=max_length,
-            description_wrap_length=max_length - 7,
-            make_summary_multi_line=True,
+        configurator = configuration.Configurater(
+            [
+                "--wrap-summaries",
+                str(max_length - 3),
+                "--wrap-descriptions",
+                str(max_length - 7),
+                "--make-summary-multi-line",
+            ]
         )
+        configurator.do_parse_arguments()
+        formatter = format.Formatter(
+            configurator.args,
+            sys.stderr,
+            sys.stdin,
+            sys.stdout,
+        )
+        content = formatter._do_format_code(content)
 
         if params:
             # Remove trailing triple quotes
             content = content[:-3].strip()
             new_lines = "\n" if content.endswith('"""') else "\n\n"
             content += f'{new_lines}{params}\n"""'
 
@@ -576,14 +589,17 @@
             return self.format_metadata(tuple(tokens), indent=8)
 
         return f"lambda: {self.format_metadata(tokens, indent=8)}"
 
     def field_type(self, attr: Attr, parents: List[str]) -> str:
         """Generate type hints for the given attribute."""
 
+        if attr.is_prohibited:
+            return "Any"
+
         type_names = collections.unique_sequence(
             self.field_type_name(x, parents) for x in attr.types
         )
 
         result = ", ".join(type_names)
         if len(type_names) > 1:
             result = f"Union[{result}]"
@@ -691,14 +707,15 @@
             "typing": {
                 "Dict": [": Dict"],
                 "List": [": List["],
                 "Optional": ["Optional["],
                 "Tuple": ["Tuple["],
                 "Type": ["Type["],
                 "Union": ["Union["],
+                "Any": type_patterns("Any"),
             },
             "xml.etree.ElementTree": {"QName": type_patterns("QName")},
             "xsdata.models.datatype": {
                 "XmlDate": type_patterns("XmlDate"),
                 "XmlDateTime": type_patterns("XmlDateTime"),
                 "XmlDuration": type_patterns("XmlDuration"),
                 "XmlPeriod": type_patterns("XmlPeriod"),
```

### Comparing `xsdata-22.9/xsdata/formats/dataclass/generator.py` & `xsdata-23.5/xsdata/formats/dataclass/generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,14 @@
         self, classes: List[Class], module_namespace: Optional[str]
     ) -> str:
         """Render the source code of the classes."""
         load = self.env.get_template
 
         def render_class(obj: Class) -> str:
             """Render class or enumeration."""
-
             if obj.is_enumeration:
                 template = load("enum.jinja2")
             elif obj.is_service:
                 template = load("service.jinja2")
             else:
                 template = load("class.jinja2")
```

### Comparing `xsdata-22.9/xsdata/formats/dataclass/models/builders.py` & `xsdata-23.5/xsdata/formats/dataclass/models/builders.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,30 +36,35 @@
     local_name: str
     nillable: bool
     namespace: Optional[str]
     target_qname: Optional[str]
 
 
 class XmlMetaBuilder:
-    __slots__ = "class_type", "element_name_generator", "attribute_name_generator"
+    __slots__ = (
+        "class_type",
+        "element_name_generator",
+        "attribute_name_generator",
+        "globalns",
+    )
 
     def __init__(
         self,
         class_type: ClassType,
         element_name_generator: Callable,
         attribute_name_generator: Callable,
+        globalns: Optional[Dict[str, Callable]] = None,
     ):
-
         self.class_type = class_type
         self.element_name_generator = element_name_generator
         self.attribute_name_generator = attribute_name_generator
+        self.globalns = globalns
 
     def build(self, clazz: Type, parent_namespace: Optional[str]) -> XmlMeta:
         """Build the binding metadata for a dataclass and its fields."""
-
         self.class_type.verify_model(clazz)
 
         meta = self.build_class_meta(clazz, parent_namespace)
         class_vars = self.build_vars(
             clazz,
             meta.namespace,
             meta.element_name_generator,
@@ -67,17 +72,20 @@
         )
 
         attributes = {}
         elements: Dict[str, List[XmlVar]] = defaultdict(list)
         choices = []
         any_attributes = []
         wildcards = []
+        wrappers: Dict[str, List[XmlVar]] = defaultdict(list)
         text = None
 
         for var in class_vars:
+            if var.wrapper is not None:
+                wrappers[var.wrapper].append(var)
             if var.is_attribute:
                 attributes[var.qname] = var
             elif var.is_element:
                 elements[var.qname].append(var)
             elif var.is_elements:
                 choices.append(var)
             elif var.is_attributes:
@@ -94,42 +102,41 @@
             nillable=meta.nillable,
             text=text,
             attributes=attributes,
             elements=elements,
             choices=choices,
             any_attributes=any_attributes,
             wildcards=wildcards,
+            wrappers=wrappers,
         )
 
     def build_vars(
         self,
         clazz: Type,
         namespace: Optional[str],
         element_name_generator: Callable,
         attribute_name_generator: Callable,
     ):
         """Build the binding metadata for the given dataclass fields."""
-        type_hints = get_type_hints(clazz)
+        type_hints = get_type_hints(clazz, globalns=self.globalns)
         builder = XmlVarBuilder(
             class_type=self.class_type,
             default_xml_type=self.default_xml_type(clazz),
             element_name_generator=element_name_generator,
             attribute_name_generator=attribute_name_generator,
         )
 
-        for index, field in enumerate(self.class_type.get_fields(clazz)):
-
+        for field in self.class_type.get_fields(clazz):
             real_clazz = self.find_declared_class(clazz, field.name)
             globalns = sys.modules[real_clazz.__module__].__dict__
             parent_namespace = namespace
             if real_clazz is not clazz and "Meta" in real_clazz.__dict__:
                 parent_namespace = getattr(real_clazz.Meta, "namespace", namespace)
 
             var = builder.build(
-                index,
                 field.name,
                 type_hints[field.name],
                 field.metadata,
                 field.init,
                 parent_namespace,
                 self.class_type.default_value(field),
                 globalns,
@@ -219,37 +226,37 @@
         if counters["undefined"] == 1 and counters[XmlType.TEXT] == 0:
             return XmlType.TEXT
 
         return XmlType.ELEMENT
 
 
 class XmlVarBuilder:
-
     __slots__ = (
+        "index",
         "class_type",
         "default_xml_type",
         "element_name_generator",
         "attribute_name_generator",
     )
 
     def __init__(
         self,
         class_type: ClassType,
         default_xml_type: str,
         element_name_generator: Callable = return_input,
         attribute_name_generator: Callable = return_input,
     ):
+        self.index = 0
         self.class_type = class_type
         self.default_xml_type = default_xml_type
         self.element_name_generator = element_name_generator
         self.attribute_name_generator = attribute_name_generator
 
     def build(
         self,
-        index: int,
         name: str,
         type_hint: Any,
         metadata: Mapping[str, Any],
         init: bool,
         parent_namespace: Optional[str],
         default_value: Any,
         globalns: Any,
@@ -264,96 +271,109 @@
         local_name = metadata.get("name")
         namespace = metadata.get("namespace")
         choices = metadata.get("choices", EMPTY_SEQUENCE)
         mixed = metadata.get("mixed", False)
         required = metadata.get("required", False)
         nillable = metadata.get("nillable", False)
         format_str = metadata.get("format", None)
-        sequential = metadata.get("sequential", False)
+        sequence = metadata.get("sequence", None)
+        wrapper = metadata.get("wrapper", None)
 
         origin, sub_origin, types = self.analyze_types(type_hint, globalns)
 
         if not self.is_valid(xml_type, origin, sub_origin, types, tokens, init):
             raise XmlContextError(
                 f"Xml type '{xml_type}' does not support typing: {type_hint}"
             )
 
+        if wrapper is not None:
+            if not isinstance(origin, type) or not issubclass(
+                origin, (list, set, tuple)
+            ):
+                raise XmlContextError(
+                    f"a wrapper requires a collection type on attribute {name}"
+                )
+
         local_name = self.build_local_name(xml_type, local_name, name)
 
         if tokens and sub_origin is None:
             sub_origin = origin
             origin = None
 
         if origin is None:
             origin = factory
 
         any_type = self.is_any_type(types, xml_type)
         clazz = first(tp for tp in types if self.class_type.is_model(tp))
         namespaces = self.resolve_namespaces(xml_type, namespace, parent_namespace)
         default_namespace = self.default_namespace(namespaces)
         qname = build_qname(default_namespace, local_name)
+        if wrapper is not None:
+            wrapper = build_qname(default_namespace, wrapper)
 
         elements = {}
         wildcards = []
+        self.index += 1
+        cur_index = self.index
         for choice in self.build_choices(
             name, choices, origin, globalns, parent_namespace
         ):
             if choice.is_element:
                 elements[choice.qname] = choice
             else:  # choice.is_wildcard:
                 wildcards.append(choice)
 
         return XmlVar(
-            index=index + 1,
+            index=cur_index,
             name=name,
             qname=qname,
             init=init,
             mixed=mixed,
             format=format_str,
             clazz=clazz,
             any_type=any_type,
             required=required,
             nillable=nillable,
-            sequential=sequential,
+            sequence=sequence,
             factory=origin,
             tokens_factory=sub_origin,
             default=default_value,
             types=types,
             elements=elements,
             wildcards=wildcards,
             namespaces=namespaces,
             xml_type=xml_type,
             derived=False,
+            wrapper=wrapper,
         )
 
     def build_choices(
         self,
         name: str,
         choices: List[Dict],
         factory: Callable,
         globalns: Any,
         parent_namespace: Optional[str],
     ) -> Iterator[XmlVar]:
         """Build the binding metadata for a compound dataclass field."""
         existing_types: Set[type] = set()
 
-        for index, choice in enumerate(choices):
+        for choice in choices:
             default_value = self.class_type.default_choice_value(choice)
 
             metadata = choice.copy()
             metadata["name"] = choice.get("name", "any")
             type_hint = metadata["type"]
 
             if choice.get("wildcard"):
                 metadata["type"] = XmlType.WILDCARD
             else:
                 metadata["type"] = XmlType.ELEMENT
 
             var = self.build(
-                index,
                 name,
                 type_hint,
                 metadata,
                 True,
                 parent_namespace,
                 default_value,
                 globalns,
```

### Comparing `xsdata-22.9/xsdata/formats/dataclass/models/elements.py` & `xsdata-23.5/xsdata/formats/dataclass/models/elements.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,21 +63,22 @@
     :param mixed:  Field supports mixed content type values
     :param tokens: Field is derived from xs:list
     :param format: Value format information
     :param derived: Wrap parsed values with a generic type
     :param any_type: Field supports dynamic value types
     :param required: Field is mandatory
     :param nillable: Field supports nillable content
-    :param sequential: Render values in sequential mode
+    :param sequence: Render values in sequential mode
     :param list_element: Field is a list of elements
     :param default: Field default value or factory
     :param xml_Type: Field xml type
     :param namespaces: List of the supported namespaces
     :param elements: Mapping of qname-repeatable elements
     :param wildcards: List of repeatable wildcards
+    :param wrapper: A name for the wrapper. Applies for list types only.
     """
 
     __slots__ = (
         "index",
         "name",
         "qname",
         "types",
@@ -87,19 +88,20 @@
         "factory",
         "tokens_factory",
         "format",
         "derived",
         "any_type",
         "required",
         "nillable",
-        "sequential",
+        "sequence",
         "default",
         "namespaces",
         "elements",
         "wildcards",
+        "wrapper",
         # Calculated
         "tokens",
         "list_element",
         "is_text",
         "is_element",
         "is_elements",
         "is_wildcard",
@@ -122,20 +124,21 @@
         factory: Optional[Callable],
         tokens_factory: Optional[Callable],
         format: Optional[str],
         derived: bool,
         any_type: bool,
         required: bool,
         nillable: bool,
-        sequential: bool,
+        sequence: Optional[int],
         default: Any,
         xml_type: str,
         namespaces: Sequence[str],
         elements: Mapping[str, "XmlVar"],
         wildcards: Sequence["XmlVar"],
+        wrapper: Optional[str] = None,
         **kwargs: Any,
     ):
         self.index = index
         self.name = name
         self.qname = qname
         self.types = types
         self.clazz = clazz
@@ -143,20 +146,21 @@
         self.mixed = mixed
         self.tokens = tokens_factory is not None
         self.format = format
         self.derived = derived
         self.any_type = any_type
         self.required = required
         self.nillable = nillable
-        self.sequential = sequential
+        self.sequence = sequence
         self.list_element = factory in (list, tuple)
         self.default = default
         self.namespaces = namespaces
         self.elements = elements
         self.wildcards = wildcards
+        self.wrapper = wrapper
 
         self.factory = factory
         self.tokens_factory = tokens_factory
 
         self.namespace_matches: Optional[Dict[str, bool]] = None
 
         self.is_clazz_union = self.clazz and len(types) > 1
@@ -253,15 +257,14 @@
 
         if callable(self.default):
             return self.default() == value
         return self.default == value
 
     def match_namespace(self, qname: str) -> bool:
         """Match the given qname to the wildcard allowed namespaces."""
-
         if self.namespace_matches is None:
             self.namespace_matches = {}
 
         matches = self.namespace_matches.get(qname)
         if matches is None:
             matches = self._match_namespace(qname)
             self.namespace_matches[qname] = matches
@@ -312,14 +315,15 @@
         "nillable",
         "text",
         "choices",
         "elements",
         "wildcards",
         "attributes",
         "any_attributes",
+        "wrappers",
         # Calculated
         "namespace",
         "mixed_content",
     )
 
     def __init__(
         self,
@@ -329,28 +333,30 @@
         nillable: bool,
         text: Optional[XmlVar],
         choices: Sequence[XmlVar],
         elements: Mapping[str, Sequence[XmlVar]],
         wildcards: Sequence[XmlVar],
         attributes: Mapping[str, XmlVar],
         any_attributes: Sequence[XmlVar],
+        wrappers: Mapping[str, Sequence[XmlVar]],
         **kwargs: Any,
     ):
         self.clazz = clazz
         self.qname = qname
         self.namespace = target_uri(qname)
         self.target_qname = target_qname
         self.nillable = nillable
         self.text = text
         self.choices = choices
         self.elements = elements
         self.wildcards = wildcards
         self.attributes = attributes
         self.any_attributes = any_attributes
         self.mixed_content = any(wildcard.mixed for wildcard in self.wildcards)
+        self.wrappers = wrappers
 
     @property
     def element_types(self) -> Set[Type]:
         return {
             tp
             for elements in self.elements.values()
             for element in elements
```

### Comparing `xsdata-22.9/xsdata/formats/dataclass/models/generics.py` & `xsdata-23.5/xsdata/formats/dataclass/models/generics.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/xsdata/formats/dataclass/parsers/bases.py` & `xsdata-23.5/xsdata/formats/dataclass/parsers/bases.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import copy
 import warnings
 from dataclasses import dataclass
 from dataclasses import field
 from typing import Any
+from typing import cast
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Type
 
 from xsdata.exceptions import ConverterWarning
@@ -78,17 +79,22 @@
             suitable models from the current context.
         :param queue: The active XmlNode queue
         :param objects: The list of all intermediate parsed objects
         :param qname: Qualified name
         :param attrs: Attribute key-value map
         :param ns_map: Namespace prefix-URI map
         """
+        from xsdata.formats.dataclass.parsers.nodes import ElementNode, WrapperNode
+
         try:
             item = queue[-1]
-            child = item.child(qname, attrs, ns_map, len(objects))
+            if isinstance(item, ElementNode) and qname in item.meta.wrappers:
+                child = cast(XmlNode, WrapperNode(parent=item))
+            else:
+                child = item.child(qname, attrs, ns_map, len(objects))
         except IndexError:
             xsi_type = ParserUtils.xsi_type(attrs, ns_map)
 
             # Match element qname directly
             if clazz is None:
                 clazz = self.context.find_type(qname)
 
@@ -104,16 +110,14 @@
             if xsi_type is None or meta.qname == qname:
                 derived_factory = None
             else:
                 derived_factory = self.context.class_type.derived_element
 
             xsi_nil = ParserUtils.xsi_nil(attrs)
 
-            from xsdata.formats.dataclass.parsers.nodes import ElementNode
-
             child = ElementNode(
                 position=0,
                 meta=meta,
                 config=self.config,
                 attrs=attrs,
                 ns_map=ns_map,
                 context=self.context,
```

### Comparing `xsdata-22.9/xsdata/formats/dataclass/parsers/config.py` & `xsdata-23.5/xsdata/formats/dataclass/parsers/config.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/xsdata/formats/dataclass/parsers/handlers/__init__.py` & `xsdata-23.5/xsdata/formats/dataclass/parsers/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/xsdata/formats/dataclass/parsers/handlers/lxml.py` & `xsdata-23.5/xsdata/formats/dataclass/parsers/handlers/lxml.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 
         When source is a system identifier or an InputSource the parser
         will ignore comments and recover from errors.
 
         When config process_xinclude is enabled the handler will parse
         the whole document and then walk down the element tree.
         """
-
         if isinstance(source, (etree._ElementTree, etree._Element)):
             ctx = etree.iterwalk(source, EVENTS)
         elif self.parser.config.process_xinclude:
             tree = etree.parse(source, base_url=self.parser.config.base_url)  # nosec
             tree.xinclude()
             ctx = etree.iterwalk(tree, EVENTS)
         else:
```

### Comparing `xsdata-22.9/xsdata/formats/dataclass/parsers/handlers/native.py` & `xsdata-23.5/xsdata/formats/dataclass/parsers/handlers/native.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 
         When source is a system identifier or an InputSource the parser
         will ignore comments and recover from errors.
 
         When config process_xinclude is enabled the handler will parse
         the whole document and then walk down the element tree.
         """
-
         if isinstance(source, etree.ElementTree):
             source = source.getroot()
 
         if isinstance(source, etree.Element):
             ctx = iterwalk(source, {})
         elif self.parser.config.process_xinclude:
             root = etree.parse(source).getroot()  # nosec
```

### Comparing `xsdata-22.9/xsdata/formats/dataclass/parsers/json.py` & `xsdata-23.5/xsdata/formats/dataclass/parsers/json.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,14 @@
         if clazz:
             return clazz
 
         raise ParserError(f"Unable to locate model with properties({list(keys)})")
 
     def bind_dataclass(self, data: Dict, clazz: Type[T]) -> T:
         """Recursively build the given model from the input dict data."""
-
         if set(data.keys()) == self.context.class_type.derived_keys:
             return self.bind_derived_dataclass(data, clazz)
 
         meta = self.context.build(clazz)
         xml_vars = meta.get_all_vars()
 
         params = {}
@@ -158,15 +157,14 @@
     def bind_best_dataclass(self, data: Dict, classes: Iterable[Type[T]]) -> T:
         """Attempt to bind the given data to one possible models, if more than
         one is successful return the object with the highest score."""
         obj = None
         keys = set(data.keys())
         max_score = -1.0
         for clazz in classes:
-
             if not self.context.class_type.is_model(clazz):
                 continue
 
             if self.context.local_names_match(keys, clazz):
                 candidate = self.bind_optional_dataclass(data, clazz)
                 score = self.context.class_type.score_object(candidate)
                 if score > max_score:
@@ -219,22 +217,24 @@
             return self.bind_derived_value(meta, var, value)
 
         # Bind data to a user defined dataclass
         return self.bind_complex_type(meta, var, value)
 
     def bind_text(self, meta: XmlMeta, var: XmlVar, value: Any) -> Any:
         """Bind text/tokens value entrypoint."""
-
         if var.is_elements:
             # Compound field we need to match the value to one of the choice elements
             check_subclass = self.context.class_type.is_model(value)
             choice = var.find_value_choice(value, check_subclass)
             if choice:
                 return self.bind_text(meta, choice, value)
 
+            if value is None:
+                return value
+
             raise ParserError(
                 f"Failed to bind '{value}' "
                 f"to {meta.clazz.__qualname__}.{var.name} field"
             )
 
         if var.any_type or var.is_wildcard:
             # field can support any object return the value as it is
@@ -248,15 +248,14 @@
             ns_map=EMPTY_MAP,
             tokens_factory=var.tokens_factory,
             format=var.format,
         )
 
     def bind_complex_type(self, meta: XmlMeta, var: XmlVar, data: Dict) -> Any:
         """Bind data to a user defined dataclass."""
-
         if var.is_clazz_union:
             # Union of dataclasses
             return self.bind_best_dataclass(data, var.types)
         if var.elements:
             # Compound field with multiple choices
             return self.bind_best_dataclass(data, var.element_types)
         if var.any_type or var.is_wildcard:
@@ -269,17 +268,16 @@
         if subclasses:
             # field annotation is an abstract/base type
             subclasses.add(var.clazz)
             return self.bind_best_dataclass(data, subclasses)
 
         return self.bind_dataclass(data, var.clazz)
 
-    def bind_derived_value(self, meta: XmlMeta, var: XmlVar, data: Dict) -> T:
+    def bind_derived_value(self, meta: XmlMeta, var: XmlVar, data: Dict) -> Any:
         """Bind derived element entry point."""
-
         qname = data["qname"]
         xsi_type = data["type"]
         params = data["value"]
 
         if var.elements:
             choice = var.find_choice(qname)
             if choice is None:
@@ -287,23 +285,23 @@
                     f"Unable to locate compound element"
                     f" {meta.clazz.__qualname__}.{var.name}[{qname}]"
                 )
             return self.bind_derived_value(meta, choice, data)
 
         if not isinstance(params, dict):
             value = self.bind_text(meta, var, params)
-        elif var.clazz:
-            value = self.bind_complex_type(meta, var, params)
         elif xsi_type:
             clazz: Optional[Type] = self.context.find_type(xsi_type)
 
             if clazz is None:
                 raise ParserError(f"Unable to locate xsi:type `{xsi_type}`")
 
             value = self.bind_dataclass(params, clazz)
+        elif var.clazz:
+            value = self.bind_complex_type(meta, var, params)
         else:
             value = self.bind_best_dataclass(params, meta.element_types)
 
         generic = self.context.class_type.derived_element
         return generic(qname=qname, value=value, type=xsi_type)
 
     @classmethod
```

### Comparing `xsdata-22.9/xsdata/formats/dataclass/parsers/mixins.py` & `xsdata-23.5/xsdata/formats/dataclass/parsers/mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,14 @@
     def register_namespace(self, prefix: NoneStr, uri: str):
         """
         Add the given prefix-URI namespaces mapping if the prefix is new.
 
         :param prefix: Namespace prefix
         :param uri: Namespace uri
         """
-
         if prefix not in self.ns_map:
             self.ns_map[prefix] = uri
 
 
 class XmlNode(abc.ABC):
     """
     The xml node interface.
@@ -132,15 +131,14 @@
         """
         Merge and return the given prefix-URI map with the parent node.
 
         Register new prefixes with the parser.
 
         :param ns_map: Namespace prefix-URI map
         """
-
         if self.queue:
             parent_ns_map = self.queue[-1].ns_map
 
             if not ns_map:
                 return parent_ns_map
 
             result = parent_ns_map.copy() if parent_ns_map else {}
@@ -162,15 +160,14 @@
     def __init__(self, parser: PushParser, clazz: Optional[Type]):
         super().__init__(parser, clazz)
         self.data_frames: List = []
         self.flush_next: Optional[str] = None
 
     def parse(self, source: List[Tuple]) -> Any:
         """Forward the pre-recorded events to the main parser."""
-
         for event, *args in source:
             if event == EventType.START:
                 qname, attrs, ns_map = args
                 self.parser.start(
                     self.clazz,
                     self.queue,
                     self.objects,
```

### Comparing `xsdata-22.9/xsdata/formats/dataclass/parsers/nodes/__init__.py` & `xsdata-23.5/xsdata/formats/dataclass/parsers/nodes/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from xsdata.formats.dataclass.parsers.nodes.element import ElementNode
 from xsdata.formats.dataclass.parsers.nodes.primitive import PrimitiveNode
 from xsdata.formats.dataclass.parsers.nodes.skip import SkipNode
 from xsdata.formats.dataclass.parsers.nodes.standard import StandardNode
 from xsdata.formats.dataclass.parsers.nodes.union import UnionNode
 from xsdata.formats.dataclass.parsers.nodes.wildcard import WildcardNode
+from xsdata.formats.dataclass.parsers.nodes.wrapper import WrapperNode
 
 __all__ = [
     "ElementNode",
     "PrimitiveNode",
     "SkipNode",
     "StandardNode",
     "UnionNode",
     "WildcardNode",
+    "WrapperNode",
 ]
```

### Comparing `xsdata-22.9/xsdata/formats/dataclass/parsers/nodes/element.py` & `xsdata-23.5/xsdata/formats/dataclass/parsers/nodes/element.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,14 @@
         self.xsi_nil = xsi_nil
         self.assigned: Set[int] = set()
         self.tail_processed: bool = False
 
     def bind(
         self, qname: str, text: Optional[str], tail: Optional[str], objects: List
     ) -> bool:
-
         obj: Any = None
         if not self.xsi_nil or self.meta.nillable:
             params: Dict = {}
             self.bind_attrs(params)
             self.bind_content(params, text, tail, objects)
             obj = self.config.class_factory(self.meta.clazz, params)
 
@@ -209,15 +208,14 @@
         Add the given value to the params dictionary with the wildcard var name
         as key.
 
         If the key is already present wrap the previous value into a
         generic AnyElement instance. If the previous value is already a
         generic instance add the current value as a child object.
         """
-
         value = self.prepare_generic_value(qname, value, var)
 
         if var.list_element:
             items = params.get(var.name)
             if items is None:
                 params[var.name] = PendingCollection([value], var.factory)
             else:
@@ -268,15 +266,14 @@
     def bind_text(self, params: Dict, text: Optional[str]) -> bool:
         """
         Add the given element's text content if any to the params dictionary
         with the text var name as key.
 
         Return if any data was bound.
         """
-
         var = self.meta.text
 
         if not var or (text is None and not self.xsi_nil):
             return False
 
         if var.init:
             if self.xsi_nil and not text:
@@ -366,24 +363,27 @@
         xsi_type = ParserUtils.xsi_type(attrs, ns_map)
         xsi_nil = ParserUtils.xsi_nil(attrs)
         derived_factory = self.context.class_type.derived_element
 
         if var.clazz:
             return self.build_element_node(
                 var.clazz,
+                var.derived,
                 attrs,
                 ns_map,
                 position,
-                derived_factory if var.derived else None,
+                derived_factory,
                 xsi_type,
                 xsi_nil,
             )
 
         if not var.any_type and not var.is_wildcard:
-            return nodes.PrimitiveNode(var, ns_map, derived_factory)
+            return nodes.PrimitiveNode(
+                var, ns_map, self.meta.mixed_content, derived_factory
+            )
 
         datatype = DataType.from_qname(xsi_type) if xsi_type else None
         derived = var.derived or var.is_wildcard
         if datatype:
             return nodes.StandardNode(
                 datatype, ns_map, var.nillable, derived_factory if derived else None
             )
@@ -392,18 +392,19 @@
         clazz = None
         if xsi_type:
             clazz = self.context.find_type(xsi_type)
 
         if clazz:
             node = self.build_element_node(
                 clazz,
+                derived,
                 attrs,
                 ns_map,
                 position,
-                derived_factory if derived else None,
+                derived_factory,
                 xsi_type,
                 xsi_nil,
             )
 
         if node:
             return node
 
@@ -414,32 +415,35 @@
             position=position,
             factory=self.context.class_type.any_element,
         )
 
     def build_element_node(
         self,
         clazz: Type,
+        derived: bool,
         attrs: Dict,
         ns_map: Dict,
         position: int,
-        derived_factory: Optional[Type] = None,
+        derived_factory: Type,
         xsi_type: Optional[str] = None,
         xsi_nil: Optional[bool] = None,
     ) -> Optional[XmlNode]:
-
         meta = self.context.fetch(clazz, self.meta.namespace, xsi_type)
 
         if not meta or (meta.nillable and xsi_nil is False):
             return None
 
+        if xsi_type and not derived and not issubclass(meta.clazz, clazz):
+            derived = True
+
         return ElementNode(
             meta=meta,
             config=self.config,
             attrs=attrs,
             ns_map=ns_map,
             context=self.context,
             position=position,
-            derived_factory=derived_factory,
+            derived_factory=derived_factory if derived else None,
             xsi_type=xsi_type,
             xsi_nil=xsi_nil,
             mixed=self.meta.mixed_content,
         )
```

### Comparing `xsdata-22.9/xsdata/formats/dataclass/parsers/nodes/primitive.py` & `xsdata-23.5/xsdata/formats/dataclass/parsers/nodes/primitive.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,23 +11,25 @@
 
 class PrimitiveNode(XmlNode):
     """
     XmlNode for text elements with primitive values like str, int, float.
 
     :param var: Class field xml var instance
     :param ns_map: Namespace prefix-URI map
+    :param mixed: The node supports mixed content
     :param derived_factory: Derived element factory
     """
 
     __slots__ = "var", "ns_map", "derived_factory"
 
-    def __init__(self, var: XmlVar, ns_map: Dict, derived_factory: Type):
+    def __init__(self, var: XmlVar, ns_map: Dict, mixed: bool, derived_factory: Type):
         self.var = var
         self.ns_map = ns_map
         self.derived_factory = derived_factory
+        self.mixed = mixed
 
     def bind(
         self, qname: str, text: Optional[str], tail: Optional[str], objects: List
     ) -> bool:
         obj = ParserUtils.parse_value(
             value=text,
             types=self.var.types,
@@ -40,11 +42,17 @@
         if obj is None and not self.var.nillable:
             obj = ""
 
         if self.var.derived:
             obj = self.derived_factory(qname=qname, value=obj)
 
         objects.append((qname, obj))
+
+        if self.mixed:
+            tail = ParserUtils.normalize_content(tail)
+            if tail:
+                objects.append((None, tail))
+
         return True
 
     def child(self, qname: str, attrs: Dict, ns_map: Dict, position: int) -> XmlNode:
         raise XmlContextError("Primitive node doesn't support child nodes!")
```

### Comparing `xsdata-22.9/xsdata/formats/dataclass/parsers/nodes/skip.py` & `xsdata-23.5/xsdata/formats/dataclass/parsers/nodes/skip.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/xsdata/formats/dataclass/parsers/nodes/standard.py` & `xsdata-23.5/xsdata/formats/dataclass/parsers/nodes/standard.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/xsdata/formats/dataclass/parsers/nodes/union.py` & `xsdata-23.5/xsdata/formats/dataclass/parsers/nodes/union.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,14 @@
 
         self.events.insert(0, ("start", qname, copy.deepcopy(self.attrs), self.ns_map))
 
         obj = None
         max_score = -1.0
         parent_namespace = target_uri(qname)
         for clazz in self.var.types:
-
             if self.context.class_type.is_model(clazz):
                 self.context.build(clazz, parent_ns=parent_namespace)
                 candidate = self.parse_class(clazz)
             else:
                 candidate = self.parse_value(text, [clazz])
 
             score = self.context.class_type.score_object(candidate)
```

### Comparing `xsdata-22.9/xsdata/formats/dataclass/parsers/nodes/wildcard.py` & `xsdata-23.5/xsdata/formats/dataclass/parsers/nodes/wildcard.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/xsdata/formats/dataclass/parsers/tree.py` & `xsdata-23.5/xsdata/formats/dataclass/parsers/tree.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,15 +50,15 @@
                 factory=None,
                 tokens_factory=None,
                 format=None,
                 derived=False,
                 any_type=False,
                 required=False,
                 nillable=False,
-                sequential=False,
+                sequence=None,
                 default=None,
                 namespaces=(),
                 elements={},
                 wildcards=(),
             )
 
             child = WildcardNode(
```

### Comparing `xsdata-22.9/xsdata/formats/dataclass/parsers/utils.py` & `xsdata-23.5/xsdata/formats/dataclass/parsers/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,23 +42,22 @@
         return xsi_nil == constants.XML_TRUE if xsi_nil else None
 
     @classmethod
     def parse_value(
         cls,
         value: Any,
         types: Sequence[Type],
-        default: Any = None,
+        default: Optional[Any] = None,
         ns_map: Optional[Dict] = None,
-        tokens_factory: Callable = None,
+        tokens_factory: Optional[Callable] = None,
         format: Optional[str] = None,
     ) -> Any:
         """Convert xml string values to s python primitive type."""
 
         if value is None:
-
             if callable(default):
                 return default() if tokens_factory else None
 
             return default
 
         if tokens_factory:
             value = value if collections.is_array(value) else value.split()
```

### Comparing `xsdata-22.9/xsdata/formats/dataclass/parsers/xml.py` & `xsdata-23.5/xsdata/formats/dataclass/parsers/xml.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,14 @@
 
             event=start, name={urn}bookTitle -> start_booking_title(**kwargs)
 
         :param event: Event type start|end
         :param name: Element qualified name
         :param kwargs: Event keyword arguments
         """
-
         key = (event, name)
         if key not in self.emit_cache:
             method_name = f"{event}_{snake_case(local_name(name))}"
             self.emit_cache[key] = getattr(self, method_name, None)
 
         method = self.emit_cache[key]
         if method:
```

### Comparing `xsdata-22.9/xsdata/formats/dataclass/serializers/code.py` & `xsdata-23.5/xsdata/formats/dataclass/serializers/code.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 from xsdata.formats.dataclass.serializers.config import SerializerConfig
 from xsdata.utils import collections
 from xsdata.utils.objects import literal_value
 
 spaces = "    "
 
 
+unset = object()
+
+
 @dataclass
 class PycodeSerializer(AbstractSerializer):
     """
     Pycode serializer for dataclasses.
 
     Return a python representation code of
     a model instance.
@@ -67,18 +70,16 @@
 
     @classmethod
     def build_imports(cls, types: Set[Type]) -> str:
         imports = []
         for tp in types:
             module = tp.__module__
             name = tp.__qualname__
-            if module == "builtins" or "." in name:
-                continue
-
-            imports.append(f"from {module} import {name}\n")
+            if module != "builtins" and "." not in name:
+                imports.append(f"from {module} import {name}\n")
 
         return "".join(sorted(imports))
 
     def write_object(self, obj: Any, level: int, types: Set[Type]):
         types.add(type(obj))
         if collections.is_array(obj):
             yield from self.write_array(obj, level, types)
@@ -121,20 +122,29 @@
 
         yield f"{spaces * level}}}"
 
     def write_class(self, obj: Any, level: int, types: Set[Type]):
         yield f"{obj.__class__.__qualname__}(\n"
 
         next_level = level + 1
-        for index, f in enumerate(self.context.class_type.get_fields(obj)):
+        index = 0
+        for f in self.context.class_type.get_fields(obj):
             if not f.init:
                 continue
 
+            value = getattr(obj, f.name, types)
+            default = self.context.class_type.default_value(f, default=unset)
+            if default is not unset and (
+                (callable(default) and default() == value) or default == value
+            ):
+                continue
+
             if index:
                 yield f",\n{spaces * next_level}{f.name}="
             else:
                 yield f"{spaces * next_level}{f.name}="
 
-            value = getattr(obj, f.name, types)
             yield from self.write_object(value, next_level, types)
 
+            index += 1
+
         yield f"\n{spaces * level})"
```

### Comparing `xsdata-22.9/xsdata/formats/dataclass/serializers/config.py` & `xsdata-23.5/xsdata/formats/dataclass/serializers/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,47 +1,58 @@
+from typing import Callable
+from typing import Dict
 from typing import Optional
 
 
 class SerializerConfig:
     """
     Serializer configuration options.
 
     Some options are not applicable for both xml or json documents.
 
     :param encoding: Text encoding
     :param xml_version: XML Version number (1.0|1.1)
     :param xml_declaration: Generate XML declaration
     :param pretty_print: Enable pretty output
+    :param pretty_print_indent: Indentation string for each indent level
     :param ignore_default_attributes: Ignore optional attributes with
         default values
     :param schema_location: xsi:schemaLocation attribute value
     :param no_namespace_schema_location: xsi:noNamespaceSchemaLocation
         attribute value
+    :param globalns: Dictionary containing global variables to extend
+        or overwrite for typing
     """
 
     __slots__ = (
         "encoding",
         "xml_version",
         "xml_declaration",
         "pretty_print",
+        "pretty_print_indent",
         "ignore_default_attributes",
         "schema_location",
         "no_namespace_schema_location",
+        "globalns",
     )
 
     def __init__(
         self,
         encoding: str = "UTF-8",
         xml_version: str = "1.0",
         xml_declaration: bool = True,
         pretty_print: bool = False,
+        pretty_print_indent: Optional[str] = None,
         ignore_default_attributes: bool = False,
         schema_location: Optional[str] = None,
         no_namespace_schema_location: Optional[str] = None,
+        globalns: Optional[Dict[str, Callable]] = None,
     ):
         self.encoding = encoding
         self.xml_version = xml_version
         self.xml_declaration = xml_declaration
         self.pretty_print = pretty_print
+        self.pretty_print_indent = pretty_print_indent
         self.ignore_default_attributes = ignore_default_attributes
         self.schema_location = schema_location
         self.no_namespace_schema_location = no_namespace_schema_location
+        self.globalns = globalns
```

### Comparing `xsdata-22.9/xsdata/formats/dataclass/serializers/json.py` & `xsdata-23.5/xsdata/formats/dataclass/serializers/json.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import Iterator
 from typing import Optional
 from typing import TextIO
 from typing import Tuple
+from typing import Union
 
 from xsdata.formats.bindings import AbstractSerializer
 from xsdata.formats.converter import converter
 from xsdata.formats.dataclass.context import XmlContext
 from xsdata.formats.dataclass.models.elements import XmlVar
 from xsdata.formats.dataclass.serializers.config import SerializerConfig
 from xsdata.utils import collections
@@ -57,30 +58,28 @@
     def write(self, out: TextIO, obj: Any):
         """
         Write the given object tree to the output text stream.
 
         :param out: The output stream
         :param obj: The input dataclass instance
         """
-
-        indent: Optional[int] = None
+        indent: Optional[Union[int, str]] = None
         if self.indent:
             warnings.warn(
                 "JsonSerializer indent property is deprecated, use SerializerConfig",
                 DeprecationWarning,
             )
             indent = self.indent
         elif self.config.pretty_print:
-            indent = 2
+            indent = self.config.pretty_print_indent or 2
 
         self.dump_factory(self.convert(obj), out, indent=indent)
 
     def convert(self, obj: Any, var: Optional[XmlVar] = None) -> Any:
         if var is None or self.context.class_type.is_model(obj):
-
             if collections.is_array(obj):
                 return [self.convert(o) for o in obj]
 
             return self.dict_factory(self.next_value(obj))
 
         if collections.is_array(obj):
             return type(obj)(self.convert(v, var) for v in obj)
@@ -92,13 +91,15 @@
             return self.convert(obj.value, var)
 
         return converter.serialize(obj, format=var.format)
 
     def next_value(self, obj: Any) -> Iterator[Tuple[str, Any]]:
         ignore_optionals = self.config.ignore_default_attributes
 
-        for var in self.context.build(obj.__class__).get_all_vars():
+        for var in self.context.build(
+            obj.__class__, globalns=self.config.globalns
+        ).get_all_vars():
             value = getattr(obj, var.name)
             if var.is_attribute and ignore_optionals and var.is_optional(value):
                 continue
 
             yield var.local_name, self.convert(value, var)
```

### Comparing `xsdata-22.9/xsdata/formats/dataclass/serializers/mixins.py` & `xsdata-23.5/xsdata/formats/dataclass/serializers/mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,14 @@
         also generate any missing namespace prefixes.
 
         :param key: Attribute name
         :param value: Attribute value
         :param check_pending: Raise exception if not no element is
             pending start
         """
-
         if not self.pending_tag and check_pending:
             raise XmlWriterError("Empty pending tag.")
 
         if self.is_xsi_type(key, value):
             value = QName(value)
 
         name = split_qname(key)
@@ -237,17 +236,15 @@
         not empty, prepare and send the namespaces prefix mappings and
         the element with its attributes to the content handler for
         generation.
 
         :param is_nil: If true add ``xsi:nil="true"`` to the element
             attributes
         """
-
         if self.pending_tag:
-
             if not is_nil:
                 self.attrs.pop(XSI_NIL, None)
 
             for name in self.attrs.keys():
                 self.add_namespace(name[0])
 
             self.reset_default_namespace()
@@ -262,16 +259,15 @@
         """
         Send the new prefixes and namespaces added in the current context to
         the content handler.
 
         Save the list of prefixes to be removed at the end of the
         current pending tag.
         """
-
-        prefixes = []
+        prefixes: List[str] = []
         self.pending_prefixes.append(prefixes)
 
         try:
             parent_ns_map = self.ns_context[-2]
         except IndexError:
             parent_ns_map = EMPTY_MAP
 
@@ -279,27 +275,26 @@
             if parent_ns_map.get(prefix) != uri:
                 prefixes.append(prefix)
                 self.handler.startPrefixMapping(prefix, uri)
 
     def reset_default_namespace(self):
         """Reset the default namespace if exists and the current pending tag is
         not qualified."""
-        if not self.pending_tag[0] and None in self.ns_map:
+        if self.pending_tag and not self.pending_tag[0] and None in self.ns_map:
             self.ns_map[None] = ""
 
     @classmethod
     def is_xsi_type(cls, key: str, value: Any) -> bool:
         """
         Return whether the value is an xsi:type or not based on the given
         attribute name/value.
 
         :param key: Attribute name
         :param value: Attribute value
         """
-
         if isinstance(value, str) and value.startswith("{"):
             return key == QNames.XSI_TYPE or DataType.from_qname(value) is not None
 
         return False
 
     def encode_data(self, data: Any) -> Optional[str]:
         """Encode data for xml rendering."""
```

### Comparing `xsdata-22.9/xsdata/formats/dataclass/serializers/writers/__init__.py` & `xsdata-23.5/xsdata/formats/dataclass/serializers/writers/__init__.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/xsdata/formats/dataclass/serializers/writers/lxml.py` & `xsdata-23.5/xsdata/formats/dataclass/serializers/writers/lxml.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Dict
 from typing import Generator
 from typing import TextIO
 
+from lxml.etree import indent
 from lxml.etree import tostring
 from lxml.sax import ElementTreeContentHandler
 
 from xsdata.formats.dataclass.serializers.config import SerializerConfig
 from xsdata.formats.dataclass.serializers.mixins import XmlWriter
 
 
@@ -33,14 +34,17 @@
         self.handler = ElementTreeContentHandler()
 
     def write(self, events: Generator):
         super().write(events)
 
         assert isinstance(self.handler, ElementTreeContentHandler)
 
+        if self.config.pretty_print and self.config.pretty_print_indent is not None:
+            indent(self.handler.etree, self.config.pretty_print_indent)
+
         xml = tostring(
             self.handler.etree,
             encoding=self.config.encoding,
             pretty_print=self.config.pretty_print,
             xml_declaration=False,
         ).decode()
```

### Comparing `xsdata-22.9/xsdata/formats/dataclass/serializers/writers/native.py` & `xsdata-23.5/xsdata/formats/dataclass/serializers/writers/native.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,27 +38,31 @@
 
     def start_tag(self, qname: str):
         super().start_tag(qname)
 
         if self.config.pretty_print:
             if self.current_level:
                 self.handler.ignorableWhitespace("\n")
-                self.handler.ignorableWhitespace("  " * self.current_level)
+                self.handler.ignorableWhitespace(
+                    (self.config.pretty_print_indent or "  ") * self.current_level
+                )
 
             self.current_level += 1
             self.pending_end_element = False
 
     def end_tag(self, qname: str):
         if not self.config.pretty_print:
             super().end_tag(qname)
             return
 
         self.current_level -= 1
         if self.pending_end_element:
             self.handler.ignorableWhitespace("\n")
-            self.handler.ignorableWhitespace("  " * self.current_level)
+            self.handler.ignorableWhitespace(
+                (self.config.pretty_print_indent or "  ") * self.current_level
+            )
 
         super().end_tag(qname)
 
         self.pending_end_element = True
         if not self.current_level:
             self.handler.ignorableWhitespace("\n")
```

### Comparing `xsdata-22.9/xsdata/formats/dataclass/serializers/xml.py` & `xsdata-23.5/xsdata/formats/dataclass/serializers/xml.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,17 @@
         )
         handler.write(events)
 
     def write_object(self, obj: Any):
         """Produce an events stream from a dataclass or a derived element."""
         qname = xsi_type = None
         if isinstance(obj, self.context.class_type.derived_element):
-            meta = self.context.build(obj.value.__class__)
+            meta = self.context.build(
+                obj.value.__class__, globalns=self.config.globalns
+            )
             qname = obj.qname
             obj = obj.value
             xsi_type = namespaces.real_xsi_type(qname, meta.target_qname)
 
         yield from self.write_dataclass(obj, qname=qname, xsi_type=xsi_type)
 
     def write_dataclass(
@@ -95,16 +97,17 @@
     ) -> Generator:
         """
         Produce an events stream from a dataclass.
 
         Optionally override the qualified name and the xsi properties
         type and nil.
         """
-
-        meta = self.context.build(obj.__class__, namespace)
+        meta = self.context.build(
+            obj.__class__, namespace, globalns=self.config.globalns
+        )
         qname = qname or meta.qname
         nillable = nillable or meta.nillable
         namespace, tag = namespaces.split_qname(qname)
 
         yield XmlWriterEvent.START, qname
 
         for key, value in self.next_attribute(
@@ -154,16 +157,22 @@
         else:
             yield from self.write_any_type(value, var, namespace)
 
     def write_list(
         self, values: Iterable, var: XmlVar, namespace: NoneStr
     ) -> Generator:
         """Produce an events stream for the given list of values."""
-        for value in values:
-            yield from self.write_value(value, var, namespace)
+        if var.wrapper is not None:
+            yield XmlWriterEvent.START, var.wrapper
+            for value in values:
+                yield from self.write_value(value, var, namespace)
+            yield XmlWriterEvent.END, var.wrapper
+        else:
+            for value in values:
+                yield from self.write_value(value, var, namespace)
 
     def write_tokens(self, value: Any, var: XmlVar, namespace: NoneStr) -> Generator:
         """Produce an events stream for the given tokens list or list of tokens
         lists."""
         if value is not None or var.nillable:
             if value and collections.is_array(value[0]):
                 for val in value:
@@ -320,38 +329,43 @@
         """
         index = 0
         attrs = meta.get_element_vars()
         stop = len(attrs)
         while index < stop:
             var = attrs[index]
 
-            if not var.sequential:
+            if var.sequence is None:
                 value = getattr(obj, var.name)
                 if value is not None or var.nillable:
                     yield var, value
                 index += 1
                 continue
 
-            indices = range(index + 1, stop)
-            end = next((i for i in indices if not attrs[i].sequential), stop)
-            sequence = attrs[index:end]
-            index = end
+            indices = range(index, stop)
+            end = next(i for i in indices[::-1] if attrs[i].sequence == var.sequence)
+            sequence = attrs[index : end + 1]
+            index = end + 1
             j = 0
 
             rolling = True
             while rolling:
                 rolling = False
                 for var in sequence:
                     values = getattr(obj, var.name)
-                    if j < len(values):
+                    if collections.is_array(values):
+                        if j < len(values):
+                            rolling = True
+                            value = values[j]
+                            if value is not None or var.nillable:
+                                yield var, value
+                    elif j == 0:
                         rolling = True
-                        value = values[j]
+                        if values is not None or var.nillable:
+                            yield var, values
 
-                        if value is not None or var.nillable:
-                            yield var, value
                 j += 1
 
     @classmethod
     def next_attribute(
         cls,
         obj: Any,
         meta: XmlMeta,
@@ -397,16 +411,16 @@
 
         Converts values to strings. QName instances is an exception,
         those values need to wait until the XmlWriter assigns prefixes
         to namespaces per element node. Enums and Tokens may contain
         QName(s) so they also get a special treatment.
 
         We can't do all the conversions in the writer because we would
-        need to carry the xml vars inside the writer. Instead of that
-        we do the easy encoding here and leave the qualified names for
+        need to carry the xml vars inside the writer. Instead of that we
+        do the easy encoding here and leave the qualified names for
         later.
         """
         if isinstance(value, (str, QName)) or var is None:
             return value
 
         if collections.is_array(value):
             return [cls.encode(v, var) for v in value]
```

### Comparing `xsdata-22.9/xsdata/formats/dataclass/templates/class.jinja2` & `xsdata-23.5/xsdata/formats/dataclass/templates/class.jinja2`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/xsdata/formats/dataclass/templates/enum.jinja2` & `xsdata-23.5/xsdata/formats/dataclass/templates/enum.jinja2`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/xsdata/formats/dataclass/transports.py` & `xsdata-23.5/xsdata/formats/dataclass/transports.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from typing import Any
 from typing import Dict
 
 import requests
 
 
 class Transport(abc.ABC):
-
     __slots__ = ()
 
     @abc.abstractmethod
     def get(self, url: str, params: Dict, headers: Dict) -> bytes:
         """Send a GET request."""
 
     @abc.abstractmethod
```

### Comparing `xsdata-22.9/xsdata/formats/dataclass/typing.py` & `xsdata-23.5/xsdata/formats/dataclass/typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import _eval_type  # type: ignore
 from typing import Any
 from typing import Dict
 from typing import Iterator
 from typing import List
+from typing import Optional
 from typing import Tuple
 from typing import Type
 from typing import TypeVar
 from typing import Union
 
 NONE_TYPE = type(None)
 EMPTY_ARGS = ()
@@ -45,15 +46,17 @@
     return None
 
 
 def get_args(tp: Any) -> Tuple:
     return getattr(tp, "__args__", EMPTY_ARGS) or EMPTY_ARGS
 
 
-def evaluate(tp: Any, globalns: Any = None, localns: Any = None) -> Tuple[Type, ...]:
+def evaluate(
+    tp: Any, globalns: Optional[Any] = None, localns: Optional[Any] = None
+) -> Tuple[Type, ...]:
     return tuple(_evaluate(_eval_type(tp, globalns, localns)))
 
 
 def _evaluate(tp: Any) -> Iterator[Type]:
     origin = get_origin(tp)
 
     func = __evaluations__.get(origin)
@@ -109,15 +112,14 @@
 
 
 def _evaluate_tuple(tp: Any) -> Iterator[Type]:
     yield tuple
 
     args = get_args(tp)
     for arg in args:
-
         if arg is Ellipsis:
             continue
 
         origin = get_origin(arg)
         if origin is None:
             yield arg
         elif origin in (Union, List, Tuple, TypeVar):
```

### Comparing `xsdata-22.9/xsdata/models/config.py` & `xsdata-23.5/xsdata/models/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -241,14 +241,17 @@
     :param filter_strategy: Class filter strategy, default: globals
     :param relative_imports: Use relative imports, default: false
     :param compound_fields: Use compound fields for repeatable elements, default: false
     :param max_line_length: Adjust the maximum line length, default: 79
     :param postponed_annotations: Enable postponed evaluation of annotations,
         default: false, python>=3.7 Only
     :param unnest_classes: Move inner classes to upper level, default: false
+    :param ignore_patterns: Ignore pattern restrictions, default: false
+    :param include_header: Include a header with codegen information in the output,
+        default: false
     """
 
     package: str = element(default="generated")
     format: OutputFormat = element(default_factory=OutputFormat)
     structure_style: StructureStyle = element(
         default=StructureStyle.FILENAMES, name="Structure"
     )
@@ -257,14 +260,16 @@
         default=ClassFilterStrategy.ALL_GLOBALS
     )
     relative_imports: bool = element(default=False)
     compound_fields: CompoundFields = element(default_factory=CompoundFields)
     max_line_length: int = attribute(default=79)
     postponed_annotations: bool = element(default=False)
     unnest_classes: bool = element(default=False)
+    ignore_patterns: bool = element(default=False)
+    include_header: bool = element(default=False)
 
     def update(self, **kwargs: Any):
         objects.update(self, **kwargs)
         self.format.validate()
 
 
 @dataclass
@@ -434,15 +439,17 @@
             obj.substitutions.substitution.append(
                 GeneratorSubstitution(
                     type=ObjectType.PACKAGE, search=ns.uri, replace=ns.prefix
                 )
             )
 
         obj.substitutions.substitution.append(
-            GeneratorSubstitution(type=ObjectType.CLASS, search="Class", replace="Type")
+            GeneratorSubstitution(
+                type=ObjectType.CLASS, search="(.*)Class$", replace="\\1Type"
+            )
         )
 
         return obj
 
     @classmethod
     def read(cls, path: Path) -> "GeneratorConfig":
         if not path.exists():
```

### Comparing `xsdata-22.9/xsdata/models/datatype.py` & `xsdata-23.5/xsdata/models/datatype.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     @classmethod
     def from_date(cls, obj: datetime.date) -> "XmlDate":
         """
         Initialize from :class:`datetime.date` instance.
 
         .. warning::
 
-            date instances don't have timezone information!
+        date instances don't have timezone information!
         """
         return cls(obj.year, obj.month, obj.day)
 
     @classmethod
     def from_datetime(cls, obj: datetime.datetime) -> "XmlDate":
         """Initialize from :class:`datetime.datetime` instance."""
         return cls(obj.year, obj.month, obj.day, calculate_offset(obj))
```

### Comparing `xsdata-22.9/xsdata/models/dtd.py` & `xsdata-23.5/xsdata/models/dtd.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/xsdata/models/enums.py` & `xsdata-23.5/xsdata/models/enums.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/xsdata/models/mixins.py` & `xsdata-23.5/xsdata/models/mixins.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/xsdata/models/wsdl.py` & `xsdata-23.5/xsdata/models/wsdl.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/xsdata/models/xsd.py` & `xsdata-23.5/xsdata/models/xsd.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,15 +266,14 @@
 
     @property
     def real_name(self) -> str:
         return DEFAULT_ATTR_NAME
 
     @property
     def attr_types(self) -> Iterator[str]:
-
         for simple_type in self.simple_types:
             yield from simple_type.attr_types
 
         if self.member_types:
             yield from self.member_types.split()
 
     def get_restrictions(self) -> Dict[str, Anything]:
@@ -326,14 +325,19 @@
         if self.simple_type:
             yield from self.simple_type.attr_types
         elif self.type:
             yield self.type
         elif self.ref:
             yield self.ref
 
+    @property
+    def default_type(self) -> str:
+        datatype = DataType.STRING if self.fixed else DataType.ANY_SIMPLE_TYPE
+        return datatype.prefixed(self.xs_prefix)
+
     def get_restrictions(self) -> Dict[str, Anything]:
         if self.use == UseType.REQUIRED:
             restrictions = {"min_occurs": 1, "max_occurs": 1}
         elif self.use == UseType.PROHIBITED:
             restrictions = {"max_occurs": 0, "min_occurs": 0}
         else:
             restrictions = {"max_occurs": 1, "min_occurs": 0}
@@ -433,16 +437,15 @@
     elements: Array["Element"] = array_element(name="element")
     groups: Array["Group"] = array_element(name="group")
 
     def get_restrictions(self) -> Dict[str, Anything]:
         max_occurs = sys.maxsize if self.max_occurs == "unbounded" else self.max_occurs
 
         return {
-            "min_occurs": self.min_occurs,
-            "max_occurs": max_occurs,
+            "path": [("a", id(self), self.min_occurs, max_occurs)],
         }
 
 
 @dataclass
 class Sequence(AnnotationBase):
     """
     Model representation of a schema xs:sequence element.
@@ -464,17 +467,15 @@
     sequences: Array["Sequence"] = array_element(name="sequence")
     any: Array["Any"] = array_element()
 
     def get_restrictions(self) -> Dict[str, Anything]:
         max_occurs = sys.maxsize if self.max_occurs == "unbounded" else self.max_occurs
 
         return {
-            "sequential": True,
-            "min_occurs": self.min_occurs,
-            "max_occurs": max_occurs,
+            "path": [("s", id(self), self.min_occurs, max_occurs)],
         }
 
 
 @dataclass
 class Choice(AnnotationBase):
     """
     Model representation of a schema xs:choice element.
@@ -493,21 +494,18 @@
     elements: Array["Element"] = array_element(name="element")
     groups: Array["Group"] = array_element(name="group")
     choices: Array["Choice"] = array_element(name="choice")
     sequences: Array[Sequence] = array_element(name="sequence")
     any: Array["Any"] = array_element()
 
     def get_restrictions(self) -> Dict[str, Anything]:
-        min_occurs = self.min_occurs if self.min_occurs > 1 else 0
         max_occurs = sys.maxsize if self.max_occurs == "unbounded" else self.max_occurs
 
         return {
-            "choice": str(id(self)),
-            "min_occurs": min_occurs,
-            "max_occurs": max_occurs,
+            "path": [("c", id(self), self.min_occurs, max_occurs)],
         }
 
 
 @dataclass
 class Group(AnnotationBase):
     """
     Model representation of a schema xs:group element.
@@ -538,16 +536,15 @@
         if self.ref:
             yield self.ref
 
     def get_restrictions(self) -> Dict[str, Anything]:
         max_occurs = sys.maxsize if self.max_occurs == "unbounded" else self.max_occurs
 
         return {
-            "min_occurs": self.min_occurs,
-            "max_occurs": max_occurs,
+            "path": [("g", id(self), self.min_occurs, max_occurs)],
         }
 
 
 @dataclass
 class OpenContent(AnnotationBase):
     """
     Model representation of a schema xs:openContent element.
@@ -1045,16 +1042,15 @@
     @property
     def bases(self) -> Iterator[str]:
         if self.type:
             yield self.type
 
     def get_restrictions(self) -> Dict[str, Anything]:
         return {
-            "choice": str(id(self)),
-            "min_occurs": 0,
+            "path": [("alt", id(self), 0, 1)],
         }
 
 
 @dataclass
 class Element(AnnotationBase):
     """
     Model representation of a schema xs:element element.
```

### Comparing `xsdata-22.9/xsdata/schemas/mathml3-common.xsd` & `xsdata-23.5/xsdata/schemas/mathml3-common.xsd`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/xsdata/schemas/mathml3-content.xsd` & `xsdata-23.5/xsdata/schemas/mathml3-content.xsd`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/xsdata/schemas/mathml3-presentation.xsd` & `xsdata-23.5/xsdata/schemas/mathml3-presentation.xsd`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/xsdata/schemas/mathml3-strict-content.xsd` & `xsdata-23.5/xsdata/schemas/mathml3-strict-content.xsd`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/xsdata/schemas/xlink.xsd` & `xsdata-23.5/xsdata/schemas/xlink.xsd`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/xsdata/schemas/xml.xsd` & `xsdata-23.5/xsdata/schemas/xml.xsd`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/xsdata/utils/click.py` & `xsdata-23.5/xsdata/utils/click.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     }
 
     def format(self, record: logging.LogRecord) -> str:
         if not record.exc_info:
             level = record.levelname.lower()
             msg = record.getMessage()
             if level in self.colors:
-                prefix = click.style(f"{level}:", **self.colors[level])
+                prefix = click.style(f"{level}", **self.colors[level])
                 msg = f"{prefix}: {msg}"
             return msg
 
         return super().format(record)  # pragma: no cover
 
 
 class LogHandler(logging.Handler):
```

### Comparing `xsdata-22.9/xsdata/utils/collections.py` & `xsdata-23.5/xsdata/utils/collections.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 from typing import Callable
 from typing import Dict
 from typing import Iterable
 from typing import Iterator
 from typing import List
 from typing import Optional
 from typing import Sequence
+from typing import Set
 from typing import TypeVar
 
 T = TypeVar("T")
 
 
 def is_array(value: Any) -> bool:
-    if isinstance(value, (list, tuple, set)):
+    if isinstance(value, tuple):
         return not hasattr(value, "_fields")
 
-    return False
+    return isinstance(value, (list, set, frozenset))
 
 
 def unique_sequence(items: Iterable[T], key: Optional[str] = None) -> List[T]:
     """
     Return a new list with the unique values from an iterable.
 
     Optionally you can also provide a lambda to generate the unique key
@@ -73,7 +74,41 @@
     """Return the first item of the iterator."""
     return next(items, None)
 
 
 def prepend(target: List, *args: Any):
     """Prepend items to the target list."""
     target[:0] = args
+
+
+def connected_components(lists: List[List[Any]]) -> Iterator[List[Any]]:
+    """
+    Merge lists of lists that share common elements.
+
+    https://stackoverflow.com/questions/4842613/merge-lists-that-share-
+    common-elements
+    """
+    neighbors = defaultdict(set)
+    for each in lists:
+        for item in each:
+            neighbors[item].update(each)
+
+    def component(node: Any, neigh: Dict[Any, Set], see: Set[Any]):
+        nodes = {node}
+        while nodes:
+            next_node = nodes.pop()
+            see.add(next_node)
+            nodes |= neigh[next_node] - see
+            yield next_node
+
+    seen: Set[Any] = set()
+    for item in neighbors:
+        if item not in seen:
+            yield sorted(component(item, neighbors, seen))
+
+
+def find_connected_component(groups: List[List[Any]], value: Any) -> int:
+    for index, group in enumerate(groups):
+        if value in group:
+            return index
+
+    return -1
```

### Comparing `xsdata-22.9/xsdata/utils/dates.py` & `xsdata-23.5/xsdata/utils/dates.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,15 +227,14 @@
         while max_digits and self.has_more() and self.peek().isdigit():
             self.vidx += 1
             max_digits -= 1
 
         return int(self.value[start : self.vidx].ljust(just, "0"))
 
     def parse_offset(self) -> Optional[int]:
-
         if not self.has_more():
             return None
 
         ctrl = self.peek()
         if ctrl == "Z":
             self.vidx += 1
             return 0
```

### Comparing `xsdata-22.9/xsdata/utils/debug.py` & `xsdata-23.5/xsdata/utils/debug.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 def dump(obj: Any):
     """
     Write any object into a dump json file.
 
     For internal troubleshooting purposes only!!!
     """
-
     with Path.cwd().joinpath("xsdata_dump.json").open("w+") as f:
         json.dump(convert(obj), f, indent=4)
 
 
 def convert(obj: Any) -> Any:
     """Dump any obj into a readable dictionary."""
     if not obj:
```

### Comparing `xsdata-22.9/xsdata/utils/downloader.py` & `xsdata-23.5/xsdata/utils/downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
     def __init__(self, output: Path):
         self.output = output
         self.base_path: Optional[Path] = None
         self.downloaded: Dict = {}
 
     def wget(self, uri: str, location: Optional[str] = None):
         """Download handler for any uri input with circular protection."""
-
         if not (uri in self.downloaded or (location and location in self.downloaded)):
             self.downloaded[uri] = None
             self.downloaded[location] = None
             self.adjust_base_path(uri)
 
             logger.info("Fetching %s", uri)
```

### Comparing `xsdata-22.9/xsdata/utils/graphs.py` & `xsdata-23.5/xsdata/utils/graphs.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     Compute Strongly Connected Components of a directed graph.
 
     From https://code.activestate.com/recipes/578507/
     From https://github.com/python/mypy/blob/master/mypy/build.py
 
     :param edges: Mapping of vertex-edges values
     """
-
     identified: Set[str] = set()
     stack: List[str] = []
     index: Dict[str, int] = {}
     boundaries: List[int] = []
 
     def dfs(v: str) -> Iterator[Set[str]]:
         index[v] = len(stack)
```

### Comparing `xsdata-22.9/xsdata/utils/namespaces.py` & `xsdata-23.5/xsdata/utils/namespaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,14 @@
     derived type."""
     return target_qname if target_qname != qname else None
 
 
 @functools.lru_cache(maxsize=50)
 def build_qname(tag_or_uri: Optional[str], tag: Optional[str] = None) -> str:
     """Create namespace qualified strings."""
-
     if not tag_or_uri:
         if not tag:
             raise ValueError("Invalid input both uri and tag are empty.")
 
         return tag
 
     return f"{{{tag_or_uri}}}{tag}" if tag else tag_or_uri
@@ -133,33 +132,30 @@
         return False
 
     char = name[0]
     if not char.isalpha() and not char == "_":
         return False
 
     for char in name[1:]:
-
         if char.isalpha() or char.isdigit() or char in NCNAME_PUNCTUATION:
             continue
         else:
             return False
 
     return True
 
 
 def is_uri(uri: Optional[str]) -> bool:
     """Verify given string is a valid uri."""
-
     return bool(URI_REGEX.search(uri)) if uri else False
 
 
 @functools.lru_cache(maxsize=50)
 def to_package_name(uri: Optional[str]) -> str:
     """Util method to convert a namespace to a dot style package name."""
-
     if not uri:
         return ""
 
     # Remove scheme
     domain_sep = "."
     if uri.startswith("http://"):
         uri = uri[7:]
```

### Comparing `xsdata-22.9/xsdata/utils/objects.py` & `xsdata-23.5/xsdata/utils/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from typing import Any
 from xml.etree.ElementTree import QName
 from xml.sax.saxutils import quoteattr
 
 
 def update(obj: Any, **kwargs: Any):
     """Update an object from keyword arguments with dotted keys."""
-
     for key, value in kwargs.items():
         attrsetter(obj, key, value)
 
 
 def attrsetter(obj: Any, attr: str, value: Any):
     names = attr.split(".")
     last = names.pop()
```

### Comparing `xsdata-22.9/xsdata/utils/package.py` & `xsdata-23.5/xsdata/utils/package.py`

 * *Files identical despite different names*

### Comparing `xsdata-22.9/xsdata/utils/testing.py` & `xsdata-23.5/xsdata/utils/testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     Namespace.XS.prefix: Namespace.XS.uri,
     Namespace.XSI.prefix: Namespace.XSI.uri,
     Namespace.XML.prefix: Namespace.XML.uri,
     Namespace.XLINK.prefix: Namespace.XLINK.uri,
 }
 
 
-def load_class(output: str, clazz_name: str) -> T:
+def load_class(output: str, clazz_name: str) -> Any:
     search = "Generating package: "
     start = len(search)
     packages = [line[start:] for line in output.splitlines() if line.startswith(search)]
 
     for package in reversed(packages):
         try:
             module = importlib.import_module(package)
@@ -123,15 +123,15 @@
         inner: Optional[List[Class]] = None,
         ns_map: Optional[Dict] = None,
         location: str = "tests.xsd",
         package: Optional[str] = None,
         module: Optional[str] = "tests",
         status: Status = Status.RAW,
         container: Optional[str] = None,
-        default: Any = None,
+        default: Optional[Any] = None,
         fixed: bool = False,
         prefix: str = "class_",
         **kwargs: Any,
     ) -> Class:
         if not qname:
             qname = build_qname("xsdata", f"{prefix}{cls.next_letter()}")
 
@@ -192,32 +192,38 @@
             attrs=AttrFactory.list(attributes, tag=Tag.ELEMENT),
             **kwargs,
         )
 
 
 class ExtensionFactory(Factory):
     counter = 65
+    tags = [Tag.ELEMENT, Tag.EXTENSION, Tag.RESTRICTION]
 
     @classmethod
     def create(
         cls,
         attr_type: Optional[AttrType] = None,
         restrictions: Optional[Restrictions] = None,
+        tag: Optional[str] = None,
         **kwargs: Any,
     ) -> Extension:
         return Extension(
+            tag=tag or random.choice(cls.tags),
             type=attr_type or AttrTypeFactory.create(**kwargs),
             restrictions=restrictions or Restrictions(),
         )
 
     @classmethod
     def reference(cls, qname: str, **kwargs: Any) -> Extension:
+        tag = kwargs.pop("tag", None)
         restrictions = kwargs.pop("restrictions", None)
         return cls.create(
-            AttrTypeFactory.create(qname=qname, **kwargs), restrictions=restrictions
+            AttrTypeFactory.create(qname=qname, **kwargs),
+            tag=tag,
+            restrictions=restrictions,
         )
 
     @classmethod
     def native(cls, datatype: DataType, **kwargs: Any) -> Extension:
         return cls.create(AttrTypeFactory.native(datatype), **kwargs)
 
 
@@ -262,15 +268,15 @@
         cls,
         name: Optional[str] = None,
         index: Optional[int] = None,
         types: Optional[List[AttrType]] = None,
         choices: Optional[List[Attr]] = None,
         tag: Optional[str] = None,
         namespace: Optional[str] = None,
-        default: Any = None,
+        default: Optional[Any] = None,
         fixed: bool = False,
         mixed: bool = False,
         restrictions: Optional[Restrictions] = None,
         prefix: str = "attr_",
         **kwargs: Any,
     ) -> Attr:
         name = name or f"{prefix}{cls.next_letter()}"
@@ -371,25 +377,24 @@
         factory: Optional[Callable] = None,
         tokens_factory: Optional[Callable] = None,
         format: Optional[str] = None,
         derived: bool = False,
         any_type: bool = False,
         required: bool = False,
         nillable: bool = False,
-        sequential: bool = False,
+        sequence: Optional[int] = None,
         list_element: bool = False,
-        default: Any = None,
+        default: Optional[Any] = None,
         xml_type: str = XmlType.ELEMENT,
         namespaces: Optional[Sequence[str]] = None,
         elements: Optional[Dict[str, XmlVar]] = None,
         wildcards: Optional[Sequence[XmlVar]] = None,
         prefix: str = "field_",
         **kwargs: Any,
     ) -> XmlVar:
-
         name = name or f"{prefix}{cls.next_letter()}"
 
         if qname is None:
             qname = name
 
         if types is None:
             types = ()
@@ -411,21 +416,22 @@
             factory=factory,
             tokens_factory=tokens_factory,
             format=format,
             derived=derived,
             any_type=any_type,
             required=required,
             nillable=nillable,
-            sequential=sequential,
+            sequence=sequence,
             list_element=list_element,
             default=default,
             xml_type=xml_type,
             namespaces=namespaces,
             elements=elements,
             wildcards=wildcards,
+            wrapper=None,
         )
 
 
 class XmlMetaFactory(Factory):
     counter = 65
 
     @classmethod
@@ -439,15 +445,14 @@
         choices: Optional[Sequence[XmlVar]] = None,
         elements: Optional[Dict[str, Sequence[XmlVar]]] = None,
         wildcards: Optional[Sequence[XmlVar]] = None,
         attributes: Optional[Dict[str, XmlVar]] = None,
         any_attributes: Optional[Sequence[XmlVar]] = None,
         **kwargs: Any,
     ) -> XmlMeta:
-
         if qname is None:
             qname = clazz.__name__
 
         if target_qname is None:
             target_qname = qname
 
         if choices is None:
@@ -472,14 +477,15 @@
             nillable=nillable,
             text=text,
             choices=choices,
             elements=elements,
             wildcards=wildcards,
             attributes=attributes,
             any_attributes=any_attributes,
+            wrappers={},
         )
 
 
 class DtdAttributeFactory(Factory):
     counter = 65
 
     @classmethod
@@ -489,15 +495,14 @@
         prefix: Optional[str] = None,
         type: Optional[DtdAttributeType] = None,
         default: Optional[DtdAttributeDefault] = None,
         default_value: Optional[str] = None,
         values: Optional[List[str]] = None,
         **kwargs: Any,
     ) -> DtdAttribute:
-
         if name is None:
             name = f"attribute_{cls.next_letter()}"
 
         if type is None:
             type = DtdAttributeType.CDATA
 
         if default is None:
@@ -557,15 +562,14 @@
         prefix: Optional[str] = None,
         type: Optional[DtdElementType] = None,
         content: Optional[DtdContent] = None,
         attributes: Optional[List[DtdAttribute]] = None,
         ns_map: Optional[Dict] = None,
         **kwargs: Any,
     ) -> DtdElement:
-
         if name is None:
             name = f"element_{cls.next_letter()}"
 
         if type is None:
             type = DtdElementType.ELEMENT
 
         if attributes is None:
```

### Comparing `xsdata-22.9/xsdata/utils/text.py` & `xsdata-23.5/xsdata/utils/text.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Any
 from typing import List
 from typing import Match
 from typing import Tuple
 
 stop_words = {
     "",
+    "Any",
     "Decimal",
     "Dict",
     "Enum",
     "False",
     "List",
     "Meta",
     "None",
@@ -172,15 +173,14 @@
     LOWER = 2
     NUMERIC = 3
     OTHER = 4
 
 
 def classify(character: str) -> int:
     """String classifier."""
-
     code_point = ord(character)
     if 64 < code_point < 91:
         return StringType.UPPER
 
     if 96 < code_point < 123:
         return StringType.LOWER
```

### Comparing `xsdata-22.9/xsdata.egg-info/PKG-INFO` & `xsdata-23.5/README.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,7 @@
-Metadata-Version: 2.1
-Name: xsdata
-Version: 22.9
-Summary: Python XML Binding
-Home-page: https://github.com/tefra/xsdata
-Author: Christodoulos Tsoulloftas
-Author-email: "chris@komposta.net",
-License: MIT
-Project-URL: Source, https://github.com/tefra/xsdata
-Project-URL: Documentation, https://xsdata.readthedocs.io/
-Project-URL: Changelog, https://xsdata.readthedocs.io/en/latest/changelog.html
-Keywords: xsd,wsdl,schema,dtd,binding,xml,json,dataclasses,generator,cli
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Topic :: Software Development :: Code Generators
-Classifier: Topic :: Text Processing :: Markup :: XML
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: cli
-Provides-Extra: docs
-Provides-Extra: lxml
-Provides-Extra: soap
-Provides-Extra: test
-License-File: LICENSE
-
 .. image:: https://github.com/tefra/xsdata/raw/master/docs/_static/logo.svg
     :target: https://xsdata.readthedocs.io/
 
 Naive XML Bindings for python
 =============================
 
 .. image:: https://github.com/tefra/xsdata/workflows/tests/badge.svg
@@ -131,15 +95,43 @@
   - Handlers and Writers based on lxml and native xml python
   - Support wildcard elements and attributes
   - Support xinclude statements and unknown properties
   - Customize behaviour through config
 
 
 
-Changelog: 22.9 (2022-08-24)
+Changelog: 23.5 (2023-05-21)
 ----------------------------
-- Fixed code generation inconsistencies in different operating systems.
-- Fixed circular imports error `#706 <https://github.com/tefra/xsdata/pull/706>`_
-- Fixed naming conflicts in imports `#706 <https://github.com/tefra/xsdata/pull/706>`_
-- Fixed issue with wrong occurrences in DTD code generation  `#705 <https://github.com/tefra/xsdata/pull/705>`_
-- Fixed xs:group and xs:attrGroup name conflicts `#702 <https://github.com/tefra/xsdata/pull/702>`_
-- Added mathml3 in standard schemas
+- Fixed XML meta var index conflicts.
+- Fixed mixed content handling for DTD elements. (`#749 <https://github.com/tefra/xsdata/pull/749>`_, `#762 <https://github.com/tefra/xsdata/pull/762>`_)
+- Fixed an issue with required attributes turning into optional ones.
+- Fixed calculation of min/max occurs when parsing XML/JSON documents. (`#756 <https://github.com/tefra/xsdata/pull/756>`_)
+- Fixed calculation of min/max occurs when parsing DTD choice content types. (`#760 <https://github.com/tefra/xsdata/pull/760>`_)
+- Fixed an issue when parsing tail content for compound wildcard elements.
+- Fixed an issue with the code analyzer not fully processing some classes.
+- Fixed an issue with the code analyzer taking forever to process very large enumerations. (`#776 <https://github.com/tefra/xsdata/issue/776>`_)
+- Fixed an issue in the JSON parser with optional choice elements.
+- Updated the transformer to silently ignore malformed JSON files. (`#750 <https://github.com/tefra/xsdata/pull/750>`_)
+- Updated the override attribute handler to fix naming conflicts.
+- Updated the override attribute handler to allow wildcard overrides.
+- Updated conditions on extensions flattening (over-flattening). (`#754 <https://github.com/tefra/xsdata/pull/754>`_)
+- Updated Group, AttributeGroup handling, skipping a few cases.
+- Updated how min/max occurs are calculated with nested containers.
+- Updated handling of element substitutions to treat them as choices. (`#786 <https://github.com/tefra/xsdata/pull/786>`_)
+- Updated Pycodeserializer to skip default field values.
+- Updated flattening restriction base classes when sequence elements are out of order.
+- Updated docformatter to v1.6.5.
+- Added support to override compound fields.
+- Added support for multiple sequential groups in a class.
+- Added support for non-list compound fields.
+- Added support to mix list and non-list fields with sequence groups.
+- Added an option to include headers in generated files. (`#746 <https://github.com/tefra/xsdata/pull/746>`_)
+- Added an option to cache the initial load and mapping of resources.
+- Added support for regular expressions in config substitutions. (`#755 <https://github.com/tefra/xsdata/pull/755>`_)
+- Added a pretty print indentation option in the serializer config. (`#780 <https://github.com/tefra/xsdata/pull/780>`_)
+- Added an option to set the encoding in the SOAP Client. (`#773 <https://github.com/tefra/xsdata/pull/773>`_)
+- Added a CLI flag to show debug messages.
+- Added a debug message for possible circular references during code generation.
+- Added support to generate prohibited fields when they restrict parent fields. (`#781 <https://github.com/tefra/xsdata/pull/781>`_)
+
+This release is bigger than intended and includes many major changes,
+that's why it took so long.
```

### Comparing `xsdata-22.9/xsdata.egg-info/SOURCES.txt` & `xsdata-23.5/xsdata.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -38,24 +38,27 @@
 docs/api/xml-datatypes.rst
 docs/api/xml-handlers.rst
 docs/api/xml-nodes.rst
 docs/api/xml-writers.rst
 docs/examples/compound-fields.rst
 docs/examples/custom-class-factory.rst
 docs/examples/custom-property-names.rst
+docs/examples/custom-type-mapping.rst
 docs/examples/dataclasses-features.rst
 docs/examples/docstrings.rst
 docs/examples/dtd-modeling.rst
 docs/examples/json-modeling.rst
 docs/examples/pycode-serializer.rst
 docs/examples/samples.rst
 docs/examples/w3c-suite.rst
 docs/examples/working-with-wildcards.rst
+docs/examples/wrapped-list.rst
 docs/examples/xml-modeling.rst
 docs/faq/error-parsing-dtd.rst
+docs/faq/how-can-i-compare-output-results-between-versions.rst
 docs/faq/why-are-elements-out-of-order.rst
 docs/faq/why-i-get-a-typeerror-requires-a-single-type.rst
 docs/faq/why-non-nullable-fields-are-marked-as-optional.rst
 docs/scripts/__init__.py
 docs/scripts/generate_data_types.py
 tests/__init__.py
 tests/conftest.py
@@ -66,24 +69,27 @@
 tests/codegen/test_resolver.py
 tests/codegen/test_transformer.py
 tests/codegen/test_utils.py
 tests/codegen/test_validator.py
 tests/codegen/test_writer.py
 tests/codegen/handlers/__init__.py
 tests/codegen/handlers/test_add_attribute_substitutions.py
+tests/codegen/handlers/test_calculate_attribute_paths.py
 tests/codegen/handlers/test_create_compound_fields.py
 tests/codegen/handlers/test_designate_class_packages.py
 tests/codegen/handlers/test_filter_classes.py
 tests/codegen/handlers/test_flatten_attribute_groups.py
 tests/codegen/handlers/test_flatten_class_extensions.py
 tests/codegen/handlers/test_merge_attributes.py
 tests/codegen/handlers/test_process_attributes_types.py
 tests/codegen/handlers/test_process_mixed_content_class.py
 tests/codegen/handlers/test_rename_duplicate_attributes.py
 tests/codegen/handlers/test_rename_duplicate_classes.py
+tests/codegen/handlers/test_reset_attribute_sequence_numbers.py
+tests/codegen/handlers/test_reset_attribute_sequences.py
 tests/codegen/handlers/test_sanitize_attributes_default_value.py
 tests/codegen/handlers/test_sanitize_enumeration_class.py
 tests/codegen/handlers/test_unnest_inner_classes.py
 tests/codegen/handlers/test_update_attributes_effective_choice.py
 tests/codegen/handlers/test_vacuum_inner_classes.py
 tests/codegen/handlers/test_validate_attributes_overrides.py
 tests/codegen/mappers/__init__.py
@@ -206,14 +212,15 @@
 tests/formats/dataclass/parsers/nodes/__init__.py
 tests/formats/dataclass/parsers/nodes/test_element.py
 tests/formats/dataclass/parsers/nodes/test_primitive.py
 tests/formats/dataclass/parsers/nodes/test_skip.py
 tests/formats/dataclass/parsers/nodes/test_standard.py
 tests/formats/dataclass/parsers/nodes/test_union.py
 tests/formats/dataclass/parsers/nodes/test_wildcard.py
+tests/formats/dataclass/parsers/nodes/test_wrapper.py
 tests/formats/dataclass/serializers/__init__.py
 tests/formats/dataclass/serializers/test_code.py
 tests/formats/dataclass/serializers/test_json.py
 tests/formats/dataclass/serializers/test_mixins.py
 tests/formats/dataclass/serializers/test_xml.py
 tests/formats/dataclass/serializers/writers/__init__.py
 tests/formats/dataclass/serializers/writers/test_lxml.py
@@ -230,20 +237,26 @@
 tests/integration/test_primer.py
 tests/integration/test_series.py
 tests/integration/test_stripe.py
 tests/integration/benchmarks/__init__.py
 tests/integration/benchmarks/conftest.py
 tests/integration/benchmarks/test_converters.py
 tests/integration/benchmarks/test_handlers.py
+tests/integration/benchmarks/utils.py
 tests/models/__init__.py
 tests/models/test_config.py
 tests/models/test_datatype.py
 tests/models/test_mixins.py
+tests/models/test_type_mapping.py
 tests/models/enums/__init__.py
 tests/models/enums/test_datatype.py
+tests/models/typemapping/__init__.py
+tests/models/typemapping/city.py
+tests/models/typemapping/house.py
+tests/models/typemapping/street.py
 tests/models/wsdl/__init__.py
 tests/models/wsdl/test_binding.py
 tests/models/wsdl/test_definitions.py
 tests/models/wsdl/test_port_type.py
 tests/models/xsd/__init__.py
 tests/models/xsd/test_all.py
 tests/models/xsd/test_alternative.py
@@ -258,14 +271,15 @@
 tests/models/xsd/test_element.py
 tests/models/xsd/test_enumeration.py
 tests/models/xsd/test_extension.py
 tests/models/xsd/test_group.py
 tests/models/xsd/test_list.py
 tests/models/xsd/test_restriction.py
 tests/models/xsd/test_schema.py
+tests/models/xsd/test_sequence.py
 tests/models/xsd/test_simple_type.py
 tests/models/xsd/test_union.py
 tests/utils/__init__.py
 tests/utils/test_collections.py
 tests/utils/test_dates.py
 tests/utils/test_downloader.py
 tests/utils/test_hooks.py
@@ -293,24 +307,27 @@
 xsdata/codegen/resolver.py
 xsdata/codegen/transformer.py
 xsdata/codegen/utils.py
 xsdata/codegen/validator.py
 xsdata/codegen/writer.py
 xsdata/codegen/handlers/__init__.py
 xsdata/codegen/handlers/add_attribute_substitutions.py
+xsdata/codegen/handlers/calculate_attribute_paths.py
 xsdata/codegen/handlers/create_compound_fields.py
 xsdata/codegen/handlers/designate_class_packages.py
 xsdata/codegen/handlers/filter_classes.py
 xsdata/codegen/handlers/flatten_attribute_groups.py
 xsdata/codegen/handlers/flatten_class_extensions.py
 xsdata/codegen/handlers/merge_attributes.py
 xsdata/codegen/handlers/process_attributes_types.py
 xsdata/codegen/handlers/process_mixed_content_class.py
 xsdata/codegen/handlers/rename_duplicate_attributes.py
 xsdata/codegen/handlers/rename_duplicate_classes.py
+xsdata/codegen/handlers/reset_attribute_sequence_numbers.py
+xsdata/codegen/handlers/reset_attribute_sequences.py
 xsdata/codegen/handlers/sanitize_attributes_default_value.py
 xsdata/codegen/handlers/sanitize_enumeration_class.py
 xsdata/codegen/handlers/unnest_inner_classes.py
 xsdata/codegen/handlers/update_attributes_effective_choice.py
 xsdata/codegen/handlers/vacuum_inner_classes.py
 xsdata/codegen/handlers/validate_attributes_overrides.py
 xsdata/codegen/mappers/__init__.py
@@ -353,14 +370,15 @@
 xsdata/formats/dataclass/parsers/nodes/__init__.py
 xsdata/formats/dataclass/parsers/nodes/element.py
 xsdata/formats/dataclass/parsers/nodes/primitive.py
 xsdata/formats/dataclass/parsers/nodes/skip.py
 xsdata/formats/dataclass/parsers/nodes/standard.py
 xsdata/formats/dataclass/parsers/nodes/union.py
 xsdata/formats/dataclass/parsers/nodes/wildcard.py
+xsdata/formats/dataclass/parsers/nodes/wrapper.py
 xsdata/formats/dataclass/serializers/__init__.py
 xsdata/formats/dataclass/serializers/code.py
 xsdata/formats/dataclass/serializers/config.py
 xsdata/formats/dataclass/serializers/json.py
 xsdata/formats/dataclass/serializers/mixins.py
 xsdata/formats/dataclass/serializers/xml.py
 xsdata/formats/dataclass/serializers/writers/__init__.py
```

