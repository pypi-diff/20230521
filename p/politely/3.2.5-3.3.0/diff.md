# Comparing `tmp/politely-3.2.5.tar.gz` & `tmp/politely-3.3.0.tar.gz`

## Comparing `politely-3.2.5.tar` & `politely-3.3.0.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 politely-3.2.5/politely/__init__.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 politely-3.2.5/politely/errors.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 politely-3.2.5/politely/fetchers.py
--rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 politely-3.2.5/politely/rules.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 politely-3.2.5/politely/scorer.py
--rw-r--r--   0        0        0     6283 2020-02-02 00:00:00.000000 politely-3.2.5/politely/styler.py
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 politely-3.2.5/.gitignore
--rw-r--r--   0        0        0    10996 2020-02-02 00:00:00.000000 politely-3.2.5/README.md
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 politely-3.2.5/pyproject.toml
--rw-r--r--   0        0        0    11929 2020-02-02 00:00:00.000000 politely-3.2.5/PKG-INFO
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 politely-3.3.0/politely/__init__.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 politely-3.3.0/politely/errors.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 politely-3.3.0/politely/fetchers.py
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 politely-3.3.0/politely/modeling_gpt2_scorer.py
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 politely-3.3.0/politely/modeling_heuristic_scorer.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 politely-3.3.0/politely/modeling_scorer.py
+-rw-r--r--   0        0        0     5120 2020-02-02 00:00:00.000000 politely-3.3.0/politely/rules.py
+-rw-r--r--   0        0        0     6232 2020-02-02 00:00:00.000000 politely-3.3.0/politely/styler.py
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 politely-3.3.0/.gitignore
+-rw-r--r--   0        0        0    10104 2020-02-02 00:00:00.000000 politely-3.3.0/README.md
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 politely-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0    11037 2020-02-02 00:00:00.000000 politely-3.3.0/PKG-INFO
```

### Comparing `politely-3.2.5/politely/errors.py` & `politely-3.3.0/politely/errors.py`

 * *Files identical despite different names*

### Comparing `politely-3.2.5/politely/rules.py` & `politely-3.3.0/politely/rules.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,24 @@
+"""
+규칙:
+1.
+"""
 from typing import Set, Tuple, Dict
 
 # --- symbols --- #
 NULL = "❌"
 TAG = "🏷"
 SEP = "🔗"
 
 
-# --- all EF's of different styles --- #
+# --- all EF's of different styles they must be singular tokens --- #
 CASUAL = {
     f"어{TAG}EF",
     f"다{TAG}EF",
+    f"니{TAG}EF",
     f"라{TAG}EF",
     f"어라{TAG}EF",
     f"자{TAG}EF",
     f"대{TAG}EF",
     f"는다{TAG}EF",
     f"마{TAG}EF",
     f"야{TAG}EF",
@@ -25,45 +30,47 @@
     f"ᆯ게{TAG}EF",
     f"ᆫ대{TAG}EF",
     f"ᆫ가{TAG}EF",
     f"지{TAG}EF"
 }
 
 POLITE = {
+    f"요{TAG}EF",
     f"어요{TAG}EF",
-    f"시{TAG}EP{SEP}어요{TAG}EF",
     f"에요{TAG}EF",
+    f"ᆫ가요{TAG}EF",
     f"지요{TAG}EF",
     f"래요{TAG}EF",
     f"죠{TAG}EF",
     f"래요{TAG}EF",
     f"네요{TAG}EF",
     f"나요{TAG}EF",
     f"대요{TAG}EF",
     f"ᆯ게요{TAG}EF",
     f"ᆫ대요{TAG}EF",
     f"ᆫ가요{TAG}EF"
 }
 
 FORMAL = {
     f"습니다{TAG}EF",
-    f"시{TAG}EP{SEP}습니다{TAG}EF",
     f"습니까{TAG}EF",
     f"랍니다{TAG}EF",
     f"ᆸ니까{TAG}EF",
     f"ᆸ시오{TAG}EF",
     f"ᆸ니다{TAG}EF",
-    f"ᆸ시다{TAG}EF"
+    f"ᆸ시다{TAG}EF",
+    f"읍시다{TAG}EF",
 }
 
 
 # --- regex --- #
 EFS = rf"(?P<MASK>({'|'.join([pair for pair in (CASUAL | POLITE | FORMAL)])}))"
 SELF = rf"\g<MASK>"
 WITH_JONG_SUNG = rf"[{''.join({chr(i) for i in range(44032, 55204)} - {chr(44032 + 28 * i) for i in range(399)})}]"
