# Comparing `tmp/starvote-2.0.4.tar.gz` & `tmp/starvote-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starvote-2.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "starvote-2.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `starvote-2.0.4.tar` & `starvote-2.0.5.tar`

### file list

```diff
@@ -1,176 +1,176 @@
--rw-r--r--   0        0        0       38 2023-05-27 15:21:37.716345 starvote-2.0.4/.gitignore
--rw-r--r--   0        0        0     1087 2023-05-20 12:48:55.372092 starvote-2.0.4/LICENSE
--rw-r--r--   0        0        0    42414 2023-06-05 17:24:51.330751 starvote-2.0.4/README.md
--rw-r--r--   0        0        0    15825 2023-06-01 10:48:31.686649 starvote-2.0.4/docs/clarifying_star_voting.md
--rw-r--r--   0        0        0     2743 2023-05-31 19:56:48.827782 starvote-2.0.4/docs/formatting_fractions_in_columns_of_text.txt
--rw-r--r--   0        0        0      217 2023-05-31 21:13:55.136896 starvote-2.0.4/example.py
--rw-r--r--   0        0        0      583 2023-06-02 19:49:52.947305 starvote-2.0.4/pyproject.toml
--rw-r--r--   0        0        0    99015 2023-06-05 17:42:03.467249 starvote-2.0.4/starvote/__init__.py
--rw-r--r--   0        0        0      106 2023-06-02 00:43:16.709978 starvote-2.0.4/starvote/__main__.py
--rw-r--r--   0        0        0     5872 2023-06-03 01:02:33.216747 starvote-2.0.4/starvote/reference.py
--rw-r--r--   0        0        0     1051 2023-06-02 01:09:12.579780 starvote-2.0.4/test_elections/README.md
--rw-r--r--   0        0        0       84 2023-06-01 23:43:37.846114 starvote-2.0.4/test_elections/bad_syntax_ballot_pragma_as_last_line.starvote
--rw-r--r--   0        0        0     1365 2023-06-05 15:58:25.628403 starvote-2.0.4/test_elections/bad_syntax_ballot_pragma_as_last_line.txt
--rw-r--r--   0        0        0       68 2023-06-01 23:24:50.800081 starvote-2.0.4/test_elections/bad_syntax_change_section_in_list.starvote
--rw-r--r--   0        0        0     1402 2023-06-05 15:58:25.628403 starvote-2.0.4/test_elections/bad_syntax_change_section_in_list.txt
--rw-r--r--   0        0        0       68 2023-06-01 23:23:06.267150 starvote-2.0.4/test_elections/bad_syntax_fussy_wrong_ballots_1.starvote
--rw-r--r--   0        0        0     1411 2023-06-05 15:58:25.628403 starvote-2.0.4/test_elections/bad_syntax_fussy_wrong_ballots_1.txt
--rw-r--r--   0        0        0       67 2023-06-01 23:23:00.095096 starvote-2.0.4/test_elections/bad_syntax_fussy_wrong_ballots_2.starvote
--rw-r--r--   0        0        0     1409 2023-06-05 15:58:25.628403 starvote-2.0.4/test_elections/bad_syntax_fussy_wrong_ballots_2.txt
--rw-r--r--   0        0        0       35 2023-06-02 19:31:20.821653 starvote-2.0.4/test_elections/bad_syntax_invalid_method.starvote
--rw-r--r--   0        0        0     1381 2023-06-05 15:58:25.628403 starvote-2.0.4/test_elections/bad_syntax_invalid_method.txt
--rw-r--r--   0        0        0       40 2023-06-01 23:17:55.140381 starvote-2.0.4/test_elections/bad_syntax_invalid_option.starvote
--rw-r--r--   0        0        0     1381 2023-06-05 15:58:25.628403 starvote-2.0.4/test_elections/bad_syntax_invalid_option.txt
--rw-r--r--   0        0        0       44 2023-06-01 23:16:35.203670 starvote-2.0.4/test_elections/bad_syntax_invalid_pragma.starvote
--rw-r--r--   0        0        0     1383 2023-06-05 15:58:25.628403 starvote-2.0.4/test_elections/bad_syntax_invalid_pragma.txt
--rw-r--r--   0        0        0       89 2023-06-01 23:37:41.946945 starvote-2.0.4/test_elections/bad_syntax_invalid_start_of_line_mode.starvote
--rw-r--r--   0        0        0     1342 2023-06-05 15:58:25.628403 starvote-2.0.4/test_elections/bad_syntax_invalid_start_of_line_mode.txt
--rw-r--r--   0        0        0       50 2023-06-01 23:14:06.126343 starvote-2.0.4/test_elections/bad_syntax_invalid_starvote_path_1.starvote
--rw-r--r--   0        0        0     1338 2023-06-05 15:58:25.628403 starvote-2.0.4/test_elections/bad_syntax_invalid_starvote_path_1.txt
--rw-r--r--   0        0        0       70 2023-06-01 23:28:17.369920 starvote-2.0.4/test_elections/bad_syntax_invalid_starvote_path_2.starvote
--rw-r--r--   0        0        0     1367 2023-06-05 15:58:25.628403 starvote-2.0.4/test_elections/bad_syntax_invalid_starvote_path_2.txt
--rw-r--r--   0        0        0       38 2023-06-01 23:13:26.765992 starvote-2.0.4/test_elections/bad_syntax_invalid_tiebreaker.starvote
--rw-r--r--   0        0        0     1389 2023-06-05 15:58:25.628403 starvote-2.0.4/test_elections/bad_syntax_invalid_tiebreaker.txt
--rw-r--r--   0        0        0       59 2023-06-02 02:02:11.939956 starvote-2.0.4/test_elections/bad_syntax_malformed_section.starvote
--rw-r--r--   0        0        0     1378 2023-06-05 15:58:25.628403 starvote-2.0.4/test_elections/bad_syntax_malformed_section.txt
--rw-r--r--   0        0        0       41 2023-06-01 23:44:44.538707 starvote-2.0.4/test_elections/bad_syntax_no_ballots.starvote
--rw-r--r--   0        0        0     1321 2023-06-05 15:58:25.628403 starvote-2.0.4/test_elections/bad_syntax_no_ballots.txt
--rw-r--r--   0        0        0       44 2023-06-01 23:34:09.385053 starvote-2.0.4/test_elections/bad_syntax_no_equals.starvote
--rw-r--r--   0        0        0     1353 2023-06-05 15:58:25.628403 starvote-2.0.4/test_elections/bad_syntax_no_equals.txt
--rw-r--r--   0        0        0       59 2023-06-02 01:03:50.036922 starvote-2.0.4/test_elections/bad_syntax_no_method.starvote
--rw-r--r--   0        0        0     1416 2023-06-05 15:58:25.628403 starvote-2.0.4/test_elections/bad_syntax_no_method.txt
--rw-r--r--   0        0        0       46 2023-06-01 23:32:02.351922 starvote-2.0.4/test_elections/bad_syntax_no_section.starvote
--rw-r--r--   0        0        0     1371 2023-06-05 15:58:25.628403 starvote-2.0.4/test_elections/bad_syntax_no_section.txt
--rw-r--r--   0        0        0       47 2023-06-01 23:21:20.118206 starvote-2.0.4/test_elections/bad_syntax_pragma_in_options.starvote
--rw-r--r--   0        0        0     1382 2023-06-05 15:58:25.628403 starvote-2.0.4/test_elections/bad_syntax_pragma_in_options.txt
--rw-r--r--   0        0        0      103 2023-06-01 23:32:48.848336 starvote-2.0.4/test_elections/bad_syntax_pragma_inside_list.starvote
--rw-r--r--   0        0        0     1394 2023-06-05 15:58:25.628403 starvote-2.0.4/test_elections/bad_syntax_pragma_inside_list.txt
--rw-r--r--   0        0        0       47 2023-06-01 23:18:10.564519 starvote-2.0.4/test_elections/bad_syntax_repeated_option.starvote
--rw-r--r--   0        0        0     1387 2023-06-05 15:58:25.628403 starvote-2.0.4/test_elections/bad_syntax_repeated_option.txt
--rw-r--r--   0        0        0       60 2023-06-01 23:31:08.239441 starvote-2.0.4/test_elections/bad_syntax_repeated_section.starvote
--rw-r--r--   0        0        0     1390 2023-06-05 15:58:25.628403 starvote-2.0.4/test_elections/bad_syntax_repeated_section.txt
--rw-r--r--   0        0        0    57750 2023-05-20 12:04:29.149807 starvote-2.0.4/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.csv
--rw-r--r--   0        0        0   575556 2023-05-20 14:35:00.177319 starvote-2.0.4/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.pdf
--rw-r--r--   0        0        0     1403 2023-06-05 15:58:25.632403 starvote-2.0.4/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.txt
--rw-r--r--   0        0        0   115221 2023-05-27 14:48:58.735061 starvote-2.0.4/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.csv
--rw-r--r--   0        0        0   410807 2023-05-27 14:59:16.160516 starvote-2.0.4/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.pdf
--rw-r--r--   0        0        0     3193 2023-06-05 15:58:25.644404 starvote-2.0.4/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.txt
--rw-r--r--   0        0        0    49711 2023-05-20 12:04:34.029848 starvote-2.0.4/test_elections/starvote_ballots_best_akali_skins.csv
--rw-r--r--   0        0        0   538128 2023-05-20 14:33:25.560528 starvote-2.0.4/test_elections/starvote_ballots_best_akali_skins.pdf
--rw-r--r--   0        0        0     1331 2023-06-05 15:58:25.648404 starvote-2.0.4/test_elections/starvote_ballots_best_akali_skins.txt
--rw-r--r--   0        0        0     1812 2023-05-20 10:35:18.365110 starvote-2.0.4/test_elections/starvote_ballots_eurovision_song_contest_2023.csv
--rw-r--r--   0        0        0   807144 2023-05-20 14:33:51.120742 starvote-2.0.4/test_elections/starvote_ballots_eurovision_song_contest_2023.pdf
--rw-r--r--   0        0        0     2879 2023-06-05 15:58:25.648404 starvote-2.0.4/test_elections/starvote_ballots_eurovision_song_contest_2023.txt
--rw-r--r--   0        0        0   250538 2023-05-20 10:34:04.044490 starvote-2.0.4/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.csv
--rw-r--r--   0        0        0   643536 2023-05-20 14:35:41.153662 starvote-2.0.4/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.pdf
--rw-r--r--   0        0        0     1596 2023-06-05 15:58:25.668404 starvote-2.0.4/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.txt
--rw-r--r--   0        0        0      141 2023-06-02 19:18:26.038889 starvote-2.0.4/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_allocated.starvote
--rw-r--r--   0        0        0    12601 2023-06-05 17:37:55.077204 starvote-2.0.4/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_allocated.txt
--rw-r--r--   0        0        0      170 2023-06-05 16:53:17.023154 starvote-2.0.4/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_bloc_star.starvote
--rw-r--r--   0        0        0     7239 2023-06-05 16:54:13.803622 starvote-2.0.4/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_bloc_star.txt
--rw-r--r--   0        0        0      135 2023-06-05 16:03:25.302834 starvote-2.0.4/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_sss.starvote
--rw-r--r--   0        0        0    60069 2023-06-05 17:20:24.228552 starvote-2.0.4/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_sss.txt
--rw-r--r--   0        0        0    31534 2023-05-20 12:04:38.493885 starvote-2.0.4/test_elections/starvote_ballots_presidential_candidates.csv
--rw-r--r--   0        0        0   325033 2023-05-20 14:34:17.572963 starvote-2.0.4/test_elections/starvote_ballots_presidential_candidates.pdf
--rw-r--r--   0        0        0      814 2023-06-05 15:58:26.312409 starvote-2.0.4/test_elections/starvote_ballots_presidential_candidates.txt
--rw-r--r--   0        0        0    48454 2023-05-20 12:04:25.689778 starvote-2.0.4/test_elections/starvote_ballots_presidential_poll_july_2020.csv
--rw-r--r--   0        0        0   360427 2023-05-20 14:36:25.050030 starvote-2.0.4/test_elections/starvote_ballots_presidential_poll_july_2020.pdf
--rw-r--r--   0        0        0      799 2023-06-05 15:58:26.316409 starvote-2.0.4/test_elections/starvote_ballots_presidential_poll_july_2020.txt
--rw-r--r--   0        0        0   123039 2023-05-20 12:04:13.781679 starvote-2.0.4/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.csv
--rw-r--r--   0        0        0   584998 2023-05-20 14:35:22.465506 starvote-2.0.4/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.pdf
--rw-r--r--   0        0        0     1434 2023-06-05 15:58:26.324409 starvote-2.0.4/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.txt
--rw-r--r--   0        0        0    52870 2023-05-20 12:04:22.533752 starvote-2.0.4/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.csv
--rw-r--r--   0        0        0   354740 2023-05-20 14:36:48.550226 starvote-2.0.4/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.pdf
--rw-r--r--   0        0        0      747 2023-06-05 15:58:26.328409 starvote-2.0.4/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.txt
--rw-r--r--   0        0        0      151 2023-06-02 19:18:20.314839 starvote-2.0.4/test_elections/test_election_all_fives_allocated.starvote
--rw-r--r--   0        0        0      476 2023-06-05 15:58:26.328409 starvote-2.0.4/test_elections/test_election_all_fives_allocated.txt
--rw-r--r--   0        0        0      146 2023-06-01 14:23:14.825743 starvote-2.0.4/test_elections/test_election_all_fives_bloc_star.starvote
--rw-r--r--   0        0        0     1080 2023-06-05 15:58:26.328409 starvote-2.0.4/test_elections/test_election_all_fives_bloc_star.txt
--rw-r--r--   0        0        0      145 2023-06-01 14:23:10.941709 starvote-2.0.4/test_elections/test_election_all_fives_rrv.starvote
--rw-r--r--   0        0        0      484 2023-06-05 15:58:26.328409 starvote-2.0.4/test_elections/test_election_all_fives_rrv.txt
--rw-r--r--   0        0        0      145 2023-06-05 16:03:21.998808 starvote-2.0.4/test_elections/test_election_all_fives_sss.starvote
--rw-r--r--   0        0        0      491 2023-06-05 17:36:55.760715 starvote-2.0.4/test_elections/test_election_all_fives_sss.txt
--rw-r--r--   0        0        0      132 2023-06-01 14:23:02.245634 starvote-2.0.4/test_elections/test_election_all_fives_star.starvote
--rw-r--r--   0        0        0     1030 2023-06-05 15:58:26.328409 starvote-2.0.4/test_elections/test_election_all_fives_star.txt
--rw-r--r--   0        0        0       98 2023-06-02 19:18:18.286821 starvote-2.0.4/test_elections/test_election_all_threes_allocated.starvote
--rw-r--r--   0        0        0      476 2023-06-05 15:58:26.328409 starvote-2.0.4/test_elections/test_election_all_threes_allocated.txt
--rw-r--r--   0        0        0      146 2023-06-01 14:23:30.837882 starvote-2.0.4/test_elections/test_election_all_threes_bloc_star.starvote
--rw-r--r--   0        0        0     1080 2023-06-05 15:58:26.328409 starvote-2.0.4/test_elections/test_election_all_threes_bloc_star.txt
--rw-r--r--   0        0        0       92 2023-06-01 22:34:03.536957 starvote-2.0.4/test_elections/test_election_all_threes_rrv.starvote
--rw-r--r--   0        0        0      484 2023-06-05 15:58:26.328409 starvote-2.0.4/test_elections/test_election_all_threes_rrv.txt
--rw-r--r--   0        0        0       92 2023-06-05 16:03:19.338786 starvote-2.0.4/test_elections/test_election_all_threes_sss.starvote
--rw-r--r--   0        0        0      491 2023-06-05 17:36:48.748658 starvote-2.0.4/test_elections/test_election_all_threes_sss.txt
--rw-r--r--   0        0        0      132 2023-06-01 14:23:19.233781 starvote-2.0.4/test_elections/test_election_all_threes_star.starvote
--rw-r--r--   0        0        0     1030 2023-06-05 15:58:26.328409 starvote-2.0.4/test_elections/test_election_all_threes_star.txt
--rw-r--r--   0        0        0      151 2023-06-02 19:18:15.894800 starvote-2.0.4/test_elections/test_election_all_zeroes_allocated.starvote
--rw-r--r--   0        0        0      473 2023-06-05 15:58:26.328409 starvote-2.0.4/test_elections/test_election_all_zeroes_allocated.txt
--rw-r--r--   0        0        0      146 2023-06-01 14:19:42.607904 starvote-2.0.4/test_elections/test_election_all_zeroes_bloc_star.starvote
--rw-r--r--   0        0        0     1077 2023-06-05 15:58:26.328409 starvote-2.0.4/test_elections/test_election_all_zeroes_bloc_star.txt
--rw-r--r--   0        0        0      145 2023-06-01 14:19:40.835888 starvote-2.0.4/test_elections/test_election_all_zeroes_rrv.starvote
--rw-r--r--   0        0        0      481 2023-06-05 15:58:26.328409 starvote-2.0.4/test_elections/test_election_all_zeroes_rrv.txt
--rw-r--r--   0        0        0      145 2023-06-05 16:03:16.750765 starvote-2.0.4/test_elections/test_election_all_zeroes_sss.starvote
--rw-r--r--   0        0        0      488 2023-06-05 17:36:35.116545 starvote-2.0.4/test_elections/test_election_all_zeroes_sss.txt
--rw-r--r--   0        0        0      132 2023-06-01 14:19:46.079934 starvote-2.0.4/test_elections/test_election_all_zeroes_star.starvote
--rw-r--r--   0        0        0     1027 2023-06-05 15:58:26.332409 starvote-2.0.4/test_elections/test_election_all_zeroes_star.txt
--rw-r--r--   0        0        0      220 2023-06-05 17:40:04.326268 starvote-2.0.4/test_elections/test_election_all_zeroes_with_tiebreaker_sss.starvote
--rw-r--r--   0        0        0     1921 2023-06-05 17:40:54.170678 starvote-2.0.4/test_elections/test_election_all_zeroes_with_tiebreaker_sss.txt
--rw-r--r--   0        0        0     2660 2023-05-31 22:55:06.890838 starvote-2.0.4/test_elections/test_election_bloc_star_and_electowiki.starvote
--rw-r--r--   0        0        0     3383 2023-06-05 15:58:26.332409 starvote-2.0.4/test_elections/test_election_bloc_star_and_electowiki.txt
--rw-r--r--   0        0        0      989 2023-05-31 14:32:27.710655 starvote-2.0.4/test_elections/test_election_bloc_star_unbreakable_tie_for_first.starvote
--rw-r--r--   0        0        0     1606 2023-06-05 15:58:26.332409 starvote-2.0.4/test_elections/test_election_bloc_star_unbreakable_tie_for_first.txt
--rw-r--r--   0        0        0      201 2023-05-31 14:32:09.618494 starvote-2.0.4/test_elections/test_election_breakable_tie_for_second_in_score_round.starvote
--rw-r--r--   0        0        0      831 2023-06-05 15:58:26.332409 starvote-2.0.4/test_elections/test_election_breakable_tie_for_second_in_score_round.txt
--rw-r--r--   0        0        0      204 2023-05-31 14:31:42.454252 starvote-2.0.4/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_max_score_count_round.starvote
--rw-r--r--   0        0        0      965 2023-06-05 15:58:26.332409 starvote-2.0.4/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_max_score_count_round.txt
--rw-r--r--   0        0        0      203 2023-05-31 14:31:18.974043 starvote-2.0.4/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_score_round.starvote
--rw-r--r--   0        0        0      744 2023-06-05 15:58:26.332409 starvote-2.0.4/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_score_round.txt
--rw-r--r--   0        0        0      838 2023-05-31 14:31:04.393913 starvote-2.0.4/test_elections/test_election_demonstrate_cloneproofness_1.starvote
--rw-r--r--   0        0        0      542 2023-06-05 15:58:26.332409 starvote-2.0.4/test_elections/test_election_demonstrate_cloneproofness_1.txt
--rw-r--r--   0        0        0      830 2023-05-31 14:09:22.654324 starvote-2.0.4/test_elections/test_election_demonstrate_cloneproofness_2.starvote
--rw-r--r--   0        0        0     1087 2023-06-05 15:58:26.332409 starvote-2.0.4/test_elections/test_election_demonstrate_cloneproofness_2.txt
--rw-r--r--   0        0        0      194 2023-06-01 16:45:03.487305 starvote-2.0.4/test_elections/test_election_extra_candidates_in_permutation.starvote
--rw-r--r--   0        0        0      142 2023-06-05 15:58:26.332409 starvote-2.0.4/test_elections/test_election_extra_candidates_in_permutation.txt
--rw-r--r--   0        0        0      165 2023-06-01 16:45:09.147349 starvote-2.0.4/test_elections/test_election_incomplete_permutation.starvote
--rw-r--r--   0        0        0      138 2023-06-05 15:58:26.332409 starvote-2.0.4/test_elections/test_election_incomplete_permutation.txt
--rw-r--r--   0        0        0      132 2023-06-03 00:43:08.954337 starvote-2.0.4/test_elections/test_election_no_output.starvote
--rw-r--r--   0        0        0       17 2023-06-05 15:58:26.332409 starvote-2.0.4/test_elections/test_election_no_output.txt
--rw-r--r--   0        0        0      130 2023-06-01 16:34:20.926370 starvote-2.0.4/test_elections/test_election_no_permuted_candidates_tiebreaker.starvote
--rw-r--r--   0        0        0     1336 2023-06-05 15:58:26.332409 starvote-2.0.4/test_elections/test_election_no_permuted_candidates_tiebreaker.txt
--rw-r--r--   0        0        0      131 2023-06-01 17:57:44.689602 starvote-2.0.4/test_elections/test_election_only_one_candidate_star.starvote
--rw-r--r--   0        0        0      505 2023-06-05 15:58:26.336409 starvote-2.0.4/test_elections/test_election_only_one_candidate_star.txt
--rw-r--r--   0        0        0      182 2023-06-02 19:18:13.310778 starvote-2.0.4/test_elections/test_election_only_two_candidates_allocated.starvote
--rw-r--r--   0        0        0      547 2023-06-05 16:34:32.017979 starvote-2.0.4/test_elections/test_election_only_two_candidates_allocated.txt
--rw-r--r--   0        0        0      177 2023-06-01 17:57:23.633416 starvote-2.0.4/test_elections/test_election_only_two_candidates_bloc_star.starvote
--rw-r--r--   0        0        0      487 2023-06-05 15:58:26.336409 starvote-2.0.4/test_elections/test_election_only_two_candidates_bloc_star.txt
--rw-r--r--   0        0        0      176 2023-06-01 17:57:20.909392 starvote-2.0.4/test_elections/test_election_only_two_candidates_rrv.starvote
--rw-r--r--   0        0        0      523 2023-06-05 15:58:26.336409 starvote-2.0.4/test_elections/test_election_only_two_candidates_rrv.txt
--rw-r--r--   0        0        0      176 2023-06-05 16:03:13.610740 starvote-2.0.4/test_elections/test_election_only_two_candidates_sss.starvote
--rw-r--r--   0        0        0      556 2023-06-05 17:36:16.484392 starvote-2.0.4/test_elections/test_election_only_two_candidates_sss.txt
--rw-r--r--   0        0        0      319 2023-06-02 19:18:05.042705 starvote-2.0.4/test_elections/test_election_proportional_star_unbreakable_tie.starvote
--rw-r--r--   0        0        0      480 2023-06-05 15:58:26.336409 starvote-2.0.4/test_elections/test_election_proportional_star_unbreakable_tie.txt
--rw-r--r--   0        0        0     5899 2023-05-22 07:24:36.945502 starvote-2.0.4/test_elections/test_election_reweighted_range_sample_election.html
--rw-r--r--   0        0        0      450 2023-06-03 00:37:52.439507 starvote-2.0.4/test_elections/test_election_reweighted_range_sample_election.starvote
--rw-r--r--   0        0        0     1150 2023-06-05 15:58:26.336409 starvote-2.0.4/test_elections/test_election_reweighted_range_sample_election.txt
--rw-r--r--   0        0        0      203 2023-05-31 14:05:02.452007 starvote-2.0.4/test_elections/test_election_unbreakable_three_way_tie_for_first_in_score_round.starvote
--rw-r--r--   0        0        0     1023 2023-06-05 15:58:26.336409 starvote-2.0.4/test_elections/test_election_unbreakable_three_way_tie_for_first_in_score_round.txt
--rw-r--r--   0        0        0      306 2023-06-01 18:06:23.106174 starvote-2.0.4/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round.starvote
--rw-r--r--   0        0        0     1788 2023-06-05 15:58:26.336409 starvote-2.0.4/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round.txt
--rw-r--r--   0        0        0      143 2023-06-02 19:18:03.054688 starvote-2.0.4/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round_allocated.starvote
--rw-r--r--   0        0        0     2033 2023-06-05 17:25:28.231055 starvote-2.0.4/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round_allocated.txt
--rw-r--r--   0        0        0      137 2023-06-05 16:03:10.882717 starvote-2.0.4/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round_sss.starvote
--rw-r--r--   0        0        0     2343 2023-06-05 17:23:26.814055 starvote-2.0.4/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round_sss.txt
--rw-r--r--   0        0        0      203 2023-05-31 14:04:09.035532 starvote-2.0.4/test_elections/test_election_unbreakable_tie_for_second_in_score_round.starvote
--rw-r--r--   0        0        0      938 2023-06-05 15:58:26.340409 starvote-2.0.4/test_elections/test_election_unbreakable_tie_for_second_in_score_round.txt
--rw-r--r--   0        0        0      155 2023-05-28 20:58:05.118365 starvote-2.0.4/test_elections/test_election_unbreakable_tie_in_automatic_runoff_round.starvote
--rw-r--r--   0        0        0     1081 2023-06-05 15:58:26.340409 starvote-2.0.4/test_elections/test_election_unbreakable_tie_in_automatic_runoff_round.txt
--rw-r--r--   0        0        0      150 2023-06-01 14:49:33.615373 starvote-2.0.4/test_elections/test_election_use_just_raise_tiebreaker.starvote
--rw-r--r--   0        0        0     1103 2023-06-05 15:58:26.340409 starvote-2.0.4/test_elections/test_election_use_just_raise_tiebreaker.txt
--rw-r--r--   0        0        0      154 2023-06-01 16:06:23.349484 starvote-2.0.4/test_elections/test_election_use_no_description_tiebreaker.starvote
--rw-r--r--   0        0        0     1030 2023-06-05 15:58:26.340409 starvote-2.0.4/test_elections/test_election_use_no_description_tiebreaker.txt
--rw-r--r--   0        0        0      152 2023-06-01 16:08:48.230596 starvote-2.0.4/test_elections/test_election_use_only_heading_tiebreaker.starvote
--rw-r--r--   0        0        0      152 2023-06-05 15:58:26.340409 starvote-2.0.4/test_elections/test_election_use_only_heading_tiebreaker.txt
--rw-r--r--   0        0        0      634 2023-06-03 00:09:38.012356 starvote-2.0.4/tests/harness.py
--rw-r--r--   0        0        0    36446 2023-06-03 01:08:39.424022 starvote-2.0.4/tests/run_tests.py
--rwxr-xr-x   0        0        0     2379 2023-06-03 00:24:17.844223 starvote-2.0.4/tools/is_ok
--rwxr-xr-x   0        0        0     2063 2023-06-03 00:15:52.499704 starvote-2.0.4/tools/remake_test_elections_output
--rw-r--r--   0        0        0    42984 1970-01-01 00:00:00.000000 starvote-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0       38 2023-05-27 15:21:37.716345 starvote-2.0.5/.gitignore
+-rw-r--r--   0        0        0     1066 2023-07-05 15:04:36.782904 starvote-2.0.5/LICENSE
+-rw-r--r--   0        0        0    42726 2023-07-05 15:07:14.716081 starvote-2.0.5/README.md
+-rw-r--r--   0        0        0    15825 2023-06-01 10:48:31.686649 starvote-2.0.5/docs/clarifying_star_voting.md
+-rw-r--r--   0        0        0     2743 2023-05-31 19:56:48.827782 starvote-2.0.5/docs/formatting_fractions_in_columns_of_text.txt
+-rw-r--r--   0        0        0      217 2023-06-09 16:10:35.292508 starvote-2.0.5/example.py
+-rw-r--r--   0        0        0      583 2023-06-02 19:49:52.947305 starvote-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0   100233 2023-07-05 15:06:08.655588 starvote-2.0.5/starvote/__init__.py
+-rw-r--r--   0        0        0      106 2023-06-02 00:43:16.709978 starvote-2.0.5/starvote/__main__.py
+-rw-r--r--   0        0        0     5872 2023-06-03 01:02:33.216747 starvote-2.0.5/starvote/reference.py
+-rw-r--r--   0        0        0     1051 2023-06-02 01:09:12.579780 starvote-2.0.5/test_elections/README.md
+-rw-r--r--   0        0        0       84 2023-06-01 23:43:37.846114 starvote-2.0.5/test_elections/bad_syntax_ballot_pragma_as_last_line.starvote
+-rw-r--r--   0        0        0     1365 2023-06-05 15:58:25.628403 starvote-2.0.5/test_elections/bad_syntax_ballot_pragma_as_last_line.txt
+-rw-r--r--   0        0        0       68 2023-06-01 23:24:50.800081 starvote-2.0.5/test_elections/bad_syntax_change_section_in_list.starvote
+-rw-r--r--   0        0        0     1402 2023-06-05 15:58:25.628403 starvote-2.0.5/test_elections/bad_syntax_change_section_in_list.txt
+-rw-r--r--   0        0        0       68 2023-06-01 23:23:06.267150 starvote-2.0.5/test_elections/bad_syntax_fussy_wrong_ballots_1.starvote
+-rw-r--r--   0        0        0     1411 2023-06-05 15:58:25.628403 starvote-2.0.5/test_elections/bad_syntax_fussy_wrong_ballots_1.txt
+-rw-r--r--   0        0        0       67 2023-06-01 23:23:00.095096 starvote-2.0.5/test_elections/bad_syntax_fussy_wrong_ballots_2.starvote
+-rw-r--r--   0        0        0     1409 2023-06-05 15:58:25.628403 starvote-2.0.5/test_elections/bad_syntax_fussy_wrong_ballots_2.txt
+-rw-r--r--   0        0        0       35 2023-06-02 19:31:20.821653 starvote-2.0.5/test_elections/bad_syntax_invalid_method.starvote
+-rw-r--r--   0        0        0     1381 2023-06-05 15:58:25.628403 starvote-2.0.5/test_elections/bad_syntax_invalid_method.txt
+-rw-r--r--   0        0        0       40 2023-06-01 23:17:55.140381 starvote-2.0.5/test_elections/bad_syntax_invalid_option.starvote
+-rw-r--r--   0        0        0     1381 2023-06-05 15:58:25.628403 starvote-2.0.5/test_elections/bad_syntax_invalid_option.txt
+-rw-r--r--   0        0        0       44 2023-06-01 23:16:35.203670 starvote-2.0.5/test_elections/bad_syntax_invalid_pragma.starvote
+-rw-r--r--   0        0        0     1383 2023-06-05 15:58:25.628403 starvote-2.0.5/test_elections/bad_syntax_invalid_pragma.txt
+-rw-r--r--   0        0        0       89 2023-06-01 23:37:41.946945 starvote-2.0.5/test_elections/bad_syntax_invalid_start_of_line_mode.starvote
+-rw-r--r--   0        0        0     1342 2023-06-05 15:58:25.628403 starvote-2.0.5/test_elections/bad_syntax_invalid_start_of_line_mode.txt
+-rw-r--r--   0        0        0       50 2023-06-01 23:14:06.126343 starvote-2.0.5/test_elections/bad_syntax_invalid_starvote_path_1.starvote
+-rw-r--r--   0        0        0     1338 2023-06-05 15:58:25.628403 starvote-2.0.5/test_elections/bad_syntax_invalid_starvote_path_1.txt
+-rw-r--r--   0        0        0       70 2023-06-01 23:28:17.369920 starvote-2.0.5/test_elections/bad_syntax_invalid_starvote_path_2.starvote
+-rw-r--r--   0        0        0     1367 2023-06-05 15:58:25.628403 starvote-2.0.5/test_elections/bad_syntax_invalid_starvote_path_2.txt
+-rw-r--r--   0        0        0       38 2023-06-01 23:13:26.765992 starvote-2.0.5/test_elections/bad_syntax_invalid_tiebreaker.starvote
+-rw-r--r--   0        0        0     1389 2023-06-05 15:58:25.628403 starvote-2.0.5/test_elections/bad_syntax_invalid_tiebreaker.txt
+-rw-r--r--   0        0        0       59 2023-06-02 02:02:11.939956 starvote-2.0.5/test_elections/bad_syntax_malformed_section.starvote
+-rw-r--r--   0        0        0     1378 2023-06-05 15:58:25.628403 starvote-2.0.5/test_elections/bad_syntax_malformed_section.txt
+-rw-r--r--   0        0        0       41 2023-06-01 23:44:44.538707 starvote-2.0.5/test_elections/bad_syntax_no_ballots.starvote
+-rw-r--r--   0        0        0     1321 2023-06-05 15:58:25.628403 starvote-2.0.5/test_elections/bad_syntax_no_ballots.txt
+-rw-r--r--   0        0        0       44 2023-06-01 23:34:09.385053 starvote-2.0.5/test_elections/bad_syntax_no_equals.starvote
+-rw-r--r--   0        0        0     1353 2023-06-05 15:58:25.628403 starvote-2.0.5/test_elections/bad_syntax_no_equals.txt
+-rw-r--r--   0        0        0       59 2023-06-02 01:03:50.036922 starvote-2.0.5/test_elections/bad_syntax_no_method.starvote
+-rw-r--r--   0        0        0     1416 2023-06-05 15:58:25.628403 starvote-2.0.5/test_elections/bad_syntax_no_method.txt
+-rw-r--r--   0        0        0       46 2023-06-01 23:32:02.351922 starvote-2.0.5/test_elections/bad_syntax_no_section.starvote
+-rw-r--r--   0        0        0     1371 2023-06-05 15:58:25.628403 starvote-2.0.5/test_elections/bad_syntax_no_section.txt
+-rw-r--r--   0        0        0       47 2023-06-01 23:21:20.118206 starvote-2.0.5/test_elections/bad_syntax_pragma_in_options.starvote
+-rw-r--r--   0        0        0     1382 2023-06-05 15:58:25.628403 starvote-2.0.5/test_elections/bad_syntax_pragma_in_options.txt
+-rw-r--r--   0        0        0      103 2023-06-01 23:32:48.848336 starvote-2.0.5/test_elections/bad_syntax_pragma_inside_list.starvote
+-rw-r--r--   0        0        0     1394 2023-06-05 15:58:25.628403 starvote-2.0.5/test_elections/bad_syntax_pragma_inside_list.txt
+-rw-r--r--   0        0        0       47 2023-06-01 23:18:10.564519 starvote-2.0.5/test_elections/bad_syntax_repeated_option.starvote
+-rw-r--r--   0        0        0     1387 2023-06-05 15:58:25.628403 starvote-2.0.5/test_elections/bad_syntax_repeated_option.txt
+-rw-r--r--   0        0        0       60 2023-06-01 23:31:08.239441 starvote-2.0.5/test_elections/bad_syntax_repeated_section.starvote
+-rw-r--r--   0        0        0     1390 2023-06-05 15:58:25.628403 starvote-2.0.5/test_elections/bad_syntax_repeated_section.txt
+-rw-r--r--   0        0        0    57750 2023-05-20 12:04:29.149807 starvote-2.0.5/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.csv
+-rw-r--r--   0        0        0   575556 2023-05-20 14:35:00.177319 starvote-2.0.5/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.pdf
+-rw-r--r--   0        0        0     1403 2023-06-05 15:58:25.632403 starvote-2.0.5/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.txt
+-rw-r--r--   0        0        0   115221 2023-05-27 14:48:58.735061 starvote-2.0.5/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.csv
+-rw-r--r--   0        0        0   410807 2023-05-27 14:59:16.160516 starvote-2.0.5/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.pdf
+-rw-r--r--   0        0        0     3193 2023-06-05 15:58:25.644404 starvote-2.0.5/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.txt
+-rw-r--r--   0        0        0    49711 2023-05-20 12:04:34.029848 starvote-2.0.5/test_elections/starvote_ballots_best_akali_skins.csv
+-rw-r--r--   0        0        0   538128 2023-05-20 14:33:25.560528 starvote-2.0.5/test_elections/starvote_ballots_best_akali_skins.pdf
+-rw-r--r--   0        0        0     1331 2023-06-05 15:58:25.648404 starvote-2.0.5/test_elections/starvote_ballots_best_akali_skins.txt
+-rw-r--r--   0        0        0     1812 2023-05-20 10:35:18.365110 starvote-2.0.5/test_elections/starvote_ballots_eurovision_song_contest_2023.csv
+-rw-r--r--   0        0        0   807144 2023-05-20 14:33:51.120742 starvote-2.0.5/test_elections/starvote_ballots_eurovision_song_contest_2023.pdf
+-rw-r--r--   0        0        0     2879 2023-06-05 15:58:25.648404 starvote-2.0.5/test_elections/starvote_ballots_eurovision_song_contest_2023.txt
+-rw-r--r--   0        0        0   250538 2023-05-20 10:34:04.044490 starvote-2.0.5/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.csv
+-rw-r--r--   0        0        0   643536 2023-05-20 14:35:41.153662 starvote-2.0.5/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.pdf
+-rw-r--r--   0        0        0     1596 2023-06-05 15:58:25.668404 starvote-2.0.5/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.txt
+-rw-r--r--   0        0        0      141 2023-06-02 19:18:26.038889 starvote-2.0.5/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_allocated.starvote
+-rw-r--r--   0        0        0    12601 2023-06-05 17:37:55.077204 starvote-2.0.5/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_allocated.txt
+-rw-r--r--   0        0        0      170 2023-06-05 16:53:17.023154 starvote-2.0.5/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_bloc_star.starvote
+-rw-r--r--   0        0        0     7239 2023-06-05 16:54:13.803622 starvote-2.0.5/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_bloc_star.txt
+-rw-r--r--   0        0        0      135 2023-06-05 16:03:25.302834 starvote-2.0.5/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_sss.starvote
+-rw-r--r--   0        0        0    60069 2023-06-05 17:20:24.228552 starvote-2.0.5/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_sss.txt
+-rw-r--r--   0        0        0    31534 2023-05-20 12:04:38.493885 starvote-2.0.5/test_elections/starvote_ballots_presidential_candidates.csv
+-rw-r--r--   0        0        0   325033 2023-05-20 14:34:17.572963 starvote-2.0.5/test_elections/starvote_ballots_presidential_candidates.pdf
+-rw-r--r--   0        0        0      814 2023-06-05 15:58:26.312409 starvote-2.0.5/test_elections/starvote_ballots_presidential_candidates.txt
+-rw-r--r--   0        0        0    48454 2023-05-20 12:04:25.689778 starvote-2.0.5/test_elections/starvote_ballots_presidential_poll_july_2020.csv
+-rw-r--r--   0        0        0   360427 2023-05-20 14:36:25.050030 starvote-2.0.5/test_elections/starvote_ballots_presidential_poll_july_2020.pdf
+-rw-r--r--   0        0        0      799 2023-06-05 15:58:26.316409 starvote-2.0.5/test_elections/starvote_ballots_presidential_poll_july_2020.txt
+-rw-r--r--   0        0        0   123039 2023-05-20 12:04:13.781679 starvote-2.0.5/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.csv
+-rw-r--r--   0        0        0   584998 2023-05-20 14:35:22.465506 starvote-2.0.5/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.pdf
+-rw-r--r--   0        0        0     1434 2023-06-05 15:58:26.324409 starvote-2.0.5/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.txt
+-rw-r--r--   0        0        0    52870 2023-05-20 12:04:22.533752 starvote-2.0.5/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.csv
+-rw-r--r--   0        0        0   354740 2023-05-20 14:36:48.550226 starvote-2.0.5/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.pdf
+-rw-r--r--   0        0        0      747 2023-06-05 15:58:26.328409 starvote-2.0.5/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.txt
+-rw-r--r--   0        0        0      151 2023-06-02 19:18:20.314839 starvote-2.0.5/test_elections/test_election_all_fives_allocated.starvote
+-rw-r--r--   0        0        0      476 2023-06-05 15:58:26.328409 starvote-2.0.5/test_elections/test_election_all_fives_allocated.txt
+-rw-r--r--   0        0        0      146 2023-06-01 14:23:14.825743 starvote-2.0.5/test_elections/test_election_all_fives_bloc_star.starvote
+-rw-r--r--   0        0        0     1080 2023-06-05 15:58:26.328409 starvote-2.0.5/test_elections/test_election_all_fives_bloc_star.txt
+-rw-r--r--   0        0        0      145 2023-06-01 14:23:10.941709 starvote-2.0.5/test_elections/test_election_all_fives_rrv.starvote
+-rw-r--r--   0        0        0      484 2023-06-05 15:58:26.328409 starvote-2.0.5/test_elections/test_election_all_fives_rrv.txt
+-rw-r--r--   0        0        0      145 2023-06-05 16:03:21.998808 starvote-2.0.5/test_elections/test_election_all_fives_sss.starvote
+-rw-r--r--   0        0        0      491 2023-06-05 17:36:55.760715 starvote-2.0.5/test_elections/test_election_all_fives_sss.txt
+-rw-r--r--   0        0        0      132 2023-06-01 14:23:02.245634 starvote-2.0.5/test_elections/test_election_all_fives_star.starvote
+-rw-r--r--   0        0        0     1030 2023-06-05 15:58:26.328409 starvote-2.0.5/test_elections/test_election_all_fives_star.txt
+-rw-r--r--   0        0        0       98 2023-06-02 19:18:18.286821 starvote-2.0.5/test_elections/test_election_all_threes_allocated.starvote
+-rw-r--r--   0        0        0      476 2023-06-05 15:58:26.328409 starvote-2.0.5/test_elections/test_election_all_threes_allocated.txt
+-rw-r--r--   0        0        0      146 2023-06-01 14:23:30.837882 starvote-2.0.5/test_elections/test_election_all_threes_bloc_star.starvote
+-rw-r--r--   0        0        0     1080 2023-06-05 15:58:26.328409 starvote-2.0.5/test_elections/test_election_all_threes_bloc_star.txt
+-rw-r--r--   0        0        0       92 2023-06-01 22:34:03.536957 starvote-2.0.5/test_elections/test_election_all_threes_rrv.starvote
+-rw-r--r--   0        0        0      484 2023-06-05 15:58:26.328409 starvote-2.0.5/test_elections/test_election_all_threes_rrv.txt
+-rw-r--r--   0        0        0       92 2023-06-05 16:03:19.338786 starvote-2.0.5/test_elections/test_election_all_threes_sss.starvote
+-rw-r--r--   0        0        0      491 2023-06-05 17:36:48.748658 starvote-2.0.5/test_elections/test_election_all_threes_sss.txt
+-rw-r--r--   0        0        0      132 2023-06-01 14:23:19.233781 starvote-2.0.5/test_elections/test_election_all_threes_star.starvote
+-rw-r--r--   0        0        0     1030 2023-06-05 15:58:26.328409 starvote-2.0.5/test_elections/test_election_all_threes_star.txt
+-rw-r--r--   0        0        0      151 2023-06-02 19:18:15.894800 starvote-2.0.5/test_elections/test_election_all_zeroes_allocated.starvote
+-rw-r--r--   0        0        0      473 2023-06-05 15:58:26.328409 starvote-2.0.5/test_elections/test_election_all_zeroes_allocated.txt
+-rw-r--r--   0        0        0      146 2023-06-01 14:19:42.607904 starvote-2.0.5/test_elections/test_election_all_zeroes_bloc_star.starvote
+-rw-r--r--   0        0        0     1077 2023-06-05 15:58:26.328409 starvote-2.0.5/test_elections/test_election_all_zeroes_bloc_star.txt
+-rw-r--r--   0        0        0      145 2023-06-01 14:19:40.835888 starvote-2.0.5/test_elections/test_election_all_zeroes_rrv.starvote
+-rw-r--r--   0        0        0      481 2023-06-05 15:58:26.328409 starvote-2.0.5/test_elections/test_election_all_zeroes_rrv.txt
+-rw-r--r--   0        0        0      145 2023-06-05 16:03:16.750765 starvote-2.0.5/test_elections/test_election_all_zeroes_sss.starvote
+-rw-r--r--   0        0        0      488 2023-06-05 17:36:35.116545 starvote-2.0.5/test_elections/test_election_all_zeroes_sss.txt
+-rw-r--r--   0        0        0      132 2023-06-01 14:19:46.079934 starvote-2.0.5/test_elections/test_election_all_zeroes_star.starvote
+-rw-r--r--   0        0        0     1027 2023-06-05 15:58:26.332409 starvote-2.0.5/test_elections/test_election_all_zeroes_star.txt
+-rw-r--r--   0        0        0      220 2023-06-05 17:40:04.326268 starvote-2.0.5/test_elections/test_election_all_zeroes_with_tiebreaker_sss.starvote
+-rw-r--r--   0        0        0     1921 2023-06-05 17:40:54.170678 starvote-2.0.5/test_elections/test_election_all_zeroes_with_tiebreaker_sss.txt
+-rw-r--r--   0        0        0     2660 2023-05-31 22:55:06.890838 starvote-2.0.5/test_elections/test_election_bloc_star_and_electowiki.starvote
+-rw-r--r--   0        0        0     3383 2023-06-05 15:58:26.332409 starvote-2.0.5/test_elections/test_election_bloc_star_and_electowiki.txt
+-rw-r--r--   0        0        0      989 2023-05-31 14:32:27.710655 starvote-2.0.5/test_elections/test_election_bloc_star_unbreakable_tie_for_first.starvote
+-rw-r--r--   0        0        0     1606 2023-06-05 15:58:26.332409 starvote-2.0.5/test_elections/test_election_bloc_star_unbreakable_tie_for_first.txt
+-rw-r--r--   0        0        0      201 2023-05-31 14:32:09.618494 starvote-2.0.5/test_elections/test_election_breakable_tie_for_second_in_score_round.starvote
+-rw-r--r--   0        0        0      831 2023-06-05 15:58:26.332409 starvote-2.0.5/test_elections/test_election_breakable_tie_for_second_in_score_round.txt
+-rw-r--r--   0        0        0      204 2023-05-31 14:31:42.454252 starvote-2.0.5/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_max_score_count_round.starvote
+-rw-r--r--   0        0        0      965 2023-06-05 15:58:26.332409 starvote-2.0.5/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_max_score_count_round.txt
+-rw-r--r--   0        0        0      203 2023-05-31 14:31:18.974043 starvote-2.0.5/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_score_round.starvote
+-rw-r--r--   0        0        0      744 2023-06-05 15:58:26.332409 starvote-2.0.5/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_score_round.txt
+-rw-r--r--   0        0        0      838 2023-05-31 14:31:04.393913 starvote-2.0.5/test_elections/test_election_demonstrate_cloneproofness_1.starvote
+-rw-r--r--   0        0        0      542 2023-06-05 15:58:26.332409 starvote-2.0.5/test_elections/test_election_demonstrate_cloneproofness_1.txt
+-rw-r--r--   0        0        0      830 2023-05-31 14:09:22.654324 starvote-2.0.5/test_elections/test_election_demonstrate_cloneproofness_2.starvote
+-rw-r--r--   0        0        0     1087 2023-06-05 15:58:26.332409 starvote-2.0.5/test_elections/test_election_demonstrate_cloneproofness_2.txt
+-rw-r--r--   0        0        0      194 2023-06-01 16:45:03.487305 starvote-2.0.5/test_elections/test_election_extra_candidates_in_permutation.starvote
+-rw-r--r--   0        0        0      142 2023-06-05 15:58:26.332409 starvote-2.0.5/test_elections/test_election_extra_candidates_in_permutation.txt
+-rw-r--r--   0        0        0      165 2023-06-01 16:45:09.147349 starvote-2.0.5/test_elections/test_election_incomplete_permutation.starvote
+-rw-r--r--   0        0        0      138 2023-06-05 15:58:26.332409 starvote-2.0.5/test_elections/test_election_incomplete_permutation.txt
+-rw-r--r--   0        0        0      132 2023-06-03 00:43:08.954337 starvote-2.0.5/test_elections/test_election_no_output.starvote
+-rw-r--r--   0        0        0       17 2023-06-05 15:58:26.332409 starvote-2.0.5/test_elections/test_election_no_output.txt
+-rw-r--r--   0        0        0      130 2023-06-01 16:34:20.926370 starvote-2.0.5/test_elections/test_election_no_permuted_candidates_tiebreaker.starvote
+-rw-r--r--   0        0        0     1336 2023-06-05 15:58:26.332409 starvote-2.0.5/test_elections/test_election_no_permuted_candidates_tiebreaker.txt
+-rw-r--r--   0        0        0      131 2023-06-01 17:57:44.689602 starvote-2.0.5/test_elections/test_election_only_one_candidate_star.starvote
+-rw-r--r--   0        0        0      505 2023-06-05 15:58:26.336409 starvote-2.0.5/test_elections/test_election_only_one_candidate_star.txt
+-rw-r--r--   0        0        0      182 2023-06-02 19:18:13.310778 starvote-2.0.5/test_elections/test_election_only_two_candidates_allocated.starvote
+-rw-r--r--   0        0        0      547 2023-06-05 16:34:32.017979 starvote-2.0.5/test_elections/test_election_only_two_candidates_allocated.txt
+-rw-r--r--   0        0        0      177 2023-06-01 17:57:23.633416 starvote-2.0.5/test_elections/test_election_only_two_candidates_bloc_star.starvote
+-rw-r--r--   0        0        0      487 2023-06-05 15:58:26.336409 starvote-2.0.5/test_elections/test_election_only_two_candidates_bloc_star.txt
+-rw-r--r--   0        0        0      176 2023-06-01 17:57:20.909392 starvote-2.0.5/test_elections/test_election_only_two_candidates_rrv.starvote
+-rw-r--r--   0        0        0      523 2023-06-05 15:58:26.336409 starvote-2.0.5/test_elections/test_election_only_two_candidates_rrv.txt
+-rw-r--r--   0        0        0      176 2023-06-05 16:03:13.610740 starvote-2.0.5/test_elections/test_election_only_two_candidates_sss.starvote
+-rw-r--r--   0        0        0      556 2023-06-05 17:36:16.484392 starvote-2.0.5/test_elections/test_election_only_two_candidates_sss.txt
+-rw-r--r--   0        0        0      319 2023-06-02 19:18:05.042705 starvote-2.0.5/test_elections/test_election_proportional_star_unbreakable_tie.starvote
+-rw-r--r--   0        0        0      480 2023-06-05 15:58:26.336409 starvote-2.0.5/test_elections/test_election_proportional_star_unbreakable_tie.txt
+-rw-r--r--   0        0        0     5899 2023-05-22 07:24:36.945502 starvote-2.0.5/test_elections/test_election_reweighted_range_sample_election.html
+-rw-r--r--   0        0        0      450 2023-06-03 00:37:52.439507 starvote-2.0.5/test_elections/test_election_reweighted_range_sample_election.starvote
+-rw-r--r--   0        0        0     1150 2023-06-05 15:58:26.336409 starvote-2.0.5/test_elections/test_election_reweighted_range_sample_election.txt
+-rw-r--r--   0        0        0      203 2023-05-31 14:05:02.452007 starvote-2.0.5/test_elections/test_election_unbreakable_three_way_tie_for_first_in_score_round.starvote
+-rw-r--r--   0        0        0     1023 2023-06-05 15:58:26.336409 starvote-2.0.5/test_elections/test_election_unbreakable_three_way_tie_for_first_in_score_round.txt
+-rw-r--r--   0        0        0      306 2023-06-01 18:06:23.106174 starvote-2.0.5/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round.starvote
+-rw-r--r--   0        0        0     1788 2023-06-05 15:58:26.336409 starvote-2.0.5/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round.txt
+-rw-r--r--   0        0        0      143 2023-06-02 19:18:03.054688 starvote-2.0.5/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round_allocated.starvote
+-rw-r--r--   0        0        0     2033 2023-06-05 17:25:28.231055 starvote-2.0.5/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round_allocated.txt
+-rw-r--r--   0        0        0      137 2023-06-05 16:03:10.882717 starvote-2.0.5/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round_sss.starvote
+-rw-r--r--   0        0        0     2343 2023-06-05 17:23:26.814055 starvote-2.0.5/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round_sss.txt
+-rw-r--r--   0        0        0      203 2023-05-31 14:04:09.035532 starvote-2.0.5/test_elections/test_election_unbreakable_tie_for_second_in_score_round.starvote
+-rw-r--r--   0        0        0      938 2023-06-05 15:58:26.340409 starvote-2.0.5/test_elections/test_election_unbreakable_tie_for_second_in_score_round.txt
+-rw-r--r--   0        0        0      155 2023-05-28 20:58:05.118365 starvote-2.0.5/test_elections/test_election_unbreakable_tie_in_automatic_runoff_round.starvote
+-rw-r--r--   0        0        0     1081 2023-06-05 15:58:26.340409 starvote-2.0.5/test_elections/test_election_unbreakable_tie_in_automatic_runoff_round.txt
+-rw-r--r--   0        0        0      150 2023-06-01 14:49:33.615373 starvote-2.0.5/test_elections/test_election_use_just_raise_tiebreaker.starvote
+-rw-r--r--   0        0        0     1103 2023-06-05 15:58:26.340409 starvote-2.0.5/test_elections/test_election_use_just_raise_tiebreaker.txt
+-rw-r--r--   0        0        0      154 2023-06-01 16:06:23.349484 starvote-2.0.5/test_elections/test_election_use_no_description_tiebreaker.starvote
+-rw-r--r--   0        0        0     1030 2023-06-05 15:58:26.340409 starvote-2.0.5/test_elections/test_election_use_no_description_tiebreaker.txt
+-rw-r--r--   0        0        0      152 2023-06-01 16:08:48.230596 starvote-2.0.5/test_elections/test_election_use_only_heading_tiebreaker.starvote
+-rw-r--r--   0        0        0      152 2023-06-05 15:58:26.340409 starvote-2.0.5/test_elections/test_election_use_only_heading_tiebreaker.txt
+-rw-r--r--   0        0        0      634 2023-06-03 00:09:38.012356 starvote-2.0.5/tests/harness.py
+-rw-r--r--   0        0        0    36446 2023-06-03 01:08:39.424022 starvote-2.0.5/tests/test_all.py
+-rwxr-xr-x   0        0        0     2379 2023-06-03 00:24:17.844223 starvote-2.0.5/tools/is_ok
+-rwxr-xr-x   0        0        0     2063 2023-06-03 00:15:52.499704 starvote-2.0.5/tools/remake_test_elections_output
+-rw-r--r--   0        0        0    43296 1970-01-01 00:00:00.000000 starvote-2.0.5/PKG-INFO
```

