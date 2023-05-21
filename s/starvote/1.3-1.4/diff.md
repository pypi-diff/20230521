# Comparing `tmp/starvote-1.3.tar.gz` & `tmp/starvote-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starvote-1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "starvote-1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `starvote-1.3.tar` & `starvote-1.4.tar`

### file list

```diff
@@ -1,48 +1,53 @@
--rw-r--r--   0        0        0       19 2023-05-20 12:58:10.568731 starvote-1.3/.gitignore
--rw-r--r--   0        0        0     1087 2023-05-20 12:48:55.372092 starvote-1.3/LICENSE
--rw-r--r--   0        0        0     5912 2023-05-21 11:18:38.666936 starvote-1.3/README.md
--rw-r--r--   0        0        0      267 2023-05-20 12:47:55.671593 starvote-1.3/example.py
--rw-r--r--   0        0        0      502 2023-05-20 12:55:16.755279 starvote-1.3/pyproject.toml
--rw-r--r--   0        0        0      406 2023-05-21 11:19:31.211412 starvote-1.3/sample_polls/README.md
--rw-r--r--   0        0        0      169 2023-05-20 12:17:24.308288 starvote-1.3/sample_polls/sample_poll_automatic_runoff_breakable_tie.csv
--rw-r--r--   0        0        0      314 2023-05-21 11:03:10.562528 starvote-1.3/sample_polls/sample_poll_automatic_runoff_breakable_tie.result.txt
--rw-r--r--   0        0        0      169 2023-05-20 12:16:12.379686 starvote-1.3/sample_polls/sample_poll_automatic_runoff_unbreakable_tie.csv
--rw-r--r--   0        0        0      405 2023-05-21 11:03:10.578528 starvote-1.3/sample_polls/sample_poll_automatic_runoff_unbreakable_tie.result.txt
--rw-r--r--   0        0        0      169 2023-05-20 12:27:44.977476 starvote-1.3/sample_polls/sample_poll_score_round_breakable_tie_between_second_and_third.csv
--rw-r--r--   0        0        0      333 2023-05-21 11:03:10.594529 starvote-1.3/sample_polls/sample_poll_score_round_breakable_tie_between_second_and_third.result.txt
--rw-r--r--   0        0        0      169 2023-05-20 12:14:18.630735 starvote-1.3/sample_polls/sample_poll_score_round_unbreakable_three_way_tie_for_first.csv
--rw-r--r--   0        0        0      227 2023-05-21 11:03:10.610529 starvote-1.3/sample_polls/sample_poll_score_round_unbreakable_three_way_tie_for_first.result.txt
--rw-r--r--   0        0        0      226 2023-05-20 14:20:22.817978 starvote-1.3/sample_polls/sample_poll_score_round_unbreakable_three_way_tie_for_second.csv
--rw-r--r--   0        0        0      260 2023-05-21 11:03:10.622529 starvote-1.3/sample_polls/sample_poll_score_round_unbreakable_three_way_tie_for_second.result.txt
--rw-r--r--   0        0        0      169 2023-05-20 12:30:43.458967 starvote-1.3/sample_polls/sample_poll_score_round_unbreakable_tie_between_second_and_third.csv
--rw-r--r--   0        0        0      367 2023-05-21 11:03:10.638529 starvote-1.3/sample_polls/sample_poll_score_round_unbreakable_tie_between_second_and_third.result.txt
--rw-r--r--   0        0        0    49711 2023-05-20 12:04:34.029848 starvote-1.3/sample_polls/starvote_ballots_4tyx27ks_20230520050434.csv
--rw-r--r--   0        0        0   538128 2023-05-20 14:33:25.560528 starvote-1.3/sample_polls/starvote_ballots_4tyx27ks_20230520050434.result.pdf
--rw-r--r--   0        0        0      869 2023-05-21 11:03:10.654529 starvote-1.3/sample_polls/starvote_ballots_4tyx27ks_20230520050434.result.txt
--rw-r--r--   0        0        0     1812 2023-05-20 10:35:18.365110 starvote-1.3/sample_polls/starvote_ballots_9fm5fp2c_20230520033518.csv
--rw-r--r--   0        0        0   807144 2023-05-20 14:33:51.120742 starvote-1.3/sample_polls/starvote_ballots_9fm5fp2c_20230520033518.result.pdf
--rw-r--r--   0        0        0     2411 2023-05-21 11:03:10.670529 starvote-1.3/sample_polls/starvote_ballots_9fm5fp2c_20230520033518.result.txt
--rw-r--r--   0        0        0    31534 2023-05-20 12:04:38.493885 starvote-1.3/sample_polls/starvote_ballots_9mm3519w_20230520050438.csv
--rw-r--r--   0        0        0   325033 2023-05-20 14:34:17.572963 starvote-1.3/sample_polls/starvote_ballots_9mm3519w_20230520050438.result.pdf
--rw-r--r--   0        0        0      401 2023-05-21 11:03:10.686529 starvote-1.3/sample_polls/starvote_ballots_9mm3519w_20230520050438.result.txt
--rw-r--r--   0        0        0    57750 2023-05-20 12:04:29.149807 starvote-1.3/sample_polls/starvote_ballots_9xrw9wch_20230520050429.csv
--rw-r--r--   0        0        0   575556 2023-05-20 14:35:00.177319 starvote-1.3/sample_polls/starvote_ballots_9xrw9wch_20230520050429.result.pdf
--rw-r--r--   0        0        0      954 2023-05-21 11:03:10.706529 starvote-1.3/sample_polls/starvote_ballots_9xrw9wch_20230520050429.result.txt
--rw-r--r--   0        0        0   123039 2023-05-20 12:04:13.781679 starvote-1.3/sample_polls/starvote_ballots_dd1wc4yx_20230520050413.csv
--rw-r--r--   0        0        0   584998 2023-05-20 14:35:22.465506 starvote-1.3/sample_polls/starvote_ballots_dd1wc4yx_20230520050413.result.pdf
--rw-r--r--   0        0        0      954 2023-05-21 11:03:10.730530 starvote-1.3/sample_polls/starvote_ballots_dd1wc4yx_20230520050413.result.txt
--rw-r--r--   0        0        0   250538 2023-05-20 10:34:04.044490 starvote-1.3/sample_polls/starvote_ballots_eh3cxxz7_20230520033403.csv
--rw-r--r--   0        0        0   643536 2023-05-20 14:35:41.153662 starvote-1.3/sample_polls/starvote_ballots_eh3cxxz7_20230520033403.result.pdf
--rw-r--r--   0        0        0     1084 2023-05-21 11:03:10.766530 starvote-1.3/sample_polls/starvote_ballots_eh3cxxz7_20230520033403.result.txt
--rw-r--r--   0        0        0   115109 2023-05-20 12:04:19.133723 starvote-1.3/sample_polls/starvote_ballots_p4rs6xn4_20230520050419.csv
--rw-r--r--   0        0        0   696161 2023-05-20 14:36:00.553825 starvote-1.3/sample_polls/starvote_ballots_p4rs6xn4_20230520050419.result.pdf
--rw-r--r--   0        0        0     2635 2023-05-21 11:03:10.790530 starvote-1.3/sample_polls/starvote_ballots_p4rs6xn4_20230520050419.result.txt
--rw-r--r--   0        0        0    48454 2023-05-20 12:04:25.689778 starvote-1.3/sample_polls/starvote_ballots_pf69snyx_20230520050425.csv
--rw-r--r--   0        0        0   360427 2023-05-20 14:36:25.050030 starvote-1.3/sample_polls/starvote_ballots_pf69snyx_20230520050425.result.pdf
--rw-r--r--   0        0        0      412 2023-05-21 11:03:10.810531 starvote-1.3/sample_polls/starvote_ballots_pf69snyx_20230520050425.result.txt
--rw-r--r--   0        0        0    52870 2023-05-20 12:04:22.533752 starvote-1.3/sample_polls/starvote_ballots_swzw2ts6_20230520050422.csv
--rw-r--r--   0        0        0   354740 2023-05-20 14:36:48.550226 starvote-1.3/sample_polls/starvote_ballots_swzw2ts6_20230520050422.result.pdf
--rw-r--r--   0        0        0      370 2023-05-21 11:03:10.826531 starvote-1.3/sample_polls/starvote_ballots_swzw2ts6_20230520050422.result.txt
--rw-r--r--   0        0        0    14350 2023-05-21 11:20:17.435830 starvote-1.3/starvote/__init__.py
--rw-r--r--   0        0        0     3412 2023-05-21 09:40:03.331105 starvote-1.3/starvote/__main__.py
--rw-r--r--   0        0        0     6330 1970-01-01 00:00:00.000000 starvote-1.3/PKG-INFO
+-rw-r--r--   0        0        0       19 2023-05-20 12:58:10.568731 starvote-1.4/.gitignore
+-rw-r--r--   0        0        0     1087 2023-05-20 12:48:55.372092 starvote-1.4/LICENSE
+-rw-r--r--   0        0        0     6128 2023-05-21 14:47:52.514438 starvote-1.4/README.md
+-rw-r--r--   0        0        0      267 2023-05-20 12:47:55.671593 starvote-1.4/example.py
+-rw-r--r--   0        0        0      502 2023-05-20 12:55:16.755279 starvote-1.4/pyproject.toml
+-rw-r--r--   0        0        0      406 2023-05-21 11:19:31.211412 starvote-1.4/sample_polls/README.md
+-rw-r--r--   0        0        0      169 2023-05-20 12:17:24.308288 starvote-1.4/sample_polls/sample_poll_automatic_runoff_breakable_tie.csv
+-rw-r--r--   0        0        0      321 2023-05-21 14:36:07.812513 starvote-1.4/sample_polls/sample_poll_automatic_runoff_breakable_tie.result.txt
+-rw-r--r--   0        0        0      169 2023-05-20 12:16:12.379686 starvote-1.4/sample_polls/sample_poll_automatic_runoff_unbreakable_tie.csv
+-rw-r--r--   0        0        0      412 2023-05-21 14:36:10.524536 starvote-1.4/sample_polls/sample_poll_automatic_runoff_unbreakable_tie.result.txt
+-rw-r--r--   0        0        0      226 2023-05-21 13:55:36.270675 starvote-1.4/sample_polls/sample_poll_proportional_star_3_seats_breakable_tie.csv
+-rw-r--r--   0        0        0      883 2023-05-21 14:46:04.809533 starvote-1.4/sample_polls/sample_poll_proportional_star_3_seats_breakable_tie.result.txt
+-rw-r--r--   0        0        0      226 2023-05-21 13:52:36.109138 starvote-1.4/sample_polls/sample_poll_proportional_star_3_seats_unbreakable_tie.csv
+-rw-r--r--   0        0        0      390 2023-05-21 14:45:20.721162 starvote-1.4/sample_polls/sample_poll_proportional_star_3_seats_unbreakable_tie.result.txt
+-rw-r--r--   0        0        0      169 2023-05-20 12:27:44.977476 starvote-1.4/sample_polls/sample_poll_score_round_breakable_tie_between_second_and_third.csv
+-rw-r--r--   0        0        0      340 2023-05-21 14:36:12.440552 starvote-1.4/sample_polls/sample_poll_score_round_breakable_tie_between_second_and_third.result.txt
+-rw-r--r--   0        0        0      169 2023-05-20 12:14:18.630735 starvote-1.4/sample_polls/sample_poll_score_round_unbreakable_three_way_tie_for_first.csv
+-rw-r--r--   0        0        0      234 2023-05-21 14:36:15.004573 starvote-1.4/sample_polls/sample_poll_score_round_unbreakable_three_way_tie_for_first.result.txt
+-rw-r--r--   0        0        0      226 2023-05-20 14:20:22.817978 starvote-1.4/sample_polls/sample_poll_score_round_unbreakable_three_way_tie_for_second.csv
+-rw-r--r--   0        0        0      267 2023-05-21 14:36:17.328593 starvote-1.4/sample_polls/sample_poll_score_round_unbreakable_three_way_tie_for_second.result.txt
+-rw-r--r--   0        0        0      169 2023-05-20 12:30:43.458967 starvote-1.4/sample_polls/sample_poll_score_round_unbreakable_tie_between_second_and_third.csv
+-rw-r--r--   0        0        0      374 2023-05-21 14:36:20.268617 starvote-1.4/sample_polls/sample_poll_score_round_unbreakable_tie_between_second_and_third.result.txt
+-rw-r--r--   0        0        0   115109 2023-05-20 12:04:19.133723 starvote-1.4/sample_polls/starvote_ballots_2020_democratic_presidential_primary.csv
+-rw-r--r--   0        0        0   696161 2023-05-20 14:36:00.553825 starvote-1.4/sample_polls/starvote_ballots_2020_democratic_presidential_primary.result.pdf
+-rw-r--r--   0        0        0     2642 2023-05-21 14:36:26.092666 starvote-1.4/sample_polls/starvote_ballots_2020_democratic_presidential_primary.result.txt
+-rw-r--r--   0        0        0    57750 2023-05-20 12:04:29.149807 starvote-1.4/sample_polls/starvote_ballots_2020_libertarian_party_presidential_nomination.csv
+-rw-r--r--   0        0        0   575556 2023-05-20 14:35:00.177319 starvote-1.4/sample_polls/starvote_ballots_2020_libertarian_party_presidential_nomination.result.pdf
+-rw-r--r--   0        0        0      961 2023-05-21 14:36:28.876690 starvote-1.4/sample_polls/starvote_ballots_2020_libertarian_party_presidential_nomination.result.txt
+-rw-r--r--   0        0        0    49711 2023-05-20 12:04:34.029848 starvote-1.4/sample_polls/starvote_ballots_best_akali_skins.csv
+-rw-r--r--   0        0        0   538128 2023-05-20 14:33:25.560528 starvote-1.4/sample_polls/starvote_ballots_best_akali_skins.result.pdf
+-rw-r--r--   0        0        0      876 2023-05-21 14:36:32.040716 starvote-1.4/sample_polls/starvote_ballots_best_akali_skins.result.txt
+-rw-r--r--   0        0        0     1812 2023-05-20 10:35:18.365110 starvote-1.4/sample_polls/starvote_ballots_eurovision_song_contest_2023.csv
+-rw-r--r--   0        0        0   807144 2023-05-20 14:33:51.120742 starvote-1.4/sample_polls/starvote_ballots_eurovision_song_contest_2023.result.pdf
+-rw-r--r--   0        0        0     2418 2023-05-21 14:36:34.744739 starvote-1.4/sample_polls/starvote_ballots_eurovision_song_contest_2023.result.txt
+-rw-r--r--   0        0        0   250538 2023-05-20 10:34:04.044490 starvote-1.4/sample_polls/starvote_ballots_libertarian_party_2020_presidential_nomination_may.csv
+-rw-r--r--   0        0        0   643536 2023-05-20 14:35:41.153662 starvote-1.4/sample_polls/starvote_ballots_libertarian_party_2020_presidential_nomination_may.result.pdf
+-rw-r--r--   0        0        0     1091 2023-05-21 14:36:37.344761 starvote-1.4/sample_polls/starvote_ballots_libertarian_party_2020_presidential_nomination_may.result.txt
+-rw-r--r--   0        0        0    31534 2023-05-20 12:04:38.493885 starvote-1.4/sample_polls/starvote_ballots_presidential_candidates.csv
+-rw-r--r--   0        0        0   325033 2023-05-20 14:34:17.572963 starvote-1.4/sample_polls/starvote_ballots_presidential_candidates.result.pdf
+-rw-r--r--   0        0        0      408 2023-05-21 14:36:39.896782 starvote-1.4/sample_polls/starvote_ballots_presidential_candidates.result.txt
+-rw-r--r--   0        0        0    48454 2023-05-20 12:04:25.689778 starvote-1.4/sample_polls/starvote_ballots_presidential_poll_july_2020.csv
+-rw-r--r--   0        0        0   360427 2023-05-20 14:36:25.050030 starvote-1.4/sample_polls/starvote_ballots_presidential_poll_july_2020.result.pdf
+-rw-r--r--   0        0        0      419 2023-05-21 14:36:42.084801 starvote-1.4/sample_polls/starvote_ballots_presidential_poll_july_2020.result.txt
+-rw-r--r--   0        0        0   123039 2023-05-20 12:04:13.781679 starvote-1.4/sample_polls/starvote_ballots_updated_2020_libertarian_presidential_candidate.csv
+-rw-r--r--   0        0        0   584998 2023-05-20 14:35:22.465506 starvote-1.4/sample_polls/starvote_ballots_updated_2020_libertarian_presidential_candidate.result.pdf
+-rw-r--r--   0        0        0      961 2023-05-21 14:36:44.284819 starvote-1.4/sample_polls/starvote_ballots_updated_2020_libertarian_presidential_candidate.result.txt
+-rw-r--r--   0        0        0    52870 2023-05-20 12:04:22.533752 starvote-1.4/sample_polls/starvote_ballots_wa_governor_2020_republican_party_straw_poll.csv
+-rw-r--r--   0        0        0   354740 2023-05-20 14:36:48.550226 starvote-1.4/sample_polls/starvote_ballots_wa_governor_2020_republican_party_straw_poll.result.pdf
+-rw-r--r--   0        0        0      377 2023-05-21 14:36:46.788840 starvote-1.4/sample_polls/starvote_ballots_wa_governor_2020_republican_party_straw_poll.result.txt
+-rw-r--r--   0        0        0    18359 2023-05-21 14:41:59.959474 starvote-1.4/starvote/__init__.py
+-rw-r--r--   0        0        0       84 2023-05-21 14:27:54.116361 starvote-1.4/starvote/__main__.py
+-rw-r--r--   0        0        0     1981 2023-05-21 14:47:39.842332 starvote-1.4/tests/run_tests.py
+-rw-r--r--   0        0        0     6546 1970-01-01 00:00:00.000000 starvote-1.4/PKG-INFO
```

