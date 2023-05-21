# Comparing `tmp/starvote-1.2.tar.gz` & `tmp/starvote-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starvote-1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "starvote-1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `starvote-1.2.tar` & `starvote-1.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0       19 2023-05-20 12:58:10.568731 starvote-1.2/.gitignore
--rw-r--r--   0        0        0     1087 2023-05-20 12:48:55.372092 starvote-1.2/LICENSE
--rw-r--r--   0        0        0     4908 2023-05-21 01:24:41.056145 starvote-1.2/README.md
--rw-r--r--   0        0        0      267 2023-05-20 12:47:55.671593 starvote-1.2/example.py
--rw-r--r--   0        0        0      502 2023-05-20 12:55:16.755279 starvote-1.2/pyproject.toml
--rw-r--r--   0        0        0      307 2023-05-20 14:24:30.072047 starvote-1.2/sample_polls/README.md
--rw-r--r--   0        0        0      169 2023-05-20 12:17:24.308288 starvote-1.2/sample_polls/sample_poll_automatic_runoff_breakable_tie.csv
--rw-r--r--   0        0        0      314 2023-05-20 14:22:01.282802 starvote-1.2/sample_polls/sample_poll_automatic_runoff_breakable_tie.result.txt
--rw-r--r--   0        0        0      169 2023-05-20 12:16:12.379686 starvote-1.2/sample_polls/sample_poll_automatic_runoff_unbreakable_tie.csv
--rw-r--r--   0        0        0      382 2023-05-20 14:22:01.298802 starvote-1.2/sample_polls/sample_poll_automatic_runoff_unbreakable_tie.result.txt
--rw-r--r--   0        0        0      169 2023-05-20 12:27:44.977476 starvote-1.2/sample_polls/sample_poll_score_round_breakable_tie_between_second_and_third.csv
--rw-r--r--   0        0        0      333 2023-05-20 14:22:01.314803 starvote-1.2/sample_polls/sample_poll_score_round_breakable_tie_between_second_and_third.result.txt
--rw-r--r--   0        0        0      169 2023-05-20 12:14:18.630735 starvote-1.2/sample_polls/sample_poll_score_round_unbreakable_three_way_tie_for_first.csv
--rw-r--r--   0        0        0      198 2023-05-20 14:22:01.330803 starvote-1.2/sample_polls/sample_poll_score_round_unbreakable_three_way_tie_for_first.result.txt
--rw-r--r--   0        0        0      226 2023-05-20 14:20:22.817978 starvote-1.2/sample_polls/sample_poll_score_round_unbreakable_three_way_tie_for_second.csv
--rw-r--r--   0        0        0      231 2023-05-20 14:22:01.346803 starvote-1.2/sample_polls/sample_poll_score_round_unbreakable_three_way_tie_for_second.result.txt
--rw-r--r--   0        0        0      169 2023-05-20 12:30:43.458967 starvote-1.2/sample_polls/sample_poll_score_round_unbreakable_tie_between_second_and_third.csv
--rw-r--r--   0        0        0      346 2023-05-20 14:22:01.358803 starvote-1.2/sample_polls/sample_poll_score_round_unbreakable_tie_between_second_and_third.result.txt
--rw-r--r--   0        0        0    49711 2023-05-20 12:04:34.029848 starvote-1.2/sample_polls/starvote_ballots_4tyx27ks_20230520050434.csv
--rw-r--r--   0        0        0   538128 2023-05-20 14:33:25.560528 starvote-1.2/sample_polls/starvote_ballots_4tyx27ks_20230520050434.result.pdf
--rw-r--r--   0        0        0      869 2023-05-20 14:22:01.378803 starvote-1.2/sample_polls/starvote_ballots_4tyx27ks_20230520050434.result.txt
--rw-r--r--   0        0        0     1812 2023-05-20 10:35:18.365110 starvote-1.2/sample_polls/starvote_ballots_9fm5fp2c_20230520033518.csv
--rw-r--r--   0        0        0   807144 2023-05-20 14:33:51.120742 starvote-1.2/sample_polls/starvote_ballots_9fm5fp2c_20230520033518.result.pdf
--rw-r--r--   0        0        0     2411 2023-05-20 14:22:01.390803 starvote-1.2/sample_polls/starvote_ballots_9fm5fp2c_20230520033518.result.txt
--rw-r--r--   0        0        0    31534 2023-05-20 12:04:38.493885 starvote-1.2/sample_polls/starvote_ballots_9mm3519w_20230520050438.csv
--rw-r--r--   0        0        0   325033 2023-05-20 14:34:17.572963 starvote-1.2/sample_polls/starvote_ballots_9mm3519w_20230520050438.result.pdf
--rw-r--r--   0        0        0      401 2023-05-20 14:22:01.406803 starvote-1.2/sample_polls/starvote_ballots_9mm3519w_20230520050438.result.txt
--rw-r--r--   0        0        0    57750 2023-05-20 12:04:29.149807 starvote-1.2/sample_polls/starvote_ballots_9xrw9wch_20230520050429.csv
--rw-r--r--   0        0        0   575556 2023-05-20 14:35:00.177319 starvote-1.2/sample_polls/starvote_ballots_9xrw9wch_20230520050429.result.pdf
--rw-r--r--   0        0        0      954 2023-05-20 14:22:01.426803 starvote-1.2/sample_polls/starvote_ballots_9xrw9wch_20230520050429.result.txt
--rw-r--r--   0        0        0   123039 2023-05-20 12:04:13.781679 starvote-1.2/sample_polls/starvote_ballots_dd1wc4yx_20230520050413.csv
--rw-r--r--   0        0        0   584998 2023-05-20 14:35:22.465506 starvote-1.2/sample_polls/starvote_ballots_dd1wc4yx_20230520050413.result.pdf
--rw-r--r--   0        0        0      954 2023-05-20 14:22:01.446804 starvote-1.2/sample_polls/starvote_ballots_dd1wc4yx_20230520050413.result.txt
--rw-r--r--   0        0        0   250538 2023-05-20 10:34:04.044490 starvote-1.2/sample_polls/starvote_ballots_eh3cxxz7_20230520033403.csv
--rw-r--r--   0        0        0   643536 2023-05-20 14:35:41.153662 starvote-1.2/sample_polls/starvote_ballots_eh3cxxz7_20230520033403.result.pdf
--rw-r--r--   0        0        0     1084 2023-05-20 14:22:01.478804 starvote-1.2/sample_polls/starvote_ballots_eh3cxxz7_20230520033403.result.txt
--rw-r--r--   0        0        0   115109 2023-05-20 12:04:19.133723 starvote-1.2/sample_polls/starvote_ballots_p4rs6xn4_20230520050419.csv
--rw-r--r--   0        0        0   696161 2023-05-20 14:36:00.553825 starvote-1.2/sample_polls/starvote_ballots_p4rs6xn4_20230520050419.result.pdf
--rw-r--r--   0        0        0     2635 2023-05-20 14:22:01.502804 starvote-1.2/sample_polls/starvote_ballots_p4rs6xn4_20230520050419.result.txt
--rw-r--r--   0        0        0    48454 2023-05-20 12:04:25.689778 starvote-1.2/sample_polls/starvote_ballots_pf69snyx_20230520050425.csv
--rw-r--r--   0        0        0   360427 2023-05-20 14:36:25.050030 starvote-1.2/sample_polls/starvote_ballots_pf69snyx_20230520050425.result.pdf
--rw-r--r--   0        0        0      412 2023-05-20 14:22:01.522804 starvote-1.2/sample_polls/starvote_ballots_pf69snyx_20230520050425.result.txt
--rw-r--r--   0        0        0    52870 2023-05-20 12:04:22.533752 starvote-1.2/sample_polls/starvote_ballots_swzw2ts6_20230520050422.csv
--rw-r--r--   0        0        0   354740 2023-05-20 14:36:48.550226 starvote-1.2/sample_polls/starvote_ballots_swzw2ts6_20230520050422.result.pdf
--rw-r--r--   0        0        0      370 2023-05-20 14:22:01.538804 starvote-1.2/sample_polls/starvote_ballots_swzw2ts6_20230520050422.result.txt
--rw-r--r--   0        0        0     8492 2023-05-21 01:26:59.249223 starvote-1.2/starvote/__init__.py
--rw-r--r--   0        0        0     3368 2023-05-21 01:23:06.091404 starvote-1.2/starvote/__main__.py
--rw-r--r--   0        0        0     5326 1970-01-01 00:00:00.000000 starvote-1.2/PKG-INFO
+-rw-r--r--   0        0        0       19 2023-05-20 12:58:10.568731 starvote-1.3/.gitignore
+-rw-r--r--   0        0        0     1087 2023-05-20 12:48:55.372092 starvote-1.3/LICENSE
+-rw-r--r--   0        0        0     5912 2023-05-21 11:18:38.666936 starvote-1.3/README.md
+-rw-r--r--   0        0        0      267 2023-05-20 12:47:55.671593 starvote-1.3/example.py
+-rw-r--r--   0        0        0      502 2023-05-20 12:55:16.755279 starvote-1.3/pyproject.toml
+-rw-r--r--   0        0        0      406 2023-05-21 11:19:31.211412 starvote-1.3/sample_polls/README.md
+-rw-r--r--   0        0        0      169 2023-05-20 12:17:24.308288 starvote-1.3/sample_polls/sample_poll_automatic_runoff_breakable_tie.csv
+-rw-r--r--   0        0        0      314 2023-05-21 11:03:10.562528 starvote-1.3/sample_polls/sample_poll_automatic_runoff_breakable_tie.result.txt
+-rw-r--r--   0        0        0      169 2023-05-20 12:16:12.379686 starvote-1.3/sample_polls/sample_poll_automatic_runoff_unbreakable_tie.csv
+-rw-r--r--   0        0        0      405 2023-05-21 11:03:10.578528 starvote-1.3/sample_polls/sample_poll_automatic_runoff_unbreakable_tie.result.txt
+-rw-r--r--   0        0        0      169 2023-05-20 12:27:44.977476 starvote-1.3/sample_polls/sample_poll_score_round_breakable_tie_between_second_and_third.csv
+-rw-r--r--   0        0        0      333 2023-05-21 11:03:10.594529 starvote-1.3/sample_polls/sample_poll_score_round_breakable_tie_between_second_and_third.result.txt
+-rw-r--r--   0        0        0      169 2023-05-20 12:14:18.630735 starvote-1.3/sample_polls/sample_poll_score_round_unbreakable_three_way_tie_for_first.csv
+-rw-r--r--   0        0        0      227 2023-05-21 11:03:10.610529 starvote-1.3/sample_polls/sample_poll_score_round_unbreakable_three_way_tie_for_first.result.txt
+-rw-r--r--   0        0        0      226 2023-05-20 14:20:22.817978 starvote-1.3/sample_polls/sample_poll_score_round_unbreakable_three_way_tie_for_second.csv
+-rw-r--r--   0        0        0      260 2023-05-21 11:03:10.622529 starvote-1.3/sample_polls/sample_poll_score_round_unbreakable_three_way_tie_for_second.result.txt
+-rw-r--r--   0        0        0      169 2023-05-20 12:30:43.458967 starvote-1.3/sample_polls/sample_poll_score_round_unbreakable_tie_between_second_and_third.csv
+-rw-r--r--   0        0        0      367 2023-05-21 11:03:10.638529 starvote-1.3/sample_polls/sample_poll_score_round_unbreakable_tie_between_second_and_third.result.txt
+-rw-r--r--   0        0        0    49711 2023-05-20 12:04:34.029848 starvote-1.3/sample_polls/starvote_ballots_4tyx27ks_20230520050434.csv
+-rw-r--r--   0        0        0   538128 2023-05-20 14:33:25.560528 starvote-1.3/sample_polls/starvote_ballots_4tyx27ks_20230520050434.result.pdf
+-rw-r--r--   0        0        0      869 2023-05-21 11:03:10.654529 starvote-1.3/sample_polls/starvote_ballots_4tyx27ks_20230520050434.result.txt
+-rw-r--r--   0        0        0     1812 2023-05-20 10:35:18.365110 starvote-1.3/sample_polls/starvote_ballots_9fm5fp2c_20230520033518.csv
+-rw-r--r--   0        0        0   807144 2023-05-20 14:33:51.120742 starvote-1.3/sample_polls/starvote_ballots_9fm5fp2c_20230520033518.result.pdf
+-rw-r--r--   0        0        0     2411 2023-05-21 11:03:10.670529 starvote-1.3/sample_polls/starvote_ballots_9fm5fp2c_20230520033518.result.txt
+-rw-r--r--   0        0        0    31534 2023-05-20 12:04:38.493885 starvote-1.3/sample_polls/starvote_ballots_9mm3519w_20230520050438.csv
+-rw-r--r--   0        0        0   325033 2023-05-20 14:34:17.572963 starvote-1.3/sample_polls/starvote_ballots_9mm3519w_20230520050438.result.pdf
+-rw-r--r--   0        0        0      401 2023-05-21 11:03:10.686529 starvote-1.3/sample_polls/starvote_ballots_9mm3519w_20230520050438.result.txt
+-rw-r--r--   0        0        0    57750 2023-05-20 12:04:29.149807 starvote-1.3/sample_polls/starvote_ballots_9xrw9wch_20230520050429.csv
+-rw-r--r--   0        0        0   575556 2023-05-20 14:35:00.177319 starvote-1.3/sample_polls/starvote_ballots_9xrw9wch_20230520050429.result.pdf
+-rw-r--r--   0        0        0      954 2023-05-21 11:03:10.706529 starvote-1.3/sample_polls/starvote_ballots_9xrw9wch_20230520050429.result.txt
+-rw-r--r--   0        0        0   123039 2023-05-20 12:04:13.781679 starvote-1.3/sample_polls/starvote_ballots_dd1wc4yx_20230520050413.csv
+-rw-r--r--   0        0        0   584998 2023-05-20 14:35:22.465506 starvote-1.3/sample_polls/starvote_ballots_dd1wc4yx_20230520050413.result.pdf
+-rw-r--r--   0        0        0      954 2023-05-21 11:03:10.730530 starvote-1.3/sample_polls/starvote_ballots_dd1wc4yx_20230520050413.result.txt
+-rw-r--r--   0        0        0   250538 2023-05-20 10:34:04.044490 starvote-1.3/sample_polls/starvote_ballots_eh3cxxz7_20230520033403.csv
+-rw-r--r--   0        0        0   643536 2023-05-20 14:35:41.153662 starvote-1.3/sample_polls/starvote_ballots_eh3cxxz7_20230520033403.result.pdf
+-rw-r--r--   0        0        0     1084 2023-05-21 11:03:10.766530 starvote-1.3/sample_polls/starvote_ballots_eh3cxxz7_20230520033403.result.txt
+-rw-r--r--   0        0        0   115109 2023-05-20 12:04:19.133723 starvote-1.3/sample_polls/starvote_ballots_p4rs6xn4_20230520050419.csv
+-rw-r--r--   0        0        0   696161 2023-05-20 14:36:00.553825 starvote-1.3/sample_polls/starvote_ballots_p4rs6xn4_20230520050419.result.pdf
+-rw-r--r--   0        0        0     2635 2023-05-21 11:03:10.790530 starvote-1.3/sample_polls/starvote_ballots_p4rs6xn4_20230520050419.result.txt
+-rw-r--r--   0        0        0    48454 2023-05-20 12:04:25.689778 starvote-1.3/sample_polls/starvote_ballots_pf69snyx_20230520050425.csv
+-rw-r--r--   0        0        0   360427 2023-05-20 14:36:25.050030 starvote-1.3/sample_polls/starvote_ballots_pf69snyx_20230520050425.result.pdf
+-rw-r--r--   0        0        0      412 2023-05-21 11:03:10.810531 starvote-1.3/sample_polls/starvote_ballots_pf69snyx_20230520050425.result.txt
+-rw-r--r--   0        0        0    52870 2023-05-20 12:04:22.533752 starvote-1.3/sample_polls/starvote_ballots_swzw2ts6_20230520050422.csv
+-rw-r--r--   0        0        0   354740 2023-05-20 14:36:48.550226 starvote-1.3/sample_polls/starvote_ballots_swzw2ts6_20230520050422.result.pdf
+-rw-r--r--   0        0        0      370 2023-05-21 11:03:10.826531 starvote-1.3/sample_polls/starvote_ballots_swzw2ts6_20230520050422.result.txt
+-rw-r--r--   0        0        0    14350 2023-05-21 11:20:17.435830 starvote-1.3/starvote/__init__.py
+-rw-r--r--   0        0        0     3412 2023-05-21 09:40:03.331105 starvote-1.3/starvote/__main__.py
+-rw-r--r--   0        0        0     6330 1970-01-01 00:00:00.000000 starvote-1.3/PKG-INFO
```

### Comparing `starvote-1.2/LICENSE` & `starvote-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `starvote-1.2/README.md` & `starvote-1.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -80,71 +80,93 @@
 
 to see how **starvote** handles a tie during the automatic runoff round.
 
 ## Multiple-winner elections
 
 **starvote** also implements the
 [Bloc STAR](https://www.starvoting.org/multi_winner)
-variant of STAR for multi-winner elections.  Simply
-instantiate your `Poll` object passing in `starvote.BLOC_STAR`
-for the `variant` parameter, and the number of winners in
-the `winners` keyword-only parameter:
+and
+[Proportional STAR](https://www.starvoting.org/star-pr)
+(aka [Allocated Score](https://electowiki.org/wiki/Allocated_Score))
+variants of STAR for multi-winner elections.  Simply
+instantiate your `Poll` object passing in the enum constant
+`starvote.BLOC_STAR` or `starvote.Proportional_STAR`
+for the `variant` parameter, and the number of seats in
+the `seats` keyword-only parameter:
 
 ```Python
