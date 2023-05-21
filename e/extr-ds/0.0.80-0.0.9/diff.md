# Comparing `tmp/extr-ds-0.0.80.tar.gz` & `tmp/extr-ds-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extr-ds-0.0.80.tar", last modified: Sun May 21 09:55:33 2023, max compression
+gzip compressed data, was "extr-ds-0.0.9.tar", last modified: Fri Apr 21 13:19:22 2023, max compression
```

## Comparing `extr-ds-0.0.80.tar` & `extr-ds-0.0.9.tar`

### file list

```diff
@@ -1,50 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 09:55:33.344877 extr-ds-0.0.80/
--rw-rw-rw-   0        0        0     5664 2023-05-21 09:55:33.342607 extr-ds-0.0.80/PKG-INFO
--rw-rw-rw-   0        0        0     3980 2023-05-19 21:13:57.000000 extr-ds-0.0.80/README.md
--rw-rw-rw-   0        0        0       42 2023-05-21 09:55:33.345875 extr-ds-0.0.80/setup.cfg
--rw-rw-rw-   0        0        0      704 2023-05-21 09:54:42.000000 extr-ds-0.0.80/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-21 09:55:32.950847 extr-ds-0.0.80/src/
-drwxrwxrwx   0        0        0        0 2023-05-21 09:55:33.012374 extr-ds-0.0.80/src/extr_ds/
--rw-rw-rw-   0        0        0       27 2023-04-15 12:51:37.000000 extr-ds-0.0.80/src/extr_ds/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-21 09:55:33.172888 extr-ds-0.0.80/src/extr_ds/labelers/
--rw-rw-rw-   0        0        0       68 2023-04-16 10:14:54.000000 extr-ds-0.0.80/src/extr_ds/labelers/__init__.py
--rw-rw-rw-   0        0        0     1797 2023-05-19 15:06:33.000000 extr-ds-0.0.80/src/extr_ds/labelers/iob.py
--rw-rw-rw-   0        0        0     5922 2023-05-20 10:11:46.000000 extr-ds-0.0.80/src/extr_ds/labelers/relation.py
-drwxrwxrwx   0        0        0        0 2023-05-21 09:55:33.193125 extr-ds-0.0.80/src/extr_ds/manager/
--rw-rw-rw-   0        0        0       54 2023-04-30 12:32:24.000000 extr-ds-0.0.80/src/extr_ds/manager/__init__.py
--rw-rw-rw-   0        0        0     2927 2023-05-11 09:38:01.000000 extr-ds-0.0.80/src/extr_ds/manager/cmd.py
-drwxrwxrwx   0        0        0        0 2023-05-21 09:55:33.220072 extr-ds-0.0.80/src/extr_ds/manager/process/
--rw-rw-rw-   0        0        0      206 2023-05-11 09:37:51.000000 extr-ds-0.0.80/src/extr_ds/manager/process/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-21 09:55:33.240748 extr-ds-0.0.80/src/extr_ds/manager/process/entities/
--rw-rw-rw-   0        0        0       32 2023-05-11 09:09:26.000000 extr-ds-0.0.80/src/extr_ds/manager/process/entities/__init__.py
--rw-rw-rw-   0        0        0     2174 2023-05-19 19:35:35.000000 extr-ds-0.0.80/src/extr_ds/manager/process/entities/annotate.py
--rw-rw-rw-   0        0        0     1651 2023-05-18 15:49:38.000000 extr-ds-0.0.80/src/extr_ds/manager/process/entities/dev.py
--rw-rw-rw-   0        0        0      303 2023-05-11 09:05:39.000000 extr-ds-0.0.80/src/extr_ds/manager/process/entities/models.py
--rw-rw-rw-   0        0        0     1467 2023-05-11 10:06:35.000000 extr-ds-0.0.80/src/extr_ds/manager/process/how_to.py
-drwxrwxrwx   0        0        0        0 2023-05-21 09:55:33.260636 extr-ds-0.0.80/src/extr_ds/manager/process/relations/
--rw-rw-rw-   0        0        0       84 2023-05-11 08:53:28.000000 extr-ds-0.0.80/src/extr_ds/manager/process/relations/__init__.py
--rw-rw-rw-   0        0        0     2982 2023-05-18 19:37:35.000000 extr-ds-0.0.80/src/extr_ds/manager/process/relations/dev.py
--rw-rw-rw-   0        0        0     2008 2023-05-19 21:14:27.000000 extr-ds-0.0.80/src/extr_ds/manager/process/relations/relate.py
--rw-rw-rw-   0        0        0     5095 2023-05-19 14:42:46.000000 extr-ds-0.0.80/src/extr_ds/manager/process/save.py
--rw-rw-rw-   0        0        0      844 2023-05-05 10:11:23.000000 extr-ds-0.0.80/src/extr_ds/manager/process/split.py
--rw-rw-rw-   0        0        0     3096 2023-05-19 14:42:06.000000 extr-ds-0.0.80/src/extr_ds/manager/process/workspace.py
-drwxrwxrwx   0        0        0        0 2023-05-21 09:55:33.278578 extr-ds-0.0.80/src/extr_ds/manager/utils/
--rw-rw-rw-   0        0        0       91 2023-04-30 12:25:13.000000 extr-ds-0.0.80/src/extr_ds/manager/utils/__init__.py
--rw-rw-rw-   0        0        0     1476 2023-05-18 15:48:48.000000 extr-ds-0.0.80/src/extr_ds/manager/utils/filesystem.py
--rw-rw-rw-   0        0        0      494 2023-04-30 09:44:47.000000 extr-ds-0.0.80/src/extr_ds/manager/utils/imports.py
-drwxrwxrwx   0        0        0        0 2023-05-21 09:55:33.291847 extr-ds-0.0.80/src/extr_ds/models/
--rw-rw-rw-   0        0        0       42 2023-04-28 10:44:38.000000 extr-ds-0.0.80/src/extr_ds/models/__init__.py
--rw-rw-rw-   0        0        0     1411 2023-05-17 10:11:47.000000 extr-ds-0.0.80/src/extr_ds/models/labels.py
-drwxrwxrwx   0        0        0        0 2023-05-21 09:55:33.313412 extr-ds-0.0.80/src/extr_ds/transformers/
--rw-rw-rw-   0        0        0       42 2023-05-05 10:03:32.000000 extr-ds-0.0.80/src/extr_ds/transformers/__init__.py
--rw-rw-rw-   0        0        0     2273 2023-05-19 13:19:31.000000 extr-ds-0.0.80/src/extr_ds/transformers/iob.py
-drwxrwxrwx   0        0        0        0 2023-05-21 09:55:33.330410 extr-ds-0.0.80/src/extr_ds/validators/
--rw-rw-rw-   0        0        0      174 2023-04-28 10:45:23.000000 extr-ds-0.0.80/src/extr_ds/validators/__init__.py
--rw-rw-rw-   0        0        0     1718 2023-04-28 10:43:16.000000 extr-ds-0.0.80/src/extr_ds/validators/differences.py
-drwxrwxrwx   0        0        0        0 2023-05-21 09:55:33.155457 extr-ds-0.0.80/src/extr_ds.egg-info/
--rw-rw-rw-   0        0        0     5664 2023-05-21 09:55:32.000000 extr-ds-0.0.80/src/extr_ds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1248 2023-05-21 09:55:32.000000 extr-ds-0.0.80/src/extr_ds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 09:55:32.000000 extr-ds-0.0.80/src/extr_ds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-05-21 09:55:32.000000 extr-ds-0.0.80/src/extr_ds.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2023-05-21 09:55:32.000000 extr-ds-0.0.80/src/extr_ds.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-21 09:55:32.000000 extr-ds-0.0.80/src/extr_ds.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 13:19:21.991749 extr-ds-0.0.9/
+-rw-rw-rw-   0        0        0     4036 2023-04-21 13:19:21.989423 extr-ds-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2857 2023-04-18 14:03:40.000000 extr-ds-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-21 13:19:21.992749 extr-ds-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      608 2023-04-21 13:18:21.000000 extr-ds-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 13:19:21.498829 extr-ds-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-04-21 13:19:21.609030 extr-ds-0.0.9/src/extr_ds/
+-rw-rw-rw-   0        0        0       27 2023-04-15 12:51:37.000000 extr-ds-0.0.9/src/extr_ds/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 13:19:21.986294 extr-ds-0.0.9/src/extr_ds/labelers/
+-rw-rw-rw-   0        0        0       68 2023-04-16 10:14:54.000000 extr-ds-0.0.9/src/extr_ds/labelers/__init__.py
+-rw-rw-rw-   0        0        0     1634 2023-04-18 10:03:06.000000 extr-ds-0.0.9/src/extr_ds/labelers/iob.py
+-rw-rw-rw-   0        0        0     3608 2023-04-18 12:35:59.000000 extr-ds-0.0.9/src/extr_ds/labelers/relation.py
+-rw-rw-rw-   0        0        0      461 2023-04-18 09:59:18.000000 extr-ds-0.0.9/src/extr_ds/models.py
+-rw-rw-rw-   0        0        0     1718 2023-04-17 21:01:45.000000 extr-ds-0.0.9/src/extr_ds/validators.py
+drwxrwxrwx   0        0        0        0 2023-04-21 13:19:21.971248 extr-ds-0.0.9/src/extr_ds.egg-info/
+-rw-rw-rw-   0        0        0     4036 2023-04-21 13:19:21.000000 extr-ds-0.0.9/src/extr_ds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      358 2023-04-21 13:19:21.000000 extr-ds-0.0.9/src/extr_ds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 13:19:21.000000 extr-ds-0.0.9/src/extr_ds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-21 13:19:21.000000 extr-ds-0.0.9/src/extr_ds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-21 13:19:21.000000 extr-ds-0.0.9/src/extr_ds.egg-info/top_level.txt
```

### Comparing `extr-ds-0.0.80/README.md` & `extr-ds-0.0.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,169 +1,115 @@
-# extr-ds
-> Library to programmatically build labeled datasets for Named-Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks.
-
-<br />
-
-## Install
-
-```
-pip install extr-ds
-```
-
-## Command Line
-
-see [Instructions](https://medium.com/@pasdan/building-custom-named-entity-recognition-models-e4d8d95804e) on how to use the command line utility to manage your project.
-
-### 1. Init Project
-```
-extr-ds --init
-```
-
-### 2. Split and Annotate
-```
-extr-ds --split
-```
-
-### 3.a Annotate Entities or Relations Again?
-```
-extr-ds --annotate -ents
-extr-ds --annotate -rels
-```
-
-### 3.b Change Relation Extraction Label
-```
-extr-ds --relate -label NO_RELATION=5,7,9
-```
-
-### 3.b Remove Relation Extraction Instance
-```
-extr-ds --relate -delete 5,6,7
-```
-
-### 3.c Recover removed Relation Extraction Instances
-```
-extr-ds --relate -recover 5,6,7
-```
-
-### 4. Save
-```
-extr-ds --save -ents
-extr-ds --save -rels
-```
-
-### 5. Reset "Gold Standard" datasets
-```
-extr-ds --reset
-```
-
-### 6. Help!?
-```
-extr-ds --help
-```
-
-## API
-
-## Example
-
-```python
-text = 'Ted Johnson is a pitcher.'
-```
-
-### 1. Label Entities for Named-Entity Recognition Task (NER)
-
-```python
-from extr import RegEx, RegExLabel
-from extr.entities import EntityExtactor
-from extr_ds.labelers import IOB
-
-entity_extractor = EntityExtactor([
-    RegExLabel('PERSON', [
-        RegEx([r'(ted\s+johnson|ted)'], re.IGNORECASE)
-    ]),
-    RegExLabel('POSITION', [
-        RegEx([r'pitcher'], re.IGNORECASE)
-    ]),
-])
-
-sentence_tokenizer = ## 3rd party tokenizer ##
-label = IOB(sentence_tokenizer, entity_extractor).label(text)
-
-## label == <Label tokens=..., labels=['B-PERSON', 'I-PERSON', 'O', 'O', 'B-POSITION', 'O']>
-```
-
-### 2. Annotate for Relation Extraction Task (RE)
-
-```python
-from extr.entities import EntityExtractor
-from extr.relations import RegExRelationLabelBuilder, \
-                           RelationExtractor
-from extr_ds.labelers import RelationClassification
-from extr_ds.labelers.relation import RelationBuilder, BaseRelationLabeler, RuleBasedRelationLabeler
-
-
-person_to_position_relationship = RegExRelationLabelBuilder('is_a') \
-    .add_e1_to_e2(
-        'PERSON',
-        [
-            r'\s+is\s+a\s+',
-        ],
-        'POSITION'
-    ) \
-    .build()
-
-base_relation_labeler = BaseRelationLabeler(
-    RelationBuilder(relation_formats=[
-        ('PERSON', 'POSITION', 'NO_RELATION')
-    ])
-)
-
-rule_based_relation_labeler = RuleBasedRelationLabeler(
-    RelationExtractor([person_to_position_relationship])
-)
-
-labeler = RelationClassification(
-    EntityExtractor([
-        RegExLabel('PERSON', [
-            RegEx([r'(ted johnson|bob)'], re.IGNORECASE)
-        ]),
-        RegExLabel('POSITION', [
-            RegEx([r'pitcher'], re.IGNORECASE)
-        ]),
-    ]),
-    base_relation_labeler,
-    relation_labelers=[
-        rule_based_relation_labeler
-    ]
-)
-
-results = labeler.label(text)
-
-## results.relation_labels == [
-##    <RelationLabel sentence="<e1>Ted Johnson</e1> is a <e2>pitcher</e2>." label="is_a">
-## ]
-```
-
-### 3. Find and define the type of difference between labels
-
-```python
-from extr_ds.validators import check_for_differences
-
-differences_in_labels = check_for_differences(
-    ['B-PERSON', 'I-PERSON', 'O', 'O', 'B-POSITION', 'O'],
-    ['B-PERSON', 'O', 'O', 'O', 'B-POSITION', 'O']
-)
-
-## differences_in_labels.has_diffs == True
-## differences_in_labels.diffs_between_labels == [
-##      <Difference index=1, diff_type=DifferenceTypes.S2_MISSING>
-## ]
-
-differences_in_labels = check_for_differences(
-    ['B-PERSON', 'I-PERSON', 'O', 'O', 'B-POSITION', 'O'],
-    ['B-PERSON', 'B-PERSON', 'O', 'O', 'B-POSITION', 'O']
-)
-
-## differences_in_labels.has_diffs == True
-## differences_in_labels.diffs_between_labels == [
-##      <Difference index=1, diff_type=DifferenceTypes.MISMATCH>
-## ]
-```
+Metadata-Version: 2.1
+Name: extr-ds
+Version: 0.0.9
+Summary: Library to quickly build basic datasets for Named Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks.
+Home-page: https://github.com/dpasse/extr-ds
+License: UNKNOWN
+Description: # extr-ds
+        > Library to programmatically build labeled datasets for Named-Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks.
+        
+        <br />
+        
+        ## Install
+        
+        ```
+        pip install extr-ds
+        ```
+        
+        ## Example
+        
+        ```python
+        text = 'Ted Johnson is a pitcher. Ted went to my school.'
+        ```
+        
+        ### 1. Label Entities for Named-Entity Recognition Task (NER)
+        
+        ```python
+        from extr import RegEx, RegExLabel
+        from extr.entities import EntityExtactor
+        from extr_ds.labelers import IOB
+        
+        entity_extractor = EntityExtactor([
+            RegExLabel('PERSON', [
+                RegEx([r'(ted\s+johnson|ted)'], re.IGNORECASE)
+            ]),
+            RegExLabel('POSITION', [
+                RegEx([r'pitcher'], re.IGNORECASE)
+            ]),
+        ])
+        
+        sentence_tokenizer = ## 3rd party tokenizer ##
+        labels = IOB(sentence_tokenizer, entity_extractor).label(text)
+        
+        ## labels ==  [
+        ##     <Label tokens=..., labels=['B-PERSON', 'I-PERSON', 'O', 'O', 'B-POSITION', 'O']>,
+        ##     <Label tokens=..., labels=['B-PERSON', 'O', 'O', 'O', 'O', 'O']>
+        ## ]
+        ```
+        
+        ### 2. Annotate for Relation Extraction Task (RE)
+        
+        ```python
+        from extr.entities import EntityExtractor
+        from extr.relations import RegExRelationLabelBuilder, \
+                                   RelationExtractor
+        from extr_ds.labelers import RelationClassification
+        
+        person_to_position_relationship = RegExRelationLabelBuilder('is_a') \
+            .add_e1_to_e2(
+                'PERSON',
+                [
+                    r'\s+is\s+a\s+',
+                ],
+                'POSITION'
+            ) \
+            .build()
+        
+        labeler = RelationClassification(
+            sentence_tokenizer,
+            EntityExtractor([
+                RegExLabel('PERSON', [
+                    RegEx([r'(ted johnson|bob)'], re.IGNORECASE)
+                ]),
+                RegExLabel('POSITION', [
+                    RegEx([r'pitcher'], re.IGNORECASE)
+                ]),
+            ]),
+            RelationExtractor([person_to_position_relationship]),
+            [('PERSON', 'POSITION', 'NO_RELATION')],
+        )
+        
+        labels = labeler.label(text)
+        
+        ## labels == [
+        ##    <RelationLabel sentence="<e1>Ted Johnson</e1> is a <e2>pitcher</e2>." label="is_a">
+        ## ]
+        ```
+        
+        ### 3. Find and define the type of difference between labels
+        
+        ```python
+        from extr_ds.validators import check_for_differences
+        
+        differences_in_labels = check_for_differences(
+            ['B-PERSON', 'I-PERSON', 'O', 'O', 'B-POSITION', 'O'],
+            ['B-PERSON', 'O', 'O', 'O', 'B-POSITION', 'O']
+        )
+        
+        ## differences_in_labels.has_diffs == True
+        ## differences_in_labels.diffs_between_labels == [
+        ##      <Difference index=1, diff_type=DifferenceTypes.S2_MISSING>
+        ## ]
+        
+        differences_in_labels = check_for_differences(
+            ['B-PERSON', 'I-PERSON', 'O', 'O', 'B-POSITION', 'O'],
+            ['B-PERSON', 'B-PERSON', 'O', 'O', 'B-POSITION', 'O']
+        )
+        
+        ## differences_in_labels.has_diffs == True
+        ## differences_in_labels.diffs_between_labels == [
+        ##      <Difference index=1, diff_type=DifferenceTypes.MISMATCH>
+        ## ]
+        ```
+        
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
```

### Comparing `extr-ds-0.0.80/setup.py` & `extr-ds-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,22 +2,19 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='extr-ds',
-    version='0.0.80',
+    version='0.0.9',
     keywords='',
     description='Library to quickly build basic datasets for Named Entity Recognition (NER) and Relation Extraction (RE) Machine Learning tasks.',
     packages=setuptools.find_packages('src'),
     package_dir={'': 'src'},
     install_requires=[
-        'extr==0.0.41'
+        'extr==0.0.13'
     ],
     url='https://github.com/dpasse/extr-ds',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    entry_points = {
-        'console_scripts': ['extr-ds=extr_ds.manager.cmd:main'],
-    }
 )