+NO_JONG_SUNG = rf"[^{''.join({chr(i) for i in range(44032, 55204)} - {chr(44032 + 28 * i) for i in range(399)})}]"
 
 
 # --- programmatically populated RULES --- #
 RULES: Dict[str, Tuple[Set[str], Set[str], Set[str]]] = dict()
 
 # --- the overarching rule --- #
 RULES.update({
@@ -93,22 +100,33 @@
             CASUAL - {f"ᆫ다{TAG}EF", f"ᆯ게{TAG}EF", f"ᆫ대{TAG}EF"},
             POLITE - {f"ᆯ게요{TAG}EF", f"ᆫ대요{TAG}EF", f"ᆫ가요{TAG}EF"},
             FORMAL - {f"ᆸ니까{TAG}EF", f"ᆸ시오{TAG}EF", f"ᆸ니다{TAG}EF", f"ᆸ시다{TAG}EF"}
         )
     }
 )
 
+# --- 종성이 없는 경우, 어/EF, f"어라{TAG}EF", 어요/EF는 사용하지 않음 --- #
+RULES.update(
+    {
+        rf"{NO_JONG_SUNG}{TAG}[A-Z\-]+?{SEP}{EFS}": (
+            CASUAL - {f"어{TAG}EF", f"어라{TAG}EF"},
+            POLITE - {f"어요{TAG}EF"},
+            FORMAL
+        )
+    }
+)
+
 
 # --- 의문형인 경우, formal은 -니까만 가능 --- #
 RULES.update(
     {
         rf"{EFS}{SEP}\?{TAG}SF": (
             CASUAL,
             POLITE,
-            {f"습니까{TAG}EF", f"ᆸ니까{TAG}EF"}
+            {f"습니까{TAG}EF", f"ᆸ니까{TAG}EF", f"시{TAG}EP{SEP}ᆸ니까{TAG}EF"}
         )
     }
 )
 
 # --- 나/저 --- #
 RULES.update(
     {
@@ -188,13 +206,27 @@
             #  전부 가능함
             FORMAL
         )
     }
 )
 
 
+# --- 시 + ㄴ가요 -> 시 + 니 --- #
+RULES.update(
+    {
+        rf"시{TAG}EP{SEP}(?P<MASK>ᆫ가요{TAG}EF)": (
+            {f"니{TAG}EF"},
+            {f"ᆫ가요{TAG}EF"},
+            {f"ᆸ니까{TAG}EF"}
+        )
+    }
+)
+
+
 # ---- to be used for scoring -- #
-PREFERENCES = {f"어{TAG}EF",
-               f"어요{TAG}EF",
-               f"어요{TAG}EF",
-               f"습니다{TAG}EF",
-               f"ᆸ니다{TAG}EF"}
+PREFERENCES = {
+    f"어{TAG}EF",
+    f"어요{TAG}EF",
+    f"어요{TAG}EF",
+    f"습니다{TAG}EF",
+    f"ᆸ니다{TAG}EF"
+}
```

### Comparing `politely-3.2.5/politely/styler.py` & `politely-3.3.0/politely/styler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 import itertools
+import os
 import re
 from copy import copy, deepcopy
+import random
 from typing import Any, List, Tuple, Dict, Set
 from functools import wraps
+import numpy as np
+import torch
 from politely.errors import EFNotSupportedError, SFNotIncludedError, EFNotIncludedError
 from politely.fetchers import fetch_kiwi
-from politely import RULES, SEP, TAG, NULL, SELF, CASUAL, POLITE, FORMAL
+from politely import RULES, SEP, TAG, NULL, SELF
+from politely.modeling_gpt2_scorer import GPT2Scorer
+from politely.modeling_scorer import Scorer
 from politely.rules import EFS
-from politely.scorer import Scorer
 
 
 def log(f):
     @wraps(f)
     def wrapper(*args, **kwargs):
         out = f(*args, **kwargs)
         # get the function signature
@@ -21,16 +26,16 @@
     return wrapper
 
 
 class Styler:
     """
     A rule-based Korean Politeness Styler
     """