-poll = starvote.Poll(variant=starvote.BLOC_STAR, winners=2)
+poll = starvote.Poll(variant=starvote.BLOC_STAR, seats=2)
 ```
 
 This changes `poll.result` to return a list of winners instead
 of a single winner.
 
 You can experiment with these with the command-line version of the
-module, too:
+module, too.  You can specify the variant with `-v` and the
+number of seats with `-s`:
 
 ```
-% python3 -m starvote -v BLOC_STAR -w 2 sample_polls/starvote_ballots_dd1wc4yx_20230520050413.csv
+% python3 -m starvote -v BLOC_STAR -s 2 sample_polls/starvote_ballots_dd1wc4yx_20230520050413.csv
 ```
 
+### Warning
 
-## Limitations
-
-Currently this module only supports single-winner STAR voting
-and the [Bloc STAR](https://www.starvoting.org/multi_winner)
-variant.  [Proportional STAR](https://www.starvoting.org/star-pr)
-(aka [Allocated Score](https://electowiki.org/wiki/Allocated_Score))
-is not yet supported.
+I haven't found a test corpus for either of these voting methods.
+I'm following the rules, as best I can, and the results I'm getting
+make sense.  But, so far, my implementations of BLOC STAR
+and Proportional STAR definitely could be wrong.
 
 ## License
 
 **starvote** is licensed using the
 [MIT license.](https://opensource.org/license/mit/)
 See the `LICENSE` file.
 
+It seems particularly relevant to repeat here:
+*there is no warranty for this software.*
+I've done the best job I can implementing this election system
+tabulator.  But this software could have bugs,
+or my understanding of the rules could be wrong,
+and either of these could affect the results of elections
+you run with this software.
+**Use at your own risk.**
+
 The source code repository includes sample ballots downloaded from
 [https://star.vote/](https://star.vote/).  The licensing of these
 sample ballots is unclear, but they're assumed to be public-domain
 or otherwise freely redistributable.
 
 ## Changelog
 
-**1.2** *under development*
+**1.3** *2023/05/21*
+
+* Added support for
+  [Proportional STAR](https://www.starvoting.org/star-pr)
+  polls.  The only visible external change is the new
+  `Proportional_STAR` enum value.
+* Renamed the `winners` parameter on the `Poll` constructor to `seats`.
+  Sorry to break your code, all zero people planetwide who already started
+  using the parameter!  But this new name is a big improvement.
+
+**1.2** *2023/05/20*
 
 * Add support for [Bloc STAR](https://www.starvoting.org/multi_winner)
-  polls.
+  polls:
 
-  * Added `PollVariant` enum.
+  * Added `PollVariant` enum containing `STAR` and `BLOC_STAR` values.
   * Added `variant` and `winners` parameters to `Poll`.
 
 * Add the list of tied candidates to the `UnbreakableTieError`
   exception as the new `candidates` attribute.
 
-**1.1** 2023/05/20
+**1.1** *2023/05/20*
 
 * Bugfix: raise `UnbreakableTieError` if there's a three-way
   tie for *second* place.  Previously **starvote** only noticed
   if there was a three-way tie for *first* place.
 * Added sample output for every sample poll in `sample_polls/`.
   These outputs have been confirmed correct by inspection, and
   could in the future be used as part of an automated test suite.
 
-**1.0** 2023/05/20
+**1.0** *2023/05/20*
 
 * Initial release.
```

