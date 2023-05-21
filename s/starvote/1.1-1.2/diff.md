# Comparing `tmp/starvote-1.1.tar.gz` & `tmp/starvote-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starvote-1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "starvote-1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `starvote-1.1.tar` & `starvote-1.2.tar`

### file list

```diff
@@ -1,39 +1,48 @@
--rw-r--r--   0        0        0       19 2023-05-20 12:58:10.568731 starvote-1.1/.gitignore
--rw-r--r--   0        0        0     1087 2023-05-20 12:48:55.372092 starvote-1.1/LICENSE
--rw-r--r--   0        0        0     3776 2023-05-20 14:24:06.899853 starvote-1.1/README.md
--rw-r--r--   0        0        0      267 2023-05-20 12:47:55.671593 starvote-1.1/example.py
--rw-r--r--   0        0        0      502 2023-05-20 12:55:16.755279 starvote-1.1/pyproject.toml
--rw-r--r--   0        0        0      307 2023-05-20 14:24:30.072047 starvote-1.1/sample_polls/README.md
--rw-r--r--   0        0        0      169 2023-05-20 12:17:24.308288 starvote-1.1/sample_polls/sample_poll_automatic_runoff_breakable_tie.csv
--rw-r--r--   0        0        0      314 2023-05-20 14:22:01.282802 starvote-1.1/sample_polls/sample_poll_automatic_runoff_breakable_tie.result.txt
--rw-r--r--   0        0        0      169 2023-05-20 12:16:12.379686 starvote-1.1/sample_polls/sample_poll_automatic_runoff_unbreakable_tie.csv
--rw-r--r--   0        0        0      382 2023-05-20 14:22:01.298802 starvote-1.1/sample_polls/sample_poll_automatic_runoff_unbreakable_tie.result.txt
--rw-r--r--   0        0        0      169 2023-05-20 12:27:44.977476 starvote-1.1/sample_polls/sample_poll_score_round_breakable_tie_between_second_and_third.csv
--rw-r--r--   0        0        0      333 2023-05-20 14:22:01.314803 starvote-1.1/sample_polls/sample_poll_score_round_breakable_tie_between_second_and_third.result.txt
--rw-r--r--   0        0        0      169 2023-05-20 12:14:18.630735 starvote-1.1/sample_polls/sample_poll_score_round_unbreakable_three_way_tie_for_first.csv
--rw-r--r--   0        0        0      198 2023-05-20 14:22:01.330803 starvote-1.1/sample_polls/sample_poll_score_round_unbreakable_three_way_tie_for_first.result.txt
--rw-r--r--   0        0        0      226 2023-05-20 14:20:22.817978 starvote-1.1/sample_polls/sample_poll_score_round_unbreakable_three_way_tie_for_second.csv
--rw-r--r--   0        0        0      231 2023-05-20 14:22:01.346803 starvote-1.1/sample_polls/sample_poll_score_round_unbreakable_three_way_tie_for_second.result.txt
--rw-r--r--   0        0        0      169 2023-05-20 12:30:43.458967 starvote-1.1/sample_polls/sample_poll_score_round_unbreakable_tie_between_second_and_third.csv
--rw-r--r--   0        0        0      346 2023-05-20 14:22:01.358803 starvote-1.1/sample_polls/sample_poll_score_round_unbreakable_tie_between_second_and_third.result.txt
--rw-r--r--   0        0        0    49711 2023-05-20 12:04:34.029848 starvote-1.1/sample_polls/starvote_ballots_4tyx27ks_20230520050434.csv
--rw-r--r--   0        0        0      869 2023-05-20 14:22:01.378803 starvote-1.1/sample_polls/starvote_ballots_4tyx27ks_20230520050434.result.txt
--rw-r--r--   0        0        0     1812 2023-05-20 10:35:18.365110 starvote-1.1/sample_polls/starvote_ballots_9fm5fp2c_20230520033518.csv
--rw-r--r--   0        0        0     2411 2023-05-20 14:22:01.390803 starvote-1.1/sample_polls/starvote_ballots_9fm5fp2c_20230520033518.result.txt
--rw-r--r--   0        0        0    31534 2023-05-20 12:04:38.493885 starvote-1.1/sample_polls/starvote_ballots_9mm3519w_20230520050438.csv
--rw-r--r--   0        0        0      401 2023-05-20 14:22:01.406803 starvote-1.1/sample_polls/starvote_ballots_9mm3519w_20230520050438.result.txt
--rw-r--r--   0        0        0    57750 2023-05-20 12:04:29.149807 starvote-1.1/sample_polls/starvote_ballots_9xrw9wch_20230520050429.csv
--rw-r--r--   0        0        0      954 2023-05-20 14:22:01.426803 starvote-1.1/sample_polls/starvote_ballots_9xrw9wch_20230520050429.result.txt
--rw-r--r--   0        0        0   123039 2023-05-20 12:04:13.781679 starvote-1.1/sample_polls/starvote_ballots_dd1wc4yx_20230520050413.csv
--rw-r--r--   0        0        0      954 2023-05-20 14:22:01.446804 starvote-1.1/sample_polls/starvote_ballots_dd1wc4yx_20230520050413.result.txt
--rw-r--r--   0        0        0   250538 2023-05-20 10:34:04.044490 starvote-1.1/sample_polls/starvote_ballots_eh3cxxz7_20230520033403.csv
--rw-r--r--   0        0        0     1084 2023-05-20 14:22:01.478804 starvote-1.1/sample_polls/starvote_ballots_eh3cxxz7_20230520033403.result.txt
--rw-r--r--   0        0        0   115109 2023-05-20 12:04:19.133723 starvote-1.1/sample_polls/starvote_ballots_p4rs6xn4_20230520050419.csv
--rw-r--r--   0        0        0     2635 2023-05-20 14:22:01.502804 starvote-1.1/sample_polls/starvote_ballots_p4rs6xn4_20230520050419.result.txt
--rw-r--r--   0        0        0    48454 2023-05-20 12:04:25.689778 starvote-1.1/sample_polls/starvote_ballots_pf69snyx_20230520050425.csv
--rw-r--r--   0        0        0      412 2023-05-20 14:22:01.522804 starvote-1.1/sample_polls/starvote_ballots_pf69snyx_20230520050425.result.txt
--rw-r--r--   0        0        0    52870 2023-05-20 12:04:22.533752 starvote-1.1/sample_polls/starvote_ballots_swzw2ts6_20230520050422.csv
--rw-r--r--   0        0        0      370 2023-05-20 14:22:01.538804 starvote-1.1/sample_polls/starvote_ballots_swzw2ts6_20230520050422.result.txt
--rw-r--r--   0        0        0     5665 2023-05-20 14:21:09.494369 starvote-1.1/starvote/__init__.py
--rw-r--r--   0        0        0     1014 2023-05-20 12:53:02.770159 starvote-1.1/starvote/__main__.py
--rw-r--r--   0        0        0     4194 1970-01-01 00:00:00.000000 starvote-1.1/PKG-INFO
+-rw-r--r--   0        0        0       19 2023-05-20 12:58:10.568731 starvote-1.2/.gitignore
+-rw-r--r--   0        0        0     1087 2023-05-20 12:48:55.372092 starvote-1.2/LICENSE
+-rw-r--r--   0        0        0     4908 2023-05-21 01:24:41.056145 starvote-1.2/README.md
+-rw-r--r--   0        0        0      267 2023-05-20 12:47:55.671593 starvote-1.2/example.py
+-rw-r--r--   0        0        0      502 2023-05-20 12:55:16.755279 starvote-1.2/pyproject.toml
+-rw-r--r--   0        0        0      307 2023-05-20 14:24:30.072047 starvote-1.2/sample_polls/README.md
+-rw-r--r--   0        0        0      169 2023-05-20 12:17:24.308288 starvote-1.2/sample_polls/sample_poll_automatic_runoff_breakable_tie.csv
+-rw-r--r--   0        0        0      314 2023-05-20 14:22:01.282802 starvote-1.2/sample_polls/sample_poll_automatic_runoff_breakable_tie.result.txt
+-rw-r--r--   0        0        0      169 2023-05-20 12:16:12.379686 starvote-1.2/sample_polls/sample_poll_automatic_runoff_unbreakable_tie.csv
+-rw-r--r--   0        0        0      382 2023-05-20 14:22:01.298802 starvote-1.2/sample_polls/sample_poll_automatic_runoff_unbreakable_tie.result.txt
+-rw-r--r--   0        0        0      169 2023-05-20 12:27:44.977476 starvote-1.2/sample_polls/sample_poll_score_round_breakable_tie_between_second_and_third.csv
+-rw-r--r--   0        0        0      333 2023-05-20 14:22:01.314803 starvote-1.2/sample_polls/sample_poll_score_round_breakable_tie_between_second_and_third.result.txt
+-rw-r--r--   0        0        0      169 2023-05-20 12:14:18.630735 starvote-1.2/sample_polls/sample_poll_score_round_unbreakable_three_way_tie_for_first.csv
+-rw-r--r--   0        0        0      198 2023-05-20 14:22:01.330803 starvote-1.2/sample_polls/sample_poll_score_round_unbreakable_three_way_tie_for_first.result.txt
+-rw-r--r--   0        0        0      226 2023-05-20 14:20:22.817978 starvote-1.2/sample_polls/sample_poll_score_round_unbreakable_three_way_tie_for_second.csv
+-rw-r--r--   0        0        0      231 2023-05-20 14:22:01.346803 starvote-1.2/sample_polls/sample_poll_score_round_unbreakable_three_way_tie_for_second.result.txt
+-rw-r--r--   0        0        0      169 2023-05-20 12:30:43.458967 starvote-1.2/sample_polls/sample_poll_score_round_unbreakable_tie_between_second_and_third.csv
+-rw-r--r--   0        0        0      346 2023-05-20 14:22:01.358803 starvote-1.2/sample_polls/sample_poll_score_round_unbreakable_tie_between_second_and_third.result.txt
+-rw-r--r--   0        0        0    49711 2023-05-20 12:04:34.029848 starvote-1.2/sample_polls/starvote_ballots_4tyx27ks_20230520050434.csv
+-rw-r--r--   0        0        0   538128 2023-05-20 14:33:25.560528 starvote-1.2/sample_polls/starvote_ballots_4tyx27ks_20230520050434.result.pdf
+-rw-r--r--   0        0        0      869 2023-05-20 14:22:01.378803 starvote-1.2/sample_polls/starvote_ballots_4tyx27ks_20230520050434.result.txt
+-rw-r--r--   0        0        0     1812 2023-05-20 10:35:18.365110 starvote-1.2/sample_polls/starvote_ballots_9fm5fp2c_20230520033518.csv
+-rw-r--r--   0        0        0   807144 2023-05-20 14:33:51.120742 starvote-1.2/sample_polls/starvote_ballots_9fm5fp2c_20230520033518.result.pdf
+-rw-r--r--   0        0        0     2411 2023-05-20 14:22:01.390803 starvote-1.2/sample_polls/starvote_ballots_9fm5fp2c_20230520033518.result.txt
+-rw-r--r--   0        0        0    31534 2023-05-20 12:04:38.493885 starvote-1.2/sample_polls/starvote_ballots_9mm3519w_20230520050438.csv
+-rw-r--r--   0        0        0   325033 2023-05-20 14:34:17.572963 starvote-1.2/sample_polls/starvote_ballots_9mm3519w_20230520050438.result.pdf
+-rw-r--r--   0        0        0      401 2023-05-20 14:22:01.406803 starvote-1.2/sample_polls/starvote_ballots_9mm3519w_20230520050438.result.txt
+-rw-r--r--   0        0        0    57750 2023-05-20 12:04:29.149807 starvote-1.2/sample_polls/starvote_ballots_9xrw9wch_20230520050429.csv
+-rw-r--r--   0        0        0   575556 2023-05-20 14:35:00.177319 starvote-1.2/sample_polls/starvote_ballots_9xrw9wch_20230520050429.result.pdf
+-rw-r--r--   0        0        0      954 2023-05-20 14:22:01.426803 starvote-1.2/sample_polls/starvote_ballots_9xrw9wch_20230520050429.result.txt
+-rw-r--r--   0        0        0   123039 2023-05-20 12:04:13.781679 starvote-1.2/sample_polls/starvote_ballots_dd1wc4yx_20230520050413.csv
+-rw-r--r--   0        0        0   584998 2023-05-20 14:35:22.465506 starvote-1.2/sample_polls/starvote_ballots_dd1wc4yx_20230520050413.result.pdf
+-rw-r--r--   0        0        0      954 2023-05-20 14:22:01.446804 starvote-1.2/sample_polls/starvote_ballots_dd1wc4yx_20230520050413.result.txt
+-rw-r--r--   0        0        0   250538 2023-05-20 10:34:04.044490 starvote-1.2/sample_polls/starvote_ballots_eh3cxxz7_20230520033403.csv
+-rw-r--r--   0        0        0   643536 2023-05-20 14:35:41.153662 starvote-1.2/sample_polls/starvote_ballots_eh3cxxz7_20230520033403.result.pdf
+-rw-r--r--   0        0        0     1084 2023-05-20 14:22:01.478804 starvote-1.2/sample_polls/starvote_ballots_eh3cxxz7_20230520033403.result.txt
+-rw-r--r--   0        0        0   115109 2023-05-20 12:04:19.133723 starvote-1.2/sample_polls/starvote_ballots_p4rs6xn4_20230520050419.csv
+-rw-r--r--   0        0        0   696161 2023-05-20 14:36:00.553825 starvote-1.2/sample_polls/starvote_ballots_p4rs6xn4_20230520050419.result.pdf
+-rw-r--r--   0        0        0     2635 2023-05-20 14:22:01.502804 starvote-1.2/sample_polls/starvote_ballots_p4rs6xn4_20230520050419.result.txt
+-rw-r--r--   0        0        0    48454 2023-05-20 12:04:25.689778 starvote-1.2/sample_polls/starvote_ballots_pf69snyx_20230520050425.csv
+-rw-r--r--   0        0        0   360427 2023-05-20 14:36:25.050030 starvote-1.2/sample_polls/starvote_ballots_pf69snyx_20230520050425.result.pdf
+-rw-r--r--   0        0        0      412 2023-05-20 14:22:01.522804 starvote-1.2/sample_polls/starvote_ballots_pf69snyx_20230520050425.result.txt
+-rw-r--r--   0        0        0    52870 2023-05-20 12:04:22.533752 starvote-1.2/sample_polls/starvote_ballots_swzw2ts6_20230520050422.csv
+-rw-r--r--   0        0        0   354740 2023-05-20 14:36:48.550226 starvote-1.2/sample_polls/starvote_ballots_swzw2ts6_20230520050422.result.pdf
+-rw-r--r--   0        0        0      370 2023-05-20 14:22:01.538804 starvote-1.2/sample_polls/starvote_ballots_swzw2ts6_20230520050422.result.txt
+-rw-r--r--   0        0        0     8492 2023-05-21 01:26:59.249223 starvote-1.2/starvote/__init__.py
+-rw-r--r--   0        0        0     3368 2023-05-21 01:23:06.091404 starvote-1.2/starvote/__main__.py
+-rw-r--r--   0        0        0     5326 1970-01-01 00:00:00.000000 starvote-1.2/PKG-INFO
```