```

### Comparing `extr-ds-0.0.80/src/extr_ds/labelers/iob.py` & `extr-ds-0.0.9/src/extr_ds/labelers/iob.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,39 @@
-from typing import List, Callable, Iterator, cast
+from typing import List, Callable, Generator, Iterator, cast
 from extr import Entity, TokenGroup
 from extr.entities import EntityExtractor
-from extr.tokenizers import word_tokenizer
+from extr.tokenizers import tokenizer
 from ..models import Label
 
 
-class Labeler():
-    def __init__(self, tokenizer: Callable[[str], List[str]]) -> None:
-        self._tokenizer = tokenizer
+class IOB():
+    def __init__(self, sentence_tokenizer: Callable[[str], List[List[str]]], entity_extractor: EntityExtractor) -> None:
+        self._sentence_tokenizer = sentence_tokenizer
+        self._entity_extractor = entity_extractor
 
-    def label(self, text: str, entities: List[Entity]) -> Label:
-        return self.__merge(
-            word_tokenizer(text, self._tokenizer(text)),
-            entities
-        )
+    def label(self, text: str) -> Generator[Label, None, None]:
+        entities = self._entity_extractor.get_entities(text)
+        token_groups = tokenizer(text, self._sentence_tokenizer(text))
 
-    def __merge(self, token_group: TokenGroup, entities: List[Entity]) -> Label:
-        tokens = list(enumerate(token_group.tokens))
-        labels = ['O' for _ in range(len(tokens))]
-        for entity in cast(Iterator[Entity], filter(token_group.contains, entities)):
-            used_counter = 0
+        return self.__merge(token_groups, entities)
 