### Comparing `starvote-1.2/sample_polls/starvote_ballots_4tyx27ks_20230520050434.csv` & `starvote-1.3/sample_polls/starvote_ballots_4tyx27ks_20230520050434.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.2/sample_polls/starvote_ballots_4tyx27ks_20230520050434.result.pdf` & `starvote-1.3/sample_polls/starvote_ballots_4tyx27ks_20230520050434.result.pdf`

 * *Files identical despite different names*

### Comparing `starvote-1.2/sample_polls/starvote_ballots_4tyx27ks_20230520050434.result.txt` & `starvote-1.3/sample_polls/starvote_ballots_4tyx27ks_20230520050434.result.txt`

 * *Files identical despite different names*

### Comparing `starvote-1.2/sample_polls/starvote_ballots_9fm5fp2c_20230520033518.csv` & `starvote-1.3/sample_polls/starvote_ballots_9fm5fp2c_20230520033518.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.2/sample_polls/starvote_ballots_9fm5fp2c_20230520033518.result.pdf` & `starvote-1.3/sample_polls/starvote_ballots_9fm5fp2c_20230520033518.result.pdf`

 * *Files identical despite different names*

### Comparing `starvote-1.2/sample_polls/starvote_ballots_9fm5fp2c_20230520033518.result.txt` & `starvote-1.3/sample_polls/starvote_ballots_9fm5fp2c_20230520033518.result.txt`

 * *Files identical despite different names*