### Comparing `starvote-1.3/LICENSE` & `starvote-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `starvote-1.3/README.md` & `starvote-1.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -133,14 +133,22 @@
 The source code repository includes sample ballots downloaded from
 [https://star.vote/](https://star.vote/).  The licensing of these
 sample ballots is unclear, but they're assumed to be public-domain
 or otherwise freely redistributable.
 
 ## Changelog
 
+**1.4** *2023/05/21*
+
+* Automated the test suite.
+* Add logging prints for tie-breaker preference round
+  for Proportional STAR.
+* Fixed presentation in `__main__` for multiple winner
+  elections that end in a tie.
+
 **1.3** *2023/05/21*
 
 * Added support for
   [Proportional STAR](https://www.starvoting.org/star-pr)
   polls.  The only visible external change is the new
   `Proportional_STAR` enum value.
 * Renamed the `winners` parameter on the `Poll` constructor to `seats`.
```

### Comparing `starvote-1.3/sample_polls/starvote_ballots_4tyx27ks_20230520050434.csv` & `starvote-1.4/sample_polls/starvote_ballots_best_akali_skins.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.3/sample_polls/starvote_ballots_4tyx27ks_20230520050434.result.pdf` & `starvote-1.4/sample_polls/starvote_ballots_best_akali_skins.result.pdf`

 * *Files identical despite different names*

### Comparing `starvote-1.3/sample_polls/starvote_ballots_4tyx27ks_20230520050434.result.txt` & `starvote-1.4/sample_polls/starvote_ballots_best_akali_skins.result.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+[STAR]
 [Score round]
   Star Guardian        -- 2930 (average 4.38)
   Prestige K/DA        -- 2458 (average 3.67)
   True Damage          -- 2379 (average 3.56)
   K/DA All Out         -- 2371 (average 3.54)
   K/DA                 -- 2325 (average 3.48)
   Original             -- 2175 (average 3.25)
```

### Comparing `starvote-1.3/sample_polls/starvote_ballots_9fm5fp2c_20230520033518.csv` & `starvote-1.4/sample_polls/starvote_ballots_eurovision_song_contest_2023.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.3/sample_polls/starvote_ballots_9fm5fp2c_20230520033518.result.pdf` & `starvote-1.4/sample_polls/starvote_ballots_eurovision_song_contest_2023.result.pdf`

 * *Files identical despite different names*

### Comparing `starvote-1.3/sample_polls/starvote_ballots_9fm5fp2c_20230520033518.result.txt` & `starvote-1.4/sample_polls/starvote_ballots_eurovision_song_contest_2023.result.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+[STAR]
 [Score round]
   Finland - &quot;Cha Cha Cha&quot;               -- 22 (average 3.67)
   Israel - &quot;Unicorn&quot;                    -- 20 (average 3.33)
   Norway - &quot;Queen of Kings&quot;             -- 17 (average 2.83)
   Croatia - &quot;Mama &Scaron;Č!&quot;           -- 17 (average 2.83)
   Australia - &quot;Promise&quot;                 -- 17 (average 2.83)
   Czechia - &quot;My Sister&#039;s Crown&quot;    -- 16 (average 2.67)
```

### Comparing `starvote-1.3/sample_polls/starvote_ballots_9mm3519w_20230520050438.csv` & `starvote-1.4/sample_polls/starvote_ballots_presidential_candidates.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.3/sample_polls/starvote_ballots_9mm3519w_20230520050438.result.pdf` & `starvote-1.4/sample_polls/starvote_ballots_presidential_candidates.result.pdf`

 * *Files identical despite different names*

### Comparing `starvote-1.3/sample_polls/starvote_ballots_9xrw9wch_20230520050429.csv` & `starvote-1.4/sample_polls/starvote_ballots_2020_libertarian_party_presidential_nomination.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.3/sample_polls/starvote_ballots_9xrw9wch_20230520050429.result.pdf` & `starvote-1.4/sample_polls/starvote_ballots_2020_libertarian_party_presidential_nomination.result.pdf`

 * *Files identical despite different names*

### Comparing `starvote-1.3/sample_polls/starvote_ballots_9xrw9wch_20230520050429.result.txt` & `starvote-1.4/sample_polls/starvote_ballots_2020_libertarian_party_presidential_nomination.result.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+[STAR]
 [Score round]
   Vermin Supreme    -- 2865 (average 3.99)
   Dan Behrman       --  708 (average 0.99)
   Jacob Hornberger  --  703 (average 0.98)
   John McAfee       --  584 (average 0.81)
   Lincoln Chafee    --  340 (average 0.47)
   Jo Jorgensen      --  333 (average 0.46)
```

### Comparing `starvote-1.3/sample_polls/starvote_ballots_dd1wc4yx_20230520050413.csv` & `starvote-1.4/sample_polls/starvote_ballots_updated_2020_libertarian_presidential_candidate.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.3/sample_polls/starvote_ballots_dd1wc4yx_20230520050413.result.pdf` & `starvote-1.4/sample_polls/starvote_ballots_updated_2020_libertarian_presidential_candidate.result.pdf`

 * *Files identical despite different names*

### Comparing `starvote-1.3/sample_polls/starvote_ballots_dd1wc4yx_20230520050413.result.txt` & `starvote-1.4/sample_polls/starvote_ballots_updated_2020_libertarian_presidential_candidate.result.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+[STAR]
 [Score round]
   Vermin Supreme    -- 4653 (average 3.03)
   Judge Jim Gray    -- 3008 (average 1.96)
   Jo Jorgensen      -- 2012 (average 1.31)
   Jacob Hornberger  -- 2011 (average 1.31)
   Adam Kokesh       -- 1403 (average 0.91)
   John Monds        -- 1132 (average 0.74)
```

### Comparing `starvote-1.3/sample_polls/starvote_ballots_eh3cxxz7_20230520033403.csv` & `starvote-1.4/sample_polls/starvote_ballots_libertarian_party_2020_presidential_nomination_may.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.3/sample_polls/starvote_ballots_eh3cxxz7_20230520033403.result.pdf` & `starvote-1.4/sample_polls/starvote_ballots_libertarian_party_2020_presidential_nomination_may.result.pdf`

 * *Files identical despite different names*

### Comparing `starvote-1.3/sample_polls/starvote_ballots_eh3cxxz7_20230520033403.result.txt` & `starvote-1.4/sample_polls/starvote_ballots_libertarian_party_2020_presidential_nomination_may.result.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+[STAR]
 [Score round]
   Justin Amash      -- 8018 (average 2.76)
   Vermin Supreme    -- 7200 (average 2.48)
   Judge Jim Gray    -- 3826 (average 1.32)
   Jacob Hornberger  -- 3193 (average 1.10)
   Jo Jorgensen      -- 2625 (average 0.90)
   Adam Kokesh       -- 2324 (average 0.80)
```

### Comparing `starvote-1.3/sample_polls/starvote_ballots_p4rs6xn4_20230520050419.csv` & `starvote-1.4/sample_polls/starvote_ballots_2020_democratic_presidential_primary.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.3/sample_polls/starvote_ballots_p4rs6xn4_20230520050419.result.pdf` & `starvote-1.4/sample_polls/starvote_ballots_2020_democratic_presidential_primary.result.pdf`

 * *Files identical despite different names*

### Comparing `starvote-1.3/sample_polls/starvote_ballots_p4rs6xn4_20230520050419.result.txt` & `starvote-1.4/sample_polls/starvote_ballots_2020_democratic_presidential_primary.result.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+[STAR]
 [Score round]
   Andrew Yang - D                               -- 3226 (average 3.16)
   Bernie Sanders - D                            -- 2020 (average 1.98)
   Tulsi Gabbard - D                             -- 1372 (average 1.34)
   Elizabeth Warren - D                          -- 1258 (average 1.23)
   Pete Buttigieg - D                            --  979 (average 0.96)
   Beto O&#039;Rourke - D                        --  791 (average 0.77)
```

### Comparing `starvote-1.3/sample_polls/starvote_ballots_pf69snyx_20230520050425.csv` & `starvote-1.4/sample_polls/starvote_ballots_presidential_poll_july_2020.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.3/sample_polls/starvote_ballots_pf69snyx_20230520050425.result.pdf` & `starvote-1.4/sample_polls/starvote_ballots_presidential_poll_july_2020.result.pdf`

 * *Files identical despite different names*

### Comparing `starvote-1.3/sample_polls/starvote_ballots_swzw2ts6_20230520050422.csv` & `starvote-1.4/sample_polls/starvote_ballots_wa_governor_2020_republican_party_straw_poll.csv`

 * *Files identical despite different names*

### Comparing `starvote-1.3/sample_polls/starvote_ballots_swzw2ts6_20230520050422.result.pdf` & `starvote-1.4/sample_polls/starvote_ballots_wa_governor_2020_republican_party_straw_poll.result.pdf`

 * *Files identical despite different names*

### Comparing `starvote-1.3/starvote/__init__.py` & `starvote-1.4/starvote/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 
 __doc__ = "A simple STAR vote tabulator"
 
-__version__ = "1.3"
+__version__ = "1.4"
 
-__all__ = ['Poll', 'UnbreakableTieError', 'PollVariant', 'STAR', 'BLOC_STAR']
+__all__ = ['Poll', 'UnbreakableTieError', 'PollVariant', 'STAR', 'BLOC_STAR', 'main']
 
 import enum
 import math
 
 try:
     from enum import global_enum
 except ImportError:
@@ -154,15 +154,17 @@
                 print(f"  {len(ballots)}{remaining} ballots.")
                 self.print_rankings(ballots, rankings, print)
 
             round_winners = [t[1] for t in rankings if t[0] == rankings[-1][0]]
             if len(round_winners) > 2:
                 raise UnbreakableTieError(f"{len(round_winners)}-way tie in round {polling_round}", *round_winners)
             if len(round_winners) == 2:
-                winner = self.preference(ballots, *round_winners, when="proportional score round {polling_round}")
+                if print:
+                    print(f"[Tie-breaker preference round {polling_round}]")
+                winner = self.preference(ballots, *round_winners, when=f"score round {polling_round}", print=print)
             else:
                 assert len(round_winners) == 1
                 winner = round_winners.pop()
 
             # we need to allocate voters to the winner,
             # do the hare quota thing, etc.
             # for simplicity of implementation, we're only going to handle
@@ -348,7 +350,145 @@
         if self.variant == STAR:
             assert len(winners) == 1
             return winner
 
         assert len(winners) == self.seats
         return winners
 
+
+def main(argv, print=None):
+    import csv
+    import os.path
+
+    text = []
+    if print is None:
+        def print(*a, sep=" "):
+            text.append(sep.join(str(o) for o in a))
+
+    def usage(s=None):
+        if s:
+            print(s)
+            print()
+        print("usage: starvote.py [-v|--variant variant] [-s|--seats seats] ballot.csv")
+        print()
+        print("-v|--variant specifies STAR variant.  supported variants are STAR (default) and BLOC_STAR.")
+        print("-s|--seats specifies number of seats, default 1.")
+        print()
+        print("ballot is assumed to be in https://start.vote CSV format.")
+        print()
+        return -1
+
+    if not argv:
+        usage()
+
+    consume_variant = False
+    variant = None
+
+    consume_seats = False
+    seats = None
+
+    csv_file = None
+
+    extraneous_args = []
+
+    for arg in argv:
+        if consume_variant:
+            variant = arg
+            consume_variant = False
+            continue
+        if arg.startswith("-v=") or arg.startswith("--variant="):
+            if variant is not None:
+                usage("variant specified twice")
+            variant = arg.partition('=')[2]
+            continue
+        if arg in ("-v", "--variant"):
+            if variant is not None:
+                usage("variant specified twice")
+            consume_variant = True
+            continue
+
+        if consume_seats:
+            seats = int(arg)
+            consume_seats = False
+            continue
+        if arg.startswith("-s=") or arg.startswith("--seats="):
+            if seats is not None:
+                usage("seats specified twice")
+            seats = int(arg.partition('='))
+            continue
+        if arg in ("-s", "--seats"):
+            if seats is not None:
+                usage("seats specified twice")
+            consume_seats = True
+            continue
+
+        if csv_file is None:
+            csv_file = arg
+            continue
+        extraneous_args.append(arg)
+
+    if extraneous_args:
+        usage("too many arguments: " + " ".join(extraneous_args))
+
+    if variant in ("STAR", None):
+        variant = STAR
+    elif variant == "BLOC_STAR":
+        variant = BLOC_STAR
+    elif variant == "Proportional_STAR":
+        variant = Proportional_STAR
+    else:
+        usage("unknown variant " + variant)
+
+    if seats == None:
+        seats = 1
+
+    if csv_file is None:
+        usage("no CSV file specified.")
+    if not os.path.isfile(csv_file):
+        usage("invalid CSV file specified.")
+
+    poll = Poll(variant=variant, seats=seats)
+    with open(csv_file, "rt") as f:
+        reader = csv.reader(f)
+        candidates = None
+        for row in reader:
+            # clip off voterid, date, and pollid
+            row = row[3:]
+            if candidates == None:
+                candidates = row
+                # for candidate in candidates:
+                #     poll.add_candidate(candidate)
+                continue
+            ballot = {candidate: int(vote) for candidate, vote in zip(candidates, row)}
+            poll.add_ballot(ballot)
+
+    winner = None
+    try:
+        winner = poll.result(print=print)
+    except UnbreakableTieError as e:
+        if len(e.candidates) == 2:
+            winner = f"Tie between {e.candidates[0]} and {e.candidates[1]}"
+        else:
+            candidates = list(e.candidates)
+            last_candidate = candidates.pop()
+            winner = f"Tie between {', '.join(candidates)}, and {last_candidate}"
+        # hack so we print winner correctly
+        seats = 1
+
+        s = str(e)
+        s = s[0].title() + s[1:]
+        print(f"\n{s}!")
+        print("")
+    if seats == 1:
+        print("[Winner]")
+        print(f"  {winner}")
+    else:
+        print("[Winners]")
+        for w in winner:
+            print(f"  {w}")
+
+    if text:
+        import builtins
+        t = "\n".join(text)
+        builtins.print(t)
+
+    return 0
```

### Comparing `starvote-1.3/PKG-INFO` & `starvote-1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starvote
-Version: 1.3
+Version: 1.4
 Summary: A simple STAR vote tabulator
 Author-email: Larry Hastings <larry@hastings.org>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -145,14 +145,22 @@
 The source code repository includes sample ballots downloaded from
 [https://star.vote/](https://star.vote/).  The licensing of these
 sample ballots is unclear, but they're assumed to be public-domain
 or otherwise freely redistributable.
 
 ## Changelog
 
+**1.4** *2023/05/21*
+
+* Automated the test suite.
+* Add logging prints for tie-breaker preference round
+  for Proportional STAR.
+* Fixed presentation in `__main__` for multiple winner
+  elections that end in a tie.
+
 **1.3** *2023/05/21*
 
 * Added support for
   [Proportional STAR](https://www.starvoting.org/star-pr)
   polls.  The only visible external change is the new
   `Proportional_STAR` enum value.
 * Renamed the `winners` parameter on the `Poll` constructor to `seats`.
```