-            for i, token in tokens:
-                if not entity.is_in(token) and not entity.contains(token):
-                    continue
+    def __merge(self, token_groups: Generator[TokenGroup, None, None], entities: List[Entity]) -> Generator[Label, None, None]:
+        for token_group in token_groups:
+            tokens = list(enumerate(token_group.tokens))
+            labels = ['O' for _ in range(len(tokens))]
+            for entity in cast(Iterator[Entity], filter(token_group.contains, entities)):
+                used_counter = 0
 
-                current_label = labels[i]
-                assert current_label == 'O', f'bad tokenizer? multiple entities belong to the same token - {current_label}'
+                for i, token in tokens:
+                    if not entity.is_in(token):
+                        continue
 
-                labels[i] = 'B-' if used_counter == 0 else 'I-'
-                labels[i] += entity.label
+                    assert labels[i] == 'O', f'bad tokenizer? multiple entities belong to the same token - {labels[i]}'
 
-                token.add_entity(entity)
+                    labels[i] = 'B-' if used_counter == 0 else 'I-'
+                    labels[i] += entity.label
 
-                used_counter += 1
+                    token.add_entity(entity)
 
-        return Label(token_group, labels)
+                    used_counter += 1
 
-class IOB():
-    def __init__(self, \
-                 tokenizer: Callable[[str], List[str]], \
-                 entity_extractor: EntityExtractor) -> None:
-        self._labeler = Labeler(tokenizer)
-        self._entity_extractor = entity_extractor
-
-    def label(self, text: str) -> Label:
-        entities = self._entity_extractor.get_entities(text)
-        return self._labeler.label(text, entities)
+            yield Label(token_group.tokens, labels)
```

### Comparing `extr-ds-0.0.80/src/extr_ds/validators/differences.py` & `extr-ds-0.0.9/src/extr_ds/validators.py`

 * *Files identical despite different names*

