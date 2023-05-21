# Comparing `tmp/pref_voting-0.2.8.tar.gz` & `tmp/pref_voting-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pref_voting-0.2.8.tar", max compression
+gzip compressed data, was "pref_voting-0.2.9.tar", max compression
```

## Comparing `pref_voting-0.2.8.tar` & `pref_voting-0.2.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1068 2022-07-08 15:47:57.000000 pref_voting-0.2.8/LICENSE
--rw-r--r--   0        0        0     2756 2023-05-16 18:00:59.189933 pref_voting-0.2.8/README.md
--rw-r--r--   0        0        0       22 2023-05-16 18:00:58.034340 pref_voting-0.2.8/pref_voting/__init__.py
--rw-r--r--   0        0        0     9631 2023-05-10 11:35:26.690819 pref_voting-0.2.8/pref_voting/analysis.py
--rw-r--r--   0        0        0     1226 2023-05-10 11:42:24.592401 pref_voting-0.2.8/pref_voting/axiom.py
--rw-r--r--   0        0        0      360 2023-05-10 11:16:28.091090 pref_voting-0.2.8/pref_voting/axiom_helpers.py
--rw-r--r--   0        0        0       43 2023-04-27 22:57:52.337540 pref_voting-0.2.8/pref_voting/axioms.py
--rw-r--r--   0        0        0    23065 2023-05-10 11:22:02.837497 pref_voting-0.2.8/pref_voting/c1_methods.py
--rw-r--r--   0        0        0     8564 2023-02-15 17:29:01.299008 pref_voting-0.2.8/pref_voting/combined_methods.py
--rw-r--r--   0        0        0    11517 2023-05-10 11:58:43.699679 pref_voting-0.2.8/pref_voting/dominance_axioms.py
--rw-r--r--   0        0        0    20643 2023-05-10 11:16:22.353419 pref_voting-0.2.8/pref_voting/generate_profiles.py
--rw-r--r--   0        0        0    10484 2023-01-11 11:10:14.000000 pref_voting-0.2.8/pref_voting/generate_weighted_majority_graphs.py
--rw-r--r--   0        0        0     1806 2022-08-08 19:08:16.000000 pref_voting-0.2.8/pref_voting/helper.py
--rw-r--r--   0        0        0    73229 2023-05-10 11:16:21.455329 pref_voting-0.2.8/pref_voting/iterative_methods.py
--rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-0.2.8/pref_voting/maj_graph_ex1.png
--rw-r--r--   0        0        0    57868 2023-05-10 11:18:39.320393 pref_voting-0.2.8/pref_voting/margin_based_methods.py
--rw-r--r--   0        0        0    25681 2023-05-10 11:20:32.560828 pref_voting-0.2.8/pref_voting/other_methods.py
--rw-r--r--   0        0        0     9526 2023-05-10 11:24:57.793416 pref_voting-0.2.8/pref_voting/pr_voting_methods.py
--rw-r--r--   0        0        0    26954 2023-05-15 22:14:59.029784 pref_voting-0.2.8/pref_voting/profiles.py
--rw-r--r--   0        0        0    34203 2023-04-27 22:31:21.483788 pref_voting-0.2.8/pref_voting/profiles_with_ties.py
--rw-r--r--   0        0        0    11064 2023-05-05 16:30:25.075183 pref_voting-0.2.8/pref_voting/scoring_methods.py
--rw-r--r--   0        0        0     5381 2023-02-15 15:31:23.315651 pref_voting-0.2.8/pref_voting/voting_method.py
--rw-r--r--   0        0        0      253 2022-07-31 21:02:46.000000 pref_voting-0.2.8/pref_voting/voting_methods.py
--rw-r--r--   0        0        0    49214 2023-05-16 18:00:25.171109 pref_voting-0.2.8/pref_voting/weighted_majority_graphs.py
--rw-r--r--   0        0        0      715 2023-05-16 18:00:58.624385 pref_voting-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     3731 1970-01-01 00:00:00.000000 pref_voting-0.2.8/setup.py
--rw-r--r--   0        0        0     3850 1970-01-01 00:00:00.000000 pref_voting-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2022-07-08 15:47:57.000000 pref_voting-0.2.9/LICENSE
+-rw-r--r--   0        0        0     2843 2023-05-16 22:54:30.865590 pref_voting-0.2.9/README.md
+-rw-r--r--   0        0        0       22 2023-05-16 22:54:28.075986 pref_voting-0.2.9/pref_voting/__init__.py
+-rw-r--r--   0        0        0     9631 2023-05-10 11:35:26.690819 pref_voting-0.2.9/pref_voting/analysis.py
+-rw-r--r--   0        0        0     1226 2023-05-10 11:42:24.592401 pref_voting-0.2.9/pref_voting/axiom.py
+-rw-r--r--   0        0        0      360 2023-05-10 11:16:28.091090 pref_voting-0.2.9/pref_voting/axiom_helpers.py
+-rw-r--r--   0        0        0       43 2023-04-27 22:57:52.337540 pref_voting-0.2.9/pref_voting/axioms.py
+-rw-r--r--   0        0        0    23065 2023-05-10 11:22:02.837497 pref_voting-0.2.9/pref_voting/c1_methods.py
+-rw-r--r--   0        0        0     8564 2023-02-15 17:29:01.299008 pref_voting-0.2.9/pref_voting/combined_methods.py
+-rw-r--r--   0        0        0    11517 2023-05-10 11:58:43.699679 pref_voting-0.2.9/pref_voting/dominance_axioms.py
+-rw-r--r--   0        0        0    20643 2023-05-10 11:16:22.353419 pref_voting-0.2.9/pref_voting/generate_profiles.py
+-rw-r--r--   0        0        0    10484 2023-01-11 11:10:14.000000 pref_voting-0.2.9/pref_voting/generate_weighted_majority_graphs.py
+-rw-r--r--   0        0        0     1806 2022-08-08 19:08:16.000000 pref_voting-0.2.9/pref_voting/helper.py
+-rw-r--r--   0        0        0    73229 2023-05-10 11:16:21.455329 pref_voting-0.2.9/pref_voting/iterative_methods.py
+-rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-0.2.9/pref_voting/maj_graph_ex1.png
+-rw-r--r--   0        0        0    59105 2023-05-16 22:53:18.787316 pref_voting-0.2.9/pref_voting/margin_based_methods.py
+-rw-r--r--   0        0        0    25681 2023-05-10 11:20:32.560828 pref_voting-0.2.9/pref_voting/other_methods.py
+-rw-r--r--   0        0        0     9526 2023-05-10 11:24:57.793416 pref_voting-0.2.9/pref_voting/pr_voting_methods.py
+-rw-r--r--   0        0        0    26954 2023-05-15 22:14:59.029784 pref_voting-0.2.9/pref_voting/profiles.py
+-rw-r--r--   0        0        0    34203 2023-04-27 22:31:21.483788 pref_voting-0.2.9/pref_voting/profiles_with_ties.py
+-rw-r--r--   0        0        0    11064 2023-05-05 16:30:25.075183 pref_voting-0.2.9/pref_voting/scoring_methods.py
+-rw-r--r--   0        0        0     5381 2023-02-15 15:31:23.315651 pref_voting-0.2.9/pref_voting/voting_method.py
+-rw-r--r--   0        0        0      253 2022-07-31 21:02:46.000000 pref_voting-0.2.9/pref_voting/voting_methods.py
+-rw-r--r--   0        0        0    49214 2023-05-16 18:00:25.171109 pref_voting-0.2.9/pref_voting/weighted_majority_graphs.py
+-rw-r--r--   0        0        0      715 2023-05-16 22:54:29.631117 pref_voting-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     3819 1970-01-01 00:00:00.000000 pref_voting-0.2.9/setup.py
+-rw-r--r--   0        0        0     3937 1970-01-01 00:00:00.000000 pref_voting-0.2.9/PKG-INFO
```

### Comparing `pref_voting-0.2.8/LICENSE` & `pref_voting-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.8/README.md` & `pref_voting-0.2.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 - v0.1.27 (2023-2-07): Add Borda for ProfileWithTies
 - v0.2 (2023-2-15): Add Benham, add anonymize to Profile method, comment out numba to make compatible with Python 3.11, add add_unranked_candidates to ProfileWithTies
 - v0.2.1 (2023-2-15): Bug fixes
 - v0.2.3 (2023-4-2): Add plurality_with_runoff_with_explanation
 - v0.2.4 (2023-4-9): Update generate_truncated_profile so that it implements the IC probability model.
 - v0.2.6 (2023-5-10): Add axiom class, dominance axioms, and axiom_violations_data.
 - v0.2.8 (2023-5-16): Add description function to Majority Graphs.