-    def __init__(self, strict: bool = False, scorer: Scorer = Scorer()):
-        # object-owned attributes
+    def __init__(self, strict: bool = False, scorer: Scorer = GPT2Scorer()):
+        #  --- object-owned attributes --- #
         self.scorer = scorer
         self.strict = strict
         self.out: Any = None
         self.kiwi = fetch_kiwi()
         self.rules = deepcopy(RULES)
         self.logs = dict()
 
@@ -51,14 +56,23 @@
     def setup(self):
         """
         Reset the out and clear all the logs,
         """
         self.out = None
         self.logs.clear()
         self.logs.update({"conjugations": set(), "honorifics": set()})
+        # --- seed everything --- #
+        seed = 318
+        random.seed(seed)
+        os.environ['PYTHONHASHSEED'] = str(seed)
+        np.random.seed(seed)
+        torch.manual_seed(seed)
+        torch.cuda.manual_seed(seed)
+        torch.backends.cudnn.deterministic = True
+        torch.backends.cudnn.benchmark = True
         return self
 
     def preprocess(self, sent: str):
         """
         Make sure each sentence ends with a period, if it does not end with any SF.
         We do this to increase the accuracy of `kiwi.join`.
         """
@@ -100,22 +114,23 @@
         Do this by chain-conjugating sets.
         """
         self.out: str
         pair2honorifics = {}
         for pattern in self.rules.keys():
             match = re.search(pattern, self.out)
             if match:
-                matched_pair = match.group("MASK")
-                honorifics = {honorific.replace(SELF, matched_pair) for honorific in self.rules[pattern][politeness]}
+                # should be only one pair
+                pair = match.group("MASK")
+                honorifics = {honorific.replace(SELF, pair) for honorific in self.rules[pattern][politeness]}
                 # progressively narrow down honorifics
-                pair2honorifics[matched_pair] = pair2honorifics.get(matched_pair, honorifics) & honorifics
+                pair2honorifics[pair] = pair2honorifics.get(pair, honorifics) & honorifics
         # get all possible candidates
         candidates = itertools.product(*[
             pair2honorifics.get(pair, {pair, })
-            for pair in self.out.split(SEP)
+            for pair in self.out.split(SEP)  # SEP
         ])
         # remove empty candidates
         candidates = [
             [pair.split(SEP) for pair in candidate if pair != NULL]
             for candidate in candidates
         ]
         # flatten pairs
@@ -129,25 +144,16 @@
 
     @log
     def guess(self):
         """
         Guess the scores.
         """
         self.out: List[List[str]]
-        politeness = self.logs['honorify']['in']['politeness']
-        original_pairs = self.logs['analyze']['out'].split(SEP)
-        if politeness == 0:
-            boost_pairs = CASUAL & set(original_pairs)
-        elif politeness == 1:
-            boost_pairs = POLITE & set(original_pairs)
-        elif politeness == 2:
-            boost_pairs = FORMAL & set(original_pairs)
-        else:
-            raise ValueError(f"politeness should be one of (0, 1, 2), but got {politeness}")
-        scores = [self.scorer(set(candidate), boost_pairs) for candidate in self.out]
+        # score each candidate
+        scores = self.scorer(self.out, self.logs, self.kiwi)
         self.out = [(candidate, score) for candidate, score in zip(self.out, scores)]
         return self
 
     def conjugate(self):
         """
         Elect the best candidate and conjugate its pairs.
         """
@@ -159,15 +165,15 @@
     def add_rules(self, rules: Dict[str, Tuple[Set,
                                                Set,
                                                Set]]):
         """
         Add rules to the existing rules.
         """
         # check if the rules are in proper format
-        for key, (val_c, val_p, val_f) in rules.items():
+        for key, _ in rules.items():
             # first, check if the key includes a group with the key; (?<MASK>...)
             # e.g. (?P<MASK>(아빠|아버지){TAG}NNG)
             if not re.search(re.escape(r"(?P<MASK>") + r".*" + re.escape(")"), key):
                 raise ValueError(f"key should include a group with the key; (?P<MASK>...), but got {key}")
         self.rules.update(rules)
         return self
```

### Comparing `politely-3.2.5/.gitignore` & `politely-3.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `politely-3.2.5/README.md` & `politely-3.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -149,37 +149,14 @@
 ```
 
 Or just visit [the demo we are hosting](https://eubinecto-politely-main-streamlit-4vmces.streamlitapp.com) for you | 
 --- |
 <img width="743" alt="image" src="https://user-images.githubusercontent.com/56193069/177812857-afa40454-1afd-4b09-873f-aa9db3495d9e.png"> | 
 
 
-## What `politely` can't 🙅
-
-`politely`'s `Styler` cannnot take contexts into account because its conjugation algorithm is fundamentally rule-based. The algorithm is nothing but a chain of glorified if-else's. As a consequence of this, `Styler` can't disambiguate context-dependent conjugations, like so:  
-
-```python3
-# 권유 / 청유의 차이는 맥락에 의존
-print(styler("저는 쓰레기를 주워요.", 2))
-print(styler("자, 같이 쓰레기를 주워요.", 2))
-```
-```
-저는 쓰레기를 줍습니다.
-자, 같이 쓰레기를 줍습니다. (should be "자, 같이 쓰레기를 주웁시다")
-```
-```python3
-# 이르 + 어 -> 이르러/일러 또한 맥락에 의존
-print(styler("하지 말라고 일렀다.", 2))
-print(styler("정상에 이르렀다.", 2))
-```
-```
-하지 말라고 일렀습니다.
-정상에 일렀습니다. (should be "정상에 이르렀습니다")
-```
-
 
 ## By whom? 👏
 - funded by: [Faculty of Oriental Studies](https://www.orinst.ox.ac.uk) at the University of Oxford 
 - led & developed by: [Jieun Kiaer](https://www.orinst.ox.ac.uk/people/jieun-kiaer) (Associate Professor of Korean Language and Linguistics at the University of Oxford)
 - co-developed by: Research assistant Eu-Bin KIM (Msc. in Applied Linguistics at the University of Oxford, Bsc. in AI at the University of Manchester )
```

### Comparing `politely-3.2.5/pyproject.toml` & `politely-3.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `politely-3.2.5/PKG-INFO` & `politely-3.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: politely
-Version: 3.2.5
+Version: 3.3.0
 Summary: A rule-based politeness styler for the Korean Language
 Project-URL: Documentation, https://github.com/unknown/politely#readme
 Project-URL: Issues, https://github.com/unknown/politely/issues
 Project-URL: Source, https://github.com/unknown/politely
 Author-email: Eu-Bin KIM <tlrndk123@gmail.com>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
@@ -171,37 +171,14 @@
 ```
 
 Or just visit [the demo we are hosting](https://eubinecto-politely-main-streamlit-4vmces.streamlitapp.com) for you | 
 --- |
 <img width="743" alt="image" src="https://user-images.githubusercontent.com/56193069/177812857-afa40454-1afd-4b09-873f-aa9db3495d9e.png"> | 
 
 
-## What `politely` can't 🙅
-
-`politely`'s `Styler` cannnot take contexts into account because its conjugation algorithm is fundamentally rule-based. The algorithm is nothing but a chain of glorified if-else's. As a consequence of this, `Styler` can't disambiguate context-dependent conjugations, like so:  
-
-```python3
-# 권유 / 청유의 차이는 맥락에 의존
-print(styler("저는 쓰레기를 주워요.", 2))
-print(styler("자, 같이 쓰레기를 주워요.", 2))
-```
-```
-저는 쓰레기를 줍습니다.
-자, 같이 쓰레기를 줍습니다. (should be "자, 같이 쓰레기를 주웁시다")
-```
-```python3
-# 이르 + 어 -> 이르러/일러 또한 맥락에 의존
-print(styler("하지 말라고 일렀다.", 2))
-print(styler("정상에 이르렀다.", 2))
-```
-```
-하지 말라고 일렀습니다.
-정상에 일렀습니다. (should be "정상에 이르렀습니다")
-```
-
 
 ## By whom? 👏
 - funded by: [Faculty of Oriental Studies](https://www.orinst.ox.ac.uk) at the University of Oxford 
 - led & developed by: [Jieun Kiaer](https://www.orinst.ox.ac.uk/people/jieun-kiaer) (Associate Professor of Korean Language and Linguistics at the University of Oxford)
 - co-developed by: Research assistant Eu-Bin KIM (Msc. in Applied Linguistics at the University of Oxford, Bsc. in AI at the University of Manchester )
```