### Comparing `starvote-1.2/sample_polls/starvote_ballots_9mm3519w_20230520050438.csv` & `starvote-1.3/sample_polls/starvote_ballots_9mm3519w_20230520050438.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.2/sample_polls/starvote_ballots_9mm3519w_20230520050438.result.pdf` & `starvote-1.3/sample_polls/starvote_ballots_9mm3519w_20230520050438.result.pdf`

 * *Files identical despite different names*

### Comparing `starvote-1.2/sample_polls/starvote_ballots_9xrw9wch_20230520050429.csv` & `starvote-1.3/sample_polls/starvote_ballots_9xrw9wch_20230520050429.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.2/sample_polls/starvote_ballots_9xrw9wch_20230520050429.result.pdf` & `starvote-1.3/sample_polls/starvote_ballots_9xrw9wch_20230520050429.result.pdf`

 * *Files identical despite different names*

### Comparing `starvote-1.2/sample_polls/starvote_ballots_9xrw9wch_20230520050429.result.txt` & `starvote-1.3/sample_polls/starvote_ballots_9xrw9wch_20230520050429.result.txt`

 * *Files identical despite different names*

### Comparing `starvote-1.2/sample_polls/starvote_ballots_dd1wc4yx_20230520050413.csv` & `starvote-1.3/sample_polls/starvote_ballots_dd1wc4yx_20230520050413.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.2/sample_polls/starvote_ballots_dd1wc4yx_20230520050413.result.pdf` & `starvote-1.3/sample_polls/starvote_ballots_dd1wc4yx_20230520050413.result.pdf`

 * *Files identical despite different names*