### Comparing `starvote-1.1/LICENSE` & `starvote-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `starvote-1.1/README.md` & `starvote-1.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -14,16 +14,19 @@
 To use, `import starvote`, then instantiate a `starvote.Poll` object.
 Feed in the ballots using `poll.add_ballot(ballot)`; ballots are `dict` objects,
 mapping the candidate to the ballot's vote for the candidate
 (an `int` in the range 0 to 5 inclusive).
 
 Once you've added all the ballots, call `poll.result` to compute the winner.
 If there's an unbreakable tie, `poll.result` will raise an
-`UnbreakableTieError`.  The following scenarios can result in an
-unbreakable tie:
+`UnbreakableTieError`.  You can get a text description of the tie by calling
+`str` on the exception; also, you can get a list of the tied candidates
+in its `candidates` attribute.
+
+The following scenarios produce an unbreakable tie:
 
 * If the top two candidates tie during the automated runoff round
   *and* their scores are also a tie.
 * If the second and third candidates during the score round tie,
   and their preference scores are also a tie.
 * If three or more candiates are tied for first *or* second place
   during the score round.
@@ -68,46 +71,80 @@
 If the module is executed as a script, it will read a single
 [CSV file](https://en.wikipedia.org/wiki/Comma-separated_values)
 in [*star.vote*](https://star.vote/) format, tabulate, and print
 the result.  For example, you can run this from the root of the
 source-code repository:
 
 ```
-% python3 -m starvote sample_polls/sample_vote_automatic_runoff_breakable_tie.csv
+% python3 -m starvote sample_polls/sample_poll_automatic_runoff_breakable_tie.csv
 ```
 
 to see how **starvote** handles a tie during the automatic runoff round.
 
+## Multiple-winner elections
+
+**starvote** also implements the
+[Bloc STAR](https://www.starvoting.org/multi_winner)
+variant of STAR for multi-winner elections.  Simply
+instantiate your `Poll` object passing in `starvote.BLOC_STAR`
+for the `variant` parameter, and the number of winners in
+the `winners` keyword-only parameter:
+
+```Python
+poll = starvote.Poll(variant=starvote.BLOC_STAR, winners=2)
+```
+
+This changes `poll.result` to return a list of winners instead
+of a single winner.
+
+You can experiment with these with the command-line version of the
+module, too:
+
+```
+% python3 -m starvote -v BLOC_STAR -w 2 sample_polls/starvote_ballots_dd1wc4yx_20230520050413.csv
+```
+
+
 ## Limitations
 
-Currently this module only supports single-winner STAR voting;
-variants such as
-[Bloc STAR](https://www.starvoting.org/multi_winner) and
-[Proportional STAR](https://www.starvoting.org/star-pr)
+Currently this module only supports single-winner STAR voting
+and the [Bloc STAR](https://www.starvoting.org/multi_winner)
+variant.  [Proportional STAR](https://www.starvoting.org/star-pr)
 (aka [Allocated Score](https://electowiki.org/wiki/Allocated_Score))
-are not yet supported.
+is not yet supported.
 
 ## License
 
 **starvote** is licensed using the
 [MIT license.](https://opensource.org/license/mit/)
 See the `LICENSE` file.
 
 The source code repository includes sample ballots downloaded from
 [https://star.vote/](https://star.vote/).  The licensing of these
 sample ballots is unclear, but they're assumed to be public-domain
 or otherwise freely redistributable.
 
 ## Changelog
 
+**1.2** *under development*
+
+* Add support for [Bloc STAR](https://www.starvoting.org/multi_winner)
+  polls.
+
+  * Added `PollVariant` enum.
+  * Added `variant` and `winners` parameters to `Poll`.
+
+* Add the list of tied candidates to the `UnbreakableTieError`
+  exception as the new `candidates` attribute.
+
 **1.1** 2023/05/20
 
 * Bugfix: raise `UnbreakableTieError` if there's a three-way
   tie for *second* place.  Previously **starvote** only noticed
   if there was a three-way tie for *first* place.
 * Added sample output for every sample poll in `sample_polls/`.
   These outputs have been confirmed correct by inspection, and
   could in the future be used as part of an automated test suite.
 
 **1.0** 2023/05/20
 
-Initial release.
+* Initial release.
```

### Comparing `starvote-1.1/sample_polls/starvote_ballots_4tyx27ks_20230520050434.csv` & `starvote-1.2/sample_polls/starvote_ballots_4tyx27ks_20230520050434.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.1/sample_polls/starvote_ballots_4tyx27ks_20230520050434.result.txt` & `starvote-1.2/sample_polls/starvote_ballots_4tyx27ks_20230520050434.result.txt`

 * *Files identical despite different names*

### Comparing `starvote-1.1/sample_polls/starvote_ballots_9fm5fp2c_20230520033518.csv` & `starvote-1.2/sample_polls/starvote_ballots_9fm5fp2c_20230520033518.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.1/sample_polls/starvote_ballots_9fm5fp2c_20230520033518.result.txt` & `starvote-1.2/sample_polls/starvote_ballots_9fm5fp2c_20230520033518.result.txt`

 * *Files identical despite different names*

### Comparing `starvote-1.1/sample_polls/starvote_ballots_9mm3519w_20230520050438.csv` & `starvote-1.2/sample_polls/starvote_ballots_9mm3519w_20230520050438.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.1/sample_polls/starvote_ballots_9xrw9wch_20230520050429.csv` & `starvote-1.2/sample_polls/starvote_ballots_9xrw9wch_20230520050429.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.1/sample_polls/starvote_ballots_9xrw9wch_20230520050429.result.txt` & `starvote-1.2/sample_polls/starvote_ballots_9xrw9wch_20230520050429.result.txt`

 * *Files identical despite different names*

### Comparing `starvote-1.1/sample_polls/starvote_ballots_dd1wc4yx_20230520050413.csv` & `starvote-1.2/sample_polls/starvote_ballots_dd1wc4yx_20230520050413.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.1/sample_polls/starvote_ballots_dd1wc4yx_20230520050413.result.txt` & `starvote-1.2/sample_polls/starvote_ballots_dd1wc4yx_20230520050413.result.txt`

 * *Files identical despite different names*

### Comparing `starvote-1.1/sample_polls/starvote_ballots_eh3cxxz7_20230520033403.csv` & `starvote-1.2/sample_polls/starvote_ballots_eh3cxxz7_20230520033403.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.1/sample_polls/starvote_ballots_eh3cxxz7_20230520033403.result.txt` & `starvote-1.2/sample_polls/starvote_ballots_eh3cxxz7_20230520033403.result.txt`

 * *Files identical despite different names*

### Comparing `starvote-1.1/sample_polls/starvote_ballots_p4rs6xn4_20230520050419.csv` & `starvote-1.2/sample_polls/starvote_ballots_p4rs6xn4_20230520050419.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.1/sample_polls/starvote_ballots_p4rs6xn4_20230520050419.result.txt` & `starvote-1.2/sample_polls/starvote_ballots_p4rs6xn4_20230520050419.result.txt`

 * *Files identical despite different names*

### Comparing `starvote-1.1/sample_polls/starvote_ballots_pf69snyx_20230520050425.csv` & `starvote-1.2/sample_polls/starvote_ballots_pf69snyx_20230520050425.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.1/sample_polls/starvote_ballots_swzw2ts6_20230520050422.csv` & `starvote-1.2/sample_polls/starvote_ballots_swzw2ts6_20230520050422.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.1/PKG-INFO` & `starvote-1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starvote
-Version: 1.1
+Version: 1.2
 Summary: A simple STAR vote tabulator
 Author-email: Larry Hastings <larry@hastings.org>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -26,16 +26,19 @@
 To use, `import starvote`, then instantiate a `starvote.Poll` object.
 Feed in the ballots using `poll.add_ballot(ballot)`; ballots are `dict` objects,
 mapping the candidate to the ballot's vote for the candidate
 (an `int` in the range 0 to 5 inclusive).
 
 Once you've added all the ballots, call `poll.result` to compute the winner.
 If there's an unbreakable tie, `poll.result` will raise an
-`UnbreakableTieError`.  The following scenarios can result in an
-unbreakable tie:
+`UnbreakableTieError`.  You can get a text description of the tie by calling
+`str` on the exception; also, you can get a list of the tied candidates
+in its `candidates` attribute.
+
+The following scenarios produce an unbreakable tie:
 
 * If the top two candidates tie during the automated runoff round
   *and* their scores are also a tie.
 * If the second and third candidates during the score round tie,
   and their preference scores are also a tie.
 * If three or more candiates are tied for first *or* second place
   during the score round.
@@ -80,47 +83,81 @@
 If the module is executed as a script, it will read a single
 [CSV file](https://en.wikipedia.org/wiki/Comma-separated_values)
 in [*star.vote*](https://star.vote/) format, tabulate, and print
 the result.  For example, you can run this from the root of the
 source-code repository:
 
 ```
-% python3 -m starvote sample_polls/sample_vote_automatic_runoff_breakable_tie.csv
+% python3 -m starvote sample_polls/sample_poll_automatic_runoff_breakable_tie.csv
 ```
 
 to see how **starvote** handles a tie during the automatic runoff round.
 
+## Multiple-winner elections
+
+**starvote** also implements the
+[Bloc STAR](https://www.starvoting.org/multi_winner)
+variant of STAR for multi-winner elections.  Simply
+instantiate your `Poll` object passing in `starvote.BLOC_STAR`
+for the `variant` parameter, and the number of winners in
+the `winners` keyword-only parameter:
+
+```Python
+poll = starvote.Poll(variant=starvote.BLOC_STAR, winners=2)
+```
+
+This changes `poll.result` to return a list of winners instead
+of a single winner.
+
+You can experiment with these with the command-line version of the
+module, too:
+
+```
+% python3 -m starvote -v BLOC_STAR -w 2 sample_polls/starvote_ballots_dd1wc4yx_20230520050413.csv
+```
+
+
 ## Limitations
 
-Currently this module only supports single-winner STAR voting;
-variants such as
-[Bloc STAR](https://www.starvoting.org/multi_winner) and
-[Proportional STAR](https://www.starvoting.org/star-pr)
+Currently this module only supports single-winner STAR voting
+and the [Bloc STAR](https://www.starvoting.org/multi_winner)
+variant.  [Proportional STAR](https://www.starvoting.org/star-pr)
 (aka [Allocated Score](https://electowiki.org/wiki/Allocated_Score))
-are not yet supported.
+is not yet supported.
 
 ## License
 
 **starvote** is licensed using the
 [MIT license.](https://opensource.org/license/mit/)
 See the `LICENSE` file.
 
 The source code repository includes sample ballots downloaded from
 [https://star.vote/](https://star.vote/).  The licensing of these
 sample ballots is unclear, but they're assumed to be public-domain
 or otherwise freely redistributable.
 
 ## Changelog
 
+**1.2** *under development*
+
+* Add support for [Bloc STAR](https://www.starvoting.org/multi_winner)
+  polls.
+
+  * Added `PollVariant` enum.
+  * Added `variant` and `winners` parameters to `Poll`.
+
+* Add the list of tied candidates to the `UnbreakableTieError`
+  exception as the new `candidates` attribute.
+
 **1.1** 2023/05/20
 
 * Bugfix: raise `UnbreakableTieError` if there's a three-way
   tie for *second* place.  Previously **starvote** only noticed
   if there was a three-way tie for *first* place.
 * Added sample output for every sample poll in `sample_polls/`.
   These outputs have been confirmed correct by inspection, and
   could in the future be used as part of an automated test suite.
 
 **1.0** 2023/05/20
 
-Initial release.
+* Initial release.
```