+- v0.2.9 (2023-5-16): Update implementation of Simple Stable Voting and Stable Voting.
 
 ## Questions?
 
 Feel free to [send me an email](https://pacuit.org/) if you have questions about the project.
 
 ## License
```

### Comparing `pref_voting-0.2.8/pref_voting/analysis.py` & `pref_voting-0.2.9/pref_voting/analysis.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.8/pref_voting/axiom.py` & `pref_voting-0.2.9/pref_voting/axiom.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.8/pref_voting/c1_methods.py` & `pref_voting-0.2.9/pref_voting/c1_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.8/pref_voting/combined_methods.py` & `pref_voting-0.2.9/pref_voting/combined_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.8/pref_voting/dominance_axioms.py` & `pref_voting-0.2.9/pref_voting/dominance_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.8/pref_voting/generate_profiles.py` & `pref_voting-0.2.9/pref_voting/generate_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.8/pref_voting/generate_weighted_majority_graphs.py` & `pref_voting-0.2.9/pref_voting/generate_weighted_majority_graphs.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.8/pref_voting/helper.py` & `pref_voting-0.2.9/pref_voting/helper.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.8/pref_voting/iterative_methods.py` & `pref_voting-0.2.9/pref_voting/iterative_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.8/pref_voting/maj_graph_ex1.png` & `pref_voting-0.2.9/pref_voting/maj_graph_ex1.png`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.8/pref_voting/margin_based_methods.py` & `pref_voting-0.2.9/pref_voting/margin_based_methods.py`

 * *Files 3% similar despite different names*

```diff
@@ -1086,50 +1086,59 @@
                         river_defeat.add_edge(e[0], e[1], weight=e[2])
                         if does_create_cycle(river_defeat, e):
                             river_defeat.remove_edge(e[0], e[1])
                 winners.append(maximal_elements(river_defeat)[0])
     return sorted(list(set(winners)))
 
 # Simple Stable Voting 
-def _simple_stable_voting(edata, curr_cands = None, mem_sv_winners = {}, strength_function = None): 
+def _simple_stable_voting(edata, 
+                          curr_cands = None, 
+                          mem_sv_winners = {}, 
+                          strength_function = None,
+                          sorted_matches = None): 
     '''
     Determine the Simple Stable Voting winners while keeping track 
     of the winners in any subprofiles checked during computation. 
     '''
     
     # curr_cands is the set of candidates who have not been removed
     curr_cands = edata.candidates if curr_cands is None else curr_cands
     strength_function = edata.margin if strength_function is None else strength_function  
     
     sv_winners = list()
 
-    matches = [(a, b) for a in curr_cands for b in curr_cands if a != b]
-    strengths = list(set([strength_function(a, b) for a,b in matches]))
-    
+    if sorted_matches is None:
+        matches = [(a, b, strength_function(a, b)) for a in curr_cands for b in curr_cands if a != b]
+        sorted_matches = sorted(matches, reverse=True, key=lambda m_w_weight: m_w_weight[2])
+        
     if len(curr_cands) == 1: 
         mem_sv_winners[tuple(curr_cands)] = curr_cands
         return curr_cands, mem_sv_winners
-    for s in sorted(strengths, reverse=True):
-        for a, b in [ab_match for ab_match in matches 
-                     if strength_function(ab_match[0], ab_match[1]) == s]:
-            if a not in sv_winners: 
-                cands_minus_b = [c for c in curr_cands if c!= b]
-                cands_minus_b_key = tuple(sorted(cands_minus_b))
-                if cands_minus_b_key not in mem_sv_winners.keys(): 
-                    ws, mem_sv_winners = _simple_stable_voting(edata, 
-                                                               curr_cands = cands_minus_b,
-                                                               mem_sv_winners = mem_sv_winners,
-                                                               strength_function = strength_function)
-                    mem_sv_winners[cands_minus_b_key] = ws
-                else: 
-                    ws = mem_sv_winners[cands_minus_b_key]
-                if a in ws:
-                    sv_winners.append(a)
-        if len(sv_winners) > 0: 
-            return sv_winners, mem_sv_winners
+    
+    max_margin_witnessing_win = -math.inf
+
+    for a, b, s in sorted_matches:
+        if s < max_margin_witnessing_win: 
+            break
+        if a not in sv_winners: 
+            cands_minus_b = [c for c in curr_cands if c != b]
+            cands_minus_b_key = tuple(sorted(cands_minus_b))
+            if cands_minus_b_key not in mem_sv_winners.keys(): 
+                ws, mem_sv_winners = _simple_stable_voting(edata, 
+                                                           curr_cands = cands_minus_b,
+                                                           mem_sv_winners = mem_sv_winners,
+                                                           strength_function = strength_function, 
+                                                           sorted_matches = [(a, c, s) for a, c, s in sorted_matches if c != b and a != b])
+                mem_sv_winners[cands_minus_b_key] = ws
+            else: 
+                ws = mem_sv_winners[cands_minus_b_key]
+            if a in ws:
+                sv_winners.append(a)
+                max_margin_witnessing_win = s
+    return sv_winners, mem_sv_winners
 
           
 @vm(name = "Simple Stable Voting")
 def simple_stable_voting(edata, curr_cands = None, strength_function = None): 
     """Implementation of  Simple Stable Voting from https://arxiv.org/abs/2108.00542. 
 
     Simple Stable Voting is a recursive voting method defined as follows: 
@@ -1159,15 +1168,19 @@
 
         mg = MarginGraph([0, 1, 2, 3], [(0, 3, 8), (1, 0, 10), (2, 0, 4), (2, 1, 8), (3, 1, 8)])
 
         simple_stable_voting.display(mg)
 
     """
     
-    return sorted(_simple_stable_voting(edata, curr_cands = curr_cands, mem_sv_winners = {}, strength_function = strength_function)[0])
+    return sorted(_simple_stable_voting(edata, 
+                                        curr_cands = curr_cands, 
+                                        mem_sv_winners = {}, 
+                                        strength_function = strength_function)[0],
+                                        sorted_matches = None)
 
 
 @vm(name = "Simple Stable Voting")
 def simple_stable_voting_faster(edata, curr_cands = None, strength_function = None): 
     """Simple Stable Voting is Condorcet consistent.   It is faster to skip executing the recursive algorithm when there is a Condorcet winnerFirst check if there is a Condorcet winner.  If so, return the Condorcet winner, otherwise find the Simple Stable Voting winner using _simple_stable_voting
 
     Args:
@@ -1197,53 +1210,67 @@
 
     """
     
     cw = edata.condorcet_winner(curr_cands = None)
     if cw is not None: 
         return [cw]
     else: 
-        return sorted(_simple_stable_voting(edata, curr_cands = curr_cands, mem_sv_winners = {}, strength_function = strength_function)[0])
+        return sorted(_simple_stable_voting(edata, 
+                                            curr_cands = curr_cands, 
+                                            mem_sv_winners = {}, 
+                                            strength_function = strength_function)[0],
+                                            sorted_matches = None)
 
     
-def _stable_voting(edata, curr_cands = None, mem_sv_winners = {}, strength_function = None): 
+def _stable_voting(edata, 
+                   curr_cands = None,
+                   mem_sv_winners = {}, 
+                   strength_function = None, 
+                   sorted_matches = None): 
     '''
     Determine the Stable Voting winners for the profile while keeping track of the winners in any subprofiles checked during computation. 
     '''
     
     # curr_cands is the set of candidates who have not been removed
     curr_cands = edata.candidates if curr_cands is None else curr_cands
     strength_function = edata.margin if strength_function is None else strength_function  
-
+    
     sv_winners = list()
     
     undefeated_candidates = split_cycle_faster(edata, curr_cands = curr_cands)
-    matches = [(a, b) for a in curr_cands for b in curr_cands if a != b if a in undefeated_candidates]
-    strengths = list(set([strength_function(a, b) for a,b in matches]))
+
+    if sorted_matches is None:
+        matches = [(a, b, strength_function(a, b)) for a in curr_cands for b in curr_cands if a != b]
+        sorted_matches = sorted(matches, reverse=True, key=lambda m_w_weight: m_w_weight[2])
         
     if len(curr_cands) == 1: 
         mem_sv_winners[tuple(curr_cands)] = curr_cands
         return curr_cands, mem_sv_winners
-    for s in sorted(strengths, reverse=True):
-        for a, b in [ab_match for ab_match in matches 
-                     if strength_function(ab_match[0], ab_match[1])  == s]:
-            if a not in sv_winners: 
-                cands_minus_b = [c for c in curr_cands if c!= b]
-                cands_minus_b_key = tuple(sorted(cands_minus_b))
-                if cands_minus_b_key not in mem_sv_winners.keys(): 
-                    ws, mem_sv_winners = _stable_voting(edata, 
-                                                        curr_cands = cands_minus_b, 
-                                                        mem_sv_winners = mem_sv_winners, 
-                                                        strength_function = strength_function)
-                    mem_sv_winners[cands_minus_b_key] = ws
-                else: 
-                    ws = mem_sv_winners[cands_minus_b_key]
-                if a in ws:
-                    sv_winners.append(a)
-        if len(sv_winners) > 0: 
-            return sv_winners, mem_sv_winners
+    
+    max_margin_witnessing_win = -math.inf
+
+    for a, b, s in sorted_matches:
+        if s < max_margin_witnessing_win: 
+            break
+        if a in undefeated_candidates and a not in sv_winners: 
+            cands_minus_b = [c for c in curr_cands if c != b]
+            cands_minus_b_key = tuple(sorted(cands_minus_b))
+            if cands_minus_b_key not in mem_sv_winners.keys(): 
+                ws, mem_sv_winners = _stable_voting(edata,
+                                                    curr_cands = cands_minus_b,
+                                                    mem_sv_winners = mem_sv_winners,
+                                                    strength_function = strength_function, 
+                                                    sorted_matches = [(a, c, s) for a, c, s in sorted_matches if c != b and a != b])
+                mem_sv_winners[cands_minus_b_key] = ws
+            else: 
+                ws = mem_sv_winners[cands_minus_b_key]
+            if a in ws:
+                sv_winners.append(a)
+                max_margin_witnessing_win = s
+    return sv_winners, mem_sv_winners
         
 @vm(name = "Stable Voting")
 def stable_voting(edata, curr_cands = None, strength_function = None): 
     """Implementation of  Stable Voting from https://arxiv.org/abs/2108.00542. 
 
     Stable Voting is a recursive voting method defined as follows: 
 
@@ -1271,15 +1298,19 @@
         from pref_voting.margin_based_methods import stable_voting
 
         mg = MarginGraph([0, 1, 2, 3], [(0, 3, 8), (1, 0, 10), (2, 0, 4), (2, 1, 8), (3, 1, 8)])
 
         stable_voting.display(mg)
 
     """
-    return sorted(_stable_voting(edata, curr_cands = curr_cands, mem_sv_winners = {}, strength_function = strength_function)[0])
+    return sorted(_stable_voting(edata, 
+                                 curr_cands = curr_cands, 
+                                 mem_sv_winners = {}, 
+                                 strength_function = strength_function)[0],
+                                 sorted_matches = None)
 
 
 @vm(name = "Stable Voting")
 def stable_voting_faster(edata, curr_cands = None, strength_function = None): 
     """
     Stable Voting is Condorcet consistent.   It is faster to skip executing the recursive algorithm when there is a Condorcet winner.  
 
@@ -1310,18 +1341,19 @@
 
 
     """
     cw = edata.condorcet_winner(curr_cands = curr_cands)
     if cw is not None: 
         return [cw]
     else: 
-        return sorted(_stable_voting(edata, curr_cands = curr_cands, mem_sv_winners = {}, strength_function = strength_function)[0])
-
-
-
+        return sorted(_stable_voting(edata, 
+                                     curr_cands = curr_cands, 
+                                     mem_sv_winners = {}, 
+                                     strength_function = strength_function)[0],
+                                     sorted_matches = None) 
 
 
 
 mg_vms = [
     minimax, 
     split_cycle,
     split_cycle_faster,
```

### Comparing `pref_voting-0.2.8/pref_voting/other_methods.py` & `pref_voting-0.2.9/pref_voting/other_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.8/pref_voting/pr_voting_methods.py` & `pref_voting-0.2.9/pref_voting/pr_voting_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.8/pref_voting/profiles.py` & `pref_voting-0.2.9/pref_voting/profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.8/pref_voting/profiles_with_ties.py` & `pref_voting-0.2.9/pref_voting/profiles_with_ties.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.8/pref_voting/scoring_methods.py` & `pref_voting-0.2.9/pref_voting/scoring_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.8/pref_voting/voting_method.py` & `pref_voting-0.2.9/pref_voting/voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.8/pref_voting/weighted_majority_graphs.py` & `pref_voting-0.2.9/pref_voting/weighted_majority_graphs.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.8/pyproject.toml` & `pref_voting-0.2.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "pref_voting"
-version = "0.2.8"
+version = "0.2.9"
 description = "pref_voting is a Python packaging that contains tools to reason about election profiles and margin graphs, and implementations of a variety of preferential voting methods."
 authors = ["Eric Pacuit <epacuit@umd.edu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/voting-tools/pref_voting"
 repository = "https://github.com/voting-tools/pref_voting"
```

### Comparing `pref_voting-0.2.8/setup.py` & `pref_voting-0.2.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,17 +12,17 @@
  'networkx>=3.0,<4.0',
  'random2>=1.0.1,<2.0.0',
  'scipy>=1.0.0,<2.0.0',
  'tabulate>=0.9.0,<0.10.0']
 
 setup_kwargs = {
     'name': 'pref-voting',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': 'pref_voting is a Python packaging that contains tools to reason about election profiles and margin graphs, and implementations of a variety of preferential voting methods.',
-    'long_description': 'pref_voting\n==========\n\n## Installation\n\nWith pip package manager:\n\n```bash\npip install pref_voting\n```\n## Documentation\n\nOnline documentation is available at [https://pref_voting.readthedocs.io](https://pref_voting.readthedocs.io).\n\n## Profiles and Voting Methods\n\nA profile (of linear orders over the candidates) is created by initializing a Profile class object.  This needs a list of rankings (each ranking is a tuple of numbers), the number of candidates, and a list giving the number of each ranking in the profile:\n\n```python\nfrom pref_voting.profiles import Profile\n\nrankings = [(0, 1, 2, 3), (2, 3, 1, 0), (3, 1, 2, 0), (1, 2, 0, 3), (1, 3, 2, 0)]\nrcounts = [5, 3, 2, 4, 3]\n\nprof = Profile(rankings, rcounts=rcounts)\n```\n\nThe function generate_profile is used to generate a profile for a given number of candidates and voters:  \n```python\nfrom pref_voting.generate_profiles import generate_profile\n\n# generate a profile using the Impartial Culture probability model\nprof = generate_profile(3, 4) # prof is a Profile object\n\n# generate a profile using the Impartial Anonymous Culture probability model\nprof = generate_profile(3, 4, probmod = "IAC") # prof is a Profile object \n```\n\n```python\nfrom pref_voting.profiles import Profile\nfrom pref_voting.voting_methods import *\n\nprof = Profile(rankings, num_cands, rcounts=rcounts)\nprint(f"{split_cycle.name} winners:  {split_cycle(prof)}")\nsplit_cycle.display(prof)\n\n```\n\n## Versions\n\n- v0.1.10 (2022-08-09): **Initial release** \n- v0.1.13 (2022-11-05): Minor updates and bug fixes \n- v0.1.14 (2022-12-19): Add plurality_scores to ProfileWithTies; add generate ceots function; bug fixes \n- v0.1.23 (2022-12-27): Add instant_runoff_for_truncated_linear_orders and functions to truncate overvotes in a ProfileWithTies, add smith_irv_put, document analysis functions\n- v0.1.25 (2023-1-11): Add condorcet_irv, condorcet_irv_put; Update documentation; add axioms.py; add display and equality to Ranking class; fix enumerate ceots functions\n- v0.1.27 (2023-2-07): Add Borda for ProfileWithTies\n- v0.2 (2023-2-15): Add Benham, add anonymize to Profile method, comment out numba to make compatible with Python 3.11, add add_unranked_candidates to ProfileWithTies\n- v0.2.1 (2023-2-15): Bug fixes\n- v0.2.3 (2023-4-2): Add plurality_with_runoff_with_explanation\n- v0.2.4 (2023-4-9): Update generate_truncated_profile so that it implements the IC probability model.\n- v0.2.6 (2023-5-10): Add axiom class, dominance axioms, and axiom_violations_data.\n- v0.2.8 (2023-5-16): Add description function to Majority Graphs.\n\n## Questions?\n\nFeel free to [send me an email](https://pacuit.org/) if you have questions about the project.\n\n## License\n\n[MIT](https://github.com/jontingvold/pyrankvote/blob/master/LICENSE.txt)\n',
+    'long_description': 'pref_voting\n==========\n\n## Installation\n\nWith pip package manager:\n\n```bash\npip install pref_voting\n```\n## Documentation\n\nOnline documentation is available at [https://pref_voting.readthedocs.io](https://pref_voting.readthedocs.io).\n\n## Profiles and Voting Methods\n\nA profile (of linear orders over the candidates) is created by initializing a Profile class object.  This needs a list of rankings (each ranking is a tuple of numbers), the number of candidates, and a list giving the number of each ranking in the profile:\n\n```python\nfrom pref_voting.profiles import Profile\n\nrankings = [(0, 1, 2, 3), (2, 3, 1, 0), (3, 1, 2, 0), (1, 2, 0, 3), (1, 3, 2, 0)]\nrcounts = [5, 3, 2, 4, 3]\n\nprof = Profile(rankings, rcounts=rcounts)\n```\n\nThe function generate_profile is used to generate a profile for a given number of candidates and voters:  \n```python\nfrom pref_voting.generate_profiles import generate_profile\n\n# generate a profile using the Impartial Culture probability model\nprof = generate_profile(3, 4) # prof is a Profile object\n\n# generate a profile using the Impartial Anonymous Culture probability model\nprof = generate_profile(3, 4, probmod = "IAC") # prof is a Profile object \n```\n\n```python\nfrom pref_voting.profiles import Profile\nfrom pref_voting.voting_methods import *\n\nprof = Profile(rankings, num_cands, rcounts=rcounts)\nprint(f"{split_cycle.name} winners:  {split_cycle(prof)}")\nsplit_cycle.display(prof)\n\n```\n\n## Versions\n\n- v0.1.10 (2022-08-09): **Initial release** \n- v0.1.13 (2022-11-05): Minor updates and bug fixes \n- v0.1.14 (2022-12-19): Add plurality_scores to ProfileWithTies; add generate ceots function; bug fixes \n- v0.1.23 (2022-12-27): Add instant_runoff_for_truncated_linear_orders and functions to truncate overvotes in a ProfileWithTies, add smith_irv_put, document analysis functions\n- v0.1.25 (2023-1-11): Add condorcet_irv, condorcet_irv_put; Update documentation; add axioms.py; add display and equality to Ranking class; fix enumerate ceots functions\n- v0.1.27 (2023-2-07): Add Borda for ProfileWithTies\n- v0.2 (2023-2-15): Add Benham, add anonymize to Profile method, comment out numba to make compatible with Python 3.11, add add_unranked_candidates to ProfileWithTies\n- v0.2.1 (2023-2-15): Bug fixes\n- v0.2.3 (2023-4-2): Add plurality_with_runoff_with_explanation\n- v0.2.4 (2023-4-9): Update generate_truncated_profile so that it implements the IC probability model.\n- v0.2.6 (2023-5-10): Add axiom class, dominance axioms, and axiom_violations_data.\n- v0.2.8 (2023-5-16): Add description function to Majority Graphs.\n- v0.2.9 (2023-5-16): Update implementation of Simple Stable Voting and Stable Voting.\n\n## Questions?\n\nFeel free to [send me an email](https://pacuit.org/) if you have questions about the project.\n\n## License\n\n[MIT](https://github.com/jontingvold/pyrankvote/blob/master/LICENSE.txt)\n',
     'author': 'Eric Pacuit',
     'author_email': 'epacuit@umd.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/voting-tools/pref_voting',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pref_voting-0.2.8/PKG-INFO` & `pref_voting-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pref-voting
-Version: 0.2.8
+Version: 0.2.9
 Summary: pref_voting is a Python packaging that contains tools to reason about election profiles and margin graphs, and implementations of a variety of preferential voting methods.
 Home-page: https://github.com/voting-tools/pref_voting
 License: MIT
 Author: Eric Pacuit
 Author-email: epacuit@umd.edu
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -81,14 +81,15 @@
 - v0.1.27 (2023-2-07): Add Borda for ProfileWithTies
 - v0.2 (2023-2-15): Add Benham, add anonymize to Profile method, comment out numba to make compatible with Python 3.11, add add_unranked_candidates to ProfileWithTies
 - v0.2.1 (2023-2-15): Bug fixes
 - v0.2.3 (2023-4-2): Add plurality_with_runoff_with_explanation
 - v0.2.4 (2023-4-9): Update generate_truncated_profile so that it implements the IC probability model.
 - v0.2.6 (2023-5-10): Add axiom class, dominance axioms, and axiom_violations_data.
 - v0.2.8 (2023-5-16): Add description function to Majority Graphs.
+- v0.2.9 (2023-5-16): Update implementation of Simple Stable Voting and Stable Voting.
 
 ## Questions?
 
 Feel free to [send me an email](https://pacuit.org/) if you have questions about the project.
 
 ## License
```