### Comparing `starvote-1.2/sample_polls/starvote_ballots_dd1wc4yx_20230520050413.result.txt` & `starvote-1.3/sample_polls/starvote_ballots_dd1wc4yx_20230520050413.result.txt`

 * *Files identical despite different names*

### Comparing `starvote-1.2/sample_polls/starvote_ballots_eh3cxxz7_20230520033403.csv` & `starvote-1.3/sample_polls/starvote_ballots_eh3cxxz7_20230520033403.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.2/sample_polls/starvote_ballots_eh3cxxz7_20230520033403.result.pdf` & `starvote-1.3/sample_polls/starvote_ballots_eh3cxxz7_20230520033403.result.pdf`

 * *Files identical despite different names*

### Comparing `starvote-1.2/sample_polls/starvote_ballots_eh3cxxz7_20230520033403.result.txt` & `starvote-1.3/sample_polls/starvote_ballots_eh3cxxz7_20230520033403.result.txt`

 * *Files identical despite different names*

### Comparing `starvote-1.2/sample_polls/starvote_ballots_p4rs6xn4_20230520050419.csv` & `starvote-1.3/sample_polls/starvote_ballots_p4rs6xn4_20230520050419.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.2/sample_polls/starvote_ballots_p4rs6xn4_20230520050419.result.pdf` & `starvote-1.3/sample_polls/starvote_ballots_p4rs6xn4_20230520050419.result.pdf`

 * *Files identical despite different names*