### Comparing `starvote-2.0.4/LICENSE` & `starvote-2.0.5/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 starvote
 Copyright 2023 by Larry Hastings
-All rights reserved.
 
 Permission is hereby granted, free of charge, to any person obtaining a
 copy of this software and associated documentation files (the "Software"),
 to deal in the Software without restriction, including without limitation
 the rights to use, copy, modify, merge, publish, distribute, sublicense,
 and/or sell copies of the Software, and to permit persons to whom the
 Software is furnished to do so, subject to the following conditions:
```

### Comparing `starvote-2.0.4/README.md` & `starvote-2.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 This module, **starvote**, implements a STAR Voting tabulator.
 It requires Python 3.7 or newer, but also supports CPython 3.6.
 (**starvote** relies on dictionaries preserving insertion order,
 which is guaranteed as of Python 3.7, but happened to work in CPython 3.6.)
 
 Features:
 
-* Supports four
+* Supports five
   [electoral systems](https://en.wikipedia.org/wiki/Electoral_system):
 
   - [STAR Voting](https://www.starvoting.org/star), the snazzy
     new single-winner voting system.
   - [Bloc STAR Voting](https://www.starvoting.org/multi_winner),
     a multiwinner variant of STAR voting that fills multiple
     seats with the *most popular* candidates.
@@ -220,15 +220,15 @@
 Since those are a lot to type, `starvote` also provides
 nicknames for these methods, respectively:
 
 * `starvote.star`,
 * `starvote.bloc`,
 * `starvote.allocated`,
 * `starvote.rrv`, and
-* `starvote.sss`, and
+* `starvote.sss`.
 
 `ballots` should be an iterable containing individual ballots.
 A ballot is a `dict` mapping the candidate to that ballot's
 score for that candidate.  The candidate can be any hashable
 Python value; the score must be an `int`.
 
 `maximum_score` specifies the maximum score allowed for
@@ -262,19 +262,19 @@
 * `reweighted_range_voting` implements Reweighted Range Voting.
 * `sequentially_spent_score` implements Sequentially Spent Score.
 
 These functions have much the same signature as `election`,
 with the following changes:
 
 * They don't have a `method` parameter; the method is implicit
-  in the function.  All four only take one positional parameter,
+  in the function.  All five only take one positional parameter,
   `ballots`, which is required.
-* `star` doesn't have a `seats` parameter.  The other three
-  have a `seats` keyword-only parameter, and this parameter
-  is required--it doesn't have a default.  (A *required*
+* `star` doesn't have a `seats` parameter.  The others do
+  accept a `seats` keyword-only parameter, and it's
+  *required*--it doesn't have a default.  (A *required*
   keyword-only parameter is pretty rare in Python!)
 * Note that, like `election`, these functions always
   return a list, even `star_voting`.
 
 #### Reference implementation of Allocated Score Voting
 
 `starvote` ships a copy of the reference implementation
@@ -497,15 +497,15 @@
 
 ballots = [
     {'Amy': 1, 'Brian': 3, 'Chuck': 5},
     {'Amy': 5, 'Brian': 2, 'Chuck': 3},
     {'Amy': 4, 'Brian': 4, 'Chuck': 5},
 ]
 
-winners = starvote.election(starvote.STAR, ballots, verbosity=1)
+winners = starvote.election(starvote.star, ballots, verbosity=1)
 ```
 
 (This example is included as `example.py` in the `starvote`
 Git repo.)
 
 After this example code finishes,
 the `winners` variable will contain the list `['Chuck']`.
@@ -665,14 +665,18 @@
 format* file is in (if the *starvote format election* was
 loaded from a file) or the current directory.  Both settings
 will load ballots from the file specified; `starvote_path`
 will also load the options from the file specified, however
 any options set in the current election will override those
 options.
 
+Note that `starvote_path` is fully recursive.  Starvote
+file A can import starvote file B, which in turn imports
+starvote file C, etc. etc.
+
 #### Example
 
 Here's a sample starvote format election:
 
     [options]
 
     seats=3
@@ -950,14 +954,20 @@
 [`https://star.vote/`](https://star.vote/).  The licensing of these
 sample ballots is unclear, but they're assumed to be public-domain
 or otherwise freely redistributable.
 
 
 ## Changelog
 
+**2.0.5** - *2023/07/05*
+
+* No code changes, just a tweak to the license to remove the
+  admittedly-confusing phrase "All rights reserved."  Also,
+  embedded the license in the module.
+
 **2.0.4** - *2023/06/05*
 
 * Added support for Sequentially Spent Score voting.
 * Changed presentation slightly for Allocated Score:
   the average vote is now computed using the count of
   *all* ballots in the election, including allocated
   ballots.  (Previously the average was computing using
```

### Comparing `starvote-2.0.4/docs/clarifying_star_voting.md` & `starvote-2.0.5/docs/clarifying_star_voting.md`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/docs/formatting_fractions_in_columns_of_text.txt` & `starvote-2.0.5/docs/formatting_fractions_in_columns_of_text.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/pyproject.toml` & `starvote-2.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/starvote/__init__.py` & `starvote-2.0.5/starvote/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,25 +5,28 @@
 ##
 ## * write a unit test that checks the code examples
 ##   in README.md are up to date
 ##     * confirms "example.py" and the output in README.md matches
 ##     * confirms the "multi-winner elections" cmdline works
 ##   (I keep breaking 'em.)
 ##
+## * have starvote format import detect a recursion loop and complain
+##   A imports B, B imports A, you blow your stack.
+##
 ## * output
 ##     * alternate output format idea:
 ##         * make something more computer-readable.
 ##         * maybe just super-regular HTML, with classes and names to make it easy?
 ##     * allow displaying in floats
 ##     * restore printing the preference matrix (it's lurking in 1.x versions)
 ##
 
 __doc__ = "An election tabulator for the STAR electoral system, and others"
 
-__version__ = "2.0.4"
+__version__ = "2.0.5"
 
 __all__ = [
     'Allocated_Score_Voting', # Method
     'allocated', # Method (nickname)
     'allocated_score_voting', # function
     'Bloc_STAR_Voting', # Method
     'bloc', # Method (nickname)
@@ -48,14 +51,37 @@
     'Tiebreaker', # class
     'tiebreakers', # maps string to tiebreakers
     'UnbreakableTieError', # exception class
     'UsageException', # exception class
     ]
 
 
+LICENSE = """
+starvote
+Copyright 2023 by Larry Hastings
+
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the "Software"),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included
+in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
+IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
+DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
+TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE
+OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+""".strip()
+
 import builtins
 from collections import defaultdict
 from contextlib import contextmanager
 import csv
 from fractions import Fraction
 import enum
 import itertools
```

### Comparing `starvote-2.0.4/starvote/reference.py` & `starvote-2.0.5/starvote/reference.py`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/README.md` & `starvote-2.0.5/test_elections/README.md`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/bad_syntax_ballot_pragma_as_last_line.txt` & `starvote-2.0.5/test_elections/bad_syntax_ballot_pragma_as_last_line.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/bad_syntax_change_section_in_list.txt` & `starvote-2.0.5/test_elections/bad_syntax_change_section_in_list.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/bad_syntax_fussy_wrong_ballots_1.txt` & `starvote-2.0.5/test_elections/bad_syntax_fussy_wrong_ballots_1.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/bad_syntax_fussy_wrong_ballots_2.txt` & `starvote-2.0.5/test_elections/bad_syntax_fussy_wrong_ballots_2.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/bad_syntax_invalid_method.txt` & `starvote-2.0.5/test_elections/bad_syntax_invalid_method.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/bad_syntax_invalid_option.txt` & `starvote-2.0.5/test_elections/bad_syntax_invalid_option.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/bad_syntax_invalid_pragma.txt` & `starvote-2.0.5/test_elections/bad_syntax_invalid_pragma.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/bad_syntax_invalid_start_of_line_mode.txt` & `starvote-2.0.5/test_elections/bad_syntax_invalid_start_of_line_mode.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/bad_syntax_invalid_starvote_path_1.txt` & `starvote-2.0.5/test_elections/bad_syntax_invalid_starvote_path_1.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/bad_syntax_invalid_starvote_path_2.txt` & `starvote-2.0.5/test_elections/bad_syntax_invalid_starvote_path_2.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/bad_syntax_invalid_tiebreaker.txt` & `starvote-2.0.5/test_elections/bad_syntax_invalid_tiebreaker.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/bad_syntax_malformed_section.txt` & `starvote-2.0.5/test_elections/bad_syntax_malformed_section.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/bad_syntax_no_ballots.txt` & `starvote-2.0.5/test_elections/bad_syntax_no_ballots.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/bad_syntax_no_equals.txt` & `starvote-2.0.5/test_elections/bad_syntax_no_equals.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/bad_syntax_no_method.txt` & `starvote-2.0.5/test_elections/bad_syntax_no_method.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/bad_syntax_no_section.txt` & `starvote-2.0.5/test_elections/bad_syntax_no_section.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/bad_syntax_pragma_in_options.txt` & `starvote-2.0.5/test_elections/bad_syntax_pragma_in_options.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/bad_syntax_pragma_inside_list.txt` & `starvote-2.0.5/test_elections/bad_syntax_pragma_inside_list.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/bad_syntax_repeated_option.txt` & `starvote-2.0.5/test_elections/bad_syntax_repeated_option.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/bad_syntax_repeated_section.txt` & `starvote-2.0.5/test_elections/bad_syntax_repeated_section.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.csv` & `starvote-2.0.5/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.pdf` & `starvote-2.0.5/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.txt` & `starvote-2.0.5/test_elections/starvote_ballots_2020_libertarian_party_presidential_nomination.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.csv` & `starvote-2.0.5/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.pdf` & `starvote-2.0.5/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.txt` & `starvote-2.0.5/test_elections/starvote_ballots_2020_presidential_election_all_contenders_all_parties.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/starvote_ballots_best_akali_skins.csv` & `starvote-2.0.5/test_elections/starvote_ballots_best_akali_skins.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/starvote_ballots_best_akali_skins.pdf` & `starvote-2.0.5/test_elections/starvote_ballots_best_akali_skins.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/starvote_ballots_best_akali_skins.txt` & `starvote-2.0.5/test_elections/starvote_ballots_best_akali_skins.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/starvote_ballots_eurovision_song_contest_2023.csv` & `starvote-2.0.5/test_elections/starvote_ballots_eurovision_song_contest_2023.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/starvote_ballots_eurovision_song_contest_2023.pdf` & `starvote-2.0.5/test_elections/starvote_ballots_eurovision_song_contest_2023.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/starvote_ballots_eurovision_song_contest_2023.txt` & `starvote-2.0.5/test_elections/starvote_ballots_eurovision_song_contest_2023.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.csv` & `starvote-2.0.5/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.pdf` & `starvote-2.0.5/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.txt` & `starvote-2.0.5/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_allocated.txt` & `starvote-2.0.5/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_allocated.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_bloc_star.txt` & `starvote-2.0.5/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_bloc_star.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_sss.txt` & `starvote-2.0.5/test_elections/starvote_ballots_libertarian_party_2020_presidential_nomination_may_sss.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/starvote_ballots_presidential_candidates.csv` & `starvote-2.0.5/test_elections/starvote_ballots_presidential_candidates.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/starvote_ballots_presidential_candidates.pdf` & `starvote-2.0.5/test_elections/starvote_ballots_presidential_candidates.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/starvote_ballots_presidential_candidates.txt` & `starvote-2.0.5/test_elections/starvote_ballots_presidential_candidates.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/starvote_ballots_presidential_poll_july_2020.csv` & `starvote-2.0.5/test_elections/starvote_ballots_presidential_poll_july_2020.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/starvote_ballots_presidential_poll_july_2020.pdf` & `starvote-2.0.5/test_elections/starvote_ballots_presidential_poll_july_2020.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/starvote_ballots_presidential_poll_july_2020.txt` & `starvote-2.0.5/test_elections/starvote_ballots_presidential_poll_july_2020.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.csv` & `starvote-2.0.5/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.pdf` & `starvote-2.0.5/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.txt` & `starvote-2.0.5/test_elections/starvote_ballots_updated_2020_libertarian_presidential_candidate.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.csv` & `starvote-2.0.5/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.csv`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.pdf` & `starvote-2.0.5/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.pdf`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.txt` & `starvote-2.0.5/test_elections/starvote_ballots_wa_governor_2020_republican_party_straw_poll.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/test_election_all_fives_bloc_star.txt` & `starvote-2.0.5/test_elections/test_election_all_fives_bloc_star.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/test_election_all_fives_star.txt` & `starvote-2.0.5/test_elections/test_election_all_fives_star.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/test_election_all_threes_bloc_star.txt` & `starvote-2.0.5/test_elections/test_election_all_threes_bloc_star.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/test_election_all_threes_star.txt` & `starvote-2.0.5/test_elections/test_election_all_threes_star.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/test_election_all_zeroes_bloc_star.txt` & `starvote-2.0.5/test_elections/test_election_all_zeroes_bloc_star.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/test_election_all_zeroes_star.txt` & `starvote-2.0.5/test_elections/test_election_all_zeroes_star.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/test_election_all_zeroes_with_tiebreaker_sss.txt` & `starvote-2.0.5/test_elections/test_election_all_zeroes_with_tiebreaker_sss.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/test_election_bloc_star_and_electowiki.starvote` & `starvote-2.0.5/test_elections/test_election_bloc_star_and_electowiki.starvote`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/test_election_bloc_star_and_electowiki.txt` & `starvote-2.0.5/test_elections/test_election_bloc_star_and_electowiki.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/test_election_bloc_star_unbreakable_tie_for_first.starvote` & `starvote-2.0.5/test_elections/test_election_bloc_star_unbreakable_tie_for_first.starvote`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/test_election_bloc_star_unbreakable_tie_for_first.txt` & `starvote-2.0.5/test_elections/test_election_bloc_star_unbreakable_tie_for_first.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/test_election_breakable_tie_for_second_in_score_round.txt` & `starvote-2.0.5/test_elections/test_election_breakable_tie_for_second_in_score_round.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_max_score_count_round.txt` & `starvote-2.0.5/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_max_score_count_round.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_score_round.txt` & `starvote-2.0.5/test_elections/test_election_breakable_tie_in_automatic_runoff_round_using_score_round.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/test_election_demonstrate_cloneproofness_1.starvote` & `starvote-2.0.5/test_elections/test_election_demonstrate_cloneproofness_1.starvote`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/test_election_demonstrate_cloneproofness_1.txt` & `starvote-2.0.5/test_elections/test_election_demonstrate_cloneproofness_1.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/test_election_demonstrate_cloneproofness_2.starvote` & `starvote-2.0.5/test_elections/test_election_demonstrate_cloneproofness_2.starvote`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/test_election_demonstrate_cloneproofness_2.txt` & `starvote-2.0.5/test_elections/test_election_demonstrate_cloneproofness_2.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/test_election_no_permuted_candidates_tiebreaker.txt` & `starvote-2.0.5/test_elections/test_election_no_permuted_candidates_tiebreaker.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/test_election_only_two_candidates_allocated.txt` & `starvote-2.0.5/test_elections/test_election_only_two_candidates_allocated.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/test_election_only_two_candidates_rrv.txt` & `starvote-2.0.5/test_elections/test_election_only_two_candidates_rrv.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/test_election_only_two_candidates_sss.txt` & `starvote-2.0.5/test_elections/test_election_only_two_candidates_sss.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/test_election_reweighted_range_sample_election.html` & `starvote-2.0.5/test_elections/test_election_reweighted_range_sample_election.html`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/test_election_reweighted_range_sample_election.txt` & `starvote-2.0.5/test_elections/test_election_reweighted_range_sample_election.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/test_election_unbreakable_three_way_tie_for_first_in_score_round.txt` & `starvote-2.0.5/test_elections/test_election_unbreakable_three_way_tie_for_first_in_score_round.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round.txt` & `starvote-2.0.5/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round_allocated.txt` & `starvote-2.0.5/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round_allocated.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round_sss.txt` & `starvote-2.0.5/test_elections/test_election_unbreakable_three_way_tie_for_second_in_score_round_sss.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/test_election_unbreakable_tie_for_second_in_score_round.txt` & `starvote-2.0.5/test_elections/test_election_unbreakable_tie_for_second_in_score_round.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/test_election_unbreakable_tie_in_automatic_runoff_round.txt` & `starvote-2.0.5/test_elections/test_election_unbreakable_tie_in_automatic_runoff_round.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/test_election_use_just_raise_tiebreaker.txt` & `starvote-2.0.5/test_elections/test_election_use_just_raise_tiebreaker.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/test_elections/test_election_use_no_description_tiebreaker.txt` & `starvote-2.0.5/test_elections/test_election_use_no_description_tiebreaker.txt`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/tests/harness.py` & `starvote-2.0.5/tests/harness.py`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/tests/run_tests.py` & `starvote-2.0.5/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/tools/is_ok` & `starvote-2.0.5/tools/is_ok`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/tools/remake_test_elections_output` & `starvote-2.0.5/tools/remake_test_elections_output`

 * *Files identical despite different names*

### Comparing `starvote-2.0.4/PKG-INFO` & `starvote-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starvote
-Version: 2.0.4
+Version: 2.0.5
 Summary: An election tabulator for the STAR electoral system, and others
 Author-email: Larry Hastings <larry@hastings.org>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -30,15 +30,15 @@
 This module, **starvote**, implements a STAR Voting tabulator.
 It requires Python 3.7 or newer, but also supports CPython 3.6.
 (**starvote** relies on dictionaries preserving insertion order,
 which is guaranteed as of Python 3.7, but happened to work in CPython 3.6.)
 
 Features:
 
-* Supports four
+* Supports five
   [electoral systems](https://en.wikipedia.org/wiki/Electoral_system):
 
   - [STAR Voting](https://www.starvoting.org/star), the snazzy
     new single-winner voting system.
   - [Bloc STAR Voting](https://www.starvoting.org/multi_winner),
     a multiwinner variant of STAR voting that fills multiple
     seats with the *most popular* candidates.
@@ -235,15 +235,15 @@
 Since those are a lot to type, `starvote` also provides
 nicknames for these methods, respectively:
 
 * `starvote.star`,
 * `starvote.bloc`,
 * `starvote.allocated`,
 * `starvote.rrv`, and
-* `starvote.sss`, and
+* `starvote.sss`.
 
 `ballots` should be an iterable containing individual ballots.
 A ballot is a `dict` mapping the candidate to that ballot's
 score for that candidate.  The candidate can be any hashable
 Python value; the score must be an `int`.
 
 `maximum_score` specifies the maximum score allowed for
@@ -277,19 +277,19 @@
 * `reweighted_range_voting` implements Reweighted Range Voting.
 * `sequentially_spent_score` implements Sequentially Spent Score.
 
 These functions have much the same signature as `election`,
 with the following changes:
 
 * They don't have a `method` parameter; the method is implicit
-  in the function.  All four only take one positional parameter,
+  in the function.  All five only take one positional parameter,
   `ballots`, which is required.
-* `star` doesn't have a `seats` parameter.  The other three
-  have a `seats` keyword-only parameter, and this parameter
-  is required--it doesn't have a default.  (A *required*
+* `star` doesn't have a `seats` parameter.  The others do
+  accept a `seats` keyword-only parameter, and it's
+  *required*--it doesn't have a default.  (A *required*
   keyword-only parameter is pretty rare in Python!)
 * Note that, like `election`, these functions always
   return a list, even `star_voting`.
 
 #### Reference implementation of Allocated Score Voting
 
 `starvote` ships a copy of the reference implementation
@@ -512,15 +512,15 @@
 
 ballots = [
     {'Amy': 1, 'Brian': 3, 'Chuck': 5},
     {'Amy': 5, 'Brian': 2, 'Chuck': 3},
     {'Amy': 4, 'Brian': 4, 'Chuck': 5},
 ]
 
-winners = starvote.election(starvote.STAR, ballots, verbosity=1)
+winners = starvote.election(starvote.star, ballots, verbosity=1)
 ```
 
 (This example is included as `example.py` in the `starvote`
 Git repo.)
 
 After this example code finishes,
 the `winners` variable will contain the list `['Chuck']`.
@@ -680,14 +680,18 @@
 format* file is in (if the *starvote format election* was
 loaded from a file) or the current directory.  Both settings
 will load ballots from the file specified; `starvote_path`
 will also load the options from the file specified, however
 any options set in the current election will override those
 options.
 
+Note that `starvote_path` is fully recursive.  Starvote
+file A can import starvote file B, which in turn imports
+starvote file C, etc. etc.
+
 #### Example
 
 Here's a sample starvote format election:
 
     [options]
 
     seats=3
@@ -965,14 +969,20 @@
 [`https://star.vote/`](https://star.vote/).  The licensing of these
 sample ballots is unclear, but they're assumed to be public-domain
 or otherwise freely redistributable.
 
 
 ## Changelog
 
+**2.0.5** - *2023/07/05*
+
+* No code changes, just a tweak to the license to remove the
+  admittedly-confusing phrase "All rights reserved."  Also,
+  embedded the license in the module.
+
 **2.0.4** - *2023/06/05*
 
 * Added support for Sequentially Spent Score voting.
 * Changed presentation slightly for Allocated Score:
   the average vote is now computed using the count of
   *all* ballots in the election, including allocated
   ballots.  (Previously the average was computing using
```