### Comparing `starvote-1.2/sample_polls/starvote_ballots_p4rs6xn4_20230520050419.result.txt` & `starvote-1.3/sample_polls/starvote_ballots_p4rs6xn4_20230520050419.result.txt`

 * *Files identical despite different names*

### Comparing `starvote-1.2/sample_polls/starvote_ballots_pf69snyx_20230520050425.csv` & `starvote-1.3/sample_polls/starvote_ballots_pf69snyx_20230520050425.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.2/sample_polls/starvote_ballots_pf69snyx_20230520050425.result.pdf` & `starvote-1.3/sample_polls/starvote_ballots_pf69snyx_20230520050425.result.pdf`

 * *Files identical despite different names*

### Comparing `starvote-1.2/sample_polls/starvote_ballots_swzw2ts6_20230520050422.csv` & `starvote-1.3/sample_polls/starvote_ballots_swzw2ts6_20230520050422.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.2/sample_polls/starvote_ballots_swzw2ts6_20230520050422.result.pdf` & `starvote-1.3/sample_polls/starvote_ballots_swzw2ts6_20230520050422.result.pdf`

 * *Files identical despite different names*

### Comparing `starvote-1.2/PKG-INFO` & `starvote-1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starvote
-Version: 1.2
+Version: 1.3
 Summary: A simple STAR vote tabulator
 Author-email: Larry Hastings <larry@hastings.org>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -92,72 +92,94 @@
 
 to see how **starvote** handles a tie during the automatic runoff round.
 
 ## Multiple-winner elections
 
 **starvote** also implements the
 [Bloc STAR](https://www.starvoting.org/multi_winner)
-variant of STAR for multi-winner elections.  Simply
-instantiate your `Poll` object passing in `starvote.BLOC_STAR`
-for the `variant` parameter, and the number of winners in
-the `winners` keyword-only parameter:
+and
+[Proportional STAR](https://www.starvoting.org/star-pr)
+(aka [Allocated Score](https://electowiki.org/wiki/Allocated_Score))
+variants of STAR for multi-winner elections.  Simply
+instantiate your `Poll` object passing in the enum constant
+`starvote.BLOC_STAR` or `starvote.Proportional_STAR`
+for the `variant` parameter, and the number of seats in
+the `seats` keyword-only parameter:
 
 ```Python
-poll = starvote.Poll(variant=starvote.BLOC_STAR, winners=2)
+poll = starvote.Poll(variant=starvote.BLOC_STAR, seats=2)
 ```
 
 This changes `poll.result` to return a list of winners instead
 of a single winner.
 
 You can experiment with these with the command-line version of the
-module, too:
+module, too.  You can specify the variant with `-v` and the
+number of seats with `-s`:
 
 ```
-% python3 -m starvote -v BLOC_STAR -w 2 sample_polls/starvote_ballots_dd1wc4yx_20230520050413.csv
+% python3 -m starvote -v BLOC_STAR -s 2 sample_polls/starvote_ballots_dd1wc4yx_20230520050413.csv
 ```
 
+### Warning
 
-## Limitations
-
-Currently this module only supports single-winner STAR voting
-and the [Bloc STAR](https://www.starvoting.org/multi_winner)
-variant.  [Proportional STAR](https://www.starvoting.org/star-pr)
-(aka [Allocated Score](https://electowiki.org/wiki/Allocated_Score))
-is not yet supported.
+I haven't found a test corpus for either of these voting methods.
+I'm following the rules, as best I can, and the results I'm getting
+make sense.  But, so far, my implementations of BLOC STAR
+and Proportional STAR definitely could be wrong.
 
 ## License
 
 **starvote** is licensed using the
 [MIT license.](https://opensource.org/license/mit/)
 See the `LICENSE` file.
 
+It seems particularly relevant to repeat here:
+*there is no warranty for this software.*
+I've done the best job I can implementing this election system
+tabulator.  But this software could have bugs,
+or my understanding of the rules could be wrong,
+and either of these could affect the results of elections
+you run with this software.
+**Use at your own risk.**
+
 The source code repository includes sample ballots downloaded from
 [https://star.vote/](https://star.vote/).  The licensing of these
 sample ballots is unclear, but they're assumed to be public-domain
 or otherwise freely redistributable.
 
 ## Changelog
 
-**1.2** *under development*
+**1.3** *2023/05/21*
+
+* Added support for
+  [Proportional STAR](https://www.starvoting.org/star-pr)
+  polls.  The only visible external change is the new
+  `Proportional_STAR` enum value.
+* Renamed the `winners` parameter on the `Poll` constructor to `seats`.
+  Sorry to break your code, all zero people planetwide who already started
+  using the parameter!  But this new name is a big improvement.
+
+**1.2** *2023/05/20*
 
 * Add support for [Bloc STAR](https://www.starvoting.org/multi_winner)
-  polls.
+  polls:
 
-  * Added `PollVariant` enum.
+  * Added `PollVariant` enum containing `STAR` and `BLOC_STAR` values.
   * Added `variant` and `winners` parameters to `Poll`.
 
 * Add the list of tied candidates to the `UnbreakableTieError`
   exception as the new `candidates` attribute.
 
-**1.1** 2023/05/20
+**1.1** *2023/05/20*
 
 * Bugfix: raise `UnbreakableTieError` if there's a three-way
   tie for *second* place.  Previously **starvote** only noticed
   if there was a three-way tie for *first* place.
 * Added sample output for every sample poll in `sample_polls/`.
   These outputs have been confirmed correct by inspection, and
   could in the future be used as part of an automated test suite.
 
-**1.0** 2023/05/20
+**1.0** *2023/05/20*
 
 * Initial release.
```

